代发 wailian999

TS:   "ab".repeat(3)
来源：http://ab.yuexingan06.cn

Java: "ab".repeat(3)
来源：http://xt.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://yo.nicolike.cn

Ruby: "ab" * 3
来源：http://qf.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rn.lnxyls.cn

[E03] 截取子串
来源：http://oc.jctech888.com.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nq.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ni.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mi.hnjuh.cn

TS:   s.slice(1, 4)
来源：http://ix.panjiajie.cn

Java: s.substring(1, 4)
来源：http://jo.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ik.521024.cn

Ruby: s[1, 3];  s[1..3]
来源：http://gn.yuexingan06.cn

C#:   s.Substring(1, 3)
来源：http://xq.shxzskj.cn

[E04] 查找子串位置
来源：http://jf.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://fy.lnxyls.cn

PHP:  strpos($s, "x");
来源：http://wr.muxihuayi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xn.jctech888.com.cn

TS:   s.indexOf("x")
来源：http://yr.nicolike.cn

Java: s.indexOf("x")
来源：http://rz.gzmigu.cn

Go:   strings.Index(s, "x")
来源：http://qj.huanxung.cn

Ruby: s.index("x")
来源：http://gl.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://wy.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sl.9csxet.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ko.newstarts.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://em.colortex.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ty.szxytkj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://wu.hnjuh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://gf.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lf.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://zw.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://va.9csxet.cn

[E06] 替换子串
来源：http://wu.nszjky.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://px.colortex.cn

PHP:  str_replace("a", "b", $s);
来源：http://ym.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cr.szsharing.cn

TS:   s.replaceAll("a", "b")
来源：http://dx.yuntaijiaju.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cp.jianghongdianzi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bw.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ft.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://zs.haigaiapp.cn

[E07] 按分隔符拆分
来源：http://gm.jctech888.com.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://in.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ac.hnjuh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tt.haigaiapp.cn

TS:   s.split(",")
来源：http://fx.colortex.cn

Java: s.split(",");  s.split("\\s+")
来源：http://xk.chemitech.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cw.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://fa.haigaiapp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://qb.shxzskj.cn

Py:   ",".join(items)
来源：http://nj.wgjwhj.cn

PHP:  implode(",", $items);
来源：http://yl.muxihuayi.cn

JS:   items.join(",")
来源：http://uc.nszjky.cn

TS:   items.join(",")
来源：http://qm.szsharing.cn

Java: String.join(",", items)
来源：http://yr.bookmarksfly.cn

Go:   strings.Join(items, ",")
来源：http://gy.nicolike.cn

Ruby: items.join(",")
来源：http://oq.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://wa.9csxet.cn

[E09] 去除所有空白字符
来源：http://sz.bjjhwx.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pu.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vs.bookmarksfly.cn

JS:   s.replace(/\s+/g, "")
来源：http://lr.bjjhwx.cn

TS:   s.replace(/\s+/g, "")
来源：http://ej.huanxung.cn

Java: s.replaceAll("\\s+", "")
来源：http://xi.lnxyls.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://se.hahajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://fr.colortex.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://dt.szxytkj.cn

[E10] 左侧补零 / 定长填充
来源：http://mw.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jv.9csxet.cn

JS:   "7".padStart(3, "0")
来源：http://du.szxytkj.cn

TS:   "7".padStart(3, "0")
来源：http://cl.panjiajie.cn

Java: String.format("%03d", 7)
来源：http://ld.haigaiapp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kx.panjiajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dt.huanxung.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zs.wgjwhj.cn

[E11] 反转字符串
来源：http://uj.jianghongdianzi.cn

Py:   s[::-1]
来源：http://ee.panjiajie.cn

PHP:  strrev($s);
来源：http://cu.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://iv.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://cz.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gp.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://yj.chemitech.net.cn

Ruby: s.reverse
来源：http://ed.colortex.cn

C#:   new string(s.Reverse().ToArray())
来源：http://wo.huanxung.cn

[E12] 统计某字符出现次数
来源：http://rf.521024.cn

Py:   s.count("a")
来源：http://bw.yuntaijiaju.cn

PHP:  substr_count($s, "a");
来源：http://kg.wgjwhj.cn

JS:   s.split("a").length - 1
来源：http://rf.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://wk.hnjuh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xq.hnjuh.cn

Go:   strings.Count(s, "a")
来源：http://ke.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://ln.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://js.wgjwhj.cn

[E13] 逐字符遍历
来源：http://vs.wgjwhj.cn

Py:   for ch in s: print(ch)
来源：http://cl.huixiangedu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qg.hahajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fp.shxzukj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bp.huanxung.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ts.colortex.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wo.bookmarksfly.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://bg.newstarts.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pl.szxytkj.cn

[E14] URL 编码与 Base64
来源：http://vn.huanxung.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vk.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://su.colortex.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ig.newstarts.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hb.shxzskj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ti.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wc.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ec.huanxung.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uf.shxzukj.cn

[E15] HTML 转义 / 反转义
来源：http://wn.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://cq.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mg.yuexingan06.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gm.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fy.jctech888.com.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ke.shxzskj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://bw.huixinmuqiang.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ct.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bg.colortex.cn

[E16] 数字千分位
来源：http://ra.panjiajie.cn

Py:   f"{1234567:,}"
来源：http://jy.muxihuayi.cn

PHP:  number_format(1234567);
来源：http://lw.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mb.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://vj.huanxung.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xf.hahajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://we.szsharing.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hy.gzmigu.cn

C#:   1234567.ToString("N0")
来源：http://qw.newstarts.cn

[E17] 首字母大写
来源：http://sc.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xb.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://in.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://si.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://eb.nszjky.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://th.shxzskj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ld.shxzukj.cn

Ruby: s.capitalize
来源：http://gy.haigaiapp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ik.jctech888.com.cn

[E18] 模板占位符替换
来源：http://jr.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zu.haigaiapp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://it.jianghongdianzi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://db.shxzukj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mk.yuexingan06.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hy.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ic.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://tr.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lb.shtwfgs.cn

[E19] 多行文本按行拆分
来源：http://rp.szxytkj.cn

Py:   s.splitlines()
来源：http://cg.nicolike.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://da.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://eh.asd995.cn

TS:   s.split(/\r?\n/)
来源：http://jd.hahajie.cn

Java: s.lines().toList()
来源：http://ts.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://xs.lnxyls.cn

Ruby: s.lines
来源：http://zu.chemitech.net.cn

C#:   s.Split('\n')
来源：http://if.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://kw.szxytkj.cn

Py:   if not s:
来源：http://jl.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wl.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gi.gzmigu.cn

TS:   if (s === "") {}
来源：http://rd.jianghongdianzi.cn

Java: if (s.isEmpty()) {}
来源：http://uw.hahajie.cn

Go:   if s == "" {}
来源：http://fw.yuexingan06.cn

Ruby: if s.empty?
来源：http://nc.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://nj.shtwfgs.cn

[E21] 超长截断加省略号
来源：http://um.chemitech.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ei.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mv.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ij.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://eo.chemitech.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ip.gzmigu.cn

Go:   // 按 rune 判断长度后截断
来源：http://oc.nszjky.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://em.panjiajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://by.bjjhwx.cn

[E22] 字节长度与字符长度
来源：http://ei.9csxet.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wo.shxzskj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vg.nicolike.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yr.yuexingan06.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fz.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tv.bookmarksfly.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ps.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://bz.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xz.bjjhwx.cn

================================================================================
来源：http://rr.panjiajie.cn

F. 文件与目录
来源：http://iz.wgjwhj.cn

================================================================================
来源：http://sz.muxihuayi.cn

[F01] 读取整个文件
来源：http://zp.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xk.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://sb.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ej.haigaiapp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mp.szxytkj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kb.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://od.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://qm.hahajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://ia.szxytkj.cn

[F02] 逐行读取文件
来源：http://mx.haigaiapp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ox.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hy.shtwfgs.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ny.nicolike.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gz.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ce.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://li.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zn.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wk.nszjky.cn

[F03] 写入文件（覆盖）
来源：http://vg.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wc.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rs.newstarts.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ay.haigaiapp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://we.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ua.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oc.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://fj.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bt.jctech888.com.cn

[F04] 追加写入文件
来源：http://nk.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lp.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qy.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://os.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://et.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tq.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mg.nszjky.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rw.9csxet.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gb.shtwfgs.cn

[F05] 判断文件或目录是否存在
来源：http://aa.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://en.huixiangedu.cn

PHP:  file_exists("a.txt");
来源：http://gj.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://oq.jctech888.com.cn

TS:   fs.existsSync("a.txt")
来源：http://lu.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pv.szxytkj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yy.nszjky.cn

Ruby: File.exist?("a.txt")
来源：http://mj.gzmigu.cn

C#:   File.Exists("a.txt")
来源：http://bi.bjjhwx.cn

[F06] 删除文件
来源：http://nt.nicolike.cn

Py:   os.remove("a.txt")
来源：http://nz.huixiangedu.cn

PHP:  unlink("a.txt");
来源：http://kp.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ht.szxytkj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jl.panjiajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://en.jctech888.com.cn

Go:   os.Remove("a.txt")
来源：http://ak.yuntaijiaju.cn

Ruby: File.delete("a.txt")
来源：http://ib.bjjhwx.cn

C#:   File.Delete("a.txt");
来源：http://jh.hnjuh.cn

[F07] 创建目录（含多级）
来源：http://xc.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ph.hahajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://io.chemitech.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zs.szxytkj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eu.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wy.huanxung.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uz.szxytkj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bh.asd995.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tw.shxzskj.cn

[F08] 遍历目录
来源：http://zz.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rn.asd995.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bu.521024.cn

JS:   fs.readdirSync("dir")
来源：http://ur.chemitech.net.cn

TS:   fs.readdirSync("dir")
来源：http://uu.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ea.jctech888.com.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hk.panjiajie.cn

Ruby: Dir.children("dir")
来源：http://ns.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://hm.huixiangedu.cn

[F09] 获取文件大小
来源：http://nw.muxihuayi.cn

Py:   os.path.getsize("a.txt")
来源：http://lu.shxzukj.cn

PHP:  filesize("a.txt");
来源：http://nn.muxihuayi.cn

JS:   fs.statSync("a.txt").size
来源：http://dp.9csxet.cn

TS:   fs.statSync("a.txt").size
来源：http://ir.colortex.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vc.asd995.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dp.gzmigu.cn

Ruby: File.size("a.txt")
来源：http://zx.huixiangedu.cn

C#:   new FileInfo("a.txt").Length
来源：http://wt.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://ny.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ym.yuexingan06.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ss.nszjky.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qb.huixiangedu.cn

TS:   path.extname("a.txt")
来源：http://di.hnjuh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ii.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rt.newstarts.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://br.521024.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://to.gzmigu.cn

[F11] 复制与移动文件
来源：http://ni.lnxyls.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ql.huanxung.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ky.asd995.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lr.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rj.muxihuayi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ic.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://en.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ze.chemitech.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pi.yuexingan06.cn

[F12] CSV 读写
来源：http://cf.huanxung.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zl.huixinmuqiang.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://cq.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fp.muxihuayi.cn

TS:   // 同上
来源：http://qx.lnxyls.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zw.yuntaijiaju.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lf.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lh.szsharing.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fr.asd995.cn

================================================================================
来源：http://nb.shxzukj.cn

G. 面向对象
来源：http://wn.muxihuayi.cn

================================================================================
来源：http://id.wgjwhj.cn

[G01] 定义类
来源：http://xz.hahajie.cn


<!-- 参考信息 -->