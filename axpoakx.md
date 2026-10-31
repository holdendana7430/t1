代发 wailian999

[E02] 重复字符串
来源：http://nv.jctech888.com.cn

Py:   "ab" * 3
来源：http://qt.szsharing.cn

PHP:  str_repeat("ab", 3);
来源：http://mn.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://gg.nszjky.cn

TS:   "ab".repeat(3)
来源：http://rl.lnxyls.cn

Java: "ab".repeat(3)
来源：http://hp.muxihuayi.cn

Go:   strings.Repeat("ab", 3)
来源：http://rw.shxzukj.cn

Ruby: "ab" * 3
来源：http://ow.jianghongdianzi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://tt.nszjky.cn

[E03] 截取子串
来源：http://gy.9csxet.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yp.521024.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ik.bookmarksfly.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pr.haigaiapp.cn

TS:   s.slice(1, 4)
来源：http://il.chemitech.net.cn

Java: s.substring(1, 4)
来源：http://vy.chemitech.net.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qz.bjjhwx.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fr.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://sw.szsharing.cn

[E04] 查找子串位置
来源：http://in.szsharing.cn

Py:   s.find("x");  s.index("x")
来源：http://sw.9csxet.cn

PHP:  strpos($s, "x");
来源：http://pj.nszjky.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ll.huixinmuqiang.cn

TS:   s.indexOf("x")
来源：http://vc.gzmigu.cn

Java: s.indexOf("x")
来源：http://nj.yuntaijiaju.cn

Go:   strings.Index(s, "x")
来源：http://jn.bookmarksfly.cn

Ruby: s.index("x")
来源：http://lq.9csxet.cn

C#:   s.IndexOf("x")
来源：http://kz.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xp.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ck.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://lw.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://tm.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://dy.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://he.lnxyls.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fu.bookmarksfly.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jz.szxytkj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bd.lnxyls.cn

[E06] 替换子串
来源：http://xv.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gw.colortex.cn

PHP:  str_replace("a", "b", $s);
来源：http://ri.huixiangedu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cp.nicolike.cn

TS:   s.replaceAll("a", "b")
来源：http://sq.huixinmuqiang.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ky.huixinmuqiang.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ru.9csxet.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dv.521024.cn

C#:   s.Replace("a", "b")
来源：http://ee.hnjuh.cn

[E07] 按分隔符拆分
来源：http://ui.wgjwhj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lr.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ot.bjjhwx.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://oz.chemitech.net.cn

TS:   s.split(",")
来源：http://hj.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ew.szxytkj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://sx.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://le.huixiangedu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://aq.shxzukj.cn

[E08] 数组按分隔符合并
来源：http://ty.huanxung.cn

Py:   ",".join(items)
来源：http://au.gzmigu.cn

PHP:  implode(",", $items);
来源：http://gd.521024.cn

JS:   items.join(",")
来源：http://ih.yuntaijiaju.cn

TS:   items.join(",")
来源：http://ep.wgjwhj.cn

Java: String.join(",", items)
来源：http://bs.gzmigu.cn

Go:   strings.Join(items, ",")
来源：http://xv.szsharing.cn

Ruby: items.join(",")
来源：http://ve.muxihuayi.cn

C#:   string.Join(",", items)
来源：http://lk.bjjhwx.cn

[E09] 去除所有空白字符
来源：http://cq.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kn.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://px.hnjuh.cn

JS:   s.replace(/\s+/g, "")
来源：http://mz.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://se.yuexingan06.cn

Java: s.replaceAll("\\s+", "")
来源：http://hc.hahajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://as.shtwfgs.cn

Ruby: s.gsub(/\s+/, "")
来源：http://re.chemitech.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xe.bookmarksfly.cn

[E10] 左侧补零 / 定长填充
来源：http://oc.huixiangedu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://op.hahajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ze.szxytkj.cn

JS:   "7".padStart(3, "0")
来源：http://he.9csxet.cn

TS:   "7".padStart(3, "0")
来源：http://ii.muxihuayi.cn

Java: String.format("%03d", 7)
来源：http://xd.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mj.shxzskj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ee.gzmigu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://xs.muxihuayi.cn

[E11] 反转字符串
来源：http://ye.panjiajie.cn

Py:   s[::-1]
来源：http://it.9csxet.cn

PHP:  strrev($s);
来源：http://oi.yuntaijiaju.cn

JS:   [...s].reverse().join("")
来源：http://up.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://ac.chemitech.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ke.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zf.jianghongdianzi.cn

Ruby: s.reverse
来源：http://up.521024.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tj.huanxung.cn

[E12] 统计某字符出现次数
来源：http://dv.bookmarksfly.cn

Py:   s.count("a")
来源：http://wr.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://zp.panjiajie.cn

JS:   s.split("a").length - 1
来源：http://ed.huixiangedu.cn

TS:   s.split("a").length - 1
来源：http://qc.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xg.muxihuayi.cn

Go:   strings.Count(s, "a")
来源：http://bd.bookmarksfly.cn

Ruby: s.count("a")
来源：http://ud.hahajie.cn

C#:   s.Count(c => c == 'a')
来源：http://lb.bjjhwx.cn

[E13] 逐字符遍历
来源：http://nm.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://qx.chemitech.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ex.wgjwhj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fx.asd995.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gb.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ul.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vj.huixinmuqiang.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://oh.gzmigu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://gy.lnxyls.cn

[E14] URL 编码与 Base64
来源：http://dv.shxzukj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jg.shtwfgs.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://od.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fq.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pg.hnjuh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://te.muxihuayi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xf.yuntaijiaju.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://pv.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://no.jianghongdianzi.cn

[E15] HTML 转义 / 反转义
来源：http://wp.huixinmuqiang.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://iy.jctech888.com.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qo.wgjwhj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mi.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ns.jctech888.com.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://jl.nszjky.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jt.521024.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jr.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pz.szxytkj.cn

[E16] 数字千分位
来源：http://vs.nszjky.cn

Py:   f"{1234567:,}"
来源：http://hi.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://ys.nszjky.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dx.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sg.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xs.szsharing.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ya.bjjhwx.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fk.521024.cn

C#:   1234567.ToString("N0")
来源：http://pw.newstarts.cn

[E17] 首字母大写
来源：http://zn.shtwfgs.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xb.colortex.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://df.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cr.muxihuayi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zz.huixiangedu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gs.shtwfgs.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qw.panjiajie.cn

Ruby: s.capitalize
来源：http://xb.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tq.gzmigu.cn

[E18] 模板占位符替换
来源：http://xf.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nz.asd995.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kf.panjiajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wr.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cd.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://if.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kf.chemitech.net.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lq.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bs.szsharing.cn

[E19] 多行文本按行拆分
来源：http://wc.hnjuh.cn

Py:   s.splitlines()
来源：http://tk.shxzskj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qi.szxytkj.cn

JS:   s.split(/\r?\n/)
来源：http://xh.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://ss.chemitech.net.cn

Java: s.lines().toList()
来源：http://lj.hnjuh.cn

Go:   strings.Split(s, "\n")
来源：http://vv.jianghongdianzi.cn

Ruby: s.lines
来源：http://xl.szsharing.cn

C#:   s.Split('\n')
来源：http://nx.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://nv.521024.cn

Py:   if not s:
来源：http://vn.newstarts.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://br.bjjhwx.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nf.panjiajie.cn

TS:   if (s === "") {}
来源：http://xe.yuntaijiaju.cn

Java: if (s.isEmpty()) {}
来源：http://yk.bookmarksfly.cn

Go:   if s == "" {}
来源：http://fb.hahajie.cn

Ruby: if s.empty?
来源：http://ru.shxzskj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kr.szsharing.cn

[E21] 超长截断加省略号
来源：http://hj.asd995.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wq.yuexingan06.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://do.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gb.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oo.shxzskj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ye.hnjuh.cn

Go:   // 按 rune 判断长度后截断
来源：http://ga.szxytkj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ut.gzmigu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yq.yuntaijiaju.cn

[E22] 字节长度与字符长度
来源：http://tx.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ux.huixinmuqiang.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vl.haigaiapp.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://og.bjjhwx.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gv.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rk.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pu.jctech888.com.cn

Ruby: s.bytesize;  s.length
来源：http://mc.gzmigu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ah.huanxung.cn

================================================================================
来源：http://uf.chemitech.net.cn

F. 文件与目录
来源：http://mv.panjiajie.cn

================================================================================
来源：http://mn.szsharing.cn

[F01] 读取整个文件
来源：http://yj.wgjwhj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hv.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://bi.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nd.hahajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://us.shtwfgs.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://za.muxihuayi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xq.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://me.muxihuayi.cn

C#:   File.ReadAllText("a.txt");
来源：http://sm.panjiajie.cn

[F02] 逐行读取文件
来源：http://dr.muxihuayi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lc.wgjwhj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://nf.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bi.nicolike.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yn.huanxung.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://me.yuexingan06.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oa.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://la.nszjky.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qy.szsharing.cn

[F03] 写入文件（覆盖）
来源：http://hd.wgjwhj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tc.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://xo.newstarts.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bc.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ml.521024.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mu.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ae.yuexingan06.cn

Ruby: File.write("a.txt", "hi")
来源：http://pt.gzmigu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://og.szxytkj.cn

[F04] 追加写入文件
来源：http://ab.hnjuh.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bu.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kg.huanxung.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vr.wgjwhj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kj.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mb.hnjuh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xf.wgjwhj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ur.yuexingan06.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iw.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://mh.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jw.hahajie.cn

PHP:  file_exists("a.txt");
来源：http://cb.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://th.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://tn.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gk.huixiangedu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qp.521024.cn

Ruby: File.exist?("a.txt")
来源：http://yq.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://ip.huanxung.cn

[F06] 删除文件
来源：http://ho.nicolike.cn

Py:   os.remove("a.txt")
来源：http://zf.shtwfgs.cn

PHP:  unlink("a.txt");
来源：http://zi.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ak.szxytkj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ej.chemitech.net.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ah.bjjhwx.cn

Go:   os.Remove("a.txt")
来源：http://xu.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://pt.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://te.chemitech.net.cn

[F07] 创建目录（含多级）
来源：http://pp.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nz.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wu.yuexingan06.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yr.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jd.nicolike.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sk.gzmigu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dy.jctech888.com.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vv.yuexingan06.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sl.nszjky.cn

[F08] 遍历目录
来源：http://rr.yuexingan06.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fv.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://by.nszjky.cn

JS:   fs.readdirSync("dir")
来源：http://wi.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://jj.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ow.jctech888.com.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://iv.colortex.cn

Ruby: Dir.children("dir")
来源：http://xg.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://ns.asd995.cn

[F09] 获取文件大小
来源：http://ga.521024.cn

Py:   os.path.getsize("a.txt")
来源：http://it.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://dk.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://pp.huixinmuqiang.cn

TS:   fs.statSync("a.txt").size
来源：http://pf.asd995.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fy.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gl.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://dz.hnjuh.cn

C#:   new FileInfo("a.txt").Length
来源：http://ke.huixiangedu.cn

[F10] 取文件扩展名 / 文件名
来源：http://wi.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tt.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xy.lnxyls.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pj.shxzskj.cn

TS:   path.extname("a.txt")
来源：http://na.haigaiapp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nb.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zl.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zg.szxytkj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://em.shtwfgs.cn

[F11] 复制与移动文件
来源：http://cl.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ff.panjiajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jy.shxzskj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://id.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tt.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vc.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zx.hahajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hj.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qe.shtwfgs.cn

[F12] CSV 读写
来源：http://kh.huixiangedu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xw.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bp.jianghongdianzi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xp.hnjuh.cn

TS:   // 同上
来源：http://bp.huixinmuqiang.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gj.nszjky.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tz.lnxyls.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xp.muxihuayi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wz.wgjwhj.cn


<!-- 参考信息 -->