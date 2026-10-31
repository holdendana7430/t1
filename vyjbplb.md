代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kq.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://er.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://om.colortex.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sj.bookmarksfly.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://by.hnjuh.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zy.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qd.nicolike.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qg.bjjhwx.cn

[E02] 重复字符串
来源：http://al.huanxung.cn

Py:   "ab" * 3
来源：http://mk.yuexingan06.cn

PHP:  str_repeat("ab", 3);
来源：http://zq.szsharing.cn

JS:   "ab".repeat(3)
来源：http://ac.9csxet.cn

TS:   "ab".repeat(3)
来源：http://yb.9csxet.cn

Java: "ab".repeat(3)
来源：http://qi.muxihuayi.cn

Go:   strings.Repeat("ab", 3)
来源：http://rs.hnjuh.cn

Ruby: "ab" * 3
来源：http://ae.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mg.haigaiapp.cn

[E03] 截取子串
来源：http://ll.chemitech.net.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rl.wgjwhj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://su.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vf.asd995.cn

TS:   s.slice(1, 4)
来源：http://da.shxzskj.cn

Java: s.substring(1, 4)
来源：http://du.yuexingan06.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wj.panjiajie.cn

Ruby: s[1, 3];  s[1..3]
来源：http://tx.wgjwhj.cn

C#:   s.Substring(1, 3)
来源：http://fo.wgjwhj.cn

[E04] 查找子串位置
来源：http://zw.huixinmuqiang.cn

Py:   s.find("x");  s.index("x")
来源：http://mg.szsharing.cn

PHP:  strpos($s, "x");
来源：http://lz.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wv.yuntaijiaju.cn

TS:   s.indexOf("x")
来源：http://gd.asd995.cn

Java: s.indexOf("x")
来源：http://zf.huanxung.cn

Go:   strings.Index(s, "x")
来源：http://xt.wgjwhj.cn

Ruby: s.index("x")
来源：http://nr.newstarts.cn

C#:   s.IndexOf("x")
来源：http://ol.nszjky.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ub.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://zc.lnxyls.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://qu.panjiajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jc.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://go.huixiangedu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ya.haigaiapp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dn.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://tk.szsharing.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://uw.huanxung.cn

[E06] 替换子串
来源：http://pa.jctech888.com.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ug.hnjuh.cn

PHP:  str_replace("a", "b", $s);
来源：http://nw.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fq.hnjuh.cn

TS:   s.replaceAll("a", "b")
来源：http://ty.huanxung.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://az.yuexingan06.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mw.colortex.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ah.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://os.nicolike.cn

[E07] 按分隔符拆分
来源：http://rw.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qq.yuntaijiaju.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uf.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jt.huixinmuqiang.cn

TS:   s.split(",")
来源：http://kn.colortex.cn

Java: s.split(",");  s.split("\\s+")
来源：http://pn.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lt.521024.cn

Ruby: s.split(",");  s.split
来源：http://uj.muxihuayi.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://an.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://aa.colortex.cn

Py:   ",".join(items)
来源：http://ly.hahajie.cn

PHP:  implode(",", $items);
来源：http://nr.521024.cn

JS:   items.join(",")
来源：http://yp.bjjhwx.cn

TS:   items.join(",")
来源：http://af.9csxet.cn

Java: String.join(",", items)
来源：http://fy.colortex.cn

Go:   strings.Join(items, ",")
来源：http://zr.szsharing.cn

Ruby: items.join(",")
来源：http://su.nszjky.cn

C#:   string.Join(",", items)
来源：http://ks.szxytkj.cn

[E09] 去除所有空白字符
来源：http://ux.huixinmuqiang.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://gu.asd995.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://go.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://pc.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://gl.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://cz.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://um.newstarts.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fm.shtwfgs.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zm.szxytkj.cn

[E10] 左侧补零 / 定长填充
来源：http://fn.jianghongdianzi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wv.lnxyls.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vd.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://qu.panjiajie.cn

TS:   "7".padStart(3, "0")
来源：http://ba.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://ek.huixiangedu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://be.newstarts.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://do.huixinmuqiang.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://je.newstarts.cn

[E11] 反转字符串
来源：http://hc.wgjwhj.cn

Py:   s[::-1]
来源：http://ji.huanxung.cn

PHP:  strrev($s);
来源：http://bb.jianghongdianzi.cn

JS:   [...s].reverse().join("")
来源：http://xg.asd995.cn

TS:   [...s].reverse().join("")
来源：http://ft.shxzukj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ut.jianghongdianzi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qn.szsharing.cn

Ruby: s.reverse
来源：http://jp.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xf.nszjky.cn

[E12] 统计某字符出现次数
来源：http://ag.colortex.cn

Py:   s.count("a")
来源：http://qg.chemitech.net.cn

PHP:  substr_count($s, "a");
来源：http://fu.colortex.cn

JS:   s.split("a").length - 1
来源：http://vj.muxihuayi.cn

TS:   s.split("a").length - 1
来源：http://qn.szsharing.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kv.jctech888.com.cn

Go:   strings.Count(s, "a")
来源：http://rf.huanxung.cn

Ruby: s.count("a")
来源：http://zg.colortex.cn

C#:   s.Count(c => c == 'a')
来源：http://tg.hnjuh.cn

[E13] 逐字符遍历
来源：http://ts.colortex.cn

Py:   for ch in s: print(ch)
来源：http://to.bookmarksfly.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mb.panjiajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://jw.gzmigu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://kq.muxihuayi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gt.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rj.panjiajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ti.haigaiapp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ls.asd995.cn

[E14] URL 编码与 Base64
来源：http://lr.asd995.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rf.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ki.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zs.shtwfgs.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zd.shxzskj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qb.muxihuayi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wh.9csxet.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lk.hahajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://kw.jctech888.com.cn

[E15] HTML 转义 / 反转义
来源：http://qa.bookmarksfly.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://vd.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bs.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dd.wgjwhj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tz.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yn.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://an.szsharing.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://yx.shxzskj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sv.muxihuayi.cn

[E16] 数字千分位
来源：http://zz.nicolike.cn

Py:   f"{1234567:,}"
来源：http://ln.gzmigu.cn

PHP:  number_format(1234567);
来源：http://ox.shtwfgs.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zu.521024.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gj.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ui.szsharing.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qh.jctech888.com.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ay.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://tf.hnjuh.cn

[E17] 首字母大写
来源：http://fc.jianghongdianzi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://kw.521024.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://le.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://up.panjiajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qd.nszjky.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ug.jianghongdianzi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hw.haigaiapp.cn

Ruby: s.capitalize
来源：http://rz.jianghongdianzi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ei.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://mu.jctech888.com.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zv.jianghongdianzi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pr.shtwfgs.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rp.newstarts.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kg.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://jo.szxytkj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gi.yuexingan06.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://by.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qx.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://hn.newstarts.cn

Py:   s.splitlines()
来源：http://qk.panjiajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yc.wgjwhj.cn

JS:   s.split(/\r?\n/)
来源：http://yn.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://hz.bookmarksfly.cn

Java: s.lines().toList()
来源：http://lc.haigaiapp.cn

Go:   strings.Split(s, "\n")
来源：http://zq.shxzskj.cn

Ruby: s.lines
来源：http://ec.hnjuh.cn

C#:   s.Split('\n')
来源：http://jd.jianghongdianzi.cn

[E20] 判断字符串是否为空
来源：http://ew.yuexingan06.cn

Py:   if not s:
来源：http://nb.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rf.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wm.huixiangedu.cn

TS:   if (s === "") {}
来源：http://km.huixiangedu.cn

Java: if (s.isEmpty()) {}
来源：http://nw.asd995.cn

Go:   if s == "" {}
来源：http://ab.shxzukj.cn

Ruby: if s.empty?
来源：http://by.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qw.asd995.cn

[E21] 超长截断加省略号
来源：http://va.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bb.szsharing.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ey.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://do.521024.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vr.szsharing.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nm.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://yx.gzmigu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fn.jctech888.com.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sr.chemitech.net.cn

[E22] 字节长度与字符长度
来源：http://fw.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://vd.shtwfgs.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ye.521024.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://is.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://if.gzmigu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hr.hnjuh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gh.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://ci.jianghongdianzi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://df.nicolike.cn

================================================================================
来源：http://zk.lnxyls.cn

F. 文件与目录
来源：http://hq.huanxung.cn

================================================================================
来源：http://ku.haigaiapp.cn

[F01] 读取整个文件
来源：http://hg.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://pt.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://vv.shxzukj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hp.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xn.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yq.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ho.jctech888.com.cn

Ruby: File.read("a.txt")
来源：http://um.lnxyls.cn

C#:   File.ReadAllText("a.txt");
来源：http://ns.nszjky.cn

[F02] 逐行读取文件
来源：http://un.newstarts.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lc.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rg.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mp.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ul.asd995.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ot.hnjuh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wg.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wi.huixinmuqiang.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sy.asd995.cn

[F03] 写入文件（覆盖）
来源：http://gi.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nz.huanxung.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hm.bookmarksfly.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pw.521024.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ll.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qz.shxzukj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nr.lnxyls.cn

Ruby: File.write("a.txt", "hi")
来源：http://yl.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tk.wgjwhj.cn

[F04] 追加写入文件
来源：http://kh.colortex.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ir.nicolike.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://gr.chemitech.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ka.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vv.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bn.panjiajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ak.wgjwhj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wu.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kv.gzmigu.cn

[F05] 判断文件或目录是否存在
来源：http://yw.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gx.bjjhwx.cn

PHP:  file_exists("a.txt");
来源：http://nu.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://na.nicolike.cn

TS:   fs.existsSync("a.txt")
来源：http://du.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://im.haigaiapp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zn.hahajie.cn

Ruby: File.exist?("a.txt")
来源：http://nq.haigaiapp.cn

C#:   File.Exists("a.txt")
来源：http://cb.521024.cn

[F06] 删除文件
来源：http://lm.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://vu.yuntaijiaju.cn

PHP:  unlink("a.txt");
来源：http://vi.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://km.huanxung.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ug.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ct.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://wy.lnxyls.cn

Ruby: File.delete("a.txt")
来源：http://oi.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://xv.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://ce.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wx.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ed.szxytkj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fe.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://no.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bk.shxzskj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mn.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kx.521024.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pn.wgjwhj.cn

[F08] 遍历目录
来源：http://vd.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ay.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://li.haigaiapp.cn

JS:   fs.readdirSync("dir")
来源：http://ag.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://fc.newstarts.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vh.jianghongdianzi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sb.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://jg.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://fe.9csxet.cn

[F09] 获取文件大小
来源：http://vh.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://dr.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://ry.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://lg.jctech888.com.cn

TS:   fs.statSync("a.txt").size
来源：http://dk.yuntaijiaju.cn

Java: Files.size(Path.of("a.txt"))
来源：http://aj.haigaiapp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://eu.huixinmuqiang.cn

Ruby: File.size("a.txt")
来源：http://lv.shtwfgs.cn

C#:   new FileInfo("a.txt").Length
来源：http://at.hnjuh.cn

[F10] 取文件扩展名 / 文件名
来源：http://zb.colortex.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nv.nszjky.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gq.chemitech.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fa.yuexingan06.cn

TS:   path.extname("a.txt")
来源：http://zr.newstarts.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ud.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dz.asd995.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cb.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://py.9csxet.cn

[F11] 复制与移动文件
来源：http://pe.shxzskj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bk.yuexingan06.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rc.newstarts.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yx.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rt.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mv.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://al.szsharing.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://os.asd995.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bp.szxytkj.cn

[F12] CSV 读写
来源：http://wk.asd995.cn


<!-- 参考信息 -->