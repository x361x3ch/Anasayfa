final SpannableTheme theme = SpannableTheme.builderWithDefaults(context)
        .headingBreakHeight(0) // <- this will remove underline 
        .build();

final SpannableConfiguration configuration = SpannableConfiguration.builder(context)
        .theme(theme)
        .build();

Markwon.setMarkdown(textView, configuration, "# No underline\n\n## No underline");
