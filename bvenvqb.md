代发 wailian999

PHP:  implode(",", $items);
来源：http://mr.shxzukj.cn

JS:   items.join(",")
来源：http://ft.huanxung.cn

TS:   items.join(",")
来源：http://vu.nszjky.cn

Java: String.join(",", items)
来源：http://fz.gzmigu.cn

Go:   strings.Join(items, ",")
来源：http://ko.nicolike.cn

Ruby: items.join(",")
来源：http://cn.lnxyls.cn

C#:   string.Join(",", items)
来源：http://uz.wgjwhj.cn

[E09] 去除所有空白字符
来源：http://of.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ow.muxihuayi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://or.huixiangedu.cn

JS:   s.replace(/\s+/g, "")
来源：http://lu.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://rn.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://dw.jianghongdianzi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://vo.muxihuayi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://hu.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://el.yuntaijiaju.cn

[E10] 左侧补零 / 定长填充
来源：http://vp.haigaiapp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ts.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ec.nszjky.cn

JS:   "7".padStart(3, "0")
来源：http://nt.yuexingan06.cn

TS:   "7".padStart(3, "0")
来源：http://yp.lnxyls.cn

Java: String.format("%03d", 7)
来源：http://ov.lnxyls.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zb.gzmigu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://by.nszjky.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rf.shxzskj.cn

[E11] 反转字符串
来源：http://gs.szxytkj.cn

Py:   s[::-1]
来源：http://sh.asd995.cn

PHP:  strrev($s);
来源：http://qk.jianghongdianzi.cn

JS:   [...s].reverse().join("")
来源：http://lm.nszjky.cn

TS:   [...s].reverse().join("")
来源：http://kr.yuntaijiaju.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://iy.wgjwhj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wr.bookmarksfly.cn

Ruby: s.reverse
来源：http://jl.lnxyls.cn

C#:   new string(s.Reverse().ToArray())
来源：http://te.521024.cn

[E12] 统计某字符出现次数
来源：http://qt.bookmarksfly.cn

Py:   s.count("a")
来源：http://au.lnxyls.cn

PHP:  substr_count($s, "a");
来源：http://sq.bookmarksfly.cn

JS:   s.split("a").length - 1
来源：http://sj.shxzskj.cn

TS:   s.split("a").length - 1
来源：http://zb.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://oz.huixiangedu.cn

Go:   strings.Count(s, "a")
来源：http://ls.chemitech.net.cn

Ruby: s.count("a")
来源：http://sl.newstarts.cn

C#:   s.Count(c => c == 'a')
来源：http://re.shxzskj.cn

[E13] 逐字符遍历
来源：http://hs.jctech888.com.cn

Py:   for ch in s: print(ch)
来源：http://jz.chemitech.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://up.shxzskj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ry.wgjwhj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bq.9csxet.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ty.hahajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wv.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dk.haigaiapp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yv.nicolike.cn

[E14] URL 编码与 Base64
来源：http://wl.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://nr.hnjuh.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://us.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zo.shtwfgs.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zy.nicolike.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://at.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dn.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ek.jianghongdianzi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bp.colortex.cn

[E15] HTML 转义 / 反转义
来源：http://ej.nszjky.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://nv.wgjwhj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://kf.hnjuh.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pa.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zd.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gs.colortex.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rh.bookmarksfly.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ej.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cl.jianghongdianzi.cn

[E16] 数字千分位
来源：http://mb.haigaiapp.cn

Py:   f"{1234567:,}"
来源：http://io.huixiangedu.cn

PHP:  number_format(1234567);
来源：http://py.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ua.9csxet.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rg.hahajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://nr.9csxet.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xk.shxzukj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pb.hnjuh.cn

C#:   1234567.ToString("N0")
来源：http://zy.yuntaijiaju.cn

[E17] 首字母大写
来源：http://yw.jianghongdianzi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ne.newstarts.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://uw.shxzukj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hu.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rc.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gc.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ho.bookmarksfly.cn

Ruby: s.capitalize
来源：http://wf.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lo.newstarts.cn

[E18] 模板占位符替换
来源：http://gz.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cx.shtwfgs.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://tj.huixiangedu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zu.jianghongdianzi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://cz.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://fj.chemitech.net.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ss.bookmarksfly.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ex.haigaiapp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lb.nszjky.cn

[E19] 多行文本按行拆分
来源：http://sk.jctech888.com.cn

Py:   s.splitlines()
来源：http://qh.shxzskj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ce.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://gz.521024.cn

TS:   s.split(/\r?\n/)
来源：http://of.shxzukj.cn

Java: s.lines().toList()
来源：http://pv.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://yv.haigaiapp.cn

Ruby: s.lines
来源：http://rh.nszjky.cn

C#:   s.Split('\n')
来源：http://sx.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://vr.huixiangedu.cn

Py:   if not s:
来源：http://iz.bjjhwx.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://td.jianghongdianzi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://am.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://ua.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://ue.nicolike.cn

Go:   if s == "" {}
来源：http://tf.nicolike.cn

Ruby: if s.empty?
来源：http://mq.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ev.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://or.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iv.bjjhwx.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pq.panjiajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://da.shtwfgs.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jh.yuntaijiaju.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rv.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://yx.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ql.shxzukj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sy.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://ae.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xr.chemitech.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ue.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xl.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ta.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zb.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://et.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://cm.huanxung.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cq.asd995.cn

================================================================================
来源：http://yd.haigaiapp.cn

F. 文件与目录
来源：http://st.asd995.cn

================================================================================
来源：http://cc.gzmigu.cn

[F01] 读取整个文件
来源：http://fr.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kt.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://fp.haigaiapp.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qk.huixinmuqiang.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://xv.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rv.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pf.9csxet.cn

Ruby: File.read("a.txt")
来源：http://se.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://zl.shxzukj.cn

[F02] 逐行读取文件
来源：http://vs.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nu.wgjwhj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wg.wgjwhj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dk.yuexingan06.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pp.chemitech.net.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tk.shxzukj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vs.shxzukj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bx.nicolike.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sl.lnxyls.cn

[F03] 写入文件（覆盖）
来源：http://ta.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://av.huixiangedu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ra.shxzskj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ls.haigaiapp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fb.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jo.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fy.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://kd.huixiangedu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ri.huixiangedu.cn

[F04] 追加写入文件
来源：http://mi.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ol.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ko.gzmigu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wi.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ft.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ee.bookmarksfly.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vb.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wn.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kk.colortex.cn

[F05] 判断文件或目录是否存在
来源：http://eh.wgjwhj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pw.haigaiapp.cn

PHP:  file_exists("a.txt");
来源：http://rh.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://oe.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://ro.szxytkj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://by.newstarts.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xy.jctech888.com.cn

Ruby: File.exist?("a.txt")
来源：http://ss.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://nl.hnjuh.cn

[F06] 删除文件
来源：http://zy.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://ns.szsharing.cn

PHP:  unlink("a.txt");
来源：http://hs.shtwfgs.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gy.shtwfgs.cn

TS:   fs.unlinkSync("a.txt")
来源：http://iu.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kb.panjiajie.cn

Go:   os.Remove("a.txt")
来源：http://lk.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://fx.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://sc.lnxyls.cn

[F07] 创建目录（含多级）
来源：http://wv.huixiangedu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lc.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rr.hahajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mv.gzmigu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nj.newstarts.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://sm.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ep.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://df.nszjky.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://en.jctech888.com.cn

[F08] 遍历目录
来源：http://vd.nicolike.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://od.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pv.jianghongdianzi.cn

JS:   fs.readdirSync("dir")
来源：http://pf.hnjuh.cn

TS:   fs.readdirSync("dir")
来源：http://fr.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://it.jctech888.com.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rk.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://sm.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://lv.wgjwhj.cn

[F09] 获取文件大小
来源：http://ar.wgjwhj.cn

Py:   os.path.getsize("a.txt")
来源：http://hq.wgjwhj.cn

PHP:  filesize("a.txt");
来源：http://jt.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://tg.huixinmuqiang.cn

TS:   fs.statSync("a.txt").size
来源：http://ex.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ko.szxytkj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ah.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://lj.szxytkj.cn

C#:   new FileInfo("a.txt").Length
来源：http://dn.hnjuh.cn

[F10] 取文件扩展名 / 文件名
来源：http://ay.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kl.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vm.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://tg.yuexingan06.cn

TS:   path.extname("a.txt")
来源：http://bp.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xb.szxytkj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mh.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hb.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zo.9csxet.cn

[F11] 复制与移动文件
来源：http://tq.huanxung.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ra.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rp.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sd.wgjwhj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zu.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mq.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://od.huixinmuqiang.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://um.huixiangedu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mg.huanxung.cn

[F12] CSV 读写
来源：http://mt.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://th.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ct.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ac.muxihuayi.cn

TS:   // 同上
来源：http://ko.nszjky.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ds.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eb.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sz.bookmarksfly.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fr.chemitech.net.cn

================================================================================
来源：http://nb.521024.cn

G. 面向对象
来源：http://jc.muxihuayi.cn

================================================================================
来源：http://aq.yuexingan06.cn

[G01] 定义类
来源：http://wk.nszjky.cn

Py:   class User: pass
来源：http://qs.gzmigu.cn

PHP:  class User {}
来源：http://vi.shtwfgs.cn

JS:   class User {}
来源：http://zq.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://ap.shtwfgs.cn

Java: class User {}
来源：http://jx.shxzskj.cn

Go:   type User struct { Name string }
来源：http://es.szsharing.cn

Ruby: class User; end
来源：http://tq.9csxet.cn

C#:   class User {}
来源：http://id.jianghongdianzi.cn

[G02] 构造函数
来源：http://il.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://bx.muxihuayi.cn

PHP:  public function __construct(public string $name) {}
来源：http://at.hnjuh.cn

JS:   constructor(name) { this.name = name; }
来源：http://fq.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://cw.jctech888.com.cn

Java: User(String name) { this.name = name; }
来源：http://qc.lnxyls.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://am.bjjhwx.cn

Ruby: def initialize(name); @name = name; end
来源：http://px.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://kr.nszjky.cn

[G03] 实例属性
来源：http://xd.szxytkj.cn

Py:   self.name = "x"
来源：http://rw.nszjky.cn

PHP:  public string $name = "x";
来源：http://py.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://zm.szxytkj.cn

TS:   name: string = "x";
来源：http://ot.nicolike.cn

Java: private String name;
来源：http://df.haigaiapp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dz.chemitech.net.cn

Ruby: @name = "x"
来源：http://lp.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://ky.shtwfgs.cn

[G04] 定义方法
来源：http://mg.asd995.cn

Py:   def greet(self): return self.name
来源：http://vh.bjjhwx.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rx.colortex.cn

JS:   greet() { return this.name; }
来源：http://cg.huixinmuqiang.cn

TS:   greet(): string { return this.name; }
来源：http://ea.haigaiapp.cn

Java: String greet() { return name; }
来源：http://mm.gzmigu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cd.hahajie.cn

Ruby: def greet; @name; end
来源：http://aj.9csxet.cn

C#:   public string Greet() => Name;
来源：http://mz.szsharing.cn

[G05] 继承
来源：http://wd.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://do.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://bj.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://iq.jianghongdianzi.cn

TS:   class Admin extends User {}
来源：http://cc.asd995.cn

Java: class Admin extends User {}
来源：http://au.9csxet.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://um.hnjuh.cn

Ruby: class Admin < User; end
来源：http://uj.jianghongdianzi.cn

C#:   class Admin : User {}
来源：http://xn.haigaiapp.cn

[G06] 重写方法
来源：http://ot.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://oo.bjjhwx.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tz.huixinmuqiang.cn

JS:   greet() { return "admin"; }
来源：http://ud.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://we.wgjwhj.cn

Java: @Override String greet() { return "admin"; }
来源：http://bt.shxzukj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lt.hnjuh.cn

Ruby: def greet; "admin"; end
来源：http://sm.shxzukj.cn


<!-- 参考信息 -->