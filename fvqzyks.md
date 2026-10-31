代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jj.shxzukj.cn

[E15] HTML 转义 / 反转义
来源：http://pf.yuexingan06.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xe.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://eq.nszjky.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qm.huanxung.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://pi.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://rw.huixiangedu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mv.haigaiapp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://iz.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://uq.yuexingan06.cn

[E16] 数字千分位
来源：http://hm.huixiangedu.cn

Py:   f"{1234567:,}"
来源：http://ev.wgjwhj.cn

PHP:  number_format(1234567);
来源：http://hs.huixiangedu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hh.haigaiapp.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://um.jianghongdianzi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wf.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lw.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://yj.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://rn.shtwfgs.cn

[E17] 首字母大写
来源：http://ke.szsharing.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://xd.newstarts.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ug.bjjhwx.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oo.hahajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ke.lnxyls.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uo.wgjwhj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://kj.nszjky.cn

Ruby: s.capitalize
来源：http://ym.nicolike.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vi.muxihuayi.cn

[E18] 模板占位符替换
来源：http://fh.9csxet.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tx.nszjky.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pf.szsharing.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wi.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sc.nicolike.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yo.wgjwhj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bz.colortex.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kx.shxzskj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ju.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://bo.newstarts.cn

Py:   s.splitlines()
来源：http://ct.shxzukj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mu.panjiajie.cn

JS:   s.split(/\r?\n/)
来源：http://rh.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://iw.521024.cn

Java: s.lines().toList()
来源：http://dw.chemitech.net.cn

Go:   strings.Split(s, "\n")
来源：http://rj.muxihuayi.cn

Ruby: s.lines
来源：http://hh.haigaiapp.cn

C#:   s.Split('\n')
来源：http://mm.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://bm.colortex.cn

Py:   if not s:
来源：http://kn.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uw.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zs.panjiajie.cn

TS:   if (s === "") {}
来源：http://sc.haigaiapp.cn

Java: if (s.isEmpty()) {}
来源：http://cn.521024.cn

Go:   if s == "" {}
来源：http://il.shxzskj.cn

Ruby: if s.empty?
来源：http://hv.jctech888.com.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wm.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://br.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://db.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vh.colortex.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://en.chemitech.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ss.bookmarksfly.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://px.jianghongdianzi.cn

Go:   // 按 rune 判断长度后截断
来源：http://fi.bookmarksfly.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zn.newstarts.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yx.szsharing.cn

[E22] 字节长度与字符长度
来源：http://pb.hahajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ty.yuexingan06.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ei.shxzukj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xx.jctech888.com.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://fc.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mq.asd995.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wz.hnjuh.cn

Ruby: s.bytesize;  s.length
来源：http://li.chemitech.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ke.yuntaijiaju.cn

================================================================================
来源：http://op.asd995.cn

F. 文件与目录
来源：http://js.huanxung.cn

================================================================================
来源：http://mj.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://nm.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vq.muxihuayi.cn

PHP:  file_get_contents("a.txt");
来源：http://fe.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://re.chemitech.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://fx.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yl.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://df.hnjuh.cn

Ruby: File.read("a.txt")
来源：http://lt.bjjhwx.cn

C#:   File.ReadAllText("a.txt");
来源：http://uq.gzmigu.cn

[F02] 逐行读取文件
来源：http://rv.hnjuh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://os.chemitech.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mw.yuntaijiaju.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sf.haigaiapp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vy.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://da.muxihuayi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hm.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tw.jianghongdianzi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vi.wgjwhj.cn

[F03] 写入文件（覆盖）
来源：http://ml.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vi.panjiajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gy.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bu.haigaiapp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ke.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://to.haigaiapp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zc.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://mn.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ds.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://xd.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qe.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lv.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vu.jianghongdianzi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ic.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sg.hnjuh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pc.asd995.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nt.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mz.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://rg.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ni.jctech888.com.cn

PHP:  file_exists("a.txt");
来源：http://kk.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://bx.huixiangedu.cn

TS:   fs.existsSync("a.txt")
来源：http://no.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nd.colortex.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ba.huixiangedu.cn

Ruby: File.exist?("a.txt")
来源：http://fk.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://as.huixinmuqiang.cn

[F06] 删除文件
来源：http://hj.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://gm.yuexingan06.cn

PHP:  unlink("a.txt");
来源：http://pe.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ye.yuexingan06.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rv.haigaiapp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://od.huanxung.cn

Go:   os.Remove("a.txt")
来源：http://ys.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://co.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://bi.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://zh.huixinmuqiang.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ie.hahajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ny.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hv.colortex.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rq.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ex.wgjwhj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ip.chemitech.net.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zx.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ol.shxzskj.cn

[F08] 遍历目录
来源：http://nj.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ue.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://op.huixiangedu.cn

JS:   fs.readdirSync("dir")
来源：http://mw.yuntaijiaju.cn

TS:   fs.readdirSync("dir")
来源：http://xn.9csxet.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pz.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yx.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://ap.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://kx.bookmarksfly.cn

[F09] 获取文件大小
来源：http://dm.huixinmuqiang.cn

Py:   os.path.getsize("a.txt")
来源：http://vt.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://bi.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://dq.hahajie.cn

TS:   fs.statSync("a.txt").size
来源：http://ej.huanxung.cn

Java: Files.size(Path.of("a.txt"))
来源：http://uq.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wl.asd995.cn

Ruby: File.size("a.txt")
来源：http://gr.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://nb.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://rb.lnxyls.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ht.shxzukj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qq.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lu.gzmigu.cn

TS:   path.extname("a.txt")
来源：http://ou.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bv.huixinmuqiang.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ul.9csxet.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tl.521024.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gc.huixiangedu.cn

[F11] 复制与移动文件
来源：http://ho.huanxung.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://df.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://di.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://he.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kn.jianghongdianzi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ua.szsharing.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zs.wgjwhj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gp.szxytkj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rn.hahajie.cn

[F12] CSV 读写
来源：http://ps.asd995.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cf.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rj.hnjuh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jf.jianghongdianzi.cn

TS:   // 同上
来源：http://qf.newstarts.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xo.lnxyls.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vc.asd995.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vy.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://uv.yuntaijiaju.cn

================================================================================
来源：http://yn.huixinmuqiang.cn

G. 面向对象
来源：http://tb.521024.cn

================================================================================
来源：http://ux.lnxyls.cn

[G01] 定义类
来源：http://ar.9csxet.cn

Py:   class User: pass
来源：http://ob.huanxung.cn

PHP:  class User {}
来源：http://jl.yuntaijiaju.cn

JS:   class User {}
来源：http://hi.shtwfgs.cn

TS:   class User { name: string = ""; }
来源：http://ki.shtwfgs.cn

Java: class User {}
来源：http://ho.nszjky.cn

Go:   type User struct { Name string }
来源：http://rt.shxzskj.cn

Ruby: class User; end
来源：http://bp.panjiajie.cn

C#:   class User {}
来源：http://uj.wgjwhj.cn

[G02] 构造函数
来源：http://ny.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://lc.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://if.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://vg.bookmarksfly.cn

TS:   constructor(public name: string) {}
来源：http://kd.jctech888.com.cn

Java: User(String name) { this.name = name; }
来源：http://cw.newstarts.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://at.yuexingan06.cn

Ruby: def initialize(name); @name = name; end
来源：http://wy.jctech888.com.cn

C#:   public User(string name) { Name = name; }
来源：http://yd.wgjwhj.cn

[G03] 实例属性
来源：http://zg.newstarts.cn

Py:   self.name = "x"
来源：http://mq.lnxyls.cn

PHP:  public string $name = "x";
来源：http://bv.yuexingan06.cn

JS:   this.name = "x";
来源：http://bf.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://xe.yuntaijiaju.cn

Java: private String name;
来源：http://nd.colortex.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cf.nicolike.cn

Ruby: @name = "x"
来源：http://sq.lnxyls.cn

C#:   public string Name { get; set; } = "x";
来源：http://jq.gzmigu.cn

[G04] 定义方法
来源：http://yv.huanxung.cn

Py:   def greet(self): return self.name
来源：http://fx.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nn.chemitech.net.cn

JS:   greet() { return this.name; }
来源：http://xb.huanxung.cn

TS:   greet(): string { return this.name; }
来源：http://el.yuntaijiaju.cn

Java: String greet() { return name; }
来源：http://ux.nszjky.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://uu.nicolike.cn

Ruby: def greet; @name; end
来源：http://iy.asd995.cn

C#:   public string Greet() => Name;
来源：http://hc.bjjhwx.cn

[G05] 继承
来源：http://jd.colortex.cn

Py:   class Admin(User): pass
来源：http://df.521024.cn

PHP:  class Admin extends User {}
来源：http://cm.jctech888.com.cn

JS:   class Admin extends User {}
来源：http://pz.huixinmuqiang.cn

TS:   class Admin extends User {}
来源：http://oo.panjiajie.cn

Java: class Admin extends User {}
来源：http://fx.wgjwhj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gi.gzmigu.cn

Ruby: class Admin < User; end
来源：http://aq.shxzukj.cn

C#:   class Admin : User {}
来源：http://ay.wgjwhj.cn

[G06] 重写方法
来源：http://zl.521024.cn

Py:   def greet(self): return "admin"
来源：http://nv.hnjuh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sh.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://xd.jianghongdianzi.cn

TS:   greet(): string { return "admin"; }
来源：http://pn.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://rc.shtwfgs.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dr.asd995.cn

Ruby: def greet; "admin"; end
来源：http://ur.panjiajie.cn

C#:   public override string Greet() => "admin";
来源：http://nz.huixiangedu.cn

[G07] 调用父类方法
来源：http://xt.yuntaijiaju.cn

Py:   super().greet()
来源：http://sj.chemitech.net.cn

PHP:  parent::greet();
来源：http://xn.huixiangedu.cn

JS:   super.greet();
来源：http://tr.jctech888.com.cn

TS:   super.greet();
来源：http://gh.asd995.cn

Java: super.greet();
来源：http://jr.szxytkj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cb.asd995.cn

Ruby: super
来源：http://ym.colortex.cn

C#:   base.Greet();
来源：http://mv.panjiajie.cn

[G08] 静态方法与属性
来源：http://rd.hahajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qs.shxzukj.cn

PHP:  public static function f() {}
来源：http://hn.hahajie.cn

JS:   static f() {}
来源：http://kk.muxihuayi.cn

TS:   static f(): void {}
来源：http://vx.szsharing.cn

Java: static void f() {}
来源：http://ph.panjiajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nh.szsharing.cn

Ruby: def self.f; end
来源：http://xn.jctech888.com.cn

C#:   public static void F() {}
来源：http://gy.gzmigu.cn

[G09] 接口 / 抽象类
来源：http://nf.huixinmuqiang.cn

Py:   from abc import ABC, abstractmethod
来源：http://tb.bookmarksfly.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vm.hahajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://iw.panjiajie.cn

TS:   interface Shape { area(): number; }
来源：http://bl.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://va.gzmigu.cn

Go:   type Shape interface { Area() float64 }
来源：http://uz.yuntaijiaju.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ok.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://wk.shxzukj.cn

[G10] 访问控制
来源：http://vt.newstarts.cn

Py:   约定 _protected / __private（不强制）
来源：http://fa.newstarts.cn

PHP:  public / protected / private
来源：http://vf.bookmarksfly.cn

JS:   #private 字段；其余公开
来源：http://qj.huixinmuqiang.cn

TS:   public / protected / private
来源：http://yv.521024.cn

Java: public / protected / private / 默认包级
来源：http://za.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rg.lnxyls.cn

Ruby: public / protected / private
来源：http://of.yuexingan06.cn

C#:   public / protected / private / internal
来源：http://sp.9csxet.cn

[G11] getter / setter
来源：http://tw.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://aa.shxzukj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ct.bjjhwx.cn

JS:   get name() { return this._name; }
来源：http://be.lnxyls.cn

TS:   get name(): string { return this._name; }
来源：http://hv.wgjwhj.cn

Java: public String getName() { return name; }
来源：http://my.haigaiapp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ys.colortex.cn

Ruby: attr_accessor :name
来源：http://kr.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://ww.gzmigu.cn

[G12] 对象转字符串
来源：http://uj.wgjwhj.cn

Py:   def __str__(self): return self.name
来源：http://bx.muxihuayi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://we.haigaiapp.cn

JS:   toString() { return this.name; }
来源：http://qz.huanxung.cn

TS:   toString(): string { return this.name; }
来源：http://ru.gzmigu.cn

Java: @Override public String toString() { return name; }
来源：http://gd.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kk.shxzskj.cn

Ruby: def to_s; @name; end
来源：http://fx.szxytkj.cn

C#:   public override string ToString() => Name;
来源：http://zb.colortex.cn

[G13] 判断对象类型
来源：http://gi.hahajie.cn

Py:   isinstance(u, User)
来源：http://tz.panjiajie.cn

PHP:  $u instanceof User
来源：http://ks.jctech888.com.cn

JS:   u instanceof User
来源：http://bh.521024.cn

TS:   u instanceof User
来源：http://ik.gzmigu.cn


<!-- 参考信息 -->