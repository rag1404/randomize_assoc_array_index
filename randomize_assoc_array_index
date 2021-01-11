// This will randomize only if the array is pre-populated
// you can only randomize the index

module test_rand_assoc_array;
  
  typedef bit[7:0] index; 
  bit[7:0] assoc_arr[index];
index idx, idx_list[$];


  
  initial begin
    assoc_arr = '{1:40,5:23,5:48,8:32};
     
    repeat (3) begin
     
     idx_list = assoc_arr.find_index() with ('1);
      std::randomize(idx) with {idx inside {idx_list};};
    
      $display ("%d",assoc_arr[idx]);
      
    end
  end
  
endmodule
