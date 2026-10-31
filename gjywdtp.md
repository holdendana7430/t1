代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://uv.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://cu.muxihuayi.cn

C#:   f(a: 1, b: 2)
来源：http://me.wgjwhj.cn

[C05] 返回多个值
来源：http://cg.9csxet.cn

Py:   return a, b
来源：http://rl.jianghongdianzi.cn

PHP:  return [$a, $b];
来源：http://vl.jctech888.com.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wn.521024.cn

TS:   return { a, b };
来源：http://fp.yuntaijiaju.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://fo.yuexingan06.cn

Go:   return a, b
来源：http://ow.9csxet.cn

Ruby: return a, b
来源：http://nm.haigaiapp.cn

C#:   return (a, b);              // ValueTuple
来源：http://lq.nszjky.cn

[C06] 匿名函数 / lambda
来源：http://dn.bjjhwx.cn

Py:   square = lambda x: x * x
来源：http://pr.hahajie.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wg.asd995.cn

JS:   const square = x => x * x;
来源：http://ja.9csxet.cn

TS:   const square = (x: number): number => x * x;
来源：http://xq.nicolike.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://az.szxytkj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://bd.newstarts.cn

Ruby: square = ->(x) { x * x }
来源：http://oq.shxzskj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://py.shxzukj.cn

[C07] 把函数作为参数传入
来源：http://ku.nszjky.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://bs.hahajie.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dy.newstarts.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://fk.asd995.cn

TS:   arr.map(String)
来源：http://af.bjjhwx.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://lj.szsharing.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://or.colortex.cn

Ruby: arr.map(&:upcase)
来源：http://sr.shxzskj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://uv.asd995.cn

[C08] 闭包
来源：http://ik.jianghongdianzi.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://dv.gzmigu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://ub.huanxung.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://yf.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://pb.lnxyls.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mz.shxzukj.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://nf.gzmigu.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://fj.gzmigu.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ny.szxytkj.cn

[C09] 递归
来源：http://xw.shxzskj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://zd.shxzskj.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wa.wgjwhj.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://ti.shxzskj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bg.huixiangedu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://ur.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://ol.huanxung.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://ev.yuexingan06.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://zk.yuexingan06.cn

[C10] 变量作用域
来源：http://um.newstarts.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://nx.hahajie.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xc.szsharing.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://qm.shxzskj.cn

TS:   同 JS
来源：http://mz.lnxyls.cn

Java: 方法内为块级作用域
来源：http://pf.panjiajie.cn

Go:   花括号块级作用域
来源：http://sd.wgjwhj.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://my.huixiangedu.cn

C#:   块级作用域
来源：http://gh.wgjwhj.cn

[C11] 模块导入与导出
来源：http://co.huanxung.cn

Py:   from module import func
来源：http://ok.521024.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lt.wgjwhj.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ih.yuexingan06.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ok.jianghongdianzi.cn

Java: import java.util.List;
来源：http://ad.panjiajie.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://vj.huixiangedu.cn

Ruby: require "json"; require_relative "./util"
来源：http://lm.bookmarksfly.cn

C#:   using System.Text;
来源：http://mx.yuntaijiaju.cn

[C12] 立即执行函数 IIFE
来源：http://tf.panjiajie.cn

Py:   (lambda: print("run"))()
来源：http://ki.shxzukj.cn

PHP:  (function () { echo "run"; })();
来源：http://er.bjjhwx.cn

JS:   (() => { console.log("run"); })();
来源：http://ci.colortex.cn

TS:   (() => { console.log("run"); })();
来源：http://pg.hahajie.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bm.muxihuayi.cn

Go:   func() { fmt.Println("run") }()
来源：http://vu.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://xe.shtwfgs.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://kj.panjiajie.cn

[C13] 类型声明 / 类型注解
来源：http://rx.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://kg.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vk.nszjky.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ga.nicolike.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://rp.yuntaijiaju.cn

Java: int add(int a, int b) { return a + b; }
来源：http://po.szsharing.cn

Go:   func add(a, b int) int
来源：http://ih.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://kd.yuntaijiaju.cn

C#:   int Add(int a, int b) => a + b;
来源：http://mj.hahajie.cn

[C14] 泛型函数
来源：http://lt.szsharing.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://rr.lnxyls.cn

PHP:  // 无泛型
来源：http://ml.jianghongdianzi.cn

JS:   // 无泛型
来源：http://wx.colortex.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://sc.yuntaijiaju.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://vr.asd995.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pf.huixinmuqiang.cn

Ruby: # 无泛型
来源：http://jc.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://om.9csxet.cn

[C15] 解构 / 展开参数
来源：http://df.wgjwhj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bw.colortex.cn

PHP:  [$a, $b] = $pair;
来源：http://oi.nszjky.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://zc.newstarts.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://qe.haigaiapp.cn

Java: // 无解构
来源：http://eh.hahajie.cn

Go:   // 无解构
来源：http://oc.nszjky.cn

Ruby: a, b = pair
来源：http://cz.huanxung.cn

C#:   var (a, b) = pair;
来源：http://om.9csxet.cn

[C16] 函数 / 方法重载
来源：http://ac.huixiangedu.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ii.szsharing.cn

PHP:  // 无重载
来源：http://fs.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ie.szxytkj.cn

TS:   // 用联合类型或重载签名声明
来源：http://sv.asd995.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ut.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://fg.chemitech.net.cn

Ruby: # 无重载：靠动态参数
来源：http://fj.szsharing.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://nw.chemitech.net.cn

================================================================================
来源：http://mf.bjjhwx.cn

D. 数组 / 列表 / 集合
来源：http://jk.huanxung.cn

================================================================================
来源：http://fb.521024.cn

[D01] 创建数组 / 列表
来源：http://hv.shxzskj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pp.haigaiapp.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://sj.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gx.chemitech.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://wz.asd995.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vf.huanxung.cn

Go:   arr := []int{1, 2, 3}
来源：http://rv.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://jf.lnxyls.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ml.muxihuayi.cn

[D02] 追加元素到末尾
来源：http://dx.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lb.lnxyls.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mr.haigaiapp.cn

JS:   arr.push(4);
来源：http://rl.szsharing.cn

TS:   arr.push(4);
来源：http://bm.bookmarksfly.cn

Java: list.add(4);
来源：http://gs.shxzukj.cn

Go:   arr = append(arr, 4)
来源：http://sh.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://dd.huixiangedu.cn

C#:   list.Add(4);
来源：http://qp.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://wo.521024.cn

Py:   arr.insert(0, 0)
来源：http://xh.szsharing.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ct.szsharing.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ci.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://jt.yuexingan06.cn

Java: list.add(0, 0);
来源：http://yp.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ai.521024.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://yq.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://ia.nicolike.cn

[D04] 删除元素
来源：http://vh.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xa.hahajie.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uq.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qq.wgjwhj.cn

TS:   arr.splice(0, 1);
来源：http://qr.colortex.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gc.hnjuh.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pd.asd995.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ww.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pf.nszjky.cn

[D05] 访问与修改元素
来源：http://uh.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://at.huixiangedu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gz.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bc.szxytkj.cn

TS:   arr[0]; arr.at(-1);
来源：http://yg.nszjky.cn

Java: list.get(0); list.set(0, 9);
来源：http://ov.hahajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://df.huixinmuqiang.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ni.colortex.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nz.jianghongdianzi.cn

[D06] 数组长度
来源：http://oj.haigaiapp.cn

Py:   len(arr)
来源：http://um.wgjwhj.cn

PHP:  count($arr);
来源：http://dd.jctech888.com.cn

JS:   arr.length
来源：http://ad.asd995.cn

TS:   arr.length
来源：http://pl.nicolike.cn

Java: list.size();
来源：http://fx.huixiangedu.cn

Go:   len(arr)
来源：http://wy.huixinmuqiang.cn

Ruby: arr.length; arr.size
来源：http://px.jianghongdianzi.cn

C#:   list.Count;
来源：http://ub.9csxet.cn

[D07] 切片 / 取子数组
来源：http://gz.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://jl.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://no.haigaiapp.cn

JS:   arr.slice(1, 4);
来源：http://ro.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://lr.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://fn.bookmarksfly.cn

Go:   arr[1:4]
来源：http://he.yuntaijiaju.cn

Ruby: arr[1, 3]
来源：http://co.asd995.cn

C#:   list.GetRange(1, 3);
来源：http://bn.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://zu.chemitech.net.cn

Py:   a + b;  a.extend(b)
来源：http://zm.wgjwhj.cn

PHP:  array_merge($a, $b);
来源：http://gk.colortex.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jh.wgjwhj.cn

TS:   [...a, ...b];
来源：http://dh.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vu.newstarts.cn

Go:   append(a, b...)
来源：http://sd.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://et.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://yb.521024.cn

[D09] 排序（升序）
来源：http://hg.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://yt.shxzskj.cn

PHP:  sort($arr);
来源：http://ju.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://rf.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rr.9csxet.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ar.yuntaijiaju.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://fq.hnjuh.cn

Ruby: arr.sort
来源：http://de.szxytkj.cn

C#:   list.Sort();
来源：http://zi.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://es.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ae.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://sw.panjiajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://nt.bjjhwx.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pt.shtwfgs.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pr.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://xs.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bh.bjjhwx.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://id.jctech888.com.cn

[D11] 反转数组
来源：http://wz.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://jt.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://kn.lnxyls.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fq.lnxyls.cn

TS:   [...arr].reverse();
来源：http://jm.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://nw.wgjwhj.cn

Go:   slices.Reverse(arr)
来源：http://np.muxihuayi.cn

Ruby: arr.reverse
来源：http://lc.hahajie.cn

C#:   list.Reverse();
来源：http://jr.muxihuayi.cn

[D12] 查找元素下标
来源：http://eb.szxytkj.cn

Py:   arr.index(x);  x in arr
来源：http://vj.szsharing.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://iy.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oh.bjjhwx.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lf.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sq.shxzskj.cn

Go:   slices.Index(arr, x)
来源：http://yb.haigaiapp.cn

Ruby: arr.index(x)
来源：http://xw.huixiangedu.cn

C#:   list.IndexOf(x);
来源：http://hs.newstarts.cn

[D13] 过滤（保留满足条件的）
来源：http://uo.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://iz.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://im.9csxet.cn

JS:   arr.filter(x => x > 3)
来源：http://kq.shtwfgs.cn

TS:   arr.filter(x => x > 3)
来源：http://hd.huixinmuqiang.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ap.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gx.jctech888.com.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qz.521024.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kw.gzmigu.cn

[D14] 映射转换（每个元素变形）
来源：http://kv.yuexingan06.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ts.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://um.bookmarksfly.cn

JS:   arr.map(x => x * 2)
来源：http://yj.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://ua.newstarts.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dl.lnxyls.cn

Go:   // 手写循环
来源：http://gp.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ve.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yj.yuntaijiaju.cn

[D15] 去重
来源：http://gp.asd995.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mp.szsharing.cn

PHP:  array_unique($arr);
来源：http://gc.gzmigu.cn

JS:   [...new Set(arr)]
来源：http://kp.nszjky.cn

TS:   [...new Set(arr)]
来源：http://dv.szsharing.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zc.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nd.lnxyls.cn

Ruby: arr.uniq
来源：http://hj.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://kv.colortex.cn

[D16] 求和与平均值
来源：http://pl.jianghongdianzi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://zr.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ls.bookmarksfly.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mw.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hl.huixiangedu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pq.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://ds.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://iu.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://kj.wgjwhj.cn

[D17] 最大值与最小值
来源：http://li.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://nc.lnxyls.cn

PHP:  max($arr);  min($arr);
来源：http://ly.hahajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://kr.shtwfgs.cn

TS:   Math.max(...arr);
来源：http://vt.jctech888.com.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yr.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hu.chemitech.net.cn

Ruby: arr.max;  arr.min
来源：http://yl.chemitech.net.cn

C#:   list.Max();  list.Min()
来源：http://ki.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://ae.bookmarksfly.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://al.asd995.cn

PHP:  array_merge(...$nested);
来源：http://hu.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://me.jianghongdianzi.cn

TS:   nested.flat();
来源：http://ft.asd995.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pp.nszjky.cn

Go:   // 手写双层循环
来源：http://ft.newstarts.cn

Ruby: nested.flatten
来源：http://xy.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ql.asd995.cn

[D19] 按字段分组
来源：http://gf.szxytkj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://oz.jctech888.com.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pw.hnjuh.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vm.shxzukj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ej.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cs.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://um.jctech888.com.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://rw.muxihuayi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ql.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://pl.chemitech.net.cn

Py:   Counter(arr)
来源：http://zj.huixiangedu.cn

PHP:  array_count_values($arr);
来源：http://so.muxihuayi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ny.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tl.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ld.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://jr.shxzskj.cn

Ruby: arr.tally
来源：http://ab.shtwfgs.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wy.yuexingan06.cn

[D21] 判断是否包含某元素
来源：http://wy.nszjky.cn

Py:   x in arr
来源：http://wr.521024.cn

PHP:  in_array($x, $arr, true);
来源：http://yn.shxzskj.cn

JS:   arr.includes(x)
来源：http://ot.yuexingan06.cn

TS:   arr.includes(x)
来源：http://jc.newstarts.cn

Java: list.contains(x)
来源：http://wa.nszjky.cn


<!-- 参考信息 -->