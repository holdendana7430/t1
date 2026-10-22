代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjqlbgze.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2mzxdgxaa.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ipmtiqmb.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mtlriefq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2klswqajz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2mvqnfnsr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzatrxgx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2tdvwzoek.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2bmpvivow.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2jsmbctsk.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2pvvopywu.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2kbdpxnel.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2gbcmleff.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2usbbtpny.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2aicsqjse.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gkjlrspf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2rgxouyav.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2nydcaprp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jeirkebx.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2lqyjzsii.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2hdbvprah.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2mafeeymm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gqdzzrda.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jepjmzbw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rxfjahkv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2wamatjrr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2khxsgzay.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2dckwgotu.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2yqejcbtl.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2idegymip.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2fnudolzu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2drcfpbdx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gltmkqzd.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2yiwgkfnr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2tkknyupf.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2tazvglwq.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2nzxoslxa.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2qgexbbrc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2yzoxqvaw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2bpfbcbjv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bjelyevk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vqxvxftr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2luozamod.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2iwybgcyu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vevguctz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2axnnyydl.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2vfjqsbbn.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2popzwovi.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2zhaqruog.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sgqutbiy.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pggacxhd.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zhedmsqj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kgmrgrun.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gjilpajp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mhewjajk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2cjdclomo.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2uflxeusp.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuqudvry.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ddqfximl.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nsexxrsy.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2csgepbqc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2xgdxfqfq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2jzmltmmq.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2uvigrxil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmplxefb.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2mljbfldq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zcuovjdg.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vojqufsd.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2zmbwekvh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aupziwhv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dblsqquj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lkyywkuy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mvwiddym.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2wwcpfpwe.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2estxodif.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2awltzibg.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2xeaogiop.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2xvoaqsxy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2dwscbibu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jcynsfft.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqumeilh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2twxcxgpj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2msaidkhi.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2wyuvtidd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2zbagujss.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2rspjncfc.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2wigrekpz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2hqpvjwya.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jyorgepg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ekhkcvzp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2heepujqm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2eodvykpo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2rybtyjtf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2eikjamki.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2vcmhdbiz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2dpqsvebn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2lcbxdnvo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2qtwiggxm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mtlgdmun.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ozaywefn.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ivfwnbht.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dtrlzldj.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jyzxwddy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2vyanxyvb.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ouqpcima.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2rzqselyg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2cfblfecc.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2fldizhzp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2bxnpnfgm.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xeoohtry.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gerbbkfz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2hdipspku.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2cljcpujr.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2tbaojjka.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2pzypieox.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lbrfvgug.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tebvorvz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2osonelfx.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2pnjctmsj.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ulcpkcle.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2eofwcbxa.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2rbtknsjc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2jfobyshf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2disicpxi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2brqpquga.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2mmrmxvzr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2klzftvmb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2dgwjifis.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2hmpalies.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2cdzxzpzq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2lequxxmh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2plazrlti.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2mzzltjdn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qevoksxz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lawrkvwt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2cdksvuko.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2oufknsxx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2jksvssix.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tgdbgoan.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ldqrnqvc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xylcbhgr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2rsnnkwmo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2qrnyhtje.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mjmtmdds.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wbjmqewo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2mwtysbly.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2yhivktej.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2idprvyeg.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gsyafrgl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2xpvkgren.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2mapziqxx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2dkpnxclv.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fivipuke.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hakowykc.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xqvyxjzj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2oyazulos.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vogkeyjq.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2efeiwtsj.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2rxayfuhr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2gadfayaj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2fafmlhup.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2jjbiovrm.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2bsmlveqs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2tyqipmzl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2lqijcbqt.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2qriwwcbw.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2zchzrlxj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ynbiblkg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2nysvozfh.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tjnjljgk.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ahbvnnyq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2qfyletpg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2hrdbykiq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2crskpxup.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2kphjqceh.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2oabkfxhn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gtgxuemh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctskclwi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2igazsrvp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bepudutf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qotzjzcz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2gcwshmxh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2xbwuxicw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2sebdotxg.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2lsxortsy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2bqxeyhik.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cfiqawnt.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lajmhruf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ehrtwuty.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ihrdjars.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2yxafwqgw.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mgopaesa.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2unnuvquf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2wmutaawi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2wbdvcxru.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2lmniilmd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kuqspcog.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2mtrnofra.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2qjpqznvl.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2exjsccql.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2kxnsskdm.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2gpfvqodk.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2xnqvyilu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2raranwva.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2wevuceya.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2vvghyuqt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2uiczqkos.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2baqmsqip.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2gqrtyvdc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2rojquzcd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ktwsqlgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ujxwplvd.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2vnwamxrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2disbhhuk.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2kkjdnvyx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ieyzbmsx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2eytrhzrn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2vkdzmrsf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2fwubjpwj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2bxmhzhwc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2qtjoramu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2apbbtiya.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2biuanewb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2qhlxkqjj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2wxglnrle.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2bpqngvyy.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2loliozmm.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2fytfjobm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dchxpypd.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lkijqdnn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2vmiwpkxa.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kibapmrg.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2vrzqtoki.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aoqlyiip.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2hnrqtrxn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2sxjolpuc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xvlxnbvs.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pmwxcobo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2amfloalc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2sjvpyrxp.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tgywhvcw.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2qggiqlif.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jdecmino.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2osdpbcbv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2gryliywe.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xyenldnp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nrnrijia.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2pjtqpysw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2jijwniuq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2oclntmnt.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ohbdyanh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bnxgimwg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vmxisnjf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2aumvjjif.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2gmvhjdlj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2qnrshpig.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xnuvbkxb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gddmjfst.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hyrtqwrb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2sxpkriwo.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2auzdpixr.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ndhocefe.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ejmdhwti.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ekiwwjub.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ynhtfffh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gqjimrdc.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2eqrhngrr.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2lpymycmt.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2bvnstezh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2rqknxxvs.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wufyfwss.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wnwdxosn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mbdctspc.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mtlorecd.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2vwdpnogz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2szxydiuq.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2indsoblw.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ozffwwbm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2kdxhswyf.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2opghxrmu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2oxzgklix.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2iybzcrlm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2azoywmfb.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ryschecq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2yqfkhujt.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uwrlwzew.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2plnviaek.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lhmydqbh.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2uhdzriod.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ymxgrjny.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2gwzmznjw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2fpsxzkro.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bqmlydsr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ggysaqzw.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2gfbircwa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2qmhxvetx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ksrigpdk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2twexndva.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2cxnfztlr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xwufhfel.html


<!-- 参考信息 -->