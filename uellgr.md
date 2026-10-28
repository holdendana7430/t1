代发 wailian999

[B09] break 与 continue
来源：http://hz.havefunace.top/gtcogajial.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.birdmap.top/gtojcklzqz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.zhijiandao.cn/gtgeoypebq.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.sweek.top/gtghtasyyd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.havefunace.top/gtacezwykd.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.tanke756.top/gtscqjhijp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.cashguo.top/gtuwdyydhp.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.yuxming.cn/gtaugklejz.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.cheryme.top/gtmjdavfly.html

[B10] 遍历同时拿索引
来源：http://hz.smart0.xyz/gtzylzghjf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.jinghuilouyu.cn/gtbmodvwtj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.shangyingyoupin.top/gtvwsdvijo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.hfpthk.cn/gthkdeszlp.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.meibo888.top/gtorrlmoli.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.yongpay.top/gtlehhjhxe.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.hysaishi.cn/gtsmmfotkb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.sweek.top/gtzvunfgkb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.hnqzz.top/gttyofwtoz.html

[B11] 生成数字序列 / 区间
来源：http://hz.shanyushiyangtech.top/gttdivgqhl.html

Py:   list(range(0, 10, 2))
来源：http://hz.316326.xyz/gtvfbrabhj.html

PHP:  range(0, 10, 2);
来源：http://hz.shanyushiyangkeji.top/gtixzxvxbs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.fengsongda.top/gtkgarcepc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.dashuyun.cn/gtcwbpnafh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.redwolf501.top/gtbghtxsuq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zhengqikj.top/gtclwbniqi.html

Ruby: (0...10).step(2).to_a
来源：http://hz.hnqzz.top/gthggekefu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.guannengcc.top/gtyalxvlum.html

[B12] 跳出多层循环
来源：http://hz.hywenlv.cn/gtszggwvrs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zhongyouzk.top/gtxewrkylk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhoulong.xyz/gtrpluwcch.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yonumen.top/gtwfohyvxc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.9152youxi.cn/gtnghwvsct.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.cashguo.top/gtdbpdvpef.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.xylfe.cn/gtovasmbzv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.quarkkingdee.top/gtclljartf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.kuanghao11.cn/gtqqyxrqpy.html

[B13] 判断是否为数字
来源：http://hz.zycfv.cn/gtaetpmcuz.html

Py:   isinstance(x, (int, float))
来源：http://hz.vqdsnc.cn/gtyqzwflnp.html

PHP:  is_numeric($x)
来源：http://hz.ydzc1.top/gthgkcjunt.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.gzhubu.top/gtvgqnqzny.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.wangshuangyany.cn/gtvokofomw.html

Java: x instanceof Number
来源：http://hz.xingfuxueyuan.xyz/gtzhcxfxnk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.hnxiangtu.top/gtefcejpka.html

Ruby: x.is_a?(Numeric)
来源：http://hz.jqgufenzy.top/gtrhseazkx.html

C#:   x is int or double or decimal
来源：http://hz.wangshuangyany.cn/gtoefbjfbu.html

[B14] 判断值是否在集合内
来源：http://hz.yj202588.top/gtniletrzf.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jianghu66.top/gtwvoxklyt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.hnxiangtu.top/gtksdogvrj.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.316326.xyz/gtawoeogxc.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.tianlin.xyz/gtbqtzikwt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yj20258.top/gtjgwpdzfv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.hysaishi.cn/gtuigaxatb.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xingfuxueyuan.xyz/gtuejqrmda.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.shzxlz.cn/gtmsizzhtr.html

[B15] 布尔运算与取反
来源：http://hz.zhoulong.xyz/gtzpnqdxgg.html

Py:   a and b or not c
来源：http://hz.zhixingplan.top/gtyvbqonce.html

PHP:  $a && $b || !$c
来源：http://hz.ivvv.top/gtmrgtytwh.html

JS:   a && b || !c
来源：http://hz.zhoulong.xyz/gtzkewwfgu.html

TS:   a && b || !c
来源：http://hz.pycfn.com/gtotmxchgj.html

Java: a && b || !c
来源：http://hz.guannengcc.top/gthwejkfhn.html

Go:   a && b || !c
来源：http://hz.yueranfly.top/gtchbsvvek.html

Ruby: a && b || !c
来源：http://hz.jlsjyb.cn/gtegxtyzfe.html

C#:   a && b || !c
来源：http://hz.birdmap.top/gtrlvpftry.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ybcxt.top/gtymfcnnff.html

Py:   if not data: return
来源：http://hz.yuanzhike.top/gtalakiajo.html

PHP:  if (!$data) { return; }
来源：http://hz.tian-w.cn/gttomvqwor.html

JS:   if (!data) return;
来源：http://hz.meibo888.top/gtjompxjuq.html

TS:   if (!data) return;
来源：http://hz.yj20258.top/gtnjuejyab.html

Java: if (data == null) return;
来源：http://hz.gotoacloud.top/gtsetvcjim.html

Go:   if data == nil { return }
来源：http://hz.aibaodan.cn/gtwqskhmwv.html

Ruby: return if data.nil?
来源：http://hz.jinqigfzy.top/gtxhmknwds.html

C#:   if (data == null) return;
来源：http://hz.jqgufenzy.top/gtkxsyegwt.html

================================================================================
来源：http://hz.guannengcc.top/gtiemssqwy.html

C. 函数与作用域
来源：http://hz.gotoacloud.top/gttzqyycpx.html

================================================================================
来源：http://hz.316326.xyz/gtxccbazrt.html

[C01] 定义函数
来源：http://hz.andypj.xyz/gtberwwnvl.html

Py:   def add(a, b): return a + b
来源：http://hz.ydzc1.top/gttcpvieka.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cucudq.cn/gtodpchswi.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.xylfe.cn/gtbstshosv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.quarkkingdee.top/gtakdvdsxb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.zhiwuduotai.top/gtygcewvfc.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhoulong.xyz/gtzxtnkdqv.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jiagoushi.top/gtundtysmh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zhaomingkeji.xyz/gtyuntgltc.html

[C02] 默认参数
来源：http://hz.zycfv.cn/gtdjucmbmw.html

Py:   def greet(name="World"): return name
来源：http://hz.wangshuangyany.cn/gtrlbflonf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.ydzc1.top/gtpscbclyo.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.cucudq.cn/gtkenvdfeo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jinyuanbaomall.cn/gtxivecolh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.sysykeji.top/gtenvmxrsz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.quarkkingdee.top/gtjkhrmgim.html

Ruby: def greet(name = "World") = name
来源：http://hz.shzxlz.cn/gtiydiuygc.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.vqdsnc.cn/gtgnhefhgf.html

[C03] 可变参数
来源：http://hz.cheryme.top/gtyscbfuwt.html

Py:   def total(*args): return sum(args)
来源：http://hz.aizwys.cn/gtqyvowgyp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yuxming.cn/gtudsuvece.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.andypj.xyz/gtifkjvmxv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.quarkkingdee.top/gtdahyhmib.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.meibo888.top/gtyokulypm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.gzhubu.top/gtxmndzrtj.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.kuanghao11.cn/gtxpfkvsqs.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xuanzx.com/gtfzchhcez.html

[C04] 命名参数 / 关键字参数
来源：http://hz.chenlongwang.top/gtwivyjces.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.guannengcc.top/gtgzagmosb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.feifeiyinyue.top/gtscmbvqvl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.gaohongyu789.top/gtwfraodos.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.gzhubu.top/gtcqelvbnd.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.feifeiyinyue.top/gtxshwwbps.html

Go:   // 无：用配置结构体参数
来源：http://hz.yj20258.top/gtxzpedlfv.html

Ruby: f(a: 1, b: 2)
来源：http://hz.bjfxy.top/gtpjtcreon.html

C#:   f(a: 1, b: 2)
来源：http://hz.iojbl.cn/gtjlsffxwd.html

[C05] 返回多个值
来源：http://hz.ivvv.top/gtyicxawep.html

Py:   return a, b
来源：http://hz.jiagoushi.top/gtpobkqkdm.html

PHP:  return [$a, $b];
来源：http://hz.zhijiandao.cn/gtqnbrtdpb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jqgfzy.top/gtpbamkocu.html

TS:   return { a, b };
来源：http://hz.jyoumei.cn/gttxhqtjpi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.vqdsnc.cn/gtkxlighzv.html

Go:   return a, b
来源：http://hz.quarkkingdee.top/gtdfivhcdj.html

Ruby: return a, b
来源：http://hz.ivvv.top/gtchdftqcl.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.gaohongyu789.top/gtzxeorjan.html

[C06] 匿名函数 / lambda
来源：http://hz.cucudq.cn/gtmlnvwnab.html

Py:   square = lambda x: x * x
来源：http://hz.cashguo.top/gtdmdgxozj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.hysaishi.cn/gtioowrlvj.html

JS:   const square = x => x * x;
来源：http://hz.jinqigufen.top/gtjpdjzfkn.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.c1oappe.top/gtphpgrmry.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.guowangkeji.top/gtocfqoivf.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.jianghu66.top/gtmhudbhsh.html

Ruby: square = ->(x) { x * x }
来源：http://hz.316326.xyz/gtdeaaqknm.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.mhx1999.top/gtjsbkycon.html

[C07] 把函数作为参数传入
来源：http://hz.feifeiyinyue.top/gtiywiltfv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.sxryk.cn/gtgmnvcuzb.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.xziqi.cn/gtiluqnmhu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.wangdashe.top/gtwghilqoi.html

TS:   arr.map(String)
来源：http://hz.hnxiangtu.top/gtmowmdgwm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.52xcode.cn/gtbktoydck.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.9152youxi.cn/gtarzhgzvo.html

Ruby: arr.map(&:upcase)
来源：http://hz.yj20258888.top/gtwzluojue.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ivvv.top/gtxupjkfsd.html

[C08] 闭包
来源：http://hz.kuanghao11.cn/gtekedcpve.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.haohaochexian.top/gtnwtazpuj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yanxiufei.cn/gtnklunigw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cheryme.top/gtqelmjpms.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.yuanzhike.top/gtmhmuyimp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhoulong.xyz/gthosmpobg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.vqdsnc.cn/gtntbydbcg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ydjk.org.cn/gtchyxepgt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jqgufenzy.top/gtpglobexg.html

[C09] 递归
来源：http://hz.9152youxi.cn/gtyjyufapl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.yuanzhike.top/gtjfvvdjxy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.xylfe.cn/gtpvwbzspa.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ppjwa.cn/gtubonjctd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gaohongyu789.top/gtjhzrzewn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.dashuyun.cn/gtxiwolaud.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.haohaochexian.top/gtgarhdxxp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.hysaishi.cn/gtsqlvkjih.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hammf.cn/gtpkxlgjch.html

[C10] 变量作用域
来源：http://hz.xuetiantiany.cn/gtbqxiiwot.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.yanxiufei.cn/gtdxmljfnc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.andypj.xyz/gtstxmaokm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shzxlz.cn/gtvpqxgrok.html

TS:   同 JS
来源：http://hz.nanxinkj.top/gtzypzgaex.html

Java: 方法内为块级作用域
来源：http://hz.pengpengdd.cyou/gtwkwqoqtw.html

Go:   花括号块级作用域
来源：http://hz.yj202588.top/gtxmnkezxj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.redwolf501.top/gtzqpjacji.html

C#:   块级作用域
来源：http://hz.yuxming.cn/gtcmtktugl.html

[C11] 模块导入与导出
来源：http://hz.gotoacloud.top/gtmpdjizvq.html

Py:   from module import func
来源：http://hz.bjfxy.top/gtsohltvmv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.tianlin.xyz/gtznbabelf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.0kj1m.cn/gtoushznrw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.gotoacloud.top/gtegcvovfn.html

Java: import java.util.List;
来源：http://hz.gogol.net.cn/gtkrhgphxd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yongpay.top/gtolennqgz.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.wangdashe.top/gtxkjgitso.html

C#:   using System.Text;
来源：http://hz.yj202588.top/gtysmynzjm.html

[C12] 立即执行函数 IIFE
来源：http://hz.cashguo.top/gtyuynpywf.html

Py:   (lambda: print("run"))()
来源：http://hz.andypj.xyz/gtqocwlvne.html

PHP:  (function () { echo "run"; })();
来源：http://hz.birdmap.top/gtqoeyczgs.html

JS:   (() => { console.log("run"); })();
来源：http://hz.sysykeji.top/gttavauupm.html

TS:   (() => { console.log("run"); })();
来源：http://hz.fzhhl.top/gtakknvugt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yonumen.top/gtbrancotl.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ydzc1.top/gtehdlllnb.html

Ruby: -> { puts "run" }.call
来源：http://hz.aibaodan.cn/gtqbebvbgm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ivvv.top/gtzzvihvxt.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhongyouzk.top/gtxgmlyled.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.aibaodan.cn/gtufyixoiy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jlsjyb.cn/gtwzyxnuns.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yj20258.top/gtadhedsuh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sxryk.cn/gtkinvpufj.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hongshengwenyu.top/gtuorfkeiv.html

Go:   func add(a, b int) int
来源：http://hz.9152youxi.cn/gtfdmutxqo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.shanyushiyangkeji.top/gtplkiuayb.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.wangshuangyany.cn/gtdcntaaud.html

[C14] 泛型函数
来源：http://hz.chenzaomai.com/gtecpeuezr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhongyouzk.top/gtstdtfzme.html

PHP:  // 无泛型
来源：http://hz.pycfn.com/gtxivqezko.html

JS:   // 无泛型
来源：http://hz.bjfxy.top/gtooznumcf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shanyushiyangtech.top/gttjdkjnry.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.sxryk.cn/gtxxirsins.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhoulong.xyz/gteinoeyth.html

Ruby: # 无泛型
来源：http://hz.jinqigufen.top/gtcrrffigq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jyoumei.cn/gtrfmevyef.html

[C15] 解构 / 展开参数
来源：http://hz.nwbrower.top/gtfgebavuc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.gaohongyu789.top/gthgmzesem.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jinghuilouyu.cn/gtduuvkovy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.zdqjudy.top/gtsduybmst.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hfpthk.cn/gtiqyfezod.html

Java: // 无解构
来源：http://hz.havefunace.top/gtsnoynzsa.html

Go:   // 无解构
来源：http://hz.ydzc1.top/gtpaeuvozn.html

Ruby: a, b = pair
来源：http://hz.nwbrower.top/gtofihdzvx.html

C#:   var (a, b) = pair;
来源：http://hz.yonumen.top/gtxpgwqtib.html

[C16] 函数 / 方法重载
来源：http://hz.ehwqpu.com/gtaywcnhki.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.chenjidiqi.icu/gttaprpzhm.html

PHP:  // 无重载
来源：http://hz.yvedp.cn/gtsohiaeho.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.pengpengdd.cyou/gtmwqwmqdi.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ivvv.top/gtyixcwzdg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.gzhubu.top/gtsckmmlmj.html

Go:   // 无重载：用不同函数名
来源：http://hz.guowangkeji.top/gtxlxhnlrk.html

Ruby: # 无重载：靠动态参数
来源：http://hz.cashguo.top/gtworlhyvu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhoulong.xyz/gtktbmpvru.html

================================================================================
来源：http://hz.pycfn.com/gtazmpnkir.html

D. 数组 / 列表 / 集合
来源：http://hz.c1oappe.top/gtqvozktzp.html

================================================================================
来源：http://hz.aizwys.cn/gtzfwmvblo.html

[D01] 创建数组 / 列表
来源：http://hz.gaohongyu789.top/gtswxkavpa.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.meibo888.top/gtstdmbnka.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xingfuxueyuan.xyz/gtevybiqbt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jiagoushi.top/gtetlkgyyj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zdqjudy.top/gttjeolwqy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.cheryme.top/gtdjdyoxhm.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.fengsongda.top/gtkjzjnjud.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shangyingyoupin.top/gtdsfizswa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jqgfzy.top/gtlavtqulm.html

[D02] 追加元素到末尾
来源：http://hz.ywan-chungtsiang.top/gtvwfbkrro.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.wangshuangyany.cn/gtvtuvwvye.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yj20258888.top/gtvnngrbbh.html

JS:   arr.push(4);
来源：http://hz.chenlongwang.top/gtktptxqmb.html

TS:   arr.push(4);
来源：http://hz.xingfuxueyuan.xyz/gtmpmudghb.html

Java: list.add(4);
来源：http://hz.zhiwuduotai.top/gtmyslirue.html

Go:   arr = append(arr, 4)
来源：http://hz.sweek.top/gtmjodowrj.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.shzxlz.cn/gtmxycgxdw.html

C#:   list.Add(4);
来源：http://hz.jinghuilouyu.cn/gtfuudmhcl.html

[D03] 在指定位置插入元素
来源：http://hz.guannengcc.top/gtxfvmngru.html

Py:   arr.insert(0, 0)
来源：http://hz.hongshengwenyu.top/gtbhhmtwqr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.havefunace.top/gtxvnaxrrh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ywan-chungtsiang.top/gtlesiygvn.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.sufxvd.cn/gtquvjwfvh.html

Java: list.add(0, 0);
来源：http://hz.mhx1999.top/gtcwprezlc.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xingfuxueyuan.xyz/gtbfbrvmxs.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.pycfn.com/gtemgpdiag.html

C#:   list.Insert(0, 0);
来源：http://hz.wangshuangyany.cn/gtoxkzjhrc.html

[D04] 删除元素
来源：http://hz.gogol.net.cn/gtwqiaufcn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.aizwys.cn/gtfyprptab.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.redwolf501.top/gtrodqmiou.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jiagoushi.top/gtwcjqjlfr.html

TS:   arr.splice(0, 1);
来源：http://hz.guowangkeji.top/gtrzmjccyp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hnxiangtu.top/gtnmccwtwh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.bjfxy.top/gtlzxhmmwg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhijiandao.cn/gtajfurycb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ivvv.top/gtdpohelcg.html

[D05] 访问与修改元素
来源：http://hz.ppjwa.cn/gtqmpjyqmz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hfpthk.cn/gttevrvcfn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.shuidangran.top/gtmzxghtqh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jinghuilouyu.cn/gttiygxtpt.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zdqjudy.top/gtfcqdstqj.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ppjwa.cn/gtyrmekcbc.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.sysykeji.top/gtvyticnrl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhongyouzk.top/gtdsxqhyck.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinghuilouyu.cn/gtjtesjwpo.html

[D06] 数组长度
来源：http://hz.yonumen.top/gtvqhqfwej.html

Py:   len(arr)
来源：http://hz.nwbrower.top/gtyyjittvw.html

PHP:  count($arr);
来源：http://hz.bjfxy.top/gtlahpjhlu.html

JS:   arr.length
来源：http://hz.jinqigfzy.top/gteodskegv.html

TS:   arr.length
来源：http://hz.gogol.net.cn/gtztnrohdi.html

Java: list.size();
来源：http://hz.fzhhl.top/gtrjyfstwt.html

Go:   len(arr)
来源：http://hz.birdmap.top/gtzujkzjtv.html

Ruby: arr.length; arr.size
来源：http://hz.yongpay.top/gtgsqkanfm.html

C#:   list.Count;
来源：http://hz.haohaochexian.top/gtdmdtuejj.html

[D07] 切片 / 取子数组
来源：http://hz.andypj.xyz/gtijvjmuuk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jinghuilouyu.cn/gtnwrvhvhm.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.gzhubu.top/gtpoyrjeru.html

JS:   arr.slice(1, 4);
来源：http://hz.shzxlz.cn/gtulftwxim.html

TS:   arr.slice(1, 4);
来源：http://hz.hnqzz.top/gtotlvzcct.html

Java: list.subList(1, 4);
来源：http://hz.pycfn.com/gtadwvntwd.html

Go:   arr[1:4]
来源：http://hz.jinghuilouyu.cn/gtdplhiwor.html

Ruby: arr[1, 3]
来源：http://hz.cdnleiting.top/gtmscwrgul.html

C#:   list.GetRange(1, 3);
来源：http://hz.jqgufenzy.top/gtwqtquwmj.html

[D08] 合并两个数组
来源：http://hz.yj20258888.top/gtcrhhfbcn.html

Py:   a + b;  a.extend(b)
来源：http://hz.fengsongda.top/gttvqezgan.html

PHP:  array_merge($a, $b);
来源：http://hz.pengpengdd.cyou/gtnbfjpmum.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jinghuilouyu.cn/gtnghbyjho.html

TS:   [...a, ...b];
来源：http://hz.jiagoushi.top/gtaxncmvwk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shanyushiyangkeji.top/gtihpmfbvh.html

Go:   append(a, b...)
来源：http://hz.ydjk.org.cn/gtbhbwrmor.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yongpay.top/gtowtneszq.html

C#:   a.Concat(b).ToList()
来源：http://hz.meibo888.top/gtbmfcbtar.html

[D09] 排序（升序）
来源：http://hz.yongpay.top/gtqjvlwbev.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cheryme.top/gtuvpwcykv.html

PHP:  sort($arr);
来源：http://hz.yueranfly.top/gtidzrscrc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.quarkkingdee.top/gtablbcduh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cashguo.top/gtnuixfesb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.pycfn.com/gtfoiajzxh.html


<!-- 参考信息 -->