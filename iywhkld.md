代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xr.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ga.yuntaijiaju.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cb.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://oj.haigaiapp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://lt.gzmigu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qz.chemitech.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://bo.huanxung.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ij.huanxung.cn

[D11] 反转数组
来源：http://fo.asd995.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wb.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://yk.shxzukj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dg.jianghongdianzi.cn

TS:   [...arr].reverse();
来源：http://ob.hnjuh.cn

Java: Collections.reverse(list);
来源：http://gl.nszjky.cn

Go:   slices.Reverse(arr)
来源：http://za.haigaiapp.cn

Ruby: arr.reverse
来源：http://sg.bjjhwx.cn

C#:   list.Reverse();
来源：http://ut.muxihuayi.cn

[D12] 查找元素下标
来源：http://vp.jianghongdianzi.cn

Py:   arr.index(x);  x in arr
来源：http://rs.nicolike.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lv.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fe.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fz.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vi.wgjwhj.cn

Go:   slices.Index(arr, x)
来源：http://vn.wgjwhj.cn

Ruby: arr.index(x)
来源：http://qy.szsharing.cn

C#:   list.IndexOf(x);
来源：http://tl.gzmigu.cn

[D13] 过滤（保留满足条件的）
来源：http://vo.haigaiapp.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://bs.shxzukj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://af.wgjwhj.cn

JS:   arr.filter(x => x > 3)
来源：http://ry.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://dm.jianghongdianzi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pk.huixiangedu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wb.wgjwhj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://cx.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://rs.huixiangedu.cn

[D14] 映射转换（每个元素变形）
来源：http://hb.panjiajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kc.hnjuh.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://tv.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://cw.jianghongdianzi.cn

TS:   arr.map(x => x * 2)
来源：http://oa.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://vm.lnxyls.cn

Go:   // 手写循环
来源：http://ay.nszjky.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ko.nszjky.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://jy.shxzskj.cn

[D15] 去重
来源：http://ky.szxytkj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vh.nszjky.cn

PHP:  array_unique($arr);
来源：http://lx.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://tl.521024.cn

TS:   [...new Set(arr)]
来源：http://iw.hahajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mz.szxytkj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://dr.newstarts.cn

Ruby: arr.uniq
来源：http://sq.huanxung.cn

C#:   list.Distinct().ToList()
来源：http://ta.hnjuh.cn

[D16] 求和与平均值
来源：http://st.haigaiapp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://yh.shxzskj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ev.yuntaijiaju.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yr.szxytkj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ir.muxihuayi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://qb.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://jd.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bb.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://jr.bookmarksfly.cn

[D17] 最大值与最小值
来源：http://uj.newstarts.cn

Py:   max(arr);  min(arr)
来源：http://sy.hahajie.cn

PHP:  max($arr);  min($arr);
来源：http://xz.gzmigu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hk.yuntaijiaju.cn

TS:   Math.max(...arr);
来源：http://fq.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://tf.huanxung.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://uu.shtwfgs.cn

Ruby: arr.max;  arr.min
来源：http://kl.shtwfgs.cn

C#:   list.Max();  list.Min()
来源：http://zv.haigaiapp.cn

[D18] 扁平化嵌套数组
来源：http://ox.colortex.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://gw.nicolike.cn

PHP:  array_merge(...$nested);
来源：http://cf.yuexingan06.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jn.jianghongdianzi.cn

TS:   nested.flat();
来源：http://ku.wgjwhj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ls.521024.cn

Go:   // 手写双层循环
来源：http://bb.newstarts.cn

Ruby: nested.flatten
来源：http://nl.muxihuayi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xt.newstarts.cn

[D19] 按字段分组
来源：http://as.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qj.newstarts.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ra.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://de.gzmigu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mg.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://aj.gzmigu.cn

Go:   // 手写 map[string][]T
来源：http://kt.haigaiapp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nw.gzmigu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://nr.shxzskj.cn

[D20] 统计每个元素出现次数
来源：http://gk.521024.cn

Py:   Counter(arr)
来源：http://sf.colortex.cn

PHP:  array_count_values($arr);
来源：http://tm.panjiajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wa.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sc.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ij.huanxung.cn

Go:   // 手写 map[T]int
来源：http://jm.newstarts.cn

Ruby: arr.tally
来源：http://mo.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ch.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://tj.szsharing.cn

Py:   x in arr
来源：http://lf.muxihuayi.cn

PHP:  in_array($x, $arr, true);
来源：http://en.lnxyls.cn

JS:   arr.includes(x)
来源：http://gy.huanxung.cn

TS:   arr.includes(x)
来源：http://pv.shtwfgs.cn

Java: list.contains(x)
来源：http://qy.bookmarksfly.cn

Go:   slices.Contains(arr, x)
来源：http://aa.huixiangedu.cn

Ruby: arr.include?(x)
来源：http://sa.nicolike.cn

C#:   list.Contains(x)
来源：http://am.nicolike.cn

[D22] 复制数组（避免共享引用）
来源：http://bp.szsharing.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wn.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ii.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://jp.huixiangedu.cn

TS:   [...arr];
来源：http://ha.9csxet.cn

Java: new ArrayList<>(list);
来源：http://ky.chemitech.net.cn

Go:   copied := append([]int(nil), arr...)
来源：http://as.muxihuayi.cn

Ruby: arr.dup;  arr.clone
来源：http://ks.nicolike.cn

C#:   new List<int>(list);
来源：http://mb.huixinmuqiang.cn

[D23] reduce 累积计算
来源：http://cg.colortex.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xo.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://bd.muxihuayi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dq.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rb.chemitech.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yk.bjjhwx.cn

Go:   // 手写循环
来源：http://ix.shxzukj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kw.huixinmuqiang.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gv.yuntaijiaju.cn

[D24] 字典 / Map 基本操作
来源：http://ls.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://jz.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pc.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://cd.shxzukj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rk.haigaiapp.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://kc.lnxyls.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://df.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://jb.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vk.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://md.shxzukj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://iy.gzmigu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yp.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zd.bookmarksfly.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://aq.lnxyls.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mz.chemitech.net.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ka.asd995.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://to.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fq.9csxet.cn

[D26] 数组转字符串
来源：http://xw.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://jb.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://ui.panjiajie.cn

JS:   arr.join(", ")
来源：http://sj.muxihuayi.cn

TS:   arr.join(", ")
来源：http://rx.yuntaijiaju.cn

Java: String.join(", ", list)
来源：http://xd.bjjhwx.cn

Go:   strings.Join(strs, ", ")
来源：http://cw.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://fz.nicolike.cn

C#:   string.Join(", ", list)
来源：http://ba.huanxung.cn

================================================================================
来源：http://ns.asd995.cn

E. 字符串处理
来源：http://mn.shtwfgs.cn

================================================================================
来源：http://ax.lnxyls.cn

[E01] 拼接字符串
来源：http://dr.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yl.jianghongdianzi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://et.bookmarksfly.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kr.haigaiapp.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ej.szsharing.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://xt.asd995.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lc.haigaiapp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cp.newstarts.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sm.bookmarksfly.cn

[E02] 重复字符串
来源：http://gu.hahajie.cn

Py:   "ab" * 3
来源：http://yn.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://kp.lnxyls.cn

JS:   "ab".repeat(3)
来源：http://jh.asd995.cn

TS:   "ab".repeat(3)
来源：http://at.szxytkj.cn

Java: "ab".repeat(3)
来源：http://qb.shtwfgs.cn

Go:   strings.Repeat("ab", 3)
来源：http://ox.yuntaijiaju.cn

Ruby: "ab" * 3
来源：http://kv.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zh.jianghongdianzi.cn

[E03] 截取子串
来源：http://wz.shtwfgs.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ax.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ym.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://yr.yuexingan06.cn

TS:   s.slice(1, 4)
来源：http://tj.asd995.cn

Java: s.substring(1, 4)
来源：http://re.colortex.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ai.bookmarksfly.cn

Ruby: s[1, 3];  s[1..3]
来源：http://qy.huixiangedu.cn

C#:   s.Substring(1, 3)
来源：http://kr.huixiangedu.cn

[E04] 查找子串位置
来源：http://rf.asd995.cn

Py:   s.find("x");  s.index("x")
来源：http://tp.colortex.cn

PHP:  strpos($s, "x");
来源：http://md.yuexingan06.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yw.hahajie.cn

TS:   s.indexOf("x")
来源：http://vh.9csxet.cn

Java: s.indexOf("x")
来源：http://zg.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://zu.9csxet.cn

Ruby: s.index("x")
来源：http://xf.huixinmuqiang.cn

C#:   s.IndexOf("x")
来源：http://rl.shtwfgs.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bs.bjjhwx.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wx.newstarts.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bp.newstarts.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://no.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tn.panjiajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fk.shtwfgs.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yv.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://og.wgjwhj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ft.colortex.cn

[E06] 替换子串
来源：http://qq.muxihuayi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xz.hahajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://px.jianghongdianzi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ry.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://di.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rf.muxihuayi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://vq.huixiangedu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wf.521024.cn

C#:   s.Replace("a", "b")
来源：http://qx.wgjwhj.cn

[E07] 按分隔符拆分
来源：http://pj.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ws.shxzukj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://lt.huixiangedu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://eb.wgjwhj.cn

TS:   s.split(",")
来源：http://bw.gzmigu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bp.hnjuh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jh.hnjuh.cn

Ruby: s.split(",");  s.split
来源：http://zp.chemitech.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://je.asd995.cn

[E08] 数组按分隔符合并
来源：http://bs.shtwfgs.cn

Py:   ",".join(items)
来源：http://qu.szsharing.cn

PHP:  implode(",", $items);
来源：http://zv.colortex.cn

JS:   items.join(",")
来源：http://qc.wgjwhj.cn

TS:   items.join(",")
来源：http://tb.shtwfgs.cn

Java: String.join(",", items)
来源：http://ee.asd995.cn

Go:   strings.Join(items, ",")
来源：http://ie.nicolike.cn

Ruby: items.join(",")
来源：http://oy.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://bi.panjiajie.cn

[E09] 去除所有空白字符
来源：http://fl.nszjky.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bh.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nu.szsharing.cn

JS:   s.replace(/\s+/g, "")
来源：http://dj.hahajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://hv.gzmigu.cn

Java: s.replaceAll("\\s+", "")
来源：http://by.newstarts.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jr.9csxet.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xg.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tj.muxihuayi.cn

[E10] 左侧补零 / 定长填充
来源：http://en.wgjwhj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ve.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://du.huixinmuqiang.cn

JS:   "7".padStart(3, "0")
来源：http://eu.colortex.cn

TS:   "7".padStart(3, "0")
来源：http://az.bjjhwx.cn

Java: String.format("%03d", 7)
来源：http://yx.jctech888.com.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ya.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kr.huixiangedu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rw.lnxyls.cn

[E11] 反转字符串
来源：http://tr.colortex.cn

Py:   s[::-1]
来源：http://lt.huanxung.cn

PHP:  strrev($s);
来源：http://mm.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://hs.shtwfgs.cn

TS:   [...s].reverse().join("")
来源：http://mf.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sw.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://er.shxzukj.cn

Ruby: s.reverse
来源：http://ai.shxzskj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://it.nicolike.cn

[E12] 统计某字符出现次数
来源：http://vr.nicolike.cn

Py:   s.count("a")
来源：http://rg.nicolike.cn

PHP:  substr_count($s, "a");
来源：http://cq.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://pz.muxihuayi.cn

TS:   s.split("a").length - 1
来源：http://wj.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gv.jianghongdianzi.cn

Go:   strings.Count(s, "a")
来源：http://gj.colortex.cn

Ruby: s.count("a")
来源：http://ml.hahajie.cn

C#:   s.Count(c => c == 'a')
来源：http://uo.huanxung.cn

[E13] 逐字符遍历
来源：http://hn.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://bw.yuexingan06.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wh.hnjuh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rl.hahajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ej.gzmigu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://dy.bookmarksfly.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wd.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://iq.haigaiapp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mb.huanxung.cn

[E14] URL 编码与 Base64
来源：http://ar.chemitech.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tk.9csxet.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rz.hahajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mr.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xo.colortex.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://au.gzmigu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ky.newstarts.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zy.wgjwhj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bb.szxytkj.cn

[E15] HTML 转义 / 反转义
来源：http://oe.huixiangedu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ak.jianghongdianzi.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ac.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mk.521024.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rt.wgjwhj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://av.newstarts.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zy.shxzukj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sc.shxzskj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zi.shxzskj.cn

[E16] 数字千分位
来源：http://wr.huanxung.cn

Py:   f"{1234567:,}"
来源：http://wq.nszjky.cn

PHP:  number_format(1234567);
来源：http://eo.newstarts.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://sh.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gw.521024.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://oi.huixiangedu.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wk.yuexingan06.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lk.nszjky.cn

C#:   1234567.ToString("N0")
来源：http://bm.nicolike.cn

[E17] 首字母大写
来源：http://wn.gzmigu.cn


<!-- 参考信息 -->