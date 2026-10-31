代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zo.hahajie.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pe.hahajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://od.asd995.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tl.nszjky.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wn.bookmarksfly.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hx.hnjuh.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ru.shxzskj.cn

[C09] 递归
来源：http://zy.shtwfgs.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tn.nszjky.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://se.jctech888.com.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://po.huixiangedu.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://tx.huanxung.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://np.jianghongdianzi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bp.chemitech.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://gj.panjiajie.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://eo.haigaiapp.cn

[C10] 变量作用域
来源：http://nl.yuntaijiaju.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://vf.muxihuayi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://da.521024.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bs.nszjky.cn

TS:   同 JS
来源：http://rq.colortex.cn

Java: 方法内为块级作用域
来源：http://cz.haigaiapp.cn

Go:   花括号块级作用域
来源：http://ts.nicolike.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fn.hnjuh.cn

C#:   块级作用域
来源：http://tw.haigaiapp.cn

[C11] 模块导入与导出
来源：http://jp.9csxet.cn

Py:   from module import func
来源：http://gx.szsharing.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sg.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fc.lnxyls.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ps.wgjwhj.cn

Java: import java.util.List;
来源：http://hc.shxzukj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xc.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://ly.colortex.cn

C#:   using System.Text;
来源：http://db.szsharing.cn

[C12] 立即执行函数 IIFE
来源：http://qi.muxihuayi.cn

Py:   (lambda: print("run"))()
来源：http://kt.521024.cn

PHP:  (function () { echo "run"; })();
来源：http://yp.yuexingan06.cn

JS:   (() => { console.log("run"); })();
来源：http://dt.gzmigu.cn

TS:   (() => { console.log("run"); })();
来源：http://nz.bjjhwx.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ec.shxzskj.cn

Go:   func() { fmt.Println("run") }()
来源：http://gs.wgjwhj.cn

Ruby: -> { puts "run" }.call
来源：http://lk.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ju.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://eu.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://st.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wy.muxihuayi.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ih.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ne.newstarts.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wb.hnjuh.cn

Go:   func add(a, b int) int
来源：http://qn.9csxet.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://bn.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sh.gzmigu.cn

[C14] 泛型函数
来源：http://bv.asd995.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xn.nszjky.cn

PHP:  // 无泛型
来源：http://tk.yuexingan06.cn

JS:   // 无泛型
来源：http://fp.jianghongdianzi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zh.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vj.yuexingan06.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://av.asd995.cn

Ruby: # 无泛型
来源：http://pm.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://kh.9csxet.cn

[C15] 解构 / 展开参数
来源：http://fn.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dr.nszjky.cn

PHP:  [$a, $b] = $pair;
来源：http://dn.wgjwhj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gd.haigaiapp.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pa.huixiangedu.cn

Java: // 无解构
来源：http://pm.yuntaijiaju.cn

Go:   // 无解构
来源：http://yu.huixiangedu.cn

Ruby: a, b = pair
来源：http://uu.huanxung.cn

C#:   var (a, b) = pair;
来源：http://ej.bjjhwx.cn

[C16] 函数 / 方法重载
来源：http://qm.gzmigu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://el.shtwfgs.cn

PHP:  // 无重载
来源：http://in.panjiajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://uu.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://ze.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wr.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://rh.huixinmuqiang.cn

Ruby: # 无重载：靠动态参数
来源：http://zp.bjjhwx.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://cj.hahajie.cn

================================================================================
来源：http://og.521024.cn

D. 数组 / 列表 / 集合
来源：http://hq.lnxyls.cn

================================================================================
来源：http://cs.yuntaijiaju.cn

[D01] 创建数组 / 列表
来源：http://dq.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://id.nicolike.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://my.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://js.yuntaijiaju.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yi.jctech888.com.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://lt.yuexingan06.cn

Go:   arr := []int{1, 2, 3}
来源：http://gu.521024.cn

Ruby: arr = [1, 2, 3]
来源：http://pg.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lu.panjiajie.cn

[D02] 追加元素到末尾
来源：http://ty.szxytkj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wp.bjjhwx.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nm.yuexingan06.cn

JS:   arr.push(4);
来源：http://fl.521024.cn

TS:   arr.push(4);
来源：http://me.bjjhwx.cn

Java: list.add(4);
来源：http://ts.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://jy.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://cd.nszjky.cn

C#:   list.Add(4);
来源：http://sh.huixinmuqiang.cn

[D03] 在指定位置插入元素
来源：http://fw.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://pi.nicolike.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ka.colortex.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://rh.yuexingan06.cn

TS:   arr.splice(0, 0, 0);
来源：http://oa.shtwfgs.cn

Java: list.add(0, 0);
来源：http://nt.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fj.shtwfgs.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://id.szxytkj.cn

C#:   list.Insert(0, 0);
来源：http://fz.jianghongdianzi.cn

[D04] 删除元素
来源：http://dg.huixinmuqiang.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://os.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://up.szxytkj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://gd.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://vm.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sm.shxzukj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ds.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yb.jianghongdianzi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zf.yuexingan06.cn

[D05] 访问与修改元素
来源：http://bp.shtwfgs.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://py.chemitech.net.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cz.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ch.hnjuh.cn

TS:   arr[0]; arr.at(-1);
来源：http://wp.jianghongdianzi.cn

Java: list.get(0); list.set(0, 9);
来源：http://cj.chemitech.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://jb.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://tj.shxzskj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kn.chemitech.net.cn

[D06] 数组长度
来源：http://sh.hnjuh.cn

Py:   len(arr)
来源：http://nr.shtwfgs.cn

PHP:  count($arr);
来源：http://ec.hahajie.cn

JS:   arr.length
来源：http://fl.huanxung.cn

TS:   arr.length
来源：http://xh.yuexingan06.cn

Java: list.size();
来源：http://qm.muxihuayi.cn

Go:   len(arr)
来源：http://cl.shtwfgs.cn

Ruby: arr.length; arr.size
来源：http://yr.bookmarksfly.cn

C#:   list.Count;
来源：http://bw.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://qq.lnxyls.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ue.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bn.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://il.chemitech.net.cn

TS:   arr.slice(1, 4);
来源：http://rr.huixinmuqiang.cn

Java: list.subList(1, 4);
来源：http://dw.newstarts.cn

Go:   arr[1:4]
来源：http://ju.jianghongdianzi.cn

Ruby: arr[1, 3]
来源：http://xs.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://dg.szxytkj.cn

[D08] 合并两个数组
来源：http://hp.521024.cn

Py:   a + b;  a.extend(b)
来源：http://jt.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://pn.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://or.szxytkj.cn

TS:   [...a, ...b];
来源：http://ab.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vz.bjjhwx.cn

Go:   append(a, b...)
来源：http://wn.nicolike.cn

Ruby: a + b;  a.concat(b)
来源：http://yf.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://ic.gzmigu.cn

[D09] 排序（升序）
来源：http://mm.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://fs.gzmigu.cn

PHP:  sort($arr);
来源：http://qd.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qx.nszjky.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hp.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zv.shxzskj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jh.shxzukj.cn

Ruby: arr.sort
来源：http://bo.huanxung.cn

C#:   list.Sort();
来源：http://mo.yuexingan06.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://pq.yuexingan06.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://at.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://pt.szxytkj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://go.hahajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bk.wgjwhj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ac.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cp.chemitech.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hi.jctech888.com.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://sl.jctech888.com.cn

[D11] 反转数组
来源：http://nx.lnxyls.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vk.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://sa.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ys.wgjwhj.cn

TS:   [...arr].reverse();
来源：http://sl.shxzukj.cn

Java: Collections.reverse(list);
来源：http://ek.shtwfgs.cn

Go:   slices.Reverse(arr)
来源：http://ab.hnjuh.cn

Ruby: arr.reverse
来源：http://ok.9csxet.cn

C#:   list.Reverse();
来源：http://qi.bjjhwx.cn

[D12] 查找元素下标
来源：http://vw.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://yn.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fa.yuntaijiaju.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jl.huixinmuqiang.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fa.yuntaijiaju.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cb.asd995.cn

Go:   slices.Index(arr, x)
来源：http://px.hnjuh.cn

Ruby: arr.index(x)
来源：http://vm.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://gj.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://ke.huanxung.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yi.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qb.huixiangedu.cn

JS:   arr.filter(x => x > 3)
来源：http://dr.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://zq.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qi.asd995.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://si.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jx.asd995.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://zn.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://sj.muxihuayi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://es.hahajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://eh.nicolike.cn

JS:   arr.map(x => x * 2)
来源：http://el.szxytkj.cn

TS:   arr.map(x => x * 2)
来源：http://dn.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vh.asd995.cn

Go:   // 手写循环
来源：http://km.newstarts.cn

Ruby: arr.map { |x| x * 2 }
来源：http://jg.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://tr.hnjuh.cn

[D15] 去重
来源：http://qx.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yk.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://fw.gzmigu.cn

JS:   [...new Set(arr)]
来源：http://at.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://sm.nszjky.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zx.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kz.nicolike.cn

Ruby: arr.uniq
来源：http://xh.szsharing.cn

C#:   list.Distinct().ToList()
来源：http://at.bookmarksfly.cn

[D16] 求和与平均值
来源：http://rc.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ua.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qj.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iz.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tj.newstarts.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ti.huixiangedu.cn

Go:   // 手写循环累加
来源：http://rv.hahajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dy.yuntaijiaju.cn

C#:   list.Sum();  list.Average()
来源：http://fc.bookmarksfly.cn

[D17] 最大值与最小值
来源：http://gg.521024.cn

Py:   max(arr);  min(arr)
来源：http://ai.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://ue.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gy.shxzskj.cn

TS:   Math.max(...arr);
来源：http://vb.nszjky.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ie.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zu.muxihuayi.cn

Ruby: arr.max;  arr.min
来源：http://iy.nszjky.cn

C#:   list.Max();  list.Min()
来源：http://cx.huixinmuqiang.cn

[D18] 扁平化嵌套数组
来源：http://bp.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qv.szxytkj.cn

PHP:  array_merge(...$nested);
来源：http://gy.jianghongdianzi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ee.9csxet.cn

TS:   nested.flat();
来源：http://ww.bjjhwx.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hf.bjjhwx.cn

Go:   // 手写双层循环
来源：http://us.huixiangedu.cn

Ruby: nested.flatten
来源：http://ka.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gh.shxzukj.cn

[D19] 按字段分组
来源：http://gg.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pk.nszjky.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fx.jianghongdianzi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yp.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ge.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zz.huixiangedu.cn

Go:   // 手写 map[string][]T
来源：http://na.colortex.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wc.panjiajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yu.bookmarksfly.cn

[D20] 统计每个元素出现次数
来源：http://kn.muxihuayi.cn

Py:   Counter(arr)
来源：http://jj.hahajie.cn

PHP:  array_count_values($arr);
来源：http://nc.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://it.jianghongdianzi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qv.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cd.wgjwhj.cn

Go:   // 手写 map[T]int
来源：http://qs.bjjhwx.cn

Ruby: arr.tally
来源：http://xz.shxzukj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://yc.yuexingan06.cn

[D21] 判断是否包含某元素
来源：http://am.bjjhwx.cn

Py:   x in arr
来源：http://dg.asd995.cn

PHP:  in_array($x, $arr, true);
来源：http://ib.nicolike.cn

JS:   arr.includes(x)
来源：http://xj.jctech888.com.cn

TS:   arr.includes(x)
来源：http://ug.huixinmuqiang.cn

Java: list.contains(x)
来源：http://ak.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://xi.shxzskj.cn

Ruby: arr.include?(x)
来源：http://lu.gzmigu.cn

C#:   list.Contains(x)
来源：http://ye.huixinmuqiang.cn

[D22] 复制数组（避免共享引用）
来源：http://bj.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://rs.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ws.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hn.panjiajie.cn

TS:   [...arr];
来源：http://vc.panjiajie.cn

Java: new ArrayList<>(list);
来源：http://di.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gt.shxzskj.cn

Ruby: arr.dup;  arr.clone
来源：http://wo.bjjhwx.cn

C#:   new List<int>(list);
来源：http://uq.nszjky.cn

[D23] reduce 累积计算
来源：http://ze.asd995.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qm.haigaiapp.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qc.shtwfgs.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kg.szxytkj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zg.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ak.huixiangedu.cn

Go:   // 手写循环
来源：http://fw.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qf.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kj.shxzskj.cn

[D24] 字典 / Map 基本操作
来源：http://lq.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gj.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ll.huixiangedu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://kk.yuntaijiaju.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qx.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ql.muxihuayi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dw.hahajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://br.521024.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gd.yuntaijiaju.cn

[D25] Set 集合去重与交并差
来源：http://xf.shxzskj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://da.9csxet.cn


<!-- 参考信息 -->