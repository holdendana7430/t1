代发 wailian999

[C14] 泛型函数
来源：http://rz.hahajie.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sa.shtwfgs.cn

PHP:  // 无泛型
来源：http://yo.nicolike.cn

JS:   // 无泛型
来源：http://sd.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hs.nicolike.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hq.yuntaijiaju.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mq.yuexingan06.cn

Ruby: # 无泛型
来源：http://ke.shxzukj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lu.newstarts.cn

[C15] 解构 / 展开参数
来源：http://ir.gzmigu.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ce.szxytkj.cn

PHP:  [$a, $b] = $pair;
来源：http://iw.hnjuh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://rj.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://oj.9csxet.cn

Java: // 无解构
来源：http://zw.yuntaijiaju.cn

Go:   // 无解构
来源：http://zy.bookmarksfly.cn

Ruby: a, b = pair
来源：http://gv.bookmarksfly.cn

C#:   var (a, b) = pair;
来源：http://ow.hahajie.cn

[C16] 函数 / 方法重载
来源：http://wk.bookmarksfly.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://ag.shxzukj.cn

PHP:  // 无重载
来源：http://aa.chemitech.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://zn.yuntaijiaju.cn

TS:   // 用联合类型或重载签名声明
来源：http://vf.nszjky.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bp.gzmigu.cn

Go:   // 无重载：用不同函数名
来源：http://ir.lnxyls.cn

Ruby: # 无重载：靠动态参数
来源：http://yl.yuntaijiaju.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://tx.asd995.cn

================================================================================
来源：http://rh.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://on.gzmigu.cn

================================================================================
来源：http://fk.nicolike.cn

[D01] 创建数组 / 列表
来源：http://ov.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ei.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://jh.szsharing.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://lh.521024.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://sp.jianghongdianzi.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://tf.nicolike.cn

Go:   arr := []int{1, 2, 3}
来源：http://ya.huanxung.cn

Ruby: arr = [1, 2, 3]
来源：http://zv.huixiangedu.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sz.bjjhwx.cn

[D02] 追加元素到末尾
来源：http://no.yuntaijiaju.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wu.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://va.hnjuh.cn

JS:   arr.push(4);
来源：http://uu.nicolike.cn

TS:   arr.push(4);
来源：http://gl.szxytkj.cn

Java: list.add(4);
来源：http://hb.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://qw.huixinmuqiang.cn

Ruby: arr << 4; arr.push(5)
来源：http://ut.szsharing.cn

C#:   list.Add(4);
来源：http://oc.jianghongdianzi.cn

[D03] 在指定位置插入元素
来源：http://gs.szxytkj.cn

Py:   arr.insert(0, 0)
来源：http://qv.521024.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ct.muxihuayi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uu.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://aq.shxzukj.cn

Java: list.add(0, 0);
来源：http://op.szxytkj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ak.wgjwhj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mm.shtwfgs.cn

C#:   list.Insert(0, 0);
来源：http://op.bookmarksfly.cn

[D04] 删除元素
来源：http://nw.jctech888.com.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://om.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fk.shxzukj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.huanxung.cn

TS:   arr.splice(0, 1);
来源：http://sv.hnjuh.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ie.muxihuayi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ea.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hb.hahajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zy.panjiajie.cn

[D05] 访问与修改元素
来源：http://jx.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://cf.asd995.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ox.shxzskj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://rv.shtwfgs.cn

TS:   arr[0]; arr.at(-1);
来源：http://er.shtwfgs.cn

Java: list.get(0); list.set(0, 9);
来源：http://la.panjiajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://xs.huanxung.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xi.asd995.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ia.huanxung.cn

[D06] 数组长度
来源：http://qk.bookmarksfly.cn

Py:   len(arr)
来源：http://fl.nicolike.cn

PHP:  count($arr);
来源：http://da.hnjuh.cn

JS:   arr.length
来源：http://hz.yuexingan06.cn

TS:   arr.length
来源：http://vh.gzmigu.cn

Java: list.size();
来源：http://io.hnjuh.cn

Go:   len(arr)
来源：http://bn.nicolike.cn

Ruby: arr.length; arr.size
来源：http://yf.nszjky.cn

C#:   list.Count;
来源：http://ga.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://mq.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mm.gzmigu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bi.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://cv.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://hi.shxzskj.cn

Java: list.subList(1, 4);
来源：http://gu.hahajie.cn

Go:   arr[1:4]
来源：http://hf.9csxet.cn

Ruby: arr[1, 3]
来源：http://ef.nszjky.cn

C#:   list.GetRange(1, 3);
来源：http://ll.hnjuh.cn

[D08] 合并两个数组
来源：http://ra.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://ju.hahajie.cn

PHP:  array_merge($a, $b);
来源：http://cr.jctech888.com.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gm.shxzukj.cn

TS:   [...a, ...b];
来源：http://up.szsharing.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://si.shtwfgs.cn

Go:   append(a, b...)
来源：http://fj.panjiajie.cn

Ruby: a + b;  a.concat(b)
来源：http://eo.yuexingan06.cn

C#:   a.Concat(b).ToList()
来源：http://nu.huixinmuqiang.cn

[D09] 排序（升序）
来源：http://ho.muxihuayi.cn

Py:   sorted(arr);  arr.sort()
来源：http://my.huixiangedu.cn

PHP:  sort($arr);
来源：http://nx.9csxet.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vv.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zp.bookmarksfly.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bi.szsharing.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gq.asd995.cn

Ruby: arr.sort
来源：http://rj.colortex.cn

C#:   list.Sort();
来源：http://av.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lu.haigaiapp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mm.haigaiapp.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ki.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yk.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gc.huanxung.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://et.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://fn.chemitech.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ej.jctech888.com.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ny.colortex.cn

[D11] 反转数组
来源：http://dg.jctech888.com.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xt.panjiajie.cn

PHP:  array_reverse($arr);
来源：http://im.jianghongdianzi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://zw.wgjwhj.cn

TS:   [...arr].reverse();
来源：http://ju.yuntaijiaju.cn

Java: Collections.reverse(list);
来源：http://yq.hnjuh.cn

Go:   slices.Reverse(arr)
来源：http://lq.szsharing.cn

Ruby: arr.reverse
来源：http://ms.szsharing.cn

C#:   list.Reverse();
来源：http://id.shxzskj.cn

[D12] 查找元素下标
来源：http://on.lnxyls.cn

Py:   arr.index(x);  x in arr
来源：http://fl.wgjwhj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ze.hnjuh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bj.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cv.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yy.szsharing.cn

Go:   slices.Index(arr, x)
来源：http://ee.colortex.cn

Ruby: arr.index(x)
来源：http://pj.yuntaijiaju.cn

C#:   list.IndexOf(x);
来源：http://uu.gzmigu.cn

[D13] 过滤（保留满足条件的）
来源：http://xb.haigaiapp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fl.asd995.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jd.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://qu.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://yz.panjiajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jr.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ob.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wx.gzmigu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ib.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://gg.shtwfgs.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://jg.yuexingan06.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://rn.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://pn.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://iu.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vs.bjjhwx.cn

Go:   // 手写循环
来源：http://fp.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wf.huixiangedu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zw.shxzskj.cn

[D15] 去重
来源：http://mp.muxihuayi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://es.chemitech.net.cn

PHP:  array_unique($arr);
来源：http://np.9csxet.cn

JS:   [...new Set(arr)]
来源：http://ra.lnxyls.cn

TS:   [...new Set(arr)]
来源：http://wp.bjjhwx.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ml.huixinmuqiang.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xi.colortex.cn

Ruby: arr.uniq
来源：http://qq.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://yq.jianghongdianzi.cn

[D16] 求和与平均值
来源：http://yp.jianghongdianzi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ij.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rz.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://le.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zo.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ad.yuexingan06.cn

Go:   // 手写循环累加
来源：http://ju.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sg.lnxyls.cn

C#:   list.Sum();  list.Average()
来源：http://wf.chemitech.net.cn

[D17] 最大值与最小值
来源：http://ps.asd995.cn

Py:   max(arr);  min(arr)
来源：http://gr.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://wk.muxihuayi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ml.bookmarksfly.cn

TS:   Math.max(...arr);
来源：http://zc.521024.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cf.521024.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://za.bjjhwx.cn

Ruby: arr.max;  arr.min
来源：http://mw.szsharing.cn

C#:   list.Max();  list.Min()
来源：http://mz.newstarts.cn

[D18] 扁平化嵌套数组
来源：http://pm.gzmigu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://we.hahajie.cn

PHP:  array_merge(...$nested);
来源：http://kw.huixiangedu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hu.shxzskj.cn

TS:   nested.flat();
来源：http://kt.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pi.newstarts.cn

Go:   // 手写双层循环
来源：http://ih.szxytkj.cn

Ruby: nested.flatten
来源：http://xu.hahajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://uh.colortex.cn

[D19] 按字段分组
来源：http://ea.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pn.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://je.lnxyls.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dc.hahajie.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lj.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zc.szsharing.cn

Go:   // 手写 map[string][]T
来源：http://wl.jianghongdianzi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ww.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://jz.hnjuh.cn

[D20] 统计每个元素出现次数
来源：http://nw.bookmarksfly.cn

Py:   Counter(arr)
来源：http://nf.szsharing.cn

PHP:  array_count_values($arr);
来源：http://cv.shxzukj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jj.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ni.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://fs.asd995.cn

Go:   // 手写 map[T]int
来源：http://zu.newstarts.cn

Ruby: arr.tally
来源：http://es.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jd.hahajie.cn

[D21] 判断是否包含某元素
来源：http://yk.szxytkj.cn

Py:   x in arr
来源：http://xj.521024.cn

PHP:  in_array($x, $arr, true);
来源：http://ld.jctech888.com.cn

JS:   arr.includes(x)
来源：http://ey.haigaiapp.cn

TS:   arr.includes(x)
来源：http://yi.panjiajie.cn

Java: list.contains(x)
来源：http://fo.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://lo.huixinmuqiang.cn

Ruby: arr.include?(x)
来源：http://xx.huixinmuqiang.cn

C#:   list.Contains(x)
来源：http://xw.jianghongdianzi.cn

[D22] 复制数组（避免共享引用）
来源：http://om.szsharing.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xt.nszjky.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ji.huixinmuqiang.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://vb.521024.cn

TS:   [...arr];
来源：http://dr.huanxung.cn

Java: new ArrayList<>(list);
来源：http://uq.huixiangedu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tv.hnjuh.cn

Ruby: arr.dup;  arr.clone
来源：http://yw.huixiangedu.cn

C#:   new List<int>(list);
来源：http://ex.lnxyls.cn

[D23] reduce 累积计算
来源：http://yq.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zu.jianghongdianzi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ds.haigaiapp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vk.newstarts.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dv.chemitech.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://du.wgjwhj.cn

Go:   // 手写循环
来源：http://sk.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://nc.szsharing.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://uj.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://ij.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jf.nicolike.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mz.huixiangedu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gx.yuexingan06.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ss.chemitech.net.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://lf.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://kl.nszjky.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://at.colortex.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jp.521024.cn

[D25] Set 集合去重与交并差
来源：http://xj.bookmarksfly.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uy.hnjuh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kd.huanxung.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rw.panjiajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hl.asd995.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pt.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jo.lnxyls.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pu.jianghongdianzi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cn.haigaiapp.cn

[D26] 数组转字符串
来源：http://yr.bjjhwx.cn

Py:   ", ".join(map(str, arr))
来源：http://br.szxytkj.cn

PHP:  implode(", ", $arr);
来源：http://ay.hahajie.cn

JS:   arr.join(", ")
来源：http://md.huanxung.cn

TS:   arr.join(", ")
来源：http://qj.wgjwhj.cn

Java: String.join(", ", list)
来源：http://wz.yuntaijiaju.cn

Go:   strings.Join(strs, ", ")
来源：http://zu.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://rs.huanxung.cn

C#:   string.Join(", ", list)
来源：http://dl.bookmarksfly.cn

================================================================================
来源：http://bl.newstarts.cn

E. 字符串处理
来源：http://dw.huanxung.cn

================================================================================
来源：http://ik.lnxyls.cn

[E01] 拼接字符串
来源：http://pj.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zw.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://eu.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hb.shxzskj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gc.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ap.asd995.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hd.haigaiapp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://id.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://lg.yuntaijiaju.cn

[E02] 重复字符串
来源：http://uv.chemitech.net.cn

Py:   "ab" * 3
来源：http://il.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://tx.hahajie.cn

JS:   "ab".repeat(3)
来源：http://my.nszjky.cn

TS:   "ab".repeat(3)
来源：http://xh.nicolike.cn

Java: "ab".repeat(3)
来源：http://pc.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://df.huixiangedu.cn

Ruby: "ab" * 3
来源：http://xz.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gz.colortex.cn

[E03] 截取子串
来源：http://jj.haigaiapp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://kp.nszjky.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zy.shxzukj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dq.yuexingan06.cn

TS:   s.slice(1, 4)
来源：http://ec.shxzukj.cn

Java: s.substring(1, 4)
来源：http://zj.colortex.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ax.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://he.jctech888.com.cn

C#:   s.Substring(1, 3)
来源：http://we.nszjky.cn

[E04] 查找子串位置
来源：http://mh.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://at.9csxet.cn

PHP:  strpos($s, "x");
来源：http://eg.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qc.szxytkj.cn

TS:   s.indexOf("x")
来源：http://el.jctech888.com.cn

Java: s.indexOf("x")
来源：http://pg.muxihuayi.cn


<!-- 参考信息 -->