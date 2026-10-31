代发 wailian999

Ruby: arr.index(x)
来源：http://ig.wgjwhj.cn

C#:   list.IndexOf(x);
来源：http://nw.huixinmuqiang.cn

[D13] 过滤（保留满足条件的）
来源：http://ne.gzmigu.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ha.nszjky.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://id.jianghongdianzi.cn

JS:   arr.filter(x => x > 3)
来源：http://sr.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://kz.szsharing.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fg.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lj.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xr.jctech888.com.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://bb.muxihuayi.cn

[D14] 映射转换（每个元素变形）
来源：http://ss.shtwfgs.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://bm.huanxung.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://zm.hahajie.cn

JS:   arr.map(x => x * 2)
来源：http://qh.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://qe.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://el.chemitech.net.cn

Go:   // 手写循环
来源：http://ey.szxytkj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hy.521024.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://vi.asd995.cn

[D15] 去重
来源：http://dr.szsharing.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://as.huanxung.cn

PHP:  array_unique($arr);
来源：http://bi.huanxung.cn

JS:   [...new Set(arr)]
来源：http://gn.colortex.cn

TS:   [...new Set(arr)]
来源：http://nv.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://jm.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://af.nszjky.cn

Ruby: arr.uniq
来源：http://dh.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://oy.yuexingan06.cn

[D16] 求和与平均值
来源：http://as.haigaiapp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bm.haigaiapp.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yq.yuexingan06.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ps.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ic.bjjhwx.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zz.chemitech.net.cn

Go:   // 手写循环累加
来源：http://pl.haigaiapp.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fp.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://ct.newstarts.cn

[D17] 最大值与最小值
来源：http://kt.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://za.jianghongdianzi.cn

PHP:  max($arr);  min($arr);
来源：http://yg.panjiajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://cb.lnxyls.cn

TS:   Math.max(...arr);
来源：http://mk.huixinmuqiang.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://cl.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ln.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://ki.nicolike.cn

C#:   list.Max();  list.Min()
来源：http://aq.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://pp.szxytkj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://oh.szxytkj.cn

PHP:  array_merge(...$nested);
来源：http://xl.szxytkj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ml.panjiajie.cn

TS:   nested.flat();
来源：http://pu.lnxyls.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://of.huixinmuqiang.cn

Go:   // 手写双层循环
来源：http://sl.colortex.cn

Ruby: nested.flatten
来源：http://iz.szsharing.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://li.haigaiapp.cn

[D19] 按字段分组
来源：http://pk.9csxet.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ww.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vw.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ar.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://mp.521024.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gz.colortex.cn

Go:   // 手写 map[string][]T
来源：http://dq.yuntaijiaju.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ib.wgjwhj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mi.bjjhwx.cn

[D20] 统计每个元素出现次数
来源：http://di.haigaiapp.cn

Py:   Counter(arr)
来源：http://ez.yuexingan06.cn

PHP:  array_count_values($arr);
来源：http://lt.gzmigu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ck.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://gj.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gm.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://yp.hnjuh.cn

Ruby: arr.tally
来源：http://gp.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://df.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://de.colortex.cn

Py:   x in arr
来源：http://hv.gzmigu.cn

PHP:  in_array($x, $arr, true);
来源：http://pz.lnxyls.cn

JS:   arr.includes(x)
来源：http://yr.huanxung.cn

TS:   arr.includes(x)
来源：http://is.nszjky.cn

Java: list.contains(x)
来源：http://sr.szxytkj.cn

Go:   slices.Contains(arr, x)
来源：http://hf.shxzukj.cn

Ruby: arr.include?(x)
来源：http://qr.wgjwhj.cn

C#:   list.Contains(x)
来源：http://bv.huixinmuqiang.cn

[D22] 复制数组（避免共享引用）
来源：http://gk.hahajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ko.wgjwhj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://bf.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ok.shtwfgs.cn

TS:   [...arr];
来源：http://lr.asd995.cn

Java: new ArrayList<>(list);
来源：http://ui.shxzskj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ps.9csxet.cn

Ruby: arr.dup;  arr.clone
来源：http://ul.nicolike.cn

C#:   new List<int>(list);
来源：http://du.newstarts.cn

[D23] reduce 累积计算
来源：http://uu.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bf.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pc.wgjwhj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ad.yuntaijiaju.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ji.hnjuh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ep.huixiangedu.cn

Go:   // 手写循环
来源：http://ul.asd995.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wd.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ue.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://mf.huanxung.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pm.gzmigu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://me.gzmigu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ie.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://au.wgjwhj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://as.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://uc.huixinmuqiang.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://gb.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://td.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://qw.gzmigu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qc.huixiangedu.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hi.bjjhwx.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lq.gzmigu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pq.huixiangedu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wa.newstarts.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://xq.shtwfgs.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ov.colortex.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zt.huixiangedu.cn

[D26] 数组转字符串
来源：http://py.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://bz.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://eo.521024.cn

JS:   arr.join(", ")
来源：http://ur.nszjky.cn

TS:   arr.join(", ")
来源：http://xo.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://js.bookmarksfly.cn

Go:   strings.Join(strs, ", ")
来源：http://zi.nicolike.cn

Ruby: arr.join(", ")
来源：http://mh.9csxet.cn

C#:   string.Join(", ", list)
来源：http://ac.muxihuayi.cn

================================================================================
来源：http://mv.bjjhwx.cn

E. 字符串处理
来源：http://hq.521024.cn

================================================================================
来源：http://gi.newstarts.cn

[E01] 拼接字符串
来源：http://nd.shxzukj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rk.panjiajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qx.chemitech.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kn.jianghongdianzi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ek.nicolike.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cb.haigaiapp.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cx.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://az.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mb.9csxet.cn

[E02] 重复字符串
来源：http://yd.9csxet.cn

Py:   "ab" * 3
来源：http://nq.panjiajie.cn

PHP:  str_repeat("ab", 3);
来源：http://yl.yuntaijiaju.cn

JS:   "ab".repeat(3)
来源：http://tl.gzmigu.cn

TS:   "ab".repeat(3)
来源：http://qf.wgjwhj.cn

Java: "ab".repeat(3)
来源：http://ve.yuexingan06.cn

Go:   strings.Repeat("ab", 3)
来源：http://mv.gzmigu.cn

Ruby: "ab" * 3
来源：http://yk.gzmigu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://jr.szxytkj.cn

[E03] 截取子串
来源：http://tw.huixiangedu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ax.bookmarksfly.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kb.hnjuh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ty.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://jo.asd995.cn

Java: s.substring(1, 4)
来源：http://dh.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qi.521024.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zp.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://ua.hnjuh.cn

[E04] 查找子串位置
来源：http://zd.asd995.cn

Py:   s.find("x");  s.index("x")
来源：http://fj.yuexingan06.cn

PHP:  strpos($s, "x");
来源：http://wd.szsharing.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://je.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://nk.bjjhwx.cn

Java: s.indexOf("x")
来源：http://qh.newstarts.cn

Go:   strings.Index(s, "x")
来源：http://qp.yuntaijiaju.cn

Ruby: s.index("x")
来源：http://ru.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://iv.szsharing.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ns.bjjhwx.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://yt.jianghongdianzi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gi.huixiangedu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wn.9csxet.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ym.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xk.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dn.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yq.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bq.hahajie.cn

[E06] 替换子串
来源：http://ey.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://bu.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://fi.shtwfgs.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xj.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://eb.bookmarksfly.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ra.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gg.shtwfgs.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fl.szsharing.cn

C#:   s.Replace("a", "b")
来源：http://wz.jianghongdianzi.cn

[E07] 按分隔符拆分
来源：http://qk.shxzskj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cy.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://me.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gr.bjjhwx.cn

TS:   s.split(",")
来源：http://df.yuexingan06.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ks.yuexingan06.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zq.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://gr.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kt.bookmarksfly.cn

[E08] 数组按分隔符合并
来源：http://eh.shxzskj.cn

Py:   ",".join(items)
来源：http://eu.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://ow.gzmigu.cn

JS:   items.join(",")
来源：http://nw.521024.cn

TS:   items.join(",")
来源：http://gh.huixiangedu.cn

Java: String.join(",", items)
来源：http://zv.asd995.cn

Go:   strings.Join(items, ",")
来源：http://dv.wgjwhj.cn

Ruby: items.join(",")
来源：http://pl.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://er.szxytkj.cn

[E09] 去除所有空白字符
来源：http://vm.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hq.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://le.panjiajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://iz.huixinmuqiang.cn

TS:   s.replace(/\s+/g, "")
来源：http://xo.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://rz.newstarts.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fu.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sc.bookmarksfly.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hh.gzmigu.cn

[E10] 左侧补零 / 定长填充
来源：http://eo.yuntaijiaju.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ri.nszjky.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://od.asd995.cn

JS:   "7".padStart(3, "0")
来源：http://ft.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://fh.jianghongdianzi.cn

Java: String.format("%03d", 7)
来源：http://wz.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cv.haigaiapp.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://or.yuntaijiaju.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yk.jctech888.com.cn

[E11] 反转字符串
来源：http://me.hahajie.cn

Py:   s[::-1]
来源：http://nd.haigaiapp.cn

PHP:  strrev($s);
来源：http://ua.shtwfgs.cn

JS:   [...s].reverse().join("")
来源：http://wk.jianghongdianzi.cn

TS:   [...s].reverse().join("")
来源：http://qh.huixiangedu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cx.newstarts.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hm.huixiangedu.cn

Ruby: s.reverse
来源：http://ir.jianghongdianzi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hk.wgjwhj.cn

[E12] 统计某字符出现次数
来源：http://dm.521024.cn

Py:   s.count("a")
来源：http://du.yuntaijiaju.cn

PHP:  substr_count($s, "a");
来源：http://ki.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://su.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://uv.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lj.nicolike.cn

Go:   strings.Count(s, "a")
来源：http://rv.gzmigu.cn

Ruby: s.count("a")
来源：http://pb.shtwfgs.cn

C#:   s.Count(c => c == 'a')
来源：http://mc.shtwfgs.cn

[E13] 逐字符遍历
来源：http://nk.lnxyls.cn

Py:   for ch in s: print(ch)
来源：http://gg.shxzukj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ko.shxzukj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://cw.lnxyls.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ve.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gn.bjjhwx.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ua.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tw.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ww.521024.cn

[E14] URL 编码与 Base64
来源：http://lk.gzmigu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://de.szsharing.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ja.hnjuh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qr.colortex.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ak.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yd.hnjuh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ww.newstarts.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fa.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ae.shtwfgs.cn

[E15] HTML 转义 / 反转义
来源：http://si.szxytkj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ju.jctech888.com.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jc.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zf.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://mm.hnjuh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ly.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xb.bjjhwx.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vw.hahajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bk.yuexingan06.cn

[E16] 数字千分位
来源：http://ag.colortex.cn

Py:   f"{1234567:,}"
来源：http://dq.shtwfgs.cn

PHP:  number_format(1234567);
来源：http://mu.9csxet.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nz.hahajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vk.jctech888.com.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://um.9csxet.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ol.hnjuh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yw.nszjky.cn

C#:   1234567.ToString("N0")
来源：http://jg.jianghongdianzi.cn

[E17] 首字母大写
来源：http://rf.bjjhwx.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cq.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xl.haigaiapp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ak.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ni.haigaiapp.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kt.521024.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nh.9csxet.cn

Ruby: s.capitalize
来源：http://sr.shxzukj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ov.yuntaijiaju.cn

[E18] 模板占位符替换
来源：http://sn.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nq.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://st.hahajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kk.szxytkj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ow.shxzskj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qk.yuexingan06.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ju.yuntaijiaju.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wa.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ww.yuexingan06.cn

[E19] 多行文本按行拆分
来源：http://qh.huixiangedu.cn

Py:   s.splitlines()
来源：http://wy.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gk.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://tc.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://gn.jctech888.com.cn

Java: s.lines().toList()
来源：http://it.nszjky.cn

Go:   strings.Split(s, "\n")
来源：http://ka.521024.cn


<!-- 参考信息 -->