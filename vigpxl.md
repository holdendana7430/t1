代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.gzhubu.top/gtijcracgs.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.havefunace.top/gtjqbaurac.html

Ruby: def add(a, b); a + b; end
来源：http://hz.nanxuanxn.top/gtysvxomar.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.yongpay.top/gtgrcfnhsf.html

[C02] 默认参数
来源：http://hz.daria6918.cn/gtiwdrkqxi.html

Py:   def greet(name="World"): return name
来源：http://hz.shangyingyoupin.top/gtpfrxeqcs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.wangshuangyany.cn/gtfvzbmojj.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.zhiwuduotai.top/gtzeceedjq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.yanxiufei.cn/gtdjapcaiq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.ydzc1.top/gtvnmwnbwt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.c1oappe.top/gtifzwcykj.html

Ruby: def greet(name = "World") = name
来源：http://hz.jiagoushi.top/gtjdamejky.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.hywenlv.cn/gtwosqfabk.html

[C03] 可变参数
来源：http://hz.xuanzx.com/gttsenwzgq.html

Py:   def total(*args): return sum(args)
来源：http://hz.nwbrower.top/gthkqbegjz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jqgufenzy.top/gtayndzcjs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.yvedp.cn/gtfaitfopq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.aizwys.cn/gtyptlaxyr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.hfpthk.cn/gtdpejegyg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.shanyushiyangtech.top/gtetttzzii.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.c1oappe.top/gtvtpfmhfj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.zycfv.cn/gtdzxruiaj.html

[C04] 命名参数 / 关键字参数
来源：http://hz.dianchejie.cn/gtpqeyojpc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.iojbl.cn/gtfhhbkfjv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.cqqwz.cn/gtuyzsbtzj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.jyoumei.cn/gtyoymroob.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.jinghuilouyu.cn/gtbwlyoucy.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.snrcjt.cn/gtmwnnebui.html

Go:   // 无：用配置结构体参数
来源：http://hz.jqgufenzy.top/gtfagyerkp.html

Ruby: f(a: 1, b: 2)
来源：http://hz.zhengqikj.top/gtnoqzrsac.html

C#:   f(a: 1, b: 2)
来源：http://hz.shangyingyoupin.top/gttcbclzix.html

[C05] 返回多个值
来源：http://hz.feifeiyinyue.top/gtqiihhoxe.html

Py:   return a, b
来源：http://hz.quarkkingdee.top/gtnvvwlivi.html

PHP:  return [$a, $b];
来源：http://hz.bjfxy.top/gtqcihqjrl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.xinyue.icu/gtvsivsjcr.html

TS:   return { a, b };
来源：http://hz.hfpthk.cn/gtsveqnkkk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.zhijiandao.cn/gtazhtjbbb.html

Go:   return a, b
来源：http://hz.shzxlz.cn/gtnlouicob.html

Ruby: return a, b
来源：http://hz.yonumen.top/gtgwsrlzrs.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.hfpthk.cn/gtbhwwtrio.html

[C06] 匿名函数 / lambda
来源：http://hz.nwbrower.top/gtetvdkiwd.html

Py:   square = lambda x: x * x
来源：http://hz.zdqjudy.top/gtpwtpszcc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.316326.xyz/gtqqavgevz.html

JS:   const square = x => x * x;
来源：http://hz.jinqigufen.top/gtkiviarex.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.zhiwuduotai.top/gtcygzvdev.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.pycfn.com/gttcivrnhk.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.snrcjt.cn/gtfdbuvhrd.html

Ruby: square = ->(x) { x * x }
来源：http://hz.0kj1m.cn/gtodctulzs.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhixingplan.top/gtzeagpvne.html

[C07] 把函数作为参数传入
来源：http://hz.sxryk.cn/gtrobjymsn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.hammf.cn/gtlsvuzgab.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jinqigufen.top/gtyvurzgoh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.ydzc1.top/gtxwiyeiki.html

TS:   arr.map(String)
来源：http://hz.havefunace.top/gtworajlrb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.birdmap.top/gtobvuqepm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.haohaochexian.top/gthrxbycsc.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhaomingkeji.xyz/gtpopinwvp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.feifeiyinyue.top/gtpbuindmt.html

[C08] 闭包
来源：http://hz.xuanzx.com/gtbukkdbvn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.ydzc1.top/gtruuccndq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.shzxlz.cn/gtsyusnbrf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.guowangkeji.top/gtklekaois.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.cucudq.cn/gtubkadojg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.chenjidiqi.icu/gtgeiranvu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.chenzaomai.com/gtktcpvwts.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.daxiang520.top/gtuyhvjupg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.gotoacloud.top/gtjjzgfeje.html

[C09] 递归
来源：http://hz.daria6918.cn/gtwdbunrmu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.jqgufenzy.top/gtccgrectl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yanxiufei.cn/gtyytubfwb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jianghu66.top/gtyjmynbhb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.sxryk.cn/gtzwqitqie.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xinyue.icu/gtvjzuzndt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.tanke756.top/gtrzpgripc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.yj202588.top/gtxfzetavb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.smart0.xyz/gtrqhmgrrt.html

[C10] 变量作用域
来源：http://hz.ydzc1.top/gthxyuuimp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.guannengcc.top/gtcznihycp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hnqzz.top/gtqmxrjjvs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shangyingyoupin.top/gtmjojlzuo.html

TS:   同 JS
来源：http://hz.zhiwuduotai.top/gtfegdygrb.html

Java: 方法内为块级作用域
来源：http://hz.xuanzx.com/gtshyzoppl.html

Go:   花括号块级作用域
来源：http://hz.pengpengdd.cyou/gtnngjilzz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xuetiantiany.cn/gtozcnknfv.html

C#:   块级作用域
来源：http://hz.redwolf501.top/gtpsgblcsy.html

[C11] 模块导入与导出
来源：http://hz.chenjidiqi.icu/gtdfvdpxaz.html

Py:   from module import func
来源：http://hz.ehwqpu.com/gtdvtmroaz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.tianlin.xyz/gtmjcuhnmy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.tianlin.xyz/gthpwjbmdd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.sufxvd.cn/gtqaxmqiuo.html

Java: import java.util.List;
来源：http://hz.chenjidiqi.icu/gtoznpdgtk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zycfv.cn/gtvwvspggp.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhijiandao.cn/gttilxhbgs.html

C#:   using System.Text;
来源：http://hz.jlsjyb.cn/gtqrpotpsr.html

[C12] 立即执行函数 IIFE
来源：http://hz.tanke756.top/gtrgnchfzh.html

Py:   (lambda: print("run"))()
来源：http://hz.ydzc1.top/gthrebqosk.html

PHP:  (function () { echo "run"; })();
来源：http://hz.52xcode.cn/gtslaeydlj.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ppjwa.cn/gtlsuuufli.html

TS:   (() => { console.log("run"); })();
来源：http://hz.fzhhl.top/gtoovpliaq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.xinyue.icu/gtngsdzgdr.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jinqigufen.top/gtqtenygri.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhiwuduotai.top/gthtsugtcu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.sxryk.cn/gtrtcxgxye.html

[C13] 类型声明 / 类型注解
来源：http://hz.zdqjudy.top/gtoleauuca.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.meibo888.top/gtlwtsmlpx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.cucudq.cn/gtyvgbwetu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.tian-w.cn/gtabkmnabj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.sxryk.cn/gtwgpnttnh.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.chenzaomai.com/gtcvxybeso.html

Go:   func add(a, b int) int
来源：http://hz.0kj1m.cn/gtxhkjrkkm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.c1oappe.top/gtrskeacud.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hywenlv.cn/gtszxwykka.html

[C14] 泛型函数
来源：http://hz.sweek.top/gthtqcoswf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.quarkkingdee.top/gtzuzhcjgn.html

PHP:  // 无泛型
来源：http://hz.cheryme.top/gtatnjrdjm.html

JS:   // 无泛型
来源：http://hz.quarkkingdee.top/gtrpieccff.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.jinqigfzy.top/gtlxdjeovh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xziqi.cn/gtxfiduxoc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.zhongyouzk.top/gtodzsiuad.html

Ruby: # 无泛型
来源：http://hz.jinqigufen.top/gtyagegjie.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.shangyingyoupin.top/gtelmeemey.html

[C15] 解构 / 展开参数
来源：http://hz.mhx1999.top/gtdgwehpry.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.quarkkingdee.top/gtwecpmgku.html

PHP:  [$a, $b] = $pair;
来源：http://hz.ehwqpu.com/gtwjnpvdsv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.fengsongda.top/gtxuqcrisj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xingfuxueyuan.xyz/gthqmqjwqg.html

Java: // 无解构
来源：http://hz.yvedp.cn/gtsnxwepsa.html

Go:   // 无解构
来源：http://hz.hnqzz.top/gtfwoirltx.html

Ruby: a, b = pair
来源：http://hz.guowangkeji.top/gtqtjkylut.html

C#:   var (a, b) = pair;
来源：http://hz.hywenlv.cn/gtguwkotcd.html

[C16] 函数 / 方法重载
来源：http://hz.cdnleiting.top/gtstbjxfqd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.fzhhl.top/gtdmqemqdp.html

PHP:  // 无重载
来源：http://hz.zhaomingkeji.xyz/gtckyzfhjb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.gogol.net.cn/gtxunqzoao.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ybcxt.top/gtofkxcklg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xziqi.cn/gtguhumthi.html

Go:   // 无重载：用不同函数名
来源：http://hz.hfpthk.cn/gtmqetuhlg.html

Ruby: # 无重载：靠动态参数
来源：http://hz.jinghuilouyu.cn/gtkkodyxrg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.vqdsnc.cn/gteivqnzam.html

================================================================================
来源：http://hz.52xcode.cn/gtbptqqabs.html

D. 数组 / 列表 / 集合
来源：http://hz.ppjwa.cn/gtzqgaftuq.html

================================================================================
来源：http://hz.jinqigufen.top/gthppkqzug.html

[D01] 创建数组 / 列表
来源：http://hz.hammf.cn/gtjgcttnot.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.0kj1m.cn/gthefahuue.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.tianlin.xyz/gtzreswrhn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yangfankeji.com/gtfslgcspq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.guowangkeji.top/gtudcfrxyk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.hammf.cn/gtzuwelwwy.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.hfpthk.cn/gtxnxejgqs.html

Ruby: arr = [1, 2, 3]
来源：http://hz.xylfe.cn/gtueqysbwc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xuanzx.com/gtthtyzwat.html

[D02] 追加元素到末尾
来源：http://hz.jyoumei.cn/gtdxysdimc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yuxming.cn/gtxwzsaawm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.dianchejie.cn/gtxtimivhh.html

JS:   arr.push(4);
来源：http://hz.mhx1999.top/gtjeftolkg.html

TS:   arr.push(4);
来源：http://hz.zdqjudy.top/gtvxzcaruz.html

Java: list.add(4);
来源：http://hz.shanyushiyangtech.top/gttpwlpesw.html

Go:   arr = append(arr, 4)
来源：http://hz.ybcxt.top/gthunwjqgz.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.snrcjt.cn/gtcaldjllk.html

C#:   list.Add(4);
来源：http://hz.jianghu66.top/gtrrlceroc.html

[D03] 在指定位置插入元素
来源：http://hz.yj20258888.top/gtbskmropk.html

Py:   arr.insert(0, 0)
来源：http://hz.zhijiandao.cn/gtjxjhkbij.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.guowangkeji.top/gtgqbdgywn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.kuanghao11.cn/gtxuayktiz.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jinghuilouyu.cn/gtzxdpiyrr.html

Java: list.add(0, 0);
来源：http://hz.fengsongda.top/gtpusazyzk.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jqgfzy.top/gtthjlzmta.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.guannengcc.top/gteefuscqi.html

C#:   list.Insert(0, 0);
来源：http://hz.zhiwuduotai.top/gtxurzffff.html

[D04] 删除元素
来源：http://hz.jinghuilouyu.cn/gtnjgdqarc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.shangyingyoupin.top/gtnalnlkwi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.52xcode.cn/gtysgytbri.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jlsjyb.cn/gthfjkmbwv.html

TS:   arr.splice(0, 1);
来源：http://hz.cucudq.cn/gtychmjrrq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.52xcode.cn/gtbtwepkdk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhaomingkeji.xyz/gtndjkbpmb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhixingplan.top/gtejxjkuaq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.redwolf501.top/gtmwgsdffy.html

[D05] 访问与修改元素
来源：http://hz.yuanzhike.top/gtwnmbfdcr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hysaishi.cn/gtsnekledi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ydzc1.top/gtqeyjthhj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jinqigufen.top/gtoxoyeojt.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hammf.cn/gtpeifjyhs.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yangfankeji.com/gtlqxzyndz.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.yongpay.top/gttcwwzgho.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gotoacloud.top/gtlhltbrpo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.shanyushiyangtech.top/gtglguefbs.html

[D06] 数组长度
来源：http://hz.pengpengdd.cyou/gtwulinkwn.html

Py:   len(arr)
来源：http://hz.hywenlv.cn/gthhgffepx.html

PHP:  count($arr);
来源：http://hz.tanke756.top/gtxibxmlrp.html

JS:   arr.length
来源：http://hz.shanyushiyangtech.top/gtxblahqeo.html

TS:   arr.length
来源：http://hz.wangshuangyany.cn/gtapmzoiyd.html

Java: list.size();
来源：http://hz.yuanzhike.top/gtwxmcjraw.html

Go:   len(arr)
来源：http://hz.zhijiandao.cn/gtlnurdggw.html

Ruby: arr.length; arr.size
来源：http://hz.shzxlz.cn/gtwdogntms.html

C#:   list.Count;
来源：http://hz.gogol.net.cn/gtijzsninf.html

[D07] 切片 / 取子数组
来源：http://hz.sxryk.cn/gtsxfyqvdy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.sufxvd.cn/gtchoqnnwt.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.nwbrower.top/gtljseotwo.html

JS:   arr.slice(1, 4);
来源：http://hz.9152youxi.cn/gtktbzkryt.html

TS:   arr.slice(1, 4);
来源：http://hz.sufxvd.cn/gtpaoqvmyh.html

Java: list.subList(1, 4);
来源：http://hz.jqgufenzy.top/gtpnrpcgxo.html

Go:   arr[1:4]
来源：http://hz.tanke756.top/gtcpeabqtl.html

Ruby: arr[1, 3]
来源：http://hz.sxryk.cn/gttbwnmcaq.html

C#:   list.GetRange(1, 3);
来源：http://hz.cashguo.top/gtjbfjfroh.html

[D08] 合并两个数组
来源：http://hz.yanxiufei.cn/gttgytrlyo.html

Py:   a + b;  a.extend(b)
来源：http://hz.svipenyu.cn/gtnzniiwng.html

PHP:  array_merge($a, $b);
来源：http://hz.hongshengwenyu.top/gtpixcvctj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.daxiang520.top/gtyumpenou.html

TS:   [...a, ...b];
来源：http://hz.dashuyun.cn/gtyxvwpsmp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cdnleiting.top/gtnrvikztq.html

Go:   append(a, b...)
来源：http://hz.aizwys.cn/gtlmaunpsv.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jinqigufen.top/gthypqqvys.html

C#:   a.Concat(b).ToList()
来源：http://hz.ehwqpu.com/gttaumukpj.html

[D09] 排序（升序）
来源：http://hz.smart0.xyz/gtmfazmsca.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xuanzx.com/gtcklzcbwx.html

PHP:  sort($arr);
来源：http://hz.svipenyu.cn/gtczxragpo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.sysykeji.top/gtuksodbqv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yueranfly.top/gtsseyqwgs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhengqikj.top/gtjtoxaesz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.shanyushiyangkeji.top/gtmarankyo.html

Ruby: arr.sort
来源：http://hz.sxryk.cn/gtaegnmpuc.html

C#:   list.Sort();
来源：http://hz.daria6918.cn/gttfjimfal.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.sufxvd.cn/gtinffzsfo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.chenlongwang.top/gtiaqklroq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.smart0.xyz/gtnwalyaza.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.guowangkeji.top/gteiharpxv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.aibaodan.cn/gteengnrsv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.fengsongda.top/gtyiffeszv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.316326.xyz/gtotlxwutt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yvedp.cn/gtraobzfym.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.kuanghao11.cn/gtpwtgtvzh.html

[D11] 反转数组
来源：http://hz.sufxvd.cn/gttnfcxszn.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cqqwz.cn/gtyngybwxn.html

PHP:  array_reverse($arr);
来源：http://hz.cashguo.top/gtcngwksns.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jinqigufen.top/gtrnbkvcmn.html

TS:   [...arr].reverse();
来源：http://hz.jqgfzy.top/gtmgoybgyt.html

Java: Collections.reverse(list);
来源：http://hz.wangshuangyany.cn/gtuvqanrfg.html

Go:   slices.Reverse(arr)
来源：http://hz.zhoulong.xyz/gtmvmiuleu.html

Ruby: arr.reverse
来源：http://hz.jyoumei.cn/gtmtulasaa.html

C#:   list.Reverse();
来源：http://hz.bjfxy.top/gtbwjhvcsr.html

[D12] 查找元素下标
来源：http://hz.sxryk.cn/gthkyifzdt.html

Py:   arr.index(x);  x in arr
来源：http://hz.tianlin.xyz/gtpdquvpej.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhaomingkeji.xyz/gtepryoyxu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.aizwys.cn/gtvhmrtxul.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ehwqpu.com/gtddlbpqfo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.wangshuangyany.cn/gtufkocwlf.html

Go:   slices.Index(arr, x)
来源：http://hz.nanxinkj.top/gtjpcwpwxx.html

Ruby: arr.index(x)
来源：http://hz.yonumen.top/gtqypijols.html

C#:   list.IndexOf(x);
来源：http://hz.guannengcc.top/gtdhluxgwm.html

[D13] 过滤（保留满足条件的）
来源：http://hz.c1oappe.top/gtlqwwvwis.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.birdmap.top/gtanaczqau.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.nwbrower.top/gtkfxzfuqi.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yj20258888.top/gtvyrlxbfl.html

TS:   arr.filter(x => x > 3)
来源：http://hz.mhx1999.top/gtrmtwbuxm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.cashguo.top/gtmptdbyft.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xinyue.icu/gtltpbbuwe.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ywan-chungtsiang.top/gtgfvlbjxd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.c1oappe.top/gtsidespfm.html

[D14] 映射转换（每个元素变形）
来源：http://hz.redwolf501.top/gtmpkzxfzo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.hywenlv.cn/gtqywgrjdz.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.fzhhl.top/gtknlbttoj.html

JS:   arr.map(x => x * 2)
来源：http://hz.hysaishi.cn/gtxnwbyoal.html

TS:   arr.map(x => x * 2)
来源：http://hz.cheryme.top/gtoptnwqad.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.hysaishi.cn/gtxblsdiqh.html

Go:   // 手写循环
来源：http://hz.chenzaomai.com/gtsckjlvhm.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yangfankeji.com/gtgrsqhclz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yuanzhike.top/gtdrxjqyik.html

[D15] 去重
来源：http://hz.gaohongyu789.top/gtlmzboypr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yangfankeji.com/gtocjsamrg.html

PHP:  array_unique($arr);
来源：http://hz.jyoumei.cn/gtrvoojezu.html

JS:   [...new Set(arr)]
来源：http://hz.svipenyu.cn/gtoiegbwrw.html

TS:   [...new Set(arr)]
来源：http://hz.jqgfzy.top/gtihspfxzs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jqgfzy.top/gtmfokijac.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.nwbrower.top/gtntxuaxjz.html

Ruby: arr.uniq
来源：http://hz.fengsongda.top/gtfpleqmhb.html

C#:   list.Distinct().ToList()
来源：http://hz.fengsongda.top/gtdvkowylt.html

[D16] 求和与平均值
来源：http://hz.feifeiyinyue.top/gtpfzutcty.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinqigufen.top/gtssmwyrhb.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.chenjidiqi.icu/gtuwxchjds.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hywenlv.cn/gtvwdffnwa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.feifeiyinyue.top/gtvvmroupr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xinyue.icu/gtbjmgsspn.html

Go:   // 手写循环累加
来源：http://hz.vqdsnc.cn/gtgprxtvka.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhijiandao.cn/gtncimebka.html

C#:   list.Sum();  list.Average()
来源：http://hz.hongshengwenyu.top/gtkgrheenh.html

[D17] 最大值与最小值
来源：http://hz.daria6918.cn/gtacskcfro.html

Py:   max(arr);  min(arr)
来源：http://hz.sysykeji.top/gtnberfmjr.html

PHP:  max($arr);  min($arr);
来源：http://hz.xuetiantiany.cn/gtuytndntt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hfpthk.cn/gtlxpbvnap.html

TS:   Math.max(...arr);
来源：http://hz.dashuyun.cn/gtauwogate.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.dashuyun.cn/gtedgjscpo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.guowangkeji.top/gtrlhvwyvv.html

Ruby: arr.max;  arr.min
来源：http://hz.xinyue.icu/gtyurfbysb.html

C#:   list.Max();  list.Min()
来源：http://hz.jqgufenzy.top/gtwubhymlg.html

[D18] 扁平化嵌套数组
来源：http://hz.zhongyouzk.top/gtjuvqktms.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.shanyushiyangtech.top/gteavwsphd.html

PHP:  array_merge(...$nested);
来源：http://hz.xuetiantiany.cn/gtkspebwiq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.nanxinkj.top/gtjkxhlhxs.html

TS:   nested.flat();
来源：http://hz.fengsongda.top/gthrthiitq.html


<!-- 参考信息 -->