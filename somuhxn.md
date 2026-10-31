代发 wailian999

PHP:  number_format(1234567);
来源：http://mt.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mq.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ul.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ij.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uy.hahajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bg.colortex.cn

C#:   1234567.ToString("N0")
来源：http://ud.chemitech.net.cn

[E17] 首字母大写
来源：http://qz.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dv.9csxet.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ts.hnjuh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://my.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gv.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sp.huixiangedu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pb.lnxyls.cn

Ruby: s.capitalize
来源：http://hr.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://pn.szxytkj.cn

[E18] 模板占位符替换
来源：http://yr.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gh.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vj.shtwfgs.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zp.hnjuh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mk.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qn.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kv.hnjuh.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kd.hnjuh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dh.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://jr.nszjky.cn

Py:   s.splitlines()
来源：http://gb.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ek.nicolike.cn

JS:   s.split(/\r?\n/)
来源：http://ba.colortex.cn

TS:   s.split(/\r?\n/)
来源：http://vr.shtwfgs.cn

Java: s.lines().toList()
来源：http://rl.yuntaijiaju.cn

Go:   strings.Split(s, "\n")
来源：http://ue.wgjwhj.cn

Ruby: s.lines
来源：http://ez.panjiajie.cn

C#:   s.Split('\n')
来源：http://sq.shtwfgs.cn

[E20] 判断字符串是否为空
来源：http://xq.521024.cn

Py:   if not s:
来源：http://zx.haigaiapp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://io.newstarts.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tm.wgjwhj.cn

TS:   if (s === "") {}
来源：http://td.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://bi.9csxet.cn

Go:   if s == "" {}
来源：http://kq.hahajie.cn

Ruby: if s.empty?
来源：http://zw.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oo.szsharing.cn

[E21] 超长截断加省略号
来源：http://sw.huixiangedu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vs.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bj.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hu.muxihuayi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://uj.yuntaijiaju.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://na.nszjky.cn

Go:   // 按 rune 判断长度后截断
来源：http://gq.jctech888.com.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xz.szxytkj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pv.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://zr.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bk.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jh.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://av.hnjuh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vr.bookmarksfly.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ng.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wm.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://ep.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gb.chemitech.net.cn

================================================================================
来源：http://vg.521024.cn

F. 文件与目录
来源：http://yb.huixiangedu.cn

================================================================================
来源：http://cw.nicolike.cn

[F01] 读取整个文件
来源：http://ag.colortex.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cu.jctech888.com.cn

PHP:  file_get_contents("a.txt");
来源：http://lg.shtwfgs.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pc.asd995.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://di.521024.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ll.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mc.chemitech.net.cn

Ruby: File.read("a.txt")
来源：http://vu.9csxet.cn

C#:   File.ReadAllText("a.txt");
来源：http://hg.hahajie.cn

[F02] 逐行读取文件
来源：http://ya.hahajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://po.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jf.9csxet.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xw.jctech888.com.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yd.shtwfgs.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://di.jianghongdianzi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ny.shxzskj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xj.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://og.panjiajie.cn

[F03] 写入文件（覆盖）
来源：http://wu.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xw.wgjwhj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nz.521024.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bh.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vb.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://pb.jctech888.com.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://md.hahajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://rj.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eb.huixiangedu.cn

[F04] 追加写入文件
来源：http://xh.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ms.gzmigu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ub.muxihuayi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://is.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zt.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fv.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://co.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ag.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zo.521024.cn

[F05] 判断文件或目录是否存在
来源：http://by.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gx.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://tl.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://nt.lnxyls.cn

TS:   fs.existsSync("a.txt")
来源：http://dx.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://io.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zu.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://pv.muxihuayi.cn

C#:   File.Exists("a.txt")
来源：http://sh.nszjky.cn

[F06] 删除文件
来源：http://bv.hahajie.cn

Py:   os.remove("a.txt")
来源：http://lz.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://dd.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://uu.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kl.shtwfgs.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ug.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://op.bjjhwx.cn

Ruby: File.delete("a.txt")
来源：http://zc.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://wy.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://zh.521024.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://yd.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vq.nicolike.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gy.colortex.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yi.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tm.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://eg.521024.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xu.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fy.huanxung.cn

[F08] 遍历目录
来源：http://lk.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mi.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rk.lnxyls.cn

JS:   fs.readdirSync("dir")
来源：http://as.muxihuayi.cn

TS:   fs.readdirSync("dir")
来源：http://rp.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yh.nicolike.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://st.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://sf.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://wk.asd995.cn

[F09] 获取文件大小
来源：http://yw.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://zu.huixinmuqiang.cn

PHP:  filesize("a.txt");
来源：http://km.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://bk.colortex.cn

TS:   fs.statSync("a.txt").size
来源：http://rb.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vi.shxzukj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://cg.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://gx.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://at.shxzskj.cn

[F10] 取文件扩展名 / 文件名
来源：http://kz.bookmarksfly.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://uh.yuexingan06.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wt.nicolike.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ea.shxzskj.cn

TS:   path.extname("a.txt")
来源：http://xt.newstarts.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rt.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oi.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sv.colortex.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fe.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://bt.bookmarksfly.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://eb.huixiangedu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cx.colortex.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iz.muxihuayi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mo.panjiajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ou.lnxyls.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bp.nszjky.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://al.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yv.nicolike.cn

[F12] CSV 读写
来源：http://kk.shxzukj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ox.chemitech.net.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rj.9csxet.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uc.nicolike.cn

TS:   // 同上
来源：http://mq.panjiajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fs.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ka.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tz.colortex.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ck.newstarts.cn

================================================================================
来源：http://xa.521024.cn

G. 面向对象
来源：http://ag.szxytkj.cn

================================================================================
来源：http://dh.panjiajie.cn

[G01] 定义类
来源：http://sf.jctech888.com.cn

Py:   class User: pass
来源：http://jk.nszjky.cn

PHP:  class User {}
来源：http://yo.hahajie.cn

JS:   class User {}
来源：http://hd.nicolike.cn

TS:   class User { name: string = ""; }
来源：http://zt.asd995.cn

Java: class User {}
来源：http://tr.nszjky.cn

Go:   type User struct { Name string }
来源：http://ah.521024.cn

Ruby: class User; end
来源：http://db.shxzukj.cn

C#:   class User {}
来源：http://du.wgjwhj.cn

[G02] 构造函数
来源：http://ec.panjiajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://vt.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://hf.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://eu.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://bn.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://ri.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://yp.shxzskj.cn

Ruby: def initialize(name); @name = name; end
来源：http://cf.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://bc.szxytkj.cn

[G03] 实例属性
来源：http://se.huixiangedu.cn

Py:   self.name = "x"
来源：http://tb.lnxyls.cn

PHP:  public string $name = "x";
来源：http://mc.shxzskj.cn

JS:   this.name = "x";
来源：http://bd.huixiangedu.cn

TS:   name: string = "x";
来源：http://hf.shxzskj.cn

Java: private String name;
来源：http://sq.panjiajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ez.wgjwhj.cn

Ruby: @name = "x"
来源：http://ns.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://mp.hahajie.cn

[G04] 定义方法
来源：http://tw.yuexingan06.cn

Py:   def greet(self): return self.name
来源：http://je.yuntaijiaju.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ca.hnjuh.cn

JS:   greet() { return this.name; }
来源：http://wg.chemitech.net.cn

TS:   greet(): string { return this.name; }
来源：http://hc.9csxet.cn

Java: String greet() { return name; }
来源：http://qh.bjjhwx.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://av.huixiangedu.cn

Ruby: def greet; @name; end
来源：http://sb.hahajie.cn

C#:   public string Greet() => Name;
来源：http://kr.hahajie.cn

[G05] 继承
来源：http://lk.shxzskj.cn

Py:   class Admin(User): pass
来源：http://jw.lnxyls.cn

PHP:  class Admin extends User {}
来源：http://gt.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://oe.szxytkj.cn

TS:   class Admin extends User {}
来源：http://mn.szxytkj.cn

Java: class Admin extends User {}
来源：http://my.bjjhwx.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xi.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://jb.lnxyls.cn

C#:   class Admin : User {}
来源：http://zx.muxihuayi.cn

[G06] 重写方法
来源：http://io.lnxyls.cn

Py:   def greet(self): return "admin"
来源：http://na.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fk.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://np.nicolike.cn

TS:   greet(): string { return "admin"; }
来源：http://md.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://ps.haigaiapp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ek.huixinmuqiang.cn

Ruby: def greet; "admin"; end
来源：http://wo.521024.cn

C#:   public override string Greet() => "admin";
来源：http://ix.jianghongdianzi.cn

[G07] 调用父类方法
来源：http://cs.nszjky.cn

Py:   super().greet()
来源：http://re.9csxet.cn

PHP:  parent::greet();
来源：http://uv.yuntaijiaju.cn

JS:   super.greet();
来源：http://mb.wgjwhj.cn

TS:   super.greet();
来源：http://uc.szxytkj.cn

Java: super.greet();
来源：http://pm.nicolike.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sj.lnxyls.cn

Ruby: super
来源：http://vl.huixinmuqiang.cn

C#:   base.Greet();
来源：http://en.colortex.cn

[G08] 静态方法与属性
来源：http://qw.9csxet.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kr.nicolike.cn

PHP:  public static function f() {}
来源：http://dh.colortex.cn

JS:   static f() {}
来源：http://ba.gzmigu.cn

TS:   static f(): void {}
来源：http://iw.hahajie.cn

Java: static void f() {}
来源：http://ty.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wt.shtwfgs.cn

Ruby: def self.f; end
来源：http://fx.huixiangedu.cn

C#:   public static void F() {}
来源：http://xm.huanxung.cn

[G09] 接口 / 抽象类
来源：http://mj.hnjuh.cn

Py:   from abc import ABC, abstractmethod
来源：http://sd.nicolike.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ol.gzmigu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ok.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://sw.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://zc.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://hl.jianghongdianzi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mj.shtwfgs.cn

C#:   interface IShape { double Area(); }
来源：http://gz.jctech888.com.cn

[G10] 访问控制
来源：http://un.jianghongdianzi.cn

Py:   约定 _protected / __private（不强制）
来源：http://ts.panjiajie.cn

PHP:  public / protected / private
来源：http://tr.yuntaijiaju.cn

JS:   #private 字段；其余公开
来源：http://pg.yuntaijiaju.cn

TS:   public / protected / private
来源：http://cl.9csxet.cn

Java: public / protected / private / 默认包级
来源：http://ii.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rq.yuntaijiaju.cn

Ruby: public / protected / private
来源：http://rw.wgjwhj.cn

C#:   public / protected / private / internal
来源：http://cp.bjjhwx.cn

[G11] getter / setter
来源：http://le.szxytkj.cn

Py:   @property 与 @x.setter
来源：http://ax.jianghongdianzi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gd.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://bu.shxzukj.cn

TS:   get name(): string { return this._name; }
来源：http://vp.jctech888.com.cn

Java: public String getName() { return name; }
来源：http://hm.jctech888.com.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gu.huixinmuqiang.cn

Ruby: attr_accessor :name
来源：http://wi.asd995.cn

C#:   public string Name { get; set; }
来源：http://md.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://pc.huixiangedu.cn

Py:   def __str__(self): return self.name
来源：http://vx.huanxung.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ze.muxihuayi.cn

JS:   toString() { return this.name; }
来源：http://bo.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://tz.gzmigu.cn

Java: @Override public String toString() { return name; }
来源：http://hx.nszjky.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fm.9csxet.cn

Ruby: def to_s; @name; end
来源：http://as.nszjky.cn

C#:   public override string ToString() => Name;
来源：http://bk.chemitech.net.cn

[G13] 判断对象类型
来源：http://bs.nicolike.cn

Py:   isinstance(u, User)
来源：http://mw.muxihuayi.cn

PHP:  $u instanceof User
来源：http://aa.lnxyls.cn

JS:   u instanceof User
来源：http://og.shxzukj.cn

TS:   u instanceof User
来源：http://sm.haigaiapp.cn

Java: u instanceof User
来源：http://ve.gzmigu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://er.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://rv.asd995.cn

C#:   u is User
来源：http://gx.hnjuh.cn

[G14] 数据类 / record
来源：http://bx.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ta.chemitech.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://cv.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lz.muxihuayi.cn

TS:   type User = { name: string; age: number };
来源：http://jw.haigaiapp.cn

Java: record User(String name, int age) {}
来源：http://su.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://ym.panjiajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cn.hnjuh.cn


<!-- 参考信息 -->