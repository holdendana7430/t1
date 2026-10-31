代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cv.jianghongdianzi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fq.hnjuh.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ig.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wg.haigaiapp.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zi.shtwfgs.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://su.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ax.haigaiapp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://km.newstarts.cn

[E02] 重复字符串
来源：http://yx.shxzskj.cn

Py:   "ab" * 3
来源：http://va.yuntaijiaju.cn

PHP:  str_repeat("ab", 3);
来源：http://cx.521024.cn

JS:   "ab".repeat(3)
来源：http://yp.colortex.cn

TS:   "ab".repeat(3)
来源：http://sx.shtwfgs.cn

Java: "ab".repeat(3)
来源：http://jg.szsharing.cn

Go:   strings.Repeat("ab", 3)
来源：http://vd.shxzskj.cn

Ruby: "ab" * 3
来源：http://hi.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qw.haigaiapp.cn

[E03] 截取子串
来源：http://nh.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hk.bjjhwx.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://id.hnjuh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://iy.gzmigu.cn

TS:   s.slice(1, 4)
来源：http://uh.panjiajie.cn

Java: s.substring(1, 4)
来源：http://lt.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fx.yuexingan06.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zc.huanxung.cn

C#:   s.Substring(1, 3)
来源：http://wd.jctech888.com.cn

[E04] 查找子串位置
来源：http://du.hahajie.cn

Py:   s.find("x");  s.index("x")
来源：http://tf.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://kk.chemitech.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fk.wgjwhj.cn

TS:   s.indexOf("x")
来源：http://wl.nszjky.cn

Java: s.indexOf("x")
来源：http://yh.yuexingan06.cn

Go:   strings.Index(s, "x")
来源：http://nq.lnxyls.cn

Ruby: s.index("x")
来源：http://vh.jctech888.com.cn

C#:   s.IndexOf("x")
来源：http://qa.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zx.szsharing.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://et.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mh.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kd.huanxung.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ei.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hr.bjjhwx.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ty.haigaiapp.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sq.haigaiapp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mc.chemitech.net.cn

[E06] 替换子串
来源：http://ud.521024.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://of.shtwfgs.cn

PHP:  str_replace("a", "b", $s);
来源：http://sa.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vo.jctech888.com.cn

TS:   s.replaceAll("a", "b")
来源：http://im.panjiajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lz.chemitech.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ao.hnjuh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wr.szsharing.cn

C#:   s.Replace("a", "b")
来源：http://hr.newstarts.cn

[E07] 按分隔符拆分
来源：http://bc.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ti.9csxet.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vj.9csxet.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://uz.yuexingan06.cn

TS:   s.split(",")
来源：http://li.bookmarksfly.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ap.chemitech.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://li.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://at.yuexingan06.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jx.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://oz.szsharing.cn

Py:   ",".join(items)
来源：http://pu.shxzukj.cn

PHP:  implode(",", $items);
来源：http://xo.nszjky.cn

JS:   items.join(",")
来源：http://fj.nszjky.cn

TS:   items.join(",")
来源：http://lb.szxytkj.cn

Java: String.join(",", items)
来源：http://mh.shtwfgs.cn

Go:   strings.Join(items, ",")
来源：http://ui.shxzskj.cn

Ruby: items.join(",")
来源：http://ok.hnjuh.cn

C#:   string.Join(",", items)
来源：http://xs.shtwfgs.cn

[E09] 去除所有空白字符
来源：http://zw.lnxyls.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://qk.nicolike.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lk.hnjuh.cn

JS:   s.replace(/\s+/g, "")
来源：http://an.bookmarksfly.cn

TS:   s.replace(/\s+/g, "")
来源：http://mf.nszjky.cn

Java: s.replaceAll("\\s+", "")
来源：http://pj.muxihuayi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qu.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ub.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wn.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://uq.huanxung.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zt.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oj.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://vn.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://ed.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://vl.shtwfgs.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gw.bjjhwx.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://at.shxzukj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rm.shtwfgs.cn

[E11] 反转字符串
来源：http://fo.hahajie.cn

Py:   s[::-1]
来源：http://ir.jctech888.com.cn

PHP:  strrev($s);
来源：http://lo.9csxet.cn

JS:   [...s].reverse().join("")
来源：http://dc.521024.cn

TS:   [...s].reverse().join("")
来源：http://mn.shxzskj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://la.yuexingan06.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mf.szxytkj.cn

Ruby: s.reverse
来源：http://gp.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kk.szsharing.cn

[E12] 统计某字符出现次数
来源：http://cu.shxzukj.cn

Py:   s.count("a")
来源：http://yo.gzmigu.cn

PHP:  substr_count($s, "a");
来源：http://kg.huixiangedu.cn

JS:   s.split("a").length - 1
来源：http://zr.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://ay.huanxung.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jm.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://tb.yuntaijiaju.cn

Ruby: s.count("a")
来源：http://pb.gzmigu.cn

C#:   s.Count(c => c == 'a')
来源：http://id.szsharing.cn

[E13] 逐字符遍历
来源：http://bd.shxzskj.cn

Py:   for ch in s: print(ch)
来源：http://yu.colortex.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://st.panjiajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yn.huixinmuqiang.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://zt.panjiajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xl.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fy.lnxyls.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ht.szxytkj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://eh.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://uc.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://kg.szxytkj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jr.shxzskj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://lj.huixiangedu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xv.shxzskj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ar.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tw.yuexingan06.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wj.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tb.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://il.lnxyls.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://cn.yuntaijiaju.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ku.shxzukj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pi.bjjhwx.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ja.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xl.shxzskj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://on.huixiangedu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://et.haigaiapp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vv.muxihuayi.cn

[E16] 数字千分位
来源：http://ci.wgjwhj.cn

Py:   f"{1234567:,}"
来源：http://bo.lnxyls.cn

PHP:  number_format(1234567);
来源：http://bh.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://eq.hahajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ir.hnjuh.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ef.lnxyls.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bm.hnjuh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bk.asd995.cn

C#:   1234567.ToString("N0")
来源：http://uk.chemitech.net.cn

[E17] 首字母大写
来源：http://hx.lnxyls.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://is.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xq.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zs.huanxung.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lx.bjjhwx.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ri.hahajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rp.yuexingan06.cn

Ruby: s.capitalize
来源：http://hz.szsharing.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ex.newstarts.cn

[E18] 模板占位符替换
来源：http://dp.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cu.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://aa.lnxyls.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zh.hnjuh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fb.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cd.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://av.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gh.asd995.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ye.muxihuayi.cn

[E19] 多行文本按行拆分
来源：http://ky.jianghongdianzi.cn

Py:   s.splitlines()
来源：http://mc.newstarts.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://eq.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://ge.shxzukj.cn

TS:   s.split(/\r?\n/)
来源：http://wb.haigaiapp.cn

Java: s.lines().toList()
来源：http://dp.haigaiapp.cn

Go:   strings.Split(s, "\n")
来源：http://cs.szxytkj.cn

Ruby: s.lines
来源：http://ys.huanxung.cn

C#:   s.Split('\n')
来源：http://oh.bjjhwx.cn

[E20] 判断字符串是否为空
来源：http://ub.shxzskj.cn

Py:   if not s:
来源：http://ns.lnxyls.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nx.shxzskj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mu.jianghongdianzi.cn

TS:   if (s === "") {}
来源：http://sx.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://tz.9csxet.cn

Go:   if s == "" {}
来源：http://mo.bjjhwx.cn

Ruby: if s.empty?
来源：http://kz.lnxyls.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://bh.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://hg.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vh.nszjky.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://la.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fw.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://av.bjjhwx.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pf.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://xs.huanxung.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ru.hnjuh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rn.nszjky.cn

[E22] 字节长度与字符长度
来源：http://pi.jctech888.com.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mu.szxytkj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lp.huixiangedu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xq.gzmigu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ye.huixinmuqiang.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zm.hnjuh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ww.panjiajie.cn

Ruby: s.bytesize;  s.length
来源：http://jv.huixiangedu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://un.jctech888.com.cn

================================================================================
来源：http://to.gzmigu.cn

F. 文件与目录
来源：http://ar.bookmarksfly.cn

================================================================================
来源：http://ie.521024.cn

[F01] 读取整个文件
来源：http://ju.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jo.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://ns.panjiajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jn.nszjky.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fa.haigaiapp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lu.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bv.huixiangedu.cn

Ruby: File.read("a.txt")
来源：http://cw.jianghongdianzi.cn

C#:   File.ReadAllText("a.txt");
来源：http://vu.9csxet.cn

[F02] 逐行读取文件
来源：http://oo.jianghongdianzi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xf.521024.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sz.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oh.chemitech.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ds.lnxyls.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ga.yuexingan06.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xp.bjjhwx.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xk.shtwfgs.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gp.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://ql.wgjwhj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bx.shtwfgs.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ct.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sb.szsharing.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nw.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vz.szsharing.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cc.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://qs.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dl.huanxung.cn

[F04] 追加写入文件
来源：http://aj.haigaiapp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gd.nicolike.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://af.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jh.gzmigu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ln.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cx.shtwfgs.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ff.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tk.bjjhwx.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://oe.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://bf.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qn.nszjky.cn

PHP:  file_exists("a.txt");
来源：http://he.colortex.cn

JS:   fs.existsSync("a.txt")
来源：http://ib.9csxet.cn

TS:   fs.existsSync("a.txt")
来源：http://zw.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://mm.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zo.jctech888.com.cn

Ruby: File.exist?("a.txt")
来源：http://hv.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://wv.chemitech.net.cn

[F06] 删除文件
来源：http://hz.chemitech.net.cn

Py:   os.remove("a.txt")
来源：http://yr.521024.cn

PHP:  unlink("a.txt");
来源：http://cc.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zx.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ew.yuntaijiaju.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qe.shxzukj.cn

Go:   os.Remove("a.txt")
来源：http://lv.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://st.szsharing.cn

C#:   File.Delete("a.txt");
来源：http://uv.wgjwhj.cn

[F07] 创建目录（含多级）
来源：http://wg.yuexingan06.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zw.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tj.wgjwhj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zq.haigaiapp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ux.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ma.shtwfgs.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mn.colortex.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sg.shxzskj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fe.huixiangedu.cn

[F08] 遍历目录
来源：http://ar.huixinmuqiang.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gl.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wj.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://qk.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://lb.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://up.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://tg.yuexingan06.cn

Ruby: Dir.children("dir")
来源：http://ar.wgjwhj.cn

C#:   Directory.GetFiles("dir")
来源：http://jr.muxihuayi.cn

[F09] 获取文件大小
来源：http://pc.huixinmuqiang.cn

Py:   os.path.getsize("a.txt")
来源：http://nb.szsharing.cn

PHP:  filesize("a.txt");
来源：http://ty.haigaiapp.cn

JS:   fs.statSync("a.txt").size
来源：http://qc.shxzukj.cn

TS:   fs.statSync("a.txt").size
来源：http://ko.colortex.cn

Java: Files.size(Path.of("a.txt"))
来源：http://eu.haigaiapp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qy.muxihuayi.cn

Ruby: File.size("a.txt")
来源：http://ww.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://qg.szsharing.cn

[F10] 取文件扩展名 / 文件名
来源：http://ku.colortex.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ly.asd995.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vy.chemitech.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://iz.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://xt.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fy.bookmarksfly.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dh.nszjky.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zu.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://za.jctech888.com.cn

[F11] 复制与移动文件
来源：http://im.huanxung.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nh.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://av.jianghongdianzi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oq.muxihuayi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://po.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rw.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tw.wgjwhj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cb.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bo.wgjwhj.cn

[F12] CSV 读写
来源：http://td.yuntaijiaju.cn


<!-- 参考信息 -->