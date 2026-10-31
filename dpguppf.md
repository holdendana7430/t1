代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://yk.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://tn.jianghongdianzi.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ji.chemitech.net.cn

[C09] 递归
来源：http://fo.huanxung.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ls.colortex.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ok.huanxung.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ia.nszjky.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bo.bookmarksfly.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://il.bookmarksfly.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://lk.9csxet.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://fn.jctech888.com.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://dc.shxzukj.cn

[C10] 变量作用域
来源：http://el.muxihuayi.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ot.chemitech.net.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kj.shxzukj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://cn.huixinmuqiang.cn

TS:   同 JS
来源：http://ig.asd995.cn

Java: 方法内为块级作用域
来源：http://iz.szsharing.cn

Go:   花括号块级作用域
来源：http://rw.bjjhwx.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ih.yuntaijiaju.cn

C#:   块级作用域
来源：http://dw.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://bp.huixinmuqiang.cn

Py:   from module import func
来源：http://bk.gzmigu.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ld.shxzskj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ot.shtwfgs.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://au.hahajie.cn

Java: import java.util.List;
来源：http://fs.huixinmuqiang.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://dl.9csxet.cn

Ruby: require "json"; require_relative "./util"
来源：http://cc.bjjhwx.cn

C#:   using System.Text;
来源：http://ra.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://vy.szxytkj.cn

Py:   (lambda: print("run"))()
来源：http://vu.wgjwhj.cn

PHP:  (function () { echo "run"; })();
来源：http://xn.nicolike.cn

JS:   (() => { console.log("run"); })();
来源：http://id.9csxet.cn

TS:   (() => { console.log("run"); })();
来源：http://wm.shtwfgs.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://vk.nicolike.cn

Go:   func() { fmt.Println("run") }()
来源：http://wv.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://ts.szsharing.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cj.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://uo.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sr.huanxung.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ci.9csxet.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://kt.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://vz.szsharing.cn

Java: int add(int a, int b) { return a + b; }
来源：http://co.huanxung.cn

Go:   func add(a, b int) int
来源：http://re.bookmarksfly.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ws.huanxung.cn

C#:   int Add(int a, int b) => a + b;
来源：http://td.szsharing.cn

[C14] 泛型函数
来源：http://gy.nszjky.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zj.panjiajie.cn

PHP:  // 无泛型
来源：http://ut.chemitech.net.cn

JS:   // 无泛型
来源：http://eh.nszjky.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hr.bookmarksfly.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rg.lnxyls.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ms.521024.cn

Ruby: # 无泛型
来源：http://wz.asd995.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pc.gzmigu.cn

[C15] 解构 / 展开参数
来源：http://uz.panjiajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://jn.521024.cn

PHP:  [$a, $b] = $pair;
来源：http://ke.jctech888.com.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mo.shtwfgs.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ff.shtwfgs.cn

Java: // 无解构
来源：http://pt.yuexingan06.cn

Go:   // 无解构
来源：http://wk.wgjwhj.cn

Ruby: a, b = pair
来源：http://ec.huanxung.cn

C#:   var (a, b) = pair;
来源：http://kb.szxytkj.cn

[C16] 函数 / 方法重载
来源：http://st.jianghongdianzi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://go.shxzskj.cn

PHP:  // 无重载
来源：http://op.huanxung.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rr.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://sz.jianghongdianzi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hq.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://cl.yuntaijiaju.cn

Ruby: # 无重载：靠动态参数
来源：http://dj.huixiangedu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://vy.521024.cn

================================================================================
来源：http://wc.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://hl.shxzskj.cn

================================================================================
来源：http://jx.szsharing.cn

[D01] 创建数组 / 列表
来源：http://ip.gzmigu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://cj.bjjhwx.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://dt.lnxyls.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ka.hnjuh.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dh.shxzskj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://we.521024.cn

Go:   arr := []int{1, 2, 3}
来源：http://zt.9csxet.cn

Ruby: arr = [1, 2, 3]
来源：http://sj.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://lb.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://oa.shxzskj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://nr.bookmarksfly.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oc.wgjwhj.cn

JS:   arr.push(4);
来源：http://di.lnxyls.cn

TS:   arr.push(4);
来源：http://dt.yuexingan06.cn

Java: list.add(4);
来源：http://mq.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://gx.shtwfgs.cn

Ruby: arr << 4; arr.push(5)
来源：http://yl.nicolike.cn

C#:   list.Add(4);
来源：http://em.9csxet.cn

[D03] 在指定位置插入元素
来源：http://pg.huixinmuqiang.cn

Py:   arr.insert(0, 0)
来源：http://ip.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://na.haigaiapp.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ar.hahajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://hu.hnjuh.cn

Java: list.add(0, 0);
来源：http://pm.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qq.haigaiapp.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://zz.gzmigu.cn

C#:   list.Insert(0, 0);
来源：http://oo.wgjwhj.cn

[D04] 删除元素
来源：http://ig.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://oi.asd995.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://by.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://nq.huixinmuqiang.cn

TS:   arr.splice(0, 1);
来源：http://ek.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yo.jctech888.com.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ki.yuntaijiaju.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://og.muxihuayi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bn.panjiajie.cn

[D05] 访问与修改元素
来源：http://qv.newstarts.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kb.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yb.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mh.jctech888.com.cn

TS:   arr[0]; arr.at(-1);
来源：http://ga.9csxet.cn

Java: list.get(0); list.set(0, 9);
来源：http://oz.shtwfgs.cn

Go:   arr[0]; arr[0] = 9
来源：http://cv.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ds.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lx.szsharing.cn

[D06] 数组长度
来源：http://yt.521024.cn

Py:   len(arr)
来源：http://qk.wgjwhj.cn

PHP:  count($arr);
来源：http://cp.haigaiapp.cn

JS:   arr.length
来源：http://kk.newstarts.cn

TS:   arr.length
来源：http://pc.chemitech.net.cn

Java: list.size();
来源：http://lg.hahajie.cn

Go:   len(arr)
来源：http://wu.bookmarksfly.cn

Ruby: arr.length; arr.size
来源：http://qb.muxihuayi.cn

C#:   list.Count;
来源：http://cg.szxytkj.cn

[D07] 切片 / 取子数组
来源：http://fv.muxihuayi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ge.huixiangedu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zf.shxzskj.cn

JS:   arr.slice(1, 4);
来源：http://ke.hahajie.cn

TS:   arr.slice(1, 4);
来源：http://wg.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://sm.bookmarksfly.cn

Go:   arr[1:4]
来源：http://sa.wgjwhj.cn

Ruby: arr[1, 3]
来源：http://tj.asd995.cn

C#:   list.GetRange(1, 3);
来源：http://ka.9csxet.cn

[D08] 合并两个数组
来源：http://tm.521024.cn

Py:   a + b;  a.extend(b)
来源：http://qt.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://lj.chemitech.net.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://kc.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://vq.gzmigu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://am.gzmigu.cn

Go:   append(a, b...)
来源：http://yz.huixinmuqiang.cn

Ruby: a + b;  a.concat(b)
来源：http://my.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://mc.haigaiapp.cn

[D09] 排序（升序）
来源：http://bu.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://ie.asd995.cn

PHP:  sort($arr);
来源：http://xf.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ht.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fx.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://me.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ze.haigaiapp.cn

Ruby: arr.sort
来源：http://ow.521024.cn

C#:   list.Sort();
来源：http://tr.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bf.bjjhwx.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bt.bjjhwx.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cb.9csxet.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xg.huanxung.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ut.chemitech.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ef.lnxyls.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rl.newstarts.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ye.gzmigu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xt.jianghongdianzi.cn

[D11] 反转数组
来源：http://mm.muxihuayi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qe.nicolike.cn

PHP:  array_reverse($arr);
来源：http://fi.lnxyls.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bn.chemitech.net.cn

TS:   [...arr].reverse();
来源：http://tf.szxytkj.cn

Java: Collections.reverse(list);
来源：http://wd.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://ly.asd995.cn

Ruby: arr.reverse
来源：http://cp.szxytkj.cn

C#:   list.Reverse();
来源：http://ta.yuexingan06.cn

[D12] 查找元素下标
来源：http://ni.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://fk.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hk.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xe.szsharing.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://px.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yr.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://zi.chemitech.net.cn

Ruby: arr.index(x)
来源：http://ki.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://ch.jctech888.com.cn

[D13] 过滤（保留满足条件的）
来源：http://gz.huanxung.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ft.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sj.yuntaijiaju.cn

JS:   arr.filter(x => x > 3)
来源：http://pf.nszjky.cn

TS:   arr.filter(x => x > 3)
来源：http://mp.panjiajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://bx.huixiangedu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xq.chemitech.net.cn

Ruby: arr.select { |x| x > 3 }
来源：http://eu.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pr.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://dq.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rf.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zm.shtwfgs.cn

JS:   arr.map(x => x * 2)
来源：http://cj.szxytkj.cn

TS:   arr.map(x => x * 2)
来源：http://kl.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sw.wgjwhj.cn

Go:   // 手写循环
来源：http://av.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://xf.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yv.newstarts.cn

[D15] 去重
来源：http://rm.yuntaijiaju.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://nv.nicolike.cn

PHP:  array_unique($arr);
来源：http://ra.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://cq.asd995.cn

TS:   [...new Set(arr)]
来源：http://ls.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lu.521024.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ko.521024.cn

Ruby: arr.uniq
来源：http://rr.szxytkj.cn

C#:   list.Distinct().ToList()
来源：http://ca.bookmarksfly.cn

[D16] 求和与平均值
来源：http://xt.nicolike.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bp.bookmarksfly.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xl.huixinmuqiang.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hk.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xc.szxytkj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xm.asd995.cn

Go:   // 手写循环累加
来源：http://vw.hnjuh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gh.shxzukj.cn

C#:   list.Sum();  list.Average()
来源：http://dt.hnjuh.cn

[D17] 最大值与最小值
来源：http://wu.szsharing.cn

Py:   max(arr);  min(arr)
来源：http://kb.huixiangedu.cn

PHP:  max($arr);  min($arr);
来源：http://ka.wgjwhj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bw.huanxung.cn

TS:   Math.max(...arr);
来源：http://el.newstarts.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ym.chemitech.net.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://sg.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://sz.bjjhwx.cn

C#:   list.Max();  list.Min()
来源：http://xn.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://hl.hnjuh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ow.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://gx.asd995.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://eh.gzmigu.cn

TS:   nested.flat();
来源：http://cn.szsharing.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kh.gzmigu.cn

Go:   // 手写双层循环
来源：http://nk.lnxyls.cn

Ruby: nested.flatten
来源：http://uc.wgjwhj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tz.shxzskj.cn

[D19] 按字段分组
来源：http://ip.huixinmuqiang.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zu.yuntaijiaju.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nd.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nz.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://nc.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://bm.521024.cn

Go:   // 手写 map[string][]T
来源：http://dg.nicolike.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qd.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pe.bookmarksfly.cn

[D20] 统计每个元素出现次数
来源：http://ep.szsharing.cn

Py:   Counter(arr)
来源：http://pa.hahajie.cn

PHP:  array_count_values($arr);
来源：http://ls.hnjuh.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jl.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ll.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mz.bookmarksfly.cn

Go:   // 手写 map[T]int
来源：http://qx.gzmigu.cn

Ruby: arr.tally
来源：http://pd.colortex.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dd.newstarts.cn

[D21] 判断是否包含某元素
来源：http://ki.newstarts.cn

Py:   x in arr
来源：http://dl.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://hd.huixiangedu.cn

JS:   arr.includes(x)
来源：http://mo.newstarts.cn

TS:   arr.includes(x)
来源：http://sd.shxzskj.cn

Java: list.contains(x)
来源：http://wu.asd995.cn

Go:   slices.Contains(arr, x)
来源：http://ot.panjiajie.cn

Ruby: arr.include?(x)
来源：http://ta.521024.cn

C#:   list.Contains(x)
来源：http://qc.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://gg.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://al.yuexingan06.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://uu.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mj.panjiajie.cn

TS:   [...arr];
来源：http://ig.asd995.cn

Java: new ArrayList<>(list);
来源：http://md.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jj.hnjuh.cn

Ruby: arr.dup;  arr.clone
来源：http://yx.newstarts.cn

C#:   new List<int>(list);
来源：http://qd.wgjwhj.cn

[D23] reduce 累积计算
来源：http://xj.jianghongdianzi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bf.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://uj.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rm.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ii.huixiangedu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://gh.muxihuayi.cn

Go:   // 手写循环
来源：http://ak.huixiangedu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vj.nszjky.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qk.huixinmuqiang.cn

[D24] 字典 / Map 基本操作
来源：http://lh.shtwfgs.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bv.newstarts.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xk.shtwfgs.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ys.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vz.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fb.huixinmuqiang.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uv.shxzskj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://lt.nszjky.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qc.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://uu.yuexingan06.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ft.panjiajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wi.asd995.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://fl.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ny.9csxet.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hf.colortex.cn


<!-- 参考信息 -->