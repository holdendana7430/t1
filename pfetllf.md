代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sy.newstarts.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ff.521024.cn

Ruby: s.capitalize
来源：http://kv.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://cd.yuexingan06.cn

[E18] 模板占位符替换
来源：http://eo.shxzukj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://nq.szxytkj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ec.shxzskj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jr.shtwfgs.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wr.huixiangedu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bi.huixinmuqiang.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vc.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ky.jctech888.com.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mp.521024.cn

[E19] 多行文本按行拆分
来源：http://rc.asd995.cn

Py:   s.splitlines()
来源：http://ne.9csxet.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pj.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://dl.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://qw.colortex.cn

Java: s.lines().toList()
来源：http://hk.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://hl.bookmarksfly.cn

Ruby: s.lines
来源：http://ff.bjjhwx.cn

C#:   s.Split('\n')
来源：http://sy.nszjky.cn

[E20] 判断字符串是否为空
来源：http://mf.yuntaijiaju.cn

Py:   if not s:
来源：http://wt.colortex.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tj.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zc.shxzskj.cn

TS:   if (s === "") {}
来源：http://pl.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://ni.jctech888.com.cn

Go:   if s == "" {}
来源：http://qt.shxzskj.cn

Ruby: if s.empty?
来源：http://ae.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tz.yuntaijiaju.cn

[E21] 超长截断加省略号
来源：http://ie.huixiangedu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kt.newstarts.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dn.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yw.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xl.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nf.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://vt.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kv.chemitech.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tj.hnjuh.cn

[E22] 字节长度与字符长度
来源：http://vo.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ye.yuexingan06.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hv.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ql.huixiangedu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hs.chemitech.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ht.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rp.521024.cn

Ruby: s.bytesize;  s.length
来源：http://xx.nicolike.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ul.gzmigu.cn

================================================================================
来源：http://fz.shxzskj.cn

F. 文件与目录
来源：http://ye.lnxyls.cn

================================================================================
来源：http://wh.lnxyls.cn

[F01] 读取整个文件
来源：http://bf.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jt.hahajie.cn

PHP:  file_get_contents("a.txt");
来源：http://xo.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qf.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nd.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vo.hahajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rz.hnjuh.cn

Ruby: File.read("a.txt")
来源：http://tc.jianghongdianzi.cn

C#:   File.ReadAllText("a.txt");
来源：http://sl.hnjuh.cn

[F02] 逐行读取文件
来源：http://fy.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ts.huanxung.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dy.newstarts.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jp.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xn.haigaiapp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ss.gzmigu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zc.nicolike.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://so.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xt.lnxyls.cn

[F03] 写入文件（覆盖）
来源：http://az.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lf.shxzukj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://th.huixinmuqiang.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jp.9csxet.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hf.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bh.jctech888.com.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oh.lnxyls.cn

Ruby: File.write("a.txt", "hi")
来源：http://mk.nszjky.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kg.wgjwhj.cn

[F04] 追加写入文件
来源：http://hi.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://rt.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xb.szxytkj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zn.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bm.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rw.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dj.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gp.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bf.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://ui.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zu.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://bu.wgjwhj.cn

JS:   fs.existsSync("a.txt")
来源：http://nm.bookmarksfly.cn

TS:   fs.existsSync("a.txt")
来源：http://gx.nszjky.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bc.bookmarksfly.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ev.hahajie.cn

Ruby: File.exist?("a.txt")
来源：http://rw.huanxung.cn

C#:   File.Exists("a.txt")
来源：http://hm.shxzukj.cn

[F06] 删除文件
来源：http://kv.nszjky.cn

Py:   os.remove("a.txt")
来源：http://zx.muxihuayi.cn

PHP:  unlink("a.txt");
来源：http://ss.nszjky.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hh.szxytkj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qr.newstarts.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://rb.asd995.cn

Go:   os.Remove("a.txt")
来源：http://ck.wgjwhj.cn

Ruby: File.delete("a.txt")
来源：http://st.yuexingan06.cn

C#:   File.Delete("a.txt");
来源：http://li.panjiajie.cn

[F07] 创建目录（含多级）
来源：http://qa.huixinmuqiang.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fj.shxzukj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://fb.shxzskj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fx.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xs.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yr.huixiangedu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://rg.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xw.haigaiapp.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gd.hahajie.cn

[F08] 遍历目录
来源：http://vf.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://aq.shxzskj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xv.521024.cn

JS:   fs.readdirSync("dir")
来源：http://yx.nszjky.cn

TS:   fs.readdirSync("dir")
来源：http://jv.bjjhwx.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ti.newstarts.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nx.bookmarksfly.cn

Ruby: Dir.children("dir")
来源：http://cu.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://px.huixinmuqiang.cn

[F09] 获取文件大小
来源：http://ma.asd995.cn

Py:   os.path.getsize("a.txt")
来源：http://oo.newstarts.cn

PHP:  filesize("a.txt");
来源：http://bh.yuntaijiaju.cn

JS:   fs.statSync("a.txt").size
来源：http://ya.szsharing.cn

TS:   fs.statSync("a.txt").size
来源：http://ne.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pw.chemitech.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qm.muxihuayi.cn

Ruby: File.size("a.txt")
来源：http://wh.gzmigu.cn

C#:   new FileInfo("a.txt").Length
来源：http://mt.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://zt.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ek.shtwfgs.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zb.jianghongdianzi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rn.jctech888.com.cn

TS:   path.extname("a.txt")
来源：http://ge.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fs.chemitech.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://no.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://az.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cz.bjjhwx.cn

[F11] 复制与移动文件
来源：http://qs.shxzskj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ev.hnjuh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nz.9csxet.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sk.gzmigu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://eo.muxihuayi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xy.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://he.shtwfgs.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sm.gzmigu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://di.jctech888.com.cn

[F12] CSV 读写
来源：http://kk.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oe.colortex.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://we.panjiajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ci.hnjuh.cn

TS:   // 同上
来源：http://oj.shtwfgs.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zx.huanxung.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qc.newstarts.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://js.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ku.nszjky.cn

================================================================================
来源：http://qk.colortex.cn

G. 面向对象
来源：http://wx.asd995.cn

================================================================================
来源：http://mt.9csxet.cn

[G01] 定义类
来源：http://hs.hahajie.cn

Py:   class User: pass
来源：http://za.521024.cn

PHP:  class User {}
来源：http://bn.gzmigu.cn

JS:   class User {}
来源：http://sp.haigaiapp.cn

TS:   class User { name: string = ""; }
来源：http://yh.gzmigu.cn

Java: class User {}
来源：http://sj.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://yp.shtwfgs.cn

Ruby: class User; end
来源：http://iq.szsharing.cn

C#:   class User {}
来源：http://sb.huixiangedu.cn

[G02] 构造函数
来源：http://jt.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://hm.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://wg.muxihuayi.cn

JS:   constructor(name) { this.name = name; }
来源：http://zf.asd995.cn

TS:   constructor(public name: string) {}
来源：http://yz.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://qz.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ce.huanxung.cn

Ruby: def initialize(name); @name = name; end
来源：http://fr.asd995.cn

C#:   public User(string name) { Name = name; }
来源：http://xp.haigaiapp.cn

[G03] 实例属性
来源：http://wg.wgjwhj.cn

Py:   self.name = "x"
来源：http://cd.huixinmuqiang.cn

PHP:  public string $name = "x";
来源：http://qd.bjjhwx.cn

JS:   this.name = "x";
来源：http://yl.shxzukj.cn

TS:   name: string = "x";
来源：http://bx.huixiangedu.cn

Java: private String name;
来源：http://im.haigaiapp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bw.bookmarksfly.cn

Ruby: @name = "x"
来源：http://uc.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://ka.9csxet.cn

[G04] 定义方法
来源：http://ix.bjjhwx.cn

Py:   def greet(self): return self.name
来源：http://jc.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cy.jianghongdianzi.cn

JS:   greet() { return this.name; }
来源：http://lo.huanxung.cn

TS:   greet(): string { return this.name; }
来源：http://cd.shxzukj.cn

Java: String greet() { return name; }
来源：http://nk.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nv.szxytkj.cn

Ruby: def greet; @name; end
来源：http://ij.nicolike.cn

C#:   public string Greet() => Name;
来源：http://aw.colortex.cn

[G05] 继承
来源：http://mu.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://qo.nicolike.cn

PHP:  class Admin extends User {}
来源：http://xu.haigaiapp.cn

JS:   class Admin extends User {}
来源：http://hx.shxzskj.cn

TS:   class Admin extends User {}
来源：http://zp.asd995.cn

Java: class Admin extends User {}
来源：http://nw.muxihuayi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bg.haigaiapp.cn

Ruby: class Admin < User; end
来源：http://hw.haigaiapp.cn

C#:   class Admin : User {}
来源：http://sw.huanxung.cn

[G06] 重写方法
来源：http://ee.wgjwhj.cn

Py:   def greet(self): return "admin"
来源：http://gh.hnjuh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hv.yuexingan06.cn

JS:   greet() { return "admin"; }
来源：http://eu.shtwfgs.cn

TS:   greet(): string { return "admin"; }
来源：http://br.panjiajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://yd.bookmarksfly.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qn.shxzukj.cn

Ruby: def greet; "admin"; end
来源：http://no.9csxet.cn

C#:   public override string Greet() => "admin";
来源：http://ve.bookmarksfly.cn

[G07] 调用父类方法
来源：http://gs.shxzukj.cn

Py:   super().greet()
来源：http://au.shxzskj.cn

PHP:  parent::greet();
来源：http://lb.szxytkj.cn

JS:   super.greet();
来源：http://dr.huixiangedu.cn

TS:   super.greet();
来源：http://rm.muxihuayi.cn

Java: super.greet();
来源：http://wk.jctech888.com.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wo.shxzskj.cn

Ruby: super
来源：http://hf.wgjwhj.cn

C#:   base.Greet();
来源：http://mg.hahajie.cn

[G08] 静态方法与属性
来源：http://di.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rl.gzmigu.cn

PHP:  public static function f() {}
来源：http://fp.haigaiapp.cn

JS:   static f() {}
来源：http://gr.wgjwhj.cn

TS:   static f(): void {}
来源：http://fm.panjiajie.cn

Java: static void f() {}
来源：http://zn.yuntaijiaju.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ug.yuexingan06.cn

Ruby: def self.f; end
来源：http://ba.nicolike.cn

C#:   public static void F() {}
来源：http://be.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://ig.yuexingan06.cn

Py:   from abc import ABC, abstractmethod
来源：http://dd.wgjwhj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ic.wgjwhj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://uh.lnxyls.cn

TS:   interface Shape { area(): number; }
来源：http://td.colortex.cn

Java: interface Shape { double area(); }
来源：http://ca.shxzukj.cn

Go:   type Shape interface { Area() float64 }
来源：http://az.szxytkj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mf.asd995.cn

C#:   interface IShape { double Area(); }
来源：http://zi.szsharing.cn

[G10] 访问控制
来源：http://pz.521024.cn

Py:   约定 _protected / __private（不强制）
来源：http://fa.chemitech.net.cn

PHP:  public / protected / private
来源：http://qv.bookmarksfly.cn

JS:   #private 字段；其余公开
来源：http://mt.shtwfgs.cn

TS:   public / protected / private
来源：http://is.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://pm.jianghongdianzi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tq.9csxet.cn

Ruby: public / protected / private
来源：http://ad.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://yi.newstarts.cn

[G11] getter / setter
来源：http://ao.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://ha.jianghongdianzi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ii.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://fb.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://qt.szxytkj.cn

Java: public String getName() { return name; }
来源：http://xv.nszjky.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yj.haigaiapp.cn

Ruby: attr_accessor :name
来源：http://ee.nszjky.cn

C#:   public string Name { get; set; }
来源：http://ia.wgjwhj.cn

[G12] 对象转字符串
来源：http://rx.nszjky.cn

Py:   def __str__(self): return self.name
来源：http://sm.jctech888.com.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lz.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://zk.nszjky.cn

TS:   toString(): string { return this.name; }
来源：http://yg.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://wy.huanxung.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ss.huanxung.cn

Ruby: def to_s; @name; end
来源：http://gl.shxzskj.cn

C#:   public override string ToString() => Name;
来源：http://pz.szxytkj.cn

[G13] 判断对象类型
来源：http://bi.hnjuh.cn

Py:   isinstance(u, User)
来源：http://da.shtwfgs.cn

PHP:  $u instanceof User
来源：http://ef.521024.cn

JS:   u instanceof User
来源：http://gs.wgjwhj.cn

TS:   u instanceof User
来源：http://zm.nszjky.cn

Java: u instanceof User
来源：http://nl.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jy.szsharing.cn

Ruby: u.is_a?(User)
来源：http://qq.panjiajie.cn

C#:   u is User
来源：http://mv.521024.cn

[G14] 数据类 / record
来源：http://fo.huixiangedu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sb.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://hw.jctech888.com.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gz.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://vp.muxihuayi.cn

Java: record User(String name, int age) {}
来源：http://ol.szxytkj.cn

Go:   type User struct { Name string; Age int }
来源：http://ak.bookmarksfly.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://py.nszjky.cn

C#:   record User(string Name, int Age);
来源：http://sm.panjiajie.cn

[G15] 枚举
来源：http://zt.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://is.haigaiapp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yw.nszjky.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gk.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uz.nszjky.cn

Java: enum Color { RED, GREEN }
来源：http://sk.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sm.shtwfgs.cn

Ruby: Color = %i[red green].freeze
来源：http://ev.nszjky.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mr.shtwfgs.cn

[G16] 对象转数组 / 字典
来源：http://rx.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eo.wgjwhj.cn


<!-- 参考信息 -->