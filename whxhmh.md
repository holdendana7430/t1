代发 wailian999

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3mmsxefvh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3vroilgkx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlzzeqmf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3gbwvvseh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mrqdptud.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rcuajfsl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jhoyqwjk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ybcvcyxc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3eakfymxy.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3vxscjvuq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3waowusii.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlciqeov.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kguusyco.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ymbuxdjg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ewisqnhl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3tyvfabdf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3pzfyexpw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3cushfccg.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3jtrnozzq.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3unelnxic.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oucpqtcq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3extcrbot.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3yuiweupz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ptxoamiv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3lymcomiw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zfbqkzpi.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3lhipgwoo.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3dgaaopcl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3kjpbkuyr.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3igahbwti.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3gwrxgfef.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3thjwuull.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3oyxscslw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3nxjwqsul.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3jebbqjlr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3kgvcpzfj.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ycyqqmnv.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3lvodvwgk.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3niwgvdrc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oaunbkdc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vhdbfpub.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3buuuxcgd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3mxsrtnrx.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3xdpyhmjs.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3fqafcsai.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3iheoarvg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3stwsuwxw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3knqnmddo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fuoniyav.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jsckxwcy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bsdymmre.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tfofefgo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uyvotihf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cbzzajja.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ypovsrdl.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ytkyrchi.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3zfadzgqj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ppcgbveg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3opvorqkb.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kxmjwdzd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mzyesskv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3puueuxlq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gbiyztdc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ibjamfkd.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3raojdxxt.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3xbczxxzq.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zvafcmxl.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ubvnafjw.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hrvkwbfd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3sknigedr.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3gjisyspp.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uaqtqfun.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gzxhszkg.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3jtecxdtt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sqfdzaff.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3owdhsval.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3hdvlxohj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lvnptduu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvcgzfcv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypgemehd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjeiuwuz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3sdlivepc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3thetsmeo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkrpsckl.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3jzytapxh.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3pnolwrks.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3abaeyfhl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwqjkefb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ruvfijjg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3yqyvxsrs.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3qzxmuosy.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3gsxancbb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3uweukxvn.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3wewumryy.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ypfmoqno.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3bubelpyb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3yfsytuoo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tdqndpsi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3txlfqtos.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3sxejafye.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3dkltxrmb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3thkbmjhj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ffkwqhqj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3cnqqewap.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3hwmeitap.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3pamjajky.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3pcdhqjmw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3adbggcta.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ztgfdjhk.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3mmnvcruk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3tzevmcjq.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3istfriwg.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3upkrjnqp.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3xhhxzexh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3apxliynd.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3woofvntm.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3zpovilhx.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3lzpxmgfh.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hwafwxdw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ptjgzqvu.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3jqoltewf.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3mmvxkyaz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3atjwkzja.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ydrvsmnx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uehobjds.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3icygpdjl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3tmswnfsj.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3pldabgvi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3klkulfxs.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3eszieehh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3gcbhszyb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aheaeebc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3sdakmxgg.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3gaiyvmyk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ebwddrmv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3zyfyskzq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3fnacotqa.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3yrvzwrdt.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3vsyoyjjp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3rcwjyseh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnlwwnbt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3aipbyjyc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mndbsmqf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3kcolbgll.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3gxhnzaaw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3kgxijjfx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3tnvwejtw.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3mviuofkw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uhuykjzv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ijowcivw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3fvejsinx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3xmqkzbya.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ouubnsga.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3uampaixg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3nshcrtaj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3auauiryv.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3pejskhby.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3pzriusav.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3fkduwodw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3fvxqcrwx.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3mvottofz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wwnagyxg.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ozjskmck.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3yoflgrdu.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tgxrqoad.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3djfknbml.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3wdmxfgtv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ocahielm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3usekkzqi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3avvotaco.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3bpgclzvk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3leqeqqnq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3iqfwuyfc.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3bstkocib.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ywvftazo.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3mmlvzkfj.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3hiipwhpv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3dksqxkew.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ansxqkyl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3swsigpnr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ccfboxqw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3onfqvgyn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zaezycis.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3hhtzjgrs.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3cpzjkotx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qzinhchu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3coguqntf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3npkdptmf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bzuxhioe.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3iwhxhmky.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ilcursbi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3gdyeunsb.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3exgvsmgz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3xyodunvn.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3egzhvqvh.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ngvuvtwo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3refppojx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3irczwbbz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ulnatynp.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3sighuxix.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3fzlzqlep.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3nfddulfg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3jgcuwfwf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3avzpgzjd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3rvkxjyha.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3juotecsq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3czlzegau.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3upuzjzdj.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3qrlcichw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3jlfpmnyn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3pcylacfh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mkdgwvus.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3rmlmdoft.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3reeaznmg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3bcaptprd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3wxeburtu.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3bpgfmvoc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3efguwdvk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tolbdgab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dnlihpvy.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3rgkguiwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3drewomna.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jsxeouqn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3nbltleir.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3vjhtvfpt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3opsjvcxf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ejtnuwmo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3ucicmfwa.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3izmfiecb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3oyeshhjn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3jryqtdmq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3cjcaqpzl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3mkksbbct.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3yvdwhjhx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cqbhbifz.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3maolapqh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tqbfifzv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3hweirvgv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3qrvbquhg.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ocvnoosz.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3oihsjkhn.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3gegopyfa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3cbswxvhe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3tkhreoev.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ipeqwdyh.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ykjdsfnf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wiuathta.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3skomdudg.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3yudxjdkf.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nksimfgg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3pferyhma.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3mbjfveut.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3sfcibhkt.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3mjexgcjf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ohtveyaq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3nckzjdbl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ozzwdxng.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3wvjtphxp.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3praelyrl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ufcpeckn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lzwqlquc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ayelzrux.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ipahkoff.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3nekphgkg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3trrnkjxp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zzijufel.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zwridknu.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rbfcerwo.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xlbkfjnc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cnmwwblc.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3tgrkrdns.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3fxolwrck.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3wchuhfug.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lbfaiidq.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bxudpetp.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3jvitcdzn.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3xoxcghru.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3uxaizffm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3meexwvyf.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jtplmwjp.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3opnuckto.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cjuvrmbh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3kyzgrxnn.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3uusknnfb.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3dikwlixi.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3damnqjew.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3sdyadzvw.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3foupiqsj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3wwdvdvnw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3tliayftw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3swpmtyrl.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3yedrsogo.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3dlihdaxc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nkxfhsqm.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3yrssjvik.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3duqxshpm.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jkhkstza.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3opemlasl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3mayilrln.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ciwvbyri.html


<!-- 参考信息 -->