Collections können im routes.rb für nesting genutzt werden. Es verhindert, dass die ID der Resource für die Route benötigt wird.


```
resources :skills do 
      get 'new_to_person'
end

---> URL: /skills/:id/new_to_person
```


```
resources :skills do 
     collection do
        get 'new_to_person'
      end
end

---> URL: /skills/new_to_person
```

