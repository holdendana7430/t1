代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://zj.huixiangedu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tc.yuexingan06.cn

[C08] 闭包
来源：http://wf.yuexingan06.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://ft.shxzskj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://dn.hnjuh.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://bc.panjiajie.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mi.szsharing.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://gh.nicolike.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://lb.9csxet.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://xk.wgjwhj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://cq.nszjky.cn

[C09] 递归
来源：http://eh.newstarts.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://nq.jianghongdianzi.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://ez.shxzukj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://gc.wgjwhj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bc.bjjhwx.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://zk.huixiangedu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://nz.hahajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://rl.nszjky.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://sq.yuntaijiaju.cn

[C10] 变量作用域
来源：http://ms.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yw.jianghongdianzi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://ky.huixinmuqiang.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ig.hahajie.cn

TS:   同 JS
来源：http://ps.lnxyls.cn

Java: 方法内为块级作用域
来源：http://mn.bjjhwx.cn

Go:   花括号块级作用域
来源：http://dz.muxihuayi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kt.szxytkj.cn

C#:   块级作用域
来源：http://ah.521024.cn

[C11] 模块导入与导出
来源：http://wq.szsharing.cn

Py:   from module import func
来源：http://vg.panjiajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://mg.jctech888.com.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://vg.panjiajie.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://by.shtwfgs.cn

Java: import java.util.List;
来源：http://jh.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://at.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://ev.asd995.cn

C#:   using System.Text;
来源：http://kw.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://fv.hnjuh.cn

Py:   (lambda: print("run"))()
来源：http://ps.muxihuayi.cn

PHP:  (function () { echo "run"; })();
来源：http://ve.szsharing.cn

JS:   (() => { console.log("run"); })();
来源：http://xc.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://wj.szsharing.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://jo.bjjhwx.cn

Go:   func() { fmt.Println("run") }()
来源：http://ut.wgjwhj.cn

Ruby: -> { puts "run" }.call
来源：http://sq.nicolike.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://mp.wgjwhj.cn

[C13] 类型声明 / 类型注解
来源：http://ju.huixinmuqiang.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bl.jianghongdianzi.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://os.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jm.newstarts.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://kt.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fl.hnjuh.cn

Go:   func add(a, b int) int
来源：http://zg.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lx.521024.cn

C#:   int Add(int a, int b) => a + b;
来源：http://sp.lnxyls.cn

[C14] 泛型函数
来源：http://os.yuexingan06.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://pd.nicolike.cn

PHP:  // 无泛型
来源：http://qy.yuntaijiaju.cn

JS:   // 无泛型
来源：http://ae.chemitech.net.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://bz.haigaiapp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sb.gzmigu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nq.huixiangedu.cn

Ruby: # 无泛型
来源：http://dy.colortex.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://oh.colortex.cn

[C15] 解构 / 展开参数
来源：http://bo.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wg.shxzukj.cn

PHP:  [$a, $b] = $pair;
来源：http://wk.521024.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ko.wgjwhj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://zf.chemitech.net.cn

Java: // 无解构
来源：http://wf.yuntaijiaju.cn

Go:   // 无解构
来源：http://fe.bjjhwx.cn

Ruby: a, b = pair
来源：http://hc.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://mk.panjiajie.cn

[C16] 函数 / 方法重载
来源：http://an.chemitech.net.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ty.hahajie.cn

PHP:  // 无重载
来源：http://yk.newstarts.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://oq.shxzukj.cn

TS:   // 用联合类型或重载签名声明
来源：http://uq.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xi.newstarts.cn

Go:   // 无重载：用不同函数名
来源：http://pi.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://jy.asd995.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://hv.gzmigu.cn

================================================================================
来源：http://is.newstarts.cn

D. 数组 / 列表 / 集合
来源：http://gf.wgjwhj.cn

================================================================================
来源：http://cg.yuexingan06.cn

[D01] 创建数组 / 列表
来源：http://zx.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bs.panjiajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://au.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ct.shxzukj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://za.jctech888.com.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://oy.wgjwhj.cn

Go:   arr := []int{1, 2, 3}
来源：http://os.huixiangedu.cn

Ruby: arr = [1, 2, 3]
来源：http://lo.huanxung.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://oa.huanxung.cn

[D02] 追加元素到末尾
来源：http://je.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://la.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oc.yuexingan06.cn

JS:   arr.push(4);
来源：http://qw.gzmigu.cn

TS:   arr.push(4);
来源：http://yk.gzmigu.cn

Java: list.add(4);
来源：http://ja.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://mz.bookmarksfly.cn

Ruby: arr << 4; arr.push(5)
来源：http://ki.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://qq.asd995.cn

[D03] 在指定位置插入元素
来源：http://cw.shxzskj.cn

Py:   arr.insert(0, 0)
来源：http://zo.wgjwhj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mt.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://qi.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://em.yuexingan06.cn

Java: list.add(0, 0);
来源：http://wd.yuexingan06.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zu.jctech888.com.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yt.yuexingan06.cn

C#:   list.Insert(0, 0);
来源：http://kh.huixiangedu.cn

[D04] 删除元素
来源：http://vd.jctech888.com.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ww.521024.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://pb.lnxyls.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uc.9csxet.cn

TS:   arr.splice(0, 1);
来源：http://zv.szsharing.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://nk.colortex.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qi.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://du.lnxyls.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://sq.jctech888.com.cn

[D05] 访问与修改元素
来源：http://uk.asd995.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gt.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kr.szxytkj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sp.newstarts.cn

TS:   arr[0]; arr.at(-1);
来源：http://ii.nicolike.cn

Java: list.get(0); list.set(0, 9);
来源：http://dd.chemitech.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://hp.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://zr.huanxung.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://yy.huixinmuqiang.cn

[D06] 数组长度
来源：http://vo.huixinmuqiang.cn

Py:   len(arr)
来源：http://nh.shtwfgs.cn

PHP:  count($arr);
来源：http://db.szsharing.cn

JS:   arr.length
来源：http://ke.jctech888.com.cn

TS:   arr.length
来源：http://ri.huixiangedu.cn

Java: list.size();
来源：http://jl.panjiajie.cn

Go:   len(arr)
来源：http://qn.haigaiapp.cn

Ruby: arr.length; arr.size
来源：http://pc.nszjky.cn

C#:   list.Count;
来源：http://wh.haigaiapp.cn

[D07] 切片 / 取子数组
来源：http://aj.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gx.gzmigu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zz.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://ym.lnxyls.cn

TS:   arr.slice(1, 4);
来源：http://ua.chemitech.net.cn

Java: list.subList(1, 4);
来源：http://zo.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://mn.huanxung.cn

Ruby: arr[1, 3]
来源：http://jo.shxzskj.cn

C#:   list.GetRange(1, 3);
来源：http://io.colortex.cn

[D08] 合并两个数组
来源：http://ui.shtwfgs.cn

Py:   a + b;  a.extend(b)
来源：http://fb.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://yy.9csxet.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://it.lnxyls.cn

TS:   [...a, ...b];
来源：http://cb.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xk.jctech888.com.cn

Go:   append(a, b...)
来源：http://ul.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://hc.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://sh.9csxet.cn

[D09] 排序（升序）
来源：http://jt.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://mk.nszjky.cn

PHP:  sort($arr);
来源：http://sd.hnjuh.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vs.hahajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://pz.jctech888.com.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://zb.szsharing.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://an.jianghongdianzi.cn

Ruby: arr.sort
来源：http://zj.jianghongdianzi.cn

C#:   list.Sort();
来源：http://kb.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lw.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cd.haigaiapp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zl.lnxyls.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mi.szsharing.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oh.yuntaijiaju.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fm.wgjwhj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mk.nicolike.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://yi.shxzukj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uz.panjiajie.cn

[D11] 反转数组
来源：http://zk.yuexingan06.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ce.colortex.cn

PHP:  array_reverse($arr);
来源：http://qo.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qp.szsharing.cn

TS:   [...arr].reverse();
来源：http://ee.nszjky.cn

Java: Collections.reverse(list);
来源：http://fi.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://ji.muxihuayi.cn

Ruby: arr.reverse
来源：http://gq.muxihuayi.cn

C#:   list.Reverse();
来源：http://qm.lnxyls.cn

[D12] 查找元素下标
来源：http://vr.huanxung.cn

Py:   arr.index(x);  x in arr
来源：http://kv.521024.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://tz.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rm.bjjhwx.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yj.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pi.colortex.cn

Go:   slices.Index(arr, x)
来源：http://pr.szsharing.cn

Ruby: arr.index(x)
来源：http://pu.yuexingan06.cn

C#:   list.IndexOf(x);
来源：http://kk.yuexingan06.cn

[D13] 过滤（保留满足条件的）
来源：http://od.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zk.asd995.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ep.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://tw.huixiangedu.cn

TS:   arr.filter(x => x > 3)
来源：http://gf.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://sg.newstarts.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gq.asd995.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tr.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://pe.colortex.cn

[D14] 映射转换（每个元素变形）
来源：http://sd.muxihuayi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nz.nszjky.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ev.panjiajie.cn

JS:   arr.map(x => x * 2)
来源：http://vm.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://vj.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mr.chemitech.net.cn

Go:   // 手写循环
来源：http://tj.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://sr.shtwfgs.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qu.huixiangedu.cn

[D15] 去重
来源：http://mw.hahajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vz.nicolike.cn

PHP:  array_unique($arr);
来源：http://cf.521024.cn

JS:   [...new Set(arr)]
来源：http://oz.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://nd.colortex.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gu.chemitech.net.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zh.nicolike.cn

Ruby: arr.uniq
来源：http://bf.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://qk.gzmigu.cn

[D16] 求和与平均值
来源：http://zl.szxytkj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zf.shxzskj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sq.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vs.chemitech.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fx.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mo.szxytkj.cn

Go:   // 手写循环累加
来源：http://cv.huixinmuqiang.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wf.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://cm.newstarts.cn

[D17] 最大值与最小值
来源：http://vh.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://rn.bookmarksfly.cn

PHP:  max($arr);  min($arr);
来源：http://cg.asd995.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ls.gzmigu.cn

TS:   Math.max(...arr);
来源：http://wo.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tm.huixiangedu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jr.521024.cn

Ruby: arr.max;  arr.min
来源：http://pf.wgjwhj.cn

C#:   list.Max();  list.Min()
来源：http://sz.hnjuh.cn

[D18] 扁平化嵌套数组
来源：http://hq.hnjuh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lm.jianghongdianzi.cn

PHP:  array_merge(...$nested);
来源：http://po.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://km.jianghongdianzi.cn

TS:   nested.flat();
来源：http://es.panjiajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://re.bookmarksfly.cn

Go:   // 手写双层循环
来源：http://qc.jianghongdianzi.cn

Ruby: nested.flatten
来源：http://hn.jctech888.com.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cb.shxzukj.cn

[D19] 按字段分组
来源：http://sk.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gh.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ip.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jh.newstarts.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ep.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gq.yuntaijiaju.cn

Go:   // 手写 map[string][]T
来源：http://er.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bc.jianghongdianzi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yh.huixinmuqiang.cn

[D20] 统计每个元素出现次数
来源：http://ux.chemitech.net.cn

Py:   Counter(arr)
来源：http://bg.yuexingan06.cn

PHP:  array_count_values($arr);
来源：http://ny.szxytkj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sz.yuntaijiaju.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vi.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fl.chemitech.net.cn

Go:   // 手写 map[T]int
来源：http://ys.hnjuh.cn

Ruby: arr.tally
来源：http://wz.huixinmuqiang.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dr.nszjky.cn

[D21] 判断是否包含某元素
来源：http://ld.nszjky.cn

Py:   x in arr
来源：http://um.jctech888.com.cn

PHP:  in_array($x, $arr, true);
来源：http://wu.szxytkj.cn

JS:   arr.includes(x)
来源：http://ah.shtwfgs.cn

TS:   arr.includes(x)
来源：http://me.521024.cn

Java: list.contains(x)
来源：http://lv.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://qz.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://ej.muxihuayi.cn

C#:   list.Contains(x)
来源：http://tk.521024.cn

[D22] 复制数组（避免共享引用）
来源：http://hp.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oy.huixinmuqiang.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://un.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dw.shtwfgs.cn

TS:   [...arr];
来源：http://xd.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://nx.hahajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://iq.szxytkj.cn

Ruby: arr.dup;  arr.clone
来源：http://rl.asd995.cn

C#:   new List<int>(list);
来源：http://xa.9csxet.cn

[D23] reduce 累积计算
来源：http://ws.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fh.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zn.lnxyls.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zv.shtwfgs.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zb.gzmigu.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://kt.yuexingan06.cn

Go:   // 手写循环
来源：http://pg.jianghongdianzi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bz.haigaiapp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mp.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://ds.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://to.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rf.yuexingan06.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dp.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://nx.lnxyls.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lu.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ye.shxzskj.cn


<!-- 参考信息 -->