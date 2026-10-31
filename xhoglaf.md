代发 wailian999

TS:   arr.slice(1, 4);
来源：http://fm.newstarts.cn

Java: list.subList(1, 4);
来源：http://lo.9csxet.cn

Go:   arr[1:4]
来源：http://sz.shxzskj.cn

Ruby: arr[1, 3]
来源：http://hf.hnjuh.cn

C#:   list.GetRange(1, 3);
来源：http://kr.muxihuayi.cn

[D08] 合并两个数组
来源：http://yn.wgjwhj.cn

Py:   a + b;  a.extend(b)
来源：http://mn.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://nl.yuntaijiaju.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ez.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://ki.nicolike.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lp.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://gj.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://px.bjjhwx.cn

C#:   a.Concat(b).ToList()
来源：http://rl.bjjhwx.cn

[D09] 排序（升序）
来源：http://ok.yuntaijiaju.cn

Py:   sorted(arr);  arr.sort()
来源：http://cj.hnjuh.cn

PHP:  sort($arr);
来源：http://is.huixinmuqiang.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://cf.szxytkj.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qr.wgjwhj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gf.9csxet.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://jz.huanxung.cn

Ruby: arr.sort
来源：http://cy.lnxyls.cn

C#:   list.Sort();
来源：http://jb.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://of.chemitech.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pn.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://by.panjiajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://aa.jctech888.com.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nl.9csxet.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vi.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hg.521024.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cx.asd995.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fu.szxytkj.cn

[D11] 反转数组
来源：http://vz.asd995.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ih.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://ob.haigaiapp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://qx.panjiajie.cn

TS:   [...arr].reverse();
来源：http://qc.huixinmuqiang.cn

Java: Collections.reverse(list);
来源：http://pv.bjjhwx.cn

Go:   slices.Reverse(arr)
来源：http://vo.huanxung.cn

Ruby: arr.reverse
来源：http://vq.yuntaijiaju.cn

C#:   list.Reverse();
来源：http://cm.gzmigu.cn

[D12] 查找元素下标
来源：http://fc.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://es.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rx.muxihuayi.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lt.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://su.yuexingan06.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://cj.hahajie.cn

Go:   slices.Index(arr, x)
来源：http://qc.521024.cn

Ruby: arr.index(x)
来源：http://cp.huixinmuqiang.cn

C#:   list.IndexOf(x);
来源：http://ng.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://jt.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://lf.gzmigu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://fb.haigaiapp.cn

JS:   arr.filter(x => x > 3)
来源：http://yx.asd995.cn

TS:   arr.filter(x => x > 3)
来源：http://rm.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pk.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://zk.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://kg.hnjuh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gn.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://gu.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lu.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dc.hahajie.cn

JS:   arr.map(x => x * 2)
来源：http://bi.jianghongdianzi.cn

TS:   arr.map(x => x * 2)
来源：http://sk.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tj.bjjhwx.cn

Go:   // 手写循环
来源：http://oo.bjjhwx.cn

Ruby: arr.map { |x| x * 2 }
来源：http://uw.yuexingan06.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yp.nicolike.cn

[D15] 去重
来源：http://xc.521024.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://se.nicolike.cn

PHP:  array_unique($arr);
来源：http://en.nicolike.cn

JS:   [...new Set(arr)]
来源：http://bu.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://hk.jctech888.com.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://xl.hnjuh.cn

Go:   // 用 map[T]struct{} 手写
来源：http://bg.lnxyls.cn

Ruby: arr.uniq
来源：http://ds.bjjhwx.cn

C#:   list.Distinct().ToList()
来源：http://ki.szxytkj.cn

[D16] 求和与平均值
来源：http://bo.szxytkj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://xg.szsharing.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fz.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ic.wgjwhj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jd.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zn.wgjwhj.cn

Go:   // 手写循环累加
来源：http://to.chemitech.net.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://jj.shtwfgs.cn

C#:   list.Sum();  list.Average()
来源：http://ct.panjiajie.cn

[D17] 最大值与最小值
来源：http://au.haigaiapp.cn

Py:   max(arr);  min(arr)
来源：http://ir.nszjky.cn

PHP:  max($arr);  min($arr);
来源：http://je.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wj.jianghongdianzi.cn

TS:   Math.max(...arr);
来源：http://ks.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nb.jctech888.com.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dw.bjjhwx.cn

Ruby: arr.max;  arr.min
来源：http://yf.hnjuh.cn

C#:   list.Max();  list.Min()
来源：http://dz.haigaiapp.cn

[D18] 扁平化嵌套数组
来源：http://wa.yuntaijiaju.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://jl.colortex.cn

PHP:  array_merge(...$nested);
来源：http://vb.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wj.haigaiapp.cn

TS:   nested.flat();
来源：http://xz.shxzskj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dj.asd995.cn

Go:   // 手写双层循环
来源：http://lt.jianghongdianzi.cn

Ruby: nested.flatten
来源：http://jc.huixinmuqiang.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gh.panjiajie.cn

[D19] 按字段分组
来源：http://qn.9csxet.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://es.panjiajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ua.shxzukj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ef.lnxyls.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ca.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vb.wgjwhj.cn

Go:   // 手写 map[string][]T
来源：http://fj.muxihuayi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jd.muxihuayi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qw.9csxet.cn

[D20] 统计每个元素出现次数
来源：http://sq.521024.cn

Py:   Counter(arr)
来源：http://ew.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://hi.9csxet.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jr.521024.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vu.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ha.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://fl.hahajie.cn

Ruby: arr.tally
来源：http://xe.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://br.shxzukj.cn

[D21] 判断是否包含某元素
来源：http://mh.shxzskj.cn

Py:   x in arr
来源：http://se.shxzukj.cn

PHP:  in_array($x, $arr, true);
来源：http://yb.521024.cn

JS:   arr.includes(x)
来源：http://ka.bookmarksfly.cn

TS:   arr.includes(x)
来源：http://rk.huixinmuqiang.cn

Java: list.contains(x)
来源：http://tc.huixiangedu.cn

Go:   slices.Contains(arr, x)
来源：http://ui.hnjuh.cn

Ruby: arr.include?(x)
来源：http://hg.asd995.cn

C#:   list.Contains(x)
来源：http://ve.huixiangedu.cn

[D22] 复制数组（避免共享引用）
来源：http://qk.yuntaijiaju.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ph.jianghongdianzi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fc.yuexingan06.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://sg.521024.cn

TS:   [...arr];
来源：http://ra.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://wz.shxzskj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://qt.jianghongdianzi.cn

Ruby: arr.dup;  arr.clone
来源：http://gq.yuexingan06.cn

C#:   new List<int>(list);
来源：http://hv.nicolike.cn

[D23] reduce 累积计算
来源：http://iv.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zg.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jh.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ya.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mo.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jz.panjiajie.cn

Go:   // 手写循环
来源：http://vl.bookmarksfly.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ly.huixinmuqiang.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ul.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://ja.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://zd.jctech888.com.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://kx.haigaiapp.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zp.asd995.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ts.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ow.hnjuh.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gq.bookmarksfly.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ao.shtwfgs.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://le.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://ev.szxytkj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ta.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cd.nicolike.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://px.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mp.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pv.newstarts.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ma.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://au.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://je.shtwfgs.cn

[D26] 数组转字符串
来源：http://ij.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://kk.muxihuayi.cn

PHP:  implode(", ", $arr);
来源：http://yh.szsharing.cn

JS:   arr.join(", ")
来源：http://zc.521024.cn

TS:   arr.join(", ")
来源：http://zk.9csxet.cn

Java: String.join(", ", list)
来源：http://lx.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://dp.huixinmuqiang.cn

Ruby: arr.join(", ")
来源：http://ru.asd995.cn

C#:   string.Join(", ", list)
来源：http://ls.hnjuh.cn

================================================================================
来源：http://yl.huixinmuqiang.cn

E. 字符串处理
来源：http://rj.hnjuh.cn

================================================================================
来源：http://ob.huixinmuqiang.cn

[E01] 拼接字符串
来源：http://dw.lnxyls.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hg.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://jl.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ft.szsharing.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ce.shtwfgs.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fr.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ys.yuntaijiaju.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://jh.haigaiapp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oj.hnjuh.cn

[E02] 重复字符串
来源：http://dc.haigaiapp.cn

Py:   "ab" * 3
来源：http://lj.huanxung.cn

PHP:  str_repeat("ab", 3);
来源：http://kn.newstarts.cn

JS:   "ab".repeat(3)
来源：http://ni.lnxyls.cn

TS:   "ab".repeat(3)
来源：http://hf.muxihuayi.cn

Java: "ab".repeat(3)
来源：http://lf.nicolike.cn

Go:   strings.Repeat("ab", 3)
来源：http://oi.chemitech.net.cn

Ruby: "ab" * 3
来源：http://gy.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://pg.wgjwhj.cn

[E03] 截取子串
来源：http://uh.asd995.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ap.wgjwhj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xw.colortex.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nc.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://cn.chemitech.net.cn

Java: s.substring(1, 4)
来源：http://sm.bjjhwx.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://xu.yuexingan06.cn

Ruby: s[1, 3];  s[1..3]
来源：http://em.asd995.cn

C#:   s.Substring(1, 3)
来源：http://gx.wgjwhj.cn

[E04] 查找子串位置
来源：http://ky.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://of.9csxet.cn

PHP:  strpos($s, "x");
来源：http://fm.bjjhwx.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jw.szsharing.cn

TS:   s.indexOf("x")
来源：http://kv.hahajie.cn

Java: s.indexOf("x")
来源：http://vd.haigaiapp.cn

Go:   strings.Index(s, "x")
来源：http://qh.shxzskj.cn

Ruby: s.index("x")
来源：http://jc.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://wm.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://va.shxzukj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://om.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://px.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yv.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bc.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ch.bookmarksfly.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://of.huanxung.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://kc.shxzukj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nz.shxzukj.cn

[E06] 替换子串
来源：http://er.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hq.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://ok.nszjky.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hh.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://zi.chemitech.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bi.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bl.shtwfgs.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xn.panjiajie.cn

C#:   s.Replace("a", "b")
来源：http://tg.colortex.cn

[E07] 按分隔符拆分
来源：http://ha.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ls.haigaiapp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://na.hnjuh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ak.hahajie.cn

TS:   s.split(",")
来源：http://fb.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://li.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zm.521024.cn

Ruby: s.split(",");  s.split
来源：http://yt.yuexingan06.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qp.panjiajie.cn

[E08] 数组按分隔符合并
来源：http://jz.haigaiapp.cn

Py:   ",".join(items)
来源：http://jx.panjiajie.cn

PHP:  implode(",", $items);
来源：http://wg.colortex.cn

JS:   items.join(",")
来源：http://vo.hnjuh.cn

TS:   items.join(",")
来源：http://cc.muxihuayi.cn

Java: String.join(",", items)
来源：http://lr.newstarts.cn

Go:   strings.Join(items, ",")
来源：http://vj.shxzukj.cn

Ruby: items.join(",")
来源：http://gh.szsharing.cn

C#:   string.Join(",", items)
来源：http://dq.szxytkj.cn

[E09] 去除所有空白字符
来源：http://jy.muxihuayi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oe.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ir.9csxet.cn

JS:   s.replace(/\s+/g, "")
来源：http://mw.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://ym.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://eq.huixinmuqiang.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://oo.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vs.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mi.9csxet.cn

[E10] 左侧补零 / 定长填充
来源：http://iu.nszjky.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://vu.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://le.hahajie.cn

JS:   "7".padStart(3, "0")
来源：http://oy.bjjhwx.cn

TS:   "7".padStart(3, "0")
来源：http://be.huixinmuqiang.cn

Java: String.format("%03d", 7)
来源：http://kf.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ck.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lv.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ee.haigaiapp.cn

[E11] 反转字符串
来源：http://yh.yuntaijiaju.cn

Py:   s[::-1]
来源：http://zp.bookmarksfly.cn

PHP:  strrev($s);
来源：http://ky.lnxyls.cn

JS:   [...s].reverse().join("")
来源：http://gu.hahajie.cn

TS:   [...s].reverse().join("")
来源：http://vp.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rb.yuntaijiaju.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://st.haigaiapp.cn

Ruby: s.reverse
来源：http://mf.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://fo.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://wa.newstarts.cn

Py:   s.count("a")
来源：http://me.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://pu.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://vk.bjjhwx.cn

TS:   s.split("a").length - 1
来源：http://lv.haigaiapp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ib.bjjhwx.cn

Go:   strings.Count(s, "a")
来源：http://rf.huixiangedu.cn

Ruby: s.count("a")
来源：http://gs.yuntaijiaju.cn

C#:   s.Count(c => c == 'a')
来源：http://rv.colortex.cn

[E13] 逐字符遍历
来源：http://yo.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://nd.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kk.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nd.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xp.shxzukj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kw.nicolike.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bj.asd995.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sb.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vb.newstarts.cn

[E14] URL 编码与 Base64
来源：http://on.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qm.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gf.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vu.bookmarksfly.cn


<!-- 参考信息 -->