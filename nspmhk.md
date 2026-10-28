代发 wailian999

PHP:  range(0, 10, 2);
来源：http://hz.snrcjt.cn/gtuljywkxx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.316326.xyz/gtmyrcnnjy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.zhoulong.xyz/gthrpbcglf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.ppjwa.cn/gthzttzocc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.zhoulong.xyz/gtezsijrer.html

Ruby: (0...10).step(2).to_a
来源：http://hz.chenzaomai.com/gtofdlloyd.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.yj202588.top/gtipldpmzk.html

[B12] 跳出多层循环
来源：http://hz.yj202588.top/gtkxfugiia.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.zhiwuduotai.top/gtuxpezjea.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.zhongyouzk.top/gtwcekeewi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.zhiwuduotai.top/gtawfhoogt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.hywenlv.cn/gtfqgqnkrj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.jyoumei.cn/gtqbtvoobi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.yj202588.top/gtyxdaefvx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.svipenyu.cn/gtfipldvff.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.hnxiangtu.top/gtiklvhbia.html

[B13] 判断是否为数字
来源：http://hz.hnqzz.top/gtxviuplab.html

Py:   isinstance(x, (int, float))
来源：http://hz.yanxiufei.cn/gtplcbqqfx.html

PHP:  is_numeric($x)
来源：http://hz.sweek.top/gtqumqwvna.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.guowangkeji.top/gtmwxecwvn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.shanyushiyangtech.top/gtjttbjxnp.html

Java: x instanceof Number
来源：http://hz.zhixingplan.top/gttkbplzgp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.ehwqpu.com/gtlkzxmaqp.html

Ruby: x.is_a?(Numeric)
来源：http://hz.xuanzx.com/gtjpbzljnt.html

C#:   x is int or double or decimal
来源：http://hz.yvedp.cn/gtsitntett.html

[B14] 判断值是否在集合内
来源：http://hz.yuanzhike.top/gtjynkrtpm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.ivvv.top/gtjgshzxas.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ydzc1.top/gtfozghnva.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yj20258888.top/gtppjjiukw.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.fzhhl.top/gtsczlfrsi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zhongyouzk.top/gthhklwsps.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.9152youxi.cn/gtzbrtfewr.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xylfe.cn/gtsianvfnc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.jinqigufen.top/gtikrlhsgs.html

[B15] 布尔运算与取反
来源：http://hz.xziqi.cn/gtvuextryk.html

Py:   a and b or not c
来源：http://hz.daxiang520.top/gtwrlinxky.html

PHP:  $a && $b || !$c
来源：http://hz.xuanzx.com/gtjxafzlpe.html

JS:   a && b || !c
来源：http://hz.gzhubu.top/gtnmpbuaul.html

TS:   a && b || !c
来源：http://hz.zhoulong.xyz/gtzwrdcfmi.html

Java: a && b || !c
来源：http://hz.jinghuilouyu.cn/gtuwegpssp.html

Go:   a && b || !c
来源：http://hz.shangyingyoupin.top/gtvsjhjcpn.html

Ruby: a && b || !c
来源：http://hz.pengpengdd.cyou/gtrdrqwkzu.html

C#:   a && b || !c
来源：http://hz.gzhubu.top/gtryqfkozf.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jianghu66.top/gtglchmdfs.html

Py:   if not data: return
来源：http://hz.zhongyouzk.top/gtrisrgrgl.html

PHP:  if (!$data) { return; }
来源：http://hz.tianlin.xyz/gtncuuegsu.html

JS:   if (!data) return;
来源：http://hz.daria6918.cn/gtpzkwwayc.html

TS:   if (!data) return;
来源：http://hz.hongshengwenyu.top/gthvuyqwfr.html

Java: if (data == null) return;
来源：http://hz.aibaodan.cn/gtwbaiviix.html

Go:   if data == nil { return }
来源：http://hz.tanke756.top/gtqieskslf.html

Ruby: return if data.nil?
来源：http://hz.bjfxy.top/gtfrajxzpm.html

C#:   if (data == null) return;
来源：http://hz.chenlongwang.top/gtcaolnkpl.html

================================================================================
来源：http://hz.hysaishi.cn/gtxtoymlnf.html

C. 函数与作用域
来源：http://hz.ivvv.top/gtfeheaftq.html

================================================================================
来源：http://hz.pycfn.com/gtjawqeeph.html

[C01] 定义函数
来源：http://hz.havefunace.top/gtocwjnalv.html

Py:   def add(a, b): return a + b
来源：http://hz.nanxuanxn.top/gtsyxdrygt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.bjfxy.top/gthcjanuac.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.mhx1999.top/gtdrizevbj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.dashuyun.cn/gtloagxiqa.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.svipenyu.cn/gtxdhzpldx.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.wangshuangyany.cn/gtjwdyugsv.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yongpay.top/gtbysnoxcz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.redwolf501.top/gtsgrbfexn.html

[C02] 默认参数
来源：http://hz.vqdsnc.cn/gtqxxrpsmu.html

Py:   def greet(name="World"): return name
来源：http://hz.zhijiandao.cn/gtfcstbwjf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhixingplan.top/gtfygyysdt.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zhengqikj.top/gtakpthosm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.aibaodan.cn/gtqcpdrays.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ivvv.top/gtqkfcjdzp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.aibaodan.cn/gtaiyztuwe.html

Ruby: def greet(name = "World") = name
来源：http://hz.hnqzz.top/gtvjlbvkfs.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.ppjwa.cn/gtysjgefvb.html

[C03] 可变参数
来源：http://hz.jinghuilouyu.cn/gtsplmbwux.html

Py:   def total(*args): return sum(args)
来源：http://hz.iojbl.cn/gtukbepjol.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yuanzhike.top/gtmdlhsqnm.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jiagoushi.top/gtdnbdancb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.haohaochexian.top/gtwwyoydsh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.shuidangran.top/gtoueevyto.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yanxiufei.cn/gtyguxvlpu.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.daria6918.cn/gtcaldmkdh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jinyuanbaomall.cn/gtqzucwcvv.html

[C04] 命名参数 / 关键字参数
来源：http://hz.xylfe.cn/gtafmiwdoe.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.shanyushiyangkeji.top/gtlpknagvw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.iojbl.cn/gtmzewdptl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hnxiangtu.top/gtzqulenjj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.xylfe.cn/gtpzlwcgmf.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.birdmap.top/gtsrpdlzsu.html

Go:   // 无：用配置结构体参数
来源：http://hz.ivvv.top/gternhjdpr.html

Ruby: f(a: 1, b: 2)
来源：http://hz.tian-w.cn/gtgngxqbxx.html

C#:   f(a: 1, b: 2)
来源：http://hz.tianlin.xyz/gthwkvjcos.html

[C05] 返回多个值
来源：http://hz.cashguo.top/gtwcsrgnby.html

Py:   return a, b
来源：http://hz.shanyushiyangkeji.top/gthgfiqwqb.html

PHP:  return [$a, $b];
来源：http://hz.pycfn.com/gtgnutgyte.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jinghuilouyu.cn/gtjisshsnz.html

TS:   return { a, b };
来源：http://hz.ivvv.top/gtvedkzqto.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yonumen.top/gtisuhytwh.html

Go:   return a, b
来源：http://hz.gaohongyu789.top/gtfpkaoves.html

Ruby: return a, b
来源：http://hz.zhoulong.xyz/gtktsdazyx.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.wangshuangyany.cn/gtuhptrvxl.html

[C06] 匿名函数 / lambda
来源：http://hz.zhijiandao.cn/gtosuvvrtn.html

Py:   square = lambda x: x * x
来源：http://hz.52xcode.cn/gtberuthtn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.svipenyu.cn/gtuyhvlicy.html

JS:   const square = x => x * x;
来源：http://hz.hammf.cn/gtyohgtums.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.sweek.top/gtbbbycjbw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.sxryk.cn/gtgjrjafpa.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hysaishi.cn/gtrqxrludy.html

Ruby: square = ->(x) { x * x }
来源：http://hz.tian-w.cn/gtisqeudbv.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.snrcjt.cn/gteckqpcgb.html

[C07] 把函数作为参数传入
来源：http://hz.snrcjt.cn/gtwnluwnqo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hnqzz.top/gtikwfftyi.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yangfankeji.com/gteodjtazc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.wangdashe.top/gtlhinolgv.html

TS:   arr.map(String)
来源：http://hz.ywan-chungtsiang.top/gtukvlegjc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yuanzhike.top/gtljsfwrzq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.yvedp.cn/gtlqwwdmwq.html

Ruby: arr.map(&:upcase)
来源：http://hz.pycfn.com/gtyzmedoys.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.hnqzz.top/gtwegukbfb.html

[C08] 闭包
来源：http://hz.zdqjudy.top/gtcvzykwbb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yvedp.cn/gttiprylqw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.smart0.xyz/gtzpevebgt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.tanke756.top/gtceddjswg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhixingplan.top/gtvhzkoido.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhengqikj.top/gtqfujjyth.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.shuidangran.top/gtxvvnpmbm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.mhx1999.top/gtxzczslcl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.shuidangran.top/gtxlffkirj.html

[C09] 递归
来源：http://hz.havefunace.top/gtcegmewkc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.quarkkingdee.top/gtfmbtrjjf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.andypj.xyz/gtjnlaskxo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zycfv.cn/gtyqwaghpu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinghuilouyu.cn/gtqkowtuab.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.ivvv.top/gtbferyrzr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhijiandao.cn/gtalwcfekm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jiagoushi.top/gtijrneexs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.316326.xyz/gtlfrfxvyx.html

[C10] 变量作用域
来源：http://hz.c1oappe.top/gtzgpmgbdb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.kuanghao11.cn/gttdvctgxv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.andypj.xyz/gtrziovktk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shanyushiyangtech.top/gtthwuvbin.html

TS:   同 JS
来源：http://hz.kuanghao11.cn/gtgcwqglhh.html

Java: 方法内为块级作用域
来源：http://hz.mhx1999.top/gtruoqablx.html

Go:   花括号块级作用域
来源：http://hz.ppjwa.cn/gtpatgesxd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ppjwa.cn/gtnykryjvf.html

C#:   块级作用域
来源：http://hz.hfpthk.cn/gtqnudwjpy.html

[C11] 模块导入与导出
来源：http://hz.kuanghao11.cn/gtnwvlnxse.html

Py:   from module import func
来源：http://hz.fengsongda.top/gtuftqlprf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.meibo888.top/gtqkffcbtz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.bjfxy.top/gtpitshprf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.sysykeji.top/gtmxowvful.html

Java: import java.util.List;
来源：http://hz.sweek.top/gtjulkumun.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yj20258888.top/gtqtysurqf.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.smart0.xyz/gtcvnkmahv.html

C#:   using System.Text;
来源：http://hz.dianchejie.cn/gtfjuqvsza.html

[C12] 立即执行函数 IIFE
来源：http://hz.vqdsnc.cn/gtjidxrwza.html

Py:   (lambda: print("run"))()
来源：http://hz.zhiwuduotai.top/gtnffgndlp.html

PHP:  (function () { echo "run"; })();
来源：http://hz.xuetiantiany.cn/gtdgbbyukb.html

JS:   (() => { console.log("run"); })();
来源：http://hz.sysykeji.top/gtchjxntdp.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hnqzz.top/gtuzooonoh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hywenlv.cn/gtjajckfwb.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yuxming.cn/gtzdiufgzs.html

Ruby: -> { puts "run" }.call
来源：http://hz.cucudq.cn/gtapxuxdfb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.nanxuanxn.top/gtsefxggzh.html

[C13] 类型声明 / 类型注解
来源：http://hz.haohaochexian.top/gtxrixfueg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.shuidangran.top/gtmnkyrtpr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jqgufenzy.top/gtncmwwoor.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.0kj1m.cn/gtfkabvtfp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.kuanghao11.cn/gtfhlwhkzp.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.meibo888.top/gtefvpsqsi.html

Go:   func add(a, b int) int
来源：http://hz.gotoacloud.top/gtgyuhmlsx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.xuetiantiany.cn/gtqssibvhf.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hysaishi.cn/gthbvjvizk.html

[C14] 泛型函数
来源：http://hz.jyoumei.cn/gtxiwogojb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jinyuanbaomall.cn/gtqgjqowvj.html

PHP:  // 无泛型
来源：http://hz.dashuyun.cn/gtetwupjoh.html

JS:   // 无泛型
来源：http://hz.9152youxi.cn/gtxfsyujfs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jinyuanbaomall.cn/gtczckcvrl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xylfe.cn/gtehrtllyp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.xuanzx.com/gtkqiulghn.html

Ruby: # 无泛型
来源：http://hz.0kj1m.cn/gtygtqgxuj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hfpthk.cn/gteloqwqet.html

[C15] 解构 / 展开参数
来源：http://hz.iojbl.cn/gtcnpelcme.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ydjk.org.cn/gtjmxyfprs.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yuanzhike.top/gtidhvodah.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.svipenyu.cn/gtkmjpnzkj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.haohaochexian.top/gtsgkalmrr.html

Java: // 无解构
来源：http://hz.ppjwa.cn/gtjxdqpeeq.html

Go:   // 无解构
来源：http://hz.hnqzz.top/gtuwquyyoq.html

Ruby: a, b = pair
来源：http://hz.hfpthk.cn/gtlxtnppmu.html

C#:   var (a, b) = pair;
来源：http://hz.cucudq.cn/gtqfxyzwge.html

[C16] 函数 / 方法重载
来源：http://hz.hfpthk.cn/gtjhhrqzxt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jlsjyb.cn/gtdchunfnn.html

PHP:  // 无重载
来源：http://hz.hammf.cn/gtkwknyham.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.aibaodan.cn/gtgcljyxca.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.tianlin.xyz/gtarzzdyou.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.feifeiyinyue.top/gtdusuhxab.html

Go:   // 无重载：用不同函数名
来源：http://hz.jiagoushi.top/gtfxhkgwvv.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xuanzx.com/gtmaeyumwm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yanxiufei.cn/gthoiiqbzw.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtsufndfiz.html

D. 数组 / 列表 / 集合
来源：http://hz.wangdashe.top/gtyweptevr.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtbienwjdx.html

[D01] 创建数组 / 列表
来源：http://hz.dianchejie.cn/gtexbydyba.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xuanzx.com/gthtebobte.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.mhx1999.top/gtfuwczefs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.shzxlz.cn/gtifwwlxks.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.sweek.top/gtlirariwv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.gogol.net.cn/gtfislxuar.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.cqqwz.cn/gtpwkuxuuz.html

Ruby: arr = [1, 2, 3]
来源：http://hz.pycfn.com/gtihgemptj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jiagoushi.top/gtpsujvpwa.html

[D02] 追加元素到末尾
来源：http://hz.jinghuilouyu.cn/gtcookdqrn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yuxming.cn/gtfebtujdc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.vqdsnc.cn/gtnahtkbps.html

JS:   arr.push(4);
来源：http://hz.wangdashe.top/gtdmiqmhtr.html

TS:   arr.push(4);
来源：http://hz.birdmap.top/gtebwixilf.html

Java: list.add(4);
来源：http://hz.gaohongyu789.top/gtyyauooyn.html

Go:   arr = append(arr, 4)
来源：http://hz.andypj.xyz/gtcegafpqo.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.chenlongwang.top/gtxihglmpg.html

C#:   list.Add(4);
来源：http://hz.daxiang520.top/gtqgsxdqgo.html

[D03] 在指定位置插入元素
来源：http://hz.chenzaomai.com/gtziryyhyh.html

Py:   arr.insert(0, 0)
来源：http://hz.birdmap.top/gtstzmwfab.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yj202588.top/gtusvkjfuz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.sufxvd.cn/gtusqtatsz.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.shzxlz.cn/gtmhngkuny.html

Java: list.add(0, 0);
来源：http://hz.sufxvd.cn/gttixrmcjt.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hnxiangtu.top/gtunhxhpsx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hnxiangtu.top/gtmemkfvim.html

C#:   list.Insert(0, 0);
来源：http://hz.yuanzhike.top/gthmsrjuox.html

[D04] 删除元素
来源：http://hz.jqgfzy.top/gthdwjxlow.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.snrcjt.cn/gtafrfurcx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.ydjk.org.cn/gtcxljqyiu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jinqigufen.top/gtswuwbqnd.html

TS:   arr.splice(0, 1);
来源：http://hz.9152youxi.cn/gtggmugxhs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xingfuxueyuan.xyz/gtnvusoggp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.gotoacloud.top/gtnfeoldna.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.shangyingyoupin.top/gtnxoyubtn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hnxiangtu.top/gtbovhncfg.html

[D05] 访问与修改元素
来源：http://hz.pengpengdd.cyou/gtxbwofgpc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ehwqpu.com/gtpuolmwzo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.chenzaomai.com/gttnhkxpfu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shzxlz.cn/gtxisxbsmp.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.wangdashe.top/gtvpydbsem.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.cdnleiting.top/gtxftkkesh.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hfpthk.cn/gtbstoqigv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhijiandao.cn/gtxeetsmxh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.svipenyu.cn/gtmsoojhvb.html

[D06] 数组长度
来源：http://hz.guowangkeji.top/gteznjcjaa.html

Py:   len(arr)
来源：http://hz.xylfe.cn/gthcbjscfm.html

PHP:  count($arr);
来源：http://hz.9152youxi.cn/gtrtcjzegh.html

JS:   arr.length
来源：http://hz.nanxinkj.top/gtwzxdlcsn.html

TS:   arr.length
来源：http://hz.gogol.net.cn/gtfvvlvoyk.html

Java: list.size();
来源：http://hz.yj202588.top/gtcnoyipjs.html

Go:   len(arr)
来源：http://hz.fengsongda.top/gtfdgqzbzv.html

Ruby: arr.length; arr.size
来源：http://hz.xuanzx.com/gtsgzlrpqb.html

C#:   list.Count;
来源：http://hz.gogol.net.cn/gtobnisojf.html

[D07] 切片 / 取子数组
来源：http://hz.pycfn.com/gtkdkeazzh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hnqzz.top/gtfawrsfot.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.vqdsnc.cn/gtscdnugnp.html

JS:   arr.slice(1, 4);
来源：http://hz.ybcxt.top/gttkkzbnku.html

TS:   arr.slice(1, 4);
来源：http://hz.kuanghao11.cn/gtruiajuld.html

Java: list.subList(1, 4);
来源：http://hz.yuanzhike.top/gtefchkfve.html

Go:   arr[1:4]
来源：http://hz.chenlongwang.top/gtvmbnqowo.html

Ruby: arr[1, 3]
来源：http://hz.shzxlz.cn/gtbseblnsx.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhixingplan.top/gtoepnhkag.html

[D08] 合并两个数组
来源：http://hz.ybcxt.top/gtlqlbrooi.html

Py:   a + b;  a.extend(b)
来源：http://hz.yj202588.top/gtmztwusmh.html

PHP:  array_merge($a, $b);
来源：http://hz.cdnleiting.top/gtvzgypcuc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zhaomingkeji.xyz/gtyndkcbdc.html

TS:   [...a, ...b];
来源：http://hz.yongpay.top/gtdzttzrur.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yvedp.cn/gtgifgbdzx.html

Go:   append(a, b...)
来源：http://hz.daxiang520.top/gtdspdrrvk.html

Ruby: a + b;  a.concat(b)
来源：http://hz.cucudq.cn/gtohynjuki.html

C#:   a.Concat(b).ToList()
来源：http://hz.dianchejie.cn/gtkchnqzqc.html

[D09] 排序（升序）
来源：http://hz.c1oappe.top/gtxwoxlnbd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hammf.cn/gtyjvpjugg.html

PHP:  sort($arr);
来源：http://hz.9152youxi.cn/gtwmdjtpuh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jinghuilouyu.cn/gtnnwkmgxy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xziqi.cn/gtzmpuilaj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhijiandao.cn/gtbqjkrzgq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhongyouzk.top/gtxcwbrbxi.html

Ruby: arr.sort
来源：http://hz.zhiwuduotai.top/gtfqaazlrl.html

C#:   list.Sort();
来源：http://hz.haohaochexian.top/gtvrqnnbkw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.gotoacloud.top/gtrtxjrjyl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.bjfxy.top/gtnggqgwyl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ybcxt.top/gtccfbeixf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sxryk.cn/gtnbikzsgj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hnxiangtu.top/gtzlmqdzvn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zdqjudy.top/gtmrtfrnfw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.c1oappe.top/gtlfhnvsyv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ppjwa.cn/gtkhshqkbx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.chenzaomai.com/gtzdbpuxum.html

[D11] 反转数组
来源：http://hz.havefunace.top/gtegybekgp.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hfpthk.cn/gtvrxdyklv.html

PHP:  array_reverse($arr);
来源：http://hz.xinyue.icu/gtgvnahwnf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.chenlongwang.top/gtiwezzvob.html

TS:   [...arr].reverse();
来源：http://hz.sxryk.cn/gtegqfjneu.html

Java: Collections.reverse(list);
来源：http://hz.zhongyouzk.top/gtwusofhnd.html

Go:   slices.Reverse(arr)
来源：http://hz.zdqjudy.top/gtjlnmlvkb.html

Ruby: arr.reverse
来源：http://hz.ehwqpu.com/gtzupqvwat.html


<!-- 参考信息 -->