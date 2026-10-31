代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://cg.asd995.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://fe.wgjwhj.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://kb.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://vd.shxzukj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://bs.gzmigu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://rj.shxzukj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://aj.newstarts.cn

[C09] 递归
来源：http://au.huixiangedu.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://vx.jianghongdianzi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bt.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://xw.jctech888.com.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://or.shtwfgs.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://tj.chemitech.net.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jj.chemitech.net.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ag.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qs.nszjky.cn

[C10] 变量作用域
来源：http://ee.hahajie.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yf.hnjuh.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://kj.muxihuayi.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ow.9csxet.cn

TS:   同 JS
来源：http://yl.lnxyls.cn

Java: 方法内为块级作用域
来源：http://mc.hnjuh.cn

Go:   花括号块级作用域
来源：http://co.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://ym.huanxung.cn

C#:   块级作用域
来源：http://gz.shtwfgs.cn

[C11] 模块导入与导出
来源：http://gs.jctech888.com.cn

Py:   from module import func
来源：http://kj.jctech888.com.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ne.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://fl.bookmarksfly.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://un.huixiangedu.cn

Java: import java.util.List;
来源：http://wy.9csxet.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://sz.lnxyls.cn

Ruby: require "json"; require_relative "./util"
来源：http://ye.jctech888.com.cn

C#:   using System.Text;
来源：http://yg.asd995.cn

[C12] 立即执行函数 IIFE
来源：http://bh.hahajie.cn

Py:   (lambda: print("run"))()
来源：http://ce.hnjuh.cn

PHP:  (function () { echo "run"; })();
来源：http://lt.huixiangedu.cn

JS:   (() => { console.log("run"); })();
来源：http://dl.shxzskj.cn

TS:   (() => { console.log("run"); })();
来源：http://lk.shtwfgs.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://gh.wgjwhj.cn

Go:   func() { fmt.Println("run") }()
来源：http://mr.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://iz.bookmarksfly.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://yq.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://mv.521024.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://gv.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vl.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://sf.szxytkj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hl.huanxung.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vc.shtwfgs.cn

Go:   func add(a, b int) int
来源：http://ly.huixiangedu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://br.huanxung.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nm.yuntaijiaju.cn

[C14] 泛型函数
来源：http://aa.huixinmuqiang.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://by.yuntaijiaju.cn

PHP:  // 无泛型
来源：http://be.chemitech.net.cn

JS:   // 无泛型
来源：http://td.huanxung.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mr.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://po.shxzukj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vm.szsharing.cn

Ruby: # 无泛型
来源：http://mz.bookmarksfly.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pm.hahajie.cn

[C15] 解构 / 展开参数
来源：http://ll.hahajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://vj.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://oo.521024.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ox.chemitech.net.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rv.panjiajie.cn

Java: // 无解构
来源：http://ku.shxzskj.cn

Go:   // 无解构
来源：http://fb.asd995.cn

Ruby: a, b = pair
来源：http://fe.gzmigu.cn

C#:   var (a, b) = pair;
来源：http://yg.szsharing.cn

[C16] 函数 / 方法重载
来源：http://uw.szsharing.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://sp.yuntaijiaju.cn

PHP:  // 无重载
来源：http://jn.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ha.lnxyls.cn

TS:   // 用联合类型或重载签名声明
来源：http://gy.wgjwhj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zv.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://gz.hnjuh.cn

Ruby: # 无重载：靠动态参数
来源：http://cy.shtwfgs.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yx.nicolike.cn

================================================================================
来源：http://vn.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://db.huanxung.cn

================================================================================
来源：http://rc.huixiangedu.cn

[D01] 创建数组 / 列表
来源：http://qw.muxihuayi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://gi.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pv.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jg.nszjky.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ru.hahajie.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rg.shxzukj.cn

Go:   arr := []int{1, 2, 3}
来源：http://ib.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://mm.nszjky.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://rg.jianghongdianzi.cn

[D02] 追加元素到末尾
来源：http://zl.szsharing.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mv.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ao.gzmigu.cn

JS:   arr.push(4);
来源：http://df.huixinmuqiang.cn

TS:   arr.push(4);
来源：http://xl.haigaiapp.cn

Java: list.add(4);
来源：http://gv.asd995.cn

Go:   arr = append(arr, 4)
来源：http://ss.bookmarksfly.cn

Ruby: arr << 4; arr.push(5)
来源：http://xh.jctech888.com.cn

C#:   list.Add(4);
来源：http://ue.colortex.cn

[D03] 在指定位置插入元素
来源：http://aj.colortex.cn

Py:   arr.insert(0, 0)
来源：http://co.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://yc.lnxyls.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://to.521024.cn

TS:   arr.splice(0, 0, 0);
来源：http://hb.gzmigu.cn

Java: list.add(0, 0);
来源：http://xw.bjjhwx.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qw.shxzukj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ng.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://ti.panjiajie.cn

[D04] 删除元素
来源：http://kj.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hf.jctech888.com.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://av.hnjuh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dj.szsharing.cn

TS:   arr.splice(0, 1);
来源：http://vv.shxzskj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yf.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://zf.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hm.wgjwhj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nq.szsharing.cn

[D05] 访问与修改元素
来源：http://ws.gzmigu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ka.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cy.nicolike.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yx.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://zd.colortex.cn

Java: list.get(0); list.set(0, 9);
来源：http://it.yuntaijiaju.cn

Go:   arr[0]; arr[0] = 9
来源：http://im.colortex.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ec.bjjhwx.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://gf.wgjwhj.cn

[D06] 数组长度
来源：http://sx.wgjwhj.cn

Py:   len(arr)
来源：http://qp.wgjwhj.cn

PHP:  count($arr);
来源：http://lp.lnxyls.cn

JS:   arr.length
来源：http://ap.shxzskj.cn

TS:   arr.length
来源：http://or.bjjhwx.cn

Java: list.size();
来源：http://wo.nszjky.cn

Go:   len(arr)
来源：http://rw.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://el.shxzukj.cn

C#:   list.Count;
来源：http://ga.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://kx.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uy.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sw.yuexingan06.cn

JS:   arr.slice(1, 4);
来源：http://tq.huanxung.cn

TS:   arr.slice(1, 4);
来源：http://va.jctech888.com.cn

Java: list.subList(1, 4);
来源：http://bl.wgjwhj.cn

Go:   arr[1:4]
来源：http://vz.huixiangedu.cn

Ruby: arr[1, 3]
来源：http://rn.9csxet.cn

C#:   list.GetRange(1, 3);
来源：http://vn.newstarts.cn

[D08] 合并两个数组
来源：http://kv.yuntaijiaju.cn

Py:   a + b;  a.extend(b)
来源：http://dv.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://xv.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wa.shxzskj.cn

TS:   [...a, ...b];
来源：http://xb.muxihuayi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://dz.newstarts.cn

Go:   append(a, b...)
来源：http://dm.nicolike.cn

Ruby: a + b;  a.concat(b)
来源：http://zs.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://jm.szsharing.cn

[D09] 排序（升序）
来源：http://wv.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://qx.asd995.cn

PHP:  sort($arr);
来源：http://ty.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pw.bjjhwx.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hh.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jh.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ok.jctech888.com.cn

Ruby: arr.sort
来源：http://ur.haigaiapp.cn

C#:   list.Sort();
来源：http://yc.newstarts.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ci.gzmigu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hm.colortex.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://dk.haigaiapp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://sa.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wo.asd995.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cy.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://sf.nszjky.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://uk.hnjuh.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://cn.huanxung.cn

[D11] 反转数组
来源：http://os.shxzskj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wy.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://ce.szsharing.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://va.nszjky.cn

TS:   [...arr].reverse();
来源：http://tt.haigaiapp.cn

Java: Collections.reverse(list);
来源：http://gw.asd995.cn

Go:   slices.Reverse(arr)
来源：http://ca.szxytkj.cn

Ruby: arr.reverse
来源：http://xi.yuntaijiaju.cn

C#:   list.Reverse();
来源：http://iu.shxzukj.cn

[D12] 查找元素下标
来源：http://zl.shxzskj.cn

Py:   arr.index(x);  x in arr
来源：http://oa.szxytkj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eb.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sr.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://av.gzmigu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zc.gzmigu.cn

Go:   slices.Index(arr, x)
来源：http://ej.yuntaijiaju.cn

Ruby: arr.index(x)
来源：http://bm.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://lv.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://fz.wgjwhj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://vs.huixinmuqiang.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://um.muxihuayi.cn

JS:   arr.filter(x => x > 3)
来源：http://py.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://ia.wgjwhj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dn.shxzskj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fl.hahajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://it.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dc.gzmigu.cn

[D14] 映射转换（每个元素变形）
来源：http://ki.colortex.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://im.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cl.colortex.cn

JS:   arr.map(x => x * 2)
来源：http://hh.huanxung.cn

TS:   arr.map(x => x * 2)
来源：http://yq.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pp.nicolike.cn

Go:   // 手写循环
来源：http://mb.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gt.shtwfgs.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jq.szsharing.cn

[D15] 去重
来源：http://gw.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ig.hnjuh.cn

PHP:  array_unique($arr);
来源：http://mo.shtwfgs.cn

JS:   [...new Set(arr)]
来源：http://xw.shtwfgs.cn

TS:   [...new Set(arr)]
来源：http://mi.asd995.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://oy.nszjky.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zz.haigaiapp.cn

Ruby: arr.uniq
来源：http://lw.szxytkj.cn

C#:   list.Distinct().ToList()
来源：http://dc.colortex.cn

[D16] 求和与平均值
来源：http://ef.hnjuh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://tb.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://jq.szxytkj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ej.9csxet.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://nv.colortex.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yd.szxytkj.cn

Go:   // 手写循环累加
来源：http://af.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hw.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://iu.chemitech.net.cn

[D17] 最大值与最小值
来源：http://ho.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://gw.521024.cn

PHP:  max($arr);  min($arr);
来源：http://hl.panjiajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://oa.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://ci.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fp.hahajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://cj.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://ok.newstarts.cn

C#:   list.Max();  list.Min()
来源：http://dd.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://tz.gzmigu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fo.bookmarksfly.cn

PHP:  array_merge(...$nested);
来源：http://wj.colortex.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://am.hahajie.cn

TS:   nested.flat();
来源：http://px.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zf.shxzukj.cn

Go:   // 手写双层循环
来源：http://ak.nszjky.cn

Ruby: nested.flatten
来源：http://zo.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yk.asd995.cn

[D19] 按字段分组
来源：http://vt.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jv.shxzukj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ul.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rb.newstarts.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ww.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://of.muxihuayi.cn

Go:   // 手写 map[string][]T
来源：http://qs.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rk.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hp.jctech888.com.cn

[D20] 统计每个元素出现次数
来源：http://kz.shtwfgs.cn

Py:   Counter(arr)
来源：http://yy.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://ug.huanxung.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://px.shxzskj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oi.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ed.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://bc.panjiajie.cn

Ruby: arr.tally
来源：http://pq.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ov.huixinmuqiang.cn

[D21] 判断是否包含某元素
来源：http://zs.hahajie.cn

Py:   x in arr
来源：http://pd.panjiajie.cn

PHP:  in_array($x, $arr, true);
来源：http://ov.nicolike.cn

JS:   arr.includes(x)
来源：http://ux.szxytkj.cn

TS:   arr.includes(x)
来源：http://df.chemitech.net.cn

Java: list.contains(x)
来源：http://zm.gzmigu.cn

Go:   slices.Contains(arr, x)
来源：http://ns.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://lj.hahajie.cn

C#:   list.Contains(x)
来源：http://rx.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://jp.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gx.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mu.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://et.521024.cn

TS:   [...arr];
来源：http://gq.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://jz.hahajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kx.haigaiapp.cn

Ruby: arr.dup;  arr.clone
来源：http://yu.haigaiapp.cn

C#:   new List<int>(list);
来源：http://gl.colortex.cn

[D23] reduce 累积计算
来源：http://ux.lnxyls.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://qh.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bl.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xz.szxytkj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yx.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rn.huixiangedu.cn

Go:   // 手写循环
来源：http://mc.bookmarksfly.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fa.jianghongdianzi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://yf.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://no.nszjky.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://uc.nszjky.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ur.haigaiapp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://sw.panjiajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bm.gzmigu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cn.shxzskj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ne.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://de.hnjuh.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kk.jctech888.com.cn

[D25] Set 集合去重与交并差
来源：http://tu.yuexingan06.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fj.shxzukj.cn


<!-- 参考信息 -->