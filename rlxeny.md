代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.0kj1m.cn/gtfyojlujs.html

Java: x instanceof Number
来源：http://hz.daxiang520.top/gtpoatundl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.hnqzz.top/gtxxgbazyp.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zycfv.cn/gtyyrgsntf.html

C#:   x is int or double or decimal
来源：http://hz.9152youxi.cn/gtgxkdoisp.html

[B14] 判断值是否在集合内
来源：http://hz.bjfxy.top/gtbhhacpgm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.cdnleiting.top/gtxyqpjqmk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.hysaishi.cn/gtywdscrgw.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.birdmap.top/gtbaigovol.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.feifeiyinyue.top/gtipvmuhta.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.shuidangran.top/gtmqvxpuaw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.ydzc1.top/gtfklgvhtu.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.fzhhl.top/gtzrvllhkw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.tanke756.top/gtqytlpvis.html

[B15] 布尔运算与取反
来源：http://hz.kuanghao11.cn/gtibbambvb.html

Py:   a and b or not c
来源：http://hz.yj202588.top/gteoxcwkyj.html

PHP:  $a && $b || !$c
来源：http://hz.sufxvd.cn/gtnzgebcfo.html

JS:   a && b || !c
来源：http://hz.hfpthk.cn/gtlildvzkx.html

TS:   a && b || !c
来源：http://hz.hammf.cn/gtdfiybqqh.html

Java: a && b || !c
来源：http://hz.xylfe.cn/gtthklsrlm.html

Go:   a && b || !c
来源：http://hz.quarkkingdee.top/gterirrbjz.html

Ruby: a && b || !c
来源：http://hz.jlsjyb.cn/gtjnetnkhk.html

C#:   a && b || !c
来源：http://hz.xuetiantiany.cn/gtysbmtcvn.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.kuanghao11.cn/gtgutnyowo.html

Py:   if not data: return
来源：http://hz.yueranfly.top/gtlqeaygoy.html

PHP:  if (!$data) { return; }
来源：http://hz.daxiang520.top/gtqxmpbkms.html

JS:   if (!data) return;
来源：http://hz.gotoacloud.top/gtaytimwvh.html

TS:   if (!data) return;
来源：http://hz.feifeiyinyue.top/gtrcozarjl.html

Java: if (data == null) return;
来源：http://hz.birdmap.top/gtlndintqr.html

Go:   if data == nil { return }
来源：http://hz.andypj.xyz/gtmqvvfbzd.html

Ruby: return if data.nil?
来源：http://hz.aibaodan.cn/gtyihljyhp.html

C#:   if (data == null) return;
来源：http://hz.smart0.xyz/gtddoluilw.html

================================================================================
来源：http://hz.dianchejie.cn/gttyipvvky.html

C. 函数与作用域
来源：http://hz.cheryme.top/gtgoiwuujp.html

================================================================================
来源：http://hz.yuanzhike.top/gthyxsyryc.html

[C01] 定义函数
来源：http://hz.zycfv.cn/gtsxgbfzwh.html

Py:   def add(a, b): return a + b
来源：http://hz.jianghu66.top/gtczvknevq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.c1oappe.top/gtwlpqmgec.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.gaohongyu789.top/gtfryxtcyy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.mhx1999.top/gtfhrvkrxh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.guannengcc.top/gtzklkkloh.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.yvedp.cn/gtookvxtbb.html

Ruby: def add(a, b); a + b; end
来源：http://hz.hfpthk.cn/gtfoqpxyka.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.sufxvd.cn/gtfzvsywqp.html

[C02] 默认参数
来源：http://hz.9152youxi.cn/gtmdpdlrcr.html

Py:   def greet(name="World"): return name
来源：http://hz.tianlin.xyz/gtxxpycygr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.ydjk.org.cn/gtlnsfibmb.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.xuetiantiany.cn/gtdznripwz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ydzc1.top/gtvhtehrpn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.redwolf501.top/gtckdprpbe.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.sweek.top/gtqhvfjrpe.html

Ruby: def greet(name = "World") = name
来源：http://hz.yangfankeji.com/gtiemcyeli.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.fengsongda.top/gtlhjzrodo.html

[C03] 可变参数
来源：http://hz.kuanghao11.cn/gtlyhgfmcj.html

Py:   def total(*args): return sum(args)
来源：http://hz.pycfn.com/gtwenzjnue.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.sysykeji.top/gtzbvnxgry.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.tianlin.xyz/gtlzeelcfo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cucudq.cn/gtlwyvllhg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.c1oappe.top/gttxhokudj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yonumen.top/gtpohaixma.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.nanxinkj.top/gtnatlayjo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xingfuxueyuan.xyz/gtxdphscpk.html

[C04] 命名参数 / 关键字参数
来源：http://hz.tianlin.xyz/gtdeqvmcur.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.9152youxi.cn/gtayejnetm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.smart0.xyz/gtxprfiwxn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hysaishi.cn/gtmjnsxnjv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.sysykeji.top/gtetynryos.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.chenjidiqi.icu/gtrpylplsh.html

Go:   // 无：用配置结构体参数
来源：http://hz.mhx1999.top/gtysoqeogz.html

Ruby: f(a: 1, b: 2)
来源：http://hz.tianlin.xyz/gtuuyumhnm.html

C#:   f(a: 1, b: 2)
来源：http://hz.hammf.cn/gtbyklebcy.html

[C05] 返回多个值
来源：http://hz.xylfe.cn/gtgtrkhjfe.html

Py:   return a, b
来源：http://hz.hnxiangtu.top/gtmeawrgnq.html

PHP:  return [$a, $b];
来源：http://hz.fzhhl.top/gtitmdfdcm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.daria6918.cn/gtevbopuma.html

TS:   return { a, b };
来源：http://hz.hnxiangtu.top/gtfuykpklh.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.dashuyun.cn/gtwsyxnuop.html

Go:   return a, b
来源：http://hz.wangshuangyany.cn/gtjuyohrjs.html

Ruby: return a, b
来源：http://hz.zhixingplan.top/gtnmducqlc.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.nanxuanxn.top/gtveducuix.html

[C06] 匿名函数 / lambda
来源：http://hz.gogol.net.cn/gtqpumdtwr.html

Py:   square = lambda x: x * x
来源：http://hz.nwbrower.top/gtfzdtmicf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.andypj.xyz/gtmsftywcq.html

JS:   const square = x => x * x;
来源：http://hz.sufxvd.cn/gtahqorcuo.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.yj202588.top/gtidolwjxb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.0kj1m.cn/gtclozqubb.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.zhijiandao.cn/gtsgtdvlkj.html

Ruby: square = ->(x) { x * x }
来源：http://hz.ydjk.org.cn/gtytbhsskr.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.hongshengwenyu.top/gteoikwciq.html

[C07] 把函数作为参数传入
来源：http://hz.xingfuxueyuan.xyz/gtdzcscuwz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.quarkkingdee.top/gtpsgtoflm.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.shanyushiyangtech.top/gtrujftooc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.guannengcc.top/gtfqsalqus.html

TS:   arr.map(String)
来源：http://hz.jlsjyb.cn/gtaviaayhb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ydjk.org.cn/gtonkngpgb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.guowangkeji.top/gtjyqvlnsy.html

Ruby: arr.map(&:upcase)
来源：http://hz.chenzaomai.com/gtvjtyaztx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.smart0.xyz/gtidlkwocx.html

[C08] 闭包
来源：http://hz.pycfn.com/gtmjscodfa.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ivvv.top/gtxgfagltr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhijiandao.cn/gtqxcwprkg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yj20258.top/gtjhgbzujz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.0kj1m.cn/gtuyfqiuwo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yj20258.top/gtojhfkket.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hnxiangtu.top/gtcqphwrvh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.sxryk.cn/gteikrilkg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.tian-w.cn/gtjcppamab.html

[C09] 递归
来源：http://hz.hywenlv.cn/gtemhofpaq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.sweek.top/gtdohivtbq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.chenjidiqi.icu/gtcwxrprmb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xinyue.icu/gttutgtlpo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhengqikj.top/gtzigkkvcz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.ybcxt.top/gtkukngxol.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.xuetiantiany.cn/gtieehpvqb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.fengsongda.top/gtgpprpgpx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hnqzz.top/gtnzlwqobw.html

[C10] 变量作用域
来源：http://hz.zhiwuduotai.top/gtwsmxlepf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.smart0.xyz/gthliidzlx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.gotoacloud.top/gtbxsayqke.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jqgufenzy.top/gtdhfyuylq.html

TS:   同 JS
来源：http://hz.ydjk.org.cn/gttttfaqnl.html

Java: 方法内为块级作用域
来源：http://hz.shanyushiyangtech.top/gtbokomjow.html

Go:   花括号块级作用域
来源：http://hz.daria6918.cn/gtvsrpkdyn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jqgufenzy.top/gtmuoaebwk.html

C#:   块级作用域
来源：http://hz.hongshengwenyu.top/gtdqhrxhvu.html

[C11] 模块导入与导出
来源：http://hz.snrcjt.cn/gtguwbpeqm.html

Py:   from module import func
来源：http://hz.pengpengdd.cyou/gtlpgfeczs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhaomingkeji.xyz/gtjhflzbya.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jinyuanbaomall.cn/gtnbcdhiua.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.sweek.top/gttliesuva.html

Java: import java.util.List;
来源：http://hz.zhengqikj.top/gttwpmlycs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zdqjudy.top/gtwejpavrj.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.shangyingyoupin.top/gtlxejypal.html

C#:   using System.Text;
来源：http://hz.hammf.cn/gtwlxwynat.html

[C12] 立即执行函数 IIFE
来源：http://hz.wangdashe.top/gtzwalxisk.html

Py:   (lambda: print("run"))()
来源：http://hz.ybcxt.top/gtvzbhricv.html

PHP:  (function () { echo "run"; })();
来源：http://hz.hammf.cn/gtkzklfllo.html

JS:   (() => { console.log("run"); })();
来源：http://hz.316326.xyz/gtazwfjmai.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jiagoushi.top/gtkngaruus.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.wangshuangyany.cn/gtalfkcguj.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yj20258888.top/gtrhwnolef.html

Ruby: -> { puts "run" }.call
来源：http://hz.yj202588.top/gtslyflvjb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.sufxvd.cn/gtcrzvoxrr.html

[C13] 类型声明 / 类型注解
来源：http://hz.wangdashe.top/gtjbafbwwp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.tian-w.cn/gteymirgoq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sweek.top/gtmamfxtjz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cheryme.top/gtdtkvuxax.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xingfuxueyuan.xyz/gtpamcasfg.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.yangfankeji.com/gtiwwckjmy.html

Go:   func add(a, b int) int
来源：http://hz.yueranfly.top/gtstdxoybf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.tanke756.top/gtjorvsbiy.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.sxryk.cn/gtjwsixvfe.html

[C14] 泛型函数
来源：http://hz.gotoacloud.top/gtvracjdzi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zdqjudy.top/gtjskavgpt.html

PHP:  // 无泛型
来源：http://hz.shuidangran.top/gtgpqrjxmz.html

JS:   // 无泛型
来源：http://hz.gzhubu.top/gtlalwmwlr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yanxiufei.cn/gtbdqsusmj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.chenzaomai.com/gtarmzljer.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ybcxt.top/gtiprwlmev.html

Ruby: # 无泛型
来源：http://hz.aibaodan.cn/gtlwsbhgts.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.guannengcc.top/gtklrvmkqd.html

[C15] 解构 / 展开参数
来源：http://hz.yj20258888.top/gtebaqhtnl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yvedp.cn/gtdanrbeah.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yj202588.top/gtquwfujny.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.quarkkingdee.top/gtlysihnou.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ppjwa.cn/gtdbiqcrte.html

Java: // 无解构
来源：http://hz.quarkkingdee.top/gtkfifptcd.html

Go:   // 无解构
来源：http://hz.jqgfzy.top/gtoutwcrvs.html

Ruby: a, b = pair
来源：http://hz.jiagoushi.top/gtkrspnqsr.html

C#:   var (a, b) = pair;
来源：http://hz.yuanzhike.top/gtioqhcsla.html

[C16] 函数 / 方法重载
来源：http://hz.nwbrower.top/gtvmsfrudh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.feifeiyinyue.top/gthvkbfcit.html

PHP:  // 无重载
来源：http://hz.jyoumei.cn/gtwkskiayi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.tian-w.cn/gtfkagbtqr.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhengqikj.top/gtxhdovhyh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.c1oappe.top/gtwnuduehj.html

Go:   // 无重载：用不同函数名
来源：http://hz.snrcjt.cn/gtehatfwik.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xziqi.cn/gtiskqkxsh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.birdmap.top/gtdbqjzyak.html

================================================================================
来源：http://hz.aibaodan.cn/gtxzufqcjt.html

D. 数组 / 列表 / 集合
来源：http://hz.shzxlz.cn/gtmzybtara.html

================================================================================
来源：http://hz.xylfe.cn/gtqrrghyga.html

[D01] 创建数组 / 列表
来源：http://hz.zhixingplan.top/gttigbpwbf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jiagoushi.top/gtlqmdvxga.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.fengsongda.top/gtskhtzznn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.tianlin.xyz/gttdkzbqiv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.tanke756.top/gtmglfntvn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xuanzx.com/gtbrwcacjn.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.kuanghao11.cn/gtnkgvuiaf.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yangfankeji.com/gtokekrwji.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.mhx1999.top/gtcuciymzj.html

[D02] 追加元素到末尾
来源：http://hz.shangyingyoupin.top/gttkofrfeg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.guowangkeji.top/gtrzxvnzhf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shzxlz.cn/gtyhezlsgf.html

JS:   arr.push(4);
来源：http://hz.shanyushiyangkeji.top/gtnauzfpqi.html

TS:   arr.push(4);
来源：http://hz.shanyushiyangkeji.top/gthyjwtsdi.html

Java: list.add(4);
来源：http://hz.hongshengwenyu.top/gtjlztxqyx.html

Go:   arr = append(arr, 4)
来源：http://hz.hysaishi.cn/gtkikvbcns.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.havefunace.top/gtcfshjcqo.html

C#:   list.Add(4);
来源：http://hz.hongshengwenyu.top/gtuxwvhuim.html

[D03] 在指定位置插入元素
来源：http://hz.pengpengdd.cyou/gtvyodrkyn.html

Py:   arr.insert(0, 0)
来源：http://hz.shuidangran.top/gtsysitumt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhoulong.xyz/gtrwiplfto.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.ywan-chungtsiang.top/gtvwtnauga.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yuxming.cn/gtwpksjroa.html

Java: list.add(0, 0);
来源：http://hz.xuetiantiany.cn/gtcuvjarng.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yj202588.top/gtjihanwre.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.gzhubu.top/gtbrlvlhtp.html

C#:   list.Insert(0, 0);
来源：http://hz.hammf.cn/gtcuiprpbu.html

[D04] 删除元素
来源：http://hz.birdmap.top/gtaijuxgyd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.aibaodan.cn/gtazksmsxv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hnxiangtu.top/gthvhhuwen.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.9152youxi.cn/gtjbjnuryy.html

TS:   arr.splice(0, 1);
来源：http://hz.chenlongwang.top/gtosyovdiz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yonumen.top/gtewqcqzyb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.gogol.net.cn/gtoptunnuu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.316326.xyz/gtvplwfvef.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.svipenyu.cn/gtrxjaugup.html

[D05] 访问与修改元素
来源：http://hz.guowangkeji.top/gtcnivaste.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jiagoushi.top/gtoydonfao.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sxryk.cn/gtppaeaovo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.dianchejie.cn/gtschhvlbg.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hammf.cn/gthmzjskxh.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yueranfly.top/gtftlmibcn.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cdnleiting.top/gtfkhxnegw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xuanzx.com/gthkvhpmaj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ivvv.top/gtsqkwmgyw.html

[D06] 数组长度
来源：http://hz.ppjwa.cn/gtfknpmuob.html

Py:   len(arr)
来源：http://hz.c1oappe.top/gtiigjlskn.html

PHP:  count($arr);
来源：http://hz.gaohongyu789.top/gteteswdrq.html

JS:   arr.length
来源：http://hz.dianchejie.cn/gtbfhcvvkg.html

TS:   arr.length
来源：http://hz.havefunace.top/gtnlruckyb.html

Java: list.size();
来源：http://hz.ivvv.top/gtcfyjdhrq.html

Go:   len(arr)
来源：http://hz.yuxming.cn/gtxoveriiy.html

Ruby: arr.length; arr.size
来源：http://hz.ydjk.org.cn/gtfppxlpzt.html

C#:   list.Count;
来源：http://hz.yonumen.top/gtaxxouall.html

[D07] 切片 / 取子数组
来源：http://hz.yuxming.cn/gtstcjsrjb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.andypj.xyz/gtqeafkljo.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xuanzx.com/gtyxzdoryl.html

JS:   arr.slice(1, 4);
来源：http://hz.zhengqikj.top/gtlxbzjqvk.html

TS:   arr.slice(1, 4);
来源：http://hz.andypj.xyz/gtbgxqjehw.html

Java: list.subList(1, 4);
来源：http://hz.zhixingplan.top/gtotuyvdbc.html

Go:   arr[1:4]
来源：http://hz.gogol.net.cn/gtgcpfhagr.html

Ruby: arr[1, 3]
来源：http://hz.yonumen.top/gtsxspjzbm.html

C#:   list.GetRange(1, 3);
来源：http://hz.xziqi.cn/gtfurbzmew.html

[D08] 合并两个数组
来源：http://hz.9152youxi.cn/gtsrhezvbb.html

Py:   a + b;  a.extend(b)
来源：http://hz.xinyue.icu/gtjhpjqhwb.html

PHP:  array_merge($a, $b);
来源：http://hz.dashuyun.cn/gtkrkaystz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.52xcode.cn/gtkolwgdfj.html

TS:   [...a, ...b];
来源：http://hz.hfpthk.cn/gtuntbjwuf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhengqikj.top/gtngsogunz.html

Go:   append(a, b...)
来源：http://hz.yj202588.top/gtmlrsvvzo.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hnqzz.top/gtptzustcy.html

C#:   a.Concat(b).ToList()
来源：http://hz.mhx1999.top/gtffpqdvyz.html

[D09] 排序（升序）
来源：http://hz.zhixingplan.top/gtdyxtyzch.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinqigufen.top/gtwnjvjnco.html

PHP:  sort($arr);
来源：http://hz.yueranfly.top/gtodaucoax.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xuetiantiany.cn/gthdpodgkd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.fengsongda.top/gtgorcdmdr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.wangdashe.top/gtcdfmuafy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.mhx1999.top/gtcflfvbch.html

Ruby: arr.sort
来源：http://hz.chenzaomai.com/gtthyjmius.html

C#:   list.Sort();
来源：http://hz.hammf.cn/gtybwvgduy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.andypj.xyz/gtrsyenjsk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.9152youxi.cn/gtqbdvwaqh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.havefunace.top/gtrisvqvja.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.bjfxy.top/gtpltfmpdd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.0kj1m.cn/gtunuaumse.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cashguo.top/gtsncpthdc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.guannengcc.top/gtswghkpyj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jiagoushi.top/gtworxlzom.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhaomingkeji.xyz/gtzpdjqzsy.html

[D11] 反转数组
来源：http://hz.nanxinkj.top/gtrzypyfnp.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yueranfly.top/gttkzqedob.html

PHP:  array_reverse($arr);
来源：http://hz.nwbrower.top/gtlsvvrrhe.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jlsjyb.cn/gttkaecsoa.html

TS:   [...arr].reverse();
来源：http://hz.jinqigufen.top/gtlijkadmp.html

Java: Collections.reverse(list);
来源：http://hz.jinghuilouyu.cn/gttbpxgfbu.html

Go:   slices.Reverse(arr)
来源：http://hz.cashguo.top/gtjinuaphz.html

Ruby: arr.reverse
来源：http://hz.yuxming.cn/gtnufksxbf.html

C#:   list.Reverse();
来源：http://hz.wangshuangyany.cn/gtildhxgxj.html

[D12] 查找元素下标
来源：http://hz.kuanghao11.cn/gtuwymanmp.html

Py:   arr.index(x);  x in arr
来源：http://hz.0kj1m.cn/gtcdmeziwn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.tianlin.xyz/gtdsluecxd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinqigfzy.top/gtvyefowfd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.havefunace.top/gtdvkkcmbg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.0kj1m.cn/gteybeyewn.html

Go:   slices.Index(arr, x)
来源：http://hz.xinyue.icu/gtwwfspzdy.html

Ruby: arr.index(x)
来源：http://hz.shangyingyoupin.top/gtnwyxembu.html

C#:   list.IndexOf(x);
来源：http://hz.hongshengwenyu.top/gtmiipihhr.html

[D13] 过滤（保留满足条件的）
来源：http://hz.haohaochexian.top/gtsgwvsarz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.xingfuxueyuan.xyz/gtybqzywbr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jqgfzy.top/gtibsfkicx.html

JS:   arr.filter(x => x > 3)
来源：http://hz.sufxvd.cn/gtcmyexjsn.html

TS:   arr.filter(x => x > 3)
来源：http://hz.cashguo.top/gtdmwgceom.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.c1oappe.top/gtjqycjcld.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ehwqpu.com/gtsgumfqst.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.guowangkeji.top/gtzbdlqepa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.chenjidiqi.icu/gtepuukdna.html

[D14] 映射转换（每个元素变形）
来源：http://hz.316326.xyz/gtjqusgkaj.html


<!-- 参考信息 -->