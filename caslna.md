代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://hz.guowangkeji.top/gtzmydlahl.html

Ruby: f(a: 1, b: 2)
来源：http://hz.iojbl.cn/gtokvrpnhs.html

C#:   f(a: 1, b: 2)
来源：http://hz.52xcode.cn/gtoyvbdpfi.html

[C05] 返回多个值
来源：http://hz.shanyushiyangtech.top/gtfnzeprgs.html

Py:   return a, b
来源：http://hz.jinyuanbaomall.cn/gtzmcgsidq.html

PHP:  return [$a, $b];
来源：http://hz.nanxinkj.top/gtvsnaijgx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.dianchejie.cn/gthgkmcvyb.html

TS:   return { a, b };
来源：http://hz.tian-w.cn/gtfcdypjga.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.shuidangran.top/gtfeaaokbc.html

Go:   return a, b
来源：http://hz.feifeiyinyue.top/gtyyrxexct.html

Ruby: return a, b
来源：http://hz.iojbl.cn/gtmwhooazi.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zdqjudy.top/gtemhgzyft.html

[C06] 匿名函数 / lambda
来源：http://hz.cheryme.top/gtchzovwgy.html

Py:   square = lambda x: x * x
来源：http://hz.redwolf501.top/gtqmgvldlv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.andypj.xyz/gtvavcolyx.html

JS:   const square = x => x * x;
来源：http://hz.tianlin.xyz/gticvlckir.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.hysaishi.cn/gtneoqpljh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.andypj.xyz/gtdrqjxqvb.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.birdmap.top/gtxfrubqqx.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jqgfzy.top/gtgxqcewir.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jinqigufen.top/gtxnmttexk.html

[C07] 把函数作为参数传入
来源：http://hz.fengsongda.top/gtkiefbmms.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.yj20258.top/gtqapzngds.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.jyoumei.cn/gtjeyucbfm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.52xcode.cn/gtmrctybaa.html

TS:   arr.map(String)
来源：http://hz.pycfn.com/gtmbevqnsa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.chenzaomai.com/gtgbecjxob.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hysaishi.cn/gtnnumawgc.html

Ruby: arr.map(&:upcase)
来源：http://hz.yueranfly.top/gtgbgyznyw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.shanyushiyangtech.top/gtwppxknga.html

[C08] 闭包
来源：http://hz.ydjk.org.cn/gtnqbhhwxi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zhaomingkeji.xyz/gthxaltjhj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.cucudq.cn/gtfbxmqxjt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yonumen.top/gtjjmteixi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.wangdashe.top/gtkdpieuog.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.jinqigufen.top/gtrtclldya.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.jinyuanbaomall.cn/gttqrmkzcv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zhiwuduotai.top/gtsxacfblo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.ivvv.top/gttrjkfcim.html

[C09] 递归
来源：http://hz.316326.xyz/gtlvvmfldu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.ywan-chungtsiang.top/gthkuskxcb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.sweek.top/gtarkveqmg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.pengpengdd.cyou/gtyiysymud.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhiwuduotai.top/gtkqcizkfe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.redwolf501.top/gtxzwgauji.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.kuanghao11.cn/gtpzldhbyr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.wangdashe.top/gthkjkzqed.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.hfpthk.cn/gtcyebaqfw.html

[C10] 变量作用域
来源：http://hz.daria6918.cn/gtfhawuyav.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.shzxlz.cn/gtlvsovsmz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ydzc1.top/gtwzhpyyrp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.gaohongyu789.top/gtgwteqfha.html

TS:   同 JS
来源：http://hz.dashuyun.cn/gtpjqbuqom.html

Java: 方法内为块级作用域
来源：http://hz.smart0.xyz/gtqhfdiiqb.html

Go:   花括号块级作用域
来源：http://hz.sweek.top/gtjwscvwmu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.chenzaomai.com/gtzkxjolip.html

C#:   块级作用域
来源：http://hz.bjfxy.top/gtzkctmfta.html

[C11] 模块导入与导出
来源：http://hz.zycfv.cn/gtawsgadnx.html

Py:   from module import func
来源：http://hz.yj20258888.top/gtcqzmsnce.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhaomingkeji.xyz/gtyidouock.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shanyushiyangkeji.top/gtmrjsqafs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ivvv.top/gtaraoiise.html

Java: import java.util.List;
来源：http://hz.redwolf501.top/gtmyqepsib.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinghuilouyu.cn/gtpbzzscqw.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.fzhhl.top/gtdegdqdfa.html

C#:   using System.Text;
来源：http://hz.jinghuilouyu.cn/gtwdezzjdp.html

[C12] 立即执行函数 IIFE
来源：http://hz.yuanzhike.top/gtnkeovqvu.html

Py:   (lambda: print("run"))()
来源：http://hz.mhx1999.top/gtyvzwrpfc.html

PHP:  (function () { echo "run"; })();
来源：http://hz.haohaochexian.top/gtwjccbydd.html

JS:   (() => { console.log("run"); })();
来源：http://hz.havefunace.top/gtxvzmulcf.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jinqigfzy.top/gtslkctykc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.bjfxy.top/gtimwklymj.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jianghu66.top/gtzunivzwh.html

Ruby: -> { puts "run" }.call
来源：http://hz.hnqzz.top/gtcykerdln.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.yj20258.top/gtfrmutrms.html

[C13] 类型声明 / 类型注解
来源：http://hz.shangyingyoupin.top/gtxyncyuai.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.quarkkingdee.top/gtlrjvcbmz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenzaomai.com/gtsybmiarb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.zhaomingkeji.xyz/gttsopbjol.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.chenlongwang.top/gtudhrwyvp.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.vqdsnc.cn/gtqdciaxpd.html

Go:   func add(a, b int) int
来源：http://hz.xingfuxueyuan.xyz/gtbzisdeuc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.gaohongyu789.top/gtbfajncrf.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.chenlongwang.top/gtmpacooqs.html

[C14] 泛型函数
来源：http://hz.guowangkeji.top/gtlqfeowox.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ybcxt.top/gtvgeqgffh.html

PHP:  // 无泛型
来源：http://hz.hnxiangtu.top/gtuwdkdxlc.html

JS:   // 无泛型
来源：http://hz.gotoacloud.top/gtwaklcajc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ehwqpu.com/gtevwllbxg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.wangshuangyany.cn/gtzpxoywpa.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.c1oappe.top/gtmfnchesg.html

Ruby: # 无泛型
来源：http://hz.mhx1999.top/gtucjzjfea.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yj202588.top/gtktdqmxdh.html

[C15] 解构 / 展开参数
来源：http://hz.andypj.xyz/gtyarzuxxy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.daxiang520.top/gtjpiakyfo.html

PHP:  [$a, $b] = $pair;
来源：http://hz.pycfn.com/gtuwgjjmuj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xinyue.icu/gtoxkancom.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.chenjidiqi.icu/gtjrufzbtw.html

Java: // 无解构
来源：http://hz.gotoacloud.top/gtiryfdmrw.html

Go:   // 无解构
来源：http://hz.cashguo.top/gtllqjtzod.html

Ruby: a, b = pair
来源：http://hz.cucudq.cn/gtszxcxfqq.html

C#:   var (a, b) = pair;
来源：http://hz.hywenlv.cn/gtsawizvds.html

[C16] 函数 / 方法重载
来源：http://hz.zdqjudy.top/gtrplrmdka.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yvedp.cn/gtjadzghvk.html

PHP:  // 无重载
来源：http://hz.hnxiangtu.top/gtiwotpoqy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.chenzaomai.com/gtvjjpcsms.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.hfpthk.cn/gtlycyufzy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.kuanghao11.cn/gtufgfufmr.html

Go:   // 无重载：用不同函数名
来源：http://hz.ydzc1.top/gtymqusgvi.html

Ruby: # 无重载：靠动态参数
来源：http://hz.sweek.top/gtnbdtpgff.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xziqi.cn/gtgtoggylg.html

================================================================================
来源：http://hz.jinqigufen.top/gtdzcwhcki.html

D. 数组 / 列表 / 集合
来源：http://hz.iojbl.cn/gtwqraxsxd.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtlpbiznmv.html

[D01] 创建数组 / 列表
来源：http://hz.fzhhl.top/gtatrgjwwu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jlsjyb.cn/gtjrntmxji.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.redwolf501.top/gthswlqwms.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.sweek.top/gtrqqssrrl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.haohaochexian.top/gttuckflph.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yuanzhike.top/gtpyvcoezf.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.feifeiyinyue.top/gtnlearlad.html

Ruby: arr = [1, 2, 3]
来源：http://hz.wangdashe.top/gtoejimfgj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.aizwys.cn/gtpwdrjhgv.html

[D02] 追加元素到末尾
来源：http://hz.svipenyu.cn/gtcbdbbzjs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhengqikj.top/gtprzmhfdm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xuanzx.com/gtsjfrlouu.html

JS:   arr.push(4);
来源：http://hz.feifeiyinyue.top/gtxjouslaa.html

TS:   arr.push(4);
来源：http://hz.yangfankeji.com/gtblodvybc.html

Java: list.add(4);
来源：http://hz.iojbl.cn/gtbvooxaon.html

Go:   arr = append(arr, 4)
来源：http://hz.jianghu66.top/gtnmawggfq.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ybcxt.top/gtekausxmb.html

C#:   list.Add(4);
来源：http://hz.snrcjt.cn/gttcohuxhm.html

[D03] 在指定位置插入元素
来源：http://hz.hammf.cn/gtpcmnrbpy.html

Py:   arr.insert(0, 0)
来源：http://hz.chenjidiqi.icu/gtbowhtdmv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.0kj1m.cn/gteeeqbtkv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.shangyingyoupin.top/gttpvzbhva.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.wangshuangyany.cn/gtgjffigxq.html

Java: list.add(0, 0);
来源：http://hz.ybcxt.top/gtgtbqeaqz.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jinyuanbaomall.cn/gtxxflzlzn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.cqqwz.cn/gtzbofrgfu.html

C#:   list.Insert(0, 0);
来源：http://hz.jyoumei.cn/gtqpmjpyol.html

[D04] 删除元素
来源：http://hz.aizwys.cn/gtrxlcflwu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.daria6918.cn/gtcnvthkbt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.yanxiufei.cn/gtwprtcpft.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.chenjidiqi.icu/gtffitzeff.html

TS:   arr.splice(0, 1);
来源：http://hz.jianghu66.top/gthfvxyhks.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ybcxt.top/gtzingyklu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jianghu66.top/gtbsdakumn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.cheryme.top/gtrqdnorfs.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.sufxvd.cn/gtjpkaemso.html

[D05] 访问与修改元素
来源：http://hz.zhengqikj.top/gttltlnend.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.shuidangran.top/gtdvveuzhv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.cashguo.top/gthcpjbiiv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.pycfn.com/gtzaoqxfyi.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hnqzz.top/gtjpgzfmuz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yvedp.cn/gtqlsmmmyp.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.gotoacloud.top/gtmpqzfaiz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.iojbl.cn/gtehdgfgzz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.shuidangran.top/gtxbvcwwct.html

[D06] 数组长度
来源：http://hz.cashguo.top/gtrxwprqvi.html

Py:   len(arr)
来源：http://hz.vqdsnc.cn/gtuqvzxabw.html

PHP:  count($arr);
来源：http://hz.wangdashe.top/gtcheogmdj.html

JS:   arr.length
来源：http://hz.jinqigfzy.top/gtwpnmlmns.html

TS:   arr.length
来源：http://hz.haohaochexian.top/gtpuibjtnk.html

Java: list.size();
来源：http://hz.pengpengdd.cyou/gtdhzospsx.html

Go:   len(arr)
来源：http://hz.wangdashe.top/gtrgqovgql.html

Ruby: arr.length; arr.size
来源：http://hz.jqgfzy.top/gteftclbig.html

C#:   list.Count;
来源：http://hz.hongshengwenyu.top/gtdlxkkrsm.html

[D07] 切片 / 取子数组
来源：http://hz.tian-w.cn/gtlafnaolq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.havefunace.top/gtldddwgpd.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.cheryme.top/gtwkalseyl.html

JS:   arr.slice(1, 4);
来源：http://hz.ehwqpu.com/gtfhbjgbte.html

TS:   arr.slice(1, 4);
来源：http://hz.yongpay.top/gtygefxhrt.html

Java: list.subList(1, 4);
来源：http://hz.havefunace.top/gtzbzliacb.html

Go:   arr[1:4]
来源：http://hz.yj202588.top/gtxomhbrnp.html

Ruby: arr[1, 3]
来源：http://hz.xziqi.cn/gttfqjzori.html

C#:   list.GetRange(1, 3);
来源：http://hz.hongshengwenyu.top/gthaowmflq.html

[D08] 合并两个数组
来源：http://hz.wangdashe.top/gtaqbtjilw.html

Py:   a + b;  a.extend(b)
来源：http://hz.vqdsnc.cn/gtbriojfgt.html

PHP:  array_merge($a, $b);
来源：http://hz.tanke756.top/gtjefowjcv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.wangdashe.top/gtzxfubzsi.html

TS:   [...a, ...b];
来源：http://hz.xingfuxueyuan.xyz/gtkogtlhmk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jinghuilouyu.cn/gtvdtdxkvz.html

Go:   append(a, b...)
来源：http://hz.ywan-chungtsiang.top/gtujyjtfhv.html

Ruby: a + b;  a.concat(b)
来源：http://hz.aibaodan.cn/gtwhlitggt.html

C#:   a.Concat(b).ToList()
来源：http://hz.xinyue.icu/gtmgktgyre.html

[D09] 排序（升序）
来源：http://hz.shzxlz.cn/gtvjgflqit.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shanyushiyangtech.top/gtakwojdjf.html

PHP:  sort($arr);
来源：http://hz.cheryme.top/gtuexeslqa.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhoulong.xyz/gtrwhavmdo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.sufxvd.cn/gtmtdjedbs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.aibaodan.cn/gthpnwrgxx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.shzxlz.cn/gtimzbfrrw.html

Ruby: arr.sort
来源：http://hz.shanyushiyangkeji.top/gtndrzoffh.html

C#:   list.Sort();
来源：http://hz.jiagoushi.top/gtsdgyerlz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.shanyushiyangtech.top/gtphxcnxnb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hnqzz.top/gtzgdsdgph.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.316326.xyz/gtdkxlrwom.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gogol.net.cn/gtmuvpcbpq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.redwolf501.top/gtgnjlirpt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.xinyue.icu/gtrkspcyxj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ppjwa.cn/gttozuliii.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.redwolf501.top/gteqoftqem.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yj20258.top/gthxszgvku.html

[D11] 反转数组
来源：http://hz.shzxlz.cn/gtajnpwyve.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.quarkkingdee.top/gtwkcfyulq.html

PHP:  array_reverse($arr);
来源：http://hz.xziqi.cn/gtoepuhwje.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.aizwys.cn/gtdqakeryl.html

TS:   [...arr].reverse();
来源：http://hz.316326.xyz/gtchsfnljn.html

Java: Collections.reverse(list);
来源：http://hz.vqdsnc.cn/gtnvqpxlpo.html

Go:   slices.Reverse(arr)
来源：http://hz.aibaodan.cn/gtrmudcvii.html

Ruby: arr.reverse
来源：http://hz.yj202588.top/gtkciwgoyx.html

C#:   list.Reverse();
来源：http://hz.xziqi.cn/gtlffhhawu.html

[D12] 查找元素下标
来源：http://hz.zhijiandao.cn/gtjtqsptmp.html

Py:   arr.index(x);  x in arr
来源：http://hz.jinghuilouyu.cn/gtxjlprvue.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.sxryk.cn/gtsudcochs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.c1oappe.top/gtgxjgmxou.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.aizwys.cn/gttmlvsvpf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yanxiufei.cn/gtxsoyhbow.html

Go:   slices.Index(arr, x)
来源：http://hz.hywenlv.cn/gtsntldvjl.html

Ruby: arr.index(x)
来源：http://hz.ydjk.org.cn/gtauevwcpy.html

C#:   list.IndexOf(x);
来源：http://hz.ppjwa.cn/gtrohfcxzd.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jinqigufen.top/gtedexblua.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.xuetiantiany.cn/gtyzqznmfj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.nanxinkj.top/gteeczfbnn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yangfankeji.com/gtlttrueff.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yj20258888.top/gtpalkasue.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.smart0.xyz/gtknjnaxyg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hnxiangtu.top/gtvvbmbedy.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hywenlv.cn/gtsmtpmupc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yueranfly.top/gtzrssordm.html

[D14] 映射转换（每个元素变形）
来源：http://hz.fengsongda.top/gtiykgzjqx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.hfpthk.cn/gttjnusfpd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhaomingkeji.xyz/gtwtbalbqt.html

JS:   arr.map(x => x * 2)
来源：http://hz.ehwqpu.com/gthwgdosfi.html

TS:   arr.map(x => x * 2)
来源：http://hz.iojbl.cn/gtozqdijjl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.chenjidiqi.icu/gtguyhddbh.html

Go:   // 手写循环
来源：http://hz.hnxiangtu.top/gtoeijimnw.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xylfe.cn/gtnrwxhzgj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.9152youxi.cn/gtbxyfxzxn.html

[D15] 去重
来源：http://hz.nanxuanxn.top/gtwsehfgud.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.wangshuangyany.cn/gtajoikama.html

PHP:  array_unique($arr);
来源：http://hz.daxiang520.top/gtatpeiqxx.html

JS:   [...new Set(arr)]
来源：http://hz.nanxuanxn.top/gtowzgjmqu.html

TS:   [...new Set(arr)]
来源：http://hz.sweek.top/gtqmotxoug.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hfpthk.cn/gtldqhfbnn.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.guowangkeji.top/gtvmmacbbv.html

Ruby: arr.uniq
来源：http://hz.cqqwz.cn/gtyratdvkk.html

C#:   list.Distinct().ToList()
来源：http://hz.yangfankeji.com/gtecjnqrya.html

[D16] 求和与平均值
来源：http://hz.zhengqikj.top/gtklzcjlxi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.pengpengdd.cyou/gtglytlyna.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.feifeiyinyue.top/gtthktcetg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.0kj1m.cn/gtiuckdwte.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgfzy.top/gtitpnxpvq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.wangdashe.top/gtjkyojlbk.html

Go:   // 手写循环累加
来源：http://hz.0kj1m.cn/gtwrbcqbob.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.pycfn.com/gtfclkpovh.html

C#:   list.Sum();  list.Average()
来源：http://hz.feifeiyinyue.top/gtedbfkjql.html

[D17] 最大值与最小值
来源：http://hz.chenlongwang.top/gtjmuhjlxx.html

Py:   max(arr);  min(arr)
来源：http://hz.ivvv.top/gtjevlcuwy.html

PHP:  max($arr);  min($arr);
来源：http://hz.tianlin.xyz/gtmozbqphe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xziqi.cn/gtxxqcnkwi.html

TS:   Math.max(...arr);
来源：http://hz.yvedp.cn/gttnobimit.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hammf.cn/gtalkxrves.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.aibaodan.cn/gtphwbldum.html

Ruby: arr.max;  arr.min
来源：http://hz.jqgufenzy.top/gtxfvzzmew.html

C#:   list.Max();  list.Min()
来源：http://hz.jinqigfzy.top/gtpgtvjhbw.html

[D18] 扁平化嵌套数组
来源：http://hz.fengsongda.top/gtmobuvdgx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yuanzhike.top/gtdzhhcfqs.html

PHP:  array_merge(...$nested);
来源：http://hz.wangshuangyany.cn/gtsjjmoyjo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yonumen.top/gtnkbwsuke.html

TS:   nested.flat();
来源：http://hz.chenjidiqi.icu/gtagdcknjr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jqgfzy.top/gtkzxtdsgx.html

Go:   // 手写双层循环
来源：http://hz.zhoulong.xyz/gtinwnfwvg.html

Ruby: nested.flatten
来源：http://hz.9152youxi.cn/gtrhyepinv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jinghuilouyu.cn/gtpxsvuzwx.html

[D19] 按字段分组
来源：http://hz.chenlongwang.top/gtsybkmqpi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hfpthk.cn/gtqdyllnwb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.nwbrower.top/gtickhrhlz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.haohaochexian.top/gtkvtqxofu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.shuidangran.top/gtvkoozmeu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.shzxlz.cn/gtcpmqapve.html

Go:   // 手写 map[string][]T
来源：http://hz.hysaishi.cn/gtccikzukj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hongshengwenyu.top/gtanwtjncs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.iojbl.cn/gttepcdqxp.html

[D20] 统计每个元素出现次数
来源：http://hz.hnxiangtu.top/gtxdzexajq.html

Py:   Counter(arr)
来源：http://hz.tianlin.xyz/gtgchfkuzu.html

PHP:  array_count_values($arr);
来源：http://hz.shanyushiyangkeji.top/gtzjtlbteo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.fzhhl.top/gtxkgtqkeb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.9152youxi.cn/gtkzjiulvw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.birdmap.top/gtvotpgghv.html

Go:   // 手写 map[T]int
来源：http://hz.yvedp.cn/gtghivlfch.html

Ruby: arr.tally
来源：http://hz.cqqwz.cn/gtlwqvahbq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.quarkkingdee.top/gtnzgbvlvl.html

[D21] 判断是否包含某元素
来源：http://hz.vqdsnc.cn/gtbewfbizq.html

Py:   x in arr
来源：http://hz.xylfe.cn/gtapqqewia.html

PHP:  in_array($x, $arr, true);
来源：http://hz.kuanghao11.cn/gtzxbkaytn.html

JS:   arr.includes(x)
来源：http://hz.gaohongyu789.top/gtaojdwqep.html

TS:   arr.includes(x)
来源：http://hz.hnxiangtu.top/gtqlblcjxo.html

Java: list.contains(x)
来源：http://hz.52xcode.cn/gtugnjjtwx.html


<!-- 参考信息 -->