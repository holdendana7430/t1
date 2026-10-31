代发 wailian999

================================================================================
来源：http://fo.colortex.cn

E. 字符串处理
来源：http://ic.bjjhwx.cn

================================================================================
来源：http://ih.9csxet.cn

[E01] 拼接字符串
来源：http://ln.haigaiapp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ox.newstarts.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gs.nicolike.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://oe.huixinmuqiang.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ju.haigaiapp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://po.shtwfgs.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wd.haigaiapp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://uv.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cj.szxytkj.cn

[E02] 重复字符串
来源：http://zq.shxzukj.cn

Py:   "ab" * 3
来源：http://ph.nicolike.cn

PHP:  str_repeat("ab", 3);
来源：http://br.nicolike.cn

JS:   "ab".repeat(3)
来源：http://vu.nszjky.cn

TS:   "ab".repeat(3)
来源：http://lj.asd995.cn

Java: "ab".repeat(3)
来源：http://jo.yuntaijiaju.cn

Go:   strings.Repeat("ab", 3)
来源：http://ho.huixinmuqiang.cn

Ruby: "ab" * 3
来源：http://db.shxzskj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://is.hahajie.cn

[E03] 截取子串
来源：http://kb.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vm.huixiangedu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://kw.shxzskj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://zu.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://xx.colortex.cn

Java: s.substring(1, 4)
来源：http://pp.jianghongdianzi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ks.yuntaijiaju.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jz.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://af.szsharing.cn

[E04] 查找子串位置
来源：http://ab.shxzukj.cn

Py:   s.find("x");  s.index("x")
来源：http://jp.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://yy.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ro.nicolike.cn

TS:   s.indexOf("x")
来源：http://ys.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://ac.wgjwhj.cn

Go:   strings.Index(s, "x")
来源：http://ne.hnjuh.cn

Ruby: s.index("x")
来源：http://wv.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://ya.lnxyls.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ax.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fi.521024.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://gk.nszjky.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jj.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://nr.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://to.hnjuh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fc.asd995.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jf.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://an.jianghongdianzi.cn

[E06] 替换子串
来源：http://gt.huixinmuqiang.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://uc.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://an.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fn.yuexingan06.cn

TS:   s.replaceAll("a", "b")
来源：http://qn.huixinmuqiang.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ad.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sh.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://zo.hnjuh.cn

C#:   s.Replace("a", "b")
来源：http://wz.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://wt.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xy.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://op.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://xo.bookmarksfly.cn

TS:   s.split(",")
来源：http://nv.gzmigu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xz.panjiajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yj.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://mg.hnjuh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tc.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://xj.chemitech.net.cn

Py:   ",".join(items)
来源：http://py.huixinmuqiang.cn

PHP:  implode(",", $items);
来源：http://pd.huixiangedu.cn

JS:   items.join(",")
来源：http://bo.huixinmuqiang.cn

TS:   items.join(",")
来源：http://ae.haigaiapp.cn

Java: String.join(",", items)
来源：http://au.lnxyls.cn

Go:   strings.Join(items, ",")
来源：http://ad.szsharing.cn

Ruby: items.join(",")
来源：http://mr.shxzukj.cn

C#:   string.Join(",", items)
来源：http://nd.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://rs.haigaiapp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://cf.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ey.huixiangedu.cn

JS:   s.replace(/\s+/g, "")
来源：http://js.yuexingan06.cn

TS:   s.replace(/\s+/g, "")
来源：http://fq.wgjwhj.cn

Java: s.replaceAll("\\s+", "")
来源：http://yv.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gj.muxihuayi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bh.muxihuayi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lc.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://yk.nszjky.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wp.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hu.521024.cn

JS:   "7".padStart(3, "0")
来源：http://yq.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://so.muxihuayi.cn

Java: String.format("%03d", 7)
来源：http://yw.newstarts.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mc.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gb.yuntaijiaju.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://oz.lnxyls.cn

[E11] 反转字符串
来源：http://xb.huanxung.cn

Py:   s[::-1]
来源：http://ue.haigaiapp.cn

PHP:  strrev($s);
来源：http://yx.huixiangedu.cn

JS:   [...s].reverse().join("")
来源：http://xy.szxytkj.cn

TS:   [...s].reverse().join("")
来源：http://kc.panjiajie.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://js.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://we.muxihuayi.cn

Ruby: s.reverse
来源：http://ef.lnxyls.cn

C#:   new string(s.Reverse().ToArray())
来源：http://uz.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://lg.colortex.cn

Py:   s.count("a")
来源：http://ua.521024.cn

PHP:  substr_count($s, "a");
来源：http://dt.bookmarksfly.cn

JS:   s.split("a").length - 1
来源：http://eu.panjiajie.cn

TS:   s.split("a").length - 1
来源：http://rr.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gz.lnxyls.cn

Go:   strings.Count(s, "a")
来源：http://mb.hahajie.cn

Ruby: s.count("a")
来源：http://ll.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://qw.jctech888.com.cn

[E13] 逐字符遍历
来源：http://dv.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://xb.jianghongdianzi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dl.szsharing.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://er.chemitech.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wc.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wi.colortex.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ii.haigaiapp.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uj.jianghongdianzi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jn.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://ai.bjjhwx.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ro.shtwfgs.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ab.hahajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tr.shxzukj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ah.nicolike.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xw.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://iv.colortex.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://zw.jctech888.com.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ob.panjiajie.cn

[E15] HTML 转义 / 反转义
来源：http://ty.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ou.shtwfgs.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ox.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xa.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ny.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yi.newstarts.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vc.wgjwhj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://by.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yu.jctech888.com.cn

[E16] 数字千分位
来源：http://xg.hahajie.cn

Py:   f"{1234567:,}"
来源：http://ac.newstarts.cn

PHP:  number_format(1234567);
来源：http://dg.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fz.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rk.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pm.bjjhwx.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ui.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nr.huanxung.cn

C#:   1234567.ToString("N0")
来源：http://wn.yuntaijiaju.cn

[E17] 首字母大写
来源：http://nf.colortex.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wm.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dn.haigaiapp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://aw.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ro.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://de.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cl.panjiajie.cn

Ruby: s.capitalize
来源：http://ob.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://he.chemitech.net.cn

[E18] 模板占位符替换
来源：http://mb.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rb.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ug.yuexingan06.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kr.wgjwhj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ac.chemitech.net.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fq.huanxung.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bw.9csxet.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oc.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gp.bjjhwx.cn

[E19] 多行文本按行拆分
来源：http://ii.shxzukj.cn

Py:   s.splitlines()
来源：http://td.colortex.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mh.9csxet.cn

JS:   s.split(/\r?\n/)
来源：http://vt.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://ul.bookmarksfly.cn

Java: s.lines().toList()
来源：http://nh.nicolike.cn

Go:   strings.Split(s, "\n")
来源：http://ba.nszjky.cn

Ruby: s.lines
来源：http://ls.muxihuayi.cn

C#:   s.Split('\n')
来源：http://xc.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://dq.nicolike.cn

Py:   if not s:
来源：http://so.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://zu.huixinmuqiang.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mc.panjiajie.cn

TS:   if (s === "") {}
来源：http://fk.huixinmuqiang.cn

Java: if (s.isEmpty()) {}
来源：http://wl.chemitech.net.cn

Go:   if s == "" {}
来源：http://ro.wgjwhj.cn

Ruby: if s.empty?
来源：http://ke.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mc.szxytkj.cn

[E21] 超长截断加省略号
来源：http://rl.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lw.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://re.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bu.szxytkj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ze.huanxung.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fa.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://fr.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nd.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fo.shtwfgs.cn

[E22] 字节长度与字符长度
来源：http://gn.bjjhwx.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wc.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tu.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cj.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nu.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mj.shtwfgs.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pn.jianghongdianzi.cn

Ruby: s.bytesize;  s.length
来源：http://ic.huanxung.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kf.szxytkj.cn

================================================================================
来源：http://de.521024.cn

F. 文件与目录
来源：http://fq.yuexingan06.cn

================================================================================
来源：http://cb.szxytkj.cn

[F01] 读取整个文件
来源：http://lw.huixinmuqiang.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cp.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://vq.hnjuh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://id.hnjuh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://km.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ai.bjjhwx.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sc.panjiajie.cn

Ruby: File.read("a.txt")
来源：http://mc.9csxet.cn

C#:   File.ReadAllText("a.txt");
来源：http://hb.asd995.cn

[F02] 逐行读取文件
来源：http://ga.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ss.newstarts.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://re.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jz.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xy.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wr.bjjhwx.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oh.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://eo.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rx.colortex.cn

[F03] 写入文件（覆盖）
来源：http://nr.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ee.nszjky.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://th.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gb.521024.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zr.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ca.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://dh.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://np.newstarts.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jj.newstarts.cn

[F04] 追加写入文件
来源：http://jl.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sf.huanxung.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://js.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://el.huixinmuqiang.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kx.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yc.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://co.wgjwhj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ip.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cd.huixinmuqiang.cn

[F05] 判断文件或目录是否存在
来源：http://ge.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ab.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://ww.hnjuh.cn

JS:   fs.existsSync("a.txt")
来源：http://de.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://ls.lnxyls.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://iz.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ww.szxytkj.cn

Ruby: File.exist?("a.txt")
来源：http://ox.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://ch.colortex.cn

[F06] 删除文件
来源：http://by.colortex.cn

Py:   os.remove("a.txt")
来源：http://zo.yuexingan06.cn

PHP:  unlink("a.txt");
来源：http://sf.jianghongdianzi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jf.jctech888.com.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cn.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sf.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://bp.nszjky.cn

Ruby: File.delete("a.txt")
来源：http://pp.colortex.cn

C#:   File.Delete("a.txt");
来源：http://sw.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://mm.bookmarksfly.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wv.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vo.huanxung.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ae.wgjwhj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ih.yuntaijiaju.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zv.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qe.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eo.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kb.lnxyls.cn

[F08] 遍历目录
来源：http://hz.huanxung.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ea.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eg.wgjwhj.cn

JS:   fs.readdirSync("dir")
来源：http://ll.panjiajie.cn

TS:   fs.readdirSync("dir")
来源：http://dq.nszjky.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qd.nicolike.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lz.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://wh.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://cs.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://bd.szxytkj.cn

Py:   os.path.getsize("a.txt")
来源：http://uv.hahajie.cn

PHP:  filesize("a.txt");
来源：http://iu.gzmigu.cn

JS:   fs.statSync("a.txt").size
来源：http://it.yuntaijiaju.cn

TS:   fs.statSync("a.txt").size
来源：http://uh.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ve.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mh.521024.cn

Ruby: File.size("a.txt")
来源：http://qi.nszjky.cn

C#:   new FileInfo("a.txt").Length
来源：http://qc.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://aq.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hi.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lg.hahajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yt.gzmigu.cn

TS:   path.extname("a.txt")
来源：http://bt.lnxyls.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jt.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vz.lnxyls.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ga.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tg.haigaiapp.cn

[F11] 复制与移动文件
来源：http://qf.huixiangedu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bm.huixiangedu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bp.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nu.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://je.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ow.lnxyls.cn


<!-- 参考信息 -->