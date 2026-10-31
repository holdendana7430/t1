代发 wailian999

Py:   len(arr)
来源：http://nj.nicolike.cn

PHP:  count($arr);
来源：http://nn.hahajie.cn

JS:   arr.length
来源：http://av.shtwfgs.cn

TS:   arr.length
来源：http://mi.521024.cn

Java: list.size();
来源：http://oy.nicolike.cn

Go:   len(arr)
来源：http://jz.bjjhwx.cn

Ruby: arr.length; arr.size
来源：http://os.shtwfgs.cn

C#:   list.Count;
来源：http://lu.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://xy.huanxung.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://bf.shxzskj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qd.lnxyls.cn

JS:   arr.slice(1, 4);
来源：http://vf.asd995.cn

TS:   arr.slice(1, 4);
来源：http://hs.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://yq.9csxet.cn

Go:   arr[1:4]
来源：http://ms.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://md.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://qx.colortex.cn

[D08] 合并两个数组
来源：http://zj.shxzskj.cn

Py:   a + b;  a.extend(b)
来源：http://vr.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://dn.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cd.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://fu.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xa.panjiajie.cn

Go:   append(a, b...)
来源：http://ep.521024.cn

Ruby: a + b;  a.concat(b)
来源：http://dw.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://lb.yuntaijiaju.cn

[D09] 排序（升序）
来源：http://na.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://dr.hnjuh.cn

PHP:  sort($arr);
来源：http://in.jianghongdianzi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://tf.haigaiapp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://yj.shtwfgs.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sj.nicolike.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://up.bjjhwx.cn

Ruby: arr.sort
来源：http://hx.newstarts.cn

C#:   list.Sort();
来源：http://jv.huixinmuqiang.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ux.szxytkj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ii.colortex.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://nk.asd995.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ep.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ra.bookmarksfly.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jianghongdianzi.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://cx.huixiangedu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zg.panjiajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://jz.yuexingan06.cn

[D11] 反转数组
来源：http://gy.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ee.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://rn.szxytkj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ep.nicolike.cn

TS:   [...arr].reverse();
来源：http://ye.haigaiapp.cn

Java: Collections.reverse(list);
来源：http://gt.jctech888.com.cn

Go:   slices.Reverse(arr)
来源：http://cl.9csxet.cn

Ruby: arr.reverse
来源：http://ep.huixiangedu.cn

C#:   list.Reverse();
来源：http://rj.yuexingan06.cn

[D12] 查找元素下标
来源：http://gs.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://xa.huanxung.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://dn.jctech888.com.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hy.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://er.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cd.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://sv.hnjuh.cn

Ruby: arr.index(x)
来源：http://hl.hnjuh.cn

C#:   list.IndexOf(x);
来源：http://sl.bookmarksfly.cn

[D13] 过滤（保留满足条件的）
来源：http://br.jianghongdianzi.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://uj.huixiangedu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://qb.asd995.cn

JS:   arr.filter(x => x > 3)
来源：http://ur.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://xt.asd995.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://rh.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://aa.shtwfgs.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ym.muxihuayi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://lv.szsharing.cn

[D14] 映射转换（每个元素变形）
来源：http://qn.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://oa.huixiangedu.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://xn.jctech888.com.cn

JS:   arr.map(x => x * 2)
来源：http://xt.haigaiapp.cn

TS:   arr.map(x => x * 2)
来源：http://gg.jianghongdianzi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ch.shxzukj.cn

Go:   // 手写循环
来源：http://bl.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lf.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://sh.newstarts.cn

[D15] 去重
来源：http://hg.lnxyls.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mw.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://fh.bookmarksfly.cn

JS:   [...new Set(arr)]
来源：http://xl.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://oq.colortex.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xq.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dt.nicolike.cn

Ruby: arr.uniq
来源：http://jj.lnxyls.cn

C#:   list.Distinct().ToList()
来源：http://cn.huanxung.cn

[D16] 求和与平均值
来源：http://jc.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wb.jctech888.com.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hx.huanxung.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://di.521024.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vh.haigaiapp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nt.yuexingan06.cn

Go:   // 手写循环累加
来源：http://uk.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hj.colortex.cn

C#:   list.Sum();  list.Average()
来源：http://cp.huixinmuqiang.cn

[D17] 最大值与最小值
来源：http://at.shxzukj.cn

Py:   max(arr);  min(arr)
来源：http://pg.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://hr.shxzukj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://as.nicolike.cn

TS:   Math.max(...arr);
来源：http://kx.asd995.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kq.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://vw.szsharing.cn

Ruby: arr.max;  arr.min
来源：http://zr.huixinmuqiang.cn

C#:   list.Max();  list.Min()
来源：http://nx.muxihuayi.cn

[D18] 扁平化嵌套数组
来源：http://pl.hahajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yh.nszjky.cn

PHP:  array_merge(...$nested);
来源：http://wx.bjjhwx.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://zc.huanxung.cn

TS:   nested.flat();
来源：http://hb.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ne.szsharing.cn

Go:   // 手写双层循环
来源：http://gi.hnjuh.cn

Ruby: nested.flatten
来源：http://ik.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wg.gzmigu.cn

[D19] 按字段分组
来源：http://ej.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ws.huixiangedu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://bl.colortex.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://uf.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://pg.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tc.hnjuh.cn

Go:   // 手写 map[string][]T
来源：http://uj.colortex.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sl.gzmigu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wg.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://bu.bjjhwx.cn

Py:   Counter(arr)
来源：http://uf.shxzskj.cn

PHP:  array_count_values($arr);
来源：http://mb.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://th.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sa.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://zo.hahajie.cn

Go:   // 手写 map[T]int
来源：http://vl.lnxyls.cn

Ruby: arr.tally
来源：http://dh.huanxung.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://tf.nicolike.cn

[D21] 判断是否包含某元素
来源：http://zb.shxzskj.cn

Py:   x in arr
来源：http://gg.jctech888.com.cn

PHP:  in_array($x, $arr, true);
来源：http://ah.haigaiapp.cn

JS:   arr.includes(x)
来源：http://db.lnxyls.cn

TS:   arr.includes(x)
来源：http://gq.yuexingan06.cn

Java: list.contains(x)
来源：http://mz.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://un.panjiajie.cn

Ruby: arr.include?(x)
来源：http://cg.yuexingan06.cn

C#:   list.Contains(x)
来源：http://tt.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://tu.asd995.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sc.huanxung.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://zi.chemitech.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dw.shtwfgs.cn

TS:   [...arr];
来源：http://rk.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://fn.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wz.jianghongdianzi.cn

Ruby: arr.dup;  arr.clone
来源：http://nm.haigaiapp.cn

C#:   new List<int>(list);
来源：http://dp.shxzukj.cn

[D23] reduce 累积计算
来源：http://so.jctech888.com.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lh.asd995.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hq.bookmarksfly.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zi.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://he.chemitech.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nr.szsharing.cn

Go:   // 手写循环
来源：http://gl.huixinmuqiang.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aw.gzmigu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wd.521024.cn

[D24] 字典 / Map 基本操作
来源：http://dw.muxihuayi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yb.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://oi.jianghongdianzi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nl.nicolike.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://di.muxihuayi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://bj.szxytkj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hv.9csxet.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sl.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://cf.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://ow.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mg.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ek.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wy.yuntaijiaju.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://jc.nszjky.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qf.9csxet.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://no.huixinmuqiang.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://xr.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://so.panjiajie.cn

[D26] 数组转字符串
来源：http://bm.newstarts.cn

Py:   ", ".join(map(str, arr))
来源：http://uk.szxytkj.cn

PHP:  implode(", ", $arr);
来源：http://wt.bjjhwx.cn

JS:   arr.join(", ")
来源：http://wo.jctech888.com.cn

TS:   arr.join(", ")
来源：http://my.hahajie.cn

Java: String.join(", ", list)
来源：http://wn.panjiajie.cn

Go:   strings.Join(strs, ", ")
来源：http://pv.asd995.cn

Ruby: arr.join(", ")
来源：http://bt.nszjky.cn

C#:   string.Join(", ", list)
来源：http://yp.shxzukj.cn

================================================================================
来源：http://io.lnxyls.cn

E. 字符串处理
来源：http://go.shxzukj.cn

================================================================================
来源：http://ca.shxzskj.cn

[E01] 拼接字符串
来源：http://iu.yuntaijiaju.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wz.chemitech.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hs.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://bc.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://kt.nszjky.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://yy.521024.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ox.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ju.muxihuayi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dk.hahajie.cn

[E02] 重复字符串
来源：http://pf.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://fc.chemitech.net.cn

PHP:  str_repeat("ab", 3);
来源：http://nu.huixiangedu.cn

JS:   "ab".repeat(3)
来源：http://ws.gzmigu.cn

TS:   "ab".repeat(3)
来源：http://cb.shtwfgs.cn

Java: "ab".repeat(3)
来源：http://ja.9csxet.cn

Go:   strings.Repeat("ab", 3)
来源：http://py.hnjuh.cn

Ruby: "ab" * 3
来源：http://sn.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ca.colortex.cn

[E03] 截取子串
来源：http://dj.huixiangedu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://oi.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://nk.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cx.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://ts.hahajie.cn

Java: s.substring(1, 4)
来源：http://kb.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wr.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qh.huixinmuqiang.cn

C#:   s.Substring(1, 3)
来源：http://zq.jianghongdianzi.cn

[E04] 查找子串位置
来源：http://hu.bjjhwx.cn

Py:   s.find("x");  s.index("x")
来源：http://tt.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://ka.huanxung.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ee.bookmarksfly.cn

TS:   s.indexOf("x")
来源：http://sb.yuntaijiaju.cn

Java: s.indexOf("x")
来源：http://vs.asd995.cn

Go:   strings.Index(s, "x")
来源：http://sq.muxihuayi.cn

Ruby: s.index("x")
来源：http://gg.shtwfgs.cn

C#:   s.IndexOf("x")
来源：http://qa.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gh.gzmigu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://da.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bo.521024.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pu.wgjwhj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ho.szxytkj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lj.szxytkj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wi.jctech888.com.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tl.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wh.gzmigu.cn

[E06] 替换子串
来源：http://ry.bookmarksfly.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yc.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://wt.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qq.jianghongdianzi.cn

TS:   s.replaceAll("a", "b")
来源：http://ut.hahajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tz.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://fg.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rz.wgjwhj.cn

C#:   s.Replace("a", "b")
来源：http://aa.szxytkj.cn

[E07] 按分隔符拆分
来源：http://ss.nicolike.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ac.huixinmuqiang.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rt.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tr.yuntaijiaju.cn

TS:   s.split(",")
来源：http://ex.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nm.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tr.9csxet.cn

Ruby: s.split(",");  s.split
来源：http://oh.hahajie.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ub.jianghongdianzi.cn

[E08] 数组按分隔符合并
来源：http://sq.panjiajie.cn

Py:   ",".join(items)
来源：http://cz.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://yk.nszjky.cn

JS:   items.join(",")
来源：http://wa.chemitech.net.cn

TS:   items.join(",")
来源：http://zw.chemitech.net.cn

Java: String.join(",", items)
来源：http://bo.szsharing.cn

Go:   strings.Join(items, ",")
来源：http://vw.nszjky.cn

Ruby: items.join(",")
来源：http://tt.jianghongdianzi.cn

C#:   string.Join(",", items)
来源：http://uo.jctech888.com.cn

[E09] 去除所有空白字符
来源：http://ue.hnjuh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fh.bookmarksfly.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ez.huixiangedu.cn

JS:   s.replace(/\s+/g, "")
来源：http://ev.huixinmuqiang.cn

TS:   s.replace(/\s+/g, "")
来源：http://lq.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://ds.haigaiapp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qq.muxihuayi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nm.haigaiapp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://if.bjjhwx.cn

[E10] 左侧补零 / 定长填充
来源：http://so.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cx.shxzskj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ov.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://hb.newstarts.cn

TS:   "7".padStart(3, "0")
来源：http://sw.hnjuh.cn

Java: String.format("%03d", 7)
来源：http://og.muxihuayi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qr.nszjky.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://vn.shxzukj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jc.muxihuayi.cn

[E11] 反转字符串
来源：http://du.jctech888.com.cn

Py:   s[::-1]
来源：http://gz.gzmigu.cn

PHP:  strrev($s);
来源：http://md.newstarts.cn

JS:   [...s].reverse().join("")
来源：http://nn.szxytkj.cn

TS:   [...s].reverse().join("")
来源：http://vj.wgjwhj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zb.hnjuh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vl.521024.cn

Ruby: s.reverse
来源：http://hg.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://km.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://js.shxzukj.cn

Py:   s.count("a")
来源：http://nh.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://mi.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://dt.bjjhwx.cn

TS:   s.split("a").length - 1
来源：http://ld.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://me.panjiajie.cn

Go:   strings.Count(s, "a")
来源：http://hj.hnjuh.cn

Ruby: s.count("a")
来源：http://pf.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://ja.asd995.cn

[E13] 逐字符遍历
来源：http://da.chemitech.net.cn


<!-- 参考信息 -->