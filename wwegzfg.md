代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://he.bookmarksfly.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://xt.hnjuh.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://pa.jianghongdianzi.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fn.asd995.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lv.szsharing.cn

Go:   func add(a, b int) int
来源：http://nw.jctech888.com.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yl.yuntaijiaju.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ux.521024.cn

[C14] 泛型函数
来源：http://ad.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://tn.huanxung.cn

PHP:  // 无泛型
来源：http://ir.bookmarksfly.cn

JS:   // 无泛型
来源：http://xq.newstarts.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://zs.huixiangedu.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://xl.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hb.bookmarksfly.cn

Ruby: # 无泛型
来源：http://bh.shxzskj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://cs.muxihuayi.cn

[C15] 解构 / 展开参数
来源：http://hw.colortex.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://dn.shxzukj.cn

PHP:  [$a, $b] = $pair;
来源：http://np.newstarts.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ql.huanxung.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://uj.yuexingan06.cn

Java: // 无解构
来源：http://sz.bjjhwx.cn

Go:   // 无解构
来源：http://oo.shtwfgs.cn

Ruby: a, b = pair
来源：http://ju.panjiajie.cn

C#:   var (a, b) = pair;
来源：http://uy.nicolike.cn

[C16] 函数 / 方法重载
来源：http://lg.hahajie.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ii.521024.cn

PHP:  // 无重载
来源：http://vw.muxihuayi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xz.huanxung.cn

TS:   // 用联合类型或重载签名声明
来源：http://lj.wgjwhj.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://tr.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://kw.bookmarksfly.cn

Ruby: # 无重载：靠动态参数
来源：http://bm.huanxung.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dk.newstarts.cn

================================================================================
来源：http://jv.nszjky.cn

D. 数组 / 列表 / 集合
来源：http://vu.nszjky.cn

================================================================================
来源：http://dk.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://ni.hahajie.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://vr.9csxet.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://gm.colortex.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ss.yuntaijiaju.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jx.muxihuayi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jc.hahajie.cn

Go:   arr := []int{1, 2, 3}
来源：http://kl.9csxet.cn

Ruby: arr = [1, 2, 3]
来源：http://hl.szsharing.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://dq.muxihuayi.cn

[D02] 追加元素到末尾
来源：http://gz.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://te.jctech888.com.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mx.huixinmuqiang.cn

JS:   arr.push(4);
来源：http://ir.bookmarksfly.cn

TS:   arr.push(4);
来源：http://dn.bookmarksfly.cn

Java: list.add(4);
来源：http://yi.chemitech.net.cn

Go:   arr = append(arr, 4)
来源：http://sn.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://cu.colortex.cn

C#:   list.Add(4);
来源：http://qe.huanxung.cn

[D03] 在指定位置插入元素
来源：http://wa.huanxung.cn

Py:   arr.insert(0, 0)
来源：http://jo.asd995.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://no.panjiajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://fp.szxytkj.cn

TS:   arr.splice(0, 0, 0);
来源：http://sd.haigaiapp.cn

Java: list.add(0, 0);
来源：http://ld.hahajie.cn

Go:   arr = append([]int{0}, arr...)
来源：http://hj.bookmarksfly.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://kq.szxytkj.cn

C#:   list.Insert(0, 0);
来源：http://um.hahajie.cn

[D04] 删除元素
来源：http://mg.521024.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yh.jctech888.com.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wt.jctech888.com.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://at.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://qb.nicolike.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fd.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://gq.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://dm.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zt.asd995.cn

[D05] 访问与修改元素
来源：http://ao.panjiajie.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yy.asd995.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ku.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tq.gzmigu.cn

TS:   arr[0]; arr.at(-1);
来源：http://dx.shxzskj.cn

Java: list.get(0); list.set(0, 9);
来源：http://le.hnjuh.cn

Go:   arr[0]; arr[0] = 9
来源：http://bs.9csxet.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://no.shtwfgs.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://eb.wgjwhj.cn

[D06] 数组长度
来源：http://ja.9csxet.cn

Py:   len(arr)
来源：http://gk.lnxyls.cn

PHP:  count($arr);
来源：http://cc.panjiajie.cn

JS:   arr.length
来源：http://lj.newstarts.cn

TS:   arr.length
来源：http://mi.shxzukj.cn

Java: list.size();
来源：http://oe.newstarts.cn

Go:   len(arr)
来源：http://bs.lnxyls.cn

Ruby: arr.length; arr.size
来源：http://mi.shtwfgs.cn

C#:   list.Count;
来源：http://hu.colortex.cn

[D07] 切片 / 取子数组
来源：http://rk.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zy.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fh.newstarts.cn

JS:   arr.slice(1, 4);
来源：http://wi.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://ux.asd995.cn

Java: list.subList(1, 4);
来源：http://sn.bookmarksfly.cn

Go:   arr[1:4]
来源：http://ok.nicolike.cn

Ruby: arr[1, 3]
来源：http://pp.bjjhwx.cn

C#:   list.GetRange(1, 3);
来源：http://tf.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://je.hnjuh.cn

Py:   a + b;  a.extend(b)
来源：http://ja.asd995.cn

PHP:  array_merge($a, $b);
来源：http://bx.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://pz.szxytkj.cn

TS:   [...a, ...b];
来源：http://px.wgjwhj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jb.shtwfgs.cn

Go:   append(a, b...)
来源：http://cs.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://wh.chemitech.net.cn

C#:   a.Concat(b).ToList()
来源：http://fv.colortex.cn

[D09] 排序（升序）
来源：http://ag.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://bc.huixinmuqiang.cn

PHP:  sort($arr);
来源：http://ir.muxihuayi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wo.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ha.panjiajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://dx.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://zd.szsharing.cn

Ruby: arr.sort
来源：http://ba.newstarts.cn

C#:   list.Sort();
来源：http://pv.yuexingan06.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ww.shtwfgs.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lg.bookmarksfly.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://gw.9csxet.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ph.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fr.shxzskj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jg.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://rl.panjiajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oj.newstarts.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wh.chemitech.net.cn

[D11] 反转数组
来源：http://jj.shxzukj.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sq.521024.cn

PHP:  array_reverse($arr);
来源：http://sl.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jr.9csxet.cn

TS:   [...arr].reverse();
来源：http://eg.wgjwhj.cn

Java: Collections.reverse(list);
来源：http://up.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://ky.huixinmuqiang.cn

Ruby: arr.reverse
来源：http://cr.huanxung.cn

C#:   list.Reverse();
来源：http://se.haigaiapp.cn

[D12] 查找元素下标
来源：http://qw.jctech888.com.cn

Py:   arr.index(x);  x in arr
来源：http://ea.bjjhwx.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://pl.yuntaijiaju.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://id.wgjwhj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qa.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ef.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://ib.9csxet.cn

Ruby: arr.index(x)
来源：http://jf.521024.cn

C#:   list.IndexOf(x);
来源：http://oc.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://jf.wgjwhj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qy.bjjhwx.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://bl.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://pb.shtwfgs.cn

TS:   arr.filter(x => x > 3)
来源：http://fz.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hk.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://oq.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yo.521024.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://mc.jctech888.com.cn

[D14] 映射转换（每个元素变形）
来源：http://vv.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lj.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xu.huixiangedu.cn

JS:   arr.map(x => x * 2)
来源：http://af.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://in.shxzskj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wc.szxytkj.cn

Go:   // 手写循环
来源：http://xq.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://de.haigaiapp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ce.huanxung.cn

[D15] 去重
来源：http://fk.9csxet.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gz.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://en.521024.cn

JS:   [...new Set(arr)]
来源：http://ux.nszjky.cn

TS:   [...new Set(arr)]
来源：http://sh.bjjhwx.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://gq.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://pg.szsharing.cn

Ruby: arr.uniq
来源：http://hz.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://ja.bjjhwx.cn

[D16] 求和与平均值
来源：http://je.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ei.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ap.hahajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://rw.szxytkj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zh.szsharing.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tx.hnjuh.cn

Go:   // 手写循环累加
来源：http://lf.shxzskj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sn.lnxyls.cn

C#:   list.Sum();  list.Average()
来源：http://cv.asd995.cn

[D17] 最大值与最小值
来源：http://bk.nszjky.cn

Py:   max(arr);  min(arr)
来源：http://ra.szsharing.cn

PHP:  max($arr);  min($arr);
来源：http://az.521024.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hu.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://vr.bjjhwx.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xq.nicolike.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rd.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://tj.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://ah.shxzukj.cn

[D18] 扁平化嵌套数组
来源：http://jt.szsharing.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://nh.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://jc.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://md.szsharing.cn

TS:   nested.flat();
来源：http://pg.hnjuh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gg.muxihuayi.cn

Go:   // 手写双层循环
来源：http://ld.jianghongdianzi.cn

Ruby: nested.flatten
来源：http://cn.huanxung.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zj.shxzukj.cn

[D19] 按字段分组
来源：http://ao.jctech888.com.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mt.yuntaijiaju.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ik.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://nw.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yt.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gw.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://vt.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ut.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qf.huixiangedu.cn

[D20] 统计每个元素出现次数
来源：http://ct.haigaiapp.cn

Py:   Counter(arr)
来源：http://lv.huixiangedu.cn

PHP:  array_count_values($arr);
来源：http://yc.huixiangedu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cj.shtwfgs.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oe.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sr.szsharing.cn

Go:   // 手写 map[T]int
来源：http://lt.bjjhwx.cn

Ruby: arr.tally
来源：http://yh.nicolike.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pp.jianghongdianzi.cn

[D21] 判断是否包含某元素
来源：http://hv.chemitech.net.cn

Py:   x in arr
来源：http://qy.9csxet.cn

PHP:  in_array($x, $arr, true);
来源：http://si.yuntaijiaju.cn

JS:   arr.includes(x)
来源：http://xl.huanxung.cn

TS:   arr.includes(x)
来源：http://ze.wgjwhj.cn

Java: list.contains(x)
来源：http://bf.bookmarksfly.cn

Go:   slices.Contains(arr, x)
来源：http://nr.colortex.cn

Ruby: arr.include?(x)
来源：http://ci.shxzskj.cn

C#:   list.Contains(x)
来源：http://hz.colortex.cn

[D22] 复制数组（避免共享引用）
来源：http://dx.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lv.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nu.hahajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jb.shxzukj.cn

TS:   [...arr];
来源：http://zo.colortex.cn

Java: new ArrayList<>(list);
来源：http://ew.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jp.hnjuh.cn

Ruby: arr.dup;  arr.clone
来源：http://je.hnjuh.cn

C#:   new List<int>(list);
来源：http://nt.shxzukj.cn

[D23] reduce 累积计算
来源：http://wv.hahajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zw.jctech888.com.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bd.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zs.newstarts.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ba.asd995.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pu.jianghongdianzi.cn

Go:   // 手写循环
来源：http://mv.shtwfgs.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://my.haigaiapp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vt.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://tf.nszjky.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ls.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mw.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://jm.hahajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cu.huixinmuqiang.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lb.colortex.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mm.asd995.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://js.521024.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ye.gzmigu.cn

[D25] Set 集合去重与交并差
来源：http://nt.huanxung.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sj.shxzskj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dy.newstarts.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qj.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ea.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://um.asd995.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rh.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://dx.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kq.chemitech.net.cn

[D26] 数组转字符串
来源：http://gt.huixiangedu.cn

Py:   ", ".join(map(str, arr))
来源：http://dj.huixinmuqiang.cn

PHP:  implode(", ", $arr);
来源：http://xs.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://ja.muxihuayi.cn

TS:   arr.join(", ")
来源：http://fs.nszjky.cn

Java: String.join(", ", list)
来源：http://wa.asd995.cn

Go:   strings.Join(strs, ", ")
来源：http://qc.panjiajie.cn

Ruby: arr.join(", ")
来源：http://zp.nszjky.cn

C#:   string.Join(", ", list)
来源：http://mk.gzmigu.cn

================================================================================
来源：http://yf.521024.cn

E. 字符串处理
来源：http://le.huixiangedu.cn

================================================================================
来源：http://ve.haigaiapp.cn

[E01] 拼接字符串
来源：http://gf.panjiajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pz.bjjhwx.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mo.nicolike.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qq.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xs.jctech888.com.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xu.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zw.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://zp.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kq.huixinmuqiang.cn

[E02] 重复字符串
来源：http://pu.muxihuayi.cn

Py:   "ab" * 3
来源：http://fx.huixinmuqiang.cn

PHP:  str_repeat("ab", 3);
来源：http://hl.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://kx.yuntaijiaju.cn

TS:   "ab".repeat(3)
来源：http://dr.gzmigu.cn

Java: "ab".repeat(3)
来源：http://bo.huixinmuqiang.cn

Go:   strings.Repeat("ab", 3)
来源：http://cf.hnjuh.cn

Ruby: "ab" * 3
来源：http://pi.gzmigu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://at.huanxung.cn

[E03] 截取子串
来源：http://qc.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gm.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qg.szxytkj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dp.asd995.cn

TS:   s.slice(1, 4)
来源：http://ru.nszjky.cn

Java: s.substring(1, 4)
来源：http://ej.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ku.newstarts.cn


<!-- 参考信息 -->