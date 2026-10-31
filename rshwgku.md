代发 wailian999

[D23] reduce 累积计算
来源：http://wg.colortex.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://oe.hnjuh.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://vx.521024.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://er.bookmarksfly.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://le.szsharing.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://cx.colortex.cn

Go:   // 手写循环
来源：http://lz.newstarts.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ng.521024.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rc.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://jn.huixinmuqiang.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ry.szxytkj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wf.jctech888.com.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rs.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ew.chemitech.net.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ip.huanxung.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ec.huixinmuqiang.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qd.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ky.muxihuayi.cn

[D25] Set 集合去重与交并差
来源：http://tv.yuntaijiaju.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://aj.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ti.yuntaijiaju.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://he.shxzukj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fv.newstarts.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://sb.newstarts.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sl.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pg.bjjhwx.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://iq.jianghongdianzi.cn

[D26] 数组转字符串
来源：http://hk.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://yh.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://fg.shtwfgs.cn

JS:   arr.join(", ")
来源：http://ae.chemitech.net.cn

TS:   arr.join(", ")
来源：http://ak.shtwfgs.cn

Java: String.join(", ", list)
来源：http://pj.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://ml.shxzukj.cn

Ruby: arr.join(", ")
来源：http://pn.9csxet.cn

C#:   string.Join(", ", list)
来源：http://wr.wgjwhj.cn

================================================================================
来源：http://he.nszjky.cn

E. 字符串处理
来源：http://ba.newstarts.cn

================================================================================
来源：http://qt.szxytkj.cn

[E01] 拼接字符串
来源：http://kw.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hy.lnxyls.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ed.asd995.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hs.nszjky.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ba.haigaiapp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ow.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vh.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qr.muxihuayi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ox.chemitech.net.cn

[E02] 重复字符串
来源：http://qc.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://ff.lnxyls.cn

PHP:  str_repeat("ab", 3);
来源：http://tc.huanxung.cn

JS:   "ab".repeat(3)
来源：http://lx.9csxet.cn

TS:   "ab".repeat(3)
来源：http://kj.colortex.cn

Java: "ab".repeat(3)
来源：http://dq.gzmigu.cn

Go:   strings.Repeat("ab", 3)
来源：http://xg.521024.cn

Ruby: "ab" * 3
来源：http://el.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://nj.muxihuayi.cn

[E03] 截取子串
来源：http://ry.hnjuh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sk.bookmarksfly.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ot.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ki.nicolike.cn

TS:   s.slice(1, 4)
来源：http://pw.hnjuh.cn

Java: s.substring(1, 4)
来源：http://ns.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yv.panjiajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://eg.gzmigu.cn

C#:   s.Substring(1, 3)
来源：http://rp.jctech888.com.cn

[E04] 查找子串位置
来源：http://jy.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://id.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://ql.asd995.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jz.szsharing.cn

TS:   s.indexOf("x")
来源：http://yd.bjjhwx.cn

Java: s.indexOf("x")
来源：http://tf.nszjky.cn

Go:   strings.Index(s, "x")
来源：http://te.szsharing.cn

Ruby: s.index("x")
来源：http://au.lnxyls.cn

C#:   s.IndexOf("x")
来源：http://wm.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hl.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cq.panjiajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://sk.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wq.asd995.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://jq.haigaiapp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://lq.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pj.chemitech.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://so.bjjhwx.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mr.9csxet.cn

[E06] 替换子串
来源：http://dd.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://go.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://qr.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://im.jianghongdianzi.cn

TS:   s.replaceAll("a", "b")
来源：http://ny.shxzskj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ca.panjiajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://pi.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://df.jctech888.com.cn

C#:   s.Replace("a", "b")
来源：http://sj.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://am.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ud.huixinmuqiang.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rd.newstarts.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://lu.nszjky.cn

TS:   s.split(",")
来源：http://pg.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://vg.colortex.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xc.wgjwhj.cn

Ruby: s.split(",");  s.split
来源：http://hg.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ru.9csxet.cn

[E08] 数组按分隔符合并
来源：http://nh.shtwfgs.cn

Py:   ",".join(items)
来源：http://lp.shxzskj.cn

PHP:  implode(",", $items);
来源：http://xi.bjjhwx.cn

JS:   items.join(",")
来源：http://ip.haigaiapp.cn

TS:   items.join(",")
来源：http://gg.hahajie.cn

Java: String.join(",", items)
来源：http://nb.jianghongdianzi.cn

Go:   strings.Join(items, ",")
来源：http://ee.panjiajie.cn

Ruby: items.join(",")
来源：http://ao.gzmigu.cn

C#:   string.Join(",", items)
来源：http://nz.wgjwhj.cn

[E09] 去除所有空白字符
来源：http://fk.yuntaijiaju.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yd.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ef.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://tr.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://qn.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://mm.yuexingan06.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mo.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zs.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rv.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://ob.521024.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yn.wgjwhj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xv.yuexingan06.cn

JS:   "7".padStart(3, "0")
来源：http://pt.nicolike.cn

TS:   "7".padStart(3, "0")
来源：http://qx.jianghongdianzi.cn

Java: String.format("%03d", 7)
来源：http://ah.521024.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zj.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zo.bjjhwx.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ga.shxzukj.cn

[E11] 反转字符串
来源：http://eg.hnjuh.cn

Py:   s[::-1]
来源：http://pa.muxihuayi.cn

PHP:  strrev($s);
来源：http://cj.9csxet.cn

JS:   [...s].reverse().join("")
来源：http://sc.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://es.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ye.bookmarksfly.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://uk.newstarts.cn

Ruby: s.reverse
来源：http://yw.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xj.jianghongdianzi.cn

[E12] 统计某字符出现次数
来源：http://hz.huixiangedu.cn

Py:   s.count("a")
来源：http://bj.panjiajie.cn

PHP:  substr_count($s, "a");
来源：http://gx.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://ma.colortex.cn

TS:   s.split("a").length - 1
来源：http://fd.gzmigu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mj.hnjuh.cn

Go:   strings.Count(s, "a")
来源：http://mm.yuntaijiaju.cn

Ruby: s.count("a")
来源：http://lr.521024.cn

C#:   s.Count(c => c == 'a')
来源：http://ae.hnjuh.cn

[E13] 逐字符遍历
来源：http://tg.newstarts.cn

Py:   for ch in s: print(ch)
来源：http://fb.huixiangedu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kw.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://un.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://cr.chemitech.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gh.huanxung.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pv.hnjuh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://er.szxytkj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oq.9csxet.cn

[E14] URL 编码与 Base64
来源：http://jt.gzmigu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ag.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pg.newstarts.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mk.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fy.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://oz.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zz.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://av.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xa.huixinmuqiang.cn

[E15] HTML 转义 / 反转义
来源：http://xx.hahajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gh.yuexingan06.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oh.shxzukj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wr.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lg.huanxung.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tu.szsharing.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zo.jianghongdianzi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tg.newstarts.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xg.hahajie.cn

[E16] 数字千分位
来源：http://rx.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://tu.hnjuh.cn

PHP:  number_format(1234567);
来源：http://je.lnxyls.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://jh.yuntaijiaju.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ux.9csxet.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ip.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ms.521024.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vb.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://kv.newstarts.cn

[E17] 首字母大写
来源：http://tv.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vc.muxihuayi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zc.haigaiapp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jr.hnjuh.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ps.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://or.shtwfgs.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ro.bookmarksfly.cn

Ruby: s.capitalize
来源：http://uw.hahajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rt.521024.cn

[E18] 模板占位符替换
来源：http://vr.huanxung.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sy.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://gg.shtwfgs.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ec.panjiajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vf.nszjky.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ke.wgjwhj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nt.colortex.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://cz.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xu.521024.cn

[E19] 多行文本按行拆分
来源：http://po.haigaiapp.cn

Py:   s.splitlines()
来源：http://zv.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://rl.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://yb.yuntaijiaju.cn

TS:   s.split(/\r?\n/)
来源：http://up.huixiangedu.cn

Java: s.lines().toList()
来源：http://ay.asd995.cn

Go:   strings.Split(s, "\n")
来源：http://ge.9csxet.cn

Ruby: s.lines
来源：http://aw.asd995.cn

C#:   s.Split('\n')
来源：http://jm.yuntaijiaju.cn

[E20] 判断字符串是否为空
来源：http://qj.huixiangedu.cn

Py:   if not s:
来源：http://lu.chemitech.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hw.nszjky.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xz.panjiajie.cn

TS:   if (s === "") {}
来源：http://xu.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://qd.hahajie.cn

Go:   if s == "" {}
来源：http://rf.huanxung.cn

Ruby: if s.empty?
来源：http://gb.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ys.9csxet.cn

[E21] 超长截断加省略号
来源：http://hz.huixinmuqiang.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://um.bjjhwx.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://rs.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zd.yuexingan06.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wd.yuntaijiaju.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pw.hnjuh.cn

Go:   // 按 rune 判断长度后截断
来源：http://oq.panjiajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://lg.jctech888.com.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ti.szsharing.cn

[E22] 字节长度与字符长度
来源：http://yu.huixinmuqiang.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fj.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jx.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mi.jctech888.com.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qh.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wv.muxihuayi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yo.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://kf.huixinmuqiang.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://oe.panjiajie.cn

================================================================================
来源：http://ex.szxytkj.cn

F. 文件与目录
来源：http://az.lnxyls.cn

================================================================================
来源：http://jp.szsharing.cn

[F01] 读取整个文件
来源：http://ff.jctech888.com.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nq.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://lz.hnjuh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lo.nszjky.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://af.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://td.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ke.bookmarksfly.cn

Ruby: File.read("a.txt")
来源：http://bn.521024.cn

C#:   File.ReadAllText("a.txt");
来源：http://wh.shtwfgs.cn

[F02] 逐行读取文件
来源：http://fy.lnxyls.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vi.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ch.9csxet.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pf.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nq.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://so.wgjwhj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ni.yuexingan06.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ew.jianghongdianzi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://la.shxzskj.cn

[F03] 写入文件（覆盖）
来源：http://eb.gzmigu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sp.bjjhwx.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vj.9csxet.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wm.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gm.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wg.panjiajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qp.jctech888.com.cn

Ruby: File.write("a.txt", "hi")
来源：http://yb.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://go.jctech888.com.cn

[F04] 追加写入文件
来源：http://ns.shtwfgs.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vz.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dv.bjjhwx.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ys.jianghongdianzi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ez.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ua.jianghongdianzi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sz.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jc.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yh.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://jz.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cp.shtwfgs.cn

PHP:  file_exists("a.txt");
来源：http://bd.bookmarksfly.cn

JS:   fs.existsSync("a.txt")
来源：http://tl.yuexingan06.cn

TS:   fs.existsSync("a.txt")
来源：http://en.shtwfgs.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jm.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://im.muxihuayi.cn

Ruby: File.exist?("a.txt")
来源：http://pg.huanxung.cn

C#:   File.Exists("a.txt")
来源：http://fx.wgjwhj.cn

[F06] 删除文件
来源：http://sc.huanxung.cn

Py:   os.remove("a.txt")
来源：http://uh.9csxet.cn

PHP:  unlink("a.txt");
来源：http://at.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mq.nszjky.cn

TS:   fs.unlinkSync("a.txt")
来源：http://er.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yv.colortex.cn

Go:   os.Remove("a.txt")
来源：http://ly.yuexingan06.cn

Ruby: File.delete("a.txt")
来源：http://ia.9csxet.cn

C#:   File.Delete("a.txt");
来源：http://ni.nszjky.cn

[F07] 创建目录（含多级）
来源：http://ek.bjjhwx.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ym.shtwfgs.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://bo.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cz.gzmigu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ov.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vc.yuntaijiaju.cn


<!-- 参考信息 -->