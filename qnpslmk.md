代发 wailian999

PHP:  strpos($s, "x");
来源：http://ku.hnjuh.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ii.shxzukj.cn

TS:   s.indexOf("x")
来源：http://xw.chemitech.net.cn

Java: s.indexOf("x")
来源：http://ra.shxzukj.cn

Go:   strings.Index(s, "x")
来源：http://ps.lnxyls.cn

Ruby: s.index("x")
来源：http://io.shtwfgs.cn

C#:   s.IndexOf("x")
来源：http://gn.szsharing.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sh.wgjwhj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://td.shxzskj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nv.panjiajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ps.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kk.9csxet.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pw.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cu.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vs.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://py.wgjwhj.cn

[E06] 替换子串
来源：http://xx.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ps.521024.cn

PHP:  str_replace("a", "b", $s);
来源：http://ha.chemitech.net.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pb.huixiangedu.cn

TS:   s.replaceAll("a", "b")
来源：http://jv.9csxet.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zn.muxihuayi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ne.shxzukj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cy.bookmarksfly.cn

C#:   s.Replace("a", "b")
来源：http://pn.nszjky.cn

[E07] 按分隔符拆分
来源：http://vc.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ko.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://uu.jianghongdianzi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hv.wgjwhj.cn

TS:   s.split(",")
来源：http://ql.wgjwhj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://yx.shxzskj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://nx.shxzukj.cn

Ruby: s.split(",");  s.split
来源：http://ue.9csxet.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qd.nicolike.cn

[E08] 数组按分隔符合并
来源：http://mi.haigaiapp.cn

Py:   ",".join(items)
来源：http://cr.muxihuayi.cn

PHP:  implode(",", $items);
来源：http://sc.521024.cn

JS:   items.join(",")
来源：http://gx.huixinmuqiang.cn

TS:   items.join(",")
来源：http://nn.yuntaijiaju.cn

Java: String.join(",", items)
来源：http://hz.colortex.cn

Go:   strings.Join(items, ",")
来源：http://dc.wgjwhj.cn

Ruby: items.join(",")
来源：http://pe.bjjhwx.cn

C#:   string.Join(",", items)
来源：http://iq.lnxyls.cn

[E09] 去除所有空白字符
来源：http://eb.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vi.haigaiapp.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://aq.hahajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://pa.haigaiapp.cn

TS:   s.replace(/\s+/g, "")
来源：http://ar.szxytkj.cn

Java: s.replaceAll("\\s+", "")
来源：http://oz.haigaiapp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pf.yuntaijiaju.cn

Ruby: s.gsub(/\s+/, "")
来源：http://og.newstarts.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mb.bjjhwx.cn

[E10] 左侧补零 / 定长填充
来源：http://ec.nicolike.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gm.9csxet.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ed.521024.cn

JS:   "7".padStart(3, "0")
来源：http://ad.shtwfgs.cn

TS:   "7".padStart(3, "0")
来源：http://wk.bjjhwx.cn

Java: String.format("%03d", 7)
来源：http://jo.muxihuayi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rf.newstarts.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pj.shtwfgs.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zp.szxytkj.cn

[E11] 反转字符串
来源：http://um.newstarts.cn

Py:   s[::-1]
来源：http://wu.nicolike.cn

PHP:  strrev($s);
来源：http://vy.haigaiapp.cn

JS:   [...s].reverse().join("")
来源：http://if.521024.cn

TS:   [...s].reverse().join("")
来源：http://rn.wgjwhj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jx.yuntaijiaju.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ho.muxihuayi.cn

Ruby: s.reverse
来源：http://be.shtwfgs.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nt.huanxung.cn

[E12] 统计某字符出现次数
来源：http://vz.hnjuh.cn

Py:   s.count("a")
来源：http://ey.szsharing.cn

PHP:  substr_count($s, "a");
来源：http://yr.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://jo.huixiangedu.cn

TS:   s.split("a").length - 1
来源：http://zc.huixinmuqiang.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wm.nicolike.cn

Go:   strings.Count(s, "a")
来源：http://gv.haigaiapp.cn

Ruby: s.count("a")
来源：http://in.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://to.huixiangedu.cn

[E13] 逐字符遍历
来源：http://ps.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://fl.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://jj.hnjuh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sj.huixinmuqiang.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bh.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vg.muxihuayi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zw.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qk.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hf.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://od.9csxet.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yf.huanxung.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://oi.shxzukj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qm.nszjky.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xy.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://eb.szsharing.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rb.haigaiapp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://cj.nszjky.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sq.newstarts.cn

[E15] HTML 转义 / 反转义
来源：http://mu.hahajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://oo.nicolike.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://is.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pb.wgjwhj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nn.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://je.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nl.bjjhwx.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mh.lnxyls.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vr.yuntaijiaju.cn

[E16] 数字千分位
来源：http://nt.huanxung.cn

Py:   f"{1234567:,}"
来源：http://qr.yuexingan06.cn

PHP:  number_format(1234567);
来源：http://bv.jianghongdianzi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rv.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://oh.bookmarksfly.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://kn.jctech888.com.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pw.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://se.yuexingan06.cn

C#:   1234567.ToString("N0")
来源：http://ou.szxytkj.cn

[E17] 首字母大写
来源：http://mo.bjjhwx.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lz.szsharing.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wz.huanxung.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://md.shtwfgs.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iw.shxzukj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://nf.muxihuayi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ve.szsharing.cn

Ruby: s.capitalize
来源：http://rt.hahajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ue.yuexingan06.cn

[E18] 模板占位符替换
来源：http://xy.muxihuayi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bx.huixiangedu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://nd.hnjuh.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://om.huixinmuqiang.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wn.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hy.huixinmuqiang.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jw.lnxyls.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pj.521024.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hw.bookmarksfly.cn

[E19] 多行文本按行拆分
来源：http://lz.chemitech.net.cn

Py:   s.splitlines()
来源：http://pk.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xq.hnjuh.cn

JS:   s.split(/\r?\n/)
来源：http://yg.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://gd.asd995.cn

Java: s.lines().toList()
来源：http://vg.lnxyls.cn

Go:   strings.Split(s, "\n")
来源：http://do.hahajie.cn

Ruby: s.lines
来源：http://fi.newstarts.cn

C#:   s.Split('\n')
来源：http://fn.521024.cn

[E20] 判断字符串是否为空
来源：http://ic.hnjuh.cn

Py:   if not s:
来源：http://zk.muxihuayi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ue.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://an.bjjhwx.cn

TS:   if (s === "") {}
来源：http://oj.shxzskj.cn

Java: if (s.isEmpty()) {}
来源：http://pk.panjiajie.cn

Go:   if s == "" {}
来源：http://is.shtwfgs.cn

Ruby: if s.empty?
来源：http://ob.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://lk.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://jl.newstarts.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ps.shxzskj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qb.huixinmuqiang.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wa.muxihuayi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cr.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ak.szsharing.cn

Go:   // 按 rune 判断长度后截断
来源：http://ez.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vh.colortex.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jy.yuntaijiaju.cn

[E22] 字节长度与字符长度
来源：http://lj.newstarts.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hm.jctech888.com.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fp.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://eg.colortex.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sj.jianghongdianzi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tc.chemitech.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ld.nicolike.cn

Ruby: s.bytesize;  s.length
来源：http://yf.muxihuayi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fw.shxzukj.cn

================================================================================
来源：http://vm.haigaiapp.cn

F. 文件与目录
来源：http://no.szsharing.cn

================================================================================
来源：http://bv.muxihuayi.cn

[F01] 读取整个文件
来源：http://dn.asd995.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qd.yuntaijiaju.cn

PHP:  file_get_contents("a.txt");
来源：http://pg.gzmigu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fg.521024.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://io.hnjuh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yf.huixinmuqiang.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rp.nszjky.cn

Ruby: File.read("a.txt")
来源：http://hu.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://dv.hnjuh.cn

[F02] 逐行读取文件
来源：http://fm.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ux.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://od.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://il.asd995.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iw.shxzskj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hl.wgjwhj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fo.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pa.shxzukj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zz.huixinmuqiang.cn

[F03] 写入文件（覆盖）
来源：http://lr.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://eo.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ft.huixinmuqiang.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cm.yuntaijiaju.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bv.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uy.nszjky.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wb.shtwfgs.cn

Ruby: File.write("a.txt", "hi")
来源：http://hd.9csxet.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wr.bjjhwx.cn

[F04] 追加写入文件
来源：http://wt.nszjky.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mz.huanxung.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ve.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xj.bjjhwx.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yl.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yx.gzmigu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bh.hahajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bx.shtwfgs.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://aw.gzmigu.cn

[F05] 判断文件或目录是否存在
来源：http://ze.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wa.9csxet.cn

PHP:  file_exists("a.txt");
来源：http://wt.hnjuh.cn

JS:   fs.existsSync("a.txt")
来源：http://bp.panjiajie.cn

TS:   fs.existsSync("a.txt")
来源：http://sw.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qh.haigaiapp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://au.hahajie.cn

Ruby: File.exist?("a.txt")
来源：http://db.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://ma.wgjwhj.cn

[F06] 删除文件
来源：http://ls.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://ra.yuexingan06.cn

PHP:  unlink("a.txt");
来源：http://ix.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://kc.huixinmuqiang.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ik.huanxung.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pl.shtwfgs.cn

Go:   os.Remove("a.txt")
来源：http://za.lnxyls.cn

Ruby: File.delete("a.txt")
来源：http://rn.shxzukj.cn

C#:   File.Delete("a.txt");
来源：http://yy.9csxet.cn

[F07] 创建目录（含多级）
来源：http://zd.huixiangedu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zp.shxzukj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rv.colortex.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yu.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gb.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lc.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oa.shxzukj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kg.bookmarksfly.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yz.nicolike.cn

[F08] 遍历目录
来源：http://zy.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xt.chemitech.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gi.huixiangedu.cn

JS:   fs.readdirSync("dir")
来源：http://qq.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://qs.shtwfgs.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ha.shtwfgs.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://us.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://lc.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://yh.szsharing.cn

[F09] 获取文件大小
来源：http://ne.colortex.cn

Py:   os.path.getsize("a.txt")
来源：http://up.shxzskj.cn

PHP:  filesize("a.txt");
来源：http://rs.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://eg.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://ip.huanxung.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ef.shxzukj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pp.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://ak.jctech888.com.cn

C#:   new FileInfo("a.txt").Length
来源：http://mx.huixinmuqiang.cn

[F10] 取文件扩展名 / 文件名
来源：http://gi.lnxyls.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://om.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fq.yuntaijiaju.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zc.wgjwhj.cn

TS:   path.extname("a.txt")
来源：http://jp.newstarts.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ps.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://em.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vw.lnxyls.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mo.szsharing.cn

[F11] 复制与移动文件
来源：http://ty.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jy.huanxung.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wk.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xt.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jj.yuntaijiaju.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mu.gzmigu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xi.bookmarksfly.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wr.jianghongdianzi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ip.shxzskj.cn

[F12] CSV 读写
来源：http://rk.jianghongdianzi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://aj.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ce.hnjuh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cw.yuexingan06.cn

TS:   // 同上
来源：http://yz.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wo.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hg.shxzukj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tq.jianghongdianzi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sv.9csxet.cn

================================================================================
来源：http://kw.bookmarksfly.cn

G. 面向对象
来源：http://fj.huixiangedu.cn

================================================================================
来源：http://ee.muxihuayi.cn

[G01] 定义类
来源：http://wt.asd995.cn

Py:   class User: pass
来源：http://ry.jctech888.com.cn

PHP:  class User {}
来源：http://ak.wgjwhj.cn

JS:   class User {}
来源：http://lv.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://pn.gzmigu.cn

Java: class User {}
来源：http://sh.9csxet.cn

Go:   type User struct { Name string }
来源：http://pf.huixiangedu.cn

Ruby: class User; end
来源：http://av.asd995.cn

C#:   class User {}
来源：http://nv.huixiangedu.cn

[G02] 构造函数
来源：http://rb.hnjuh.cn

Py:   def __init__(self, name): self.name = name
来源：http://bx.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://uy.wgjwhj.cn

JS:   constructor(name) { this.name = name; }
来源：http://uc.nicolike.cn

TS:   constructor(public name: string) {}
来源：http://ml.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://gn.szxytkj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fo.muxihuayi.cn

Ruby: def initialize(name); @name = name; end
来源：http://eq.muxihuayi.cn


<!-- 参考信息 -->