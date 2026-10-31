代发 wailian999

[C06] 匿名函数 / lambda
来源：http://vt.shxzukj.cn

Py:   square = lambda x: x * x
来源：http://xl.huixinmuqiang.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ak.szxytkj.cn

JS:   const square = x => x * x;
来源：http://hl.shxzukj.cn

TS:   const square = (x: number): number => x * x;
来源：http://vg.yuntaijiaju.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://po.jctech888.com.cn

Go:   sq := func(x int) int { return x * x }
来源：http://nk.shxzskj.cn

Ruby: square = ->(x) { x * x }
来源：http://mj.shtwfgs.cn

C#:   Func<int, int> square = x => x * x;
来源：http://of.chemitech.net.cn

[C07] 把函数作为参数传入
来源：http://xn.shtwfgs.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jc.jianghongdianzi.cn

PHP:  array_map("strtoupper", $arr);
来源：http://xg.muxihuayi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ni.yuexingan06.cn

TS:   arr.map(String)
来源：http://rf.bjjhwx.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ra.huanxung.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wy.asd995.cn

Ruby: arr.map(&:upcase)
来源：http://kh.jctech888.com.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://bm.szxytkj.cn

[C08] 闭包
来源：http://hb.lnxyls.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zz.nicolike.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://lg.chemitech.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wb.haigaiapp.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://rv.jctech888.com.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://sp.9csxet.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yq.asd995.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ll.hnjuh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ob.newstarts.cn

[C09] 递归
来源：http://vo.yuntaijiaju.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://bf.yuntaijiaju.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://gh.panjiajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cs.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://px.shxzukj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://sr.bjjhwx.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://je.jctech888.com.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://nl.newstarts.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://uj.521024.cn

[C10] 变量作用域
来源：http://fk.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ke.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qu.colortex.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://il.panjiajie.cn

TS:   同 JS
来源：http://ci.muxihuayi.cn

Java: 方法内为块级作用域
来源：http://pp.colortex.cn

Go:   花括号块级作用域
来源：http://cs.newstarts.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sc.yuexingan06.cn

C#:   块级作用域
来源：http://cr.bjjhwx.cn

[C11] 模块导入与导出
来源：http://nn.shtwfgs.cn

Py:   from module import func
来源：http://xg.bjjhwx.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mb.szxytkj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ew.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://fu.asd995.cn

Java: import java.util.List;
来源：http://un.hnjuh.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ob.szxytkj.cn

Ruby: require "json"; require_relative "./util"
来源：http://pt.hahajie.cn

C#:   using System.Text;
来源：http://tg.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://vh.shxzskj.cn

Py:   (lambda: print("run"))()
来源：http://ll.jctech888.com.cn

PHP:  (function () { echo "run"; })();
来源：http://aq.yuexingan06.cn

JS:   (() => { console.log("run"); })();
来源：http://tg.nicolike.cn

TS:   (() => { console.log("run"); })();
来源：http://zy.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hc.szxytkj.cn

Go:   func() { fmt.Println("run") }()
来源：http://rq.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://iz.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ne.jctech888.com.cn

[C13] 类型声明 / 类型注解
来源：http://an.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yg.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vi.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ml.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://cc.haigaiapp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bk.panjiajie.cn

Go:   func add(a, b int) int
来源：http://mj.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sm.yuexingan06.cn

C#:   int Add(int a, int b) => a + b;
来源：http://oy.szxytkj.cn

[C14] 泛型函数
来源：http://qf.hnjuh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lx.shxzukj.cn

PHP:  // 无泛型
来源：http://rq.szxytkj.cn

JS:   // 无泛型
来源：http://wm.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kr.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://oy.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wm.jctech888.com.cn

Ruby: # 无泛型
来源：http://fe.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ja.asd995.cn

[C15] 解构 / 展开参数
来源：http://mu.muxihuayi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lh.shxzukj.cn

PHP:  [$a, $b] = $pair;
来源：http://rz.bjjhwx.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://nu.hahajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://yx.huixiangedu.cn

Java: // 无解构
来源：http://kn.huixiangedu.cn

Go:   // 无解构
来源：http://pa.huanxung.cn

Ruby: a, b = pair
来源：http://sk.huixiangedu.cn

C#:   var (a, b) = pair;
来源：http://ji.yuexingan06.cn

[C16] 函数 / 方法重载
来源：http://cg.panjiajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://op.9csxet.cn

PHP:  // 无重载
来源：http://wj.gzmigu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ex.chemitech.net.cn

TS:   // 用联合类型或重载签名声明
来源：http://jy.lnxyls.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wg.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://um.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://cu.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ng.shtwfgs.cn

================================================================================
来源：http://pq.bjjhwx.cn

D. 数组 / 列表 / 集合
来源：http://ni.yuexingan06.cn

================================================================================
来源：http://bx.yuexingan06.cn

[D01] 创建数组 / 列表
来源：http://vs.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bl.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://py.chemitech.net.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mp.yuntaijiaju.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wi.nszjky.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mh.huixinmuqiang.cn

Go:   arr := []int{1, 2, 3}
来源：http://gp.jianghongdianzi.cn

Ruby: arr = [1, 2, 3]
来源：http://bm.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://od.szxytkj.cn

[D02] 追加元素到末尾
来源：http://jb.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ae.9csxet.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wu.asd995.cn

JS:   arr.push(4);
来源：http://bz.nicolike.cn

TS:   arr.push(4);
来源：http://nf.bjjhwx.cn

Java: list.add(4);
来源：http://xp.bjjhwx.cn

Go:   arr = append(arr, 4)
来源：http://hm.panjiajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://uv.haigaiapp.cn

C#:   list.Add(4);
来源：http://db.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://mj.jctech888.com.cn

Py:   arr.insert(0, 0)
来源：http://fb.lnxyls.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://rp.bjjhwx.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fs.jianghongdianzi.cn

TS:   arr.splice(0, 0, 0);
来源：http://cm.gzmigu.cn

Java: list.add(0, 0);
来源：http://hi.yuexingan06.cn

Go:   arr = append([]int{0}, arr...)
来源：http://nl.shtwfgs.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uw.colortex.cn

C#:   list.Insert(0, 0);
来源：http://ke.chemitech.net.cn

[D04] 删除元素
来源：http://kr.szsharing.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mr.asd995.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xe.hahajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://yu.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://cb.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zx.nszjky.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://re.haigaiapp.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ry.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://va.asd995.cn

[D05] 访问与修改元素
来源：http://td.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://jn.lnxyls.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://px.bjjhwx.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://aq.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://hq.huixiangedu.cn

Java: list.get(0); list.set(0, 9);
来源：http://jv.521024.cn

Go:   arr[0]; arr[0] = 9
来源：http://ml.chemitech.net.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://gr.hnjuh.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hl.asd995.cn

[D06] 数组长度
来源：http://xm.asd995.cn

Py:   len(arr)
来源：http://qn.bookmarksfly.cn

PHP:  count($arr);
来源：http://tn.newstarts.cn

JS:   arr.length
来源：http://kw.szxytkj.cn

TS:   arr.length
来源：http://hu.nicolike.cn

Java: list.size();
来源：http://mh.huixiangedu.cn

Go:   len(arr)
来源：http://ml.huixinmuqiang.cn

Ruby: arr.length; arr.size
来源：http://rj.yuexingan06.cn

C#:   list.Count;
来源：http://ok.gzmigu.cn

[D07] 切片 / 取子数组
来源：http://mf.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://rx.huixiangedu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vr.chemitech.net.cn

JS:   arr.slice(1, 4);
来源：http://ey.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://we.hahajie.cn

Java: list.subList(1, 4);
来源：http://pz.gzmigu.cn

Go:   arr[1:4]
来源：http://eo.huanxung.cn

Ruby: arr[1, 3]
来源：http://vm.9csxet.cn

C#:   list.GetRange(1, 3);
来源：http://cu.shxzukj.cn

[D08] 合并两个数组
来源：http://ml.panjiajie.cn

Py:   a + b;  a.extend(b)
来源：http://av.haigaiapp.cn

PHP:  array_merge($a, $b);
来源：http://dn.hahajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ns.shxzukj.cn

TS:   [...a, ...b];
来源：http://xz.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://uf.shxzskj.cn

Go:   append(a, b...)
来源：http://ac.huanxung.cn

Ruby: a + b;  a.concat(b)
来源：http://cj.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://nw.gzmigu.cn

[D09] 排序（升序）
来源：http://rt.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://uw.jianghongdianzi.cn

PHP:  sort($arr);
来源：http://iw.haigaiapp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xw.bookmarksfly.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ab.yuntaijiaju.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wi.yuexingan06.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://iy.shxzukj.cn

Ruby: arr.sort
来源：http://jo.colortex.cn

C#:   list.Sort();
来源：http://zg.newstarts.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://qt.gzmigu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://og.yuexingan06.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hj.yuntaijiaju.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sd.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yg.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://kb.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fi.muxihuayi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://dh.szxytkj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gi.shxzskj.cn

[D11] 反转数组
来源：http://xx.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qc.huanxung.cn

PHP:  array_reverse($arr);
来源：http://oi.chemitech.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ud.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://iu.asd995.cn

Java: Collections.reverse(list);
来源：http://vn.nicolike.cn

Go:   slices.Reverse(arr)
来源：http://jj.huanxung.cn

Ruby: arr.reverse
来源：http://st.szxytkj.cn

C#:   list.Reverse();
来源：http://vc.hahajie.cn

[D12] 查找元素下标
来源：http://la.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://pn.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oh.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wc.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rp.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ls.bookmarksfly.cn

Go:   slices.Index(arr, x)
来源：http://ev.9csxet.cn

Ruby: arr.index(x)
来源：http://zs.bjjhwx.cn

C#:   list.IndexOf(x);
来源：http://on.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://wi.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qu.newstarts.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ko.yuntaijiaju.cn

JS:   arr.filter(x => x > 3)
来源：http://ar.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://sb.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://nn.huixiangedu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://jg.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fg.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wf.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://xq.lnxyls.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ac.wgjwhj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ff.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://mg.shxzskj.cn

TS:   arr.map(x => x * 2)
来源：http://ws.huanxung.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://st.jctech888.com.cn

Go:   // 手写循环
来源：http://ts.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tu.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wy.panjiajie.cn

[D15] 去重
来源：http://zq.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cc.szxytkj.cn

PHP:  array_unique($arr);
来源：http://ih.jctech888.com.cn

JS:   [...new Set(arr)]
来源：http://tk.colortex.cn

TS:   [...new Set(arr)]
来源：http://vt.hahajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://dg.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lp.huanxung.cn

Ruby: arr.uniq
来源：http://rm.521024.cn

C#:   list.Distinct().ToList()
来源：http://iu.newstarts.cn

[D16] 求和与平均值
来源：http://ak.nicolike.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ma.hahajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kk.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jv.bjjhwx.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fk.huanxung.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://vc.shtwfgs.cn

Go:   // 手写循环累加
来源：http://xm.muxihuayi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://uy.gzmigu.cn

C#:   list.Sum();  list.Average()
来源：http://mu.jctech888.com.cn

[D17] 最大值与最小值
来源：http://wt.asd995.cn

Py:   max(arr);  min(arr)
来源：http://fc.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://zq.hahajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ax.hahajie.cn

TS:   Math.max(...arr);
来源：http://zz.huixiangedu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bm.bookmarksfly.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://lc.huixinmuqiang.cn

Ruby: arr.max;  arr.min
来源：http://zj.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://bd.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://jy.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dc.colortex.cn

PHP:  array_merge(...$nested);
来源：http://tn.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://js.gzmigu.cn

TS:   nested.flat();
来源：http://mr.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ft.shxzskj.cn

Go:   // 手写双层循环
来源：http://ff.asd995.cn

Ruby: nested.flatten
来源：http://iv.bookmarksfly.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zt.chemitech.net.cn

[D19] 按字段分组
来源：http://xp.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://my.wgjwhj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://kh.lnxyls.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ai.bjjhwx.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dw.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://is.colortex.cn

Go:   // 手写 map[string][]T
来源：http://as.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fu.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lk.muxihuayi.cn

[D20] 统计每个元素出现次数
来源：http://bh.colortex.cn

Py:   Counter(arr)
来源：http://dm.bookmarksfly.cn

PHP:  array_count_values($arr);
来源：http://yq.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ct.newstarts.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uh.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fm.9csxet.cn

Go:   // 手写 map[T]int
来源：http://im.jctech888.com.cn

Ruby: arr.tally
来源：http://db.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ef.jianghongdianzi.cn

[D21] 判断是否包含某元素
来源：http://cw.lnxyls.cn

Py:   x in arr
来源：http://yo.newstarts.cn

PHP:  in_array($x, $arr, true);
来源：http://qe.hnjuh.cn

JS:   arr.includes(x)
来源：http://lc.newstarts.cn

TS:   arr.includes(x)
来源：http://ir.jianghongdianzi.cn

Java: list.contains(x)
来源：http://dx.szsharing.cn

Go:   slices.Contains(arr, x)
来源：http://ml.asd995.cn

Ruby: arr.include?(x)
来源：http://ch.9csxet.cn

C#:   list.Contains(x)
来源：http://gg.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://ef.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wj.shxzskj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sg.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ul.wgjwhj.cn

TS:   [...arr];
来源：http://qz.panjiajie.cn

Java: new ArrayList<>(list);
来源：http://zh.bookmarksfly.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wx.hahajie.cn

Ruby: arr.dup;  arr.clone
来源：http://gu.chemitech.net.cn

C#:   new List<int>(list);
来源：http://rp.hnjuh.cn


<!-- 参考信息 -->