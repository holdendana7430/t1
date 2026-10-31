代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://mp.haigaiapp.cn

Ruby: f(a: 1, b: 2)
来源：http://uz.asd995.cn

C#:   f(a: 1, b: 2)
来源：http://ue.huixinmuqiang.cn

[C05] 返回多个值
来源：http://mi.huixiangedu.cn

Py:   return a, b
来源：http://ps.jianghongdianzi.cn

PHP:  return [$a, $b];
来源：http://en.yuexingan06.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://wi.jianghongdianzi.cn

TS:   return { a, b };
来源：http://vi.muxihuayi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://iu.9csxet.cn

Go:   return a, b
来源：http://yq.newstarts.cn

Ruby: return a, b
来源：http://pd.asd995.cn

C#:   return (a, b);              // ValueTuple
来源：http://ni.panjiajie.cn

[C06] 匿名函数 / lambda
来源：http://zp.huanxung.cn

Py:   square = lambda x: x * x
来源：http://go.bjjhwx.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://zn.shxzukj.cn

JS:   const square = x => x * x;
来源：http://ms.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://tq.jianghongdianzi.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://jk.yuntaijiaju.cn

Go:   sq := func(x int) int { return x * x }
来源：http://pp.shtwfgs.cn

Ruby: square = ->(x) { x * x }
来源：http://va.wgjwhj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://ll.newstarts.cn

[C07] 把函数作为参数传入
来源：http://jf.nicolike.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://xa.nszjky.cn

PHP:  array_map("strtoupper", $arr);
来源：http://dk.shxzskj.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://ta.nszjky.cn

TS:   arr.map(String)
来源：http://aa.asd995.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://id.chemitech.net.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://tq.newstarts.cn

Ruby: arr.map(&:upcase)
来源：http://nz.nszjky.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tf.colortex.cn

[C08] 闭包
来源：http://ha.newstarts.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wp.colortex.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://uc.bookmarksfly.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://pl.yuntaijiaju.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://of.nicolike.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://jr.gzmigu.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://qz.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://ha.wgjwhj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hv.haigaiapp.cn

[C09] 递归
来源：http://ui.szsharing.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ce.huixinmuqiang.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://rw.jianghongdianzi.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://py.jianghongdianzi.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://zp.shxzskj.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://kk.huanxung.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://us.jianghongdianzi.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://tp.shxzskj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://ls.9csxet.cn

[C10] 变量作用域
来源：http://hh.nszjky.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://yu.yuntaijiaju.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://uz.chemitech.net.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wq.asd995.cn

TS:   同 JS
来源：http://ni.hnjuh.cn

Java: 方法内为块级作用域
来源：http://lv.hahajie.cn

Go:   花括号块级作用域
来源：http://ij.hnjuh.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://vj.jianghongdianzi.cn

C#:   块级作用域
来源：http://np.huanxung.cn

[C11] 模块导入与导出
来源：http://th.521024.cn

Py:   from module import func
来源：http://dz.huixinmuqiang.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://lu.panjiajie.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://op.yuntaijiaju.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://qr.521024.cn

Java: import java.util.List;
来源：http://vi.nicolike.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qe.newstarts.cn

Ruby: require "json"; require_relative "./util"
来源：http://fm.yuntaijiaju.cn

C#:   using System.Text;
来源：http://jt.jianghongdianzi.cn

[C12] 立即执行函数 IIFE
来源：http://qr.bookmarksfly.cn

Py:   (lambda: print("run"))()
来源：http://hs.hnjuh.cn

PHP:  (function () { echo "run"; })();
来源：http://yo.9csxet.cn

JS:   (() => { console.log("run"); })();
来源：http://yg.gzmigu.cn

TS:   (() => { console.log("run"); })();
来源：http://hc.nszjky.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hm.asd995.cn

Go:   func() { fmt.Println("run") }()
来源：http://gv.gzmigu.cn

Ruby: -> { puts "run" }.call
来源：http://yv.9csxet.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://oz.hnjuh.cn

[C13] 类型声明 / 类型注解
来源：http://fw.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://cz.hnjuh.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xr.shxzukj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://me.haigaiapp.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://uf.shtwfgs.cn

Java: int add(int a, int b) { return a + b; }
来源：http://cr.jctech888.com.cn

Go:   func add(a, b int) int
来源：http://vl.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://an.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fn.521024.cn

[C14] 泛型函数
来源：http://ri.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wl.huixiangedu.cn

PHP:  // 无泛型
来源：http://qg.9csxet.cn

JS:   // 无泛型
来源：http://eg.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://xt.wgjwhj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://cs.yuexingan06.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://cp.bjjhwx.cn

Ruby: # 无泛型
来源：http://im.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vg.hahajie.cn

[C15] 解构 / 展开参数
来源：http://fe.nszjky.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://km.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://kx.bjjhwx.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://yx.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fd.521024.cn

Java: // 无解构
来源：http://da.gzmigu.cn

Go:   // 无解构
来源：http://cx.panjiajie.cn

Ruby: a, b = pair
来源：http://am.9csxet.cn

C#:   var (a, b) = pair;
来源：http://bi.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://xw.nszjky.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://pc.hnjuh.cn

PHP:  // 无重载
来源：http://ge.nszjky.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://nc.bjjhwx.cn

TS:   // 用联合类型或重载签名声明
来源：http://ou.shxzukj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yk.jctech888.com.cn

Go:   // 无重载：用不同函数名
来源：http://le.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://lj.newstarts.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://kl.lnxyls.cn

================================================================================
来源：http://rl.szxytkj.cn

D. 数组 / 列表 / 集合
来源：http://pe.hnjuh.cn

================================================================================
来源：http://zm.yuntaijiaju.cn

[D01] 创建数组 / 列表
来源：http://mm.huixiangedu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://pm.lnxyls.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://an.gzmigu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://rn.shxzukj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://fq.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kb.wgjwhj.cn

Go:   arr := []int{1, 2, 3}
来源：http://vk.haigaiapp.cn

Ruby: arr = [1, 2, 3]
来源：http://nd.yuexingan06.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nj.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://re.jctech888.com.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hw.jianghongdianzi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bs.shtwfgs.cn

JS:   arr.push(4);
来源：http://yr.nszjky.cn

TS:   arr.push(4);
来源：http://hr.shxzukj.cn

Java: list.add(4);
来源：http://vl.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://ws.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://aq.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://to.9csxet.cn

[D03] 在指定位置插入元素
来源：http://xp.muxihuayi.cn

Py:   arr.insert(0, 0)
来源：http://qb.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tt.jianghongdianzi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://jd.9csxet.cn

TS:   arr.splice(0, 0, 0);
来源：http://sk.wgjwhj.cn

Java: list.add(0, 0);
来源：http://hl.shxzukj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wn.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sw.jianghongdianzi.cn

C#:   list.Insert(0, 0);
来源：http://rz.huixinmuqiang.cn

[D04] 删除元素
来源：http://xm.hnjuh.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hk.jctech888.com.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://dz.hnjuh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ag.huanxung.cn

TS:   arr.splice(0, 1);
来源：http://dl.wgjwhj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://gv.521024.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://yr.newstarts.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qe.jianghongdianzi.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tw.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://jq.huixinmuqiang.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xw.yuntaijiaju.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xu.hahajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ih.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://pb.gzmigu.cn

Java: list.get(0); list.set(0, 9);
来源：http://fb.lnxyls.cn

Go:   arr[0]; arr[0] = 9
来源：http://ee.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xr.muxihuayi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bg.chemitech.net.cn

[D06] 数组长度
来源：http://gk.chemitech.net.cn

Py:   len(arr)
来源：http://ow.shxzskj.cn

PHP:  count($arr);
来源：http://rl.gzmigu.cn

JS:   arr.length
来源：http://ad.haigaiapp.cn

TS:   arr.length
来源：http://hz.hnjuh.cn

Java: list.size();
来源：http://cp.521024.cn

Go:   len(arr)
来源：http://zh.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://xp.huixinmuqiang.cn

C#:   list.Count;
来源：http://lc.huanxung.cn

[D07] 切片 / 取子数组
来源：http://rc.yuntaijiaju.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://za.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qu.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://nm.colortex.cn

TS:   arr.slice(1, 4);
来源：http://mo.szxytkj.cn

Java: list.subList(1, 4);
来源：http://nt.gzmigu.cn

Go:   arr[1:4]
来源：http://of.521024.cn

Ruby: arr[1, 3]
来源：http://pu.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://yj.colortex.cn

[D08] 合并两个数组
来源：http://fm.nszjky.cn

Py:   a + b;  a.extend(b)
来源：http://kg.haigaiapp.cn

PHP:  array_merge($a, $b);
来源：http://ha.hnjuh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://oj.huanxung.cn

TS:   [...a, ...b];
来源：http://zk.szxytkj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sj.bjjhwx.cn

Go:   append(a, b...)
来源：http://uc.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://ar.hahajie.cn

C#:   a.Concat(b).ToList()
来源：http://qv.wgjwhj.cn

[D09] 排序（升序）
来源：http://jk.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://hl.asd995.cn

PHP:  sort($arr);
来源：http://jg.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ql.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ga.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gd.nszjky.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ht.colortex.cn

Ruby: arr.sort
来源：http://vc.bookmarksfly.cn

C#:   list.Sort();
来源：http://sq.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lv.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mk.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://so.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://vd.9csxet.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dn.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hc.bjjhwx.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mk.jctech888.com.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vg.huanxung.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ry.shxzukj.cn

[D11] 反转数组
来源：http://qg.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://br.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://wt.nszjky.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://of.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://go.haigaiapp.cn

Java: Collections.reverse(list);
来源：http://sx.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://fe.huixinmuqiang.cn

Ruby: arr.reverse
来源：http://gr.nszjky.cn

C#:   list.Reverse();
来源：http://rr.gzmigu.cn

[D12] 查找元素下标
来源：http://we.521024.cn

Py:   arr.index(x);  x in arr
来源：http://ot.shxzskj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eh.jctech888.com.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yt.huanxung.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hh.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gq.nszjky.cn

Go:   slices.Index(arr, x)
来源：http://bj.bjjhwx.cn

Ruby: arr.index(x)
来源：http://kb.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://dh.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://uf.jianghongdianzi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ww.nszjky.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vy.haigaiapp.cn

JS:   arr.filter(x => x > 3)
来源：http://va.jianghongdianzi.cn

TS:   arr.filter(x => x > 3)
来源：http://ro.wgjwhj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gx.lnxyls.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://dy.nicolike.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fl.szxytkj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ie.muxihuayi.cn

[D14] 映射转换（每个元素变形）
来源：http://sr.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://np.nszjky.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://nr.jctech888.com.cn

JS:   arr.map(x => x * 2)
来源：http://vm.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://sl.shtwfgs.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://za.colortex.cn

Go:   // 手写循环
来源：http://zi.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://go.shxzukj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rf.wgjwhj.cn

[D15] 去重
来源：http://dn.huixinmuqiang.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gn.nszjky.cn

PHP:  array_unique($arr);
来源：http://lv.9csxet.cn

JS:   [...new Set(arr)]
来源：http://ru.9csxet.cn

TS:   [...new Set(arr)]
来源：http://nu.nicolike.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zn.hahajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://as.huixiangedu.cn

Ruby: arr.uniq
来源：http://rk.chemitech.net.cn

C#:   list.Distinct().ToList()
来源：http://lc.lnxyls.cn

[D16] 求和与平均值
来源：http://pw.newstarts.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ok.gzmigu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iv.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ic.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ea.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://sy.bjjhwx.cn

Go:   // 手写循环累加
来源：http://kx.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sl.szxytkj.cn

C#:   list.Sum();  list.Average()
来源：http://on.shxzskj.cn

[D17] 最大值与最小值
来源：http://vb.szsharing.cn

Py:   max(arr);  min(arr)
来源：http://eq.yuntaijiaju.cn

PHP:  max($arr);  min($arr);
来源：http://gw.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bq.yuntaijiaju.cn

TS:   Math.max(...arr);
来源：http://jd.nszjky.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nk.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ww.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://ph.nicolike.cn

C#:   list.Max();  list.Min()
来源：http://oc.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://pk.bookmarksfly.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xq.hnjuh.cn

PHP:  array_merge(...$nested);
来源：http://jf.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://le.asd995.cn

TS:   nested.flat();
来源：http://co.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gx.hahajie.cn

Go:   // 手写双层循环
来源：http://sh.huixiangedu.cn

Ruby: nested.flatten
来源：http://la.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hy.jctech888.com.cn

[D19] 按字段分组
来源：http://fn.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kw.huixiangedu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zv.panjiajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nt.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://st.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ij.lnxyls.cn

Go:   // 手写 map[string][]T
来源：http://qc.bjjhwx.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://th.hahajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pf.huixiangedu.cn

[D20] 统计每个元素出现次数
来源：http://ga.haigaiapp.cn

Py:   Counter(arr)
来源：http://jv.wgjwhj.cn

PHP:  array_count_values($arr);
来源：http://oe.szsharing.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mq.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ek.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bd.521024.cn

Go:   // 手写 map[T]int
来源：http://bl.yuntaijiaju.cn

Ruby: arr.tally
来源：http://vu.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://by.szsharing.cn

[D21] 判断是否包含某元素
来源：http://wk.shtwfgs.cn

Py:   x in arr
来源：http://uk.yuntaijiaju.cn

PHP:  in_array($x, $arr, true);
来源：http://dm.yuntaijiaju.cn

JS:   arr.includes(x)
来源：http://xv.huixiangedu.cn

TS:   arr.includes(x)
来源：http://rr.yuntaijiaju.cn

Java: list.contains(x)
来源：http://mt.nicolike.cn


<!-- 参考信息 -->