代发 wailian999

Java: list.size();
来源：http://yp.huixiangedu.cn

Go:   len(arr)
来源：http://mk.nicolike.cn

Ruby: arr.length; arr.size
来源：http://wd.huanxung.cn

C#:   list.Count;
来源：http://oj.shxzukj.cn

[D07] 切片 / 取子数组
来源：http://ow.bookmarksfly.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://gr.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://md.muxihuayi.cn

JS:   arr.slice(1, 4);
来源：http://ur.huixiangedu.cn

TS:   arr.slice(1, 4);
来源：http://eq.jctech888.com.cn

Java: list.subList(1, 4);
来源：http://ln.huanxung.cn

Go:   arr[1:4]
来源：http://at.nicolike.cn

Ruby: arr[1, 3]
来源：http://ii.nszjky.cn

C#:   list.GetRange(1, 3);
来源：http://ks.asd995.cn

[D08] 合并两个数组
来源：http://yx.yuntaijiaju.cn

Py:   a + b;  a.extend(b)
来源：http://yp.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://wz.nszjky.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sd.wgjwhj.cn

TS:   [...a, ...b];
来源：http://uh.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://iu.shxzskj.cn

Go:   append(a, b...)
来源：http://tf.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://wh.nszjky.cn

C#:   a.Concat(b).ToList()
来源：http://nd.hahajie.cn

[D09] 排序（升序）
来源：http://sl.9csxet.cn

Py:   sorted(arr);  arr.sort()
来源：http://rl.shxzukj.cn

PHP:  sort($arr);
来源：http://cx.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ye.shtwfgs.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://tz.muxihuayi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ev.muxihuayi.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://te.shxzskj.cn

Ruby: arr.sort
来源：http://wb.gzmigu.cn

C#:   list.Sort();
来源：http://ht.jctech888.com.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://iv.szsharing.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ro.yuexingan06.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://yd.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://og.lnxyls.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ws.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ap.bookmarksfly.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uu.colortex.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pk.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hg.hnjuh.cn

[D11] 反转数组
来源：http://px.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://bm.huanxung.cn

PHP:  array_reverse($arr);
来源：http://ys.bookmarksfly.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vc.yuntaijiaju.cn

TS:   [...arr].reverse();
来源：http://yh.shtwfgs.cn

Java: Collections.reverse(list);
来源：http://jz.newstarts.cn

Go:   slices.Reverse(arr)
来源：http://ir.lnxyls.cn

Ruby: arr.reverse
来源：http://li.panjiajie.cn

C#:   list.Reverse();
来源：http://et.yuexingan06.cn

[D12] 查找元素下标
来源：http://ar.huixiangedu.cn

Py:   arr.index(x);  x in arr
来源：http://yx.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sd.colortex.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nb.asd995.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uc.lnxyls.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://pn.nszjky.cn

Go:   slices.Index(arr, x)
来源：http://na.jctech888.com.cn

Ruby: arr.index(x)
来源：http://qi.521024.cn

C#:   list.IndexOf(x);
来源：http://wa.szsharing.cn

[D13] 过滤（保留满足条件的）
来源：http://yk.huixiangedu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ku.yuntaijiaju.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://km.wgjwhj.cn

JS:   arr.filter(x => x > 3)
来源：http://dr.jctech888.com.cn

TS:   arr.filter(x => x > 3)
来源：http://cu.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ln.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ld.gzmigu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ms.huanxung.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ps.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://cc.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://vd.jianghongdianzi.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uj.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://fj.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://uq.huixiangedu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dl.szxytkj.cn

Go:   // 手写循环
来源：http://tj.bjjhwx.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yy.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ue.jctech888.com.cn

[D15] 去重
来源：http://nu.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ii.yuexingan06.cn

PHP:  array_unique($arr);
来源：http://po.szsharing.cn

JS:   [...new Set(arr)]
来源：http://uj.wgjwhj.cn

TS:   [...new Set(arr)]
来源：http://ts.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ny.shxzskj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://io.asd995.cn

Ruby: arr.uniq
来源：http://wf.yuexingan06.cn

C#:   list.Distinct().ToList()
来源：http://ll.muxihuayi.cn

[D16] 求和与平均值
来源：http://iw.nszjky.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://my.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://xu.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://iy.newstarts.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://iv.hnjuh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://or.gzmigu.cn

Go:   // 手写循环累加
来源：http://kw.szsharing.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dm.newstarts.cn

C#:   list.Sum();  list.Average()
来源：http://au.jianghongdianzi.cn

[D17] 最大值与最小值
来源：http://vt.haigaiapp.cn

Py:   max(arr);  min(arr)
来源：http://uj.muxihuayi.cn

PHP:  max($arr);  min($arr);
来源：http://ci.panjiajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ha.521024.cn

TS:   Math.max(...arr);
来源：http://wv.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yc.muxihuayi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gb.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://fw.szxytkj.cn

C#:   list.Max();  list.Min()
来源：http://mb.huixinmuqiang.cn

[D18] 扁平化嵌套数组
来源：http://tv.hahajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://di.wgjwhj.cn

PHP:  array_merge(...$nested);
来源：http://kx.gzmigu.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ij.bookmarksfly.cn

TS:   nested.flat();
来源：http://xf.szsharing.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://zj.huixinmuqiang.cn

Go:   // 手写双层循环
来源：http://iy.newstarts.cn

Ruby: nested.flatten
来源：http://yo.yuntaijiaju.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://uz.yuexingan06.cn

[D19] 按字段分组
来源：http://mb.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hk.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://py.colortex.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ey.bjjhwx.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bq.shxzskj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://cm.gzmigu.cn

Go:   // 手写 map[string][]T
来源：http://bu.hnjuh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bv.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xj.hahajie.cn

[D20] 统计每个元素出现次数
来源：http://cx.gzmigu.cn

Py:   Counter(arr)
来源：http://un.chemitech.net.cn

PHP:  array_count_values($arr);
来源：http://sc.yuntaijiaju.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yn.yuntaijiaju.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://je.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://sw.gzmigu.cn

Go:   // 手写 map[T]int
来源：http://fc.jctech888.com.cn

Ruby: arr.tally
来源：http://sm.wgjwhj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://iy.muxihuayi.cn

[D21] 判断是否包含某元素
来源：http://ee.colortex.cn

Py:   x in arr
来源：http://dw.shtwfgs.cn

PHP:  in_array($x, $arr, true);
来源：http://rg.521024.cn

JS:   arr.includes(x)
来源：http://ar.huixinmuqiang.cn

TS:   arr.includes(x)
来源：http://im.wgjwhj.cn

Java: list.contains(x)
来源：http://sn.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://ux.muxihuayi.cn

Ruby: arr.include?(x)
来源：http://hs.jctech888.com.cn

C#:   list.Contains(x)
来源：http://tb.nszjky.cn

[D22] 复制数组（避免共享引用）
来源：http://yf.gzmigu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oc.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://op.szxytkj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kf.haigaiapp.cn

TS:   [...arr];
来源：http://ip.yuexingan06.cn

Java: new ArrayList<>(list);
来源：http://ei.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dl.szxytkj.cn

Ruby: arr.dup;  arr.clone
来源：http://mh.shtwfgs.cn

C#:   new List<int>(list);
来源：http://qi.wgjwhj.cn

[D23] reduce 累积计算
来源：http://mp.colortex.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://de.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kb.szsharing.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lf.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iq.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jy.jianghongdianzi.cn

Go:   // 手写循环
来源：http://ne.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sj.lnxyls.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://kd.lnxyls.cn

[D24] 字典 / Map 基本操作
来源：http://ew.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://iv.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pz.gzmigu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://uh.newstarts.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jh.wgjwhj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ht.shtwfgs.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gj.panjiajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://be.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://rb.gzmigu.cn

[D25] Set 集合去重与交并差
来源：http://gt.shxzukj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zx.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pm.yuntaijiaju.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://et.haigaiapp.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ia.yuntaijiaju.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sj.521024.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lz.gzmigu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hq.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vz.haigaiapp.cn

[D26] 数组转字符串
来源：http://qn.yuexingan06.cn

Py:   ", ".join(map(str, arr))
来源：http://ey.bjjhwx.cn

PHP:  implode(", ", $arr);
来源：http://ku.asd995.cn

JS:   arr.join(", ")
来源：http://jj.huixiangedu.cn

TS:   arr.join(", ")
来源：http://op.gzmigu.cn

Java: String.join(", ", list)
来源：http://yv.muxihuayi.cn

Go:   strings.Join(strs, ", ")
来源：http://ut.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://oy.szsharing.cn

C#:   string.Join(", ", list)
来源：http://ee.huixinmuqiang.cn

================================================================================
来源：http://sz.panjiajie.cn

E. 字符串处理
来源：http://xq.yuexingan06.cn

================================================================================
来源：http://wf.muxihuayi.cn

[E01] 拼接字符串
来源：http://fe.huixiangedu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ce.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oa.muxihuayi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ei.asd995.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jw.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gw.yuexingan06.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lj.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qz.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tb.muxihuayi.cn

[E02] 重复字符串
来源：http://je.nszjky.cn

Py:   "ab" * 3
来源：http://pp.panjiajie.cn

PHP:  str_repeat("ab", 3);
来源：http://ia.hahajie.cn

JS:   "ab".repeat(3)
来源：http://ha.huixinmuqiang.cn

TS:   "ab".repeat(3)
来源：http://mt.yuntaijiaju.cn

Java: "ab".repeat(3)
来源：http://pa.muxihuayi.cn

Go:   strings.Repeat("ab", 3)
来源：http://hn.newstarts.cn

Ruby: "ab" * 3
来源：http://yb.9csxet.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wv.hnjuh.cn

[E03] 截取子串
来源：http://nz.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oe.yuexingan06.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gt.szsharing.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zl.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://ek.asd995.cn

Java: s.substring(1, 4)
来源：http://wb.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uu.jctech888.com.cn

Ruby: s[1, 3];  s[1..3]
来源：http://eu.panjiajie.cn

C#:   s.Substring(1, 3)
来源：http://ic.521024.cn

[E04] 查找子串位置
来源：http://nz.colortex.cn

Py:   s.find("x");  s.index("x")
来源：http://jw.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://vq.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://kr.gzmigu.cn

TS:   s.indexOf("x")
来源：http://lt.newstarts.cn

Java: s.indexOf("x")
来源：http://pm.9csxet.cn

Go:   strings.Index(s, "x")
来源：http://mk.huanxung.cn

Ruby: s.index("x")
来源：http://ga.shxzskj.cn

C#:   s.IndexOf("x")
来源：http://ts.asd995.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mx.jctech888.com.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://py.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ru.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gv.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hj.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vn.lnxyls.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sx.hahajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bl.szsharing.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://aa.shxzskj.cn

[E06] 替换子串
来源：http://bh.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xn.bookmarksfly.cn

PHP:  str_replace("a", "b", $s);
来源：http://lt.huixiangedu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cn.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://te.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ac.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://za.szxytkj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wx.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://fg.newstarts.cn

[E07] 按分隔符拆分
来源：http://my.newstarts.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://vh.yuntaijiaju.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vc.521024.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://di.jianghongdianzi.cn

TS:   s.split(",")
来源：http://xm.huixinmuqiang.cn

Java: s.split(",");  s.split("\\s+")
来源：http://yk.jctech888.com.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vi.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://mo.asd995.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zd.haigaiapp.cn

[E08] 数组按分隔符合并
来源：http://re.muxihuayi.cn

Py:   ",".join(items)
来源：http://my.wgjwhj.cn

PHP:  implode(",", $items);
来源：http://bn.jctech888.com.cn

JS:   items.join(",")
来源：http://ic.521024.cn

TS:   items.join(",")
来源：http://eb.nicolike.cn

Java: String.join(",", items)
来源：http://br.jianghongdianzi.cn

Go:   strings.Join(items, ",")
来源：http://of.nszjky.cn

Ruby: items.join(",")
来源：http://wm.nszjky.cn

C#:   string.Join(",", items)
来源：http://ah.nszjky.cn

[E09] 去除所有空白字符
来源：http://nw.nszjky.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://sm.huixiangedu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mm.nicolike.cn

JS:   s.replace(/\s+/g, "")
来源：http://az.hnjuh.cn

TS:   s.replace(/\s+/g, "")
来源：http://pp.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://qu.521024.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hl.hahajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://yq.wgjwhj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://la.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://wp.szsharing.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qc.newstarts.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lm.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://ft.bookmarksfly.cn

TS:   "7".padStart(3, "0")
来源：http://mx.szsharing.cn

Java: String.format("%03d", 7)
来源：http://sb.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bk.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ae.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sb.lnxyls.cn

[E11] 反转字符串
来源：http://wv.szxytkj.cn

Py:   s[::-1]
来源：http://uc.chemitech.net.cn

PHP:  strrev($s);
来源：http://fg.colortex.cn

JS:   [...s].reverse().join("")
来源：http://wn.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://hw.521024.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fd.521024.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ss.huixiangedu.cn

Ruby: s.reverse
来源：http://qz.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://is.lnxyls.cn

[E12] 统计某字符出现次数
来源：http://xe.lnxyls.cn

Py:   s.count("a")
来源：http://vi.wgjwhj.cn

PHP:  substr_count($s, "a");
来源：http://tp.huixinmuqiang.cn

JS:   s.split("a").length - 1
来源：http://zt.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://fg.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xp.lnxyls.cn

Go:   strings.Count(s, "a")
来源：http://wp.bookmarksfly.cn

Ruby: s.count("a")
来源：http://ph.panjiajie.cn

C#:   s.Count(c => c == 'a')
来源：http://pz.shtwfgs.cn

[E13] 逐字符遍历
来源：http://ed.bookmarksfly.cn

Py:   for ch in s: print(ch)
来源：http://sg.yuexingan06.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fe.shtwfgs.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ta.nszjky.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ot.szsharing.cn


<!-- 参考信息 -->