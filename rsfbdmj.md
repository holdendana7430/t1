代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qn.huixiangedu.cn

TS:   arr.map(String)
来源：http://lv.9csxet.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://zk.szsharing.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ye.lnxyls.cn

Ruby: arr.map(&:upcase)
来源：http://id.yuexingan06.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://di.bjjhwx.cn

[C08] 闭包
来源：http://dp.jctech888.com.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://gx.shxzskj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://tn.jianghongdianzi.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pn.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://lr.9csxet.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://bl.colortex.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mk.yuntaijiaju.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://nr.hahajie.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://qn.panjiajie.cn

[C09] 递归
来源：http://er.yuntaijiaju.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ci.yuexingan06.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bz.nszjky.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ol.shtwfgs.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qw.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://vn.jianghongdianzi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://cd.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://qv.hahajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://au.shtwfgs.cn

[C10] 变量作用域
来源：http://dl.huixiangedu.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vq.newstarts.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lz.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hu.newstarts.cn

TS:   同 JS
来源：http://sk.521024.cn

Java: 方法内为块级作用域
来源：http://qg.bjjhwx.cn

Go:   花括号块级作用域
来源：http://hy.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zx.shtwfgs.cn

C#:   块级作用域
来源：http://ly.panjiajie.cn

[C11] 模块导入与导出
来源：http://yw.szsharing.cn

Py:   from module import func
来源：http://pi.yuntaijiaju.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bo.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://uq.lnxyls.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ea.bookmarksfly.cn

Java: import java.util.List;
来源：http://si.newstarts.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uc.muxihuayi.cn

Ruby: require "json"; require_relative "./util"
来源：http://uq.asd995.cn

C#:   using System.Text;
来源：http://uz.lnxyls.cn

[C12] 立即执行函数 IIFE
来源：http://fw.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://ya.huixiangedu.cn

PHP:  (function () { echo "run"; })();
来源：http://wj.hnjuh.cn

JS:   (() => { console.log("run"); })();
来源：http://pu.huixinmuqiang.cn

TS:   (() => { console.log("run"); })();
来源：http://zo.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jv.colortex.cn

Go:   func() { fmt.Println("run") }()
来源：http://vd.bjjhwx.cn

Ruby: -> { puts "run" }.call
来源：http://kw.521024.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ek.szxytkj.cn

[C13] 类型声明 / 类型注解
来源：http://jk.yuexingan06.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ge.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ol.nszjky.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://al.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uj.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://md.colortex.cn

Go:   func add(a, b int) int
来源：http://hs.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://oa.huixinmuqiang.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gh.nszjky.cn

[C14] 泛型函数
来源：http://yj.shxzukj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://oa.521024.cn

PHP:  // 无泛型
来源：http://jo.bjjhwx.cn

JS:   // 无泛型
来源：http://si.nszjky.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://it.shtwfgs.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://if.jctech888.com.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cn.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://qv.szxytkj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wl.521024.cn

[C15] 解构 / 展开参数
来源：http://fr.haigaiapp.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://om.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://px.lnxyls.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fl.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ut.panjiajie.cn

Java: // 无解构
来源：http://tr.asd995.cn

Go:   // 无解构
来源：http://lw.bjjhwx.cn

Ruby: a, b = pair
来源：http://kj.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://xg.521024.cn

[C16] 函数 / 方法重载
来源：http://gl.jctech888.com.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nh.lnxyls.cn

PHP:  // 无重载
来源：http://gd.huanxung.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ck.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://kq.huanxung.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://lz.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://hn.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://gi.hahajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://es.gzmigu.cn

================================================================================
来源：http://sf.gzmigu.cn

D. 数组 / 列表 / 集合
来源：http://xi.yuntaijiaju.cn

================================================================================
来源：http://gu.shxzskj.cn

[D01] 创建数组 / 列表
来源：http://dd.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gb.newstarts.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wd.hahajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gq.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ab.521024.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://bo.bookmarksfly.cn

Go:   arr := []int{1, 2, 3}
来源：http://fz.newstarts.cn

Ruby: arr = [1, 2, 3]
来源：http://oi.hnjuh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xz.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://bt.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://jz.hahajie.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wf.jianghongdianzi.cn

JS:   arr.push(4);
来源：http://ug.huixiangedu.cn

TS:   arr.push(4);
来源：http://fc.jctech888.com.cn

Java: list.add(4);
来源：http://sd.nicolike.cn

Go:   arr = append(arr, 4)
来源：http://pu.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://cc.jianghongdianzi.cn

C#:   list.Add(4);
来源：http://kx.szxytkj.cn

[D03] 在指定位置插入元素
来源：http://pe.jctech888.com.cn

Py:   arr.insert(0, 0)
来源：http://bk.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://uo.asd995.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fh.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://uc.jianghongdianzi.cn

Java: list.add(0, 0);
来源：http://di.huixiangedu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ir.shtwfgs.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://it.chemitech.net.cn

C#:   list.Insert(0, 0);
来源：http://xg.nszjky.cn

[D04] 删除元素
来源：http://sr.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ib.9csxet.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ml.hahajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xx.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://as.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eb.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://eh.hahajie.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://eo.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fu.shxzukj.cn

[D05] 访问与修改元素
来源：http://hy.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ve.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hn.shtwfgs.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://eb.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://lq.huixinmuqiang.cn

Java: list.get(0); list.set(0, 9);
来源：http://um.nszjky.cn

Go:   arr[0]; arr[0] = 9
来源：http://by.shxzskj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://la.shxzskj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://er.shxzskj.cn

[D06] 数组长度
来源：http://ch.shtwfgs.cn

Py:   len(arr)
来源：http://tw.lnxyls.cn

PHP:  count($arr);
来源：http://ky.hahajie.cn

JS:   arr.length
来源：http://ww.jianghongdianzi.cn

TS:   arr.length
来源：http://xc.yuntaijiaju.cn

Java: list.size();
来源：http://zj.hahajie.cn

Go:   len(arr)
来源：http://vi.nszjky.cn

Ruby: arr.length; arr.size
来源：http://fd.hahajie.cn

C#:   list.Count;
来源：http://om.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://nb.chemitech.net.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hn.wgjwhj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yj.huixiangedu.cn

JS:   arr.slice(1, 4);
来源：http://tj.wgjwhj.cn

TS:   arr.slice(1, 4);
来源：http://ps.hnjuh.cn

Java: list.subList(1, 4);
来源：http://gn.panjiajie.cn

Go:   arr[1:4]
来源：http://yl.newstarts.cn

Ruby: arr[1, 3]
来源：http://vd.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://jb.shxzukj.cn

[D08] 合并两个数组
来源：http://bl.asd995.cn

Py:   a + b;  a.extend(b)
来源：http://ho.chemitech.net.cn

PHP:  array_merge($a, $b);
来源：http://jb.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rv.huixiangedu.cn

TS:   [...a, ...b];
来源：http://el.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://tk.szxytkj.cn

Go:   append(a, b...)
来源：http://ti.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://wf.newstarts.cn

C#:   a.Concat(b).ToList()
来源：http://oc.huixiangedu.cn

[D09] 排序（升序）
来源：http://ob.nicolike.cn

Py:   sorted(arr);  arr.sort()
来源：http://ii.szxytkj.cn

PHP:  sort($arr);
来源：http://tt.haigaiapp.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ym.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://iv.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ed.haigaiapp.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://se.bookmarksfly.cn

Ruby: arr.sort
来源：http://af.nicolike.cn

C#:   list.Sort();
来源：http://wz.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lu.lnxyls.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gd.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gn.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ms.shtwfgs.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ko.asd995.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fo.huixinmuqiang.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dk.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vo.chemitech.net.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gy.shtwfgs.cn

[D11] 反转数组
来源：http://jo.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sg.szsharing.cn

PHP:  array_reverse($arr);
来源：http://eo.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qh.lnxyls.cn

TS:   [...arr].reverse();
来源：http://vz.shxzukj.cn

Java: Collections.reverse(list);
来源：http://rr.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://fu.jctech888.com.cn

Ruby: arr.reverse
来源：http://qk.szsharing.cn

C#:   list.Reverse();
来源：http://ny.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://og.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://js.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://oh.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yq.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sd.yuexingan06.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kn.521024.cn

Go:   slices.Index(arr, x)
来源：http://ob.nszjky.cn

Ruby: arr.index(x)
来源：http://xx.hahajie.cn

C#:   list.IndexOf(x);
来源：http://mh.lnxyls.cn

[D13] 过滤（保留满足条件的）
来源：http://ba.haigaiapp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sx.huanxung.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jv.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://sj.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://cu.bjjhwx.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://uf.szxytkj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ko.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://rv.hnjuh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pz.hahajie.cn

[D14] 映射转换（每个元素变形）
来源：http://nz.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://um.hnjuh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://oh.colortex.cn

JS:   arr.map(x => x * 2)
来源：http://rw.9csxet.cn

TS:   arr.map(x => x * 2)
来源：http://qr.shtwfgs.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rk.jctech888.com.cn

Go:   // 手写循环
来源：http://hy.szsharing.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ay.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vg.gzmigu.cn

[D15] 去重
来源：http://wc.yuexingan06.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://zh.jianghongdianzi.cn

PHP:  array_unique($arr);
来源：http://ho.9csxet.cn

JS:   [...new Set(arr)]
来源：http://nr.colortex.cn

TS:   [...new Set(arr)]
来源：http://no.huixiangedu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ih.nszjky.cn

Go:   // 用 map[T]struct{} 手写
来源：http://gg.hnjuh.cn

Ruby: arr.uniq
来源：http://cj.shxzskj.cn

C#:   list.Distinct().ToList()
来源：http://rc.chemitech.net.cn

[D16] 求和与平均值
来源：http://qi.jctech888.com.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ea.huanxung.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mu.szxytkj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://lq.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://eb.gzmigu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://jb.haigaiapp.cn

Go:   // 手写循环累加
来源：http://zu.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pr.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://hi.9csxet.cn

[D17] 最大值与最小值
来源：http://bb.yuntaijiaju.cn

Py:   max(arr);  min(arr)
来源：http://gm.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://el.colortex.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://eu.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://yp.9csxet.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pu.9csxet.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hw.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://hu.shxzskj.cn

C#:   list.Max();  list.Min()
来源：http://eg.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://hu.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xa.colortex.cn

PHP:  array_merge(...$nested);
来源：http://zw.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ae.szsharing.cn

TS:   nested.flat();
来源：http://om.haigaiapp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hi.colortex.cn

Go:   // 手写双层循环
来源：http://ba.gzmigu.cn

Ruby: nested.flatten
来源：http://of.yuexingan06.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://eb.asd995.cn

[D19] 按字段分组
来源：http://sq.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jy.nicolike.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ia.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qh.nicolike.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xb.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fs.nszjky.cn

Go:   // 手写 map[string][]T
来源：http://pb.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cp.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://dl.haigaiapp.cn

[D20] 统计每个元素出现次数
来源：http://yx.lnxyls.cn

Py:   Counter(arr)
来源：http://jl.colortex.cn

PHP:  array_count_values($arr);
来源：http://gn.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://aq.shxzskj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ua.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hl.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://pr.huanxung.cn

Ruby: arr.tally
来源：http://kn.shxzskj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fo.hahajie.cn

[D21] 判断是否包含某元素
来源：http://zz.jctech888.com.cn

Py:   x in arr
来源：http://qd.jctech888.com.cn

PHP:  in_array($x, $arr, true);
来源：http://bh.asd995.cn

JS:   arr.includes(x)
来源：http://tc.shxzukj.cn

TS:   arr.includes(x)
来源：http://yw.hahajie.cn

Java: list.contains(x)
来源：http://ie.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://zh.9csxet.cn

Ruby: arr.include?(x)
来源：http://ed.lnxyls.cn

C#:   list.Contains(x)
来源：http://bn.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://rf.wgjwhj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kc.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oc.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ct.huixiangedu.cn

TS:   [...arr];
来源：http://ex.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://ib.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qa.9csxet.cn

Ruby: arr.dup;  arr.clone
来源：http://sq.9csxet.cn

C#:   new List<int>(list);
来源：http://cs.szsharing.cn

[D23] reduce 累积计算
来源：http://wq.nicolike.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mt.shxzukj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hx.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://je.bjjhwx.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yi.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ok.muxihuayi.cn

Go:   // 手写循环
来源：http://jk.asd995.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rx.wgjwhj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://et.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://km.bookmarksfly.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cf.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://vj.nicolike.cn


<!-- 参考信息 -->