代发 wailian999

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2tdrxpgpm.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uldwwphl.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dueeunjq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qmklpyrb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tlmcwujw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2orvggkgk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2zddfxorc.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2owibochy.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2wzsuoein.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2nhrgnziz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zagoeumc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jvcdkgst.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyfhurof.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vuzcqupv.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qsrzltls.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2bnsivvqi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnxsqmqt.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2fmcoemeh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ekndzzzd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dracejlf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2atmlqugm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2epxjdjec.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2asivujye.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2wkgmlklj.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ypdnnhho.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ocqiioyq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2tjxozvrn.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2myrxrnrq.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2vmznoubs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gwvtqpfr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ifqhymtu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jzqepzls.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2xugwynbj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xldddzii.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xqnohbzk.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2adovykzu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2exwqinyn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2vdhnhttf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fqwznhiw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hzwiolqj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zxaagufw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2opyuufxk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2rceblqdg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2rohskfke.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2aqbfwuci.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2uhmfdefs.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2wlrehelc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aistzgxo.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2glcfxiru.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2oylewfph.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2gcityqga.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2aepozhxw.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2kxqqueto.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2jkhtrkey.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2dezemthp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ylftoift.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oqqiauil.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2smsvksxf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zyqxqgwj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qbtfbiyp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nxylphcm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bdrgewwv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2oalbgxjw.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2lfaqfryi.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2kbssfydh.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ukrvthcf.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wyxyblax.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yfpxuyaf.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zzzubpbt.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2spnhwpmv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vhyvnlcg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2udkuvnjs.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2gbmqdtas.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlirladg.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qfqrkbyu.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hvciiglu.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kqcqaiow.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2eslffufh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2jpixttjb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2wsshzbue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdrfehgd.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2iilbmsqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pelzdycp.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2sxxjltdh.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2lgvprlfu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zyyxuqoe.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rjxiuogj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bokhnxct.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewwnibgg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kagpaoir.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2osfduklo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lsbolfgk.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dnojetxg.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2dtctrbdx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ujzjsfwv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibaqutfo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sodqmfia.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2kaoaozri.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2dysqoftl.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2baimgsby.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2mlqbemqc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ncjlinuq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2swnkqxfi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2vnmgdoqp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vekfvwsa.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2wqkqqhns.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2flcfrush.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2jjvomrep.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2gamcwcwm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2osiwfewy.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2hdykhyhc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2kzwfsljd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2kjdwlvyp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2cqfptzzv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2dqhubang.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2dqvykwqb.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2qptgwiha.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ntjlxttm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ctjbmoqr.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2btoqxuuf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cicsbten.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2hvxfkqst.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2hzjugnph.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2eqqvedry.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2lizkyslh.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2wivkjzli.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2luxsbimi.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2rfcrbhtc.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2rmotjtns.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2qdjqanuc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2wiguqqtd.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bujmyhxn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hfgpjqgx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2pjkdocuy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2neuziiuy.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2nimtuqza.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xgofvgdv.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2xybylnuz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2hoyzheef.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rgygygiw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2mrmcqbwm.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2lvrsiyse.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2sdmstndg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2aotyuvdd.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2kpbwnazr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2mejqwvgt.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2mvtmzfha.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2pfkxrnjv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2nrbvgvxt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zhrsdemz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2knxkqgab.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2zggcxeln.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2cuskciao.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2dexdoqqc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wvmaksdd.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2bwozimgg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2pscqorke.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2kmoqzaun.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2hvmfkmex.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mjftzqrh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2aecrqmrh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2kiifjnue.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hqtipltl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2tohweddm.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2dwwioxll.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2kzczbigo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2bbzigiko.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ttclsaqa.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2xauvocyk.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rjnvgvav.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nhysctvn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2scwpsgfs.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pwmcnbig.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2xxzgfyve.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2xwkvbljz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2tjxharnp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2kjukexme.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2iiyptqvy.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2kjefwvhu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2sfvgxgyp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2vyssswgp.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2jfofjmvo.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2hrrvxfuq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2cdqqbjfa.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2zrwmnyyi.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2gysffeqg.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vzdcrgys.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2boadgjpa.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2gxnilvzs.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ihfyaeik.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2qxkndpei.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2qpkakotn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tjocithg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2quysgequ.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2drwthlou.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bwybrwem.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eefvmgzc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2kkekgzzp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2blvqfnks.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2waaybdtr.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2takxkvct.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2fvbzcrxo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2upzcdety.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nezuvgmb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2khpfsxts.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2abjnxnpt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ubbkezsr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2phtvqier.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2xglkdghd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2mbozepoc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2asvexxma.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2yvtelhcd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvsavfqf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eylifeql.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2nwpaigav.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2kdrijgzh.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2fhvujmqj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2karbqshy.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2irvlxdea.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2wfwgrvqk.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2vkqelinf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ifxwjjnf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2doivuhao.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2cyyjahqu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ahcoedkd.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2dgmfiksw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zjmecxso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2urbldgok.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2tdnffuzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fblnzxjv.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2mhwdxaup.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2niiknncf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cxprbaow.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2hetiwbuo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2vdmgdvow.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2yzkohwmr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2yeqhglhr.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fadymdwf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2qltwqynu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2kjfqwmii.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2exfhprlk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2niiwhzud.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wgzjznrh.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vidbjgon.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2avhiptbr.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wqbblolv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2lzvnoaet.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2qmmuvnny.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2vfvkuvlj.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2frxoryrg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2wssdcvcc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2fjcrkzgs.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rpqgbqhk.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2unysgfml.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2jttrjhdz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2qsymyyvv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eqdkhown.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2fqgqijhy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lqxpihyn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2glqteqst.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2xjnpxpqo.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2kquzuwis.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2lqiqydux.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2qyaldvia.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qvfpvfxo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2bauggded.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2oemwcqfm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2allbvmdh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2doyfkcpg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zraklrjv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ncqoyaby.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2tdfjcvpd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2aqnyxexd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fyoyqtpp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ohadomot.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2dehjcdnp.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xzcusrqt.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nzkqxasm.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2aaoyzyoz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2rgkywrsp.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2oxztsjgb.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2cohtfsff.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2bzhavegj.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2sdxuijsq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2zrvdnsrb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2scqvlbdu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hswrfyym.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yizqdvgc.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2uqvyoaan.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bubwzofl.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2wpiiilgz.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2tifnupxo.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2lhvqlnhm.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2wzdsouxt.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rlbhrjgb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2degnkulf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2dmwcgisu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2rqguvalo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xdydetrm.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2yhgnejvj.html


<!-- 参考信息 -->