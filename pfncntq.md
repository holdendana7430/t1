代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://hn.szsharing.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://pw.9csxet.cn

[C08] 闭包
来源：http://jh.huixiangedu.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mv.nszjky.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cp.bjjhwx.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yi.jianghongdianzi.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kq.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ve.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rx.jctech888.com.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ww.shxzskj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://je.panjiajie.cn

[C09] 递归
来源：http://yl.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zd.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://fu.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vs.hahajie.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rf.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kv.huixiangedu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://by.yuexingan06.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jk.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wl.nszjky.cn

[C10] 变量作用域
来源：http://xb.panjiajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://so.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://aa.muxihuayi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://sd.shtwfgs.cn

TS:   同 JS
来源：http://zq.bjjhwx.cn

Java: 方法内为块级作用域
来源：http://cb.yuntaijiaju.cn

Go:   花括号块级作用域
来源：http://cs.bookmarksfly.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rz.jctech888.com.cn

C#:   块级作用域
来源：http://mn.shtwfgs.cn

[C11] 模块导入与导出
来源：http://rz.haigaiapp.cn

Py:   from module import func
来源：http://ka.wgjwhj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ea.szxytkj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://za.huanxung.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://iz.newstarts.cn

Java: import java.util.List;
来源：http://zl.nszjky.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://yb.chemitech.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://os.chemitech.net.cn

C#:   using System.Text;
来源：http://hv.hnjuh.cn

[C12] 立即执行函数 IIFE
来源：http://jc.szxytkj.cn

Py:   (lambda: print("run"))()
来源：http://tp.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://zl.bjjhwx.cn

JS:   (() => { console.log("run"); })();
来源：http://rq.newstarts.cn

TS:   (() => { console.log("run"); })();
来源：http://xh.yuexingan06.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vf.huixiangedu.cn

Go:   func() { fmt.Println("run") }()
来源：http://ql.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://fk.shxzskj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gn.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://ep.shxzskj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://fp.shxzukj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ft.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://fe.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://te.521024.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wk.hahajie.cn

Go:   func add(a, b int) int
来源：http://ca.huixinmuqiang.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://rt.shxzukj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hu.huixiangedu.cn

[C14] 泛型函数
来源：http://sp.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bj.newstarts.cn

PHP:  // 无泛型
来源：http://vf.haigaiapp.cn

JS:   // 无泛型
来源：http://lm.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zx.shxzskj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fn.panjiajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hi.asd995.cn

Ruby: # 无泛型
来源：http://oq.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ky.nicolike.cn

[C15] 解构 / 展开参数
来源：http://sb.newstarts.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ui.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://gq.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ae.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://lm.haigaiapp.cn

Java: // 无解构
来源：http://pk.gzmigu.cn

Go:   // 无解构
来源：http://bo.hnjuh.cn

Ruby: a, b = pair
来源：http://mg.asd995.cn

C#:   var (a, b) = pair;
来源：http://th.shxzukj.cn

[C16] 函数 / 方法重载
来源：http://zv.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sm.huixiangedu.cn

PHP:  // 无重载
来源：http://rd.haigaiapp.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lq.yuntaijiaju.cn

TS:   // 用联合类型或重载签名声明
来源：http://mi.shtwfgs.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://id.asd995.cn

Go:   // 无重载：用不同函数名
来源：http://qr.yuntaijiaju.cn

Ruby: # 无重载：靠动态参数
来源：http://hy.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kz.asd995.cn

================================================================================
来源：http://yr.shtwfgs.cn

D. 数组 / 列表 / 集合
来源：http://yd.hahajie.cn

================================================================================
来源：http://cl.yuntaijiaju.cn

[D01] 创建数组 / 列表
来源：http://mz.nicolike.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ga.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://om.colortex.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ge.yuexingan06.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cj.huixiangedu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oh.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://fp.huixiangedu.cn

Ruby: arr = [1, 2, 3]
来源：http://sx.panjiajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ib.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://gx.huixinmuqiang.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sf.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://kn.huanxung.cn

JS:   arr.push(4);
来源：http://bn.yuexingan06.cn

TS:   arr.push(4);
来源：http://vu.shxzskj.cn

Java: list.add(4);
来源：http://ep.jctech888.com.cn

Go:   arr = append(arr, 4)
来源：http://kt.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://it.muxihuayi.cn

C#:   list.Add(4);
来源：http://qb.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://mi.hnjuh.cn

Py:   arr.insert(0, 0)
来源：http://lo.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://kg.szxytkj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ja.bjjhwx.cn

TS:   arr.splice(0, 0, 0);
来源：http://fw.bjjhwx.cn

Java: list.add(0, 0);
来源：http://gy.shtwfgs.cn

Go:   arr = append([]int{0}, arr...)
来源：http://az.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gl.521024.cn

C#:   list.Insert(0, 0);
来源：http://ve.hahajie.cn

[D04] 删除元素
来源：http://yn.panjiajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ll.szsharing.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tl.jianghongdianzi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://we.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://zw.wgjwhj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://cx.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://js.huanxung.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zm.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bf.haigaiapp.cn

[D05] 访问与修改元素
来源：http://gl.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://co.shxzskj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://bj.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ui.panjiajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://ch.colortex.cn

Java: list.get(0); list.set(0, 9);
来源：http://bm.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://zu.szsharing.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://in.shxzukj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://da.chemitech.net.cn

[D06] 数组长度
来源：http://cc.hnjuh.cn

Py:   len(arr)
来源：http://cf.shxzskj.cn

PHP:  count($arr);
来源：http://bx.yuexingan06.cn

JS:   arr.length
来源：http://rt.yuexingan06.cn

TS:   arr.length
来源：http://ch.shxzukj.cn

Java: list.size();
来源：http://of.jianghongdianzi.cn

Go:   len(arr)
来源：http://kq.huanxung.cn

Ruby: arr.length; arr.size
来源：http://yz.huanxung.cn

C#:   list.Count;
来源：http://yu.muxihuayi.cn

[D07] 切片 / 取子数组
来源：http://mg.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://xe.yuntaijiaju.cn

PHP:  array_slice($arr, 1, 3);
来源：http://uw.hnjuh.cn

JS:   arr.slice(1, 4);
来源：http://bo.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://ox.colortex.cn

Java: list.subList(1, 4);
来源：http://hf.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://gt.nicolike.cn

Ruby: arr[1, 3]
来源：http://tf.yuexingan06.cn

C#:   list.GetRange(1, 3);
来源：http://yf.hahajie.cn

[D08] 合并两个数组
来源：http://hw.huanxung.cn

Py:   a + b;  a.extend(b)
来源：http://ve.haigaiapp.cn

PHP:  array_merge($a, $b);
来源：http://sk.shxzskj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zz.chemitech.net.cn

TS:   [...a, ...b];
来源：http://iq.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jw.shtwfgs.cn

Go:   append(a, b...)
来源：http://zf.szsharing.cn

Ruby: a + b;  a.concat(b)
来源：http://fy.chemitech.net.cn

C#:   a.Concat(b).ToList()
来源：http://jk.muxihuayi.cn

[D09] 排序（升序）
来源：http://sc.jianghongdianzi.cn

Py:   sorted(arr);  arr.sort()
来源：http://ei.haigaiapp.cn

PHP:  sort($arr);
来源：http://ku.jianghongdianzi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ll.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wt.szsharing.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rf.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sg.shtwfgs.cn

Ruby: arr.sort
来源：http://iy.szsharing.cn

C#:   list.Sort();
来源：http://ic.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hp.bjjhwx.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mi.huixiangedu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lk.gzmigu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ns.jianghongdianzi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ks.asd995.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xq.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qx.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://kr.gzmigu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zp.hahajie.cn

[D11] 反转数组
来源：http://ax.huanxung.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ae.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://ig.shtwfgs.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rv.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://bn.9csxet.cn

Java: Collections.reverse(list);
来源：http://to.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://hp.muxihuayi.cn

Ruby: arr.reverse
来源：http://da.jianghongdianzi.cn

C#:   list.Reverse();
来源：http://lx.wgjwhj.cn

[D12] 查找元素下标
来源：http://uk.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://ug.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://se.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fl.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xj.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bn.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://iz.asd995.cn

Ruby: arr.index(x)
来源：http://zo.huanxung.cn

C#:   list.IndexOf(x);
来源：http://fs.9csxet.cn

[D13] 过滤（保留满足条件的）
来源：http://uc.haigaiapp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iy.haigaiapp.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ct.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://ie.newstarts.cn

TS:   arr.filter(x => x > 3)
来源：http://iu.9csxet.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mn.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qf.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ct.9csxet.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gz.hahajie.cn

[D14] 映射转换（每个元素变形）
来源：http://fd.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://st.huanxung.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ad.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://eh.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://qb.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ak.lnxyls.cn

Go:   // 手写循环
来源：http://vp.asd995.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ig.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ec.bookmarksfly.cn

[D15] 去重
来源：http://nu.newstarts.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zs.yuntaijiaju.cn

PHP:  array_unique($arr);
来源：http://ao.huixiangedu.cn

JS:   [...new Set(arr)]
来源：http://hc.panjiajie.cn

TS:   [...new Set(arr)]
来源：http://zt.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lk.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ik.newstarts.cn

Ruby: arr.uniq
来源：http://bv.szxytkj.cn

C#:   list.Distinct().ToList()
来源：http://jy.521024.cn

[D16] 求和与平均值
来源：http://qx.nszjky.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://sq.huanxung.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yn.huixiangedu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bg.bookmarksfly.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fp.haigaiapp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cn.yuexingan06.cn

Go:   // 手写循环累加
来源：http://dt.muxihuayi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ed.bookmarksfly.cn

C#:   list.Sum();  list.Average()
来源：http://wc.chemitech.net.cn

[D17] 最大值与最小值
来源：http://tm.colortex.cn

Py:   max(arr);  min(arr)
来源：http://ws.hahajie.cn

PHP:  max($arr);  min($arr);
来源：http://uk.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://la.asd995.cn

TS:   Math.max(...arr);
来源：http://ad.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wp.521024.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ba.huixiangedu.cn

Ruby: arr.max;  arr.min
来源：http://sh.newstarts.cn

C#:   list.Max();  list.Min()
来源：http://tv.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://ue.chemitech.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tw.jianghongdianzi.cn

PHP:  array_merge(...$nested);
来源：http://um.huixiangedu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nf.szsharing.cn

TS:   nested.flat();
来源：http://he.huixiangedu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dx.szsharing.cn

Go:   // 手写双层循环
来源：http://ws.haigaiapp.cn

Ruby: nested.flatten
来源：http://cb.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ki.lnxyls.cn

[D19] 按字段分组
来源：http://ul.panjiajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://br.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oh.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mw.shxzukj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xj.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ve.huixinmuqiang.cn

Go:   // 手写 map[string][]T
来源：http://zi.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mk.gzmigu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eo.huixinmuqiang.cn

[D20] 统计每个元素出现次数
来源：http://dx.jianghongdianzi.cn

Py:   Counter(arr)
来源：http://ha.521024.cn

PHP:  array_count_values($arr);
来源：http://rv.bjjhwx.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uf.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gu.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kj.colortex.cn

Go:   // 手写 map[T]int
来源：http://cr.shtwfgs.cn

Ruby: arr.tally
来源：http://sf.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jq.szxytkj.cn

[D21] 判断是否包含某元素
来源：http://ud.chemitech.net.cn

Py:   x in arr
来源：http://ul.shxzukj.cn

PHP:  in_array($x, $arr, true);
来源：http://bv.yuntaijiaju.cn

JS:   arr.includes(x)
来源：http://ol.hnjuh.cn

TS:   arr.includes(x)
来源：http://fz.szsharing.cn

Java: list.contains(x)
来源：http://js.hnjuh.cn

Go:   slices.Contains(arr, x)
来源：http://qo.yuexingan06.cn

Ruby: arr.include?(x)
来源：http://uk.szsharing.cn

C#:   list.Contains(x)
来源：http://yo.muxihuayi.cn

[D22] 复制数组（避免共享引用）
来源：http://ux.szxytkj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wo.huixiangedu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://me.yuexingan06.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ph.panjiajie.cn

TS:   [...arr];
来源：http://qr.muxihuayi.cn

Java: new ArrayList<>(list);
来源：http://lw.panjiajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jq.521024.cn

Ruby: arr.dup;  arr.clone
来源：http://or.jianghongdianzi.cn

C#:   new List<int>(list);
来源：http://xx.bjjhwx.cn

[D23] reduce 累积计算
来源：http://fk.nszjky.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wh.huixiangedu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bl.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ky.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ic.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://un.newstarts.cn

Go:   // 手写循环
来源：http://oc.bjjhwx.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uc.lnxyls.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fp.shtwfgs.cn

[D24] 字典 / Map 基本操作
来源：http://us.hahajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ld.shxzukj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oj.szxytkj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cm.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://lu.huixinmuqiang.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cl.lnxyls.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kr.bookmarksfly.cn


<!-- 参考信息 -->