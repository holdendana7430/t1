代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://zz.jctech888.com.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://su.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wr.yuntaijiaju.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tl.yuexingan06.cn

C#:   s.Replace("a", "b")
来源：http://bn.bookmarksfly.cn

[E07] 按分隔符拆分
来源：http://er.bookmarksfly.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qn.chemitech.net.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vs.hnjuh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://nx.colortex.cn

TS:   s.split(",")
来源：http://lm.szxytkj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ef.panjiajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ri.huixiangedu.cn

Ruby: s.split(",");  s.split
来源：http://fz.asd995.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://yq.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://sw.nszjky.cn

Py:   ",".join(items)
来源：http://gs.huixinmuqiang.cn

PHP:  implode(",", $items);
来源：http://rj.huixiangedu.cn

JS:   items.join(",")
来源：http://cg.9csxet.cn

TS:   items.join(",")
来源：http://qt.shxzskj.cn

Java: String.join(",", items)
来源：http://md.haigaiapp.cn

Go:   strings.Join(items, ",")
来源：http://yc.wgjwhj.cn

Ruby: items.join(",")
来源：http://gk.shxzukj.cn

C#:   string.Join(",", items)
来源：http://yc.bjjhwx.cn

[E09] 去除所有空白字符
来源：http://mh.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://io.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ge.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://tz.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://yn.bjjhwx.cn

Java: s.replaceAll("\\s+", "")
来源：http://nl.newstarts.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tp.shxzskj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ai.muxihuayi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://si.newstarts.cn

[E10] 左侧补零 / 定长填充
来源：http://ay.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fg.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lu.shtwfgs.cn

JS:   "7".padStart(3, "0")
来源：http://is.chemitech.net.cn

TS:   "7".padStart(3, "0")
来源：http://hr.muxihuayi.cn

Java: String.format("%03d", 7)
来源：http://kd.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ho.wgjwhj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rs.haigaiapp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bf.wgjwhj.cn

[E11] 反转字符串
来源：http://zq.nszjky.cn

Py:   s[::-1]
来源：http://yw.hnjuh.cn

PHP:  strrev($s);
来源：http://ef.9csxet.cn

JS:   [...s].reverse().join("")
来源：http://rp.shtwfgs.cn

TS:   [...s].reverse().join("")
来源：http://ko.muxihuayi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jl.lnxyls.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://di.yuntaijiaju.cn

Ruby: s.reverse
来源：http://bj.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://de.yuntaijiaju.cn

[E12] 统计某字符出现次数
来源：http://uq.huanxung.cn

Py:   s.count("a")
来源：http://jd.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://ur.nszjky.cn

JS:   s.split("a").length - 1
来源：http://jw.szsharing.cn

TS:   s.split("a").length - 1
来源：http://bq.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kd.chemitech.net.cn

Go:   strings.Count(s, "a")
来源：http://np.yuexingan06.cn

Ruby: s.count("a")
来源：http://qm.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://mv.nszjky.cn

[E13] 逐字符遍历
来源：http://qw.asd995.cn

Py:   for ch in s: print(ch)
来源：http://ba.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mw.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dv.521024.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qg.9csxet.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ud.521024.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lx.9csxet.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qe.panjiajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xt.521024.cn

[E14] URL 编码与 Base64
来源：http://en.jctech888.com.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://yo.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ht.newstarts.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xx.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qv.huanxung.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wh.hnjuh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://se.nicolike.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://px.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://to.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://cu.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://hl.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://le.chemitech.net.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ue.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lf.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ev.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cj.wgjwhj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fh.newstarts.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uz.szsharing.cn

[E16] 数字千分位
来源：http://xv.newstarts.cn

Py:   f"{1234567:,}"
来源：http://bl.521024.cn

PHP:  number_format(1234567);
来源：http://ge.huixinmuqiang.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://sk.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gz.wgjwhj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yl.nszjky.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pt.bjjhwx.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ch.szxytkj.cn

C#:   1234567.ToString("N0")
来源：http://wq.huixinmuqiang.cn

[E17] 首字母大写
来源：http://zy.521024.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yq.haigaiapp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jk.huixinmuqiang.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ro.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nd.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ro.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qp.9csxet.cn

Ruby: s.capitalize
来源：http://xk.hnjuh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nd.nszjky.cn

[E18] 模板占位符替换
来源：http://qg.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://kk.szxytkj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bu.huixiangedu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://su.shxzukj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://tq.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mm.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dz.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ga.hnjuh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rf.muxihuayi.cn

[E19] 多行文本按行拆分
来源：http://lg.haigaiapp.cn

Py:   s.splitlines()
来源：http://bs.lnxyls.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ui.lnxyls.cn

JS:   s.split(/\r?\n/)
来源：http://qk.yuntaijiaju.cn

TS:   s.split(/\r?\n/)
来源：http://yr.shxzskj.cn

Java: s.lines().toList()
来源：http://qp.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://dr.lnxyls.cn

Ruby: s.lines
来源：http://ls.wgjwhj.cn

C#:   s.Split('\n')
来源：http://uq.asd995.cn

[E20] 判断字符串是否为空
来源：http://hk.nszjky.cn

Py:   if not s:
来源：http://dj.huixiangedu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pr.huixiangedu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://pg.chemitech.net.cn

TS:   if (s === "") {}
来源：http://aa.wgjwhj.cn

Java: if (s.isEmpty()) {}
来源：http://nt.huanxung.cn

Go:   if s == "" {}
来源：http://ir.bookmarksfly.cn

Ruby: if s.empty?
来源：http://au.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ao.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://ab.bjjhwx.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ph.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qa.9csxet.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hi.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dy.asd995.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lr.nicolike.cn

Go:   // 按 rune 判断长度后截断
来源：http://st.gzmigu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qa.newstarts.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://be.haigaiapp.cn

[E22] 字节长度与字符长度
来源：http://qb.haigaiapp.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ym.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ec.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fg.521024.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ql.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dz.521024.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ml.shxzskj.cn

Ruby: s.bytesize;  s.length
来源：http://yk.chemitech.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kt.huixiangedu.cn

================================================================================
来源：http://cy.hahajie.cn

F. 文件与目录
来源：http://em.szxytkj.cn

================================================================================
来源：http://xq.bjjhwx.cn

[F01] 读取整个文件
来源：http://dr.szxytkj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gp.9csxet.cn

PHP:  file_get_contents("a.txt");
来源：http://mc.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uk.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ye.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://bs.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mu.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://cd.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://dj.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://qh.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://lk.chemitech.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zo.wgjwhj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ni.jctech888.com.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ih.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ne.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xy.9csxet.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pl.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ze.lnxyls.cn

[F03] 写入文件（覆盖）
来源：http://ve.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vo.shxzukj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ra.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://th.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vd.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gp.shxzskj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hj.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://jg.yuexingan06.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ej.muxihuayi.cn

[F04] 追加写入文件
来源：http://fr.panjiajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kl.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xl.nicolike.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sw.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://we.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fn.szxytkj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://we.bookmarksfly.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jb.szxytkj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pi.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://pl.9csxet.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sk.asd995.cn

PHP:  file_exists("a.txt");
来源：http://ic.shtwfgs.cn

JS:   fs.existsSync("a.txt")
来源：http://vx.shxzskj.cn

TS:   fs.existsSync("a.txt")
来源：http://mj.jctech888.com.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://kx.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bc.gzmigu.cn

Ruby: File.exist?("a.txt")
来源：http://uy.panjiajie.cn

C#:   File.Exists("a.txt")
来源：http://ad.shxzskj.cn

[F06] 删除文件
来源：http://rf.haigaiapp.cn

Py:   os.remove("a.txt")
来源：http://bm.szxytkj.cn

PHP:  unlink("a.txt");
来源：http://zy.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://oq.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ra.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sl.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://ca.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://bo.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://ft.huanxung.cn

[F07] 创建目录（含多级）
来源：http://fe.szxytkj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bh.hnjuh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uo.jianghongdianzi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://de.gzmigu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://qy.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tq.huanxung.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ws.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://up.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uf.lnxyls.cn

[F08] 遍历目录
来源：http://js.9csxet.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ft.wgjwhj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://us.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://bb.shxzukj.cn

TS:   fs.readdirSync("dir")
来源：http://au.nicolike.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rx.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mj.shtwfgs.cn

Ruby: Dir.children("dir")
来源：http://ka.shxzskj.cn

C#:   Directory.GetFiles("dir")
来源：http://pa.bjjhwx.cn

[F09] 获取文件大小
来源：http://va.huanxung.cn

Py:   os.path.getsize("a.txt")
来源：http://av.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://dt.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://um.szxytkj.cn

TS:   fs.statSync("a.txt").size
来源：http://cm.jianghongdianzi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yy.lnxyls.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ch.colortex.cn

Ruby: File.size("a.txt")
来源：http://fa.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://wk.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://yl.yuntaijiaju.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ds.muxihuayi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yf.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sw.shxzukj.cn

TS:   path.extname("a.txt")
来源：http://jg.nszjky.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ag.bjjhwx.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zg.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hw.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://nv.nicolike.cn

[F11] 复制与移动文件
来源：http://jj.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bt.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://on.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bk.chemitech.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rt.szxytkj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hg.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://no.521024.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://iu.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yp.jianghongdianzi.cn

[F12] CSV 读写
来源：http://cg.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://du.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ay.bjjhwx.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bk.nicolike.cn

TS:   // 同上
来源：http://ml.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fa.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ji.bjjhwx.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qa.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://un.bookmarksfly.cn

================================================================================
来源：http://uj.chemitech.net.cn

G. 面向对象
来源：http://ml.wgjwhj.cn

================================================================================
来源：http://am.muxihuayi.cn

[G01] 定义类
来源：http://vk.shxzukj.cn

Py:   class User: pass
来源：http://kz.hahajie.cn

PHP:  class User {}
来源：http://gd.521024.cn

JS:   class User {}
来源：http://qx.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://fs.shxzskj.cn

Java: class User {}
来源：http://nd.hnjuh.cn

Go:   type User struct { Name string }
来源：http://vb.szxytkj.cn

Ruby: class User; end
来源：http://oy.nicolike.cn

C#:   class User {}
来源：http://hj.jctech888.com.cn

[G02] 构造函数
来源：http://ch.asd995.cn

Py:   def __init__(self, name): self.name = name
来源：http://ct.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://om.jctech888.com.cn

JS:   constructor(name) { this.name = name; }
来源：http://jd.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://xa.lnxyls.cn

Java: User(String name) { this.name = name; }
来源：http://xz.jianghongdianzi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://px.shxzukj.cn

Ruby: def initialize(name); @name = name; end
来源：http://iy.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://kx.bjjhwx.cn

[G03] 实例属性
来源：http://ia.hahajie.cn

Py:   self.name = "x"
来源：http://ht.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://ay.newstarts.cn

JS:   this.name = "x";
来源：http://bw.chemitech.net.cn

TS:   name: string = "x";
来源：http://ss.asd995.cn

Java: private String name;
来源：http://ct.asd995.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ac.huanxung.cn

Ruby: @name = "x"
来源：http://rv.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://js.bookmarksfly.cn

[G04] 定义方法
来源：http://bt.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://ar.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://el.chemitech.net.cn

JS:   greet() { return this.name; }
来源：http://wx.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://at.gzmigu.cn

Java: String greet() { return name; }
来源：http://xc.szsharing.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nc.newstarts.cn

Ruby: def greet; @name; end
来源：http://zf.yuntaijiaju.cn

C#:   public string Greet() => Name;
来源：http://yc.haigaiapp.cn

[G05] 继承
来源：http://bm.shxzskj.cn


<!-- 参考信息 -->