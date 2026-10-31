代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://od.szxytkj.cn

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://kr.asd995.cn

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://xp.gzmigu.cn

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://rb.newstarts.cn

[C10] 变量作用域
来源：http://ht.wgjwhj.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://ok.bookmarksfly.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://xu.shxzskj.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://ej.bjjhwx.cn

TS:   同 JS
来源：http://ke.yuexingan06.cn

Java: 方法内为块级作用域
来源：http://ol.haigaiapp.cn

Go:   花括号块级作用域
来源：http://nk.jianghongdianzi.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://kj.bjjhwx.cn

C#:   块级作用域
来源：http://tt.shxzskj.cn

[C11] 模块导入与导出
来源：http://rj.hahajie.cn

Py:   from module import func
来源：http://sq.nszjky.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://uw.yuntaijiaju.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://ni.shtwfgs.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://jd.521024.cn

Java: import java.util.List;
来源：http://td.shxzukj.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://eu.gzmigu.cn

Ruby: require "json"; require_relative "./util"
来源：http://cr.shtwfgs.cn

C#:   using System.Text;
来源：http://em.haigaiapp.cn

[C12] 立即执行函数 IIFE
来源：http://bv.521024.cn

Py:   (lambda: print("run"))()
来源：http://to.hnjuh.cn

PHP:  (function () { echo "run"; })();
来源：http://ks.nszjky.cn

JS:   (() => { console.log("run"); })();
来源：http://jv.asd995.cn

TS:   (() => { console.log("run"); })();
来源：http://im.muxihuayi.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://eo.panjiajie.cn

Go:   func() { fmt.Println("run") }()
来源：http://kc.521024.cn

Ruby: -> { puts "run" }.call
来源：http://ex.hnjuh.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://jq.szsharing.cn

[C13] 类型声明 / 类型注解
来源：http://kd.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://vg.shxzskj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pl.hnjuh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://zj.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ul.nicolike.cn

Java: int add(int a, int b) { return a + b; }
来源：http://wl.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://dq.521024.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://lf.huanxung.cn

C#:   int Add(int a, int b) => a + b;
来源：http://xa.wgjwhj.cn

[C14] 泛型函数
来源：http://my.wgjwhj.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://le.9csxet.cn

PHP:  // 无泛型
来源：http://vl.wgjwhj.cn

JS:   // 无泛型
来源：http://jw.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ik.huanxung.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mm.szxytkj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://nr.hnjuh.cn

Ruby: # 无泛型
来源：http://wt.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://pb.nszjky.cn

[C15] 解构 / 展开参数
来源：http://vu.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bl.newstarts.cn

PHP:  [$a, $b] = $pair;
来源：http://ur.haigaiapp.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://bg.newstarts.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://sl.shtwfgs.cn

Java: // 无解构
来源：http://ex.wgjwhj.cn

Go:   // 无解构
来源：http://hq.huixinmuqiang.cn

Ruby: a, b = pair
来源：http://lu.nicolike.cn

C#:   var (a, b) = pair;
来源：http://qj.jctech888.com.cn

[C16] 函数 / 方法重载
来源：http://ly.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wx.shxzskj.cn

PHP:  // 无重载
来源：http://aw.hnjuh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gr.colortex.cn

TS:   // 用联合类型或重载签名声明
来源：http://by.hnjuh.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://yb.521024.cn

Go:   // 无重载：用不同函数名
来源：http://if.bookmarksfly.cn

Ruby: # 无重载：靠动态参数
来源：http://do.huixinmuqiang.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tk.hahajie.cn

================================================================================
来源：http://lk.huixiangedu.cn

D. 数组 / 列表 / 集合
来源：http://jy.colortex.cn

================================================================================
来源：http://kh.colortex.cn

[D01] 创建数组 / 列表
来源：http://bo.wgjwhj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fd.muxihuayi.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pu.bjjhwx.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gl.huixinmuqiang.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://dd.yuntaijiaju.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://su.jianghongdianzi.cn

Go:   arr := []int{1, 2, 3}
来源：http://gh.shtwfgs.cn

Ruby: arr = [1, 2, 3]
来源：http://lu.jianghongdianzi.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://fe.jianghongdianzi.cn

[D02] 追加元素到末尾
来源：http://om.hnjuh.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://fx.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://qq.yuntaijiaju.cn

JS:   arr.push(4);
来源：http://qd.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://jw.jctech888.com.cn

Java: list.add(4);
来源：http://mw.shxzskj.cn

Go:   arr = append(arr, 4)
来源：http://uh.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://ft.hnjuh.cn

C#:   list.Add(4);
来源：http://td.colortex.cn

[D03] 在指定位置插入元素
来源：http://kp.colortex.cn

Py:   arr.insert(0, 0)
来源：http://rx.gzmigu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://gr.nszjky.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fb.521024.cn

TS:   arr.splice(0, 0, 0);
来源：http://vk.hahajie.cn

Java: list.add(0, 0);
来源：http://ti.chemitech.net.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wn.jianghongdianzi.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://nn.jianghongdianzi.cn

C#:   list.Insert(0, 0);
来源：http://wz.huixiangedu.cn

[D04] 删除元素
来源：http://xe.wgjwhj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://pm.muxihuayi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xw.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rv.huixinmuqiang.cn

TS:   arr.splice(0, 1);
来源：http://cd.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dn.newstarts.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://og.nicolike.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hv.haigaiapp.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://nj.newstarts.cn

[D05] 访问与修改元素
来源：http://sq.hnjuh.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://uy.szxytkj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://vu.hahajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fy.colortex.cn

TS:   arr[0]; arr.at(-1);
来源：http://zp.shxzskj.cn

Java: list.get(0); list.set(0, 9);
来源：http://aw.chemitech.net.cn

Go:   arr[0]; arr[0] = 9
来源：http://qp.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yg.nszjky.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://tj.shtwfgs.cn

[D06] 数组长度
来源：http://gf.lnxyls.cn

Py:   len(arr)
来源：http://hn.asd995.cn

PHP:  count($arr);
来源：http://mc.jianghongdianzi.cn

JS:   arr.length
来源：http://bz.521024.cn

TS:   arr.length
来源：http://wl.muxihuayi.cn

Java: list.size();
来源：http://fh.panjiajie.cn

Go:   len(arr)
来源：http://fu.bjjhwx.cn

Ruby: arr.length; arr.size
来源：http://oa.nicolike.cn

C#:   list.Count;
来源：http://jw.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://rm.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://qz.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://jv.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://on.haigaiapp.cn

TS:   arr.slice(1, 4);
来源：http://or.bookmarksfly.cn

Java: list.subList(1, 4);
来源：http://qn.newstarts.cn

Go:   arr[1:4]
来源：http://dm.yuntaijiaju.cn

Ruby: arr[1, 3]
来源：http://wn.wgjwhj.cn

C#:   list.GetRange(1, 3);
来源：http://ku.wgjwhj.cn

[D08] 合并两个数组
来源：http://oe.chemitech.net.cn

Py:   a + b;  a.extend(b)
来源：http://ni.chemitech.net.cn

PHP:  array_merge($a, $b);
来源：http://dy.shxzukj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gl.bjjhwx.cn

TS:   [...a, ...b];
来源：http://ji.9csxet.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wz.shxzskj.cn

Go:   append(a, b...)
来源：http://ty.jctech888.com.cn

Ruby: a + b;  a.concat(b)
来源：http://ts.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://qj.9csxet.cn

[D09] 排序（升序）
来源：http://fg.yuexingan06.cn

Py:   sorted(arr);  arr.sort()
来源：http://mg.hnjuh.cn

PHP:  sort($arr);
来源：http://qu.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hq.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wz.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ji.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://cz.shxzskj.cn

Ruby: arr.sort
来源：http://tx.yuexingan06.cn

C#:   list.Sort();
来源：http://nd.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yn.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fk.bjjhwx.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wf.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://lf.521024.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jw.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://cv.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gg.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://vo.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ho.9csxet.cn

[D11] 反转数组
来源：http://mj.nicolike.cn

Py:   arr[::-1];  arr.reverse()
来源：http://yw.521024.cn

PHP:  array_reverse($arr);
来源：http://lq.jctech888.com.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hr.huixinmuqiang.cn

TS:   [...arr].reverse();
来源：http://ph.521024.cn

Java: Collections.reverse(list);
来源：http://cg.yuntaijiaju.cn

Go:   slices.Reverse(arr)
来源：http://xc.nicolike.cn

Ruby: arr.reverse
来源：http://yy.szxytkj.cn

C#:   list.Reverse();
来源：http://hd.haigaiapp.cn

[D12] 查找元素下标
来源：http://uw.jctech888.com.cn

Py:   arr.index(x);  x in arr
来源：http://wu.szsharing.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://co.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vm.9csxet.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jq.szxytkj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gl.yuntaijiaju.cn

Go:   slices.Index(arr, x)
来源：http://hz.lnxyls.cn

Ruby: arr.index(x)
来源：http://gm.jctech888.com.cn

C#:   list.IndexOf(x);
来源：http://wz.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://dc.huanxung.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://np.shtwfgs.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tp.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://oz.huixiangedu.cn

TS:   arr.filter(x => x > 3)
来源：http://er.panjiajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ov.wgjwhj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xt.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xj.shxzskj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ai.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://yb.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bh.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cf.szsharing.cn

JS:   arr.map(x => x * 2)
来源：http://go.szxytkj.cn

TS:   arr.map(x => x * 2)
来源：http://ot.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://rc.nszjky.cn

Go:   // 手写循环
来源：http://bp.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wh.shtwfgs.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ow.huixiangedu.cn

[D15] 去重
来源：http://qs.wgjwhj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kf.nszjky.cn

PHP:  array_unique($arr);
来源：http://in.szxytkj.cn

JS:   [...new Set(arr)]
来源：http://fw.nicolike.cn

TS:   [...new Set(arr)]
来源：http://mt.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://zp.huixinmuqiang.cn

Go:   // 用 map[T]struct{} 手写
来源：http://du.szsharing.cn

Ruby: arr.uniq
来源：http://ko.jianghongdianzi.cn

C#:   list.Distinct().ToList()
来源：http://yy.jianghongdianzi.cn

[D16] 求和与平均值
来源：http://gy.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yz.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ip.huixiangedu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ne.hnjuh.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://th.huanxung.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://dt.gzmigu.cn

Go:   // 手写循环累加
来源：http://uk.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cc.yuexingan06.cn

C#:   list.Sum();  list.Average()
来源：http://eu.panjiajie.cn

[D17] 最大值与最小值
来源：http://ij.nicolike.cn

Py:   max(arr);  min(arr)
来源：http://kc.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://ef.bjjhwx.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://or.szxytkj.cn

TS:   Math.max(...arr);
来源：http://rm.wgjwhj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hg.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qv.521024.cn

Ruby: arr.max;  arr.min
来源：http://rq.bjjhwx.cn

C#:   list.Max();  list.Min()
来源：http://fs.newstarts.cn

[D18] 扁平化嵌套数组
来源：http://ox.szxytkj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ow.hnjuh.cn

PHP:  array_merge(...$nested);
来源：http://ye.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fn.yuntaijiaju.cn

TS:   nested.flat();
来源：http://wn.hahajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ko.9csxet.cn

Go:   // 手写双层循环
来源：http://gq.haigaiapp.cn

Ruby: nested.flatten
来源：http://bi.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://hr.jianghongdianzi.cn

[D19] 按字段分组
来源：http://xv.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zr.shxzukj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tk.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fb.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://qo.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wi.521024.cn

Go:   // 手写 map[string][]T
来源：http://wn.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yl.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jd.haigaiapp.cn

[D20] 统计每个元素出现次数
来源：http://xp.nicolike.cn

Py:   Counter(arr)
来源：http://he.szsharing.cn

PHP:  array_count_values($arr);
来源：http://ez.jctech888.com.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vc.hahajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ge.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hy.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://fe.panjiajie.cn

Ruby: arr.tally
来源：http://nn.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fe.yuexingan06.cn

[D21] 判断是否包含某元素
来源：http://ff.jianghongdianzi.cn

Py:   x in arr
来源：http://ld.szxytkj.cn

PHP:  in_array($x, $arr, true);
来源：http://bj.wgjwhj.cn

JS:   arr.includes(x)
来源：http://dv.panjiajie.cn

TS:   arr.includes(x)
来源：http://qz.newstarts.cn

Java: list.contains(x)
来源：http://cc.szsharing.cn

Go:   slices.Contains(arr, x)
来源：http://kb.szxytkj.cn

Ruby: arr.include?(x)
来源：http://ot.shxzukj.cn

C#:   list.Contains(x)
来源：http://gg.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://vh.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://kc.chemitech.net.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ke.bookmarksfly.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gu.bookmarksfly.cn

TS:   [...arr];
来源：http://hb.jctech888.com.cn

Java: new ArrayList<>(list);
来源：http://yh.huixinmuqiang.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cz.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://dm.colortex.cn

C#:   new List<int>(list);
来源：http://nk.nicolike.cn

[D23] reduce 累积计算
来源：http://cy.9csxet.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lc.szsharing.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ak.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://le.yuntaijiaju.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cc.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://bv.shxzskj.cn

Go:   // 手写循环
来源：http://rm.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://bf.yuntaijiaju.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tq.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://zn.nicolike.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://be.panjiajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://te.huanxung.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ei.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fa.shxzskj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xw.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hu.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ib.hahajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yz.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://fc.521024.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wb.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zg.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xr.wgjwhj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qf.shtwfgs.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wl.newstarts.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://zy.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tb.hahajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hv.szsharing.cn

[D26] 数组转字符串
来源：http://yv.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://ys.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://aw.lnxyls.cn

JS:   arr.join(", ")
来源：http://lv.haigaiapp.cn

TS:   arr.join(", ")
来源：http://kd.yuexingan06.cn


<!-- 参考信息 -->