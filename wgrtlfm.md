代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cr.szxytkj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://op.521024.cn

[D05] 访问与修改元素
来源：http://uy.colortex.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yz.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://eh.521024.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kf.huixinmuqiang.cn

TS:   arr[0]; arr.at(-1);
来源：http://ov.haigaiapp.cn

Java: list.get(0); list.set(0, 9);
来源：http://ob.gzmigu.cn

Go:   arr[0]; arr[0] = 9
来源：http://nt.szsharing.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mv.hahajie.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://br.hahajie.cn

[D06] 数组长度
来源：http://hr.nszjky.cn

Py:   len(arr)
来源：http://qm.shxzskj.cn

PHP:  count($arr);
来源：http://jc.huixinmuqiang.cn

JS:   arr.length
来源：http://nl.hahajie.cn

TS:   arr.length
来源：http://za.521024.cn

Java: list.size();
来源：http://tz.lnxyls.cn

Go:   len(arr)
来源：http://yt.newstarts.cn

Ruby: arr.length; arr.size
来源：http://pb.panjiajie.cn

C#:   list.Count;
来源：http://um.hahajie.cn

[D07] 切片 / 取子数组
来源：http://fc.szsharing.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ig.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://yf.gzmigu.cn

JS:   arr.slice(1, 4);
来源：http://oj.panjiajie.cn

TS:   arr.slice(1, 4);
来源：http://qd.jctech888.com.cn

Java: list.subList(1, 4);
来源：http://vo.asd995.cn

Go:   arr[1:4]
来源：http://cd.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://pn.hahajie.cn

C#:   list.GetRange(1, 3);
来源：http://wa.gzmigu.cn

[D08] 合并两个数组
来源：http://mw.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://fo.shxzskj.cn

PHP:  array_merge($a, $b);
来源：http://fl.gzmigu.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ac.huixinmuqiang.cn

TS:   [...a, ...b];
来源：http://he.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://do.asd995.cn

Go:   append(a, b...)
来源：http://nu.shxzskj.cn

Ruby: a + b;  a.concat(b)
来源：http://ss.chemitech.net.cn

C#:   a.Concat(b).ToList()
来源：http://ra.haigaiapp.cn

[D09] 排序（升序）
来源：http://qh.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://zm.newstarts.cn

PHP:  sort($arr);
来源：http://cj.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://yi.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lv.szxytkj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://fg.bjjhwx.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://xl.nicolike.cn

Ruby: arr.sort
来源：http://hc.huanxung.cn

C#:   list.Sort();
来源：http://pb.9csxet.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://it.szxytkj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://di.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://oa.chemitech.net.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yu.panjiajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bk.yuntaijiaju.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://xv.bookmarksfly.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uq.huixiangedu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zb.huixiangedu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wt.yuntaijiaju.cn

[D11] 反转数组
来源：http://yz.9csxet.cn

Py:   arr[::-1];  arr.reverse()
来源：http://fp.521024.cn

PHP:  array_reverse($arr);
来源：http://if.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fx.colortex.cn

TS:   [...arr].reverse();
来源：http://vv.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://ab.hnjuh.cn

Go:   slices.Reverse(arr)
来源：http://uw.yuexingan06.cn

Ruby: arr.reverse
来源：http://hv.bjjhwx.cn

C#:   list.Reverse();
来源：http://jv.jianghongdianzi.cn

[D12] 查找元素下标
来源：http://ha.huixinmuqiang.cn

Py:   arr.index(x);  x in arr
来源：http://zg.asd995.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://zz.szxytkj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qi.wgjwhj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://at.newstarts.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yq.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://ud.shtwfgs.cn

Ruby: arr.index(x)
来源：http://ru.shtwfgs.cn

C#:   list.IndexOf(x);
来源：http://ex.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://ng.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fl.lnxyls.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://lq.muxihuayi.cn

JS:   arr.filter(x => x > 3)
来源：http://oe.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://ah.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ko.shxzukj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gc.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://av.nicolike.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yr.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://hp.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ef.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://cv.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://lp.nszjky.cn

TS:   arr.map(x => x * 2)
来源：http://sf.gzmigu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://by.nszjky.cn

Go:   // 手写循环
来源：http://hx.muxihuayi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://aq.newstarts.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hp.gzmigu.cn

[D15] 去重
来源：http://wt.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fy.huixiangedu.cn

PHP:  array_unique($arr);
来源：http://qd.panjiajie.cn

JS:   [...new Set(arr)]
来源：http://vu.9csxet.cn

TS:   [...new Set(arr)]
来源：http://dg.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://eo.huanxung.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ug.521024.cn

Ruby: arr.uniq
来源：http://gu.shtwfgs.cn

C#:   list.Distinct().ToList()
来源：http://ds.9csxet.cn

[D16] 求和与平均值
来源：http://pk.asd995.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ue.shtwfgs.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vx.muxihuayi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cn.9csxet.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ri.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bz.shxzukj.cn

Go:   // 手写循环累加
来源：http://ub.shxzskj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://aa.muxihuayi.cn

C#:   list.Sum();  list.Average()
来源：http://xy.hnjuh.cn

[D17] 最大值与最小值
来源：http://kv.huixinmuqiang.cn

Py:   max(arr);  min(arr)
来源：http://xo.bjjhwx.cn

PHP:  max($arr);  min($arr);
来源：http://zq.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fp.bookmarksfly.cn

TS:   Math.max(...arr);
来源：http://ni.szxytkj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://qd.bookmarksfly.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://bp.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://oe.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://fn.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://fy.asd995.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://lx.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://lt.yuexingan06.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://kf.gzmigu.cn

TS:   nested.flat();
来源：http://vp.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yo.gzmigu.cn

Go:   // 手写双层循环
来源：http://zy.9csxet.cn

Ruby: nested.flatten
来源：http://mk.huixiangedu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://dx.jctech888.com.cn

[D19] 按字段分组
来源：http://ek.szxytkj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sr.panjiajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vb.9csxet.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mo.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://le.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://yp.shtwfgs.cn

Go:   // 手写 map[string][]T
来源：http://zu.gzmigu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hn.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ch.nszjky.cn

[D20] 统计每个元素出现次数
来源：http://gj.nszjky.cn

Py:   Counter(arr)
来源：http://gs.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://ul.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sj.yuexingan06.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://rs.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mi.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://jm.shtwfgs.cn

Ruby: arr.tally
来源：http://dn.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qm.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://cd.asd995.cn

Py:   x in arr
来源：http://xg.nicolike.cn

PHP:  in_array($x, $arr, true);
来源：http://uw.jctech888.com.cn

JS:   arr.includes(x)
来源：http://de.huixiangedu.cn

TS:   arr.includes(x)
来源：http://nw.jctech888.com.cn

Java: list.contains(x)
来源：http://qr.521024.cn

Go:   slices.Contains(arr, x)
来源：http://yx.9csxet.cn

Ruby: arr.include?(x)
来源：http://fd.szsharing.cn

C#:   list.Contains(x)
来源：http://xe.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://gp.newstarts.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mv.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mx.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mf.yuntaijiaju.cn

TS:   [...arr];
来源：http://jh.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://id.muxihuayi.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ll.wgjwhj.cn

Ruby: arr.dup;  arr.clone
来源：http://jj.shxzskj.cn

C#:   new List<int>(list);
来源：http://ix.9csxet.cn

[D23] reduce 累积计算
来源：http://la.hahajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yg.shxzukj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ai.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cw.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mb.muxihuayi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://dc.shxzukj.cn

Go:   // 手写循环
来源：http://gw.yuexingan06.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ve.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ao.jianghongdianzi.cn

[D24] 字典 / Map 基本操作
来源：http://ej.colortex.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pk.shxzskj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://db.haigaiapp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://va.yuntaijiaju.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zd.huixinmuqiang.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ua.huanxung.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yl.colortex.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tu.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://en.jctech888.com.cn

[D25] Set 集合去重与交并差
来源：http://hs.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pr.yuntaijiaju.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zn.9csxet.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vn.szsharing.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ej.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://il.521024.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lm.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ox.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://un.wgjwhj.cn

[D26] 数组转字符串
来源：http://dr.521024.cn

Py:   ", ".join(map(str, arr))
来源：http://lm.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://hu.yuexingan06.cn

JS:   arr.join(", ")
来源：http://mh.szsharing.cn

TS:   arr.join(", ")
来源：http://hi.521024.cn

Java: String.join(", ", list)
来源：http://qb.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://is.nicolike.cn

Ruby: arr.join(", ")
来源：http://ma.lnxyls.cn

C#:   string.Join(", ", list)
来源：http://ob.huixiangedu.cn

================================================================================
来源：http://no.shtwfgs.cn

E. 字符串处理
来源：http://yb.huixiangedu.cn

================================================================================
来源：http://xd.nicolike.cn

[E01] 拼接字符串
来源：http://rb.shxzskj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eu.szxytkj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wz.chemitech.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lj.lnxyls.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zk.yuexingan06.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cu.chemitech.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kk.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rb.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sw.newstarts.cn

[E02] 重复字符串
来源：http://vn.huixiangedu.cn

Py:   "ab" * 3
来源：http://nt.lnxyls.cn

PHP:  str_repeat("ab", 3);
来源：http://ki.hahajie.cn

JS:   "ab".repeat(3)
来源：http://sv.huanxung.cn

TS:   "ab".repeat(3)
来源：http://nh.panjiajie.cn

Java: "ab".repeat(3)
来源：http://tu.asd995.cn

Go:   strings.Repeat("ab", 3)
来源：http://gq.nszjky.cn

Ruby: "ab" * 3
来源：http://gq.wgjwhj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://js.521024.cn

[E03] 截取子串
来源：http://sp.haigaiapp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://dg.bookmarksfly.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ek.bjjhwx.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://qa.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://lt.9csxet.cn

Java: s.substring(1, 4)
来源：http://eq.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://po.9csxet.cn

Ruby: s[1, 3];  s[1..3]
来源：http://wu.haigaiapp.cn

C#:   s.Substring(1, 3)
来源：http://dp.asd995.cn

[E04] 查找子串位置
来源：http://wr.huanxung.cn

Py:   s.find("x");  s.index("x")
来源：http://yo.9csxet.cn

PHP:  strpos($s, "x");
来源：http://zz.chemitech.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://os.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://yh.nszjky.cn

Java: s.indexOf("x")
来源：http://ld.jianghongdianzi.cn

Go:   strings.Index(s, "x")
来源：http://tl.9csxet.cn

Ruby: s.index("x")
来源：http://mh.asd995.cn

C#:   s.IndexOf("x")
来源：http://ny.nszjky.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://dz.szsharing.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bb.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ar.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qp.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cn.hnjuh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hu.nicolike.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vj.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tq.hnjuh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wr.szsharing.cn

[E06] 替换子串
来源：http://id.chemitech.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://km.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://ys.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cg.huixiangedu.cn

TS:   s.replaceAll("a", "b")
来源：http://to.yuexingan06.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://os.lnxyls.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yp.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mi.shtwfgs.cn

C#:   s.Replace("a", "b")
来源：http://la.wgjwhj.cn

[E07] 按分隔符拆分
来源：http://fj.huixinmuqiang.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://du.colortex.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://id.szsharing.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mb.panjiajie.cn

TS:   s.split(",")
来源：http://ta.shxzskj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qf.jianghongdianzi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ev.muxihuayi.cn

Ruby: s.split(",");  s.split
来源：http://mi.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mk.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://ml.huanxung.cn

Py:   ",".join(items)
来源：http://dx.wgjwhj.cn

PHP:  implode(",", $items);
来源：http://en.panjiajie.cn

JS:   items.join(",")
来源：http://cd.shxzukj.cn

TS:   items.join(",")
来源：http://jq.bookmarksfly.cn

Java: String.join(",", items)
来源：http://bh.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://xd.shxzskj.cn

Ruby: items.join(",")
来源：http://tk.colortex.cn

C#:   string.Join(",", items)
来源：http://dg.panjiajie.cn

[E09] 去除所有空白字符
来源：http://qb.muxihuayi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nh.nicolike.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jt.jianghongdianzi.cn

JS:   s.replace(/\s+/g, "")
来源：http://uj.jianghongdianzi.cn

TS:   s.replace(/\s+/g, "")
来源：http://dz.haigaiapp.cn

Java: s.replaceAll("\\s+", "")
来源：http://sa.wgjwhj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ps.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pp.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ek.bookmarksfly.cn

[E10] 左侧补零 / 定长填充
来源：http://pu.shtwfgs.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ij.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yn.9csxet.cn

JS:   "7".padStart(3, "0")
来源：http://pf.gzmigu.cn

TS:   "7".padStart(3, "0")
来源：http://lz.bjjhwx.cn

Java: String.format("%03d", 7)
来源：http://ci.newstarts.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nu.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yg.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ql.newstarts.cn

[E11] 反转字符串
来源：http://nq.huixinmuqiang.cn

Py:   s[::-1]
来源：http://ar.muxihuayi.cn

PHP:  strrev($s);
来源：http://hq.9csxet.cn

JS:   [...s].reverse().join("")
来源：http://pa.bjjhwx.cn

TS:   [...s].reverse().join("")
来源：http://on.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qz.hnjuh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://iq.newstarts.cn


<!-- 参考信息 -->