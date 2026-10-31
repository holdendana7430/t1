代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ej.hnjuh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://da.szsharing.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://az.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://km.panjiajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pe.hnjuh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fh.521024.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sg.colortex.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://us.yuexingan06.cn

[E02] 重复字符串
来源：http://sl.huanxung.cn

Py:   "ab" * 3
来源：http://lf.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://sp.yuexingan06.cn

JS:   "ab".repeat(3)
来源：http://zl.chemitech.net.cn

TS:   "ab".repeat(3)
来源：http://cd.yuntaijiaju.cn

Java: "ab".repeat(3)
来源：http://dh.muxihuayi.cn

Go:   strings.Repeat("ab", 3)
来源：http://bh.hnjuh.cn

Ruby: "ab" * 3
来源：http://mw.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://uf.gzmigu.cn

[E03] 截取子串
来源：http://ay.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yf.bookmarksfly.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://by.shtwfgs.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ky.yuexingan06.cn

TS:   s.slice(1, 4)
来源：http://co.huanxung.cn

Java: s.substring(1, 4)
来源：http://ka.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ca.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tz.huanxung.cn

C#:   s.Substring(1, 3)
来源：http://jj.yuntaijiaju.cn

[E04] 查找子串位置
来源：http://xn.lnxyls.cn

Py:   s.find("x");  s.index("x")
来源：http://mu.yuexingan06.cn

PHP:  strpos($s, "x");
来源：http://jo.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ku.wgjwhj.cn

TS:   s.indexOf("x")
来源：http://lq.szsharing.cn

Java: s.indexOf("x")
来源：http://wg.bjjhwx.cn

Go:   strings.Index(s, "x")
来源：http://mu.szsharing.cn

Ruby: s.index("x")
来源：http://ox.yuntaijiaju.cn

C#:   s.IndexOf("x")
来源：http://tw.yuexingan06.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://br.lnxyls.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qa.asd995.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ux.panjiajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fr.shxzukj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://py.wgjwhj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fb.jianghongdianzi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hk.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pl.gzmigu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wl.hahajie.cn

[E06] 替换子串
来源：http://tf.szxytkj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gs.newstarts.cn

PHP:  str_replace("a", "b", $s);
来源：http://tj.nszjky.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wx.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://xs.haigaiapp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kz.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ak.shxzskj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zx.yuexingan06.cn

C#:   s.Replace("a", "b")
来源：http://ux.shtwfgs.cn

[E07] 按分隔符拆分
来源：http://ia.nszjky.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pz.haigaiapp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ay.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xz.huixiangedu.cn

TS:   s.split(",")
来源：http://gf.gzmigu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dk.hnjuh.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ek.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://os.huanxung.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://aj.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://td.muxihuayi.cn

Py:   ",".join(items)
来源：http://ac.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://pt.chemitech.net.cn

JS:   items.join(",")
来源：http://gw.huixiangedu.cn

TS:   items.join(",")
来源：http://vn.gzmigu.cn

Java: String.join(",", items)
来源：http://ua.asd995.cn

Go:   strings.Join(items, ",")
来源：http://it.bookmarksfly.cn

Ruby: items.join(",")
来源：http://ss.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://rx.wgjwhj.cn

[E09] 去除所有空白字符
来源：http://pf.hnjuh.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wf.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ei.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://gp.huixinmuqiang.cn

TS:   s.replace(/\s+/g, "")
来源：http://nn.asd995.cn

Java: s.replaceAll("\\s+", "")
来源：http://iy.huixinmuqiang.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://an.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://cw.nicolike.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cf.asd995.cn

[E10] 左侧补零 / 定长填充
来源：http://kt.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wp.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bt.hahajie.cn

JS:   "7".padStart(3, "0")
来源：http://ag.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://ak.521024.cn

Java: String.format("%03d", 7)
来源：http://gr.haigaiapp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wm.nszjky.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dj.huanxung.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pt.shtwfgs.cn

[E11] 反转字符串
来源：http://zw.huanxung.cn

Py:   s[::-1]
来源：http://qe.yuntaijiaju.cn

PHP:  strrev($s);
来源：http://xz.panjiajie.cn

JS:   [...s].reverse().join("")
来源：http://co.jctech888.com.cn

TS:   [...s].reverse().join("")
来源：http://ma.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://oy.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ys.jianghongdianzi.cn

Ruby: s.reverse
来源：http://ih.jctech888.com.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hg.huanxung.cn

[E12] 统计某字符出现次数
来源：http://uv.yuntaijiaju.cn

Py:   s.count("a")
来源：http://dz.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://by.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://xb.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://ft.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ke.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://mw.gzmigu.cn

Ruby: s.count("a")
来源：http://ew.wgjwhj.cn

C#:   s.Count(c => c == 'a')
来源：http://hn.hahajie.cn

[E13] 逐字符遍历
来源：http://yt.lnxyls.cn

Py:   for ch in s: print(ch)
来源：http://tc.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ho.hnjuh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gm.hnjuh.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yc.bookmarksfly.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ro.yuntaijiaju.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://sb.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sk.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uf.colortex.cn

[E14] URL 编码与 Base64
来源：http://xy.gzmigu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://la.jianghongdianzi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ks.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wx.shxzskj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tr.yuexingan06.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wb.newstarts.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gr.nszjky.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wi.jianghongdianzi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://np.jianghongdianzi.cn

[E15] HTML 转义 / 反转义
来源：http://lc.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://my.chemitech.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dx.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ot.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://np.panjiajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wx.shxzskj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ss.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vf.jianghongdianzi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bo.hnjuh.cn

[E16] 数字千分位
来源：http://go.9csxet.cn

Py:   f"{1234567:,}"
来源：http://bx.szxytkj.cn

PHP:  number_format(1234567);
来源：http://qe.colortex.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vj.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zx.nicolike.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kq.nszjky.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tm.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mo.lnxyls.cn

C#:   1234567.ToString("N0")
来源：http://hs.lnxyls.cn

[E17] 首字母大写
来源：http://uu.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ni.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mj.shxzukj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xx.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jk.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hp.shtwfgs.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rh.panjiajie.cn

Ruby: s.capitalize
来源：http://gp.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wp.521024.cn

[E18] 模板占位符替换
来源：http://vu.shtwfgs.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zv.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yv.panjiajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://uk.nicolike.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kx.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://aw.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yu.shxzukj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xu.lnxyls.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nr.shxzukj.cn

[E19] 多行文本按行拆分
来源：http://wh.yuexingan06.cn

Py:   s.splitlines()
来源：http://iq.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qh.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://nb.jianghongdianzi.cn

TS:   s.split(/\r?\n/)
来源：http://hu.muxihuayi.cn

Java: s.lines().toList()
来源：http://yz.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://yg.asd995.cn

Ruby: s.lines
来源：http://cm.9csxet.cn

C#:   s.Split('\n')
来源：http://jc.wgjwhj.cn

[E20] 判断字符串是否为空
来源：http://vh.shxzskj.cn

Py:   if not s:
来源：http://za.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kw.lnxyls.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xl.szsharing.cn

TS:   if (s === "") {}
来源：http://zf.asd995.cn

Java: if (s.isEmpty()) {}
来源：http://ky.wgjwhj.cn

Go:   if s == "" {}
来源：http://jo.hahajie.cn

Ruby: if s.empty?
来源：http://lx.shtwfgs.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ug.nicolike.cn

[E21] 超长截断加省略号
来源：http://ku.lnxyls.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ub.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://fu.haigaiapp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xk.hnjuh.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cl.huixinmuqiang.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mb.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://ud.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cu.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pc.asd995.cn

[E22] 字节长度与字符长度
来源：http://cg.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nf.haigaiapp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uk.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mw.lnxyls.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lj.9csxet.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yv.jctech888.com.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sj.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://rh.huixiangedu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ta.bookmarksfly.cn

================================================================================
来源：http://wj.chemitech.net.cn

F. 文件与目录
来源：http://qc.wgjwhj.cn

================================================================================
来源：http://jn.huixiangedu.cn

[F01] 读取整个文件
来源：http://zi.shtwfgs.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dc.shxzukj.cn

PHP:  file_get_contents("a.txt");
来源：http://yq.yuntaijiaju.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vf.shxzskj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cs.yuntaijiaju.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xe.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yf.szsharing.cn

Ruby: File.read("a.txt")
来源：http://kw.huanxung.cn

C#:   File.ReadAllText("a.txt");
来源：http://md.nszjky.cn

[F02] 逐行读取文件
来源：http://xj.bookmarksfly.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wi.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ni.wgjwhj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lp.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ql.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://iy.muxihuayi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xg.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ll.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xr.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://kg.szsharing.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ya.shtwfgs.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vk.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nk.521024.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hv.521024.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rn.gzmigu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bd.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://ql.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uo.haigaiapp.cn

[F04] 追加写入文件
来源：http://nm.hnjuh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://af.nicolike.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fs.huanxung.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rx.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wr.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lz.szsharing.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sw.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tn.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://eb.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://ak.wgjwhj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dm.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://jw.szsharing.cn

JS:   fs.existsSync("a.txt")
来源：http://gf.521024.cn

TS:   fs.existsSync("a.txt")
来源：http://af.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://tr.newstarts.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xo.yuexingan06.cn

Ruby: File.exist?("a.txt")
来源：http://lt.bookmarksfly.cn

C#:   File.Exists("a.txt")
来源：http://rt.521024.cn

[F06] 删除文件
来源：http://ei.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://wy.jianghongdianzi.cn

PHP:  unlink("a.txt");
来源：http://fe.huanxung.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yj.huixiangedu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ot.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yy.jctech888.com.cn

Go:   os.Remove("a.txt")
来源：http://sw.newstarts.cn

Ruby: File.delete("a.txt")
来源：http://oy.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://xy.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://kh.chemitech.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zl.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ud.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qu.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ti.huixiangedu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ua.yuntaijiaju.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ie.shtwfgs.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qo.panjiajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fh.jctech888.com.cn

[F08] 遍历目录
来源：http://zl.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bd.gzmigu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://od.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://ev.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://me.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xd.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zh.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://ea.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://uv.colortex.cn

[F09] 获取文件大小
来源：http://tb.szsharing.cn

Py:   os.path.getsize("a.txt")
来源：http://to.nicolike.cn

PHP:  filesize("a.txt");
来源：http://to.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://uc.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://ta.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rw.jianghongdianzi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://it.colortex.cn

Ruby: File.size("a.txt")
来源：http://rg.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://gv.szxytkj.cn

[F10] 取文件扩展名 / 文件名
来源：http://aj.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yj.bjjhwx.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bx.gzmigu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bo.hnjuh.cn

TS:   path.extname("a.txt")
来源：http://iu.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ci.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fy.jctech888.com.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pm.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lv.newstarts.cn

[F11] 复制与移动文件
来源：http://ow.shxzukj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dj.hahajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ch.shtwfgs.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tr.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ad.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zb.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dj.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mn.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://el.bookmarksfly.cn

[F12] CSV 读写
来源：http://op.jctech888.com.cn


<!-- 参考信息 -->