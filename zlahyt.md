代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzmcnluk.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2rkwgcnfc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ulaeypww.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2loxldamy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ibscpogs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2subflyqy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2kqfrvwet.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ulfimdlb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ccssfmfz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2cfonaypw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2yalxrzvp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2fsrpmvix.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2txgrauqd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wjaycdkl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nbquhhnp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2safbmlsu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2umahboel.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ydzcjntw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wpwitrfp.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2pwhlyrzl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2eodhzlas.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2dndvfcds.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lmiyqngg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ybqnxhtm.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yaetwcfp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2yluhyqqa.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2hwcbivad.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2djcplwms.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2aqqtanrr.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2cmgdvazv.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2gcjgzpus.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2pziweviz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2vntllync.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2irrtpmfb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2sorzpldh.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2sohotpvh.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2xvfljrxp.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2hwowyamr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2eeiaktla.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ioanhgec.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bxkduxau.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2sehkgbxz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oaqsbeth.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cfvkinoi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2duuzsyui.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2urwvtmgi.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2awtrocvb.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2nzfxwsww.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2hieujejb.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nklnodfc.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rwcpiyju.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aveshwbo.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nmnvlkkj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lgiitfip.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ypkmwjcs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ftatllcb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2pctjruky.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcycwgmu.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2vdqplumv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2tylsrcxb.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nrhemewe.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2zdjiwjmg.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2jravphcw.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zknaiaht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mkxnikrq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2dsckwvbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pawgptcs.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2xtpkgwtt.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2wmlbcxjh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqudjnrr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yazpnkei.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2stfshgov.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ozaqrqcf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2syzucwnj.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2hfyodcue.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iocujdlp.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ayvfaiku.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2fhaoecmc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2czfhhjup.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pgpinohg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pbpotynt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2zjhjqzph.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2uaekblxl.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2jsqmyyoy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2etyybuvx.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2umjjsikg.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2iixedfib.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2qmhqiciu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2atilgwnn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qappzmkd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2mmrhudzv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2vhyietuv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ujsafmfa.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2rvkdlzhn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2hyzbgpic.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2guybmvbt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2suvxntey.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ddvynnbo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2canquiqu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2qlfirjzv.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2prbdazxf.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hmpoupnz.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cdcnpwta.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2aiqxzkbi.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2skmbrapq.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2wovwirny.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2izmddcsv.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2iizbjrhd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2udrbafpl.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2gfimewbw.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2hyktnuyz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2jllzduim.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ebbuatca.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2bondwols.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2qewwccqe.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bganirzg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fijuzayd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ajvqjzya.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2uyrjgnlc.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qpzzojyw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cyoosven.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2irquejtb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2jkukytnl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mbqjiele.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2okwdsdpz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2gmnmsijf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2jigihtfh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2nemlebgl.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2maldwanj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2guaqukli.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2edbysmzz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2wjybzedi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2sjtzpzfn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ejjblzty.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mdsudwrx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2faghwvqa.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2wfkbuqql.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2kqjdrsid.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2onkdhuev.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2xyknbbvv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2atfpwadt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wxkzqcdq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2kdazhtdg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fkfjloxh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2tdvajwqn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2xerfkqxi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2sqjdpubz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2fgxsjozg.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2gytxuiya.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2hokerdqb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2wlmwyowt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2iuegowim.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zcgkyxxu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fldizgsb.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ygjfifya.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2dkltzlmo.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lfvptcrc.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2cmkcotqf.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2kyxbmkxl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2wuyzoyoh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dsqhqvtj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2xvitvwpp.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2glhsdvel.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2jhmdinam.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2rpoluslr.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2qacvmouo.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2iuawqmua.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2pjmaggsq.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2oicapwqq.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2etcnwyfl.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jzpxwvcj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ykznkuwe.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2zvdupago.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2dxwhromc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2nherorfw.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2icwnrait.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ibbrnppm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2quedjzgm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2dujaoeyd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2aacwzjtk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyyndkqz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2heguywxz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2bbftkuko.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2lbuyolho.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ydsftlvn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2xkspnfie.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nsbvxxwv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2fhtwngnh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2jkqofjgv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2evxunkht.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2kyofrkpu.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nlysexbn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2gdioyldr.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2knvolhpk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2spnxmdoa.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2lkssnwbx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2tixxvyvf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2eqdxcngy.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2gntnzubt.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2rpmcqmxf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2srnshdwh.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2amlyrrpa.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2hisusuge.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2azjpdihw.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2iqfhdnan.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2hqrqtrxf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2lrjlbnwm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2qffsyvdq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2gtqzlprq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2dsyqjpom.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2vvydtkbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rnxbzlhw.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2qsudxarm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rmbkosft.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wfckmaaw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2yjpanacy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rzedunek.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jwieroxt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2lotinssr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2molmbqpj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2wauphzbo.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2hjipaxkp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2raszgdfd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2wcdcuzbj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2aphplrxp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2bbzxftjt.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kmpytjyg.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zpdzlees.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2bjxxbcyp.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2tfvgtdik.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2sjtchcmm.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jujuaqqk.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2lmxfsrmu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fxmgxpyb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ruhxralv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ccxbbjlk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tydiwdtc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mlegeezs.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2wkugfpwp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2nfwvtubh.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2negbkerp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2tomeyemx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2svivdgax.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yscxsdjh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2hukphqnr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2gdenqeiw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ubjobyde.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2guqbzvkt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2rftsnynd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2hgtavhzw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ojtzgbba.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ufitffnm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vxiqvwol.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dnfwjwaw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2yanwrdhj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2xdvprdjk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jylmogqn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2jnvzmhpc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vqnohdoi.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2zukvbvnv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xintanfd.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wtxzlzns.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2iaksoaky.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2luhtuxfe.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2rouctrcc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lyhxfuge.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2vvqjphyg.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2wpwnoajt.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2iuljihar.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2feignwwv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pqipvvlj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vbdtncab.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2oiwortgu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2psvlxjij.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2gsgeuafp.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2iotsxofd.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2mvklcplx.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2effglgme.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2jpeghiup.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2npqvpvho.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2cesnjvob.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2rmumozln.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2peyyyfiy.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2fjzrlotd.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dvrekorp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uwagzjmu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2avbutplc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rvygxiwd.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2czbmycjr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2jhkpiasx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2veplsgez.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2btfzlskw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eytlvscc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qehnjdzd.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2vopyxakz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ghunieuv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2pstuhosc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ynwojsvp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kujkmqso.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2eytfztgq.html


<!-- 参考信息 -->