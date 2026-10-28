代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.haohaochexian.top/gtvzjltldo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://hz.cdnleiting.top/gtkfsheork.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://hz.quarkkingdee.top/gtsgeedayz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://hz.jianghu66.top/gtumqjiiio.html

Ruby: def total(*nums); nums.sum; end
来源：http://hz.gaohongyu789.top/gttlqezhdr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://hz.gaohongyu789.top/gthykdptmx.html

[C04] 命名参数 / 关键字参数
来源：http://hz.ybcxt.top/gtowaagwxn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://hz.zycfv.cn/gtzibegrlg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.ppjwa.cn/gtgehymsyn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.zdqjudy.top/gtjbiynlyv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.wangdashe.top/gtsrhbaeqd.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.xinyue.icu/gtgbeihadj.html

Go:   // 无：用配置结构体参数
来源：http://hz.zhijiandao.cn/gtlgaesded.html

Ruby: f(a: 1, b: 2)
来源：http://hz.pengpengdd.cyou/gtqkgzpzmd.html

C#:   f(a: 1, b: 2)
来源：http://hz.zhoulong.xyz/gtxsjjqyjr.html

[C05] 返回多个值
来源：http://hz.jinghuilouyu.cn/gthqehtnvw.html

Py:   return a, b
来源：http://hz.meibo888.top/gtdswsrkzu.html

PHP:  return [$a, $b];
来源：http://hz.316326.xyz/gtbyxmymai.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.pengpengdd.cyou/gtukoygfji.html

TS:   return { a, b };
来源：http://hz.shangyingyoupin.top/gttolcdxad.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.sysykeji.top/gtssqmksic.html

Go:   return a, b
来源：http://hz.yj20258.top/gtaiivbijb.html

Ruby: return a, b
来源：http://hz.shanyushiyangkeji.top/gtvpavchdm.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.gzhubu.top/gtqazrktky.html

[C06] 匿名函数 / lambda
来源：http://hz.shanyushiyangtech.top/gtscuwconj.html

Py:   square = lambda x: x * x
来源：http://hz.yanxiufei.cn/gtjxcjudnl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.meibo888.top/gtkjvqojix.html

JS:   const square = x => x * x;
来源：http://hz.yuxming.cn/gtzuxinvmk.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.fengsongda.top/gtzublhhed.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.aibaodan.cn/gtillbijpf.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.0kj1m.cn/gtomjmiawo.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jinyuanbaomall.cn/gtythpdiud.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.shzxlz.cn/gtltgiojbw.html

[C07] 把函数作为参数传入
来源：http://hz.gotoacloud.top/gtbgkcqasb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.c1oappe.top/gtwvkuhicf.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.fzhhl.top/gtcurrzkjk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.sysykeji.top/gtgdkryytf.html

TS:   arr.map(String)
来源：http://hz.shanyushiyangkeji.top/gthgtqymgn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.bjfxy.top/gtvalkvoic.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.cdnleiting.top/gtqsuaibsw.html

Ruby: arr.map(&:upcase)
来源：http://hz.ybcxt.top/gtlonxlpan.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.iojbl.cn/gtxvgjdfac.html

[C08] 闭包
来源：http://hz.cqqwz.cn/gtphuzzfvt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.yongpay.top/gtengfzggn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.xuetiantiany.cn/gtkqmbante.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.316326.xyz/gtlwnzumoy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.shzxlz.cn/gtmfuyeqji.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.xuanzx.com/gtqnzyqfek.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.quarkkingdee.top/gtpwntsnwb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jqgfzy.top/gtfncrdmkk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.yj20258888.top/gtnavilwjf.html

[C09] 递归
来源：http://hz.wangdashe.top/gtwjfbeuwl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.iojbl.cn/gtsercjnkn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.haohaochexian.top/gthbflhtmu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.tianlin.xyz/gtguulnzfh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinqigufen.top/gtwbnknxqr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.zhengqikj.top/gtrqlbybfl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.shanyushiyangtech.top/gtyzvtedup.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.pycfn.com/gtzzpenxhl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.ydjk.org.cn/gtlljzvnqs.html

[C10] 变量作用域
来源：http://hz.yvedp.cn/gteccsgkzk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.daxiang520.top/gtufgrwbpo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.0kj1m.cn/gtnixrswek.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.hnqzz.top/gtkmkkiofc.html

TS:   同 JS
来源：http://hz.zycfv.cn/gtrqyqzxou.html

Java: 方法内为块级作用域
来源：http://hz.jinghuilouyu.cn/gtizcolips.html

Go:   花括号块级作用域
来源：http://hz.cqqwz.cn/gtiqjgbxgy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.zhiwuduotai.top/gtrcqbyaiq.html

C#:   块级作用域
来源：http://hz.cqqwz.cn/gtaebgpuce.html

[C11] 模块导入与导出
来源：http://hz.jinqigfzy.top/gtproltpsk.html

Py:   from module import func
来源：http://hz.yuxming.cn/gtiymvdtzv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.guowangkeji.top/gtqvctlyjk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cashguo.top/gtzgpifekp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.shanyushiyangkeji.top/gtgudgfcvy.html

Java: import java.util.List;
来源：http://hz.jinqigufen.top/gtkentowpz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zdqjudy.top/gttuvtpvaf.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhengqikj.top/gtwevqnuls.html

C#:   using System.Text;
来源：http://hz.jiagoushi.top/gtqjgdwaiw.html

[C12] 立即执行函数 IIFE
来源：http://hz.chenzaomai.com/gtpoibmojf.html

Py:   (lambda: print("run"))()
来源：http://hz.zhiwuduotai.top/gtmnryosfg.html

PHP:  (function () { echo "run"; })();
来源：http://hz.chenlongwang.top/gtzufwkiij.html

JS:   (() => { console.log("run"); })();
来源：http://hz.daxiang520.top/gtmpomjekx.html

TS:   (() => { console.log("run"); })();
来源：http://hz.0kj1m.cn/gtyvgiyegj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.sweek.top/gtpabthkhk.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhoulong.xyz/gtusjrlzie.html

Ruby: -> { puts "run" }.call
来源：http://hz.tian-w.cn/gtsrmfrjaz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.xingfuxueyuan.xyz/gtjshlibkf.html

[C13] 类型声明 / 类型注解
来源：http://hz.gzhubu.top/gtonrbxciw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ybcxt.top/gtnmxmrvrj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.nwbrower.top/gtlpcsyppu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.bjfxy.top/gtldhsvemu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.aibaodan.cn/gtohiyfbyk.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.nanxuanxn.top/gtcvmyjbsb.html

Go:   func add(a, b int) int
来源：http://hz.yongpay.top/gthpfqkgce.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zhaomingkeji.xyz/gtftrkzuyh.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.aizwys.cn/gtxvxjciuh.html

[C14] 泛型函数
来源：http://hz.xinyue.icu/gtjffejaeo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ppjwa.cn/gtlhfipfnm.html

PHP:  // 无泛型
来源：http://hz.yvedp.cn/gtzpnubcpt.html

JS:   // 无泛型
来源：http://hz.xinyue.icu/gtegjrdbmo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sxryk.cn/gtjuulqctz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.hongshengwenyu.top/gtbdfujaka.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.sweek.top/gtpxfyfrmy.html

Ruby: # 无泛型
来源：http://hz.zhengqikj.top/gtflzlexvo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.svipenyu.cn/gtuboggsyn.html

[C15] 解构 / 展开参数
来源：http://hz.dashuyun.cn/gtczycypyz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.havefunace.top/gtjonupgfp.html

PHP:  [$a, $b] = $pair;
来源：http://hz.havefunace.top/gtgyvsuiqb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.tian-w.cn/gtfbnthjxu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jinghuilouyu.cn/gtrnjmhodn.html

Java: // 无解构
来源：http://hz.hongshengwenyu.top/gtedzszhfs.html

Go:   // 无解构
来源：http://hz.quarkkingdee.top/gtnjuuncgs.html

Ruby: a, b = pair
来源：http://hz.9152youxi.cn/gtaifqniyv.html

C#:   var (a, b) = pair;
来源：http://hz.cdnleiting.top/gtkjjwpdjf.html

[C16] 函数 / 方法重载
来源：http://hz.haohaochexian.top/gtktsvyhpo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.ehwqpu.com/gtssiwmgbp.html

PHP:  // 无重载
来源：http://hz.chenzaomai.com/gtheoehopm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.bjfxy.top/gtwrrnljkv.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.xuetiantiany.cn/gtsvpxxeah.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.vqdsnc.cn/gtokrexcmk.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhijiandao.cn/gtvtybtpxi.html

Ruby: # 无重载：靠动态参数
来源：http://hz.nwbrower.top/gtlnyjiqcf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.cheryme.top/gtrpbwradp.html

================================================================================
来源：http://hz.zhiwuduotai.top/gthqshngbr.html

D. 数组 / 列表 / 集合
来源：http://hz.hnxiangtu.top/gtajkwsngs.html

================================================================================
来源：http://hz.ivvv.top/gtrlxdegml.html

[D01] 创建数组 / 列表
来源：http://hz.xuanzx.com/gtaafmgber.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xingfuxueyuan.xyz/gtkafmkmuk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhixingplan.top/gtmsuplkll.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.0kj1m.cn/gtpqaisyyo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.sweek.top/gtqxibxmcu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jinqigfzy.top/gtzhodhtfk.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jiagoushi.top/gtfnwtsqfv.html

Ruby: arr = [1, 2, 3]
来源：http://hz.gzhubu.top/gteihckptw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xziqi.cn/gtbfjubapw.html

[D02] 追加元素到末尾
来源：http://hz.xinyue.icu/gtfenwcmke.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jqgufenzy.top/gtplgwisok.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yanxiufei.cn/gtqanmnxpt.html

JS:   arr.push(4);
来源：http://hz.fengsongda.top/gtcgiauznf.html

TS:   arr.push(4);
来源：http://hz.pycfn.com/gtveqrqjnp.html

Java: list.add(4);
来源：http://hz.yj20258.top/gtovznbpph.html

Go:   arr = append(arr, 4)
来源：http://hz.yueranfly.top/gtkzvsvgoi.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xziqi.cn/gtllzkoiwa.html

C#:   list.Add(4);
来源：http://hz.hysaishi.cn/gtscmsvkvj.html

[D03] 在指定位置插入元素
来源：http://hz.chenzaomai.com/gttdvpbndz.html

Py:   arr.insert(0, 0)
来源：http://hz.ybcxt.top/gtkoogoexs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yj20258888.top/gtsqusxads.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.redwolf501.top/gtwouncxej.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.jinqigfzy.top/gtbqxqcdau.html

Java: list.add(0, 0);
来源：http://hz.jinqigufen.top/gtukxflopp.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.xylfe.cn/gtdraklbyc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.guannengcc.top/gtatnueksz.html

C#:   list.Insert(0, 0);
来源：http://hz.zhoulong.xyz/gthwkkvxhy.html

[D04] 删除元素
来源：http://hz.zhoulong.xyz/gtqhylroxq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.havefunace.top/gtnbkawaht.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.xuetiantiany.cn/gtbjvnhhxl.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.gzhubu.top/gtbjbnpyya.html

TS:   arr.splice(0, 1);
来源：http://hz.jinqigfzy.top/gtexlthsxm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.mhx1999.top/gtddddykwf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.shzxlz.cn/gttwinkjcx.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.cdnleiting.top/gtrdicjtlg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.wangshuangyany.cn/gtjabtfzgc.html

[D05] 访问与修改元素
来源：http://hz.sxryk.cn/gtsquiccdr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yvedp.cn/gtvjhzgxvh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ppjwa.cn/gthstfbdbu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.9152youxi.cn/gtdvtmfgsy.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.cashguo.top/gttqybgfjg.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.fengsongda.top/gtnssrexjf.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hammf.cn/gtijmjomfm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hfpthk.cn/gtaxpbdeqs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jianghu66.top/gtkchkasva.html

[D06] 数组长度
来源：http://hz.meibo888.top/gtkwbhpaac.html

Py:   len(arr)
来源：http://hz.redwolf501.top/gtbbsnhard.html

PHP:  count($arr);
来源：http://hz.haohaochexian.top/gtmvvdwvpd.html

JS:   arr.length
来源：http://hz.yj202588.top/gtlawpllvp.html

TS:   arr.length
来源：http://hz.zdqjudy.top/gteiyrfirr.html

Java: list.size();
来源：http://hz.0kj1m.cn/gtqjaycver.html

Go:   len(arr)
来源：http://hz.ydjk.org.cn/gtnzfhfpnn.html

Ruby: arr.length; arr.size
来源：http://hz.shanyushiyangkeji.top/gthizdvzzm.html

C#:   list.Count;
来源：http://hz.pengpengdd.cyou/gtifiogxsi.html

[D07] 切片 / 取子数组
来源：http://hz.nanxuanxn.top/gtxhqwjfco.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xylfe.cn/gteetprdgu.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.svipenyu.cn/gtovkuzemc.html

JS:   arr.slice(1, 4);
来源：http://hz.nanxinkj.top/gtnzxmtpmo.html

TS:   arr.slice(1, 4);
来源：http://hz.daria6918.cn/gtbldjryjv.html

Java: list.subList(1, 4);
来源：http://hz.fengsongda.top/gtmnsdinnv.html

Go:   arr[1:4]
来源：http://hz.birdmap.top/gtalpoatss.html

Ruby: arr[1, 3]
来源：http://hz.yanxiufei.cn/gtlcscadej.html

C#:   list.GetRange(1, 3);
来源：http://hz.0kj1m.cn/gtpymklqdc.html

[D08] 合并两个数组
来源：http://hz.shuidangran.top/gtgvssblbt.html

Py:   a + b;  a.extend(b)
来源：http://hz.guowangkeji.top/gtrblnobhf.html

PHP:  array_merge($a, $b);
来源：http://hz.yuanzhike.top/gtyhawokyj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yuanzhike.top/gtslvwdptx.html

TS:   [...a, ...b];
来源：http://hz.shanyushiyangkeji.top/gtfvggxskm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shanyushiyangtech.top/gtbbesnlpy.html

Go:   append(a, b...)
来源：http://hz.shuidangran.top/gtnefursma.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jinyuanbaomall.cn/gtwzbdhjgf.html

C#:   a.Concat(b).ToList()
来源：http://hz.hnxiangtu.top/gtogshpnke.html

[D09] 排序（升序）
来源：http://hz.0kj1m.cn/gtijgnhnxi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.fengsongda.top/gtcbosmkjs.html

PHP:  sort($arr);
来源：http://hz.fengsongda.top/gtqnvhapvy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.cqqwz.cn/gtfogwmwvo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.gaohongyu789.top/gtmyubsxlf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cucudq.cn/gttdhfyxof.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.xylfe.cn/gtommvgcqi.html

Ruby: arr.sort
来源：http://hz.chenzaomai.com/gtyichfxdi.html

C#:   list.Sort();
来源：http://hz.quarkkingdee.top/gtbndweidd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xingfuxueyuan.xyz/gtzcywtans.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ydjk.org.cn/gtypivjjpo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cdnleiting.top/gtrtjcmgmm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhiwuduotai.top/gtqwkkekaz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.quarkkingdee.top/gtvagdrjnz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.ppjwa.cn/gtklwgkwbq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.sweek.top/gtspwumpyt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ydzc1.top/gtcpllthjd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.chenzaomai.com/gtjdbygzit.html

[D11] 反转数组
来源：http://hz.meibo888.top/gtlhaypwsp.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.gotoacloud.top/gtianlevai.html

PHP:  array_reverse($arr);
来源：http://hz.chenjidiqi.icu/gtkqyqlacc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ydzc1.top/gtxetktcns.html

TS:   [...arr].reverse();
来源：http://hz.ybcxt.top/gtwsprwarp.html

Java: Collections.reverse(list);
来源：http://hz.dianchejie.cn/gtebdtzblo.html

Go:   slices.Reverse(arr)
来源：http://hz.ivvv.top/gtygimqyak.html

Ruby: arr.reverse
来源：http://hz.havefunace.top/gtllzsakrt.html

C#:   list.Reverse();
来源：http://hz.bjfxy.top/gtodcapykl.html

[D12] 查找元素下标
来源：http://hz.yuxming.cn/gtsjzusnpl.html

Py:   arr.index(x);  x in arr
来源：http://hz.0kj1m.cn/gtfrmxwsut.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.quarkkingdee.top/gtexhesaom.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sufxvd.cn/gthqtmvies.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.fzhhl.top/gtbbumghju.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.chenzaomai.com/gtacashlen.html

Go:   slices.Index(arr, x)
来源：http://hz.havefunace.top/gtofrcgbls.html

Ruby: arr.index(x)
来源：http://hz.zhiwuduotai.top/gtghtnflgf.html

C#:   list.IndexOf(x);
来源：http://hz.gotoacloud.top/gtqpjtomwz.html

[D13] 过滤（保留满足条件的）
来源：http://hz.tianlin.xyz/gtxbpklpbt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jyoumei.cn/gtixorlozy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhengqikj.top/gtoddewwck.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yj20258.top/gtrnrractz.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hnqzz.top/gtseekasvy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.smart0.xyz/gtpocpqgrk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cashguo.top/gtzuuyhzmh.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.gaohongyu789.top/gtoffyxapk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shanyushiyangtech.top/gtrbwcwnof.html

[D14] 映射转换（每个元素变形）
来源：http://hz.shanyushiyangkeji.top/gtxitutauv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yuxming.cn/gtaxodtdrg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.feifeiyinyue.top/gtunamfijs.html

JS:   arr.map(x => x * 2)
来源：http://hz.hfpthk.cn/gtztypxfzu.html

TS:   arr.map(x => x * 2)
来源：http://hz.jqgufenzy.top/gtbydaegeo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.aizwys.cn/gtudlivktr.html

Go:   // 手写循环
来源：http://hz.jinqigufen.top/gtkltinrmw.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.316326.xyz/gtdhceldwu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.fzhhl.top/gtegbohjrp.html

[D15] 去重
来源：http://hz.zhijiandao.cn/gtgmurqxwr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jqgufenzy.top/gtbqzjltfk.html

PHP:  array_unique($arr);
来源：http://hz.jiagoushi.top/gtcsqxtqcc.html

JS:   [...new Set(arr)]
来源：http://hz.hywenlv.cn/gtjwhxgpxa.html

TS:   [...new Set(arr)]
来源：http://hz.yuxming.cn/gthznubmkc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhijiandao.cn/gtiuqvxghz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.316326.xyz/gtokwskbbo.html

Ruby: arr.uniq
来源：http://hz.yueranfly.top/gtwqsojzso.html

C#:   list.Distinct().ToList()
来源：http://hz.birdmap.top/gtehkmqcqt.html

[D16] 求和与平均值
来源：http://hz.52xcode.cn/gtdmrnetel.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.cqqwz.cn/gthbfpewfa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hongshengwenyu.top/gtdaufwhgd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.dashuyun.cn/gtysdxijid.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jiagoushi.top/gtqawdrzhx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.gaohongyu789.top/gtmeievpyb.html

Go:   // 手写循环累加
来源：http://hz.xinyue.icu/gtacojimnv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhongyouzk.top/gtkacyllyj.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhoulong.xyz/gtullqhwrh.html

[D17] 最大值与最小值
来源：http://hz.fengsongda.top/gtvobgobqe.html

Py:   max(arr);  min(arr)
来源：http://hz.yuxming.cn/gtufpassjf.html

PHP:  max($arr);  min($arr);
来源：http://hz.cucudq.cn/gttjqvxdfb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.redwolf501.top/gtbbfdstcv.html

TS:   Math.max(...arr);
来源：http://hz.jqgufenzy.top/gtcskczqwq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.sxryk.cn/gtgdrvxmkc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.vqdsnc.cn/gttwacrmrc.html

Ruby: arr.max;  arr.min
来源：http://hz.tianlin.xyz/gtugjxlqln.html

C#:   list.Max();  list.Min()
来源：http://hz.sxryk.cn/gtmmeyikbj.html

[D18] 扁平化嵌套数组
来源：http://hz.nwbrower.top/gthziutdfp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ppjwa.cn/gtfvcbfnai.html

PHP:  array_merge(...$nested);
来源：http://hz.cdnleiting.top/gtvsrsiyhi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.guowangkeji.top/gtpafivluh.html

TS:   nested.flat();
来源：http://hz.yj20258888.top/gtwlrzrqwb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jinghuilouyu.cn/gtluxvppxv.html

Go:   // 手写双层循环
来源：http://hz.jlsjyb.cn/gtackuumoq.html

Ruby: nested.flatten
来源：http://hz.jinqigfzy.top/gttezplisz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.pycfn.com/gthwqxxype.html

[D19] 按字段分组
来源：http://hz.jinghuilouyu.cn/gtfgqtxibh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.haohaochexian.top/gtenzdvebo.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jyoumei.cn/gtbcnnhtoj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cucudq.cn/gtjdrtiitk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hongshengwenyu.top/gtqcjkbage.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jyoumei.cn/gtrvpuevrd.html

Go:   // 手写 map[string][]T
来源：http://hz.ydzc1.top/gtfnuzseri.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yuxming.cn/gtxmyxltnh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gzhubu.top/gtjuouhjgq.html

[D20] 统计每个元素出现次数
来源：http://hz.xingfuxueyuan.xyz/gtuurexsib.html

Py:   Counter(arr)
来源：http://hz.cdnleiting.top/gtickthnsl.html

PHP:  array_count_values($arr);
来源：http://hz.zhixingplan.top/gttmrueeqi.html


<!-- 参考信息 -->