代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://if.asd995.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dp.bjjhwx.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://px.gzmigu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://on.chemitech.net.cn

[E02] 重复字符串
来源：http://gh.shxzukj.cn

Py:   "ab" * 3
来源：http://ux.jctech888.com.cn

PHP:  str_repeat("ab", 3);
来源：http://ng.colortex.cn

JS:   "ab".repeat(3)
来源：http://cg.jctech888.com.cn

TS:   "ab".repeat(3)
来源：http://fh.lnxyls.cn

Java: "ab".repeat(3)
来源：http://jc.newstarts.cn

Go:   strings.Repeat("ab", 3)
来源：http://an.521024.cn

Ruby: "ab" * 3
来源：http://xc.shtwfgs.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://vx.huanxung.cn

[E03] 截取子串
来源：http://br.yuntaijiaju.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gj.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fu.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ly.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://bb.huixiangedu.cn

Java: s.substring(1, 4)
来源：http://bl.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ca.bookmarksfly.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hs.lnxyls.cn

C#:   s.Substring(1, 3)
来源：http://ny.hnjuh.cn

[E04] 查找子串位置
来源：http://fj.gzmigu.cn

Py:   s.find("x");  s.index("x")
来源：http://kt.panjiajie.cn

PHP:  strpos($s, "x");
来源：http://bf.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hy.wgjwhj.cn

TS:   s.indexOf("x")
来源：http://xv.chemitech.net.cn

Java: s.indexOf("x")
来源：http://hr.yuexingan06.cn

Go:   strings.Index(s, "x")
来源：http://qm.newstarts.cn

Ruby: s.index("x")
来源：http://ua.szxytkj.cn

C#:   s.IndexOf("x")
来源：http://fd.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://tv.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://cn.lnxyls.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xw.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ol.asd995.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://qb.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iu.huanxung.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xi.nicolike.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://iz.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://sc.yuexingan06.cn

[E06] 替换子串
来源：http://sx.chemitech.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ca.colortex.cn

PHP:  str_replace("a", "b", $s);
来源：http://er.colortex.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aj.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://ye.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yp.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bs.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nu.gzmigu.cn

C#:   s.Replace("a", "b")
来源：http://sm.hahajie.cn

[E07] 按分隔符拆分
来源：http://zf.jianghongdianzi.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hf.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gm.asd995.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ey.shxzukj.cn

TS:   s.split(",")
来源：http://qu.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zi.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ug.lnxyls.cn

Ruby: s.split(",");  s.split
来源：http://du.szxytkj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bv.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://rd.bookmarksfly.cn

Py:   ",".join(items)
来源：http://qp.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://ap.muxihuayi.cn

JS:   items.join(",")
来源：http://wd.haigaiapp.cn

TS:   items.join(",")
来源：http://fk.hahajie.cn

Java: String.join(",", items)
来源：http://qb.gzmigu.cn

Go:   strings.Join(items, ",")
来源：http://su.hahajie.cn

Ruby: items.join(",")
来源：http://qr.chemitech.net.cn

C#:   string.Join(",", items)
来源：http://gl.shtwfgs.cn

[E09] 去除所有空白字符
来源：http://qw.chemitech.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ho.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sr.hnjuh.cn

JS:   s.replace(/\s+/g, "")
来源：http://ee.asd995.cn

TS:   s.replace(/\s+/g, "")
来源：http://yx.szxytkj.cn

Java: s.replaceAll("\\s+", "")
来源：http://hf.chemitech.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mz.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ha.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sm.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://uf.colortex.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bs.chemitech.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rh.szxytkj.cn

JS:   "7".padStart(3, "0")
来源：http://cs.newstarts.cn

TS:   "7".padStart(3, "0")
来源：http://ya.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://ld.asd995.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ez.szsharing.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qz.521024.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gi.shxzukj.cn

[E11] 反转字符串
来源：http://qg.jianghongdianzi.cn

Py:   s[::-1]
来源：http://nu.szsharing.cn

PHP:  strrev($s);
来源：http://gl.shtwfgs.cn

JS:   [...s].reverse().join("")
来源：http://kx.yuntaijiaju.cn

TS:   [...s].reverse().join("")
来源：http://kh.newstarts.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://kx.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://au.newstarts.cn

Ruby: s.reverse
来源：http://qu.szxytkj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://py.chemitech.net.cn

[E12] 统计某字符出现次数
来源：http://uw.bjjhwx.cn

Py:   s.count("a")
来源：http://hu.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://nc.shxzukj.cn

JS:   s.split("a").length - 1
来源：http://dx.yuntaijiaju.cn

TS:   s.split("a").length - 1
来源：http://yk.shxzukj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sh.huanxung.cn

Go:   strings.Count(s, "a")
来源：http://bc.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://wy.haigaiapp.cn

C#:   s.Count(c => c == 'a')
来源：http://ya.lnxyls.cn

[E13] 逐字符遍历
来源：http://xl.haigaiapp.cn

Py:   for ch in s: print(ch)
来源：http://ip.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ap.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://he.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vt.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xe.panjiajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vg.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tz.bjjhwx.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sq.nicolike.cn

[E14] URL 编码与 Base64
来源：http://yf.szsharing.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gy.muxihuayi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://mu.shxzukj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://es.hahajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://eq.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xu.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://oi.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://rm.wgjwhj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ub.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://jt.shxzukj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hs.hnjuh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://xj.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rr.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://mq.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xu.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yi.muxihuayi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nk.hnjuh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mx.shxzukj.cn

[E16] 数字千分位
来源：http://tx.9csxet.cn

Py:   f"{1234567:,}"
来源：http://ix.huixiangedu.cn

PHP:  number_format(1234567);
来源：http://hd.shxzskj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ow.shxzskj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://et.wgjwhj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ig.szsharing.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bq.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bh.szsharing.cn

C#:   1234567.ToString("N0")
来源：http://xk.shxzskj.cn

[E17] 首字母大写
来源：http://zt.haigaiapp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ge.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qs.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uv.newstarts.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qo.asd995.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zu.hahajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sb.yuexingan06.cn

Ruby: s.capitalize
来源：http://zr.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cq.jctech888.com.cn

[E18] 模板占位符替换
来源：http://ns.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nw.nicolike.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://av.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://lx.panjiajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qw.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://lh.yuntaijiaju.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://de.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://og.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fj.521024.cn

[E19] 多行文本按行拆分
来源：http://bc.9csxet.cn

Py:   s.splitlines()
来源：http://as.muxihuayi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://st.muxihuayi.cn

JS:   s.split(/\r?\n/)
来源：http://bx.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://pl.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://by.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://tc.szxytkj.cn

Ruby: s.lines
来源：http://cx.haigaiapp.cn

C#:   s.Split('\n')
来源：http://hd.asd995.cn

[E20] 判断字符串是否为空
来源：http://mr.huanxung.cn

Py:   if not s:
来源：http://ra.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oq.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uj.hahajie.cn

TS:   if (s === "") {}
来源：http://ik.shxzskj.cn

Java: if (s.isEmpty()) {}
来源：http://wt.huixiangedu.cn

Go:   if s == "" {}
来源：http://rt.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://em.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gx.asd995.cn

[E21] 超长截断加省略号
来源：http://ew.wgjwhj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mf.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gz.wgjwhj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://td.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jy.asd995.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ie.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://uz.gzmigu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uo.chemitech.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wk.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://bj.newstarts.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dy.huixinmuqiang.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bh.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nj.shtwfgs.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jh.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://do.yuexingan06.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://fa.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://xq.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mu.wgjwhj.cn

================================================================================
来源：http://uk.szxytkj.cn

F. 文件与目录
来源：http://qx.huanxung.cn

================================================================================
来源：http://fb.haigaiapp.cn

[F01] 读取整个文件
来源：http://gf.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xz.huixinmuqiang.cn

PHP:  file_get_contents("a.txt");
来源：http://pm.chemitech.net.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vd.panjiajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vh.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kq.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wv.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://fb.yuntaijiaju.cn

C#:   File.ReadAllText("a.txt");
来源：http://tx.newstarts.cn

[F02] 逐行读取文件
来源：http://kb.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fp.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ui.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qv.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gf.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xl.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lq.haigaiapp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://od.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ze.colortex.cn

[F03] 写入文件（覆盖）
来源：http://fp.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ra.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://he.szxytkj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ld.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://un.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ro.gzmigu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://le.panjiajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://ug.yuntaijiaju.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uk.shtwfgs.cn

[F04] 追加写入文件
来源：http://gi.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hd.huanxung.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cn.jctech888.com.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fp.shtwfgs.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://st.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://we.wgjwhj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oi.newstarts.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pq.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xk.asd995.cn

[F05] 判断文件或目录是否存在
来源：http://ce.gzmigu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://me.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://qt.jctech888.com.cn

JS:   fs.existsSync("a.txt")
来源：http://dt.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://ra.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hs.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hm.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://yb.szxytkj.cn

C#:   File.Exists("a.txt")
来源：http://jg.szxytkj.cn

[F06] 删除文件
来源：http://mc.colortex.cn

Py:   os.remove("a.txt")
来源：http://mx.wgjwhj.cn

PHP:  unlink("a.txt");
来源：http://ws.shtwfgs.cn

JS:   fs.unlinkSync("a.txt")
来源：http://eh.9csxet.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wa.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ud.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://ge.wgjwhj.cn

Ruby: File.delete("a.txt")
来源：http://id.huixinmuqiang.cn

C#:   File.Delete("a.txt");
来源：http://fp.hahajie.cn

[F07] 创建目录（含多级）
来源：http://qd.haigaiapp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dq.9csxet.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fx.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ei.shxzukj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gs.nicolike.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ec.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gj.jctech888.com.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nj.bookmarksfly.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fb.jctech888.com.cn

[F08] 遍历目录
来源：http://hh.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cw.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jb.yuexingan06.cn

JS:   fs.readdirSync("dir")
来源：http://in.yuntaijiaju.cn

TS:   fs.readdirSync("dir")
来源：http://oz.haigaiapp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mm.newstarts.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wz.asd995.cn

Ruby: Dir.children("dir")
来源：http://wb.nszjky.cn

C#:   Directory.GetFiles("dir")
来源：http://hz.hnjuh.cn

[F09] 获取文件大小
来源：http://ih.muxihuayi.cn

Py:   os.path.getsize("a.txt")
来源：http://av.lnxyls.cn

PHP:  filesize("a.txt");
来源：http://fq.shxzskj.cn

JS:   fs.statSync("a.txt").size
来源：http://iz.huixinmuqiang.cn

TS:   fs.statSync("a.txt").size
来源：http://no.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://il.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qc.jctech888.com.cn

Ruby: File.size("a.txt")
来源：http://kq.newstarts.cn

C#:   new FileInfo("a.txt").Length
来源：http://zf.huanxung.cn

[F10] 取文件扩展名 / 文件名
来源：http://cb.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qh.shtwfgs.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://de.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mk.9csxet.cn

TS:   path.extname("a.txt")
来源：http://mh.yuntaijiaju.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qi.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ey.jctech888.com.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zl.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://es.nszjky.cn

[F11] 复制与移动文件
来源：http://py.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pi.wgjwhj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://va.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vh.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://td.colortex.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xs.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jw.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bx.muxihuayi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zd.yuntaijiaju.cn

[F12] CSV 读写
来源：http://wg.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nr.yuexingan06.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ao.jianghongdianzi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qe.shxzskj.cn

TS:   // 同上
来源：http://cw.jianghongdianzi.cn


<!-- 参考信息 -->