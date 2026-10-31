代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://io.nszjky.cn

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://us.jctech888.com.cn

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://bw.newstarts.cn

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://at.lnxyls.cn

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://lj.panjiajie.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://sp.panjiajie.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://in.jianghongdianzi.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://xl.szsharing.cn

[C10] 变量作用域
来源：http://ip.newstarts.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ai.gzmigu.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://fo.lnxyls.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://bc.nicolike.cn

TS:   同 JS
来源：http://cz.hahajie.cn

Java: 方法内为块级作用域
来源：http://nn.yuexingan06.cn

Go:   花括号块级作用域
来源：http://tt.nszjky.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://fv.panjiajie.cn

C#:   块级作用域
来源：http://ve.lnxyls.cn

[C11] 模块导入与导出
来源：http://op.yuntaijiaju.cn

Py:   from module import func
来源：http://of.521024.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ko.huixinmuqiang.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ra.lnxyls.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://au.chemitech.net.cn

Java: import java.util.List;
来源：http://ph.muxihuayi.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://kl.bjjhwx.cn

Ruby: require "json"; require_relative "./util"
来源：http://oj.shxzukj.cn

C#:   using System.Text;
来源：http://dd.colortex.cn

[C12] 立即执行函数 IIFE
来源：http://qe.9csxet.cn

Py:   (lambda: print("run"))()
来源：http://iz.muxihuayi.cn

PHP:  (function () { echo "run"; })();
来源：http://ie.shxzskj.cn

JS:   (() => { console.log("run"); })();
来源：http://lc.yuntaijiaju.cn

TS:   (() => { console.log("run"); })();
来源：http://vd.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://il.szxytkj.cn

Go:   func() { fmt.Println("run") }()
来源：http://ol.asd995.cn

Ruby: -> { puts "run" }.call
来源：http://tp.panjiajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://xe.9csxet.cn

[C13] 类型声明 / 类型注解
来源：http://zc.haigaiapp.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://zn.yuexingan06.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://yr.wgjwhj.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://tu.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pd.szxytkj.cn

Java: int add(int a, int b) { return a + b; }
来源：http://vh.nszjky.cn

Go:   func add(a, b int) int
来源：http://dc.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ik.shxzukj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://eq.lnxyls.cn

[C14] 泛型函数
来源：http://cr.jctech888.com.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ih.newstarts.cn

PHP:  // 无泛型
来源：http://wh.nicolike.cn

JS:   // 无泛型
来源：http://ma.huixiangedu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://qi.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ok.521024.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mo.9csxet.cn

Ruby: # 无泛型
来源：http://xj.chemitech.net.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vu.shxzskj.cn

[C15] 解构 / 展开参数
来源：http://cg.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://kz.shxzukj.cn

PHP:  [$a, $b] = $pair;
来源：http://kl.jianghongdianzi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ks.nszjky.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jb.wgjwhj.cn

Java: // 无解构
来源：http://wj.bjjhwx.cn

Go:   // 无解构
来源：http://fp.shxzskj.cn

Ruby: a, b = pair
来源：http://ab.huanxung.cn

C#:   var (a, b) = pair;
来源：http://am.9csxet.cn

[C16] 函数 / 方法重载
来源：http://td.lnxyls.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ix.muxihuayi.cn

PHP:  // 无重载
来源：http://zg.muxihuayi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://lz.9csxet.cn

TS:   // 用联合类型或重载签名声明
来源：http://si.szxytkj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dl.gzmigu.cn

Go:   // 无重载：用不同函数名
来源：http://xb.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://ou.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://us.shxzskj.cn

================================================================================
来源：http://jb.yuexingan06.cn

D. 数组 / 列表 / 集合
来源：http://ck.shxzukj.cn

================================================================================
来源：http://ud.muxihuayi.cn

[D01] 创建数组 / 列表
来源：http://xo.huixiangedu.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ql.asd995.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vc.nszjky.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ze.chemitech.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://qk.gzmigu.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://nf.9csxet.cn

Go:   arr := []int{1, 2, 3}
来源：http://li.bookmarksfly.cn

Ruby: arr = [1, 2, 3]
来源：http://js.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://tt.wgjwhj.cn

[D02] 追加元素到末尾
来源：http://gh.muxihuayi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://no.521024.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://xz.wgjwhj.cn

JS:   arr.push(4);
来源：http://bn.huixiangedu.cn

TS:   arr.push(4);
来源：http://jb.521024.cn

Java: list.add(4);
来源：http://bi.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://wo.nicolike.cn

Ruby: arr << 4; arr.push(5)
来源：http://wb.lnxyls.cn

C#:   list.Add(4);
来源：http://vd.yuexingan06.cn

[D03] 在指定位置插入元素
来源：http://ga.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://ch.nicolike.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tt.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sn.haigaiapp.cn

TS:   arr.splice(0, 0, 0);
来源：http://id.panjiajie.cn

Java: list.add(0, 0);
来源：http://jv.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qi.521024.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://bc.asd995.cn

C#:   list.Insert(0, 0);
来源：http://pl.gzmigu.cn

[D04] 删除元素
来源：http://rq.panjiajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tq.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://qm.huixiangedu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://aa.lnxyls.cn

TS:   arr.splice(0, 1);
来源：http://eg.szxytkj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://il.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gs.jianghongdianzi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dq.huixinmuqiang.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://lh.newstarts.cn

[D05] 访问与修改元素
来源：http://ql.colortex.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://xe.colortex.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sw.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qa.bjjhwx.cn

TS:   arr[0]; arr.at(-1);
来源：http://ce.shtwfgs.cn

Java: list.get(0); list.set(0, 9);
来源：http://ob.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ef.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kp.huanxung.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hl.yuntaijiaju.cn

[D06] 数组长度
来源：http://ag.lnxyls.cn

Py:   len(arr)
来源：http://rx.muxihuayi.cn

PHP:  count($arr);
来源：http://jo.newstarts.cn

JS:   arr.length
来源：http://qo.shtwfgs.cn

TS:   arr.length
来源：http://et.szsharing.cn

Java: list.size();
来源：http://qs.lnxyls.cn

Go:   len(arr)
来源：http://zy.panjiajie.cn

Ruby: arr.length; arr.size
来源：http://qe.huixinmuqiang.cn

C#:   list.Count;
来源：http://cd.szsharing.cn

[D07] 切片 / 取子数组
来源：http://id.gzmigu.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ew.wgjwhj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ot.bookmarksfly.cn

JS:   arr.slice(1, 4);
来源：http://wg.hnjuh.cn

TS:   arr.slice(1, 4);
来源：http://my.jianghongdianzi.cn

Java: list.subList(1, 4);
来源：http://ic.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://oq.lnxyls.cn

Ruby: arr[1, 3]
来源：http://an.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://eo.bjjhwx.cn

[D08] 合并两个数组
来源：http://hc.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://yq.panjiajie.cn

PHP:  array_merge($a, $b);
来源：http://sf.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fz.bjjhwx.cn

TS:   [...a, ...b];
来源：http://bl.szxytkj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jb.9csxet.cn

Go:   append(a, b...)
来源：http://hz.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://pt.521024.cn

C#:   a.Concat(b).ToList()
来源：http://nm.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://ql.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://rz.9csxet.cn

PHP:  sort($arr);
来源：http://sg.huixinmuqiang.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hq.wgjwhj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://rw.panjiajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uy.shxzukj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://oy.hnjuh.cn

Ruby: arr.sort
来源：http://ua.wgjwhj.cn

C#:   list.Sort();
来源：http://mk.shtwfgs.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fw.jianghongdianzi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ic.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ti.jctech888.com.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hw.shtwfgs.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mm.9csxet.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hm.szxytkj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uc.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hu.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://th.nicolike.cn

[D11] 反转数组
来源：http://zg.asd995.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nv.521024.cn

PHP:  array_reverse($arr);
来源：http://vm.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.gzmigu.cn

TS:   [...arr].reverse();
来源：http://rp.colortex.cn

Java: Collections.reverse(list);
来源：http://dx.huixinmuqiang.cn

Go:   slices.Reverse(arr)
来源：http://hi.chemitech.net.cn

Ruby: arr.reverse
来源：http://gt.muxihuayi.cn

C#:   list.Reverse();
来源：http://iu.hahajie.cn

[D12] 查找元素下标
来源：http://jd.newstarts.cn

Py:   arr.index(x);  x in arr
来源：http://ts.asd995.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fy.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ed.newstarts.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nx.521024.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://fr.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://nz.nszjky.cn

Ruby: arr.index(x)
来源：http://uq.521024.cn

C#:   list.IndexOf(x);
来源：http://rz.szxytkj.cn

[D13] 过滤（保留满足条件的）
来源：http://qe.lnxyls.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pd.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tl.huixiangedu.cn

JS:   arr.filter(x => x > 3)
来源：http://zc.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://pm.jianghongdianzi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tx.9csxet.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oy.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vq.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yo.huixinmuqiang.cn

[D14] 映射转换（每个元素变形）
来源：http://gf.jctech888.com.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nv.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pm.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://la.panjiajie.cn

TS:   arr.map(x => x * 2)
来源：http://kk.huixinmuqiang.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yr.hahajie.cn

Go:   // 手写循环
来源：http://tw.haigaiapp.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cu.hahajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dc.shxzskj.cn

[D15] 去重
来源：http://ho.huanxung.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fz.szsharing.cn

PHP:  array_unique($arr);
来源：http://zt.yuexingan06.cn

JS:   [...new Set(arr)]
来源：http://to.bookmarksfly.cn

TS:   [...new Set(arr)]
来源：http://mg.chemitech.net.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://im.muxihuayi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://vp.yuexingan06.cn

Ruby: arr.uniq
来源：http://qx.gzmigu.cn

C#:   list.Distinct().ToList()
来源：http://gk.yuntaijiaju.cn

[D16] 求和与平均值
来源：http://qn.bjjhwx.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dk.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://kc.wgjwhj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ku.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lz.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ph.lnxyls.cn

Go:   // 手写循环累加
来源：http://ze.huanxung.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nw.muxihuayi.cn

C#:   list.Sum();  list.Average()
来源：http://eb.colortex.cn

[D17] 最大值与最小值
来源：http://tn.shtwfgs.cn

Py:   max(arr);  min(arr)
来源：http://zz.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://cu.chemitech.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://qa.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://xi.bjjhwx.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gn.hahajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bm.asd995.cn

Ruby: arr.max;  arr.min
来源：http://ka.szxytkj.cn

C#:   list.Max();  list.Min()
来源：http://os.huanxung.cn

[D18] 扁平化嵌套数组
来源：http://ft.szxytkj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gn.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://sm.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cp.yuntaijiaju.cn

TS:   nested.flat();
来源：http://pg.szxytkj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://id.colortex.cn

Go:   // 手写双层循环
来源：http://sm.panjiajie.cn

Ruby: nested.flatten
来源：http://by.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zq.huixiangedu.cn

[D19] 按字段分组
来源：http://jf.521024.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ng.lnxyls.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ra.muxihuayi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://tg.gzmigu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ds.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pc.521024.cn

Go:   // 手写 map[string][]T
来源：http://rh.szsharing.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://br.hahajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oh.huixinmuqiang.cn

[D20] 统计每个元素出现次数
来源：http://is.bookmarksfly.cn

Py:   Counter(arr)
来源：http://wr.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://lj.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yr.huixinmuqiang.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wm.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ku.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://ob.chemitech.net.cn

Ruby: arr.tally
来源：http://qk.wgjwhj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fa.521024.cn

[D21] 判断是否包含某元素
来源：http://zl.521024.cn

Py:   x in arr
来源：http://cl.asd995.cn

PHP:  in_array($x, $arr, true);
来源：http://sr.szxytkj.cn

JS:   arr.includes(x)
来源：http://hc.yuntaijiaju.cn

TS:   arr.includes(x)
来源：http://hl.huixinmuqiang.cn

Java: list.contains(x)
来源：http://ge.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://bm.nszjky.cn

Ruby: arr.include?(x)
来源：http://bh.yuexingan06.cn

C#:   list.Contains(x)
来源：http://cs.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://kf.yuexingan06.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wd.szxytkj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ia.shtwfgs.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hh.521024.cn

TS:   [...arr];
来源：http://yh.newstarts.cn

Java: new ArrayList<>(list);
来源：http://xk.hnjuh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ca.shxzukj.cn

Ruby: arr.dup;  arr.clone
来源：http://eq.jctech888.com.cn

C#:   new List<int>(list);
来源：http://sl.huixiangedu.cn

[D23] reduce 累积计算
来源：http://vj.shxzskj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gs.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pf.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qk.nicolike.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fk.nicolike.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rt.asd995.cn

Go:   // 手写循环
来源：http://vu.521024.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yd.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ve.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://mr.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ro.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hx.huixiangedu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qg.asd995.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cx.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://en.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dq.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gv.bookmarksfly.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mr.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://hq.bjjhwx.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dd.wgjwhj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wb.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bt.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xz.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hv.asd995.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cz.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uh.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ii.muxihuayi.cn

[D26] 数组转字符串
来源：http://wl.wgjwhj.cn


<!-- 参考信息 -->