代发 wailian999

TS:   "ab".repeat(3)
来源：http://qt.szxytkj.cn

Java: "ab".repeat(3)
来源：http://eq.szxytkj.cn

Go:   strings.Repeat("ab", 3)
来源：http://pn.gzmigu.cn

Ruby: "ab" * 3
来源：http://jw.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://zx.gzmigu.cn

[E03] 截取子串
来源：http://na.521024.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://to.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://aa.jianghongdianzi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://uw.bookmarksfly.cn

TS:   s.slice(1, 4)
来源：http://qi.colortex.cn

Java: s.substring(1, 4)
来源：http://tv.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://jv.jctech888.com.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pj.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://hy.hnjuh.cn

[E04] 查找子串位置
来源：http://fc.huixinmuqiang.cn

Py:   s.find("x");  s.index("x")
来源：http://zn.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://dw.yuexingan06.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ms.shxzukj.cn

TS:   s.indexOf("x")
来源：http://yd.hahajie.cn

Java: s.indexOf("x")
来源：http://md.huixiangedu.cn

Go:   strings.Index(s, "x")
来源：http://vz.9csxet.cn

Ruby: s.index("x")
来源：http://dk.wgjwhj.cn

C#:   s.IndexOf("x")
来源：http://vj.hahajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fe.hnjuh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ub.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ri.huixiangedu.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uv.yuexingan06.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://se.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ng.shxzukj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jo.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://yb.shtwfgs.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bv.nicolike.cn

[E06] 替换子串
来源：http://pf.shxzukj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://de.muxihuayi.cn

PHP:  str_replace("a", "b", $s);
来源：http://er.9csxet.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mc.colortex.cn

TS:   s.replaceAll("a", "b")
来源：http://sa.hnjuh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://bx.jctech888.com.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bb.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ut.shxzskj.cn

C#:   s.Replace("a", "b")
来源：http://ji.lnxyls.cn

[E07] 按分隔符拆分
来源：http://wd.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cx.huixiangedu.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ht.9csxet.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nj.huanxung.cn

TS:   s.split(",")
来源：http://mq.shtwfgs.cn

Java: s.split(",");  s.split("\\s+")
来源：http://uj.yuntaijiaju.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://xi.colortex.cn

Ruby: s.split(",");  s.split
来源：http://fz.huixinmuqiang.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ob.hahajie.cn

[E08] 数组按分隔符合并
来源：http://jg.shxzskj.cn

Py:   ",".join(items)
来源：http://nr.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://ob.colortex.cn

JS:   items.join(",")
来源：http://mj.wgjwhj.cn

TS:   items.join(",")
来源：http://re.9csxet.cn

Java: String.join(",", items)
来源：http://xt.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://ge.nszjky.cn

Ruby: items.join(",")
来源：http://tc.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://lk.szxytkj.cn

[E09] 去除所有空白字符
来源：http://bw.muxihuayi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dg.nicolike.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wa.newstarts.cn

JS:   s.replace(/\s+/g, "")
来源：http://mm.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://ue.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://mq.yuexingan06.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cn.9csxet.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wd.gzmigu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jf.panjiajie.cn

[E10] 左侧补零 / 定长填充
来源：http://sd.521024.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://go.jctech888.com.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ly.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://fm.colortex.cn

TS:   "7".padStart(3, "0")
来源：http://cf.nicolike.cn

Java: String.format("%03d", 7)
来源：http://tj.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://dl.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ye.nicolike.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ow.shxzukj.cn

[E11] 反转字符串
来源：http://ve.gzmigu.cn

Py:   s[::-1]
来源：http://du.hahajie.cn

PHP:  strrev($s);
来源：http://xo.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://ql.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://fa.521024.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sk.newstarts.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qu.nszjky.cn

Ruby: s.reverse
来源：http://ix.521024.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hh.panjiajie.cn

[E12] 统计某字符出现次数
来源：http://uk.huanxung.cn

Py:   s.count("a")
来源：http://km.muxihuayi.cn

PHP:  substr_count($s, "a");
来源：http://gl.521024.cn

JS:   s.split("a").length - 1
来源：http://pj.asd995.cn

TS:   s.split("a").length - 1
来源：http://zd.gzmigu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kh.jianghongdianzi.cn

Go:   strings.Count(s, "a")
来源：http://rm.lnxyls.cn

Ruby: s.count("a")
来源：http://cv.jianghongdianzi.cn

C#:   s.Count(c => c == 'a')
来源：http://zr.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://xo.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://oo.asd995.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fa.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ai.yuntaijiaju.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bd.nszjky.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mb.shxzukj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bn.panjiajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://vy.muxihuayi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ah.yuntaijiaju.cn

[E14] URL 编码与 Base64
来源：http://pi.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://go.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cf.huanxung.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://uz.newstarts.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://at.gzmigu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ly.chemitech.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://km.gzmigu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qc.521024.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ch.hahajie.cn

[E15] HTML 转义 / 反转义
来源：http://qc.huixiangedu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hj.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bz.panjiajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dx.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wt.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wn.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yu.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pw.hahajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sa.szxytkj.cn

[E16] 数字千分位
来源：http://ca.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://oa.colortex.cn

PHP:  number_format(1234567);
来源：http://tc.huanxung.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ik.shtwfgs.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nz.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://io.panjiajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nh.huanxung.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://eu.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://jj.nicolike.cn

[E17] 首字母大写
来源：http://tg.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://md.huixinmuqiang.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ds.huixinmuqiang.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ku.asd995.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sp.shxzskj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vt.gzmigu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mj.shxzukj.cn

Ruby: s.capitalize
来源：http://nh.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qx.newstarts.cn

[E18] 模板占位符替换
来源：http://nk.bjjhwx.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ij.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pn.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kw.huanxung.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://oo.szxytkj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://de.yuntaijiaju.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zn.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wc.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rl.huanxung.cn

[E19] 多行文本按行拆分
来源：http://dn.hahajie.cn

Py:   s.splitlines()
来源：http://hm.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oa.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://sw.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://ra.panjiajie.cn

Java: s.lines().toList()
来源：http://cs.huixinmuqiang.cn

Go:   strings.Split(s, "\n")
来源：http://cx.panjiajie.cn

Ruby: s.lines
来源：http://nw.jianghongdianzi.cn

C#:   s.Split('\n')
来源：http://mz.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://mj.wgjwhj.cn

Py:   if not s:
来源：http://lc.huanxung.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rl.huixinmuqiang.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lg.shtwfgs.cn

TS:   if (s === "") {}
来源：http://od.huixinmuqiang.cn

Java: if (s.isEmpty()) {}
来源：http://vo.wgjwhj.cn

Go:   if s == "" {}
来源：http://vn.szsharing.cn

Ruby: if s.empty?
来源：http://xq.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://us.shxzskj.cn

[E21] 超长截断加省略号
来源：http://bv.szsharing.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ry.bjjhwx.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wy.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iy.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qr.asd995.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://sb.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://dc.jianghongdianzi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kt.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ew.asd995.cn

[E22] 字节长度与字符长度
来源：http://hd.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bc.gzmigu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://oi.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ma.panjiajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fe.bookmarksfly.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kc.huanxung.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kt.yuntaijiaju.cn

Ruby: s.bytesize;  s.length
来源：http://sn.yuntaijiaju.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://km.lnxyls.cn

================================================================================
来源：http://vn.bjjhwx.cn

F. 文件与目录
来源：http://ub.szxytkj.cn

================================================================================
来源：http://na.gzmigu.cn

[F01] 读取整个文件
来源：http://ih.huixinmuqiang.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xj.chemitech.net.cn

PHP:  file_get_contents("a.txt");
来源：http://iw.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jx.hahajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://og.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fw.jianghongdianzi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mu.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://au.asd995.cn

C#:   File.ReadAllText("a.txt");
来源：http://zz.asd995.cn

[F02] 逐行读取文件
来源：http://if.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pe.colortex.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vr.panjiajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gp.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ds.yuexingan06.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ya.asd995.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vt.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qj.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zi.hnjuh.cn

[F03] 写入文件（覆盖）
来源：http://as.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jj.muxihuayi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tt.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ju.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lc.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sr.shxzskj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://du.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://uy.shxzukj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jt.gzmigu.cn

[F04] 追加写入文件
来源：http://xn.bookmarksfly.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xc.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ae.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fp.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rn.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nb.hahajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qk.bjjhwx.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kg.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rd.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://oo.bookmarksfly.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vf.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://zv.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://de.hnjuh.cn

TS:   fs.existsSync("a.txt")
来源：http://mf.nicolike.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cv.nszjky.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mg.521024.cn

Ruby: File.exist?("a.txt")
来源：http://ru.yuexingan06.cn

C#:   File.Exists("a.txt")
来源：http://lo.huanxung.cn

[F06] 删除文件
来源：http://vx.chemitech.net.cn

Py:   os.remove("a.txt")
来源：http://rl.jianghongdianzi.cn

PHP:  unlink("a.txt");
来源：http://kd.jianghongdianzi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xd.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://od.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ma.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://do.shtwfgs.cn

Ruby: File.delete("a.txt")
来源：http://tg.yuexingan06.cn

C#:   File.Delete("a.txt");
来源：http://nk.shxzukj.cn

[F07] 创建目录（含多级）
来源：http://up.521024.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://os.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ym.yuexingan06.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sa.colortex.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://du.521024.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://re.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xh.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yw.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://iv.asd995.cn

[F08] 遍历目录
来源：http://vb.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://es.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fs.lnxyls.cn

JS:   fs.readdirSync("dir")
来源：http://ya.nicolike.cn

TS:   fs.readdirSync("dir")
来源：http://fj.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wd.shxzskj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gb.jianghongdianzi.cn

Ruby: Dir.children("dir")
来源：http://zr.jianghongdianzi.cn

C#:   Directory.GetFiles("dir")
来源：http://cv.szxytkj.cn

[F09] 获取文件大小
来源：http://zx.huixiangedu.cn

Py:   os.path.getsize("a.txt")
来源：http://ic.yuntaijiaju.cn

PHP:  filesize("a.txt");
来源：http://hs.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://fj.shxzukj.cn

TS:   fs.statSync("a.txt").size
来源：http://nf.szsharing.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pw.shtwfgs.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gd.521024.cn

Ruby: File.size("a.txt")
来源：http://nf.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://au.muxihuayi.cn

[F10] 取文件扩展名 / 文件名
来源：http://ar.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ch.nicolike.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pq.521024.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jz.lnxyls.cn

TS:   path.extname("a.txt")
来源：http://zy.nszjky.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ej.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://eb.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sq.yuexingan06.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aa.yuexingan06.cn

[F11] 复制与移动文件
来源：http://aj.bookmarksfly.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qw.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jz.bjjhwx.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jd.newstarts.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mp.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bq.szxytkj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ox.yuexingan06.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fm.521024.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yf.muxihuayi.cn

[F12] CSV 读写
来源：http://kn.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wg.bookmarksfly.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://bw.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://po.muxihuayi.cn

TS:   // 同上
来源：http://de.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://um.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ug.chemitech.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uq.szsharing.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://mp.nicolike.cn

================================================================================
来源：http://pt.huixiangedu.cn

G. 面向对象
来源：http://eo.521024.cn

================================================================================
来源：http://rk.shxzukj.cn

[G01] 定义类
来源：http://yh.hnjuh.cn


<!-- 参考信息 -->