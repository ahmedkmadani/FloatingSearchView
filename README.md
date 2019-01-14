# FloatingSearchView
An implementation of a floating view search box and suggestions. 

Usage: 

1- In your dependencies add : 

         implemention 'com.github.arimorty:floatingsearchview:2.1.1'
         
2- add Floating Search View in your view heircuy and adjuts weight and width 

Example : 

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


                mSearchView.setOnQueryChangeListener(new FloatingSearchView.OnQueryChangeListener() {
              @Override
              public void onSearchTextChanged(String oldQuery, final String newQuery) {

                  //get suggestions based on newQuery

                  //pass them on to the search view
                  mSearchView.swapSuggestions(newSuggestions);
              }
          });
