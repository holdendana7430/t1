代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://en.jianghongdianzi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nf.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tl.jianghongdianzi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ii.nicolike.cn

[E14] URL 编码与 Base64
来源：http://nr.wgjwhj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://le.panjiajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://io.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ii.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vt.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dk.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ta.9csxet.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xr.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ga.newstarts.cn

[E15] HTML 转义 / 反转义
来源：http://lw.colortex.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ph.nszjky.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ow.wgjwhj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rk.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://so.jctech888.com.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://pj.hnjuh.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gi.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://nm.szxytkj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ux.hnjuh.cn

[E16] 数字千分位
来源：http://ju.colortex.cn

Py:   f"{1234567:,}"
来源：http://ej.huanxung.cn

PHP:  number_format(1234567);
来源：http://kd.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://yo.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wu.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wj.bjjhwx.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ez.nszjky.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yp.nszjky.cn

C#:   1234567.ToString("N0")
来源：http://pu.colortex.cn

[E17] 首字母大写
来源：http://jv.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uz.chemitech.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://vh.szxytkj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xo.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wa.hahajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://bf.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wt.haigaiapp.cn

Ruby: s.capitalize
来源：http://uj.szxytkj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mq.panjiajie.cn

[E18] 模板占位符替换
来源：http://ub.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cf.haigaiapp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dm.colortex.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qy.lnxyls.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://lg.9csxet.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xp.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bd.huanxung.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://he.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://id.bjjhwx.cn

[E19] 多行文本按行拆分
来源：http://uk.huixinmuqiang.cn

Py:   s.splitlines()
来源：http://ys.szxytkj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://gb.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://qf.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://sg.9csxet.cn

Java: s.lines().toList()
来源：http://gt.9csxet.cn

Go:   strings.Split(s, "\n")
来源：http://ov.muxihuayi.cn

Ruby: s.lines
来源：http://of.asd995.cn

C#:   s.Split('\n')
来源：http://kh.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://hc.nicolike.cn

Py:   if not s:
来源：http://fm.huixinmuqiang.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gj.hnjuh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://eh.asd995.cn

TS:   if (s === "") {}
来源：http://wz.yuexingan06.cn

Java: if (s.isEmpty()) {}
来源：http://ce.szxytkj.cn

Go:   if s == "" {}
来源：http://ua.lnxyls.cn

Ruby: if s.empty?
来源：http://yn.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vu.shxzukj.cn

[E21] 超长截断加省略号
来源：http://sv.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ib.nicolike.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mm.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zt.szxytkj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://iu.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cc.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://co.hahajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wq.gzmigu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jo.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://le.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qb.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ye.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ah.shxzukj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ym.bjjhwx.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qz.colortex.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://si.shxzskj.cn

Ruby: s.bytesize;  s.length
来源：http://me.nicolike.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://iw.yuntaijiaju.cn

================================================================================
来源：http://ie.lnxyls.cn

F. 文件与目录
来源：http://hz.9csxet.cn

================================================================================
来源：http://yj.huixiangedu.cn

[F01] 读取整个文件
来源：http://mv.bjjhwx.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wl.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://lv.szxytkj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://as.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vo.jianghongdianzi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yz.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://er.hahajie.cn

Ruby: File.read("a.txt")
来源：http://tg.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://pd.yuexingan06.cn

[F02] 逐行读取文件
来源：http://yj.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://vc.huanxung.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ty.shxzukj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dd.szsharing.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://no.panjiajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zj.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ys.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dc.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vs.yuntaijiaju.cn

[F03] 写入文件（覆盖）
来源：http://xn.9csxet.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ce.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bd.szxytkj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dc.szxytkj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uz.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uk.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gc.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://bx.huixinmuqiang.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://on.chemitech.net.cn

[F04] 追加写入文件
来源：http://gz.huixiangedu.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yx.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dp.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ru.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xr.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ml.shxzukj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rd.haigaiapp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://co.huanxung.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wz.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://eb.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zv.hahajie.cn

PHP:  file_exists("a.txt");
来源：http://go.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://pm.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://zt.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://zo.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fh.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://gv.nszjky.cn

C#:   File.Exists("a.txt")
来源：http://ny.huixinmuqiang.cn

[F06] 删除文件
来源：http://ul.asd995.cn

Py:   os.remove("a.txt")
来源：http://rf.huixinmuqiang.cn

PHP:  unlink("a.txt");
来源：http://mv.hnjuh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gx.chemitech.net.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ga.shxzskj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wc.shtwfgs.cn

Go:   os.Remove("a.txt")
来源：http://lt.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://hw.szsharing.cn

C#:   File.Delete("a.txt");
来源：http://kz.newstarts.cn

[F07] 创建目录（含多级）
来源：http://hs.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zk.hnjuh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cu.haigaiapp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ta.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wn.huixiangedu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bt.shxzskj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qj.chemitech.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hk.jctech888.com.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ig.haigaiapp.cn

[F08] 遍历目录
来源：http://uu.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://el.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rv.newstarts.cn

JS:   fs.readdirSync("dir")
来源：http://pa.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://wc.huixinmuqiang.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nt.panjiajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zn.hahajie.cn

Ruby: Dir.children("dir")
来源：http://kk.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://nc.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://om.nicolike.cn

Py:   os.path.getsize("a.txt")
来源：http://pe.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://dr.hahajie.cn

JS:   fs.statSync("a.txt").size
来源：http://mc.bookmarksfly.cn

TS:   fs.statSync("a.txt").size
来源：http://pr.jctech888.com.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mi.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ds.yuntaijiaju.cn

Ruby: File.size("a.txt")
来源：http://ty.nicolike.cn

C#:   new FileInfo("a.txt").Length
来源：http://hw.szsharing.cn

[F10] 取文件扩展名 / 文件名
来源：http://mc.huixiangedu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jy.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://pd.nszjky.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ie.jctech888.com.cn

TS:   path.extname("a.txt")
来源：http://rm.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://we.panjiajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rj.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ip.nszjky.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xs.yuntaijiaju.cn

[F11] 复制与移动文件
来源：http://ty.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vc.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gt.newstarts.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ml.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qc.huixiangedu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://po.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zb.shxzskj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sn.haigaiapp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eu.jianghongdianzi.cn

[F12] CSV 读写
来源：http://vg.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://da.shtwfgs.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://up.huixiangedu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bb.muxihuayi.cn

TS:   // 同上
来源：http://yt.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://sw.szsharing.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ap.panjiajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xb.colortex.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ft.newstarts.cn

================================================================================
来源：http://ak.huixiangedu.cn

G. 面向对象
来源：http://if.huanxung.cn

================================================================================
来源：http://es.huixinmuqiang.cn

[G01] 定义类
来源：http://cm.bjjhwx.cn

Py:   class User: pass
来源：http://kc.lnxyls.cn

PHP:  class User {}
来源：http://dq.szxytkj.cn

JS:   class User {}
来源：http://ns.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://eu.bookmarksfly.cn

Java: class User {}
来源：http://lb.szsharing.cn

Go:   type User struct { Name string }
来源：http://if.shxzskj.cn

Ruby: class User; end
来源：http://vk.huixiangedu.cn

C#:   class User {}
来源：http://md.szxytkj.cn

[G02] 构造函数
来源：http://rj.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://mg.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://uu.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://oc.shxzukj.cn

TS:   constructor(public name: string) {}
来源：http://ur.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://ri.chemitech.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lk.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://la.nszjky.cn

C#:   public User(string name) { Name = name; }
来源：http://jx.szxytkj.cn

[G03] 实例属性
来源：http://jw.nicolike.cn

Py:   self.name = "x"
来源：http://qg.shxzskj.cn

PHP:  public string $name = "x";
来源：http://nl.shxzskj.cn

JS:   this.name = "x";
来源：http://zg.hnjuh.cn

TS:   name: string = "x";
来源：http://ui.huanxung.cn

Java: private String name;
来源：http://im.jianghongdianzi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oy.lnxyls.cn

Ruby: @name = "x"
来源：http://bx.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://ng.shxzukj.cn

[G04] 定义方法
来源：http://ce.asd995.cn

Py:   def greet(self): return self.name
来源：http://fj.shxzukj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ey.jianghongdianzi.cn

JS:   greet() { return this.name; }
来源：http://et.wgjwhj.cn

TS:   greet(): string { return this.name; }
来源：http://hn.nicolike.cn

Java: String greet() { return name; }
来源：http://jo.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://oa.muxihuayi.cn

Ruby: def greet; @name; end
来源：http://wp.nicolike.cn

C#:   public string Greet() => Name;
来源：http://al.yuntaijiaju.cn

[G05] 继承
来源：http://zp.shxzukj.cn

Py:   class Admin(User): pass
来源：http://yp.szxytkj.cn

PHP:  class Admin extends User {}
来源：http://mj.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://uy.nicolike.cn

TS:   class Admin extends User {}
来源：http://ze.szxytkj.cn

Java: class Admin extends User {}
来源：http://az.gzmigu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://su.521024.cn

Ruby: class Admin < User; end
来源：http://cq.szxytkj.cn

C#:   class Admin : User {}
来源：http://ea.haigaiapp.cn

[G06] 重写方法
来源：http://qc.asd995.cn

Py:   def greet(self): return "admin"
来源：http://jw.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wo.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://aw.szxytkj.cn

TS:   greet(): string { return "admin"; }
来源：http://qv.shxzukj.cn

Java: @Override String greet() { return "admin"; }
来源：http://up.shtwfgs.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gu.jctech888.com.cn

Ruby: def greet; "admin"; end
来源：http://of.bjjhwx.cn

C#:   public override string Greet() => "admin";
来源：http://xe.521024.cn

[G07] 调用父类方法
来源：http://yw.bjjhwx.cn

Py:   super().greet()
来源：http://av.hahajie.cn

PHP:  parent::greet();
来源：http://kg.nszjky.cn

JS:   super.greet();
来源：http://lc.nszjky.cn

TS:   super.greet();
来源：http://yo.521024.cn

Java: super.greet();
来源：http://lx.nszjky.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gn.huixinmuqiang.cn

Ruby: super
来源：http://wc.hnjuh.cn

C#:   base.Greet();
来源：http://mo.asd995.cn

[G08] 静态方法与属性
来源：http://np.9csxet.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wj.9csxet.cn

PHP:  public static function f() {}
来源：http://ju.shxzukj.cn

JS:   static f() {}
来源：http://hz.jctech888.com.cn

TS:   static f(): void {}
来源：http://bj.chemitech.net.cn

Java: static void f() {}
来源：http://mv.huixiangedu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://gm.haigaiapp.cn

Ruby: def self.f; end
来源：http://ye.hahajie.cn

C#:   public static void F() {}
来源：http://md.chemitech.net.cn

[G09] 接口 / 抽象类
来源：http://my.bookmarksfly.cn

Py:   from abc import ABC, abstractmethod
来源：http://jk.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hv.shxzskj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jt.chemitech.net.cn

TS:   interface Shape { area(): number; }
来源：http://py.yuexingan06.cn

Java: interface Shape { double area(); }
来源：http://ng.shtwfgs.cn

Go:   type Shape interface { Area() float64 }
来源：http://qo.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ik.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://je.wgjwhj.cn

[G10] 访问控制
来源：http://yl.newstarts.cn

Py:   约定 _protected / __private（不强制）
来源：http://ak.chemitech.net.cn

PHP:  public / protected / private
来源：http://uk.shxzukj.cn

JS:   #private 字段；其余公开
来源：http://zn.yuntaijiaju.cn

TS:   public / protected / private
来源：http://cp.shxzskj.cn

Java: public / protected / private / 默认包级
来源：http://mf.shxzskj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lm.yuexingan06.cn

Ruby: public / protected / private
来源：http://fl.asd995.cn

C#:   public / protected / private / internal
来源：http://cu.nicolike.cn

[G11] getter / setter
来源：http://ek.newstarts.cn

Py:   @property 与 @x.setter
来源：http://ec.bookmarksfly.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ia.gzmigu.cn

JS:   get name() { return this._name; }
来源：http://tn.chemitech.net.cn

TS:   get name(): string { return this._name; }
来源：http://wl.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://em.gzmigu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dp.wgjwhj.cn

Ruby: attr_accessor :name
来源：http://rr.hahajie.cn

C#:   public string Name { get; set; }
来源：http://gz.szsharing.cn

[G12] 对象转字符串
来源：http://gq.hnjuh.cn

Py:   def __str__(self): return self.name
来源：http://sp.newstarts.cn


<!-- 参考信息 -->