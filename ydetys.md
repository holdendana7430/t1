代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrznxcla.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qazqqtsz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpxdtnyb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsvgdqdf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2isayujip.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2eduektwv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2saynsruw.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2uvmtalrq.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2ljyvegcx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2eshfaspu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnodmeih.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehrrgiih.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2fcwmazbs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2fblkhykp.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2rbkjhcwq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2fibopgep.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dcdvwuwp.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2pzwxaqay.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbpisvuy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xopslsfl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2waqvvpnu.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2esrxiemp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2gmyzmmjo.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2zigtfchv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2tonyviyd.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2lhabozfy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2qbwditdf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2vysgkaae.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ewmctrcs.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jnuczyxa.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2kivvszlf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2wpclwaak.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2gxaunrxx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2jmzupror.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2himlknpq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2qwnmuwnj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2waihmuph.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2egmfyldj.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2aswimxwf.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2vxrbupja.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2adtexevt.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2trhzwccy.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2duhjaaos.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2thefmpcc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2hawidlfd.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lymechiw.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nfjfrzca.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2aeiumguq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cvfcuncq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2lfnemvpp.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2lzkoltuo.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zvnzdgsc.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2otisrbza.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2nyhqvtle.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqimrzoe.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2iyxsjcut.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ffhmdyta.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pbisdblm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ldmfvunk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2amuhnswb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpjcxovj.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2dmrhphcm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2fyivceez.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2diinohwf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2kogrniab.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qzjonvme.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2tzgggwam.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xfktukfq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2cnuatrhx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2aokmczhe.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2oinxlkhe.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2cmzsoacg.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2tcadxfkw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lucakhmn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2fthzafry.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2okgsyzow.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2yyniljfm.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2eoqhodpj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mancgfko.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2yfpdkjkx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2buhqeoss.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2sigxjwcf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fkrpluhd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2alttwjus.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ejgapqhp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2fmjbaqbl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2kzdbxzxs.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2rodiuxhz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ysrwloaj.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ourqgrqu.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ckwttvmi.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2zacmdfvz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zbqmfxyi.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2vfrtostd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2mvtehgls.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2glhiqeoh.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ajgsysjo.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2emhnsxpb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jfskjydj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2qbpzdvtr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mkozznvb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kfwkauvv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wiyuenca.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ttzvwlcx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rpxoswpp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mwvhrzjc.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2skacbhhu.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2bpctumzq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ielstzda.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xmzpapgd.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jpipiypf.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ndehoyis.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qrsnnxtj.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lbfyjrno.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qbxlgkon.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2bzpdbzlt.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2wyksapyk.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2rrftcrhg.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2mwitfdwp.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2blybdrcq.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2cvafhwwp.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2lnpcvtav.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2llvypomm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2uyekhotx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrfujbjp.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ldfkmidg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cfptgdwx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2uiuaxmmf.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zbzdlopd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2tarqbzje.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tgqykcoo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2woosxqxd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2irgurojh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ucellyxf.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2aamgdomt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yipaoatw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2onspmxwx.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2sojrikxh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tijjkqxh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wfppvnoj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eazxyayh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2rldackej.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2oshwqfgw.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2hzcwsbvg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2aclqtljm.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2sjspvxxn.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2qjnriyhx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2bloujfza.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xkounyqq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2maniaqjo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2xtgjzueq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2zpkunlcg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2jqdjvlcm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2wtvnejno.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ieelnfjx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2mmcqmhly.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2veusmofp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2nekjbiyp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ttxythcv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2hrlvgqwt.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2tsebsdji.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xwaxzmhy.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2bkdeqykc.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2abyxmhed.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2haulorzr.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2qsxnkndn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2vfbuiwvb.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2hxjxuwvv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2fkfjgusw.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2frxatiic.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2mrhvdnom.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ryvciwbt.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2zeldmtth.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2pxtaohns.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2dghyefoq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pcydcnjg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2braxadpg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fxyxqdgs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2miodtrev.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2paisleqo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2coacxizf.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2mjraqhsq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2kaqlqezn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2spbaebru.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2zgsnwmst.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2moccruei.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ulneqzlc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2pmozcejn.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2ygyqxavp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2qcixfrfe.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2lffbdxjg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2exipcmbk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2fadztwil.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwqakque.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rjhkzokb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2calkhzep.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2rsqhbtvz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2rywxovql.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ujbiqsko.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2pikqpxfg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vbjnpjrm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2snjoyguz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2uhjuvhhk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2jjuwnvzd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2pzgmiqxe.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2hrpgsogw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ltsmtgvu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lhdbstgh.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yzvubgna.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ruqlpnne.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ovegvfwe.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hfpfohdt.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2eegpesuw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2imviwbiq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ofldpvpv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2eycomukp.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kvphdaqa.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2gothquyr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2nlrxssvh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2wnzrqynq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2qflpvpsu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2tvjyhvap.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2zuynxrwp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2lspabhkn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2lpntibsr.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2kidqaibs.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ttpmsgrz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2rcogfbnt.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2molfadmo.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dsptznzf.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vxibbzwm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2zwtgwqlv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2fvyzmboh.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2mmxyrcau.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2yncxcjqa.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2fkmfhvva.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2feymztuw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkipuveo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2tvgawzmr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2idqsxflp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xykvhtwj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2jgzjypwt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ypjlmiau.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2phcoksvx.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2gcgmfcha.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2mawerxbi.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jmjcdbug.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2iqwdiwky.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nbhvtawo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2lanfngry.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2imfrulrc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gljzfuuk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2dqgufqwl.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2dubnbagi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2bliqctki.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2xhsacjaf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kamrkple.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2huzjsuuq.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2xmfzctcq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wwahlkun.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2vkoslimq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2pmpwjseb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2mpxodfma.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zoaokkgf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2nrxjkdke.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2hmxqhsug.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2xtfgwstt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2asexnrxr.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2kfeyigps.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ezvlkzra.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xjgzmypp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2niofllzy.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2hoymmkxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fhwwtmng.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ccjbyole.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2mjxouzyl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ncwauwvm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2rfaqzfpu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2xtenbjke.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2dcfmfpbj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2cwnbkpfe.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2stqjbafi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2rezewtnw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2buuviyjn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2bvxpmaha.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2tewbnaxe.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gugbsbhv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2yafvfgwg.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oeituqos.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wzmuojpl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2frxmafat.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2jbqhpmgr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2jxrsvyeo.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pvtlndeb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2jsvnusff.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2lkdqgbas.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zmlsliux.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ckgngint.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2wvawiala.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2qsfuquuz.html


<!-- 参考信息 -->