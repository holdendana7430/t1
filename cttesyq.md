代发 wailian999

Py:   len(arr)
来源：http://sv.chemitech.net.cn

PHP:  count($arr);
来源：http://te.haigaiapp.cn

JS:   arr.length
来源：http://yz.panjiajie.cn

TS:   arr.length
来源：http://fs.yuexingan06.cn

Java: list.size();
来源：http://hr.haigaiapp.cn

Go:   len(arr)
来源：http://fn.huanxung.cn

Ruby: arr.length; arr.size
来源：http://ye.huixinmuqiang.cn

C#:   list.Count;
来源：http://ua.nicolike.cn

[D07] 切片 / 取子数组
来源：http://qw.panjiajie.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yj.huixiangedu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://cz.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://sd.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://zy.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://bh.huanxung.cn

Go:   arr[1:4]
来源：http://gy.shxzukj.cn

Ruby: arr[1, 3]
来源：http://gh.haigaiapp.cn

C#:   list.GetRange(1, 3);
来源：http://oh.colortex.cn

[D08] 合并两个数组
来源：http://vg.yuexingan06.cn

Py:   a + b;  a.extend(b)
来源：http://kc.panjiajie.cn

PHP:  array_merge($a, $b);
来源：http://px.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://fp.colortex.cn

TS:   [...a, ...b];
来源：http://ka.asd995.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lb.bookmarksfly.cn

Go:   append(a, b...)
来源：http://qq.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://vx.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://kw.bjjhwx.cn

[D09] 排序（升序）
来源：http://ko.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://kt.shxzukj.cn

PHP:  sort($arr);
来源：http://vx.bookmarksfly.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qx.521024.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://hr.lnxyls.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qx.yuntaijiaju.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://tl.gzmigu.cn

Ruby: arr.sort
来源：http://vu.nszjky.cn

C#:   list.Sort();
来源：http://rp.bjjhwx.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://cg.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fc.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://go.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zc.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hs.jianghongdianzi.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ag.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ui.newstarts.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://un.521024.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://rn.9csxet.cn

[D11] 反转数组
来源：http://sb.huixinmuqiang.cn

Py:   arr[::-1];  arr.reverse()
来源：http://nd.asd995.cn

PHP:  array_reverse($arr);
来源：http://ng.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://bt.nszjky.cn

TS:   [...arr].reverse();
来源：http://ny.newstarts.cn

Java: Collections.reverse(list);
来源：http://st.shtwfgs.cn

Go:   slices.Reverse(arr)
来源：http://qr.wgjwhj.cn

Ruby: arr.reverse
来源：http://vq.muxihuayi.cn

C#:   list.Reverse();
来源：http://uh.yuexingan06.cn

[D12] 查找元素下标
来源：http://pc.jianghongdianzi.cn

Py:   arr.index(x);  x in arr
来源：http://qf.muxihuayi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ag.jianghongdianzi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://if.haigaiapp.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pz.wgjwhj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gn.newstarts.cn

Go:   slices.Index(arr, x)
来源：http://hb.lnxyls.cn

Ruby: arr.index(x)
来源：http://uk.muxihuayi.cn

C#:   list.IndexOf(x);
来源：http://hj.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://xp.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://en.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://sv.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://jz.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://de.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ep.chemitech.net.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://af.shxzskj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vf.colortex.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://kk.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://hd.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://eo.wgjwhj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bi.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://zc.hahajie.cn

TS:   arr.map(x => x * 2)
来源：http://kv.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cs.muxihuayi.cn

Go:   // 手写循环
来源：http://vv.9csxet.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gm.wgjwhj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://uz.nicolike.cn

[D15] 去重
来源：http://je.szxytkj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jj.huanxung.cn

PHP:  array_unique($arr);
来源：http://bc.gzmigu.cn

JS:   [...new Set(arr)]
来源：http://sd.521024.cn

TS:   [...new Set(arr)]
来源：http://kz.szsharing.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yb.lnxyls.cn

Go:   // 用 map[T]struct{} 手写
来源：http://yu.shtwfgs.cn

Ruby: arr.uniq
来源：http://vs.haigaiapp.cn

C#:   list.Distinct().ToList()
来源：http://mb.haigaiapp.cn

[D16] 求和与平均值
来源：http://pp.wgjwhj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hs.bookmarksfly.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://aw.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://od.bookmarksfly.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ro.newstarts.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://pl.szxytkj.cn

Go:   // 手写循环累加
来源：http://ph.muxihuayi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ni.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://gu.szsharing.cn

[D17] 最大值与最小值
来源：http://vj.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://jv.wgjwhj.cn

PHP:  max($arr);  min($arr);
来源：http://dl.chemitech.net.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://is.haigaiapp.cn

TS:   Math.max(...arr);
来源：http://il.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ht.lnxyls.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rv.hahajie.cn

Ruby: arr.max;  arr.min
来源：http://jy.shtwfgs.cn

C#:   list.Max();  list.Min()
来源：http://tu.bjjhwx.cn

[D18] 扁平化嵌套数组
来源：http://dk.colortex.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cf.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://zg.yuexingan06.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://lh.yuexingan06.cn

TS:   nested.flat();
来源：http://ol.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hf.chemitech.net.cn

Go:   // 手写双层循环
来源：http://qe.nicolike.cn

Ruby: nested.flatten
来源：http://dd.yuntaijiaju.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wp.shxzukj.cn

[D19] 按字段分组
来源：http://kd.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wh.newstarts.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://it.jctech888.com.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://sl.szxytkj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://xy.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://af.szsharing.cn

Go:   // 手写 map[string][]T
来源：http://ld.newstarts.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://hf.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pq.huixinmuqiang.cn

[D20] 统计每个元素出现次数
来源：http://yi.szxytkj.cn

Py:   Counter(arr)
来源：http://qc.panjiajie.cn

PHP:  array_count_values($arr);
来源：http://zf.chemitech.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mc.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://se.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ky.9csxet.cn

Go:   // 手写 map[T]int
来源：http://ko.szxytkj.cn

Ruby: arr.tally
来源：http://ar.wgjwhj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zn.lnxyls.cn

[D21] 判断是否包含某元素
来源：http://oj.hnjuh.cn

Py:   x in arr
来源：http://ef.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://cl.haigaiapp.cn

JS:   arr.includes(x)
来源：http://pj.hnjuh.cn

TS:   arr.includes(x)
来源：http://lb.521024.cn

Java: list.contains(x)
来源：http://gt.bookmarksfly.cn

Go:   slices.Contains(arr, x)
来源：http://vg.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://ee.nicolike.cn

C#:   list.Contains(x)
来源：http://yt.521024.cn

[D22] 复制数组（避免共享引用）
来源：http://rr.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://et.colortex.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fy.9csxet.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ls.yuntaijiaju.cn

TS:   [...arr];
来源：http://jn.jianghongdianzi.cn

Java: new ArrayList<>(list);
来源：http://fi.newstarts.cn

Go:   copied := append([]int(nil), arr...)
来源：http://vp.hahajie.cn

Ruby: arr.dup;  arr.clone
来源：http://rt.newstarts.cn

C#:   new List<int>(list);
来源：http://he.wgjwhj.cn

[D23] reduce 累积计算
来源：http://da.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://an.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://zl.newstarts.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://bz.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gn.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ss.asd995.cn

Go:   // 手写循环
来源：http://kl.chemitech.net.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://er.szsharing.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://al.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://ua.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ao.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jg.szsharing.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vp.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://we.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://om.nszjky.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://nd.shxzukj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bl.shxzukj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://js.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://dj.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zl.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://zt.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://sx.bjjhwx.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://je.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wj.hnjuh.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://cb.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://tz.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gb.szsharing.cn

[D26] 数组转字符串
来源：http://tb.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://dn.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://mv.shxzukj.cn

JS:   arr.join(", ")
来源：http://mm.gzmigu.cn

TS:   arr.join(", ")
来源：http://hv.bjjhwx.cn

Java: String.join(", ", list)
来源：http://hw.newstarts.cn

Go:   strings.Join(strs, ", ")
来源：http://xr.hahajie.cn

Ruby: arr.join(", ")
来源：http://mb.nszjky.cn

C#:   string.Join(", ", list)
来源：http://oj.huixiangedu.cn

================================================================================
来源：http://pc.521024.cn

E. 字符串处理
来源：http://tx.lnxyls.cn

================================================================================
来源：http://kk.jianghongdianzi.cn

[E01] 拼接字符串
来源：http://fz.gzmigu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qz.panjiajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://py.newstarts.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ri.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://nf.haigaiapp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xr.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://su.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ld.asd995.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://kv.bookmarksfly.cn

[E02] 重复字符串
来源：http://zx.shxzukj.cn

Py:   "ab" * 3
来源：http://uv.haigaiapp.cn

PHP:  str_repeat("ab", 3);
来源：http://bk.asd995.cn

JS:   "ab".repeat(3)
来源：http://kt.521024.cn

TS:   "ab".repeat(3)
来源：http://xd.shtwfgs.cn

Java: "ab".repeat(3)
来源：http://db.bookmarksfly.cn

Go:   strings.Repeat("ab", 3)
来源：http://uj.wgjwhj.cn

Ruby: "ab" * 3
来源：http://cd.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rn.newstarts.cn

[E03] 截取子串
来源：http://sa.hnjuh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nv.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vw.gzmigu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://eg.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://ay.huixinmuqiang.cn

Java: s.substring(1, 4)
来源：http://lv.9csxet.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wb.9csxet.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tz.wgjwhj.cn

C#:   s.Substring(1, 3)
来源：http://eg.gzmigu.cn

[E04] 查找子串位置
来源：http://uw.shxzskj.cn

Py:   s.find("x");  s.index("x")
来源：http://al.521024.cn

PHP:  strpos($s, "x");
来源：http://fo.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xz.hahajie.cn

TS:   s.indexOf("x")
来源：http://ni.yuexingan06.cn

Java: s.indexOf("x")
来源：http://az.szsharing.cn

Go:   strings.Index(s, "x")
来源：http://zj.huanxung.cn

Ruby: s.index("x")
来源：http://ge.gzmigu.cn

C#:   s.IndexOf("x")
来源：http://zs.huixiangedu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cc.nicolike.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ka.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ys.shxzukj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jy.gzmigu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://cv.nszjky.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fs.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ua.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kf.huixinmuqiang.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://eb.lnxyls.cn

[E06] 替换子串
来源：http://mu.haigaiapp.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ml.yuntaijiaju.cn

PHP:  str_replace("a", "b", $s);
来源：http://nx.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jb.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://sf.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wo.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sz.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ik.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://si.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://pt.yuntaijiaju.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fk.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hk.muxihuayi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://iv.haigaiapp.cn

TS:   s.split(",")
来源：http://hq.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qe.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ij.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://xp.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hp.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://fi.jianghongdianzi.cn

Py:   ",".join(items)
来源：http://kl.asd995.cn

PHP:  implode(",", $items);
来源：http://dc.newstarts.cn

JS:   items.join(",")
来源：http://xq.gzmigu.cn

TS:   items.join(",")
来源：http://sb.hnjuh.cn

Java: String.join(",", items)
来源：http://ep.gzmigu.cn

Go:   strings.Join(items, ",")
来源：http://wz.gzmigu.cn

Ruby: items.join(",")
来源：http://qz.huanxung.cn

C#:   string.Join(",", items)
来源：http://wy.bookmarksfly.cn

[E09] 去除所有空白字符
来源：http://ff.haigaiapp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sk.hnjuh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uz.panjiajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://kk.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://ci.shxzskj.cn

Java: s.replaceAll("\\s+", "")
来源：http://wb.521024.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://at.521024.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rb.colortex.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fg.newstarts.cn

[E10] 左侧补零 / 定长填充
来源：http://id.bjjhwx.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gk.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zd.jianghongdianzi.cn

JS:   "7".padStart(3, "0")
来源：http://eo.szsharing.cn

TS:   "7".padStart(3, "0")
来源：http://qu.lnxyls.cn

Java: String.format("%03d", 7)
来源：http://sa.huanxung.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tg.jianghongdianzi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qs.jctech888.com.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dq.huixiangedu.cn

[E11] 反转字符串
来源：http://sg.gzmigu.cn

Py:   s[::-1]
来源：http://fp.panjiajie.cn

PHP:  strrev($s);
来源：http://nm.haigaiapp.cn

JS:   [...s].reverse().join("")
来源：http://sa.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://od.521024.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uk.haigaiapp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://st.bjjhwx.cn

Ruby: s.reverse
来源：http://cy.shxzskj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wi.colortex.cn

[E12] 统计某字符出现次数
来源：http://sc.newstarts.cn

Py:   s.count("a")
来源：http://ii.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://jy.newstarts.cn

JS:   s.split("a").length - 1
来源：http://wc.asd995.cn

TS:   s.split("a").length - 1
来源：http://qn.jctech888.com.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hk.panjiajie.cn

Go:   strings.Count(s, "a")
来源：http://mv.chemitech.net.cn

Ruby: s.count("a")
来源：http://uv.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://ue.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://sg.wgjwhj.cn


<!-- 参考信息 -->