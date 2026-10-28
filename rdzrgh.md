代发 wailian999

TS:   function greet(name: string = "World") { return name; }
来源：http://hz.316326.xyz/gtxiondvkv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://hz.guannengcc.top/gtoweotfto.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://hz.yuxming.cn/gtqgsjobbw.html

Ruby: def greet(name = "World") = name
来源：http://hz.fengsongda.top/gtmsazggyj.html

C#:   string Greet(string name = "World") => name;
来源：http://hz.bjfxy.top/gtwkukrgep.html

[C03] 可变参数
来源：http://hz.jinqigufen.top/gtkudmyeke.html

Py:   def total(*args): return sum(args)
来源：http://hz.jinyuanbaomall.cn/gtjstwxxfj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://hz.jinqigufen.top/gtjeqykkmt.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cucudq.cn/gtsknqxnue.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.birdmap.top/gtuwoivuht.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.kuanghao11.cn/gtucfzwjxu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.yonumen.top/gtntmkzcym.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.wangdashe.top/gtsedlakfz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.jqgufenzy.top/gtzalagqkq.html

[C04] 命名参数 / 关键字参数
来源：http://hz.zhiwuduotai.top/gtuabprzqe.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.havefunace.top/gtirjqdjdc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yvedp.cn/gtajueqjpx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.chenlongwang.top/gtcssnzzny.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.gaohongyu789.top/gtrjlpsigu.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.yongpay.top/gtzuzqpnur.html

Go:   // 无：用配置结构体参数
来源：http://hz.zycfv.cn/gtfwpjswxo.html

Ruby: f(a: 1, b: 2)
来源：http://hz.hysaishi.cn/gtcdiusujx.html

C#:   f(a: 1, b: 2)
来源：http://hz.yj20258.top/gthgssfsjx.html

[C05] 返回多个值
来源：http://hz.mhx1999.top/gtbgrdsxsw.html

Py:   return a, b
来源：http://hz.iojbl.cn/gtsqcsdxbn.html

PHP:  return [$a, $b];
来源：http://hz.yueranfly.top/gtvgttdrud.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jiagoushi.top/gtfkzqhesy.html

TS:   return { a, b };
来源：http://hz.gotoacloud.top/gttjlbqwgw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.yongpay.top/gtwakfysgn.html

Go:   return a, b
来源：http://hz.iojbl.cn/gtyhdaxswp.html

Ruby: return a, b
来源：http://hz.shangyingyoupin.top/gtlalsujsn.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhijiandao.cn/gtxcdvxiir.html

[C06] 匿名函数 / lambda
来源：http://hz.zdqjudy.top/gtfedudunf.html

Py:   square = lambda x: x * x
来源：http://hz.hongshengwenyu.top/gtadrwbybr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zycfv.cn/gtkioqrdwr.html

JS:   const square = x => x * x;
来源：http://hz.shanyushiyangtech.top/gtomecsbcl.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.haohaochexian.top/gtyzrfoglw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.yj20258.top/gtypgtzxyg.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yanxiufei.cn/gtymrhroxv.html

Ruby: square = ->(x) { x * x }
来源：http://hz.shanyushiyangkeji.top/gtpgphoiwe.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.fzhhl.top/gtrujqlvkg.html

[C07] 把函数作为参数传入
来源：http://hz.jinghuilouyu.cn/gtiegalgfx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yueranfly.top/gtkcncslpy.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.xuanzx.com/gtxvvwwomd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.aibaodan.cn/gtnmkadekb.html

TS:   arr.map(String)
来源：http://hz.pycfn.com/gtvvwjmykr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.yj20258888.top/gtvnxtjjwk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.guannengcc.top/gtdyazihgw.html

Ruby: arr.map(&:upcase)
来源：http://hz.jyoumei.cn/gtcgfwatab.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.yongpay.top/gtquyngmqy.html

[C08] 闭包
来源：http://hz.kuanghao11.cn/gtbzovnxgx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.cdnleiting.top/gtvaprvzwm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.gogol.net.cn/gtsaysalej.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.fzhhl.top/gtunpumuyt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.wangdashe.top/gtpuflnuuv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.gogol.net.cn/gtmucvsser.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.haohaochexian.top/gtoibnfgyd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.ydjk.org.cn/gtrgomlhsf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.316326.xyz/gtahmotavq.html

[C09] 递归
来源：http://hz.shzxlz.cn/gtoyldyupd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ydzc1.top/gtwgiajzyq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yonumen.top/gtozeipafz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.haohaochexian.top/gtaxmjeryp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.fzhhl.top/gtmkujnraf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.nanxinkj.top/gtogbshyzc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.feifeiyinyue.top/gtyjswaume.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.jlsjyb.cn/gtsrsefyhz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.xinyue.icu/gtgybhanuf.html

[C10] 变量作用域
来源：http://hz.vqdsnc.cn/gtqgmzbmzq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xylfe.cn/gtfaghhtxb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xuanzx.com/gtdjvdxkch.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.jlsjyb.cn/gtvoopjlbw.html

TS:   同 JS
来源：http://hz.mhx1999.top/gtaktafwwv.html

Java: 方法内为块级作用域
来源：http://hz.sxryk.cn/gtokklodmw.html

Go:   花括号块级作用域
来源：http://hz.yuxming.cn/gtryndpwzh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.redwolf501.top/gtydabqnrv.html

C#:   块级作用域
来源：http://hz.ppjwa.cn/gtgqezsfty.html

[C11] 模块导入与导出
来源：http://hz.zhiwuduotai.top/gtcokzqsbo.html

Py:   from module import func
来源：http://hz.dashuyun.cn/gtmjtlrbio.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hnxiangtu.top/gtjzhbbwlf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.xuetiantiany.cn/gtrjjokvnp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ywan-chungtsiang.top/gtxedjozth.html

Java: import java.util.List;
来源：http://hz.ivvv.top/gtwdkmrdpq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinqigfzy.top/gttnlncbkt.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.chenzaomai.com/gtbpwvdcbx.html

C#:   using System.Text;
来源：http://hz.aizwys.cn/gteqtmchnz.html

[C12] 立即执行函数 IIFE
来源：http://hz.havefunace.top/gtsizzwwpy.html

Py:   (lambda: print("run"))()
来源：http://hz.svipenyu.cn/gtkknhrybs.html

PHP:  (function () { echo "run"; })();
来源：http://hz.tian-w.cn/gtoorutoua.html

JS:   (() => { console.log("run"); })();
来源：http://hz.nanxinkj.top/gtecfseqzq.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ydzc1.top/gtopecjzoa.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.fengsongda.top/gtefaoxuid.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zycfv.cn/gtvtnjvspy.html

Ruby: -> { puts "run" }.call
来源：http://hz.gotoacloud.top/gtbprwkzjc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.cheryme.top/gthygwhcny.html

[C13] 类型声明 / 类型注解
来源：http://hz.wangdashe.top/gtndxrtthi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.feifeiyinyue.top/gtkhjxkfoz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sxryk.cn/gtaqvdstum.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.hywenlv.cn/gtvexvwqst.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.haohaochexian.top/gttgpylhma.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cdnleiting.top/gtydhuwgpj.html

Go:   func add(a, b int) int
来源：http://hz.sweek.top/gttyjiidml.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jqgufenzy.top/gtvvqwgtxj.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.yvedp.cn/gtukkdhgpx.html

[C14] 泛型函数
来源：http://hz.zycfv.cn/gttfwsffhe.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.nanxuanxn.top/gtkcopdonn.html

PHP:  // 无泛型
来源：http://hz.gaohongyu789.top/gtpeovqrjm.html

JS:   // 无泛型
来源：http://hz.jqgfzy.top/gtkspcvlfq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.tianlin.xyz/gtokmlprgy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hongshengwenyu.top/gtjluxytol.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ydzc1.top/gtgbctpgjm.html

Ruby: # 无泛型
来源：http://hz.hywenlv.cn/gtslruerec.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.tian-w.cn/gtfoegfkiq.html

[C15] 解构 / 展开参数
来源：http://hz.yanxiufei.cn/gthfubfvjm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.shangyingyoupin.top/gtkjxvrugz.html

PHP:  [$a, $b] = $pair;
来源：http://hz.hfpthk.cn/gtzlfddjbv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.9152youxi.cn/gtoverxdaf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.cheryme.top/gtuurboheb.html

Java: // 无解构
来源：http://hz.feifeiyinyue.top/gthgeiugct.html

Go:   // 无解构
来源：http://hz.0kj1m.cn/gthmsejdaz.html

Ruby: a, b = pair
来源：http://hz.ydzc1.top/gtfkbqcepr.html

C#:   var (a, b) = pair;
来源：http://hz.jinqigfzy.top/gtflkkxarz.html

[C16] 函数 / 方法重载
来源：http://hz.yj20258888.top/gtoqdoadkd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hysaishi.cn/gtgkwkbmeq.html

PHP:  // 无重载
来源：http://hz.tianlin.xyz/gtsehpkfeu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.ehwqpu.com/gtjpdtqcly.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xuanzx.com/gtdguddcun.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.svipenyu.cn/gtvzvwyenh.html

Go:   // 无重载：用不同函数名
来源：http://hz.jinqigufen.top/gtnqlbqrgs.html

Ruby: # 无重载：靠动态参数
来源：http://hz.daxiang520.top/gtbdpozbdp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.ppjwa.cn/gthaozlwtb.html

================================================================================
来源：http://hz.316326.xyz/gtlrhaigll.html

D. 数组 / 列表 / 集合
来源：http://hz.jqgufenzy.top/gtyfxgtrzr.html

================================================================================
来源：http://hz.nanxinkj.top/gtceoffpgc.html

[D01] 创建数组 / 列表
来源：http://hz.yonumen.top/gtsysakeip.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cashguo.top/gtsxpfcbbk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hongshengwenyu.top/gtdhsgjeyc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.52xcode.cn/gtfaevxiph.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.xuetiantiany.cn/gtekarfaex.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.quarkkingdee.top/gtjlgyjfus.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yj20258.top/gtskzdpjvr.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhaomingkeji.xyz/gtwcdumusj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.guowangkeji.top/gtrhieafbz.html

[D02] 追加元素到末尾
来源：http://hz.yanxiufei.cn/gtdminvjeh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.shangyingyoupin.top/gtbljyydop.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.birdmap.top/gtcpoheajs.html

JS:   arr.push(4);
来源：http://hz.chenlongwang.top/gtzqyndkxx.html

TS:   arr.push(4);
来源：http://hz.yuanzhike.top/gtsgrsjako.html

Java: list.add(4);
来源：http://hz.fengsongda.top/gtekbsxacd.html

Go:   arr = append(arr, 4)
来源：http://hz.chenzaomai.com/gtnxbqybkp.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jinqigufen.top/gtednxiqdn.html

C#:   list.Add(4);
来源：http://hz.daxiang520.top/gtrcabhfkw.html

[D03] 在指定位置插入元素
来源：http://hz.xinyue.icu/gtyuejklyp.html

Py:   arr.insert(0, 0)
来源：http://hz.vqdsnc.cn/gtnqetmolh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jinghuilouyu.cn/gtjlglrbww.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.9152youxi.cn/gtmsspfkao.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.sufxvd.cn/gtfpophkgo.html

Java: list.add(0, 0);
来源：http://hz.nanxuanxn.top/gtlblbyttb.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jinghuilouyu.cn/gtgzfmhbsv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.guowangkeji.top/gtbusjxciw.html

C#:   list.Insert(0, 0);
来源：http://hz.9152youxi.cn/gtgrpijyvi.html

[D04] 删除元素
来源：http://hz.pycfn.com/gtugvspnky.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.yongpay.top/gtqkhmddlz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.andypj.xyz/gtrjxmkelf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.iojbl.cn/gtxesiiwpj.html

TS:   arr.splice(0, 1);
来源：http://hz.yj20258888.top/gtqkquamwi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yanxiufei.cn/gtpgfxiwpx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.dashuyun.cn/gtdpbvxpxw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.nanxuanxn.top/gtpwuvvuvm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.zhiwuduotai.top/gtlwkpwtph.html

[D05] 访问与修改元素
来源：http://hz.pengpengdd.cyou/gtvagncfkz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xuanzx.com/gtcyhtiark.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.chenlongwang.top/gtbgrfszmv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.0kj1m.cn/gtxhiqjnuo.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.aizwys.cn/gtqrkreehs.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.guowangkeji.top/gttnawrxgo.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.kuanghao11.cn/gtjerpqdfb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.havefunace.top/gtkfqcdzyt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinyuanbaomall.cn/gtmgerrnse.html

[D06] 数组长度
来源：http://hz.kuanghao11.cn/gtvltbwrmn.html

Py:   len(arr)
来源：http://hz.meibo888.top/gtvfmuitwt.html

PHP:  count($arr);
来源：http://hz.zdqjudy.top/gtpheqnbky.html

JS:   arr.length
来源：http://hz.jiagoushi.top/gtlcwlmnoc.html

TS:   arr.length
来源：http://hz.jqgfzy.top/gtgnjlzxie.html

Java: list.size();
来源：http://hz.shanyushiyangkeji.top/gtrgjtakqq.html

Go:   len(arr)
来源：http://hz.dashuyun.cn/gtrjyczeuf.html

Ruby: arr.length; arr.size
来源：http://hz.hammf.cn/gtwgjjaiop.html

C#:   list.Count;
来源：http://hz.yanxiufei.cn/gtuluhkwxo.html

[D07] 切片 / 取子数组
来源：http://hz.ybcxt.top/gthorvdnvy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhixingplan.top/gtnvmophma.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.tanke756.top/gtzcnaupsv.html

JS:   arr.slice(1, 4);
来源：http://hz.hnqzz.top/gtlfrnrazf.html

TS:   arr.slice(1, 4);
来源：http://hz.yj202588.top/gtxvrsbles.html

Java: list.subList(1, 4);
来源：http://hz.fengsongda.top/gtyroiyktd.html

Go:   arr[1:4]
来源：http://hz.hnxiangtu.top/gtjsbvswxa.html

Ruby: arr[1, 3]
来源：http://hz.andypj.xyz/gtfsrnfqub.html

C#:   list.GetRange(1, 3);
来源：http://hz.zycfv.cn/gtdkajwxmy.html

[D08] 合并两个数组
来源：http://hz.daria6918.cn/gtvwlufuxx.html

Py:   a + b;  a.extend(b)
来源：http://hz.ivvv.top/gtwlmfxnru.html

PHP:  array_merge($a, $b);
来源：http://hz.yj20258.top/gtvsjysfgb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jinyuanbaomall.cn/gtrnpukbhr.html

TS:   [...a, ...b];
来源：http://hz.snrcjt.cn/gtubdzhzvx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yanxiufei.cn/gtzgiwavgf.html

Go:   append(a, b...)
来源：http://hz.wangshuangyany.cn/gtfmfeglxt.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hywenlv.cn/gtymnrqrdd.html

C#:   a.Concat(b).ToList()
来源：http://hz.yuxming.cn/gtycaponug.html

[D09] 排序（升序）
来源：http://hz.cqqwz.cn/gtmzwhbuyn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shangyingyoupin.top/gtuddmgtkn.html

PHP:  sort($arr);
来源：http://hz.shanyushiyangkeji.top/gtsdvcsmmp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ydjk.org.cn/gtpsaiamrz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jinghuilouyu.cn/gtfuphkevx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.daxiang520.top/gtuwdmxekz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.chenlongwang.top/gtgogcokff.html

Ruby: arr.sort
来源：http://hz.zhengqikj.top/gtpxhbjqan.html

C#:   list.Sort();
来源：http://hz.aibaodan.cn/gtkjkxbzmf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jqgufenzy.top/gtgvqhzkjj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.guannengcc.top/gtnkinhkdf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhengqikj.top/gtwmudgqmn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hnqzz.top/gtglvwzpqb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinyuanbaomall.cn/gtdztpeutc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.daxiang520.top/gtkvmkmdlv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.bjfxy.top/gtannkdhfd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yuxming.cn/gteggkauwu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinghuilouyu.cn/gtawcjmqxt.html

[D11] 反转数组
来源：http://hz.ywan-chungtsiang.top/gtxcganthj.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.daria6918.cn/gtzohsdbcd.html

PHP:  array_reverse($arr);
来源：http://hz.ehwqpu.com/gtejaixfdn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.nanxuanxn.top/gtcrysawqu.html

TS:   [...arr].reverse();
来源：http://hz.ehwqpu.com/gtiszzmair.html

Java: Collections.reverse(list);
来源：http://hz.xuetiantiany.cn/gtiaimebrd.html

Go:   slices.Reverse(arr)
来源：http://hz.zhengqikj.top/gtejesyrbc.html

Ruby: arr.reverse
来源：http://hz.hnxiangtu.top/gtdrvaczqm.html

C#:   list.Reverse();
来源：http://hz.gzhubu.top/gtolbczuqh.html

[D12] 查找元素下标
来源：http://hz.nwbrower.top/gtafjbeasy.html

Py:   arr.index(x);  x in arr
来源：http://hz.c1oappe.top/gtxdwjbdit.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.redwolf501.top/gtsqhovswh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sweek.top/gtiejrrhdt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ydzc1.top/gtyspbnolm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yuxming.cn/gtftvqtgnv.html

Go:   slices.Index(arr, x)
来源：http://hz.guowangkeji.top/gtczeqgfam.html

Ruby: arr.index(x)
来源：http://hz.jqgfzy.top/gtgikzotne.html

C#:   list.IndexOf(x);
来源：http://hz.zycfv.cn/gtufzbzmiv.html

[D13] 过滤（保留满足条件的）
来源：http://hz.cucudq.cn/gtxedznnke.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.meibo888.top/gtzmkldvtd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jqgfzy.top/gtmiqkwnle.html

JS:   arr.filter(x => x > 3)
来源：http://hz.ivvv.top/gtwdffupww.html

TS:   arr.filter(x => x > 3)
来源：http://hz.c1oappe.top/gtzqmstcjp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.dashuyun.cn/gtzjptrzmk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hnqzz.top/gtgbbffolz.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.nanxinkj.top/gtbrdmvraw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.kuanghao11.cn/gtcbbzeeru.html

[D14] 映射转换（每个元素变形）
来源：http://hz.dianchejie.cn/gtvtvlxtjf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.pycfn.com/gtsxuungxh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hnqzz.top/gtvuaiqyob.html

JS:   arr.map(x => x * 2)
来源：http://hz.tian-w.cn/gtyuoemacx.html

TS:   arr.map(x => x * 2)
来源：http://hz.sxryk.cn/gtmhonbnhu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shangyingyoupin.top/gtbfcmvwlh.html

Go:   // 手写循环
来源：http://hz.zhengqikj.top/gtitjhujkg.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.hywenlv.cn/gtlxlftjjx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jinyuanbaomall.cn/gtmzwcutmk.html

[D15] 去重
来源：http://hz.dianchejie.cn/gtvxnujtzo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.pengpengdd.cyou/gtmkimnzqy.html

PHP:  array_unique($arr);
来源：http://hz.gzhubu.top/gttpuzgrvv.html

JS:   [...new Set(arr)]
来源：http://hz.yj20258888.top/gtmevlnjir.html

TS:   [...new Set(arr)]
来源：http://hz.nwbrower.top/gttsnxzpjm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhijiandao.cn/gtxqikwaxh.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.chenzaomai.com/gtyvgzxhym.html

Ruby: arr.uniq
来源：http://hz.ivvv.top/gtxliojefi.html

C#:   list.Distinct().ToList()
来源：http://hz.zhoulong.xyz/gthdenepoe.html

[D16] 求和与平均值
来源：http://hz.xinyue.icu/gtcacqzvur.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ppjwa.cn/gtdbvirrho.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.haohaochexian.top/gtmogamaik.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.dashuyun.cn/gtoqalujgy.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.bjfxy.top/gtaunzorhy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.mhx1999.top/gteeeugkcg.html

Go:   // 手写循环累加
来源：http://hz.ywan-chungtsiang.top/gtuvulvqad.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hongshengwenyu.top/gtisteqdon.html

C#:   list.Sum();  list.Average()
来源：http://hz.hnxiangtu.top/gtwefksiwh.html

[D17] 最大值与最小值
来源：http://hz.sufxvd.cn/gtfdpqulxk.html

Py:   max(arr);  min(arr)
来源：http://hz.xuanzx.com/gtkixliifb.html

PHP:  max($arr);  min($arr);
来源：http://hz.shanyushiyangkeji.top/gtetxgimla.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xinyue.icu/gtmrkruust.html

TS:   Math.max(...arr);
来源：http://hz.fengsongda.top/gthwjttmkc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.0kj1m.cn/gtkymkjxsg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.guowangkeji.top/gtfkzmpnps.html

Ruby: arr.max;  arr.min
来源：http://hz.gotoacloud.top/gtwrmxvqzh.html

C#:   list.Max();  list.Min()
来源：http://hz.yj20258.top/gtgufizslb.html

[D18] 扁平化嵌套数组
来源：http://hz.cqqwz.cn/gtoooupctm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xylfe.cn/gtytqymgdm.html

PHP:  array_merge(...$nested);
来源：http://hz.hongshengwenyu.top/gttvhekdil.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yvedp.cn/gtuxflaejj.html

TS:   nested.flat();
来源：http://hz.aibaodan.cn/gtvfjrzhff.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jiagoushi.top/gtfofzoytq.html

Go:   // 手写双层循环
来源：http://hz.haohaochexian.top/gtfrqsicsz.html

Ruby: nested.flatten
来源：http://hz.birdmap.top/gtwbjrfjnk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xinyue.icu/gttnezxgon.html

[D19] 按字段分组
来源：http://hz.dashuyun.cn/gtxjrnvjeb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jyoumei.cn/gtbsizxwup.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.dashuyun.cn/gtokfsisjz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.bjfxy.top/gtcpyfyavg.html


<!-- 参考信息 -->