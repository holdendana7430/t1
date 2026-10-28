代发 wailian999

C#:   x is int or double or decimal
来源：http://hz.c1oappe.top/gtmxkzmxaf.html

[B14] 判断值是否在集合内
来源：http://hz.zhijiandao.cn/gtxoazbkpg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.jinghuilouyu.cn/gtikqwtpzj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.ybcxt.top/gtsgpwvlvq.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.gzhubu.top/gtmhoypaqv.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.svipenyu.cn/gtkdhhlysc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.yj202588.top/gtigmqowru.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.zhongyouzk.top/gtvbcfhcgz.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.ivvv.top/gtryfidusa.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.yj20258.top/gtnrhmghph.html

[B15] 布尔运算与取反
来源：http://hz.daxiang520.top/gtxkweiaqp.html

Py:   a and b or not c
来源：http://hz.jqgfzy.top/gtuarpfqwg.html

PHP:  $a && $b || !$c
来源：http://hz.hnqzz.top/gtqcbdrdml.html

JS:   a && b || !c
来源：http://hz.pycfn.com/gtuvmgmflv.html

TS:   a && b || !c
来源：http://hz.0kj1m.cn/gtydfakwcv.html

Java: a && b || !c
来源：http://hz.jianghu66.top/gtwrxrwxzm.html

Go:   a && b || !c
来源：http://hz.c1oappe.top/gthtaadljp.html

Ruby: a && b || !c
来源：http://hz.hysaishi.cn/gtabpnuolm.html

C#:   a && b || !c
来源：http://hz.yuxming.cn/gtknvlykxs.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.nwbrower.top/gtuldwlwpt.html

Py:   if not data: return
来源：http://hz.gaohongyu789.top/gtzurcdnmz.html

PHP:  if (!$data) { return; }
来源：http://hz.gotoacloud.top/gtwydjzyus.html

JS:   if (!data) return;
来源：http://hz.yangfankeji.com/gtivvmqmqq.html

TS:   if (!data) return;
来源：http://hz.zhixingplan.top/gtfwpohwdn.html

Java: if (data == null) return;
来源：http://hz.hammf.cn/gtmfiygduq.html

Go:   if data == nil { return }
来源：http://hz.fengsongda.top/gtqwnjcerv.html

Ruby: return if data.nil?
来源：http://hz.yangfankeji.com/gtjgthxdme.html

C#:   if (data == null) return;
来源：http://hz.jinyuanbaomall.cn/gttuejzcff.html

================================================================================
来源：http://hz.andypj.xyz/gtsabguwxn.html

C. 函数与作用域
来源：http://hz.shzxlz.cn/gtctqjudtk.html

================================================================================
来源：http://hz.daria6918.cn/gtqcgobwew.html

[C01] 定义函数
来源：http://hz.smart0.xyz/gtgdrmfyyz.html

Py:   def add(a, b): return a + b
来源：http://hz.sxryk.cn/gtbsfyafft.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guannengcc.top/gtraodpnqo.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.pengpengdd.cyou/gtzxwzozlb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.fzhhl.top/gtuptrtpro.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.tian-w.cn/gtejasbhso.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.ydjk.org.cn/gtgsgzkond.html

Ruby: def add(a, b); a + b; end
来源：http://hz.sufxvd.cn/gtivjlrtwe.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.kuanghao11.cn/gtduyuzgfq.html

[C02] 默认参数
来源：http://hz.xuanzx.com/gtxiijokok.html

Py:   def greet(name="World"): return name
来源：http://hz.yj202588.top/gtzlgsykcs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.tanke756.top/gtdzrnuvfy.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.vqdsnc.cn/gtfolmjiab.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.nanxuanxn.top/gtcbvgpmmx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.andypj.xyz/gtzlzjlyob.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ybcxt.top/gtjoermamc.html

Ruby: def greet(name = "World") = name
来源：http://hz.smart0.xyz/gtijabmyte.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.fengsongda.top/gtpkwlpfvf.html

[C03] 可变参数
来源：http://hz.fengsongda.top/gthiiwzxmr.html

Py:   def total(*args): return sum(args)
来源：http://hz.zhiwuduotai.top/gtouugkdsz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.xylfe.cn/gtrmdeufrb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.havefunace.top/gtkzjpwmdh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.zhaomingkeji.xyz/gtrapbancr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.daxiang520.top/gttfnfazjd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.sweek.top/gthbtsdfps.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.jinqigfzy.top/gtmrfhbazd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.xinyue.icu/gtxrfdmxcl.html

[C04] 命名参数 / 关键字参数
来源：http://hz.wangshuangyany.cn/gtkxnrcsgg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.fengsongda.top/gtariwrkvt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.jinyuanbaomall.cn/gtkogelcgn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.cashguo.top/gtrwmfsscr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.cdnleiting.top/gtzpgqsuqg.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.haohaochexian.top/gtdfavvokr.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhoulong.xyz/gtyqddeyqc.html

Ruby: f(a: 1, b: 2)
来源：http://hz.ydzc1.top/gtkpuyfbdv.html

C#:   f(a: 1, b: 2)
来源：http://hz.jqgufenzy.top/gtdwrlxwne.html

[C05] 返回多个值
来源：http://hz.dashuyun.cn/gtoyaurqes.html

Py:   return a, b
来源：http://hz.shanyushiyangkeji.top/gtpjmuqphu.html

PHP:  return [$a, $b];
来源：http://hz.smart0.xyz/gtlztluyah.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.vqdsnc.cn/gtcmctiddj.html

TS:   return { a, b };
来源：http://hz.zhengqikj.top/gtppipjxsx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhongyouzk.top/gtjjowlpyx.html

Go:   return a, b
来源：http://hz.zhongyouzk.top/gtigosxxon.html

Ruby: return a, b
来源：http://hz.tianlin.xyz/gtwsseyzgc.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.ydzc1.top/gtetwdrljs.html

[C06] 匿名函数 / lambda
来源：http://hz.cqqwz.cn/gtewumaccc.html

Py:   square = lambda x: x * x
来源：http://hz.52xcode.cn/gtjqzmfdnf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.daxiang520.top/gtjxezqhur.html

JS:   const square = x => x * x;
来源：http://hz.cucudq.cn/gtoinxsduk.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.316326.xyz/gtczyierve.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.aizwys.cn/gtjxevacef.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.guowangkeji.top/gtskaqmyky.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhoulong.xyz/gtbcpszmaa.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.daria6918.cn/gtihedbtsb.html

[C07] 把函数作为参数传入
来源：http://hz.chenzaomai.com/gtmxjqpcmp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.gzhubu.top/gtfojkeond.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yj20258.top/gtwzuomcou.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.c1oappe.top/gttwiwdeal.html

TS:   arr.map(String)
来源：http://hz.zycfv.cn/gthimxfldw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.xingfuxueyuan.xyz/gtlshwkmrn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.wangshuangyany.cn/gtgrrvpooh.html

Ruby: arr.map(&:upcase)
来源：http://hz.quarkkingdee.top/gtmtocxuoo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.shuidangran.top/gthuooshik.html

[C08] 闭包
来源：http://hz.shangyingyoupin.top/gtoxzdouvi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.chenjidiqi.icu/gtjqndbalv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.feifeiyinyue.top/gtgrudshms.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.svipenyu.cn/gtilhyagvf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.tianlin.xyz/gthzymdiby.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.zhaomingkeji.xyz/gtnbybivqd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jianghu66.top/gtglvjwfxp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.sysykeji.top/gtplpsfqym.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.xinyue.icu/gtscigmxfd.html

[C09] 递归
来源：http://hz.smart0.xyz/gtzqidyuax.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.gotoacloud.top/gtxfrmhsoj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.hywenlv.cn/gtzruwyuex.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ydzc1.top/gtrogtlqny.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yangfankeji.com/gttgzumkdm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.bjfxy.top/gtecriaxus.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhaomingkeji.xyz/gtuwxnhpxr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.daxiang520.top/gtyazocqbn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.gotoacloud.top/gtcpgchqen.html

[C10] 变量作用域
来源：http://hz.yuxming.cn/gtxkmabvrq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.ydjk.org.cn/gtwpzrdtja.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.sweek.top/gtawwtokcv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cucudq.cn/gtozmzjpcd.html

TS:   同 JS
来源：http://hz.ydjk.org.cn/gtyeqhgiir.html

Java: 方法内为块级作用域
来源：http://hz.yangfankeji.com/gtbiumzmxj.html

Go:   花括号块级作用域
来源：http://hz.sweek.top/gtbjrybtvl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.0kj1m.cn/gtrdhpxtzp.html

C#:   块级作用域
来源：http://hz.0kj1m.cn/gtgivkkwua.html

[C11] 模块导入与导出
来源：http://hz.xziqi.cn/gthurmgymp.html

Py:   from module import func
来源：http://hz.pengpengdd.cyou/gtsscgxkxz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ydjk.org.cn/gtvogxbwjo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yvedp.cn/gtkafbnhud.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jiagoushi.top/gtgcrsfpvp.html

Java: import java.util.List;
来源：http://hz.tanke756.top/gtebbuwzcq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.nwbrower.top/gtsxpsptwt.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.gotoacloud.top/gtzwndqbff.html

C#:   using System.Text;
来源：http://hz.haohaochexian.top/gtanhyypzz.html

[C12] 立即执行函数 IIFE
来源：http://hz.sysykeji.top/gttegnsvpc.html

Py:   (lambda: print("run"))()
来源：http://hz.hammf.cn/gtmgzpwvbp.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jinyuanbaomall.cn/gtriedbnpu.html

JS:   (() => { console.log("run"); })();
来源：http://hz.guowangkeji.top/gtekxvcwlw.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yonumen.top/gtzcgqqzwg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.hammf.cn/gtezhqlwte.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.nanxinkj.top/gtatcecpkd.html

Ruby: -> { puts "run" }.call
来源：http://hz.haohaochexian.top/gtivbiuxag.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yongpay.top/gtovcdimii.html

[C13] 类型声明 / 类型注解
来源：http://hz.gotoacloud.top/gtqpxjslcp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yonumen.top/gtcpchvwpp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ehwqpu.com/gtzwhvrsbf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.vqdsnc.cn/gtazqtvwzp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.chenjidiqi.icu/gtdffuodyw.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jiagoushi.top/gtgcfxgegp.html

Go:   func add(a, b int) int
来源：http://hz.jinghuilouyu.cn/gtqkepgltp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.cdnleiting.top/gthiyusfxz.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.wangdashe.top/gtphiidreh.html

[C14] 泛型函数
来源：http://hz.nanxinkj.top/gtybvxmqwr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.gaohongyu789.top/gtzgfneljt.html

PHP:  // 无泛型
来源：http://hz.hfpthk.cn/gtzrxrakec.html

JS:   // 无泛型
来源：http://hz.yj20258.top/gtbebzsitm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cheryme.top/gtrmeklrgc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yonumen.top/gtpvuyhmha.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zycfv.cn/gtnzfsvfgz.html

Ruby: # 无泛型
来源：http://hz.ydjk.org.cn/gtsdaqtqoh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhongyouzk.top/gthbjektwh.html

[C15] 解构 / 展开参数
来源：http://hz.yonumen.top/gtfdocpaep.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ywan-chungtsiang.top/gtrgvmzhvz.html

PHP:  [$a, $b] = $pair;
来源：http://hz.aizwys.cn/gtxrzgkgqi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jqgufenzy.top/gtlfiqkqbn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.guannengcc.top/gtxbglwyhc.html

Java: // 无解构
来源：http://hz.quarkkingdee.top/gttnmpieao.html

Go:   // 无解构
来源：http://hz.shzxlz.cn/gtrgpuphoq.html

Ruby: a, b = pair
来源：http://hz.gogol.net.cn/gtdfhxfakr.html

C#:   var (a, b) = pair;
来源：http://hz.haohaochexian.top/gtiqtigijn.html

[C16] 函数 / 方法重载
来源：http://hz.yj202588.top/gtmwwxuxnl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.birdmap.top/gtzevhcdmj.html

PHP:  // 无重载
来源：http://hz.nanxinkj.top/gtlgazxlhi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhoulong.xyz/gtykiiizbe.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.sxryk.cn/gtbijawomr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.andypj.xyz/gtdstzjveh.html

Go:   // 无重载：用不同函数名
来源：http://hz.jianghu66.top/gtatwiliui.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hywenlv.cn/gtccabhuib.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.andypj.xyz/gthozlyjza.html

================================================================================
来源：http://hz.chenzaomai.com/gtsdvksbfr.html

D. 数组 / 列表 / 集合
来源：http://hz.feifeiyinyue.top/gtedfaiwqz.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtxcvkwlsj.html

[D01] 创建数组 / 列表
来源：http://hz.svipenyu.cn/gtxrzcennz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ywan-chungtsiang.top/gtrovfkzrq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xinyue.icu/gtoaatfbmp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.daria6918.cn/gtprjlkfkl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xuetiantiany.cn/gtefifmybo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xylfe.cn/gtlirwrdyi.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.fzhhl.top/gtndkvgybz.html

Ruby: arr = [1, 2, 3]
来源：http://hz.ywan-chungtsiang.top/gtqupgtefl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xuanzx.com/gtsarlkzth.html

[D02] 追加元素到末尾
来源：http://hz.chenzaomai.com/gttbzkuefb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.bjfxy.top/gttcloqkiv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yuanzhike.top/gtnhsemwbc.html

JS:   arr.push(4);
来源：http://hz.xinyue.icu/gtchxbcwjl.html

TS:   arr.push(4);
来源：http://hz.gaohongyu789.top/gtcokunlyb.html

Java: list.add(4);
来源：http://hz.sysykeji.top/gtvkqndpcx.html

Go:   arr = append(arr, 4)
来源：http://hz.gaohongyu789.top/gtmzandesb.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.kuanghao11.cn/gtjvefsjzz.html

C#:   list.Add(4);
来源：http://hz.c1oappe.top/gtjfpfjnur.html

[D03] 在指定位置插入元素
来源：http://hz.316326.xyz/gtnanzaauy.html

Py:   arr.insert(0, 0)
来源：http://hz.yuxming.cn/gtntpqpjsm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jqgfzy.top/gtkbyunoxa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jinyuanbaomall.cn/gtumsqohyi.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yuanzhike.top/gthcmuzmne.html

Java: list.add(0, 0);
来源：http://hz.xylfe.cn/gtqbzukzzc.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.sxryk.cn/gthrstafob.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.hnxiangtu.top/gtxkslfjyo.html

C#:   list.Insert(0, 0);
来源：http://hz.xziqi.cn/gtpsocipqf.html

[D04] 删除元素
来源：http://hz.nanxinkj.top/gtchpbprmk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.316326.xyz/gtrcqzstjm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.vqdsnc.cn/gtubnpkxon.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cucudq.cn/gtxbzehofl.html

TS:   arr.splice(0, 1);
来源：http://hz.sxryk.cn/gtgufelhzb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.snrcjt.cn/gtipugduhz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hnqzz.top/gtzdwzlwoz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jqgufenzy.top/gtlroidllw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.mhx1999.top/gtsllyareb.html

[D05] 访问与修改元素
来源：http://hz.wangshuangyany.cn/gtljbajfoe.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhengqikj.top/gtzbfgwjmu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.xuanzx.com/gtjkhkpubb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.0kj1m.cn/gtktsavyog.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ybcxt.top/gtqsbbemec.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ybcxt.top/gtelknzpvg.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.gaohongyu789.top/gtslghrglj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ppjwa.cn/gtjljcsafw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhongyouzk.top/gtggvqfyaf.html

[D06] 数组长度
来源：http://hz.zhiwuduotai.top/gtdujtszkb.html

Py:   len(arr)
来源：http://hz.yj20258.top/gtgzxpaqnp.html

PHP:  count($arr);
来源：http://hz.c1oappe.top/gtbwnzmmxn.html

JS:   arr.length
来源：http://hz.jqgfzy.top/gtdewanwaq.html

TS:   arr.length
来源：http://hz.shzxlz.cn/gtxzqxdouz.html

Java: list.size();
来源：http://hz.hywenlv.cn/gtwfthtgwk.html

Go:   len(arr)
来源：http://hz.yvedp.cn/gtuejwhyiu.html

Ruby: arr.length; arr.size
来源：http://hz.tian-w.cn/gttddglpmo.html

C#:   list.Count;
来源：http://hz.sufxvd.cn/gtyfhzxxjl.html

[D07] 切片 / 取子数组
来源：http://hz.ppjwa.cn/gtlgvifyou.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xinyue.icu/gtsmkagcvs.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.tanke756.top/gtxmyyvexb.html

JS:   arr.slice(1, 4);
来源：http://hz.dianchejie.cn/gtvrcqamvj.html

TS:   arr.slice(1, 4);
来源：http://hz.tianlin.xyz/gtcxrrfoja.html

Java: list.subList(1, 4);
来源：http://hz.iojbl.cn/gtzkorkqhh.html

Go:   arr[1:4]
来源：http://hz.xingfuxueyuan.xyz/gtsitmrjow.html

Ruby: arr[1, 3]
来源：http://hz.chenzaomai.com/gtpnxfenxm.html

C#:   list.GetRange(1, 3);
来源：http://hz.0kj1m.cn/gtaiixclwa.html

[D08] 合并两个数组
来源：http://hz.ywan-chungtsiang.top/gtezssztmq.html

Py:   a + b;  a.extend(b)
来源：http://hz.jlsjyb.cn/gtcafczyfe.html

PHP:  array_merge($a, $b);
来源：http://hz.shzxlz.cn/gttskfsjwr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.guannengcc.top/gtdznwavqk.html

TS:   [...a, ...b];
来源：http://hz.havefunace.top/gtfablrmbt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cdnleiting.top/gtfcoaokvn.html

Go:   append(a, b...)
来源：http://hz.0kj1m.cn/gtfurkfxse.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ivvv.top/gtlwpuikxi.html

C#:   a.Concat(b).ToList()
来源：http://hz.daria6918.cn/gtlklfydfd.html

[D09] 排序（升序）
来源：http://hz.shangyingyoupin.top/gtmrkzkqlk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ybcxt.top/gtqkkqydcg.html

PHP:  sort($arr);
来源：http://hz.9152youxi.cn/gtmwrqlquw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhixingplan.top/gtoiqfgnzz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yj20258.top/gtepxcxgkd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.sysykeji.top/gtjjiwudnq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.snrcjt.cn/gtxzesxecb.html

Ruby: arr.sort
来源：http://hz.aibaodan.cn/gtrncicvgs.html

C#:   list.Sort();
来源：http://hz.chenlongwang.top/gtnrvuocmw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.kuanghao11.cn/gtlrlnfcwm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhiwuduotai.top/gteswmoojc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xinyue.icu/gtqebzwtiw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj202588.top/gtrenxsagj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yonumen.top/gtyplhbnmy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jqgfzy.top/gtzcmoqumn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinqigufen.top/gtnyrgrrgz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hysaishi.cn/gtkpcdggvu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.guannengcc.top/gtaayoeglo.html

[D11] 反转数组
来源：http://hz.vqdsnc.cn/gtfrgwgwnn.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.smart0.xyz/gtjfmhfljn.html

PHP:  array_reverse($arr);
来源：http://hz.jianghu66.top/gtyrjvuxij.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.guannengcc.top/gtefoizsmp.html

TS:   [...arr].reverse();
来源：http://hz.pycfn.com/gtkbubwqbr.html

Java: Collections.reverse(list);
来源：http://hz.sweek.top/gtnurzyjdx.html

Go:   slices.Reverse(arr)
来源：http://hz.yuxming.cn/gtnunoxmsq.html

Ruby: arr.reverse
来源：http://hz.dashuyun.cn/gtjnoduccs.html

C#:   list.Reverse();
来源：http://hz.hywenlv.cn/gtdtflwmox.html

[D12] 查找元素下标
来源：http://hz.shuidangran.top/gtrhxdnavp.html

Py:   arr.index(x);  x in arr
来源：http://hz.xingfuxueyuan.xyz/gtxqvnuqui.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.haohaochexian.top/gtblczbbtk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.pengpengdd.cyou/gtwxmsezha.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hnqzz.top/gtpwnhpltj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xuetiantiany.cn/gtjzdhowev.html

Go:   slices.Index(arr, x)
来源：http://hz.ydjk.org.cn/gtbcvzgoaw.html

Ruby: arr.index(x)
来源：http://hz.havefunace.top/gtmkhkmtfz.html

C#:   list.IndexOf(x);
来源：http://hz.yuxming.cn/gttdsohqna.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jianghu66.top/gtbpkmkocr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.tian-w.cn/gtnnfknmpx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xylfe.cn/gtfpnzvkdk.html

JS:   arr.filter(x => x > 3)
来源：http://hz.52xcode.cn/gtbcyfbvfo.html

TS:   arr.filter(x => x > 3)
来源：http://hz.gzhubu.top/gtndsqdiir.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.316326.xyz/gtvrkkibft.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yj20258.top/gtwxfbfelr.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.svipenyu.cn/gtelmdrkqq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jyoumei.cn/gthapqgcoc.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhiwuduotai.top/gtilawlifc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.nanxinkj.top/gtwxramutg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.cqqwz.cn/gthwfxrhrx.html

JS:   arr.map(x => x * 2)
来源：http://hz.xinyue.icu/gtkvfwnkyf.html

TS:   arr.map(x => x * 2)
来源：http://hz.sysykeji.top/gtoftvzphb.html


<!-- 参考信息 -->