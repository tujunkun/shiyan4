``
<?xml version="1.0" encoding="utf-8"?>
<PreferenceScreen xmlns:android="http://schemas.android.com/apk/res/android">
    <CheckBoxPreference
        android:key="checkboxpreference"
        android:title="checkbox"
        android:summary="This is a checkbox"
        android:defaultValue="false"
        />
    <PreferenceCategory android:title="edit">
        <EditTextPreference
            android:key="editpreference"
            android:title="edit preference"
            android:summary="this is a edittext"/>
    </PreferenceCategory>
    <ListPreference
        android:key="list"
        android:title="List"
        android:summary="An example that use a list dialog"
        android:entries="@array/list_option"
        android:entryValues="@array/list_options_values"
        />
    <CheckBoxPreference
        android:key="parent checkboxpreference"
        android:title="parent checkbox"
        android:summary="This is a parent checkbox"
        android:defaultValue="false"/>
    <CheckBoxPreference
        android:key="child checkboxpreference"
        android:title="child checkbox"
        android:summary="This is a child checkbox"
        android:defaultValue="false"
        android:dependency="parent checkboxpreference"
        />
    <PreferenceScreen
        android:title="preferenceScreen">
        <EditTextPreference
            android:key="edit"
            android:title="edit"
            android:summary="edit"/>
    </PreferenceScreen>
    <Preference
        android:title="intent preference">
        <intent
            android:action="android.intent.action.VIEW"
            android:data="http://www.baidu.com"/>
    </Preference>
</PreferenceScreen>
``
