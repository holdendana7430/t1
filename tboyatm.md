代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://bn.panjiajie.cn

C#:   s.Substring(1, 3)
来源：http://hy.shxzukj.cn

[E04] 查找子串位置
来源：http://je.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://kd.hahajie.cn

PHP:  strpos($s, "x");
来源：http://kv.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jl.nszjky.cn

TS:   s.indexOf("x")
来源：http://kb.jctech888.com.cn

Java: s.indexOf("x")
来源：http://is.shxzukj.cn

Go:   strings.Index(s, "x")
来源：http://sa.huixinmuqiang.cn

Ruby: s.index("x")
来源：http://sh.nicolike.cn

C#:   s.IndexOf("x")
来源：http://dh.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kw.hnjuh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jd.colortex.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kf.521024.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ex.9csxet.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hu.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dh.huixiangedu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://xj.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nt.colortex.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gp.nszjky.cn

[E06] 替换子串
来源：http://xb.huanxung.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://fi.jianghongdianzi.cn

PHP:  str_replace("a", "b", $s);
来源：http://og.hnjuh.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oz.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://qb.bookmarksfly.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sr.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yn.hnjuh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fs.bookmarksfly.cn

C#:   s.Replace("a", "b")
来源：http://dh.asd995.cn

[E07] 按分隔符拆分
来源：http://cf.9csxet.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ov.bjjhwx.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://li.9csxet.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://as.shxzukj.cn

TS:   s.split(",")
来源：http://ls.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://lo.yuntaijiaju.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zx.nszjky.cn

Ruby: s.split(",");  s.split
来源：http://hj.szsharing.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tv.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://ef.wgjwhj.cn

Py:   ",".join(items)
来源：http://bk.newstarts.cn

PHP:  implode(",", $items);
来源：http://kh.muxihuayi.cn

JS:   items.join(",")
来源：http://bw.yuntaijiaju.cn

TS:   items.join(",")
来源：http://eb.bookmarksfly.cn

Java: String.join(",", items)
来源：http://vz.huixinmuqiang.cn

Go:   strings.Join(items, ",")
来源：http://ed.huixiangedu.cn

Ruby: items.join(",")
来源：http://qg.lnxyls.cn

C#:   string.Join(",", items)
来源：http://qu.bookmarksfly.cn

[E09] 去除所有空白字符
来源：http://ev.huixinmuqiang.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dc.szxytkj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://eu.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://nb.bjjhwx.cn

TS:   s.replace(/\s+/g, "")
来源：http://cu.shxzskj.cn

Java: s.replaceAll("\\s+", "")
来源：http://ng.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dr.lnxyls.cn

Ruby: s.gsub(/\s+/, "")
来源：http://wa.jctech888.com.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tj.newstarts.cn

[E10] 左侧补零 / 定长填充
来源：http://hy.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rx.newstarts.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wg.gzmigu.cn

JS:   "7".padStart(3, "0")
来源：http://qa.jctech888.com.cn

TS:   "7".padStart(3, "0")
来源：http://aq.yuntaijiaju.cn

Java: String.format("%03d", 7)
来源：http://ry.yuntaijiaju.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qm.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://at.huanxung.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wl.huixiangedu.cn

[E11] 反转字符串
来源：http://sa.yuexingan06.cn

Py:   s[::-1]
来源：http://fj.szsharing.cn

PHP:  strrev($s);
来源：http://jy.huixiangedu.cn

JS:   [...s].reverse().join("")
来源：http://al.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://po.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ea.panjiajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://os.wgjwhj.cn

Ruby: s.reverse
来源：http://ws.hahajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ec.nicolike.cn

[E12] 统计某字符出现次数
来源：http://zf.hnjuh.cn

Py:   s.count("a")
来源：http://ku.newstarts.cn

PHP:  substr_count($s, "a");
来源：http://vg.shtwfgs.cn

JS:   s.split("a").length - 1
来源：http://li.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://fe.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zn.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://fl.szsharing.cn

Ruby: s.count("a")
来源：http://dk.wgjwhj.cn

C#:   s.Count(c => c == 'a')
来源：http://vm.wgjwhj.cn

[E13] 逐字符遍历
来源：http://oc.newstarts.cn

Py:   for ch in s: print(ch)
来源：http://kf.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dk.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lj.nszjky.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sn.yuntaijiaju.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://om.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nc.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://eo.newstarts.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://om.bjjhwx.cn

[E14] URL 编码与 Base64
来源：http://wz.haigaiapp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://au.hahajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rz.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://og.szxytkj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dp.lnxyls.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://sv.521024.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://di.szsharing.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tb.jctech888.com.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xq.szsharing.cn

[E15] HTML 转义 / 反转义
来源：http://kz.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bk.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uz.nicolike.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ks.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://nu.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rf.muxihuayi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qf.hnjuh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cz.shxzukj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qa.panjiajie.cn

[E16] 数字千分位
来源：http://ds.szsharing.cn

Py:   f"{1234567:,}"
来源：http://ok.521024.cn

PHP:  number_format(1234567);
来源：http://vz.bjjhwx.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://oy.nszjky.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gx.9csxet.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sg.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://zr.szsharing.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ua.huixinmuqiang.cn

C#:   1234567.ToString("N0")
来源：http://gk.shxzskj.cn

[E17] 首字母大写
来源：http://rh.huanxung.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://no.huixinmuqiang.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ya.haigaiapp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yt.jctech888.com.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ks.szxytkj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qb.hnjuh.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ok.nszjky.cn

Ruby: s.capitalize
来源：http://vd.shtwfgs.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tt.colortex.cn

[E18] 模板占位符替换
来源：http://gs.jctech888.com.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wr.panjiajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://is.yuexingan06.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yo.nszjky.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lx.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sq.huixiangedu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pa.panjiajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ps.shxzskj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qv.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://iw.wgjwhj.cn

Py:   s.splitlines()
来源：http://us.yuexingan06.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mw.huanxung.cn

JS:   s.split(/\r?\n/)
来源：http://sk.nicolike.cn

TS:   s.split(/\r?\n/)
来源：http://jg.szxytkj.cn

Java: s.lines().toList()
来源：http://zc.gzmigu.cn

Go:   strings.Split(s, "\n")
来源：http://wm.wgjwhj.cn

Ruby: s.lines
来源：http://ad.panjiajie.cn

C#:   s.Split('\n')
来源：http://yr.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://bg.hahajie.cn

Py:   if not s:
来源：http://xa.bjjhwx.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://nz.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ok.panjiajie.cn

TS:   if (s === "") {}
来源：http://tg.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://xs.haigaiapp.cn

Go:   if s == "" {}
来源：http://cr.colortex.cn

Ruby: if s.empty?
来源：http://fo.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tg.asd995.cn

[E21] 超长截断加省略号
来源：http://au.panjiajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pn.szsharing.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zv.hnjuh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://li.gzmigu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ec.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://im.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://vy.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jf.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zk.huanxung.cn

[E22] 字节长度与字符长度
来源：http://bx.gzmigu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rh.9csxet.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pz.colortex.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fy.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ay.haigaiapp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qy.wgjwhj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tc.chemitech.net.cn

Ruby: s.bytesize;  s.length
来源：http://pr.bjjhwx.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hp.bjjhwx.cn

================================================================================
来源：http://cl.newstarts.cn

F. 文件与目录
来源：http://eb.wgjwhj.cn

================================================================================
来源：http://vr.huixiangedu.cn

[F01] 读取整个文件
来源：http://fy.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ka.szsharing.cn

PHP:  file_get_contents("a.txt");
来源：http://gc.shtwfgs.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ar.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://st.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qo.hnjuh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://go.shxzskj.cn

Ruby: File.read("a.txt")
来源：http://cn.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://gs.shtwfgs.cn

[F02] 逐行读取文件
来源：http://df.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qt.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ze.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sc.bookmarksfly.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ls.nicolike.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pj.huanxung.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://db.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lz.huanxung.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qk.9csxet.cn

[F03] 写入文件（覆盖）
来源：http://nh.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wn.shxzskj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ww.jctech888.com.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ry.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xn.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qs.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jf.muxihuayi.cn

Ruby: File.write("a.txt", "hi")
来源：http://vc.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bl.hahajie.cn

[F04] 追加写入文件
来源：http://ad.shxzukj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tm.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wh.muxihuayi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wn.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ex.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ne.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://al.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ul.shxzukj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yh.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://bj.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ob.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://jx.9csxet.cn

JS:   fs.existsSync("a.txt")
来源：http://vz.shxzskj.cn

TS:   fs.existsSync("a.txt")
来源：http://je.9csxet.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xz.huanxung.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bb.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://ew.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://jt.yuntaijiaju.cn

[F06] 删除文件
来源：http://ov.huixiangedu.cn

Py:   os.remove("a.txt")
来源：http://kb.shtwfgs.cn

PHP:  unlink("a.txt");
来源：http://lv.chemitech.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yp.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ok.yuntaijiaju.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yu.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://gc.shtwfgs.cn

Ruby: File.delete("a.txt")
来源：http://nc.yuexingan06.cn

C#:   File.Delete("a.txt");
来源：http://ye.9csxet.cn

[F07] 创建目录（含多级）
来源：http://jy.nszjky.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wf.muxihuayi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://eb.panjiajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jo.jianghongdianzi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xu.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pg.muxihuayi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gr.gzmigu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nk.nicolike.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vk.shxzukj.cn

[F08] 遍历目录
来源：http://xe.szsharing.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mt.gzmigu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://le.wgjwhj.cn

JS:   fs.readdirSync("dir")
来源：http://op.lnxyls.cn

TS:   fs.readdirSync("dir")
来源：http://fu.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://oh.nicolike.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bk.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://kd.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://sf.521024.cn

[F09] 获取文件大小
来源：http://rp.colortex.cn

Py:   os.path.getsize("a.txt")
来源：http://kz.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://bp.haigaiapp.cn

JS:   fs.statSync("a.txt").size
来源：http://ft.chemitech.net.cn

TS:   fs.statSync("a.txt").size
来源：http://yz.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://os.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kk.9csxet.cn

Ruby: File.size("a.txt")
来源：http://vc.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://gb.huixinmuqiang.cn

[F10] 取文件扩展名 / 文件名
来源：http://de.szsharing.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://po.wgjwhj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ua.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hu.huanxung.cn

TS:   path.extname("a.txt")
来源：http://np.lnxyls.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ii.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ua.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ms.haigaiapp.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uo.lnxyls.cn

[F11] 复制与移动文件
来源：http://rv.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dw.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tu.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jw.szsharing.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xn.gzmigu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://aw.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zk.wgjwhj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bb.muxihuayi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kl.yuntaijiaju.cn

[F12] CSV 读写
来源：http://di.nicolike.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tq.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qo.shxzukj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uw.huixinmuqiang.cn

TS:   // 同上
来源：http://bj.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dn.szsharing.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://te.hnjuh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hf.jctech888.com.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lx.9csxet.cn

================================================================================
来源：http://wb.szsharing.cn

G. 面向对象
来源：http://ia.huixinmuqiang.cn

================================================================================
来源：http://zd.muxihuayi.cn

[G01] 定义类
来源：http://qn.haigaiapp.cn

Py:   class User: pass
来源：http://lr.colortex.cn

PHP:  class User {}
来源：http://bf.bookmarksfly.cn

JS:   class User {}
来源：http://cb.lnxyls.cn

TS:   class User { name: string = ""; }
来源：http://yf.nszjky.cn

Java: class User {}
来源：http://ht.haigaiapp.cn

Go:   type User struct { Name string }
来源：http://oj.haigaiapp.cn

Ruby: class User; end
来源：http://dl.hahajie.cn

C#:   class User {}
来源：http://cr.huixiangedu.cn

[G02] 构造函数
来源：http://eq.gzmigu.cn

Py:   def __init__(self, name): self.name = name
来源：http://bv.nicolike.cn

PHP:  public function __construct(public string $name) {}
来源：http://zm.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://iy.bjjhwx.cn


<!-- 参考信息 -->