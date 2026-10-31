代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://oq.szsharing.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cl.bjjhwx.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hu.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mo.wgjwhj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://iu.hahajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ez.panjiajie.cn

[E16] 数字千分位
来源：http://lc.szsharing.cn

Py:   f"{1234567:,}"
来源：http://xz.huixiangedu.cn

PHP:  number_format(1234567);
来源：http://os.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dp.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ef.jianghongdianzi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ll.bjjhwx.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wy.hahajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://tt.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://bd.haigaiapp.cn

[E17] 首字母大写
来源：http://em.bookmarksfly.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ae.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://de.9csxet.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vx.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://br.gzmigu.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uf.huixiangedu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sx.newstarts.cn

Ruby: s.capitalize
来源：http://zo.wgjwhj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nd.szsharing.cn

[E18] 模板占位符替换
来源：http://vp.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ed.newstarts.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kj.szsharing.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ab.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://no.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yf.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://as.hnjuh.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bt.lnxyls.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vu.521024.cn

[E19] 多行文本按行拆分
来源：http://ms.yuntaijiaju.cn

Py:   s.splitlines()
来源：http://ni.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://nn.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://jn.colortex.cn

TS:   s.split(/\r?\n/)
来源：http://xe.9csxet.cn

Java: s.lines().toList()
来源：http://lw.bookmarksfly.cn

Go:   strings.Split(s, "\n")
来源：http://iy.szxytkj.cn

Ruby: s.lines
来源：http://co.shxzukj.cn

C#:   s.Split('\n')
来源：http://tt.9csxet.cn

[E20] 判断字符串是否为空
来源：http://vk.hahajie.cn

Py:   if not s:
来源：http://pf.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bf.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ju.hnjuh.cn

TS:   if (s === "") {}
来源：http://qp.521024.cn

Java: if (s.isEmpty()) {}
来源：http://wr.521024.cn

Go:   if s == "" {}
来源：http://wc.9csxet.cn

Ruby: if s.empty?
来源：http://tx.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pr.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://at.yuexingan06.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jt.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vg.panjiajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://he.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zp.newstarts.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://na.jianghongdianzi.cn

Go:   // 按 rune 判断长度后截断
来源：http://pe.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ng.haigaiapp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://kl.chemitech.net.cn

[E22] 字节长度与字符长度
来源：http://nv.shtwfgs.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://kz.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gb.jianghongdianzi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sc.newstarts.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xo.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lm.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cl.huixiangedu.cn

Ruby: s.bytesize;  s.length
来源：http://sr.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ws.huixinmuqiang.cn

================================================================================
来源：http://vq.nszjky.cn

F. 文件与目录
来源：http://my.asd995.cn

================================================================================
来源：http://gl.hnjuh.cn

[F01] 读取整个文件
来源：http://nk.asd995.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://aa.szsharing.cn

PHP:  file_get_contents("a.txt");
来源：http://tp.shxzskj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dj.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://al.gzmigu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zx.huixiangedu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://he.521024.cn

Ruby: File.read("a.txt")
来源：http://pk.jctech888.com.cn

C#:   File.ReadAllText("a.txt");
来源：http://ct.hahajie.cn

[F02] 逐行读取文件
来源：http://cp.huixiangedu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nc.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://kf.nicolike.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hm.colortex.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vk.lnxyls.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://he.gzmigu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fm.shxzukj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gy.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://sh.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://ls.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rf.haigaiapp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dp.haigaiapp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xm.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oq.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ow.chemitech.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://uo.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://qn.jianghongdianzi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ca.huanxung.cn

[F04] 追加写入文件
来源：http://cn.szsharing.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zz.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ea.huixinmuqiang.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pv.nicolike.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uc.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://uu.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ex.lnxyls.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yo.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bx.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://nj.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zl.huixiangedu.cn

PHP:  file_exists("a.txt");
来源：http://uv.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://oq.huixiangedu.cn

TS:   fs.existsSync("a.txt")
来源：http://un.yuexingan06.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fd.9csxet.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rd.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://hz.521024.cn

C#:   File.Exists("a.txt")
来源：http://dt.bjjhwx.cn

[F06] 删除文件
来源：http://nj.haigaiapp.cn

Py:   os.remove("a.txt")
来源：http://iv.hahajie.cn

PHP:  unlink("a.txt");
来源：http://mb.jctech888.com.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bj.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jh.hahajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://py.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://id.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://us.asd995.cn

C#:   File.Delete("a.txt");
来源：http://un.nszjky.cn

[F07] 创建目录（含多级）
来源：http://rd.shxzukj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ga.yuexingan06.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qs.chemitech.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://en.haigaiapp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ys.newstarts.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zd.colortex.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nu.jianghongdianzi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gz.bookmarksfly.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ex.shtwfgs.cn

[F08] 遍历目录
来源：http://um.bjjhwx.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ip.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bv.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://ow.szsharing.cn

TS:   fs.readdirSync("dir")
来源：http://aa.nszjky.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fv.haigaiapp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hl.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://av.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://xf.nszjky.cn

[F09] 获取文件大小
来源：http://xg.lnxyls.cn

Py:   os.path.getsize("a.txt")
来源：http://gt.hahajie.cn

PHP:  filesize("a.txt");
来源：http://ks.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://nv.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://nw.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yp.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nv.9csxet.cn

Ruby: File.size("a.txt")
来源：http://ne.521024.cn

C#:   new FileInfo("a.txt").Length
来源：http://lb.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://lh.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jx.hnjuh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rx.9csxet.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kt.shxzskj.cn

TS:   path.extname("a.txt")
来源：http://ti.chemitech.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sa.bjjhwx.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xi.nicolike.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sc.lnxyls.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bp.chemitech.net.cn

[F11] 复制与移动文件
来源：http://gp.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ab.shxzskj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hx.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tw.nszjky.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fp.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kg.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ng.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sa.yuexingan06.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vs.lnxyls.cn

[F12] CSV 读写
来源：http://ou.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pu.bookmarksfly.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nb.lnxyls.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uz.haigaiapp.cn

TS:   // 同上
来源：http://tj.bjjhwx.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pq.lnxyls.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dx.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dh.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lf.newstarts.cn

================================================================================
来源：http://ol.shtwfgs.cn

G. 面向对象
来源：http://in.lnxyls.cn

================================================================================
来源：http://iv.colortex.cn

[G01] 定义类
来源：http://oi.panjiajie.cn

Py:   class User: pass
来源：http://cp.haigaiapp.cn

PHP:  class User {}
来源：http://ge.nszjky.cn

JS:   class User {}
来源：http://ye.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://uf.colortex.cn

Java: class User {}
来源：http://ps.colortex.cn

Go:   type User struct { Name string }
来源：http://sp.shxzskj.cn

Ruby: class User; end
来源：http://ch.jctech888.com.cn

C#:   class User {}
来源：http://ws.bjjhwx.cn

[G02] 构造函数
来源：http://wx.9csxet.cn

Py:   def __init__(self, name): self.name = name
来源：http://vo.bjjhwx.cn

PHP:  public function __construct(public string $name) {}
来源：http://kz.asd995.cn

JS:   constructor(name) { this.name = name; }
来源：http://ga.panjiajie.cn

TS:   constructor(public name: string) {}
来源：http://ri.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://zx.szxytkj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lb.yuexingan06.cn

Ruby: def initialize(name); @name = name; end
来源：http://pa.nicolike.cn

C#:   public User(string name) { Name = name; }
来源：http://ba.huanxung.cn

[G03] 实例属性
来源：http://gk.wgjwhj.cn

Py:   self.name = "x"
来源：http://kt.newstarts.cn

PHP:  public string $name = "x";
来源：http://lb.shxzskj.cn

JS:   this.name = "x";
来源：http://az.521024.cn

TS:   name: string = "x";
来源：http://nf.szxytkj.cn

Java: private String name;
来源：http://ke.huixinmuqiang.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zv.shxzukj.cn

Ruby: @name = "x"
来源：http://ih.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://sh.szxytkj.cn

[G04] 定义方法
来源：http://yd.huixiangedu.cn

Py:   def greet(self): return self.name
来源：http://sg.szsharing.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zt.newstarts.cn

JS:   greet() { return this.name; }
来源：http://wc.huixinmuqiang.cn

TS:   greet(): string { return this.name; }
来源：http://xg.huixinmuqiang.cn

Java: String greet() { return name; }
来源：http://ip.hnjuh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jw.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://pc.szsharing.cn

C#:   public string Greet() => Name;
来源：http://yo.szsharing.cn

[G05] 继承
来源：http://sf.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://uv.asd995.cn

PHP:  class Admin extends User {}
来源：http://dm.huanxung.cn

JS:   class Admin extends User {}
来源：http://gu.yuntaijiaju.cn

TS:   class Admin extends User {}
来源：http://sl.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://im.bjjhwx.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jj.newstarts.cn

Ruby: class Admin < User; end
来源：http://yv.newstarts.cn

C#:   class Admin : User {}
来源：http://qr.lnxyls.cn

[G06] 重写方法
来源：http://li.yuntaijiaju.cn

Py:   def greet(self): return "admin"
来源：http://cc.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://lp.panjiajie.cn

JS:   greet() { return "admin"; }
来源：http://dx.huixiangedu.cn

TS:   greet(): string { return "admin"; }
来源：http://lf.jctech888.com.cn

Java: @Override String greet() { return "admin"; }
来源：http://yt.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pw.lnxyls.cn

Ruby: def greet; "admin"; end
来源：http://rn.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://tm.szxytkj.cn

[G07] 调用父类方法
来源：http://fs.yuntaijiaju.cn

Py:   super().greet()
来源：http://fe.shxzukj.cn

PHP:  parent::greet();
来源：http://hq.huixiangedu.cn

JS:   super.greet();
来源：http://nj.nszjky.cn

TS:   super.greet();
来源：http://xt.shxzukj.cn

Java: super.greet();
来源：http://tn.szxytkj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hi.bjjhwx.cn

Ruby: super
来源：http://eq.shxzskj.cn

C#:   base.Greet();
来源：http://az.shxzukj.cn

[G08] 静态方法与属性
来源：http://bj.hahajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ww.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://yl.jianghongdianzi.cn

JS:   static f() {}
来源：http://tc.shxzukj.cn

TS:   static f(): void {}
来源：http://yj.9csxet.cn

Java: static void f() {}
来源：http://bf.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ot.nszjky.cn

Ruby: def self.f; end
来源：http://eu.bjjhwx.cn

C#:   public static void F() {}
来源：http://zm.szsharing.cn

[G09] 接口 / 抽象类
来源：http://wa.9csxet.cn

Py:   from abc import ABC, abstractmethod
来源：http://zi.huanxung.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ix.huanxung.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kh.521024.cn

TS:   interface Shape { area(): number; }
来源：http://ep.yuntaijiaju.cn

Java: interface Shape { double area(); }
来源：http://gg.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://kk.panjiajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ii.9csxet.cn

C#:   interface IShape { double Area(); }
来源：http://ar.hahajie.cn

[G10] 访问控制
来源：http://xf.hahajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://fs.colortex.cn

PHP:  public / protected / private
来源：http://kc.521024.cn

JS:   #private 字段；其余公开
来源：http://yn.nszjky.cn

TS:   public / protected / private
来源：http://qq.9csxet.cn

Java: public / protected / private / 默认包级
来源：http://tx.gzmigu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sy.nszjky.cn

Ruby: public / protected / private
来源：http://dq.panjiajie.cn

C#:   public / protected / private / internal
来源：http://ou.szsharing.cn

[G11] getter / setter
来源：http://xh.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://uy.chemitech.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gp.huixinmuqiang.cn

JS:   get name() { return this._name; }
来源：http://xv.huixinmuqiang.cn

TS:   get name(): string { return this._name; }
来源：http://hx.521024.cn

Java: public String getName() { return name; }
来源：http://mu.hnjuh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gu.bjjhwx.cn

Ruby: attr_accessor :name
来源：http://qu.wgjwhj.cn

C#:   public string Name { get; set; }
来源：http://fg.haigaiapp.cn

[G12] 对象转字符串
来源：http://ub.panjiajie.cn

Py:   def __str__(self): return self.name
来源：http://yq.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vv.lnxyls.cn

JS:   toString() { return this.name; }
来源：http://gd.muxihuayi.cn

TS:   toString(): string { return this.name; }
来源：http://sp.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://uo.asd995.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cb.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://ui.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://qr.huixinmuqiang.cn

[G13] 判断对象类型
来源：http://wx.jctech888.com.cn

Py:   isinstance(u, User)
来源：http://ek.panjiajie.cn

PHP:  $u instanceof User
来源：http://lf.gzmigu.cn

JS:   u instanceof User
来源：http://gb.9csxet.cn

TS:   u instanceof User
来源：http://pc.muxihuayi.cn

Java: u instanceof User
来源：http://lh.bookmarksfly.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://da.9csxet.cn

Ruby: u.is_a?(User)
来源：http://wi.haigaiapp.cn

C#:   u is User
来源：http://ro.shxzskj.cn


<!-- 参考信息 -->