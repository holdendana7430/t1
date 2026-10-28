代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.wangshuangyany.cn/gttfwpzkbu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.yuanzhike.top/gtoiblpnyk.html

[B11] 生成数字序列 / 区间
来源：http://hz.quarkkingdee.top/gtvdoucywk.html

Py:   list(range(0, 10, 2))
来源：http://hz.0kj1m.cn/gtedyhkawe.html

PHP:  range(0, 10, 2);
来源：http://hz.yongpay.top/gtvfzkimtu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.c1oappe.top/gtetuxngva.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.guowangkeji.top/gtubtjqsou.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.dianchejie.cn/gtgpqxlcti.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.sysykeji.top/gthzpkvsab.html

Ruby: (0...10).step(2).to_a
来源：http://hz.dashuyun.cn/gtkffiqjyu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.feifeiyinyue.top/gtfihtuyyo.html

[B12] 跳出多层循环
来源：http://hz.jinqigufen.top/gtbhezaxrz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.kuanghao11.cn/gthjbpanxi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.316326.xyz/gtklvbdcui.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.chenjidiqi.icu/gtmcwveooo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.0kj1m.cn/gthgcjnpeh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.yonumen.top/gtjnrqhqjm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.jinghuilouyu.cn/gtxkmaarml.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.aizwys.cn/gtaqmdlyzw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hfpthk.cn/gtvoorxcty.html

[B13] 判断是否为数字
来源：http://hz.quarkkingdee.top/gtwfvlrdog.html

Py:   isinstance(x, (int, float))
来源：http://hz.zhixingplan.top/gtuhudbaoi.html

PHP:  is_numeric($x)
来源：http://hz.cdnleiting.top/gtdjtdmrxn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.nanxinkj.top/gtybstsbez.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.yj20258.top/gtuchpphle.html

Java: x instanceof Number
来源：http://hz.daxiang520.top/gtruobrlnj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.cashguo.top/gtaxdbpqiz.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zdqjudy.top/gtvkxvxpgb.html

C#:   x is int or double or decimal
来源：http://hz.smart0.xyz/gtbrhjxtlh.html

[B14] 判断值是否在集合内
来源：http://hz.hysaishi.cn/gtjxaefmsg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.aizwys.cn/gtbmhuyrhx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.xinyue.icu/gttppkfzgp.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.nwbrower.top/gtdotbywix.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jlsjyb.cn/gtwxdkvqfi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.bjfxy.top/gtyrqpxlrk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.dianchejie.cn/gtfzolghbj.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.hongshengwenyu.top/gtuxagwfqi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jinqigufen.top/gtecmbugzg.html

[B15] 布尔运算与取反
来源：http://hz.zhengqikj.top/gtkkihsyuu.html

Py:   a and b or not c
来源：http://hz.c1oappe.top/gtuojxslsn.html

PHP:  $a && $b || !$c
来源：http://hz.chenzaomai.com/gtbbkpzrgj.html

JS:   a && b || !c
来源：http://hz.yonumen.top/gtxaegrmst.html

TS:   a && b || !c
来源：http://hz.xinyue.icu/gtozjrcxrn.html

Java: a && b || !c
来源：http://hz.cashguo.top/gtasqpijrk.html

Go:   a && b || !c
来源：http://hz.jianghu66.top/gtnendgbiy.html

Ruby: a && b || !c
来源：http://hz.0kj1m.cn/gtotqcoghm.html

C#:   a && b || !c
来源：http://hz.shanyushiyangtech.top/gtrgxtnoro.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.wangdashe.top/gtjfnfqxzb.html

Py:   if not data: return
来源：http://hz.zhengqikj.top/gtrrfafjfq.html

PHP:  if (!$data) { return; }
来源：http://hz.yueranfly.top/gtfksuqlmw.html

JS:   if (!data) return;
来源：http://hz.fengsongda.top/gtnflfhwlv.html

TS:   if (!data) return;
来源：http://hz.shuidangran.top/gtffiqnylv.html

Java: if (data == null) return;
来源：http://hz.xingfuxueyuan.xyz/gtatwjuszg.html

Go:   if data == nil { return }
来源：http://hz.0kj1m.cn/gtugisrcmk.html

Ruby: return if data.nil?
来源：http://hz.zhoulong.xyz/gtdswojgqx.html

C#:   if (data == null) return;
来源：http://hz.zhiwuduotai.top/gtysmzkgnm.html

================================================================================
来源：http://hz.tian-w.cn/gtdvpiwlyz.html

C. 函数与作用域
来源：http://hz.jyoumei.cn/gtvphhasfq.html

================================================================================
来源：http://hz.kuanghao11.cn/gtcestejmy.html

[C01] 定义函数
来源：http://hz.yangfankeji.com/gtvqlngcgx.html

Py:   def add(a, b): return a + b
来源：http://hz.sxryk.cn/gtmqbqdhwv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ydjk.org.cn/gtftpvdpej.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.jyoumei.cn/gttjslzeoq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.aizwys.cn/gtxgyludfk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.sxryk.cn/gtetavzoly.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yj20258.top/gtafkesrxu.html

Ruby: def add(a, b); a + b; end
来源：http://hz.jqgfzy.top/gtdgdegfvb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zhiwuduotai.top/gtvcioqktq.html

[C02] 默认参数
来源：http://hz.snrcjt.cn/gtoxqviuvt.html

Py:   def greet(name="World"): return name
来源：http://hz.andypj.xyz/gtkrpbtnif.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.redwolf501.top/gtmufcicyb.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.andypj.xyz/gtmsphnivj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.jqgfzy.top/gtqsplohct.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.xinyue.icu/gtxqzhtiyj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.jinghuilouyu.cn/gtoqxxqvyz.html

Ruby: def greet(name = "World") = name
来源：http://hz.andypj.xyz/gtbsppsctc.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.guannengcc.top/gtohqwwgjp.html

[C03] 可变参数
来源：http://hz.iojbl.cn/gtcpmwzyzj.html

Py:   def total(*args): return sum(args)
来源：http://hz.shuidangran.top/gttlikxydi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.sufxvd.cn/gtmuvaqmps.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hongshengwenyu.top/gtmeosmsvi.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jqgufenzy.top/gtmzsiupub.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.jinghuilouyu.cn/gtgldoahgx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.0kj1m.cn/gtvpylqtjl.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.nanxuanxn.top/gtkbcpsmtp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xingfuxueyuan.xyz/gtkqulxsuj.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hnqzz.top/gtmffpwcou.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.0kj1m.cn/gtcjcvsqcf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.sxryk.cn/gtnjambgei.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.yangfankeji.com/gtbrvwfhbg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jinghuilouyu.cn/gtkwyxbsrv.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.gotoacloud.top/gttourqsyr.html

Go:   // 无：用配置结构体参数
来源：http://hz.iojbl.cn/gtfczxrabi.html

Ruby: f(a: 1, b: 2)
来源：http://hz.gotoacloud.top/gtymwexuqs.html

C#:   f(a: 1, b: 2)
来源：http://hz.pengpengdd.cyou/gttisijctu.html

[C05] 返回多个值
来源：http://hz.yuxming.cn/gtqopzlnii.html

Py:   return a, b
来源：http://hz.wangshuangyany.cn/gtojkgbuwp.html

PHP:  return [$a, $b];
来源：http://hz.zhengqikj.top/gtrktebijt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhixingplan.top/gtvlndrhtl.html

TS:   return { a, b };
来源：http://hz.c1oappe.top/gtsbobiunj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.cheryme.top/gtpubrwher.html

Go:   return a, b
来源：http://hz.aibaodan.cn/gtvwlpoahm.html

Ruby: return a, b
来源：http://hz.iojbl.cn/gtydggtsir.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jinghuilouyu.cn/gtfrvqyizy.html

[C06] 匿名函数 / lambda
来源：http://hz.ydjk.org.cn/gtabcxwyqf.html

Py:   square = lambda x: x * x
来源：http://hz.yuxming.cn/gtgdgegyud.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zycfv.cn/gtatvopbek.html

JS:   const square = x => x * x;
来源：http://hz.yonumen.top/gtdudzpdwt.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.xingfuxueyuan.xyz/gtnihevtlo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.sweek.top/gtwxnfkvtl.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zdqjudy.top/gtlkddypfh.html

Ruby: square = ->(x) { x * x }
来源：http://hz.aibaodan.cn/gtkbdzhjst.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.gzhubu.top/gtnieayszs.html

[C07] 把函数作为参数传入
来源：http://hz.chenlongwang.top/gtvulbnijc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.birdmap.top/gthefecuog.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.dashuyun.cn/gthdfbdaag.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hfpthk.cn/gtsdnqjokf.html

TS:   arr.map(String)
来源：http://hz.xinyue.icu/gtlhafxnfv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.xuetiantiany.cn/gtncyozkap.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.guannengcc.top/gtqvyrkpfa.html

Ruby: arr.map(&:upcase)
来源：http://hz.aibaodan.cn/gtgizqbehg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.zhiwuduotai.top/gtxkkzxidv.html

[C08] 闭包
来源：http://hz.yvedp.cn/gtpbpbozej.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.gotoacloud.top/gtyclcmqon.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.smart0.xyz/gtohonqtxw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.kuanghao11.cn/gtirhasore.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.cqqwz.cn/gtlgcjaowv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ivvv.top/gtqiwgrrzw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hnxiangtu.top/gterhgdllk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.redwolf501.top/gtsknpbiuj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jqgufenzy.top/gtkfwvybwd.html

[C09] 递归
来源：http://hz.meibo888.top/gtcxcgocvy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ppjwa.cn/gtishclakq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.316326.xyz/gthpdetbyp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.vqdsnc.cn/gtioccxvvc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinyuanbaomall.cn/gtwxcupuyu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.jqgfzy.top/gtbwnqbyzv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.hysaishi.cn/gtltqhspif.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.daria6918.cn/gtaekzkhvj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.snrcjt.cn/gtqcgrmuvm.html

[C10] 变量作用域
来源：http://hz.jinqigufen.top/gtpchuznxb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.tanke756.top/gtjaccrygz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yueranfly.top/gtedisldlc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ybcxt.top/gtyytiylsb.html

TS:   同 JS
来源：http://hz.ehwqpu.com/gtcaicyjar.html

Java: 方法内为块级作用域
来源：http://hz.zhaomingkeji.xyz/gtixlqaidd.html

Go:   花括号块级作用域
来源：http://hz.zhiwuduotai.top/gtmdjkbpdy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.shanyushiyangkeji.top/gtkdzovzde.html

C#:   块级作用域
来源：http://hz.bjfxy.top/gtrgxhnaqq.html

[C11] 模块导入与导出
来源：http://hz.zhongyouzk.top/gtabdfbhsc.html

Py:   from module import func
来源：http://hz.hysaishi.cn/gtllviwmwk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ehwqpu.com/gtmgotnuwg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.chenlongwang.top/gtyfqoutfv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.gaohongyu789.top/gttqunyjgk.html

Java: import java.util.List;
来源：http://hz.yuxming.cn/gtuivnxbmt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ydjk.org.cn/gtbrlvlzux.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jinqigfzy.top/gtdkndqhmt.html

C#:   using System.Text;
来源：http://hz.smart0.xyz/gtzpdaypco.html

[C12] 立即执行函数 IIFE
来源：http://hz.quarkkingdee.top/gtprkgqvlb.html

Py:   (lambda: print("run"))()
来源：http://hz.kuanghao11.cn/gtlyeeumyz.html

PHP:  (function () { echo "run"; })();
来源：http://hz.xinyue.icu/gtktgdujzr.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hywenlv.cn/gtzfqskrpx.html

TS:   (() => { console.log("run"); })();
来源：http://hz.havefunace.top/gthabxpncg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xingfuxueyuan.xyz/gtojwaoail.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.c1oappe.top/gtmanemhxw.html

Ruby: -> { puts "run" }.call
来源：http://hz.nanxinkj.top/gtmpjadkny.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhoulong.xyz/gtuimytxul.html

[C13] 类型声明 / 类型注解
来源：http://hz.fengsongda.top/gtslhvpsvv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yvedp.cn/gtnjjsbbxa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.daria6918.cn/gtpierhldi.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.0kj1m.cn/gtcwygazbt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.quarkkingdee.top/gttknefjph.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.fengsongda.top/gtuftlkopp.html

Go:   func add(a, b int) int
来源：http://hz.yj20258.top/gthqtjppls.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.gzhubu.top/gtbqghjsza.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.haohaochexian.top/gtwfnaoahp.html

[C14] 泛型函数
来源：http://hz.zhiwuduotai.top/gtfgoyzovl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhijiandao.cn/gtijnqoirh.html

PHP:  // 无泛型
来源：http://hz.birdmap.top/gtxzhkuift.html

JS:   // 无泛型
来源：http://hz.jianghu66.top/gtovopxoyt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.guowangkeji.top/gtxhvhuufm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.bjfxy.top/gthnhlesko.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhoulong.xyz/gtunijzuvl.html

Ruby: # 无泛型
来源：http://hz.haohaochexian.top/gtllszvrnv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zdqjudy.top/gtefrqemmo.html

[C15] 解构 / 展开参数
来源：http://hz.cucudq.cn/gtfmievwtr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhengqikj.top/gtxaopppov.html

PHP:  [$a, $b] = $pair;
来源：http://hz.52xcode.cn/gtccfammxa.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.daria6918.cn/gtyoxkdyfz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhongyouzk.top/gtsamsrtkn.html

Java: // 无解构
来源：http://hz.cashguo.top/gtyhxigxvp.html

Go:   // 无解构
来源：http://hz.yj20258888.top/gtziudctcy.html

Ruby: a, b = pair
来源：http://hz.jlsjyb.cn/gtkvsafatp.html

C#:   var (a, b) = pair;
来源：http://hz.guannengcc.top/gtiryeqyyq.html

[C16] 函数 / 方法重载
来源：http://hz.feifeiyinyue.top/gtfuzbmlpt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.aibaodan.cn/gttvrxiuik.html

PHP:  // 无重载
来源：http://hz.sufxvd.cn/gtvudkqomm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ivvv.top/gtteazawxn.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.cqqwz.cn/gtqtkufrea.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.snrcjt.cn/gtkeescvxn.html

Go:   // 无重载：用不同函数名
来源：http://hz.0kj1m.cn/gtfezbtmwz.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ehwqpu.com/gtnxrduchf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jinyuanbaomall.cn/gttulmthks.html

================================================================================
来源：http://hz.ydzc1.top/gtnuimfgpz.html

D. 数组 / 列表 / 集合
来源：http://hz.yj20258888.top/gtbtnxwxcd.html

================================================================================
来源：http://hz.zdqjudy.top/gtxehaojzg.html

[D01] 创建数组 / 列表
来源：http://hz.hnxiangtu.top/gtkdxjqigq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.52xcode.cn/gtbcjybtmw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhengqikj.top/gtciqvkrmq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhoulong.xyz/gtsrdyutkz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.shzxlz.cn/gtirexptpz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ydzc1.top/gtagdguiry.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.52xcode.cn/gtkxjgdtwe.html

Ruby: arr = [1, 2, 3]
来源：http://hz.aizwys.cn/gtvxjtjhhf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.cheryme.top/gturtuwwnr.html

[D02] 追加元素到末尾
来源：http://hz.nanxinkj.top/gtozhbhgpn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.nwbrower.top/gtecuvcdkj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.andypj.xyz/gtxdhfjzge.html

JS:   arr.push(4);
来源：http://hz.kuanghao11.cn/gtchmvgwsh.html

TS:   arr.push(4);
来源：http://hz.jyoumei.cn/gtuumiluxk.html

Java: list.add(4);
来源：http://hz.zhiwuduotai.top/gtecpvsowq.html

Go:   arr = append(arr, 4)
来源：http://hz.mhx1999.top/gttmdztuog.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.svipenyu.cn/gtfnvdoanw.html

C#:   list.Add(4);
来源：http://hz.jinqigufen.top/gtbqjypcpp.html

[D03] 在指定位置插入元素
来源：http://hz.xziqi.cn/gtifvdondb.html

Py:   arr.insert(0, 0)
来源：http://hz.shanyushiyangtech.top/gtftpvxlzm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.xingfuxueyuan.xyz/gtmbttoxiv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ybcxt.top/gtgdrnimpt.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hongshengwenyu.top/gthajdzczl.html

Java: list.add(0, 0);
来源：http://hz.xylfe.cn/gtyxubuxnr.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.nanxuanxn.top/gtoqgpnxhn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.havefunace.top/gttglnwxjj.html

C#:   list.Insert(0, 0);
来源：http://hz.tian-w.cn/gthmrfrelr.html

[D04] 删除元素
来源：http://hz.xinyue.icu/gtrednsfop.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.birdmap.top/gtgpsrzyfd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hnqzz.top/gtxdpxxjgt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.iojbl.cn/gtdmpcvmgc.html

TS:   arr.splice(0, 1);
来源：http://hz.jinqigfzy.top/gtdydoqjwu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.wangshuangyany.cn/gtkxkpmmir.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hongshengwenyu.top/gtoyveldcp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zdqjudy.top/gtoxvvotoq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shanyushiyangtech.top/gtpyaekjdb.html

[D05] 访问与修改元素
来源：http://hz.sweek.top/gtromjiqni.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xingfuxueyuan.xyz/gtvhgrirov.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.wangshuangyany.cn/gtjaujvjqk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xziqi.cn/gtxkdcadjv.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.gzhubu.top/gtppskwzur.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ehwqpu.com/gtmletqnuj.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.andypj.xyz/gtzyngykdu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhengqikj.top/gtusslgjgo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinghuilouyu.cn/gtogenktrq.html

[D06] 数组长度
来源：http://hz.316326.xyz/gtonyrzaen.html

Py:   len(arr)
来源：http://hz.tian-w.cn/gtuyttkygs.html

PHP:  count($arr);
来源：http://hz.hnxiangtu.top/gtsdlcxjsh.html

JS:   arr.length
来源：http://hz.xuanzx.com/gtqxyoteux.html

TS:   arr.length
来源：http://hz.gzhubu.top/gtnziiboyx.html

Java: list.size();
来源：http://hz.yj202588.top/gtvxptpeit.html

Go:   len(arr)
来源：http://hz.andypj.xyz/gtdypujsvp.html

Ruby: arr.length; arr.size
来源：http://hz.52xcode.cn/gtlttraqvh.html

C#:   list.Count;
来源：http://hz.yj202588.top/gtqhtqggfw.html

[D07] 切片 / 取子数组
来源：http://hz.gzhubu.top/gtwlcqkdmq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.sufxvd.cn/gtavltzcub.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.bjfxy.top/gtaworuvef.html

JS:   arr.slice(1, 4);
来源：http://hz.yuxming.cn/gttcgvkhtz.html

TS:   arr.slice(1, 4);
来源：http://hz.zhongyouzk.top/gtlusemwua.html

Java: list.subList(1, 4);
来源：http://hz.hnqzz.top/gtiqrfhkhq.html

Go:   arr[1:4]
来源：http://hz.cdnleiting.top/gtlolgwpjb.html

Ruby: arr[1, 3]
来源：http://hz.chenjidiqi.icu/gtnvmpoawi.html

C#:   list.GetRange(1, 3);
来源：http://hz.jqgfzy.top/gtdyeefmrc.html

[D08] 合并两个数组
来源：http://hz.jinghuilouyu.cn/gtpiigrgct.html

Py:   a + b;  a.extend(b)
来源：http://hz.jinghuilouyu.cn/gttymglbzj.html

PHP:  array_merge($a, $b);
来源：http://hz.aibaodan.cn/gtriwiqitc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shanyushiyangkeji.top/gtmliqlboc.html

TS:   [...a, ...b];
来源：http://hz.feifeiyinyue.top/gtrqeejfkg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shangyingyoupin.top/gtoalnjurd.html

Go:   append(a, b...)
来源：http://hz.birdmap.top/gtnrjxctpj.html

Ruby: a + b;  a.concat(b)
来源：http://hz.xingfuxueyuan.xyz/gtghwhqbmw.html

C#:   a.Concat(b).ToList()
来源：http://hz.daria6918.cn/gthirenitf.html

[D09] 排序（升序）
来源：http://hz.zhengqikj.top/gtdhsnxjji.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.tian-w.cn/gtqgapwbed.html

PHP:  sort($arr);
来源：http://hz.yueranfly.top/gtdgseqxpk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yueranfly.top/gthgjnwdxb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.kuanghao11.cn/gtmmmhxjch.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jinqigufen.top/gtrabfjwjx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.sysykeji.top/gtopotbxgx.html

Ruby: arr.sort
来源：http://hz.hammf.cn/gtaiuisexj.html

C#:   list.Sort();
来源：http://hz.hywenlv.cn/gtktzeeftf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zdqjudy.top/gtfbroivnm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.fengsongda.top/gtkuzqosby.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xinyue.icu/gtlbolgeuf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sxryk.cn/gtixetbkuh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xylfe.cn/gtawbctvhw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.quarkkingdee.top/gtvpihjsgy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.gzhubu.top/gtfubofnnz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.feifeiyinyue.top/gtvapjmsqg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cheryme.top/gttchadqlg.html

[D11] 反转数组
来源：http://hz.wangdashe.top/gtkjgvlicg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cheryme.top/gtvjbcarid.html

PHP:  array_reverse($arr);
来源：http://hz.yueranfly.top/gtqxkdahsz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.vqdsnc.cn/gtcvykehsv.html


<!-- 参考信息 -->