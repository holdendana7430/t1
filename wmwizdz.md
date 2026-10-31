代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://kr.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ak.yuexingan06.cn

[E16] 数字千分位
来源：http://ze.muxihuayi.cn

Py:   f"{1234567:,}"
来源：http://lj.nszjky.cn

PHP:  number_format(1234567);
来源：http://wf.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cn.nszjky.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fq.muxihuayi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yq.nicolike.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vb.gzmigu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hj.szsharing.cn

C#:   1234567.ToString("N0")
来源：http://ef.521024.cn

[E17] 首字母大写
来源：http://yf.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ef.szsharing.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ie.szsharing.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kk.jianghongdianzi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vv.asd995.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rg.newstarts.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zq.colortex.cn

Ruby: s.capitalize
来源：http://qn.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ls.gzmigu.cn

[E18] 模板占位符替换
来源：http://wt.jctech888.com.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sh.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://sn.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gu.hahajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kw.newstarts.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://yu.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kx.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rp.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qx.newstarts.cn

[E19] 多行文本按行拆分
来源：http://jr.haigaiapp.cn

Py:   s.splitlines()
来源：http://ys.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xh.huanxung.cn

JS:   s.split(/\r?\n/)
来源：http://mz.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://im.newstarts.cn

Java: s.lines().toList()
来源：http://zw.huixinmuqiang.cn

Go:   strings.Split(s, "\n")
来源：http://ow.huixinmuqiang.cn

Ruby: s.lines
来源：http://uy.huanxung.cn

C#:   s.Split('\n')
来源：http://ow.hnjuh.cn

[E20] 判断字符串是否为空
来源：http://wo.muxihuayi.cn

Py:   if not s:
来源：http://dh.shxzukj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ic.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mp.panjiajie.cn

TS:   if (s === "") {}
来源：http://ht.shxzukj.cn

Java: if (s.isEmpty()) {}
来源：http://jb.muxihuayi.cn

Go:   if s == "" {}
来源：http://ht.hahajie.cn

Ruby: if s.empty?
来源：http://nh.szxytkj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kw.nicolike.cn

[E21] 超长截断加省略号
来源：http://cw.asd995.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lg.9csxet.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://en.gzmigu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gt.muxihuayi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qg.hahajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ru.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://xq.shxzukj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://bg.hnjuh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ut.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://cd.jctech888.com.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uj.wgjwhj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sg.huixinmuqiang.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pk.yuexingan06.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gg.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hu.huanxung.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://uq.nszjky.cn

Ruby: s.bytesize;  s.length
来源：http://hz.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://tj.haigaiapp.cn

================================================================================
来源：http://we.shxzskj.cn

F. 文件与目录
来源：http://zq.jianghongdianzi.cn

================================================================================
来源：http://rh.muxihuayi.cn

[F01] 读取整个文件
来源：http://mk.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zf.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://bf.panjiajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vu.hnjuh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ud.muxihuayi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rj.asd995.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://el.haigaiapp.cn

Ruby: File.read("a.txt")
来源：http://mn.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://yo.huanxung.cn

[F02] 逐行读取文件
来源：http://ks.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dw.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ia.shtwfgs.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wl.nicolike.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://la.yuntaijiaju.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jw.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lp.gzmigu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lm.shxzukj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nz.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://em.szxytkj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ok.wgjwhj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tq.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zu.hahajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://he.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ix.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nz.bookmarksfly.cn

Ruby: File.write("a.txt", "hi")
来源：http://qz.panjiajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ir.haigaiapp.cn

[F04] 追加写入文件
来源：http://jr.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xe.lnxyls.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qv.huixinmuqiang.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mf.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hb.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nq.chemitech.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lt.gzmigu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vp.nszjky.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ba.gzmigu.cn

[F05] 判断文件或目录是否存在
来源：http://os.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mn.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://hb.wgjwhj.cn

JS:   fs.existsSync("a.txt")
来源：http://dh.bookmarksfly.cn

TS:   fs.existsSync("a.txt")
来源：http://dx.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ii.haigaiapp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://be.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://kq.asd995.cn

C#:   File.Exists("a.txt")
来源：http://bk.521024.cn

[F06] 删除文件
来源：http://dv.szxytkj.cn

Py:   os.remove("a.txt")
来源：http://ey.hahajie.cn

PHP:  unlink("a.txt");
来源：http://ac.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rw.asd995.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wp.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cv.hnjuh.cn

Go:   os.Remove("a.txt")
来源：http://me.yuexingan06.cn

Ruby: File.delete("a.txt")
来源：http://wh.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://fu.nicolike.cn

[F07] 创建目录（含多级）
来源：http://an.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://uo.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hx.chemitech.net.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wi.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hq.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mm.nicolike.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dj.colortex.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zp.newstarts.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ug.jianghongdianzi.cn

[F08] 遍历目录
来源：http://jb.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cf.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xx.jianghongdianzi.cn

JS:   fs.readdirSync("dir")
来源：http://bz.huixinmuqiang.cn

TS:   fs.readdirSync("dir")
来源：http://xp.wgjwhj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://at.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xj.colortex.cn

Ruby: Dir.children("dir")
来源：http://nj.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://ot.9csxet.cn

[F09] 获取文件大小
来源：http://pf.lnxyls.cn

Py:   os.path.getsize("a.txt")
来源：http://fp.bookmarksfly.cn

PHP:  filesize("a.txt");
来源：http://xi.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://ck.hnjuh.cn

TS:   fs.statSync("a.txt").size
来源：http://qk.jianghongdianzi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ly.newstarts.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jf.panjiajie.cn

Ruby: File.size("a.txt")
来源：http://we.muxihuayi.cn

C#:   new FileInfo("a.txt").Length
来源：http://il.szxytkj.cn

[F10] 取文件扩展名 / 文件名
来源：http://jw.shxzukj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mz.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://la.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uq.lnxyls.cn

TS:   path.extname("a.txt")
来源：http://un.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fy.asd995.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://md.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mr.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uh.asd995.cn

[F11] 复制与移动文件
来源：http://jk.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://te.panjiajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dj.bookmarksfly.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mu.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ze.chemitech.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://so.colortex.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ng.hnjuh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uw.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://eb.yuexingan06.cn

[F12] CSV 读写
来源：http://av.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sx.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ow.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://sq.bjjhwx.cn

TS:   // 同上
来源：http://dl.shtwfgs.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://nf.bjjhwx.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://aj.hahajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jx.huixinmuqiang.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://oq.huixiangedu.cn

================================================================================
来源：http://kd.shxzukj.cn

G. 面向对象
来源：http://pj.hnjuh.cn

================================================================================
来源：http://gm.haigaiapp.cn

[G01] 定义类
来源：http://gy.huixiangedu.cn

Py:   class User: pass
来源：http://ie.panjiajie.cn

PHP:  class User {}
来源：http://ad.hahajie.cn

JS:   class User {}
来源：http://eo.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://ux.521024.cn

Java: class User {}
来源：http://bd.colortex.cn

Go:   type User struct { Name string }
来源：http://ol.szxytkj.cn

Ruby: class User; end
来源：http://xp.yuexingan06.cn

C#:   class User {}
来源：http://xj.bjjhwx.cn

[G02] 构造函数
来源：http://ev.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://vc.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://af.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://wm.haigaiapp.cn

TS:   constructor(public name: string) {}
来源：http://sb.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://at.huanxung.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ic.jianghongdianzi.cn

Ruby: def initialize(name); @name = name; end
来源：http://kg.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://wl.shtwfgs.cn

[G03] 实例属性
来源：http://ud.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://ij.521024.cn

PHP:  public string $name = "x";
来源：http://bt.bookmarksfly.cn

JS:   this.name = "x";
来源：http://wy.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://ai.jianghongdianzi.cn

Java: private String name;
来源：http://ek.shxzskj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zi.shxzskj.cn

Ruby: @name = "x"
来源：http://fo.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://px.huixinmuqiang.cn

[G04] 定义方法
来源：http://oy.asd995.cn

Py:   def greet(self): return self.name
来源：http://fh.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ks.bjjhwx.cn

JS:   greet() { return this.name; }
来源：http://ik.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://ae.nszjky.cn

Java: String greet() { return name; }
来源：http://oe.jianghongdianzi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kg.hnjuh.cn

Ruby: def greet; @name; end
来源：http://ix.gzmigu.cn

C#:   public string Greet() => Name;
来源：http://gv.9csxet.cn

[G05] 继承
来源：http://fp.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://cb.huixiangedu.cn

PHP:  class Admin extends User {}
来源：http://rk.nicolike.cn

JS:   class Admin extends User {}
来源：http://kq.panjiajie.cn

TS:   class Admin extends User {}
来源：http://oh.521024.cn

Java: class Admin extends User {}
来源：http://zf.wgjwhj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ye.bookmarksfly.cn

Ruby: class Admin < User; end
来源：http://hg.shxzukj.cn

C#:   class Admin : User {}
来源：http://ah.wgjwhj.cn

[G06] 重写方法
来源：http://ok.yuntaijiaju.cn

Py:   def greet(self): return "admin"
来源：http://tf.huixinmuqiang.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hu.panjiajie.cn

JS:   greet() { return "admin"; }
来源：http://ft.jianghongdianzi.cn

TS:   greet(): string { return "admin"; }
来源：http://ko.huixinmuqiang.cn

Java: @Override String greet() { return "admin"; }
来源：http://dm.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sm.huixinmuqiang.cn

Ruby: def greet; "admin"; end
来源：http://ed.yuexingan06.cn

C#:   public override string Greet() => "admin";
来源：http://ch.nicolike.cn

[G07] 调用父类方法
来源：http://wq.hnjuh.cn

Py:   super().greet()
来源：http://zv.shtwfgs.cn

PHP:  parent::greet();
来源：http://zo.nszjky.cn

JS:   super.greet();
来源：http://lr.huixinmuqiang.cn

TS:   super.greet();
来源：http://rf.bjjhwx.cn

Java: super.greet();
来源：http://sf.chemitech.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dn.bjjhwx.cn

Ruby: super
来源：http://oo.nszjky.cn

C#:   base.Greet();
来源：http://hr.newstarts.cn

[G08] 静态方法与属性
来源：http://xj.hahajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://aq.wgjwhj.cn

PHP:  public static function f() {}
来源：http://kg.szxytkj.cn

JS:   static f() {}
来源：http://cp.9csxet.cn

TS:   static f(): void {}
来源：http://en.huanxung.cn

Java: static void f() {}
来源：http://fn.shxzukj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://iz.newstarts.cn

Ruby: def self.f; end
来源：http://ns.asd995.cn

C#:   public static void F() {}
来源：http://qw.panjiajie.cn

[G09] 接口 / 抽象类
来源：http://uk.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://qu.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wv.jianghongdianzi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nb.huixinmuqiang.cn

TS:   interface Shape { area(): number; }
来源：http://gq.chemitech.net.cn

Java: interface Shape { double area(); }
来源：http://au.hahajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://qh.shxzukj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wm.huixiangedu.cn

C#:   interface IShape { double Area(); }
来源：http://fy.nicolike.cn

[G10] 访问控制
来源：http://os.huixinmuqiang.cn

Py:   约定 _protected / __private（不强制）
来源：http://zs.asd995.cn

PHP:  public / protected / private
来源：http://pu.yuexingan06.cn

JS:   #private 字段；其余公开
来源：http://ty.hnjuh.cn

TS:   public / protected / private
来源：http://bg.newstarts.cn

Java: public / protected / private / 默认包级
来源：http://qf.nicolike.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ok.nicolike.cn

Ruby: public / protected / private
来源：http://fw.shxzukj.cn

C#:   public / protected / private / internal
来源：http://bk.haigaiapp.cn

[G11] getter / setter
来源：http://gs.9csxet.cn

Py:   @property 与 @x.setter
来源：http://en.jctech888.com.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cd.jianghongdianzi.cn

JS:   get name() { return this._name; }
来源：http://gd.9csxet.cn

TS:   get name(): string { return this._name; }
来源：http://gu.yuexingan06.cn

Java: public String getName() { return name; }
来源：http://ij.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ig.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://sz.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://xh.szsharing.cn

[G12] 对象转字符串
来源：http://jv.huixiangedu.cn

Py:   def __str__(self): return self.name
来源：http://gw.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tr.lnxyls.cn

JS:   toString() { return this.name; }
来源：http://pt.colortex.cn

TS:   toString(): string { return this.name; }
来源：http://ba.jianghongdianzi.cn

Java: @Override public String toString() { return name; }
来源：http://vs.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pz.jianghongdianzi.cn

Ruby: def to_s; @name; end
来源：http://lr.nicolike.cn

C#:   public override string ToString() => Name;
来源：http://xj.huanxung.cn

[G13] 判断对象类型
来源：http://xf.nszjky.cn

Py:   isinstance(u, User)
来源：http://ev.9csxet.cn

PHP:  $u instanceof User
来源：http://om.521024.cn

JS:   u instanceof User
来源：http://ed.shxzukj.cn

TS:   u instanceof User
来源：http://yp.jctech888.com.cn

Java: u instanceof User
来源：http://xn.nszjky.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ed.lnxyls.cn

Ruby: u.is_a?(User)
来源：http://kr.gzmigu.cn

C#:   u is User
来源：http://ra.shxzskj.cn

[G14] 数据类 / record
来源：http://rz.muxihuayi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qx.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://nw.shxzukj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vs.nicolike.cn


<!-- 参考信息 -->