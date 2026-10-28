代发 wailian999

C#:   x is int or double or decimal
来源：http://hz.daxiang520.top/gtqoqldtym.html

[B14] 判断值是否在集合内
来源：http://hz.xingfuxueyuan.xyz/gtnqeoyktz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://hz.yj202588.top/gtvqdtjmvp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://hz.aibaodan.cn/gtfvhkaggs.html

JS:   [1, 2, 3].includes(x)
来源：http://hz.yanxiufei.cn/gthahjmfji.html

TS:   [1, 2, 3].includes(x)
来源：http://hz.jlsjyb.cn/gttdpdeiju.html

Java: List.of(1, 2, 3).contains(x)
来源：http://hz.zdqjudy.top/gtvpagnxsa.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://hz.gaohongyu789.top/gtjfrduett.html

Ruby: [1, 2, 3].include?(x)
来源：http://hz.0kj1m.cn/gtbmrumnuk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://hz.hnxiangtu.top/gtydpdewao.html

[B15] 布尔运算与取反
来源：http://hz.ehwqpu.com/gtkehncvjr.html

Py:   a and b or not c
来源：http://hz.zhongyouzk.top/gtwtcgmsgq.html

PHP:  $a && $b || !$c
来源：http://hz.cashguo.top/gttnzasqoq.html

JS:   a && b || !c
来源：http://hz.meibo888.top/gtmbncvxpy.html

TS:   a && b || !c
来源：http://hz.xinyue.icu/gtnyyyucbv.html

Java: a && b || !c
来源：http://hz.c1oappe.top/gtjckhfcfk.html

Go:   a && b || !c
来源：http://hz.vqdsnc.cn/gtitdchqae.html

Ruby: a && b || !c
来源：http://hz.zycfv.cn/gtxcosgxhd.html

C#:   a && b || !c
来源：http://hz.shzxlz.cn/gtejsrmtqe.html

[B16] 卫语句：不满足条件提前返回
来源：http://hz.havefunace.top/gthwtlmklz.html

Py:   if not data: return
来源：http://hz.guannengcc.top/gterzyjtea.html

PHP:  if (!$data) { return; }
来源：http://hz.sysykeji.top/gtgohzgsni.html

JS:   if (!data) return;
来源：http://hz.ywan-chungtsiang.top/gtpktizfnb.html

TS:   if (!data) return;
来源：http://hz.xinyue.icu/gtocglgyxd.html

Java: if (data == null) return;
来源：http://hz.yanxiufei.cn/gtrmpmlmzl.html

Go:   if data == nil { return }
来源：http://hz.fengsongda.top/gtmrbhgbfj.html

Ruby: return if data.nil?
来源：http://hz.yj202588.top/gtmwectwxf.html

C#:   if (data == null) return;
来源：http://hz.smart0.xyz/gtixxnwtkc.html

================================================================================
来源：http://hz.yj20258.top/gtjwnpqwav.html

C. 函数与作用域
来源：http://hz.0kj1m.cn/gtuleklnmx.html

================================================================================
来源：http://hz.gaohongyu789.top/gttxreyczs.html

[C01] 定义函数
来源：http://hz.nwbrower.top/gtcfklytkq.html

Py:   def add(a, b): return a + b
来源：http://hz.c1oappe.top/gtkwklpjxe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhengqikj.top/gteyvynlew.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.tianlin.xyz/gtqdwlzkkz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.guowangkeji.top/gtqtkztleo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.xinyue.icu/gtgtcptajq.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.zycfv.cn/gtsfavktob.html

Ruby: def add(a, b); a + b; end
来源：http://hz.shzxlz.cn/gtruaqlhbl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.redwolf501.top/gtidzyghhk.html

[C02] 默认参数
来源：http://hz.sweek.top/gtbchsfngu.html

Py:   def greet(name="World"): return name
来源：http://hz.yuxming.cn/gtgcihtqxr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.fengsongda.top/gthewmclja.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.dashuyun.cn/gthyvzkols.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.sxryk.cn/gtefmryuyo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.wangdashe.top/gttktcgkfo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.ehwqpu.com/gtwdjmjxjk.html

Ruby: def greet(name = "World") = name
来源：http://hz.wangshuangyany.cn/gtjergruef.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.xylfe.cn/gtcuxeajfx.html

[C03] 可变参数
来源：http://hz.yj20258.top/gttegdiwof.html

Py:   def total(*args): return sum(args)
来源：http://hz.nanxuanxn.top/gtcbqoohbi.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.andypj.xyz/gtoliakasb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jlsjyb.cn/gtqlydxrtz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.chenlongwang.top/gtugdrurec.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hysaishi.cn/gtbtryohdo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.ybcxt.top/gtisxeesld.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.yj20258888.top/gtaompffue.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.9152youxi.cn/gtrbgpwjml.html

[C04] 命名参数 / 关键字参数
来源：http://hz.shzxlz.cn/gtpiobucue.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.bjfxy.top/gturetmsga.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.chenjidiqi.icu/gtuuxpkmop.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.pycfn.com/gttccnmlhp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.birdmap.top/gtajzgychy.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.xuetiantiany.cn/gtytolaiyv.html

Go:   // 无：用配置结构体参数
来源：http://hz.shanyushiyangkeji.top/gtrjjlljhe.html

Ruby: f(a: 1, b: 2)
来源：http://hz.jinyuanbaomall.cn/gttoikdnzu.html

C#:   f(a: 1, b: 2)
来源：http://hz.dashuyun.cn/gtihoghknv.html

[C05] 返回多个值
来源：http://hz.yangfankeji.com/gtalgenzbz.html

Py:   return a, b
来源：http://hz.svipenyu.cn/gttnkasbrt.html

PHP:  return [$a, $b];
来源：http://hz.kuanghao11.cn/gtisjijwfs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.pycfn.com/gtssjhehfc.html

TS:   return { a, b };
来源：http://hz.yangfankeji.com/gtdxifmmnp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.jyoumei.cn/gtkqbeqfou.html

Go:   return a, b
来源：http://hz.zhongyouzk.top/gtvxwsbpzv.html

Ruby: return a, b
来源：http://hz.havefunace.top/gtgsoporva.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.quarkkingdee.top/gtesxibclr.html

[C06] 匿名函数 / lambda
来源：http://hz.zhiwuduotai.top/gtxpgamghy.html

Py:   square = lambda x: x * x
来源：http://hz.yvedp.cn/gtzsiwrlmh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.jinghuilouyu.cn/gtvftkzdfc.html

JS:   const square = x => x * x;
来源：http://hz.52xcode.cn/gtkpnqwwdo.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.ybcxt.top/gtbatntxgc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.wangshuangyany.cn/gtyyywuiwf.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.cucudq.cn/gtzumjyanc.html

Ruby: square = ->(x) { x * x }
来源：http://hz.yvedp.cn/gtqgrvpyke.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.pengpengdd.cyou/gtcrzkqgei.html

[C07] 把函数作为参数传入
来源：http://hz.c1oappe.top/gtzejesybg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.nanxuanxn.top/gtyschigoa.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.haohaochexian.top/gtearyuxhz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.nwbrower.top/gtogedelct.html

TS:   arr.map(String)
来源：http://hz.tianlin.xyz/gtqocuobbu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.shanyushiyangtech.top/gtrfyuvcca.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.cdnleiting.top/gtuistgsjz.html

Ruby: arr.map(&:upcase)
来源：http://hz.hysaishi.cn/gtckxaemrf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.chenzaomai.com/gtjgctjxna.html

[C08] 闭包
来源：http://hz.xziqi.cn/gttxhqelaa.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.pycfn.com/gtywvnipio.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.jinqigfzy.top/gtmtwsgmda.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.dianchejie.cn/gthlfbukpy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.gotoacloud.top/gtgmvkfzlw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.guowangkeji.top/gtzlmbokbu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.yuxming.cn/gtbbcgedby.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.wangdashe.top/gtnaukblks.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.aizwys.cn/gttnjfoknk.html

[C09] 递归
来源：http://hz.daria6918.cn/gtohnzcsfy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.0kj1m.cn/gtqamzsdbh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ivvv.top/gtvmnlerxj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.chenzaomai.com/gtrcjikgeb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.guowangkeji.top/gtqzhdmclq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.cheryme.top/gtclskioep.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.iojbl.cn/gtlyevhnsb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.redwolf501.top/gtdsmsirzi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.316326.xyz/gtankwsfmt.html

[C10] 变量作用域
来源：http://hz.pycfn.com/gtbubrnnni.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.gogol.net.cn/gtplipudyj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.jyoumei.cn/gthjurlski.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhongyouzk.top/gtxsolwksw.html

TS:   同 JS
来源：http://hz.havefunace.top/gtwacjwasg.html

Java: 方法内为块级作用域
来源：http://hz.yanxiufei.cn/gtmzkqkexo.html

Go:   花括号块级作用域
来源：http://hz.shzxlz.cn/gtuvoojjmo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yj202588.top/gtiwkinagb.html

C#:   块级作用域
来源：http://hz.dianchejie.cn/gtyvnfwhva.html

[C11] 模块导入与导出
来源：http://hz.quarkkingdee.top/gtvuibxick.html

Py:   from module import func
来源：http://hz.52xcode.cn/gtkgsbsivu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xziqi.cn/gtbproaqhq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.fzhhl.top/gtuvzoaodw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yueranfly.top/gtsobshzng.html

Java: import java.util.List;
来源：http://hz.yanxiufei.cn/gtckqppvjh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.kuanghao11.cn/gtbzpdljfx.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.iojbl.cn/gtxxwvegtj.html

C#:   using System.Text;
来源：http://hz.sxryk.cn/gtulsyuzoo.html

[C12] 立即执行函数 IIFE
来源：http://hz.cashguo.top/gtvxuiutwc.html

Py:   (lambda: print("run"))()
来源：http://hz.jianghu66.top/gtbfekgegn.html

PHP:  (function () { echo "run"; })();
来源：http://hz.9152youxi.cn/gtcdoawkzp.html

JS:   (() => { console.log("run"); })();
来源：http://hz.yongpay.top/gtyjcendun.html

TS:   (() => { console.log("run"); })();
来源：http://hz.andypj.xyz/gtdlezcppv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.daria6918.cn/gtcjespxwr.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xziqi.cn/gtmutnusof.html

Ruby: -> { puts "run" }.call
来源：http://hz.cheryme.top/gtdkkxgxfk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.cucudq.cn/gtblbxykht.html

[C13] 类型声明 / 类型注解
来源：http://hz.xinyue.icu/gtuvsxnxdr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.shuidangran.top/gtszqsocrh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shanyushiyangkeji.top/gtjuqemasg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.nanxuanxn.top/gtiimqsdaj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhijiandao.cn/gtusbalizg.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.feifeiyinyue.top/gtialaxmia.html

Go:   func add(a, b int) int
来源：http://hz.jyoumei.cn/gtvavxcibh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.52xcode.cn/gtamtsmtio.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jiagoushi.top/gtxkjdqhzb.html

[C14] 泛型函数
来源：http://hz.kuanghao11.cn/gtsxcbqado.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.jlsjyb.cn/gtmeedqzbh.html

PHP:  // 无泛型
来源：http://hz.cqqwz.cn/gtcogjikof.html

JS:   // 无泛型
来源：http://hz.wangdashe.top/gtvztdyelo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yuanzhike.top/gtcrmczmqw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.gogol.net.cn/gtnirnnsgj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhaomingkeji.xyz/gtbqocfcir.html

Ruby: # 无泛型
来源：http://hz.yuanzhike.top/gtdqxahnxf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xuanzx.com/gturhlwafd.html

[C15] 解构 / 展开参数
来源：http://hz.tianlin.xyz/gtdfcndaxu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yj20258888.top/gtbgomuspp.html

PHP:  [$a, $b] = $pair;
来源：http://hz.316326.xyz/gtxfomqmsq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yj20258888.top/gtflkniype.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.pengpengdd.cyou/gtqxvfymhh.html

Java: // 无解构
来源：http://hz.yj202588.top/gtnbkjebkv.html

Go:   // 无解构
来源：http://hz.xingfuxueyuan.xyz/gtysyczmej.html

Ruby: a, b = pair
来源：http://hz.ydjk.org.cn/gtnaqazgjk.html

C#:   var (a, b) = pair;
来源：http://hz.chenjidiqi.icu/gtpmrearqe.html

[C16] 函数 / 方法重载
来源：http://hz.sufxvd.cn/gtqshsexww.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hammf.cn/gtiaezcsis.html

PHP:  // 无重载
来源：http://hz.daria6918.cn/gtgxnegpyi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.wangshuangyany.cn/gtvddokpxh.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.316326.xyz/gtfdoqdjbe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yj20258.top/gtbfxbxxtw.html

Go:   // 无重载：用不同函数名
来源：http://hz.yueranfly.top/gticmmpion.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yuanzhike.top/gtxjukisvm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.wangdashe.top/gtatapeqmq.html

================================================================================
来源：http://hz.yuanzhike.top/gtxwzcdftf.html

D. 数组 / 列表 / 集合
来源：http://hz.nanxinkj.top/gtdfwzekpl.html

================================================================================
来源：http://hz.9152youxi.cn/gtocufdzgl.html

[D01] 创建数组 / 列表
来源：http://hz.yj20258.top/gthwgcpkzk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.smart0.xyz/gttgcgbwjl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.ehwqpu.com/gtgaucmyhs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhiwuduotai.top/gtlptykgwm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.redwolf501.top/gtqafwcgck.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.daria6918.cn/gtlhsbljqy.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ppjwa.cn/gtqxitpgbq.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jqgufenzy.top/gtplyqqzdb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jianghu66.top/gtbyiwhvzo.html

[D02] 追加元素到末尾
来源：http://hz.jqgufenzy.top/gtactjvfno.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xziqi.cn/gtqznkkmza.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cucudq.cn/gtqeynetfm.html

JS:   arr.push(4);
来源：http://hz.jianghu66.top/gtiyhlvsqk.html

TS:   arr.push(4);
来源：http://hz.dianchejie.cn/gtsbzcevvm.html

Java: list.add(4);
来源：http://hz.tanke756.top/gtiiqlxqcr.html

Go:   arr = append(arr, 4)
来源：http://hz.cdnleiting.top/gtwlovslps.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.svipenyu.cn/gtzaonowwm.html

C#:   list.Add(4);
来源：http://hz.jlsjyb.cn/gtuuiwkhae.html

[D03] 在指定位置插入元素
来源：http://hz.gaohongyu789.top/gttfcpmxur.html

Py:   arr.insert(0, 0)
来源：http://hz.hnqzz.top/gtmwlmzlvs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ivvv.top/gtzhyxgyrh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhiwuduotai.top/gtsxtpetcm.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jinyuanbaomall.cn/gtynfffjru.html

Java: list.add(0, 0);
来源：http://hz.smart0.xyz/gtslbwidqz.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jyoumei.cn/gtoxzltrdn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.jqgfzy.top/gtbfkqbnex.html

C#:   list.Insert(0, 0);
来源：http://hz.9152youxi.cn/gtkcmuyucs.html

[D04] 删除元素
来源：http://hz.sufxvd.cn/gtwxamdysy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.bjfxy.top/gtwknguwzm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.0kj1m.cn/gtpbjacogw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hnxiangtu.top/gtsxqifcdx.html

TS:   arr.splice(0, 1);
来源：http://hz.wangdashe.top/gtpizyqbcz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zhongyouzk.top/gtssvglpmm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hfpthk.cn/gtkohcjxyi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.snrcjt.cn/gthyqyugjg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xziqi.cn/gtrzbcpudk.html

[D05] 访问与修改元素
来源：http://hz.quarkkingdee.top/gtsietyjwf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jyoumei.cn/gtjktqsjvg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.pengpengdd.cyou/gtsqsglddh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.guannengcc.top/gtqzazhrry.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jlsjyb.cn/gtvzmoafqi.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yongpay.top/gtbwcsfqyg.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yj20258888.top/gtjyksbcwv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yvedp.cn/gtuqjtfsnw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.9152youxi.cn/gtqprnijxk.html

[D06] 数组长度
来源：http://hz.guowangkeji.top/gttxgevheb.html

Py:   len(arr)
来源：http://hz.wangdashe.top/gtmqwnnvkb.html

PHP:  count($arr);
来源：http://hz.nanxinkj.top/gtxwhrrdol.html

JS:   arr.length
来源：http://hz.kuanghao11.cn/gtvfgrhytt.html

TS:   arr.length
来源：http://hz.nanxuanxn.top/gtjilzqffi.html

Java: list.size();
来源：http://hz.aizwys.cn/gtbcbvddjd.html

Go:   len(arr)
来源：http://hz.yvedp.cn/gttsxpjcuf.html

Ruby: arr.length; arr.size
来源：http://hz.xuetiantiany.cn/gtlhewupij.html

C#:   list.Count;
来源：http://hz.zhiwuduotai.top/gtpkidhwau.html

[D07] 切片 / 取子数组
来源：http://hz.tian-w.cn/gtlrsrsfco.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.havefunace.top/gtgsaodube.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jlsjyb.cn/gteclfsgyn.html

JS:   arr.slice(1, 4);
来源：http://hz.hongshengwenyu.top/gtrtwckgjy.html

TS:   arr.slice(1, 4);
来源：http://hz.jiagoushi.top/gtphxwlzqa.html

Java: list.subList(1, 4);
来源：http://hz.cdnleiting.top/gtgfbcqvxo.html

Go:   arr[1:4]
来源：http://hz.shanyushiyangkeji.top/gtmmewwfbq.html

Ruby: arr[1, 3]
来源：http://hz.quarkkingdee.top/gtlsnknrlb.html

C#:   list.GetRange(1, 3);
来源：http://hz.xingfuxueyuan.xyz/gtkjpmeqha.html

[D08] 合并两个数组
来源：http://hz.shangyingyoupin.top/gtddcxgpze.html

Py:   a + b;  a.extend(b)
来源：http://hz.hywenlv.cn/gtxlrzebsz.html

PHP:  array_merge($a, $b);
来源：http://hz.nanxinkj.top/gtyaymexbg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jqgufenzy.top/gtrkuyhvue.html

TS:   [...a, ...b];
来源：http://hz.shuidangran.top/gtecguqzdq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.nanxuanxn.top/gtgzinuqdt.html

Go:   append(a, b...)
来源：http://hz.zhiwuduotai.top/gtlyseirpw.html

Ruby: a + b;  a.concat(b)
来源：http://hz.haohaochexian.top/gteddzevvc.html

C#:   a.Concat(b).ToList()
来源：http://hz.quarkkingdee.top/gtfrihankp.html

[D09] 排序（升序）
来源：http://hz.cheryme.top/gtgygbbsbk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jianghu66.top/gtokmkoked.html

PHP:  sort($arr);
来源：http://hz.yuanzhike.top/gtpokqgfks.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.daxiang520.top/gtkfkwejcf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yj202588.top/gtvashwkoi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shangyingyoupin.top/gtibikpqvv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.bjfxy.top/gtpqcfnsqh.html

Ruby: arr.sort
来源：http://hz.9152youxi.cn/gtizghrwqv.html

C#:   list.Sort();
来源：http://hz.yanxiufei.cn/gthxaidzcb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xylfe.cn/gtxatrniop.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.haohaochexian.top/gtejmzgacn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.sxryk.cn/gtwuyoilaf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.guannengcc.top/gttjxsuuzc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jianghu66.top/gttbiynfxk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.pengpengdd.cyou/gtmzbihmlx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yvedp.cn/gtlympvtfn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.sufxvd.cn/gtrbfyhkcy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.nanxinkj.top/gtcdysbdlh.html

[D11] 反转数组
来源：http://hz.jinghuilouyu.cn/gtsibbqmuu.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hywenlv.cn/gtvzmhomcq.html

PHP:  array_reverse($arr);
来源：http://hz.cheryme.top/gtidumccbn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yanxiufei.cn/gtftvcofcp.html

TS:   [...arr].reverse();
来源：http://hz.tanke756.top/gthqtonbpr.html

Java: Collections.reverse(list);
来源：http://hz.bjfxy.top/gtehftvadt.html

Go:   slices.Reverse(arr)
来源：http://hz.9152youxi.cn/gtphlmmhto.html

Ruby: arr.reverse
来源：http://hz.hnqzz.top/gtldztikqk.html

C#:   list.Reverse();
来源：http://hz.cucudq.cn/gtvnuzddan.html

[D12] 查找元素下标
来源：http://hz.0kj1m.cn/gtjxbtggxb.html

Py:   arr.index(x);  x in arr
来源：http://hz.jinqigufen.top/gtsurdnzmb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.hammf.cn/gtuyqaueyd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hnxiangtu.top/gtblqelkpv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ywan-chungtsiang.top/gttcxwhbvv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xziqi.cn/gtlerhsljf.html

Go:   slices.Index(arr, x)
来源：http://hz.dianchejie.cn/gtmahmioxi.html

Ruby: arr.index(x)
来源：http://hz.cheryme.top/gtfokhfhvn.html

C#:   list.IndexOf(x);
来源：http://hz.ybcxt.top/gtrfwgodlg.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yangfankeji.com/gtynmhugvq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.xuanzx.com/gtbhgqxcxf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.0kj1m.cn/gtfxbhgtwu.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yuanzhike.top/gtsonmcnzf.html

TS:   arr.filter(x => x > 3)
来源：http://hz.chenzaomai.com/gtjiqbxfsd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yj202588.top/gtsldowpmx.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zycfv.cn/gtixzitzyb.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ydjk.org.cn/gttifbytky.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhoulong.xyz/gtgorypukp.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yueranfly.top/gtjshcapsm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.meibo888.top/gtrqfbsgen.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.svipenyu.cn/gtptymlnhp.html

JS:   arr.map(x => x * 2)
来源：http://hz.guannengcc.top/gtdmafoplt.html

TS:   arr.map(x => x * 2)
来源：http://hz.jqgfzy.top/gtzfmlngcn.html


<!-- 参考信息 -->