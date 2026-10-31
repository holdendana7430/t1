代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://ft.nicolike.cn

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://nn.jctech888.com.cn

[C04] 命名参数 / 关键字参数
来源：http://ht.chemitech.net.cn

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://ld.panjiajie.cn

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://xr.bookmarksfly.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://lm.huixinmuqiang.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://de.jianghongdianzi.cn

Java: // 无：用 Builder 模式或 record
来源：http://gs.521024.cn

Go:   // 无：用配置结构体参数
来源：http://bv.jctech888.com.cn

Ruby: f(a: 1, b: 2)
来源：http://ig.nszjky.cn

C#:   f(a: 1, b: 2)
来源：http://hi.muxihuayi.cn

[C05] 返回多个值
来源：http://xh.shxzukj.cn

Py:   return a, b
来源：http://wx.shxzskj.cn

PHP:  return [$a, $b];
来源：http://au.panjiajie.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://sb.hahajie.cn

TS:   return { a, b };
来源：http://je.jctech888.com.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://cg.hnjuh.cn

Go:   return a, b
来源：http://wq.hnjuh.cn

Ruby: return a, b
来源：http://ie.szxytkj.cn

C#:   return (a, b);              // ValueTuple
来源：http://hn.colortex.cn

[C06] 匿名函数 / lambda
来源：http://qw.szsharing.cn

Py:   square = lambda x: x * x
来源：http://rb.szxytkj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://hh.huixiangedu.cn

JS:   const square = x => x * x;
来源：http://ww.huixiangedu.cn

TS:   const square = (x: number): number => x * x;
来源：http://sp.jctech888.com.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://uc.huixiangedu.cn

Go:   sq := func(x int) int { return x * x }
来源：http://oz.nszjky.cn

Ruby: square = ->(x) { x * x }
来源：http://bf.shxzukj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wq.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://yr.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://gc.huanxung.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dr.nszjky.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qq.panjiajie.cn

TS:   arr.map(String)
来源：http://uh.9csxet.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://dv.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ss.521024.cn

Ruby: arr.map(&:upcase)
来源：http://xc.521024.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://fg.szxytkj.cn

[C08] 闭包
来源：http://yo.gzmigu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://bn.jctech888.com.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ss.9csxet.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yo.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://or.huixiangedu.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rh.huixinmuqiang.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://zp.huixiangedu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ck.jianghongdianzi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://nn.lnxyls.cn

[C09] 递归
来源：http://va.lnxyls.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://sf.gzmigu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://dx.yuexingan06.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vk.shxzskj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://he.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ue.szsharing.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://id.yuexingan06.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ox.chemitech.net.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ls.bookmarksfly.cn

[C10] 变量作用域
来源：http://vj.nicolike.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ud.nicolike.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xz.szxytkj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://xx.yuexingan06.cn

TS:   同 JS
来源：http://yp.hahajie.cn

Java: 方法内为块级作用域
来源：http://ku.newstarts.cn

Go:   花括号块级作用域
来源：http://zs.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sp.gzmigu.cn

C#:   块级作用域
来源：http://xf.huixiangedu.cn

[C11] 模块导入与导出
来源：http://ub.asd995.cn

Py:   from module import func
来源：http://it.colortex.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://au.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://hk.jianghongdianzi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://js.szxytkj.cn

Java: import java.util.List;
来源：http://ur.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dc.nicolike.cn

Ruby: require "json"; require_relative "./util"
来源：http://yh.muxihuayi.cn

C#:   using System.Text;
来源：http://ge.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://ca.shtwfgs.cn

Py:   (lambda: print("run"))()
来源：http://on.jctech888.com.cn

PHP:  (function () { echo "run"; })();
来源：http://qp.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://xu.chemitech.net.cn

TS:   (() => { console.log("run"); })();
来源：http://ju.521024.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cs.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://gs.hnjuh.cn

Ruby: -> { puts "run" }.call
来源：http://vl.szxytkj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://hw.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://fv.jctech888.com.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://lw.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hl.gzmigu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fp.asd995.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://lt.szsharing.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ol.9csxet.cn

Go:   func add(a, b int) int
来源：http://yl.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://qk.muxihuayi.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vj.nicolike.cn

[C14] 泛型函数
来源：http://pu.panjiajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zy.jctech888.com.cn

PHP:  // 无泛型
来源：http://ns.panjiajie.cn

JS:   // 无泛型
来源：http://vo.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ub.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://gz.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://eh.nicolike.cn

Ruby: # 无泛型
来源：http://xc.haigaiapp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ic.bookmarksfly.cn

[C15] 解构 / 展开参数
来源：http://zv.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gj.521024.cn

PHP:  [$a, $b] = $pair;
来源：http://sk.huixinmuqiang.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://vj.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pt.chemitech.net.cn

Java: // 无解构
来源：http://vk.huanxung.cn

Go:   // 无解构
来源：http://tq.gzmigu.cn

Ruby: a, b = pair
来源：http://wm.nicolike.cn

C#:   var (a, b) = pair;
来源：http://gl.shxzskj.cn

[C16] 函数 / 方法重载
来源：http://hj.bookmarksfly.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://yd.9csxet.cn

PHP:  // 无重载
来源：http://hc.colortex.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zy.szsharing.cn

TS:   // 用联合类型或重载签名声明
来源：http://ku.521024.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xg.521024.cn

Go:   // 无重载：用不同函数名
来源：http://rk.gzmigu.cn

Ruby: # 无重载：靠动态参数
来源：http://lq.shxzukj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://gf.yuntaijiaju.cn

================================================================================
来源：http://as.panjiajie.cn

D. 数组 / 列表 / 集合
来源：http://xo.bookmarksfly.cn

================================================================================
来源：http://wr.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://ga.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://rj.jianghongdianzi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://zx.huixiangedu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gu.hahajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sk.521024.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ot.bjjhwx.cn

Go:   arr := []int{1, 2, 3}
来源：http://ns.jianghongdianzi.cn

Ruby: arr = [1, 2, 3]
来源：http://ph.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fe.nicolike.cn

[D02] 追加元素到末尾
来源：http://yu.521024.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kp.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ky.shxzukj.cn

JS:   arr.push(4);
来源：http://vb.gzmigu.cn

TS:   arr.push(4);
来源：http://ll.shtwfgs.cn

Java: list.add(4);
来源：http://kw.hahajie.cn

Go:   arr = append(arr, 4)
来源：http://ph.huanxung.cn

Ruby: arr << 4; arr.push(5)
来源：http://vl.huanxung.cn

C#:   list.Add(4);
来源：http://ee.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://er.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://ie.huixiangedu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xv.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cu.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://ke.shxzukj.cn

Java: list.add(0, 0);
来源：http://mz.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vi.hnjuh.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yx.yuntaijiaju.cn

C#:   list.Insert(0, 0);
来源：http://pj.hahajie.cn

[D04] 删除元素
来源：http://vv.hnjuh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sj.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://oq.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yq.shxzukj.cn

TS:   arr.splice(0, 1);
来源：http://aj.muxihuayi.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://up.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://in.huanxung.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fw.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://us.lnxyls.cn

[D05] 访问与修改元素
来源：http://mn.yuntaijiaju.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wm.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vp.shtwfgs.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yt.asd995.cn

TS:   arr[0]; arr.at(-1);
来源：http://yl.9csxet.cn

Java: list.get(0); list.set(0, 9);
来源：http://mf.shxzukj.cn

Go:   arr[0]; arr[0] = 9
来源：http://st.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://se.newstarts.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fb.wgjwhj.cn

[D06] 数组长度
来源：http://pq.hnjuh.cn

Py:   len(arr)
来源：http://sf.wgjwhj.cn

PHP:  count($arr);
来源：http://bv.yuexingan06.cn

JS:   arr.length
来源：http://zj.asd995.cn

TS:   arr.length
来源：http://ro.jctech888.com.cn

Java: list.size();
来源：http://ig.nszjky.cn

Go:   len(arr)
来源：http://ft.huanxung.cn

Ruby: arr.length; arr.size
来源：http://zo.nszjky.cn

C#:   list.Count;
来源：http://fw.asd995.cn

[D07] 切片 / 取子数组
来源：http://pf.huixiangedu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nz.lnxyls.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yi.shxzskj.cn

JS:   arr.slice(1, 4);
来源：http://dt.9csxet.cn

TS:   arr.slice(1, 4);
来源：http://ad.hahajie.cn

Java: list.subList(1, 4);
来源：http://xs.nszjky.cn

Go:   arr[1:4]
来源：http://ch.szxytkj.cn

Ruby: arr[1, 3]
来源：http://zw.jctech888.com.cn

C#:   list.GetRange(1, 3);
来源：http://pa.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://oq.gzmigu.cn

Py:   a + b;  a.extend(b)
来源：http://ol.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://mi.521024.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ob.asd995.cn

TS:   [...a, ...b];
来源：http://mq.bookmarksfly.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sx.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://wa.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://dt.szsharing.cn

C#:   a.Concat(b).ToList()
来源：http://qu.haigaiapp.cn

[D09] 排序（升序）
来源：http://rg.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://kw.shtwfgs.cn

PHP:  sort($arr);
来源：http://kp.9csxet.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rn.hahajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tq.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://im.nszjky.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jp.bjjhwx.cn

Ruby: arr.sort
来源：http://xt.hahajie.cn

C#:   list.Sort();
来源：http://ce.colortex.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ac.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lc.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://od.shxzskj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ky.shxzskj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://rh.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ze.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gg.szxytkj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oh.jianghongdianzi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jv.colortex.cn

[D11] 反转数组
来源：http://yh.newstarts.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gd.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://sv.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ud.gzmigu.cn

TS:   [...arr].reverse();
来源：http://hw.panjiajie.cn

Java: Collections.reverse(list);
来源：http://qt.jianghongdianzi.cn

Go:   slices.Reverse(arr)
来源：http://eu.huixinmuqiang.cn

Ruby: arr.reverse
来源：http://lx.shxzskj.cn

C#:   list.Reverse();
来源：http://gq.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://jp.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://oz.gzmigu.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://li.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ub.yuexingan06.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tk.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ns.yuntaijiaju.cn

Go:   slices.Index(arr, x)
来源：http://tc.huanxung.cn

Ruby: arr.index(x)
来源：http://sz.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://hj.colortex.cn

[D13] 过滤（保留满足条件的）
来源：http://lp.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qf.bookmarksfly.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mh.huanxung.cn

JS:   arr.filter(x => x > 3)
来源：http://kj.huixiangedu.cn

TS:   arr.filter(x => x > 3)
来源：http://jz.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fr.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oe.bjjhwx.cn

Ruby: arr.select { |x| x > 3 }
来源：http://li.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nx.newstarts.cn

[D14] 映射转换（每个元素变形）
来源：http://iu.colortex.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fs.hnjuh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zj.hahajie.cn

JS:   arr.map(x => x * 2)
来源：http://yg.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://xl.shtwfgs.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sg.521024.cn

Go:   // 手写循环
来源：http://dm.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://zp.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://mt.bookmarksfly.cn

[D15] 去重
来源：http://yl.huixinmuqiang.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bi.hahajie.cn

PHP:  array_unique($arr);
来源：http://mr.chemitech.net.cn

JS:   [...new Set(arr)]
来源：http://lr.haigaiapp.cn

TS:   [...new Set(arr)]
来源：http://nk.colortex.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://st.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ql.huanxung.cn

Ruby: arr.uniq
来源：http://or.shxzukj.cn

C#:   list.Distinct().ToList()
来源：http://hz.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://te.yuntaijiaju.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ck.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://go.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mn.shxzukj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rc.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fz.yuexingan06.cn

Go:   // 手写循环累加
来源：http://if.shtwfgs.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xb.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://es.huixiangedu.cn

[D17] 最大值与最小值
来源：http://vd.szsharing.cn

Py:   max(arr);  min(arr)
来源：http://jn.shxzukj.cn

PHP:  max($arr);  min($arr);
来源：http://sj.521024.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://vj.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://jq.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ug.newstarts.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ls.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://ag.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://pv.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://si.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zf.hnjuh.cn

PHP:  array_merge(...$nested);
来源：http://zl.newstarts.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wt.shxzukj.cn

TS:   nested.flat();
来源：http://un.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://no.huixinmuqiang.cn

Go:   // 手写双层循环
来源：http://oc.wgjwhj.cn

Ruby: nested.flatten
来源：http://mv.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://os.wgjwhj.cn

[D19] 按字段分组
来源：http://ju.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ys.shxzukj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zn.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uj.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yk.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gb.gzmigu.cn

Go:   // 手写 map[string][]T
来源：http://sh.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ce.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mz.huixinmuqiang.cn

[D20] 统计每个元素出现次数
来源：http://hd.huixinmuqiang.cn

Py:   Counter(arr)
来源：http://nk.huixinmuqiang.cn

PHP:  array_count_values($arr);
来源：http://rk.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hp.bjjhwx.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ih.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fh.huixiangedu.cn

Go:   // 手写 map[T]int
来源：http://sw.9csxet.cn


<!-- 参考信息 -->