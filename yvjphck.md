代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://cd.jianghongdianzi.cn

TS:   arr.map(String)
来源：http://ah.colortex.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://sg.nicolike.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://vl.jctech888.com.cn

Ruby: arr.map(&:upcase)
来源：http://fo.muxihuayi.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://lw.521024.cn

[C08] 闭包
来源：http://ck.yuntaijiaju.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kj.bjjhwx.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://im.lnxyls.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vm.hnjuh.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://tp.521024.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://ya.huanxung.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://rn.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://cp.jianghongdianzi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://zd.lnxyls.cn

[C09] 递归
来源：http://vo.jctech888.com.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://lb.huixiangedu.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://jw.szsharing.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://dj.nicolike.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fd.panjiajie.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rc.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://te.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ss.colortex.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://jm.colortex.cn

[C10] 变量作用域
来源：http://lp.jctech888.com.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nk.nicolike.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://sb.hnjuh.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://lz.jianghongdianzi.cn

TS:   同 JS
来源：http://xl.nicolike.cn

Java: 方法内为块级作用域
来源：http://kl.lnxyls.cn

Go:   花括号块级作用域
来源：http://vm.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://rd.szxytkj.cn

C#:   块级作用域
来源：http://uz.newstarts.cn

[C11] 模块导入与导出
来源：http://op.huixiangedu.cn

Py:   from module import func
来源：http://ks.yuntaijiaju.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://on.szsharing.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vl.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qi.colortex.cn

Java: import java.util.List;
来源：http://nx.jctech888.com.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eo.colortex.cn

Ruby: require "json"; require_relative "./util"
来源：http://rb.szsharing.cn

C#:   using System.Text;
来源：http://uw.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://gh.shxzskj.cn

Py:   (lambda: print("run"))()
来源：http://hg.nicolike.cn

PHP:  (function () { echo "run"; })();
来源：http://xt.szxytkj.cn

JS:   (() => { console.log("run"); })();
来源：http://gv.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://kv.shxzukj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fd.shxzukj.cn

Go:   func() { fmt.Println("run") }()
来源：http://ab.huanxung.cn

Ruby: -> { puts "run" }.call
来源：http://lw.shtwfgs.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cd.huanxung.cn

[C13] 类型声明 / 类型注解
来源：http://gl.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://pm.jctech888.com.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://qj.newstarts.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ld.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ag.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xq.nicolike.cn

Go:   func add(a, b int) int
来源：http://hz.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ps.szsharing.cn

C#:   int Add(int a, int b) => a + b;
来源：http://hh.huixinmuqiang.cn

[C14] 泛型函数
来源：http://pt.9csxet.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zm.asd995.cn

PHP:  // 无泛型
来源：http://yr.muxihuayi.cn

JS:   // 无泛型
来源：http://ia.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ju.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://pt.hahajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ih.shxzukj.cn

Ruby: # 无泛型
来源：http://xw.9csxet.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://zz.panjiajie.cn

[C15] 解构 / 展开参数
来源：http://ib.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://nu.jctech888.com.cn

PHP:  [$a, $b] = $pair;
来源：http://nu.gzmigu.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zv.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vf.chemitech.net.cn

Java: // 无解构
来源：http://ff.hnjuh.cn

Go:   // 无解构
来源：http://mz.nszjky.cn

Ruby: a, b = pair
来源：http://tm.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://ea.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://ul.jctech888.com.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://fu.gzmigu.cn

PHP:  // 无重载
来源：http://xh.shxzukj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://hg.bookmarksfly.cn

TS:   // 用联合类型或重载签名声明
来源：http://fw.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://rg.bookmarksfly.cn

Go:   // 无重载：用不同函数名
来源：http://ta.asd995.cn

Ruby: # 无重载：靠动态参数
来源：http://ep.521024.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bq.newstarts.cn

================================================================================
来源：http://zf.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://ha.shtwfgs.cn

================================================================================
来源：http://ky.szxytkj.cn

[D01] 创建数组 / 列表
来源：http://lx.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://as.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dh.yuntaijiaju.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wb.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yh.huanxung.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://yh.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://so.shxzskj.cn

Ruby: arr = [1, 2, 3]
来源：http://sc.nicolike.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hj.bjjhwx.cn

[D02] 追加元素到末尾
来源：http://se.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://xn.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wu.colortex.cn

JS:   arr.push(4);
来源：http://gv.bookmarksfly.cn

TS:   arr.push(4);
来源：http://hp.jctech888.com.cn

Java: list.add(4);
来源：http://qm.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://ht.huixiangedu.cn

Ruby: arr << 4; arr.push(5)
来源：http://xs.lnxyls.cn

C#:   list.Add(4);
来源：http://dn.yuexingan06.cn

[D03] 在指定位置插入元素
来源：http://cq.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://bt.panjiajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tu.yuexingan06.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sz.panjiajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://et.huixiangedu.cn

Java: list.add(0, 0);
来源：http://vu.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jd.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bp.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://rb.muxihuayi.cn

[D04] 删除元素
来源：http://tr.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wn.nszjky.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vg.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ae.nicolike.cn

TS:   arr.splice(0, 1);
来源：http://rf.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hl.hnjuh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xp.newstarts.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://xa.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://rq.huixiangedu.cn

[D05] 访问与修改元素
来源：http://at.wgjwhj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ho.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tj.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hb.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://wt.asd995.cn

Java: list.get(0); list.set(0, 9);
来源：http://rd.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://to.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://cs.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ob.lnxyls.cn

[D06] 数组长度
来源：http://ed.newstarts.cn

Py:   len(arr)
来源：http://gk.nicolike.cn

PHP:  count($arr);
来源：http://el.asd995.cn

JS:   arr.length
来源：http://iw.huixinmuqiang.cn

TS:   arr.length
来源：http://ma.wgjwhj.cn

Java: list.size();
来源：http://fq.panjiajie.cn

Go:   len(arr)
来源：http://ya.newstarts.cn

Ruby: arr.length; arr.size
来源：http://qc.colortex.cn

C#:   list.Count;
来源：http://wg.chemitech.net.cn

[D07] 切片 / 取子数组
来源：http://hr.muxihuayi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://lk.nicolike.cn

PHP:  array_slice($arr, 1, 3);
来源：http://si.jianghongdianzi.cn

JS:   arr.slice(1, 4);
来源：http://lr.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://ty.huanxung.cn

Java: list.subList(1, 4);
来源：http://go.asd995.cn

Go:   arr[1:4]
来源：http://du.lnxyls.cn

Ruby: arr[1, 3]
来源：http://mo.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://ta.hnjuh.cn

[D08] 合并两个数组
来源：http://vi.bookmarksfly.cn

Py:   a + b;  a.extend(b)
来源：http://ru.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://nx.asd995.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://hn.nicolike.cn

TS:   [...a, ...b];
来源：http://in.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://rw.bjjhwx.cn

Go:   append(a, b...)
来源：http://ci.huixinmuqiang.cn

Ruby: a + b;  a.concat(b)
来源：http://qa.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://ro.asd995.cn

[D09] 排序（升序）
来源：http://bh.asd995.cn

Py:   sorted(arr);  arr.sort()
来源：http://id.hahajie.cn

PHP:  sort($arr);
来源：http://nk.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://uh.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xt.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://vb.szsharing.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ps.nszjky.cn

Ruby: arr.sort
来源：http://iw.jctech888.com.cn

C#:   list.Sort();
来源：http://wj.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yr.shtwfgs.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wt.yuntaijiaju.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://vf.shtwfgs.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ri.jianghongdianzi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yl.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://io.wgjwhj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ec.huanxung.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://eq.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://zw.haigaiapp.cn

[D11] 反转数组
来源：http://yg.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://av.colortex.cn

PHP:  array_reverse($arr);
来源：http://th.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://at.panjiajie.cn

TS:   [...arr].reverse();
来源：http://nm.wgjwhj.cn

Java: Collections.reverse(list);
来源：http://tm.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://pn.bjjhwx.cn

Ruby: arr.reverse
来源：http://dp.asd995.cn

C#:   list.Reverse();
来源：http://ey.shxzskj.cn

[D12] 查找元素下标
来源：http://xf.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://ll.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kw.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ur.muxihuayi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cv.panjiajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wy.colortex.cn

Go:   slices.Index(arr, x)
来源：http://ja.bookmarksfly.cn

Ruby: arr.index(x)
来源：http://gd.hnjuh.cn

C#:   list.IndexOf(x);
来源：http://rj.newstarts.cn

[D13] 过滤（保留满足条件的）
来源：http://yd.huanxung.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cs.nicolike.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mo.huixiangedu.cn

JS:   arr.filter(x => x > 3)
来源：http://cb.yuexingan06.cn

TS:   arr.filter(x => x > 3)
来源：http://zu.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pu.huixiangedu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://id.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qw.wgjwhj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ir.bjjhwx.cn

[D14] 映射转换（每个元素变形）
来源：http://ow.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dk.shxzskj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://kv.colortex.cn

JS:   arr.map(x => x * 2)
来源：http://iv.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://zs.huixinmuqiang.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://he.shtwfgs.cn

Go:   // 手写循环
来源：http://op.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://sg.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ld.hnjuh.cn

[D15] 去重
来源：http://yv.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ez.hnjuh.cn

PHP:  array_unique($arr);
来源：http://cz.huanxung.cn

JS:   [...new Set(arr)]
来源：http://tr.huanxung.cn

TS:   [...new Set(arr)]
来源：http://zu.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bm.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nz.wgjwhj.cn

Ruby: arr.uniq
来源：http://ba.shxzskj.cn

C#:   list.Distinct().ToList()
来源：http://xe.szxytkj.cn

[D16] 求和与平均值
来源：http://pz.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fu.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://cs.newstarts.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ys.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zn.bookmarksfly.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zp.shxzukj.cn

Go:   // 手写循环累加
来源：http://rp.jctech888.com.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hj.shxzukj.cn

C#:   list.Sum();  list.Average()
来源：http://af.bookmarksfly.cn

[D17] 最大值与最小值
来源：http://ih.shtwfgs.cn

Py:   max(arr);  min(arr)
来源：http://gp.yuexingan06.cn

PHP:  max($arr);  min($arr);
来源：http://wz.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://uv.asd995.cn

TS:   Math.max(...arr);
来源：http://kg.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://vo.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sc.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://li.colortex.cn

C#:   list.Max();  list.Min()
来源：http://kc.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://uc.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sd.hnjuh.cn

PHP:  array_merge(...$nested);
来源：http://vg.jianghongdianzi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cb.nicolike.cn

TS:   nested.flat();
来源：http://xi.bookmarksfly.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uq.yuntaijiaju.cn

Go:   // 手写双层循环
来源：http://tw.hahajie.cn

Ruby: nested.flatten
来源：http://qi.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zf.bookmarksfly.cn

[D19] 按字段分组
来源：http://on.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qd.panjiajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qx.jianghongdianzi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ca.yuexingan06.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zh.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xd.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://sn.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qo.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qg.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://zr.shxzukj.cn

Py:   Counter(arr)
来源：http://nk.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://rx.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dq.lnxyls.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xl.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://oj.bjjhwx.cn

Go:   // 手写 map[T]int
来源：http://ch.colortex.cn

Ruby: arr.tally
来源：http://so.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://vr.wgjwhj.cn

[D21] 判断是否包含某元素
来源：http://ma.huanxung.cn

Py:   x in arr
来源：http://wh.muxihuayi.cn

PHP:  in_array($x, $arr, true);
来源：http://ov.lnxyls.cn

JS:   arr.includes(x)
来源：http://cl.bjjhwx.cn

TS:   arr.includes(x)
来源：http://pm.asd995.cn

Java: list.contains(x)
来源：http://fi.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://qx.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://cb.wgjwhj.cn

C#:   list.Contains(x)
来源：http://mk.panjiajie.cn

[D22] 复制数组（避免共享引用）
来源：http://ws.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wi.gzmigu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fr.nicolike.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gx.colortex.cn

TS:   [...arr];
来源：http://sj.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://md.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qb.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://il.shtwfgs.cn

C#:   new List<int>(list);
来源：http://hb.muxihuayi.cn

[D23] reduce 累积计算
来源：http://xf.521024.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://aa.yuntaijiaju.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wv.huixinmuqiang.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sv.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ka.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ay.muxihuayi.cn

Go:   // 手写循环
来源：http://rx.asd995.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lz.wgjwhj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fc.szsharing.cn

[D24] 字典 / Map 基本操作
来源：http://qi.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qr.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fn.nicolike.cn


<!-- 参考信息 -->