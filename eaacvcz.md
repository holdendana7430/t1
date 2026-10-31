代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://op.haigaiapp.cn

TS:   arr.map(String)
来源：http://cc.wgjwhj.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://tl.shxzukj.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://uh.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://lb.bjjhwx.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jp.panjiajie.cn

[C08] 闭包
来源：http://nu.colortex.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qv.gzmigu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://py.bjjhwx.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ul.gzmigu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://ib.shxzskj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://yr.jctech888.com.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ry.gzmigu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hf.huanxung.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://uw.muxihuayi.cn

[C09] 递归
来源：http://wp.shxzukj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ae.szsharing.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nu.9csxet.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ki.chemitech.net.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://px.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://cz.huanxung.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fu.521024.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wn.colortex.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zs.huixinmuqiang.cn

[C10] 变量作用域
来源：http://dg.huanxung.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hl.521024.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://bi.gzmigu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wn.jianghongdianzi.cn

TS:   同 JS
来源：http://zu.hnjuh.cn

Java: 方法内为块级作用域
来源：http://dk.yuntaijiaju.cn

Go:   花括号块级作用域
来源：http://zx.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://cz.jctech888.com.cn

C#:   块级作用域
来源：http://ct.wgjwhj.cn

[C11] 模块导入与导出
来源：http://zt.huixinmuqiang.cn

Py:   from module import func
来源：http://zj.nszjky.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://wl.jctech888.com.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://sh.haigaiapp.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vc.bookmarksfly.cn

Java: import java.util.List;
来源：http://tk.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://br.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://gf.shtwfgs.cn

C#:   using System.Text;
来源：http://bw.9csxet.cn

[C12] 立即执行函数 IIFE
来源：http://kq.lnxyls.cn

Py:   (lambda: print("run"))()
来源：http://le.szsharing.cn

PHP:  (function () { echo "run"; })();
来源：http://go.hnjuh.cn

JS:   (() => { console.log("run"); })();
来源：http://st.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://nv.nicolike.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hs.shxzukj.cn

Go:   func() { fmt.Println("run") }()
来源：http://tv.lnxyls.cn

Ruby: -> { puts "run" }.call
来源：http://gk.yuexingan06.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qo.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://xk.chemitech.net.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://xg.huixinmuqiang.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ew.wgjwhj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://il.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.haigaiapp.cn

Java: int add(int a, int b) { return a + b; }
来源：http://tl.newstarts.cn

Go:   func add(a, b int) int
来源：http://ez.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vx.bookmarksfly.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ct.shtwfgs.cn

[C14] 泛型函数
来源：http://rh.haigaiapp.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://gn.shxzukj.cn

PHP:  // 无泛型
来源：http://jo.yuexingan06.cn

JS:   // 无泛型
来源：http://jw.gzmigu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ho.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sy.bookmarksfly.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wf.shxzukj.cn

Ruby: # 无泛型
来源：http://lr.huixiangedu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://gu.yuexingan06.cn

[C15] 解构 / 展开参数
来源：http://pt.hahajie.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://js.shtwfgs.cn

PHP:  [$a, $b] = $pair;
来源：http://gm.bookmarksfly.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ax.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://nh.bookmarksfly.cn

Java: // 无解构
来源：http://ur.jctech888.com.cn

Go:   // 无解构
来源：http://us.hnjuh.cn

Ruby: a, b = pair
来源：http://md.9csxet.cn

C#:   var (a, b) = pair;
来源：http://jt.muxihuayi.cn

[C16] 函数 / 方法重载
来源：http://fw.newstarts.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://da.shtwfgs.cn

PHP:  // 无重载
来源：http://fv.huixiangedu.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://mm.9csxet.cn

TS:   // 用联合类型或重载签名声明
来源：http://mx.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://fn.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://rw.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://la.nszjky.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ox.lnxyls.cn

================================================================================
来源：http://wp.9csxet.cn

D. 数组 / 列表 / 集合
来源：http://lz.huanxung.cn

================================================================================
来源：http://mn.hnjuh.cn

[D01] 创建数组 / 列表
来源：http://mn.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jn.gzmigu.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vd.huanxung.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://jn.huixiangedu.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xw.lnxyls.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://eb.hnjuh.cn

Go:   arr := []int{1, 2, 3}
来源：http://it.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://ua.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nb.panjiajie.cn

[D02] 追加元素到末尾
来源：http://tb.szsharing.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://us.shxzukj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://po.shtwfgs.cn

JS:   arr.push(4);
来源：http://gv.shxzukj.cn

TS:   arr.push(4);
来源：http://tj.muxihuayi.cn

Java: list.add(4);
来源：http://un.gzmigu.cn

Go:   arr = append(arr, 4)
来源：http://in.hahajie.cn

Ruby: arr << 4; arr.push(5)
来源：http://od.shxzskj.cn

C#:   list.Add(4);
来源：http://qo.colortex.cn

[D03] 在指定位置插入元素
来源：http://ng.hahajie.cn

Py:   arr.insert(0, 0)
来源：http://ga.chemitech.net.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cz.chemitech.net.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://nb.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://ig.shxzukj.cn

Java: list.add(0, 0);
来源：http://og.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://by.shtwfgs.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://df.panjiajie.cn

C#:   list.Insert(0, 0);
来源：http://cs.9csxet.cn

[D04] 删除元素
来源：http://ad.nszjky.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.panjiajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nn.szsharing.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://xj.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://nf.shtwfgs.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://zj.huanxung.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://io.shxzskj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://sd.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ku.shtwfgs.cn

[D05] 访问与修改元素
来源：http://bf.yuexingan06.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qf.bjjhwx.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dm.hahajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ec.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://tn.colortex.cn

Java: list.get(0); list.set(0, 9);
来源：http://tj.shtwfgs.cn

Go:   arr[0]; arr[0] = 9
来源：http://kq.shtwfgs.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wz.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ee.shxzskj.cn

[D06] 数组长度
来源：http://iq.bookmarksfly.cn

Py:   len(arr)
来源：http://jz.nszjky.cn

PHP:  count($arr);
来源：http://ci.huixiangedu.cn

JS:   arr.length
来源：http://yc.asd995.cn

TS:   arr.length
来源：http://pj.shtwfgs.cn

Java: list.size();
来源：http://eb.jianghongdianzi.cn

Go:   len(arr)
来源：http://tt.bjjhwx.cn

Ruby: arr.length; arr.size
来源：http://fj.huanxung.cn

C#:   list.Count;
来源：http://hm.yuntaijiaju.cn

[D07] 切片 / 取子数组
来源：http://zr.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://kn.colortex.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fm.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://qc.bookmarksfly.cn

TS:   arr.slice(1, 4);
来源：http://ft.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://yw.shtwfgs.cn

Go:   arr[1:4]
来源：http://os.haigaiapp.cn

Ruby: arr[1, 3]
来源：http://ao.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://dl.shtwfgs.cn

[D08] 合并两个数组
来源：http://gb.hahajie.cn

Py:   a + b;  a.extend(b)
来源：http://gh.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://sx.huixiangedu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://lf.shxzskj.cn

TS:   [...a, ...b];
来源：http://ax.huixinmuqiang.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gq.jianghongdianzi.cn

Go:   append(a, b...)
来源：http://ju.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://mb.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://nl.521024.cn

[D09] 排序（升序）
来源：http://te.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://po.colortex.cn

PHP:  sort($arr);
来源：http://vr.hahajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zq.shxzskj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fu.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sh.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zy.huixinmuqiang.cn

Ruby: arr.sort
来源：http://jw.muxihuayi.cn

C#:   list.Sort();
来源：http://iw.9csxet.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fv.gzmigu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ak.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sy.panjiajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hj.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://es.nicolike.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jr.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rd.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mz.jctech888.com.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tt.bjjhwx.cn

[D11] 反转数组
来源：http://vz.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zy.muxihuayi.cn

PHP:  array_reverse($arr);
来源：http://zl.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://if.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://nz.gzmigu.cn

Java: Collections.reverse(list);
来源：http://mx.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://jo.shxzukj.cn

Ruby: arr.reverse
来源：http://rb.panjiajie.cn

C#:   list.Reverse();
来源：http://th.szsharing.cn

[D12] 查找元素下标
来源：http://me.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://yb.hnjuh.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vj.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://og.szxytkj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hp.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gb.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://rm.chemitech.net.cn

Ruby: arr.index(x)
来源：http://hj.newstarts.cn

C#:   list.IndexOf(x);
来源：http://oy.muxihuayi.cn

[D13] 过滤（保留满足条件的）
来源：http://wd.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://gz.shxzukj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hs.haigaiapp.cn

JS:   arr.filter(x => x > 3)
来源：http://ha.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://hn.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zc.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zu.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://mc.muxihuayi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://te.shtwfgs.cn

[D14] 映射转换（每个元素变形）
来源：http://xp.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ko.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ii.chemitech.net.cn

JS:   arr.map(x => x * 2)
来源：http://xi.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://zq.lnxyls.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ik.shxzskj.cn

Go:   // 手写循环
来源：http://fi.szxytkj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ry.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ip.asd995.cn

[D15] 去重
来源：http://ko.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hc.muxihuayi.cn

PHP:  array_unique($arr);
来源：http://pd.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://hr.wgjwhj.cn

TS:   [...new Set(arr)]
来源：http://dq.haigaiapp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://we.gzmigu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pj.bjjhwx.cn

Ruby: arr.uniq
来源：http://cc.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://nu.chemitech.net.cn

[D16] 求和与平均值
来源：http://lm.shxzukj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gl.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ux.lnxyls.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zx.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://bc.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ke.shxzukj.cn

Go:   // 手写循环累加
来源：http://uc.haigaiapp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cj.yuntaijiaju.cn

C#:   list.Sum();  list.Average()
来源：http://ii.panjiajie.cn

[D17] 最大值与最小值
来源：http://iy.shtwfgs.cn

Py:   max(arr);  min(arr)
来源：http://wh.huixiangedu.cn

PHP:  max($arr);  min($arr);
来源：http://ju.yuexingan06.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bo.9csxet.cn

TS:   Math.max(...arr);
来源：http://ds.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ib.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hs.hahajie.cn

Ruby: arr.max;  arr.min
来源：http://af.gzmigu.cn

C#:   list.Max();  list.Min()
来源：http://bw.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://xr.haigaiapp.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ii.yuexingan06.cn

PHP:  array_merge(...$nested);
来源：http://cl.huixinmuqiang.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ab.shxzukj.cn

TS:   nested.flat();
来源：http://gr.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oo.muxihuayi.cn

Go:   // 手写双层循环
来源：http://yj.shtwfgs.cn

Ruby: nested.flatten
来源：http://gk.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ne.szsharing.cn

[D19] 按字段分组
来源：http://ps.hnjuh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://af.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qg.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ob.yuexingan06.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bi.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://nr.szsharing.cn

Go:   // 手写 map[string][]T
来源：http://sy.nicolike.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cy.jianghongdianzi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kr.lnxyls.cn

[D20] 统计每个元素出现次数
来源：http://ji.huixinmuqiang.cn

Py:   Counter(arr)
来源：http://pp.hahajie.cn

PHP:  array_count_values($arr);
来源：http://sd.huanxung.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wd.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gy.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://tt.asd995.cn

Go:   // 手写 map[T]int
来源：http://yy.jctech888.com.cn

Ruby: arr.tally
来源：http://yb.shxzukj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rz.hahajie.cn

[D21] 判断是否包含某元素
来源：http://mn.chemitech.net.cn

Py:   x in arr
来源：http://lq.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://ln.yuexingan06.cn

JS:   arr.includes(x)
来源：http://tz.panjiajie.cn

TS:   arr.includes(x)
来源：http://wx.haigaiapp.cn

Java: list.contains(x)
来源：http://gl.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://av.chemitech.net.cn

Ruby: arr.include?(x)
来源：http://fp.bookmarksfly.cn

C#:   list.Contains(x)
来源：http://jz.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://qz.bookmarksfly.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jp.gzmigu.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://dy.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://br.bookmarksfly.cn

TS:   [...arr];
来源：http://ae.huixiangedu.cn

Java: new ArrayList<>(list);
来源：http://xs.bookmarksfly.cn

Go:   copied := append([]int(nil), arr...)
来源：http://up.chemitech.net.cn

Ruby: arr.dup;  arr.clone
来源：http://py.haigaiapp.cn

C#:   new List<int>(list);
来源：http://ze.yuntaijiaju.cn

[D23] reduce 累积计算
来源：http://rk.hahajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cr.wgjwhj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rn.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vg.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aw.newstarts.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ot.521024.cn

Go:   // 手写循环
来源：http://ki.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://io.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ga.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://si.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://nb.yuntaijiaju.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qn.newstarts.cn


<!-- 参考信息 -->