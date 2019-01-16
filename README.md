# FloatingSearchView
An implementation of a floating view search box and suggestions. 
 

###### Implemention : 

         implemention 'com.github.arimorty:floatingsearchview:2.1.1'
         

###### Layout :

     <com.arlib.floatingsearchview.FloatingSearchView
                  android:id="@+id/floating_search_view"
                  android:layout_width="match_parent"
                  android:layout_height="match_parent"
                  app:floatingSearch_searchBarMarginLeft="@dimen/search_view_inset"
                  app:floatingSearch_searchBarMarginTop="@dimen/search_view_inset"
                  app:floatingSearch_searchBarMarginRight="@dimen/search_view_inset"
                  app:floatingSearch_searchHint="Search..."
                  app:floatingSearch_suggestionsListAnimDuration="250"
                  app:floatingSearch_showSearchKey="false"
                  app:floatingSearch_leftActionMode="showHamburger"
                  app:floatingSearch_menu="@menu/menu_main"
                  app:floatingSearch_close_search_on_keyboard_dismiss="true"/>


###### Activity :


                mSearchView.setOnQueryChangeListener(new FloatingSearchView.OnQueryChangeListener() {
              @Override
              public void onSearchTextChanged(String oldQuery, final String newQuery) {

                  //get suggestions based on newQuery

                  //pass them on to the search view
                  mSearchView.swapSuggestions(newSuggestions);
              }
          });
          
          
###### Styling : 

            <style name="SearchView">
                    <item name="floatingSearch_backgroundColor"></item>
                    <item name="floatingSearch_viewSearchInputTextColor"></item>
                    <item name="floatingSearch_viewSuggestionItemTextColor"></item>
                    <item name="floatingSearch_hintTextColor"></item>
                    <item name="floatingSearch_dividerColor"></item>
                    <item name="floatingSearch_clearBtnColor"></item>
                    <item name="floatingSearch_leftActionColor"></item>
                    <item name="floatingSearch_menuItemIconColor"></item>
                    <item name="floatingSearch_suggestionRightIconColor"></item>
                    <item name="floatingSearch_actionMenuOverflowColor"></item>
            </style>
            
            
            
            
    
    
 
 
 
###### Screenshots : 



![Image of FloatingSearchView](https://github.com/ahmedkmadani/FloatingSearchView/blob/master/Screenshots/Screenshot_2019-01-16-00-59-17.png)



![Image of FloatingSearchView](https://github.com/ahmedkmadani/FloatingSearchView/blob/master/Screenshots/Screenshot_2019-01-16-00-59-33.png)




