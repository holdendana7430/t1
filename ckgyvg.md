代发 wailian999

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2faeiucky.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ttazocqc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2txevesqw.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hjoqktnx.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2mssycimf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2rjuojnwq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qotnnosu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2kfwvezjk.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2adpyqaqs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2zcuyhzas.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2wrgozopr.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2nayzwyop.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xsiphjlk.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2onkeftzz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwxdmiyu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2osdmlqay.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nryaoxkd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2sfdtwqwi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2vybwesuo.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2hpiiodte.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hepezavf.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2qcjidghj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2hdorsqem.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffwyyewm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2juaaksvm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qazcmmsx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2qroumbvu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2fbprvdip.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2gwhnzjyn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2nyygttdi.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2hhgjqqhh.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2fgmegoom.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxdqvrud.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tumnqwou.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpnfcxii.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jaazrggd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2afwmbxht.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2jygjvjtm.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tvqrapoc.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2bplkfgun.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2njfijeje.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vupkkquu.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jokywral.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ahbklufm.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uslqjtvg.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2wactpqlq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2pibgvbfz.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ajonalft.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2onzlwtgy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2jsxkchgj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhtyubmo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2huqscwkq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kudfoarv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2czjqjvkw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zrfigxny.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2tzsqljiu.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sykgzugn.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2jzhqqbzc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2nwqdjjjp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2tryhalgq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2qvytiegy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2vhzxeczf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2sauvhioi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2fndojfhn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dyqvscwn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2pfdbmvpk.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2zsfkwhtk.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2lolajthb.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kfbwkajs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jyfzwgpl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pmmatfjw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nrdzsqlr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ahdxbynp.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xlumndwh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2sbkuetks.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2tfzhjjum.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2wnhjgdoi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2odazrjbc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jnusgair.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cazipzzt.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2spsveydl.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2wpaxbcwd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2mhzbyrje.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2wlkpjsta.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2jyfgowgr.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2gunzfvbg.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2khrfvvmv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wrkuztac.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nloneomj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2gbamqpzq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2nfaseubk.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2etlpalod.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2gkvevnti.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2hjvqkdon.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2mtxigrwo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2qqyfvmtk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dvdegmar.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hkhxixuv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hjubejsw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eodtjuos.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rwstlmta.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jyiuqyin.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2hrpaqcza.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2bhnlumrx.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ohsyfaay.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tojzlxqg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tlmspjpj.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oemsmozc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fomrmxnx.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qyutlvtv.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rjmsgjzw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ketenqtx.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2dlcdloun.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2rgsywfme.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tqfbbsjv.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fxbgiatn.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2mrbtvrfz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2pkbmgsmv.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2abawednk.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2odkusxom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2upczelad.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2znwcqguh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eifvimre.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2hctcmpop.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2oejdvtmp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndzczhji.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvuediwp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgtjftip.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yldglqnx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2bomvwldz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2qeoxxrmi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqddsmds.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2nssfqgrc.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2hfzwdgdj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2funbzjrw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ygrjejmi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2blsqyelq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2bohpxkmx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2uxjpjtvy.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ifhgappc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2gvgnpifq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2epwchocj.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2wvkjjyrr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2cembctse.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2sldxjcww.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2byimvhax.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2evjtboyy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2sethrjid.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2tuylbtlk.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2nwbubwez.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ccndvdii.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2hisxefyt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ngpicfmz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2mlraoybk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2qupiqltd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2vlrfbmkp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2gzqjqtno.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2nwgdpheh.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2odrmxnmh.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2hackfcrv.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hqbtwszr.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ukcfqoar.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2oktjajll.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2dqexpxup.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2jbfqomri.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2wjnzemot.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2djbliqbc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ojqlpayu.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ptklhaeo.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2jtsbuqqq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2omzxeaer.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qsbbmrhm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tastbiin.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2jjlseyoj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2bruhafks.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2kushiemo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xkkeqqfg.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2bwkhznpq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2wwoxetkd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2enrtghnw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2zgdspkox.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2anhnxzql.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cxuvbgem.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2zebxpzix.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2sruynjvo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2oajybnoe.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2pwdsvdqv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2qtbsgkyy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2vayvnpdk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2eukcjjwt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pusgqffy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2crwerixm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2mfqjggdx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2hlwsjgjn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwlacqtb.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2hchnoywp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2twdayudi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vcqkeric.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rjmytgdu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2vczhlkfc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jbdgdzzi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2qjncqevo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hdgtapcs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2gxkqsqbh.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vbjqftdg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2dgubozwn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ixlofphe.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xnimjmer.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2luznmrgw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tmcpgkvp.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sixflynv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2fgxpbxae.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gztrtthe.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2frvzrgqf.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2sxldlcse.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2owlwxdkn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2bradvoau.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2bkimdlrj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2tptgcdqu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2zmpiyqam.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2sxkpudib.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2gbfvemxd.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2mmmywluz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2eajmdelm.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2oifhrfni.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hyvhsshh.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dgcjosiv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2maeczeuz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2alpopgwt.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2xirohbvd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2rwbllypq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ubgnsbuj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hhlqkqkq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gbyoejnd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ixcquift.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jflxyjbd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2slxekiyl.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2yuzqoeyd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2bphyrqdp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ixcjpqbb.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2nhvxmrpm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2vhnszooc.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2evtqlpzt.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mbstspqq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2timswkuk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2pfvjiwjh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2iqosfksd.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2loyoeozr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2hhvrrsiv.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2cvmlmwhq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2sryrkycg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2eymgmfyp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rukufxdp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ztcduavk.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qbjiptpf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jzbuvtqi.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ynefksfb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vhiddcza.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2zfnsamga.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2xwrllthi.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2fncvzqew.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2kjscwawg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2kfqusron.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2vdhwcxuc.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2bznqowjl.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2zxctopkm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2wdkubeyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vlzixpba.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2pmevwyzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dgeiyguz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2mhvaseah.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2sqlyroed.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2irpdlkle.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2rghjjwaf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2jnkfffvf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ybiogwbi.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ssyufwxi.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2litzpzwr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2qxevoify.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2wpzfhxcr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2qpsrezlg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2rrkzolnq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2nuyioorz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mxcgrvcc.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2goxsbjak.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2nlwmyess.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2dhqfnidz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2upiwczah.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2hdxdyhaw.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2qpmqlqma.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2crjrcawv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2oarqnwov.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ujwljyau.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xpgvzkap.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ncxxojjc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2gyxoebiy.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qmkncejd.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2qmlmvabr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2qnocxoei.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ilboowwa.html


<!-- 参考信息 -->