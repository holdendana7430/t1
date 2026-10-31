代发 wailian999

Java: new ArrayList<>(list);
来源：http://jm.bookmarksfly.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ee.bjjhwx.cn

Ruby: arr.dup;  arr.clone
来源：http://go.hnjuh.cn

C#:   new List<int>(list);
来源：http://uv.hnjuh.cn

[D23] reduce 累积计算
来源：http://zm.haigaiapp.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cm.huanxung.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://qw.yuntaijiaju.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kd.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sm.huixinmuqiang.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://zq.shtwfgs.cn

Go:   // 手写循环
来源：http://wr.gzmigu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://cp.haigaiapp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bp.wgjwhj.cn

[D24] 字典 / Map 基本操作
来源：http://kq.521024.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ln.muxihuayi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fq.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rw.shxzukj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sn.panjiajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yg.lnxyls.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gp.gzmigu.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vb.asd995.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ug.szsharing.cn

[D25] Set 集合去重与交并差
来源：http://py.wgjwhj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mr.nicolike.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://rx.jianghongdianzi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pt.shxzukj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cl.gzmigu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yf.nicolike.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jn.shxzukj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sg.nszjky.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://kr.nszjky.cn

[D26] 数组转字符串
来源：http://vw.nicolike.cn

Py:   ", ".join(map(str, arr))
来源：http://hz.panjiajie.cn

PHP:  implode(", ", $arr);
来源：http://mm.yuntaijiaju.cn

JS:   arr.join(", ")
来源：http://zj.9csxet.cn

TS:   arr.join(", ")
来源：http://oj.szsharing.cn

Java: String.join(", ", list)
来源：http://an.asd995.cn

Go:   strings.Join(strs, ", ")
来源：http://iy.huanxung.cn

Ruby: arr.join(", ")
来源：http://pi.hahajie.cn

C#:   string.Join(", ", list)
来源：http://ka.szsharing.cn

================================================================================
来源：http://nl.jctech888.com.cn

E. 字符串处理
来源：http://lq.haigaiapp.cn

================================================================================
来源：http://vt.hahajie.cn

[E01] 拼接字符串
来源：http://wu.jctech888.com.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://pe.wgjwhj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ka.bookmarksfly.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ee.bjjhwx.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sv.nicolike.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://di.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ks.shxzskj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ap.szxytkj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ev.huixinmuqiang.cn

[E02] 重复字符串
来源：http://ri.szxytkj.cn

Py:   "ab" * 3
来源：http://fi.muxihuayi.cn

PHP:  str_repeat("ab", 3);
来源：http://cs.asd995.cn

JS:   "ab".repeat(3)
来源：http://is.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://eg.jctech888.com.cn

Java: "ab".repeat(3)
来源：http://sl.521024.cn

Go:   strings.Repeat("ab", 3)
来源：http://cj.huixinmuqiang.cn

Ruby: "ab" * 3
来源：http://um.newstarts.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yg.bjjhwx.cn

[E03] 截取子串
来源：http://tj.huixinmuqiang.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://tm.hahajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ur.huixiangedu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://kc.newstarts.cn

TS:   s.slice(1, 4)
来源：http://ki.huixiangedu.cn

Java: s.substring(1, 4)
来源：http://gp.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zd.panjiajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ah.nszjky.cn

C#:   s.Substring(1, 3)
来源：http://kp.newstarts.cn

[E04] 查找子串位置
来源：http://ae.jctech888.com.cn

Py:   s.find("x");  s.index("x")
来源：http://bq.chemitech.net.cn

PHP:  strpos($s, "x");
来源：http://xi.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vv.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://qo.9csxet.cn

Java: s.indexOf("x")
来源：http://ax.huixinmuqiang.cn

Go:   strings.Index(s, "x")
来源：http://fi.huanxung.cn

Ruby: s.index("x")
来源：http://cc.asd995.cn

C#:   s.IndexOf("x")
来源：http://ru.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ww.chemitech.net.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ju.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ta.shxzskj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fg.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mi.lnxyls.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ad.huanxung.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pe.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yo.bjjhwx.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ju.hahajie.cn

[E06] 替换子串
来源：http://fg.newstarts.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://we.chemitech.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://kc.jianghongdianzi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uy.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://nb.bookmarksfly.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ov.shxzukj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://aq.panjiajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fs.9csxet.cn

C#:   s.Replace("a", "b")
来源：http://ts.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://ax.chemitech.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mk.lnxyls.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://dj.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jb.asd995.cn

TS:   s.split(",")
来源：http://id.newstarts.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qr.521024.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ax.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://zr.szxytkj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sj.newstarts.cn

[E08] 数组按分隔符合并
来源：http://rw.jctech888.com.cn

Py:   ",".join(items)
来源：http://lf.hahajie.cn

PHP:  implode(",", $items);
来源：http://qa.panjiajie.cn

JS:   items.join(",")
来源：http://wg.bookmarksfly.cn

TS:   items.join(",")
来源：http://ig.shtwfgs.cn

Java: String.join(",", items)
来源：http://kz.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://cz.haigaiapp.cn

Ruby: items.join(",")
来源：http://gh.newstarts.cn

C#:   string.Join(",", items)
来源：http://sa.szsharing.cn

[E09] 去除所有空白字符
来源：http://kc.muxihuayi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zz.newstarts.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://eq.yuexingan06.cn

JS:   s.replace(/\s+/g, "")
来源：http://uu.haigaiapp.cn

TS:   s.replace(/\s+/g, "")
来源：http://ci.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://qs.bookmarksfly.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ij.521024.cn

Ruby: s.gsub(/\s+/, "")
来源：http://pt.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sf.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://rn.chemitech.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tz.shxzskj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ng.nszjky.cn

JS:   "7".padStart(3, "0")
来源：http://le.colortex.cn

TS:   "7".padStart(3, "0")
来源：http://bx.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://ms.huixinmuqiang.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ah.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gl.jctech888.com.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pv.huixiangedu.cn

[E11] 反转字符串
来源：http://sb.shtwfgs.cn

Py:   s[::-1]
来源：http://zs.bjjhwx.cn

PHP:  strrev($s);
来源：http://nw.521024.cn

JS:   [...s].reverse().join("")
来源：http://yq.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://ak.huanxung.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hr.nicolike.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gk.shtwfgs.cn

Ruby: s.reverse
来源：http://ea.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ix.jianghongdianzi.cn

[E12] 统计某字符出现次数
来源：http://ld.huixinmuqiang.cn

Py:   s.count("a")
来源：http://ua.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://ms.huixinmuqiang.cn

JS:   s.split("a").length - 1
来源：http://ce.yuexingan06.cn

TS:   s.split("a").length - 1
来源：http://vs.huixinmuqiang.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tz.521024.cn

Go:   strings.Count(s, "a")
来源：http://kd.bookmarksfly.cn

Ruby: s.count("a")
来源：http://et.haigaiapp.cn

C#:   s.Count(c => c == 'a')
来源：http://cl.nicolike.cn

[E13] 逐字符遍历
来源：http://xf.bookmarksfly.cn

Py:   for ch in s: print(ch)
来源：http://nh.szsharing.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dc.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ku.9csxet.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bz.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mx.shtwfgs.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sf.shxzskj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ib.newstarts.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sz.yuexingan06.cn

[E14] URL 编码与 Base64
来源：http://uu.chemitech.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yk.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://iw.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://af.muxihuayi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yg.shxzskj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sk.muxihuayi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pw.shxzukj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qg.9csxet.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gb.shtwfgs.cn

[E15] HTML 转义 / 反转义
来源：http://wk.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rw.nszjky.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yp.szsharing.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hu.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ez.bjjhwx.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tu.muxihuayi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zs.shxzskj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cg.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hx.szxytkj.cn

[E16] 数字千分位
来源：http://wv.huixiangedu.cn

Py:   f"{1234567:,}"
来源：http://la.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://hk.huixiangedu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://eh.yuexingan06.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fa.shxzskj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://di.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ii.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bo.muxihuayi.cn

C#:   1234567.ToString("N0")
来源：http://xj.huanxung.cn

[E17] 首字母大写
来源：http://to.colortex.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fl.jctech888.com.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://zm.szsharing.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oa.muxihuayi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ue.colortex.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mf.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bx.nszjky.cn

Ruby: s.capitalize
来源：http://zw.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rj.521024.cn

[E18] 模板占位符替换
来源：http://wg.jctech888.com.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qy.shtwfgs.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ri.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://cs.wgjwhj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lt.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ta.asd995.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qm.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mk.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ue.asd995.cn

[E19] 多行文本按行拆分
来源：http://kz.bookmarksfly.cn

Py:   s.splitlines()
来源：http://tt.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dy.nszjky.cn

JS:   s.split(/\r?\n/)
来源：http://ge.nszjky.cn

TS:   s.split(/\r?\n/)
来源：http://om.shxzskj.cn

Java: s.lines().toList()
来源：http://wa.gzmigu.cn

Go:   strings.Split(s, "\n")
来源：http://lt.panjiajie.cn

Ruby: s.lines
来源：http://ab.nszjky.cn

C#:   s.Split('\n')
来源：http://to.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://xr.haigaiapp.cn

Py:   if not s:
来源：http://dc.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xg.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jg.chemitech.net.cn

TS:   if (s === "") {}
来源：http://yr.yuexingan06.cn

Java: if (s.isEmpty()) {}
来源：http://ma.chemitech.net.cn

Go:   if s == "" {}
来源：http://hw.hahajie.cn

Ruby: if s.empty?
来源：http://sh.szsharing.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zn.yuexingan06.cn

[E21] 超长截断加省略号
来源：http://lf.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jv.chemitech.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://go.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xi.lnxyls.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://db.haigaiapp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oa.colortex.cn

Go:   // 按 rune 判断长度后截断
来源：http://qa.panjiajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rm.yuexingan06.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uh.shtwfgs.cn

[E22] 字节长度与字符长度
来源：http://ep.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hm.wgjwhj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xs.szxytkj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pe.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://go.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sg.colortex.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zh.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://af.asd995.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yj.newstarts.cn

================================================================================
来源：http://ih.nicolike.cn

F. 文件与目录
来源：http://lg.9csxet.cn

================================================================================
来源：http://ha.lnxyls.cn

[F01] 读取整个文件
来源：http://pg.hnjuh.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jc.colortex.cn

PHP:  file_get_contents("a.txt");
来源：http://el.shtwfgs.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ea.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fa.lnxyls.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://wu.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iq.521024.cn

Ruby: File.read("a.txt")
来源：http://yr.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://vr.521024.cn

[F02] 逐行读取文件
来源：http://bg.jctech888.com.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vf.chemitech.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sc.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jq.huixinmuqiang.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ne.szxytkj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lc.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qe.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ws.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ip.hnjuh.cn

[F03] 写入文件（覆盖）
来源：http://ma.lnxyls.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ri.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zz.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ze.panjiajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zn.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dm.haigaiapp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mn.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://tx.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dp.newstarts.cn

[F04] 追加写入文件
来源：http://mh.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gs.muxihuayi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://up.hahajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vc.yuntaijiaju.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cg.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tk.hnjuh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ia.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zm.nszjky.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pu.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://zw.huixiangedu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pb.szsharing.cn

PHP:  file_exists("a.txt");
来源：http://yw.panjiajie.cn

JS:   fs.existsSync("a.txt")
来源：http://vb.gzmigu.cn

TS:   fs.existsSync("a.txt")
来源：http://go.shxzskj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zl.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://lj.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://sm.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://wh.shxzskj.cn

[F06] 删除文件
来源：http://ta.huanxung.cn

Py:   os.remove("a.txt")
来源：http://ba.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://eg.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lb.hnjuh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kl.chemitech.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://da.haigaiapp.cn

Go:   os.Remove("a.txt")
来源：http://ff.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://tg.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://as.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://fi.huixinmuqiang.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sd.hahajie.cn


<!-- 参考信息 -->