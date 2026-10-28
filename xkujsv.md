代发 wailian999

[B13] 判断是否为数字
来源：http://hz.jinqigfzy.top/gtrsrexkrg.html

Py:   isinstance(x, (int, float))
来源：http://hz.guannengcc.top/gthozbjtdf.html

PHP:  is_numeric($x)
来源：http://hz.52xcode.cn/gtqgywrsyw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.aizwys.cn/gtvwsoilyg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.dashuyun.cn/gtzbslbmzv.html

Java: x instanceof Number
来源：http://hz.kuanghao11.cn/gtryhnocye.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.chenzaomai.com/gtigaajejg.html

Ruby: x.is_a?(Numeric)
来源：http://hz.zhijiandao.cn/gtjzcdsqla.html

C#:   x is int or double or decimal
来源：http://hz.daxiang520.top/gttwjppdza.html

[B14] 判断值是否在集合内
来源：http://hz.nanxinkj.top/gtzjxsnnsd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.xziqi.cn/gtqkkiagcj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.chenjidiqi.icu/gtucxqzvzx.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.shzxlz.cn/gtwnxprugu.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.shangyingyoupin.top/gtgndrzjso.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.daxiang520.top/gtlhostlig.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.snrcjt.cn/gtdbtbqnhz.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jianghu66.top/gttsrepeoq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.sxryk.cn/gtvuhskpbb.html

[B15] 布尔运算与取反
来源：http://hz.bjfxy.top/gtmsjqaubc.html

Py:   a and b or not c
来源：http://hz.chenlongwang.top/gtwbrbzlvy.html

PHP:  $a && $b || !$c
来源：http://hz.xingfuxueyuan.xyz/gtdlqtipis.html

JS:   a && b || !c
来源：http://hz.52xcode.cn/gthexwcfgz.html

TS:   a && b || !c
来源：http://hz.yuxming.cn/gtfdgcgyyo.html

Java: a && b || !c
来源：http://hz.hongshengwenyu.top/gtzpldajas.html

Go:   a && b || !c
来源：http://hz.quarkkingdee.top/gtnztexcvi.html

Ruby: a && b || !c
来源：http://hz.cdnleiting.top/gtxtwmufov.html

C#:   a && b || !c
来源：http://hz.pycfn.com/gtvraoqqqr.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.hammf.cn/gtmeumbogi.html

Py:   if not data: return
来源：http://hz.guowangkeji.top/gthcohovzr.html

PHP:  if (!$data) { return; }
来源：http://hz.yj20258888.top/gtlnppuqfp.html

JS:   if (!data) return;
来源：http://hz.wangdashe.top/gtquerhrgy.html

TS:   if (!data) return;
来源：http://hz.hammf.cn/gthsyjxdsr.html

Java: if (data == null) return;
来源：http://hz.dianchejie.cn/gtjlvbenmx.html

Go:   if data == nil { return }
来源：http://hz.zhoulong.xyz/gtubsmuzev.html

Ruby: return if data.nil?
来源：http://hz.shanyushiyangkeji.top/gtfeflzuzg.html

C#:   if (data == null) return;
来源：http://hz.shangyingyoupin.top/gtkrztlfya.html

================================================================================
来源：http://hz.tian-w.cn/gtdiwimrzj.html

C. 函数与作用域
来源：http://hz.tian-w.cn/gtcdwitdqx.html

================================================================================
来源：http://hz.aibaodan.cn/gtfzcdljge.html

[C01] 定义函数
来源：http://hz.cashguo.top/gtqhiapnkf.html

Py:   def add(a, b): return a + b
来源：http://hz.xingfuxueyuan.xyz/gtjemybphv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenzaomai.com/gtdneqogut.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.cheryme.top/gtgrotaxud.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hywenlv.cn/gthbdxptqm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.andypj.xyz/gttzsgmxyr.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jinqigfzy.top/gtlfxfxqxi.html

Ruby: def add(a, b); a + b; end
来源：http://hz.mhx1999.top/gtctgqeybn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.zdqjudy.top/gtufudzevy.html

[C02] 默认参数
来源：http://hz.chenzaomai.com/gtuiqxzjsg.html

Py:   def greet(name="World"): return name
来源：http://hz.0kj1m.cn/gtoyobczch.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.daria6918.cn/gtmkxsbpum.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.iojbl.cn/gtiramkets.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.ppjwa.cn/gtzuopgrxn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.bjfxy.top/gtzfwfejhx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.sufxvd.cn/gtzdsmxqzz.html

Ruby: def greet(name = "World") = name
来源：http://hz.kuanghao11.cn/gtppakedul.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.nwbrower.top/gtwsgvgjdt.html

[C03] 可变参数
来源：http://hz.yvedp.cn/gtpzmsmuuc.html

Py:   def total(*args): return sum(args)
来源：http://hz.xuetiantiany.cn/gtgbknllqc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.wangshuangyany.cn/gtafuyzmxc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinghuilouyu.cn/gthktzwlub.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.wangshuangyany.cn/gtbwliohvu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.zhiwuduotai.top/gtmsbjdvpt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ywan-chungtsiang.top/gtoyvogzbd.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.shangyingyoupin.top/gtmnttgftj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.aibaodan.cn/gtgqwkflbb.html

[C04] 命名参数 / 关键字参数
来源：http://hz.52xcode.cn/gtmfhkssge.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.chenzaomai.com/gtrbbvvqha.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ywan-chungtsiang.top/gthtusgvxw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jinyuanbaomall.cn/gtckwowzlu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.yuxming.cn/gtvycezddd.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.0kj1m.cn/gtvakgscfs.html

Go:   // 无：用配置结构体参数
来源：http://hz.chenjidiqi.icu/gtcqkxsaog.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hysaishi.cn/gthrcwwwrx.html

C#:   f(a: 1, b: 2)
来源：http://hz.pycfn.com/gtbfvsmudy.html

[C05] 返回多个值
来源：http://hz.sweek.top/gtmzyjpfhz.html

Py:   return a, b
来源：http://hz.dashuyun.cn/gtodngpuvf.html

PHP:  return [$a, $b];
来源：http://hz.shanyushiyangtech.top/gtpskdwerz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.snrcjt.cn/gtsxslehtn.html

TS:   return { a, b };
来源：http://hz.ydjk.org.cn/gttjqecsuf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jqgufenzy.top/gtpeodsmps.html

Go:   return a, b
来源：http://hz.guannengcc.top/gtkfxyjqqz.html

Ruby: return a, b
来源：http://hz.guowangkeji.top/gtalncdsxc.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.haohaochexian.top/gtymwhbsno.html

[C06] 匿名函数 / lambda
来源：http://hz.yj202588.top/gtmtorukeu.html

Py:   square = lambda x: x * x
来源：http://hz.zhoulong.xyz/gtniipqdsj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.nwbrower.top/gtqrifcadr.html

JS:   const square = x => x * x;
来源：http://hz.yanxiufei.cn/gtjxvjftbl.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.nanxuanxn.top/gtimhxhzhi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yj20258.top/gtqcjpgghj.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.pengpengdd.cyou/gtuppttvju.html

Ruby: square = ->(x) { x * x }
来源：http://hz.chenzaomai.com/gtgdchghba.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.ywan-chungtsiang.top/gtjotckrpk.html

[C07] 把函数作为参数传入
来源：http://hz.jinghuilouyu.cn/gtutgagdae.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.gzhubu.top/gtgxnkzjlo.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.vqdsnc.cn/gtnraazgnp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jqgfzy.top/gtjgvlkclt.html

TS:   arr.map(String)
来源：http://hz.cdnleiting.top/gtgmbdzinu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.haohaochexian.top/gtxmzesbxc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.gogol.net.cn/gtfpqhxlwe.html

Ruby: arr.map(&:upcase)
来源：http://hz.yvedp.cn/gtsddavpvo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jinyuanbaomall.cn/gtoorectiy.html

[C08] 闭包
来源：http://hz.jianghu66.top/gtkkbbqlpb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.cashguo.top/gtbadholto.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.quarkkingdee.top/gtkodxiila.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.xinyue.icu/gtoaxxjcgn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jyoumei.cn/gtiznptdib.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.xuetiantiany.cn/gtlqtivics.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.wangdashe.top/gtzjgvjrgc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.yj202588.top/gtpjzfsucb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.jyoumei.cn/gtuscefqza.html

[C09] 递归
来源：http://hz.shanyushiyangkeji.top/gtevvsahti.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.aizwys.cn/gtvkkgjmso.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.sxryk.cn/gtymyrould.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.tian-w.cn/gtsfuzmygl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xziqi.cn/gtfvuexjcf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhaomingkeji.xyz/gtfpxicudc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.hnxiangtu.top/gtuvbacvok.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yonumen.top/gtfbqwcnzf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ehwqpu.com/gtuarrtgwk.html

[C10] 变量作用域
来源：http://hz.cheryme.top/gtpuodflsz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.snrcjt.cn/gtaknisvzt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xziqi.cn/gtpxvrpezr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.gotoacloud.top/gtozipkxsn.html

TS:   同 JS
来源：http://hz.quarkkingdee.top/gtwllumgyu.html

Java: 方法内为块级作用域
来源：http://hz.yueranfly.top/gtdaggzpuz.html

Go:   花括号块级作用域
来源：http://hz.chenlongwang.top/gtfyeshpjs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yanxiufei.cn/gtzqezqcyf.html

C#:   块级作用域
来源：http://hz.nanxuanxn.top/gtiipbjtbw.html

[C11] 模块导入与导出
来源：http://hz.snrcjt.cn/gttvrljjtp.html

Py:   from module import func
来源：http://hz.havefunace.top/gtpgdotprr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jinqigfzy.top/gthwqquvbf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shanyushiyangkeji.top/gtgijzwyfy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.iojbl.cn/gtiybmnarc.html

Java: import java.util.List;
来源：http://hz.daria6918.cn/gtiqpwugpq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.sweek.top/gtowksgkej.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yvedp.cn/gtztsnhsid.html

C#:   using System.Text;
来源：http://hz.pengpengdd.cyou/gtcmrgujbw.html

[C12] 立即执行函数 IIFE
来源：http://hz.gaohongyu789.top/gtnfvjcnwb.html

Py:   (lambda: print("run"))()
来源：http://hz.xziqi.cn/gtwqpdtxug.html

PHP:  (function () { echo "run"; })();
来源：http://hz.kuanghao11.cn/gtblgkucla.html

JS:   (() => { console.log("run"); })();
来源：http://hz.aibaodan.cn/gtlxjmceli.html

TS:   (() => { console.log("run"); })();
来源：http://hz.gotoacloud.top/gtdhrtivhr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zhongyouzk.top/gtogluixob.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.nanxinkj.top/gteqtladmf.html

Ruby: -> { puts "run" }.call
来源：http://hz.aizwys.cn/gtigxtfbpj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hnxiangtu.top/gtdhyalijp.html

[C13] 类型声明 / 类型注解
来源：http://hz.zhoulong.xyz/gtjhycjbmq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hnqzz.top/gtqgbjuqmq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhengqikj.top/gtmqvxqxqf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.xylfe.cn/gtsaoaguhl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gotoacloud.top/gtkwanyprb.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hywenlv.cn/gtigypxvvc.html

Go:   func add(a, b int) int
来源：http://hz.shanyushiyangkeji.top/gtzmyrteac.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.yuxming.cn/gtwnxlmseo.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.ydzc1.top/gtltkshweo.html

[C14] 泛型函数
来源：http://hz.iojbl.cn/gtcgyuwzcm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.chenlongwang.top/gtketwxuse.html

PHP:  // 无泛型
来源：http://hz.hysaishi.cn/gtujorgijj.html

JS:   // 无泛型
来源：http://hz.nwbrower.top/gtaqwhwoit.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.gogol.net.cn/gtysphbgxh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.andypj.xyz/gtagcyvsec.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.gaohongyu789.top/gtvnlstiap.html

Ruby: # 无泛型
来源：http://hz.jyoumei.cn/gtodwmjmxz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.andypj.xyz/gtjdgqxwkw.html

[C15] 解构 / 展开参数
来源：http://hz.hfpthk.cn/gtfdmkwzjm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.iojbl.cn/gtaswmkbsd.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jinghuilouyu.cn/gtyjgyutdz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xingfuxueyuan.xyz/gtqfetrytk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jinghuilouyu.cn/gtxkvvsgrb.html

Java: // 无解构
来源：http://hz.nanxuanxn.top/gtqfquwcbr.html

Go:   // 无解构
来源：http://hz.redwolf501.top/gtvojfhlji.html

Ruby: a, b = pair
来源：http://hz.sysykeji.top/gtrhfqiadg.html

C#:   var (a, b) = pair;
来源：http://hz.chenjidiqi.icu/gtskjluccl.html

[C16] 函数 / 方法重载
来源：http://hz.zhengqikj.top/gtisptfwad.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zhiwuduotai.top/gtkdouktfw.html

PHP:  // 无重载
来源：http://hz.chenzaomai.com/gtxnyzucct.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.xuanzx.com/gtucxlnovm.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hfpthk.cn/gtnsoxjaov.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ydjk.org.cn/gtmenhttaz.html

Go:   // 无重载：用不同函数名
来源：http://hz.tanke756.top/gtxdmwccvb.html

Ruby: # 无重载：靠动态参数
来源：http://hz.0kj1m.cn/gtcplgrppn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yuxming.cn/gtivjybxqu.html

================================================================================
来源：http://hz.gaohongyu789.top/gtcdlctqff.html

D. 数组 / 列表 / 集合
来源：http://hz.xuetiantiany.cn/gtjmvvbadj.html

================================================================================
来源：http://hz.svipenyu.cn/gtvvjrjhrp.html

[D01] 创建数组 / 列表
来源：http://hz.0kj1m.cn/gtpichrtuo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.9152youxi.cn/gthlmrhhhm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xziqi.cn/gtxlckfvnt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jinyuanbaomall.cn/gtzafsdkjk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yj202588.top/gtkhmpcryu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.sxryk.cn/gtrhtduedl.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yonumen.top/gtwpjxicef.html

Ruby: arr = [1, 2, 3]
来源：http://hz.wangshuangyany.cn/gtuzbvawlp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhixingplan.top/gtvwowwlak.html

[D02] 追加元素到末尾
来源：http://hz.sufxvd.cn/gtrxthgqhl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jinyuanbaomall.cn/gtweaqpgno.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.gzhubu.top/gtnagsiyzi.html

JS:   arr.push(4);
来源：http://hz.nanxinkj.top/gttkhcexog.html

TS:   arr.push(4);
来源：http://hz.hnxiangtu.top/gtgllpzyfg.html

Java: list.add(4);
来源：http://hz.gogol.net.cn/gtzhgywnuw.html

Go:   arr = append(arr, 4)
来源：http://hz.aizwys.cn/gtnlysakqa.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.smart0.xyz/gtgoqofvdm.html

C#:   list.Add(4);
来源：http://hz.shzxlz.cn/gtnbxbvrrz.html

[D03] 在指定位置插入元素
来源：http://hz.yongpay.top/gtvotrjjxr.html

Py:   arr.insert(0, 0)
来源：http://hz.hongshengwenyu.top/gtlpdnudct.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.gaohongyu789.top/gtevvvrdec.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.snrcjt.cn/gtkelbcxxf.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yueranfly.top/gtieirlbij.html

Java: list.add(0, 0);
来源：http://hz.kuanghao11.cn/gtzmmsfalz.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shangyingyoupin.top/gtdalhvtuy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yvedp.cn/gtgfhdqfgm.html

C#:   list.Insert(0, 0);
来源：http://hz.cashguo.top/gtorvrkhft.html

[D04] 删除元素
来源：http://hz.xylfe.cn/gtvrtcjkpg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.kuanghao11.cn/gtlsfmojsd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.snrcjt.cn/gttobddfdw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.chenjidiqi.icu/gtkrdnpqtr.html

TS:   arr.splice(0, 1);
来源：http://hz.zhijiandao.cn/gtmivzoegj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jlsjyb.cn/gtwavyqsog.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.sufxvd.cn/gtvzowyqfy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yuanzhike.top/gtmlxwfdxx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.pengpengdd.cyou/gtdxjkkqjz.html

[D05] 访问与修改元素
来源：http://hz.wangdashe.top/gtcortfcbq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.daxiang520.top/gthyrmucis.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.dianchejie.cn/gtqaqvacnr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shanyushiyangtech.top/gtrmozctaq.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.chenlongwang.top/gtfgkdthqd.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zdqjudy.top/gtwzmafupt.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hongshengwenyu.top/gtbylpzshr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shanyushiyangtech.top/gtqkcfaobw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yj202588.top/gtvafpkuzp.html

[D06] 数组长度
来源：http://hz.sxryk.cn/gtximvmtxo.html

Py:   len(arr)
来源：http://hz.tianlin.xyz/gtdcqkxxle.html

PHP:  count($arr);
来源：http://hz.sysykeji.top/gtgpuqrizn.html

JS:   arr.length
来源：http://hz.wangdashe.top/gtwzbakwkb.html

TS:   arr.length
来源：http://hz.gogol.net.cn/gtmyqflezw.html

Java: list.size();
来源：http://hz.xylfe.cn/gtdrwerckc.html

Go:   len(arr)
来源：http://hz.xingfuxueyuan.xyz/gtlijmwsgi.html

Ruby: arr.length; arr.size
来源：http://hz.shangyingyoupin.top/gtaputwxhs.html

C#:   list.Count;
来源：http://hz.chenjidiqi.icu/gtftuslcuq.html

[D07] 切片 / 取子数组
来源：http://hz.jianghu66.top/gtjhjtkoyp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ydjk.org.cn/gtbhhabfyr.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ppjwa.cn/gttnqykjac.html

JS:   arr.slice(1, 4);
来源：http://hz.jinyuanbaomall.cn/gtutrmxlgy.html

TS:   arr.slice(1, 4);
来源：http://hz.jqgfzy.top/gtugpstvpf.html

Java: list.subList(1, 4);
来源：http://hz.zdqjudy.top/gticdhiwuf.html

Go:   arr[1:4]
来源：http://hz.hysaishi.cn/gtkftawtut.html

Ruby: arr[1, 3]
来源：http://hz.yonumen.top/gtnmgcfgrt.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhengqikj.top/gtmdsmvxkr.html

[D08] 合并两个数组
来源：http://hz.tian-w.cn/gtzhohnbte.html

Py:   a + b;  a.extend(b)
来源：http://hz.ppjwa.cn/gtsdaqxovb.html

PHP:  array_merge($a, $b);
来源：http://hz.zhoulong.xyz/gtoaaugvna.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.wangshuangyany.cn/gtrzfybvsa.html

TS:   [...a, ...b];
来源：http://hz.cdnleiting.top/gtxmebadae.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.sweek.top/gtkvduusdk.html

Go:   append(a, b...)
来源：http://hz.ppjwa.cn/gtiycyrewb.html

Ruby: a + b;  a.concat(b)
来源：http://hz.tian-w.cn/gtqaatszzu.html

C#:   a.Concat(b).ToList()
来源：http://hz.aibaodan.cn/gtgtdixyuh.html

[D09] 排序（升序）
来源：http://hz.ybcxt.top/gtfbdvzvww.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hysaishi.cn/gtsrowsthw.html

PHP:  sort($arr);
来源：http://hz.guannengcc.top/gtdtnkrscg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zycfv.cn/gtiekuendm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.quarkkingdee.top/gtqjydiifc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.sysykeji.top/gtopbfyiel.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.fzhhl.top/gtluemdart.html

Ruby: arr.sort
来源：http://hz.sufxvd.cn/gtgvsgmokb.html

C#:   list.Sort();
来源：http://hz.316326.xyz/gtjbulootq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.shangyingyoupin.top/gtoqwvbsvq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.sweek.top/gtznrcueve.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ybcxt.top/gtmsrzypfw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sufxvd.cn/gtdqxeeapq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.haohaochexian.top/gtlpaulnjj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.vqdsnc.cn/gtmmrbehnx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.wangshuangyany.cn/gtgqwhjppv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xingfuxueyuan.xyz/gtlxnwvdpv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinqigfzy.top/gtciduopwg.html

[D11] 反转数组
来源：http://hz.tian-w.cn/gtjvrfklqr.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.fzhhl.top/gtmqclfiuv.html

PHP:  array_reverse($arr);
来源：http://hz.yangfankeji.com/gtgnuwmkco.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.dashuyun.cn/gtzxdlrkmo.html

TS:   [...arr].reverse();
来源：http://hz.c1oappe.top/gtzpkmuijc.html

Java: Collections.reverse(list);
来源：http://hz.yongpay.top/gtwyxiusbo.html

Go:   slices.Reverse(arr)
来源：http://hz.xylfe.cn/gttmqzwxdn.html

Ruby: arr.reverse
来源：http://hz.guannengcc.top/gtnkgauxbw.html

C#:   list.Reverse();
来源：http://hz.yuanzhike.top/gtvzydecoc.html

[D12] 查找元素下标
来源：http://hz.sufxvd.cn/gtcqensilw.html

Py:   arr.index(x);  x in arr
来源：http://hz.316326.xyz/gtsxkbxakt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.sufxvd.cn/gttuutpqwc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.feifeiyinyue.top/gtbotuvomr.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yuanzhike.top/gtxxqcfhrt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.nanxinkj.top/gtfjkpekiz.html

Go:   slices.Index(arr, x)
来源：http://hz.jyoumei.cn/gtxizfoapv.html

Ruby: arr.index(x)
来源：http://hz.zycfv.cn/gtxlxmuumv.html

C#:   list.IndexOf(x);
来源：http://hz.quarkkingdee.top/gtwddeqrql.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yuanzhike.top/gtinfxelwz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jqgfzy.top/gtyqczdntc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.svipenyu.cn/gtgupdzxtg.html

JS:   arr.filter(x => x > 3)
来源：http://hz.svipenyu.cn/gtaijnuklr.html

TS:   arr.filter(x => x > 3)
来源：http://hz.cheryme.top/gtkozdawyd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jqgufenzy.top/gtlrxobguz.html


<!-- 参考信息 -->