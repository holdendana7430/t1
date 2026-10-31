代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qs.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://cx.hahajie.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ke.huanxung.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://si.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xk.haigaiapp.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fx.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://ik.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ty.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://si.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qh.shxzskj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sl.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qi.hahajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ue.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://re.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://vo.gzmigu.cn

[D26] 数组转字符串
来源：http://wb.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://ak.yuexingan06.cn

PHP:  implode(", ", $arr);
来源：http://cs.521024.cn

JS:   arr.join(", ")
来源：http://aa.nicolike.cn

TS:   arr.join(", ")
来源：http://do.chemitech.net.cn

Java: String.join(", ", list)
来源：http://ez.9csxet.cn

Go:   strings.Join(strs, ", ")
来源：http://cv.521024.cn

Ruby: arr.join(", ")
来源：http://yv.jctech888.com.cn

C#:   string.Join(", ", list)
来源：http://hh.colortex.cn

================================================================================
来源：http://fp.yuexingan06.cn

E. 字符串处理
来源：http://yk.newstarts.cn

================================================================================
来源：http://si.panjiajie.cn

[E01] 拼接字符串
来源：http://uj.colortex.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://dp.shxzskj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://er.bjjhwx.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://if.hahajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wp.lnxyls.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://dm.asd995.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hb.chemitech.net.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qt.muxihuayi.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gb.szxytkj.cn

[E02] 重复字符串
来源：http://of.huixiangedu.cn

Py:   "ab" * 3
来源：http://sp.newstarts.cn

PHP:  str_repeat("ab", 3);
来源：http://so.haigaiapp.cn

JS:   "ab".repeat(3)
来源：http://wh.szsharing.cn

TS:   "ab".repeat(3)
来源：http://lw.panjiajie.cn

Java: "ab".repeat(3)
来源：http://ws.yuntaijiaju.cn

Go:   strings.Repeat("ab", 3)
来源：http://jt.wgjwhj.cn

Ruby: "ab" * 3
来源：http://ud.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sf.gzmigu.cn

[E03] 截取子串
来源：http://pe.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lo.asd995.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zh.hahajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wn.huanxung.cn

TS:   s.slice(1, 4)
来源：http://mj.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://qx.gzmigu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wc.hnjuh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mq.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://qx.shxzskj.cn

[E04] 查找子串位置
来源：http://ch.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://ph.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://gi.jctech888.com.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vp.szsharing.cn

TS:   s.indexOf("x")
来源：http://ju.yuexingan06.cn

Java: s.indexOf("x")
来源：http://vy.bookmarksfly.cn

Go:   strings.Index(s, "x")
来源：http://mt.gzmigu.cn

Ruby: s.index("x")
来源：http://zi.bjjhwx.cn

C#:   s.IndexOf("x")
来源：http://rr.huanxung.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gi.jctech888.com.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qp.haigaiapp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ld.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zg.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sz.haigaiapp.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qj.szxytkj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ro.521024.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vc.jctech888.com.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://es.hnjuh.cn

[E06] 替换子串
来源：http://mf.newstarts.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hj.9csxet.cn

PHP:  str_replace("a", "b", $s);
来源：http://ak.jctech888.com.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yx.newstarts.cn

TS:   s.replaceAll("a", "b")
来源：http://jd.chemitech.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://na.bookmarksfly.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ko.nszjky.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wn.yuexingan06.cn

C#:   s.Replace("a", "b")
来源：http://wi.yuntaijiaju.cn

[E07] 按分隔符拆分
来源：http://ou.lnxyls.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hy.huanxung.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gl.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://by.szsharing.cn

TS:   s.split(",")
来源：http://nd.shxzskj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xd.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ql.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://ai.nszjky.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://nc.chemitech.net.cn

[E08] 数组按分隔符合并
来源：http://bw.nszjky.cn

Py:   ",".join(items)
来源：http://nu.9csxet.cn

PHP:  implode(",", $items);
来源：http://cj.shtwfgs.cn

JS:   items.join(",")
来源：http://bx.hahajie.cn

TS:   items.join(",")
来源：http://oq.asd995.cn

Java: String.join(",", items)
来源：http://xx.chemitech.net.cn

Go:   strings.Join(items, ",")
来源：http://dl.nicolike.cn

Ruby: items.join(",")
来源：http://jp.nszjky.cn

C#:   string.Join(",", items)
来源：http://yb.shxzukj.cn

[E09] 去除所有空白字符
来源：http://bm.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cq.shtwfgs.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ok.nicolike.cn

JS:   s.replace(/\s+/g, "")
来源：http://em.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://eb.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://qv.lnxyls.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xb.huixiangedu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wf.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bm.szxytkj.cn

[E10] 左侧补零 / 定长填充
来源：http://in.newstarts.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://px.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bl.asd995.cn

JS:   "7".padStart(3, "0")
来源：http://lr.chemitech.net.cn

TS:   "7".padStart(3, "0")
来源：http://yc.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://ds.yuntaijiaju.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ks.huixiangedu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://aj.9csxet.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rh.wgjwhj.cn

[E11] 反转字符串
来源：http://mz.panjiajie.cn

Py:   s[::-1]
来源：http://th.szsharing.cn

PHP:  strrev($s);
来源：http://gb.9csxet.cn

JS:   [...s].reverse().join("")
来源：http://xr.szsharing.cn

TS:   [...s].reverse().join("")
来源：http://ej.huixiangedu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dp.wgjwhj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hn.shxzskj.cn

Ruby: s.reverse
来源：http://uv.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://vt.jianghongdianzi.cn

[E12] 统计某字符出现次数
来源：http://xq.nszjky.cn

Py:   s.count("a")
来源：http://we.lnxyls.cn

PHP:  substr_count($s, "a");
来源：http://hl.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://yy.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://in.wgjwhj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://lp.szsharing.cn

Go:   strings.Count(s, "a")
来源：http://xf.bookmarksfly.cn

Ruby: s.count("a")
来源：http://zv.huixiangedu.cn

C#:   s.Count(c => c == 'a')
来源：http://zd.hnjuh.cn

[E13] 逐字符遍历
来源：http://kn.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://zk.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dd.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://rz.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gw.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://il.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sz.9csxet.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ew.yuntaijiaju.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://tr.hahajie.cn

[E14] URL 编码与 Base64
来源：http://dc.szxytkj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wf.panjiajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://di.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zo.shxzskj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://nv.521024.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qg.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jv.haigaiapp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ny.shxzskj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bp.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://sl.hahajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fm.yuexingan06.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://zg.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://oz.newstarts.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bm.newstarts.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ct.hnjuh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pg.jctech888.com.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fp.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ss.wgjwhj.cn

[E16] 数字千分位
来源：http://ab.huanxung.cn

Py:   f"{1234567:,}"
来源：http://ub.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://ca.jctech888.com.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://es.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xi.szxytkj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ri.nszjky.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vk.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ge.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://fh.gzmigu.cn

[E17] 首字母大写
来源：http://jz.haigaiapp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xs.bjjhwx.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://uo.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ta.jctech888.com.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qd.huixiangedu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://fo.newstarts.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wk.9csxet.cn

Ruby: s.capitalize
来源：http://ho.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://si.9csxet.cn

[E18] 模板占位符替换
来源：http://ef.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ez.huixinmuqiang.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jq.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://tq.wgjwhj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vp.shxzskj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ec.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://or.yuexingan06.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fk.hahajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://it.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://ui.chemitech.net.cn

Py:   s.splitlines()
来源：http://co.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uf.panjiajie.cn

JS:   s.split(/\r?\n/)
来源：http://dh.nszjky.cn

TS:   s.split(/\r?\n/)
来源：http://mt.521024.cn

Java: s.lines().toList()
来源：http://gx.jctech888.com.cn

Go:   strings.Split(s, "\n")
来源：http://wl.szxytkj.cn

Ruby: s.lines
来源：http://vc.szxytkj.cn

C#:   s.Split('\n')
来源：http://li.bjjhwx.cn

[E20] 判断字符串是否为空
来源：http://ie.colortex.cn

Py:   if not s:
来源：http://rx.9csxet.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gp.nszjky.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qy.hnjuh.cn

TS:   if (s === "") {}
来源：http://oc.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://vu.asd995.cn

Go:   if s == "" {}
来源：http://wy.9csxet.cn

Ruby: if s.empty?
来源：http://sa.9csxet.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ng.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://gx.nszjky.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nj.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://be.haigaiapp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fl.muxihuayi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ic.gzmigu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://io.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://zh.jianghongdianzi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bz.hnjuh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gc.asd995.cn

[E22] 字节长度与字符长度
来源：http://nv.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vi.yuexingan06.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://zj.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://du.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wi.szxytkj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ut.9csxet.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wg.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://nq.huixinmuqiang.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ut.shxzukj.cn

================================================================================
来源：http://fq.asd995.cn

F. 文件与目录
来源：http://bd.szsharing.cn

================================================================================
来源：http://ip.bookmarksfly.cn

[F01] 读取整个文件
来源：http://mw.gzmigu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://fc.panjiajie.cn

PHP:  file_get_contents("a.txt");
来源：http://cx.yuexingan06.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qi.yuntaijiaju.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xw.521024.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://of.muxihuayi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kx.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://tx.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://zb.nszjky.cn

[F02] 逐行读取文件
来源：http://gs.yuntaijiaju.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://aq.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xt.bookmarksfly.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://io.chemitech.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nu.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sk.huixiangedu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ab.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qh.szxytkj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ax.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://yd.wgjwhj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cp.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ry.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bo.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wk.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bp.huixinmuqiang.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gi.bjjhwx.cn

Ruby: File.write("a.txt", "hi")
来源：http://am.gzmigu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ll.yuexingan06.cn

[F04] 追加写入文件
来源：http://ct.haigaiapp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://vh.shxzskj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://it.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rw.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vg.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tr.huanxung.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ni.gzmigu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pa.hahajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ee.asd995.cn

[F05] 判断文件或目录是否存在
来源：http://ty.yuexingan06.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bf.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://ej.colortex.cn

JS:   fs.existsSync("a.txt")
来源：http://ds.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://do.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jb.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wp.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://gb.huixiangedu.cn

C#:   File.Exists("a.txt")
来源：http://uq.szxytkj.cn

[F06] 删除文件
来源：http://yg.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://yw.9csxet.cn

PHP:  unlink("a.txt");
来源：http://wr.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tb.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fc.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dq.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://kw.shtwfgs.cn

Ruby: File.delete("a.txt")
来源：http://ih.muxihuayi.cn

C#:   File.Delete("a.txt");
来源：http://oy.521024.cn

[F07] 创建目录（含多级）
来源：http://vd.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qs.panjiajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jr.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tc.yuntaijiaju.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kz.newstarts.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ae.shtwfgs.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://te.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://pr.huixiangedu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://js.huixinmuqiang.cn

[F08] 遍历目录
来源：http://yu.bjjhwx.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://np.colortex.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ed.huixinmuqiang.cn

JS:   fs.readdirSync("dir")
来源：http://uo.yuntaijiaju.cn

TS:   fs.readdirSync("dir")
来源：http://jh.9csxet.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://cf.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cp.shxzukj.cn

Ruby: Dir.children("dir")
来源：http://od.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://rk.jctech888.com.cn


<!-- 参考信息 -->