---
layout: post
title: GUI i Android - XML-layouter
---

- TOC
{:toc}

## GUI i Android
Det enklaste sättet att designa en androidapp är genom XML-layouter. Vad och varför XML? Tre snabba:
* XML står för eXtensible Markup Language.
* XML är designat för att lagra och transportera data.
* XML är designat för att vara läsbart för både människor och maskiner.

Dessa egenskaperna gör XML väl passat till att skapa layouter med. Det är enkelt att överblicka och man separerar appens funktion från dess utseende och kan därför lätt ändra utseendet utan att röra källkoden vilket är väldigt smidigt (t.ex. för olika skärmorienteringar eller skärmstorlekar). Alla XML-layouter måste sparas i `/res/layouts`.

Ett alternativt sätt att skapa appens utseende genom `View` eller `Viewgroup` objekt i källkoden. Denna lite mödosammare metoden behövs ibland för mer avancerade funkktioner.  

## Exempelkod på en RelativeLayout

Exempel på XML-kod för en Relative Layout med en `Button` och en `TextView`:

```html
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent" android:layout_height="match_parent">

    <Button
        android:id="@+id/my_button"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignParentTop="true"
        android:layout_centerHorizontal="true"
        android:layout_marginTop="171dp"
        android:text="Button" />

    <TextView
        android:id="@+id/textView2"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignBottom="@+id/button3"
        android:layout_centerHorizontal="true"
        android:layout_marginBottom="93dp"
        android:text="Här har jag lite text." />
</RelativeLayout>
```

`<?xml version="1.0" encoding="utf-8"?>` - Första raden specifierar vilken XML-version som används samt vilken kodning, denna behövs aldrig ändras på i Androidsammanhang.

`RelativeLayout` - Därefter följer rotelementet som i detta fallet är `RelativeLayout`. I rotelementet sticker några attributer ut med följande syntax:

## Namespace

I XLM tillåts alla att definera sina egna element samt attributer, detta kan skapa konflikter när man för samman flera XML-filer. För att undvika detta kan man göra attributnamn mer unika genom att ge dem ett prefix som kallas namespace.

```html
xmlns:android="http://schemas.android.com/apk/res/android"
```

Detta är en deklarering av ett namespace och har syntaxen `xlmns:prefix="URI"`. Vanliga prefix är `android:`, `app:` samt `tools:`. ([w3school](https://www.w3schools.com/xml/xml_namespaces.asp))

## ID

Varje `View` objekt har ett unik ID. Syntaxet för detta är:

```
android:id="@+id/my_button"
```

'@'-symbolen talar om för XML-parsern att resten av textsträngen är ett ID. '+'-symbolen talar om att det är en ny resurs som måste skapas och läggas till (i ´R.java´-filen) <https://developer.android.com/guide/topics/ui/declaring-layout.html> bra upplägg
