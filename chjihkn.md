代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://nb.chemitech.net.cn

[E11] 反转字符串
来源：http://pi.gzmigu.cn

Py:   s[::-1]
来源：http://cm.chemitech.net.cn

PHP:  strrev($s);
来源：http://bm.muxihuayi.cn

JS:   [...s].reverse().join("")
来源：http://xz.hahajie.cn

TS:   [...s].reverse().join("")
来源：http://sl.wgjwhj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://so.bookmarksfly.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gs.huixinmuqiang.cn

Ruby: s.reverse
来源：http://ul.521024.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sv.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://gb.newstarts.cn

Py:   s.count("a")
来源：http://ha.nszjky.cn

PHP:  substr_count($s, "a");
来源：http://gf.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://lr.yuntaijiaju.cn

TS:   s.split("a").length - 1
来源：http://qp.huanxung.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dl.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://lf.9csxet.cn

Ruby: s.count("a")
来源：http://vf.bjjhwx.cn

C#:   s.Count(c => c == 'a')
来源：http://ur.gzmigu.cn

[E13] 逐字符遍历
来源：http://bu.shtwfgs.cn

Py:   for ch in s: print(ch)
来源：http://zo.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://na.gzmigu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kp.lnxyls.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dk.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ex.bjjhwx.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bt.hnjuh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pe.jctech888.com.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hi.colortex.cn

[E14] URL 编码与 Base64
来源：http://xj.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xd.hahajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nz.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hc.szsharing.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fa.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://la.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wx.shxzukj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oc.521024.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rs.shxzskj.cn

[E15] HTML 转义 / 反转义
来源：http://lt.szxytkj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ml.yuntaijiaju.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ap.huanxung.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ul.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jk.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ao.panjiajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://li.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gl.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rz.yuexingan06.cn

[E16] 数字千分位
来源：http://gm.szsharing.cn

Py:   f"{1234567:,}"
来源：http://ky.hahajie.cn

PHP:  number_format(1234567);
来源：http://qv.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hu.shtwfgs.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://iq.szxytkj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://eq.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://az.gzmigu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lp.szsharing.cn

C#:   1234567.ToString("N0")
来源：http://xe.521024.cn

[E17] 首字母大写
来源：http://rz.panjiajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://nb.newstarts.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://va.jctech888.com.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://at.panjiajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://si.shtwfgs.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hv.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gm.shxzskj.cn

Ruby: s.capitalize
来源：http://tv.shxzukj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ib.shxzskj.cn

[E18] 模板占位符替换
来源：http://ia.lnxyls.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gp.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vt.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pf.hahajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ye.yuexingan06.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dw.muxihuayi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cb.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ul.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rw.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://zp.muxihuayi.cn

Py:   s.splitlines()
来源：http://oq.panjiajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://me.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://eo.shxzukj.cn

TS:   s.split(/\r?\n/)
来源：http://xf.yuntaijiaju.cn

Java: s.lines().toList()
来源：http://jq.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://sf.shxzukj.cn

Ruby: s.lines
来源：http://vy.wgjwhj.cn

C#:   s.Split('\n')
来源：http://kd.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://jk.bjjhwx.cn

Py:   if not s:
来源：http://wa.haigaiapp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://qk.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://so.szxytkj.cn

TS:   if (s === "") {}
来源：http://fc.asd995.cn

Java: if (s.isEmpty()) {}
来源：http://to.jctech888.com.cn

Go:   if s == "" {}
来源：http://hr.colortex.cn

Ruby: if s.empty?
来源：http://cu.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ia.muxihuayi.cn

[E21] 超长截断加省略号
来源：http://ou.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ax.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mb.lnxyls.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://th.haigaiapp.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://es.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zj.yuntaijiaju.cn

Go:   // 按 rune 判断长度后截断
来源：http://yi.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jy.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ot.shxzukj.cn

[E22] 字节长度与字符长度
来源：http://ud.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ec.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://aa.hnjuh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://en.lnxyls.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rc.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jj.muxihuayi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sb.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://bc.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ob.shtwfgs.cn

================================================================================
来源：http://nc.colortex.cn

F. 文件与目录
来源：http://hc.lnxyls.cn

================================================================================
来源：http://ox.wgjwhj.cn

[F01] 读取整个文件
来源：http://cz.colortex.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rn.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://tq.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vs.nszjky.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ub.yuntaijiaju.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lk.huixinmuqiang.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nf.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://xo.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://pm.huanxung.cn

[F02] 逐行读取文件
来源：http://lx.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://an.shtwfgs.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cu.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://em.colortex.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jo.lnxyls.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mp.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://an.yuexingan06.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://da.huixinmuqiang.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ic.bookmarksfly.cn

[F03] 写入文件（覆盖）
来源：http://mw.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yw.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tf.shxzskj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ag.muxihuayi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dt.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lq.9csxet.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lk.wgjwhj.cn

Ruby: File.write("a.txt", "hi")
来源：http://jc.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tg.panjiajie.cn

[F04] 追加写入文件
来源：http://rc.haigaiapp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gr.huanxung.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wz.hahajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yq.yuexingan06.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cm.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://av.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qs.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://cc.panjiajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ce.bjjhwx.cn

[F05] 判断文件或目录是否存在
来源：http://ex.yuexingan06.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ma.nszjky.cn

PHP:  file_exists("a.txt");
来源：http://rk.yuntaijiaju.cn

JS:   fs.existsSync("a.txt")
来源：http://zm.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://lh.shxzskj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ir.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ba.muxihuayi.cn

Ruby: File.exist?("a.txt")
来源：http://tp.huanxung.cn

C#:   File.Exists("a.txt")
来源：http://qs.jianghongdianzi.cn

[F06] 删除文件
来源：http://zx.newstarts.cn

Py:   os.remove("a.txt")
来源：http://oh.newstarts.cn

PHP:  unlink("a.txt");
来源：http://ue.chemitech.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://us.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dh.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ip.newstarts.cn

Go:   os.Remove("a.txt")
来源：http://vh.hahajie.cn

Ruby: File.delete("a.txt")
来源：http://fc.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://qq.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://ct.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ck.szsharing.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cw.huixinmuqiang.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://re.wgjwhj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kk.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wa.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tp.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ur.huanxung.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ty.gzmigu.cn

[F08] 遍历目录
来源：http://zm.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://dp.nszjky.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lb.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://iq.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://fu.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nu.shxzskj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wo.newstarts.cn

Ruby: Dir.children("dir")
来源：http://mt.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://ld.wgjwhj.cn

[F09] 获取文件大小
来源：http://tr.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://mq.bookmarksfly.cn

PHP:  filesize("a.txt");
来源：http://nn.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://ll.asd995.cn

TS:   fs.statSync("a.txt").size
来源：http://sv.gzmigu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://tr.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aa.521024.cn

Ruby: File.size("a.txt")
来源：http://mu.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://yk.shxzukj.cn

[F10] 取文件扩展名 / 文件名
来源：http://ud.szsharing.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ii.yuexingan06.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gy.jianghongdianzi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lk.nszjky.cn

TS:   path.extname("a.txt")
来源：http://vl.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gb.huixinmuqiang.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kw.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nq.shtwfgs.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://jw.newstarts.cn

[F11] 复制与移动文件
来源：http://vu.huanxung.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xk.lnxyls.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://uo.shtwfgs.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rf.muxihuayi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wb.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kj.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hv.521024.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://di.szxytkj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cc.yuntaijiaju.cn

[F12] CSV 读写
来源：http://ca.huixinmuqiang.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tp.shtwfgs.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ws.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kp.bookmarksfly.cn

TS:   // 同上
来源：http://au.huixinmuqiang.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vm.jctech888.com.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://tz.lnxyls.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://il.colortex.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://cp.shxzukj.cn

================================================================================
来源：http://tr.gzmigu.cn

G. 面向对象
来源：http://ex.haigaiapp.cn

================================================================================
来源：http://tt.hahajie.cn

[G01] 定义类
来源：http://yo.asd995.cn

Py:   class User: pass
来源：http://go.9csxet.cn

PHP:  class User {}
来源：http://xq.newstarts.cn

JS:   class User {}
来源：http://ad.bjjhwx.cn

TS:   class User { name: string = ""; }
来源：http://ka.hahajie.cn

Java: class User {}
来源：http://ku.colortex.cn

Go:   type User struct { Name string }
来源：http://wa.asd995.cn

Ruby: class User; end
来源：http://ic.521024.cn

C#:   class User {}
来源：http://ce.shxzukj.cn

[G02] 构造函数
来源：http://gu.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://xm.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://jk.szsharing.cn

JS:   constructor(name) { this.name = name; }
来源：http://ly.szxytkj.cn

TS:   constructor(public name: string) {}
来源：http://dc.9csxet.cn

Java: User(String name) { this.name = name; }
来源：http://bl.chemitech.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hl.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://iv.9csxet.cn

C#:   public User(string name) { Name = name; }
来源：http://qv.muxihuayi.cn

[G03] 实例属性
来源：http://tk.bookmarksfly.cn

Py:   self.name = "x"
来源：http://kf.yuntaijiaju.cn

PHP:  public string $name = "x";
来源：http://rc.chemitech.net.cn

JS:   this.name = "x";
来源：http://dh.bjjhwx.cn

TS:   name: string = "x";
来源：http://in.nszjky.cn

Java: private String name;
来源：http://km.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ce.nszjky.cn

Ruby: @name = "x"
来源：http://ru.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://fk.jianghongdianzi.cn

[G04] 定义方法
来源：http://hu.nicolike.cn

Py:   def greet(self): return self.name
来源：http://vr.huanxung.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wt.chemitech.net.cn

JS:   greet() { return this.name; }
来源：http://ft.bookmarksfly.cn

TS:   greet(): string { return this.name; }
来源：http://oy.jianghongdianzi.cn

Java: String greet() { return name; }
来源：http://ba.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yf.hnjuh.cn

Ruby: def greet; @name; end
来源：http://nq.haigaiapp.cn

C#:   public string Greet() => Name;
来源：http://bv.hahajie.cn

[G05] 继承
来源：http://fq.hnjuh.cn

Py:   class Admin(User): pass
来源：http://ij.shtwfgs.cn

PHP:  class Admin extends User {}
来源：http://jw.jianghongdianzi.cn

JS:   class Admin extends User {}
来源：http://ma.hahajie.cn

TS:   class Admin extends User {}
来源：http://yb.wgjwhj.cn

Java: class Admin extends User {}
来源：http://by.asd995.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hm.panjiajie.cn

Ruby: class Admin < User; end
来源：http://fs.bookmarksfly.cn

C#:   class Admin : User {}
来源：http://dd.chemitech.net.cn

[G06] 重写方法
来源：http://wo.bjjhwx.cn

Py:   def greet(self): return "admin"
来源：http://qy.wgjwhj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://so.newstarts.cn

JS:   greet() { return "admin"; }
来源：http://ic.yuntaijiaju.cn

TS:   greet(): string { return "admin"; }
来源：http://ic.asd995.cn

Java: @Override String greet() { return "admin"; }
来源：http://yw.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://en.bookmarksfly.cn

Ruby: def greet; "admin"; end
来源：http://mt.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://ir.gzmigu.cn

[G07] 调用父类方法
来源：http://ry.521024.cn

Py:   super().greet()
来源：http://op.nszjky.cn

PHP:  parent::greet();
来源：http://de.nszjky.cn

JS:   super.greet();
来源：http://yq.hahajie.cn

TS:   super.greet();
来源：http://hm.shxzukj.cn

Java: super.greet();
来源：http://le.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yv.wgjwhj.cn

Ruby: super
来源：http://yp.lnxyls.cn

C#:   base.Greet();
来源：http://ga.hnjuh.cn

[G08] 静态方法与属性
来源：http://il.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lg.huanxung.cn

PHP:  public static function f() {}
来源：http://ml.szsharing.cn

JS:   static f() {}
来源：http://qf.shxzukj.cn

TS:   static f(): void {}
来源：http://il.haigaiapp.cn

Java: static void f() {}
来源：http://fy.shxzukj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qc.szxytkj.cn

Ruby: def self.f; end
来源：http://gr.muxihuayi.cn

C#:   public static void F() {}
来源：http://hq.asd995.cn

[G09] 接口 / 抽象类
来源：http://kk.chemitech.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://gq.bookmarksfly.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hn.yuexingan06.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xp.521024.cn

TS:   interface Shape { area(): number; }
来源：http://lw.jctech888.com.cn


<!-- 参考信息 -->