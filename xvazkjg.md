代发 wailian999

Go:   strings.Index(s, "x")
来源：http://sk.shxzskj.cn

Ruby: s.index("x")
来源：http://kc.521024.cn

C#:   s.IndexOf("x")
来源：http://mc.yuexingan06.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://td.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jk.yuntaijiaju.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://es.bookmarksfly.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rl.jianghongdianzi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://th.panjiajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vd.jctech888.com.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pc.jctech888.com.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://at.szsharing.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fa.panjiajie.cn

[E06] 替换子串
来源：http://ro.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vz.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://lf.shxzukj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ag.bookmarksfly.cn

TS:   s.replaceAll("a", "b")
来源：http://dj.asd995.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ib.wgjwhj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ef.nszjky.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ix.wgjwhj.cn

C#:   s.Replace("a", "b")
来源：http://eq.shxzskj.cn

[E07] 按分隔符拆分
来源：http://uw.nszjky.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xy.nszjky.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://id.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jt.haigaiapp.cn

TS:   s.split(",")
来源：http://hq.9csxet.cn

Java: s.split(",");  s.split("\\s+")
来源：http://es.gzmigu.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qt.huixiangedu.cn

Ruby: s.split(",");  s.split
来源：http://th.chemitech.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zp.hahajie.cn

[E08] 数组按分隔符合并
来源：http://ju.9csxet.cn

Py:   ",".join(items)
来源：http://zz.bjjhwx.cn

PHP:  implode(",", $items);
来源：http://jn.wgjwhj.cn

JS:   items.join(",")
来源：http://xn.shtwfgs.cn

TS:   items.join(",")
来源：http://kc.haigaiapp.cn

Java: String.join(",", items)
来源：http://ln.gzmigu.cn

Go:   strings.Join(items, ",")
来源：http://ti.colortex.cn

Ruby: items.join(",")
来源：http://ky.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://zp.lnxyls.cn

[E09] 去除所有空白字符
来源：http://mg.wgjwhj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pc.wgjwhj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zh.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://lz.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://md.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://tq.newstarts.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://nh.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://af.wgjwhj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://zz.shxzukj.cn

[E10] 左侧补零 / 定长填充
来源：http://el.nszjky.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ru.shxzskj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yy.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://uz.colortex.cn

TS:   "7".padStart(3, "0")
来源：http://vi.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://sl.yuntaijiaju.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jl.wgjwhj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zp.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vn.bookmarksfly.cn

[E11] 反转字符串
来源：http://vw.asd995.cn

Py:   s[::-1]
来源：http://cs.hahajie.cn

PHP:  strrev($s);
来源：http://tv.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://hy.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://cm.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ey.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tn.haigaiapp.cn

Ruby: s.reverse
来源：http://pr.hahajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ij.yuexingan06.cn

[E12] 统计某字符出现次数
来源：http://ea.lnxyls.cn

Py:   s.count("a")
来源：http://qa.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://dw.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://fj.9csxet.cn

TS:   s.split("a").length - 1
来源：http://sb.szsharing.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fp.huanxung.cn

Go:   strings.Count(s, "a")
来源：http://na.hnjuh.cn

Ruby: s.count("a")
来源：http://ry.wgjwhj.cn

C#:   s.Count(c => c == 'a')
来源：http://vj.jctech888.com.cn

[E13] 逐字符遍历
来源：http://ra.szxytkj.cn

Py:   for ch in s: print(ch)
来源：http://jz.huixiangedu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xq.jianghongdianzi.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tk.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fr.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ep.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vw.szxytkj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://oo.huixinmuqiang.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zi.szsharing.cn

[E14] URL 编码与 Base64
来源：http://gx.colortex.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vr.jianghongdianzi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zv.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vk.jctech888.com.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ya.521024.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://np.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ve.lnxyls.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ir.yuntaijiaju.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bx.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://tf.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qw.huixinmuqiang.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jd.jctech888.com.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ly.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://tu.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ee.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://el.hnjuh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gc.szxytkj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hj.gzmigu.cn

[E16] 数字千分位
来源：http://cx.521024.cn

Py:   f"{1234567:,}"
来源：http://fu.asd995.cn

PHP:  number_format(1234567);
来源：http://xt.bookmarksfly.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://be.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tu.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qa.chemitech.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yr.hnjuh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ui.muxihuayi.cn

C#:   1234567.ToString("N0")
来源：http://lr.asd995.cn

[E17] 首字母大写
来源：http://fe.bookmarksfly.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yf.yuntaijiaju.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mq.yuntaijiaju.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yw.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sz.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oq.panjiajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ho.huanxung.cn

Ruby: s.capitalize
来源：http://ro.szsharing.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sm.hahajie.cn

[E18] 模板占位符替换
来源：http://ad.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zx.nszjky.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ka.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wy.shtwfgs.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mn.wgjwhj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kk.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gv.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ty.jianghongdianzi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uu.panjiajie.cn

[E19] 多行文本按行拆分
来源：http://lm.huanxung.cn

Py:   s.splitlines()
来源：http://zw.shxzskj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oe.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://zc.huixiangedu.cn

TS:   s.split(/\r?\n/)
来源：http://bd.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://hz.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://xm.szsharing.cn

Ruby: s.lines
来源：http://vq.jctech888.com.cn

C#:   s.Split('\n')
来源：http://mt.jianghongdianzi.cn

[E20] 判断字符串是否为空
来源：http://vw.haigaiapp.cn

Py:   if not s:
来源：http://vz.nicolike.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bd.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yn.haigaiapp.cn

TS:   if (s === "") {}
来源：http://rp.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://xs.yuexingan06.cn

Go:   if s == "" {}
来源：http://pc.hnjuh.cn

Ruby: if s.empty?
来源：http://mi.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ur.shxzukj.cn

[E21] 超长截断加省略号
来源：http://ty.yuexingan06.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ho.newstarts.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bb.colortex.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mw.panjiajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://og.chemitech.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lx.bookmarksfly.cn

Go:   // 按 rune 判断长度后截断
来源：http://xm.muxihuayi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pm.szsharing.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ql.yuexingan06.cn

[E22] 字节长度与字符长度
来源：http://gu.hahajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ss.huixinmuqiang.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tq.jianghongdianzi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pt.muxihuayi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://kr.bookmarksfly.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yc.bjjhwx.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tp.panjiajie.cn

Ruby: s.bytesize;  s.length
来源：http://wj.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lk.asd995.cn

================================================================================
来源：http://bw.huixinmuqiang.cn

F. 文件与目录
来源：http://nm.chemitech.net.cn

================================================================================
来源：http://xd.521024.cn

[F01] 读取整个文件
来源：http://kw.muxihuayi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dy.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://br.asd995.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://im.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://co.jianghongdianzi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yr.nicolike.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://uc.shxzskj.cn

Ruby: File.read("a.txt")
来源：http://ha.yuntaijiaju.cn

C#:   File.ReadAllText("a.txt");
来源：http://hk.colortex.cn

[F02] 逐行读取文件
来源：http://oq.asd995.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cq.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://en.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cv.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rj.haigaiapp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yc.nszjky.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jy.asd995.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rk.shxzskj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pj.bjjhwx.cn

[F03] 写入文件（覆盖）
来源：http://md.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ka.gzmigu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lk.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ro.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dy.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ol.panjiajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vm.hnjuh.cn

Ruby: File.write("a.txt", "hi")
来源：http://ao.newstarts.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gj.szxytkj.cn

[F04] 追加写入文件
来源：http://qf.newstarts.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://lc.szxytkj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xn.szxytkj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xc.shtwfgs.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yv.521024.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://an.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tj.szxytkj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xg.shtwfgs.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bi.newstarts.cn

[F05] 判断文件或目录是否存在
来源：http://fp.jctech888.com.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uu.colortex.cn

PHP:  file_exists("a.txt");
来源：http://vn.panjiajie.cn

JS:   fs.existsSync("a.txt")
来源：http://wi.muxihuayi.cn

TS:   fs.existsSync("a.txt")
来源：http://ok.huanxung.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hc.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zv.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://vo.9csxet.cn

C#:   File.Exists("a.txt")
来源：http://ef.nszjky.cn

[F06] 删除文件
来源：http://qu.nszjky.cn

Py:   os.remove("a.txt")
来源：http://wz.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://js.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cu.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://th.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ep.jianghongdianzi.cn

Go:   os.Remove("a.txt")
来源：http://eb.nszjky.cn

Ruby: File.delete("a.txt")
来源：http://ca.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://tz.asd995.cn

[F07] 创建目录（含多级）
来源：http://nf.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tp.bjjhwx.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jj.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vn.hnjuh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xi.huanxung.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zv.haigaiapp.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vt.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vv.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://de.chemitech.net.cn

[F08] 遍历目录
来源：http://eu.panjiajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://um.wgjwhj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ug.bookmarksfly.cn

JS:   fs.readdirSync("dir")
来源：http://kk.szxytkj.cn

TS:   fs.readdirSync("dir")
来源：http://ed.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mi.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ud.huixinmuqiang.cn

Ruby: Dir.children("dir")
来源：http://rg.newstarts.cn

C#:   Directory.GetFiles("dir")
来源：http://ty.hnjuh.cn

[F09] 获取文件大小
来源：http://lb.nicolike.cn

Py:   os.path.getsize("a.txt")
来源：http://si.jianghongdianzi.cn

PHP:  filesize("a.txt");
来源：http://ag.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://nf.szsharing.cn

TS:   fs.statSync("a.txt").size
来源：http://km.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tq.hahajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tx.jctech888.com.cn

Ruby: File.size("a.txt")
来源：http://ty.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://hv.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://or.gzmigu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tc.wgjwhj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ke.bookmarksfly.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://oa.hnjuh.cn

TS:   path.extname("a.txt")
来源：http://lv.nszjky.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mn.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zx.asd995.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mg.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pp.panjiajie.cn

[F11] 复制与移动文件
来源：http://vu.521024.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jv.yuexingan06.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://je.hahajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yj.jianghongdianzi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.haigaiapp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ig.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yy.jctech888.com.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://nw.szsharing.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eo.yuntaijiaju.cn

[F12] CSV 读写
来源：http://cm.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cp.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qu.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oh.muxihuayi.cn

TS:   // 同上
来源：http://xx.huixinmuqiang.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qy.lnxyls.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ag.bookmarksfly.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ut.szxytkj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zt.chemitech.net.cn

================================================================================
来源：http://fm.newstarts.cn

G. 面向对象
来源：http://yz.9csxet.cn

================================================================================
来源：http://jv.jctech888.com.cn

[G01] 定义类
来源：http://wd.shxzskj.cn

Py:   class User: pass
来源：http://rl.haigaiapp.cn

PHP:  class User {}
来源：http://vy.colortex.cn

JS:   class User {}
来源：http://ax.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://cx.nszjky.cn

Java: class User {}
来源：http://je.jianghongdianzi.cn

Go:   type User struct { Name string }
来源：http://eg.nicolike.cn

Ruby: class User; end
来源：http://ho.haigaiapp.cn

C#:   class User {}
来源：http://yi.haigaiapp.cn

[G02] 构造函数
来源：http://js.panjiajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://yq.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://lp.hnjuh.cn

JS:   constructor(name) { this.name = name; }
来源：http://sq.shxzukj.cn

TS:   constructor(public name: string) {}
来源：http://wb.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://qb.shxzukj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://np.shtwfgs.cn

Ruby: def initialize(name); @name = name; end
来源：http://un.huixinmuqiang.cn

C#:   public User(string name) { Name = name; }
来源：http://lv.muxihuayi.cn

[G03] 实例属性
来源：http://jr.bookmarksfly.cn

Py:   self.name = "x"
来源：http://sh.newstarts.cn

PHP:  public string $name = "x";
来源：http://fm.9csxet.cn


<!-- 参考信息 -->