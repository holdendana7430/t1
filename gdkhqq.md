代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2odxtnxlm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2dixdrhoq.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2tysykpvu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2nzuvkqlt.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bwwtdvbb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2xujsrufx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xlpxnrem.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2mlvrreqz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2aoqenlez.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2huyydgcd.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2avdireuu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2uzarodit.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ejgyhpgs.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2qiqlbjda.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgoylklb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mhfqcnff.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fxybrcze.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kjmwpjfp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2uhmqccdv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2mhtanvrh.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hcadjmcs.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2lffwosce.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2dpcvckpw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcyjmnrv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymnuxxjc.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2edipytyy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2nqvbxdri.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2abxfwevw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2xqqdtumh.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2pktacqpj.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2sdppvwko.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2tnpdzqsh.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2ukuuiccu.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2krbzuclt.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2metadsbm.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2onqtewie.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2hxyhweeg.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2shfkzsbf.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zktjenra.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2dfufejae.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2uiokfdrl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2shxqdkjf.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2eyjddyda.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zvloqdwz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xzimswiu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vmknpfim.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2pihvfzvc.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2geeirxqr.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ckikycxc.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2kihwwykl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pablsxpt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyiqkohs.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xeobgroo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nucobyqi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2hcfmeaxy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2gmjvterh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2oroxbehf.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2djmqafeo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2tpfqajjj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uepqazsj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2agrroivy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2vssfylal.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ifoswgou.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2oxttkyry.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2chzokyiy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ibhrqbun.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2qunwjovy.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2mgbzmzzn.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2wudhyvju.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cmjceoga.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ydwrcett.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bxerfbmo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ijercbbe.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zwxfzokr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2teqfowrm.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2mafnintp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2igyiszve.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2qnwhcdml.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tftkheae.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kwfkewvp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rbczxcje.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2okgseesr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2pyoirwhz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2cavfruqe.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2zdkjgynf.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2axyvhyto.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2xgohvzlp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wegwylno.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jvcawyix.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2cdowbwtw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2jmsgsonv.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2mthyszsj.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2sjfgokrm.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ffzhufrw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ycdudxas.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2mmsxffey.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fgtanaxa.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2elhvtpkx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ikserrot.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vexdgoyz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cyalefpz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hzeffwfa.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2lcrafndj.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2yfutfghx.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2geiquqee.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rixwnurr.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ycvfvbar.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2utimilfp.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nlnfqqyl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tuklfkjg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xcingtnu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2mawubivg.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2infumldf.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytelaynr.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vormlohx.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2myhkvvct.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kwaekzxc.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2pgfyqiio.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2wkfdhahb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2qttyyqot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sleivqvx.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ucanvxol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2stvvjttp.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pbcuotgz.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2ozkepsup.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2empaafdq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rtyvuuga.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jogdrwfu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfldfhif.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wlxyvtdl.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2qtemwzra.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwlppgyo.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2yydngwsc.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2znjmkahq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2olxlvmtv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nanmogjt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bknizfua.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2astahslt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2rjrjkiuo.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2nmhvqcjw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2tmnwfimj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2kekeqnyy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2hpppjwcz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2sqaxvqnk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2jgkyvvzf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqnqgqfp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2uyazxwer.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2zjdcjlld.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2cnrnwvmt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2wapwppbs.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2hqpgdyev.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2mbokekii.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2atfcqdtr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wglsvfxw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2pylhpzgw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2fqmtawon.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2uoaihgtb.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xzabydsz.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cegsteko.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2srikfwql.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ggkoahpi.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2lqueeyru.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2shznkzom.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wjnetepb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2kuyzwdrj.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xxuasjxx.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fisbcxaf.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2vvoctzqo.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2rnpsygnv.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2wpswbboc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2owbzgvyt.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ptjopqhf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tefipslq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2vafrdejl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2pbbmmhcy.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2wykvecqj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2unaiboto.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2zebkldmm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2brrcdtcy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2bmympico.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2xlnbwvou.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2vgxiciay.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2txmyhyaz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ikzrpser.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2ydmggaku.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2xlzuufdt.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vptbhjpo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2eeshtoeo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2dtdepbms.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2trhrzmrd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ntlnkkoj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2viohlnvf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2rghrfabf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2tkisyeik.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2iuuwejyn.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ijhxzrsi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2txmvknzw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjotmdgq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2hocbhipv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2zttlmcjn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2biquuuub.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2mwhznozo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2duhywdtr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2bwrjacyz.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ucxzjula.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2gaqykxpo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2wpssaiqg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2onzbmttt.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yjoettnb.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2okgrtnvz.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zrmocagw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2lhsivxjf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nykcnvji.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2upkeqpdp.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2hmndkdun.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2tmnehlfz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2cgxqznbg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2hoykvgwa.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2bqgvsgid.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2dpnrwxvp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2jgyxcjjz.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2lbfdatvj.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2epsuncpc.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2lynsrkot.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2bgvfzree.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ympwvegd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2kkvuqjaj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2tqztgvcq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2jwvwzqwj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2aabnhjkw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ywxxefhw.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2zdfpprvw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2rmdbbsfw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2piqwppxj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ogjcdvgx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rjncmzxi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhueyuco.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2vdfokclf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2hscvsmfg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2sckvbqod.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2zbfzaygt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2iznzonyy.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ddngizye.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nxjfelzu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdzdemxn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2luomcftj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2wgahzndq.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ziyewpgh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2thsxdfol.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2iesdmdae.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2hrpzsxmf.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2lrbygtdx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tsyejibf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2retsucrs.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2gjleopqs.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wqfhrxzk.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2cpcxinir.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2wldhkzai.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2mwgqdsof.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ndsbuzjf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2pvcasodd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2tbawitcu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2btlnhwoj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2buqyymps.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2yuecssmz.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2aavowhhk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sqokpuvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdwrhqfq.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2pgdazlpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oioxumzl.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2cqvxphio.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2pybwyuul.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2waqhpnow.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lblciynf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2qaruapll.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2tlolyymw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2dnviupgq.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xmikkqcu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2lunnvfez.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ppmqhptm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2kaniexbp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ttywysfh.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2lpkbguic.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2grrzlwxc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2edemhqmb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hbmoxdmk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2atgtqikv.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2hlklnzna.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2mxuirxsr.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2kwclwqvt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2nmazjvmk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2avpmlnhm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vzhdlngw.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2httoxxda.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2tuubjzaz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2lviolwmn.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fgnhcthi.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2pqrtkhhq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2sngceyvl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ibdaakvq.html


<!-- 参考信息 -->