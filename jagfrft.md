代发 wailian999

PHP:  (function () { echo "run"; })();
来源：http://iz.szsharing.cn

JS:   (() => { console.log("run"); })();
来源：http://fk.wgjwhj.cn

TS:   (() => { console.log("run"); })();
来源：http://vp.huixinmuqiang.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://td.9csxet.cn

Go:   func() { fmt.Println("run") }()
来源：http://vj.muxihuayi.cn

Ruby: -> { puts "run" }.call
来源：http://ay.muxihuayi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ej.haigaiapp.cn

[C13] 类型声明 / 类型注解
来源：http://xl.jctech888.com.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bc.521024.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://vq.asd995.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://oh.yuexingan06.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fk.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://dj.huixiangedu.cn

Go:   func add(a, b int) int
来源：http://lf.hahajie.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://sf.nszjky.cn

C#:   int Add(int a, int b) => a + b;
来源：http://lq.521024.cn

[C14] 泛型函数
来源：http://yr.chemitech.net.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cb.szxytkj.cn

PHP:  // 无泛型
来源：http://zx.newstarts.cn

JS:   // 无泛型
来源：http://pk.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://ch.szxytkj.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ma.bookmarksfly.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hs.muxihuayi.cn

Ruby: # 无泛型
来源：http://cl.huixiangedu.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://yq.shxzskj.cn

[C15] 解构 / 展开参数
来源：http://tq.asd995.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://bz.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://in.bjjhwx.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://sp.jctech888.com.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mh.bjjhwx.cn

Java: // 无解构
来源：http://ub.muxihuayi.cn

Go:   // 无解构
来源：http://ar.szxytkj.cn

Ruby: a, b = pair
来源：http://fd.szxytkj.cn

C#:   var (a, b) = pair;
来源：http://aa.hahajie.cn

[C16] 函数 / 方法重载
来源：http://iv.9csxet.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://eu.521024.cn

PHP:  // 无重载
来源：http://au.huixinmuqiang.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zc.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://rw.shxzskj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://vj.9csxet.cn

Go:   // 无重载：用不同函数名
来源：http://ax.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://zq.shxzukj.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://id.shxzukj.cn

================================================================================
来源：http://jb.521024.cn

D. 数组 / 列表 / 集合
来源：http://ph.muxihuayi.cn

================================================================================
来源：http://db.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://rq.jianghongdianzi.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ac.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://oy.huixiangedu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://zr.nszjky.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tg.asd995.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ul.panjiajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://gn.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://bk.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yl.521024.cn

[D02] 追加元素到末尾
来源：http://ra.huanxung.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wg.haigaiapp.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zi.9csxet.cn

JS:   arr.push(4);
来源：http://cg.yuntaijiaju.cn

TS:   arr.push(4);
来源：http://mo.shxzskj.cn

Java: list.add(4);
来源：http://hm.huixinmuqiang.cn

Go:   arr = append(arr, 4)
来源：http://gf.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://jy.panjiajie.cn

C#:   list.Add(4);
来源：http://pd.shxzskj.cn

[D03] 在指定位置插入元素
来源：http://kl.jianghongdianzi.cn

Py:   arr.insert(0, 0)
来源：http://ll.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://bl.huixinmuqiang.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://pq.bjjhwx.cn

TS:   arr.splice(0, 0, 0);
来源：http://rx.nicolike.cn

Java: list.add(0, 0);
来源：http://eq.huanxung.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ro.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://uy.bookmarksfly.cn

C#:   list.Insert(0, 0);
来源：http://fn.shxzukj.cn

[D04] 删除元素
来源：http://ms.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://xm.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ol.bjjhwx.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://rb.newstarts.cn

TS:   arr.splice(0, 1);
来源：http://hu.521024.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pk.huixiangedu.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://xo.jianghongdianzi.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://pv.lnxyls.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://po.nszjky.cn

[D05] 访问与修改元素
来源：http://lz.huixinmuqiang.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fc.bjjhwx.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://yo.9csxet.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hf.shxzukj.cn

TS:   arr[0]; arr.at(-1);
来源：http://ki.huanxung.cn

Java: list.get(0); list.set(0, 9);
来源：http://zf.yuntaijiaju.cn

Go:   arr[0]; arr[0] = 9
来源：http://oi.yuexingan06.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rv.jctech888.com.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://on.panjiajie.cn

[D06] 数组长度
来源：http://fe.jianghongdianzi.cn

Py:   len(arr)
来源：http://yj.hnjuh.cn

PHP:  count($arr);
来源：http://mx.521024.cn

JS:   arr.length
来源：http://ae.hnjuh.cn

TS:   arr.length
来源：http://kx.nicolike.cn

Java: list.size();
来源：http://up.muxihuayi.cn

Go:   len(arr)
来源：http://fg.huanxung.cn

Ruby: arr.length; arr.size
来源：http://is.szsharing.cn

C#:   list.Count;
来源：http://il.521024.cn

[D07] 切片 / 取子数组
来源：http://mv.asd995.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ff.wgjwhj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mi.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://eb.huixinmuqiang.cn

TS:   arr.slice(1, 4);
来源：http://rf.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://qj.lnxyls.cn

Go:   arr[1:4]
来源：http://sl.szxytkj.cn

Ruby: arr[1, 3]
来源：http://nq.jianghongdianzi.cn

C#:   list.GetRange(1, 3);
来源：http://wh.hnjuh.cn

[D08] 合并两个数组
来源：http://at.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://rc.shxzukj.cn

PHP:  array_merge($a, $b);
来源：http://gp.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wp.jctech888.com.cn

TS:   [...a, ...b];
来源：http://ym.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://cr.colortex.cn

Go:   append(a, b...)
来源：http://se.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://ud.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://zt.muxihuayi.cn

[D09] 排序（升序）
来源：http://lh.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://so.newstarts.cn

PHP:  sort($arr);
来源：http://js.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://my.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://vp.haigaiapp.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yx.szsharing.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ha.bjjhwx.cn

Ruby: arr.sort
来源：http://io.lnxyls.cn

C#:   list.Sort();
来源：http://yd.haigaiapp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://nl.9csxet.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://bz.hahajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ty.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kr.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ft.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://da.nicolike.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dt.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ls.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fc.shxzukj.cn

[D11] 反转数组
来源：http://cr.asd995.cn

Py:   arr[::-1];  arr.reverse()
来源：http://iq.colortex.cn

PHP:  array_reverse($arr);
来源：http://eo.colortex.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ku.szsharing.cn

TS:   [...arr].reverse();
来源：http://pr.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://xq.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://fw.szxytkj.cn

Ruby: arr.reverse
来源：http://tt.shtwfgs.cn

C#:   list.Reverse();
来源：http://uj.newstarts.cn

[D12] 查找元素下标
来源：http://hh.shxzukj.cn

Py:   arr.index(x);  x in arr
来源：http://yl.bjjhwx.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zn.chemitech.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://db.bookmarksfly.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ey.gzmigu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mp.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://gn.bookmarksfly.cn

Ruby: arr.index(x)
来源：http://zh.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://iv.chemitech.net.cn

[D13] 过滤（保留满足条件的）
来源：http://zc.wgjwhj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fh.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://az.colortex.cn

JS:   arr.filter(x => x > 3)
来源：http://rt.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://dy.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rm.panjiajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://sx.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://am.hahajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ot.9csxet.cn

[D14] 映射转换（每个元素变形）
来源：http://rh.chemitech.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xc.muxihuayi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qt.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://as.9csxet.cn

TS:   arr.map(x => x * 2)
来源：http://mm.chemitech.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sn.bjjhwx.cn

Go:   // 手写循环
来源：http://sn.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cv.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://be.shxzukj.cn

[D15] 去重
来源：http://iv.yuntaijiaju.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oq.lnxyls.cn

PHP:  array_unique($arr);
来源：http://ns.9csxet.cn

JS:   [...new Set(arr)]
来源：http://we.szsharing.cn

TS:   [...new Set(arr)]
来源：http://ul.panjiajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ef.hahajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://av.shxzskj.cn

Ruby: arr.uniq
来源：http://wx.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://pi.bjjhwx.cn

[D16] 求和与平均值
来源：http://fm.shxzskj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uo.shxzukj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://un.lnxyls.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://on.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://lh.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://to.muxihuayi.cn

Go:   // 手写循环累加
来源：http://bq.bjjhwx.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jm.huanxung.cn

C#:   list.Sum();  list.Average()
来源：http://pd.chemitech.net.cn

[D17] 最大值与最小值
来源：http://ew.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://dw.nszjky.cn

PHP:  max($arr);  min($arr);
来源：http://aa.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ec.nszjky.cn

TS:   Math.max(...arr);
来源：http://vs.lnxyls.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ql.yuexingan06.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zv.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://dw.nszjky.cn

C#:   list.Max();  list.Min()
来源：http://uf.szsharing.cn

[D18] 扁平化嵌套数组
来源：http://an.nszjky.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://td.yuexingan06.cn

PHP:  array_merge(...$nested);
来源：http://pk.muxihuayi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nn.huixiangedu.cn

TS:   nested.flat();
来源：http://xu.muxihuayi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ab.bookmarksfly.cn

Go:   // 手写双层循环
来源：http://nw.hnjuh.cn

Ruby: nested.flatten
来源：http://al.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ke.hahajie.cn

[D19] 按字段分组
来源：http://on.9csxet.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ks.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ww.yuexingan06.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mo.bjjhwx.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://de.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kx.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://rr.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ys.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fd.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://eq.lnxyls.cn

Py:   Counter(arr)
来源：http://ig.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://cw.bookmarksfly.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tt.szxytkj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yy.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://in.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://zr.hahajie.cn

Ruby: arr.tally
来源：http://cn.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eo.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://wr.chemitech.net.cn

Py:   x in arr
来源：http://jt.asd995.cn

PHP:  in_array($x, $arr, true);
来源：http://gx.shtwfgs.cn

JS:   arr.includes(x)
来源：http://sf.haigaiapp.cn

TS:   arr.includes(x)
来源：http://jh.huanxung.cn

Java: list.contains(x)
来源：http://xw.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://xa.bookmarksfly.cn

Ruby: arr.include?(x)
来源：http://dg.shtwfgs.cn

C#:   list.Contains(x)
来源：http://xf.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://ip.521024.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://on.yuexingan06.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vt.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lz.bjjhwx.cn

TS:   [...arr];
来源：http://ey.colortex.cn

Java: new ArrayList<>(list);
来源：http://kn.panjiajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xf.jctech888.com.cn

Ruby: arr.dup;  arr.clone
来源：http://tq.asd995.cn

C#:   new List<int>(list);
来源：http://pn.lnxyls.cn

[D23] reduce 累积计算
来源：http://ug.szsharing.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hg.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qo.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wn.newstarts.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hb.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://qm.bookmarksfly.cn

Go:   // 手写循环
来源：http://jr.jctech888.com.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://dt.yuexingan06.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kt.nszjky.cn

[D24] 字典 / Map 基本操作
来源：http://zr.huixinmuqiang.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://fw.jctech888.com.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hf.shtwfgs.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ok.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ip.szsharing.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ak.szsharing.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pk.panjiajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hb.nicolike.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ba.newstarts.cn

[D25] Set 集合去重与交并差
来源：http://ju.jianghongdianzi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ib.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cv.yuntaijiaju.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qt.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ue.9csxet.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://tr.nicolike.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rs.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sc.huixiangedu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hw.huanxung.cn

[D26] 数组转字符串
来源：http://ao.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://ln.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://lq.szsharing.cn

JS:   arr.join(", ")
来源：http://iz.huanxung.cn

TS:   arr.join(", ")
来源：http://gm.szsharing.cn

Java: String.join(", ", list)
来源：http://nj.szxytkj.cn

Go:   strings.Join(strs, ", ")
来源：http://zn.panjiajie.cn

Ruby: arr.join(", ")
来源：http://is.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://po.jctech888.com.cn

================================================================================
来源：http://hl.jianghongdianzi.cn

E. 字符串处理
来源：http://pb.chemitech.net.cn

================================================================================
来源：http://tp.yuexingan06.cn

[E01] 拼接字符串
来源：http://yf.jctech888.com.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rv.asd995.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oa.asd995.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://om.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nz.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zl.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bw.bjjhwx.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zc.shtwfgs.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://nu.asd995.cn

[E02] 重复字符串
来源：http://qv.521024.cn

Py:   "ab" * 3
来源：http://bn.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://gw.yuexingan06.cn

JS:   "ab".repeat(3)
来源：http://ca.panjiajie.cn

TS:   "ab".repeat(3)
来源：http://zl.shxzukj.cn

Java: "ab".repeat(3)
来源：http://jt.nicolike.cn

Go:   strings.Repeat("ab", 3)
来源：http://lz.hahajie.cn

Ruby: "ab" * 3
来源：http://pc.asd995.cn


<!-- 参考信息 -->