代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://bd.huanxung.cn

C#:   s.Substring(1, 3)
来源：http://af.yuntaijiaju.cn

[E04] 查找子串位置
来源：http://ru.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://ji.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://cb.huixiangedu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://zg.gzmigu.cn

TS:   s.indexOf("x")
来源：http://wh.521024.cn

Java: s.indexOf("x")
来源：http://cd.bjjhwx.cn

Go:   strings.Index(s, "x")
来源：http://zj.szxytkj.cn

Ruby: s.index("x")
来源：http://tw.jianghongdianzi.cn

C#:   s.IndexOf("x")
来源：http://lu.shxzskj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://xw.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hg.hahajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://tb.colortex.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uz.newstarts.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://yf.521024.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bw.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xn.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wf.nicolike.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://tr.shtwfgs.cn

[E06] 替换子串
来源：http://qx.huanxung.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ab.hnjuh.cn

PHP:  str_replace("a", "b", $s);
来源：http://fc.9csxet.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zp.muxihuayi.cn

TS:   s.replaceAll("a", "b")
来源：http://xn.yuntaijiaju.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oh.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wt.wgjwhj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pz.9csxet.cn

C#:   s.Replace("a", "b")
来源：http://yj.521024.cn

[E07] 按分隔符拆分
来源：http://pf.asd995.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ns.hnjuh.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://kh.lnxyls.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://do.nszjky.cn

TS:   s.split(",")
来源：http://vk.bookmarksfly.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ds.bookmarksfly.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dh.yuntaijiaju.cn

Ruby: s.split(",");  s.split
来源：http://zz.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ca.huixinmuqiang.cn

[E08] 数组按分隔符合并
来源：http://bp.hnjuh.cn

Py:   ",".join(items)
来源：http://ic.haigaiapp.cn

PHP:  implode(",", $items);
来源：http://nf.lnxyls.cn

JS:   items.join(",")
来源：http://ic.hnjuh.cn

TS:   items.join(",")
来源：http://pj.bookmarksfly.cn

Java: String.join(",", items)
来源：http://zf.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://vo.shxzskj.cn

Ruby: items.join(",")
来源：http://qd.szxytkj.cn

C#:   string.Join(",", items)
来源：http://kv.jctech888.com.cn

[E09] 去除所有空白字符
来源：http://pf.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://nr.9csxet.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://sj.bookmarksfly.cn

JS:   s.replace(/\s+/g, "")
来源：http://qz.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://wo.yuexingan06.cn

Java: s.replaceAll("\\s+", "")
来源：http://pe.szsharing.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qu.hnjuh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ab.colortex.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rt.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://kc.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qh.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jh.huixiangedu.cn

JS:   "7".padStart(3, "0")
来源：http://lt.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://xd.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://jc.yuexingan06.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mg.chemitech.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ax.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vq.colortex.cn

[E11] 反转字符串
来源：http://mf.shxzskj.cn

Py:   s[::-1]
来源：http://sb.szxytkj.cn

PHP:  strrev($s);
来源：http://cj.huanxung.cn

JS:   [...s].reverse().join("")
来源：http://ru.521024.cn

TS:   [...s].reverse().join("")
来源：http://vn.shxzukj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lj.jianghongdianzi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cj.newstarts.cn

Ruby: s.reverse
来源：http://kj.yuntaijiaju.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gq.hnjuh.cn

[E12] 统计某字符出现次数
来源：http://br.hahajie.cn

Py:   s.count("a")
来源：http://yn.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://ea.huixinmuqiang.cn

JS:   s.split("a").length - 1
来源：http://nz.9csxet.cn

TS:   s.split("a").length - 1
来源：http://nv.gzmigu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xe.huixiangedu.cn

Go:   strings.Count(s, "a")
来源：http://rh.huixiangedu.cn

Ruby: s.count("a")
来源：http://nd.szxytkj.cn

C#:   s.Count(c => c == 'a')
来源：http://qq.huixiangedu.cn

[E13] 逐字符遍历
来源：http://cu.521024.cn

Py:   for ch in s: print(ch)
来源：http://lf.bjjhwx.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xj.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lr.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ec.panjiajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hy.shxzukj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://xk.hnjuh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fe.wgjwhj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cc.huanxung.cn

[E14] URL 编码与 Base64
来源：http://er.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://gf.nszjky.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bl.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yr.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wy.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qr.newstarts.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yr.colortex.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yo.lnxyls.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xl.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://er.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://od.shxzskj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ht.wgjwhj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ou.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ng.nszjky.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hs.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://su.szsharing.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jo.hnjuh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ry.huixiangedu.cn

[E16] 数字千分位
来源：http://gg.colortex.cn

Py:   f"{1234567:,}"
来源：http://pu.nicolike.cn

PHP:  number_format(1234567);
来源：http://rz.huixiangedu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://de.nszjky.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tk.521024.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pj.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zz.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dt.chemitech.net.cn

C#:   1234567.ToString("N0")
来源：http://ay.nszjky.cn

[E17] 首字母大写
来源：http://iv.nicolike.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fm.hnjuh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bh.huanxung.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vu.9csxet.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rx.lnxyls.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yb.asd995.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sg.9csxet.cn

Ruby: s.capitalize
来源：http://ot.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ls.9csxet.cn

[E18] 模板占位符替换
来源：http://co.panjiajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yp.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qb.lnxyls.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://it.nicolike.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tv.shxzskj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ly.muxihuayi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://de.bjjhwx.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zr.yuexingan06.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lh.jianghongdianzi.cn

[E19] 多行文本按行拆分
来源：http://cx.wgjwhj.cn

Py:   s.splitlines()
来源：http://qm.bjjhwx.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gj.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://za.lnxyls.cn

TS:   s.split(/\r?\n/)
来源：http://vy.chemitech.net.cn

Java: s.lines().toList()
来源：http://vz.nszjky.cn

Go:   strings.Split(s, "\n")
来源：http://wp.hnjuh.cn

Ruby: s.lines
来源：http://ug.colortex.cn

C#:   s.Split('\n')
来源：http://tb.colortex.cn

[E20] 判断字符串是否为空
来源：http://je.yuexingan06.cn

Py:   if not s:
来源：http://mc.muxihuayi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xp.bjjhwx.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zo.chemitech.net.cn

TS:   if (s === "") {}
来源：http://di.9csxet.cn

Java: if (s.isEmpty()) {}
来源：http://zo.muxihuayi.cn

Go:   if s == "" {}
来源：http://to.nicolike.cn

Ruby: if s.empty?
来源：http://se.521024.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ks.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://np.huixinmuqiang.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ef.szxytkj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://lg.jctech888.com.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xr.asd995.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uz.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ct.szxytkj.cn

Go:   // 按 rune 判断长度后截断
来源：http://il.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hy.haigaiapp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iu.asd995.cn

[E22] 字节长度与字符长度
来源：http://vp.huixinmuqiang.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://at.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://vc.hahajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zo.szxytkj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ad.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yt.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://no.521024.cn

Ruby: s.bytesize;  s.length
来源：http://zn.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ec.jctech888.com.cn

================================================================================
来源：http://yv.muxihuayi.cn

F. 文件与目录
来源：http://of.chemitech.net.cn

================================================================================
来源：http://vj.lnxyls.cn

[F01] 读取整个文件
来源：http://oc.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oa.shxzskj.cn

PHP:  file_get_contents("a.txt");
来源：http://jc.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cq.huixiangedu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ph.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ti.nicolike.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mt.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://oz.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://wo.shtwfgs.cn

[F02] 逐行读取文件
来源：http://ym.jctech888.com.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sm.huixinmuqiang.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ns.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://se.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yj.asd995.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ok.shxzukj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ec.bjjhwx.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fy.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xl.jctech888.com.cn

[F03] 写入文件（覆盖）
来源：http://qy.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jw.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ri.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lh.shxzukj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jc.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bw.chemitech.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zu.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://kf.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mv.bjjhwx.cn

[F04] 追加写入文件
来源：http://ak.huixinmuqiang.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qc.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rj.yuntaijiaju.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eq.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rs.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sc.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jf.bookmarksfly.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://up.nicolike.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qd.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://gp.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fl.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://fg.chemitech.net.cn

JS:   fs.existsSync("a.txt")
来源：http://qj.jctech888.com.cn

TS:   fs.existsSync("a.txt")
来源：http://eu.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zj.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fx.panjiajie.cn

Ruby: File.exist?("a.txt")
来源：http://eq.muxihuayi.cn

C#:   File.Exists("a.txt")
来源：http://hp.szsharing.cn

[F06] 删除文件
来源：http://ba.asd995.cn

Py:   os.remove("a.txt")
来源：http://rj.bjjhwx.cn

PHP:  unlink("a.txt");
来源：http://ct.colortex.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ua.haigaiapp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yf.nszjky.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ta.muxihuayi.cn

Go:   os.Remove("a.txt")
来源：http://fa.521024.cn

Ruby: File.delete("a.txt")
来源：http://qy.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://pj.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://ha.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://xj.szxytkj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zy.haigaiapp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ap.521024.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yh.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jv.yuexingan06.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uw.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oz.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pv.nszjky.cn

[F08] 遍历目录
来源：http://oc.yuexingan06.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dv.hnjuh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ht.huanxung.cn

JS:   fs.readdirSync("dir")
来源：http://ki.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://zp.haigaiapp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://kt.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ih.muxihuayi.cn

Ruby: Dir.children("dir")
来源：http://xt.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://wh.nicolike.cn

[F09] 获取文件大小
来源：http://ce.chemitech.net.cn

Py:   os.path.getsize("a.txt")
来源：http://nk.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://bi.huixiangedu.cn

JS:   fs.statSync("a.txt").size
来源：http://eg.yuexingan06.cn

TS:   fs.statSync("a.txt").size
来源：http://pb.szsharing.cn

Java: Files.size(Path.of("a.txt"))
来源：http://md.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ei.bjjhwx.cn

Ruby: File.size("a.txt")
来源：http://tx.newstarts.cn

C#:   new FileInfo("a.txt").Length
来源：http://ma.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://cf.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gp.jctech888.com.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vu.chemitech.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://or.huanxung.cn

TS:   path.extname("a.txt")
来源：http://og.9csxet.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ul.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://fd.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ic.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hc.colortex.cn

[F11] 复制与移动文件
来源：http://mu.asd995.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ux.haigaiapp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cx.bjjhwx.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wy.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jd.panjiajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qu.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dd.bjjhwx.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nz.gzmigu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vn.yuntaijiaju.cn

[F12] CSV 读写
来源：http://qg.gzmigu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://uh.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rd.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wb.huanxung.cn

TS:   // 同上
来源：http://jb.szsharing.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vo.chemitech.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wh.jianghongdianzi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ud.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rh.nszjky.cn

================================================================================
来源：http://cq.jianghongdianzi.cn

G. 面向对象
来源：http://yo.haigaiapp.cn

================================================================================
来源：http://kh.hnjuh.cn

[G01] 定义类
来源：http://st.szxytkj.cn

Py:   class User: pass
来源：http://sd.gzmigu.cn

PHP:  class User {}
来源：http://ib.hahajie.cn

JS:   class User {}
来源：http://zk.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://is.hahajie.cn

Java: class User {}
来源：http://ur.szxytkj.cn

Go:   type User struct { Name string }
来源：http://nn.haigaiapp.cn

Ruby: class User; end
来源：http://dn.huanxung.cn

C#:   class User {}
来源：http://ne.yuexingan06.cn

[G02] 构造函数
来源：http://js.9csxet.cn

Py:   def __init__(self, name): self.name = name
来源：http://vl.hnjuh.cn

PHP:  public function __construct(public string $name) {}
来源：http://gr.shxzskj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ou.huixiangedu.cn


<!-- 参考信息 -->