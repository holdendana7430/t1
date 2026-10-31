代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://iz.hahajie.cn

Ruby: f(a: 1, b: 2)
来源：http://ry.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://bz.wgjwhj.cn

[C05] 返回多个值
来源：http://wr.jctech888.com.cn

Py:   return a, b
来源：http://ub.jianghongdianzi.cn

PHP:  return [$a, $b];
来源：http://re.jctech888.com.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wb.asd995.cn

TS:   return { a, b };
来源：http://sg.muxihuayi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xy.chemitech.net.cn

Go:   return a, b
来源：http://wv.szxytkj.cn

Ruby: return a, b
来源：http://ju.bookmarksfly.cn

C#:   return (a, b);              // ValueTuple
来源：http://zc.shxzukj.cn

[C06] 匿名函数 / lambda
来源：http://iq.bookmarksfly.cn

Py:   square = lambda x: x * x
来源：http://rb.huixiangedu.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://lt.lnxyls.cn

JS:   const square = x => x * x;
来源：http://hg.shxzukj.cn

TS:   const square = (x: number): number => x * x;
来源：http://nc.shtwfgs.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ao.newstarts.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pq.shxzukj.cn

Ruby: square = ->(x) { x * x }
来源：http://ox.huixinmuqiang.cn

C#:   Func<int, int> square = x => x * x;
来源：http://wr.szsharing.cn

[C07] 把函数作为参数传入
来源：http://oj.huixinmuqiang.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://jb.shtwfgs.cn

PHP:  array_map("strtoupper", $arr);
来源：http://vl.huixinmuqiang.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://qr.hahajie.cn

TS:   arr.map(String)
来源：http://mk.521024.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://gr.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://td.yuntaijiaju.cn

Ruby: arr.map(&:upcase)
来源：http://hz.hahajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://jp.hnjuh.cn

[C08] 闭包
来源：http://gn.bjjhwx.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mp.shxzukj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://he.shtwfgs.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://ik.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hh.yuntaijiaju.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://rv.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://dn.chemitech.net.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://kn.chemitech.net.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://yq.nicolike.cn

[C09] 递归
来源：http://xb.hnjuh.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://dv.shtwfgs.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mc.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://cw.shxzskj.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://rf.gzmigu.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kt.gzmigu.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://jt.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://en.bjjhwx.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://qb.lnxyls.cn

[C10] 变量作用域
来源：http://nb.chemitech.net.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ad.huanxung.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://qf.shxzskj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tp.newstarts.cn

TS:   同 JS
来源：http://ys.nszjky.cn

Java: 方法内为块级作用域
来源：http://sp.newstarts.cn

Go:   花括号块级作用域
来源：http://ax.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://zl.shxzukj.cn

C#:   块级作用域
来源：http://rj.wgjwhj.cn

[C11] 模块导入与导出
来源：http://qq.jianghongdianzi.cn

Py:   from module import func
来源：http://ha.bookmarksfly.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://aw.jianghongdianzi.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lc.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://as.haigaiapp.cn

Java: import java.util.List;
来源：http://wn.521024.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://cj.shtwfgs.cn

Ruby: require "json"; require_relative "./util"
来源：http://cq.jianghongdianzi.cn

C#:   using System.Text;
来源：http://ts.gzmigu.cn

[C12] 立即执行函数 IIFE
来源：http://vm.asd995.cn

Py:   (lambda: print("run"))()
来源：http://aq.hahajie.cn

PHP:  (function () { echo "run"; })();
来源：http://zm.chemitech.net.cn

JS:   (() => { console.log("run"); })();
来源：http://no.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://wg.szxytkj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://cm.haigaiapp.cn

Go:   func() { fmt.Println("run") }()
来源：http://zh.colortex.cn

Ruby: -> { puts "run" }.call
来源：http://eu.nszjky.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qr.huanxung.cn

[C13] 类型声明 / 类型注解
来源：http://bh.bookmarksfly.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ib.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uv.chemitech.net.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ce.szsharing.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://on.lnxyls.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bn.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://gi.hnjuh.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vn.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://by.huanxung.cn

[C14] 泛型函数
来源：http://ko.huanxung.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://fq.haigaiapp.cn

PHP:  // 无泛型
来源：http://js.shxzukj.cn

JS:   // 无泛型
来源：http://gz.yuexingan06.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://cv.huixinmuqiang.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ur.shxzskj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fc.colortex.cn

Ruby: # 无泛型
来源：http://wr.bjjhwx.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xu.jctech888.com.cn

[C15] 解构 / 展开参数
来源：http://ix.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yv.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://tu.asd995.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://lv.521024.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://vl.newstarts.cn

Java: // 无解构
来源：http://ad.lnxyls.cn

Go:   // 无解构
来源：http://ws.szxytkj.cn

Ruby: a, b = pair
来源：http://np.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://as.chemitech.net.cn

[C16] 函数 / 方法重载
来源：http://uh.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://nw.hahajie.cn

PHP:  // 无重载
来源：http://ae.szxytkj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://vd.gzmigu.cn

TS:   // 用联合类型或重载签名声明
来源：http://vl.haigaiapp.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kw.shxzukj.cn

Go:   // 无重载：用不同函数名
来源：http://ba.bjjhwx.cn

Ruby: # 无重载：靠动态参数
来源：http://gm.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yx.hnjuh.cn

================================================================================
来源：http://ta.hnjuh.cn

D. 数组 / 列表 / 集合
来源：http://mu.lnxyls.cn

================================================================================
来源：http://ab.gzmigu.cn

[D01] 创建数组 / 列表
来源：http://zo.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vk.nszjky.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://ra.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rh.shxzukj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://xk.yuexingan06.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://pv.huanxung.cn

Go:   arr := []int{1, 2, 3}
来源：http://cr.shxzskj.cn

Ruby: arr = [1, 2, 3]
来源：http://ul.shxzukj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ai.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://he.wgjwhj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yr.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://tx.yuexingan06.cn

JS:   arr.push(4);
来源：http://zb.hnjuh.cn

TS:   arr.push(4);
来源：http://kh.newstarts.cn

Java: list.add(4);
来源：http://jb.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://jw.nszjky.cn

Ruby: arr << 4; arr.push(5)
来源：http://pg.yuexingan06.cn

C#:   list.Add(4);
来源：http://wh.wgjwhj.cn

[D03] 在指定位置插入元素
来源：http://tv.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://vs.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://qo.newstarts.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://er.hahajie.cn

TS:   arr.splice(0, 0, 0);
来源：http://hh.hnjuh.cn

Java: list.add(0, 0);
来源：http://we.colortex.cn

Go:   arr = append([]int{0}, arr...)
来源：http://og.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ji.nszjky.cn

C#:   list.Insert(0, 0);
来源：http://wr.szxytkj.cn

[D04] 删除元素
来源：http://ly.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ea.chemitech.net.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tx.bookmarksfly.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ue.hnjuh.cn

TS:   arr.splice(0, 1);
来源：http://sk.bookmarksfly.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://yh.shtwfgs.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ni.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://yz.hnjuh.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://fv.huixiangedu.cn

[D05] 访问与修改元素
来源：http://vh.bookmarksfly.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zh.bjjhwx.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://op.hnjuh.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ug.nicolike.cn

TS:   arr[0]; arr.at(-1);
来源：http://oa.shxzukj.cn

Java: list.get(0); list.set(0, 9);
来源：http://bh.newstarts.cn

Go:   arr[0]; arr[0] = 9
来源：http://ct.nszjky.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ts.asd995.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sh.colortex.cn

[D06] 数组长度
来源：http://ao.lnxyls.cn

Py:   len(arr)
来源：http://jg.huixinmuqiang.cn

PHP:  count($arr);
来源：http://xb.colortex.cn

JS:   arr.length
来源：http://sa.shtwfgs.cn

TS:   arr.length
来源：http://qm.szsharing.cn

Java: list.size();
来源：http://fk.huixinmuqiang.cn

Go:   len(arr)
来源：http://zr.huixiangedu.cn

Ruby: arr.length; arr.size
来源：http://aw.hnjuh.cn

C#:   list.Count;
来源：http://zf.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://jz.nicolike.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uf.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sm.gzmigu.cn

JS:   arr.slice(1, 4);
来源：http://ve.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://js.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://yf.hnjuh.cn

Go:   arr[1:4]
来源：http://fv.wgjwhj.cn

Ruby: arr[1, 3]
来源：http://iy.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://ik.lnxyls.cn

[D08] 合并两个数组
来源：http://yp.521024.cn

Py:   a + b;  a.extend(b)
来源：http://yb.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://dy.hahajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://az.newstarts.cn

TS:   [...a, ...b];
来源：http://cw.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ak.shxzskj.cn

Go:   append(a, b...)
来源：http://ky.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://iz.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://rj.huixiangedu.cn

[D09] 排序（升序）
来源：http://uz.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://kl.haigaiapp.cn

PHP:  sort($arr);
来源：http://rj.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ef.hahajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ev.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oc.szsharing.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hn.wgjwhj.cn

Ruby: arr.sort
来源：http://hz.yuntaijiaju.cn

C#:   list.Sort();
来源：http://wf.gzmigu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fh.lnxyls.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vu.nszjky.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hh.jianghongdianzi.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rp.gzmigu.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nn.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wr.yuexingan06.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vy.panjiajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://km.shtwfgs.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://xq.gzmigu.cn

[D11] 反转数组
来源：http://df.asd995.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wc.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://nz.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://rr.9csxet.cn

TS:   [...arr].reverse();
来源：http://oc.chemitech.net.cn

Java: Collections.reverse(list);
来源：http://ge.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://bi.chemitech.net.cn

Ruby: arr.reverse
来源：http://zn.asd995.cn

C#:   list.Reverse();
来源：http://tx.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://nz.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://zf.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lu.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zy.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yp.gzmigu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sq.9csxet.cn

Go:   slices.Index(arr, x)
来源：http://sh.hnjuh.cn

Ruby: arr.index(x)
来源：http://nu.hahajie.cn

C#:   list.IndexOf(x);
来源：http://de.bookmarksfly.cn

[D13] 过滤（保留满足条件的）
来源：http://zi.jianghongdianzi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pu.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://nb.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://xd.chemitech.net.cn

TS:   arr.filter(x => x > 3)
来源：http://vr.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ie.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://my.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://aa.haigaiapp.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ig.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://xx.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fe.shxzukj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nh.521024.cn

JS:   arr.map(x => x * 2)
来源：http://gu.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://so.yuexingan06.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ee.szsharing.cn

Go:   // 手写循环
来源：http://fm.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://er.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://go.panjiajie.cn

[D15] 去重
来源：http://qi.chemitech.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mk.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://lu.haigaiapp.cn

JS:   [...new Set(arr)]
来源：http://mp.chemitech.net.cn

TS:   [...new Set(arr)]
来源：http://pr.asd995.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://za.huixinmuqiang.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lh.hahajie.cn

Ruby: arr.uniq
来源：http://pw.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://cw.hahajie.cn

[D16] 求和与平均值
来源：http://pq.shtwfgs.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ng.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vs.yuntaijiaju.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yj.gzmigu.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gr.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ml.yuexingan06.cn

Go:   // 手写循环累加
来源：http://er.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ge.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://xk.9csxet.cn

[D17] 最大值与最小值
来源：http://zg.chemitech.net.cn

Py:   max(arr);  min(arr)
来源：http://hp.521024.cn

PHP:  max($arr);  min($arr);
来源：http://zx.shxzukj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nh.lnxyls.cn

TS:   Math.max(...arr);
来源：http://yr.521024.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://rz.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zq.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://fo.hnjuh.cn

C#:   list.Max();  list.Min()
来源：http://ad.newstarts.cn

[D18] 扁平化嵌套数组
来源：http://up.panjiajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ns.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://zh.hnjuh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ts.haigaiapp.cn

TS:   nested.flat();
来源：http://ui.huixinmuqiang.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yr.shxzskj.cn

Go:   // 手写双层循环
来源：http://tv.panjiajie.cn

Ruby: nested.flatten
来源：http://ik.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xt.521024.cn

[D19] 按字段分组
来源：http://jx.jianghongdianzi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://au.jctech888.com.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ta.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nl.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yc.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xu.yuexingan06.cn

Go:   // 手写 map[string][]T
来源：http://db.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://gf.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rx.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://ya.nicolike.cn

Py:   Counter(arr)
来源：http://bv.szsharing.cn

PHP:  array_count_values($arr);
来源：http://rg.bookmarksfly.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fe.chemitech.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bz.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rr.asd995.cn

Go:   // 手写 map[T]int
来源：http://qv.huixiangedu.cn

Ruby: arr.tally
来源：http://ob.huanxung.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dh.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://yj.huixinmuqiang.cn

Py:   x in arr
来源：http://po.jctech888.com.cn

PHP:  in_array($x, $arr, true);
来源：http://gb.wgjwhj.cn

JS:   arr.includes(x)
来源：http://ml.lnxyls.cn

TS:   arr.includes(x)
来源：http://kr.colortex.cn

Java: list.contains(x)
来源：http://iy.huixiangedu.cn


<!-- 参考信息 -->