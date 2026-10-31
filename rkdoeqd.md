代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://fu.yuexingan06.cn

Ruby: -> { puts "run" }.call
来源：http://hf.bjjhwx.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://cd.shxzskj.cn

[C13] 类型声明 / 类型注解
来源：http://je.bjjhwx.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://bo.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://pc.521024.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://ru.jctech888.com.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://pg.panjiajie.cn

Java: int add(int a, int b) { return a + b; }
来源：http://oi.huixinmuqiang.cn

Go:   func add(a, b int) int
来源：http://ua.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yb.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://cr.huanxung.cn

[C14] 泛型函数
来源：http://dy.huixinmuqiang.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://bh.hnjuh.cn

PHP:  // 无泛型
来源：http://gg.lnxyls.cn

JS:   // 无泛型
来源：http://tg.hnjuh.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://gx.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xc.colortex.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://yq.szsharing.cn

Ruby: # 无泛型
来源：http://db.wgjwhj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://we.hahajie.cn

[C15] 解构 / 展开参数
来源：http://bn.bookmarksfly.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://qp.wgjwhj.cn

PHP:  [$a, $b] = $pair;
来源：http://ms.wgjwhj.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://cn.bookmarksfly.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://xa.chemitech.net.cn

Java: // 无解构
来源：http://ml.hahajie.cn

Go:   // 无解构
来源：http://et.huixiangedu.cn

Ruby: a, b = pair
来源：http://yg.panjiajie.cn

C#:   var (a, b) = pair;
来源：http://xz.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://zu.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ko.nicolike.cn

PHP:  // 无重载
来源：http://mg.jctech888.com.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://os.bookmarksfly.cn

TS:   // 用联合类型或重载签名声明
来源：http://zh.huanxung.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wc.panjiajie.cn

Go:   // 无重载：用不同函数名
来源：http://tj.hahajie.cn

Ruby: # 无重载：靠动态参数
来源：http://in.bookmarksfly.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://za.haigaiapp.cn

================================================================================
来源：http://fy.bjjhwx.cn

D. 数组 / 列表 / 集合
来源：http://za.hahajie.cn

================================================================================
来源：http://cm.jianghongdianzi.cn

[D01] 创建数组 / 列表
来源：http://ey.szxytkj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://fs.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jy.huixinmuqiang.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://or.nicolike.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://yh.haigaiapp.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://px.shxzskj.cn

Go:   arr := []int{1, 2, 3}
来源：http://xl.shxzskj.cn

Ruby: arr = [1, 2, 3]
来源：http://dy.yuntaijiaju.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ze.yuexingan06.cn

[D02] 追加元素到末尾
来源：http://gw.jianghongdianzi.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ix.huixinmuqiang.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://um.bjjhwx.cn

JS:   arr.push(4);
来源：http://ea.huanxung.cn

TS:   arr.push(4);
来源：http://ii.jctech888.com.cn

Java: list.add(4);
来源：http://bv.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://hk.jianghongdianzi.cn

Ruby: arr << 4; arr.push(5)
来源：http://oz.gzmigu.cn

C#:   list.Add(4);
来源：http://pm.asd995.cn

[D03] 在指定位置插入元素
来源：http://tw.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://sm.jctech888.com.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://om.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://zp.jctech888.com.cn

TS:   arr.splice(0, 0, 0);
来源：http://wm.jianghongdianzi.cn

Java: list.add(0, 0);
来源：http://vd.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://qw.hahajie.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://et.newstarts.cn

C#:   list.Insert(0, 0);
来源：http://ak.shxzskj.cn

[D04] 删除元素
来源：http://pd.haigaiapp.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yt.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mu.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pj.wgjwhj.cn

TS:   arr.splice(0, 1);
来源：http://rs.chemitech.net.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fl.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.lnxyls.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://oj.asd995.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qm.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://if.shxzukj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://fo.haigaiapp.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uu.lnxyls.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ep.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://un.newstarts.cn

Java: list.get(0); list.set(0, 9);
来源：http://qn.9csxet.cn

Go:   arr[0]; arr[0] = 9
来源：http://po.jianghongdianzi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jo.huanxung.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hh.szsharing.cn

[D06] 数组长度
来源：http://zy.muxihuayi.cn

Py:   len(arr)
来源：http://it.huanxung.cn

PHP:  count($arr);
来源：http://is.9csxet.cn

JS:   arr.length
来源：http://qx.wgjwhj.cn

TS:   arr.length
来源：http://sz.huixiangedu.cn

Java: list.size();
来源：http://ol.shxzskj.cn

Go:   len(arr)
来源：http://io.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://xz.haigaiapp.cn

C#:   list.Count;
来源：http://cg.jctech888.com.cn

[D07] 切片 / 取子数组
来源：http://vn.colortex.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ou.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://sb.gzmigu.cn

JS:   arr.slice(1, 4);
来源：http://tg.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://wq.haigaiapp.cn

Java: list.subList(1, 4);
来源：http://hi.muxihuayi.cn

Go:   arr[1:4]
来源：http://oj.muxihuayi.cn

Ruby: arr[1, 3]
来源：http://ig.jianghongdianzi.cn

C#:   list.GetRange(1, 3);
来源：http://hc.huixiangedu.cn

[D08] 合并两个数组
来源：http://td.szxytkj.cn

Py:   a + b;  a.extend(b)
来源：http://ha.wgjwhj.cn

PHP:  array_merge($a, $b);
来源：http://xz.jctech888.com.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://qw.shtwfgs.cn

TS:   [...a, ...b];
来源：http://vu.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://sq.haigaiapp.cn

Go:   append(a, b...)
来源：http://jq.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://ga.huanxung.cn

C#:   a.Concat(b).ToList()
来源：http://vg.jianghongdianzi.cn

[D09] 排序（升序）
来源：http://jp.lnxyls.cn

Py:   sorted(arr);  arr.sort()
来源：http://hw.nicolike.cn

PHP:  sort($arr);
来源：http://yq.asd995.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bi.9csxet.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://aq.jctech888.com.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ug.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mf.gzmigu.cn

Ruby: arr.sort
来源：http://mo.chemitech.net.cn

C#:   list.Sort();
来源：http://qz.bookmarksfly.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://km.muxihuayi.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://vb.9csxet.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ej.huixinmuqiang.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zp.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://op.yuexingan06.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://nh.colortex.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://vr.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://px.nszjky.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rc.muxihuayi.cn

[D11] 反转数组
来源：http://iw.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ct.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://xs.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pn.jctech888.com.cn

TS:   [...arr].reverse();
来源：http://zr.shtwfgs.cn

Java: Collections.reverse(list);
来源：http://hn.haigaiapp.cn

Go:   slices.Reverse(arr)
来源：http://xb.yuntaijiaju.cn

Ruby: arr.reverse
来源：http://nz.wgjwhj.cn

C#:   list.Reverse();
来源：http://tc.szxytkj.cn

[D12] 查找元素下标
来源：http://qg.shxzskj.cn

Py:   arr.index(x);  x in arr
来源：http://ls.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://se.szxytkj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://eu.jctech888.com.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ba.gzmigu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://en.nicolike.cn

Go:   slices.Index(arr, x)
来源：http://jr.lnxyls.cn

Ruby: arr.index(x)
来源：http://ug.jianghongdianzi.cn

C#:   list.IndexOf(x);
来源：http://jf.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://qz.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://sq.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://aw.lnxyls.cn

JS:   arr.filter(x => x > 3)
来源：http://cb.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://pi.yuntaijiaju.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fs.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nr.haigaiapp.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hq.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lr.nicolike.cn

[D14] 映射转换（每个元素变形）
来源：http://fw.panjiajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://xt.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fv.nszjky.cn

JS:   arr.map(x => x * 2)
来源：http://fi.gzmigu.cn

TS:   arr.map(x => x * 2)
来源：http://fy.panjiajie.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://op.bookmarksfly.cn

Go:   // 手写循环
来源：http://sq.jianghongdianzi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://um.yuntaijiaju.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qk.szxytkj.cn

[D15] 去重
来源：http://al.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://eq.newstarts.cn

PHP:  array_unique($arr);
来源：http://vb.jctech888.com.cn

JS:   [...new Set(arr)]
来源：http://zg.hahajie.cn

TS:   [...new Set(arr)]
来源：http://go.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vc.panjiajie.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nq.bookmarksfly.cn

Ruby: arr.uniq
来源：http://km.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://tt.yuexingan06.cn

[D16] 求和与平均值
来源：http://yv.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://vj.asd995.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bv.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ji.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rc.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qi.bjjhwx.cn

Go:   // 手写循环累加
来源：http://wb.yuntaijiaju.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vc.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://th.asd995.cn

[D17] 最大值与最小值
来源：http://of.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://wl.szxytkj.cn

PHP:  max($arr);  min($arr);
来源：http://wo.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://od.521024.cn

TS:   Math.max(...arr);
来源：http://ik.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pf.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://go.chemitech.net.cn

Ruby: arr.max;  arr.min
来源：http://ll.colortex.cn

C#:   list.Max();  list.Min()
来源：http://ks.wgjwhj.cn

[D18] 扁平化嵌套数组
来源：http://gq.shxzskj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lb.chemitech.net.cn

PHP:  array_merge(...$nested);
来源：http://ql.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ra.lnxyls.cn

TS:   nested.flat();
来源：http://mt.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jb.hnjuh.cn

Go:   // 手写双层循环
来源：http://un.huixiangedu.cn

Ruby: nested.flatten
来源：http://cu.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yh.muxihuayi.cn

[D19] 按字段分组
来源：http://ta.huixinmuqiang.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qa.521024.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sq.huanxung.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qh.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ob.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ke.yuexingan06.cn

Go:   // 手写 map[string][]T
来源：http://wv.panjiajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jn.bookmarksfly.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gj.haigaiapp.cn

[D20] 统计每个元素出现次数
来源：http://qh.huixinmuqiang.cn

Py:   Counter(arr)
来源：http://bo.lnxyls.cn

PHP:  array_count_values($arr);
来源：http://my.chemitech.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bl.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bz.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ko.newstarts.cn

Go:   // 手写 map[T]int
来源：http://fl.huixiangedu.cn

Ruby: arr.tally
来源：http://hp.haigaiapp.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bx.huanxung.cn

[D21] 判断是否包含某元素
来源：http://tg.nicolike.cn

Py:   x in arr
来源：http://wv.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://xp.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://li.nszjky.cn

TS:   arr.includes(x)
来源：http://kz.wgjwhj.cn

Java: list.contains(x)
来源：http://cq.hnjuh.cn

Go:   slices.Contains(arr, x)
来源：http://ob.lnxyls.cn

Ruby: arr.include?(x)
来源：http://vl.jctech888.com.cn

C#:   list.Contains(x)
来源：http://mk.huixinmuqiang.cn

[D22] 复制数组（避免共享引用）
来源：http://yv.jianghongdianzi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tu.colortex.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ij.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zu.bookmarksfly.cn

TS:   [...arr];
来源：http://yh.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://zc.hnjuh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ys.szsharing.cn

Ruby: arr.dup;  arr.clone
来源：http://os.shxzskj.cn

C#:   new List<int>(list);
来源：http://gp.haigaiapp.cn

[D23] reduce 累积计算
来源：http://rz.shxzukj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ft.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://sd.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qc.bjjhwx.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://up.asd995.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://eh.shtwfgs.cn

Go:   // 手写循环
来源：http://ii.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://rq.jianghongdianzi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zp.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://em.bookmarksfly.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://og.nszjky.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xr.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xq.bjjhwx.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gt.nicolike.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ve.hahajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ci.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sx.yuexingan06.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://yi.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://wf.yuntaijiaju.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qb.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://iu.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yu.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ke.9csxet.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ah.asd995.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://as.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://aw.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://sh.haigaiapp.cn

[D26] 数组转字符串
来源：http://ex.bjjhwx.cn

Py:   ", ".join(map(str, arr))
来源：http://bc.huixinmuqiang.cn

PHP:  implode(", ", $arr);
来源：http://oq.szxytkj.cn

JS:   arr.join(", ")
来源：http://ba.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://hq.gzmigu.cn

Java: String.join(", ", list)
来源：http://gh.haigaiapp.cn

Go:   strings.Join(strs, ", ")
来源：http://wv.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://nm.yuexingan06.cn

C#:   string.Join(", ", list)
来源：http://pr.bjjhwx.cn

================================================================================
来源：http://ul.wgjwhj.cn

E. 字符串处理
来源：http://se.panjiajie.cn

================================================================================
来源：http://nx.muxihuayi.cn

[E01] 拼接字符串
来源：http://bz.9csxet.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://gr.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dx.hnjuh.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qc.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pn.hahajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cr.newstarts.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mc.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ik.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://vo.jctech888.com.cn

[E02] 重复字符串
来源：http://zw.9csxet.cn

Py:   "ab" * 3
来源：http://lq.huanxung.cn

PHP:  str_repeat("ab", 3);
来源：http://mn.yuntaijiaju.cn

JS:   "ab".repeat(3)
来源：http://dx.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://wg.chemitech.net.cn

Java: "ab".repeat(3)
来源：http://ds.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://lr.shxzskj.cn

Ruby: "ab" * 3
来源：http://tm.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ys.chemitech.net.cn

[E03] 截取子串
来源：http://qx.hahajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ms.panjiajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rw.jctech888.com.cn


<!-- 参考信息 -->