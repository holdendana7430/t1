代发 wailian999

Py:   def add(a, b): return a + b
来源：http://hz.cqqwz.cn/gtlvkhzzre.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.shanyushiyangtech.top/gtxqwxzlan.html

JS:   function add(a, b) { return a + b; }
来源：http://hz.ybcxt.top/gtilyctkmx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.jinyuanbaomall.cn/gtcpuitpdi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://hz.fzhhl.top/gtiiaadruw.html

Go:   func add(a, b int) int { return a + b }
来源：http://hz.nanxinkj.top/gtxjxedbjg.html

Ruby: def add(a, b); a + b; end
来源：http://hz.zhijiandao.cn/gtjbkvcoab.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://hz.wangdashe.top/gtbnbvzqhj.html

[C02] 默认参数
来源：http://hz.yuanzhike.top/gtzlcsqbxr.html

Py:   def greet(name="World"): return name
来源：http://hz.ywan-chungtsiang.top/gtttqkxtxl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://hz.zhiwuduotai.top/gtxjphjhkq.html

JS:   function greet(name = "World") { return name; }
来源：http://hz.ybcxt.top/gtoftkkayw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.zhaomingkeji.xyz/gtgustbtaz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.yongpay.top/gtaaueqiyr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.dashuyun.cn/gtpapojzgy.html

Ruby: def greet(name = "World") = name
来源：http://hz.jinqigufen.top/gtlqfxzuxe.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.pengpengdd.cyou/gtqqahramg.html

[C03] 可变参数
来源：http://hz.chenjidiqi.icu/gtyskcvpbc.html

Py:   def total(*args): return sum(args)
来源：http://hz.mhx1999.top/gtjrasenqp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.ivvv.top/gtiiuvmcgw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.sufxvd.cn/gtgdbyhzkh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.jinghuilouyu.cn/gttkjfopwh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.snrcjt.cn/gtpzhopuhr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.xingfuxueyuan.xyz/gtmkbjsehc.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.shanyushiyangtech.top/gtqozvseai.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.tanke756.top/gteoutjctk.html

[C04] 命名参数 / 关键字参数
来源：http://hz.hnxiangtu.top/gtyhwtgrxu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.ybcxt.top/gtjvcyfyib.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yj20258888.top/gthtkrcuzn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hfpthk.cn/gtcmajrmjd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.kuanghao11.cn/gtfsjlfqfl.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.hnxiangtu.top/gtiqbtbncd.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhongyouzk.top/gtrmldjtxv.html

Ruby: f(a: 1, b: 2)
来源：http://hz.havefunace.top/gtykzqxokw.html

C#:   f(a: 1, b: 2)
来源：http://hz.hywenlv.cn/gtethctkqw.html

[C05] 返回多个值
来源：http://hz.xingfuxueyuan.xyz/gtpqmskleu.html

Py:   return a, b
来源：http://hz.jyoumei.cn/gtmibyrxsj.html

PHP:  return [$a, $b];
来源：http://hz.jinyuanbaomall.cn/gtmpmngufr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.9152youxi.cn/gtfocvhekf.html

TS:   return { a, b };
来源：http://hz.shzxlz.cn/gtbjgoakrw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.birdmap.top/gtsidudnla.html

Go:   return a, b
来源：http://hz.haohaochexian.top/gtjeqecxyz.html

Ruby: return a, b
来源：http://hz.xuetiantiany.cn/gtktmggyij.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.gotoacloud.top/gtdzmehkcv.html

[C06] 匿名函数 / lambda
来源：http://hz.gzhubu.top/gtsngzxzqw.html

Py:   square = lambda x: x * x
来源：http://hz.yj20258888.top/gtcqairmdn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.yonumen.top/gtmfrzmyao.html

JS:   const square = x => x * x;
来源：http://hz.pycfn.com/gtrrxbfjxp.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.cdnleiting.top/gtcxdjchxj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.shanyushiyangtech.top/gttpbwsopb.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.ppjwa.cn/gtgwhtipbw.html

Ruby: square = ->(x) { x * x }
来源：http://hz.sxryk.cn/gtxryancpl.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.pycfn.com/gtavxkqqro.html

[C07] 把函数作为参数传入
来源：http://hz.daxiang520.top/gtqstrduuv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.xuanzx.com/gtfjfbodub.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.zhongyouzk.top/gtpjyjqzas.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.haohaochexian.top/gtwrotylig.html

TS:   arr.map(String)
来源：http://hz.chenlongwang.top/gtlewhzzjl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yvedp.cn/gtyrgcrgsv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.shanyushiyangkeji.top/gtsfairjlh.html

Ruby: arr.map(&:upcase)
来源：http://hz.jinghuilouyu.cn/gthpdumlee.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yj202588.top/gtthdojkys.html

[C08] 闭包
来源：http://hz.tianlin.xyz/gtutavwvgw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hfpthk.cn/gttbyiplrf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.quarkkingdee.top/gtttgdsjpz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.52xcode.cn/gtxrkpkqoj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.tanke756.top/gtmjueziio.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ywan-chungtsiang.top/gtloviujrr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.sxryk.cn/gtduvoglbl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ydjk.org.cn/gtdqxnhagg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.dashuyun.cn/gtruuhloup.html

[C09] 递归
来源：http://hz.hnxiangtu.top/gtwnprraas.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.wangshuangyany.cn/gtpnxfurnm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ehwqpu.com/gtchanvdnz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hammf.cn/gtebdbeimf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.pengpengdd.cyou/gtrnkbjoph.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.yuxming.cn/gtkavmkjhi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.shuidangran.top/gtytxvjadm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.shangyingyoupin.top/gtolfqklyp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.316326.xyz/gtxyxcujtl.html

[C10] 变量作用域
来源：http://hz.hnxiangtu.top/gtipscfsru.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.pengpengdd.cyou/gtlgbnirah.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.guowangkeji.top/gtfeyrvbgv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.sufxvd.cn/gtrhyvoqqp.html

TS:   同 JS
来源：http://hz.vqdsnc.cn/gtijumbomt.html

Java: 方法内为块级作用域
来源：http://hz.jlsjyb.cn/gtkfcvtoac.html

Go:   花括号块级作用域
来源：http://hz.shangyingyoupin.top/gtpomxawsa.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.snrcjt.cn/gtakvtysru.html

C#:   块级作用域
来源：http://hz.jqgufenzy.top/gtiuvvrckn.html

[C11] 模块导入与导出
来源：http://hz.jyoumei.cn/gtawzxtmlf.html

Py:   from module import func
来源：http://hz.52xcode.cn/gttlyhjyfi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hammf.cn/gtondgmebe.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.jqgfzy.top/gtyfsjbqdv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hywenlv.cn/gttoobnwjx.html

Java: import java.util.List;
来源：http://hz.guowangkeji.top/gtrlxnqnlu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinqigfzy.top/gtfqoiwrki.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhixingplan.top/gtiyvajjbp.html

C#:   using System.Text;
来源：http://hz.zhaomingkeji.xyz/gtrdoscpej.html

[C12] 立即执行函数 IIFE
来源：http://hz.316326.xyz/gtboevslpk.html

Py:   (lambda: print("run"))()
来源：http://hz.xylfe.cn/gtezdtgack.html

PHP:  (function () { echo "run"; })();
来源：http://hz.c1oappe.top/gtufsgtsux.html

JS:   (() => { console.log("run"); })();
来源：http://hz.guowangkeji.top/gtfpywskwd.html

TS:   (() => { console.log("run"); })();
来源：http://hz.xylfe.cn/gticuwjaoq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.nanxuanxn.top/gtbjvcqbvr.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.chenlongwang.top/gtkbuuogfb.html

Ruby: -> { puts "run" }.call
来源：http://hz.guannengcc.top/gtitwtsdkn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.mhx1999.top/gtukljaise.html

[C13] 类型声明 / 类型注解
来源：http://hz.ppjwa.cn/gtzmhruwra.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jinqigufen.top/gtndyatplw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.0kj1m.cn/gtxllsfoue.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yuxming.cn/gtreatpocy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhixingplan.top/gtzmrbikmq.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.gotoacloud.top/gtnbioxpdb.html

Go:   func add(a, b int) int
来源：http://hz.haohaochexian.top/gtvthlhuyw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jqgufenzy.top/gtiglifbqp.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.shanyushiyangkeji.top/gtwuvakmko.html

[C14] 泛型函数
来源：http://hz.nanxinkj.top/gtqccrgmvv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.mhx1999.top/gtykafknuv.html

PHP:  // 无泛型
来源：http://hz.aibaodan.cn/gtijkpxxja.html

JS:   // 无泛型
来源：http://hz.redwolf501.top/gtzuezzltd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.mhx1999.top/gtmxbmnkso.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jinghuilouyu.cn/gtvwhbetzc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ivvv.top/gtbikxpcns.html

Ruby: # 无泛型
来源：http://hz.zhoulong.xyz/gtaaeenavs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zdqjudy.top/gtslcgehji.html

[C15] 解构 / 展开参数
来源：http://hz.redwolf501.top/gtnmnhyjxj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.chenjidiqi.icu/gtbwpfqdsa.html

PHP:  [$a, $b] = $pair;
来源：http://hz.fengsongda.top/gtxuwivlyp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.chenjidiqi.icu/gtfywxtyrc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.nwbrower.top/gtpchxhmtl.html

Java: // 无解构
来源：http://hz.c1oappe.top/gttohbpwrg.html

Go:   // 无解构
来源：http://hz.cheryme.top/gtotsbmway.html

Ruby: a, b = pair
来源：http://hz.tanke756.top/gtqglmvwxi.html

C#:   var (a, b) = pair;
来源：http://hz.shanyushiyangtech.top/gtdkutwopg.html

[C16] 函数 / 方法重载
来源：http://hz.ywan-chungtsiang.top/gtsmkwjlku.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jinqigufen.top/gteyychjoc.html

PHP:  // 无重载
来源：http://hz.hfpthk.cn/gtybfszqax.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.wangdashe.top/gthiyvidhk.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.andypj.xyz/gtrzslyast.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yonumen.top/gtykabrxpn.html

Go:   // 无重载：用不同函数名
来源：http://hz.hnxiangtu.top/gtgjiyxhmh.html

Ruby: # 无重载：靠动态参数
来源：http://hz.wangshuangyany.cn/gtpuvjtrts.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.andypj.xyz/gtdphkjtqx.html

================================================================================
来源：http://hz.xinyue.icu/gtaxxrprvt.html

D. 数组 / 列表 / 集合
来源：http://hz.tian-w.cn/gtuecrlngn.html

================================================================================
来源：http://hz.dianchejie.cn/gtdvjlonwh.html

[D01] 创建数组 / 列表
来源：http://hz.jlsjyb.cn/gtjgcijkfz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yj20258.top/gtfaegwefz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.wangdashe.top/gtahuexnvi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xinyue.icu/gtbdxtrqas.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xziqi.cn/gtfwiwlebw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yuanzhike.top/gtpzevgmuy.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.fengsongda.top/gteddypvze.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yuxming.cn/gtbbvjvdrj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.wangshuangyany.cn/gtinnkryms.html

[D02] 追加元素到末尾
来源：http://hz.svipenyu.cn/gtyavpyybf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.shanyushiyangkeji.top/gtefsitfge.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shuidangran.top/gtfhlslxvr.html

JS:   arr.push(4);
来源：http://hz.wangdashe.top/gtnwlvlqva.html

TS:   arr.push(4);
来源：http://hz.vqdsnc.cn/gtdhbrwftw.html

Java: list.add(4);
来源：http://hz.sxryk.cn/gtawfylbsq.html

Go:   arr = append(arr, 4)
来源：http://hz.tanke756.top/gtzjemxhdu.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xylfe.cn/gtmtgoxtyo.html

C#:   list.Add(4);
来源：http://hz.aibaodan.cn/gtrssfspwl.html

[D03] 在指定位置插入元素
来源：http://hz.gotoacloud.top/gtlkuryobl.html

Py:   arr.insert(0, 0)
来源：http://hz.zhoulong.xyz/gtjzjmpusz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jianghu66.top/gtwpjhdfgw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.hysaishi.cn/gtgdolcipc.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.andypj.xyz/gttgzeopln.html

Java: list.add(0, 0);
来源：http://hz.hammf.cn/gtaogsfyis.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xinyue.icu/gtgfpstjfu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shuidangran.top/gthxsgioov.html

C#:   list.Insert(0, 0);
来源：http://hz.birdmap.top/gtegnftcoz.html

[D04] 删除元素
来源：http://hz.zhiwuduotai.top/gtdjnguibs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hongshengwenyu.top/gtqkxnzfql.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jqgufenzy.top/gtmdohwhyi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.fzhhl.top/gtvwhaoosq.html

TS:   arr.splice(0, 1);
来源：http://hz.havefunace.top/gtgncfuofe.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.dianchejie.cn/gtxaytuofb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.chenlongwang.top/gtutdgwbaq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.kuanghao11.cn/gtimvcwyno.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xingfuxueyuan.xyz/gtzpstharw.html

[D05] 访问与修改元素
来源：http://hz.nanxuanxn.top/gtlksqvvxy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gotoacloud.top/gtwmcrmgza.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.9152youxi.cn/gtihglwllp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.smart0.xyz/gtuhtsgnii.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.gogol.net.cn/gtxwbzaubf.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.snrcjt.cn/gtwqnfjxnm.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.redwolf501.top/gtruhccozr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.andypj.xyz/gtkybblocg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.shzxlz.cn/gtovjmvcgk.html

[D06] 数组长度
来源：http://hz.sxryk.cn/gtsfgtqgsu.html

Py:   len(arr)
来源：http://hz.316326.xyz/gtkcokytrw.html

PHP:  count($arr);
来源：http://hz.hysaishi.cn/gtxorzemap.html

JS:   arr.length
来源：http://hz.hongshengwenyu.top/gtprvloyrq.html

TS:   arr.length
来源：http://hz.jqgfzy.top/gttlexeafp.html

Java: list.size();
来源：http://hz.dashuyun.cn/gtxyhzxdge.html

Go:   len(arr)
来源：http://hz.yonumen.top/gtxunjcmif.html

Ruby: arr.length; arr.size
来源：http://hz.bjfxy.top/gtqcuprdgm.html

C#:   list.Count;
来源：http://hz.bjfxy.top/gtoyyfttfz.html

[D07] 切片 / 取子数组
来源：http://hz.bjfxy.top/gtablozzip.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhiwuduotai.top/gtujrxbrvm.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.tianlin.xyz/gtvqrwzzdq.html

JS:   arr.slice(1, 4);
来源：http://hz.aibaodan.cn/gtxbtetkqk.html

TS:   arr.slice(1, 4);
来源：http://hz.yj20258.top/gtzfhoeqcr.html

Java: list.subList(1, 4);
来源：http://hz.hywenlv.cn/gtxmzfnxhg.html

Go:   arr[1:4]
来源：http://hz.nanxinkj.top/gtnqjzpfpx.html

Ruby: arr[1, 3]
来源：http://hz.ppjwa.cn/gthjkwqrgo.html

C#:   list.GetRange(1, 3);
来源：http://hz.yanxiufei.cn/gtqneqkvvi.html

[D08] 合并两个数组
来源：http://hz.iojbl.cn/gtlxnjaxbu.html

Py:   a + b;  a.extend(b)
来源：http://hz.0kj1m.cn/gtpgriiyii.html

PHP:  array_merge($a, $b);
来源：http://hz.svipenyu.cn/gtkizeinsz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zhiwuduotai.top/gtcblqcdet.html

TS:   [...a, ...b];
来源：http://hz.hongshengwenyu.top/gtrfrtzrnn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.daxiang520.top/gtrqpadiou.html

Go:   append(a, b...)
来源：http://hz.shzxlz.cn/gtgbxrhsso.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hfpthk.cn/gthnvahrwv.html

C#:   a.Concat(b).ToList()
来源：http://hz.yueranfly.top/gtfkrvgvvb.html

[D09] 排序（升序）
来源：http://hz.feifeiyinyue.top/gtscwfendi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.0kj1m.cn/gttiirhvqm.html

PHP:  sort($arr);
来源：http://hz.hongshengwenyu.top/gtfepqvjxa.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ywan-chungtsiang.top/gtrwfxlmpw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.wangdashe.top/gtkldzoqhn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cdnleiting.top/gtbraueltp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.guowangkeji.top/gtmpksirjt.html

Ruby: arr.sort
来源：http://hz.hysaishi.cn/gtmzsuhcrw.html

C#:   list.Sort();
来源：http://hz.xziqi.cn/gtncwoalbf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.andypj.xyz/gtzcnhwfkq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.redwolf501.top/gtcoblqrxg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jyoumei.cn/gtbbazradb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yueranfly.top/gtjmhykmos.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.haohaochexian.top/gtlaqlqdvk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hnqzz.top/gtkwhhffhc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jlsjyb.cn/gttndzxwtd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.sxryk.cn/gtasspqzsr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.shanyushiyangkeji.top/gttpgjbzdq.html

[D11] 反转数组
来源：http://hz.aibaodan.cn/gthhxuthbz.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.iojbl.cn/gtfgwysggc.html

PHP:  array_reverse($arr);
来源：http://hz.316326.xyz/gtpnuqdiww.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.aizwys.cn/gtdfhkdyog.html

TS:   [...arr].reverse();
来源：http://hz.ywan-chungtsiang.top/gtctdtvjmo.html

Java: Collections.reverse(list);
来源：http://hz.dashuyun.cn/gtpttpojdx.html

Go:   slices.Reverse(arr)
来源：http://hz.mhx1999.top/gtdlwvywgh.html

Ruby: arr.reverse
来源：http://hz.xuetiantiany.cn/gtzhvnwvyu.html

C#:   list.Reverse();
来源：http://hz.xuanzx.com/gtkvpprjep.html

[D12] 查找元素下标
来源：http://hz.smart0.xyz/gtfcwgarqh.html

Py:   arr.index(x);  x in arr
来源：http://hz.bjfxy.top/gtykolnzma.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.iojbl.cn/gtfcrzojeg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.wangdashe.top/gtxpgoedpu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hnxiangtu.top/gtxjaegdds.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.52xcode.cn/gtonyjhxrq.html

Go:   slices.Index(arr, x)
来源：http://hz.hammf.cn/gtaeaxzqjc.html

Ruby: arr.index(x)
来源：http://hz.yj202588.top/gtmpnfsfiz.html

C#:   list.IndexOf(x);
来源：http://hz.ehwqpu.com/gtliqkjpuv.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yanxiufei.cn/gtytkwkhoh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.xuetiantiany.cn/gtlfampboo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hywenlv.cn/gtenhtyxeu.html

JS:   arr.filter(x => x > 3)
来源：http://hz.gaohongyu789.top/gtdcalbhgr.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jlsjyb.cn/gtixoxkjja.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shanyushiyangkeji.top/gtcxsgukxo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.shanyushiyangkeji.top/gtdbnrsgyg.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zdqjudy.top/gtercumfdl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.svipenyu.cn/gtqgmlcirc.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jinqigufen.top/gtnrgxavwp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ehwqpu.com/gtiggnzvgp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ehwqpu.com/gteepzluka.html

JS:   arr.map(x => x * 2)
来源：http://hz.yj20258888.top/gtxhhwqeav.html

TS:   arr.map(x => x * 2)
来源：http://hz.zhaomingkeji.xyz/gtujfxxlal.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.iojbl.cn/gtsuenqeit.html

Go:   // 手写循环
来源：http://hz.yangfankeji.com/gtvkufatiu.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.bjfxy.top/gttqeqnisy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.havefunace.top/gtvzfdhdpk.html

[D15] 去重
来源：http://hz.xinyue.icu/gtexacobhf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yvedp.cn/gteeikurkd.html

PHP:  array_unique($arr);
来源：http://hz.52xcode.cn/gtlypjbucn.html

JS:   [...new Set(arr)]
来源：http://hz.vqdsnc.cn/gtkuckvjzr.html

TS:   [...new Set(arr)]
来源：http://hz.0kj1m.cn/gtqsdmnvvz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.sufxvd.cn/gtioobgkvg.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.tian-w.cn/gtkglwipjj.html

Ruby: arr.uniq
来源：http://hz.nwbrower.top/gtoybftcgr.html

C#:   list.Distinct().ToList()
来源：http://hz.sufxvd.cn/gthhyoeioa.html

[D16] 求和与平均值
来源：http://hz.jyoumei.cn/gtutwiggir.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yueranfly.top/gtviudlgez.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.nwbrower.top/gtxejlreyw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj202588.top/gtztdpkove.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.meibo888.top/gttdsqlktq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.aizwys.cn/gtjqqpinau.html

Go:   // 手写循环累加
来源：http://hz.316326.xyz/gtpcqyfcro.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jlsjyb.cn/gtpidhztha.html

C#:   list.Sum();  list.Average()
来源：http://hz.0kj1m.cn/gtcplhkjnq.html

[D17] 最大值与最小值
来源：http://hz.iojbl.cn/gtuhprpaav.html

Py:   max(arr);  min(arr)
来源：http://hz.wangdashe.top/gtyrusgaev.html

PHP:  max($arr);  min($arr);
来源：http://hz.ybcxt.top/gtbpwhzods.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.wangshuangyany.cn/gtsjkajwmk.html

TS:   Math.max(...arr);
来源：http://hz.tanke756.top/gtdlfyeiic.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.nanxinkj.top/gttgecihgi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.chenjidiqi.icu/gtonfuerzt.html

Ruby: arr.max;  arr.min
来源：http://hz.316326.xyz/gtyuuanuez.html

C#:   list.Max();  list.Min()
来源：http://hz.tanke756.top/gtvspcusxa.html

[D18] 扁平化嵌套数组
来源：http://hz.kuanghao11.cn/gtcsdoumyy.html


<!-- 参考信息 -->