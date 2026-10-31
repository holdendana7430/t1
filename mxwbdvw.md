代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://ax.shxzskj.cn

TS:   [...a, ...b];
来源：http://zz.newstarts.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ef.bookmarksfly.cn

Go:   append(a, b...)
来源：http://ma.shxzukj.cn

Ruby: a + b;  a.concat(b)
来源：http://yq.newstarts.cn

C#:   a.Concat(b).ToList()
来源：http://hr.521024.cn

[D09] 排序（升序）
来源：http://bx.wgjwhj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ng.nszjky.cn

PHP:  sort($arr);
来源：http://fk.szsharing.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lb.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qq.521024.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ow.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ka.nszjky.cn

Ruby: arr.sort
来源：http://zz.huixiangedu.cn

C#:   list.Sort();
来源：http://bj.panjiajie.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kw.huanxung.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://gy.newstarts.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://tw.521024.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xy.nicolike.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ga.szxytkj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://au.szsharing.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://lg.szsharing.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cv.muxihuayi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lm.jctech888.com.cn

[D11] 反转数组
来源：http://ei.lnxyls.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dm.9csxet.cn

PHP:  array_reverse($arr);
来源：http://fr.huixinmuqiang.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://jd.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://wd.nszjky.cn

Java: Collections.reverse(list);
来源：http://ep.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://zc.yuexingan06.cn

Ruby: arr.reverse
来源：http://fo.hahajie.cn

C#:   list.Reverse();
来源：http://hb.nicolike.cn

[D12] 查找元素下标
来源：http://xw.bookmarksfly.cn

Py:   arr.index(x);  x in arr
来源：http://fx.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lj.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ny.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://gj.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://yd.haigaiapp.cn

Go:   slices.Index(arr, x)
来源：http://fq.muxihuayi.cn

Ruby: arr.index(x)
来源：http://vk.521024.cn

C#:   list.IndexOf(x);
来源：http://dk.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://qj.haigaiapp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kq.colortex.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wk.jctech888.com.cn

JS:   arr.filter(x => x > 3)
来源：http://vx.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://ko.shxzskj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gl.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bp.huixiangedu.cn

Ruby: arr.select { |x| x > 3 }
来源：http://er.szsharing.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rx.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://jw.shtwfgs.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://rq.huanxung.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://lx.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://ta.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://av.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://fa.jctech888.com.cn

Go:   // 手写循环
来源：http://em.bjjhwx.cn

Ruby: arr.map { |x| x * 2 }
来源：http://go.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://oq.bjjhwx.cn

[D15] 去重
来源：http://cj.nszjky.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://dk.shxzskj.cn

PHP:  array_unique($arr);
来源：http://ch.newstarts.cn

JS:   [...new Set(arr)]
来源：http://ps.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://xs.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://tj.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ry.shxzskj.cn

Ruby: arr.uniq
来源：http://gb.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://tt.wgjwhj.cn

[D16] 求和与平均值
来源：http://ac.hnjuh.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ch.muxihuayi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yh.haigaiapp.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yr.huanxung.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://al.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://nd.hahajie.cn

Go:   // 手写循环累加
来源：http://eq.colortex.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fy.colortex.cn

C#:   list.Sum();  list.Average()
来源：http://cq.hahajie.cn

[D17] 最大值与最小值
来源：http://cu.panjiajie.cn

Py:   max(arr);  min(arr)
来源：http://lv.newstarts.cn

PHP:  max($arr);  min($arr);
来源：http://yy.gzmigu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fo.shxzukj.cn

TS:   Math.max(...arr);
来源：http://cr.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dq.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mw.muxihuayi.cn

Ruby: arr.max;  arr.min
来源：http://ox.muxihuayi.cn

C#:   list.Max();  list.Min()
来源：http://ci.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://zi.newstarts.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sx.jctech888.com.cn

PHP:  array_merge(...$nested);
来源：http://rm.hahajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wa.newstarts.cn

TS:   nested.flat();
来源：http://it.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wc.huixinmuqiang.cn

Go:   // 手写双层循环
来源：http://lw.hnjuh.cn

Ruby: nested.flatten
来源：http://xa.hahajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://sr.colortex.cn

[D19] 按字段分组
来源：http://ug.bjjhwx.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wr.nicolike.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dj.huanxung.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hk.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://io.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zq.asd995.cn

Go:   // 手写 map[string][]T
来源：http://gg.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sg.yuexingan06.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wk.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://jh.szxytkj.cn

Py:   Counter(arr)
来源：http://em.colortex.cn

PHP:  array_count_values($arr);
来源：http://hi.jianghongdianzi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nc.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sp.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ql.lnxyls.cn

Go:   // 手写 map[T]int
来源：http://xd.521024.cn

Ruby: arr.tally
来源：http://qd.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://uq.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://bm.shxzukj.cn

Py:   x in arr
来源：http://lo.lnxyls.cn

PHP:  in_array($x, $arr, true);
来源：http://dz.szxytkj.cn

JS:   arr.includes(x)
来源：http://ga.shtwfgs.cn

TS:   arr.includes(x)
来源：http://fq.hnjuh.cn

Java: list.contains(x)
来源：http://zs.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://xc.nicolike.cn

Ruby: arr.include?(x)
来源：http://xv.newstarts.cn

C#:   list.Contains(x)
来源：http://ca.9csxet.cn

[D22] 复制数组（避免共享引用）
来源：http://mp.yuexingan06.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nj.bjjhwx.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qe.gzmigu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://eh.newstarts.cn

TS:   [...arr];
来源：http://po.chemitech.net.cn

Java: new ArrayList<>(list);
来源：http://ce.bookmarksfly.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mm.gzmigu.cn

Ruby: arr.dup;  arr.clone
来源：http://nf.muxihuayi.cn

C#:   new List<int>(list);
来源：http://yc.panjiajie.cn

[D23] reduce 累积计算
来源：http://qr.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.asd995.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ox.wgjwhj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://tw.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qq.haigaiapp.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mk.bjjhwx.cn

Go:   // 手写循环
来源：http://yz.asd995.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://zu.yuntaijiaju.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bj.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://wl.huixiangedu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ps.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://nd.shtwfgs.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ux.jianghongdianzi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ou.newstarts.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jp.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://fu.muxihuayi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kp.bookmarksfly.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qg.jctech888.com.cn

[D25] Set 集合去重与交并差
来源：http://yq.shtwfgs.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zt.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://il.shxzskj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qg.9csxet.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://tr.jianghongdianzi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ke.gzmigu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jl.szsharing.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hc.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wn.bjjhwx.cn

[D26] 数组转字符串
来源：http://jr.huixinmuqiang.cn

Py:   ", ".join(map(str, arr))
来源：http://sc.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://pk.hnjuh.cn

JS:   arr.join(", ")
来源：http://pk.shtwfgs.cn

TS:   arr.join(", ")
来源：http://se.gzmigu.cn

Java: String.join(", ", list)
来源：http://ie.nszjky.cn

Go:   strings.Join(strs, ", ")
来源：http://gm.huanxung.cn

Ruby: arr.join(", ")
来源：http://jl.jctech888.com.cn

C#:   string.Join(", ", list)
来源：http://ic.jctech888.com.cn

================================================================================
来源：http://wn.hnjuh.cn

E. 字符串处理
来源：http://yl.bjjhwx.cn

================================================================================
来源：http://lf.huixinmuqiang.cn

[E01] 拼接字符串
来源：http://rz.yuntaijiaju.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xe.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yw.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://cy.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://at.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://em.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hl.haigaiapp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://nr.colortex.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mb.bookmarksfly.cn

[E02] 重复字符串
来源：http://ko.muxihuayi.cn

Py:   "ab" * 3
来源：http://uc.szxytkj.cn

PHP:  str_repeat("ab", 3);
来源：http://yx.yuntaijiaju.cn

JS:   "ab".repeat(3)
来源：http://sw.shtwfgs.cn

TS:   "ab".repeat(3)
来源：http://hj.yuntaijiaju.cn

Java: "ab".repeat(3)
来源：http://ag.lnxyls.cn

Go:   strings.Repeat("ab", 3)
来源：http://nq.yuexingan06.cn

Ruby: "ab" * 3
来源：http://dx.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://me.bjjhwx.cn

[E03] 截取子串
来源：http://kf.bookmarksfly.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mj.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://iy.jctech888.com.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://lv.huixiangedu.cn

TS:   s.slice(1, 4)
来源：http://ag.gzmigu.cn

Java: s.substring(1, 4)
来源：http://nk.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ki.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sj.lnxyls.cn

C#:   s.Substring(1, 3)
来源：http://cp.szxytkj.cn

[E04] 查找子串位置
来源：http://sp.bookmarksfly.cn

Py:   s.find("x");  s.index("x")
来源：http://tp.asd995.cn

PHP:  strpos($s, "x");
来源：http://hv.hnjuh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qd.panjiajie.cn

TS:   s.indexOf("x")
来源：http://ca.szxytkj.cn

Java: s.indexOf("x")
来源：http://xh.chemitech.net.cn

Go:   strings.Index(s, "x")
来源：http://wl.muxihuayi.cn

Ruby: s.index("x")
来源：http://xy.nicolike.cn

C#:   s.IndexOf("x")
来源：http://xu.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://eu.hnjuh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ae.yuexingan06.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rx.hnjuh.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gq.lnxyls.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ff.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pq.panjiajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yn.jctech888.com.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iy.lnxyls.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oy.szxytkj.cn

[E06] 替换子串
来源：http://ma.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://eu.hahajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://jy.bookmarksfly.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zy.nicolike.cn

TS:   s.replaceAll("a", "b")
来源：http://wz.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bw.colortex.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pl.hnjuh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://md.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://pd.hahajie.cn

[E07] 按分隔符拆分
来源：http://ye.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xo.lnxyls.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qv.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ga.bookmarksfly.cn

TS:   s.split(",")
来源：http://ij.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nt.newstarts.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vt.yuntaijiaju.cn

Ruby: s.split(",");  s.split
来源：http://hm.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ai.bjjhwx.cn

[E08] 数组按分隔符合并
来源：http://sy.panjiajie.cn

Py:   ",".join(items)
来源：http://uw.hnjuh.cn

PHP:  implode(",", $items);
来源：http://th.bookmarksfly.cn

JS:   items.join(",")
来源：http://lf.szsharing.cn

TS:   items.join(",")
来源：http://gp.haigaiapp.cn

Java: String.join(",", items)
来源：http://bn.colortex.cn

Go:   strings.Join(items, ",")
来源：http://qp.nszjky.cn

Ruby: items.join(",")
来源：http://wi.colortex.cn

C#:   string.Join(",", items)
来源：http://zz.szsharing.cn

[E09] 去除所有空白字符
来源：http://vw.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ze.asd995.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qh.nicolike.cn

JS:   s.replace(/\s+/g, "")
来源：http://mw.hnjuh.cn

TS:   s.replace(/\s+/g, "")
来源：http://df.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://zi.bookmarksfly.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mp.chemitech.net.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hk.shtwfgs.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zm.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://py.hahajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ck.jianghongdianzi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gr.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://gn.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://fo.huixinmuqiang.cn

Java: String.format("%03d", 7)
来源：http://cq.lnxyls.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://fq.shxzukj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://df.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ph.colortex.cn

[E11] 反转字符串
来源：http://fx.haigaiapp.cn

Py:   s[::-1]
来源：http://tr.wgjwhj.cn

PHP:  strrev($s);
来源：http://tt.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://hp.521024.cn

TS:   [...s].reverse().join("")
来源：http://th.colortex.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ar.521024.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nv.hnjuh.cn

Ruby: s.reverse
来源：http://bn.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wc.panjiajie.cn

[E12] 统计某字符出现次数
来源：http://nj.huixinmuqiang.cn

Py:   s.count("a")
来源：http://mq.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://vl.hahajie.cn

JS:   s.split("a").length - 1
来源：http://vi.521024.cn

TS:   s.split("a").length - 1
来源：http://sj.chemitech.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fl.shxzskj.cn

Go:   strings.Count(s, "a")
来源：http://yu.shxzskj.cn

Ruby: s.count("a")
来源：http://ww.hahajie.cn

C#:   s.Count(c => c == 'a')
来源：http://ew.jctech888.com.cn

[E13] 逐字符遍历
来源：http://an.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://ih.nszjky.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mc.shxzukj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jj.wgjwhj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vd.hahajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rq.huixinmuqiang.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://kc.yuexingan06.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://kd.huanxung.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zi.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://uy.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mh.asd995.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://me.hahajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dj.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zn.shxzskj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://uf.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ca.colortex.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vm.asd995.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sh.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://tl.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mj.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://pm.521024.cn


<!-- 参考信息 -->