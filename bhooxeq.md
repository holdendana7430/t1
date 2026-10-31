代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://qz.nszjky.cn

C#:   using System.Text;
来源：http://re.shxzukj.cn

[C12] 立即执行函数 IIFE
来源：http://tq.nszjky.cn

Py:   (lambda: print("run"))()
来源：http://fw.chemitech.net.cn

PHP:  (function () { echo "run"; })();
来源：http://bc.colortex.cn

JS:   (() => { console.log("run"); })();
来源：http://lp.muxihuayi.cn

TS:   (() => { console.log("run"); })();
来源：http://ob.szxytkj.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://de.lnxyls.cn

Go:   func() { fmt.Println("run") }()
来源：http://nn.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://mg.lnxyls.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ly.huanxung.cn

[C13] 类型声明 / 类型注解
来源：http://ux.lnxyls.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://tq.szxytkj.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://gq.bookmarksfly.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://jw.gzmigu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://en.521024.cn

Java: int add(int a, int b) { return a + b; }
来源：http://fn.yuexingan06.cn

Go:   func add(a, b int) int
来源：http://fl.shxzukj.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://xf.bjjhwx.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cl.bookmarksfly.cn

[C14] 泛型函数
来源：http://gs.lnxyls.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://up.yuexingan06.cn

PHP:  // 无泛型
来源：http://hb.jctech888.com.cn

JS:   // 无泛型
来源：http://pv.hahajie.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://dx.jctech888.com.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ro.szxytkj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://fu.muxihuayi.cn

Ruby: # 无泛型
来源：http://hg.wgjwhj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bj.colortex.cn

[C15] 解构 / 展开参数
来源：http://gq.jctech888.com.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://xb.szsharing.cn

PHP:  [$a, $b] = $pair;
来源：http://qy.szsharing.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://km.9csxet.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xt.colortex.cn

Java: // 无解构
来源：http://kl.shtwfgs.cn

Go:   // 无解构
来源：http://go.bjjhwx.cn

Ruby: a, b = pair
来源：http://sq.lnxyls.cn

C#:   var (a, b) = pair;
来源：http://vr.asd995.cn

[C16] 函数 / 方法重载
来源：http://nm.jianghongdianzi.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://je.newstarts.cn

PHP:  // 无重载
来源：http://gy.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://up.shxzskj.cn

TS:   // 用联合类型或重载签名声明
来源：http://et.asd995.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://do.nszjky.cn

Go:   // 无重载：用不同函数名
来源：http://bp.jctech888.com.cn

Ruby: # 无重载：靠动态参数
来源：http://ch.muxihuayi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://pb.yuntaijiaju.cn

================================================================================
来源：http://wc.huixinmuqiang.cn

D. 数组 / 列表 / 集合
来源：http://ge.newstarts.cn

================================================================================
来源：http://fz.bjjhwx.cn

[D01] 创建数组 / 列表
来源：http://ae.nicolike.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://bl.huixinmuqiang.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mc.shtwfgs.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ef.shxzukj.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://zd.shxzukj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://kj.shtwfgs.cn

Go:   arr := []int{1, 2, 3}
来源：http://mb.gzmigu.cn

Ruby: arr = [1, 2, 3]
来源：http://zw.nicolike.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mz.jianghongdianzi.cn

[D02] 追加元素到末尾
来源：http://yx.newstarts.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://kd.newstarts.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ui.huixiangedu.cn

JS:   arr.push(4);
来源：http://eq.asd995.cn

TS:   arr.push(4);
来源：http://dt.lnxyls.cn

Java: list.add(4);
来源：http://rn.bookmarksfly.cn

Go:   arr = append(arr, 4)
来源：http://fs.jctech888.com.cn

Ruby: arr << 4; arr.push(5)
来源：http://dl.huixiangedu.cn

C#:   list.Add(4);
来源：http://lt.bjjhwx.cn

[D03] 在指定位置插入元素
来源：http://qr.bookmarksfly.cn

Py:   arr.insert(0, 0)
来源：http://du.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fy.nicolike.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mq.bjjhwx.cn

TS:   arr.splice(0, 0, 0);
来源：http://no.bjjhwx.cn

Java: list.add(0, 0);
来源：http://yf.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ej.szxytkj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://gl.hahajie.cn

C#:   list.Insert(0, 0);
来源：http://xe.szsharing.cn

[D04] 删除元素
来源：http://ui.nicolike.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ht.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://vn.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cg.bookmarksfly.cn

TS:   arr.splice(0, 1);
来源：http://ej.panjiajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://md.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://is.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qu.huixinmuqiang.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ah.shtwfgs.cn

[D05] 访问与修改元素
来源：http://wm.lnxyls.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://kl.huixinmuqiang.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dk.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yc.wgjwhj.cn

TS:   arr[0]; arr.at(-1);
来源：http://pb.szsharing.cn

Java: list.get(0); list.set(0, 9);
来源：http://yt.asd995.cn

Go:   arr[0]; arr[0] = 9
来源：http://vr.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fh.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cw.panjiajie.cn

[D06] 数组长度
来源：http://zp.szsharing.cn

Py:   len(arr)
来源：http://ew.colortex.cn

PHP:  count($arr);
来源：http://cr.yuexingan06.cn

JS:   arr.length
来源：http://pr.huanxung.cn

TS:   arr.length
来源：http://ua.hnjuh.cn

Java: list.size();
来源：http://ty.huixiangedu.cn

Go:   len(arr)
来源：http://xv.wgjwhj.cn

Ruby: arr.length; arr.size
来源：http://gk.hnjuh.cn

C#:   list.Count;
来源：http://ro.gzmigu.cn

[D07] 切片 / 取子数组
来源：http://bo.haigaiapp.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nk.asd995.cn

PHP:  array_slice($arr, 1, 3);
来源：http://wt.gzmigu.cn

JS:   arr.slice(1, 4);
来源：http://tz.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://sf.colortex.cn

Java: list.subList(1, 4);
来源：http://qg.colortex.cn

Go:   arr[1:4]
来源：http://xq.colortex.cn

Ruby: arr[1, 3]
来源：http://oz.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://lx.colortex.cn

[D08] 合并两个数组
来源：http://sa.wgjwhj.cn

Py:   a + b;  a.extend(b)
来源：http://vh.jianghongdianzi.cn

PHP:  array_merge($a, $b);
来源：http://tq.huixiangedu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bj.haigaiapp.cn

TS:   [...a, ...b];
来源：http://dt.huixiangedu.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ak.szxytkj.cn

Go:   append(a, b...)
来源：http://yg.shxzskj.cn

Ruby: a + b;  a.concat(b)
来源：http://nr.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://st.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://xq.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://zq.huanxung.cn

PHP:  sort($arr);
来源：http://kl.yuexingan06.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ax.chemitech.net.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://dp.shxzukj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://wp.panjiajie.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://et.521024.cn

Ruby: arr.sort
来源：http://tp.szsharing.cn

C#:   list.Sort();
来源：http://ss.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://hy.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ei.nszjky.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ty.szsharing.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gv.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://pd.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ws.nszjky.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gz.nszjky.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://of.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mi.lnxyls.cn

[D11] 反转数组
来源：http://yn.nicolike.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ya.bjjhwx.cn

PHP:  array_reverse($arr);
来源：http://xn.nicolike.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zs.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://bo.shxzukj.cn

Java: Collections.reverse(list);
来源：http://pu.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://ye.panjiajie.cn

Ruby: arr.reverse
来源：http://cw.newstarts.cn

C#:   list.Reverse();
来源：http://fj.yuntaijiaju.cn

[D12] 查找元素下标
来源：http://sc.9csxet.cn

Py:   arr.index(x);  x in arr
来源：http://tu.chemitech.net.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zt.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://yu.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://jf.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vo.newstarts.cn

Go:   slices.Index(arr, x)
来源：http://xt.9csxet.cn

Ruby: arr.index(x)
来源：http://az.nszjky.cn

C#:   list.IndexOf(x);
来源：http://kx.newstarts.cn

[D13] 过滤（保留满足条件的）
来源：http://da.yuntaijiaju.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://re.shxzskj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gj.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://gx.lnxyls.cn

TS:   arr.filter(x => x > 3)
来源：http://ip.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lp.yuntaijiaju.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gs.nicolike.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qr.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yc.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://rr.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dr.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ci.nicolike.cn

JS:   arr.map(x => x * 2)
来源：http://jh.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://vr.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mb.asd995.cn

Go:   // 手写循环
来源：http://dw.shxzukj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://pi.huixiangedu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jf.huixinmuqiang.cn

[D15] 去重
来源：http://ax.newstarts.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mq.panjiajie.cn

PHP:  array_unique($arr);
来源：http://tv.hahajie.cn

JS:   [...new Set(arr)]
来源：http://xt.wgjwhj.cn

TS:   [...new Set(arr)]
来源：http://pk.szxytkj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://uu.huixiangedu.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uw.jctech888.com.cn

Ruby: arr.uniq
来源：http://yn.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://js.colortex.cn

[D16] 求和与平均值
来源：http://aq.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://oq.bookmarksfly.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aw.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iu.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ps.chemitech.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bs.newstarts.cn

Go:   // 手写循环累加
来源：http://yl.nicolike.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kj.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://oa.hahajie.cn

[D17] 最大值与最小值
来源：http://lc.huixinmuqiang.cn

Py:   max(arr);  min(arr)
来源：http://av.nszjky.cn

PHP:  max($arr);  min($arr);
来源：http://mv.szsharing.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://lv.gzmigu.cn

TS:   Math.max(...arr);
来源：http://uh.newstarts.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mm.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dn.asd995.cn

Ruby: arr.max;  arr.min
来源：http://tk.szxytkj.cn

C#:   list.Max();  list.Min()
来源：http://qh.521024.cn

[D18] 扁平化嵌套数组
来源：http://dq.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://bd.bjjhwx.cn

PHP:  array_merge(...$nested);
来源：http://vy.newstarts.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wi.chemitech.net.cn

TS:   nested.flat();
来源：http://yt.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ie.wgjwhj.cn

Go:   // 手写双层循环
来源：http://qv.nszjky.cn

Ruby: nested.flatten
来源：http://js.szsharing.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nm.huixiangedu.cn

[D19] 按字段分组
来源：http://sg.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fv.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ig.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cy.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yq.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tx.hahajie.cn

Go:   // 手写 map[string][]T
来源：http://po.jianghongdianzi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ra.gzmigu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pu.wgjwhj.cn

[D20] 统计每个元素出现次数
来源：http://pd.szsharing.cn

Py:   Counter(arr)
来源：http://mg.colortex.cn

PHP:  array_count_values($arr);
来源：http://su.gzmigu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wg.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://my.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ku.muxihuayi.cn

Go:   // 手写 map[T]int
来源：http://qo.huixiangedu.cn

Ruby: arr.tally
来源：http://uw.nicolike.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ft.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://os.asd995.cn

Py:   x in arr
来源：http://sv.szxytkj.cn

PHP:  in_array($x, $arr, true);
来源：http://ok.9csxet.cn

JS:   arr.includes(x)
来源：http://zs.gzmigu.cn

TS:   arr.includes(x)
来源：http://oq.lnxyls.cn

Java: list.contains(x)
来源：http://ym.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://je.bjjhwx.cn

Ruby: arr.include?(x)
来源：http://vh.huanxung.cn

C#:   list.Contains(x)
来源：http://hm.colortex.cn

[D22] 复制数组（避免共享引用）
来源：http://pp.asd995.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lh.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ip.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fk.jctech888.com.cn

TS:   [...arr];
来源：http://lv.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://um.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://il.shxzukj.cn

Ruby: arr.dup;  arr.clone
来源：http://ml.nicolike.cn

C#:   new List<int>(list);
来源：http://xi.bjjhwx.cn

[D23] reduce 累积计算
来源：http://ew.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://za.huixinmuqiang.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lf.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://by.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ei.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://rj.wgjwhj.cn

Go:   // 手写循环
来源：http://bi.szxytkj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nz.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vd.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://bp.shtwfgs.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pj.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://yy.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://dy.szxytkj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tr.hahajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fy.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tm.9csxet.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://px.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://dh.huixiangedu.cn

[D25] Set 集合去重与交并差
来源：http://yx.9csxet.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wp.hahajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nc.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vj.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uv.szsharing.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ms.bookmarksfly.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.newstarts.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dv.shxzukj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://li.shxzukj.cn

[D26] 数组转字符串
来源：http://um.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://xv.szxytkj.cn

PHP:  implode(", ", $arr);
来源：http://li.shxzukj.cn

JS:   arr.join(", ")
来源：http://ik.521024.cn

TS:   arr.join(", ")
来源：http://jk.panjiajie.cn

Java: String.join(", ", list)
来源：http://za.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://yw.huanxung.cn

Ruby: arr.join(", ")
来源：http://fe.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://rx.szsharing.cn

================================================================================
来源：http://xp.wgjwhj.cn

E. 字符串处理
来源：http://eo.newstarts.cn

================================================================================
来源：http://wa.nicolike.cn

[E01] 拼接字符串
来源：http://io.shxzskj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gl.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ec.muxihuayi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jt.shxzukj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bq.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://df.huixinmuqiang.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://iw.bjjhwx.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jx.yuexingan06.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pw.chemitech.net.cn

[E02] 重复字符串
来源：http://wj.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://vz.szxytkj.cn

PHP:  str_repeat("ab", 3);
来源：http://my.colortex.cn

JS:   "ab".repeat(3)
来源：http://lk.shtwfgs.cn


<!-- 参考信息 -->