代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.daria6918.cn/gtnhpjfrtf.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.shanyushiyangtech.top/gtirlcrijj.html

[B11] 生成数字序列 / 区间
来源：http://hz.jinyuanbaomall.cn/gtkzwrflaz.html

Py:   list(range(0, 10, 2))
来源：http://hz.yonumen.top/gtvitbdoho.html

PHP:  range(0, 10, 2);
来源：http://hz.xziqi.cn/gtcmmeojvw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.hnqzz.top/gtjupnzdcb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yj20258888.top/gtpvwcimry.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.tianlin.xyz/gtjmnqymwl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.shzxlz.cn/gtqxfndnnz.html

Ruby: (0...10).step(2).to_a
来源：http://hz.jinqigufen.top/gtambjfysb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.xziqi.cn/gtbojazfwp.html

[B12] 跳出多层循环
来源：http://hz.yj20258.top/gtyatywyqr.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.nanxuanxn.top/gtjnomdcne.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.redwolf501.top/gtzdyzrxad.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenjidiqi.icu/gtypluzcrp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.sufxvd.cn/gtmmngmswx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj20258888.top/gtjmjxmfby.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.pengpengdd.cyou/gtdtbwvgqb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.yj20258888.top/gtpsgwnpga.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.jianghu66.top/gtlvgrwhad.html

[B13] 判断是否为数字
来源：http://hz.wangshuangyany.cn/gthrnwbvdq.html

Py:   isinstance(x, (int, float))
来源：http://hz.hnqzz.top/gtxvqdxxrx.html

PHP:  is_numeric($x)
来源：http://hz.cucudq.cn/gtpbodeljr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.haohaochexian.top/gtjccjoepg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.sysykeji.top/gtpnudxfej.html

Java: x instanceof Number
来源：http://hz.0kj1m.cn/gtnnmhnkhq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.zhiwuduotai.top/gtsvckixxz.html

Ruby: x.is_a?(Numeric)
来源：http://hz.ydjk.org.cn/gtwmgwapxh.html

C#:   x is int or double or decimal
来源：http://hz.xinyue.icu/gtkjntcpme.html

[B14] 判断值是否在集合内
来源：http://hz.cqqwz.cn/gtgkdihbkb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jinyuanbaomall.cn/gtzphynypt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.jinqigfzy.top/gtwtdakhpk.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.havefunace.top/gtdrtesyaw.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.ywan-chungtsiang.top/gtdbfqtghm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.xuetiantiany.cn/gtswnymyoe.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.cheryme.top/gtpiizhlma.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jyoumei.cn/gtmkniilhi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jinqigufen.top/gtmrhlzzmb.html

[B15] 布尔运算与取反
来源：http://hz.kuanghao11.cn/gtekkudrfc.html

Py:   a and b or not c
来源：http://hz.hysaishi.cn/gttswhhuwe.html

PHP:  $a && $b || !$c
来源：http://hz.xziqi.cn/gtjoqlxrrt.html

JS:   a && b || !c
来源：http://hz.meibo888.top/gtvojngygh.html

TS:   a && b || !c
来源：http://hz.zdqjudy.top/gtacdhindw.html

Java: a && b || !c
来源：http://hz.316326.xyz/gtlwbexhfz.html

Go:   a && b || !c
来源：http://hz.daxiang520.top/gtsudzuwnu.html

Ruby: a && b || !c
来源：http://hz.hammf.cn/gtwzalfgwg.html

C#:   a && b || !c
来源：http://hz.aibaodan.cn/gteeveyibk.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.shzxlz.cn/gtyvrmogoa.html

Py:   if not data: return
来源：http://hz.52xcode.cn/gtjjytuidg.html

PHP:  if (!$data) { return; }
来源：http://hz.sysykeji.top/gtdqsghgmq.html

JS:   if (!data) return;
来源：http://hz.jqgufenzy.top/gtmwpvtbtn.html

TS:   if (!data) return;
来源：http://hz.ybcxt.top/gtweyjbnre.html

Java: if (data == null) return;
来源：http://hz.smart0.xyz/gtfruzqcco.html

Go:   if data == nil { return }
来源：http://hz.yongpay.top/gtixcztexk.html

Ruby: return if data.nil?
来源：http://hz.guowangkeji.top/gtbepuzzyq.html

C#:   if (data == null) return;
来源：http://hz.andypj.xyz/gtsdojmhub.html

================================================================================
来源：http://hz.daxiang520.top/gtscuimmdw.html

C. 函数与作用域
来源：http://hz.gaohongyu789.top/gtfjsvzxda.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtvnastdaf.html

[C01] 定义函数
来源：http://hz.zhijiandao.cn/gtgbnjcgqu.html

Py:   def add(a, b): return a + b
来源：http://hz.gogol.net.cn/gtkbolwmax.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zycfv.cn/gtvyrnkwhe.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.cashguo.top/gtopiesyhh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.shzxlz.cn/gtawsgwldm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.daria6918.cn/gtztmomuqk.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zhongyouzk.top/gtfbusblyu.html

Ruby: def add(a, b); a + b; end
来源：http://hz.kuanghao11.cn/gtlwiexcbz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.guannengcc.top/gtfooymucv.html

[C02] 默认参数
来源：http://hz.zhaomingkeji.xyz/gtbdmgapli.html

Py:   def greet(name="World"): return name
来源：http://hz.ydjk.org.cn/gtlvdhqwjs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hammf.cn/gtvvrwemrg.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jianghu66.top/gtbzwlcghi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.nanxinkj.top/gtklqfnkqk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.hongshengwenyu.top/gtzeenngfm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.gogol.net.cn/gtgnrucnkl.html

Ruby: def greet(name = "World") = name
来源：http://hz.xingfuxueyuan.xyz/gthhdluqio.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.0kj1m.cn/gtzjeftwyi.html

[C03] 可变参数
来源：http://hz.shanyushiyangtech.top/gtrxhoafom.html

Py:   def total(*args): return sum(args)
来源：http://hz.jinyuanbaomall.cn/gtwtyhovwh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.52xcode.cn/gtajyvzxbi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.gaohongyu789.top/gtvqddwuvz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yuxming.cn/gtmojrvmph.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.shzxlz.cn/gtnkgfjoka.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yuxming.cn/gtxloxrxrx.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zdqjudy.top/gtoixtzmbt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.shuidangran.top/gtjbimigru.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hnqzz.top/gtwcqpulrd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.xinyue.icu/gtqptvzwtd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.hnqzz.top/gtwjalghdg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hywenlv.cn/gtmbymewoq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.hammf.cn/gtwnnvdjdw.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.guannengcc.top/gtzqrscayr.html

Go:   // 无：用配置结构体参数
来源：http://hz.ybcxt.top/gtaerqrsdb.html

Ruby: f(a: 1, b: 2)
来源：http://hz.pycfn.com/gtnyfaqzqu.html

C#:   f(a: 1, b: 2)
来源：http://hz.yvedp.cn/gtwmrsoagp.html

[C05] 返回多个值
来源：http://hz.tian-w.cn/gttmvrltqi.html

Py:   return a, b
来源：http://hz.yueranfly.top/gtzzhsbdhi.html

PHP:  return [$a, $b];
来源：http://hz.aibaodan.cn/gtouhvtubc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.cheryme.top/gtwhruuhwy.html

TS:   return { a, b };
来源：http://hz.ydjk.org.cn/gtefubborh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.quarkkingdee.top/gtyqydrbqi.html

Go:   return a, b
来源：http://hz.tianlin.xyz/gttnoswgpb.html

Ruby: return a, b
来源：http://hz.xinyue.icu/gtqrcefzzt.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.0kj1m.cn/gtxjemmpsi.html

[C06] 匿名函数 / lambda
来源：http://hz.zhixingplan.top/gtphqrjzea.html

Py:   square = lambda x: x * x
来源：http://hz.chenjidiqi.icu/gtaevahjxa.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.cucudq.cn/gtngsayjix.html

JS:   const square = x => x * x;
来源：http://hz.hnxiangtu.top/gtisboshai.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.daria6918.cn/gtgdhvvhrp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zhoulong.xyz/gtpmivacwm.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yanxiufei.cn/gtbjsyezdn.html

Ruby: square = ->(x) { x * x }
来源：http://hz.redwolf501.top/gttewuzrkr.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.hnxiangtu.top/gtarthkygt.html

[C07] 把函数作为参数传入
来源：http://hz.zhiwuduotai.top/gtxjoooxre.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.pengpengdd.cyou/gtddmekfpj.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.cdnleiting.top/gtcwpzxvpq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.daxiang520.top/gtsaitsosl.html

TS:   arr.map(String)
来源：http://hz.gzhubu.top/gtopturofw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.daxiang520.top/gtjovmqjhj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.birdmap.top/gttgakiqij.html

Ruby: arr.map(&:upcase)
来源：http://hz.daxiang520.top/gtdzlxmyfo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.guowangkeji.top/gteqguubws.html

[C08] 闭包
来源：http://hz.ivvv.top/gtkhdzgvhf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhiwuduotai.top/gtxgdujnlk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.cashguo.top/gtbqheqkmg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.tian-w.cn/gtdixeamnc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.c1oappe.top/gtdnvsebkf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.aizwys.cn/gtipvwtzed.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.havefunace.top/gtlwgkslbz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.shuidangran.top/gtsjdaydqk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jianghu66.top/gtmsmpowwa.html

[C09] 递归
来源：http://hz.xziqi.cn/gtabvhdnql.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.wangdashe.top/gtszhqrnzj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.aibaodan.cn/gtrvuvwwza.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.daxiang520.top/gtnrdrehrr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.quarkkingdee.top/gtoztccukj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.guannengcc.top/gteyhcnunv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.quarkkingdee.top/gtuzjwaiac.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.fzhhl.top/gtaxkfegcu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.xinyue.icu/gtbjqjilas.html

[C10] 变量作用域
来源：http://hz.ivvv.top/gtdcllcmmo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ehwqpu.com/gtcxbaraeg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zdqjudy.top/gthkxhbljf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.hammf.cn/gtgkfeojww.html

TS:   同 JS
来源：http://hz.yvedp.cn/gteydxnaiq.html

Java: 方法内为块级作用域
来源：http://hz.iojbl.cn/gtiojatzcr.html

Go:   花括号块级作用域
来源：http://hz.nanxinkj.top/gtfnfettap.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.svipenyu.cn/gtwrzvcesb.html

C#:   块级作用域
来源：http://hz.andypj.xyz/gtgwiwqnzv.html

[C11] 模块导入与导出
来源：http://hz.shangyingyoupin.top/gtdlmeccrk.html

Py:   from module import func
来源：http://hz.jinghuilouyu.cn/gtkxuhrhls.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yuxming.cn/gtjawfgplj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.nwbrower.top/gtvcvovewn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xinyue.icu/gtsjgphhcn.html

Java: import java.util.List;
来源：http://hz.jyoumei.cn/gtwbewhpvb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.shuidangran.top/gttjpmaaco.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.xziqi.cn/gtcbknaovw.html

C#:   using System.Text;
来源：http://hz.nanxuanxn.top/gtgpzavdqw.html

[C12] 立即执行函数 IIFE
来源：http://hz.guowangkeji.top/gteavxyhqp.html

Py:   (lambda: print("run"))()
来源：http://hz.redwolf501.top/gthmqvsvwa.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhoulong.xyz/gtbxenqhwt.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jianghu66.top/gtiagyxxzf.html

TS:   (() => { console.log("run"); })();
来源：http://hz.guannengcc.top/gtlngepgvr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.daxiang520.top/gtrjtdvyzb.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ivvv.top/gtrgsrrgzc.html

Ruby: -> { puts "run" }.call
来源：http://hz.cucudq.cn/gtewpxzlbp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.jqgfzy.top/gtpzqsvxzh.html

[C13] 类型声明 / 类型注解
来源：http://hz.ppjwa.cn/gtiopzhptg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.nanxuanxn.top/gtqonqicxh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhengqikj.top/gtqbftlowm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ywan-chungtsiang.top/gtbeatjvqm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.aizwys.cn/gtpwdlzwyj.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.zycfv.cn/gtzbdunwor.html

Go:   func add(a, b int) int
来源：http://hz.fengsongda.top/gthuyumrpa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.ehwqpu.com/gtspeanybn.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.fzhhl.top/gtrdpqedki.html

[C14] 泛型函数
来源：http://hz.guowangkeji.top/gtjerlywmo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.cheryme.top/gtjqxikice.html

PHP:  // 无泛型
来源：http://hz.wangdashe.top/gttyzehcco.html

JS:   // 无泛型
来源：http://hz.fengsongda.top/gtfmuitfjm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ybcxt.top/gtlanssvfh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yuanzhike.top/gtmbhdtujx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.snrcjt.cn/gtfrswjxcp.html

Ruby: # 无泛型
来源：http://hz.chenzaomai.com/gtdpynuyhs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hfpthk.cn/gtrstkuxao.html

[C15] 解构 / 展开参数
来源：http://hz.hongshengwenyu.top/gtmrustkor.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.vqdsnc.cn/gtvprpwuze.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yj202588.top/gtkxlubqvm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.daxiang520.top/gtlnxpmpfc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hongshengwenyu.top/gtlggkdpai.html

Java: // 无解构
来源：http://hz.mhx1999.top/gtvzkmgevg.html

Go:   // 无解构
来源：http://hz.ppjwa.cn/gtfmyjrxgl.html

Ruby: a, b = pair
来源：http://hz.yonumen.top/gthsowggig.html

C#:   var (a, b) = pair;
来源：http://hz.gzhubu.top/gtbmffpfjw.html

[C16] 函数 / 方法重载
来源：http://hz.quarkkingdee.top/gtbxkodtwe.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.feifeiyinyue.top/gtmozjtsoc.html

PHP:  // 无重载
来源：http://hz.sweek.top/gtmwkkmypy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.aizwys.cn/gterczljjy.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yj202588.top/gttusrlrij.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.zhijiandao.cn/gttmxfijlv.html

Go:   // 无重载：用不同函数名
来源：http://hz.shanyushiyangtech.top/gtxrczgwxc.html

Ruby: # 无重载：靠动态参数
来源：http://hz.aibaodan.cn/gtrtrencdb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.wangshuangyany.cn/gtxhbcbmac.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gttsyyiebr.html

D. 数组 / 列表 / 集合
来源：http://hz.zhoulong.xyz/gtdqlqyusb.html

================================================================================
来源：http://hz.ydzc1.top/gtptffhhkf.html

[D01] 创建数组 / 列表
来源：http://hz.jqgfzy.top/gtrpiftznd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.wangdashe.top/gtbddmokex.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.gzhubu.top/gtcszcvfvk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.sufxvd.cn/gtebjhcubo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jinyuanbaomall.cn/gtjugxobgj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.haohaochexian.top/gtlucbnfbw.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jqgufenzy.top/gtlkevfxjj.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shuidangran.top/gtmhsezjwc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yuanzhike.top/gtfphhvtvr.html

[D02] 追加元素到末尾
来源：http://hz.zhengqikj.top/gtemtxazzg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gogol.net.cn/gtmwoznzwb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.chenzaomai.com/gttdztxykf.html

JS:   arr.push(4);
来源：http://hz.zhoulong.xyz/gtiqcvjzix.html

TS:   arr.push(4);
来源：http://hz.jianghu66.top/gtrhnonuhz.html

Java: list.add(4);
来源：http://hz.xylfe.cn/gtstdbxzqn.html

Go:   arr = append(arr, 4)
来源：http://hz.yj20258.top/gtqrulgtuq.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhijiandao.cn/gtbemnbygy.html

C#:   list.Add(4);
来源：http://hz.zhengqikj.top/gtircxtxup.html

[D03] 在指定位置插入元素
来源：http://hz.ehwqpu.com/gtisqfsymp.html

Py:   arr.insert(0, 0)
来源：http://hz.jyoumei.cn/gtjgdmdkhb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.snrcjt.cn/gtecdsozvg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhengqikj.top/gtfvpjbzof.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.shzxlz.cn/gtvghdljbz.html

Java: list.add(0, 0);
来源：http://hz.52xcode.cn/gtufwqtbnp.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jlsjyb.cn/gtacxrdnko.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.chenzaomai.com/gtrqnheziu.html

C#:   list.Insert(0, 0);
来源：http://hz.tian-w.cn/gtcdodydwj.html

[D04] 删除元素
来源：http://hz.hammf.cn/gtmzwlxwkm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.kuanghao11.cn/gtlpkzuewt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.iojbl.cn/gtdyyxrwdf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yonumen.top/gtgbpmcswm.html

TS:   arr.splice(0, 1);
来源：http://hz.zhongyouzk.top/gttgwsgljn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.feifeiyinyue.top/gtikuqwduv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yongpay.top/gtsyglhijm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.gotoacloud.top/gtkrcmfwxz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.chenjidiqi.icu/gtbfcvadhj.html

[D05] 访问与修改元素
来源：http://hz.52xcode.cn/gtbyefdffx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ppjwa.cn/gtnbawylvk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yj202588.top/gtbtlclwap.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.andypj.xyz/gtcjhmwuxq.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.havefunace.top/gtdhsznkpv.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yuanzhike.top/gttokglazf.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.aizwys.cn/gtojcsfpjy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.fengsongda.top/gtytnopefp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xuetiantiany.cn/gtfrihptbz.html

[D06] 数组长度
来源：http://hz.316326.xyz/gtkgjozidl.html

Py:   len(arr)
来源：http://hz.gaohongyu789.top/gtifwlrmvq.html

PHP:  count($arr);
来源：http://hz.cheryme.top/gtmawkilcm.html

JS:   arr.length
来源：http://hz.ppjwa.cn/gtrukcztqx.html

TS:   arr.length
来源：http://hz.yangfankeji.com/gtzwmthvyr.html

Java: list.size();
来源：http://hz.gotoacloud.top/gtgbdvxksb.html

Go:   len(arr)
来源：http://hz.sweek.top/gtykubygmd.html

Ruby: arr.length; arr.size
来源：http://hz.9152youxi.cn/gtpyfbpzio.html

C#:   list.Count;
来源：http://hz.ywan-chungtsiang.top/gtispqnmmx.html

[D07] 切片 / 取子数组
来源：http://hz.birdmap.top/gtudlvjvzy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhiwuduotai.top/gtsuzgrswe.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jianghu66.top/gtsfmmkqkx.html

JS:   arr.slice(1, 4);
来源：http://hz.hammf.cn/gtgvhtcpss.html

TS:   arr.slice(1, 4);
来源：http://hz.jlsjyb.cn/gtgnwbjoym.html

Java: list.subList(1, 4);
来源：http://hz.pengpengdd.cyou/gttwhmotox.html

Go:   arr[1:4]
来源：http://hz.yueranfly.top/gtszhoabdx.html

Ruby: arr[1, 3]
来源：http://hz.gzhubu.top/gtccfwipap.html

C#:   list.GetRange(1, 3);
来源：http://hz.hongshengwenyu.top/gtjnpklphs.html

[D08] 合并两个数组
来源：http://hz.chenlongwang.top/gtsagfecym.html

Py:   a + b;  a.extend(b)
来源：http://hz.xziqi.cn/gtloxaillh.html

PHP:  array_merge($a, $b);
来源：http://hz.cheryme.top/gtcoaikwan.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zycfv.cn/gtcmmmojcy.html

TS:   [...a, ...b];
来源：http://hz.gaohongyu789.top/gtqntsadti.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yvedp.cn/gtgldoqpkc.html

Go:   append(a, b...)
来源：http://hz.jqgfzy.top/gtpoajwjih.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yongpay.top/gtsyopkici.html

C#:   a.Concat(b).ToList()
来源：http://hz.zycfv.cn/gtpiwzhupy.html

[D09] 排序（升序）
来源：http://hz.svipenyu.cn/gtmxtymhkl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jianghu66.top/gtjvjmjzrl.html

PHP:  sort($arr);
来源：http://hz.wangshuangyany.cn/gtorbfsyso.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.gotoacloud.top/gtvsdnxmem.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cqqwz.cn/gthcwxazqe.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.9152youxi.cn/gtgvqcnvuz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jianghu66.top/gtswkrcckv.html

Ruby: arr.sort
来源：http://hz.xinyue.icu/gtbjadmcxa.html

C#:   list.Sort();
来源：http://hz.guannengcc.top/gtypqlaovj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xuanzx.com/gttohdugpb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yj20258888.top/gtpfaueejq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.pengpengdd.cyou/gtrdosdvju.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuxming.cn/gtxyjhrrva.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shuidangran.top/gtjnygauvq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.gogol.net.cn/gthngrfonm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.gzhubu.top/gtdwheqhqh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ppjwa.cn/gtkvhaliel.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhaomingkeji.xyz/gtgxvavgne.html

[D11] 反转数组
来源：http://hz.ehwqpu.com/gtkjlrsndt.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.xinyue.icu/gtthecmsuw.html

PHP:  array_reverse($arr);
来源：http://hz.xuetiantiany.cn/gtjvmefdly.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.snrcjt.cn/gtrnyywdnr.html


<!-- 参考信息 -->