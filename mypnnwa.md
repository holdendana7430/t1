代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://md.shtwfgs.cn

Go:   func add(a, b int) int
来源：http://nw.gzmigu.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ea.haigaiapp.cn

C#:   int Add(int a, int b) => a + b;
来源：http://vc.huixinmuqiang.cn

[C14] 泛型函数
来源：http://vp.hnjuh.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://cm.bookmarksfly.cn

PHP:  // 无泛型
来源：http://hc.colortex.cn

JS:   // 无泛型
来源：http://ps.shtwfgs.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://aa.nszjky.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://eh.jianghongdianzi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ld.szxytkj.cn

Ruby: # 无泛型
来源：http://yk.panjiajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vi.jctech888.com.cn

[C15] 解构 / 展开参数
来源：http://gb.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wl.jctech888.com.cn

PHP:  [$a, $b] = $pair;
来源：http://mn.bjjhwx.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ci.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://rg.nicolike.cn

Java: // 无解构
来源：http://ch.huixiangedu.cn

Go:   // 无解构
来源：http://aa.szxytkj.cn

Ruby: a, b = pair
来源：http://so.9csxet.cn

C#:   var (a, b) = pair;
来源：http://vh.hnjuh.cn

[C16] 函数 / 方法重载
来源：http://eg.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vi.yuntaijiaju.cn

PHP:  // 无重载
来源：http://jz.yuexingan06.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://pe.nszjky.cn

TS:   // 用联合类型或重载签名声明
来源：http://yt.shtwfgs.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://il.haigaiapp.cn

Go:   // 无重载：用不同函数名
来源：http://nx.huixiangedu.cn

Ruby: # 无重载：靠动态参数
来源：http://ra.jctech888.com.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://zw.jctech888.com.cn

================================================================================
来源：http://uq.lnxyls.cn

D. 数组 / 列表 / 集合
来源：http://yv.asd995.cn

================================================================================
来源：http://ms.huanxung.cn

[D01] 创建数组 / 列表
来源：http://ht.chemitech.net.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://yj.jctech888.com.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://lz.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://kz.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bi.hnjuh.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://af.jianghongdianzi.cn

Go:   arr := []int{1, 2, 3}
来源：http://jo.haigaiapp.cn

Ruby: arr = [1, 2, 3]
来源：http://zj.asd995.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://xu.szxytkj.cn

[D02] 追加元素到末尾
来源：http://hc.bookmarksfly.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://am.colortex.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://dg.nszjky.cn

JS:   arr.push(4);
来源：http://yo.colortex.cn

TS:   arr.push(4);
来源：http://ir.szsharing.cn

Java: list.add(4);
来源：http://fy.521024.cn

Go:   arr = append(arr, 4)
来源：http://hi.nszjky.cn

Ruby: arr << 4; arr.push(5)
来源：http://za.jctech888.com.cn

C#:   list.Add(4);
来源：http://fg.shtwfgs.cn

[D03] 在指定位置插入元素
来源：http://yt.szxytkj.cn

Py:   arr.insert(0, 0)
来源：http://wx.panjiajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://tu.yuntaijiaju.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://gp.huixiangedu.cn

TS:   arr.splice(0, 0, 0);
来源：http://ek.yuntaijiaju.cn

Java: list.add(0, 0);
来源：http://vh.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lr.asd995.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sp.huanxung.cn

C#:   list.Insert(0, 0);
来源：http://ir.szsharing.cn

[D04] 删除元素
来源：http://fc.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sp.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://tc.hnjuh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://uj.shtwfgs.cn

TS:   arr.splice(0, 1);
来源：http://sj.yuexingan06.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://ym.9csxet.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nu.bookmarksfly.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qr.yuexingan06.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://oy.nicolike.cn

[D05] 访问与修改元素
来源：http://yd.szxytkj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://rc.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://fp.shxzukj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://qu.bookmarksfly.cn

TS:   arr[0]; arr.at(-1);
来源：http://ao.shxzukj.cn

Java: list.get(0); list.set(0, 9);
来源：http://hy.hahajie.cn

Go:   arr[0]; arr[0] = 9
来源：http://ke.hnjuh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fl.colortex.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sa.jctech888.com.cn

[D06] 数组长度
来源：http://th.muxihuayi.cn

Py:   len(arr)
来源：http://qr.colortex.cn

PHP:  count($arr);
来源：http://bd.jctech888.com.cn

JS:   arr.length
来源：http://ny.wgjwhj.cn

TS:   arr.length
来源：http://dm.shtwfgs.cn

Java: list.size();
来源：http://xc.jianghongdianzi.cn

Go:   len(arr)
来源：http://ge.chemitech.net.cn

Ruby: arr.length; arr.size
来源：http://hb.hahajie.cn

C#:   list.Count;
来源：http://ak.bookmarksfly.cn

[D07] 切片 / 取子数组
来源：http://gg.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hw.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gf.9csxet.cn

JS:   arr.slice(1, 4);
来源：http://yv.haigaiapp.cn

TS:   arr.slice(1, 4);
来源：http://qi.panjiajie.cn

Java: list.subList(1, 4);
来源：http://ei.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://gs.nicolike.cn

Ruby: arr[1, 3]
来源：http://un.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://qn.newstarts.cn

[D08] 合并两个数组
来源：http://sm.huixiangedu.cn

Py:   a + b;  a.extend(b)
来源：http://eg.bjjhwx.cn

PHP:  array_merge($a, $b);
来源：http://ej.szxytkj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://mu.haigaiapp.cn

TS:   [...a, ...b];
来源：http://fn.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nm.shxzskj.cn

Go:   append(a, b...)
来源：http://ly.nicolike.cn

Ruby: a + b;  a.concat(b)
来源：http://gc.huanxung.cn

C#:   a.Concat(b).ToList()
来源：http://uc.chemitech.net.cn

[D09] 排序（升序）
来源：http://ai.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://wh.muxihuayi.cn

PHP:  sort($arr);
来源：http://ae.shxzskj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tn.szxytkj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fh.wgjwhj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ti.huixinmuqiang.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dl.newstarts.cn

Ruby: arr.sort
来源：http://qd.huanxung.cn

C#:   list.Sort();
来源：http://wq.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://oz.panjiajie.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xd.panjiajie.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://qj.bjjhwx.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bj.shxzukj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://yi.huixinmuqiang.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xl.521024.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dn.jctech888.com.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ot.huanxung.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://pn.panjiajie.cn

[D11] 反转数组
来源：http://gd.nszjky.cn

Py:   arr[::-1];  arr.reverse()
来源：http://vo.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://mu.muxihuayi.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://gh.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://wv.szsharing.cn

Java: Collections.reverse(list);
来源：http://ir.lnxyls.cn

Go:   slices.Reverse(arr)
来源：http://cb.9csxet.cn

Ruby: arr.reverse
来源：http://ty.huixiangedu.cn

C#:   list.Reverse();
来源：http://ql.bookmarksfly.cn

[D12] 查找元素下标
来源：http://vl.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://po.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eu.szxytkj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nq.hahajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tx.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dv.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://bz.shxzskj.cn

Ruby: arr.index(x)
来源：http://fo.nszjky.cn

C#:   list.IndexOf(x);
来源：http://ix.newstarts.cn

[D13] 过滤（保留满足条件的）
来源：http://nb.nszjky.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jj.yuexingan06.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://xr.muxihuayi.cn

JS:   arr.filter(x => x > 3)
来源：http://xe.shxzskj.cn

TS:   arr.filter(x => x > 3)
来源：http://id.bookmarksfly.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dm.hahajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nv.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ck.shxzukj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://is.muxihuayi.cn

[D14] 映射转换（每个元素变形）
来源：http://qb.haigaiapp.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rm.yuntaijiaju.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ur.haigaiapp.cn

JS:   arr.map(x => x * 2)
来源：http://yk.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://gu.chemitech.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://um.shxzukj.cn

Go:   // 手写循环
来源：http://es.shtwfgs.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ct.szsharing.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rd.nszjky.cn

[D15] 去重
来源：http://zt.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yt.shxzskj.cn

PHP:  array_unique($arr);
来源：http://vn.muxihuayi.cn

JS:   [...new Set(arr)]
来源：http://rz.shxzskj.cn

TS:   [...new Set(arr)]
来源：http://ay.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://np.haigaiapp.cn

Go:   // 用 map[T]struct{} 手写
来源：http://uo.bookmarksfly.cn

Ruby: arr.uniq
来源：http://ag.lnxyls.cn

C#:   list.Distinct().ToList()
来源：http://pn.jianghongdianzi.cn

[D16] 求和与平均值
来源：http://ct.panjiajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://eu.hnjuh.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yr.huanxung.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bx.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://tz.huixiangedu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ij.hahajie.cn

Go:   // 手写循环累加
来源：http://lo.nicolike.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nn.haigaiapp.cn

C#:   list.Sum();  list.Average()
来源：http://xo.yuexingan06.cn

[D17] 最大值与最小值
来源：http://ov.szsharing.cn

Py:   max(arr);  min(arr)
来源：http://qz.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://ak.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xv.nszjky.cn

TS:   Math.max(...arr);
来源：http://rf.bjjhwx.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bz.shxzskj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://nb.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://ri.haigaiapp.cn

C#:   list.Max();  list.Min()
来源：http://jf.asd995.cn

[D18] 扁平化嵌套数组
来源：http://cb.nszjky.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ss.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://kt.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://th.shxzukj.cn

TS:   nested.flat();
来源：http://zz.lnxyls.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ks.yuexingan06.cn

Go:   // 手写双层循环
来源：http://js.wgjwhj.cn

Ruby: nested.flatten
来源：http://ky.huanxung.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://kh.bjjhwx.cn

[D19] 按字段分组
来源：http://ga.yuexingan06.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vz.shxzukj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hr.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jo.bookmarksfly.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jh.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wc.colortex.cn

Go:   // 手写 map[string][]T
来源：http://rg.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ir.huixinmuqiang.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rf.yuntaijiaju.cn

[D20] 统计每个元素出现次数
来源：http://wu.bjjhwx.cn

Py:   Counter(arr)
来源：http://rr.jianghongdianzi.cn

PHP:  array_count_values($arr);
来源：http://ej.jianghongdianzi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hd.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://el.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://xk.asd995.cn

Go:   // 手写 map[T]int
来源：http://bu.521024.cn

Ruby: arr.tally
来源：http://pp.gzmigu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fd.jianghongdianzi.cn

[D21] 判断是否包含某元素
来源：http://vn.wgjwhj.cn

Py:   x in arr
来源：http://ze.yuntaijiaju.cn

PHP:  in_array($x, $arr, true);
来源：http://dp.gzmigu.cn

JS:   arr.includes(x)
来源：http://pt.muxihuayi.cn

TS:   arr.includes(x)
来源：http://qz.nszjky.cn

Java: list.contains(x)
来源：http://rb.shtwfgs.cn

Go:   slices.Contains(arr, x)
来源：http://qm.huixiangedu.cn

Ruby: arr.include?(x)
来源：http://rg.9csxet.cn

C#:   list.Contains(x)
来源：http://zi.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://fw.szsharing.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ml.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zc.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://av.hahajie.cn

TS:   [...arr];
来源：http://lv.shxzskj.cn

Java: new ArrayList<>(list);
来源：http://vi.nicolike.cn

Go:   copied := append([]int(nil), arr...)
来源：http://fs.wgjwhj.cn

Ruby: arr.dup;  arr.clone
来源：http://tp.jctech888.com.cn

C#:   new List<int>(list);
来源：http://km.newstarts.cn

[D23] reduce 累积计算
来源：http://qm.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fd.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://dr.panjiajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zd.nszjky.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fo.haigaiapp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yh.shxzskj.cn

Go:   // 手写循环
来源：http://kh.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vj.wgjwhj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qr.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://fo.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://vq.huixinmuqiang.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qd.bookmarksfly.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ht.yuntaijiaju.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bw.szxytkj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://cn.nicolike.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bi.yuntaijiaju.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://if.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kt.bjjhwx.cn

[D25] Set 集合去重与交并差
来源：http://oh.shxzukj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ug.nszjky.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ci.muxihuayi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nt.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jo.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://nq.yuntaijiaju.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://md.hahajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ym.nszjky.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fh.gzmigu.cn

[D26] 数组转字符串
来源：http://ig.gzmigu.cn

Py:   ", ".join(map(str, arr))
来源：http://nc.muxihuayi.cn

PHP:  implode(", ", $arr);
来源：http://xu.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://ma.panjiajie.cn

TS:   arr.join(", ")
来源：http://gb.521024.cn

Java: String.join(", ", list)
来源：http://bn.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://th.shxzskj.cn

Ruby: arr.join(", ")
来源：http://gb.521024.cn

C#:   string.Join(", ", list)
来源：http://zv.hnjuh.cn

================================================================================
来源：http://it.hahajie.cn

E. 字符串处理
来源：http://is.huixiangedu.cn

================================================================================
来源：http://pb.yuexingan06.cn

[E01] 拼接字符串
来源：http://ml.huanxung.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fd.bookmarksfly.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://il.chemitech.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://el.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://di.jianghongdianzi.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uj.shtwfgs.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://np.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://fv.lnxyls.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mh.hnjuh.cn

[E02] 重复字符串
来源：http://sg.shtwfgs.cn

Py:   "ab" * 3
来源：http://vi.9csxet.cn

PHP:  str_repeat("ab", 3);
来源：http://vm.shtwfgs.cn

JS:   "ab".repeat(3)
来源：http://gu.hahajie.cn

TS:   "ab".repeat(3)
来源：http://wm.asd995.cn

Java: "ab".repeat(3)
来源：http://qe.521024.cn

Go:   strings.Repeat("ab", 3)
来源：http://af.yuexingan06.cn

Ruby: "ab" * 3
来源：http://pe.9csxet.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vp.shtwfgs.cn

[E03] 截取子串
来源：http://co.newstarts.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ie.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qw.huixiangedu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.nicolike.cn

TS:   s.slice(1, 4)
来源：http://bn.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://xg.shxzskj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rh.hahajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://op.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://yf.panjiajie.cn

[E04] 查找子串位置
来源：http://og.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://vs.shxzskj.cn


<!-- 参考信息 -->