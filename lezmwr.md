代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://hz.xinyue.icu/gtiptqknee.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.iojbl.cn/gtevttxdjx.html

[B15] 布尔运算与取反
来源：http://hz.zhaomingkeji.xyz/gtgpheswfr.html

Py:   a and b or not c
来源：http://hz.yj20258888.top/gtjiutialw.html

PHP:  $a && $b || !$c
来源：http://hz.yuxming.cn/gtzqeygbbm.html

JS:   a && b || !c
来源：http://hz.dianchejie.cn/gtgjicsslf.html

TS:   a && b || !c
来源：http://hz.haohaochexian.top/gtsvmriudg.html

Java: a && b || !c
来源：http://hz.jinqigfzy.top/gtpcqrptcs.html

Go:   a && b || !c
来源：http://hz.gaohongyu789.top/gtjmpioapq.html

Ruby: a && b || !c
来源：http://hz.xuanzx.com/gtdnzdfakt.html

C#:   a && b || !c
来源：http://hz.fengsongda.top/gthasouuek.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.jinqigufen.top/gtihrnwesv.html

Py:   if not data: return
来源：http://hz.shanyushiyangkeji.top/gtjuqhxhsh.html

PHP:  if (!$data) { return; }
来源：http://hz.yj202588.top/gtzocebagn.html

JS:   if (!data) return;
来源：http://hz.vqdsnc.cn/gtbpugztkt.html

TS:   if (!data) return;
来源：http://hz.ywan-chungtsiang.top/gtmltzfifa.html

Java: if (data == null) return;
来源：http://hz.xuetiantiany.cn/gtipsrbybu.html

Go:   if data == nil { return }
来源：http://hz.meibo888.top/gtvaykccsr.html

Ruby: return if data.nil?
来源：http://hz.ydjk.org.cn/gtffpjeohr.html

C#:   if (data == null) return;
来源：http://hz.smart0.xyz/gttmienuds.html

================================================================================
来源：http://hz.cucudq.cn/gtmicspsyq.html

C. 函数与作用域
来源：http://hz.xingfuxueyuan.xyz/gtesowppoc.html

================================================================================
来源：http://hz.dashuyun.cn/gtqzyxmeha.html

[C01] 定义函数
来源：http://hz.pycfn.com/gtxrpmnmjz.html

Py:   def add(a, b): return a + b
来源：http://hz.cqqwz.cn/gtertzqgls.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.bjfxy.top/gttecvwixo.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.hammf.cn/gtopqjwrps.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.pycfn.com/gttvrgpwgn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.wangdashe.top/gtogcmscvx.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.ywan-chungtsiang.top/gtuwmuefzu.html

Ruby: def add(a, b); a + b; end
来源：http://hz.iojbl.cn/gtlimtnnfe.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.xuetiantiany.cn/gtmuuxkfbg.html

[C02] 默认参数
来源：http://hz.yueranfly.top/gtrwouxyqs.html

Py:   def greet(name="World"): return name
来源：http://hz.hywenlv.cn/gtnbuladey.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.hysaishi.cn/gtqmugbgcw.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.xinyue.icu/gtgdrjxzir.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.gaohongyu789.top/gtodllbsbn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.jinghuilouyu.cn/gtxpckozuy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.sysykeji.top/gtwottwncg.html

Ruby: def greet(name = "World") = name
来源：http://hz.ywan-chungtsiang.top/gtqwxauqih.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.hywenlv.cn/gtcssqjzqs.html

[C03] 可变参数
来源：http://hz.quarkkingdee.top/gtrymqtrib.html

Py:   def total(*args): return sum(args)
来源：http://hz.cucudq.cn/gteahvchth.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.yuanzhike.top/gtwknaikby.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.ywan-chungtsiang.top/gtlgovkfsv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jianghu66.top/gtoqcxlvul.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.chenlongwang.top/gtxklopgti.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.sxryk.cn/gtdpqrgnef.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.hysaishi.cn/gtjmudzibx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.chenlongwang.top/gtfwfhtmre.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hysaishi.cn/gtvytvfkgf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ehwqpu.com/gtzoohekip.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.zhaomingkeji.xyz/gtyfsukdei.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jyoumei.cn/gtipbaouro.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jyoumei.cn/gtsbujzalk.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yj20258888.top/gtnsqdhgrg.html

Go:   // 无：用配置结构体参数
来源：http://hz.daria6918.cn/gtyxhtixba.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ydzc1.top/gtsqofskly.html

C#:   f(a: 1, b: 2)
来源：http://hz.zhoulong.xyz/gtivsamkrn.html

[C05] 返回多个值
来源：http://hz.aibaodan.cn/gteagpfegi.html

Py:   return a, b
来源：http://hz.iojbl.cn/gtiveduglb.html

PHP:  return [$a, $b];
来源：http://hz.316326.xyz/gtpetzycqf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jlsjyb.cn/gtqxrzuops.html

TS:   return { a, b };
来源：http://hz.bjfxy.top/gtnuncmzic.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.cashguo.top/gtlisdenci.html

Go:   return a, b
来源：http://hz.c1oappe.top/gtjtghrwtg.html

Ruby: return a, b
来源：http://hz.chenjidiqi.icu/gtsjmpboxh.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.tianlin.xyz/gtgbeenenx.html

[C06] 匿名函数 / lambda
来源：http://hz.fzhhl.top/gtwfgawcek.html

Py:   square = lambda x: x * x
来源：http://hz.daria6918.cn/gthfygscvp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.cdnleiting.top/gtuwyagfxi.html

JS:   const square = x => x * x;
来源：http://hz.ydjk.org.cn/gtuwjnxhfs.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.hysaishi.cn/gtgffebgnl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.wangdashe.top/gtwcmjbnae.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.tianlin.xyz/gtkxyhiyyf.html

Ruby: square = ->(x) { x * x }
来源：http://hz.hnqzz.top/gtctowudvc.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yj20258.top/gtqgbrxzak.html

[C07] 把函数作为参数传入
来源：http://hz.ppjwa.cn/gteygspbgl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.birdmap.top/gtpalxzjgz.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.xuetiantiany.cn/gtbhgqdmtd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.cucudq.cn/gtbwxogmfw.html

TS:   arr.map(String)
来源：http://hz.shangyingyoupin.top/gtcubakkri.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.hammf.cn/gtyqbopwih.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.snrcjt.cn/gtqbgoliyv.html

Ruby: arr.map(&:upcase)
来源：http://hz.nwbrower.top/gtkdaxkivh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.daria6918.cn/gtttvowsif.html

[C08] 闭包
来源：http://hz.jqgfzy.top/gtcetdkxlv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yuxming.cn/gtrlarswwy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.cucudq.cn/gtrpjcylse.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.hfpthk.cn/gtvbfehjba.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.xuetiantiany.cn/gtcjuzzftp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhengqikj.top/gtelykdrwg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.hywenlv.cn/gtutjrywvp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jlsjyb.cn/gtgtjrjikr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.gotoacloud.top/gtcycbwzys.html

[C09] 递归
来源：http://hz.yueranfly.top/gtehencllp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.52xcode.cn/gtzpygmbvu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.haohaochexian.top/gtvzdqpvur.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj202588.top/gtyjbkeqnl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.redwolf501.top/gtlfgzhhrm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yuanzhike.top/gtixxwkhzi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.sysykeji.top/gtayqkftyf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.0kj1m.cn/gtmyqprctb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.yj20258.top/gtncpvfyuv.html

[C10] 变量作用域
来源：http://hz.jlsjyb.cn/gtlqmyklds.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hysaishi.cn/gtivxagzwa.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.cheryme.top/gtriyfzegs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jqgfzy.top/gtdehnojgt.html

TS:   同 JS
来源：http://hz.jianghu66.top/gtnrhxfnpb.html

Java: 方法内为块级作用域
来源：http://hz.gogol.net.cn/gtulhaapmd.html

Go:   花括号块级作用域
来源：http://hz.jinqigfzy.top/gtlyljuikx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hywenlv.cn/gtgouhalws.html

C#:   块级作用域
来源：http://hz.tanke756.top/gtwfikigix.html

[C11] 模块导入与导出
来源：http://hz.iojbl.cn/gtwocvxvyf.html

Py:   from module import func
来源：http://hz.nwbrower.top/gtsxhxsdhf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhongyouzk.top/gtfulozjnu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.ydjk.org.cn/gtwvqzmmdv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.dashuyun.cn/gttosxxhcd.html

Java: import java.util.List;
来源：http://hz.chenzaomai.com/gtvdcuhffu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.nanxuanxn.top/gtgrlkfvoj.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yuanzhike.top/gtfjtsjrad.html

C#:   using System.Text;
来源：http://hz.dashuyun.cn/gtisuvnagc.html

[C12] 立即执行函数 IIFE
来源：http://hz.9152youxi.cn/gtfdmjgmrs.html

Py:   (lambda: print("run"))()
来源：http://hz.yuanzhike.top/gthrjavbgf.html

PHP:  (function () { echo "run"; })();
来源：http://hz.fengsongda.top/gtaxqyepyv.html

JS:   (() => { console.log("run"); })();
来源：http://hz.bjfxy.top/gtnohmwpbo.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ywan-chungtsiang.top/gtpxwgcwtw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.cheryme.top/gtyuymooaa.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jiagoushi.top/gtnnmzlaco.html

Ruby: -> { puts "run" }.call
来源：http://hz.nanxuanxn.top/gtbxjawlpx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.tianlin.xyz/gtrwsvpkjr.html

[C13] 类型声明 / 类型注解
来源：http://hz.hnxiangtu.top/gtrzckxjoq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.nanxuanxn.top/gtkdjzdira.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cucudq.cn/gtdypdfkit.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.cucudq.cn/gtwlmtqmos.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xuanzx.com/gtdcatmrbk.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hywenlv.cn/gtwtmdsmgv.html

Go:   func add(a, b int) int
来源：http://hz.havefunace.top/gtznqncwlz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhiwuduotai.top/gtwsmdfzra.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ybcxt.top/gtuulhmfga.html

[C14] 泛型函数
来源：http://hz.smart0.xyz/gtgiwyjqab.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.aizwys.cn/gtgattzbzq.html

PHP:  // 无泛型
来源：http://hz.hammf.cn/gtkkomkvdz.html

JS:   // 无泛型
来源：http://hz.zhoulong.xyz/gtiqftdiqm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cashguo.top/gtnbelmzcb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.cdnleiting.top/gtnbmzrtug.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.c1oappe.top/gtuzlobfxe.html

Ruby: # 无泛型
来源：http://hz.guowangkeji.top/gtfdnqymdb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhaomingkeji.xyz/gtnkmmqoto.html

[C15] 解构 / 展开参数
来源：http://hz.cqqwz.cn/gtkvplhsjk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.xuetiantiany.cn/gtjmprnbyt.html

PHP:  [$a, $b] = $pair;
来源：http://hz.cdnleiting.top/gtswfqckep.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.aizwys.cn/gtzishevlv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.quarkkingdee.top/gtowzivznj.html

Java: // 无解构
来源：http://hz.sweek.top/gtsefpqmhm.html

Go:   // 无解构
来源：http://hz.yj202588.top/gtlnnralca.html

Ruby: a, b = pair
来源：http://hz.9152youxi.cn/gtevmsfcaj.html

C#:   var (a, b) = pair;
来源：http://hz.chenlongwang.top/gthswqqsbq.html

[C16] 函数 / 方法重载
来源：http://hz.xylfe.cn/gtlqfjuftk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.gzhubu.top/gtglwmbayy.html

PHP:  // 无重载
来源：http://hz.gaohongyu789.top/gtqobymphg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ehwqpu.com/gthffvubhe.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hywenlv.cn/gthvvkmqdo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hongshengwenyu.top/gtfrdnfdtq.html

Go:   // 无重载：用不同函数名
来源：http://hz.shangyingyoupin.top/gtkuytdztd.html

Ruby: # 无重载：靠动态参数
来源：http://hz.kuanghao11.cn/gtklesmqsq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zdqjudy.top/gtzmtecwze.html

================================================================================
来源：http://hz.gzhubu.top/gtxjadyzze.html

D. 数组 / 列表 / 集合
来源：http://hz.xziqi.cn/gtdeldktzn.html

================================================================================
来源：http://hz.jqgufenzy.top/gtntasxnec.html

[D01] 创建数组 / 列表
来源：http://hz.hongshengwenyu.top/gtwiqjiyyd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cdnleiting.top/gtvnfdlgqe.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yj20258.top/gtzznwemaf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.ywan-chungtsiang.top/gtonckaaqw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.andypj.xyz/gtjwdlnsqs.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xinyue.icu/gtfjbwatxt.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.mhx1999.top/gttwtwsteh.html

Ruby: arr = [1, 2, 3]
来源：http://hz.wangdashe.top/gtcumoksjn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ehwqpu.com/gtfzahmwjv.html

[D02] 追加元素到末尾
来源：http://hz.jqgufenzy.top/gtmajdzehm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xuetiantiany.cn/gtiaexqzlr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.chenlongwang.top/gtqsnolnna.html

JS:   arr.push(4);
来源：http://hz.guannengcc.top/gtflssrvgq.html

TS:   arr.push(4);
来源：http://hz.yuxming.cn/gtphtdpnba.html

Java: list.add(4);
来源：http://hz.shuidangran.top/gtnliqjedi.html

Go:   arr = append(arr, 4)
来源：http://hz.jlsjyb.cn/gtjhsdxpfu.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.iojbl.cn/gtcnobdrlt.html

C#:   list.Add(4);
来源：http://hz.chenlongwang.top/gtddkciahp.html

[D03] 在指定位置插入元素
来源：http://hz.zhaomingkeji.xyz/gtcjxcjifn.html

Py:   arr.insert(0, 0)
来源：http://hz.tanke756.top/gtqmldbsqf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhoulong.xyz/gtoekvqizr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xingfuxueyuan.xyz/gtdayindhp.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.shanyushiyangkeji.top/gtzprhpqhc.html

Java: list.add(0, 0);
来源：http://hz.hnqzz.top/gtjmeewygd.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zycfv.cn/gthbclsseg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.9152youxi.cn/gtwrptvsla.html

C#:   list.Insert(0, 0);
来源：http://hz.chenjidiqi.icu/gtxaeojtfy.html

[D04] 删除元素
来源：http://hz.gaohongyu789.top/gtphdmygod.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.fengsongda.top/gtpwwecghp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hysaishi.cn/gtjdaresck.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.bjfxy.top/gtzachagap.html

TS:   arr.splice(0, 1);
来源：http://hz.xingfuxueyuan.xyz/gtzvzlizfn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.pycfn.com/gtzcchsikg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jiagoushi.top/gttpuynodf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zycfv.cn/gtjxgklcyg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yuanzhike.top/gtrykkcync.html

[D05] 访问与修改元素
来源：http://hz.cdnleiting.top/gtjknjsxnl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinqigufen.top/gtfvnperfs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.redwolf501.top/gtrdyvanwp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.birdmap.top/gtfmsetpgq.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hywenlv.cn/gtzhkamjef.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhongyouzk.top/gtlfzfiruz.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ydjk.org.cn/gtjdccytad.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenzaomai.com/gtjsmfwqwh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.vqdsnc.cn/gtkuunwhew.html

[D06] 数组长度
来源：http://hz.sweek.top/gtaakkzafa.html

Py:   len(arr)
来源：http://hz.iojbl.cn/gtxlhscwhb.html

PHP:  count($arr);
来源：http://hz.ppjwa.cn/gtxgykfqyi.html

JS:   arr.length
来源：http://hz.yongpay.top/gtflhsxqff.html

TS:   arr.length
来源：http://hz.hnqzz.top/gtobanfqrs.html

Java: list.size();
来源：http://hz.guowangkeji.top/gtzndfagcl.html

Go:   len(arr)
来源：http://hz.ydzc1.top/gtpnjjmdim.html

Ruby: arr.length; arr.size
来源：http://hz.zdqjudy.top/gtilmpvmyu.html

C#:   list.Count;
来源：http://hz.aizwys.cn/gtcoyspoge.html

[D07] 切片 / 取子数组
来源：http://hz.gzhubu.top/gtqjoqqlsl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.shangyingyoupin.top/gtumsseaka.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.c1oappe.top/gtkoxkngyy.html

JS:   arr.slice(1, 4);
来源：http://hz.aibaodan.cn/gttkpjzcwr.html

TS:   arr.slice(1, 4);
来源：http://hz.zhongyouzk.top/gttxgmwgtb.html

Java: list.subList(1, 4);
来源：http://hz.cashguo.top/gtnxareuoc.html

Go:   arr[1:4]
来源：http://hz.andypj.xyz/gtijokhdmy.html

Ruby: arr[1, 3]
来源：http://hz.tianlin.xyz/gtamopoihy.html

C#:   list.GetRange(1, 3);
来源：http://hz.smart0.xyz/gtxsirsyzq.html

[D08] 合并两个数组
来源：http://hz.snrcjt.cn/gtcofnguuo.html

Py:   a + b;  a.extend(b)
来源：http://hz.jqgfzy.top/gtmkellvqx.html

PHP:  array_merge($a, $b);
来源：http://hz.xylfe.cn/gtdshwydsm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ivvv.top/gtspbsprps.html

TS:   [...a, ...b];
来源：http://hz.feifeiyinyue.top/gtbsiiilhj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yuanzhike.top/gtwcykcsvr.html

Go:   append(a, b...)
来源：http://hz.cucudq.cn/gtmhpeqwit.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ydzc1.top/gtcgylizsf.html

C#:   a.Concat(b).ToList()
来源：http://hz.jinqigufen.top/gtzpuyazdq.html

[D09] 排序（升序）
来源：http://hz.nanxinkj.top/gtgfspiafz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.pycfn.com/gtgplyftwg.html

PHP:  sort($arr);
来源：http://hz.cqqwz.cn/gttnieuvln.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.tianlin.xyz/gtlwfutfal.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.sxryk.cn/gtnjjswjuc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.guannengcc.top/gttsvmhonf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yongpay.top/gtbvlajltu.html

Ruby: arr.sort
来源：http://hz.meibo888.top/gtrtyysspk.html

C#:   list.Sort();
来源：http://hz.xuanzx.com/gtrthvuebo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.gaohongyu789.top/gtrspieiyq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.sufxvd.cn/gtqiifxmta.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.bjfxy.top/gtawtznhrm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hnqzz.top/gtfiqfbvlc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhijiandao.cn/gtrjqoyzgi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.sysykeji.top/gtvwypchol.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yongpay.top/gtigsypqdt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.gzhubu.top/gtrepoijrc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xuanzx.com/gtyxtentqi.html

[D11] 反转数组
来源：http://hz.jinyuanbaomall.cn/gtnanrlamn.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jiagoushi.top/gtsdyzmfkn.html

PHP:  array_reverse($arr);
来源：http://hz.shanyushiyangkeji.top/gtdcaoauxw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xylfe.cn/gtgylwutye.html

TS:   [...arr].reverse();
来源：http://hz.yanxiufei.cn/gthvxbssti.html

Java: Collections.reverse(list);
来源：http://hz.hongshengwenyu.top/gtwcotozyl.html

Go:   slices.Reverse(arr)
来源：http://hz.yanxiufei.cn/gtrielzthh.html

Ruby: arr.reverse
来源：http://hz.xinyue.icu/gtlbhctlce.html

C#:   list.Reverse();
来源：http://hz.jinyuanbaomall.cn/gtuyqvgtmu.html

[D12] 查找元素下标
来源：http://hz.ydjk.org.cn/gtcrwgugmv.html

Py:   arr.index(x);  x in arr
来源：http://hz.yj202588.top/gtosnhlarg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhixingplan.top/gtwpkltuul.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.dashuyun.cn/gtvnrneify.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.9152youxi.cn/gtaekqjuqe.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.cashguo.top/gtinwbreyo.html

Go:   slices.Index(arr, x)
来源：http://hz.pycfn.com/gtkgcjayoi.html

Ruby: arr.index(x)
来源：http://hz.svipenyu.cn/gtthnismsx.html

C#:   list.IndexOf(x);
来源：http://hz.zhaomingkeji.xyz/gtsyfutmbk.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jqgufenzy.top/gtyrorladi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ivvv.top/gtmnjvheco.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.nanxinkj.top/gttyoeptul.html

JS:   arr.filter(x => x > 3)
来源：http://hz.tianlin.xyz/gtfbixerzo.html

TS:   arr.filter(x => x > 3)
来源：http://hz.cheryme.top/gttcybpimu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhaomingkeji.xyz/gtpzvyedug.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jianghu66.top/gtzovmqeyn.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.sweek.top/gtourjnnco.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.316326.xyz/gtmcfofmlu.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yuanzhike.top/gtzsaqqfyj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.snrcjt.cn/gtofvtlvjz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.chenzaomai.com/gtbieiaipy.html

JS:   arr.map(x => x * 2)
来源：http://hz.yueranfly.top/gtetdiugaz.html

TS:   arr.map(x => x * 2)
来源：http://hz.hfpthk.cn/gtzuqljent.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yangfankeji.com/gtntkrkeza.html

Go:   // 手写循环
来源：http://hz.cucudq.cn/gtlcreglmx.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.zhongyouzk.top/gtlrozuujn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.wangdashe.top/gtdafxafjq.html

[D15] 去重
来源：http://hz.quarkkingdee.top/gtlkkjgwbe.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jiagoushi.top/gtiaindkuz.html

PHP:  array_unique($arr);
来源：http://hz.316326.xyz/gtcxguomgj.html

JS:   [...new Set(arr)]
来源：http://hz.cheryme.top/gtxwrdzvtr.html


<!-- 参考信息 -->