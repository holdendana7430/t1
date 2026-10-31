代发 wailian999

Go:   strings.Join(items, ",")
来源：http://we.9csxet.cn

Ruby: items.join(",")
来源：http://wf.shxzskj.cn

C#:   string.Join(",", items)
来源：http://hf.9csxet.cn

[E09] 去除所有空白字符
来源：http://ep.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dm.hahajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ke.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://wp.hnjuh.cn

TS:   s.replace(/\s+/g, "")
来源：http://us.bookmarksfly.cn

Java: s.replaceAll("\\s+", "")
来源：http://ok.hahajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qg.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hl.huixiangedu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bx.szsharing.cn

[E10] 左侧补零 / 定长填充
来源：http://jb.chemitech.net.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bk.yuntaijiaju.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zr.gzmigu.cn

JS:   "7".padStart(3, "0")
来源：http://wq.newstarts.cn

TS:   "7".padStart(3, "0")
来源：http://eb.hnjuh.cn

Java: String.format("%03d", 7)
来源：http://tg.haigaiapp.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cs.huanxung.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://if.bjjhwx.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yt.jianghongdianzi.cn

[E11] 反转字符串
来源：http://op.9csxet.cn

Py:   s[::-1]
来源：http://uf.gzmigu.cn

PHP:  strrev($s);
来源：http://hc.wgjwhj.cn

JS:   [...s].reverse().join("")
来源：http://hw.asd995.cn

TS:   [...s].reverse().join("")
来源：http://yc.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jg.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qa.yuntaijiaju.cn

Ruby: s.reverse
来源：http://uz.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://aw.newstarts.cn

[E12] 统计某字符出现次数
来源：http://cu.lnxyls.cn

Py:   s.count("a")
来源：http://ck.yuntaijiaju.cn

PHP:  substr_count($s, "a");
来源：http://qt.shxzskj.cn

JS:   s.split("a").length - 1
来源：http://vm.muxihuayi.cn

TS:   s.split("a").length - 1
来源：http://oz.huixinmuqiang.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://pp.shxzukj.cn

Go:   strings.Count(s, "a")
来源：http://do.jianghongdianzi.cn

Ruby: s.count("a")
来源：http://th.colortex.cn

C#:   s.Count(c => c == 'a')
来源：http://ph.wgjwhj.cn

[E13] 逐字符遍历
来源：http://us.szxytkj.cn

Py:   for ch in s: print(ch)
来源：http://ei.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ff.nicolike.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://iq.lnxyls.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pl.shxzskj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sg.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://do.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rj.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ey.jianghongdianzi.cn

[E14] URL 编码与 Base64
来源：http://hg.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://rg.hahajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cc.asd995.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://un.yuexingan06.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sc.521024.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vc.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://cl.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hk.newstarts.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://tk.bjjhwx.cn

[E15] HTML 转义 / 反转义
来源：http://rh.yuntaijiaju.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jt.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vb.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ie.shxzukj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yq.shtwfgs.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fh.jctech888.com.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ir.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jf.muxihuayi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jq.nszjky.cn

[E16] 数字千分位
来源：http://tf.asd995.cn

Py:   f"{1234567:,}"
来源：http://fj.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://yv.wgjwhj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vq.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://iz.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ws.bookmarksfly.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yz.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vy.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://wo.asd995.cn

[E17] 首字母大写
来源：http://kg.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ne.jianghongdianzi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hb.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gc.bookmarksfly.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jw.shxzskj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oe.chemitech.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://du.shxzskj.cn

Ruby: s.capitalize
来源：http://zz.yuntaijiaju.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://oy.hahajie.cn

[E18] 模板占位符替换
来源：http://en.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://re.chemitech.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://av.hahajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xz.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fu.hnjuh.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://re.9csxet.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jf.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pl.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dp.bjjhwx.cn

[E19] 多行文本按行拆分
来源：http://ul.chemitech.net.cn

Py:   s.splitlines()
来源：http://wv.hnjuh.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ao.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://zn.521024.cn

TS:   s.split(/\r?\n/)
来源：http://pd.bookmarksfly.cn

Java: s.lines().toList()
来源：http://zm.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://um.huixinmuqiang.cn

Ruby: s.lines
来源：http://lw.huixinmuqiang.cn

C#:   s.Split('\n')
来源：http://ai.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://cc.muxihuayi.cn

Py:   if not s:
来源：http://rc.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uw.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hc.9csxet.cn

TS:   if (s === "") {}
来源：http://ue.hnjuh.cn

Java: if (s.isEmpty()) {}
来源：http://wb.huanxung.cn

Go:   if s == "" {}
来源：http://dy.lnxyls.cn

Ruby: if s.empty?
来源：http://zh.bjjhwx.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://up.nicolike.cn

[E21] 超长截断加省略号
来源：http://qg.nicolike.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wp.newstarts.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zy.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cw.colortex.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pc.yuexingan06.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oz.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://rj.szsharing.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tu.yuexingan06.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cg.gzmigu.cn

[E22] 字节长度与字符长度
来源：http://cd.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zb.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hj.yuntaijiaju.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ue.colortex.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uv.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ql.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ji.521024.cn

Ruby: s.bytesize;  s.length
来源：http://ua.newstarts.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hc.chemitech.net.cn

================================================================================
来源：http://xs.huixinmuqiang.cn

F. 文件与目录
来源：http://ga.asd995.cn

================================================================================
来源：http://wt.yuexingan06.cn

[F01] 读取整个文件
来源：http://zv.bjjhwx.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tw.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://ld.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://sa.hnjuh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zm.bjjhwx.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xo.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://sx.colortex.cn

Ruby: File.read("a.txt")
来源：http://xn.jctech888.com.cn

C#:   File.ReadAllText("a.txt");
来源：http://lh.shtwfgs.cn

[F02] 逐行读取文件
来源：http://gq.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xy.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rj.panjiajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lp.bjjhwx.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hy.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ow.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xo.shxzukj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yf.colortex.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gu.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://bz.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pf.shxzukj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://eu.bookmarksfly.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ej.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wk.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xe.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ys.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://xs.nszjky.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qf.panjiajie.cn

[F04] 追加写入文件
来源：http://ik.chemitech.net.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fa.muxihuayi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yd.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ya.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oo.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zj.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dj.nicolike.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cx.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lx.huanxung.cn

[F05] 判断文件或目录是否存在
来源：http://dx.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ce.lnxyls.cn

PHP:  file_exists("a.txt");
来源：http://dy.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://mf.huanxung.cn

TS:   fs.existsSync("a.txt")
来源：http://sh.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://uq.bookmarksfly.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cc.jctech888.com.cn

Ruby: File.exist?("a.txt")
来源：http://op.bjjhwx.cn

C#:   File.Exists("a.txt")
来源：http://rc.521024.cn

[F06] 删除文件
来源：http://qk.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://oh.jctech888.com.cn

PHP:  unlink("a.txt");
来源：http://rk.hnjuh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ta.muxihuayi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uq.newstarts.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ab.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://jp.colortex.cn

Ruby: File.delete("a.txt")
来源：http://xv.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://ke.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://iv.shxzukj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tl.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sm.szxytkj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://to.colortex.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mv.hnjuh.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://cj.yuntaijiaju.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ux.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dx.shxzskj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tp.huixiangedu.cn

[F08] 遍历目录
来源：http://bd.jctech888.com.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qc.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://au.muxihuayi.cn

JS:   fs.readdirSync("dir")
来源：http://il.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://pe.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dr.hahajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bk.huixiangedu.cn

Ruby: Dir.children("dir")
来源：http://zw.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://co.szsharing.cn

[F09] 获取文件大小
来源：http://ui.yuntaijiaju.cn

Py:   os.path.getsize("a.txt")
来源：http://ho.huixinmuqiang.cn

PHP:  filesize("a.txt");
来源：http://kp.gzmigu.cn

JS:   fs.statSync("a.txt").size
来源：http://km.chemitech.net.cn

TS:   fs.statSync("a.txt").size
来源：http://yd.bookmarksfly.cn

Java: Files.size(Path.of("a.txt"))
来源：http://eb.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kp.nszjky.cn

Ruby: File.size("a.txt")
来源：http://iw.panjiajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://jf.colortex.cn

[F10] 取文件扩展名 / 文件名
来源：http://pb.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ts.jctech888.com.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ig.shtwfgs.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rr.hnjuh.cn

TS:   path.extname("a.txt")
来源：http://dc.jianghongdianzi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kk.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ov.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kw.szxytkj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wm.huanxung.cn

[F11] 复制与移动文件
来源：http://dy.lnxyls.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ll.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ky.colortex.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qe.gzmigu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yn.haigaiapp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hk.huanxung.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fe.gzmigu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ru.shtwfgs.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://to.521024.cn

[F12] CSV 读写
来源：http://aj.panjiajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cv.huanxung.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gr.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xh.haigaiapp.cn

TS:   // 同上
来源：http://qb.yuexingan06.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cn.jianghongdianzi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hd.haigaiapp.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lm.jctech888.com.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dx.shxzskj.cn

================================================================================
来源：http://vk.bookmarksfly.cn

G. 面向对象
来源：http://sd.bookmarksfly.cn

================================================================================
来源：http://ws.lnxyls.cn

[G01] 定义类
来源：http://ig.huixinmuqiang.cn

Py:   class User: pass
来源：http://oz.521024.cn

PHP:  class User {}
来源：http://zt.bjjhwx.cn

JS:   class User {}
来源：http://wo.shtwfgs.cn

TS:   class User { name: string = ""; }
来源：http://li.shxzukj.cn

Java: class User {}
来源：http://fp.9csxet.cn

Go:   type User struct { Name string }
来源：http://az.szxytkj.cn

Ruby: class User; end
来源：http://kl.colortex.cn

C#:   class User {}
来源：http://wh.9csxet.cn

[G02] 构造函数
来源：http://ao.521024.cn

Py:   def __init__(self, name): self.name = name
来源：http://tc.9csxet.cn

PHP:  public function __construct(public string $name) {}
来源：http://zh.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://wr.nicolike.cn

TS:   constructor(public name: string) {}
来源：http://gl.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://sl.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jb.nicolike.cn

Ruby: def initialize(name); @name = name; end
来源：http://mj.9csxet.cn

C#:   public User(string name) { Name = name; }
来源：http://nz.521024.cn

[G03] 实例属性
来源：http://qm.9csxet.cn

Py:   self.name = "x"
来源：http://do.colortex.cn

PHP:  public string $name = "x";
来源：http://zh.wgjwhj.cn

JS:   this.name = "x";
来源：http://az.bjjhwx.cn

TS:   name: string = "x";
来源：http://zl.szsharing.cn

Java: private String name;
来源：http://zl.yuexingan06.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rp.yuexingan06.cn

Ruby: @name = "x"
来源：http://qc.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://ft.gzmigu.cn

[G04] 定义方法
来源：http://dk.huanxung.cn

Py:   def greet(self): return self.name
来源：http://ve.huixinmuqiang.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jo.shxzukj.cn

JS:   greet() { return this.name; }
来源：http://oy.szsharing.cn

TS:   greet(): string { return this.name; }
来源：http://zi.shxzukj.cn

Java: String greet() { return name; }
来源：http://nv.yuntaijiaju.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yq.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://bx.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://tc.panjiajie.cn

[G05] 继承
来源：http://tk.yuntaijiaju.cn

Py:   class Admin(User): pass
来源：http://hq.jianghongdianzi.cn

PHP:  class Admin extends User {}
来源：http://fs.shxzskj.cn

JS:   class Admin extends User {}
来源：http://zg.shtwfgs.cn

TS:   class Admin extends User {}
来源：http://ad.gzmigu.cn

Java: class Admin extends User {}
来源：http://xi.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://go.wgjwhj.cn

Ruby: class Admin < User; end
来源：http://qf.jianghongdianzi.cn

C#:   class Admin : User {}
来源：http://ar.521024.cn

[G06] 重写方法
来源：http://he.huixiangedu.cn

Py:   def greet(self): return "admin"
来源：http://jm.9csxet.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xn.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://ak.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://df.shxzskj.cn

Java: @Override String greet() { return "admin"; }
来源：http://ow.newstarts.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dy.yuexingan06.cn

Ruby: def greet; "admin"; end
来源：http://xw.chemitech.net.cn

C#:   public override string Greet() => "admin";
来源：http://ro.wgjwhj.cn

[G07] 调用父类方法
来源：http://cj.wgjwhj.cn

Py:   super().greet()
来源：http://do.muxihuayi.cn

PHP:  parent::greet();
来源：http://nz.yuntaijiaju.cn


<!-- 参考信息 -->