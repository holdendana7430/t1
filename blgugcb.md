代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jm.jianghongdianzi.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://zb.bjjhwx.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://eu.lnxyls.cn

[C09] 递归
来源：http://fk.nszjky.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ob.panjiajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://yf.muxihuayi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://qq.shxzukj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ql.szsharing.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lw.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://vk.nszjky.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://jn.huanxung.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://bz.muxihuayi.cn

[C10] 变量作用域
来源：http://lu.521024.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ko.shtwfgs.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xi.hahajie.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ci.newstarts.cn

TS:   同 JS
来源：http://qx.colortex.cn

Java: 方法内为块级作用域
来源：http://rk.panjiajie.cn

Go:   花括号块级作用域
来源：http://cb.colortex.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://qc.colortex.cn

C#:   块级作用域
来源：http://ow.nszjky.cn

[C11] 模块导入与导出
来源：http://aw.huixinmuqiang.cn

Py:   from module import func
来源：http://vv.huanxung.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://cn.szxytkj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ks.hahajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://zg.nszjky.cn

Java: import java.util.List;
来源：http://bq.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://uo.huanxung.cn

Ruby: require "json"; require_relative "./util"
来源：http://dr.bjjhwx.cn

C#:   using System.Text;
来源：http://fa.9csxet.cn

[C12] 立即执行函数 IIFE
来源：http://tv.chemitech.net.cn

Py:   (lambda: print("run"))()
来源：http://wk.hahajie.cn

PHP:  (function () { echo "run"; })();
来源：http://ye.bjjhwx.cn

JS:   (() => { console.log("run"); })();
来源：http://jn.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://qu.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jq.jianghongdianzi.cn

Go:   func() { fmt.Println("run") }()
来源：http://zi.shtwfgs.cn

Ruby: -> { puts "run" }.call
来源：http://xg.huixinmuqiang.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://zi.szsharing.cn

[C13] 类型声明 / 类型注解
来源：http://uo.521024.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://yh.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://sk.huanxung.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://he.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://bq.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://nz.asd995.cn

Go:   func add(a, b int) int
来源：http://lu.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lb.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://db.huanxung.cn

[C14] 泛型函数
来源：http://nf.nicolike.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://au.hahajie.cn

PHP:  // 无泛型
来源：http://my.lnxyls.cn

JS:   // 无泛型
来源：http://ch.chemitech.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://kn.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://is.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://sa.hahajie.cn

Ruby: # 无泛型
来源：http://wv.nicolike.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oo.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://qa.colortex.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://np.muxihuayi.cn

PHP:  [$a, $b] = $pair;
来源：http://ws.shxzskj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rw.521024.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ll.shxzskj.cn

Java: // 无解构
来源：http://uj.shtwfgs.cn

Go:   // 无解构
来源：http://lz.nicolike.cn

Ruby: a, b = pair
来源：http://db.bjjhwx.cn

C#:   var (a, b) = pair;
来源：http://bs.yuntaijiaju.cn

[C16] 函数 / 方法重载
来源：http://cg.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kn.shtwfgs.cn

PHP:  // 无重载
来源：http://fv.shxzskj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gr.asd995.cn

TS:   // 用联合类型或重载签名声明
来源：http://dc.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hd.huanxung.cn

Go:   // 无重载：用不同函数名
来源：http://jp.huixiangedu.cn

Ruby: # 无重载：靠动态参数
来源：http://ne.haigaiapp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://bk.szsharing.cn

================================================================================
来源：http://by.wgjwhj.cn

D. 数组 / 列表 / 集合
来源：http://wb.shxzukj.cn

================================================================================
来源：http://ry.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://re.szsharing.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ot.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vv.haigaiapp.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tv.gzmigu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://lh.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://gx.shxzukj.cn

Go:   arr := []int{1, 2, 3}
来源：http://cx.shxzukj.cn

Ruby: arr = [1, 2, 3]
来源：http://jn.9csxet.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bx.hnjuh.cn

[D02] 追加元素到末尾
来源：http://dr.szxytkj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://rh.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://sh.haigaiapp.cn

JS:   arr.push(4);
来源：http://vq.wgjwhj.cn

TS:   arr.push(4);
来源：http://qu.wgjwhj.cn

Java: list.add(4);
来源：http://at.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://sj.shxzskj.cn

Ruby: arr << 4; arr.push(5)
来源：http://kb.shtwfgs.cn

C#:   list.Add(4);
来源：http://im.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://wy.muxihuayi.cn

Py:   arr.insert(0, 0)
来源：http://da.haigaiapp.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lc.szxytkj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dw.asd995.cn

TS:   arr.splice(0, 0, 0);
来源：http://te.bjjhwx.cn

Java: list.add(0, 0);
来源：http://nb.huixinmuqiang.cn

Go:   arr = append([]int{0}, arr...)
来源：http://gg.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://rf.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://lg.colortex.cn

[D04] 删除元素
来源：http://ki.lnxyls.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ii.yuexingan06.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://sd.nicolike.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hn.huixiangedu.cn

TS:   arr.splice(0, 1);
来源：http://bt.yuntaijiaju.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hg.shtwfgs.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ks.hnjuh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wo.wgjwhj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yh.yuntaijiaju.cn

[D05] 访问与修改元素
来源：http://fh.huixiangedu.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qr.nszjky.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xx.lnxyls.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fk.hahajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://ag.shtwfgs.cn

Java: list.get(0); list.set(0, 9);
来源：http://ut.chemitech.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://yw.yuexingan06.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zs.lnxyls.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ue.haigaiapp.cn

[D06] 数组长度
来源：http://ob.521024.cn

Py:   len(arr)
来源：http://wb.shxzskj.cn

PHP:  count($arr);
来源：http://hz.jctech888.com.cn

JS:   arr.length
来源：http://mg.panjiajie.cn

TS:   arr.length
来源：http://ei.hnjuh.cn

Java: list.size();
来源：http://ej.lnxyls.cn

Go:   len(arr)
来源：http://vg.hahajie.cn

Ruby: arr.length; arr.size
来源：http://xa.bjjhwx.cn

C#:   list.Count;
来源：http://gt.asd995.cn

[D07] 切片 / 取子数组
来源：http://ek.yuexingan06.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nv.newstarts.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ye.shxzskj.cn

JS:   arr.slice(1, 4);
来源：http://xw.huanxung.cn

TS:   arr.slice(1, 4);
来源：http://rp.asd995.cn

Java: list.subList(1, 4);
来源：http://es.huanxung.cn

Go:   arr[1:4]
来源：http://ch.panjiajie.cn

Ruby: arr[1, 3]
来源：http://ep.muxihuayi.cn

C#:   list.GetRange(1, 3);
来源：http://la.asd995.cn

[D08] 合并两个数组
来源：http://rc.bjjhwx.cn

Py:   a + b;  a.extend(b)
来源：http://bq.nicolike.cn

PHP:  array_merge($a, $b);
来源：http://hm.huixiangedu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sc.haigaiapp.cn

TS:   [...a, ...b];
来源：http://rd.jianghongdianzi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ou.yuexingan06.cn

Go:   append(a, b...)
来源：http://zr.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://qi.huanxung.cn

C#:   a.Concat(b).ToList()
来源：http://dm.szxytkj.cn

[D09] 排序（升序）
来源：http://mg.hnjuh.cn

Py:   sorted(arr);  arr.sort()
来源：http://po.nicolike.cn

PHP:  sort($arr);
来源：http://na.shxzskj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://oy.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wj.jctech888.com.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ki.huixiangedu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zu.hnjuh.cn

Ruby: arr.sort
来源：http://ch.bookmarksfly.cn

C#:   list.Sort();
来源：http://wj.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ti.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yo.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qw.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bp.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ib.chemitech.net.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://bj.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://jb.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ct.muxihuayi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://gk.hnjuh.cn

[D11] 反转数组
来源：http://at.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xl.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://hx.521024.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kt.521024.cn

TS:   [...arr].reverse();
来源：http://nn.szxytkj.cn

Java: Collections.reverse(list);
来源：http://vf.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://mx.szxytkj.cn

Ruby: arr.reverse
来源：http://uj.panjiajie.cn

C#:   list.Reverse();
来源：http://od.521024.cn

[D12] 查找元素下标
来源：http://hl.shxzskj.cn

Py:   arr.index(x);  x in arr
来源：http://oo.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fx.colortex.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qj.9csxet.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mf.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ph.szxytkj.cn

Go:   slices.Index(arr, x)
来源：http://ez.shtwfgs.cn

Ruby: arr.index(x)
来源：http://uj.colortex.cn

C#:   list.IndexOf(x);
来源：http://pe.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://tl.asd995.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://re.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ig.asd995.cn

JS:   arr.filter(x => x > 3)
来源：http://kh.huixinmuqiang.cn

TS:   arr.filter(x => x > 3)
来源：http://qf.gzmigu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fh.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wk.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bx.haigaiapp.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ws.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://rs.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kn.hnjuh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tn.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://ac.haigaiapp.cn

TS:   arr.map(x => x * 2)
来源：http://cg.wgjwhj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wo.asd995.cn

Go:   // 手写循环
来源：http://qk.nicolike.cn

Ruby: arr.map { |x| x * 2 }
来源：http://sn.shxzskj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ji.hnjuh.cn

[D15] 去重
来源：http://lh.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fa.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://ku.newstarts.cn

JS:   [...new Set(arr)]
来源：http://ap.wgjwhj.cn

TS:   [...new Set(arr)]
来源：http://zp.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vu.szxytkj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tx.wgjwhj.cn

Ruby: arr.uniq
来源：http://kx.9csxet.cn

C#:   list.Distinct().ToList()
来源：http://kt.huixiangedu.cn

[D16] 求和与平均值
来源：http://ok.521024.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://cn.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gi.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hw.yuntaijiaju.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shxzukj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://uv.huixiangedu.cn

Go:   // 手写循环累加
来源：http://uo.yuexingan06.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://rx.huanxung.cn

C#:   list.Sum();  list.Average()
来源：http://yw.szxytkj.cn

[D17] 最大值与最小值
来源：http://dl.huixiangedu.cn

Py:   max(arr);  min(arr)
来源：http://hr.wgjwhj.cn

PHP:  max($arr);  min($arr);
来源：http://vk.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://sr.huanxung.cn

TS:   Math.max(...arr);
来源：http://gm.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cw.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://su.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://cv.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://ud.shxzskj.cn

[D18] 扁平化嵌套数组
来源：http://kp.wgjwhj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://zq.muxihuayi.cn

PHP:  array_merge(...$nested);
来源：http://oy.panjiajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fp.shxzskj.cn

TS:   nested.flat();
来源：http://rh.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ys.hahajie.cn

Go:   // 手写双层循环
来源：http://lo.shxzskj.cn

Ruby: nested.flatten
来源：http://up.chemitech.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xk.yuntaijiaju.cn

[D19] 按字段分组
来源：http://if.bjjhwx.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://jg.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qm.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mu.panjiajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xy.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ux.huixiangedu.cn

Go:   // 手写 map[string][]T
来源：http://bf.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wf.nicolike.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ja.huanxung.cn

[D20] 统计每个元素出现次数
来源：http://ke.521024.cn

Py:   Counter(arr)
来源：http://xm.shxzskj.cn

PHP:  array_count_values($arr);
来源：http://lk.shtwfgs.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tx.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oh.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sz.9csxet.cn

Go:   // 手写 map[T]int
来源：http://on.hahajie.cn

Ruby: arr.tally
来源：http://dt.huixinmuqiang.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://cd.521024.cn

[D21] 判断是否包含某元素
来源：http://hx.wgjwhj.cn

Py:   x in arr
来源：http://xb.yuntaijiaju.cn

PHP:  in_array($x, $arr, true);
来源：http://bb.newstarts.cn

JS:   arr.includes(x)
来源：http://yp.9csxet.cn

TS:   arr.includes(x)
来源：http://zc.bjjhwx.cn

Java: list.contains(x)
来源：http://sd.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://an.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://ip.huanxung.cn

C#:   list.Contains(x)
来源：http://pi.lnxyls.cn

[D22] 复制数组（避免共享引用）
来源：http://an.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wk.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://gg.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://up.521024.cn

TS:   [...arr];
来源：http://uf.muxihuayi.cn

Java: new ArrayList<>(list);
来源：http://gw.huixinmuqiang.cn

Go:   copied := append([]int(nil), arr...)
来源：http://yu.szxytkj.cn

Ruby: arr.dup;  arr.clone
来源：http://dm.jianghongdianzi.cn

C#:   new List<int>(list);
来源：http://hz.jctech888.com.cn

[D23] reduce 累积计算
来源：http://bk.shxzskj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ln.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://iw.lnxyls.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vw.nszjky.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://eo.jianghongdianzi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hp.haigaiapp.cn

Go:   // 手写循环
来源：http://rl.huixinmuqiang.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nf.colortex.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pi.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://px.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pq.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ip.yuexingan06.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://me.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sg.huixiangedu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uh.shtwfgs.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hu.gzmigu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tp.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hy.jctech888.com.cn

[D25] Set 集合去重与交并差
来源：http://al.hahajie.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kl.wgjwhj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wf.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bp.haigaiapp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wd.haigaiapp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://po.yuntaijiaju.cn


<!-- 参考信息 -->