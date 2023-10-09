<script setup>
import { ref } from 'vue';

const inputText = ref('hello')
const brand = ref('')

</script>
<template >
  <!-- <div class="bg-primary p-2 text-dark bg-opacity-20" > -->
    <div class="mx-auto p-2" style="width: 400px; ">
    <h3 class= "text-white">Select Brand of Laptop</h3>
 
  <div class="border border-black">
    <div  class="p-3 mb-2 bg-dark text-white">
    <select v-model="brand" class="form-select form-select-lg mb-3" aria-label="Large select example">
      
        <option value="acer">Acer</option>
        <option value="lenovo">Lenovo</option>
        <option value="hp">hp</option>
        <option value="sony">Sony</option>
        <option value="asus">Asus</option>
        <option value="toshiba">Toshiba</option>
        <option value="msi">MSI</option>
        <option value="huawei">Huawei</option>
        <option value="realme">Realme</option>
        <option value="samsung">Samsung</option>
        <option value="itel">Itel</option>
    </select>
    <p v-if="brand == 'acer'">
    <h5>
      <ul>
        <li>Model: Acer Swift 3</li>
        <li>Model: Acer Swift 3</li>
        <li>ROM: 512GB NVMe SSD</li>
        <li>Battery: All-day battery life</li>
        <li>Camera: HD webcam</li>
        <li>Display: 13.5-inch IPS display</li>
        <li>Storage: Fast and spacious SSD storage</li>
      
      </ul>
    </h5>
    </p>
    <p v-if="brand == 'lenovo'">
      <h5>
      <ul>
        <li>Model: Lenovo ThinkPad X1 Carbon</li>
        <li>RAM: 16GB LPDDR4X</li>
        <li>ROM: 1TB NVMe SSD</li>
        <li>Battery: Extended battery life</li>
        <li>Camera: HD webcam</li>
        <li>Display: 14-inch 4K IPS display</li>
        <li>Storage: Spacious SSD storage for professionals</li>
        
      </ul>
    </h5>
    </p>
    <p v-if="brand == 'hp'">
      <h5>
      <ul>
        <li>Model: HP Spectre x360</li>
        <li>RAM: 16GB LPDDR4X</li>
        <li>ROM: 512GB NVMe SSD</li>
        <li>Battery: All-day battery life with fast charging</li>
        <li>Camera: HD webcam</li>
        <li>Display: 13.3-inch 4K OLED touchscreen</li>
        <li>Storage: High-speed SSD storage for versatility</li>
         
      </ul>
    </h5>
    </p>
    <p v-if="brand == 'sony'">
      <h5>
      <ul>
        <li>Model: Sony VAIO S</li>
        <li>RAM: 16GB DDR4</li>
        <li>ROM: 512GB PCIe SSD</li>
        <li>Battery: Efficient and long-lasting</li>
        <li>Camera: Integrated webcam</li>
        <li>Display: 15.6-inch Full HD display</li>
        <li>Storage: Fast PCIe SSD storage for productivity</li>
      </ul>
    </h5>
    </p>
    <p v-if="brand == 'asus'">
      <h5>
      <ul>
        <li>Model: Asus ROG Zephyrus G14</li>
        <li>RAM: 16GB DDR4</li>
        <li>ROM: 1TB NVMe SSD</li>
        <li>Battery: Long-lasting with fast charging</li>
        <li>Camera: Integrated HD webcam</li>
        <li>Display: 14-inch QHD display</li>
        <li>Storage: High-capacity SSD for gaming and multimedia</li>
        
      </ul>
    </h5>
    </p>
    <p v-if="brand == 'toshiba'">
      <h5>
      <ul>
        <li>Model: Toshiba Satellite C</li>
        <li>RAM: 4GB DDR4</li>
        <li>ROM: 128GB eMMC</li>
        <li>Battery: Standard battery life</li>
        <li>Camera: Basic integrated webcam</li>
        <li>Display: 15.6-inch HD LED display</li>
        <li>Storage: Adequate eMMC storage</li>
        
      </ul>
    </h5>
    </p> 
    <p v-if="brand =='msi'">
      <h5>
      <ul>
        <li>Model: MSI GS66 Stealth</li>
        <li>RAM: 32GB DDR4</li>
        <li>ROM: 1TB NVMe SSD</li>
        <li>Battery: Extended battery life for gaming</li>
        <li>Camera: Integrated HD webcam</li>
        <li>Display: 15.6-inch Full HD 300Hz display</li>
        <li>Storage: High-capacity SSD for gaming and content creation.</li>
        
      </ul>
    </h5>
    </p>
    <p v-if="brand == 'huawei'">
      <h5>
      <ul>
        <li>Model: Huawei MateBook X Pro</li>
        <li>RAM: 16GB LPDDR3</li>
        <li>ROM: 512GB NVMe SSD</li>
        <li>Battery: All-day battery life with fast charging</li>
        <li>Camera: Pop-up webcam</li>
        <li>Display: 13.9-inch 3K touchscreen</li>
        <li>Storage: High-speed SSD storage for productivity</li>
        
      </ul>
    </h5>
    </p>
    <p v-if="brand == 'realme'">
      <h5>
      <ul>
        <li>Model: Realme Book</li>
        <li>RAM: 8GB LPDDR4X</li>
        <li>ROM: 256GB NVMe SSD</li>
        <li>Battery: Long-lasting with fast charging</li>
        <li>Camera: HD webcam</li>
        <li>Display: 14-inch Full HD display</li>
        <li>Storage: Fast SSD storage for everyday use</li>
        
      </ul>
    </h5>
    </p>
    <p v-if="brand == 'samsung'">
      <h5>
      <ul>
        <li>Model: Samsung Galaxy Book Flex</li>
        <li>RAM: 12GB LPDDR4X</li>
        <li>ROM: 512GB NVMe SSD</li>
        <li>Battery: Long-lasting with fast charging</li>
        <li>Camera: Integrated HD webcam</li>
        <li>Display: 13.3-inch QLED touchscreen</li>
        <li>Storage: High-speed SSD storage for versatility</li>
        
      </ul>
    </h5>
    </p>
    <p v-if="brand == 'itel'">
      <h5>
      <ul>
        <li>Model: Itel VisionBook Pro X</li>
        <li>RAM: 8GB DDR4</li>
        <li>ROM: 256GB NVMe SSD</li>
        <li>Battery: Dependable battery performance</li>
        <li>Camera: HD webcam</li>
        <li>Display: 14-inch Full HD display</li>
        <li>Storage: SSD storage for everyday tasks.
</li>
        
      </ul>
    </h5>
    </p>
    
    <!-- <p v-else>3</p> -->
  
  </div>
  </div>
 </div> 
<!-- </div> -->

</template>