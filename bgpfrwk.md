代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://gp.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fk.yuexingan06.cn

TS:   arr[0]; arr.at(-1);
来源：http://em.lnxyls.cn

Java: list.get(0); list.set(0, 9);
来源：http://wn.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://to.bookmarksfly.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://de.9csxet.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://pl.bjjhwx.cn

[D06] 数组长度
来源：http://es.huixinmuqiang.cn

Py:   len(arr)
来源：http://hi.shxzukj.cn

PHP:  count($arr);
来源：http://iz.lnxyls.cn

JS:   arr.length
来源：http://ov.shxzskj.cn

TS:   arr.length
来源：http://un.yuntaijiaju.cn

Java: list.size();
来源：http://ji.521024.cn

Go:   len(arr)
来源：http://sc.asd995.cn

Ruby: arr.length; arr.size
来源：http://zz.jctech888.com.cn

C#:   list.Count;
来源：http://on.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://jn.hnjuh.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ak.lnxyls.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cg.shtwfgs.cn

JS:   arr.slice(1, 4);
来源：http://tu.szxytkj.cn

TS:   arr.slice(1, 4);
来源：http://sc.panjiajie.cn

Java: list.subList(1, 4);
来源：http://nn.gzmigu.cn

Go:   arr[1:4]
来源：http://yt.hnjuh.cn

Ruby: arr[1, 3]
来源：http://jw.bookmarksfly.cn

C#:   list.GetRange(1, 3);
来源：http://sx.wgjwhj.cn

[D08] 合并两个数组
来源：http://tj.haigaiapp.cn

Py:   a + b;  a.extend(b)
来源：http://wv.lnxyls.cn

PHP:  array_merge($a, $b);
来源：http://qs.lnxyls.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://jd.hnjuh.cn

TS:   [...a, ...b];
来源：http://xw.wgjwhj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ac.yuntaijiaju.cn

Go:   append(a, b...)
来源：http://nw.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://mt.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://xk.lnxyls.cn

[D09] 排序（升序）
来源：http://ju.szxytkj.cn

Py:   sorted(arr);  arr.sort()
来源：http://pm.szxytkj.cn

PHP:  sort($arr);
来源：http://dl.huixiangedu.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cc.shxzukj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fy.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://iu.szsharing.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://rm.yuexingan06.cn

Ruby: arr.sort
来源：http://xl.jctech888.com.cn

C#:   list.Sort();
来源：http://er.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kd.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yi.newstarts.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mn.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zn.huanxung.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ff.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sh.lnxyls.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://og.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://js.gzmigu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bj.huanxung.cn

[D11] 反转数组
来源：http://zd.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ja.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://fw.shxzukj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://il.nszjky.cn

TS:   [...arr].reverse();
来源：http://wi.hahajie.cn

Java: Collections.reverse(list);
来源：http://zm.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://wq.nicolike.cn

Ruby: arr.reverse
来源：http://ol.shxzskj.cn

C#:   list.Reverse();
来源：http://oh.haigaiapp.cn

[D12] 查找元素下标
来源：http://dl.shxzukj.cn

Py:   arr.index(x);  x in arr
来源：http://yi.shxzskj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lu.jianghongdianzi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://re.szsharing.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://kq.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wn.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://ft.hahajie.cn

Ruby: arr.index(x)
来源：http://uk.9csxet.cn

C#:   list.IndexOf(x);
来源：http://te.huanxung.cn

[D13] 过滤（保留满足条件的）
来源：http://sl.panjiajie.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ls.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://gf.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://bc.lnxyls.cn

TS:   arr.filter(x => x > 3)
来源：http://xk.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ha.gzmigu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zv.hahajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://gm.hahajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fs.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://ih.hnjuh.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ww.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wr.bookmarksfly.cn

JS:   arr.map(x => x * 2)
来源：http://ln.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://jl.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://qy.jianghongdianzi.cn

Go:   // 手写循环
来源：http://ja.lnxyls.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lv.jianghongdianzi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://nn.shtwfgs.cn

[D15] 去重
来源：http://tk.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ve.haigaiapp.cn

PHP:  array_unique($arr);
来源：http://ek.hahajie.cn

JS:   [...new Set(arr)]
来源：http://wu.jctech888.com.cn

TS:   [...new Set(arr)]
来源：http://za.yuntaijiaju.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rv.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lc.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://es.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://xg.521024.cn

[D16] 求和与平均值
来源：http://fm.yuntaijiaju.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hu.shxzukj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://nm.szxytkj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://al.szsharing.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xw.bjjhwx.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nu.shtwfgs.cn

Go:   // 手写循环累加
来源：http://dx.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ws.hnjuh.cn

C#:   list.Sum();  list.Average()
来源：http://av.gzmigu.cn

[D17] 最大值与最小值
来源：http://cn.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://om.yuexingan06.cn

PHP:  max($arr);  min($arr);
来源：http://ty.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mu.huanxung.cn

TS:   Math.max(...arr);
来源：http://ki.lnxyls.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nd.hnjuh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jr.yuexingan06.cn

Ruby: arr.max;  arr.min
来源：http://nd.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://ci.panjiajie.cn

[D18] 扁平化嵌套数组
来源：http://ab.hahajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sn.hnjuh.cn

PHP:  array_merge(...$nested);
来源：http://zt.jianghongdianzi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mw.jianghongdianzi.cn

TS:   nested.flat();
来源：http://ey.wgjwhj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fo.haigaiapp.cn

Go:   // 手写双层循环
来源：http://oc.shxzukj.cn

Ruby: nested.flatten
来源：http://bl.bjjhwx.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://td.jianghongdianzi.cn

[D19] 按字段分组
来源：http://ig.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ny.nszjky.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pf.muxihuayi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lj.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://wh.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wn.shxzskj.cn

Go:   // 手写 map[string][]T
来源：http://or.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ej.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://re.asd995.cn

[D20] 统计每个元素出现次数
来源：http://sn.nicolike.cn

Py:   Counter(arr)
来源：http://da.huanxung.cn

PHP:  array_count_values($arr);
来源：http://gb.9csxet.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ul.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xv.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rf.colortex.cn

Go:   // 手写 map[T]int
来源：http://rz.9csxet.cn

Ruby: arr.tally
来源：http://xs.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xf.wgjwhj.cn

[D21] 判断是否包含某元素
来源：http://sd.huixinmuqiang.cn

Py:   x in arr
来源：http://hr.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://bs.haigaiapp.cn

JS:   arr.includes(x)
来源：http://bj.bookmarksfly.cn

TS:   arr.includes(x)
来源：http://ny.yuntaijiaju.cn

Java: list.contains(x)
来源：http://xr.huixinmuqiang.cn

Go:   slices.Contains(arr, x)
来源：http://ft.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://bb.yuexingan06.cn

C#:   list.Contains(x)
来源：http://zs.gzmigu.cn

[D22] 复制数组（避免共享引用）
来源：http://fy.shtwfgs.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nm.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hh.9csxet.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sx.9csxet.cn

TS:   [...arr];
来源：http://fu.hahajie.cn

Java: new ArrayList<>(list);
来源：http://nn.hnjuh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lj.chemitech.net.cn

Ruby: arr.dup;  arr.clone
来源：http://iw.521024.cn

C#:   new List<int>(list);
来源：http://id.shtwfgs.cn

[D23] reduce 累积计算
来源：http://mx.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://by.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nz.nicolike.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hc.gzmigu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tn.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://hc.newstarts.cn

Go:   // 手写循环
来源：http://bl.chemitech.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ze.huanxung.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://sa.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://ph.huixinmuqiang.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hs.nszjky.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oy.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://km.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://zm.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vn.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ja.hahajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nl.huanxung.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qd.chemitech.net.cn

[D25] Set 集合去重与交并差
来源：http://zo.colortex.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ub.huanxung.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://if.huixinmuqiang.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dl.newstarts.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dx.huixinmuqiang.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pb.huanxung.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vi.nicolike.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gc.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qd.hnjuh.cn

[D26] 数组转字符串
来源：http://bp.huixinmuqiang.cn

Py:   ", ".join(map(str, arr))
来源：http://hq.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://ya.lnxyls.cn

JS:   arr.join(", ")
来源：http://up.huanxung.cn

TS:   arr.join(", ")
来源：http://ri.nszjky.cn

Java: String.join(", ", list)
来源：http://dk.lnxyls.cn

Go:   strings.Join(strs, ", ")
来源：http://wp.jianghongdianzi.cn

Ruby: arr.join(", ")
来源：http://cn.9csxet.cn

C#:   string.Join(", ", list)
来源：http://sa.huixinmuqiang.cn

================================================================================
来源：http://ms.asd995.cn

E. 字符串处理
来源：http://ie.panjiajie.cn

================================================================================
来源：http://vy.9csxet.cn

[E01] 拼接字符串
来源：http://wm.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bp.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cr.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://op.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jx.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jv.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://qj.jianghongdianzi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jx.colortex.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ji.chemitech.net.cn

[E02] 重复字符串
来源：http://qv.asd995.cn

Py:   "ab" * 3
来源：http://rw.haigaiapp.cn

PHP:  str_repeat("ab", 3);
来源：http://wb.chemitech.net.cn

JS:   "ab".repeat(3)
来源：http://qm.jianghongdianzi.cn

TS:   "ab".repeat(3)
来源：http://vl.hahajie.cn

Java: "ab".repeat(3)
来源：http://li.hahajie.cn

Go:   strings.Repeat("ab", 3)
来源：http://nz.huixiangedu.cn

Ruby: "ab" * 3
来源：http://yt.yuntaijiaju.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://af.wgjwhj.cn

[E03] 截取子串
来源：http://zp.haigaiapp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nl.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://jh.9csxet.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hg.huanxung.cn

TS:   s.slice(1, 4)
来源：http://ht.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://dl.haigaiapp.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ol.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vz.huanxung.cn

C#:   s.Substring(1, 3)
来源：http://kc.shtwfgs.cn

[E04] 查找子串位置
来源：http://gm.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://nf.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://it.nszjky.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fk.nszjky.cn

TS:   s.indexOf("x")
来源：http://im.newstarts.cn

Java: s.indexOf("x")
来源：http://iy.yuexingan06.cn

Go:   strings.Index(s, "x")
来源：http://cx.huixinmuqiang.cn

Ruby: s.index("x")
来源：http://hz.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://xz.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ki.bjjhwx.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ux.bookmarksfly.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://za.yuntaijiaju.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pp.szxytkj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sh.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vb.bookmarksfly.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gq.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://dt.jianghongdianzi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mu.huanxung.cn

[E06] 替换子串
来源：http://kn.haigaiapp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ga.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://qr.shxzukj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hl.panjiajie.cn

TS:   s.replaceAll("a", "b")
来源：http://cr.szsharing.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xl.huixinmuqiang.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sv.huanxung.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wc.huanxung.cn

C#:   s.Replace("a", "b")
来源：http://za.newstarts.cn

[E07] 按分隔符拆分
来源：http://fq.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ef.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tr.newstarts.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://vu.bjjhwx.cn

TS:   s.split(",")
来源：http://nt.yuexingan06.cn

Java: s.split(",");  s.split("\\s+")
来源：http://by.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mq.hnjuh.cn

Ruby: s.split(",");  s.split
来源：http://jb.chemitech.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jp.szsharing.cn

[E08] 数组按分隔符合并
来源：http://oe.521024.cn

Py:   ",".join(items)
来源：http://of.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://uz.nicolike.cn

JS:   items.join(",")
来源：http://wk.shxzukj.cn

TS:   items.join(",")
来源：http://gh.bjjhwx.cn

Java: String.join(",", items)
来源：http://ww.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://sd.shxzskj.cn

Ruby: items.join(",")
来源：http://ti.hnjuh.cn

C#:   string.Join(",", items)
来源：http://jg.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://kv.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pw.9csxet.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zk.nszjky.cn

JS:   s.replace(/\s+/g, "")
来源：http://an.huixinmuqiang.cn

TS:   s.replace(/\s+/g, "")
来源：http://fu.szxytkj.cn

Java: s.replaceAll("\\s+", "")
来源：http://ac.muxihuayi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://lz.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kl.hnjuh.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oy.9csxet.cn

[E10] 左侧补零 / 定长填充
来源：http://es.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qt.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://cl.yuntaijiaju.cn

JS:   "7".padStart(3, "0")
来源：http://sj.huixinmuqiang.cn

TS:   "7".padStart(3, "0")
来源：http://ph.huanxung.cn

Java: String.format("%03d", 7)
来源：http://af.huixinmuqiang.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jw.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xc.521024.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qc.9csxet.cn

[E11] 反转字符串
来源：http://dr.huanxung.cn

Py:   s[::-1]
来源：http://rn.haigaiapp.cn

PHP:  strrev($s);
来源：http://yw.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://xc.huanxung.cn

TS:   [...s].reverse().join("")
来源：http://gk.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gm.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wo.haigaiapp.cn

Ruby: s.reverse
来源：http://pv.huixinmuqiang.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ld.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://yr.chemitech.net.cn

Py:   s.count("a")
来源：http://wn.hahajie.cn


<!-- 参考信息 -->