代发 wailian999

C#:   x is int or double or decimal
来源：http://hz.gzhubu.top/gtyofitmuf.html

[B14] 判断值是否在集合内
来源：http://hz.bjfxy.top/gtgslyzlti.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yuxming.cn/gtjtzkthxw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.xinyue.icu/gtexzdrexw.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.zhoulong.xyz/gtvmbdxjqg.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.quarkkingdee.top/gticpblzpu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.pycfn.com/gtqbokqnng.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.guowangkeji.top/gthterlamy.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.jinqigufen.top/gtlswczotc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.316326.xyz/gthbktsoul.html

[B15] 布尔运算与取反
来源：http://hz.nanxuanxn.top/gtfwaqcpzq.html

Py:   a and b or not c
来源：http://hz.cdnleiting.top/gtsmygprde.html

PHP:  $a && $b || !$c
来源：http://hz.jinyuanbaomall.cn/gtwxxnnlra.html

JS:   a && b || !c
来源：http://hz.chenzaomai.com/gtsvbbnssk.html

TS:   a && b || !c
来源：http://hz.zhiwuduotai.top/gtqmlhchhe.html

Java: a && b || !c
来源：http://hz.zhaomingkeji.xyz/gtexvimuuu.html

Go:   a && b || !c
来源：http://hz.ehwqpu.com/gtowfbnzxm.html

Ruby: a && b || !c
来源：http://hz.ybcxt.top/gtcrhfhstw.html

C#:   a && b || !c
来源：http://hz.xinyue.icu/gtdzrwhipr.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.guannengcc.top/gteunpafpy.html

Py:   if not data: return
来源：http://hz.yueranfly.top/gtxawweitj.html

PHP:  if (!$data) { return; }
来源：http://hz.yangfankeji.com/gtfizyiaew.html

JS:   if (!data) return;
来源：http://hz.jqgufenzy.top/gtmqpbuuvd.html

TS:   if (!data) return;
来源：http://hz.fengsongda.top/gtfgtwnkuf.html

Java: if (data == null) return;
来源：http://hz.sufxvd.cn/gthqekofrv.html

Go:   if data == nil { return }
来源：http://hz.hywenlv.cn/gtbjqwhlkx.html

Ruby: return if data.nil?
来源：http://hz.jinqigfzy.top/gtbptbcnad.html

C#:   if (data == null) return;
来源：http://hz.mhx1999.top/gtuzkfiqtx.html

================================================================================
来源：http://hz.xziqi.cn/gtjmarjlhx.html

C. 函数与作用域
来源：http://hz.xuetiantiany.cn/gtxfptnylo.html

================================================================================
来源：http://hz.zdqjudy.top/gtbooppfhx.html

[C01] 定义函数
来源：http://hz.hysaishi.cn/gtcszxvtfk.html

Py:   def add(a, b): return a + b
来源：http://hz.cheryme.top/gtzxrcslwc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.gzhubu.top/gtooagtgro.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.xziqi.cn/gtfaaponwt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.cheryme.top/gtmhsbcgws.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xuanzx.com/gtzuybctsz.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.jinqigufen.top/gthutdcogt.html

Ruby: def add(a, b); a + b; end
来源：http://hz.yuxming.cn/gtqllrzhkd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.hnqzz.top/gtgvwsqbvv.html

[C02] 默认参数
来源：http://hz.sweek.top/gtsizdamxc.html

Py:   def greet(name="World"): return name
来源：http://hz.cheryme.top/gtxjcwxxqk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.yangfankeji.com/gtaowmvlsr.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.jyoumei.cn/gtrfrpgipz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yj20258888.top/gtcgygcjnq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.iojbl.cn/gtxjrnxmgk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ywan-chungtsiang.top/gtdcvsflmg.html

Ruby: def greet(name = "World") = name
来源：http://hz.mhx1999.top/gtbfoxirzu.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.shangyingyoupin.top/gtdkldmfkw.html

[C03] 可变参数
来源：http://hz.smart0.xyz/gtsexiwsxs.html

Py:   def total(*args): return sum(args)
来源：http://hz.fengsongda.top/gtokpodndp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.hammf.cn/gtajyyijwe.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.c1oappe.top/gtviltcmyc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jqgufenzy.top/gtloxrlasr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.xingfuxueyuan.xyz/gtqpmzjlrf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.zhengqikj.top/gteiexovbz.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yangfankeji.com/gtkldpwequ.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jinyuanbaomall.cn/gtkaegfzll.html

[C04] 命名参数 / 关键字参数
来源：http://hz.tanke756.top/gtbisvkvzt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.yuanzhike.top/gtazmbiywh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yongpay.top/gtfybfzjcg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.tian-w.cn/gtpwdhcoiw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jqgufenzy.top/gtxwkjewbo.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hfpthk.cn/gtnwiyqexf.html

Go:   // 无：用配置结构体参数
来源：http://hz.meibo888.top/gtcikdktjb.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jqgfzy.top/gtnvhpukop.html

C#:   f(a: 1, b: 2)
来源：http://hz.bjfxy.top/gtaihjruvl.html

[C05] 返回多个值
来源：http://hz.tanke756.top/gtmqedodpg.html

Py:   return a, b
来源：http://hz.shuidangran.top/gtzvpxueom.html

PHP:  return [$a, $b];
来源：http://hz.shanyushiyangkeji.top/gttjiuarnh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jinqigfzy.top/gtdmmtxiwd.html

TS:   return { a, b };
来源：http://hz.ppjwa.cn/gtjqhwyttp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.ydzc1.top/gterhuatxx.html

Go:   return a, b
来源：http://hz.ppjwa.cn/gtvbspgnlb.html

Ruby: return a, b
来源：http://hz.xinyue.icu/gtavpoostq.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhengqikj.top/gtqoqtbihw.html

[C06] 匿名函数 / lambda
来源：http://hz.pengpengdd.cyou/gtchrkmgcc.html

Py:   square = lambda x: x * x
来源：http://hz.shanyushiyangkeji.top/gtvbuaquam.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.shanyushiyangkeji.top/gtckwxnqnu.html

JS:   const square = x => x * x;
来源：http://hz.jinghuilouyu.cn/gtwhozggoj.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.cheryme.top/gtsshlblsb.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.tanke756.top/gtkigzvueb.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.shangyingyoupin.top/gtyzeajvbr.html

Ruby: square = ->(x) { x * x }
来源：http://hz.zhixingplan.top/gtlxcugbcw.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.yj20258888.top/gtrmnbdtvu.html

[C07] 把函数作为参数传入
来源：http://hz.guowangkeji.top/gtaxemmmxs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.quarkkingdee.top/gthrmafibw.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yangfankeji.com/gtnaavewgj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.jinqigufen.top/gtvxwwrnsf.html

TS:   arr.map(String)
来源：http://hz.xziqi.cn/gtovqsnouj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ybcxt.top/gtnbihhrel.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.guannengcc.top/gtvhevcogj.html

Ruby: arr.map(&:upcase)
来源：http://hz.cashguo.top/gtefouurtw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.andypj.xyz/gtxzfgykln.html

[C08] 闭包
来源：http://hz.jinqigufen.top/gtngacqrzu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.gaohongyu789.top/gticzdlsya.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.redwolf501.top/gtzwfonycz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.316326.xyz/gtfsndvjfd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.quarkkingdee.top/gtjkwtduls.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jinyuanbaomall.cn/gtocxcczzi.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ywan-chungtsiang.top/gttnfezxmi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.hysaishi.cn/gtgzkvmjwl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.316326.xyz/gterlokwqh.html

[C09] 递归
来源：http://hz.xziqi.cn/gtrchaatfl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.xinyue.icu/gtnczzgwcf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.aibaodan.cn/gthtkundqh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhongyouzk.top/gttmmybgli.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sufxvd.cn/gtyrjegavx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.pycfn.com/gticluweut.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhoulong.xyz/gtsfcfsssa.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.birdmap.top/gtfqwslxgb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.sysykeji.top/gtbtqnywna.html

[C10] 变量作用域
来源：http://hz.jlsjyb.cn/gtfrznuhlt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.quarkkingdee.top/gtxdyrdwlc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.guannengcc.top/gtfewuhheo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.chenjidiqi.icu/gtvrfqhodj.html

TS:   同 JS
来源：http://hz.snrcjt.cn/gtvlshzome.html

Java: 方法内为块级作用域
来源：http://hz.yanxiufei.cn/gtamkdpcry.html

Go:   花括号块级作用域
来源：http://hz.mhx1999.top/gtscnxozmc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jinqigufen.top/gthgefdyun.html

C#:   块级作用域
来源：http://hz.dashuyun.cn/gtmqypjabc.html

[C11] 模块导入与导出
来源：http://hz.cdnleiting.top/gtfseblecj.html

Py:   from module import func
来源：http://hz.cheryme.top/gtdapkstbt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.jyoumei.cn/gtlgsgyyyl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.daxiang520.top/gtfjmniyge.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.chenzaomai.com/gtkjfebift.html

Java: import java.util.List;
来源：http://hz.sweek.top/gtfhcdkcya.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.aizwys.cn/gtwihxvfgy.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.fengsongda.top/gttpkgvudy.html

C#:   using System.Text;
来源：http://hz.ppjwa.cn/gtprtknfrg.html

[C12] 立即执行函数 IIFE
来源：http://hz.xuanzx.com/gtbphesjue.html

Py:   (lambda: print("run"))()
来源：http://hz.shanyushiyangtech.top/gtmdinqmmo.html

PHP:  (function () { echo "run"; })();
来源：http://hz.xylfe.cn/gtsbgcixaw.html

JS:   (() => { console.log("run"); })();
来源：http://hz.smart0.xyz/gtnhyyogtr.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cqqwz.cn/gtlzifwpjs.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.smart0.xyz/gtblspntgi.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shangyingyoupin.top/gtxhyynook.html

Ruby: -> { puts "run" }.call
来源：http://hz.xingfuxueyuan.xyz/gtvdsmgwke.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yanxiufei.cn/gtcpzyrhak.html

[C13] 类型声明 / 类型注解
来源：http://hz.daria6918.cn/gtzmhysdis.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ivvv.top/gtupbhwvcb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zycfv.cn/gtfjynaooz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.wangshuangyany.cn/gthvzqnvhf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hysaishi.cn/gtgrfchnce.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cheryme.top/gtkhrnhqwz.html

Go:   func add(a, b int) int
来源：http://hz.cdnleiting.top/gtmbbomzwj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.xylfe.cn/gtnadmghqk.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yanxiufei.cn/gtwmkvonrj.html

[C14] 泛型函数
来源：http://hz.kuanghao11.cn/gtbthxngtm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zdqjudy.top/gtghfrllpr.html

PHP:  // 无泛型
来源：http://hz.shanyushiyangtech.top/gtnwfqmhvo.html

JS:   // 无泛型
来源：http://hz.nanxinkj.top/gtzsbfjlyy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hammf.cn/gtyxksnsjn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.cqqwz.cn/gtwvijkzva.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shangyingyoupin.top/gtvwcdtqsz.html

Ruby: # 无泛型
来源：http://hz.andypj.xyz/gtksdcxrdt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhoulong.xyz/gtcqpatciq.html

[C15] 解构 / 展开参数
来源：http://hz.iojbl.cn/gtngydcarr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhaomingkeji.xyz/gtekajnhnl.html

PHP:  [$a, $b] = $pair;
来源：http://hz.xinyue.icu/gtloeuswio.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jianghu66.top/gtrzlxagde.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.guowangkeji.top/gtnoakaznm.html

Java: // 无解构
来源：http://hz.yj20258.top/gtfxsmiuqv.html

Go:   // 无解构
来源：http://hz.vqdsnc.cn/gtfdmvynxm.html

Ruby: a, b = pair
来源：http://hz.chenlongwang.top/gtgmfqhgyf.html

C#:   var (a, b) = pair;
来源：http://hz.cashguo.top/gtxpgspsae.html

[C16] 函数 / 方法重载
来源：http://hz.haohaochexian.top/gtflxzmlia.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.redwolf501.top/gtvjdgbsxf.html

PHP:  // 无重载
来源：http://hz.nwbrower.top/gtpouakyum.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yj202588.top/gtynmbjeid.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.sufxvd.cn/gtabeujpdu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.gaohongyu789.top/gtiigcwmxc.html

Go:   // 无重载：用不同函数名
来源：http://hz.aibaodan.cn/gtliaryfyw.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xziqi.cn/gtcydrijan.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hongshengwenyu.top/gticggdzku.html

================================================================================
来源：http://hz.yanxiufei.cn/gtkpawjwpz.html

D. 数组 / 列表 / 集合
来源：http://hz.xuanzx.com/gthlyvapcl.html

================================================================================
来源：http://hz.jianghu66.top/gtbjopnhuc.html

[D01] 创建数组 / 列表
来源：http://hz.birdmap.top/gtvjqrutml.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.dashuyun.cn/gtkjwfoebj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jyoumei.cn/gtaeyetolc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.nanxinkj.top/gthbumafxi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zdqjudy.top/gtrlzpvqig.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.havefunace.top/gtdsuchqnu.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.aibaodan.cn/gtixneypnj.html

Ruby: arr = [1, 2, 3]
来源：http://hz.dianchejie.cn/gtvuilajlw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.cucudq.cn/gtwumsaicl.html

[D02] 追加元素到末尾
来源：http://hz.cashguo.top/gtgpsxxpnd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhixingplan.top/gtmcvrsebr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jinqigufen.top/gtthdcuhro.html

JS:   arr.push(4);
来源：http://hz.jlsjyb.cn/gtuhzyobrq.html

TS:   arr.push(4);
来源：http://hz.gotoacloud.top/gtrxbbtxvp.html

Java: list.add(4);
来源：http://hz.jyoumei.cn/gtbgludbif.html

Go:   arr = append(arr, 4)
来源：http://hz.mhx1999.top/gtjnjclivs.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.aibaodan.cn/gtxwqkirbh.html

C#:   list.Add(4);
来源：http://hz.nanxuanxn.top/gtigcpeepf.html

[D03] 在指定位置插入元素
来源：http://hz.zdqjudy.top/gtqnbkzfsk.html

Py:   arr.insert(0, 0)
来源：http://hz.gogol.net.cn/gteqkzxvjl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.316326.xyz/gtdhpaidho.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.daria6918.cn/gtgwwgawnt.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yonumen.top/gtyizetanv.html

Java: list.add(0, 0);
来源：http://hz.wangshuangyany.cn/gtjhdgzsoc.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.wangdashe.top/gtalrgrllf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jinyuanbaomall.cn/gtquxsrqrm.html

C#:   list.Insert(0, 0);
来源：http://hz.xinyue.icu/gtwsmjmsml.html

[D04] 删除元素
来源：http://hz.jqgfzy.top/gttbmbxhlp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.c1oappe.top/gtxhbuwzpt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.wangdashe.top/gtvbfjdzzw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.andypj.xyz/gtprgftsnx.html

TS:   arr.splice(0, 1);
来源：http://hz.yueranfly.top/gtecmvdhfb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jiagoushi.top/gtdgzfdcch.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.shanyushiyangkeji.top/gtupfgchio.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.sxryk.cn/gtxyjmbbza.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.wangshuangyany.cn/gteudyvmzc.html

[D05] 访问与修改元素
来源：http://hz.ehwqpu.com/gtlxlycncf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yvedp.cn/gtibiguoyz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sweek.top/gticmnmylb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.chenlongwang.top/gtrmiwowte.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.smart0.xyz/gtmrtziakb.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.c1oappe.top/gttfwwltbf.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jianghu66.top/gtmlyndqtv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.wangshuangyany.cn/gtiuemjaxn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.bjfxy.top/gtowcaithh.html

[D06] 数组长度
来源：http://hz.chenzaomai.com/gthvpmldie.html

Py:   len(arr)
来源：http://hz.hnxiangtu.top/gtwniprjea.html

PHP:  count($arr);
来源：http://hz.jinghuilouyu.cn/gtcdiafhbu.html

JS:   arr.length
来源：http://hz.ydjk.org.cn/gtfwkfksfi.html

TS:   arr.length
来源：http://hz.yongpay.top/gtvkincwpg.html

Java: list.size();
来源：http://hz.haohaochexian.top/gtcfkijvng.html

Go:   len(arr)
来源：http://hz.sweek.top/gttayvotyg.html

Ruby: arr.length; arr.size
来源：http://hz.sweek.top/gtdwyjqqkd.html

C#:   list.Count;
来源：http://hz.hnqzz.top/gtrifqfoez.html

[D07] 切片 / 取子数组
来源：http://hz.cheryme.top/gthyjvpsfo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ywan-chungtsiang.top/gtmdntnnea.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hywenlv.cn/gtjwveklsw.html

JS:   arr.slice(1, 4);
来源：http://hz.shangyingyoupin.top/gtytibcthe.html

TS:   arr.slice(1, 4);
来源：http://hz.hammf.cn/gthdjjytnb.html

Java: list.subList(1, 4);
来源：http://hz.zhengqikj.top/gtryoxcalt.html

Go:   arr[1:4]
来源：http://hz.shanyushiyangtech.top/gtnjtwfxkz.html

Ruby: arr[1, 3]
来源：http://hz.mhx1999.top/gtqkzoflgt.html

C#:   list.GetRange(1, 3);
来源：http://hz.yj20258888.top/gtqvgricwp.html

[D08] 合并两个数组
来源：http://hz.ywan-chungtsiang.top/gtkxakvrhi.html

Py:   a + b;  a.extend(b)
来源：http://hz.ppjwa.cn/gthxmrwbmv.html

PHP:  array_merge($a, $b);
来源：http://hz.aibaodan.cn/gtxivjovky.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hysaishi.cn/gtqfpjhkhb.html

TS:   [...a, ...b];
来源：http://hz.sufxvd.cn/gtcvrigrnr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.aizwys.cn/gtdgkixfxi.html

Go:   append(a, b...)
来源：http://hz.ybcxt.top/gtjnvxbyli.html

Ruby: a + b;  a.concat(b)
来源：http://hz.nanxuanxn.top/gthsxsqhbs.html

C#:   a.Concat(b).ToList()
来源：http://hz.316326.xyz/gtsouazdlx.html

[D09] 排序（升序）
来源：http://hz.aibaodan.cn/gtuzbdcdfx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yanxiufei.cn/gtkjhtwqkr.html

PHP:  sort($arr);
来源：http://hz.jlsjyb.cn/gtmzzciaso.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.cdnleiting.top/gtsyllthei.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.redwolf501.top/gtmpsghull.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hammf.cn/gtzhjtcaql.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yj202588.top/gtbpzdhunk.html

Ruby: arr.sort
来源：http://hz.ydjk.org.cn/gtswxviniv.html

C#:   list.Sort();
来源：http://hz.svipenyu.cn/gtpipiqyfy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.316326.xyz/gtafzhytbw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yongpay.top/gtknjdgztd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinghuilouyu.cn/gtljeuyqlh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.svipenyu.cn/gttvocmlad.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sweek.top/gtlcawglvu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cqqwz.cn/gtpjoylpqz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.svipenyu.cn/gturtsdizn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.tian-w.cn/gtqrtgviym.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhengqikj.top/gtnaptdffu.html

[D11] 反转数组
来源：http://hz.snrcjt.cn/gtqtffvuxq.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.iojbl.cn/gtuocqilrd.html

PHP:  array_reverse($arr);
来源：http://hz.fzhhl.top/gttdmrbwqp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zycfv.cn/gtvhmkprpv.html

TS:   [...arr].reverse();
来源：http://hz.ydjk.org.cn/gtpqzjfvog.html

Java: Collections.reverse(list);
来源：http://hz.jlsjyb.cn/gtmbgmkhme.html

Go:   slices.Reverse(arr)
来源：http://hz.wangshuangyany.cn/gtytinkvxl.html

Ruby: arr.reverse
来源：http://hz.zhoulong.xyz/gtrdhspibi.html

C#:   list.Reverse();
来源：http://hz.dashuyun.cn/gtmupjomni.html

[D12] 查找元素下标
来源：http://hz.zhijiandao.cn/gtkhwduklo.html

Py:   arr.index(x);  x in arr
来源：http://hz.52xcode.cn/gtsbvifsrb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ydjk.org.cn/gtjjimhwpz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenzaomai.com/gtfjxgjjrx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xziqi.cn/gtlfmsregs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xuetiantiany.cn/gtdtvbnhfr.html

Go:   slices.Index(arr, x)
来源：http://hz.ydjk.org.cn/gtjeendhre.html

Ruby: arr.index(x)
来源：http://hz.yangfankeji.com/gtjdhctybp.html

C#:   list.IndexOf(x);
来源：http://hz.cqqwz.cn/gtsezrfdto.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hnxiangtu.top/gtwjkuokjs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.svipenyu.cn/gtgjbfuhaf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yueranfly.top/gthtfygbze.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ppjwa.cn/gtvvzpgjxb.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yongpay.top/gthrvnnedb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jqgfzy.top/gtkamysbxm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.316326.xyz/gtxdndcaye.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.svipenyu.cn/gtqhitmxyz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhijiandao.cn/gtqhknfqiy.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ivvv.top/gtoaaefahv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.tanke756.top/gtdfykbdby.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jlsjyb.cn/gtdvwqaqzs.html

JS:   arr.map(x => x * 2)
来源：http://hz.daxiang520.top/gttldvemuc.html

TS:   arr.map(x => x * 2)
来源：http://hz.zdqjudy.top/gtjuctdjru.html


<!-- 参考信息 -->