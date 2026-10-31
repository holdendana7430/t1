代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://tv.haigaiapp.cn

TS:   arr.map(String)
来源：http://bm.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ad.bjjhwx.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://fw.521024.cn

Ruby: arr.map(&:upcase)
来源：http://rp.asd995.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ll.jianghongdianzi.cn

[C08] 闭包
来源：http://rz.chemitech.net.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://eh.szsharing.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://us.panjiajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ow.huixinmuqiang.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://et.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://kp.huixiangedu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hr.hnjuh.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://gn.gzmigu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://fi.nicolike.cn

[C09] 递归
来源：http://yo.521024.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://my.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://am.hahajie.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://vn.colortex.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gb.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kc.shtwfgs.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://oh.shtwfgs.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ry.9csxet.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://er.yuexingan06.cn

[C10] 变量作用域
来源：http://fb.nszjky.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mp.lnxyls.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jj.9csxet.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://au.huixiangedu.cn

TS:   同 JS
来源：http://un.nszjky.cn

Java: 方法内为块级作用域
来源：http://sx.shtwfgs.cn

Go:   花括号块级作用域
来源：http://zo.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://yv.huixiangedu.cn

C#:   块级作用域
来源：http://lo.lnxyls.cn

[C11] 模块导入与导出
来源：http://hj.nszjky.cn

Py:   from module import func
来源：http://vi.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zf.jctech888.com.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fq.521024.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://us.szxytkj.cn

Java: import java.util.List;
来源：http://kz.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://bj.bjjhwx.cn

Ruby: require "json"; require_relative "./util"
来源：http://oo.szsharing.cn

C#:   using System.Text;
来源：http://xi.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://ig.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://ds.bookmarksfly.cn

PHP:  (function () { echo "run"; })();
来源：http://ms.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://ck.shxzukj.cn

TS:   (() => { console.log("run"); })();
来源：http://ij.szsharing.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vu.newstarts.cn

Go:   func() { fmt.Println("run") }()
来源：http://ue.huixinmuqiang.cn

Ruby: -> { puts "run" }.call
来源：http://uv.shxzskj.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://sh.szxytkj.cn

[C13] 类型声明 / 类型注解
来源：http://hy.newstarts.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://aq.panjiajie.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yi.szsharing.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jd.bjjhwx.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://gm.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yl.asd995.cn

Go:   func add(a, b int) int
来源：http://xq.yuntaijiaju.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://nm.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://uy.szsharing.cn

[C14] 泛型函数
来源：http://zj.shxzskj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wp.asd995.cn

PHP:  // 无泛型
来源：http://ab.wgjwhj.cn

JS:   // 无泛型
来源：http://xs.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jf.lnxyls.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mk.yuntaijiaju.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vd.jctech888.com.cn

Ruby: # 无泛型
来源：http://vt.bookmarksfly.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://jd.huixiangedu.cn

[C15] 解构 / 展开参数
来源：http://ru.huanxung.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://tw.9csxet.cn

PHP:  [$a, $b] = $pair;
来源：http://bk.szxytkj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tu.jctech888.com.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qr.haigaiapp.cn

Java: // 无解构
来源：http://ju.asd995.cn

Go:   // 无解构
来源：http://ot.jctech888.com.cn

Ruby: a, b = pair
来源：http://ng.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://kf.panjiajie.cn

[C16] 函数 / 方法重载
来源：http://kj.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mx.panjiajie.cn

PHP:  // 无重载
来源：http://sk.huanxung.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://no.colortex.cn

TS:   // 用联合类型或重载签名声明
来源：http://am.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://et.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://ai.nicolike.cn

Ruby: # 无重载：靠动态参数
来源：http://cu.szsharing.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pi.szsharing.cn

================================================================================
来源：http://nn.yuntaijiaju.cn

D. 数组 / 列表 / 集合
来源：http://ht.panjiajie.cn

================================================================================
来源：http://vq.nicolike.cn

[D01] 创建数组 / 列表
来源：http://dz.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xm.colortex.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ex.shxzskj.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pm.jctech888.com.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nl.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tv.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://ee.shxzukj.cn

Ruby: arr = [1, 2, 3]
来源：http://ri.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ro.muxihuayi.cn

[D02] 追加元素到末尾
来源：http://ga.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://me.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oz.haigaiapp.cn

JS:   arr.push(4);
来源：http://fx.shxzukj.cn

TS:   arr.push(4);
来源：http://ma.yuexingan06.cn

Java: list.add(4);
来源：http://my.nszjky.cn

Go:   arr = append(arr, 4)
来源：http://ec.haigaiapp.cn

Ruby: arr << 4; arr.push(5)
来源：http://rj.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://zk.shtwfgs.cn

[D03] 在指定位置插入元素
来源：http://fe.shxzukj.cn

Py:   arr.insert(0, 0)
来源：http://wf.9csxet.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://pt.bjjhwx.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cd.wgjwhj.cn

TS:   arr.splice(0, 0, 0);
来源：http://oo.chemitech.net.cn

Java: list.add(0, 0);
来源：http://mz.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://xe.shxzukj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://es.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://km.yuexingan06.cn

[D04] 删除元素
来源：http://ml.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://dj.wgjwhj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://iz.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mt.asd995.cn

TS:   arr.splice(0, 1);
来源：http://ng.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rt.asd995.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sp.shtwfgs.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sm.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://on.shtwfgs.cn

[D05] 访问与修改元素
来源：http://hk.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ml.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://iw.lnxyls.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zd.bookmarksfly.cn

TS:   arr[0]; arr.at(-1);
来源：http://ge.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://qk.huixinmuqiang.cn

Go:   arr[0]; arr[0] = 9
来源：http://sp.shxzukj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xv.szxytkj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://oq.gzmigu.cn

[D06] 数组长度
来源：http://lg.muxihuayi.cn

Py:   len(arr)
来源：http://sb.huixinmuqiang.cn

PHP:  count($arr);
来源：http://ip.9csxet.cn

JS:   arr.length
来源：http://mk.wgjwhj.cn

TS:   arr.length
来源：http://cw.szsharing.cn

Java: list.size();
来源：http://xw.colortex.cn

Go:   len(arr)
来源：http://mz.521024.cn

Ruby: arr.length; arr.size
来源：http://ba.bookmarksfly.cn

C#:   list.Count;
来源：http://vf.9csxet.cn

[D07] 切片 / 取子数组
来源：http://hr.lnxyls.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fh.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bu.huanxung.cn

JS:   arr.slice(1, 4);
来源：http://yl.hnjuh.cn

TS:   arr.slice(1, 4);
来源：http://ze.szsharing.cn

Java: list.subList(1, 4);
来源：http://pr.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://gq.bjjhwx.cn

Ruby: arr[1, 3]
来源：http://cc.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://tn.jctech888.com.cn

[D08] 合并两个数组
来源：http://dd.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://sv.szxytkj.cn

PHP:  array_merge($a, $b);
来源：http://ya.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://be.nicolike.cn

TS:   [...a, ...b];
来源：http://dg.lnxyls.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lr.hnjuh.cn

Go:   append(a, b...)
来源：http://oi.newstarts.cn

Ruby: a + b;  a.concat(b)
来源：http://fu.haigaiapp.cn

C#:   a.Concat(b).ToList()
来源：http://cs.nicolike.cn

[D09] 排序（升序）
来源：http://el.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://yu.panjiajie.cn

PHP:  sort($arr);
来源：http://nr.lnxyls.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://kl.hahajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qc.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ir.bjjhwx.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ow.muxihuayi.cn

Ruby: arr.sort
来源：http://kn.lnxyls.cn

C#:   list.Sort();
来源：http://af.haigaiapp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://jk.szsharing.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ic.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ms.gzmigu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wt.jctech888.com.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://xx.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://yi.huixinmuqiang.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nd.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ks.nszjky.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://kc.bookmarksfly.cn

[D11] 反转数组
来源：http://rn.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rl.newstarts.cn

PHP:  array_reverse($arr);
来源：http://ym.haigaiapp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jt.shxzskj.cn

TS:   [...arr].reverse();
来源：http://yc.wgjwhj.cn

Java: Collections.reverse(list);
来源：http://xi.wgjwhj.cn

Go:   slices.Reverse(arr)
来源：http://dd.hnjuh.cn

Ruby: arr.reverse
来源：http://mj.shtwfgs.cn

C#:   list.Reverse();
来源：http://ty.muxihuayi.cn

[D12] 查找元素下标
来源：http://nm.jctech888.com.cn

Py:   arr.index(x);  x in arr
来源：http://fw.shxzskj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rw.nszjky.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ow.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qv.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wu.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://zm.wgjwhj.cn

Ruby: arr.index(x)
来源：http://lx.nszjky.cn

C#:   list.IndexOf(x);
来源：http://gb.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://nm.yuntaijiaju.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pw.huixiangedu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yd.521024.cn

JS:   arr.filter(x => x > 3)
来源：http://go.haigaiapp.cn

TS:   arr.filter(x => x > 3)
来源：http://rc.huanxung.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ic.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bi.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://eu.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ay.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://ek.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ej.haigaiapp.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lf.huixiangedu.cn

JS:   arr.map(x => x * 2)
来源：http://zm.asd995.cn

TS:   arr.map(x => x * 2)
来源：http://iu.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ix.9csxet.cn

Go:   // 手写循环
来源：http://uv.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fu.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://lw.nicolike.cn

[D15] 去重
来源：http://ng.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yc.nicolike.cn

PHP:  array_unique($arr);
来源：http://wy.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://se.hahajie.cn

TS:   [...new Set(arr)]
来源：http://tk.huixinmuqiang.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qu.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://se.shxzskj.cn

Ruby: arr.uniq
来源：http://sz.huanxung.cn

C#:   list.Distinct().ToList()
来源：http://gp.nszjky.cn

[D16] 求和与平均值
来源：http://wh.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://db.lnxyls.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ab.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://jk.haigaiapp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mz.bjjhwx.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dh.shxzskj.cn

Go:   // 手写循环累加
来源：http://yd.panjiajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fm.szxytkj.cn

C#:   list.Sum();  list.Average()
来源：http://mj.hnjuh.cn

[D17] 最大值与最小值
来源：http://sy.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://fw.shxzukj.cn

PHP:  max($arr);  min($arr);
来源：http://sy.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xb.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://tq.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ls.wgjwhj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oz.chemitech.net.cn

Ruby: arr.max;  arr.min
来源：http://ur.shtwfgs.cn

C#:   list.Max();  list.Min()
来源：http://tf.nicolike.cn

[D18] 扁平化嵌套数组
来源：http://rp.jianghongdianzi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zl.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://bn.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://yl.jianghongdianzi.cn

TS:   nested.flat();
来源：http://je.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ht.nicolike.cn

Go:   // 手写双层循环
来源：http://cv.shxzukj.cn

Ruby: nested.flatten
来源：http://oz.hnjuh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xj.newstarts.cn

[D19] 按字段分组
来源：http://gg.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fh.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tj.huanxung.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://os.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zx.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bg.bjjhwx.cn

Go:   // 手写 map[string][]T
来源：http://vz.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bn.nszjky.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://vw.bjjhwx.cn

[D20] 统计每个元素出现次数
来源：http://ue.asd995.cn

Py:   Counter(arr)
来源：http://uk.521024.cn

PHP:  array_count_values($arr);
来源：http://qe.hahajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xm.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gt.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ko.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://pf.nszjky.cn

Ruby: arr.tally
来源：http://vm.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zq.huixinmuqiang.cn

[D21] 判断是否包含某元素
来源：http://qc.gzmigu.cn

Py:   x in arr
来源：http://mq.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://hn.szsharing.cn

JS:   arr.includes(x)
来源：http://ej.chemitech.net.cn

TS:   arr.includes(x)
来源：http://ct.shxzukj.cn

Java: list.contains(x)
来源：http://wg.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://ic.9csxet.cn

Ruby: arr.include?(x)
来源：http://mi.chemitech.net.cn

C#:   list.Contains(x)
来源：http://gh.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://qd.shtwfgs.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vh.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wy.nszjky.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ze.wgjwhj.cn

TS:   [...arr];
来源：http://lc.bookmarksfly.cn

Java: new ArrayList<>(list);
来源：http://vk.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://bp.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://cw.nicolike.cn

C#:   new List<int>(list);
来源：http://wk.huixinmuqiang.cn

[D23] reduce 累积计算
来源：http://jd.shxzskj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hd.lnxyls.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://go.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ru.yuntaijiaju.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eg.shxzukj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ma.panjiajie.cn

Go:   // 手写循环
来源：http://cx.newstarts.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://pp.yuntaijiaju.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pz.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://ff.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://qz.shxzukj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jh.huixinmuqiang.cn


<!-- 参考信息 -->