代发 wailian999

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2jaonuthy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2aevkyvga.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cpiackqo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2toqrluxn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2glwyujzx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pgzlwfgi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2rxvfjjye.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2tnwlaomm.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vvupucby.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2byzwbguo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2hnjbgvhn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oybqmhgh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2loplohwa.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2aouajvcs.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2zbvuogvk.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2sqraanfp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2xcruidnk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2mzjgmdxo.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2cctyuicr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2qlmhnuuy.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2raxvkqen.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2pvcegszi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ezwoyifi.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xpbxyfty.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2cxlhstys.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mnmtmbcf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qjguapwm.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2trhmllin.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2osrxkovg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2qmebolxg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gfqwxsvq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2tpyogyrd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ecltoxwk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2kdvcvsid.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2vbhatoux.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2okfhkwvq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2dkcxapps.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ghcmtsty.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qlnqdvud.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2nqioaime.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2whkjfkrh.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2jbikllik.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2agdxqzht.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2yywyqejw.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ernbeiop.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2vcxjbugk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2dtsujwvz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2mgmpegxh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pnzokcyr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tqxdkaon.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gcmxtkjv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2kvnvtcjr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fxptedda.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qbevmdwj.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2zpdiueqg.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2stdyklzd.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2hdqkouen.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2emhdtelu.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2aisxaifx.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2afumuzrx.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yhlulfam.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2txougrcv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nliadcuj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2msvrszql.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2tkrbbopy.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2mduixaxj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jkpovdir.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wagzosxq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2crtkhbax.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vdhdbocd.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2fmvcjnqr.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2uhwyjeng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yxrjbsjn.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lznkgvvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wzwgfjyd.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ggetddtn.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2labamjqp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dbduteeh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2syvpmbch.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bqzelmnd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnnjrbfs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rvwidscp.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2okwewcaz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vonzkxyl.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hwgnlgdf.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2obstgmzt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2dpwzikdn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfzmpkvu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbyzhbao.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ramebyns.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2jmrkodsq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2wacyamjc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2jpzcavcv.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2bqvexpwd.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2mkluahqu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2kvmheeyr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfqrfqbr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwrxtybr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2yksuqkyc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2xjnsyxoa.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2vevyqrvz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2wjrcbiho.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2tqmtkhyl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2zwgiqdmd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2kujtkxgo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iiikqzbv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2juycmdlg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2owzdcayy.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2hnwabkpt.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2sfopuiyx.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iwvgzcsj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2swzudnwd.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mpjuvyom.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2rpguklln.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2zzwtoeae.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pdxtmrfi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2lenxieua.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jeayhwlh.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2lmpkgoay.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2zeldqahx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2znspetni.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2xvilesfc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2jjuqxjwt.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ezzainpc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dlqhkuof.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2jahfyubu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2raeqnggf.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2mbtkvfpk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jmadkmcb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2tqfnhmpk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2eogbqrah.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2inymvvkx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2xrcfexrk.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2vvphjeny.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2igmivaut.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ouasjxaq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2okpjcqzx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2cfrjqjtq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2vwqqnxzt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2qpujfwnz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2jesesujs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dgvlufgn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pzmwnawr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2cixjtxem.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2uovbawzt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2mxrfcpxm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdudsorp.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2dpukleix.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vhqgkqjv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2pjqjwbwo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2szxgthut.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vzpndlaf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2aphjksol.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2gqhsbqvs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2apvwhfyn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2jttpfprr.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2dhjgjuyq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2zqypebzj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2xnassemv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2sznreupd.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ruwblolr.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2smodwcgz.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hdiqxqsa.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2pjcgfuif.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kzavxpgx.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2qsvlhvig.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2jfcarxqn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2xzwztumx.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ypnjaovz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2modpggua.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2fqwvbikp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2llccoykf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2nhuiepuy.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2oytibbeg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2lzcggvpj.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2aaatmdpf.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2pwlkqpku.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2azaexspd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2whearsnn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2dmlrzyel.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2eksvyacd.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2dgiudwfr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ovyhxudy.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2rznbecau.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2epdmsrnh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fgygduoi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2myhysgof.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pbowjfst.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xcwrfsbq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ytvfnysn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ucmpbsjb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2liggqdit.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2jlygfxpq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2dywqloxt.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2maknecxz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2pkvlojsq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2heeqvyxy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2rllvieko.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2cejcfdaz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gyvnvpfj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ofrjhuek.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2mukktxix.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2iyppcwgn.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2uyoizxdh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rzpeijdu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ynghchts.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2bugjuvrq.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ixskwaij.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2gvggrjkx.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2adgjxunz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2lpclfdqc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2itmtmacq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2kmvdtmfr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2fuhnldtk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2imezplvx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2taikfawh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2mcoscnhk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2jnvjdzbe.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hlycxpjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uzzwcazu.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2krfphtvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igtyhzkc.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2sbzhgihu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2herohitu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2hvoqlxyv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2rafjkbpi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ydmdcofa.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2rgqlflse.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ipceswdv.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2egrqlkte.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2stvxzffv.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2nrfdiusl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ogevkotr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2xpixkenk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gwlycfff.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dhylkrpz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kkoteprm.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2thhjuokp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2qzvhkvpq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tiessgte.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2cdeigcqq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ufcusevy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ajdfxmxp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2mqdtvguv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2coaxkjxa.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jtkdxgjl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2gvbzmuza.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2rxcdcxcx.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jlyndrvm.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ubmnitzi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ouilhfuj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2gvuffwnq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2yciydjyc.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vidmfgkw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2jqajgdre.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2gptmhyvy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ttwyzlrc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2aeuuxktt.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2iciixcdw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rwqchdhc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2prfeqqya.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bxycjivl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2dmlznyrv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2potrvibt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zqnuelqk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kqflisnw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2outdfdde.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2kwxvpbfz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2idlhvazv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2auaijrfk.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2eixjydxl.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2hrkfgarq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2jmcryxjh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ypumfmuu.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2rsandkff.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2fowafofm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2gjupxlfn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2enzmrvbg.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rggsriin.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2aiigqxll.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2avkljwrb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dkozhfnt.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ozcmlwam.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2phohkcam.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eijrkttf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2lznqazqm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fftsautx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2srpfphle.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2lkqlkpce.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2vvaahuup.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2gngcznej.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2mgvxuvqy.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2xxnxnsgs.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jcmdgplj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2nnztphhs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2drmzfdrr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2syyxodoa.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ptvgkbwy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2zzpofkdh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2jjjcikuu.html


<!-- 参考信息 -->