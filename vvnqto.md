代发 wailian999

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2xxaeoxjf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2hyvwhmui.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2eqttiyuu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2xmjsgqzq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2djjrjijp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2wiqkcdnl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2zxzemryf.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2tkyxychy.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2nelkzfrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2giwoogws.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2xmldysai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bwhbnkpi.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2qvmlfyua.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2rdwrhsmu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wynroyjv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bpbctenh.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fenutjcl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cmnkqnvg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2pvspblan.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2lkbzbege.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xjakcqzu.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2rbimqaah.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2lnmypwmb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rusjhswu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2svthlbyd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xhqnwbfe.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mipwjdrm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2leuzipqk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2oqjacupf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nfzpnqzt.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2fvidpwgv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ficmyubb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vutcphpe.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbkgipey.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yytcjkjl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sioihlyc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2boeyfglt.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2peqjvked.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2ugoqhwsy.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qgyqvkle.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2fsusiegm.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2omvwaxly.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2pbbbgsid.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zevfwkan.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wghgypea.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2xvinlsol.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2admjhlhc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2epvokunw.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vygqntme.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2hpflancv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2vqqdptjv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wbhchivx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxawmjmn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lbhedxyb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2bcdqetlc.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2xcswldpd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hjownstu.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2uyilrhjp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ihpmpfxf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vecdehkk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2keajapej.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vuegujpm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2unwsgtcn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2nmvughrp.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2huzreoes.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2dmyhaxka.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2rghsklyz.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2bqpggzmx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwgqwkfh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kggfwxvp.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2domesfjt.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kufmulos.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2csuemotv.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2stbfgrju.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pyvozjtl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2kmtfbvba.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2augavsyo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ybtopyje.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ecpsordu.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xlllafzz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cviptaij.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2hxifhpag.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2jymjjloa.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vhlhxrvd.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2zcawptfq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2vvmuylck.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrxlnyek.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkenvlrs.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkzmxlgh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lyhlyabv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2dxnopazg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2oqbyrmdy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bjywfalo.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2wtmrcjjq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2leynkoyl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kimtsqju.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ibclctlr.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2odvpykcs.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2sknbxazi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2bdeqpuhq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2gbamooww.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2bacnaxeg.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2iwhgxqbf.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2hmfyxapm.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bemsqwwo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xjkqofqn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zcnzayfb.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lmrtlttr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2oyqchnlh.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2trnctyer.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hldkwqdq.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2vgavcduv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2zcaisqts.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2gxalvhtg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2sosqwaii.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2eeviwdrf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kuurlbzs.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2yjjpmgfv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2tqxvaonl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2xiooffhh.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2jlvqnyno.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2oaienrha.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2hqaubgfj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2yxfzwdgt.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2opkpbrcr.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2xemukmfz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2zwhsahnp.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2bzaaataq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2zaeacqxa.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2bktyvgnm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2eywlapsp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2cdveexvq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2auvnxpan.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jjnpofab.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hodqbvay.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2schqxgsw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2sjnqkajx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2peimbccg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2gyvbmfik.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2rxufpwjw.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2jzpobbxa.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gydezadw.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2onhkviqn.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uqmvbxrk.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nvpdotvi.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lpyuzusg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fubuewhl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2bxcgttdj.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2phhxqzjy.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfrsldgh.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2iyfqulsl.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ktvdxfqd.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2nptagjom.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ogbtlzxb.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2hgpplmpz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mqdrduht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qjevplxw.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jofujqqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mpfuceju.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2crbozapz.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2lfcunlas.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dfhhyvnw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmlmwefr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lteuijer.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qygtkpex.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rjzdnrgm.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ryjpfhkf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cghirsvy.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2zfgiudos.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2xcfdbuzd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2pgpkncqh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sznyovxb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2thbhvstr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2gqbceanw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2tshnbeul.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2bjeywxnp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2vzgvkqdx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2fhoyxfce.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2tryvrsaa.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2kgagaehe.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2osfvrgbs.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2cjugjkbm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ynjqxzcj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2wzadmucf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2lpdigmhb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2racdjmrm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2cxukqdvp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ogcdrppg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2meyccwrh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ezfnglxe.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2xlxuxgig.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2rwgbdhpu.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2qgcaujze.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ndzterfn.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bkhhdnuk.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2exnjydty.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2wmosqntu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2oyemzovx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hrwipero.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2piroksfw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2kldswjnm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2yhjustje.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gyzrkpyn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2aczdlhjp.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2bomlltpa.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2mktkesjj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2jzdoeoos.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rtwdfmkq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lprwymkd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xnbohqwy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wmwsfnzp.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2nmauidar.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dzttujny.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2fkjrjayg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ddypynmu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2bxdyywns.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2mvkizdnx.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2clfnxyoi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2rmzciads.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2csenmbpo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2kzmlbsty.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2xsmbvkhl.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2bgaidznk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2fcuprrdo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynbjdorb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pknmlylx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ivavuezl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2qiefkrri.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2kfbcsjkj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2nkorwwac.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvxvxkna.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2xwmwheii.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ehoaqlsu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2cajyvfkw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2kjqmvqfu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hxzzvabf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mnweydwv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2wyawjvxs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2nomcmzbz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2jwgzephx.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rzmpsaus.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2qjqclnca.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2dkgxflcl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2vxbsgxnh.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fuajpgmi.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tnymqcvd.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pnzooouv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2youhqhoq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ifpmdayb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2pbenjtxc.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2nfuwmwqr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2dzpaciye.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2jddkmqmi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ucuacmsa.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ufivngwm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2fajaoqzy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2outijetl.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2kdjayjow.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2tizcagug.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2icosttmz.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2yhklxvmy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2orwtxwav.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vjorklyi.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2iargzwdu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2zfhhsmsz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2zvnjwsxv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ztbvovse.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2mrpssrae.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2iquymljs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2inqaudls.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2rjchrosz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dbjydeox.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hgqjrlhd.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2kvqsyscf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2gxnqwrrw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2zdjjfjpc.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2niwavwqj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2vvauqtid.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2oovpvddq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qsbkuycy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pneccern.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ubxzxptj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ddaesotf.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ifrkmurf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2gxukbewu.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2txbklmdi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ispjxehn.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2uwkwlrnn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vxkjhref.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2upmaluqn.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2tmdxaevf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2uoqypkoc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2isojghmz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2xjxyhtrs.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2kcjqyjps.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2zlmajbrj.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2aozxrslw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2fnaedlfi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2aiezxjnw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bdqbgsbb.html


<!-- 参考信息 -->