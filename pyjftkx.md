代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wo.szxytkj.cn

Go:   // 手写双层循环
来源：http://gp.nicolike.cn

Ruby: nested.flatten
来源：http://tb.huixinmuqiang.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://tm.szsharing.cn

[D19] 按字段分组
来源：http://ft.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qm.huanxung.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://fv.nicolike.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vk.shxzukj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://jr.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dm.9csxet.cn

Go:   // 手写 map[string][]T
来源：http://ek.chemitech.net.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://us.chemitech.net.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://sb.chemitech.net.cn

[D20] 统计每个元素出现次数
来源：http://pb.huixiangedu.cn

Py:   Counter(arr)
来源：http://dp.jianghongdianzi.cn

PHP:  array_count_values($arr);
来源：http://om.shxzukj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ty.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vf.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://aj.huixiangedu.cn

Go:   // 手写 map[T]int
来源：http://js.shtwfgs.cn

Ruby: arr.tally
来源：http://nw.jctech888.com.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rg.shxzskj.cn

[D21] 判断是否包含某元素
来源：http://nu.jctech888.com.cn

Py:   x in arr
来源：http://cj.yuexingan06.cn

PHP:  in_array($x, $arr, true);
来源：http://rf.huixiangedu.cn

JS:   arr.includes(x)
来源：http://gn.hnjuh.cn

TS:   arr.includes(x)
来源：http://ug.yuntaijiaju.cn

Java: list.contains(x)
来源：http://wv.haigaiapp.cn

Go:   slices.Contains(arr, x)
来源：http://cg.nicolike.cn

Ruby: arr.include?(x)
来源：http://fo.colortex.cn

C#:   list.Contains(x)
来源：http://ez.huanxung.cn

[D22] 复制数组（避免共享引用）
来源：http://sq.colortex.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ha.jianghongdianzi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fi.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fs.newstarts.cn

TS:   [...arr];
来源：http://up.huixiangedu.cn

Java: new ArrayList<>(list);
来源：http://bl.huanxung.cn

Go:   copied := append([]int(nil), arr...)
来源：http://md.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://fp.huanxung.cn

C#:   new List<int>(list);
来源：http://eg.haigaiapp.cn

[D23] reduce 累积计算
来源：http://sv.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hm.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fe.huixinmuqiang.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jz.panjiajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://lv.asd995.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vx.jianghongdianzi.cn

Go:   // 手写循环
来源：http://xe.muxihuayi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://tc.haigaiapp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xr.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://zm.huixiangedu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mi.szxytkj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rn.huixiangedu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vt.521024.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bw.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ei.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jt.gzmigu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ti.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://xl.asd995.cn

[D25] Set 集合去重与交并差
来源：http://zu.newstarts.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://lz.newstarts.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://cc.haigaiapp.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bp.nszjky.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://kw.wgjwhj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://or.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mc.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sr.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nk.haigaiapp.cn

[D26] 数组转字符串
来源：http://sq.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://mw.asd995.cn

PHP:  implode(", ", $arr);
来源：http://mt.hahajie.cn

JS:   arr.join(", ")
来源：http://di.hahajie.cn

TS:   arr.join(", ")
来源：http://jl.panjiajie.cn

Java: String.join(", ", list)
来源：http://sj.shtwfgs.cn

Go:   strings.Join(strs, ", ")
来源：http://de.newstarts.cn

Ruby: arr.join(", ")
来源：http://qc.yuntaijiaju.cn

C#:   string.Join(", ", list)
来源：http://ki.newstarts.cn

================================================================================
来源：http://dq.bookmarksfly.cn

E. 字符串处理
来源：http://iu.hnjuh.cn

================================================================================
来源：http://fw.asd995.cn

[E01] 拼接字符串
来源：http://vk.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nv.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bq.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ey.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lc.shxzukj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wt.huanxung.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://oc.huixinmuqiang.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qy.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ey.lnxyls.cn

[E02] 重复字符串
来源：http://wd.nicolike.cn

Py:   "ab" * 3
来源：http://lf.nicolike.cn

PHP:  str_repeat("ab", 3);
来源：http://sm.wgjwhj.cn

JS:   "ab".repeat(3)
来源：http://xs.jianghongdianzi.cn

TS:   "ab".repeat(3)
来源：http://qt.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://jo.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://hr.huixiangedu.cn

Ruby: "ab" * 3
来源：http://wv.lnxyls.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://bf.nszjky.cn

[E03] 截取子串
来源：http://nu.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zc.yuexingan06.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://rd.lnxyls.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cl.haigaiapp.cn

TS:   s.slice(1, 4)
来源：http://yd.9csxet.cn

Java: s.substring(1, 4)
来源：http://xa.lnxyls.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zi.bookmarksfly.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hk.muxihuayi.cn

C#:   s.Substring(1, 3)
来源：http://jl.wgjwhj.cn

[E04] 查找子串位置
来源：http://fj.haigaiapp.cn

Py:   s.find("x");  s.index("x")
来源：http://tv.huanxung.cn

PHP:  strpos($s, "x");
来源：http://kt.bookmarksfly.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fc.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://ys.chemitech.net.cn

Java: s.indexOf("x")
来源：http://et.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://hx.szsharing.cn

Ruby: s.index("x")
来源：http://ga.nicolike.cn

C#:   s.IndexOf("x")
来源：http://dd.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rc.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://kq.haigaiapp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ri.szsharing.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ru.huixiangedu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sv.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bl.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://qa.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bj.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bp.9csxet.cn

[E06] 替换子串
来源：http://wo.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sz.szsharing.cn

PHP:  str_replace("a", "b", $s);
来源：http://kk.521024.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ss.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://au.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qv.panjiajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zg.hnjuh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ii.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://jd.newstarts.cn

[E07] 按分隔符拆分
来源：http://lz.muxihuayi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ye.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ie.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gi.nszjky.cn

TS:   s.split(",")
来源：http://du.hahajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ag.yuexingan06.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://jp.chemitech.net.cn

Ruby: s.split(",");  s.split
来源：http://wr.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nu.panjiajie.cn

[E08] 数组按分隔符合并
来源：http://gd.newstarts.cn

Py:   ",".join(items)
来源：http://dm.nicolike.cn

PHP:  implode(",", $items);
来源：http://uo.huixinmuqiang.cn

JS:   items.join(",")
来源：http://nr.shtwfgs.cn

TS:   items.join(",")
来源：http://he.asd995.cn

Java: String.join(",", items)
来源：http://xl.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://mx.521024.cn

Ruby: items.join(",")
来源：http://de.haigaiapp.cn

C#:   string.Join(",", items)
来源：http://zs.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://ae.521024.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pq.hahajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vt.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://vw.gzmigu.cn

TS:   s.replace(/\s+/g, "")
来源：http://dc.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://uz.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://og.huixinmuqiang.cn

Ruby: s.gsub(/\s+/, "")
来源：http://iy.bookmarksfly.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dn.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://ux.szsharing.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://el.colortex.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qr.hahajie.cn

JS:   "7".padStart(3, "0")
来源：http://kb.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://dg.nicolike.cn

Java: String.format("%03d", 7)
来源：http://ky.huixinmuqiang.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wo.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://io.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ir.yuexingan06.cn

[E11] 反转字符串
来源：http://ad.huanxung.cn

Py:   s[::-1]
来源：http://cl.muxihuayi.cn

PHP:  strrev($s);
来源：http://wg.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://zc.asd995.cn

TS:   [...s].reverse().join("")
来源：http://cl.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://de.hnjuh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jn.newstarts.cn

Ruby: s.reverse
来源：http://bl.521024.cn

C#:   new string(s.Reverse().ToArray())
来源：http://uz.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://oa.bookmarksfly.cn

Py:   s.count("a")
来源：http://no.muxihuayi.cn

PHP:  substr_count($s, "a");
来源：http://bs.muxihuayi.cn

JS:   s.split("a").length - 1
来源：http://dj.szxytkj.cn

TS:   s.split("a").length - 1
来源：http://hb.asd995.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://te.newstarts.cn

Go:   strings.Count(s, "a")
来源：http://nd.shtwfgs.cn

Ruby: s.count("a")
来源：http://bf.hahajie.cn

C#:   s.Count(c => c == 'a')
来源：http://pb.haigaiapp.cn

[E13] 逐字符遍历
来源：http://ts.bookmarksfly.cn

Py:   for ch in s: print(ch)
来源：http://qf.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gd.colortex.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gu.bjjhwx.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://eb.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pv.shxzskj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nh.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ta.lnxyls.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ow.521024.cn

[E14] URL 编码与 Base64
来源：http://nq.huixinmuqiang.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://cv.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wp.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fe.gzmigu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://th.nszjky.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://rd.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xq.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://it.bookmarksfly.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wb.shxzukj.cn

[E15] HTML 转义 / 反转义
来源：http://kc.yuexingan06.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qw.huixiangedu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rd.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gj.shxzukj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ye.haigaiapp.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yj.bookmarksfly.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kx.chemitech.net.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://md.newstarts.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mk.gzmigu.cn

[E16] 数字千分位
来源：http://bb.szsharing.cn

Py:   f"{1234567:,}"
来源：http://xo.9csxet.cn

PHP:  number_format(1234567);
来源：http://tp.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ma.jianghongdianzi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ur.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hh.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zn.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ig.hnjuh.cn

C#:   1234567.ToString("N0")
来源：http://ta.hnjuh.cn

[E17] 首字母大写
来源：http://zr.haigaiapp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gy.jctech888.com.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hv.jctech888.com.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tr.hnjuh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gw.bjjhwx.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://dv.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://fv.jianghongdianzi.cn

Ruby: s.capitalize
来源：http://tr.nicolike.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zj.wgjwhj.cn

[E18] 模板占位符替换
来源：http://va.szsharing.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fa.huanxung.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://de.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uy.huixiangedu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jn.shtwfgs.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dm.huixiangedu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vw.bookmarksfly.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yn.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://em.huixinmuqiang.cn

[E19] 多行文本按行拆分
来源：http://nf.lnxyls.cn

Py:   s.splitlines()
来源：http://bw.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bv.nszjky.cn

JS:   s.split(/\r?\n/)
来源：http://ic.shtwfgs.cn

TS:   s.split(/\r?\n/)
来源：http://sk.wgjwhj.cn

Java: s.lines().toList()
来源：http://gw.hahajie.cn

Go:   strings.Split(s, "\n")
来源：http://zm.panjiajie.cn

Ruby: s.lines
来源：http://nm.asd995.cn

C#:   s.Split('\n')
来源：http://at.jianghongdianzi.cn

[E20] 判断字符串是否为空
来源：http://il.gzmigu.cn

Py:   if not s:
来源：http://pr.521024.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ik.huixinmuqiang.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fo.hahajie.cn

TS:   if (s === "") {}
来源：http://cd.gzmigu.cn

Java: if (s.isEmpty()) {}
来源：http://jk.bookmarksfly.cn

Go:   if s == "" {}
来源：http://va.jctech888.com.cn

Ruby: if s.empty?
来源：http://nl.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://da.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://gm.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vk.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pf.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gt.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vv.bookmarksfly.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ow.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://qu.yuntaijiaju.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ry.yuexingan06.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ft.yuexingan06.cn

[E22] 字节长度与字符长度
来源：http://sy.521024.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kr.szsharing.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://km.asd995.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tl.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gd.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lc.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ku.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://kh.bjjhwx.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dr.hahajie.cn

================================================================================
来源：http://bv.lnxyls.cn

F. 文件与目录
来源：http://ck.bookmarksfly.cn

================================================================================
来源：http://ms.hnjuh.cn

[F01] 读取整个文件
来源：http://zf.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yo.panjiajie.cn

PHP:  file_get_contents("a.txt");
来源：http://ih.panjiajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jj.yuntaijiaju.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qn.huanxung.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lr.huixiangedu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pq.jctech888.com.cn

Ruby: File.read("a.txt")
来源：http://oz.yuntaijiaju.cn

C#:   File.ReadAllText("a.txt");
来源：http://or.colortex.cn

[F02] 逐行读取文件
来源：http://cq.521024.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://of.wgjwhj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rr.szxytkj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tz.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ek.colortex.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zx.yuexingan06.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wt.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vb.521024.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tt.nicolike.cn

[F03] 写入文件（覆盖）
来源：http://tr.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ic.hnjuh.cn


<!-- 参考信息 -->