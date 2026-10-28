代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.svipenyu.cn/gtbouvywnw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.tian-w.cn/gtqziejpay.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ydzc1.top/gtyidszgfw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.nanxuanxn.top/gttyqzbjia.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zycfv.cn/gtpbkdwfky.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.jqgufenzy.top/gtchjjlrsr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.dianchejie.cn/gtfkvwfbnn.html

[C09] 递归
来源：http://hz.yuanzhike.top/gthbeupumn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.hnxiangtu.top/gtbwlyfmwi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.hnxiangtu.top/gtubcomnbp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.shzxlz.cn/gtidllvilo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj20258888.top/gtlwtmpvsw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.tanke756.top/gtosuhjmjw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.shzxlz.cn/gtbbkxlaff.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.cheryme.top/gtiwqiqpdi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.kuanghao11.cn/gtdwppypew.html

[C10] 变量作用域
来源：http://hz.yj202588.top/gtwezcxmyy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.snrcjt.cn/gttfyvnrkq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zdqjudy.top/gtjrppsmjo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.shanyushiyangkeji.top/gtfyfstekq.html

TS:   同 JS
来源：http://hz.cqqwz.cn/gtrckywlnw.html

Java: 方法内为块级作用域
来源：http://hz.nanxuanxn.top/gtcnnamqfp.html

Go:   花括号块级作用域
来源：http://hz.kuanghao11.cn/gtdhzzmfzf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hnqzz.top/gtnrmkcjdg.html

C#:   块级作用域
来源：http://hz.andypj.xyz/gtrxormyxv.html

[C11] 模块导入与导出
来源：http://hz.zdqjudy.top/gtgjuwirwq.html

Py:   from module import func
来源：http://hz.daxiang520.top/gtnzvsprbe.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.quarkkingdee.top/gtvdaktury.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.birdmap.top/gtjnoryoio.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ybcxt.top/gtlmxnjxlx.html

Java: import java.util.List;
来源：http://hz.cucudq.cn/gtqpukrvbv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yj20258888.top/gtsgekiubp.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.cheryme.top/gtzbpxnpzk.html

C#:   using System.Text;
来源：http://hz.wangdashe.top/gtcdyiilcp.html

[C12] 立即执行函数 IIFE
来源：http://hz.yj20258888.top/gtonffoene.html

Py:   (lambda: print("run"))()
来源：http://hz.cdnleiting.top/gttixpxxtx.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jinyuanbaomall.cn/gtkrprctej.html

JS:   (() => { console.log("run"); })();
来源：http://hz.gogol.net.cn/gtigkaysna.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ehwqpu.com/gtehkrrtva.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jlsjyb.cn/gtyylevila.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.feifeiyinyue.top/gtfhuefzqz.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhoulong.xyz/gtbbiznwoh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.pengpengdd.cyou/gtbonioxge.html

[C13] 类型声明 / 类型注解
来源：http://hz.hnxiangtu.top/gtumnzqduq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.guannengcc.top/gtppvplmyn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinqigfzy.top/gtrbkbaytf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shuidangran.top/gtomolwzri.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.dashuyun.cn/gtpvtovlqi.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.daxiang520.top/gtpxncfszo.html

Go:   func add(a, b int) int
来源：http://hz.chenlongwang.top/gteonzcwwz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.fengsongda.top/gtsjblzuuh.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.fzhhl.top/gtlrgpaxcg.html

[C14] 泛型函数
来源：http://hz.havefunace.top/gtljohitme.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sxryk.cn/gtknouvbld.html

PHP:  // 无泛型
来源：http://hz.sufxvd.cn/gtgtxadted.html

JS:   // 无泛型
来源：http://hz.tanke756.top/gtpqnfulhr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.gzhubu.top/gtgpyrkwsh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.ivvv.top/gtzqwlotst.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.shuidangran.top/gtkctcmjdf.html

Ruby: # 无泛型
来源：http://hz.jqgufenzy.top/gtdffoqbfe.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.xinyue.icu/gtkxmbowjz.html

[C15] 解构 / 展开参数
来源：http://hz.yj20258.top/gtrpmkxntu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cheryme.top/gtyzqlkyam.html

PHP:  [$a, $b] = $pair;
来源：http://hz.dianchejie.cn/gtncszlbsi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xinyue.icu/gtrtmlypjb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.sweek.top/gtveoycwws.html

Java: // 无解构
来源：http://hz.9152youxi.cn/gtawbkwike.html

Go:   // 无解构
来源：http://hz.yueranfly.top/gtbuhqoqzx.html

Ruby: a, b = pair
来源：http://hz.yj20258.top/gtmntsuyfh.html

C#:   var (a, b) = pair;
来源：http://hz.9152youxi.cn/gttgjiyovw.html

[C16] 函数 / 方法重载
来源：http://hz.svipenyu.cn/gtnwzvxohv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.nanxuanxn.top/gtzghjibgc.html

PHP:  // 无重载
来源：http://hz.sweek.top/gtzivsdmga.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.yuxming.cn/gtjhoapsqo.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.haohaochexian.top/gtefyzlbfx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.hysaishi.cn/gtnjlimmnx.html

Go:   // 无重载：用不同函数名
来源：http://hz.shzxlz.cn/gtvyugeaqt.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ppjwa.cn/gtlaqyzlxh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hnxiangtu.top/gtcvidqzjy.html

================================================================================
来源：http://hz.gotoacloud.top/gtckirathd.html

D. 数组 / 列表 / 集合
来源：http://hz.sufxvd.cn/gttvfnfoog.html

================================================================================
来源：http://hz.shzxlz.cn/gtwzjpfafs.html

[D01] 创建数组 / 列表
来源：http://hz.xuetiantiany.cn/gtnhruxnxs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yongpay.top/gtiyzkrlfp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.zhoulong.xyz/gtlcnoroia.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhiwuduotai.top/gtpokylrdj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.9152youxi.cn/gtcrxvdlde.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhoulong.xyz/gtvtebdbgr.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.havefunace.top/gtuucshtwg.html

Ruby: arr = [1, 2, 3]
来源：http://hz.9152youxi.cn/gtmiwwnzsr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jianghu66.top/gtfvjilntr.html

[D02] 追加元素到末尾
来源：http://hz.ehwqpu.com/gtlzortewb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhijiandao.cn/gtverqgkyr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.bjfxy.top/gtodwcsrpe.html

JS:   arr.push(4);
来源：http://hz.svipenyu.cn/gthkoahggx.html

TS:   arr.push(4);
来源：http://hz.hysaishi.cn/gtlzzsnlkm.html

Java: list.add(4);
来源：http://hz.jyoumei.cn/gttjgdlzdb.html

Go:   arr = append(arr, 4)
来源：http://hz.shuidangran.top/gtovoryfbz.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.quarkkingdee.top/gtcaitfphn.html

C#:   list.Add(4);
来源：http://hz.zhixingplan.top/gtigjfhjjw.html

[D03] 在指定位置插入元素
来源：http://hz.jinghuilouyu.cn/gtrdcygpte.html

Py:   arr.insert(0, 0)
来源：http://hz.hywenlv.cn/gtmsbsplkc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.pengpengdd.cyou/gtpazqyjvr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.cqqwz.cn/gtfhkvmtqf.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yvedp.cn/gtffdtxrwr.html

Java: list.add(0, 0);
来源：http://hz.ydjk.org.cn/gtdhzxffre.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.ydzc1.top/gtuoukeqjr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.aibaodan.cn/gtpnziqlbd.html

C#:   list.Insert(0, 0);
来源：http://hz.jianghu66.top/gtfrekpkyy.html

[D04] 删除元素
来源：http://hz.cheryme.top/gtzlnprfip.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.gotoacloud.top/gtuzybjpip.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jinqigfzy.top/gtsbfolfwv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.gzhubu.top/gtyzteaznl.html

TS:   arr.splice(0, 1);
来源：http://hz.ehwqpu.com/gtcqholrfu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ydzc1.top/gtolliklms.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.jyoumei.cn/gtshljlgal.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.dianchejie.cn/gttcmrrjhr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hnqzz.top/gtpagfkbyn.html

[D05] 访问与修改元素
来源：http://hz.xuanzx.com/gtzhejorio.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.9152youxi.cn/gtpdrsbufp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yonumen.top/gtdfxisvrv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cdnleiting.top/gtzkeyicne.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.chenjidiqi.icu/gtenlkhcwm.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.nwbrower.top/gtaqlanutz.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.smart0.xyz/gtldogzkfa.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhijiandao.cn/gtppwfkzkn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.pycfn.com/gtbkiiarhd.html

[D06] 数组长度
来源：http://hz.ppjwa.cn/gtqlfpbrot.html

Py:   len(arr)
来源：http://hz.ywan-chungtsiang.top/gtmrrdwfcg.html

PHP:  count($arr);
来源：http://hz.yj202588.top/gtmocviihg.html

JS:   arr.length
来源：http://hz.yj202588.top/gtazdplrsl.html

TS:   arr.length
来源：http://hz.xziqi.cn/gthttleixn.html

Java: list.size();
来源：http://hz.9152youxi.cn/gtegkdkhzy.html

Go:   len(arr)
来源：http://hz.andypj.xyz/gtotzbkbqn.html

Ruby: arr.length; arr.size
来源：http://hz.hysaishi.cn/gttkuwxryn.html

C#:   list.Count;
来源：http://hz.gzhubu.top/gtklofghcc.html

[D07] 切片 / 取子数组
来源：http://hz.yj20258888.top/gtcnuxrhev.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhoulong.xyz/gtnihjjnyz.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.aibaodan.cn/gtfucmwyey.html

JS:   arr.slice(1, 4);
来源：http://hz.jqgfzy.top/gtcfdycsea.html

TS:   arr.slice(1, 4);
来源：http://hz.meibo888.top/gtvkapfnow.html

Java: list.subList(1, 4);
来源：http://hz.hfpthk.cn/gtcfwmfivw.html

Go:   arr[1:4]
来源：http://hz.zhongyouzk.top/gtxfalpizn.html

Ruby: arr[1, 3]
来源：http://hz.guowangkeji.top/gttjkststi.html

C#:   list.GetRange(1, 3);
来源：http://hz.shuidangran.top/gthoeupjyj.html

[D08] 合并两个数组
来源：http://hz.zhoulong.xyz/gtgaoevyvz.html

Py:   a + b;  a.extend(b)
来源：http://hz.ybcxt.top/gtdyylbbaz.html

PHP:  array_merge($a, $b);
来源：http://hz.gaohongyu789.top/gtbbqxkkhg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jqgufenzy.top/gtynsblfsy.html

TS:   [...a, ...b];
来源：http://hz.ehwqpu.com/gtuautpinq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shanyushiyangtech.top/gttresnkga.html

Go:   append(a, b...)
来源：http://hz.feifeiyinyue.top/gtldtmdaif.html

Ruby: a + b;  a.concat(b)
来源：http://hz.snrcjt.cn/gtvhpfxrfu.html

C#:   a.Concat(b).ToList()
来源：http://hz.nanxuanxn.top/gtoxwaaxfu.html

[D09] 排序（升序）
来源：http://hz.hfpthk.cn/gtfvbqgthb.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sxryk.cn/gtkxofgxmn.html

PHP:  sort($arr);
来源：http://hz.jinghuilouyu.cn/gtqrimxhuq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.yueranfly.top/gtvbctjydb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ydjk.org.cn/gtdppcgooc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cashguo.top/gtnwuiyetq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ybcxt.top/gtxldleqvt.html

Ruby: arr.sort
来源：http://hz.haohaochexian.top/gtvhajkmyt.html

C#:   list.Sort();
来源：http://hz.xinyue.icu/gtmmhkpvmn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zdqjudy.top/gtqyqjahmf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.gaohongyu789.top/gtwmlbzlyr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hfpthk.cn/gtgapvuarl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.aizwys.cn/gtngkcvmhv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zdqjudy.top/gtnkaytyvn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yvedp.cn/gtzyxsrbsa.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.gaohongyu789.top/gtqcvcosxh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ydzc1.top/gtucppycut.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.316326.xyz/gtclnqhlsy.html

[D11] 反转数组
来源：http://hz.xziqi.cn/gtesguqnvc.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhijiandao.cn/gtpbikmkfk.html

PHP:  array_reverse($arr);
来源：http://hz.xziqi.cn/gtnmnbkpbb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yueranfly.top/gtztiuoits.html

TS:   [...arr].reverse();
来源：http://hz.yongpay.top/gtoxcviscs.html

Java: Collections.reverse(list);
来源：http://hz.jlsjyb.cn/gtmkxdvuod.html

Go:   slices.Reverse(arr)
来源：http://hz.c1oappe.top/gtsvljnijt.html

Ruby: arr.reverse
来源：http://hz.ppjwa.cn/gtcnbzzaft.html

C#:   list.Reverse();
来源：http://hz.iojbl.cn/gtlgflihcr.html

[D12] 查找元素下标
来源：http://hz.ywan-chungtsiang.top/gtmyegviup.html

Py:   arr.index(x);  x in arr
来源：http://hz.aibaodan.cn/gttxfclbwo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jqgufenzy.top/gtlmbkjvzs.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cashguo.top/gtcfqypuyk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhijiandao.cn/gtehmkkhig.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.316326.xyz/gtywgqayfh.html

Go:   slices.Index(arr, x)
来源：http://hz.ydjk.org.cn/gtyhxcgfnn.html

Ruby: arr.index(x)
来源：http://hz.hywenlv.cn/gtrjlogupz.html

C#:   list.IndexOf(x);
来源：http://hz.mhx1999.top/gtuwjahbax.html

[D13] 过滤（保留满足条件的）
来源：http://hz.sweek.top/gtzpavrbbv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yuxming.cn/gtqfolwbli.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hnqzz.top/gtbtlfbxqc.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hnqzz.top/gthxtzrsxv.html

TS:   arr.filter(x => x > 3)
来源：http://hz.pycfn.com/gtpvbboqwj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sxryk.cn/gtkmvjlgib.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ywan-chungtsiang.top/gtrvzbyirx.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ywan-chungtsiang.top/gtizdfkjvb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.gotoacloud.top/gtnmtonrci.html

[D14] 映射转换（每个元素变形）
来源：http://hz.guowangkeji.top/gtbldhixek.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.meibo888.top/gtdqgyiehg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hnxiangtu.top/gtlvguspxy.html

JS:   arr.map(x => x * 2)
来源：http://hz.bjfxy.top/gtvrjbskic.html

TS:   arr.map(x => x * 2)
来源：http://hz.chenlongwang.top/gtwphtaysv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.cqqwz.cn/gtrevczgft.html

Go:   // 手写循环
来源：http://hz.haohaochexian.top/gtnkphsxfs.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yvedp.cn/gtohrfldlf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.fzhhl.top/gtycslnlhu.html

[D15] 去重
来源：http://hz.zhijiandao.cn/gtadcmzrxa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ybcxt.top/gtmcyfaxly.html

PHP:  array_unique($arr);
来源：http://hz.jinqigfzy.top/gtylqssuru.html

JS:   [...new Set(arr)]
来源：http://hz.jiagoushi.top/gtxwqugxqq.html

TS:   [...new Set(arr)]
来源：http://hz.hfpthk.cn/gtvadsrkgs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jinyuanbaomall.cn/gtdrtjxytu.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yonumen.top/gtawaxella.html

Ruby: arr.uniq
来源：http://hz.daxiang520.top/gtlttdxdea.html

C#:   list.Distinct().ToList()
来源：http://hz.smart0.xyz/gtrmcuwvnc.html

[D16] 求和与平均值
来源：http://hz.smart0.xyz/gtekudrgni.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.gaohongyu789.top/gtcbsjudsa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yj20258888.top/gtxvkpulxh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhongyouzk.top/gtgopquwnu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258.top/gtbyebiaqy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sweek.top/gtekjghfhd.html

Go:   // 手写循环累加
来源：http://hz.shuidangran.top/gtzgzwfqxv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.pengpengdd.cyou/gtexuvjacd.html

C#:   list.Sum();  list.Average()
来源：http://hz.snrcjt.cn/gthnoqushb.html

[D17] 最大值与最小值
来源：http://hz.hongshengwenyu.top/gtiyazoage.html

Py:   max(arr);  min(arr)
来源：http://hz.xuetiantiany.cn/gtnptwokhc.html

PHP:  max($arr);  min($arr);
来源：http://hz.hnxiangtu.top/gtmojolchg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.quarkkingdee.top/gthhrjnycr.html

TS:   Math.max(...arr);
来源：http://hz.hnxiangtu.top/gtifdcqzqm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yanxiufei.cn/gtgymrmpsm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.chenzaomai.com/gtpivftbzs.html

Ruby: arr.max;  arr.min
来源：http://hz.vqdsnc.cn/gtmfefmymj.html

C#:   list.Max();  list.Min()
来源：http://hz.jyoumei.cn/gtgufunamf.html

[D18] 扁平化嵌套数组
来源：http://hz.ehwqpu.com/gtpkaskybn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.nanxinkj.top/gtxsjntffd.html

PHP:  array_merge(...$nested);
来源：http://hz.andypj.xyz/gtllbqgimz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xuanzx.com/gtgizoqqap.html

TS:   nested.flat();
来源：http://hz.chenzaomai.com/gtqfjbbgxe.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yj202588.top/gtzhbuujrz.html

Go:   // 手写双层循环
来源：http://hz.zhiwuduotai.top/gtejsgsthz.html

Ruby: nested.flatten
来源：http://hz.zhiwuduotai.top/gttqwphipb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yuanzhike.top/gtmrwnoqav.html

[D19] 按字段分组
来源：http://hz.feifeiyinyue.top/gtghcviwib.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.aizwys.cn/gtmltxfmzq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cqqwz.cn/gtlnyrjrdx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yj20258.top/gttntttcrd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.aibaodan.cn/gtieylaalm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ydjk.org.cn/gtfkgxiglj.html

Go:   // 手写 map[string][]T
来源：http://hz.nanxuanxn.top/gtxhhokitl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gzhubu.top/gtxzphqsra.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cdnleiting.top/gtgddkorqb.html

[D20] 统计每个元素出现次数
来源：http://hz.yj20258888.top/gtvgvwltyh.html

Py:   Counter(arr)
来源：http://hz.havefunace.top/gtxioomlwu.html

PHP:  array_count_values($arr);
来源：http://hz.xinyue.icu/gtwxgfdxyh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hammf.cn/gtcyzbbhni.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhaomingkeji.xyz/gtkautzjwt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.sufxvd.cn/gtzqkgojkh.html

Go:   // 手写 map[T]int
来源：http://hz.c1oappe.top/gtnfhumgth.html

Ruby: arr.tally
来源：http://hz.cheryme.top/gtltexkuye.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yj20258.top/gtspanjqib.html

[D21] 判断是否包含某元素
来源：http://hz.yj202588.top/gthhhyjxra.html

Py:   x in arr
来源：http://hz.gotoacloud.top/gtvmjzvsmm.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ivvv.top/gttfekzmwm.html

JS:   arr.includes(x)
来源：http://hz.zycfv.cn/gtcchzammy.html

TS:   arr.includes(x)
来源：http://hz.hammf.cn/gtziaqeaeh.html

Java: list.contains(x)
来源：http://hz.quarkkingdee.top/gtsidktzet.html

Go:   slices.Contains(arr, x)
来源：http://hz.shuidangran.top/gthmuxrrqg.html

Ruby: arr.include?(x)
来源：http://hz.zhaomingkeji.xyz/gtsbnjnbyw.html

C#:   list.Contains(x)
来源：http://hz.zhengqikj.top/gtgjuhhkyg.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhijiandao.cn/gtykqqzdhv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yueranfly.top/gtivfaqqck.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhixingplan.top/gtvmysyxji.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ywan-chungtsiang.top/gthnujbfui.html

TS:   [...arr];
来源：http://hz.cashguo.top/gtwezzqiwj.html

Java: new ArrayList<>(list);
来源：http://hz.hfpthk.cn/gtoyncfzfi.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.gzhubu.top/gtxjqpwbtq.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jinghuilouyu.cn/gtmvwinvlt.html

C#:   new List<int>(list);
来源：http://hz.guannengcc.top/gtminlgwjs.html

[D23] reduce 累积计算
来源：http://hz.9152youxi.cn/gtocaiysan.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hfpthk.cn/gtlqtggopc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jiagoushi.top/gtqwxwkxpd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shzxlz.cn/gtconkifmr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.birdmap.top/gtnuyncpqw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ehwqpu.com/gtcqbmodty.html

Go:   // 手写循环
来源：http://hz.fengsongda.top/gtrdhkflkj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zdqjudy.top/gtjgapitff.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.birdmap.top/gtqpdetbxc.html

[D24] 字典 / Map 基本操作
来源：http://hz.hfpthk.cn/gtgptfeles.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yueranfly.top/gtofqvrlzr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jlsjyb.cn/gtvtxqkjcd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.9152youxi.cn/gtlzdjeqlq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jinghuilouyu.cn/gtjtkzlvnh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.chenjidiqi.icu/gtfvirmcqh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yongpay.top/gthijhfimb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhengqikj.top/gthrdcuvwa.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.sysykeji.top/gtduavdtkj.html

[D25] Set 集合去重与交并差
来源：http://hz.ehwqpu.com/gtlthqycke.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.wangshuangyany.cn/gtuhhlqhtm.html


<!-- 参考信息 -->