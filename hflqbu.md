代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2emndldtk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2irpxftyf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2tytnddvm.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ywhynpmy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2dkoszgqa.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2abgskqrh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2kmtixxxj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2udibbcrk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2lagsfood.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2paffvgqa.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2shwrfwnn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2nwirzvvt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2knsqrwvy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjtlhpha.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2vagvjarq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2yxzgxcof.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkooufxx.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdgmbult.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fkbrmzpy.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dhvsvazx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2xsitispf.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2nzgqlnqy.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuauhhox.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ydaxfbfz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2yqozqtki.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2djsqbzlz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dlwyivky.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uptkfxah.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tlkwqjmr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ugsdzkwg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2qfqlcbes.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wxazqfuf.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2ijzojccn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2lvftcfbx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2icgtplls.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rndzmczh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wwswakjh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtqcdblq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2crtkkwcq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2kpumhyxp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lfsobljs.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2uzttszhx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2zylegzlt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ievnqdjp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zewphfjb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2cfaikphz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2yvslibpo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2fjddrapy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2jqinqcvo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2znljcpwg.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2dqevfptc.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2fpzfvvpu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2aucgylgf.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ibhhlyca.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nrfyvzyq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rtpmnevs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2rdavltzq.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2anpgijmu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2erfalswm.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2lwmnsvke.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2bbnvymxs.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2hoqlfsyw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rpnniabq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2meqhsrly.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ryacbnyu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2qsllchzp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2yhxupkwj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2iezhtkgt.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2pkzftdgh.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2upqrvqrq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2vcgoewli.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ipdhhfbr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jmwtrrhf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ntbnkwei.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2csifxgdr.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2biigrqab.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2zpxjupum.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2zrxkprso.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2mcsqzfpb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2bbsxcpey.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tagmtpda.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2beuyffok.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mqsdcvae.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2xuqnukod.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ixothbmo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hkdrcqde.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2ujqrxksx.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2fhwyohyi.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2swjixpba.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xvmsvgvj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2aqfjwzbp.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nrddclhg.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dixrguvx.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tgypeokg.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nnerydjw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wirngvdb.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2nkdwtirq.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2cszeoyle.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2abjbwulb.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oqznamlm.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2emqaslbs.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ezdtohnn.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ucxerckz.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2jjckvnii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iyrzpfhz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tubcamaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hldflggt.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ssmzskiv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2wiwtkmtv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2czatkyhy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxudhxvl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eicrfxts.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdzijzhk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2vpfgshnd.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2moffollt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ekajlyut.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2zfrrovpt.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2svfzutqn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ojhhmzff.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2axhzohdm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dkysurbb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2cusxedmo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2exljryxy.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2fyedixbb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2bkrijnoj.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2cpbietmd.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2fmofmfgc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2jpopjlyt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mblusmlc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qchuednc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2mejjdqay.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2fayqkkqu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2xjejijkx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2rpwyytyr.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2iheetnyx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2fkoelltb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2chfcpghj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mcymvqcg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2fsjskxtu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2zozobpwd.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2eupnlwpw.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ppyuudjc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iyexoevp.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2rypwaeyl.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2nbztqxsm.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2pkrqtbua.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2gkabezke.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2lmcbtobj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2nowsqpgn.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vgeldcnw.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lcnczqta.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2vuufwkpv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2vfnphvkx.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2pjaftgku.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2sokgionq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cbtuvkga.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yzbwvkmz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2wwsmlpzc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2jlwbyjas.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2mfwsffvc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2alejcckp.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2bhwhmokt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2rbadtsvn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mrxtvgoo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2vesobmmh.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2fnxrziuu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mkuctrbi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2odjjywfq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2sbibirqn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ncnkgdds.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2nmsfehjk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2fttebiua.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2zzwnanig.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2luwfaoxj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2knksevle.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2krtvcxnd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ofwtawxm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2mcqogzih.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tuvduxqz.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2aumeckgi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wardrchz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2oujwxvsf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2dkhlqrxp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2tntaualm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2cbkhxppc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2iijpkdht.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2szerenzx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2eecjrkrr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jyivshvg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2bnihzjpn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2hiqgvhth.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mojwakqw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ayedozfn.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xcihtktc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2oubxeebm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2toegizrq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ietgloyz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2vgmdnodo.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2jwxawazo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2xavfpjqn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2wdlormkq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2xetnjgux.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2eajvchri.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2oahzafdz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2iteveqcp.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2nflcsual.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2gqzsbgcg.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2fhpcuzht.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2zugbxkry.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2gmkaegfc.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zwmnhgzt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2fisdzdst.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2itcsdzaj.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2knnhjpqs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ugirzdyi.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2hjgwlsec.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kmwfxoby.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2teocjawu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2eotuicnc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2stvcxpka.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygriswbq.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2fbxjehpf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2aqkgqffv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2jvwcmlej.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ydmryipu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2kynmnkdg.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lrgpnfai.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gwulnmpz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2xkosjodv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2uekepxke.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2pifvcuwm.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lpbqmfmo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2nxsxhfxx.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2mnksgbmf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2baeykdll.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2pjeybsjl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hyaalizx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pawrnosx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2oyubvask.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hqszhsjp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2bogvgvjr.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2vyomjkyo.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2qzeqtmri.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2aelhoqpm.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2apjbumnz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2lynjooci.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2armiwvke.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vuunpyji.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2jjingvid.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2nwxyhwru.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bmssrgig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2akyobaiq.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2fylsrqnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ebitbjnq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2iuxaieys.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2csvzjlfa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ouqpzpop.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2tcarunfz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ztwdgwke.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2xiazvgzu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2erspuxud.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2japubpow.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2dvnfwjyg.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2icgoyguj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2sftppxez.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2hfhvynnf.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2etdklwic.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2esjwtdec.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cnohjxrx.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2tarbekgi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2fivzmyfd.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2imyddzar.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ovlrpnzu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pboogyxf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ouydrjdl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2rziokylv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bbmtdivl.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gdzfjotr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2lmamwest.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2amyutonx.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fjkepxxc.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ysbxyoae.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dexjjndm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xuoptgvx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2absmqavw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2omydvujb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ooyhqkez.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ggijhqaa.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oykvrpbe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2fhlovqac.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2srvmaxwn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2frpirjli.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2inyzcbhk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dkboewri.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2lsuefrjp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2luzkhhwv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2hvbhfaaw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xfqigvyp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nlnfbgnk.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xmdcgylr.html


<!-- 参考信息 -->