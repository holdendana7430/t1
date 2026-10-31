代发 wailian999

================================================================================
来源：http://cx.huanxung.cn

E. 字符串处理
来源：http://bj.bookmarksfly.cn

================================================================================
来源：http://zq.shtwfgs.cn

[E01] 拼接字符串
来源：http://ok.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://nq.huixinmuqiang.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qa.muxihuayi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qv.9csxet.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://eg.szsharing.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://sa.gzmigu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ee.jianghongdianzi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ii.colortex.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://tn.wgjwhj.cn

[E02] 重复字符串
来源：http://me.nszjky.cn

Py:   "ab" * 3
来源：http://js.jianghongdianzi.cn

PHP:  str_repeat("ab", 3);
来源：http://qb.hahajie.cn

JS:   "ab".repeat(3)
来源：http://sd.bjjhwx.cn

TS:   "ab".repeat(3)
来源：http://ie.gzmigu.cn

Java: "ab".repeat(3)
来源：http://jx.shtwfgs.cn

Go:   strings.Repeat("ab", 3)
来源：http://cp.huixiangedu.cn

Ruby: "ab" * 3
来源：http://ua.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ld.panjiajie.cn

[E03] 截取子串
来源：http://uo.szsharing.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bz.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fi.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wt.bookmarksfly.cn

TS:   s.slice(1, 4)
来源：http://fm.gzmigu.cn

Java: s.substring(1, 4)
来源：http://dx.asd995.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qe.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ku.521024.cn

C#:   s.Substring(1, 3)
来源：http://dx.bookmarksfly.cn

[E04] 查找子串位置
来源：http://tf.lnxyls.cn

Py:   s.find("x");  s.index("x")
来源：http://mn.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://ks.panjiajie.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ac.yuexingan06.cn

TS:   s.indexOf("x")
来源：http://qe.wgjwhj.cn

Java: s.indexOf("x")
来源：http://yl.muxihuayi.cn

Go:   strings.Index(s, "x")
来源：http://mo.asd995.cn

Ruby: s.index("x")
来源：http://pn.yuntaijiaju.cn

C#:   s.IndexOf("x")
来源：http://qx.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qx.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://qo.wgjwhj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://eg.huixiangedu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jl.9csxet.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pb.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xy.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uc.bjjhwx.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hh.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tz.jctech888.com.cn

[E06] 替换子串
来源：http://sm.9csxet.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yw.szsharing.cn

PHP:  str_replace("a", "b", $s);
来源：http://tj.gzmigu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ff.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://qd.asd995.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oa.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gg.huanxung.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cx.shxzskj.cn

C#:   s.Replace("a", "b")
来源：http://mp.muxihuayi.cn

[E07] 按分隔符拆分
来源：http://tc.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://iw.huanxung.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ll.wgjwhj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://uq.yuntaijiaju.cn

TS:   s.split(",")
来源：http://al.yuntaijiaju.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dz.9csxet.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ve.shtwfgs.cn

Ruby: s.split(",");  s.split
来源：http://tw.9csxet.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://xx.chemitech.net.cn

[E08] 数组按分隔符合并
来源：http://sv.jctech888.com.cn

Py:   ",".join(items)
来源：http://rn.huanxung.cn

PHP:  implode(",", $items);
来源：http://yy.bookmarksfly.cn

JS:   items.join(",")
来源：http://sd.nszjky.cn

TS:   items.join(",")
来源：http://cr.shxzukj.cn

Java: String.join(",", items)
来源：http://gr.colortex.cn

Go:   strings.Join(items, ",")
来源：http://ox.muxihuayi.cn

Ruby: items.join(",")
来源：http://zj.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://dy.yuexingan06.cn

[E09] 去除所有空白字符
来源：http://ic.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nx.muxihuayi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zr.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://hh.jctech888.com.cn

TS:   s.replace(/\s+/g, "")
来源：http://bk.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://xu.chemitech.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ia.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jm.panjiajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jj.hnjuh.cn

[E10] 左侧补零 / 定长填充
来源：http://gp.jianghongdianzi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xz.nszjky.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xr.chemitech.net.cn

JS:   "7".padStart(3, "0")
来源：http://ys.bjjhwx.cn

TS:   "7".padStart(3, "0")
来源：http://nw.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://py.huanxung.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://iy.huixiangedu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mv.9csxet.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rn.yuexingan06.cn

[E11] 反转字符串
来源：http://dd.huixinmuqiang.cn

Py:   s[::-1]
来源：http://jz.bjjhwx.cn

PHP:  strrev($s);
来源：http://rk.asd995.cn

JS:   [...s].reverse().join("")
来源：http://bf.asd995.cn

TS:   [...s].reverse().join("")
来源：http://yd.newstarts.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lz.nszjky.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ae.nicolike.cn

Ruby: s.reverse
来源：http://cz.muxihuayi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nm.newstarts.cn

[E12] 统计某字符出现次数
来源：http://un.hnjuh.cn

Py:   s.count("a")
来源：http://qt.colortex.cn

PHP:  substr_count($s, "a");
来源：http://dx.huanxung.cn

JS:   s.split("a").length - 1
来源：http://qo.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://jx.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://za.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://cp.huixiangedu.cn

Ruby: s.count("a")
来源：http://sj.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://tv.521024.cn

[E13] 逐字符遍历
来源：http://vz.nszjky.cn

Py:   for ch in s: print(ch)
来源：http://yx.shxzskj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://db.asd995.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gw.shxzukj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://tf.gzmigu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pz.haigaiapp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nx.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xu.jctech888.com.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://em.szsharing.cn

[E14] URL 编码与 Base64
来源：http://jy.9csxet.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mr.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://gw.hnjuh.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lp.shxzukj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qf.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://om.panjiajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ag.yuexingan06.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://no.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rw.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://vv.yuntaijiaju.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ep.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ps.yuntaijiaju.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tr.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://op.szsharing.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ju.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hf.jianghongdianzi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wm.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://gk.shxzskj.cn

[E16] 数字千分位
来源：http://hu.huanxung.cn

Py:   f"{1234567:,}"
来源：http://rr.colortex.cn

PHP:  number_format(1234567);
来源：http://oz.bookmarksfly.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vf.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://le.nicolike.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jl.jianghongdianzi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://so.lnxyls.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://nd.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://sb.bookmarksfly.cn

[E17] 首字母大写
来源：http://rh.521024.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://eb.asd995.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://db.shtwfgs.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vn.jctech888.com.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oy.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://lr.newstarts.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://cl.szxytkj.cn

Ruby: s.capitalize
来源：http://ds.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vg.muxihuayi.cn

[E18] 模板占位符替换
来源：http://ak.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ds.hahajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xs.9csxet.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xi.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xx.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rq.yuexingan06.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://qw.chemitech.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ka.muxihuayi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xq.nszjky.cn

[E19] 多行文本按行拆分
来源：http://zp.lnxyls.cn

Py:   s.splitlines()
来源：http://ec.shxzukj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tu.yuntaijiaju.cn

JS:   s.split(/\r?\n/)
来源：http://ah.hnjuh.cn

TS:   s.split(/\r?\n/)
来源：http://gt.521024.cn

Java: s.lines().toList()
来源：http://ex.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://ty.lnxyls.cn

Ruby: s.lines
来源：http://ba.jctech888.com.cn

C#:   s.Split('\n')
来源：http://yk.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://qu.szsharing.cn

Py:   if not s:
来源：http://pu.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rw.szsharing.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://va.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://vz.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://cs.521024.cn

Go:   if s == "" {}
来源：http://nm.nszjky.cn

Ruby: if s.empty?
来源：http://pt.gzmigu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tj.yuntaijiaju.cn

[E21] 超长截断加省略号
来源：http://rs.yuexingan06.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dx.huixinmuqiang.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mr.hahajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zg.panjiajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yh.newstarts.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fs.colortex.cn

Go:   // 按 rune 判断长度后截断
来源：http://wz.521024.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ss.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sx.huanxung.cn

[E22] 字节长度与字符长度
来源：http://qz.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rt.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oy.hnjuh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ug.szxytkj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jx.haigaiapp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mr.bookmarksfly.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gi.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://zy.521024.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qo.521024.cn

================================================================================
来源：http://ca.panjiajie.cn

F. 文件与目录
来源：http://xz.nszjky.cn

================================================================================
来源：http://xw.asd995.cn

[F01] 读取整个文件
来源：http://gu.shxzskj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rn.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://bc.nszjky.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://tx.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fx.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kb.nicolike.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tq.huixinmuqiang.cn

Ruby: File.read("a.txt")
来源：http://qo.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://wo.newstarts.cn

[F02] 逐行读取文件
来源：http://bg.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wk.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ks.nicolike.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vt.nicolike.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ba.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pu.nszjky.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lr.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ra.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://aj.huixinmuqiang.cn

[F03] 写入文件（覆盖）
来源：http://xp.bookmarksfly.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mi.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://po.wgjwhj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ds.szxytkj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://av.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gm.nszjky.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rg.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://ow.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sd.muxihuayi.cn

[F04] 追加写入文件
来源：http://dc.bookmarksfly.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://se.shtwfgs.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ej.jctech888.com.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aj.jianghongdianzi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nv.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hy.huanxung.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ug.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dx.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xj.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://em.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dr.hnjuh.cn

PHP:  file_exists("a.txt");
来源：http://jb.yuexingan06.cn

JS:   fs.existsSync("a.txt")
来源：http://us.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://pe.yuexingan06.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wk.colortex.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cr.lnxyls.cn

Ruby: File.exist?("a.txt")
来源：http://jj.yuntaijiaju.cn

C#:   File.Exists("a.txt")
来源：http://id.hahajie.cn

[F06] 删除文件
来源：http://zg.lnxyls.cn

Py:   os.remove("a.txt")
来源：http://lc.szxytkj.cn

PHP:  unlink("a.txt");
来源：http://ef.gzmigu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bo.yuexingan06.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ud.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vl.shxzskj.cn

Go:   os.Remove("a.txt")
来源：http://ku.wgjwhj.cn

Ruby: File.delete("a.txt")
来源：http://ff.yuexingan06.cn

C#:   File.Delete("a.txt");
来源：http://bm.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://ja.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hk.hnjuh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pf.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zx.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rp.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dk.yuexingan06.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ao.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nh.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://eu.nszjky.cn

[F08] 遍历目录
来源：http://ta.9csxet.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yn.bookmarksfly.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cx.newstarts.cn

JS:   fs.readdirSync("dir")
来源：http://so.huixiangedu.cn

TS:   fs.readdirSync("dir")
来源：http://gy.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ek.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ml.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://df.nszjky.cn

C#:   Directory.GetFiles("dir")
来源：http://bo.panjiajie.cn

[F09] 获取文件大小
来源：http://qw.lnxyls.cn

Py:   os.path.getsize("a.txt")
来源：http://zn.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://ls.bjjhwx.cn

JS:   fs.statSync("a.txt").size
来源：http://bt.shxzskj.cn

TS:   fs.statSync("a.txt").size
来源：http://eg.shtwfgs.cn

Java: Files.size(Path.of("a.txt"))
来源：http://df.lnxyls.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://td.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://uu.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://wn.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://lo.lnxyls.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ly.nszjky.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sg.jctech888.com.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://dn.lnxyls.cn

TS:   path.extname("a.txt")
来源：http://iz.hnjuh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hl.hnjuh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yg.gzmigu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ve.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://st.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://uy.lnxyls.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gn.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vx.nszjky.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zi.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fn.chemitech.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://zu.bookmarksfly.cn


<!-- 参考信息 -->