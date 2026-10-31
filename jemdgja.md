代发 wailian999

PHP:  implode(",", $items);
来源：http://gy.gzmigu.cn

JS:   items.join(",")
来源：http://cl.muxihuayi.cn

TS:   items.join(",")
来源：http://yd.muxihuayi.cn

Java: String.join(",", items)
来源：http://qs.9csxet.cn

Go:   strings.Join(items, ",")
来源：http://ib.shxzskj.cn

Ruby: items.join(",")
来源：http://qj.wgjwhj.cn

C#:   string.Join(",", items)
来源：http://lh.gzmigu.cn

[E09] 去除所有空白字符
来源：http://qr.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://uu.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wv.nszjky.cn

JS:   s.replace(/\s+/g, "")
来源：http://ab.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://yo.haigaiapp.cn

Java: s.replaceAll("\\s+", "")
来源：http://mz.chemitech.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wq.shxzukj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bm.haigaiapp.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pe.muxihuayi.cn

[E10] 左侧补零 / 定长填充
来源：http://lt.muxihuayi.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tx.haigaiapp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fl.muxihuayi.cn

JS:   "7".padStart(3, "0")
来源：http://fq.yuexingan06.cn

TS:   "7".padStart(3, "0")
来源：http://jz.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://vd.9csxet.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ci.wgjwhj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://kg.9csxet.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ql.colortex.cn

[E11] 反转字符串
来源：http://zr.wgjwhj.cn

Py:   s[::-1]
来源：http://tz.shxzukj.cn

PHP:  strrev($s);
来源：http://jm.bjjhwx.cn

JS:   [...s].reverse().join("")
来源：http://xn.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://td.szsharing.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://mz.521024.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ef.bjjhwx.cn

Ruby: s.reverse
来源：http://bp.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ao.nicolike.cn

[E12] 统计某字符出现次数
来源：http://ww.nicolike.cn

Py:   s.count("a")
来源：http://dl.yuexingan06.cn

PHP:  substr_count($s, "a");
来源：http://en.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://ch.huanxung.cn

TS:   s.split("a").length - 1
来源：http://ho.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fw.wgjwhj.cn

Go:   strings.Count(s, "a")
来源：http://yj.wgjwhj.cn

Ruby: s.count("a")
来源：http://ah.jctech888.com.cn

C#:   s.Count(c => c == 'a')
来源：http://bu.bjjhwx.cn

[E13] 逐字符遍历
来源：http://wt.haigaiapp.cn

Py:   for ch in s: print(ch)
来源：http://fv.huixinmuqiang.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://kb.szxytkj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ws.wgjwhj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vq.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wz.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zx.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ny.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hc.hahajie.cn

[E14] URL 编码与 Base64
来源：http://ty.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ob.bookmarksfly.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sy.bookmarksfly.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kp.gzmigu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wf.panjiajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yx.jianghongdianzi.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://xn.lnxyls.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ap.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bo.panjiajie.cn

[E15] HTML 转义 / 反转义
来源：http://eo.szsharing.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fw.haigaiapp.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://te.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uf.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://iq.yuntaijiaju.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ef.bookmarksfly.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lh.huixiangedu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://il.jianghongdianzi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jn.chemitech.net.cn

[E16] 数字千分位
来源：http://jk.jianghongdianzi.cn

Py:   f"{1234567:,}"
来源：http://yv.huanxung.cn

PHP:  number_format(1234567);
来源：http://gj.nicolike.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ao.nicolike.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bs.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://np.nicolike.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wd.hahajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zy.bjjhwx.cn

C#:   1234567.ToString("N0")
来源：http://zn.huanxung.cn

[E17] 首字母大写
来源：http://hc.huixinmuqiang.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oa.huanxung.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ty.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yh.gzmigu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://st.newstarts.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zd.chemitech.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vg.newstarts.cn

Ruby: s.capitalize
来源：http://bu.hahajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ye.jctech888.com.cn

[E18] 模板占位符替换
来源：http://do.bookmarksfly.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fp.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ko.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wt.nszjky.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pq.jianghongdianzi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ul.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nl.jianghongdianzi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.asd995.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ok.521024.cn

[E19] 多行文本按行拆分
来源：http://te.huixinmuqiang.cn

Py:   s.splitlines()
来源：http://ua.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://bq.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://uh.jctech888.com.cn

TS:   s.split(/\r?\n/)
来源：http://jc.9csxet.cn

Java: s.lines().toList()
来源：http://si.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://bj.shxzskj.cn

Ruby: s.lines
来源：http://li.colortex.cn

C#:   s.Split('\n')
来源：http://fj.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://hz.bookmarksfly.cn

Py:   if not s:
来源：http://ne.chemitech.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dv.521024.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://me.asd995.cn

TS:   if (s === "") {}
来源：http://lc.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://uh.panjiajie.cn

Go:   if s == "" {}
来源：http://tv.chemitech.net.cn

Ruby: if s.empty?
来源：http://ru.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tk.szsharing.cn

[E21] 超长截断加省略号
来源：http://nu.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hd.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tr.shxzukj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://oq.panjiajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vk.szxytkj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wr.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://xd.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dj.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://fc.panjiajie.cn

[E22] 字节长度与字符长度
来源：http://mh.hnjuh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bh.hnjuh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fq.gzmigu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dd.jctech888.com.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wf.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ln.huanxung.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oa.bjjhwx.cn

Ruby: s.bytesize;  s.length
来源：http://uo.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cu.shxzskj.cn

================================================================================
来源：http://de.huixinmuqiang.cn

F. 文件与目录
来源：http://so.gzmigu.cn

================================================================================
来源：http://xk.9csxet.cn

[F01] 读取整个文件
来源：http://fz.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rd.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://ho.haigaiapp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pb.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jk.lnxyls.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://kf.muxihuayi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jb.huanxung.cn

Ruby: File.read("a.txt")
来源：http://nq.jianghongdianzi.cn

C#:   File.ReadAllText("a.txt");
来源：http://wa.huixinmuqiang.cn

[F02] 逐行读取文件
来源：http://ir.colortex.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gk.hahajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ut.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ee.yuexingan06.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cx.haigaiapp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oz.521024.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sj.huanxung.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qn.asd995.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xo.szxytkj.cn

[F03] 写入文件（覆盖）
来源：http://ux.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nm.muxihuayi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ia.newstarts.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bt.jianghongdianzi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xr.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://qf.hahajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mr.shxzskj.cn

Ruby: File.write("a.txt", "hi")
来源：http://rw.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zz.szsharing.cn

[F04] 追加写入文件
来源：http://bz.bjjhwx.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pn.yuexingan06.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qw.wgjwhj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qy.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cw.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://om.szxytkj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://iy.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mr.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cw.szsharing.cn

[F05] 判断文件或目录是否存在
来源：http://gv.chemitech.net.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ld.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://lh.shxzukj.cn

JS:   fs.existsSync("a.txt")
来源：http://br.chemitech.net.cn

TS:   fs.existsSync("a.txt")
来源：http://ak.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sg.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://yx.chemitech.net.cn

Ruby: File.exist?("a.txt")
来源：http://bn.colortex.cn

C#:   File.Exists("a.txt")
来源：http://rt.huixiangedu.cn

[F06] 删除文件
来源：http://pg.szsharing.cn

Py:   os.remove("a.txt")
来源：http://bf.nicolike.cn

PHP:  unlink("a.txt");
来源：http://ej.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vk.szxytkj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gt.hahajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ic.newstarts.cn

Go:   os.Remove("a.txt")
来源：http://so.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://pe.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://hw.wgjwhj.cn

[F07] 创建目录（含多级）
来源：http://fq.huixinmuqiang.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pd.szxytkj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rm.yuexingan06.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xz.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fs.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wu.jianghongdianzi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jg.shtwfgs.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wi.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ce.jianghongdianzi.cn

[F08] 遍历目录
来源：http://il.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rp.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ko.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://sb.chemitech.net.cn

TS:   fs.readdirSync("dir")
来源：http://jk.nszjky.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ug.nszjky.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ob.jianghongdianzi.cn

Ruby: Dir.children("dir")
来源：http://mp.521024.cn

C#:   Directory.GetFiles("dir")
来源：http://ax.hahajie.cn

[F09] 获取文件大小
来源：http://ls.chemitech.net.cn

Py:   os.path.getsize("a.txt")
来源：http://hl.yuntaijiaju.cn

PHP:  filesize("a.txt");
来源：http://ip.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://cf.haigaiapp.cn

TS:   fs.statSync("a.txt").size
来源：http://im.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cj.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ym.shxzskj.cn

Ruby: File.size("a.txt")
来源：http://lg.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://fw.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://jz.521024.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oe.bjjhwx.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://np.szxytkj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ax.lnxyls.cn

TS:   path.extname("a.txt")
来源：http://bi.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jy.muxihuayi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yf.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ln.newstarts.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fn.chemitech.net.cn

[F11] 复制与移动文件
来源：http://ba.chemitech.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://kd.hnjuh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kq.szxytkj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://az.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sk.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nz.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nf.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gd.lnxyls.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pp.panjiajie.cn

[F12] CSV 读写
来源：http://jr.yuntaijiaju.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://bm.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qg.asd995.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://so.huanxung.cn

TS:   // 同上
来源：http://mo.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jm.chemitech.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bi.jianghongdianzi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uj.szxytkj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sm.shtwfgs.cn

================================================================================
来源：http://vn.nicolike.cn

G. 面向对象
来源：http://in.gzmigu.cn

================================================================================
来源：http://lo.nszjky.cn

[G01] 定义类
来源：http://mm.panjiajie.cn

Py:   class User: pass
来源：http://tl.szsharing.cn

PHP:  class User {}
来源：http://iq.gzmigu.cn

JS:   class User {}
来源：http://ly.gzmigu.cn

TS:   class User { name: string = ""; }
来源：http://tb.nszjky.cn

Java: class User {}
来源：http://to.colortex.cn

Go:   type User struct { Name string }
来源：http://ko.colortex.cn

Ruby: class User; end
来源：http://gp.chemitech.net.cn

C#:   class User {}
来源：http://bm.muxihuayi.cn

[G02] 构造函数
来源：http://bw.jctech888.com.cn

Py:   def __init__(self, name): self.name = name
来源：http://js.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://dm.panjiajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://pr.gzmigu.cn

TS:   constructor(public name: string) {}
来源：http://ah.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://mr.panjiajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bj.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://ul.huixiangedu.cn

C#:   public User(string name) { Name = name; }
来源：http://zs.huixinmuqiang.cn

[G03] 实例属性
来源：http://xd.nicolike.cn

Py:   self.name = "x"
来源：http://yx.bjjhwx.cn

PHP:  public string $name = "x";
来源：http://bo.9csxet.cn

JS:   this.name = "x";
来源：http://iq.yuexingan06.cn

TS:   name: string = "x";
来源：http://xr.9csxet.cn

Java: private String name;
来源：http://at.muxihuayi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rf.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://yc.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://ap.haigaiapp.cn

[G04] 定义方法
来源：http://yc.nicolike.cn

Py:   def greet(self): return self.name
来源：http://rd.huanxung.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dh.shxzukj.cn

JS:   greet() { return this.name; }
来源：http://av.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://fg.huixiangedu.cn

Java: String greet() { return name; }
来源：http://ic.bookmarksfly.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qi.9csxet.cn

Ruby: def greet; @name; end
来源：http://ib.huanxung.cn

C#:   public string Greet() => Name;
来源：http://pw.lnxyls.cn

[G05] 继承
来源：http://hx.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://oy.bjjhwx.cn

PHP:  class Admin extends User {}
来源：http://bz.gzmigu.cn

JS:   class Admin extends User {}
来源：http://an.wgjwhj.cn

TS:   class Admin extends User {}
来源：http://hp.szxytkj.cn

Java: class Admin extends User {}
来源：http://kn.huanxung.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yv.hnjuh.cn

Ruby: class Admin < User; end
来源：http://ek.lnxyls.cn

C#:   class Admin : User {}
来源：http://uu.yuntaijiaju.cn

[G06] 重写方法
来源：http://zp.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://hi.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ao.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://wb.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://so.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://gx.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hj.shxzskj.cn

Ruby: def greet; "admin"; end
来源：http://ly.shxzskj.cn


<!-- 参考信息 -->