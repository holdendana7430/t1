代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://vy.yuntaijiaju.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://sm.chemitech.net.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ud.shxzskj.cn

Java: // 无：用 Builder 模式或 record
来源：http://dt.yuexingan06.cn

Go:   // 无：用配置结构体参数
来源：http://ep.huanxung.cn

Ruby: f(a: 1, b: 2)
来源：http://et.panjiajie.cn

C#:   f(a: 1, b: 2)
来源：http://eo.hnjuh.cn

[C05] 返回多个值
来源：http://os.lnxyls.cn

Py:   return a, b
来源：http://fx.nszjky.cn

PHP:  return [$a, $b];
来源：http://zd.bjjhwx.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://un.huanxung.cn

TS:   return { a, b };
来源：http://uv.szxytkj.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ts.521024.cn

Go:   return a, b
来源：http://kl.asd995.cn

Ruby: return a, b
来源：http://eg.jctech888.com.cn

C#:   return (a, b);              // ValueTuple
来源：http://ub.lnxyls.cn

[C06] 匿名函数 / lambda
来源：http://on.shtwfgs.cn

Py:   square = lambda x: x * x
来源：http://uo.jianghongdianzi.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://ih.huanxung.cn

JS:   const square = x => x * x;
来源：http://cr.jctech888.com.cn

TS:   const square = (x: number): number => x * x;
来源：http://ns.nszjky.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://ji.shxzskj.cn

Go:   sq := func(x int) int { return x * x }
来源：http://lb.yuexingan06.cn

Ruby: square = ->(x) { x * x }
来源：http://oi.panjiajie.cn

C#:   Func<int, int> square = x => x * x;
来源：http://hw.yuntaijiaju.cn

[C07] 把函数作为参数传入
来源：http://ku.yuexingan06.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://vu.9csxet.cn

PHP:  array_map("strtoupper", $arr);
来源：http://wn.newstarts.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://yq.yuntaijiaju.cn

TS:   arr.map(String)
来源：http://us.gzmigu.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hx.gzmigu.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://kc.shxzukj.cn

Ruby: arr.map(&:upcase)
来源：http://dg.gzmigu.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://gd.shxzskj.cn

[C08] 闭包
来源：http://sc.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://kl.newstarts.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://zp.jctech888.com.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://qw.huixiangedu.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://gj.chemitech.net.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hi.bjjhwx.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://ch.shxzskj.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wv.wgjwhj.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://kt.hahajie.cn

[C09] 递归
来源：http://aa.shxzskj.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://tk.521024.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://nz.yuntaijiaju.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://fb.huixinmuqiang.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bl.521024.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://bb.muxihuayi.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://bm.haigaiapp.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://zb.colortex.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://un.jianghongdianzi.cn

[C10] 变量作用域
来源：http://ee.asd995.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qz.521024.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://be.nicolike.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://df.yuexingan06.cn

TS:   同 JS
来源：http://rn.9csxet.cn

Java: 方法内为块级作用域
来源：http://cp.9csxet.cn

Go:   花括号块级作用域
来源：http://xy.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://bc.nszjky.cn

C#:   块级作用域
来源：http://jx.huixiangedu.cn

[C11] 模块导入与导出
来源：http://xm.jianghongdianzi.cn

Py:   from module import func
来源：http://gv.nszjky.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://kb.jctech888.com.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ro.muxihuayi.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://pa.shxzukj.cn

Java: import java.util.List;
来源：http://hu.huixinmuqiang.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://nn.shxzukj.cn

Ruby: require "json"; require_relative "./util"
来源：http://wv.huixinmuqiang.cn

C#:   using System.Text;
来源：http://ej.bookmarksfly.cn

[C12] 立即执行函数 IIFE
来源：http://fq.521024.cn

Py:   (lambda: print("run"))()
来源：http://dd.huixiangedu.cn

PHP:  (function () { echo "run"; })();
来源：http://nq.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://gd.nszjky.cn

TS:   (() => { console.log("run"); })();
来源：http://si.521024.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://qn.haigaiapp.cn

Go:   func() { fmt.Println("run") }()
来源：http://zm.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://ub.haigaiapp.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://li.newstarts.cn

[C13] 类型声明 / 类型注解
来源：http://kp.szxytkj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://sc.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://iy.yuntaijiaju.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://em.hahajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wu.nszjky.cn

Java: int add(int a, int b) { return a + b; }
来源：http://yk.nicolike.cn

Go:   func add(a, b int) int
来源：http://dy.szsharing.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ja.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://nm.huixinmuqiang.cn

[C14] 泛型函数
来源：http://ag.colortex.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://xj.yuntaijiaju.cn

PHP:  // 无泛型
来源：http://gz.521024.cn

JS:   // 无泛型
来源：http://dd.hnjuh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://nt.panjiajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wy.hnjuh.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://pp.gzmigu.cn

Ruby: # 无泛型
来源：http://tj.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hj.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://lk.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://yc.szsharing.cn

PHP:  [$a, $b] = $pair;
来源：http://zk.muxihuayi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://jz.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fj.huixinmuqiang.cn

Java: // 无解构
来源：http://bg.wgjwhj.cn

Go:   // 无解构
来源：http://lv.jianghongdianzi.cn

Ruby: a, b = pair
来源：http://yg.hnjuh.cn

C#:   var (a, b) = pair;
来源：http://pm.huanxung.cn

[C16] 函数 / 方法重载
来源：http://te.hnjuh.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jg.jctech888.com.cn

PHP:  // 无重载
来源：http://ut.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://te.nszjky.cn

TS:   // 用联合类型或重载签名声明
来源：http://qz.9csxet.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://xa.szsharing.cn

Go:   // 无重载：用不同函数名
来源：http://dk.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://kv.bjjhwx.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yj.huanxung.cn

================================================================================
来源：http://vz.shxzukj.cn

D. 数组 / 列表 / 集合
来源：http://fj.newstarts.cn

================================================================================
来源：http://jo.huanxung.cn

[D01] 创建数组 / 列表
来源：http://ms.9csxet.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://io.yuexingan06.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qn.lnxyls.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ls.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bw.huanxung.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vq.colortex.cn

Go:   arr := []int{1, 2, 3}
来源：http://qt.shxzskj.cn

Ruby: arr = [1, 2, 3]
来源：http://sc.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://nd.huanxung.cn

[D02] 追加元素到末尾
来源：http://xr.shtwfgs.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://bq.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://jy.yuntaijiaju.cn

JS:   arr.push(4);
来源：http://cg.chemitech.net.cn

TS:   arr.push(4);
来源：http://nk.newstarts.cn

Java: list.add(4);
来源：http://vz.asd995.cn

Go:   arr = append(arr, 4)
来源：http://gl.gzmigu.cn

Ruby: arr << 4; arr.push(5)
来源：http://qi.shxzukj.cn

C#:   list.Add(4);
来源：http://rd.nszjky.cn

[D03] 在指定位置插入元素
来源：http://ur.jianghongdianzi.cn

Py:   arr.insert(0, 0)
来源：http://yt.nicolike.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://os.bookmarksfly.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://il.chemitech.net.cn

TS:   arr.splice(0, 0, 0);
来源：http://sf.nicolike.cn

Java: list.add(0, 0);
来源：http://lx.panjiajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tz.shxzukj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://xq.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://ox.huixiangedu.cn

[D04] 删除元素
来源：http://zx.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xa.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ke.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rb.hahajie.cn

TS:   arr.splice(0, 1);
来源：http://fy.yuexingan06.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kp.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ca.chemitech.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://zg.panjiajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mv.yuexingan06.cn

[D05] 访问与修改元素
来源：http://qm.szsharing.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vn.nicolike.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cu.huanxung.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ny.haigaiapp.cn

TS:   arr[0]; arr.at(-1);
来源：http://ll.colortex.cn

Java: list.get(0); list.set(0, 9);
来源：http://ye.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://fc.hahajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qy.huixiangedu.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nr.newstarts.cn

[D06] 数组长度
来源：http://tf.bjjhwx.cn

Py:   len(arr)
来源：http://rh.huixiangedu.cn

PHP:  count($arr);
来源：http://nc.shxzukj.cn

JS:   arr.length
来源：http://cc.newstarts.cn

TS:   arr.length
来源：http://oh.wgjwhj.cn

Java: list.size();
来源：http://cu.521024.cn

Go:   len(arr)
来源：http://lu.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://fb.muxihuayi.cn

C#:   list.Count;
来源：http://bz.huanxung.cn

[D07] 切片 / 取子数组
来源：http://ju.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nh.lnxyls.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qa.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://kj.hahajie.cn

TS:   arr.slice(1, 4);
来源：http://sy.newstarts.cn

Java: list.subList(1, 4);
来源：http://cg.521024.cn

Go:   arr[1:4]
来源：http://nd.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://oe.szxytkj.cn

C#:   list.GetRange(1, 3);
来源：http://xe.newstarts.cn

[D08] 合并两个数组
来源：http://fc.lnxyls.cn

Py:   a + b;  a.extend(b)
来源：http://rg.521024.cn

PHP:  array_merge($a, $b);
来源：http://re.9csxet.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://zf.gzmigu.cn

TS:   [...a, ...b];
来源：http://ty.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mk.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://cb.bookmarksfly.cn

Ruby: a + b;  a.concat(b)
来源：http://hf.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://yh.wgjwhj.cn

[D09] 排序（升序）
来源：http://qn.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://or.hnjuh.cn

PHP:  sort($arr);
来源：http://sf.lnxyls.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zg.szsharing.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ct.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bj.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ks.nicolike.cn

Ruby: arr.sort
来源：http://ur.gzmigu.cn

C#:   list.Sort();
来源：http://zu.521024.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://vr.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fm.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://lh.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rc.chemitech.net.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oo.muxihuayi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jg.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lw.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://li.9csxet.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dd.wgjwhj.cn

[D11] 反转数组
来源：http://yj.chemitech.net.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ql.521024.cn

PHP:  array_reverse($arr);
来源：http://pt.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zr.521024.cn

TS:   [...arr].reverse();
来源：http://zl.panjiajie.cn

Java: Collections.reverse(list);
来源：http://ca.asd995.cn

Go:   slices.Reverse(arr)
来源：http://bq.yuntaijiaju.cn

Ruby: arr.reverse
来源：http://al.lnxyls.cn

C#:   list.Reverse();
来源：http://fz.yuntaijiaju.cn

[D12] 查找元素下标
来源：http://rp.huixiangedu.cn

Py:   arr.index(x);  x in arr
来源：http://mt.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ki.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cz.wgjwhj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ef.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mc.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://dj.nicolike.cn

Ruby: arr.index(x)
来源：http://md.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://qn.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://zy.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ru.muxihuayi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://yy.asd995.cn

JS:   arr.filter(x => x > 3)
来源：http://lw.huixinmuqiang.cn

TS:   arr.filter(x => x > 3)
来源：http://dt.colortex.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xg.huixinmuqiang.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://of.wgjwhj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wz.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nf.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://od.newstarts.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://st.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://by.521024.cn

JS:   arr.map(x => x * 2)
来源：http://jz.shxzskj.cn

TS:   arr.map(x => x * 2)
来源：http://qc.wgjwhj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://iw.asd995.cn

Go:   // 手写循环
来源：http://lh.jianghongdianzi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fa.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://at.newstarts.cn

[D15] 去重
来源：http://vr.szxytkj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cl.szsharing.cn

PHP:  array_unique($arr);
来源：http://bh.gzmigu.cn

JS:   [...new Set(arr)]
来源：http://bj.shtwfgs.cn

TS:   [...new Set(arr)]
来源：http://ps.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://lw.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://qb.bookmarksfly.cn

Ruby: arr.uniq
来源：http://mm.yuexingan06.cn

C#:   list.Distinct().ToList()
来源：http://ba.gzmigu.cn

[D16] 求和与平均值
来源：http://rf.gzmigu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ew.hnjuh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yh.shxzskj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://id.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ap.huanxung.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ue.shxzukj.cn

Go:   // 手写循环累加
来源：http://zd.yuexingan06.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://pt.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://ip.bjjhwx.cn

[D17] 最大值与最小值
来源：http://zd.shtwfgs.cn

Py:   max(arr);  min(arr)
来源：http://yp.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://rl.gzmigu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iw.panjiajie.cn

TS:   Math.max(...arr);
来源：http://az.yuexingan06.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ud.yuntaijiaju.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mq.hahajie.cn

Ruby: arr.max;  arr.min
来源：http://pr.huixiangedu.cn

C#:   list.Max();  list.Min()
来源：http://hn.huixiangedu.cn

[D18] 扁平化嵌套数组
来源：http://ty.huixinmuqiang.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yg.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://rc.huixinmuqiang.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pw.panjiajie.cn

TS:   nested.flat();
来源：http://fe.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://aq.lnxyls.cn

Go:   // 手写双层循环
来源：http://ay.hnjuh.cn

Ruby: nested.flatten
来源：http://vj.szxytkj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://bj.huanxung.cn

[D19] 按字段分组
来源：http://ty.haigaiapp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ea.nszjky.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://oq.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://eu.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xb.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://oi.nicolike.cn

Go:   // 手写 map[string][]T
来源：http://np.haigaiapp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ni.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nw.huanxung.cn

[D20] 统计每个元素出现次数
来源：http://wa.gzmigu.cn

Py:   Counter(arr)
来源：http://aj.huixiangedu.cn

PHP:  array_count_values($arr);
来源：http://dd.shxzskj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sf.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uf.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vu.szsharing.cn

Go:   // 手写 map[T]int
来源：http://hk.chemitech.net.cn

Ruby: arr.tally
来源：http://jj.gzmigu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kc.huixinmuqiang.cn

[D21] 判断是否包含某元素
来源：http://hf.nicolike.cn

Py:   x in arr
来源：http://kq.asd995.cn


<!-- 参考信息 -->