代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xp.hnjuh.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://dt.newstarts.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dd.hnjuh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xt.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://fx.shxzskj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://dj.newstarts.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ft.hnjuh.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rd.szsharing.cn

[E02] 重复字符串
来源：http://uk.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://ub.nszjky.cn

PHP:  str_repeat("ab", 3);
来源：http://cq.chemitech.net.cn

JS:   "ab".repeat(3)
来源：http://kv.huanxung.cn

TS:   "ab".repeat(3)
来源：http://um.nicolike.cn

Java: "ab".repeat(3)
来源：http://kx.wgjwhj.cn

Go:   strings.Repeat("ab", 3)
来源：http://rb.haigaiapp.cn

Ruby: "ab" * 3
来源：http://uy.hahajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mr.newstarts.cn

[E03] 截取子串
来源：http://cc.nszjky.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yl.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://da.wgjwhj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://po.jianghongdianzi.cn

TS:   s.slice(1, 4)
来源：http://yq.colortex.cn

Java: s.substring(1, 4)
来源：http://ir.9csxet.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yi.jctech888.com.cn

Ruby: s[1, 3];  s[1..3]
来源：http://sf.jianghongdianzi.cn

C#:   s.Substring(1, 3)
来源：http://sr.yuntaijiaju.cn

[E04] 查找子串位置
来源：http://ln.lnxyls.cn

Py:   s.find("x");  s.index("x")
来源：http://jv.hahajie.cn

PHP:  strpos($s, "x");
来源：http://fs.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://nl.szsharing.cn

TS:   s.indexOf("x")
来源：http://iv.huanxung.cn

Java: s.indexOf("x")
来源：http://ek.yuexingan06.cn

Go:   strings.Index(s, "x")
来源：http://wa.shxzskj.cn

Ruby: s.index("x")
来源：http://yv.gzmigu.cn

C#:   s.IndexOf("x")
来源：http://kk.huanxung.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qb.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wr.gzmigu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://of.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ac.haigaiapp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://iz.hahajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wg.lnxyls.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://uy.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qy.haigaiapp.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yc.chemitech.net.cn

[E06] 替换子串
来源：http://pf.lnxyls.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://dm.lnxyls.cn

PHP:  str_replace("a", "b", $s);
来源：http://fl.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yx.shxzukj.cn

TS:   s.replaceAll("a", "b")
来源：http://qq.huixinmuqiang.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ei.asd995.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xb.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://sj.hnjuh.cn

C#:   s.Replace("a", "b")
来源：http://us.hahajie.cn

[E07] 按分隔符拆分
来源：http://rf.bookmarksfly.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kr.panjiajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tu.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://mh.9csxet.cn

TS:   s.split(",")
来源：http://fc.521024.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sm.panjiajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://pi.gzmigu.cn

Ruby: s.split(",");  s.split
来源：http://nl.shtwfgs.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://oo.shxzskj.cn

[E08] 数组按分隔符合并
来源：http://nr.bjjhwx.cn

Py:   ",".join(items)
来源：http://ng.newstarts.cn

PHP:  implode(",", $items);
来源：http://dd.chemitech.net.cn

JS:   items.join(",")
来源：http://ws.lnxyls.cn

TS:   items.join(",")
来源：http://pc.gzmigu.cn

Java: String.join(",", items)
来源：http://ji.jianghongdianzi.cn

Go:   strings.Join(items, ",")
来源：http://wl.haigaiapp.cn

Ruby: items.join(",")
来源：http://ia.szxytkj.cn

C#:   string.Join(",", items)
来源：http://wc.bookmarksfly.cn

[E09] 去除所有空白字符
来源：http://lj.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://lf.haigaiapp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://oh.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://rk.bookmarksfly.cn

TS:   s.replace(/\s+/g, "")
来源：http://gj.jctech888.com.cn

Java: s.replaceAll("\\s+", "")
来源：http://hn.asd995.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ux.colortex.cn

Ruby: s.gsub(/\s+/, "")
来源：http://os.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gf.huixinmuqiang.cn

[E10] 左侧补零 / 定长填充
来源：http://qa.nszjky.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jb.shxzskj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://za.shxzukj.cn

JS:   "7".padStart(3, "0")
来源：http://ns.jctech888.com.cn

TS:   "7".padStart(3, "0")
来源：http://wj.yuntaijiaju.cn

Java: String.format("%03d", 7)
来源：http://vn.bookmarksfly.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ri.wgjwhj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ku.521024.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://tt.wgjwhj.cn

[E11] 反转字符串
来源：http://xj.9csxet.cn

Py:   s[::-1]
来源：http://ue.yuexingan06.cn

PHP:  strrev($s);
来源：http://ky.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://jk.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://xk.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://up.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://re.asd995.cn

Ruby: s.reverse
来源：http://ai.shtwfgs.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qs.shxzskj.cn

[E12] 统计某字符出现次数
来源：http://zm.gzmigu.cn

Py:   s.count("a")
来源：http://gx.panjiajie.cn

PHP:  substr_count($s, "a");
来源：http://qq.gzmigu.cn

JS:   s.split("a").length - 1
来源：http://da.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://yy.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uk.newstarts.cn

Go:   strings.Count(s, "a")
来源：http://oh.newstarts.cn

Ruby: s.count("a")
来源：http://sp.bookmarksfly.cn

C#:   s.Count(c => c == 'a')
来源：http://ov.shxzskj.cn

[E13] 逐字符遍历
来源：http://sh.jctech888.com.cn

Py:   for ch in s: print(ch)
来源：http://jf.huixiangedu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://og.muxihuayi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://mj.nicolike.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vx.asd995.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://be.9csxet.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mn.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://oz.nszjky.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yt.yuexingan06.cn

[E14] URL 编码与 Base64
来源：http://dn.huixiangedu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rr.huixinmuqiang.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://iy.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mw.asd995.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ub.chemitech.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kz.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xf.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kt.9csxet.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bl.shxzskj.cn

[E15] HTML 转义 / 反转义
来源：http://rb.hnjuh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wn.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gy.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uy.szsharing.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ig.lnxyls.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vj.nicolike.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hr.huixiangedu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jh.gzmigu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://us.jianghongdianzi.cn

[E16] 数字千分位
来源：http://wn.panjiajie.cn

Py:   f"{1234567:,}"
来源：http://fm.gzmigu.cn

PHP:  number_format(1234567);
来源：http://gw.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ed.newstarts.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://lz.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xa.jctech888.com.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pr.nszjky.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ar.muxihuayi.cn

C#:   1234567.ToString("N0")
来源：http://mm.jctech888.com.cn

[E17] 首字母大写
来源：http://wr.nicolike.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oe.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bc.shxzskj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yi.gzmigu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ox.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yd.yuntaijiaju.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hd.huixiangedu.cn

Ruby: s.capitalize
来源：http://wr.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wn.chemitech.net.cn

[E18] 模板占位符替换
来源：http://jn.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dr.chemitech.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zo.yuntaijiaju.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rx.lnxyls.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://aq.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://is.yuexingan06.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pe.huixiangedu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://du.jianghongdianzi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://of.nszjky.cn

[E19] 多行文本按行拆分
来源：http://lc.yuntaijiaju.cn

Py:   s.splitlines()
来源：http://fm.521024.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xe.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://kc.wgjwhj.cn

TS:   s.split(/\r?\n/)
来源：http://wj.panjiajie.cn

Java: s.lines().toList()
来源：http://fv.haigaiapp.cn

Go:   strings.Split(s, "\n")
来源：http://fu.jianghongdianzi.cn

Ruby: s.lines
来源：http://lq.szxytkj.cn

C#:   s.Split('\n')
来源：http://im.colortex.cn

[E20] 判断字符串是否为空
来源：http://fz.yuexingan06.cn

Py:   if not s:
来源：http://ep.huanxung.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lm.newstarts.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://rn.haigaiapp.cn

TS:   if (s === "") {}
来源：http://ka.shtwfgs.cn

Java: if (s.isEmpty()) {}
来源：http://zg.colortex.cn

Go:   if s == "" {}
来源：http://oc.asd995.cn

Ruby: if s.empty?
来源：http://gr.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fz.lnxyls.cn

[E21] 超长截断加省略号
来源：http://hi.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://uw.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://iq.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wh.huixiangedu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tg.huixinmuqiang.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://on.yuntaijiaju.cn

Go:   // 按 rune 判断长度后截断
来源：http://mo.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ry.9csxet.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://eq.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://at.panjiajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cq.jctech888.com.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kc.nicolike.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cn.nszjky.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ue.huixinmuqiang.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://et.panjiajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dz.szxytkj.cn

Ruby: s.bytesize;  s.length
来源：http://qb.nicolike.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tv.jianghongdianzi.cn

================================================================================
来源：http://rg.hahajie.cn

F. 文件与目录
来源：http://gp.yuntaijiaju.cn

================================================================================
来源：http://xn.wgjwhj.cn

[F01] 读取整个文件
来源：http://ci.huixinmuqiang.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://go.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://uh.panjiajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ti.hahajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vr.jianghongdianzi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yi.yuntaijiaju.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wl.yuexingan06.cn

Ruby: File.read("a.txt")
来源：http://iy.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://vg.haigaiapp.cn

[F02] 逐行读取文件
来源：http://vi.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ip.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ic.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ky.gzmigu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ah.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://be.shxzukj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jk.shxzskj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://cs.colortex.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tb.hnjuh.cn

[F03] 写入文件（覆盖）
来源：http://ze.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sn.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hr.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zf.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nk.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://so.haigaiapp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cl.bjjhwx.cn

Ruby: File.write("a.txt", "hi")
来源：http://ui.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dk.szxytkj.cn

[F04] 追加写入文件
来源：http://vx.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rb.shtwfgs.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://oo.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cu.nszjky.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oi.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sm.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jy.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wa.yuntaijiaju.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://fh.huixinmuqiang.cn

[F05] 判断文件或目录是否存在
来源：http://pr.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ct.bjjhwx.cn

PHP:  file_exists("a.txt");
来源：http://du.shxzskj.cn

JS:   fs.existsSync("a.txt")
来源：http://mm.shxzskj.cn

TS:   fs.existsSync("a.txt")
来源：http://zv.nszjky.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hk.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ar.521024.cn

Ruby: File.exist?("a.txt")
来源：http://wz.shxzukj.cn

C#:   File.Exists("a.txt")
来源：http://jt.newstarts.cn

[F06] 删除文件
来源：http://mc.asd995.cn

Py:   os.remove("a.txt")
来源：http://vh.521024.cn

PHP:  unlink("a.txt");
来源：http://ac.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xa.jctech888.com.cn

TS:   fs.unlinkSync("a.txt")
来源：http://on.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mh.asd995.cn

Go:   os.Remove("a.txt")
来源：http://zp.colortex.cn

Ruby: File.delete("a.txt")
来源：http://fa.hahajie.cn

C#:   File.Delete("a.txt");
来源：http://qt.hnjuh.cn

[F07] 创建目录（含多级）
来源：http://zw.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rk.yuexingan06.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cp.huixinmuqiang.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kv.lnxyls.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hd.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xa.newstarts.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://my.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mv.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://im.huixinmuqiang.cn

[F08] 遍历目录
来源：http://dk.nszjky.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://kc.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zr.521024.cn

JS:   fs.readdirSync("dir")
来源：http://cl.szsharing.cn

TS:   fs.readdirSync("dir")
来源：http://qq.shxzskj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hp.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vm.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://cr.9csxet.cn

C#:   Directory.GetFiles("dir")
来源：http://qu.hnjuh.cn

[F09] 获取文件大小
来源：http://gd.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://yc.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://ol.huanxung.cn

JS:   fs.statSync("a.txt").size
来源：http://oa.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://yg.shtwfgs.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hm.newstarts.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bu.shxzskj.cn

Ruby: File.size("a.txt")
来源：http://xn.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://ss.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://ql.chemitech.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rh.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bk.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://td.szsharing.cn

TS:   path.extname("a.txt")
来源：http://fx.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ju.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jm.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vc.hnjuh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vd.asd995.cn

[F11] 复制与移动文件
来源：http://ea.nszjky.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://rl.huixiangedu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sl.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kt.jctech888.com.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gw.hahajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://su.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ar.newstarts.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wo.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vx.szxytkj.cn

[F12] CSV 读写
来源：http://yt.bjjhwx.cn


<!-- 参考信息 -->