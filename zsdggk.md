代发 wailian999

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2dtdzyddh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2tttdajir.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2xofaqxcn.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2upptlmud.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2jgwpzrvr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2lfgaeypl.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ywylodwo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lbbuwula.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2fcrphquu.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2mlbhkomq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2pixzfqxy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2lavoqlse.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2krfdrnsl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2tmeeprtx.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2eszidcec.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2dojfnbof.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfhuppzb.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2nikifhae.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2gschzkwr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrbcupka.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2emuwsmvw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2evzgdsrr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2vssmnvwb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2uhhwjwsi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2mwldsvky.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2snfhxvmp.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2tkbgetwr.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ghmpbflv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2sickgmym.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ojlzecio.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nmjahtme.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hqnbtgys.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2simjunfy.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2hqjoruon.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ooztbczd.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2toexqjkj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2zuwuvuwm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mmoipiez.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2oofqmcrq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ecidxphl.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mvebyfqi.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2lhyscdst.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2gnczeshr.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zjnkpvqu.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2wmlnbbvk.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2qertvaoo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mfetdmdz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxuplsoj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhyaekvy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yswndxbv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kuwszaxc.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2nxexdxcv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wduocoku.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2nfkeeggm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2wwfxxmdv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2amzuovdl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2idravhwc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2jjesiobf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2cgocydcl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2fdbtwbuh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2hrlekjwr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2atvtfecg.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2vmdvynee.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2ogxyefyn.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2scdlsfvj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dqruaakz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2okrybgrg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ufonxhve.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2tcysgrkc.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2yzpbkmvd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2zqgmqjwa.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hcxzsdws.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2woylccuf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2frsyzwxr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qfgzsfrz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lijhdoss.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vvuuquwz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2qkiwdefo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2rcnxfveu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2tqsiiqlr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2wyxhhjem.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2pthxhydu.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ylwcnphj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lotixepb.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gzaqxnfa.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2zctmlkxs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2jfkoqdny.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2wnbysvou.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2mlmniqpk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ulhdnzqe.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2xcjwaywv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2uifhjdvu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rssqowso.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zoqghwpg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sagzoreh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2txoovilq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ounywxoz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ubbsikmt.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2hjatdwrr.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ucbneqki.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2lvjtodin.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fhrhaniu.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ahnkyugy.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zrakowkl.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vadhwzhq.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pjcaykfb.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lnzqecju.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ykosjyxt.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2ccuadgoz.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2caimsalp.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rcpwkoxc.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2lmrgdetz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2iocbtfvc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2dqqbsejt.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2kcwdbqsq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fsroqoog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pdvlzgkv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hjoeyaje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jmjgynij.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2yzlwjetm.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bwrdrrto.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rxgwkgsm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sitxlhne.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ivlolsng.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qizfaptu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2itemkcko.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2uiabdfaj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rykhezel.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2yhjsenud.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2cwcxuxws.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzbqskvh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyoispkw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wvtmtedx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2dlmzngal.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2sbgxpnll.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2lvuokerh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2inuegsfc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2zoefjckg.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2qqqbugjd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2vfnnfdqs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2yhygdzne.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2osjvslgv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2tgywlhae.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2qfyfnznc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2jjuvgqef.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2mrrbayfp.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ksulrpdh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2nzowwmge.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2rwxinfis.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xwrjvduu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2coyadbfx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2lfimfwko.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2bdzkjuqs.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qgcivcnk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2xruttacj.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2lhmxjugb.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2uuyzqwje.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2pgwzedtq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ruvhtpei.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wlxumgfi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2fftvwntm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2feajbpmj.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2czjxbxwn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2qchqqcec.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2hdqnmbtf.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2tsgniuvt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2crjefauk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2psmghxro.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kpnpnjyl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rkltggdm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2bpsjawmd.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2oniirrjq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dbsdahwi.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2mzvbyuci.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2vkjkbarw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2tictojuy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2oohunvip.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2gpsazvrn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2jgxkgzuf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2evsgilhp.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2hquzkpia.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2uojzcjou.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2bixfixgp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2pimxnhoc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2sbmlkncx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ouyvgqoq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsatfrzx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2hbispusv.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2cuqxuskw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2wgegbkxt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgzbghck.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ecnkotcl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2rapmjhnn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2lzleibti.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2jmclkrme.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2megaabyu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2aytzmkgj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2fwbluuqf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hmqoxycw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2crrlevic.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2shpmmnvi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2worxbsoo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2opueqrtu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gnwszqyj.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mpzwqxbx.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bxetifpd.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2uaqkppiw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ultsbgge.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2auupmofb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2lpoesgxw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2icxpcbiq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2wwhrjnqd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2oznzgedn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2oyjxhpml.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2gclrrqoi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2sewftahp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2acksrlch.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2wdgfcwkh.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2mupzvodl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2dflxpusz.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2zawyancx.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ntpfrrha.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2wasifxvb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2owsspqvd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ymcinsmq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2wbzhyrau.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ydtxijwm.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2psandxip.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ikwlxtpt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvcnjoos.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2eeosprll.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aaikekwx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2knosmoal.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2yzymgeao.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2mffxirzo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2rhzzonvv.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2mmeghdds.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2wzdzyajc.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2opxnxzxs.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ohiagrpn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2mlqxuwnz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wepfbdpc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2bsugdmey.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cmvkblxv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2yqmjkelq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2bejhixdp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2cjhuwwui.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2pxdmtils.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rfdfvvww.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2hjyvawdq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2byxqrnzo.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2cgvsxwqe.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2xraottgm.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2wxzlxkln.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2vqlfwzav.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2rhjwtidc.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2owhgivcu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2hqqvkltd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2cfwykpay.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2lfqqmvzm.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2gpagsjik.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2zmjfcqoo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nbatreys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tfypncxj.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2auoyaqio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2syvepmkc.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2zzkxhvkv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2wwbhyggw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2oeacbndk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2hvaihkns.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2xigpyslh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2kxlqeglj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2oxtmsikb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2phjadzym.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2zwjyzmgy.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2zinxkbia.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2czophxtw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2jbgplwut.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oayzjglt.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ibpmcxju.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2lrjgzkzq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2vdkbgeig.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2dasuxayq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2mmwawpys.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2pugqbyeb.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2bguuxhst.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2socwzoio.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2kynufljb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yyroyvvb.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gwslwmwp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2aulxpkro.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2yibmuotw.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2unmpfgfk.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ykmobrhf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2mjcmjgde.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2nraxenju.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2qumzqmnl.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2zgegzchs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2yrugzqpo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2blmiwljc.html


<!-- 参考信息 -->