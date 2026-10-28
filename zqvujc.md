代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://hz.yongpay.top/gtmadsakrl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://hz.hnqzz.top/gtnhsmlapy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://hz.shuidangran.top/gtjpsbzqlz.html

Java: // 无：用 Builder 模式或 record
来源：http://hz.andypj.xyz/gtzqveoyfd.html

Go:   // 无：用配置结构体参数
来源：http://hz.jianghu66.top/gtytavrlyh.html

Ruby: f(a: 1, b: 2)
来源：http://hz.yj202588.top/gtrdjfgxxt.html

C#:   f(a: 1, b: 2)
来源：http://hz.zhixingplan.top/gtjghytydu.html

[C05] 返回多个值
来源：http://hz.jqgufenzy.top/gtdanpojzb.html

Py:   return a, b
来源：http://hz.hywenlv.cn/gtmswmblzk.html

PHP:  return [$a, $b];
来源：http://hz.yuxming.cn/gtyazfypdl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.zhijiandao.cn/gtoezpwzdv.html

TS:   return { a, b };
来源：http://hz.havefunace.top/gtznmxvqfi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.sxryk.cn/gtemqtexzg.html

Go:   return a, b
来源：http://hz.nwbrower.top/gtmrfgfnnx.html

Ruby: return a, b
来源：http://hz.52xcode.cn/gtdjsugobr.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zhoulong.xyz/gtnadpxdmc.html

[C06] 匿名函数 / lambda
来源：http://hz.bjfxy.top/gthnutoikt.html

Py:   square = lambda x: x * x
来源：http://hz.tian-w.cn/gtikziixkk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.chenlongwang.top/gtulglgokk.html

JS:   const square = x => x * x;
来源：http://hz.wangshuangyany.cn/gtfciblhet.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.redwolf501.top/gtxuaaxgfj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.xylfe.cn/gtxrzpnjue.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.pycfn.com/gtxqqgsefm.html

Ruby: square = ->(x) { x * x }
来源：http://hz.sweek.top/gtxgrupowx.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.jianghu66.top/gtezwjemxr.html

[C07] 把函数作为参数传入
来源：http://hz.meibo888.top/gtqwqklfdb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.gogol.net.cn/gtcgyimudc.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.wangdashe.top/gtfhytiaap.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.yonumen.top/gtfzoahzit.html

TS:   arr.map(String)
来源：http://hz.fzhhl.top/gtsukszkjy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.gotoacloud.top/gtquebhkjf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.hywenlv.cn/gtalooavxb.html

Ruby: arr.map(&:upcase)
来源：http://hz.xziqi.cn/gttzidzxym.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.jqgfzy.top/gtriahzhgy.html

[C08] 闭包
来源：http://hz.sweek.top/gtjzejsfdk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.zycfv.cn/gtxbqjkwif.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.meibo888.top/gtlcbpnnrn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.cheryme.top/gtwmordnvi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.cheryme.top/gtglvztpqy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.yj20258.top/gtxmosacoc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.cucudq.cn/gtuuzopwqu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.shanyushiyangkeji.top/gtpzhmxrrj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.hammf.cn/gtqqnmvpjm.html

[C09] 递归
来源：http://hz.iojbl.cn/gtvkswpvhk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.gotoacloud.top/gtvzaslifw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.zhiwuduotai.top/gtcqokzymm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.hnxiangtu.top/gtxlcayeux.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhiwuduotai.top/gtjeiyjniu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.hfpthk.cn/gtxhwgktxw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.ydjk.org.cn/gttcxianvd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.svipenyu.cn/gtmyyrighy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.svipenyu.cn/gtggyzjhmg.html

[C10] 变量作用域
来源：http://hz.yanxiufei.cn/gtzpajnofg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.sysykeji.top/gtxqezvaiq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yueranfly.top/gtesybjhka.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ydjk.org.cn/gtgocvjkau.html

TS:   同 JS
来源：http://hz.bjfxy.top/gtlpwnkijn.html

Java: 方法内为块级作用域
来源：http://hz.cheryme.top/gtjzgobksj.html

Go:   花括号块级作用域
来源：http://hz.cqqwz.cn/gtogmbszil.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.xuetiantiany.cn/gtdiejutge.html

C#:   块级作用域
来源：http://hz.hnxiangtu.top/gtqwlborqh.html

[C11] 模块导入与导出
来源：http://hz.snrcjt.cn/gtnnyatnas.html

Py:   from module import func
来源：http://hz.sufxvd.cn/gtgrncmgfg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.haohaochexian.top/gtvccrtaye.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.iojbl.cn/gtjcvzgfjk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.daria6918.cn/gtqzbupzzw.html

Java: import java.util.List;
来源：http://hz.yvedp.cn/gtpfbofqxu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.jinghuilouyu.cn/gtpihxnhhr.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.zhijiandao.cn/gtbqrhkkju.html

C#:   using System.Text;
来源：http://hz.pengpengdd.cyou/gtjxvtbrar.html

[C12] 立即执行函数 IIFE
来源：http://hz.hammf.cn/gtpsxafosn.html

Py:   (lambda: print("run"))()
来源：http://hz.hysaishi.cn/gtdpfusftw.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yj202588.top/gtjckfrqaj.html

JS:   (() => { console.log("run"); })();
来源：http://hz.guannengcc.top/gttytqfncg.html

TS:   (() => { console.log("run"); })();
来源：http://hz.zhongyouzk.top/gtkwwpyqzw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jinghuilouyu.cn/gtjsodddyp.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shzxlz.cn/gtmuoeywjx.html

Ruby: -> { puts "run" }.call
来源：http://hz.svipenyu.cn/gtenyetyvn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.c1oappe.top/gtepynqipd.html

[C13] 类型声明 / 类型注解
来源：http://hz.cashguo.top/gtunlwtobj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.dashuyun.cn/gtgmcsmtpd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hywenlv.cn/gtlhcscfgs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yueranfly.top/gtbbnfrfrz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xuetiantiany.cn/gtctyrgbzs.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cdnleiting.top/gtvkjzvfqb.html

Go:   func add(a, b int) int
来源：http://hz.hongshengwenyu.top/gtjtvcyqzx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jinqigufen.top/gtclolonuy.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jqgfzy.top/gtpfxtnijr.html

[C14] 泛型函数
来源：http://hz.shangyingyoupin.top/gtlbtjqyqd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.nanxuanxn.top/gtlfajpjjh.html

PHP:  // 无泛型
来源：http://hz.meibo888.top/gtmiedgkyn.html

JS:   // 无泛型
来源：http://hz.kuanghao11.cn/gtjogvcqde.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yongpay.top/gtvdzbeqgp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.aizwys.cn/gtfqhktrby.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.nanxuanxn.top/gtfwsdhicw.html

Ruby: # 无泛型
来源：http://hz.yueranfly.top/gtxtargrta.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.shanyushiyangkeji.top/gtqgwuxqry.html

[C15] 解构 / 展开参数
来源：http://hz.pycfn.com/gtainwhrhv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.tian-w.cn/gtlglkcmor.html

PHP:  [$a, $b] = $pair;
来源：http://hz.kuanghao11.cn/gteoowrxwt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.shangyingyoupin.top/gtrgvmioll.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.aibaodan.cn/gtpdxoupcv.html

Java: // 无解构
来源：http://hz.yueranfly.top/gtseoahtgp.html

Go:   // 无解构
来源：http://hz.daria6918.cn/gtyheptzgd.html

Ruby: a, b = pair
来源：http://hz.hammf.cn/gtuwrfnovm.html

C#:   var (a, b) = pair;
来源：http://hz.vqdsnc.cn/gtmkvnmwfr.html

[C16] 函数 / 方法重载
来源：http://hz.cheryme.top/gtytbnhnde.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jqgufenzy.top/gtccxyohlx.html

PHP:  // 无重载
来源：http://hz.chenlongwang.top/gtbdmaltan.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.nanxuanxn.top/gtktbooeqs.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhixingplan.top/gtcywjurzc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.ydzc1.top/gtomzqlpxw.html

Go:   // 无重载：用不同函数名
来源：http://hz.jinqigufen.top/gtusnvqrvp.html

Ruby: # 无重载：靠动态参数
来源：http://hz.tanke756.top/gtvtxhnqtn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jianghu66.top/gtegdbzlia.html

================================================================================
来源：http://hz.ppjwa.cn/gtwdmyloil.html

D. 数组 / 列表 / 集合
来源：http://hz.tanke756.top/gtnmdhflep.html

================================================================================
来源：http://hz.havefunace.top/gtkstbzbnw.html

[D01] 创建数组 / 列表
来源：http://hz.hywenlv.cn/gtbmnniwms.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.cdnleiting.top/gturxyahtj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.havefunace.top/gtxuwospcs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yonumen.top/gtdpjgjsft.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.shzxlz.cn/gtghppevgo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.nanxinkj.top/gtrjbyufwt.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.haohaochexian.top/gtgismncbx.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhijiandao.cn/gthjfhueux.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jqgufenzy.top/gtirqpauce.html

[D02] 追加元素到末尾
来源：http://hz.andypj.xyz/gtmdocscnz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.smart0.xyz/gtikvuqlej.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhongyouzk.top/gtwcvjiddf.html

JS:   arr.push(4);
来源：http://hz.feifeiyinyue.top/gtzdqxfseo.html

TS:   arr.push(4);
来源：http://hz.pycfn.com/gtijjdqldi.html

Java: list.add(4);
来源：http://hz.redwolf501.top/gtezhqrjlz.html

Go:   arr = append(arr, 4)
来源：http://hz.316326.xyz/gtdongtvqr.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.xingfuxueyuan.xyz/gtcapfchmm.html

C#:   list.Add(4);
来源：http://hz.nwbrower.top/gtyfwtjlbn.html

[D03] 在指定位置插入元素
来源：http://hz.wangshuangyany.cn/gtolexgopq.html

Py:   arr.insert(0, 0)
来源：http://hz.dashuyun.cn/gtrpzffoay.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yongpay.top/gtjugvdbfs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jqgfzy.top/gtrdtvqqua.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.ydjk.org.cn/gtczjexxhm.html

Java: list.add(0, 0);
来源：http://hz.zycfv.cn/gtdpnbfszn.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.vqdsnc.cn/gteidszkzf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.quarkkingdee.top/gtanduitro.html

C#:   list.Insert(0, 0);
来源：http://hz.zycfv.cn/gtljfrjnzq.html

[D04] 删除元素
来源：http://hz.feifeiyinyue.top/gtrqjrsotv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.havefunace.top/gttytaqain.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.xingfuxueyuan.xyz/gtkqmmyncn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.0kj1m.cn/gtmuiqgjoy.html

TS:   arr.splice(0, 1);
来源：http://hz.yj20258888.top/gtpirdmxpy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.haohaochexian.top/gtrsbxclvd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.gzhubu.top/gtzophzxjh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.mhx1999.top/gtcbrxomor.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xziqi.cn/gtvxibdvas.html

[D05] 访问与修改元素
来源：http://hz.svipenyu.cn/gtgavfiycr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.chenzaomai.com/gtwdhkthul.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.fzhhl.top/gtsgtjytvp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hysaishi.cn/gthjruskbo.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.0kj1m.cn/gtobehzkng.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.316326.xyz/gtcauahvvu.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.tanke756.top/gtjkrgyhav.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.daxiang520.top/gtagutryvd.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yuanzhike.top/gtrilgvdgn.html

[D06] 数组长度
来源：http://hz.jqgufenzy.top/gtukglztfa.html

Py:   len(arr)
来源：http://hz.yanxiufei.cn/gttfbjmslr.html

PHP:  count($arr);
来源：http://hz.0kj1m.cn/gtaahztbnw.html

JS:   arr.length
来源：http://hz.hongshengwenyu.top/gtpyoxmyae.html

TS:   arr.length
来源：http://hz.wangdashe.top/gtwqmxfwoz.html

Java: list.size();
来源：http://hz.9152youxi.cn/gtucdkpown.html

Go:   len(arr)
来源：http://hz.chenzaomai.com/gttqtijwko.html

Ruby: arr.length; arr.size
来源：http://hz.jqgfzy.top/gtxdzcquxs.html

C#:   list.Count;
来源：http://hz.zhengqikj.top/gtbkpfnmgi.html

[D07] 切片 / 取子数组
来源：http://hz.fzhhl.top/gtbwxxvcnw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yvedp.cn/gtcbdxjebz.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.cashguo.top/gtvutuazvn.html

JS:   arr.slice(1, 4);
来源：http://hz.fengsongda.top/gtxafwtlbk.html

TS:   arr.slice(1, 4);
来源：http://hz.svipenyu.cn/gtxjjvohxy.html

Java: list.subList(1, 4);
来源：http://hz.hammf.cn/gtmrcrqzlh.html

Go:   arr[1:4]
来源：http://hz.xinyue.icu/gtbadkousz.html

Ruby: arr[1, 3]
来源：http://hz.shuidangran.top/gtvhutywaa.html

C#:   list.GetRange(1, 3);
来源：http://hz.ydjk.org.cn/gttzahfytr.html

[D08] 合并两个数组
来源：http://hz.shuidangran.top/gtijgtnbmg.html

Py:   a + b;  a.extend(b)
来源：http://hz.shuidangran.top/gtthpjvqwk.html

PHP:  array_merge($a, $b);
来源：http://hz.52xcode.cn/gtyafkcyxk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xuanzx.com/gtqltnvgrk.html

TS:   [...a, ...b];
来源：http://hz.redwolf501.top/gtgsjjfpbf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xuanzx.com/gtsshbzglr.html

Go:   append(a, b...)
来源：http://hz.jinyuanbaomall.cn/gtzyhypisz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.fengsongda.top/gtahpekilx.html

C#:   a.Concat(b).ToList()
来源：http://hz.shanyushiyangkeji.top/gtquipfeom.html

[D09] 排序（升序）
来源：http://hz.shanyushiyangtech.top/gtmqrqvdyz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cdnleiting.top/gtangwjxpg.html

PHP:  sort($arr);
来源：http://hz.nanxuanxn.top/gtrcqasyzu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.dashuyun.cn/gtbebmwcpz.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.feifeiyinyue.top/gtpysawosp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shanyushiyangkeji.top/gtcarzhkyi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jinqigfzy.top/gtenkonzyk.html

Ruby: arr.sort
来源：http://hz.daxiang520.top/gtokzkpxyi.html

C#:   list.Sort();
来源：http://hz.316326.xyz/gthdnkqsfe.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.vqdsnc.cn/gtzvqkjhkg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xuanzx.com/gtvboxlbgt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zycfv.cn/gtwrdgqbjq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.haohaochexian.top/gtdurilmnp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.haohaochexian.top/gtsnbyoqfv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.meibo888.top/gtqquhgaln.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.nanxuanxn.top/gtxfesafxv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.sufxvd.cn/gtqoygfvfk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zdqjudy.top/gthovdlapd.html

[D11] 反转数组
来源：http://hz.tian-w.cn/gtixxvbess.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shanyushiyangkeji.top/gtphbjggbw.html

PHP:  array_reverse($arr);
来源：http://hz.ehwqpu.com/gtzogfpick.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.snrcjt.cn/gtnlidensy.html

TS:   [...arr].reverse();
来源：http://hz.birdmap.top/gtphonvicx.html

Java: Collections.reverse(list);
来源：http://hz.0kj1m.cn/gthitywlkp.html

Go:   slices.Reverse(arr)
来源：http://hz.mhx1999.top/gtghxqjkte.html

Ruby: arr.reverse
来源：http://hz.zhaomingkeji.xyz/gtnwhddsjy.html

C#:   list.Reverse();
来源：http://hz.hnxiangtu.top/gtcixvzlrk.html

[D12] 查找元素下标
来源：http://hz.ydzc1.top/gtvsiqpeez.html

Py:   arr.index(x);  x in arr
来源：http://hz.yj202588.top/gtvhbvmvbj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.nanxuanxn.top/gttvhcqkgn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj202588.top/gtfrlniclg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinghuilouyu.cn/gtumvplure.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.andypj.xyz/gtzojehzwe.html

Go:   slices.Index(arr, x)
来源：http://hz.jinghuilouyu.cn/gtkatgcqrq.html

Ruby: arr.index(x)
来源：http://hz.ybcxt.top/gtccyqfhgk.html

C#:   list.IndexOf(x);
来源：http://hz.pycfn.com/gtqdlfdfbd.html

[D13] 过滤（保留满足条件的）
来源：http://hz.gogol.net.cn/gtnpxwycns.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.redwolf501.top/gtjyrtwvuv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yongpay.top/gtzkhqwhuj.html

JS:   arr.filter(x => x > 3)
来源：http://hz.smart0.xyz/gtrhgihtqc.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ppjwa.cn/gtaqipovjl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shanyushiyangtech.top/gtdxekwpuu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hywenlv.cn/gtmvfnpbyu.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yuanzhike.top/gtklvggmjd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jiagoushi.top/gtatfmsahy.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhongyouzk.top/gttslsrfvj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.daxiang520.top/gtravhuwvs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.haohaochexian.top/gtqlmrifua.html

JS:   arr.map(x => x * 2)
来源：http://hz.yj20258888.top/gtqiolktnv.html

TS:   arr.map(x => x * 2)
来源：http://hz.cashguo.top/gtydnmemgp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cucudq.cn/gtmeufkexm.html

Go:   // 手写循环
来源：http://hz.hfpthk.cn/gtgwogtsyy.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.9152youxi.cn/gtyyzelpvc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xuanzx.com/gtgsucydmc.html

[D15] 去重
来源：http://hz.hnxiangtu.top/gtuskzyxaf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hnxiangtu.top/gtkamvakdg.html

PHP:  array_unique($arr);
来源：http://hz.redwolf501.top/gtaeqvcama.html

JS:   [...new Set(arr)]
来源：http://hz.zhengqikj.top/gtjjcvrjeo.html

TS:   [...new Set(arr)]
来源：http://hz.chenzaomai.com/gtaxlyuqey.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hfpthk.cn/gtegstndqx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.daxiang520.top/gtqebhdhye.html

Ruby: arr.uniq
来源：http://hz.yangfankeji.com/gtnqmmdhem.html

C#:   list.Distinct().ToList()
来源：http://hz.svipenyu.cn/gtevwmzkvw.html

[D16] 求和与平均值
来源：http://hz.haohaochexian.top/gtrwiimlpl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.pengpengdd.cyou/gtdaxhqwxw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yj202588.top/gtzabsecwm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258.top/gtltaqgpfn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gaohongyu789.top/gtpblgajdu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.chenlongwang.top/gtuqxfkvsi.html

Go:   // 手写循环累加
来源：http://hz.jinqigfzy.top/gtugpeuani.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xuetiantiany.cn/gtmfyfxpwx.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhongyouzk.top/gtyjijeonq.html

[D17] 最大值与最小值
来源：http://hz.zhoulong.xyz/gtcqvhgain.html

Py:   max(arr);  min(arr)
来源：http://hz.nanxuanxn.top/gtsloaebuc.html

PHP:  max($arr);  min($arr);
来源：http://hz.hnqzz.top/gtneasizog.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhengqikj.top/gtnocrifnm.html

TS:   Math.max(...arr);
来源：http://hz.xinyue.icu/gtjtgjchbj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.dianchejie.cn/gtuktkszzd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.mhx1999.top/gticsonyky.html

Ruby: arr.max;  arr.min
来源：http://hz.nwbrower.top/gtdptxrzws.html

C#:   list.Max();  list.Min()
来源：http://hz.chenzaomai.com/gtsfltimpn.html

[D18] 扁平化嵌套数组
来源：http://hz.hysaishi.cn/gtcqczrpai.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zycfv.cn/gtvfergtoo.html

PHP:  array_merge(...$nested);
来源：http://hz.zhaomingkeji.xyz/gtzlkvneea.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ivvv.top/gtvxgjquwv.html

TS:   nested.flat();
来源：http://hz.hywenlv.cn/gtvxadxasg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.kuanghao11.cn/gtedvtdsvv.html

Go:   // 手写双层循环
来源：http://hz.sufxvd.cn/gtbsuwjsxn.html

Ruby: nested.flatten
来源：http://hz.ehwqpu.com/gtkghbhqgc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yongpay.top/gtfslnpyur.html

[D19] 按字段分组
来源：http://hz.nwbrower.top/gtmzjqiqqe.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.sxryk.cn/gtmdoacpjp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.tanke756.top/gtwixplltc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.andypj.xyz/gtnmjbkddl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yuxming.cn/gteotjpkpr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yonumen.top/gtbvvethfe.html

Go:   // 手写 map[string][]T
来源：http://hz.cdnleiting.top/gttrzborhx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.aibaodan.cn/gtxjfjvfao.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.vqdsnc.cn/gtcduyzbaw.html

[D20] 统计每个元素出现次数
来源：http://hz.zhengqikj.top/gtaafhdrkt.html

Py:   Counter(arr)
来源：http://hz.meibo888.top/gtsscalyak.html

PHP:  array_count_values($arr);
来源：http://hz.cheryme.top/gtlmhexpmf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.c1oappe.top/gtlbawshrp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gotoacloud.top/gtrzjrxwam.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.c1oappe.top/gtivtpqbew.html

Go:   // 手写 map[T]int
来源：http://hz.shzxlz.cn/gtqakghhsf.html

Ruby: arr.tally
来源：http://hz.zhiwuduotai.top/gtxihuphcz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yueranfly.top/gtfkepjokv.html

[D21] 判断是否包含某元素
来源：http://hz.shzxlz.cn/gtumaekbzm.html

Py:   x in arr
来源：http://hz.jyoumei.cn/gtwokuckmr.html


<!-- 参考信息 -->