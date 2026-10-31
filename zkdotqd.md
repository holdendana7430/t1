代发 wailian999

C#:   list.Distinct().ToList()
来源：http://pv.colortex.cn

[D16] 求和与平均值
来源：http://bu.9csxet.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dl.wgjwhj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://yb.panjiajie.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://xk.nszjky.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mp.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hy.gzmigu.cn

Go:   // 手写循环累加
来源：http://gi.9csxet.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vl.colortex.cn

C#:   list.Sum();  list.Average()
来源：http://gv.muxihuayi.cn

[D17] 最大值与最小值
来源：http://gz.hahajie.cn

Py:   max(arr);  min(arr)
来源：http://ju.9csxet.cn

PHP:  max($arr);  min($arr);
来源：http://ks.yuexingan06.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://pv.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://dn.shtwfgs.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xo.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hn.nicolike.cn

Ruby: arr.max;  arr.min
来源：http://nb.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://bq.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://da.bookmarksfly.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wn.hahajie.cn

PHP:  array_merge(...$nested);
来源：http://xw.chemitech.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pt.szsharing.cn

TS:   nested.flat();
来源：http://eg.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://dt.panjiajie.cn

Go:   // 手写双层循环
来源：http://sn.szxytkj.cn

Ruby: nested.flatten
来源：http://xp.haigaiapp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://rc.yuexingan06.cn

[D19] 按字段分组
来源：http://je.shtwfgs.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zd.szxytkj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fu.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lq.hnjuh.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://of.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://me.shtwfgs.cn

Go:   // 手写 map[string][]T
来源：http://qa.newstarts.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://by.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fu.nicolike.cn

[D20] 统计每个元素出现次数
来源：http://iz.yuexingan06.cn

Py:   Counter(arr)
来源：http://rb.wgjwhj.cn

PHP:  array_count_values($arr);
来源：http://xu.panjiajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zp.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tc.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yu.wgjwhj.cn

Go:   // 手写 map[T]int
来源：http://jz.shxzukj.cn

Ruby: arr.tally
来源：http://gv.jianghongdianzi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://kl.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://gr.hahajie.cn

Py:   x in arr
来源：http://xm.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://zy.huixinmuqiang.cn

JS:   arr.includes(x)
来源：http://hm.jctech888.com.cn

TS:   arr.includes(x)
来源：http://vp.huixinmuqiang.cn

Java: list.contains(x)
来源：http://tk.hnjuh.cn

Go:   slices.Contains(arr, x)
来源：http://pi.panjiajie.cn

Ruby: arr.include?(x)
来源：http://ap.shxzukj.cn

C#:   list.Contains(x)
来源：http://um.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://yx.bookmarksfly.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://eu.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://of.muxihuayi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://bv.huixinmuqiang.cn

TS:   [...arr];
来源：http://er.yuexingan06.cn

Java: new ArrayList<>(list);
来源：http://ek.shtwfgs.cn

Go:   copied := append([]int(nil), arr...)
来源：http://oa.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://cl.yuexingan06.cn

C#:   new List<int>(list);
来源：http://vj.huixiangedu.cn

[D23] reduce 累积计算
来源：http://lu.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cz.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fi.shxzskj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ph.muxihuayi.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ei.nszjky.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mh.colortex.cn

Go:   // 手写循环
来源：http://sq.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://iv.shxzskj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vz.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://wq.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hv.shxzukj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gs.yuexingan06.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gu.huanxung.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ut.szsharing.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mk.yuntaijiaju.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ui.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://er.newstarts.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lk.hahajie.cn

[D25] Set 集合去重与交并差
来源：http://dz.chemitech.net.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://yo.lnxyls.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ll.colortex.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mm.nicolike.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://zr.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ov.shtwfgs.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rg.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ig.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ys.521024.cn

[D26] 数组转字符串
来源：http://fk.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://ip.asd995.cn

PHP:  implode(", ", $arr);
来源：http://xm.hahajie.cn

JS:   arr.join(", ")
来源：http://ep.gzmigu.cn

TS:   arr.join(", ")
来源：http://hl.newstarts.cn

Java: String.join(", ", list)
来源：http://xj.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://nw.hahajie.cn

Ruby: arr.join(", ")
来源：http://nq.panjiajie.cn

C#:   string.Join(", ", list)
来源：http://nt.jianghongdianzi.cn

================================================================================
来源：http://ee.nszjky.cn

E. 字符串处理
来源：http://yr.colortex.cn

================================================================================
来源：http://aw.newstarts.cn

[E01] 拼接字符串
来源：http://ot.gzmigu.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xs.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ui.szxytkj.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hx.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://je.shtwfgs.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://rn.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bf.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gm.gzmigu.cn

[E02] 重复字符串
来源：http://zz.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://fm.yuexingan06.cn

PHP:  str_repeat("ab", 3);
来源：http://di.nicolike.cn

JS:   "ab".repeat(3)
来源：http://rx.chemitech.net.cn

TS:   "ab".repeat(3)
来源：http://xx.hahajie.cn

Java: "ab".repeat(3)
来源：http://rl.bookmarksfly.cn

Go:   strings.Repeat("ab", 3)
来源：http://vv.gzmigu.cn

Ruby: "ab" * 3
来源：http://yj.chemitech.net.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://oj.szsharing.cn

[E03] 截取子串
来源：http://nm.huixiangedu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bj.szsharing.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://xw.huanxung.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ye.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://wt.521024.cn

Java: s.substring(1, 4)
来源：http://gp.shxzskj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yq.panjiajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://py.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://me.huanxung.cn

[E04] 查找子串位置
来源：http://io.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://fy.nicolike.cn

PHP:  strpos($s, "x");
来源：http://vc.lnxyls.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://qo.bookmarksfly.cn

TS:   s.indexOf("x")
来源：http://ml.shxzskj.cn

Java: s.indexOf("x")
来源：http://vx.haigaiapp.cn

Go:   strings.Index(s, "x")
来源：http://pm.huanxung.cn

Ruby: s.index("x")
来源：http://ov.lnxyls.cn

C#:   s.IndexOf("x")
来源：http://zf.yuntaijiaju.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nv.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fy.szsharing.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ig.nicolike.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gm.huixiangedu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.shxzskj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xu.shxzukj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xj.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gf.nszjky.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dj.nicolike.cn

[E06] 替换子串
来源：http://gp.shxzskj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ki.yuexingan06.cn

PHP:  str_replace("a", "b", $s);
来源：http://uc.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vl.521024.cn

TS:   s.replaceAll("a", "b")
来源：http://sa.szsharing.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gw.asd995.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ap.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://oy.szsharing.cn

C#:   s.Replace("a", "b")
来源：http://kj.asd995.cn

[E07] 按分隔符拆分
来源：http://ro.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fr.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rt.wgjwhj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://py.szsharing.cn

TS:   s.split(",")
来源：http://zx.shxzukj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lp.muxihuayi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ly.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://yi.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dz.chemitech.net.cn

[E08] 数组按分隔符合并
来源：http://cy.bjjhwx.cn

Py:   ",".join(items)
来源：http://nz.huixinmuqiang.cn

PHP:  implode(",", $items);
来源：http://yb.bjjhwx.cn

JS:   items.join(",")
来源：http://ro.huixinmuqiang.cn

TS:   items.join(",")
来源：http://lj.bookmarksfly.cn

Java: String.join(",", items)
来源：http://mo.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://ej.hnjuh.cn

Ruby: items.join(",")
来源：http://it.521024.cn

C#:   string.Join(",", items)
来源：http://va.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://yi.wgjwhj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ow.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bb.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://fx.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://gy.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://ch.wgjwhj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bb.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nw.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nb.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://pb.lnxyls.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ah.yuntaijiaju.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ps.gzmigu.cn

JS:   "7".padStart(3, "0")
来源：http://xx.9csxet.cn

TS:   "7".padStart(3, "0")
来源：http://vc.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://nk.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nz.huixiangedu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://bc.gzmigu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ic.muxihuayi.cn

[E11] 反转字符串
来源：http://vh.shxzskj.cn

Py:   s[::-1]
来源：http://mg.panjiajie.cn

PHP:  strrev($s);
来源：http://ha.jctech888.com.cn

JS:   [...s].reverse().join("")
来源：http://dc.muxihuayi.cn

TS:   [...s].reverse().join("")
来源：http://gw.bookmarksfly.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uo.wgjwhj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://aa.9csxet.cn

Ruby: s.reverse
来源：http://zd.521024.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vn.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://tk.chemitech.net.cn

Py:   s.count("a")
来源：http://de.gzmigu.cn

PHP:  substr_count($s, "a");
来源：http://ze.yuexingan06.cn

JS:   s.split("a").length - 1
来源：http://ek.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://mn.lnxyls.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://st.panjiajie.cn

Go:   strings.Count(s, "a")
来源：http://sf.chemitech.net.cn

Ruby: s.count("a")
来源：http://jk.jianghongdianzi.cn

C#:   s.Count(c => c == 'a')
来源：http://cl.bjjhwx.cn

[E13] 逐字符遍历
来源：http://wv.gzmigu.cn

Py:   for ch in s: print(ch)
来源：http://vq.bookmarksfly.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ln.bjjhwx.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xj.huixiangedu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mv.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://om.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nh.9csxet.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sx.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tj.asd995.cn

[E14] URL 编码与 Base64
来源：http://iu.gzmigu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://de.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kz.jctech888.com.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pg.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xi.jctech888.com.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hc.wgjwhj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wr.colortex.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ji.newstarts.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://qz.panjiajie.cn

[E15] HTML 转义 / 反转义
来源：http://kl.yuntaijiaju.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bp.nszjky.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jx.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qa.newstarts.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nt.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hc.szxytkj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://uf.shxzskj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kf.lnxyls.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pz.muxihuayi.cn

[E16] 数字千分位
来源：http://zr.nszjky.cn

Py:   f"{1234567:,}"
来源：http://ub.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://pz.yuntaijiaju.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qz.haigaiapp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pw.jctech888.com.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qa.chemitech.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nm.nszjky.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dn.colortex.cn

C#:   1234567.ToString("N0")
来源：http://nk.huanxung.cn

[E17] 首字母大写
来源：http://wy.yuntaijiaju.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yp.chemitech.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gi.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ri.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pz.521024.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ld.huanxung.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://lk.jianghongdianzi.cn

Ruby: s.capitalize
来源：http://xa.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gn.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://so.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xz.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://we.gzmigu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rp.jianghongdianzi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://uq.bookmarksfly.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gd.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zg.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sd.muxihuayi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ke.bookmarksfly.cn

[E19] 多行文本按行拆分
来源：http://mo.wgjwhj.cn

Py:   s.splitlines()
来源：http://xq.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fb.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://us.colortex.cn

TS:   s.split(/\r?\n/)
来源：http://se.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://br.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://fs.shxzukj.cn

Ruby: s.lines
来源：http://ec.szsharing.cn

C#:   s.Split('\n')
来源：http://mt.9csxet.cn

[E20] 判断字符串是否为空
来源：http://lf.huixinmuqiang.cn

Py:   if not s:
来源：http://ca.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nv.lnxyls.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uz.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://uz.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://xa.hnjuh.cn

Go:   if s == "" {}
来源：http://wg.9csxet.cn

Ruby: if s.empty?
来源：http://ph.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yi.jianghongdianzi.cn

[E21] 超长截断加省略号
来源：http://sa.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qe.newstarts.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ow.huanxung.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wi.asd995.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gi.newstarts.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ll.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://tw.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nq.9csxet.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://xt.bookmarksfly.cn

[E22] 字节长度与字符长度
来源：http://ll.hahajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ui.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ts.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lo.nszjky.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://po.wgjwhj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://cw.huixinmuqiang.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mj.gzmigu.cn

Ruby: s.bytesize;  s.length
来源：http://xb.colortex.cn


<!-- 参考信息 -->