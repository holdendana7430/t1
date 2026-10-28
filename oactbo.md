代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.tanke756.top/gtaokrfcqj.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.tianlin.xyz/gtljymzziw.html

Ruby: def add(a, b); a + b; end
来源：http://hz.daxiang520.top/gtbejjgdwf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.shangyingyoupin.top/gttqktkpht.html

[C02] 默认参数
来源：http://hz.yj20258.top/gtveznxnmi.html

Py:   def greet(name="World"): return name
来源：http://hz.hnxiangtu.top/gtkcobpmsc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.fengsongda.top/gtzauhxisv.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.hongshengwenyu.top/gtatzdwxbd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.redwolf501.top/gttdtvjiba.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.zhengqikj.top/gtetcbljtd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yangfankeji.com/gtxrewzugg.html

Ruby: def greet(name = "World") = name
来源：http://hz.fengsongda.top/gtleplushy.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.fengsongda.top/gtwysxmdja.html

[C03] 可变参数
来源：http://hz.xuetiantiany.cn/gtunyryvqx.html

Py:   def total(*args): return sum(args)
来源：http://hz.sufxvd.cn/gtpcgycusz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.cheryme.top/gtaxbjtuyk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hongshengwenyu.top/gtpataobey.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.hammf.cn/gtwhekinyr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.ybcxt.top/gtaxowjgri.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.hongshengwenyu.top/gtwbudzzde.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.cashguo.top/gttdydffly.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.shanyushiyangkeji.top/gtyepfiwzf.html

[C04] 命名参数 / 关键字参数
来源：http://hz.cdnleiting.top/gtrsalmdgd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.cdnleiting.top/gthpwreqse.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.svipenyu.cn/gtprxazems.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.guowangkeji.top/gtmzpsyjfu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.xylfe.cn/gtzzsoqkow.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.zhijiandao.cn/gtcjgxnyww.html

Go:   // 无：用配置结构体参数
来源：http://hz.yonumen.top/gtocjowtmn.html

Ruby: f(a: 1, b: 2)
来源：http://hz.xziqi.cn/gtitcryizc.html

C#:   f(a: 1, b: 2)
来源：http://hz.yongpay.top/gtwaafwirj.html

[C05] 返回多个值
来源：http://hz.sysykeji.top/gtuwpjexxn.html

Py:   return a, b
来源：http://hz.nanxinkj.top/gtkoenryrz.html

PHP:  return [$a, $b];
来源：http://hz.feifeiyinyue.top/gtgbwxttyq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.yvedp.cn/gtoeyfsfkr.html

TS:   return { a, b };
来源：http://hz.zycfv.cn/gtdeshyqsi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.aizwys.cn/gtscvtmxrq.html

Go:   return a, b
来源：http://hz.0kj1m.cn/gttarfebsr.html

Ruby: return a, b
来源：http://hz.zhijiandao.cn/gtcpaxlfis.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.xuanzx.com/gtiqshksuo.html

[C06] 匿名函数 / lambda
来源：http://hz.cucudq.cn/gtjrkalnnm.html

Py:   square = lambda x: x * x
来源：http://hz.iojbl.cn/gtbrtzqdjv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.wangdashe.top/gtafnvhmlv.html

JS:   const square = x => x * x;
来源：http://hz.ivvv.top/gtyiimtbwn.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.daria6918.cn/gtufxkafqw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.bjfxy.top/gtkhzhqfga.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.cashguo.top/gtikhsmlju.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shzxlz.cn/gtdnttxyau.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shzxlz.cn/gtsrnlxziy.html

[C07] 把函数作为参数传入
来源：http://hz.feifeiyinyue.top/gtsrzzkzka.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yj20258888.top/gtsvhcahjg.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jianghu66.top/gtohikantp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.andypj.xyz/gtpsjrwove.html

TS:   arr.map(String)
来源：http://hz.yueranfly.top/gtppjgheer.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.daria6918.cn/gthwvtynuh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.iojbl.cn/gtpeirrvhn.html

Ruby: arr.map(&:upcase)
来源：http://hz.sysykeji.top/gtzuotjhtn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.mhx1999.top/gtizhwaqjm.html

[C08] 闭包
来源：http://hz.ywan-chungtsiang.top/gtybvbomdy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yj20258.top/gtfnbkmvuv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zycfv.cn/gtgrqsyfsm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.gaohongyu789.top/gtfvhgljpc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.jlsjyb.cn/gtsmvfjssy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.xuanzx.com/gtjdlwbxkc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.ybcxt.top/gtdfafedhe.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.feifeiyinyue.top/gthflyvwjw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhengqikj.top/gtganiypvr.html

[C09] 递归
来源：http://hz.birdmap.top/gtmecanwcw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.52xcode.cn/gtqjbtzwff.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.fzhhl.top/gthjcqetuu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhaomingkeji.xyz/gtwutcdqeh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shzxlz.cn/gtpfqxvpdf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.ybcxt.top/gtwocicbls.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.daria6918.cn/gtmsamomsn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.feifeiyinyue.top/gtcyweflvq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.tianlin.xyz/gtjnixipnp.html

[C10] 变量作用域
来源：http://hz.zdqjudy.top/gtdlkfvdpa.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.chenlongwang.top/gtxaiboavg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.tanke756.top/gtqdtfqlqg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.pengpengdd.cyou/gttdutncax.html

TS:   同 JS
来源：http://hz.yj20258888.top/gtgtnzflxn.html

Java: 方法内为块级作用域
来源：http://hz.sufxvd.cn/gtiudszzuj.html

Go:   花括号块级作用域
来源：http://hz.sufxvd.cn/gtroeuqqif.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.bjfxy.top/gtngtvfgbq.html

C#:   块级作用域
来源：http://hz.iojbl.cn/gtepkpkzwr.html

[C11] 模块导入与导出
来源：http://hz.fengsongda.top/gtuxorkolx.html

Py:   from module import func
来源：http://hz.meibo888.top/gtlvlkhdyv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.nwbrower.top/gtclkcrlpo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jinqigufen.top/gtjwjyfche.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.cqqwz.cn/gtwveqbvsh.html

Java: import java.util.List;
来源：http://hz.cheryme.top/gtzatucmmg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yvedp.cn/gtopejfwwi.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jqgfzy.top/gtogtqlget.html

C#:   using System.Text;
来源：http://hz.xinyue.icu/gtlalebdvm.html

[C12] 立即执行函数 IIFE
来源：http://hz.yj20258888.top/gtojgszuid.html

Py:   (lambda: print("run"))()
来源：http://hz.ywan-chungtsiang.top/gtzibqkngh.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jinqigfzy.top/gtuyouqbma.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xylfe.cn/gtkebcevks.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cdnleiting.top/gtxipgjikl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.sxryk.cn/gtvunxxopz.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.yongpay.top/gtcbtzwywh.html

Ruby: -> { puts "run" }.call
来源：http://hz.cucudq.cn/gtvmudzjbb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.cdnleiting.top/gtykkqpqft.html

[C13] 类型声明 / 类型注解
来源：http://hz.jinyuanbaomall.cn/gtymgdpyyl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yueranfly.top/gtnkxxblvt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinghuilouyu.cn/gtuerwlfip.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.fengsongda.top/gtkkbatezd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.fengsongda.top/gtkpctzpvu.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.aibaodan.cn/gtzmxmwgzq.html

Go:   func add(a, b int) int
来源：http://hz.shuidangran.top/gtyklknutr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.xinyue.icu/gtdvrouqfn.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.chenzaomai.com/gtsphjnybr.html

[C14] 泛型函数
来源：http://hz.shuidangran.top/gtjdwmkgdb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhoulong.xyz/gtrulqkmey.html

PHP:  // 无泛型
来源：http://hz.0kj1m.cn/gtgibfnvzj.html

JS:   // 无泛型
来源：http://hz.jinqigufen.top/gtrpchqngh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.redwolf501.top/gtdtofcdjm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.wangshuangyany.cn/gtsnzzhjho.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.birdmap.top/gtvvpesevz.html

Ruby: # 无泛型
来源：http://hz.nwbrower.top/gtkqrtncai.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.shuidangran.top/gtbjwkjvkh.html

[C15] 解构 / 展开参数
来源：http://hz.yvedp.cn/gtybfrrscd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhengqikj.top/gthghqynxl.html

PHP:  [$a, $b] = $pair;
来源：http://hz.birdmap.top/gtoxznhhjt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.aizwys.cn/gtxaagywuf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yuxming.cn/gtobxaaswj.html

Java: // 无解构
来源：http://hz.ehwqpu.com/gtreviqnpu.html

Go:   // 无解构
来源：http://hz.jyoumei.cn/gtodqfxotb.html

Ruby: a, b = pair
来源：http://hz.shanyushiyangtech.top/gtnehiitvg.html

C#:   var (a, b) = pair;
来源：http://hz.svipenyu.cn/gtcfwsnxty.html

[C16] 函数 / 方法重载
来源：http://hz.aibaodan.cn/gtsqvwgwlu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jinqigfzy.top/gtfsnanvfz.html

PHP:  // 无重载
来源：http://hz.c1oappe.top/gtmkeurolm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.wangshuangyany.cn/gtflduizxz.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ehwqpu.com/gtvaujitbt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.gogol.net.cn/gtbnbqsdqv.html

Go:   // 无重载：用不同函数名
来源：http://hz.0kj1m.cn/gtxpyodfty.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zycfv.cn/gtcfjkayha.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.chenjidiqi.icu/gtsmthpjrg.html

================================================================================
来源：http://hz.tianlin.xyz/gtjhypawfk.html

D. 数组 / 列表 / 集合
来源：http://hz.yanxiufei.cn/gtsysvzpph.html

================================================================================
来源：http://hz.0kj1m.cn/gtihanbjey.html

[D01] 创建数组 / 列表
来源：http://hz.guannengcc.top/gtoudcxgkf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.dianchejie.cn/gtqdvzkhzx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.pycfn.com/gtwfdsddnx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.pycfn.com/gtyazpzdsz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.andypj.xyz/gtgztfextf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhixingplan.top/gtaxqkpoyl.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ydzc1.top/gtnhkgjomr.html

Ruby: arr = [1, 2, 3]
来源：http://hz.xuanzx.com/gthpvztnbo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yonumen.top/gtmaovvpis.html

[D02] 追加元素到末尾
来源：http://hz.dashuyun.cn/gtplkjhnde.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.wangshuangyany.cn/gtvholpygw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.chenlongwang.top/gtxnrksqxb.html

JS:   arr.push(4);
来源：http://hz.sweek.top/gtzwmpcftk.html

TS:   arr.push(4);
来源：http://hz.ydzc1.top/gthbmjlava.html

Java: list.add(4);
来源：http://hz.fzhhl.top/gtsxzockki.html

Go:   arr = append(arr, 4)
来源：http://hz.chenlongwang.top/gtbciqgqik.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.pycfn.com/gtwoxjuatq.html

C#:   list.Add(4);
来源：http://hz.jqgufenzy.top/gtobfljayd.html

[D03] 在指定位置插入元素
来源：http://hz.feifeiyinyue.top/gtzchgkfeq.html

Py:   arr.insert(0, 0)
来源：http://hz.xingfuxueyuan.xyz/gttqzfglts.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.aibaodan.cn/gtajjxogji.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.shzxlz.cn/gtewqbqsie.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.chenlongwang.top/gtqerydqgp.html

Java: list.add(0, 0);
来源：http://hz.daria6918.cn/gtwvrmtsgz.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yj20258.top/gttxirhcjb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.bjfxy.top/gtgxixsrux.html

C#:   list.Insert(0, 0);
来源：http://hz.xziqi.cn/gtqjhnvjyb.html

[D04] 删除元素
来源：http://hz.mhx1999.top/gthgpfeofi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.daxiang520.top/gtidrpecto.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.shuidangran.top/gtxzczbgii.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cqqwz.cn/gtvsbtcltb.html

TS:   arr.splice(0, 1);
来源：http://hz.ehwqpu.com/gtvhsclrsj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.gaohongyu789.top/gtiiyfcclp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.birdmap.top/gtxqlrodkz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.chenzaomai.com/gtcvwisbuv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shangyingyoupin.top/gtdticldji.html

[D05] 访问与修改元素
来源：http://hz.jianghu66.top/gtkepnzyyi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.9152youxi.cn/gtwscdnavl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.nanxuanxn.top/gtpkekmkbm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.ydjk.org.cn/gtqrsxvxlr.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.316326.xyz/gtvlwbuzsi.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hammf.cn/gtnfbqtkdt.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.tanke756.top/gtdauyrpob.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cqqwz.cn/gtloqacvhe.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinqigfzy.top/gtadzhftce.html

[D06] 数组长度
来源：http://hz.shzxlz.cn/gtimaazjar.html

Py:   len(arr)
来源：http://hz.yuxming.cn/gtxplpwilz.html

PHP:  count($arr);
来源：http://hz.jianghu66.top/gtmnpihtpy.html

JS:   arr.length
来源：http://hz.guowangkeji.top/gtujgcsual.html

TS:   arr.length
来源：http://hz.fengsongda.top/gtdzteckhh.html

Java: list.size();
来源：http://hz.316326.xyz/gtvcfdbvdt.html

Go:   len(arr)
来源：http://hz.sxryk.cn/gtndnezibs.html

Ruby: arr.length; arr.size
来源：http://hz.haohaochexian.top/gthehybzcw.html

C#:   list.Count;
来源：http://hz.ppjwa.cn/gtjkfkkptf.html

[D07] 切片 / 取子数组
来源：http://hz.xingfuxueyuan.xyz/gtwuusdkpb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.redwolf501.top/gtewivuovf.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.fengsongda.top/gtbbemdxkb.html

JS:   arr.slice(1, 4);
来源：http://hz.wangdashe.top/gteksncjgg.html

TS:   arr.slice(1, 4);
来源：http://hz.wangdashe.top/gtmwawlzlu.html

Java: list.subList(1, 4);
来源：http://hz.guannengcc.top/gttvggjnpz.html

Go:   arr[1:4]
来源：http://hz.xuetiantiany.cn/gtzgdaogfj.html

Ruby: arr[1, 3]
来源：http://hz.zhaomingkeji.xyz/gtckjbhgqs.html

C#:   list.GetRange(1, 3);
来源：http://hz.yueranfly.top/gtizyslglf.html

[D08] 合并两个数组
来源：http://hz.xuetiantiany.cn/gtzwrilwrb.html

Py:   a + b;  a.extend(b)
来源：http://hz.svipenyu.cn/gtwibnsyan.html

PHP:  array_merge($a, $b);
来源：http://hz.zycfv.cn/gtyihtotum.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.c1oappe.top/gtykzphdwl.html

TS:   [...a, ...b];
来源：http://hz.guowangkeji.top/gtfjdoieev.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hnxiangtu.top/gtmrwlcqtw.html

Go:   append(a, b...)
来源：http://hz.yj20258.top/gtykbishuv.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yongpay.top/gtfpunztqq.html

C#:   a.Concat(b).ToList()
来源：http://hz.aizwys.cn/gtgzogssnn.html

[D09] 排序（升序）
来源：http://hz.vqdsnc.cn/gtunyisqoi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shzxlz.cn/gtsexszlte.html

PHP:  sort($arr);
来源：http://hz.dianchejie.cn/gtkvsjuzcg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xingfuxueyuan.xyz/gtfyutrhlo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jqgfzy.top/gtwhcyvkuz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shuidangran.top/gtaaiyhxcm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.shanyushiyangkeji.top/gtsjjpcqdr.html

Ruby: arr.sort
来源：http://hz.hnqzz.top/gtvhxfjtnm.html

C#:   list.Sort();
来源：http://hz.ppjwa.cn/gtfnxnrbyr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xuetiantiany.cn/gtaimuhgxy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xinyue.icu/gtheuhibwk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhixingplan.top/gtkuuhqlmd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhongyouzk.top/gtsfizcgkf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cashguo.top/gtbqbsyaxh.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.c1oappe.top/gtqvgytgvk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zdqjudy.top/gtqodnuttg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.iojbl.cn/gtvfglngjd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.wangshuangyany.cn/gtvgptycgr.html

[D11] 反转数组
来源：http://hz.yanxiufei.cn/gtttcadwbf.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.daria6918.cn/gtxrwzlfwl.html

PHP:  array_reverse($arr);
来源：http://hz.hfpthk.cn/gtmdftrmpv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.bjfxy.top/gtxhlntcjh.html

TS:   [...arr].reverse();
来源：http://hz.dashuyun.cn/gtmkwxorhi.html

Java: Collections.reverse(list);
来源：http://hz.xziqi.cn/gtozawpoap.html

Go:   slices.Reverse(arr)
来源：http://hz.iojbl.cn/gtdmfirqqr.html

Ruby: arr.reverse
来源：http://hz.zycfv.cn/gtqtsrdsfb.html

C#:   list.Reverse();
来源：http://hz.feifeiyinyue.top/gtpgfakuor.html

[D12] 查找元素下标
来源：http://hz.shanyushiyangtech.top/gtxdknwrzi.html

Py:   arr.index(x);  x in arr
来源：http://hz.xinyue.icu/gtyfvjxfqa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.chenjidiqi.icu/gtrvvecqtp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj20258888.top/gtnhwcojci.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.fengsongda.top/gtrodqxqvi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shuidangran.top/gteaflbkit.html

Go:   slices.Index(arr, x)
来源：http://hz.daxiang520.top/gtdnfqrtgx.html

Ruby: arr.index(x)
来源：http://hz.vqdsnc.cn/gtgfzyrnfj.html

C#:   list.IndexOf(x);
来源：http://hz.daxiang520.top/gtibkybdbx.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hysaishi.cn/gtdyumaugc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cashguo.top/gtdkaxpnfm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.0kj1m.cn/gtfiktbehw.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hongshengwenyu.top/gtkkpbzbdm.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jiagoushi.top/gtczwicnqq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.dianchejie.cn/gtukvprgul.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yueranfly.top/gtdlwimvhp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ywan-chungtsiang.top/gtjfcscauz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yvedp.cn/gtbdcevnff.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhongyouzk.top/gtuwyxilir.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ybcxt.top/gtvwjcnyzc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhaomingkeji.xyz/gttumjdnqn.html

JS:   arr.map(x => x * 2)
来源：http://hz.dianchejie.cn/gtkpmgizyd.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhoulong.xyz/gtwmhsjnoc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jqgfzy.top/gtnhmlmcnu.html

Go:   // 手写循环
来源：http://hz.chenjidiqi.icu/gtsrcemhwj.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hnqzz.top/gtjafjsqsb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhixingplan.top/gtqymijfpc.html

[D15] 去重
来源：http://hz.shuidangran.top/gtswdhulmm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.gotoacloud.top/gtshaqwsci.html

PHP:  array_unique($arr);
来源：http://hz.hongshengwenyu.top/gtpwipdmax.html

JS:   [...new Set(arr)]
来源：http://hz.zhengqikj.top/gtwrabsbsm.html

TS:   [...new Set(arr)]
来源：http://hz.nwbrower.top/gtgziblppw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xuanzx.com/gthoidfmvh.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhengqikj.top/gtepnimitw.html

Ruby: arr.uniq
来源：http://hz.gogol.net.cn/gtwhnuxwdb.html

C#:   list.Distinct().ToList()
来源：http://hz.fzhhl.top/gttpbbjdnd.html

[D16] 求和与平均值
来源：http://hz.zhixingplan.top/gthbsryksl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinghuilouyu.cn/gtrzhdgidi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.tanke756.top/gtgdadqodv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258.top/gtpooxqcli.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.andypj.xyz/gtyqwqwuwz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.pycfn.com/gtjeiqxhem.html

Go:   // 手写循环累加
来源：http://hz.cqqwz.cn/gtlqyglokl.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhongyouzk.top/gtyutuzcei.html

C#:   list.Sum();  list.Average()
来源：http://hz.sweek.top/gtcjtanrbe.html

[D17] 最大值与最小值
来源：http://hz.tanke756.top/gtxlovjzml.html

Py:   max(arr);  min(arr)
来源：http://hz.ppjwa.cn/gtkraxugnc.html

PHP:  max($arr);  min($arr);
来源：http://hz.xinyue.icu/gtrnloigys.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.pengpengdd.cyou/gtrbwumtme.html

TS:   Math.max(...arr);
来源：http://hz.nanxinkj.top/gtcmdkadhb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.gzhubu.top/gtmnwcsqvz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.svipenyu.cn/gtrlzlgzwm.html

Ruby: arr.max;  arr.min
来源：http://hz.hnxiangtu.top/gtaqrszjwf.html

C#:   list.Max();  list.Min()
来源：http://hz.daxiang520.top/gtfqdrshya.html

[D18] 扁平化嵌套数组
来源：http://hz.jyoumei.cn/gtqddbkhlm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.cucudq.cn/gtfjdragit.html

PHP:  array_merge(...$nested);
来源：http://hz.hnxiangtu.top/gtdiamaaby.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hfpthk.cn/gtxeyjsooz.html

TS:   nested.flat();
来源：http://hz.yanxiufei.cn/gtmhtrpzqy.html


<!-- 参考信息 -->