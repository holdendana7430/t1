代发 wailian999

Py:   return a, b
来源：http://is.521024.cn

PHP:  return [$a, $b];
来源：http://cm.shxzskj.cn

JS:   return [a, b];             // 或 return { a, b };
来源：http://fn.hahajie.cn

TS:   return { a, b };
来源：http://ao.jianghongdianzi.cn

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://xu.jctech888.com.cn

Go:   return a, b
来源：http://kh.yuexingan06.cn

Ruby: return a, b
来源：http://ae.haigaiapp.cn

C#:   return (a, b);              // ValueTuple
来源：http://gk.hnjuh.cn

[C06] 匿名函数 / lambda
来源：http://qj.yuntaijiaju.cn

Py:   square = lambda x: x * x
来源：http://wk.nicolike.cn

PHP:  $square = fn($x) => $x * $x;
来源：http://sl.hnjuh.cn

JS:   const square = x => x * x;
来源：http://rz.asd995.cn

TS:   const square = (x: number): number => x * x;
来源：http://gn.haigaiapp.cn

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hh.9csxet.cn

Go:   sq := func(x int) int { return x * x }
来源：http://qc.jctech888.com.cn

Ruby: square = ->(x) { x * x }
来源：http://vx.gzmigu.cn

C#:   Func<int, int> square = x => x * x;
来源：http://gt.9csxet.cn

[C07] 把函数作为参数传入
来源：http://ni.shxzukj.cn

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://sp.521024.cn

PHP:  array_map("strtoupper", $arr);
来源：http://pa.jianghongdianzi.cn

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://zd.bjjhwx.cn

TS:   arr.map(String)
来源：http://lv.hnjuh.cn

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://ik.bookmarksfly.cn

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://ae.gzmigu.cn

Ruby: arr.map(&:upcase)
来源：http://zh.panjiajie.cn

C#:   arr.Select(s => s.ToUpper())
来源：http://mw.bookmarksfly.cn

[C08] 闭包
来源：http://bt.haigaiapp.cn

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://li.wgjwhj.cn

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://vt.chemitech.net.cn

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://if.nszjky.cn

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://co.szxytkj.cn

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://tj.shtwfgs.cn

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mf.bjjhwx.cn

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://be.nszjky.cn

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://sx.gzmigu.cn

[C09] 递归
来源：http://qt.9csxet.cn

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://ee.panjiajie.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://bm.shtwfgs.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://jl.hnjuh.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hd.huixinmuqiang.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://rq.hnjuh.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://qj.yuntaijiaju.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://oy.nicolike.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://op.jianghongdianzi.cn

[C10] 变量作用域
来源：http://il.shtwfgs.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://xj.muxihuayi.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://lp.huixiangedu.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://tl.colortex.cn

TS:   同 JS
来源：http://ea.hahajie.cn

Java: 方法内为块级作用域
来源：http://az.bjjhwx.cn

Go:   花括号块级作用域
来源：http://bu.huixinmuqiang.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://io.shxzskj.cn

C#:   块级作用域
来源：http://wc.lnxyls.cn

[C11] 模块导入与导出
来源：http://to.jianghongdianzi.cn

Py:   from module import func
来源：http://nw.panjiajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zm.lnxyls.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://lz.bjjhwx.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://vm.hahajie.cn

Java: import java.util.List;
来源：http://cw.huanxung.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://qh.colortex.cn

Ruby: require "json"; require_relative "./util"
来源：http://ww.hahajie.cn

C#:   using System.Text;
来源：http://tr.yuexingan06.cn

[C12] 立即执行函数 IIFE
来源：http://xa.huanxung.cn

Py:   (lambda: print("run"))()
来源：http://wz.panjiajie.cn

PHP:  (function () { echo "run"; })();
来源：http://jq.asd995.cn

JS:   (() => { console.log("run"); })();
来源：http://sd.panjiajie.cn

TS:   (() => { console.log("run"); })();
来源：http://tu.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ph.gzmigu.cn

Go:   func() { fmt.Println("run") }()
来源：http://hr.shxzskj.cn

Ruby: -> { puts "run" }.call
来源：http://cz.huixiangedu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://uv.huixinmuqiang.cn

[C13] 类型声明 / 类型注解
来源：http://bw.shtwfgs.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://uh.bjjhwx.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hr.szxytkj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://lg.bookmarksfly.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://xh.yuntaijiaju.cn

Java: int add(int a, int b) { return a + b; }
来源：http://le.huixiangedu.cn

Go:   func add(a, b int) int
来源：http://bm.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://va.wgjwhj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lx.shxzskj.cn

[C14] 泛型函数
来源：http://jg.szsharing.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vo.huixinmuqiang.cn

PHP:  // 无泛型
来源：http://vm.wgjwhj.cn

JS:   // 无泛型
来源：http://fx.huanxung.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://rj.panjiajie.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hp.shtwfgs.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://lw.nszjky.cn

Ruby: # 无泛型
来源：http://gs.wgjwhj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mk.bookmarksfly.cn

[C15] 解构 / 展开参数
来源：http://bj.nszjky.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://lo.chemitech.net.cn

PHP:  [$a, $b] = $pair;
来源：http://am.jctech888.com.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ox.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wt.szxytkj.cn

Java: // 无解构
来源：http://hg.asd995.cn

Go:   // 无解构
来源：http://di.huanxung.cn

Ruby: a, b = pair
来源：http://go.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://zw.wgjwhj.cn

[C16] 函数 / 方法重载
来源：http://pt.lnxyls.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://jt.shtwfgs.cn

PHP:  // 无重载
来源：http://am.9csxet.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://aq.wgjwhj.cn

TS:   // 用联合类型或重载签名声明
来源：http://ni.gzmigu.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tn.wgjwhj.cn

Go:   // 无重载：用不同函数名
来源：http://lc.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://uc.jctech888.com.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://oh.shxzskj.cn

================================================================================
来源：http://lo.huixinmuqiang.cn

D. 数组 / 列表 / 集合
来源：http://vd.haigaiapp.cn

================================================================================
来源：http://ff.newstarts.cn

[D01] 创建数组 / 列表
来源：http://xy.huixinmuqiang.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ug.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mo.szsharing.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://dz.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://oa.huixiangedu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://vc.szxytkj.cn

Go:   arr := []int{1, 2, 3}
来源：http://su.wgjwhj.cn

Ruby: arr = [1, 2, 3]
来源：http://jk.bookmarksfly.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://bf.hnjuh.cn

[D02] 追加元素到末尾
来源：http://zn.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://dx.bookmarksfly.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://nn.panjiajie.cn

JS:   arr.push(4);
来源：http://et.gzmigu.cn

TS:   arr.push(4);
来源：http://fo.521024.cn

Java: list.add(4);
来源：http://vj.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://zj.bjjhwx.cn

Ruby: arr << 4; arr.push(5)
来源：http://ju.bookmarksfly.cn

C#:   list.Add(4);
来源：http://ao.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://sz.yuexingan06.cn

Py:   arr.insert(0, 0)
来源：http://xp.shxzskj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oi.gzmigu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://va.haigaiapp.cn

TS:   arr.splice(0, 0, 0);
来源：http://ea.panjiajie.cn

Java: list.add(0, 0);
来源：http://kd.lnxyls.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wi.lnxyls.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wd.nicolike.cn

C#:   list.Insert(0, 0);
来源：http://jy.lnxyls.cn

[D04] 删除元素
来源：http://yk.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yi.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fl.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ef.wgjwhj.cn

TS:   arr.splice(0, 1);
来源：http://vg.huixinmuqiang.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://rr.wgjwhj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hw.szsharing.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://uf.huixinmuqiang.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nr.nicolike.cn

[D05] 访问与修改元素
来源：http://xk.shxzskj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yl.gzmigu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://it.huixiangedu.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gt.newstarts.cn

TS:   arr[0]; arr.at(-1);
来源：http://di.chemitech.net.cn

Java: list.get(0); list.set(0, 9);
来源：http://hh.szxytkj.cn

Go:   arr[0]; arr[0] = 9
来源：http://cw.hnjuh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nb.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dd.asd995.cn

[D06] 数组长度
来源：http://qo.shxzukj.cn

Py:   len(arr)
来源：http://iy.gzmigu.cn

PHP:  count($arr);
来源：http://hz.szxytkj.cn

JS:   arr.length
来源：http://hd.szsharing.cn

TS:   arr.length
来源：http://uz.muxihuayi.cn

Java: list.size();
来源：http://xg.panjiajie.cn

Go:   len(arr)
来源：http://er.nszjky.cn

Ruby: arr.length; arr.size
来源：http://dr.asd995.cn

C#:   list.Count;
来源：http://mw.yuexingan06.cn

[D07] 切片 / 取子数组
来源：http://ys.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ux.shxzskj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sx.jctech888.com.cn

JS:   arr.slice(1, 4);
来源：http://mr.hnjuh.cn

TS:   arr.slice(1, 4);
来源：http://yb.szsharing.cn

Java: list.subList(1, 4);
来源：http://xp.lnxyls.cn

Go:   arr[1:4]
来源：http://ow.yuexingan06.cn

Ruby: arr[1, 3]
来源：http://sc.haigaiapp.cn

C#:   list.GetRange(1, 3);
来源：http://or.szxytkj.cn

[D08] 合并两个数组
来源：http://hl.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://qn.wgjwhj.cn

PHP:  array_merge($a, $b);
来源：http://qd.hnjuh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wo.huanxung.cn

TS:   [...a, ...b];
来源：http://ja.szsharing.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://kf.nszjky.cn

Go:   append(a, b...)
来源：http://pa.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://vt.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://jh.bjjhwx.cn

[D09] 排序（升序）
来源：http://wp.gzmigu.cn

Py:   sorted(arr);  arr.sort()
来源：http://uq.nszjky.cn

PHP:  sort($arr);
来源：http://tr.colortex.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xs.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://xa.wgjwhj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pk.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rc.shxzukj.cn

Ruby: arr.sort
来源：http://xs.bjjhwx.cn

C#:   list.Sort();
来源：http://me.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://iu.colortex.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ok.521024.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ox.haigaiapp.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wt.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ya.yuntaijiaju.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jd.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://eh.asd995.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://xv.panjiajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bi.shtwfgs.cn

[D11] 反转数组
来源：http://je.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pc.hahajie.cn

PHP:  array_reverse($arr);
来源：http://lq.gzmigu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ge.521024.cn

TS:   [...arr].reverse();
来源：http://pf.jianghongdianzi.cn

Java: Collections.reverse(list);
来源：http://fy.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://ag.bookmarksfly.cn

Ruby: arr.reverse
来源：http://hv.haigaiapp.cn

C#:   list.Reverse();
来源：http://ca.colortex.cn

[D12] 查找元素下标
来源：http://jt.szsharing.cn

Py:   arr.index(x);  x in arr
来源：http://hl.bjjhwx.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://jb.521024.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dc.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ci.huanxung.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://jn.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://mi.bjjhwx.cn

Ruby: arr.index(x)
来源：http://sr.newstarts.cn

C#:   list.IndexOf(x);
来源：http://qg.asd995.cn

[D13] 过滤（保留满足条件的）
来源：http://vt.nicolike.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://et.szxytkj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ag.huanxung.cn

JS:   arr.filter(x => x > 3)
来源：http://yp.wgjwhj.cn

TS:   arr.filter(x => x > 3)
来源：http://cj.521024.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://be.szxytkj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wq.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hf.hnjuh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hu.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://ab.muxihuayi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ix.asd995.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ud.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://rv.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://gr.colortex.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rp.muxihuayi.cn

Go:   // 手写循环
来源：http://zj.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://un.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://id.hnjuh.cn

[D15] 去重
来源：http://lp.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://qr.panjiajie.cn

PHP:  array_unique($arr);
来源：http://si.bjjhwx.cn

JS:   [...new Set(arr)]
来源：http://zc.panjiajie.cn

TS:   [...new Set(arr)]
来源：http://ck.bookmarksfly.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hp.huixinmuqiang.cn

Go:   // 用 map[T]struct{} 手写
来源：http://kz.hnjuh.cn

Ruby: arr.uniq
来源：http://kb.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://ll.shxzukj.cn

[D16] 求和与平均值
来源：http://zq.asd995.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yn.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fu.521024.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dm.hahajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jx.jctech888.com.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://er.jianghongdianzi.cn

Go:   // 手写循环累加
来源：http://lj.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://if.szxytkj.cn

C#:   list.Sum();  list.Average()
来源：http://al.yuntaijiaju.cn

[D17] 最大值与最小值
来源：http://vx.shtwfgs.cn

Py:   max(arr);  min(arr)
来源：http://dt.huixiangedu.cn

PHP:  max($arr);  min($arr);
来源：http://qf.asd995.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jy.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://hi.nszjky.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bc.lnxyls.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bl.panjiajie.cn

Ruby: arr.max;  arr.min
来源：http://dt.jctech888.com.cn

C#:   list.Max();  list.Min()
来源：http://bz.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://xc.jianghongdianzi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oz.huanxung.cn

PHP:  array_merge(...$nested);
来源：http://vv.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mg.shxzukj.cn

TS:   nested.flat();
来源：http://yr.shxzukj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ly.colortex.cn

Go:   // 手写双层循环
来源：http://nd.nicolike.cn

Ruby: nested.flatten
来源：http://dm.hnjuh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tn.nszjky.cn

[D19] 按字段分组
来源：http://wi.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ll.nszjky.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cj.asd995.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://es.szxytkj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gm.huixinmuqiang.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ke.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://ff.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://kp.bookmarksfly.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://bu.bjjhwx.cn

[D20] 统计每个元素出现次数
来源：http://cw.yuexingan06.cn

Py:   Counter(arr)
来源：http://ye.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://vh.bjjhwx.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dk.haigaiapp.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ou.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gm.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://ld.shxzukj.cn

Ruby: arr.tally
来源：http://mg.hnjuh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gf.nicolike.cn

[D21] 判断是否包含某元素
来源：http://te.haigaiapp.cn

Py:   x in arr
来源：http://kl.521024.cn

PHP:  in_array($x, $arr, true);
来源：http://tg.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://ju.yuexingan06.cn

TS:   arr.includes(x)
来源：http://ek.huixinmuqiang.cn

Java: list.contains(x)
来源：http://ic.nszjky.cn

Go:   slices.Contains(arr, x)
来源：http://jk.colortex.cn

Ruby: arr.include?(x)
来源：http://dj.huixinmuqiang.cn

C#:   list.Contains(x)
来源：http://ce.shxzskj.cn

[D22] 复制数组（避免共享引用）
来源：http://ml.huanxung.cn


<!-- 参考信息 -->