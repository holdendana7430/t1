代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://la.haigaiapp.cn

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://pq.lnxyls.cn

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://ya.asd995.cn

Java: // 无：用 Builder 模式或 record
来源：http://qe.hahajie.cn

Go:   // 无：用配置结构体参数
来源：http://xr.huixiangedu.cn

Ruby: f(a: 1, b: 2)
来源：http://yg.nszjky.cn

C#:   f(a: 1, b: 2)
来源：http://cy.bookmarksfly.cn

[C05] 返回多个值
来源：http://tj.jctech888.com.cn

Py:   return a, b
来源：http://zu.muxihuayi.cn

PHP:  return [$a, $b];
来源：http://nk.521024.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://mu.huixinmuqiang.cn

TS:   return { a, b };
来源：http://lz.muxihuayi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://ym.yuexingan06.cn

Go:   return a, b
来源：http://ef.hnjuh.cn

Ruby: return a, b
来源：http://dd.newstarts.cn

C#:   return (a, b);              // ValueTuple
来源：http://lm.bjjhwx.cn

[C06] 匿名函数 / lambda
来源：http://sp.521024.cn

Py:   square = lambda x: x * x
来源：http://oq.wgjwhj.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://wa.huixinmuqiang.cn

JS:   const square = x => x * x;
来源：http://iv.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://wj.chemitech.net.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://um.muxihuayi.cn

Go:   sq := func(x int) int { return x * x }
来源：http://xy.bookmarksfly.cn

Ruby: square = ->(x) { x * x }
来源：http://bw.wgjwhj.cn

C#:   Func<int, int> square = x => x * x;
来源：http://mh.hnjuh.cn

[C07] 把函数作为参数传入
来源：http://dn.lnxyls.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://im.yuntaijiaju.cn

PHP:  array_map("strtoupper", $arr);
来源：http://uq.huixinmuqiang.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://uf.newstarts.cn

TS:   arr.map(String)
来源：http://bm.lnxyls.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://vm.yuexingan06.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ns.shxzskj.cn

Ruby: arr.map(&:upcase)
来源：http://gm.szxytkj.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://tv.lnxyls.cn

[C08] 闭包
来源：http://fe.szsharing.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://qv.gzmigu.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://yi.nszjky.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://vx.shtwfgs.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://vm.haigaiapp.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://fl.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://jz.shtwfgs.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://to.jctech888.com.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://ot.shtwfgs.cn

[C09] 递归
来源：http://ro.chemitech.net.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://cq.chemitech.net.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://oq.huixinmuqiang.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://of.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://nh.muxihuayi.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hd.szsharing.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://fz.huixinmuqiang.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://cb.szxytkj.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://kk.yuexingan06.cn

[C10] 变量作用域
来源：http://jq.9csxet.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://zh.haigaiapp.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wq.asd995.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mu.jianghongdianzi.cn

TS:   同 JS
来源：http://sr.asd995.cn

Java: 方法内为块级作用域
来源：http://ld.jctech888.com.cn

Go:   花括号块级作用域
来源：http://tr.chemitech.net.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://sk.asd995.cn

C#:   块级作用域
来源：http://kc.shtwfgs.cn

[C11] 模块导入与导出
来源：http://ih.lnxyls.cn

Py:   from module import func
来源：http://ll.jianghongdianzi.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://rj.9csxet.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qi.hnjuh.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://ws.shxzskj.cn

Java: import java.util.List;
来源：http://hq.nszjky.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mp.panjiajie.cn

Ruby: require "json"; require_relative "./util"
来源：http://sk.szxytkj.cn

C#:   using System.Text;
来源：http://be.shtwfgs.cn

[C12] 立即执行函数 IIFE
来源：http://mf.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://jd.huixinmuqiang.cn

PHP:  (function () { echo "run"; })();
来源：http://lw.panjiajie.cn

JS:   (() => { console.log("run"); })();
来源：http://pa.521024.cn

TS:   (() => { console.log("run"); })();
来源：http://cl.haigaiapp.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://rz.chemitech.net.cn

Go:   func() { fmt.Println("run") }()
来源：http://tr.yuntaijiaju.cn

Ruby: -> { puts "run" }.call
来源：http://zw.bookmarksfly.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://gq.lnxyls.cn

[C13] 类型声明 / 类型注解
来源：http://ua.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zk.wgjwhj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vl.521024.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ba.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xd.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://ud.huixiangedu.cn

Go:   func add(a, b int) int
来源：http://as.panjiajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vy.chemitech.net.cn

C#:   int Add(int a, int b) => a + b;
来源：http://fm.nszjky.cn

[C14] 泛型函数
来源：http://tn.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://qz.wgjwhj.cn

PHP:  // 无泛型
来源：http://jt.hahajie.cn

JS:   // 无泛型
来源：http://zk.yuntaijiaju.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uv.521024.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://sz.szsharing.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://rf.jctech888.com.cn

Ruby: # 无泛型
来源：http://ym.yuntaijiaju.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wu.chemitech.net.cn

[C15] 解构 / 展开参数
来源：http://ya.shtwfgs.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hq.shxzskj.cn

PHP:  [$a, $b] = $pair;
来源：http://dk.hnjuh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://le.asd995.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bp.yuntaijiaju.cn

Java: // 无解构
来源：http://ir.jctech888.com.cn

Go:   // 无解构
来源：http://qj.colortex.cn

Ruby: a, b = pair
来源：http://fy.wgjwhj.cn

C#:   var (a, b) = pair;
来源：http://xz.wgjwhj.cn

[C16] 函数 / 方法重载
来源：http://kb.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mb.huanxung.cn

PHP:  // 无重载
来源：http://sx.panjiajie.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qa.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://fk.yuntaijiaju.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://cp.bookmarksfly.cn

Go:   // 无重载：用不同函数名
来源：http://jg.gzmigu.cn

Ruby: # 无重载：靠动态参数
来源：http://ww.panjiajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://ua.nszjky.cn

================================================================================
来源：http://iu.521024.cn

D. 数组 / 列表 / 集合
来源：http://zw.gzmigu.cn

================================================================================
来源：http://nw.bookmarksfly.cn

[D01] 创建数组 / 列表
来源：http://nm.nszjky.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xo.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tk.nicolike.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://pb.bjjhwx.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yf.asd995.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ps.huixinmuqiang.cn

Go:   arr := []int{1, 2, 3}
来源：http://bu.521024.cn

Ruby: arr = [1, 2, 3]
来源：http://mb.gzmigu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://al.newstarts.cn

[D02] 追加元素到末尾
来源：http://kv.panjiajie.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yd.shxzukj.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ie.yuntaijiaju.cn

JS:   arr.push(4);
来源：http://wj.shtwfgs.cn

TS:   arr.push(4);
来源：http://fv.haigaiapp.cn

Java: list.add(4);
来源：http://nr.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://od.huanxung.cn

Ruby: arr << 4; arr.push(5)
来源：http://dr.hahajie.cn

C#:   list.Add(4);
来源：http://hn.hnjuh.cn

[D03] 在指定位置插入元素
来源：http://wt.shtwfgs.cn

Py:   arr.insert(0, 0)
来源：http://mb.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vf.gzmigu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ft.bjjhwx.cn

TS:   arr.splice(0, 0, 0);
来源：http://yd.yuexingan06.cn

Java: list.add(0, 0);
来源：http://ss.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://it.muxihuayi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ti.huixiangedu.cn

C#:   list.Insert(0, 0);
来源：http://da.gzmigu.cn

[D04] 删除元素
来源：http://py.521024.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ic.szsharing.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fz.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://la.shtwfgs.cn

TS:   arr.splice(0, 1);
来源：http://tj.gzmigu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eb.huixinmuqiang.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://uz.jianghongdianzi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gs.szxytkj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ro.chemitech.net.cn

[D05] 访问与修改元素
来源：http://pb.wgjwhj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fj.nicolike.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ui.asd995.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://dm.521024.cn

TS:   arr[0]; arr.at(-1);
来源：http://pu.gzmigu.cn

Java: list.get(0); list.set(0, 9);
来源：http://ka.colortex.cn

Go:   arr[0]; arr[0] = 9
来源：http://rh.hnjuh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jt.huanxung.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hs.huixiangedu.cn

[D06] 数组长度
来源：http://ra.bookmarksfly.cn

Py:   len(arr)
来源：http://bb.huixiangedu.cn

PHP:  count($arr);
来源：http://gh.9csxet.cn

JS:   arr.length
来源：http://dn.colortex.cn

TS:   arr.length
来源：http://nu.jianghongdianzi.cn

Java: list.size();
来源：http://wa.bookmarksfly.cn

Go:   len(arr)
来源：http://dm.szsharing.cn

Ruby: arr.length; arr.size
来源：http://ba.shxzukj.cn

C#:   list.Count;
来源：http://xv.yuntaijiaju.cn

[D07] 切片 / 取子数组
来源：http://oc.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mu.jctech888.com.cn

PHP:  array_slice($arr, 1, 3);
来源：http://zd.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://no.hahajie.cn

TS:   arr.slice(1, 4);
来源：http://ld.szsharing.cn

Java: list.subList(1, 4);
来源：http://tj.bjjhwx.cn

Go:   arr[1:4]
来源：http://tk.huanxung.cn

Ruby: arr[1, 3]
来源：http://hw.521024.cn

C#:   list.GetRange(1, 3);
来源：http://da.colortex.cn

[D08] 合并两个数组
来源：http://yy.szxytkj.cn

Py:   a + b;  a.extend(b)
来源：http://qo.jctech888.com.cn

PHP:  array_merge($a, $b);
来源：http://bj.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://vg.colortex.cn

TS:   [...a, ...b];
来源：http://ik.hahajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cs.chemitech.net.cn

Go:   append(a, b...)
来源：http://jv.asd995.cn

Ruby: a + b;  a.concat(b)
来源：http://fo.bookmarksfly.cn

C#:   a.Concat(b).ToList()
来源：http://oc.newstarts.cn

[D09] 排序（升序）
来源：http://vm.szsharing.cn

Py:   sorted(arr);  arr.sort()
来源：http://kr.huanxung.cn

PHP:  sort($arr);
来源：http://ru.huanxung.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hj.521024.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ce.9csxet.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xa.bookmarksfly.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rk.panjiajie.cn

Ruby: arr.sort
来源：http://lk.newstarts.cn

C#:   list.Sort();
来源：http://hz.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://uo.shtwfgs.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://cc.521024.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nr.shxzskj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://em.huixinmuqiang.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fy.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fb.szxytkj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ha.9csxet.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xr.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yi.hnjuh.cn

[D11] 反转数组
来源：http://sk.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gd.shtwfgs.cn

PHP:  array_reverse($arr);
来源：http://es.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://tn.huixiangedu.cn

TS:   [...arr].reverse();
来源：http://wr.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://it.shtwfgs.cn

Go:   slices.Reverse(arr)
来源：http://oi.bookmarksfly.cn

Ruby: arr.reverse
来源：http://hl.yuexingan06.cn

C#:   list.Reverse();
来源：http://an.yuntaijiaju.cn

[D12] 查找元素下标
来源：http://se.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://lv.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://nm.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ki.nszjky.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wj.yuexingan06.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zu.huixinmuqiang.cn

Go:   slices.Index(arr, x)
来源：http://rg.szxytkj.cn

Ruby: arr.index(x)
来源：http://su.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://yy.hnjuh.cn

[D13] 过滤（保留满足条件的）
来源：http://il.jctech888.com.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://so.nszjky.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://vy.huanxung.cn

JS:   arr.filter(x => x > 3)
来源：http://lx.newstarts.cn

TS:   arr.filter(x => x > 3)
来源：http://ni.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://qj.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qb.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xd.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://qu.huanxung.cn

[D14] 映射转换（每个元素变形）
来源：http://py.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://uf.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://yl.521024.cn

JS:   arr.map(x => x * 2)
来源：http://hh.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://mi.jctech888.com.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://gi.521024.cn

Go:   // 手写循环
来源：http://hm.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://to.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xy.haigaiapp.cn

[D15] 去重
来源：http://hv.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kp.szxytkj.cn

PHP:  array_unique($arr);
来源：http://qt.yuexingan06.cn

JS:   [...new Set(arr)]
来源：http://sp.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://mk.muxihuayi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ua.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ac.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://zs.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://zw.huixinmuqiang.cn

[D16] 求和与平均值
来源：http://wr.colortex.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yl.jianghongdianzi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rd.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ml.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zr.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://fb.asd995.cn

Go:   // 手写循环累加
来源：http://ho.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://br.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://qt.gzmigu.cn

[D17] 最大值与最小值
来源：http://za.huixinmuqiang.cn

Py:   max(arr);  min(arr)
来源：http://kd.muxihuayi.cn

PHP:  max($arr);  min($arr);
来源：http://ye.shxzskj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://or.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://hm.szsharing.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dh.bjjhwx.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gt.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://ey.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://om.gzmigu.cn

[D18] 扁平化嵌套数组
来源：http://vm.yuexingan06.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hf.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://qp.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ku.jianghongdianzi.cn

TS:   nested.flat();
来源：http://dp.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ww.521024.cn

Go:   // 手写双层循环
来源：http://hc.shxzskj.cn

Ruby: nested.flatten
来源：http://oh.chemitech.net.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xt.bjjhwx.cn

[D19] 按字段分组
来源：http://xv.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fa.haigaiapp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fm.lnxyls.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uh.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gi.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ez.colortex.cn

Go:   // 手写 map[string][]T
来源：http://zz.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hn.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ts.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://op.muxihuayi.cn

Py:   Counter(arr)
来源：http://ts.szsharing.cn

PHP:  array_count_values($arr);
来源：http://gf.huanxung.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ek.jctech888.com.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ao.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vq.hahajie.cn

Go:   // 手写 map[T]int
来源：http://gj.huixinmuqiang.cn

Ruby: arr.tally
来源：http://hb.wgjwhj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ip.wgjwhj.cn

[D21] 判断是否包含某元素
来源：http://uq.muxihuayi.cn

Py:   x in arr
来源：http://cq.jianghongdianzi.cn


<!-- 参考信息 -->