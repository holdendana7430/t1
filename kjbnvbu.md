代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pw.asd995.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://vc.bookmarksfly.cn

JS:   s.replace(/\s+/g, "")
来源：http://ic.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://ce.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://wy.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dd.szsharing.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jz.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://gv.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://ol.hnjuh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://cn.lnxyls.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fk.huanxung.cn

JS:   "7".padStart(3, "0")
来源：http://az.shxzukj.cn

TS:   "7".padStart(3, "0")
来源：http://kg.colortex.cn

Java: String.format("%03d", 7)
来源：http://ne.lnxyls.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tr.chemitech.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ba.colortex.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://uh.asd995.cn

[E11] 反转字符串
来源：http://px.muxihuayi.cn

Py:   s[::-1]
来源：http://ze.gzmigu.cn

PHP:  strrev($s);
来源：http://tc.newstarts.cn

JS:   [...s].reverse().join("")
来源：http://pr.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://zm.nszjky.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://uf.hnjuh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://er.huixinmuqiang.cn

Ruby: s.reverse
来源：http://qw.9csxet.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ar.szsharing.cn

[E12] 统计某字符出现次数
来源：http://iv.lnxyls.cn

Py:   s.count("a")
来源：http://fv.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://ni.gzmigu.cn

JS:   s.split("a").length - 1
来源：http://ke.haigaiapp.cn

TS:   s.split("a").length - 1
来源：http://mq.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mc.szsharing.cn

Go:   strings.Count(s, "a")
来源：http://lk.muxihuayi.cn

Ruby: s.count("a")
来源：http://hh.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://rd.muxihuayi.cn

[E13] 逐字符遍历
来源：http://ck.nszjky.cn

Py:   for ch in s: print(ch)
来源：http://qp.szxytkj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gx.9csxet.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sm.wgjwhj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qo.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://in.chemitech.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yd.bookmarksfly.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ob.yuexingan06.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qn.wgjwhj.cn

[E14] URL 编码与 Base64
来源：http://tr.lnxyls.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://to.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dl.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yj.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xo.huixiangedu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dv.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://gu.hahajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fb.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://bu.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://gy.lnxyls.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jt.huanxung.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://dx.shxzskj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bf.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://dq.muxihuayi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hh.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hx.yuntaijiaju.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tm.haigaiapp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sy.521024.cn

[E16] 数字千分位
来源：http://uf.huixiangedu.cn

Py:   f"{1234567:,}"
来源：http://wp.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://ij.jianghongdianzi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rn.yuexingan06.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ct.lnxyls.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sg.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ew.huixiangedu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://qp.gzmigu.cn

C#:   1234567.ToString("N0")
来源：http://qz.jianghongdianzi.cn

[E17] 首字母大写
来源：http://jr.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nt.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://up.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nu.asd995.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zm.lnxyls.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jj.newstarts.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gq.asd995.cn

Ruby: s.capitalize
来源：http://ro.nszjky.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uu.bookmarksfly.cn

[E18] 模板占位符替换
来源：http://sb.szsharing.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fl.asd995.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://te.9csxet.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sm.haigaiapp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ad.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://br.asd995.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://rb.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dp.bjjhwx.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://tw.hnjuh.cn

[E19] 多行文本按行拆分
来源：http://wh.bjjhwx.cn

Py:   s.splitlines()
来源：http://vg.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wr.nszjky.cn

JS:   s.split(/\r?\n/)
来源：http://vm.lnxyls.cn

TS:   s.split(/\r?\n/)
来源：http://hy.muxihuayi.cn

Java: s.lines().toList()
来源：http://zw.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://um.yuntaijiaju.cn

Ruby: s.lines
来源：http://ed.shtwfgs.cn

C#:   s.Split('\n')
来源：http://ms.bjjhwx.cn

[E20] 判断字符串是否为空
来源：http://te.szxytkj.cn

Py:   if not s:
来源：http://cn.wgjwhj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://my.colortex.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mr.shtwfgs.cn

TS:   if (s === "") {}
来源：http://fx.gzmigu.cn

Java: if (s.isEmpty()) {}
来源：http://mc.shtwfgs.cn

Go:   if s == "" {}
来源：http://op.shxzukj.cn

Ruby: if s.empty?
来源：http://yq.nszjky.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gd.521024.cn

[E21] 超长截断加省略号
来源：http://ec.szxytkj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://dk.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ga.szsharing.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://aj.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kr.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fn.newstarts.cn

Go:   // 按 rune 判断长度后截断
来源：http://mz.yuntaijiaju.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gt.yuntaijiaju.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yd.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://om.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dp.hahajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ox.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wl.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ho.newstarts.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jf.chemitech.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sk.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://kp.huixiangedu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ij.shxzskj.cn

================================================================================
来源：http://dq.jianghongdianzi.cn

F. 文件与目录
来源：http://cp.shtwfgs.cn

================================================================================
来源：http://so.huixinmuqiang.cn

[F01] 读取整个文件
来源：http://pe.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dp.shtwfgs.cn

PHP:  file_get_contents("a.txt");
来源：http://vz.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gl.jctech888.com.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cv.jianghongdianzi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://gx.jianghongdianzi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://si.huixinmuqiang.cn

Ruby: File.read("a.txt")
来源：http://tt.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://dy.huixinmuqiang.cn

[F02] 逐行读取文件
来源：http://bw.muxihuayi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gy.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gx.lnxyls.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ze.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://uu.yuntaijiaju.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://os.haigaiapp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://za.nicolike.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ws.chemitech.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tv.yuexingan06.cn

[F03] 写入文件（覆盖）
来源：http://ry.chemitech.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://la.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jb.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://el.szsharing.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kr.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bu.9csxet.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://sl.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://ar.nszjky.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://aq.panjiajie.cn

[F04] 追加写入文件
来源：http://cf.huixinmuqiang.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ps.jctech888.com.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://js.gzmigu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kg.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://po.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vr.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wi.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qn.yuntaijiaju.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bn.chemitech.net.cn

[F05] 判断文件或目录是否存在
来源：http://sc.huixiangedu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nj.newstarts.cn

PHP:  file_exists("a.txt");
来源：http://zi.huixinmuqiang.cn

JS:   fs.existsSync("a.txt")
来源：http://wu.muxihuayi.cn

TS:   fs.existsSync("a.txt")
来源：http://rt.yuexingan06.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fd.jctech888.com.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ex.yuntaijiaju.cn

Ruby: File.exist?("a.txt")
来源：http://pt.asd995.cn

C#:   File.Exists("a.txt")
来源：http://ii.wgjwhj.cn

[F06] 删除文件
来源：http://np.muxihuayi.cn

Py:   os.remove("a.txt")
来源：http://cg.hnjuh.cn

PHP:  unlink("a.txt");
来源：http://bn.huanxung.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bs.bookmarksfly.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ds.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kq.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://zk.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://iq.yuexingan06.cn

C#:   File.Delete("a.txt");
来源：http://pe.colortex.cn

[F07] 创建目录（含多级）
来源：http://yb.gzmigu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://by.hnjuh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hd.hahajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dg.haigaiapp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://di.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ak.huanxung.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fw.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ee.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uw.hahajie.cn

[F08] 遍历目录
来源：http://vj.huixinmuqiang.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qv.nszjky.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://eg.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://wj.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://hy.nszjky.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tl.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jf.yuexingan06.cn

Ruby: Dir.children("dir")
来源：http://sh.521024.cn

C#:   Directory.GetFiles("dir")
来源：http://gg.colortex.cn

[F09] 获取文件大小
来源：http://ug.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://uk.chemitech.net.cn

PHP:  filesize("a.txt");
来源：http://ma.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://da.haigaiapp.cn

TS:   fs.statSync("a.txt").size
来源：http://ht.yuexingan06.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ae.gzmigu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gw.shxzukj.cn

Ruby: File.size("a.txt")
来源：http://sz.asd995.cn

C#:   new FileInfo("a.txt").Length
来源：http://cp.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://hm.521024.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://eq.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nz.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uc.wgjwhj.cn

TS:   path.extname("a.txt")
来源：http://tz.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://au.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ec.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ns.huanxung.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uw.yuntaijiaju.cn

[F11] 复制与移动文件
来源：http://bh.chemitech.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hx.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kh.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hq.9csxet.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wa.huixiangedu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://od.chemitech.net.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://dn.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hj.haigaiapp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nh.nicolike.cn

[F12] CSV 读写
来源：http://dm.yuntaijiaju.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lk.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uk.haigaiapp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ua.colortex.cn

TS:   // 同上
来源：http://dt.nszjky.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nz.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fy.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pk.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zg.wgjwhj.cn

================================================================================
来源：http://bn.nszjky.cn

G. 面向对象
来源：http://sl.asd995.cn

================================================================================
来源：http://nd.nicolike.cn

[G01] 定义类
来源：http://hq.bjjhwx.cn

Py:   class User: pass
来源：http://kf.shxzskj.cn

PHP:  class User {}
来源：http://lz.nszjky.cn

JS:   class User {}
来源：http://ob.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://cf.colortex.cn

Java: class User {}
来源：http://cd.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://ns.huixinmuqiang.cn

Ruby: class User; end
来源：http://js.yuexingan06.cn

C#:   class User {}
来源：http://zs.yuexingan06.cn

[G02] 构造函数
来源：http://pf.shxzukj.cn

Py:   def __init__(self, name): self.name = name
来源：http://vt.jianghongdianzi.cn

PHP:  public function __construct(public string $name) {}
来源：http://zh.shxzskj.cn

JS:   constructor(name) { this.name = name; }
来源：http://dz.asd995.cn

TS:   constructor(public name: string) {}
来源：http://rp.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://db.shxzukj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vr.9csxet.cn

Ruby: def initialize(name); @name = name; end
来源：http://iy.szxytkj.cn

C#:   public User(string name) { Name = name; }
来源：http://wf.wgjwhj.cn

[G03] 实例属性
来源：http://ac.hnjuh.cn

Py:   self.name = "x"
来源：http://ou.hahajie.cn

PHP:  public string $name = "x";
来源：http://fb.szxytkj.cn

JS:   this.name = "x";
来源：http://ww.huanxung.cn

TS:   name: string = "x";
来源：http://en.huanxung.cn

Java: private String name;
来源：http://uc.gzmigu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bx.hahajie.cn

Ruby: @name = "x"
来源：http://hf.bjjhwx.cn

C#:   public string Name { get; set; } = "x";
来源：http://ld.asd995.cn

[G04] 定义方法
来源：http://aq.nszjky.cn

Py:   def greet(self): return self.name
来源：http://xd.panjiajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ew.szxytkj.cn

JS:   greet() { return this.name; }
来源：http://if.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://dv.muxihuayi.cn

Java: String greet() { return name; }
来源：http://pu.hnjuh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nr.newstarts.cn

Ruby: def greet; @name; end
来源：http://rr.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://hi.newstarts.cn

[G05] 继承
来源：http://nm.yuntaijiaju.cn

Py:   class Admin(User): pass
来源：http://nr.huanxung.cn

PHP:  class Admin extends User {}
来源：http://lm.szxytkj.cn

JS:   class Admin extends User {}
来源：http://fz.wgjwhj.cn

TS:   class Admin extends User {}
来源：http://kq.asd995.cn

Java: class Admin extends User {}
来源：http://fh.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gc.9csxet.cn

Ruby: class Admin < User; end
来源：http://rl.muxihuayi.cn

C#:   class Admin : User {}
来源：http://sg.jctech888.com.cn

[G06] 重写方法
来源：http://tf.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://is.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jo.yuexingan06.cn

JS:   greet() { return "admin"; }
来源：http://zs.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://yk.nszjky.cn

Java: @Override String greet() { return "admin"; }
来源：http://nj.chemitech.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hu.muxihuayi.cn

Ruby: def greet; "admin"; end
来源：http://km.bjjhwx.cn

C#:   public override string Greet() => "admin";
来源：http://ht.muxihuayi.cn

[G07] 调用父类方法
来源：http://am.shxzukj.cn

Py:   super().greet()
来源：http://gp.huixiangedu.cn

PHP:  parent::greet();
来源：http://rb.jianghongdianzi.cn

JS:   super.greet();
来源：http://vi.jianghongdianzi.cn

TS:   super.greet();
来源：http://ae.colortex.cn

Java: super.greet();
来源：http://hu.bookmarksfly.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rn.bookmarksfly.cn


<!-- 参考信息 -->