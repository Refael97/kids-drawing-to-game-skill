# kids-drawing-to-game 🎨→🎮

סקיל ל־Claude שהופך צילום של ציור ילדים למשחק אמיתי בדפדפן.
הדמויות והרקע במשחק **גזורים מהציור עצמו**, כך שהילד רואה את מה שהוא צייר זז על המסך.

A Claude skill that turns a photo of a child's drawing into a playable browser game, built from the drawing's own cut-out elements.

## מה יוצא

- קובץ HTML אחד, עובד בלי אינטרנט
- מתאים לגילאי 3–8: בלי פסילות, סבב של דקה, "כל הכבוד!" עם קונפטי בסוף
- טקסטים בעברית, צלילים שמחים
- עובד במחשב (חיצים + רווח), בטלפון ובטאבלט (כפתורים גדולים), ובטלוויזיה (שלט)

Claude מזהה מה יש בציור ובוחר משחק שמתאים לו: עץ עם פירות → אוספים פירות, נהר עם דג → קופצים לתפוס את הדג, ציפור בשמיים → עפים בין עננים.

## מה צריך

- **Claude Code**, או claude.ai עם הרצת קוד
- **Python 3** עם Pillow ו־numpy (לגזירת האלמנטים מהתמונה)
- אופציונלי: Playwright לבדיקה, ffmpeg להקלטת סרטון של המשחק

## התקנה

### Claude Code, כפלאגין
```
/plugin marketplace add Refael97/kids-drawing-to-game-skill
/plugin install kids-drawing-to-game@kids-drawing-to-game
```

### Claude Code, ידנית
מעתיקים את התיקייה `skills/kids-drawing-to-game` אל `~/.claude/skills/`.

### claude.ai
אורזים את התיקייה `skills/kids-drawing-to-game` כקובץ zip ומעלים בהגדרות, באזור ה־Skills.

## שימוש

מצלמים את הציור, שולחים ל־Claude וכותבים:
```
/kids-drawing-to-game תהפוך את הציור הזה למשחק
```

## עוד

נבנה על ידי רפאל לוי · [refael-ai.com](https://refael-ai.com/pages/kids-drawing-to-game) · [@refaelleviii](https://instagram.com/refaelleviii)

רישיון MIT.
