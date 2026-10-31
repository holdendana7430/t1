代发 wailian999

TS:   [...arr].reverse();
来源：http://vf.lnxyls.cn

Java: Collections.reverse(list);
来源：http://to.yuexingan06.cn

Go:   slices.Reverse(arr)
来源：http://nn.bookmarksfly.cn

Ruby: arr.reverse
来源：http://ya.521024.cn

C#:   list.Reverse();
来源：http://qm.chemitech.net.cn

[D12] 查找元素下标
来源：http://pe.521024.cn

Py:   arr.index(x);  x in arr
来源：http://nw.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://lc.chemitech.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ik.muxihuayi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://la.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ri.bjjhwx.cn

Go:   slices.Index(arr, x)
来源：http://ft.nszjky.cn

Ruby: arr.index(x)
来源：http://ma.shtwfgs.cn

C#:   list.IndexOf(x);
来源：http://co.shtwfgs.cn

[D13] 过滤（保留满足条件的）
来源：http://ta.bookmarksfly.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jg.panjiajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ci.huixinmuqiang.cn

JS:   arr.filter(x => x > 3)
来源：http://ar.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://dk.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pw.huanxung.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wu.szsharing.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ia.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dw.lnxyls.cn

[D14] 映射转换（每个元素变形）
来源：http://py.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zh.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jt.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://sg.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://yz.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ig.hnjuh.cn

Go:   // 手写循环
来源：http://uo.521024.cn

Ruby: arr.map { |x| x * 2 }
来源：http://us.yuexingan06.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://su.nszjky.cn

[D15] 去重
来源：http://lq.szxytkj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://bh.muxihuayi.cn

PHP:  array_unique($arr);
来源：http://ja.asd995.cn

JS:   [...new Set(arr)]
来源：http://oh.lnxyls.cn

TS:   [...new Set(arr)]
来源：http://fs.lnxyls.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jx.nszjky.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ue.bjjhwx.cn

Ruby: arr.uniq
来源：http://rv.muxihuayi.cn

C#:   list.Distinct().ToList()
来源：http://lx.jianghongdianzi.cn

[D16] 求和与平均值
来源：http://ie.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://lz.jianghongdianzi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://qs.szxytkj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://py.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://rd.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bj.521024.cn

Go:   // 手写循环累加
来源：http://rz.lnxyls.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://zb.shtwfgs.cn

C#:   list.Sum();  list.Average()
来源：http://yo.shtwfgs.cn

[D17] 最大值与最小值
来源：http://qo.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://uk.yuntaijiaju.cn

PHP:  max($arr);  min($arr);
来源：http://ib.gzmigu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xu.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://jp.huixinmuqiang.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bi.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://zb.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://hi.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://ig.asd995.cn

[D18] 扁平化嵌套数组
来源：http://af.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dk.gzmigu.cn

PHP:  array_merge(...$nested);
来源：http://lt.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://jg.nszjky.cn

TS:   nested.flat();
来源：http://la.panjiajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uf.521024.cn

Go:   // 手写双层循环
来源：http://ii.asd995.cn

Ruby: nested.flatten
来源：http://yn.colortex.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://td.panjiajie.cn

[D19] 按字段分组
来源：http://lx.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ws.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dm.gzmigu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kz.jianghongdianzi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bm.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sx.huixiangedu.cn

Go:   // 手写 map[string][]T
来源：http://zu.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://vv.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://me.huanxung.cn

[D20] 统计每个元素出现次数
来源：http://ab.jianghongdianzi.cn

Py:   Counter(arr)
来源：http://vk.muxihuayi.cn

PHP:  array_count_values($arr);
来源：http://vm.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ej.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zr.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gg.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://ip.newstarts.cn

Ruby: arr.tally
来源：http://gd.hnjuh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://io.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://pj.nszjky.cn

Py:   x in arr
来源：http://ug.muxihuayi.cn

PHP:  in_array($x, $arr, true);
来源：http://ni.nicolike.cn

JS:   arr.includes(x)
来源：http://kp.lnxyls.cn

TS:   arr.includes(x)
来源：http://si.jianghongdianzi.cn

Java: list.contains(x)
来源：http://pf.newstarts.cn

Go:   slices.Contains(arr, x)
来源：http://lc.nszjky.cn

Ruby: arr.include?(x)
来源：http://sx.jianghongdianzi.cn

C#:   list.Contains(x)
来源：http://oz.bookmarksfly.cn

[D22] 复制数组（避免共享引用）
来源：http://ee.huanxung.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://bo.yuexingan06.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://yv.wgjwhj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://va.colortex.cn

TS:   [...arr];
来源：http://hh.gzmigu.cn

Java: new ArrayList<>(list);
来源：http://ud.colortex.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rv.asd995.cn

Ruby: arr.dup;  arr.clone
来源：http://as.wgjwhj.cn

C#:   new List<int>(list);
来源：http://zp.nszjky.cn

[D23] reduce 累积计算
来源：http://wa.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://kd.shtwfgs.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ia.asd995.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gb.bookmarksfly.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ug.huixinmuqiang.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ls.hnjuh.cn

Go:   // 手写循环
来源：http://om.gzmigu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gr.chemitech.net.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ym.asd995.cn

[D24] 字典 / Map 基本操作
来源：http://np.lnxyls.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://py.chemitech.net.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://th.nicolike.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ar.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kg.hnjuh.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qz.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lh.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dp.521024.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://di.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://ya.szsharing.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ll.haigaiapp.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://pw.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://yj.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qs.hahajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wk.wgjwhj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://kx.newstarts.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ag.wgjwhj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xy.yuntaijiaju.cn

[D26] 数组转字符串
来源：http://la.yuntaijiaju.cn

Py:   ", ".join(map(str, arr))
来源：http://hu.hnjuh.cn

PHP:  implode(", ", $arr);
来源：http://mt.shxzukj.cn

JS:   arr.join(", ")
来源：http://np.hahajie.cn

TS:   arr.join(", ")
来源：http://nx.shxzskj.cn

Java: String.join(", ", list)
来源：http://hb.jianghongdianzi.cn

Go:   strings.Join(strs, ", ")
来源：http://iz.nszjky.cn

Ruby: arr.join(", ")
来源：http://qb.asd995.cn

C#:   string.Join(", ", list)
来源：http://xy.szxytkj.cn

================================================================================
来源：http://yy.yuexingan06.cn

E. 字符串处理
来源：http://bd.chemitech.net.cn

================================================================================
来源：http://mw.huixinmuqiang.cn

[E01] 拼接字符串
来源：http://ud.szxytkj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ch.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ml.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ne.szxytkj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://gx.shtwfgs.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ra.huixinmuqiang.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vk.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rf.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://or.szsharing.cn

[E02] 重复字符串
来源：http://ra.9csxet.cn

Py:   "ab" * 3
来源：http://yn.panjiajie.cn

PHP:  str_repeat("ab", 3);
来源：http://rx.panjiajie.cn

JS:   "ab".repeat(3)
来源：http://ue.nszjky.cn

TS:   "ab".repeat(3)
来源：http://qq.huanxung.cn

Java: "ab".repeat(3)
来源：http://oh.9csxet.cn

Go:   strings.Repeat("ab", 3)
来源：http://ip.huanxung.cn

Ruby: "ab" * 3
来源：http://fb.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lf.bookmarksfly.cn

[E03] 截取子串
来源：http://fq.huanxung.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pm.huixinmuqiang.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kx.szsharing.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fr.chemitech.net.cn

TS:   s.slice(1, 4)
来源：http://lt.hnjuh.cn

Java: s.substring(1, 4)
来源：http://pj.hahajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sv.colortex.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jw.bookmarksfly.cn

C#:   s.Substring(1, 3)
来源：http://ht.nicolike.cn

[E04] 查找子串位置
来源：http://pb.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://or.yuntaijiaju.cn

PHP:  strpos($s, "x");
来源：http://md.521024.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zd.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://nj.asd995.cn

Java: s.indexOf("x")
来源：http://gt.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://kp.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://ao.szsharing.cn

C#:   s.IndexOf("x")
来源：http://oy.bookmarksfly.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://vr.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ui.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ca.lnxyls.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://no.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nr.nszjky.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ok.chemitech.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sx.bookmarksfly.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ch.hnjuh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ng.haigaiapp.cn

[E06] 替换子串
来源：http://jv.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sa.shtwfgs.cn

PHP:  str_replace("a", "b", $s);
来源：http://hw.gzmigu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ot.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://wy.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kv.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://kz.yuntaijiaju.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qe.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://qm.jctech888.com.cn

[E07] 按分隔符拆分
来源：http://qz.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://da.lnxyls.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gf.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nb.szxytkj.cn

TS:   s.split(",")
来源：http://ah.lnxyls.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jp.panjiajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ye.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://ws.hnjuh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://uu.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://tn.jctech888.com.cn

Py:   ",".join(items)
来源：http://kv.colortex.cn

PHP:  implode(",", $items);
来源：http://ee.haigaiapp.cn

JS:   items.join(",")
来源：http://qo.shxzukj.cn

TS:   items.join(",")
来源：http://kl.asd995.cn

Java: String.join(",", items)
来源：http://tv.huixiangedu.cn

Go:   strings.Join(items, ",")
来源：http://ho.9csxet.cn

Ruby: items.join(",")
来源：http://gx.chemitech.net.cn

C#:   string.Join(",", items)
来源：http://ke.szxytkj.cn

[E09] 去除所有空白字符
来源：http://dz.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ge.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://aj.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://tb.jianghongdianzi.cn

TS:   s.replace(/\s+/g, "")
来源：http://ms.wgjwhj.cn

Java: s.replaceAll("\\s+", "")
来源：http://uc.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yb.newstarts.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xt.nicolike.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ox.chemitech.net.cn

[E10] 左侧补零 / 定长填充
来源：http://qq.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://je.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wr.huanxung.cn

JS:   "7".padStart(3, "0")
来源：http://zr.lnxyls.cn

TS:   "7".padStart(3, "0")
来源：http://sn.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://ut.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://sa.nszjky.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://iw.colortex.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ga.shxzukj.cn

[E11] 反转字符串
来源：http://kn.bookmarksfly.cn

Py:   s[::-1]
来源：http://qs.muxihuayi.cn

PHP:  strrev($s);
来源：http://wm.huixinmuqiang.cn

JS:   [...s].reverse().join("")
来源：http://oc.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://az.huixiangedu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ch.huixiangedu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ni.bjjhwx.cn

Ruby: s.reverse
来源：http://ey.bookmarksfly.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ox.szsharing.cn

[E12] 统计某字符出现次数
来源：http://gp.shtwfgs.cn

Py:   s.count("a")
来源：http://fg.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://ch.gzmigu.cn

JS:   s.split("a").length - 1
来源：http://xj.hnjuh.cn

TS:   s.split("a").length - 1
来源：http://xi.haigaiapp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kq.bjjhwx.cn

Go:   strings.Count(s, "a")
来源：http://ns.bookmarksfly.cn

Ruby: s.count("a")
来源：http://im.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://fe.bjjhwx.cn

[E13] 逐字符遍历
来源：http://yx.asd995.cn

Py:   for ch in s: print(ch)
来源：http://ty.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dp.shxzukj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ae.lnxyls.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://cn.shxzskj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ut.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pt.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vb.bjjhwx.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dp.yuntaijiaju.cn

[E14] URL 编码与 Base64
来源：http://gs.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hv.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yw.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ce.newstarts.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://uf.bjjhwx.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pd.szxytkj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mr.colortex.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pd.lnxyls.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dq.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://cc.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ee.yuntaijiaju.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jc.huixiangedu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dc.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://en.nszjky.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hi.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gx.9csxet.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mc.nicolike.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ai.huixiangedu.cn

[E16] 数字千分位
来源：http://ou.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://dc.szsharing.cn

PHP:  number_format(1234567);
来源：http://he.shxzskj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qx.huixinmuqiang.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://io.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://cz.newstarts.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://cz.colortex.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://uf.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://xl.shtwfgs.cn

[E17] 首字母大写
来源：http://wp.9csxet.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ox.jctech888.com.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yk.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zb.wgjwhj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://es.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jf.shtwfgs.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pu.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://nn.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kt.hnjuh.cn

[E18] 模板占位符替换
来源：http://ez.panjiajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ud.chemitech.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kz.panjiajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ns.bjjhwx.cn


<!-- 参考信息 -->