代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vz.521024.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://du.chemitech.net.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://gc.colortex.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://iy.muxihuayi.cn

Go:   arr := []int{1, 2, 3}
来源：http://fa.hahajie.cn

Ruby: arr = [1, 2, 3]
来源：http://zd.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ix.shxzskj.cn

[D02] 追加元素到末尾
来源：http://wu.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://lj.521024.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://le.asd995.cn

JS:   arr.push(4);
来源：http://pt.hnjuh.cn

TS:   arr.push(4);
来源：http://fi.yuexingan06.cn

Java: list.add(4);
来源：http://mj.nszjky.cn

Go:   arr = append(arr, 4)
来源：http://xr.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://qg.shxzukj.cn

C#:   list.Add(4);
来源：http://ug.wgjwhj.cn

[D03] 在指定位置插入元素
来源：http://ds.asd995.cn

Py:   arr.insert(0, 0)
来源：http://tu.yuexingan06.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mm.lnxyls.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cp.nszjky.cn

TS:   arr.splice(0, 0, 0);
来源：http://ec.nicolike.cn

Java: list.add(0, 0);
来源：http://qx.huanxung.cn

Go:   arr = append([]int{0}, arr...)
来源：http://sa.newstarts.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ds.bjjhwx.cn

C#:   list.Insert(0, 0);
来源：http://rw.newstarts.cn

[D04] 删除元素
来源：http://tx.huanxung.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://zs.szsharing.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://zt.hahajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bf.shxzskj.cn

TS:   arr.splice(0, 1);
来源：http://bs.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mg.521024.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ua.hnjuh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gj.yuntaijiaju.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://qm.panjiajie.cn

[D05] 访问与修改元素
来源：http://pq.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://az.shtwfgs.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://uz.szsharing.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xv.huixiangedu.cn

TS:   arr[0]; arr.at(-1);
来源：http://ek.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://ht.huanxung.cn

Go:   arr[0]; arr[0] = 9
来源：http://yw.haigaiapp.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://ln.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://fr.gzmigu.cn

[D06] 数组长度
来源：http://qz.huixinmuqiang.cn

Py:   len(arr)
来源：http://ri.bookmarksfly.cn

PHP:  count($arr);
来源：http://yr.jianghongdianzi.cn

JS:   arr.length
来源：http://uf.asd995.cn

TS:   arr.length
来源：http://ry.lnxyls.cn

Java: list.size();
来源：http://xc.huanxung.cn

Go:   len(arr)
来源：http://sx.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://de.huixinmuqiang.cn

C#:   list.Count;
来源：http://ia.huanxung.cn

[D07] 切片 / 取子数组
来源：http://ew.nszjky.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://oo.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://lu.shxzukj.cn

JS:   arr.slice(1, 4);
来源：http://wx.jctech888.com.cn

TS:   arr.slice(1, 4);
来源：http://za.yuntaijiaju.cn

Java: list.subList(1, 4);
来源：http://ac.gzmigu.cn

Go:   arr[1:4]
来源：http://nt.hahajie.cn

Ruby: arr[1, 3]
来源：http://bv.shtwfgs.cn

C#:   list.GetRange(1, 3);
来源：http://zf.shtwfgs.cn

[D08] 合并两个数组
来源：http://mw.bookmarksfly.cn

Py:   a + b;  a.extend(b)
来源：http://rs.9csxet.cn

PHP:  array_merge($a, $b);
来源：http://jg.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://he.panjiajie.cn

TS:   [...a, ...b];
来源：http://uu.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://us.haigaiapp.cn

Go:   append(a, b...)
来源：http://nt.yuntaijiaju.cn

Ruby: a + b;  a.concat(b)
来源：http://wk.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://cu.asd995.cn

[D09] 排序（升序）
来源：http://eh.colortex.cn

Py:   sorted(arr);  arr.sort()
来源：http://tn.nicolike.cn

PHP:  sort($arr);
来源：http://hc.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://vn.huanxung.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tc.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://oz.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tq.huixinmuqiang.cn

Ruby: arr.sort
来源：http://ah.asd995.cn

C#:   list.Sort();
来源：http://hu.hahajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://da.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zf.jctech888.com.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mf.jctech888.com.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rv.asd995.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ce.panjiajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zb.muxihuayi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kx.nszjky.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gc.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hi.gzmigu.cn

[D11] 反转数组
来源：http://kg.bookmarksfly.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gm.huanxung.cn

PHP:  array_reverse($arr);
来源：http://ga.gzmigu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://cq.colortex.cn

TS:   [...arr].reverse();
来源：http://nl.nicolike.cn

Java: Collections.reverse(list);
来源：http://te.huixiangedu.cn

Go:   slices.Reverse(arr)
来源：http://jw.9csxet.cn

Ruby: arr.reverse
来源：http://xi.huanxung.cn

C#:   list.Reverse();
来源：http://vs.hnjuh.cn

[D12] 查找元素下标
来源：http://lw.yuntaijiaju.cn

Py:   arr.index(x);  x in arr
来源：http://ye.yuexingan06.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://gm.yuntaijiaju.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://da.wgjwhj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://if.yuexingan06.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://on.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://ic.521024.cn

Ruby: arr.index(x)
来源：http://xg.newstarts.cn

C#:   list.IndexOf(x);
来源：http://pz.yuexingan06.cn

[D13] 过滤（保留满足条件的）
来源：http://tl.huixinmuqiang.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ie.chemitech.net.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tu.yuexingan06.cn

JS:   arr.filter(x => x > 3)
来源：http://by.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://va.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dv.newstarts.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yi.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qp.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://du.asd995.cn

[D14] 映射转换（每个元素变形）
来源：http://oa.nicolike.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gg.521024.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ul.haigaiapp.cn

JS:   arr.map(x => x * 2)
来源：http://ep.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://wt.yuexingan06.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wa.shxzukj.cn

Go:   // 手写循环
来源：http://zj.shtwfgs.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ir.bjjhwx.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vw.szxytkj.cn

[D15] 去重
来源：http://uk.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yn.huanxung.cn

PHP:  array_unique($arr);
来源：http://vw.muxihuayi.cn

JS:   [...new Set(arr)]
来源：http://zg.newstarts.cn

TS:   [...new Set(arr)]
来源：http://yn.haigaiapp.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wa.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dd.muxihuayi.cn

Ruby: arr.uniq
来源：http://ky.nicolike.cn

C#:   list.Distinct().ToList()
来源：http://xa.nicolike.cn

[D16] 求和与平均值
来源：http://dz.chemitech.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fr.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://au.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cy.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zf.shxzskj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mr.shxzukj.cn

Go:   // 手写循环累加
来源：http://wt.hnjuh.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ve.panjiajie.cn

C#:   list.Sum();  list.Average()
来源：http://nd.hnjuh.cn

[D17] 最大值与最小值
来源：http://qs.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://wt.hahajie.cn

PHP:  max($arr);  min($arr);
来源：http://ih.muxihuayi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gi.nszjky.cn

TS:   Math.max(...arr);
来源：http://pn.newstarts.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://lb.muxihuayi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vl.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://cv.shxzukj.cn

C#:   list.Max();  list.Min()
来源：http://tg.panjiajie.cn

[D18] 扁平化嵌套数组
来源：http://dx.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mx.nicolike.cn

PHP:  array_merge(...$nested);
来源：http://yw.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://rg.newstarts.cn

TS:   nested.flat();
来源：http://yu.haigaiapp.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pg.9csxet.cn

Go:   // 手写双层循环
来源：http://er.yuntaijiaju.cn

Ruby: nested.flatten
来源：http://st.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xr.9csxet.cn

[D19] 按字段分组
来源：http://yy.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://an.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cd.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://fy.huixinmuqiang.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wz.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kx.asd995.cn

Go:   // 手写 map[string][]T
来源：http://jd.muxihuayi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ic.hnjuh.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ov.jianghongdianzi.cn

[D20] 统计每个元素出现次数
来源：http://ng.521024.cn

Py:   Counter(arr)
来源：http://ph.newstarts.cn

PHP:  array_count_values($arr);
来源：http://fq.colortex.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ao.chemitech.net.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fv.asd995.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wo.shtwfgs.cn

Go:   // 手写 map[T]int
来源：http://xt.jctech888.com.cn

Ruby: arr.tally
来源：http://an.szxytkj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lm.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://oa.nszjky.cn

Py:   x in arr
来源：http://is.huixiangedu.cn

PHP:  in_array($x, $arr, true);
来源：http://ym.huixinmuqiang.cn

JS:   arr.includes(x)
来源：http://qa.asd995.cn

TS:   arr.includes(x)
来源：http://fa.521024.cn

Java: list.contains(x)
来源：http://vj.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://ha.hahajie.cn

Ruby: arr.include?(x)
来源：http://hb.9csxet.cn

C#:   list.Contains(x)
来源：http://zi.lnxyls.cn

[D22] 复制数组（避免共享引用）
来源：http://kx.yuexingan06.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fw.muxihuayi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qs.yuexingan06.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://be.szsharing.cn

TS:   [...arr];
来源：http://ba.shxzskj.cn

Java: new ArrayList<>(list);
来源：http://wa.shtwfgs.cn

Go:   copied := append([]int(nil), arr...)
来源：http://tq.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://tp.huixiangedu.cn

C#:   new List<int>(list);
来源：http://ut.wgjwhj.cn

[D23] reduce 累积计算
来源：http://ua.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hb.szsharing.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ry.jianghongdianzi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fa.yuexingan06.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://pq.jianghongdianzi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fi.huixinmuqiang.cn

Go:   // 手写循环
来源：http://bu.9csxet.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cs.huixiangedu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://tb.nicolike.cn

[D24] 字典 / Map 基本操作
来源：http://bs.szsharing.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ou.nicolike.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://zg.hnjuh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ep.9csxet.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gx.nicolike.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jm.shxzskj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wo.bookmarksfly.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pl.asd995.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qx.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://hh.wgjwhj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zt.colortex.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://dx.shxzukj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ws.gzmigu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pf.gzmigu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ey.shxzukj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tp.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://cv.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://aj.shtwfgs.cn

[D26] 数组转字符串
来源：http://ik.bjjhwx.cn

Py:   ", ".join(map(str, arr))
来源：http://gi.shtwfgs.cn

PHP:  implode(", ", $arr);
来源：http://bh.9csxet.cn

JS:   arr.join(", ")
来源：http://rh.asd995.cn

TS:   arr.join(", ")
来源：http://ub.huixiangedu.cn

Java: String.join(", ", list)
来源：http://qf.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://ex.haigaiapp.cn

Ruby: arr.join(", ")
来源：http://rf.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://ho.colortex.cn

================================================================================
来源：http://op.nszjky.cn

E. 字符串处理
来源：http://yg.yuntaijiaju.cn

================================================================================
来源：http://kt.jctech888.com.cn

[E01] 拼接字符串
来源：http://sh.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ox.chemitech.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://rs.bjjhwx.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://uk.9csxet.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nw.jctech888.com.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xa.lnxyls.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oc.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ao.jianghongdianzi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://re.bjjhwx.cn

[E02] 重复字符串
来源：http://do.szxytkj.cn

Py:   "ab" * 3
来源：http://nd.jianghongdianzi.cn

PHP:  str_repeat("ab", 3);
来源：http://bl.colortex.cn

JS:   "ab".repeat(3)
来源：http://zr.jianghongdianzi.cn

TS:   "ab".repeat(3)
来源：http://uk.shxzskj.cn

Java: "ab".repeat(3)
来源：http://ke.nicolike.cn

Go:   strings.Repeat("ab", 3)
来源：http://qx.colortex.cn

Ruby: "ab" * 3
来源：http://bw.hnjuh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mv.yuntaijiaju.cn

[E03] 截取子串
来源：http://ed.szsharing.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zh.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ky.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ws.chemitech.net.cn

TS:   s.slice(1, 4)
来源：http://dm.nszjky.cn

Java: s.substring(1, 4)
来源：http://at.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://iu.huanxung.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ns.huixinmuqiang.cn

C#:   s.Substring(1, 3)
来源：http://ap.nszjky.cn

[E04] 查找子串位置
来源：http://ks.huixinmuqiang.cn

Py:   s.find("x");  s.index("x")
来源：http://tf.bookmarksfly.cn

PHP:  strpos($s, "x");
来源：http://jj.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gg.bookmarksfly.cn

TS:   s.indexOf("x")
来源：http://yc.haigaiapp.cn

Java: s.indexOf("x")
来源：http://yc.newstarts.cn

Go:   strings.Index(s, "x")
来源：http://vj.shtwfgs.cn

Ruby: s.index("x")
来源：http://wl.szxytkj.cn

C#:   s.IndexOf("x")
来源：http://ld.bjjhwx.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.newstarts.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cq.chemitech.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bn.shxzukj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yr.shxzukj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ef.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kj.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tj.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ic.jianghongdianzi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nd.bjjhwx.cn

[E06] 替换子串
来源：http://qb.chemitech.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ok.jctech888.com.cn

PHP:  str_replace("a", "b", $s);
来源：http://pj.shtwfgs.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xb.colortex.cn

TS:   s.replaceAll("a", "b")
来源：http://xg.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ou.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rw.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lv.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://py.521024.cn

[E07] 按分隔符拆分
来源：http://eq.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vf.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ve.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bs.nicolike.cn

TS:   s.split(",")
来源：http://tz.shtwfgs.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sf.yuexingan06.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nv.gzmigu.cn

Ruby: s.split(",");  s.split
来源：http://al.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bb.shxzskj.cn

[E08] 数组按分隔符合并
来源：http://jj.chemitech.net.cn

Py:   ",".join(items)
来源：http://aj.nicolike.cn


<!-- 参考信息 -->