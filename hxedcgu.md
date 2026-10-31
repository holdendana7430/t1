代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://gq.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://ro.nszjky.cn

[C08] 闭包
来源：http://nd.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://zf.yuntaijiaju.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mu.huixinmuqiang.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://sj.asd995.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ms.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hv.szsharing.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qk.wgjwhj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://yk.szsharing.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://xw.gzmigu.cn

[C09] 递归
来源：http://jk.muxihuayi.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zh.bjjhwx.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://lj.gzmigu.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wx.9csxet.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://yi.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://gu.jianghongdianzi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://da.521024.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xn.wgjwhj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mv.wgjwhj.cn

[C10] 变量作用域
来源：http://ls.colortex.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://re.muxihuayi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://jb.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://fr.huanxung.cn

TS:   同 JS
来源：http://ji.shxzskj.cn

Java: 方法内为块级作用域
来源：http://ds.bookmarksfly.cn

Go:   花括号块级作用域
来源：http://ac.jctech888.com.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vf.shxzskj.cn

C#:   块级作用域
来源：http://pt.bjjhwx.cn

[C11] 模块导入与导出
来源：http://pm.521024.cn

Py:   from module import func
来源：http://ns.jianghongdianzi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://we.jctech888.com.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://du.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jz.panjiajie.cn

Java: import java.util.List;
来源：http://xo.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wt.newstarts.cn

Ruby: require "json"; require_relative "./util"
来源：http://dp.shxzukj.cn

C#:   using System.Text;
来源：http://te.szxytkj.cn

[C12] 立即执行函数 IIFE
来源：http://sq.wgjwhj.cn

Py:   (lambda: print("run"))()
来源：http://ao.panjiajie.cn

PHP:  (function () { echo "run"; })();
来源：http://fh.szxytkj.cn

JS:   (() => { console.log("run"); })();
来源：http://jl.huanxung.cn

TS:   (() => { console.log("run"); })();
来源：http://ow.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://fv.jctech888.com.cn

Go:   func() { fmt.Println("run") }()
来源：http://oo.wgjwhj.cn

Ruby: -> { puts "run" }.call
来源：http://uu.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yq.jctech888.com.cn

[C13] 类型声明 / 类型注解
来源：http://so.bookmarksfly.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qj.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://fe.shtwfgs.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://xk.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fk.newstarts.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ns.bookmarksfly.cn

Go:   func add(a, b int) int
来源：http://ag.bookmarksfly.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hl.huixiangedu.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vo.bookmarksfly.cn

[C14] 泛型函数
来源：http://ob.nszjky.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://uo.gzmigu.cn

PHP:  // 无泛型
来源：http://er.wgjwhj.cn

JS:   // 无泛型
来源：http://sk.muxihuayi.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bs.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://af.panjiajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ar.panjiajie.cn

Ruby: # 无泛型
来源：http://zg.huixiangedu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xh.jctech888.com.cn

[C15] 解构 / 展开参数
来源：http://tq.muxihuayi.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ew.lnxyls.cn

PHP:  [$a, $b] = $pair;
来源：http://qk.jianghongdianzi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://st.szxytkj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ok.yuexingan06.cn

Java: // 无解构
来源：http://lr.huixiangedu.cn

Go:   // 无解构
来源：http://sl.521024.cn

Ruby: a, b = pair
来源：http://zf.panjiajie.cn

C#:   var (a, b) = pair;
来源：http://vk.jctech888.com.cn

[C16] 函数 / 方法重载
来源：http://ul.huixinmuqiang.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ib.hnjuh.cn

PHP:  // 无重载
来源：http://od.muxihuayi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://th.haigaiapp.cn

TS:   // 用联合类型或重载签名声明
来源：http://xw.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wz.hnjuh.cn

Go:   // 无重载：用不同函数名
来源：http://fk.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://xx.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pv.jianghongdianzi.cn

================================================================================
来源：http://cd.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://ar.shxzukj.cn

================================================================================
来源：http://ah.shtwfgs.cn

[D01] 创建数组 / 列表
来源：http://oy.lnxyls.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fa.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ub.panjiajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lc.colortex.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://cs.521024.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pk.wgjwhj.cn

Go:   arr := []int{1, 2, 3}
来源：http://re.panjiajie.cn

Ruby: arr = [1, 2, 3]
来源：http://cd.asd995.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tr.szsharing.cn

[D02] 追加元素到末尾
来源：http://ma.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://by.nicolike.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://rw.lnxyls.cn

JS:   arr.push(4);
来源：http://hv.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://fk.gzmigu.cn

Java: list.add(4);
来源：http://lv.shtwfgs.cn

Go:   arr = append(arr, 4)
来源：http://gu.haigaiapp.cn

Ruby: arr << 4; arr.push(5)
来源：http://ly.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://wc.huanxung.cn

[D03] 在指定位置插入元素
来源：http://av.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://bt.colortex.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dr.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bn.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://em.huanxung.cn

Java: list.add(0, 0);
来源：http://tj.hnjuh.cn

Go:   arr = append([]int{0}, arr...)
来源：http://os.colortex.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://iu.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://fz.shxzukj.cn

[D04] 删除元素
来源：http://nc.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kq.szsharing.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://jz.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ql.hnjuh.cn

TS:   arr.splice(0, 1);
来源：http://mi.nicolike.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fv.yuexingan06.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zv.gzmigu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://fa.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://cs.gzmigu.cn

[D05] 访问与修改元素
来源：http://ea.muxihuayi.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ev.wgjwhj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fd.gzmigu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tr.panjiajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://wg.9csxet.cn

Java: list.get(0); list.set(0, 9);
来源：http://mt.nszjky.cn

Go:   arr[0]; arr[0] = 9
来源：http://av.wgjwhj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://al.jctech888.com.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://en.shtwfgs.cn

[D06] 数组长度
来源：http://hd.panjiajie.cn

Py:   len(arr)
来源：http://kc.hnjuh.cn

PHP:  count($arr);
来源：http://oz.gzmigu.cn

JS:   arr.length
来源：http://hp.gzmigu.cn

TS:   arr.length
来源：http://dr.9csxet.cn

Java: list.size();
来源：http://eo.chemitech.net.cn

Go:   len(arr)
来源：http://oi.hnjuh.cn

Ruby: arr.length; arr.size
来源：http://ny.chemitech.net.cn

C#:   list.Count;
来源：http://xd.chemitech.net.cn

[D07] 切片 / 取子数组
来源：http://hl.bookmarksfly.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ei.huanxung.cn

PHP:  array_slice($arr, 1, 3);
来源：http://vt.shxzukj.cn

JS:   arr.slice(1, 4);
来源：http://xb.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://xv.szsharing.cn

Java: list.subList(1, 4);
来源：http://ox.huanxung.cn

Go:   arr[1:4]
来源：http://fz.wgjwhj.cn

Ruby: arr[1, 3]
来源：http://pi.asd995.cn

C#:   list.GetRange(1, 3);
来源：http://if.szsharing.cn

[D08] 合并两个数组
来源：http://bp.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://ck.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://hz.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mj.haigaiapp.cn

TS:   [...a, ...b];
来源：http://bj.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wm.muxihuayi.cn

Go:   append(a, b...)
来源：http://jl.gzmigu.cn

Ruby: a + b;  a.concat(b)
来源：http://tx.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://zo.szsharing.cn

[D09] 排序（升序）
来源：http://kf.521024.cn

Py:   sorted(arr);  arr.sort()
来源：http://ta.huanxung.cn

PHP:  sort($arr);
来源：http://px.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://km.szxytkj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://oe.muxihuayi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qi.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yy.jctech888.com.cn

Ruby: arr.sort
来源：http://cx.nicolike.cn

C#:   list.Sort();
来源：http://fe.huanxung.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vy.yuexingan06.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lf.haigaiapp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://et.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://iy.shxzskj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://zi.jctech888.com.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ni.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bf.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oh.jianghongdianzi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://st.gzmigu.cn

[D11] 反转数组
来源：http://gf.haigaiapp.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pw.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://gk.521024.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xd.shxzukj.cn

TS:   [...arr].reverse();
来源：http://mj.szsharing.cn

Java: Collections.reverse(list);
来源：http://rc.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://wb.yuntaijiaju.cn

Ruby: arr.reverse
来源：http://bs.huanxung.cn

C#:   list.Reverse();
来源：http://we.szxytkj.cn

[D12] 查找元素下标
来源：http://pn.hahajie.cn

Py:   arr.index(x);  x in arr
来源：http://xu.szxytkj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ek.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ta.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bb.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://lu.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://lm.nicolike.cn

Ruby: arr.index(x)
来源：http://yv.hahajie.cn

C#:   list.IndexOf(x);
来源：http://co.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://ns.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ok.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://he.hahajie.cn

JS:   arr.filter(x => x > 3)
来源：http://jk.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://rf.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qr.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yf.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hm.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ut.9csxet.cn

[D14] 映射转换（每个元素变形）
来源：http://hx.chemitech.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dw.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://my.nicolike.cn

JS:   arr.map(x => x * 2)
来源：http://xa.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://zd.huanxung.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://uz.521024.cn

Go:   // 手写循环
来源：http://gy.asd995.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hc.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://cv.szsharing.cn

[D15] 去重
来源：http://ft.newstarts.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://pd.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://ef.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://nm.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://pd.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ol.nicolike.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jr.gzmigu.cn

Ruby: arr.uniq
来源：http://fn.szxytkj.cn

C#:   list.Distinct().ToList()
来源：http://aw.jianghongdianzi.cn

[D16] 求和与平均值
来源：http://is.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tm.shtwfgs.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nh.lnxyls.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://va.wgjwhj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lx.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xp.huixiangedu.cn

Go:   // 手写循环累加
来源：http://fm.hahajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yi.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://zz.hahajie.cn

[D17] 最大值与最小值
来源：http://az.bjjhwx.cn

Py:   max(arr);  min(arr)
来源：http://ar.huanxung.cn

PHP:  max($arr);  min($arr);
来源：http://ov.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hp.jianghongdianzi.cn

TS:   Math.max(...arr);
来源：http://cf.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://st.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://na.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://ma.szxytkj.cn

C#:   list.Max();  list.Min()
来源：http://dd.521024.cn

[D18] 扁平化嵌套数组
来源：http://ra.colortex.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://qc.521024.cn

PHP:  array_merge(...$nested);
来源：http://ku.huixinmuqiang.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ca.huixinmuqiang.cn

TS:   nested.flat();
来源：http://ip.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://kn.shxzskj.cn

Go:   // 手写双层循环
来源：http://qx.huanxung.cn

Ruby: nested.flatten
来源：http://om.hnjuh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://oz.9csxet.cn

[D19] 按字段分组
来源：http://it.yuntaijiaju.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rn.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dc.wgjwhj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yu.jianghongdianzi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dg.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ab.newstarts.cn

Go:   // 手写 map[string][]T
来源：http://fq.9csxet.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jo.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://lg.521024.cn

[D20] 统计每个元素出现次数
来源：http://kd.asd995.cn

Py:   Counter(arr)
来源：http://ew.shxzskj.cn

PHP:  array_count_values($arr);
来源：http://kt.bjjhwx.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://et.wgjwhj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gi.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ob.yuexingan06.cn

Go:   // 手写 map[T]int
来源：http://pl.colortex.cn

Ruby: arr.tally
来源：http://wy.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rz.szxytkj.cn

[D21] 判断是否包含某元素
来源：http://vz.asd995.cn

Py:   x in arr
来源：http://dp.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://fc.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://ye.lnxyls.cn

TS:   arr.includes(x)
来源：http://ke.wgjwhj.cn

Java: list.contains(x)
来源：http://jq.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://pr.9csxet.cn

Ruby: arr.include?(x)
来源：http://lo.chemitech.net.cn

C#:   list.Contains(x)
来源：http://gl.9csxet.cn

[D22] 复制数组（避免共享引用）
来源：http://ag.9csxet.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jn.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lr.9csxet.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vg.nicolike.cn

TS:   [...arr];
来源：http://tv.nicolike.cn

Java: new ArrayList<>(list);
来源：http://nd.colortex.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jn.szxytkj.cn

Ruby: arr.dup;  arr.clone
来源：http://rj.gzmigu.cn

C#:   new List<int>(list);
来源：http://jp.hahajie.cn

[D23] reduce 累积计算
来源：http://rb.szsharing.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://du.huixiangedu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://iv.colortex.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iy.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gz.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yg.shxzukj.cn

Go:   // 手写循环
来源：http://ct.gzmigu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ll.521024.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ye.yuexingan06.cn

[D24] 字典 / Map 基本操作
来源：http://tq.gzmigu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fm.shtwfgs.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://sp.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qo.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bz.shxzukj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uk.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://la.521024.cn


<!-- 参考信息 -->