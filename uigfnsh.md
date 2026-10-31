代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sb.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://rg.yuexingan06.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://im.521024.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wo.lnxyls.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://js.shxzskj.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://jk.jianghongdianzi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uv.bjjhwx.cn

[D26] 数组转字符串
来源：http://hk.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://ir.9csxet.cn

PHP:  implode(", ", $arr);
来源：http://fp.9csxet.cn

JS:   arr.join(", ")
来源：http://xg.szxytkj.cn

TS:   arr.join(", ")
来源：http://lp.chemitech.net.cn

Java: String.join(", ", list)
来源：http://rf.shxzskj.cn

Go:   strings.Join(strs, ", ")
来源：http://vi.wgjwhj.cn

Ruby: arr.join(", ")
来源：http://bs.nicolike.cn

C#:   string.Join(", ", list)
来源：http://dm.szxytkj.cn

================================================================================
来源：http://np.muxihuayi.cn

E. 字符串处理
来源：http://ex.bjjhwx.cn

================================================================================
来源：http://bw.hnjuh.cn

[E01] 拼接字符串
来源：http://bh.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sl.nicolike.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://zn.jianghongdianzi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dy.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ei.huixiangedu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ux.lnxyls.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lf.muxihuayi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ky.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://xo.huixiangedu.cn

[E02] 重复字符串
来源：http://ex.yuexingan06.cn

Py:   "ab" * 3
来源：http://ly.bjjhwx.cn

PHP:  str_repeat("ab", 3);
来源：http://kv.jctech888.com.cn

JS:   "ab".repeat(3)
来源：http://ki.shxzskj.cn

TS:   "ab".repeat(3)
来源：http://tu.521024.cn

Java: "ab".repeat(3)
来源：http://by.jctech888.com.cn

Go:   strings.Repeat("ab", 3)
来源：http://yu.yuexingan06.cn

Ruby: "ab" * 3
来源：http://wb.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ah.asd995.cn

[E03] 截取子串
来源：http://zg.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wg.szsharing.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qs.huixiangedu.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zf.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://ur.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://ne.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jw.521024.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sz.wgjwhj.cn

C#:   s.Substring(1, 3)
来源：http://ps.521024.cn

[E04] 查找子串位置
来源：http://yo.yuntaijiaju.cn

Py:   s.find("x");  s.index("x")
来源：http://cz.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://mc.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xx.bjjhwx.cn

TS:   s.indexOf("x")
来源：http://ce.yuexingan06.cn

Java: s.indexOf("x")
来源：http://wp.wgjwhj.cn

Go:   strings.Index(s, "x")
来源：http://jh.nszjky.cn

Ruby: s.index("x")
来源：http://pj.haigaiapp.cn

C#:   s.IndexOf("x")
来源：http://fi.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kw.yuntaijiaju.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oc.lnxyls.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://rq.shxzskj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wi.shxzukj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qj.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://oq.huanxung.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ou.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gu.haigaiapp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://cw.bookmarksfly.cn

[E06] 替换子串
来源：http://xr.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://qb.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://zy.yuntaijiaju.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hk.bookmarksfly.cn

TS:   s.replaceAll("a", "b")
来源：http://hk.asd995.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qv.hnjuh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://px.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ed.shxzskj.cn

C#:   s.Replace("a", "b")
来源：http://ig.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://hi.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wm.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://eo.huixiangedu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://io.huanxung.cn

TS:   s.split(",")
来源：http://hy.huanxung.cn

Java: s.split(",");  s.split("\\s+")
来源：http://mx.huixiangedu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ze.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://ij.chemitech.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jp.bjjhwx.cn

[E08] 数组按分隔符合并
来源：http://ev.9csxet.cn

Py:   ",".join(items)
来源：http://ke.huixinmuqiang.cn

PHP:  implode(",", $items);
来源：http://ii.shxzukj.cn

JS:   items.join(",")
来源：http://ry.hahajie.cn

TS:   items.join(",")
来源：http://iv.huixiangedu.cn

Java: String.join(",", items)
来源：http://px.haigaiapp.cn

Go:   strings.Join(items, ",")
来源：http://th.nicolike.cn

Ruby: items.join(",")
来源：http://mt.wgjwhj.cn

C#:   string.Join(",", items)
来源：http://ku.gzmigu.cn

[E09] 去除所有空白字符
来源：http://wv.szxytkj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zp.shxzskj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rv.szsharing.cn

JS:   s.replace(/\s+/g, "")
来源：http://jj.panjiajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://jm.521024.cn

Java: s.replaceAll("\\s+", "")
来源：http://gr.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jw.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ai.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tq.bookmarksfly.cn

[E10] 左侧补零 / 定长填充
来源：http://jg.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nh.szxytkj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vx.huixinmuqiang.cn

JS:   "7".padStart(3, "0")
来源：http://eu.szxytkj.cn

TS:   "7".padStart(3, "0")
来源：http://mz.huixinmuqiang.cn

Java: String.format("%03d", 7)
来源：http://lz.haigaiapp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kp.szsharing.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ga.jctech888.com.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://jj.yuexingan06.cn

[E11] 反转字符串
来源：http://jr.huanxung.cn

Py:   s[::-1]
来源：http://ci.huixiangedu.cn

PHP:  strrev($s);
来源：http://iz.asd995.cn

JS:   [...s].reverse().join("")
来源：http://we.bjjhwx.cn

TS:   [...s].reverse().join("")
来源：http://vg.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ex.muxihuayi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://nz.yuexingan06.cn

Ruby: s.reverse
来源：http://ut.hahajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ok.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://pi.chemitech.net.cn

Py:   s.count("a")
来源：http://sr.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://le.jianghongdianzi.cn

JS:   s.split("a").length - 1
来源：http://ad.yuexingan06.cn

TS:   s.split("a").length - 1
来源：http://kh.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://iw.shxzukj.cn

Go:   strings.Count(s, "a")
来源：http://wh.521024.cn

Ruby: s.count("a")
来源：http://nc.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://de.shxzskj.cn

[E13] 逐字符遍历
来源：http://wk.nszjky.cn

Py:   for ch in s: print(ch)
来源：http://qi.shxzukj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ie.colortex.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nx.wgjwhj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ks.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ug.huanxung.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fd.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://je.nszjky.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hl.szsharing.cn

[E14] URL 编码与 Base64
来源：http://xd.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xd.shtwfgs.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lr.lnxyls.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ew.nszjky.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rt.colortex.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ab.szxytkj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nq.szxytkj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yt.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vi.gzmigu.cn

[E15] HTML 转义 / 反转义
来源：http://hq.hahajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ck.chemitech.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qv.jianghongdianzi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ce.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://og.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wz.colortex.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qp.hnjuh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://se.szxytkj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eq.shtwfgs.cn

[E16] 数字千分位
来源：http://nk.nszjky.cn

Py:   f"{1234567:,}"
来源：http://bi.521024.cn

PHP:  number_format(1234567);
来源：http://ux.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dz.huixinmuqiang.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xw.9csxet.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wd.jianghongdianzi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ah.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qv.colortex.cn

C#:   1234567.ToString("N0")
来源：http://lv.wgjwhj.cn

[E17] 首字母大写
来源：http://js.shxzskj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nf.szxytkj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nu.szsharing.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ys.huanxung.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vb.colortex.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ck.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ht.hnjuh.cn

Ruby: s.capitalize
来源：http://mz.hahajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sj.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://lv.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mx.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yu.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ze.szsharing.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ob.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://iu.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jj.yuexingan06.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gg.asd995.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ky.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://df.haigaiapp.cn

Py:   s.splitlines()
来源：http://pd.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cw.colortex.cn

JS:   s.split(/\r?\n/)
来源：http://aa.nicolike.cn

TS:   s.split(/\r?\n/)
来源：http://co.jctech888.com.cn

Java: s.lines().toList()
来源：http://kt.colortex.cn

Go:   strings.Split(s, "\n")
来源：http://ur.szxytkj.cn

Ruby: s.lines
来源：http://hk.muxihuayi.cn

C#:   s.Split('\n')
来源：http://pt.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://ov.bookmarksfly.cn

Py:   if not s:
来源：http://eg.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ao.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lu.gzmigu.cn

TS:   if (s === "") {}
来源：http://fy.jianghongdianzi.cn

Java: if (s.isEmpty()) {}
来源：http://jj.muxihuayi.cn

Go:   if s == "" {}
来源：http://zq.hnjuh.cn

Ruby: if s.empty?
来源：http://qc.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ai.hnjuh.cn

[E21] 超长截断加省略号
来源：http://ql.wgjwhj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://im.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ku.yuntaijiaju.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://za.nszjky.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ll.shxzskj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ic.gzmigu.cn

Go:   // 按 rune 判断长度后截断
来源：http://oq.yuntaijiaju.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://up.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yf.yuntaijiaju.cn

[E22] 字节长度与字符长度
来源：http://zm.521024.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jn.nszjky.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xb.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tz.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jm.yuntaijiaju.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vw.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ym.panjiajie.cn

Ruby: s.bytesize;  s.length
来源：http://nk.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yr.521024.cn

================================================================================
来源：http://ce.521024.cn

F. 文件与目录
来源：http://rn.yuexingan06.cn

================================================================================
来源：http://sl.szsharing.cn

[F01] 读取整个文件
来源：http://qx.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://am.colortex.cn

PHP:  file_get_contents("a.txt");
来源：http://ba.panjiajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ln.hahajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gy.gzmigu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://aj.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zt.nicolike.cn

Ruby: File.read("a.txt")
来源：http://pu.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://po.panjiajie.cn

[F02] 逐行读取文件
来源：http://zn.bookmarksfly.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qn.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xi.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://or.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gu.newstarts.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pz.colortex.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qi.huanxung.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cy.huixinmuqiang.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ch.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://nq.gzmigu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nc.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ty.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dq.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ct.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mi.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fp.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://yi.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qq.nszjky.cn

[F04] 追加写入文件
来源：http://hm.shxzukj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://up.huanxung.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hk.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://en.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zv.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://um.nicolike.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tw.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vm.yuexingan06.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vs.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://zl.hahajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dh.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://yp.bookmarksfly.cn

JS:   fs.existsSync("a.txt")
来源：http://ft.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://yq.asd995.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pz.yuntaijiaju.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cl.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://zz.huixinmuqiang.cn

C#:   File.Exists("a.txt")
来源：http://eh.shxzukj.cn

[F06] 删除文件
来源：http://mj.huanxung.cn

Py:   os.remove("a.txt")
来源：http://wx.nszjky.cn

PHP:  unlink("a.txt");
来源：http://ak.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qj.hnjuh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qt.haigaiapp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rx.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://fz.521024.cn

Ruby: File.delete("a.txt")
来源：http://ug.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://gz.huanxung.cn

[F07] 创建目录（含多级）
来源：http://jh.muxihuayi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qm.hahajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ll.shxzukj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ho.haigaiapp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nc.newstarts.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rh.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://aq.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://et.newstarts.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://to.lnxyls.cn

[F08] 遍历目录
来源：http://bt.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://uk.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zj.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://dn.yuntaijiaju.cn

TS:   fs.readdirSync("dir")
来源：http://ei.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ng.huixinmuqiang.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kp.bookmarksfly.cn

Ruby: Dir.children("dir")
来源：http://mz.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://rs.nszjky.cn

[F09] 获取文件大小
来源：http://yt.lnxyls.cn

Py:   os.path.getsize("a.txt")
来源：http://yn.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://xm.asd995.cn

JS:   fs.statSync("a.txt").size
来源：http://vg.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://li.nszjky.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hb.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vi.haigaiapp.cn

Ruby: File.size("a.txt")
来源：http://hm.haigaiapp.cn


<!-- 参考信息 -->