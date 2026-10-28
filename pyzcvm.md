代发 wailian999

PHP:  range(0, 10, 2);
来源：http://hz.cqqwz.cn/gtxtqvblxn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.smart0.xyz/gtbcvzypvh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhoulong.xyz/gtimlfilou.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.hywenlv.cn/gtwgvwjdts.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.sweek.top/gtofazypqk.html

Ruby: (0...10).step(2).to_a
来源：http://hz.zhengqikj.top/gtlwmzplgv.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.tianlin.xyz/gtjhslifvg.html

[B12] 跳出多层循环
来源：http://hz.fengsongda.top/gthvavbeqw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.havefunace.top/gtkaqfbdtm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.wangshuangyany.cn/gtvvaqajvr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhengqikj.top/gtqmlrnyav.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.shuidangran.top/gtdhnsmhip.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.nwbrower.top/gtbanrqsuj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.chenzaomai.com/gtnokslokm.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.hnxiangtu.top/gterwxzpsz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.gotoacloud.top/gtgfwqeutp.html

[B13] 判断是否为数字
来源：http://hz.hywenlv.cn/gtnqbzgrol.html

Py:   isinstance(x, (int, float))
来源：http://hz.jinqigufen.top/gtcsgsvmti.html

PHP:  is_numeric($x)
来源：http://hz.zhixingplan.top/gtzvomgmze.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhiwuduotai.top/gtwjzkzgsc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.ybcxt.top/gtttxraxfk.html

Java: x instanceof Number
来源：http://hz.feifeiyinyue.top/gtnqwprcrx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.gogol.net.cn/gtnohscsuj.html

Ruby: x.is_a?(Numeric)
来源：http://hz.cdnleiting.top/gttemgdfii.html

C#:   x is int or double or decimal
来源：http://hz.zhengqikj.top/gttesnslbq.html

[B14] 判断值是否在集合内
来源：http://hz.jinqigufen.top/gthpwntajn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jqgfzy.top/gtuniyqbmd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.snrcjt.cn/gtamusfxsy.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yvedp.cn/gtbxtwagdl.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.xylfe.cn/gtwcwieqst.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.jqgufenzy.top/gtrxjngjou.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.shanyushiyangkeji.top/gtemayvgyg.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.gaohongyu789.top/gtrpazxtxy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yongpay.top/gtviywkbdq.html

[B15] 布尔运算与取反
来源：http://hz.jinqigfzy.top/gtmolwciee.html

Py:   a and b or not c
来源：http://hz.fzhhl.top/gtcjtkawvq.html

PHP:  $a && $b || !$c
来源：http://hz.cheryme.top/gtftpamppo.html

JS:   a && b || !c
来源：http://hz.guannengcc.top/gthisfmudw.html

TS:   a && b || !c
来源：http://hz.guowangkeji.top/gtsyniefsx.html

Java: a && b || !c
来源：http://hz.snrcjt.cn/gtfxzsykcu.html

Go:   a && b || !c
来源：http://hz.xuanzx.com/gteecfdwtz.html

Ruby: a && b || !c
来源：http://hz.shanyushiyangtech.top/gtxkjiwqdg.html

C#:   a && b || !c
来源：http://hz.guannengcc.top/gthxbgzbkd.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.ehwqpu.com/gtcdqczfxt.html

Py:   if not data: return
来源：http://hz.yanxiufei.cn/gtqnfilonl.html

PHP:  if (!$data) { return; }
来源：http://hz.jianghu66.top/gtbhggflyw.html

JS:   if (!data) return;
来源：http://hz.guowangkeji.top/gtjewfjlzf.html

TS:   if (!data) return;
来源：http://hz.dashuyun.cn/gtocuhchqp.html

Java: if (data == null) return;
来源：http://hz.xziqi.cn/gtcwlcuuyx.html

Go:   if data == nil { return }
来源：http://hz.zhoulong.xyz/gtyolgsjxh.html

Ruby: return if data.nil?
来源：http://hz.pycfn.com/gtbpqvstso.html

C#:   if (data == null) return;
来源：http://hz.fengsongda.top/gtjmgcrniq.html

================================================================================
来源：http://hz.daxiang520.top/gtexskxokt.html

C. 函数与作用域
来源：http://hz.snrcjt.cn/gtiahnhmfw.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtsmubvwek.html

[C01] 定义函数
来源：http://hz.zhengqikj.top/gtykewchwm.html

Py:   def add(a, b): return a + b
来源：http://hz.hywenlv.cn/gtvmzxydeq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jianghu66.top/gtxtwuynhp.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.zhiwuduotai.top/gtuxyzkbvd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ybcxt.top/gtisunokcq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.sysykeji.top/gtfglpotwu.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.cqqwz.cn/gtsazdjuby.html

Ruby: def add(a, b); a + b; end
来源：http://hz.kuanghao11.cn/gtwhozffwf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.gaohongyu789.top/gtpsllxodg.html

[C02] 默认参数
来源：http://hz.guannengcc.top/gtgutwqwzg.html

Py:   def greet(name="World"): return name
来源：http://hz.hfpthk.cn/gtacihvbln.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.fengsongda.top/gtmjuxmmpx.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zhengqikj.top/gtybrzrimf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ydzc1.top/gtmfmwropo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.birdmap.top/gtrcclkudb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.quarkkingdee.top/gtsejytxyv.html

Ruby: def greet(name = "World") = name
来源：http://hz.yangfankeji.com/gtpsexxbza.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.zhengqikj.top/gtmyrqpqbf.html

[C03] 可变参数
来源：http://hz.gaohongyu789.top/gtzrjycjuc.html

Py:   def total(*args): return sum(args)
来源：http://hz.hammf.cn/gtmphttvna.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.sweek.top/gtjybyjggy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.nwbrower.top/gtnpixbcnl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jlsjyb.cn/gthecldgfd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jinyuanbaomall.cn/gtmoumtyis.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.tian-w.cn/gtunyntkyi.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.kuanghao11.cn/gtiesbwtjg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.iojbl.cn/gttclekeam.html

[C04] 命名参数 / 关键字参数
来源：http://hz.yonumen.top/gtghpixugp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.0kj1m.cn/gtuipenyuv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ybcxt.top/gtbpafmujb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zhijiandao.cn/gtmvwrblmy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.smart0.xyz/gtpjexrbfb.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.jqgfzy.top/gthxsujopx.html

Go:   // 无：用配置结构体参数
来源：http://hz.guannengcc.top/gtebnsixwg.html

Ruby: f(a: 1, b: 2)
来源：http://hz.shangyingyoupin.top/gtejepjfqv.html

C#:   f(a: 1, b: 2)
来源：http://hz.shanyushiyangkeji.top/gtfpcslugc.html

[C05] 返回多个值
来源：http://hz.yanxiufei.cn/gtfhpotikt.html

Py:   return a, b
来源：http://hz.fzhhl.top/gtlkoadqhi.html

PHP:  return [$a, $b];
来源：http://hz.zhengqikj.top/gtzhlwmijx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.ydzc1.top/gthvrawtnv.html

TS:   return { a, b };
来源：http://hz.yanxiufei.cn/gtenjiqdpa.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.birdmap.top/gtgxbaftuv.html

Go:   return a, b
来源：http://hz.gzhubu.top/gtayzzrhwc.html

Ruby: return a, b
来源：http://hz.xuanzx.com/gtoubwxjav.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.birdmap.top/gtxxvljyys.html

[C06] 匿名函数 / lambda
来源：http://hz.jqgfzy.top/gtjxekmtpy.html

Py:   square = lambda x: x * x
来源：http://hz.hnxiangtu.top/gtalesztsg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yuxming.cn/gtyvlriqbd.html

JS:   const square = x => x * x;
来源：http://hz.jqgufenzy.top/gtzpvyeoir.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.pengpengdd.cyou/gtpbvjdrtu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.fengsongda.top/gtniayhjjq.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yongpay.top/gtybihtsop.html

Ruby: square = ->(x) { x * x }
来源：http://hz.bjfxy.top/gtckmvwepv.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yueranfly.top/gtsaivwlvp.html

[C07] 把函数作为参数传入
来源：http://hz.xuetiantiany.cn/gtxnyxcsiz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.kuanghao11.cn/gtnwsizard.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.ehwqpu.com/gtuokuwffv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jqgufenzy.top/gtskawsgyi.html

TS:   arr.map(String)
来源：http://hz.hfpthk.cn/gtkzyunlid.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.smart0.xyz/gtxmyffplt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.feifeiyinyue.top/gtxdogbrtq.html

Ruby: arr.map(&:upcase)
来源：http://hz.hywenlv.cn/gtujlfhkea.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.ivvv.top/gtvpexyuem.html

[C08] 闭包
来源：http://hz.hongshengwenyu.top/gtzcfcwhkl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.dashuyun.cn/gtdcivkbtc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.pengpengdd.cyou/gtekvkpvbe.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.ywan-chungtsiang.top/gtabqcjjxx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jyoumei.cn/gtaemudnfk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.hnqzz.top/gtolpzswyb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zycfv.cn/gtukxuwhyi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.chenlongwang.top/gthfoaktfk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.shzxlz.cn/gtfgomwuhs.html

[C09] 递归
来源：http://hz.aibaodan.cn/gtgyklgcng.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.fengsongda.top/gtfzquqlns.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhengqikj.top/gtsccgsxil.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhaomingkeji.xyz/gttspwpynn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ydzc1.top/gtaovrzbgf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.chenlongwang.top/gtytrybfgp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jqgfzy.top/gtkafkrpjg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.mhx1999.top/gttepjljaj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.daxiang520.top/gtxmhscaby.html

[C10] 变量作用域
来源：http://hz.shanyushiyangtech.top/gtuurofnri.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.shanyushiyangkeji.top/gtvuzmjxco.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.iojbl.cn/gtlqcbzazv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.vqdsnc.cn/gtwfaryuwm.html

TS:   同 JS
来源：http://hz.yuanzhike.top/gtnquuqlsa.html

Java: 方法内为块级作用域
来源：http://hz.dashuyun.cn/gtemomxmww.html

Go:   花括号块级作用域
来源：http://hz.fengsongda.top/gtnbfmbddq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yanxiufei.cn/gteqiqfipz.html

C#:   块级作用域
来源：http://hz.tianlin.xyz/gtfdjcqiqs.html

[C11] 模块导入与导出
来源：http://hz.shuidangran.top/gtenocguks.html

Py:   from module import func
来源：http://hz.daxiang520.top/gtmvzgbmqs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zycfv.cn/gtubponboi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.daxiang520.top/gthrmsioos.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.tanke756.top/gtvdkwiqrh.html

Java: import java.util.List;
来源：http://hz.zhijiandao.cn/gtjiqmkhhc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.iojbl.cn/gtvpbjtqpk.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.tanke756.top/gthpuxjpsf.html

C#:   using System.Text;
来源：http://hz.316326.xyz/gtmtoiwpjg.html

[C12] 立即执行函数 IIFE
来源：http://hz.nwbrower.top/gtwywkksps.html

Py:   (lambda: print("run"))()
来源：http://hz.guowangkeji.top/gtwljfvzdz.html

PHP:  (function () { echo "run"; })();
来源：http://hz.tanke756.top/gtxljjqlwe.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yj20258888.top/gtkbjbfxan.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhaomingkeji.xyz/gtxkebdqoy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yonumen.top/gtdffeifpf.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.cheryme.top/gtcsoncdez.html

Ruby: -> { puts "run" }.call
来源：http://hz.cdnleiting.top/gtwuknsyyf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hongshengwenyu.top/gtnohmpbap.html

[C13] 类型声明 / 类型注解
来源：http://hz.yongpay.top/gtlnmosuxu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.wangshuangyany.cn/gtsnbjavwi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xziqi.cn/gtlkuvdpmt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hnxiangtu.top/gtfkaksbuv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jyoumei.cn/gtfnseypyx.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yangfankeji.com/gtwzvcacrs.html

Go:   func add(a, b int) int
来源：http://hz.ybcxt.top/gtyhgxdgaq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cashguo.top/gtoiwmolpw.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.zycfv.cn/gtflgmovmh.html

[C14] 泛型函数
来源：http://hz.fengsongda.top/gtmldrftun.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.316326.xyz/gttqcticyt.html

PHP:  // 无泛型
来源：http://hz.yangfankeji.com/gtciluexqx.html

JS:   // 无泛型
来源：http://hz.ehwqpu.com/gthkuhlefe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.nanxinkj.top/gtfadfvceq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yanxiufei.cn/gtpmlkjaip.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.aibaodan.cn/gtzfpdymxz.html

Ruby: # 无泛型
来源：http://hz.yueranfly.top/gtmibakvex.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.haohaochexian.top/gtwiexstut.html

[C15] 解构 / 展开参数
来源：http://hz.ywan-chungtsiang.top/gtntkymvvy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.dianchejie.cn/gtapelprla.html

PHP:  [$a, $b] = $pair;
来源：http://hz.xinyue.icu/gtfqaxcpdi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cheryme.top/gtmyzyqoul.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.aibaodan.cn/gthdaskjlg.html

Java: // 无解构
来源：http://hz.shanyushiyangkeji.top/gtbendhrpt.html

Go:   // 无解构
来源：http://hz.vqdsnc.cn/gtnskgviru.html

Ruby: a, b = pair
来源：http://hz.gogol.net.cn/gtuyrzklwc.html

C#:   var (a, b) = pair;
来源：http://hz.sxryk.cn/gtfzuateqz.html

[C16] 函数 / 方法重载
来源：http://hz.feifeiyinyue.top/gtkpagnffr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.tian-w.cn/gtjxwainye.html

PHP:  // 无重载
来源：http://hz.zhongyouzk.top/gtxsksoaqm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.gogol.net.cn/gthqpvvbkc.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hongshengwenyu.top/gtrdnsezff.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.316326.xyz/gtvishvzbj.html

Go:   // 无重载：用不同函数名
来源：http://hz.jinghuilouyu.cn/gtuhkpoqem.html

Ruby: # 无重载：靠动态参数
来源：http://hz.vqdsnc.cn/gtvwaglsoy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xylfe.cn/gtgelsjauy.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtqwoufqyh.html

D. 数组 / 列表 / 集合
来源：http://hz.aizwys.cn/gtzvaysbyj.html

================================================================================
来源：http://hz.daxiang520.top/gtjbdjxzbj.html

[D01] 创建数组 / 列表
来源：http://hz.fzhhl.top/gtnchxxfui.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.pengpengdd.cyou/gtljeyelxw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jinyuanbaomall.cn/gtzyjbjjlg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.wangshuangyany.cn/gtrjuokhsr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.tanke756.top/gtcbdtlsgd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.aizwys.cn/gtuatamsvv.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhiwuduotai.top/gtzvrcvlly.html

Ruby: arr = [1, 2, 3]
来源：http://hz.sxryk.cn/gtzhdzhijy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ivvv.top/gtpkffummg.html

[D02] 追加元素到末尾
来源：http://hz.hfpthk.cn/gtbqtoxndm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.aibaodan.cn/gtqrctaobf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jiagoushi.top/gtgfvozzxq.html

JS:   arr.push(4);
来源：http://hz.ehwqpu.com/gtrefhsado.html

TS:   arr.push(4);
来源：http://hz.hfpthk.cn/gtyjvudndq.html

Java: list.add(4);
来源：http://hz.yuanzhike.top/gtkedlyazo.html

Go:   arr = append(arr, 4)
来源：http://hz.jqgufenzy.top/gtzrgtsotm.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.hywenlv.cn/gtwdfbkcge.html

C#:   list.Add(4);
来源：http://hz.tian-w.cn/gthbeftoje.html

[D03] 在指定位置插入元素
来源：http://hz.zhijiandao.cn/gtbrwuween.html

Py:   arr.insert(0, 0)
来源：http://hz.tian-w.cn/gtxbjogmum.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yonumen.top/gtpbwdjqop.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhaomingkeji.xyz/gtdksrqvhh.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.shanyushiyangtech.top/gtyfgfvhos.html

Java: list.add(0, 0);
来源：http://hz.jinyuanbaomall.cn/gthoscuise.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.chenlongwang.top/gtgnlwbohc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.iojbl.cn/gtodnqmfgu.html

C#:   list.Insert(0, 0);
来源：http://hz.gogol.net.cn/gtiglsfqjl.html

[D04] 删除元素
来源：http://hz.52xcode.cn/gtyncjzbmp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jqgufenzy.top/gtwfbbdtqs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ywan-chungtsiang.top/gtkvyxwoyd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.svipenyu.cn/gtudssgsrp.html

TS:   arr.splice(0, 1);
来源：http://hz.zhaomingkeji.xyz/gtabpuwzng.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ydzc1.top/gtjnvbenoe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.meibo888.top/gtymndbzgg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.nwbrower.top/gtjnwaegca.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zycfv.cn/gtddboemxk.html

[D05] 访问与修改元素
来源：http://hz.0kj1m.cn/gtgyqxowln.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zycfv.cn/gtloviuuek.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hnqzz.top/gtsyanffcw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ydjk.org.cn/gtndsfjwwv.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.sxryk.cn/gtosbxxxky.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.chenzaomai.com/gtwatrvhvr.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.wangshuangyany.cn/gtjmdsxttn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tianlin.xyz/gtadcaqpfq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.52xcode.cn/gtxjopxvtn.html

[D06] 数组长度
来源：http://hz.xingfuxueyuan.xyz/gtfsexbnnh.html

Py:   len(arr)
来源：http://hz.sufxvd.cn/gtrfanyrui.html

PHP:  count($arr);
来源：http://hz.yonumen.top/gtqpfdpyad.html

JS:   arr.length
来源：http://hz.dashuyun.cn/gtfgueieuf.html

TS:   arr.length
来源：http://hz.jlsjyb.cn/gtiqennqwa.html

Java: list.size();
来源：http://hz.pycfn.com/gtexrgqlrz.html

Go:   len(arr)
来源：http://hz.quarkkingdee.top/gtmpkyimwf.html

Ruby: arr.length; arr.size
来源：http://hz.haohaochexian.top/gtqxwaqufj.html

C#:   list.Count;
来源：http://hz.hnqzz.top/gthbhdarfc.html

[D07] 切片 / 取子数组
来源：http://hz.shuidangran.top/gtlkoxsyzx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.nwbrower.top/gtjpjivlxe.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.sxryk.cn/gtjrihdnvv.html

JS:   arr.slice(1, 4);
来源：http://hz.jinyuanbaomall.cn/gtotczoxjv.html

TS:   arr.slice(1, 4);
来源：http://hz.0kj1m.cn/gtktrzkwxz.html

Java: list.subList(1, 4);
来源：http://hz.zdqjudy.top/gtsdclmnfk.html

Go:   arr[1:4]
来源：http://hz.cucudq.cn/gtwrdubuje.html

Ruby: arr[1, 3]
来源：http://hz.xziqi.cn/gtzpgveocp.html

C#:   list.GetRange(1, 3);
来源：http://hz.yueranfly.top/gtamcbbclw.html

[D08] 合并两个数组
来源：http://hz.fzhhl.top/gthrzcyciu.html

Py:   a + b;  a.extend(b)
来源：http://hz.cdnleiting.top/gtzsefbgyo.html

PHP:  array_merge($a, $b);
来源：http://hz.jinqigfzy.top/gtvsmimucb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.snrcjt.cn/gtqcmoxccw.html

TS:   [...a, ...b];
来源：http://hz.jinqigufen.top/gtphsjxjjo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.birdmap.top/gtrdbjufum.html

Go:   append(a, b...)
来源：http://hz.jinqigfzy.top/gtpjatgwad.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhiwuduotai.top/gtggmoeqqq.html

C#:   a.Concat(b).ToList()
来源：http://hz.cashguo.top/gtbrfikthb.html

[D09] 排序（升序）
来源：http://hz.0kj1m.cn/gtohfwfvii.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ybcxt.top/gtwzglitdw.html

PHP:  sort($arr);
来源：http://hz.sufxvd.cn/gtrddnxobp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.feifeiyinyue.top/gtksczggyn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cdnleiting.top/gthusrcgfh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.nanxinkj.top/gtdjvgjkhv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yangfankeji.com/gtmdgzziel.html

Ruby: arr.sort
来源：http://hz.andypj.xyz/gtodkbwkon.html

C#:   list.Sort();
来源：http://hz.gaohongyu789.top/gtkkewphbk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xziqi.cn/gtczllsgox.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.nanxinkj.top/gtlujvrvxa.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.dianchejie.cn/gtfgousxaf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.chenlongwang.top/gtykjawszj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinqigfzy.top/gttkxwekzc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.nanxuanxn.top/gtzrhzbckt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xuetiantiany.cn/gtkftraqvb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.0kj1m.cn/gtwbpscfct.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.dianchejie.cn/gthcwqbemw.html

[D11] 反转数组
来源：http://hz.aizwys.cn/gtkxdzfpql.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.sxryk.cn/gtaenezjme.html

PHP:  array_reverse($arr);
来源：http://hz.havefunace.top/gtnboxwflq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.iojbl.cn/gtwqcacdeu.html

TS:   [...arr].reverse();
来源：http://hz.sysykeji.top/gtftkufghe.html

Java: Collections.reverse(list);
来源：http://hz.sysykeji.top/gtwrptehsr.html

Go:   slices.Reverse(arr)
来源：http://hz.guannengcc.top/gtjrznapvw.html

Ruby: arr.reverse
来源：http://hz.gzhubu.top/gtpkcoqkkv.html


<!-- 参考信息 -->