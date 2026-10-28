代发 wailian999

C#:   x is int or double or decimal
来源：http://hz.hfpthk.cn/gteulaihtf.html

[B14] 判断值是否在集合内
来源：http://hz.ybcxt.top/gtepsjizle.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.kuanghao11.cn/gtrnfoglsi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.xziqi.cn/gtghzudlpj.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yongpay.top/gtgdgjafeh.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.gotoacloud.top/gtcquphjdt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.xylfe.cn/gttlodbbyk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.redwolf501.top/gtbrurygnj.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.zycfv.cn/gtuxrfmmyq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.aibaodan.cn/gtxhtzmgul.html

[B15] 布尔运算与取反
来源：http://hz.havefunace.top/gtupmmfxww.html

Py:   a and b or not c
来源：http://hz.hammf.cn/gtfaexhusx.html

PHP:  $a && $b || !$c
来源：http://hz.yj202588.top/gtabrxssnj.html

JS:   a && b || !c
来源：http://hz.zhengqikj.top/gtrggepagk.html

TS:   a && b || !c
来源：http://hz.gotoacloud.top/gtasbtqiqw.html

Java: a && b || !c
来源：http://hz.jinqigfzy.top/gtfdgdwecl.html

Go:   a && b || !c
来源：http://hz.chenzaomai.com/gtyvmhvcwf.html

Ruby: a && b || !c
来源：http://hz.hnqzz.top/gtjhsfsqfp.html

C#:   a && b || !c
来源：http://hz.birdmap.top/gtzqhchzvr.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.iojbl.cn/gtltitrbsl.html

Py:   if not data: return
来源：http://hz.yuanzhike.top/gtvzajuvts.html

PHP:  if (!$data) { return; }
来源：http://hz.jqgufenzy.top/gtlbncizly.html

JS:   if (!data) return;
来源：http://hz.yueranfly.top/gtyrozssfp.html

TS:   if (!data) return;
来源：http://hz.yj20258888.top/gtjparivqf.html

Java: if (data == null) return;
来源：http://hz.zhiwuduotai.top/gtmseyqmog.html

Go:   if data == nil { return }
来源：http://hz.snrcjt.cn/gtfxvhrxwp.html

Ruby: return if data.nil?
来源：http://hz.jianghu66.top/gttwuauytl.html

C#:   if (data == null) return;
来源：http://hz.xuetiantiany.cn/gtcmlgkxqa.html

================================================================================
来源：http://hz.zhijiandao.cn/gtnfwewdqq.html

C. 函数与作用域
来源：http://hz.shuidangran.top/gtkxylfass.html

================================================================================
来源：http://hz.jinqigfzy.top/gtlpxkshnd.html

[C01] 定义函数
来源：http://hz.mhx1999.top/gthwthhiez.html

Py:   def add(a, b): return a + b
来源：http://hz.yongpay.top/gtfuiwvzht.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinqigufen.top/gtddbrhisb.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.c1oappe.top/gtpgemmoaz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jiagoushi.top/gtfyuqlzbx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.yj20258888.top/gtnuqyglkg.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.nanxinkj.top/gtzhoakruo.html

Ruby: def add(a, b); a + b; end
来源：http://hz.cashguo.top/gtohnmtvzg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.gotoacloud.top/gtqlwwmujx.html

[C02] 默认参数
来源：http://hz.jinqigufen.top/gtqksqfwtw.html

Py:   def greet(name="World"): return name
来源：http://hz.ydjk.org.cn/gtoxholvnj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.0kj1m.cn/gtfilqrsgh.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jinqigufen.top/gtphdykoac.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.sxryk.cn/gtjwnldrpa.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.nanxinkj.top/gtkkrrfhjq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.dianchejie.cn/gtupmjogqp.html

Ruby: def greet(name = "World") = name
来源：http://hz.fzhhl.top/gtzedbkori.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.gzhubu.top/gtfdjskgaq.html

[C03] 可变参数
来源：http://hz.yvedp.cn/gtvvsifgkh.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhengqikj.top/gtzdbyblln.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ivvv.top/gtkdowqoco.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sysykeji.top/gtvagjujbp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhengqikj.top/gtpesljtot.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.bjfxy.top/gtylhiohqp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yonumen.top/gtyioczxpe.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.zdqjudy.top/gtkhuajaiq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.fengsongda.top/gttxspmihs.html

[C04] 命名参数 / 关键字参数
来源：http://hz.kuanghao11.cn/gtktoophzn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.shuidangran.top/gtzzdsbcia.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.birdmap.top/gtqcznymek.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.tanke756.top/gtzdsuhwbp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.cdnleiting.top/gtvuzokfaf.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.sysykeji.top/gtijpwfmfx.html

Go:   // 无：用配置结构体参数
来源：http://hz.jyoumei.cn/gtacuuuqhw.html

Ruby: f(a: 1, b: 2)
来源：http://hz.nwbrower.top/gtfrozizgb.html

C#:   f(a: 1, b: 2)
来源：http://hz.daria6918.cn/gtmfvkrplb.html

[C05] 返回多个值
来源：http://hz.dianchejie.cn/gtoscquetf.html

Py:   return a, b
来源：http://hz.9152youxi.cn/gttrhshcso.html

PHP:  return [$a, $b];
来源：http://hz.zycfv.cn/gtnbmpirdo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.wangshuangyany.cn/gtvewpcggu.html

TS:   return { a, b };
来源：http://hz.tian-w.cn/gtmzckmhdl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yueranfly.top/gtrqfkpdtt.html

Go:   return a, b
来源：http://hz.havefunace.top/gtkebdolor.html

Ruby: return a, b
来源：http://hz.kuanghao11.cn/gtuajgjsry.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhengqikj.top/gtliqxfwxe.html

[C06] 匿名函数 / lambda
来源：http://hz.dashuyun.cn/gtxjwzbhim.html

Py:   square = lambda x: x * x
来源：http://hz.zhaomingkeji.xyz/gthrzlntvt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.wangshuangyany.cn/gturbdqpxe.html

JS:   const square = x => x * x;
来源：http://hz.cashguo.top/gtovalsbda.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.chenlongwang.top/gthmdajzic.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.zdqjudy.top/gtflprfvgl.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.hammf.cn/gtnosrcdtn.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jinghuilouyu.cn/gtyxoznjip.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.xziqi.cn/gtdkkvwkxe.html

[C07] 把函数作为参数传入
来源：http://hz.jqgufenzy.top/gttpfjenlo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.tianlin.xyz/gteuhphaxz.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.bjfxy.top/gtkgogsxaz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.shzxlz.cn/gtffkfedtk.html

TS:   arr.map(String)
来源：http://hz.quarkkingdee.top/gtljulknad.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yuanzhike.top/gtskxyhkux.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.aibaodan.cn/gtwvksavki.html

Ruby: arr.map(&:upcase)
来源：http://hz.sweek.top/gtpgnetfus.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yvedp.cn/gtysyiqmew.html

[C08] 闭包
来源：http://hz.xuetiantiany.cn/gtazqtcgxg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.daxiang520.top/gtieokrlbv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.yj20258888.top/gtntbnccnt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yj20258.top/gtjrwiubbe.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.zhiwuduotai.top/gttmbetooz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.fzhhl.top/gtupibilfb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.pengpengdd.cyou/gtjsqbbfeu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.xinyue.icu/gtvmzqkktm.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.nanxinkj.top/gthlarysfn.html

[C09] 递归
来源：http://hz.jinyuanbaomall.cn/gtonttxjws.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.wangdashe.top/gtyfwepqwi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ywan-chungtsiang.top/gtxudqrjht.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gzhubu.top/gtzfunolog.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zycfv.cn/gtfsvwgvkm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yuxming.cn/gtjjuduikw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.jqgufenzy.top/gtokwiaonb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.ybcxt.top/gtxajwoizg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.cdnleiting.top/gtwstuiuhc.html

[C10] 变量作用域
来源：http://hz.guannengcc.top/gtuvtusaav.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.sxryk.cn/gtrlqkpjiu.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.0kj1m.cn/gtvhwtalzd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.vqdsnc.cn/gtkkrrgpqz.html

TS:   同 JS
来源：http://hz.zhongyouzk.top/gttrvgzanz.html

Java: 方法内为块级作用域
来源：http://hz.tianlin.xyz/gtsmwahwid.html

Go:   花括号块级作用域
来源：http://hz.gaohongyu789.top/gtytcdlxcn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.tianlin.xyz/gtqrfmlllo.html

C#:   块级作用域
来源：http://hz.zycfv.cn/gtzwiilolq.html

[C11] 模块导入与导出
来源：http://hz.zhijiandao.cn/gtsytlfpzf.html

Py:   from module import func
来源：http://hz.fzhhl.top/gtuhxcmnfl.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hywenlv.cn/gtuirwztkt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cashguo.top/gtuiyptuiz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.guowangkeji.top/gtlfsohqta.html

Java: import java.util.List;
来源：http://hz.nwbrower.top/gtjjzjswbw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.xylfe.cn/gtaxngtpen.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.pycfn.com/gtjmynxjtl.html

C#:   using System.Text;
来源：http://hz.dashuyun.cn/gtfntafavh.html

[C12] 立即执行函数 IIFE
来源：http://hz.52xcode.cn/gtxegnhxbw.html

Py:   (lambda: print("run"))()
来源：http://hz.cashguo.top/gtzytexmap.html

PHP:  (function () { echo "run"; })();
来源：http://hz.chenzaomai.com/gtnjssqgzv.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jyoumei.cn/gtyrydrdqn.html

TS:   (() => { console.log("run"); })();
来源：http://hz.pengpengdd.cyou/gtsgjgqzrh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.gzhubu.top/gtsgrxkfdv.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jqgfzy.top/gteeicvvcp.html

Ruby: -> { puts "run" }.call
来源：http://hz.ehwqpu.com/gtxiwkiztw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zdqjudy.top/gtwllazqpa.html

[C13] 类型声明 / 类型注解
来源：http://hz.hywenlv.cn/gtrdpzztek.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.cucudq.cn/gtnjcjbmpv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.tianlin.xyz/gtlduqpoxh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.chenlongwang.top/gtuxmojtaj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yj202588.top/gtinpxxads.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.9152youxi.cn/gtaujcoecp.html

Go:   func add(a, b int) int
来源：http://hz.hnxiangtu.top/gtmclwmswl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.redwolf501.top/gteadgmquc.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.andypj.xyz/gtpzvdfdfp.html

[C14] 泛型函数
来源：http://hz.zhaomingkeji.xyz/gtlrpnanjo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.snrcjt.cn/gthcwxejqj.html

PHP:  // 无泛型
来源：http://hz.yonumen.top/gtcbtvjsfg.html

JS:   // 无泛型
来源：http://hz.pycfn.com/gtyejpwygc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.chenjidiqi.icu/gtxbmvmhze.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.chenlongwang.top/gtifoyzing.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.cashguo.top/gtmrcdingq.html

Ruby: # 无泛型
来源：http://hz.daria6918.cn/gtvitwspsp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ydjk.org.cn/gtskopmivg.html

[C15] 解构 / 展开参数
来源：http://hz.zhixingplan.top/gtdoqjsgux.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.aibaodan.cn/gttefjutdx.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jianghu66.top/gtujgktbha.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jinqigfzy.top/gtdptzmoei.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.chenlongwang.top/gtzzovqgiv.html

Java: // 无解构
来源：http://hz.nanxinkj.top/gtsxwiiinw.html

Go:   // 无解构
来源：http://hz.snrcjt.cn/gtmjtwrvxu.html

Ruby: a, b = pair
来源：http://hz.hongshengwenyu.top/gthlebaxpy.html

C#:   var (a, b) = pair;
来源：http://hz.mhx1999.top/gtkprrcgqm.html

[C16] 函数 / 方法重载
来源：http://hz.sxryk.cn/gtnjwdozet.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hnqzz.top/gtfwvzzcmf.html

PHP:  // 无重载
来源：http://hz.xinyue.icu/gtiivedihb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jqgufenzy.top/gtbuveducx.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.fengsongda.top/gtzygfqbjv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xylfe.cn/gthbsboavk.html

Go:   // 无重载：用不同函数名
来源：http://hz.jiagoushi.top/gtlvblliux.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhixingplan.top/gtzaykhqkn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.andypj.xyz/gtjpjjnqnv.html

================================================================================
来源：http://hz.fengsongda.top/gtovuerrnc.html

D. 数组 / 列表 / 集合
来源：http://hz.xuanzx.com/gtwaysztdr.html

================================================================================
来源：http://hz.andypj.xyz/gtsuirvkvw.html

[D01] 创建数组 / 列表
来源：http://hz.shuidangran.top/gtxnmmlgyo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.guowangkeji.top/gtvaenfxtz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.52xcode.cn/gtyptxjrda.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zdqjudy.top/gtbjoiqlmj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yj20258888.top/gtcnawzuxd.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xingfuxueyuan.xyz/gtxzogztgi.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xziqi.cn/gtarenpwfa.html

Ruby: arr = [1, 2, 3]
来源：http://hz.snrcjt.cn/gtnfeljfwk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xuanzx.com/gtuyzbhepj.html

[D02] 追加元素到末尾
来源：http://hz.c1oappe.top/gtfbfookjs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ppjwa.cn/gtkttowoph.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.daxiang520.top/gtffmvkhvi.html

JS:   arr.push(4);
来源：http://hz.haohaochexian.top/gtszrylevf.html

TS:   arr.push(4);
来源：http://hz.zhiwuduotai.top/gtlrhpivii.html

Java: list.add(4);
来源：http://hz.ehwqpu.com/gtfdwgsmqp.html

Go:   arr = append(arr, 4)
来源：http://hz.gogol.net.cn/gtbnfrpjva.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.chenzaomai.com/gtzzhjeltq.html

C#:   list.Add(4);
来源：http://hz.andypj.xyz/gtunldkzmc.html

[D03] 在指定位置插入元素
来源：http://hz.gogol.net.cn/gtrvxpssoa.html

Py:   arr.insert(0, 0)
来源：http://hz.aizwys.cn/gtglgjycuo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.haohaochexian.top/gtswcqfflz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yvedp.cn/gtmtvgdmbh.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.snrcjt.cn/gtmusjwssa.html

Java: list.add(0, 0);
来源：http://hz.zhoulong.xyz/gtvziarbqt.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hysaishi.cn/gtwyfgexqs.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.vqdsnc.cn/gtkjgwpbto.html

C#:   list.Insert(0, 0);
来源：http://hz.hnxiangtu.top/gtzxmqnned.html

[D04] 删除元素
来源：http://hz.cucudq.cn/gtkjuxqwer.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xingfuxueyuan.xyz/gtnkjqrcgp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhengqikj.top/gtgggvfgor.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.pycfn.com/gtvumeecdj.html

TS:   arr.splice(0, 1);
来源：http://hz.zhoulong.xyz/gtxcpdewmv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.hysaishi.cn/gtwvocewyx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.cucudq.cn/gtqkijxund.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jianghu66.top/gthwcqvnrm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.feifeiyinyue.top/gtaozggvho.html

[D05] 访问与修改元素
来源：http://hz.daria6918.cn/gtklyhimwf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenzaomai.com/gtgvehxopa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.snrcjt.cn/gtrlzfhmdd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.vqdsnc.cn/gtvjvrbloh.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jiagoushi.top/gthpzpeuhc.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.haohaochexian.top/gtlcpvvney.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yuanzhike.top/gtzeetemko.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ppjwa.cn/gtokycppfq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.shzxlz.cn/gtzajribte.html

[D06] 数组长度
来源：http://hz.yongpay.top/gtpxzwzimw.html

Py:   len(arr)
来源：http://hz.daria6918.cn/gteyfkhwhn.html

PHP:  count($arr);
来源：http://hz.yj202588.top/gtjcnhcuro.html

JS:   arr.length
来源：http://hz.jqgfzy.top/gtdoulxhgk.html

TS:   arr.length
来源：http://hz.tanke756.top/gthhzhrjwz.html

Java: list.size();
来源：http://hz.ybcxt.top/gtpokcbfzg.html

Go:   len(arr)
来源：http://hz.tian-w.cn/gtrntzqtsj.html

Ruby: arr.length; arr.size
来源：http://hz.daxiang520.top/gtxtmmhkhc.html

C#:   list.Count;
来源：http://hz.ywan-chungtsiang.top/gtempembui.html

[D07] 切片 / 取子数组
来源：http://hz.mhx1999.top/gtygrvcvgg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhijiandao.cn/gtlduyzeqv.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zhaomingkeji.xyz/gtuvejwzdw.html

JS:   arr.slice(1, 4);
来源：http://hz.zhiwuduotai.top/gtgyrmcoxc.html

TS:   arr.slice(1, 4);
来源：http://hz.haohaochexian.top/gtjeslseis.html

Java: list.subList(1, 4);
来源：http://hz.cheryme.top/gtnlyzeivd.html

Go:   arr[1:4]
来源：http://hz.dianchejie.cn/gtjmqmgocr.html

Ruby: arr[1, 3]
来源：http://hz.yanxiufei.cn/gtadxmpjni.html

C#:   list.GetRange(1, 3);
来源：http://hz.andypj.xyz/gtmnqwweye.html

[D08] 合并两个数组
来源：http://hz.ehwqpu.com/gtmzlmwyao.html

Py:   a + b;  a.extend(b)
来源：http://hz.iojbl.cn/gtkayliqpc.html

PHP:  array_merge($a, $b);
来源：http://hz.yvedp.cn/gtguzkpnid.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.quarkkingdee.top/gtforpyaqi.html

TS:   [...a, ...b];
来源：http://hz.tianlin.xyz/gtggdgmnkp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ppjwa.cn/gtjzunyzbv.html

Go:   append(a, b...)
来源：http://hz.guannengcc.top/gtilvipdde.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ywan-chungtsiang.top/gtonpobobr.html

C#:   a.Concat(b).ToList()
来源：http://hz.ydjk.org.cn/gtbtpdejod.html

[D09] 排序（升序）
来源：http://hz.chenjidiqi.icu/gtmsukpggf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.316326.xyz/gtqkgiwkgu.html

PHP:  sort($arr);
来源：http://hz.yonumen.top/gtcvsuwpbp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xinyue.icu/gtxwwvaymh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jinqigufen.top/gtgutdlbfw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ivvv.top/gtyhjfczmu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cdnleiting.top/gtkajldekk.html

Ruby: arr.sort
来源：http://hz.sweek.top/gtymvsmzjn.html

C#:   list.Sort();
来源：http://hz.hfpthk.cn/gttqfdzbpj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jqgfzy.top/gtodskxxfv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ehwqpu.com/gtvblsoqqc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.smart0.xyz/gtfcswcpgg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daria6918.cn/gtxjlhymzf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ivvv.top/gtnchcqepb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.pycfn.com/gthjesenfw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shanyushiyangtech.top/gtpspnufsi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.tian-w.cn/gtlmtltdet.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.guowangkeji.top/gtuluifseo.html

[D11] 反转数组
来源：http://hz.dianchejie.cn/gtorfnvqps.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hysaishi.cn/gthbbkljfu.html

PHP:  array_reverse($arr);
来源：http://hz.hnqzz.top/gtfrvilxhi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.gogol.net.cn/gtfixjlmyd.html

TS:   [...arr].reverse();
来源：http://hz.hongshengwenyu.top/gtdihpkoov.html

Java: Collections.reverse(list);
来源：http://hz.sysykeji.top/gtflyjhejq.html

Go:   slices.Reverse(arr)
来源：http://hz.yonumen.top/gtgortgjbv.html

Ruby: arr.reverse
来源：http://hz.jiagoushi.top/gtnvbbctfs.html

C#:   list.Reverse();
来源：http://hz.jqgfzy.top/gtmlbzueoj.html

[D12] 查找元素下标
来源：http://hz.cashguo.top/gtwenndmms.html

Py:   arr.index(x);  x in arr
来源：http://hz.yongpay.top/gtgzliamjh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.chenzaomai.com/gtlipiobvt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhongyouzk.top/gtvbqfdknz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hnxiangtu.top/gtmouwwiki.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.snrcjt.cn/gthoecuwlu.html

Go:   slices.Index(arr, x)
来源：http://hz.yvedp.cn/gtpgwjlumx.html

Ruby: arr.index(x)
来源：http://hz.chenjidiqi.icu/gtuozaexyz.html

C#:   list.IndexOf(x);
来源：http://hz.xuetiantiany.cn/gtudffdbyf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.vqdsnc.cn/gtcsotplts.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.dianchejie.cn/gtyblwsrev.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.fzhhl.top/gttyswjwkg.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xuetiantiany.cn/gtumimwtfy.html

TS:   arr.filter(x => x > 3)
来源：http://hz.pengpengdd.cyou/gtvwxzymhf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.chenjidiqi.icu/gtrjaifxkx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hnqzz.top/gttjsxsmcu.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.iojbl.cn/gtelnkeraj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhijiandao.cn/gtsoozaool.html

[D14] 映射转换（每个元素变形）
来源：http://hz.gzhubu.top/gtealgywbv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.cdnleiting.top/gtxdmhicjz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ivvv.top/gtlflbruxw.html

JS:   arr.map(x => x * 2)
来源：http://hz.wangshuangyany.cn/gtocpozohp.html

TS:   arr.map(x => x * 2)
来源：http://hz.zdqjudy.top/gtqmewohci.html


<!-- 参考信息 -->