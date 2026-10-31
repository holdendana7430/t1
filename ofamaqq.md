代发 wailian999

Java: String.join(", ", list)
来源：http://gs.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://sm.panjiajie.cn

Ruby: arr.join(", ")
来源：http://ph.nicolike.cn

C#:   string.Join(", ", list)
来源：http://js.jianghongdianzi.cn

================================================================================
来源：http://tr.bookmarksfly.cn

E. 字符串处理
来源：http://wf.521024.cn

================================================================================
来源：http://ql.9csxet.cn

[E01] 拼接字符串
来源：http://tu.nicolike.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://vs.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://bq.yuntaijiaju.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kj.nszjky.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ug.nicolike.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ax.chemitech.net.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xu.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sk.yuntaijiaju.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gx.bookmarksfly.cn

[E02] 重复字符串
来源：http://dy.yuexingan06.cn

Py:   "ab" * 3
来源：http://mi.hnjuh.cn

PHP:  str_repeat("ab", 3);
来源：http://ih.lnxyls.cn

JS:   "ab".repeat(3)
来源：http://xl.newstarts.cn

TS:   "ab".repeat(3)
来源：http://mb.shtwfgs.cn

Java: "ab".repeat(3)
来源：http://ty.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://cp.bjjhwx.cn

Ruby: "ab" * 3
来源：http://ub.yuntaijiaju.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wz.hahajie.cn

[E03] 截取子串
来源：http://sg.huanxung.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ss.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uo.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fd.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://mz.bjjhwx.cn

Java: s.substring(1, 4)
来源：http://us.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://id.huixiangedu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jy.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://pw.huixinmuqiang.cn

[E04] 查找子串位置
来源：http://rj.huixiangedu.cn

Py:   s.find("x");  s.index("x")
来源：http://zr.bookmarksfly.cn

PHP:  strpos($s, "x");
来源：http://lx.szxytkj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fm.gzmigu.cn

TS:   s.indexOf("x")
来源：http://fd.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://oe.521024.cn

Go:   strings.Index(s, "x")
来源：http://gq.yuexingan06.cn

Ruby: s.index("x")
来源：http://iz.colortex.cn

C#:   s.IndexOf("x")
来源：http://ue.szsharing.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ni.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cs.lnxyls.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ck.bjjhwx.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jn.hahajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tj.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kd.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://un.nicolike.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mt.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qf.szxytkj.cn

[E06] 替换子串
来源：http://af.asd995.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fe.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://xz.hnjuh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rc.hahajie.cn

TS:   s.replaceAll("a", "b")
来源：http://yv.newstarts.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://id.bjjhwx.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qs.521024.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://kf.newstarts.cn

C#:   s.Replace("a", "b")
来源：http://pn.panjiajie.cn

[E07] 按分隔符拆分
来源：http://py.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://jh.yuntaijiaju.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ca.shxzukj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bx.szsharing.cn

TS:   s.split(",")
来源：http://hy.hahajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qt.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ye.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://aj.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fk.jianghongdianzi.cn

[E08] 数组按分隔符合并
来源：http://le.bookmarksfly.cn

Py:   ",".join(items)
来源：http://uf.huixiangedu.cn

PHP:  implode(",", $items);
来源：http://or.szsharing.cn

JS:   items.join(",")
来源：http://dz.wgjwhj.cn

TS:   items.join(",")
来源：http://mj.huixinmuqiang.cn

Java: String.join(",", items)
来源：http://bu.nicolike.cn

Go:   strings.Join(items, ",")
来源：http://jn.haigaiapp.cn

Ruby: items.join(",")
来源：http://ie.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://iy.colortex.cn

[E09] 去除所有空白字符
来源：http://br.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://up.shxzukj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zm.bjjhwx.cn

JS:   s.replace(/\s+/g, "")
来源：http://ij.szsharing.cn

TS:   s.replace(/\s+/g, "")
来源：http://is.bookmarksfly.cn

Java: s.replaceAll("\\s+", "")
来源：http://vb.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://uf.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://et.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://au.szxytkj.cn

[E10] 左侧补零 / 定长填充
来源：http://xk.szsharing.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wz.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rw.jianghongdianzi.cn

JS:   "7".padStart(3, "0")
来源：http://vp.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://oz.szxytkj.cn

Java: String.format("%03d", 7)
来源：http://wq.muxihuayi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pn.szxytkj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fd.hnjuh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nz.hnjuh.cn

[E11] 反转字符串
来源：http://hb.yuntaijiaju.cn

Py:   s[::-1]
来源：http://ah.newstarts.cn

PHP:  strrev($s);
来源：http://jp.lnxyls.cn

JS:   [...s].reverse().join("")
来源：http://fq.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://zf.wgjwhj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gf.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gs.huixinmuqiang.cn

Ruby: s.reverse
来源：http://om.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gz.colortex.cn

[E12] 统计某字符出现次数
来源：http://yf.chemitech.net.cn

Py:   s.count("a")
来源：http://bt.9csxet.cn

PHP:  substr_count($s, "a");
来源：http://ai.bookmarksfly.cn

JS:   s.split("a").length - 1
来源：http://uv.hahajie.cn

TS:   s.split("a").length - 1
来源：http://or.shxzukj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fd.panjiajie.cn

Go:   strings.Count(s, "a")
来源：http://hg.hnjuh.cn

Ruby: s.count("a")
来源：http://jz.shxzukj.cn

C#:   s.Count(c => c == 'a')
来源：http://vu.colortex.cn

[E13] 逐字符遍历
来源：http://dp.bookmarksfly.cn

Py:   for ch in s: print(ch)
来源：http://sv.521024.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ib.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tf.gzmigu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fz.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qd.521024.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mz.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://jk.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ba.asd995.cn

[E14] URL 编码与 Base64
来源：http://zu.yuexingan06.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://iz.asd995.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://fq.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pe.shxzskj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ib.szxytkj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pe.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bu.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sr.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vo.chemitech.net.cn

[E15] HTML 转义 / 反转义
来源：http://kb.shxzskj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uw.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sg.wgjwhj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bb.lnxyls.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sz.yuntaijiaju.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://by.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ig.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nh.nicolike.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pj.muxihuayi.cn

[E16] 数字千分位
来源：http://gh.shxzukj.cn

Py:   f"{1234567:,}"
来源：http://ov.jianghongdianzi.cn

PHP:  number_format(1234567);
来源：http://xn.521024.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://sl.szxytkj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ju.wgjwhj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yz.jianghongdianzi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lf.bjjhwx.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hv.haigaiapp.cn

C#:   1234567.ToString("N0")
来源：http://nk.9csxet.cn

[E17] 首字母大写
来源：http://yj.haigaiapp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cm.shxzskj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://za.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sq.asd995.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://si.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ye.wgjwhj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sq.gzmigu.cn

Ruby: s.capitalize
来源：http://tq.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://dy.lnxyls.cn

[E18] 模板占位符替换
来源：http://dd.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tw.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ya.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fu.szxytkj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tg.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yn.9csxet.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ap.bjjhwx.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://au.huanxung.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gw.panjiajie.cn

[E19] 多行文本按行拆分
来源：http://hi.asd995.cn

Py:   s.splitlines()
来源：http://gm.jianghongdianzi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cb.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://fn.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://or.huanxung.cn

Java: s.lines().toList()
来源：http://sg.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://mx.shtwfgs.cn

Ruby: s.lines
来源：http://cj.szsharing.cn

C#:   s.Split('\n')
来源：http://xy.panjiajie.cn

[E20] 判断字符串是否为空
来源：http://fw.newstarts.cn

Py:   if not s:
来源：http://ox.521024.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://go.newstarts.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yr.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://kc.panjiajie.cn

Java: if (s.isEmpty()) {}
来源：http://gd.gzmigu.cn

Go:   if s == "" {}
来源：http://ye.wgjwhj.cn

Ruby: if s.empty?
来源：http://ig.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lw.panjiajie.cn

[E21] 超长截断加省略号
来源：http://hb.yuexingan06.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wv.haigaiapp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bb.muxihuayi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qx.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rs.gzmigu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://dj.hahajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://ox.szsharing.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://rk.haigaiapp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uv.9csxet.cn

[E22] 字节长度与字符长度
来源：http://cf.jctech888.com.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://po.bjjhwx.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://br.jianghongdianzi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qi.jianghongdianzi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ts.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://bd.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://re.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://nm.bjjhwx.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mn.shtwfgs.cn

================================================================================
来源：http://mr.panjiajie.cn

F. 文件与目录
来源：http://xj.hnjuh.cn

================================================================================
来源：http://di.lnxyls.cn

[F01] 读取整个文件
来源：http://jx.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zq.asd995.cn

PHP:  file_get_contents("a.txt");
来源：http://lo.huixinmuqiang.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://xx.newstarts.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pw.shxzukj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vw.gzmigu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oo.wgjwhj.cn

Ruby: File.read("a.txt")
来源：http://oz.shxzukj.cn

C#:   File.ReadAllText("a.txt");
来源：http://bl.bookmarksfly.cn

[F02] 逐行读取文件
来源：http://ra.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lv.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ov.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aw.bookmarksfly.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zh.huixinmuqiang.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zp.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://gt.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://el.szxytkj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pb.yuexingan06.cn

[F03] 写入文件（覆盖）
来源：http://bd.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pb.shtwfgs.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yy.muxihuayi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yf.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rd.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://rc.haigaiapp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pt.haigaiapp.cn

Ruby: File.write("a.txt", "hi")
来源：http://ws.shxzskj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lr.nicolike.cn

[F04] 追加写入文件
来源：http://zz.panjiajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://af.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://td.huixinmuqiang.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nq.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kv.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cp.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jt.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vz.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ir.huanxung.cn

[F05] 判断文件或目录是否存在
来源：http://xy.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rz.hahajie.cn

PHP:  file_exists("a.txt");
来源：http://qd.chemitech.net.cn

JS:   fs.existsSync("a.txt")
来源：http://kj.521024.cn

TS:   fs.existsSync("a.txt")
来源：http://yl.huixiangedu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ct.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yu.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://gp.yuntaijiaju.cn

C#:   File.Exists("a.txt")
来源：http://fu.yuntaijiaju.cn

[F06] 删除文件
来源：http://hm.huixiangedu.cn

Py:   os.remove("a.txt")
来源：http://nf.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://jq.huixiangedu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wd.shxzskj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nw.szxytkj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mu.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://ca.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://xf.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://xc.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://vg.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://vd.yuexingan06.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zi.shxzukj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://to.szxytkj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xr.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jl.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zv.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sk.shtwfgs.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jo.muxihuayi.cn

[F08] 遍历目录
来源：http://jo.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://md.nicolike.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://de.muxihuayi.cn

JS:   fs.readdirSync("dir")
来源：http://zg.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://uc.nicolike.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ew.shxzskj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xz.9csxet.cn

Ruby: Dir.children("dir")
来源：http://uc.shxzukj.cn

C#:   Directory.GetFiles("dir")
来源：http://gt.szxytkj.cn

[F09] 获取文件大小
来源：http://pj.huixiangedu.cn

Py:   os.path.getsize("a.txt")
来源：http://id.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://cn.yuntaijiaju.cn

JS:   fs.statSync("a.txt").size
来源：http://qn.colortex.cn

TS:   fs.statSync("a.txt").size
来源：http://zb.bookmarksfly.cn

Java: Files.size(Path.of("a.txt"))
来源：http://dt.lnxyls.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dw.nszjky.cn

Ruby: File.size("a.txt")
来源：http://kf.bookmarksfly.cn

C#:   new FileInfo("a.txt").Length
来源：http://sv.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://uj.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ik.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uv.shtwfgs.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bh.9csxet.cn

TS:   path.extname("a.txt")
来源：http://ic.shtwfgs.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jx.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://he.nszjky.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zq.muxihuayi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kh.521024.cn

[F11] 复制与移动文件
来源：http://dj.jianghongdianzi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zj.chemitech.net.cn


<!-- 参考信息 -->