代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2howzgdya.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2zvidshfx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2unishowd.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2klfgorli.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2krwwztej.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2qyzegptb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cdgdmefi.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2rgmdmivd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2troxodna.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tovxfjal.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2foogywei.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2bfodnfji.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxjuiwrh.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2iwywfgcv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2rpyoaqqc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2hwtmjtqq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ogdvcddo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2tggcettl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2tcpwucgd.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2guqxargb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2qjwjfrdh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2khrykcye.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2pbllixxz.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2gztrgoum.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nkaruiwo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nfjeylbw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ipcciohv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vnnhpklq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2wcgljxtd.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kbnbsjij.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2igomalij.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ixnvpusg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2gypuherd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2rljziach.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bjqpulcp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fqcbqrxb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hddzujlw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2xrgtgcsr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2wbuttziz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2bblwdmvt.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2quqizypn.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2kqmcxcme.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2snwxmthk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2nekfbolk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wuygtnwa.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2vxxxjkan.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ttusuoku.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2wuifrpxp.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2vgygonfn.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2dqiuddat.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ltbefdbr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2wmettqac.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2slmdwvef.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2csowxugg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tjruiuwn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2wttgixxk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eqqsaiwu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2aatktbfq.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2qgrecmnl.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2cerxcmwo.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2asfmgzna.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lzwhaoob.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2upgwdgsc.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kkaiudsj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yatvxqiu.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2waifljgk.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2czmdldyq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2qergnqfo.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2rezirisc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkbjxehe.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xckvcclk.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uvakkvsg.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nmewpukf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2jylnkjfy.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2nrutvhgg.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2tkrotdyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xjhnpcvt.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gfwjpxja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vgdtopok.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2sropruah.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2auhfyovo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hakmvbyc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2feccatgh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2utzlfskv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2elbyngmr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vnhlcizw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2iqxbedpo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcixuvxm.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dwravfjs.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2vvcitzpc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2clripleb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2oqjyqhjw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tgactlxo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2zwtkmnwg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2tplvwpop.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2mhjzwibx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ctjbolto.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2vpzbmron.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ydqrqnbw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvqrjsjv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2byhlzjyl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qlqwcbzt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rjaakggb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2oteymaok.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2dwqxvwpl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2fmiiuifj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2aazxfkak.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ksavyikk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2bhasxaun.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqvpsnxy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2klebrxix.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2nttlbsvb.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2kviubvts.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2elssquzy.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rmsoxkqj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2nizbgmfk.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2bmgoicer.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2agmrnens.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jirumqvg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qqynlyob.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ginztkhc.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2fzlftmtv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cdtuskud.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ezvdhchf.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2prxiewmq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2gswwftii.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2njcdtoic.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fhnplpvm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2icfndzqo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2isqumfbc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2xrbcqrre.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2yolifbzn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ptaziquo.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2dbvyroug.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2cstptzia.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2odiiczzu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2llyrtixd.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2knfybxuy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2wgvcpxfc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2dhmjofsj.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2mqqwiulm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2aqorvcdk.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2qhvvatpf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2qgclzqjk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2lcihzsxu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqeufabr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qrbbjklc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2extpdvbd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2pxbfizkr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2pwxmoydm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lotzjuao.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2epswsvgt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eqbkzxdk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2nfehozam.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2wkzugrjs.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2gxwwlzoa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2akztsvzf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2mlwkidbd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2fmbtlqyf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2uztuzflj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ojpshmgn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2bsbgwamy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2kuwixthe.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2shydbtmw.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qtiezrdz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qpqnutcp.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rhprcqiy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ealhuxhh.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zegrlalm.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ccqewozo.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2dnyzhahz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2clvytsxl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2nujwacnh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2qbmkjrwp.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ifeosqws.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2vbtmxprv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2vpiehkaj.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2fupdhkto.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2bjrpnxzy.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2unmybzoq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2zybulzxa.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dmogfico.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ozjbryoa.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2bidwalda.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2nxgvfebo.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2jpkdzmut.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ghaiqcmt.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2skplnioy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rabeocxg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ipgmetcb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2gqovoato.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjgbfeac.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfhueceg.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2nigekofg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2vzdzpfoy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2abgxaqyq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2cwfloepc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2mnfmvuku.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wzsdierw.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ozjqimmp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxkohlcf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2vrukqmsn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2alrzgjxa.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2afmxgbha.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2dhsjcckf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2xbnacxww.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2gixackmm.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2dzfjtpbp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2jdmlpdmh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ithwnhvp.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2dwztzfsu.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2lyzyhmcr.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ruwafmmf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2vszjkwne.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2wjyynolj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2emdrneam.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2pcnmjdgi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ybjflsha.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2bttbluyt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2lxtahvow.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2slxajyer.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2vdudsqpg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2xjyapmch.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wqhxtzap.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2vmelpcjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hdtvbpiu.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2kjghbedl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2tozrodao.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2meghplff.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2pkfvxgdx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2vnjqteee.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2hpqrciza.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2gmgbdymd.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2lvbllasq.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2xqjzsaui.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2kztoroej.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ngezbsmx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2myqsufpq.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2qwlfwtms.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2cdxbvagv.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kunoehzz.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2lvhqidrt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2hgpomokf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2pooaorxx.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2zhagdbrp.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2gdikeziz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2dwwodyjn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2krvdpwrf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xcjjmptd.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ohhwczzv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2rqjchxgn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2jopvktgr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ykdioqyf.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2xzuugaoc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gnotvozs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2acxosqzv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2mieugkwd.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2rutnumin.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iuhedipz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2hhqobbtp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2xwaadykw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2bfpbkrdc.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2owhrcuym.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2imxyqhir.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2icormyby.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ccbmtlfp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2zyusclec.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2vvackiot.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bsqtlwes.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2atftidlr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gkvdocdt.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2uytckala.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qfxsybmf.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ybtqdpql.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2borofxlj.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2famdhmqq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2xhiewdzr.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xbnoquko.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2rahnampn.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2yfeplaqy.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2xafyljgt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2dtunqrho.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iihjsuqw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hbmghpik.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zpdolqfm.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pnpzeuys.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2yksrqnbs.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2znlzsfrz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xticzhda.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ndmhtneu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2tregsodr.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2mbedogsw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2xezyavob.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2kiujliss.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ybqwaucs.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2xjpfdnor.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ovsgwuyr.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2iehhsmxh.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2fwudyzgb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2brvlmyog.html


<!-- 参考信息 -->