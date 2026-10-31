代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://zj.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ry.nicolike.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ne.shtwfgs.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ut.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://np.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rd.panjiajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ai.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://rd.gzmigu.cn

TS:   "7".padStart(3, "0")
来源：http://od.shxzskj.cn

Java: String.format("%03d", 7)
来源：http://nc.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kh.jianghongdianzi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rg.yuntaijiaju.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pd.szsharing.cn

[E11] 反转字符串
来源：http://ny.panjiajie.cn

Py:   s[::-1]
来源：http://mu.bookmarksfly.cn

PHP:  strrev($s);
来源：http://yp.hnjuh.cn

JS:   [...s].reverse().join("")
来源：http://xz.521024.cn

TS:   [...s].reverse().join("")
来源：http://ge.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://cl.jianghongdianzi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://wj.jctech888.com.cn

Ruby: s.reverse
来源：http://ms.hnjuh.cn

C#:   new string(s.Reverse().ToArray())
来源：http://qi.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://mg.asd995.cn

Py:   s.count("a")
来源：http://no.gzmigu.cn

PHP:  substr_count($s, "a");
来源：http://dn.nszjky.cn

JS:   s.split("a").length - 1
来源：http://sq.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://hl.haigaiapp.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://uk.hahajie.cn

Go:   strings.Count(s, "a")
来源：http://qt.muxihuayi.cn

Ruby: s.count("a")
来源：http://ci.colortex.cn

C#:   s.Count(c => c == 'a')
来源：http://cd.yuntaijiaju.cn

[E13] 逐字符遍历
来源：http://ai.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://yx.bookmarksfly.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://km.bjjhwx.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hx.yuntaijiaju.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chemitech.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ek.panjiajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lh.jianghongdianzi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sg.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pz.colortex.cn

[E14] URL 编码与 Base64
来源：http://gl.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dy.colortex.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bj.shxzskj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ez.shxzukj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pb.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qy.haigaiapp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://fn.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nt.hahajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hf.shtwfgs.cn

[E15] HTML 转义 / 反转义
来源：http://ly.jctech888.com.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dh.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bb.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hw.shxzskj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://qa.nszjky.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://sh.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ns.9csxet.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hv.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kt.bookmarksfly.cn

[E16] 数字千分位
来源：http://ch.asd995.cn

Py:   f"{1234567:,}"
来源：http://pp.szxytkj.cn

PHP:  number_format(1234567);
来源：http://eq.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://lp.nicolike.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ro.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://iw.huanxung.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xw.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tj.yuntaijiaju.cn

C#:   1234567.ToString("N0")
来源：http://kl.muxihuayi.cn

[E17] 首字母大写
来源：http://od.gzmigu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vm.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://dk.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dc.muxihuayi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uy.nszjky.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ug.hahajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gy.bookmarksfly.cn

Ruby: s.capitalize
来源：http://vz.yuexingan06.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://kf.yuntaijiaju.cn

[E18] 模板占位符替换
来源：http://fm.muxihuayi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ht.521024.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yr.muxihuayi.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://en.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ql.nszjky.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zf.colortex.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dc.lnxyls.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hi.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mo.hnjuh.cn

[E19] 多行文本按行拆分
来源：http://ck.szsharing.cn

Py:   s.splitlines()
来源：http://oo.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://po.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://ut.jctech888.com.cn

TS:   s.split(/\r?\n/)
来源：http://eo.521024.cn

Java: s.lines().toList()
来源：http://ro.huanxung.cn

Go:   strings.Split(s, "\n")
来源：http://ch.haigaiapp.cn

Ruby: s.lines
来源：http://kk.nicolike.cn

C#:   s.Split('\n')
来源：http://eh.asd995.cn

[E20] 判断字符串是否为空
来源：http://bq.bookmarksfly.cn

Py:   if not s:
来源：http://zu.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xt.shxzskj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://lg.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://sv.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://pq.shxzukj.cn

Go:   if s == "" {}
来源：http://lg.szsharing.cn

Ruby: if s.empty?
来源：http://qy.hahajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://py.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://tx.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xj.szxytkj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mw.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ix.bjjhwx.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ua.bjjhwx.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nv.haigaiapp.cn

Go:   // 按 rune 判断长度后截断
来源：http://rs.jianghongdianzi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ng.panjiajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ds.nszjky.cn

[E22] 字节长度与字符长度
来源：http://vi.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ia.szsharing.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ja.hnjuh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ck.szxytkj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zz.huixinmuqiang.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gl.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tz.shxzukj.cn

Ruby: s.bytesize;  s.length
来源：http://wx.wgjwhj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pk.hahajie.cn

================================================================================
来源：http://vv.nszjky.cn

F. 文件与目录
来源：http://xa.9csxet.cn

================================================================================
来源：http://lp.9csxet.cn

[F01] 读取整个文件
来源：http://rt.jctech888.com.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rx.huixinmuqiang.cn

PHP:  file_get_contents("a.txt");
来源：http://xn.521024.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bv.jctech888.com.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fr.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pt.yuexingan06.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qu.lnxyls.cn

Ruby: File.read("a.txt")
来源：http://yl.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://vf.wgjwhj.cn

[F02] 逐行读取文件
来源：http://ub.gzmigu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cx.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zt.huixinmuqiang.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ed.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gr.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sq.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wd.szsharing.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oh.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://na.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://ny.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zo.yuexingan06.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nj.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yb.shxzukj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yx.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ju.shxzskj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jz.lnxyls.cn

Ruby: File.write("a.txt", "hi")
来源：http://wp.muxihuayi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mj.gzmigu.cn

[F04] 追加写入文件
来源：http://xh.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ec.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cg.huanxung.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ag.szxytkj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hw.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kj.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kp.nszjky.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://iy.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ul.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://bd.huixiangedu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://id.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://dk.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://yx.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://pr.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pl.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hf.521024.cn

Ruby: File.exist?("a.txt")
来源：http://yv.shxzskj.cn

C#:   File.Exists("a.txt")
来源：http://xa.jctech888.com.cn

[F06] 删除文件
来源：http://wh.chemitech.net.cn

Py:   os.remove("a.txt")
来源：http://fk.yuntaijiaju.cn

PHP:  unlink("a.txt");
来源：http://an.colortex.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qz.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mu.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sv.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://il.lnxyls.cn

Ruby: File.delete("a.txt")
来源：http://xj.szsharing.cn

C#:   File.Delete("a.txt");
来源：http://us.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://rc.wgjwhj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jc.wgjwhj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rr.chemitech.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gh.shxzukj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xp.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wz.yuexingan06.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vg.huixiangedu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://px.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pz.haigaiapp.cn

[F08] 遍历目录
来源：http://mi.huanxung.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dp.shtwfgs.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://de.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://tt.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://av.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gw.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vs.chemitech.net.cn

Ruby: Dir.children("dir")
来源：http://ku.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://jg.haigaiapp.cn

[F09] 获取文件大小
来源：http://za.haigaiapp.cn

Py:   os.path.getsize("a.txt")
来源：http://ey.huixinmuqiang.cn

PHP:  filesize("a.txt");
来源：http://ag.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://ai.yuexingan06.cn

TS:   fs.statSync("a.txt").size
来源：http://qi.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lc.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tr.521024.cn

Ruby: File.size("a.txt")
来源：http://fq.chemitech.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://bk.huixinmuqiang.cn

[F10] 取文件扩展名 / 文件名
来源：http://mo.huanxung.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kn.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zp.hahajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ee.newstarts.cn

TS:   path.extname("a.txt")
来源：http://io.huixinmuqiang.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lo.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pq.9csxet.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lp.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ij.huanxung.cn

[F11] 复制与移动文件
来源：http://lp.lnxyls.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wu.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gn.muxihuayi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eb.nicolike.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pj.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ln.szxytkj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ql.szsharing.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ng.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zn.shtwfgs.cn

[F12] CSV 读写
来源：http://fd.shxzskj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vn.chemitech.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ra.newstarts.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bk.hahajie.cn

TS:   // 同上
来源：http://xa.huanxung.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rp.huanxung.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pg.gzmigu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sy.szxytkj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ls.gzmigu.cn

================================================================================
来源：http://rz.hahajie.cn

G. 面向对象
来源：http://mb.9csxet.cn

================================================================================
来源：http://px.shtwfgs.cn

[G01] 定义类
来源：http://kj.yuntaijiaju.cn

Py:   class User: pass
来源：http://el.panjiajie.cn

PHP:  class User {}
来源：http://my.colortex.cn

JS:   class User {}
来源：http://oy.hnjuh.cn

TS:   class User { name: string = ""; }
来源：http://lf.nszjky.cn

Java: class User {}
来源：http://pf.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://jz.lnxyls.cn

Ruby: class User; end
来源：http://dy.shxzskj.cn

C#:   class User {}
来源：http://ev.shxzskj.cn

[G02] 构造函数
来源：http://km.521024.cn

Py:   def __init__(self, name): self.name = name
来源：http://fo.9csxet.cn

PHP:  public function __construct(public string $name) {}
来源：http://hd.wgjwhj.cn

JS:   constructor(name) { this.name = name; }
来源：http://hs.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://gu.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://dj.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mk.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://fq.shtwfgs.cn

C#:   public User(string name) { Name = name; }
来源：http://en.yuexingan06.cn

[G03] 实例属性
来源：http://um.9csxet.cn

Py:   self.name = "x"
来源：http://ch.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://pg.bookmarksfly.cn

JS:   this.name = "x";
来源：http://fa.9csxet.cn

TS:   name: string = "x";
来源：http://sx.szxytkj.cn

Java: private String name;
来源：http://ua.hnjuh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://au.gzmigu.cn

Ruby: @name = "x"
来源：http://gd.9csxet.cn

C#:   public string Name { get; set; } = "x";
来源：http://vj.shxzskj.cn

[G04] 定义方法
来源：http://ki.nicolike.cn

Py:   def greet(self): return self.name
来源：http://bz.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pj.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://fi.newstarts.cn

TS:   greet(): string { return this.name; }
来源：http://hs.gzmigu.cn

Java: String greet() { return name; }
来源：http://zx.521024.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nu.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://gu.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://wo.hahajie.cn

[G05] 继承
来源：http://oh.lnxyls.cn

Py:   class Admin(User): pass
来源：http://cp.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://tw.hnjuh.cn

JS:   class Admin extends User {}
来源：http://dr.huixinmuqiang.cn

TS:   class Admin extends User {}
来源：http://th.bjjhwx.cn

Java: class Admin extends User {}
来源：http://qt.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zd.hahajie.cn

Ruby: class Admin < User; end
来源：http://ps.colortex.cn

C#:   class Admin : User {}
来源：http://fh.bookmarksfly.cn

[G06] 重写方法
来源：http://ax.bookmarksfly.cn

Py:   def greet(self): return "admin"
来源：http://ih.muxihuayi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lz.wgjwhj.cn

JS:   greet() { return "admin"; }
来源：http://az.shxzukj.cn

TS:   greet(): string { return "admin"; }
来源：http://uf.shxzskj.cn

Java: @Override String greet() { return "admin"; }
来源：http://cj.shxzskj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ym.asd995.cn

Ruby: def greet; "admin"; end
来源：http://dr.shtwfgs.cn

C#:   public override string Greet() => "admin";
来源：http://ta.bjjhwx.cn

[G07] 调用父类方法
来源：http://dc.gzmigu.cn

Py:   super().greet()
来源：http://jw.bjjhwx.cn

PHP:  parent::greet();
来源：http://es.shxzukj.cn

JS:   super.greet();
来源：http://mz.9csxet.cn

TS:   super.greet();
来源：http://kj.nszjky.cn

Java: super.greet();
来源：http://dh.huixiangedu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xy.newstarts.cn

Ruby: super
来源：http://ku.bjjhwx.cn

C#:   base.Greet();
来源：http://mm.szsharing.cn

[G08] 静态方法与属性
来源：http://jv.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xc.chemitech.net.cn


<!-- 参考信息 -->