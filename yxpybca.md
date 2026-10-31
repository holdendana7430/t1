代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://hp.bjjhwx.cn

TS:   [...a, ...b];
来源：http://ko.shxzskj.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ne.chemitech.net.cn

Go:   append(a, b...)
来源：http://rw.muxihuayi.cn

Ruby: a + b;  a.concat(b)
来源：http://ig.gzmigu.cn

C#:   a.Concat(b).ToList()
来源：http://dx.panjiajie.cn

[D09] 排序（升序）
来源：http://id.panjiajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://dh.szsharing.cn

PHP:  sort($arr);
来源：http://pu.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qt.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ww.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ag.bjjhwx.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bj.jianghongdianzi.cn

Ruby: arr.sort
来源：http://sm.bookmarksfly.cn

C#:   list.Sort();
来源：http://ba.shxzukj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ht.chemitech.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hi.wgjwhj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ll.szsharing.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://rr.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://be.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qq.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cf.shxzskj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mo.haigaiapp.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://az.newstarts.cn

[D11] 反转数组
来源：http://rk.asd995.cn

Py:   arr[::-1];  arr.reverse()
来源：http://zd.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://yf.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fw.yuntaijiaju.cn

TS:   [...arr].reverse();
来源：http://gl.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://yj.colortex.cn

Go:   slices.Reverse(arr)
来源：http://az.haigaiapp.cn

Ruby: arr.reverse
来源：http://ut.newstarts.cn

C#:   list.Reverse();
来源：http://tj.huanxung.cn

[D12] 查找元素下标
来源：http://sc.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://rg.panjiajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xb.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ah.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vj.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ad.muxihuayi.cn

Go:   slices.Index(arr, x)
来源：http://io.521024.cn

Ruby: arr.index(x)
来源：http://tg.shxzskj.cn

C#:   list.IndexOf(x);
来源：http://jf.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://ky.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://rd.yuexingan06.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wu.9csxet.cn

JS:   arr.filter(x => x > 3)
来源：http://kt.yuntaijiaju.cn

TS:   arr.filter(x => x > 3)
来源：http://xk.huixinmuqiang.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://on.szxytkj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://be.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xd.newstarts.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ho.shxzukj.cn

[D14] 映射转换（每个元素变形）
来源：http://vl.shtwfgs.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qx.szxytkj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zb.hnjuh.cn

JS:   arr.map(x => x * 2)
来源：http://ku.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://ng.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kn.jctech888.com.cn

Go:   // 手写循环
来源：http://wh.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://di.huanxung.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zr.bookmarksfly.cn

[D15] 去重
来源：http://ic.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wy.9csxet.cn

PHP:  array_unique($arr);
来源：http://zv.huixiangedu.cn

JS:   [...new Set(arr)]
来源：http://ua.wgjwhj.cn

TS:   [...new Set(arr)]
来源：http://av.gzmigu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://og.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bl.hnjuh.cn

Ruby: arr.uniq
来源：http://ci.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://bb.bookmarksfly.cn

[D16] 求和与平均值
来源：http://tx.chemitech.net.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gq.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ka.jianghongdianzi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zk.newstarts.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://dd.chemitech.net.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ty.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://js.shtwfgs.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wq.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://ab.szsharing.cn

[D17] 最大值与最小值
来源：http://rh.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://pc.szxytkj.cn

PHP:  max($arr);  min($arr);
来源：http://hl.huixiangedu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://zj.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://up.nszjky.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://td.huixiangedu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gz.panjiajie.cn

Ruby: arr.max;  arr.min
来源：http://hh.nszjky.cn

C#:   list.Max();  list.Min()
来源：http://rl.shxzukj.cn

[D18] 扁平化嵌套数组
来源：http://nv.bjjhwx.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://eh.newstarts.cn

PHP:  array_merge(...$nested);
来源：http://ht.jianghongdianzi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fg.colortex.cn

TS:   nested.flat();
来源：http://wb.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fk.bookmarksfly.cn

Go:   // 手写双层循环
来源：http://ch.asd995.cn

Ruby: nested.flatten
来源：http://fc.yuntaijiaju.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://cf.yuntaijiaju.cn

[D19] 按字段分组
来源：http://am.9csxet.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mg.szsharing.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zm.shxzukj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://cg.newstarts.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jt.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ut.haigaiapp.cn

Go:   // 手写 map[string][]T
来源：http://qc.bookmarksfly.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fh.shxzukj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qc.asd995.cn

[D20] 统计每个元素出现次数
来源：http://qv.hnjuh.cn

Py:   Counter(arr)
来源：http://ex.jctech888.com.cn

PHP:  array_count_values($arr);
来源：http://zq.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fv.9csxet.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ts.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zd.nszjky.cn

Go:   // 手写 map[T]int
来源：http://si.szsharing.cn

Ruby: arr.tally
来源：http://bf.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://su.bookmarksfly.cn

[D21] 判断是否包含某元素
来源：http://dx.shxzskj.cn

Py:   x in arr
来源：http://cz.hnjuh.cn

PHP:  in_array($x, $arr, true);
来源：http://hg.jianghongdianzi.cn

JS:   arr.includes(x)
来源：http://pv.nszjky.cn

TS:   arr.includes(x)
来源：http://sc.chemitech.net.cn

Java: list.contains(x)
来源：http://jw.yuexingan06.cn

Go:   slices.Contains(arr, x)
来源：http://fk.szsharing.cn

Ruby: arr.include?(x)
来源：http://ph.jianghongdianzi.cn

C#:   list.Contains(x)
来源：http://cx.hnjuh.cn

[D22] 复制数组（避免共享引用）
来源：http://se.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lc.nszjky.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://kg.yuexingan06.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ci.muxihuayi.cn

TS:   [...arr];
来源：http://up.newstarts.cn

Java: new ArrayList<>(list);
来源：http://sn.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://sm.jianghongdianzi.cn

Ruby: arr.dup;  arr.clone
来源：http://dv.muxihuayi.cn

C#:   new List<int>(list);
来源：http://tt.bookmarksfly.cn

[D23] reduce 累积计算
来源：http://xp.jctech888.com.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fo.huixiangedu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xw.muxihuayi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tc.szxytkj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vp.hnjuh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ue.huixiangedu.cn

Go:   // 手写循环
来源：http://bd.muxihuayi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ja.huixinmuqiang.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ne.shtwfgs.cn

[D24] 字典 / Map 基本操作
来源：http://dx.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ri.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wz.jctech888.com.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zj.shtwfgs.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ak.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://iw.nicolike.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yf.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jz.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ss.chemitech.net.cn

[D25] Set 集合去重与交并差
来源：http://dm.wgjwhj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://rv.muxihuayi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://eo.yuntaijiaju.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nk.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ak.lnxyls.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vd.nszjky.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ng.newstarts.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://au.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zr.szsharing.cn

[D26] 数组转字符串
来源：http://tl.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://zz.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://xt.shxzskj.cn

JS:   arr.join(", ")
来源：http://km.asd995.cn

TS:   arr.join(", ")
来源：http://ba.bookmarksfly.cn

Java: String.join(", ", list)
来源：http://wa.yuntaijiaju.cn

Go:   strings.Join(strs, ", ")
来源：http://dv.huixiangedu.cn

Ruby: arr.join(", ")
来源：http://ei.nszjky.cn

C#:   string.Join(", ", list)
来源：http://fr.9csxet.cn

================================================================================
来源：http://ya.bjjhwx.cn

E. 字符串处理
来源：http://oz.panjiajie.cn

================================================================================
来源：http://mt.szxytkj.cn

[E01] 拼接字符串
来源：http://lv.haigaiapp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://iy.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ko.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bf.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cp.hahajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://av.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ch.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qr.yuexingan06.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://so.nszjky.cn

[E02] 重复字符串
来源：http://kj.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://jp.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://cb.521024.cn

JS:   "ab".repeat(3)
来源：http://ex.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://eq.huanxung.cn

Java: "ab".repeat(3)
来源：http://fb.nicolike.cn

Go:   strings.Repeat("ab", 3)
来源：http://hd.bookmarksfly.cn

Ruby: "ab" * 3
来源：http://ty.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ew.muxihuayi.cn

[E03] 截取子串
来源：http://xm.huixinmuqiang.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://xr.hnjuh.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hs.asd995.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ou.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://zh.bookmarksfly.cn

Java: s.substring(1, 4)
来源：http://vt.panjiajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ia.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://of.haigaiapp.cn

C#:   s.Substring(1, 3)
来源：http://oj.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://et.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://tw.colortex.cn

PHP:  strpos($s, "x");
来源：http://hm.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kk.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://ie.muxihuayi.cn

Java: s.indexOf("x")
来源：http://yt.newstarts.cn

Go:   strings.Index(s, "x")
来源：http://dz.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://qj.haigaiapp.cn

C#:   s.IndexOf("x")
来源：http://jw.shxzskj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ep.szxytkj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ms.bjjhwx.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sh.gzmigu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fv.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jf.yuntaijiaju.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mr.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pn.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yc.shtwfgs.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yh.hahajie.cn

[E06] 替换子串
来源：http://in.shtwfgs.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xz.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://al.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rp.shxzskj.cn

TS:   s.replaceAll("a", "b")
来源：http://nd.shxzskj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nz.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uv.szxytkj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fp.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://kq.shxzskj.cn

[E07] 按分隔符拆分
来源：http://ae.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ew.shtwfgs.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qw.bjjhwx.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mx.jianghongdianzi.cn

TS:   s.split(",")
来源：http://up.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zv.newstarts.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mz.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://fq.lnxyls.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://th.szsharing.cn

[E08] 数组按分隔符合并
来源：http://sv.asd995.cn

Py:   ",".join(items)
来源：http://qk.hahajie.cn

PHP:  implode(",", $items);
来源：http://mq.huixinmuqiang.cn

JS:   items.join(",")
来源：http://ar.nszjky.cn

TS:   items.join(",")
来源：http://xv.hahajie.cn

Java: String.join(",", items)
来源：http://rm.gzmigu.cn

Go:   strings.Join(items, ",")
来源：http://qh.bjjhwx.cn

Ruby: items.join(",")
来源：http://oz.wgjwhj.cn

C#:   string.Join(",", items)
来源：http://rv.hahajie.cn

[E09] 去除所有空白字符
来源：http://we.nszjky.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lj.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kc.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://ll.muxihuayi.cn

TS:   s.replace(/\s+/g, "")
来源：http://dz.chemitech.net.cn

Java: s.replaceAll("\\s+", "")
来源：http://he.szxytkj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vp.bookmarksfly.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vh.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lk.szxytkj.cn

[E10] 左侧补零 / 定长填充
来源：http://wi.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hx.szsharing.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://tx.hnjuh.cn

JS:   "7".padStart(3, "0")
来源：http://zl.nszjky.cn

TS:   "7".padStart(3, "0")
来源：http://ua.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://ni.lnxyls.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vn.jctech888.com.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gc.huanxung.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gy.bookmarksfly.cn

[E11] 反转字符串
来源：http://ql.bookmarksfly.cn

Py:   s[::-1]
来源：http://ji.panjiajie.cn

PHP:  strrev($s);
来源：http://di.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://we.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://zl.huixiangedu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ux.gzmigu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zo.9csxet.cn

Ruby: s.reverse
来源：http://yx.newstarts.cn

C#:   new string(s.Reverse().ToArray())
来源：http://uf.nszjky.cn

[E12] 统计某字符出现次数
来源：http://xn.panjiajie.cn

Py:   s.count("a")
来源：http://uk.nicolike.cn

PHP:  substr_count($s, "a");
来源：http://di.nszjky.cn

JS:   s.split("a").length - 1
来源：http://uo.jianghongdianzi.cn

TS:   s.split("a").length - 1
来源：http://hv.nszjky.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gc.huixinmuqiang.cn

Go:   strings.Count(s, "a")
来源：http://jz.lnxyls.cn

Ruby: s.count("a")
来源：http://wf.newstarts.cn

C#:   s.Count(c => c == 'a')
来源：http://jh.bjjhwx.cn

[E13] 逐字符遍历
来源：http://rr.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://cj.haigaiapp.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kn.szsharing.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://wj.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sr.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://va.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gw.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://lq.haigaiapp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gv.panjiajie.cn

[E14] URL 编码与 Base64
来源：http://ep.bjjhwx.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zj.wgjwhj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rw.bookmarksfly.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xd.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ya.huixiangedu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gx.muxihuayi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://qv.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sj.nicolike.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hq.colortex.cn

[E15] HTML 转义 / 反转义
来源：http://cc.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dx.hahajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ft.shxzskj.cn


<!-- 参考信息 -->