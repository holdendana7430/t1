代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://ic.newstarts.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ht.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bf.lnxyls.cn

JS:   "7".padStart(3, "0")
来源：http://gi.colortex.cn

TS:   "7".padStart(3, "0")
来源：http://ys.nicolike.cn

Java: String.format("%03d", 7)
来源：http://ix.521024.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mb.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yw.huixiangedu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cc.lnxyls.cn

[E11] 反转字符串
来源：http://fq.haigaiapp.cn

Py:   s[::-1]
来源：http://vu.hahajie.cn

PHP:  strrev($s);
来源：http://oe.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://vn.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://oz.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pr.gzmigu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ag.nszjky.cn

Ruby: s.reverse
来源：http://cg.bookmarksfly.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jb.newstarts.cn

[E12] 统计某字符出现次数
来源：http://ft.lnxyls.cn

Py:   s.count("a")
来源：http://fg.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://hv.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://kr.hnjuh.cn

TS:   s.split("a").length - 1
来源：http://od.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://tf.lnxyls.cn

Go:   strings.Count(s, "a")
来源：http://mz.nicolike.cn

Ruby: s.count("a")
来源：http://nt.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://fr.huanxung.cn

[E13] 逐字符遍历
来源：http://nz.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://wh.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bs.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ov.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://il.colortex.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wm.panjiajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://il.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ye.nicolike.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xj.bjjhwx.cn

[E14] URL 编码与 Base64
来源：http://ip.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lz.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xn.lnxyls.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zg.huixinmuqiang.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://km.shxzskj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bj.panjiajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ds.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ef.huixiangedu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://aw.panjiajie.cn

[E15] HTML 转义 / 反转义
来源：http://xh.nszjky.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://gp.gzmigu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://re.bjjhwx.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yp.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bt.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://te.jctech888.com.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qz.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rt.lnxyls.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vp.hnjuh.cn

[E16] 数字千分位
来源：http://od.haigaiapp.cn

Py:   f"{1234567:,}"
来源：http://zq.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://gj.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xx.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://cg.jianghongdianzi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pb.jianghongdianzi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jz.yuexingan06.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://je.huanxung.cn

C#:   1234567.ToString("N0")
来源：http://jv.9csxet.cn

[E17] 首字母大写
来源：http://rl.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://bw.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yv.newstarts.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qn.panjiajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ak.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zj.newstarts.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jx.huixiangedu.cn

Ruby: s.capitalize
来源：http://vo.jctech888.com.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://aa.nszjky.cn

[E18] 模板占位符替换
来源：http://ve.lnxyls.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ft.panjiajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://eo.hahajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://an.szxytkj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ue.szxytkj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://se.haigaiapp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vd.jianghongdianzi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://vh.szxytkj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://af.hahajie.cn

[E19] 多行文本按行拆分
来源：http://hb.muxihuayi.cn

Py:   s.splitlines()
来源：http://ia.panjiajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gp.bjjhwx.cn

JS:   s.split(/\r?\n/)
来源：http://ld.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://kv.haigaiapp.cn

Java: s.lines().toList()
来源：http://lo.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://qy.wgjwhj.cn

Ruby: s.lines
来源：http://sb.bookmarksfly.cn

C#:   s.Split('\n')
来源：http://av.yuntaijiaju.cn

[E20] 判断字符串是否为空
来源：http://la.shtwfgs.cn

Py:   if not s:
来源：http://ai.lnxyls.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://lf.jctech888.com.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://um.521024.cn

TS:   if (s === "") {}
来源：http://fb.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://hy.wgjwhj.cn

Go:   if s == "" {}
来源：http://ve.shtwfgs.cn

Ruby: if s.empty?
来源：http://gb.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://jl.shxzskj.cn

[E21] 超长截断加省略号
来源：http://lt.huixiangedu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wj.huixinmuqiang.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ao.colortex.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vx.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kj.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hu.yuntaijiaju.cn

Go:   // 按 rune 判断长度后截断
来源：http://wr.huanxung.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vc.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qx.bookmarksfly.cn

[E22] 字节长度与字符长度
来源：http://yl.jctech888.com.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cg.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://qc.huixinmuqiang.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ru.hnjuh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mr.shxzukj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xx.asd995.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hnjuh.cn

Ruby: s.bytesize;  s.length
来源：http://je.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ze.asd995.cn

================================================================================
来源：http://ba.shxzukj.cn

F. 文件与目录
来源：http://ju.nszjky.cn

================================================================================
来源：http://as.shtwfgs.cn

[F01] 读取整个文件
来源：http://gg.haigaiapp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ck.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://py.panjiajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yr.yuntaijiaju.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://af.lnxyls.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vm.yuntaijiaju.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ao.shxzskj.cn

Ruby: File.read("a.txt")
来源：http://vp.huixinmuqiang.cn

C#:   File.ReadAllText("a.txt");
来源：http://um.bjjhwx.cn

[F02] 逐行读取文件
来源：http://jp.bookmarksfly.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fl.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gq.hahajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kp.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ru.nicolike.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yt.gzmigu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sp.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jo.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sa.gzmigu.cn

[F03] 写入文件（覆盖）
来源：http://kf.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zg.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vm.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ea.haigaiapp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zv.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ba.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ym.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://ux.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mq.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://jy.gzmigu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hy.wgjwhj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ow.bjjhwx.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eo.wgjwhj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ii.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xw.jianghongdianzi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yv.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://rk.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wj.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://fp.9csxet.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gp.chemitech.net.cn

PHP:  file_exists("a.txt");
来源：http://uw.521024.cn

JS:   fs.existsSync("a.txt")
来源：http://om.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://ps.muxihuayi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ez.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://io.jctech888.com.cn

Ruby: File.exist?("a.txt")
来源：http://iw.hahajie.cn

C#:   File.Exists("a.txt")
来源：http://gc.szxytkj.cn

[F06] 删除文件
来源：http://lb.yuexingan06.cn

Py:   os.remove("a.txt")
来源：http://yl.lnxyls.cn

PHP:  unlink("a.txt");
来源：http://fj.shtwfgs.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ow.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://bg.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://id.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://sf.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://yk.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://sc.yuexingan06.cn

[F07] 创建目录（含多级）
来源：http://vt.colortex.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://lx.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ua.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mb.muxihuayi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dm.asd995.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pk.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://df.chemitech.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bs.nicolike.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bi.huanxung.cn

[F08] 遍历目录
来源：http://lg.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ta.yuexingan06.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bg.nicolike.cn

JS:   fs.readdirSync("dir")
来源：http://zt.newstarts.cn

TS:   fs.readdirSync("dir")
来源：http://ax.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://co.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yz.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://sq.nszjky.cn

C#:   Directory.GetFiles("dir")
来源：http://hy.chemitech.net.cn

[F09] 获取文件大小
来源：http://nv.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://ry.huixinmuqiang.cn

PHP:  filesize("a.txt");
来源：http://yj.hahajie.cn

JS:   fs.statSync("a.txt").size
来源：http://ih.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://kd.szxytkj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xn.nicolike.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cc.yuntaijiaju.cn

Ruby: File.size("a.txt")
来源：http://kc.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://lg.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://yy.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://iq.haigaiapp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nv.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://md.wgjwhj.cn

TS:   path.extname("a.txt")
来源：http://dy.chemitech.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://el.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ej.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zv.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sk.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://er.hnjuh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://au.hahajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bj.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://id.chemitech.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yd.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ho.hnjuh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://me.huixiangedu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sm.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oa.hnjuh.cn

[F12] CSV 读写
来源：http://zc.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jj.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vn.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ea.jctech888.com.cn

TS:   // 同上
来源：http://tj.gzmigu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cm.huanxung.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://zf.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://th.521024.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dj.jctech888.com.cn

================================================================================
来源：http://en.521024.cn

G. 面向对象
来源：http://du.jctech888.com.cn

================================================================================
来源：http://ic.asd995.cn

[G01] 定义类
来源：http://qs.nszjky.cn

Py:   class User: pass
来源：http://mz.szxytkj.cn

PHP:  class User {}
来源：http://zr.huixiangedu.cn

JS:   class User {}
来源：http://rs.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://dc.9csxet.cn

Java: class User {}
来源：http://mb.hnjuh.cn

Go:   type User struct { Name string }
来源：http://cy.asd995.cn

Ruby: class User; end
来源：http://id.hnjuh.cn

C#:   class User {}
来源：http://db.yuexingan06.cn

[G02] 构造函数
来源：http://tt.szxytkj.cn

Py:   def __init__(self, name): self.name = name
来源：http://bl.panjiajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://ki.shtwfgs.cn

JS:   constructor(name) { this.name = name; }
来源：http://dz.jianghongdianzi.cn

TS:   constructor(public name: string) {}
来源：http://qx.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://ar.jianghongdianzi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ns.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://uj.panjiajie.cn

C#:   public User(string name) { Name = name; }
来源：http://mo.yuexingan06.cn

[G03] 实例属性
来源：http://yd.9csxet.cn

Py:   self.name = "x"
来源：http://qy.9csxet.cn

PHP:  public string $name = "x";
来源：http://fp.huixiangedu.cn

JS:   this.name = "x";
来源：http://ep.huixiangedu.cn

TS:   name: string = "x";
来源：http://kz.9csxet.cn

Java: private String name;
来源：http://ne.panjiajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pw.521024.cn

Ruby: @name = "x"
来源：http://ga.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://xu.panjiajie.cn

[G04] 定义方法
来源：http://xd.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://sr.wgjwhj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ui.huanxung.cn

JS:   greet() { return this.name; }
来源：http://yx.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://fn.9csxet.cn

Java: String greet() { return name; }
来源：http://be.521024.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://sm.haigaiapp.cn

Ruby: def greet; @name; end
来源：http://lp.bookmarksfly.cn

C#:   public string Greet() => Name;
来源：http://ob.hahajie.cn

[G05] 继承
来源：http://wz.panjiajie.cn

Py:   class Admin(User): pass
来源：http://cf.yuntaijiaju.cn

PHP:  class Admin extends User {}
来源：http://qu.gzmigu.cn

JS:   class Admin extends User {}
来源：http://vm.lnxyls.cn

TS:   class Admin extends User {}
来源：http://qk.gzmigu.cn

Java: class Admin extends User {}
来源：http://zj.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wy.shxzukj.cn

Ruby: class Admin < User; end
来源：http://ls.panjiajie.cn

C#:   class Admin : User {}
来源：http://qp.colortex.cn

[G06] 重写方法
来源：http://xs.szsharing.cn

Py:   def greet(self): return "admin"
来源：http://sk.9csxet.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://su.hnjuh.cn

JS:   greet() { return "admin"; }
来源：http://ve.jianghongdianzi.cn

TS:   greet(): string { return "admin"; }
来源：http://of.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://mi.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ue.bookmarksfly.cn

Ruby: def greet; "admin"; end
来源：http://oy.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://xv.shxzskj.cn

[G07] 调用父类方法
来源：http://xy.newstarts.cn

Py:   super().greet()
来源：http://jd.newstarts.cn

PHP:  parent::greet();
来源：http://dh.shxzukj.cn

JS:   super.greet();
来源：http://zo.szxytkj.cn

TS:   super.greet();
来源：http://te.huixinmuqiang.cn

Java: super.greet();
来源：http://rz.szxytkj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vr.huixinmuqiang.cn

Ruby: super
来源：http://zs.hahajie.cn

C#:   base.Greet();
来源：http://bl.haigaiapp.cn

[G08] 静态方法与属性
来源：http://fn.szxytkj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xa.lnxyls.cn

PHP:  public static function f() {}
来源：http://kf.jctech888.com.cn

JS:   static f() {}
来源：http://hg.huanxung.cn

TS:   static f(): void {}
来源：http://jo.shtwfgs.cn

Java: static void f() {}
来源：http://ex.szsharing.cn


<!-- 参考信息 -->