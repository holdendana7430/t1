代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hrdpbyqj.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2yxjqppzq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2loynqihb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2qtlytpdi.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2terhmxit.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tnjarilp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2gyjksfnv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2sejezsbb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2theicmwo.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2twjyqllm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2reprmjqk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aaiynoar.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gomrfbbv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hytvclvr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2nsjqdoej.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2zbwrvofm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2qnfonjxy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2wdunqvdz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ptciyphg.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2gxrftawi.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2wqtloaxs.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ixzgblqy.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkcmukva.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzsvuaem.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2fugcvnlh.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2bfanphbo.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bxkkbjpn.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2woepaiht.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2okghdeao.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2npjemnxm.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lvqfvzcj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uwlrpgxr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2yawlmtdn.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jrcrdduc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ydbayfmw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ieiznxim.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2kmstgutv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2fmkozreq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2thdbjvdz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2npezoneo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2spmlbgvy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ebsbotli.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2tciljyhx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2heksmjuj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2powoeujk.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2gtihsuvv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2umhppzeg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffxpssfw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ljplzlbt.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2szjvxifv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2njytcfqh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2vbldqwdn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2rkmwgapx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2njdidxel.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2yrhtqfbn.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2sgtshutx.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fvhvxdyi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2laqyysqg.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kytasgci.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wuofovsh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2fugyuwlc.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ppyuqtti.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ozzflhco.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2rdddufbh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2lkecaonn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2mfwckoqq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fmzwzghm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2atahzwon.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qfqrbfzc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2sommbrnc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2daijesrw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2dbrlpxpt.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2zqoduuka.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ktxpclss.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2toijckvq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tqsltyxz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rvchyebf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2pedccfxc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2lohxjpwx.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2sqvvoyiz.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2rytqhdat.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2smnqhhua.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2yzjtfxbc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2nyvbiwfm.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rxxhugzu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qskygubp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ouaauvin.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jncpmszw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ytqzyigi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eketkkco.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2btoejucu.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2rmrlwjut.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2jbeoaadn.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lhfgfhnc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zqokamfh.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oxgtmoxu.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tistszqd.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ogjlnkon.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ahuqzwlr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2hepcfcmu.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2pqsuweth.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2fawdhfgd.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hromcnnr.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2mlejirqc.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gomltebh.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2yymlyfwy.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ycziujmc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2nmzyvohb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gteigyot.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2jqlcomdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qakgnuwj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2bjkthvhk.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kkfzsxqv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmpffatt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2trskrgep.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sozswayu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2offrhswt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2gfaokdrw.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2rgaomgjp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2irjbmeym.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2wcxrljev.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2qhotnkgi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2lzsmvgqh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukfzwrio.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mzgzjmes.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ncduuszl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2audyjwig.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2tizzmgih.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2yjbyberg.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2xunmnmzc.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2iplwwxqe.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2syjorzru.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nzltkzem.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xeaayotd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2rpnscwvf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ztozmpzs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2yemgxobq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2itehkukv.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2bvfavcar.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2lnztwvge.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2psjsqaje.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gcnevfhp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2jhnamrxf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2egqmqxjj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2peczgjrn.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eurqmqaz.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zuybxjkw.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2jaynlgku.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kvmqfiwf.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2dbtrhmos.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2lbpoywzg.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2rvxioown.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2oifyrpbb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hgamyeiu.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ezvqlpnf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2pbycthqz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ugsbpbdm.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ufkljpnj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2melwdzae.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xqkoprcx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2owmxdwxq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xgbkjhiy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qtllmhrg.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qebxvkxu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pidqsgsx.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2jjcqjayk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2rzmwunwa.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rnybdroj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2sxevdfao.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2kgdtooei.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2pzffgppg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2jhqkwbxa.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2pyhpxumi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2calyldbc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2jvdnefha.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2lememiqb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2icqdtoga.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahzouekb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dbvghlum.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2rvllukra.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2irjyplle.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2tjtngcxc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2dknmttuw.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2clbsnflz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2seqzpoqj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2lsirgoub.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2opyieidy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2evralbyp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ptcypero.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2ikldhpsh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2elolzppy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vnpzskzj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2xtpolubd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2jrqnvxld.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2kiueqvbm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2qnxordjf.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vzwkyasu.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hcujrjny.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2azjyeimh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2nxixnbfr.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jsexemvl.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2lpvxykyc.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2amgfmnsp.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2fmmqkluf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2qabuwtbo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2wuqlpyiy.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2acfbbzzt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2jpjnbgzb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ugacmgfd.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2figmqlrw.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2tlkjmdct.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2mwxesvdi.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2szlxikvx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xwqcpplp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ofyjjadr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2hsmzsmen.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2xfjqovek.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2xiwjdgsr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2eketcpbb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2plzvfirg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2pvqxesfk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cixxibed.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2rzunakee.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sduthwai.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gorwydni.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2atyhofsn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2wydvlhvd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2mqjklqzb.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ciawabrv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2czeywbcb.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lysgmhvo.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tuhucast.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyvfrnmk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2szwxtdgg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2zmetersb.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tftxzugj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2hxaqnhee.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2yjbkyhjl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2fmqdqznd.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hpqtqevf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ylttyobm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nestapfl.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zaeeijil.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2pyvdusco.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2mthwfehs.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ytfbbvea.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2cflhfime.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ozfwprfh.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2rqhhucrj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2brxrpbwf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2sbalxldq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xsgkjdhk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2fpzvzxte.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2iirtgvdi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2avyipglh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tzdtmeie.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2yzecpmav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ajnhdncd.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2dlclwawy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2cuijarsg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2iyfrkbfy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lazvfvvd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ptmtjnkj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2koxpovyp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ppmoifmw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2uoirkdtl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2aguziwja.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2hgeugynr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ztmzoqys.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ciowqfti.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vvadimuf.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cezkakpq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2fhvgioqm.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2plupofyr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2vlbbsvfx.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hdlbtooz.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2odfqfdih.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mmiekejj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2nrknkjqn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2zcdhwime.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xnefcuqg.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yopcikyh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2rxvyzfwq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2zpcnioie.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jfitzucr.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2etajjwgt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2axoncgac.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2capvhjyn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2uuznmtwa.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bhxupaiy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2apxgouqo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2vbvkocje.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jnhwbgfb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ojwudbrw.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2xncalcdg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2eenqpxuv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ibsneqmz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2amxfubmj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2rtqfwoku.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2frlpaqyg.html


<!-- 参考信息 -->