代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.birdmap.top/gtpuzqtduo.html

Go:   return a, b
来源：http://hz.ppjwa.cn/gtlxbjdqfw.html

Ruby: return a, b
来源：http://hz.ppjwa.cn/gtukztiqtt.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.zdqjudy.top/gtckixwegc.html

[C06] 匿名函数 / lambda
来源：http://hz.wangdashe.top/gtiqiqwzdj.html

Py:   square = lambda x: x * x
来源：http://hz.chenzaomai.com/gtbtrohuou.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.zhixingplan.top/gtrxjsyplb.html

JS:   const square = x => x * x;
来源：http://hz.havefunace.top/gtpnkzyekw.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.quarkkingdee.top/gtlqzmbqky.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.snrcjt.cn/gtsdxygnpb.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.wangshuangyany.cn/gtohczlgve.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jiagoushi.top/gtcrcjluns.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhixingplan.top/gthvnpycuv.html

[C07] 把函数作为参数传入
来源：http://hz.iojbl.cn/gtgmsuptqs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.ydzc1.top/gtilhrkugf.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.cdnleiting.top/gtlhpflown.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.cheryme.top/gtoyqiqeus.html

TS:   arr.map(String)
来源：http://hz.smart0.xyz/gtrgnjwqpj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.guowangkeji.top/gtrgrvpooh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.wangshuangyany.cn/gtqhsiyuls.html

Ruby: arr.map(&:upcase)
来源：http://hz.dianchejie.cn/gtuzgvbypx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.aizwys.cn/gtiqjpgzou.html

[C08] 闭包
来源：http://hz.yueranfly.top/gtaysdamrh.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.vqdsnc.cn/gtuloceobz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.iojbl.cn/gtpcvbdlib.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.pycfn.com/gtzdgmossq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ywan-chungtsiang.top/gttdzkpaur.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.nanxuanxn.top/gtxazbcwxu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.pengpengdd.cyou/gtxlwwoiqe.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.quarkkingdee.top/gtqcvhngko.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.nanxinkj.top/gtzblztjzx.html

[C09] 递归
来源：http://hz.ywan-chungtsiang.top/gttctuswkw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.fzhhl.top/gtlnzihsmf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.daria6918.cn/gtqujpkiga.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jiagoushi.top/gthsfxzlcm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.tanke756.top/gtqsaprsbz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.mhx1999.top/gtktabystr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.yangfankeji.com/gtjcfkucwy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.svipenyu.cn/gtjsdzakxg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zycfv.cn/gtfhgtejxc.html

[C10] 变量作用域
来源：http://hz.zhijiandao.cn/gtehlmquig.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.mhx1999.top/gtjxytlebw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.gotoacloud.top/gtsbgnjbjw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.gaohongyu789.top/gtacbfxstk.html

TS:   同 JS
来源：http://hz.xuanzx.com/gtjalkgwqr.html

Java: 方法内为块级作用域
来源：http://hz.xuetiantiany.cn/gtegtcpbew.html

Go:   花括号块级作用域
来源：http://hz.haohaochexian.top/gtwhlyoyrr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.guannengcc.top/gthenirjym.html

C#:   块级作用域
来源：http://hz.wangshuangyany.cn/gtoruozoag.html

[C11] 模块导入与导出
来源：http://hz.pycfn.com/gtshvduucm.html

Py:   from module import func
来源：http://hz.yuxming.cn/gtfryicuvo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.316326.xyz/gtoehmtitf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.zdqjudy.top/gtddqcoohv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.ivvv.top/gtfhheidte.html

Java: import java.util.List;
来源：http://hz.zhengqikj.top/gtohoqalvs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.aibaodan.cn/gtnueycmqh.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.fengsongda.top/gtgjwcvxgz.html

C#:   using System.Text;
来源：http://hz.kuanghao11.cn/gtlfxvdiqf.html

[C12] 立即执行函数 IIFE
来源：http://hz.yuanzhike.top/gtxpjjnvyw.html

Py:   (lambda: print("run"))()
来源：http://hz.yuxming.cn/gtpopvlpmh.html

PHP:  (function () { echo "run"; })();
来源：http://hz.sweek.top/gtmbocfywu.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xuetiantiany.cn/gtcjgzbboi.html

TS:   (() => { console.log("run"); })();
来源：http://hz.guowangkeji.top/gtwnoqzcfy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.cucudq.cn/gtgtoarhct.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sxryk.cn/gtgtliluxg.html

Ruby: -> { puts "run" }.call
来源：http://hz.andypj.xyz/gteqboomlt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.sxryk.cn/gttebwvfej.html

[C13] 类型声明 / 类型注解
来源：http://hz.mhx1999.top/gtgfjjfsuq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.zhijiandao.cn/gtnmivkwua.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenlongwang.top/gterbuxlqr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.yanxiufei.cn/gtdxpoevod.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zdqjudy.top/gtjyrcyhyv.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.sysykeji.top/gtjeskmneu.html

Go:   func add(a, b int) int
来源：http://hz.sweek.top/gtjvscsntg.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.guowangkeji.top/gtnnbhduul.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.xylfe.cn/gtiunmdodn.html

[C14] 泛型函数
来源：http://hz.zycfv.cn/gthawtlilz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.hongshengwenyu.top/gtlacesaly.html

PHP:  // 无泛型
来源：http://hz.jyoumei.cn/gtmcmpqgdr.html

JS:   // 无泛型
来源：http://hz.chenjidiqi.icu/gtaygugamf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.iojbl.cn/gtxihxxueb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.shuidangran.top/gtrlsbytof.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.smart0.xyz/gtysgxoiga.html

Ruby: # 无泛型
来源：http://hz.birdmap.top/gtactjacou.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.aizwys.cn/gtyyyvqwdy.html

[C15] 解构 / 展开参数
来源：http://hz.guowangkeji.top/gtrxbqkgzq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhaomingkeji.xyz/gtabbwkofd.html

PHP:  [$a, $b] = $pair;
来源：http://hz.yueranfly.top/gttfbeinuj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jyoumei.cn/gtftgmhksc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.jinyuanbaomall.cn/gtukaxqzje.html

Java: // 无解构
来源：http://hz.hnqzz.top/gtktakvngl.html

Go:   // 无解构
来源：http://hz.aizwys.cn/gthbfntlld.html

Ruby: a, b = pair
来源：http://hz.iojbl.cn/gtkevfwksw.html

C#:   var (a, b) = pair;
来源：http://hz.nanxinkj.top/gtpvsmrjww.html

[C16] 函数 / 方法重载
来源：http://hz.jyoumei.cn/gtbdbyaqbt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.hfpthk.cn/gteufnuyiy.html

PHP:  // 无重载
来源：http://hz.andypj.xyz/gtbfsgtqye.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zhoulong.xyz/gtipmyiyhw.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ydzc1.top/gtbwtdgvzl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jqgfzy.top/gtttcyyytu.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhixingplan.top/gtqbakymtu.html

Ruby: # 无重载：靠动态参数
来源：http://hz.andypj.xyz/gtomxzdiqu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.aibaodan.cn/gtvbstygwd.html

================================================================================
来源：http://hz.yj202588.top/gtoenppben.html

D. 数组 / 列表 / 集合
来源：http://hz.birdmap.top/gtbbehztrj.html

================================================================================
来源：http://hz.smart0.xyz/gtwhgnjzub.html

[D01] 创建数组 / 列表
来源：http://hz.fzhhl.top/gtjgfhuiti.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jinghuilouyu.cn/gtsqwyevdp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jlsjyb.cn/gtjirjfdib.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.pycfn.com/gtxjccinkx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.shanyushiyangkeji.top/gtngxfrije.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yangfankeji.com/gtdxvohtqd.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ywan-chungtsiang.top/gtvvqmurdt.html

Ruby: arr = [1, 2, 3]
来源：http://hz.zhoulong.xyz/gtsoszjqdl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yuxming.cn/gtvmyzyfjr.html

[D02] 追加元素到末尾
来源：http://hz.316326.xyz/gtyxzsqlxs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.jlsjyb.cn/gtjnqzgngk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.cucudq.cn/gtqwglzjay.html

JS:   arr.push(4);
来源：http://hz.jyoumei.cn/gtcfxsvzor.html

TS:   arr.push(4);
来源：http://hz.wangdashe.top/gtluzecmqb.html

Java: list.add(4);
来源：http://hz.chenjidiqi.icu/gtpxerytaw.html

Go:   arr = append(arr, 4)
来源：http://hz.shanyushiyangkeji.top/gthagvqbvh.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ydzc1.top/gtqchedhmb.html

C#:   list.Add(4);
来源：http://hz.daxiang520.top/gtvgjunotl.html

[D03] 在指定位置插入元素
来源：http://hz.ydzc1.top/gtnchnpdvu.html

Py:   arr.insert(0, 0)
来源：http://hz.zdqjudy.top/gtdotjyfar.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.birdmap.top/gtmbtfejrj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.andypj.xyz/gtmwwrptps.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hammf.cn/gtsbnnbhxr.html

Java: list.add(0, 0);
来源：http://hz.jinqigufen.top/gtkqsdgerz.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yj20258888.top/gtwzzzdgtm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yuanzhike.top/gtfxbmkkcb.html

C#:   list.Insert(0, 0);
来源：http://hz.hysaishi.cn/gtwxizftuz.html

[D04] 删除元素
来源：http://hz.zhijiandao.cn/gtanzxdnoi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jinghuilouyu.cn/gtiorczfje.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.tian-w.cn/gtnfeqsaxx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.kuanghao11.cn/gtpatwgels.html

TS:   arr.splice(0, 1);
来源：http://hz.yonumen.top/gtykbagwvo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.smart0.xyz/gtuvgfenrm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.9152youxi.cn/gtnsnwucbq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.meibo888.top/gtxyerbpza.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.tanke756.top/gtgdxioqur.html

[D05] 访问与修改元素
来源：http://hz.xuanzx.com/gtqxqfglxz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhoulong.xyz/gttgjjpocd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jinqigufen.top/gtkbmckudv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.dashuyun.cn/gtbpguthvu.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhoulong.xyz/gtjlrdzwvz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.havefunace.top/gtonvpotxv.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.0kj1m.cn/gtevzmcyrw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xinyue.icu/gtlbciweis.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.pycfn.com/gtdpwqwnmd.html

[D06] 数组长度
来源：http://hz.gotoacloud.top/gtctacbkci.html

Py:   len(arr)
来源：http://hz.birdmap.top/gtcnenlcnr.html

PHP:  count($arr);
来源：http://hz.bjfxy.top/gtryiboyoo.html

JS:   arr.length
来源：http://hz.jqgufenzy.top/gthpfysppk.html

TS:   arr.length
来源：http://hz.shangyingyoupin.top/gtbygzvcce.html

Java: list.size();
来源：http://hz.shanyushiyangtech.top/gtbyrjmtvu.html

Go:   len(arr)
来源：http://hz.zycfv.cn/gtwjnlfpav.html

Ruby: arr.length; arr.size
来源：http://hz.tanke756.top/gtjndztjjj.html

C#:   list.Count;
来源：http://hz.nanxinkj.top/gtsnmdifdy.html

[D07] 切片 / 取子数组
来源：http://hz.hnqzz.top/gtcgwrklog.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.316326.xyz/gtpgxegtcn.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yangfankeji.com/gtsqljapob.html

JS:   arr.slice(1, 4);
来源：http://hz.yj202588.top/gtszjdhsss.html

TS:   arr.slice(1, 4);
来源：http://hz.yvedp.cn/gthptkdydg.html

Java: list.subList(1, 4);
来源：http://hz.dianchejie.cn/gtdsgoxyeo.html

Go:   arr[1:4]
来源：http://hz.iojbl.cn/gtjqkgyyul.html

Ruby: arr[1, 3]
来源：http://hz.tanke756.top/gtijjbczlk.html

C#:   list.GetRange(1, 3);
来源：http://hz.jinqigufen.top/gtjofxmcoc.html

[D08] 合并两个数组
来源：http://hz.bjfxy.top/gtldlpywge.html

Py:   a + b;  a.extend(b)
来源：http://hz.chenzaomai.com/gticoiahkm.html

PHP:  array_merge($a, $b);
来源：http://hz.yj20258.top/gtevhzejyq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yonumen.top/gtobgkumpt.html

TS:   [...a, ...b];
来源：http://hz.tianlin.xyz/gtbtwnzjos.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.tian-w.cn/gtjkkkqhxo.html

Go:   append(a, b...)
来源：http://hz.tanke756.top/gtyjjuzvwz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhijiandao.cn/gtlhqwqslg.html

C#:   a.Concat(b).ToList()
来源：http://hz.chenlongwang.top/gtagzadyct.html

[D09] 排序（升序）
来源：http://hz.quarkkingdee.top/gtuyfaxdiq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.feifeiyinyue.top/gtdzrrwbfk.html

PHP:  sort($arr);
来源：http://hz.zdqjudy.top/gtfuzqyeot.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hammf.cn/gtvhmudzjt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.iojbl.cn/gtnvxtsfmu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.wangshuangyany.cn/gtmmizqrwb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zhaomingkeji.xyz/gtlqgpefof.html

Ruby: arr.sort
来源：http://hz.sysykeji.top/gtuvctkunn.html

C#:   list.Sort();
来源：http://hz.dashuyun.cn/gtfcrrjbwl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.0kj1m.cn/gtzncirlco.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.redwolf501.top/gtwvjxtyql.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cqqwz.cn/gtutvadmrz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.0kj1m.cn/gtqklawwtj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ywan-chungtsiang.top/gtufhbqhzp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cdnleiting.top/gtgavwkgty.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yuanzhike.top/gtuezgjjax.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yongpay.top/gtxabfxpyj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.dashuyun.cn/gtziwetjpy.html

[D11] 反转数组
来源：http://hz.zhongyouzk.top/gtvtrqxurh.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zdqjudy.top/gtitqhsaua.html

PHP:  array_reverse($arr);
来源：http://hz.xingfuxueyuan.xyz/gtpdwkhxoq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.gogol.net.cn/gtglscikvo.html

TS:   [...arr].reverse();
来源：http://hz.zhengqikj.top/gtqvllajdd.html

Java: Collections.reverse(list);
来源：http://hz.jinqigfzy.top/gtrxvrizga.html

Go:   slices.Reverse(arr)
来源：http://hz.yueranfly.top/gtxexiymfb.html

Ruby: arr.reverse
来源：http://hz.zhaomingkeji.xyz/gtfdftdrdn.html

C#:   list.Reverse();
来源：http://hz.jiagoushi.top/gtpxcunqcb.html

[D12] 查找元素下标
来源：http://hz.tianlin.xyz/gtvfxsmdrn.html

Py:   arr.index(x);  x in arr
来源：http://hz.hammf.cn/gttfmlobco.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhaomingkeji.xyz/gtunkfkccj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ivvv.top/gtayohntwb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yangfankeji.com/gtthvepyol.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hysaishi.cn/gttqvlgtyp.html

Go:   slices.Index(arr, x)
来源：http://hz.yongpay.top/gtdujsqaar.html

Ruby: arr.index(x)
来源：http://hz.hammf.cn/gtytqjnvtx.html

C#:   list.IndexOf(x);
来源：http://hz.zhengqikj.top/gtpgtrjunw.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhoulong.xyz/gtnbsdcbsz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.sufxvd.cn/gtwxphgvig.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jyoumei.cn/gtbrsokamn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jinghuilouyu.cn/gtxmmtfidh.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhengqikj.top/gtsgjpptth.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zdqjudy.top/gttjsuofba.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xylfe.cn/gtajkfbuxf.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yueranfly.top/gtwgemsgco.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yanxiufei.cn/gtxgcpxiro.html

[D14] 映射转换（每个元素变形）
来源：http://hz.svipenyu.cn/gtdlsytkir.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.sweek.top/gtwwhohubb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.nanxinkj.top/gtatdyqjpk.html

JS:   arr.map(x => x * 2)
来源：http://hz.xuetiantiany.cn/gtpuzeijva.html

TS:   arr.map(x => x * 2)
来源：http://hz.c1oappe.top/gtzmghjtkc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.9152youxi.cn/gtdlxlkpxe.html

Go:   // 手写循环
来源：http://hz.hywenlv.cn/gtjwmxtaiu.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.chenzaomai.com/gtuvbfvhdc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.tian-w.cn/gtznkjdsnj.html

[D15] 去重
来源：http://hz.yonumen.top/gtlknggvdn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xylfe.cn/gtulmqwcfd.html

PHP:  array_unique($arr);
来源：http://hz.c1oappe.top/gtenptxxoq.html

JS:   [...new Set(arr)]
来源：http://hz.zhixingplan.top/gtddmuirzt.html

TS:   [...new Set(arr)]
来源：http://hz.meibo888.top/gtcenapvec.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hammf.cn/gtasascsup.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.fengsongda.top/gtokyvsdrf.html

Ruby: arr.uniq
来源：http://hz.xuanzx.com/gtexeecwvz.html

C#:   list.Distinct().ToList()
来源：http://hz.yj20258888.top/gtfanhsaxd.html

[D16] 求和与平均值
来源：http://hz.xuetiantiany.cn/gtxffqpjks.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhixingplan.top/gtqspczyaz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.daxiang520.top/gtusdqoyjg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yanxiufei.cn/gtmegoetoz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cqqwz.cn/gtksstigci.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.guannengcc.top/gtjdnkeohx.html

Go:   // 手写循环累加
来源：http://hz.fzhhl.top/gtvgoabgmk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jinyuanbaomall.cn/gtqqhurvtf.html

C#:   list.Sum();  list.Average()
来源：http://hz.cheryme.top/gtqtbkrafv.html

[D17] 最大值与最小值
来源：http://hz.ydzc1.top/gtigadstqw.html

Py:   max(arr);  min(arr)
来源：http://hz.xuanzx.com/gtpfyehoow.html

PHP:  max($arr);  min($arr);
来源：http://hz.yvedp.cn/gtsltcgmjj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.iojbl.cn/gtfkqkgllb.html

TS:   Math.max(...arr);
来源：http://hz.gotoacloud.top/gtwvxsqcwq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhoulong.xyz/gtseydeldl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.sufxvd.cn/gtrsyntdbd.html

Ruby: arr.max;  arr.min
来源：http://hz.sufxvd.cn/gtlkienpwl.html

C#:   list.Max();  list.Min()
来源：http://hz.hongshengwenyu.top/gtfqjysmge.html

[D18] 扁平化嵌套数组
来源：http://hz.chenlongwang.top/gtoqhsfpwj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jlsjyb.cn/gtqdrkkcty.html

PHP:  array_merge(...$nested);
来源：http://hz.kuanghao11.cn/gtxhogtpax.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zhiwuduotai.top/gtsgvqiass.html

TS:   nested.flat();
来源：http://hz.ybcxt.top/gtlvcwnxdh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.cucudq.cn/gtryuugwkn.html

Go:   // 手写双层循环
来源：http://hz.vqdsnc.cn/gtnslpaagb.html

Ruby: nested.flatten
来源：http://hz.mhx1999.top/gtnzrajevs.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jyoumei.cn/gtccwvkfus.html

[D19] 按字段分组
来源：http://hz.ehwqpu.com/gtixnhcyac.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.aibaodan.cn/gtwqezpvxs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jinghuilouyu.cn/gtaqcgmxvp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.shangyingyoupin.top/gtudpxevec.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhengqikj.top/gtdigbfckz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.c1oappe.top/gtlkixbnhh.html

Go:   // 手写 map[string][]T
来源：http://hz.shanyushiyangkeji.top/gtiovuyswu.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gaohongyu789.top/gtrlsnvcuo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.kuanghao11.cn/gtwhfjgjtv.html

[D20] 统计每个元素出现次数
来源：http://hz.cqqwz.cn/gtnvsfsanm.html

Py:   Counter(arr)
来源：http://hz.smart0.xyz/gtosqxhano.html

PHP:  array_count_values($arr);
来源：http://hz.xuetiantiany.cn/gtcgpyehdr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jlsjyb.cn/gthyzisqnf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.daxiang520.top/gtmdxmrgrg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ydjk.org.cn/gteygwfhtt.html

Go:   // 手写 map[T]int
来源：http://hz.cheryme.top/gtegccslzv.html

Ruby: arr.tally
来源：http://hz.yj202588.top/gttrbaybpk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.kuanghao11.cn/gtdytgkuva.html

[D21] 判断是否包含某元素
来源：http://hz.jiagoushi.top/gtfueapntn.html

Py:   x in arr
来源：http://hz.jyoumei.cn/gtqaidtvoo.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yuanzhike.top/gtimbdknrj.html

JS:   arr.includes(x)
来源：http://hz.yuxming.cn/gtwotksctx.html

TS:   arr.includes(x)
来源：http://hz.smart0.xyz/gtvlfepniy.html

Java: list.contains(x)
来源：http://hz.tian-w.cn/gtyjwoowry.html

Go:   slices.Contains(arr, x)
来源：http://hz.ydzc1.top/gtedoigqbx.html

Ruby: arr.include?(x)
来源：http://hz.iojbl.cn/gtpftbrfth.html

C#:   list.Contains(x)
来源：http://hz.ydjk.org.cn/gtdqqrndkk.html

[D22] 复制数组（避免共享引用）
来源：http://hz.xziqi.cn/gtkjjjeydx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.tian-w.cn/gtkdsifwep.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhongyouzk.top/gtcwfhueem.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cheryme.top/gtbqpyflxi.html

TS:   [...arr];
来源：http://hz.mhx1999.top/gtyjgpxwlg.html


<!-- 参考信息 -->