代发 wailian999

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://rg.521024.cn

[E19] 多行文本按行拆分
来源：http://jr.colortex.cn

Py:   s.splitlines()
来源：http://yg.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ax.yuntaijiaju.cn

JS:   s.split(/\r?\n/)
来源：http://lo.huixinmuqiang.cn

TS:   s.split(/\r?\n/)
来源：http://rb.jctech888.com.cn

Java: s.lines().toList()
来源：http://zm.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://ig.bjjhwx.cn

Ruby: s.lines
来源：http://fl.shxzukj.cn

C#:   s.Split('\n')
来源：http://cw.asd995.cn

[E20] 判断字符串是否为空
来源：http://es.huanxung.cn

Py:   if not s:
来源：http://qr.panjiajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wu.chemitech.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ck.muxihuayi.cn

TS:   if (s === "") {}
来源：http://ds.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://nk.panjiajie.cn

Go:   if s == "" {}
来源：http://gl.huixiangedu.cn

Ruby: if s.empty?
来源：http://rk.lnxyls.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eq.hahajie.cn

[E21] 超长截断加省略号
来源：http://vk.yuexingan06.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tu.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://da.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mn.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pw.huixiangedu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://aq.haigaiapp.cn

Go:   // 按 rune 判断长度后截断
来源：http://cr.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sa.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://tb.9csxet.cn

[E22] 字节长度与字符长度
来源：http://kj.shxzskj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://at.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pa.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kn.gzmigu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nz.haigaiapp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qd.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kg.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://qt.huixinmuqiang.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yo.hnjuh.cn

================================================================================
来源：http://xt.asd995.cn

F. 文件与目录
来源：http://bp.gzmigu.cn

================================================================================
来源：http://xi.huixinmuqiang.cn

[F01] 读取整个文件
来源：http://yw.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://eq.asd995.cn

PHP:  file_get_contents("a.txt");
来源：http://nd.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mx.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://eu.wgjwhj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xa.gzmigu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nr.huixinmuqiang.cn

Ruby: File.read("a.txt")
来源：http://wt.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://sx.shtwfgs.cn

[F02] 逐行读取文件
来源：http://ke.bookmarksfly.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fz.bjjhwx.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://bx.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ih.bookmarksfly.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gt.bookmarksfly.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wf.huixiangedu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bo.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hw.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://we.szsharing.cn

[F03] 写入文件（覆盖）
来源：http://eo.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bs.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qs.colortex.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gz.szsharing.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zh.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vi.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wm.bjjhwx.cn

Ruby: File.write("a.txt", "hi")
来源：http://jf.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kr.panjiajie.cn

[F04] 追加写入文件
来源：http://hb.shxzukj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mb.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://og.huixinmuqiang.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gz.wgjwhj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fl.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sc.wgjwhj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vp.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dk.hahajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dr.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://bl.huixinmuqiang.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jr.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://xi.shxzskj.cn

JS:   fs.existsSync("a.txt")
来源：http://ao.panjiajie.cn

TS:   fs.existsSync("a.txt")
来源：http://la.521024.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cz.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://up.colortex.cn

Ruby: File.exist?("a.txt")
来源：http://sf.newstarts.cn

C#:   File.Exists("a.txt")
来源：http://sz.yuexingan06.cn

[F06] 删除文件
来源：http://ee.yuexingan06.cn

Py:   os.remove("a.txt")
来源：http://ec.lnxyls.cn

PHP:  unlink("a.txt");
来源：http://qw.nszjky.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fk.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mn.newstarts.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dn.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://uy.asd995.cn

Ruby: File.delete("a.txt")
来源：http://rx.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://jy.lnxyls.cn

[F07] 创建目录（含多级）
来源：http://ai.bookmarksfly.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oo.yuexingan06.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://co.wgjwhj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bm.jianghongdianzi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mx.newstarts.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fo.shxzukj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ux.521024.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qw.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://na.nicolike.cn

[F08] 遍历目录
来源：http://gj.muxihuayi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xf.gzmigu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qz.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://zn.shxzukj.cn

TS:   fs.readdirSync("dir")
来源：http://uw.panjiajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://if.hnjuh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ut.nicolike.cn

Ruby: Dir.children("dir")
来源：http://ml.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://pd.colortex.cn

[F09] 获取文件大小
来源：http://sj.yuntaijiaju.cn

Py:   os.path.getsize("a.txt")
来源：http://le.shxzskj.cn

PHP:  filesize("a.txt");
来源：http://ep.newstarts.cn

JS:   fs.statSync("a.txt").size
来源：http://rl.yuntaijiaju.cn

TS:   fs.statSync("a.txt").size
来源：http://ed.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fa.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://er.asd995.cn

Ruby: File.size("a.txt")
来源：http://vz.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://pp.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://qn.yuntaijiaju.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nd.shxzukj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mo.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://li.huixinmuqiang.cn

TS:   path.extname("a.txt")
来源：http://fo.szxytkj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nb.nszjky.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vn.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ba.jctech888.com.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://az.yuntaijiaju.cn

[F11] 复制与移动文件
来源：http://vs.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pm.shtwfgs.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cb.lnxyls.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sw.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kc.jianghongdianzi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hn.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ua.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ei.shxzukj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wd.hnjuh.cn

[F12] CSV 读写
来源：http://pw.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mg.newstarts.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xx.newstarts.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mn.shxzukj.cn

TS:   // 同上
来源：http://uv.nszjky.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mp.bjjhwx.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kz.wgjwhj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://vi.wgjwhj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://py.jctech888.com.cn

================================================================================
来源：http://br.521024.cn

G. 面向对象
来源：http://xu.jianghongdianzi.cn

================================================================================
来源：http://mt.panjiajie.cn

[G01] 定义类
来源：http://fc.yuntaijiaju.cn

Py:   class User: pass
来源：http://yo.haigaiapp.cn

PHP:  class User {}
来源：http://ju.bookmarksfly.cn

JS:   class User {}
来源：http://xn.shxzskj.cn

TS:   class User { name: string = ""; }
来源：http://qj.shxzskj.cn

Java: class User {}
来源：http://gq.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://cd.shxzukj.cn

Ruby: class User; end
来源：http://td.chemitech.net.cn

C#:   class User {}
来源：http://jc.yuexingan06.cn

[G02] 构造函数
来源：http://sb.jctech888.com.cn

Py:   def __init__(self, name): self.name = name
来源：http://jm.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://al.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://jt.asd995.cn

TS:   constructor(public name: string) {}
来源：http://vm.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://ql.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ng.yuntaijiaju.cn

Ruby: def initialize(name); @name = name; end
来源：http://yc.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://dy.asd995.cn

[G03] 实例属性
来源：http://jb.chemitech.net.cn

Py:   self.name = "x"
来源：http://cy.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://tj.bookmarksfly.cn

JS:   this.name = "x";
来源：http://jd.newstarts.cn

TS:   name: string = "x";
来源：http://gx.shxzukj.cn

Java: private String name;
来源：http://pc.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cy.colortex.cn

Ruby: @name = "x"
来源：http://xy.jctech888.com.cn

C#:   public string Name { get; set; } = "x";
来源：http://ce.szxytkj.cn

[G04] 定义方法
来源：http://io.szsharing.cn

Py:   def greet(self): return self.name
来源：http://zt.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bk.bookmarksfly.cn

JS:   greet() { return this.name; }
来源：http://dr.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://qy.nszjky.cn

Java: String greet() { return name; }
来源：http://cb.szxytkj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xk.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://nj.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://wu.huanxung.cn

[G05] 继承
来源：http://yu.panjiajie.cn

Py:   class Admin(User): pass
来源：http://fi.newstarts.cn

PHP:  class Admin extends User {}
来源：http://ia.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://sq.nszjky.cn

TS:   class Admin extends User {}
来源：http://el.shtwfgs.cn

Java: class Admin extends User {}
来源：http://fh.nicolike.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pk.szsharing.cn

Ruby: class Admin < User; end
来源：http://aq.newstarts.cn

C#:   class Admin : User {}
来源：http://os.chemitech.net.cn

[G06] 重写方法
来源：http://hv.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://vl.huanxung.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://iv.wgjwhj.cn

JS:   greet() { return "admin"; }
来源：http://wm.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://rv.yuntaijiaju.cn

Java: @Override String greet() { return "admin"; }
来源：http://kw.nicolike.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kh.hnjuh.cn

Ruby: def greet; "admin"; end
来源：http://bc.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://cj.shxzukj.cn

[G07] 调用父类方法
来源：http://dy.nicolike.cn

Py:   super().greet()
来源：http://rf.newstarts.cn

PHP:  parent::greet();
来源：http://mb.colortex.cn

JS:   super.greet();
来源：http://kq.bookmarksfly.cn

TS:   super.greet();
来源：http://rs.panjiajie.cn

Java: super.greet();
来源：http://jw.shxzukj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zo.chemitech.net.cn

Ruby: super
来源：http://pf.bookmarksfly.cn

C#:   base.Greet();
来源：http://yi.521024.cn

[G08] 静态方法与属性
来源：http://rx.wgjwhj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://my.huixinmuqiang.cn

PHP:  public static function f() {}
来源：http://us.asd995.cn

JS:   static f() {}
来源：http://zt.shtwfgs.cn

TS:   static f(): void {}
来源：http://iv.yuexingan06.cn

Java: static void f() {}
来源：http://id.shtwfgs.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mr.gzmigu.cn

Ruby: def self.f; end
来源：http://yz.shxzskj.cn

C#:   public static void F() {}
来源：http://vj.jctech888.com.cn

[G09] 接口 / 抽象类
来源：http://gt.9csxet.cn

Py:   from abc import ABC, abstractmethod
来源：http://eq.huanxung.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qn.jctech888.com.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hq.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://jj.shtwfgs.cn

Java: interface Shape { double area(); }
来源：http://eb.huixinmuqiang.cn

Go:   type Shape interface { Area() float64 }
来源：http://bu.panjiajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nr.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://ht.lnxyls.cn

[G10] 访问控制
来源：http://ic.yuexingan06.cn

Py:   约定 _protected / __private（不强制）
来源：http://dw.huixiangedu.cn

PHP:  public / protected / private
来源：http://ce.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://zw.bjjhwx.cn

TS:   public / protected / private
来源：http://af.hnjuh.cn

Java: public / protected / private / 默认包级
来源：http://jx.nicolike.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://um.muxihuayi.cn

Ruby: public / protected / private
来源：http://fi.newstarts.cn

C#:   public / protected / private / internal
来源：http://ao.nicolike.cn

[G11] getter / setter
来源：http://dt.521024.cn

Py:   @property 与 @x.setter
来源：http://lk.bookmarksfly.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hp.shxzukj.cn

JS:   get name() { return this._name; }
来源：http://ou.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://uy.wgjwhj.cn

Java: public String getName() { return name; }
来源：http://pb.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dw.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://lu.hahajie.cn

C#:   public string Name { get; set; }
来源：http://fd.shxzskj.cn

[G12] 对象转字符串
来源：http://qe.hnjuh.cn

Py:   def __str__(self): return self.name
来源：http://dr.asd995.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://eq.colortex.cn

JS:   toString() { return this.name; }
来源：http://om.chemitech.net.cn

TS:   toString(): string { return this.name; }
来源：http://tg.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://se.lnxyls.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vf.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://ir.huixiangedu.cn

C#:   public override string ToString() => Name;
来源：http://wc.wgjwhj.cn

[G13] 判断对象类型
来源：http://ux.9csxet.cn

Py:   isinstance(u, User)
来源：http://lp.haigaiapp.cn

PHP:  $u instanceof User
来源：http://xq.chemitech.net.cn

JS:   u instanceof User
来源：http://kt.bjjhwx.cn

TS:   u instanceof User
来源：http://ft.asd995.cn

Java: u instanceof User
来源：http://ey.colortex.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ie.521024.cn

Ruby: u.is_a?(User)
来源：http://zs.szsharing.cn

C#:   u is User
来源：http://ro.szsharing.cn

[G14] 数据类 / record
来源：http://fn.shxzskj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dh.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://ep.huanxung.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sm.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://yp.lnxyls.cn

Java: record User(String name, int age) {}
来源：http://he.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://ch.newstarts.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mn.szsharing.cn

C#:   record User(string Name, int Age);
来源：http://lb.gzmigu.cn

[G15] 枚举
来源：http://sp.chemitech.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mg.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lh.nszjky.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://td.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://an.haigaiapp.cn

Java: enum Color { RED, GREEN }
来源：http://kg.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://es.asd995.cn

Ruby: Color = %i[red green].freeze
来源：http://wd.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lj.jianghongdianzi.cn

[G16] 对象转数组 / 字典
来源：http://sm.asd995.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gx.haigaiapp.cn

PHP:  get_object_vars($obj);
来源：http://lg.gzmigu.cn

JS:   Object.entries(obj)
来源：http://xl.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://ex.gzmigu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jc.huixiangedu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://md.shxzskj.cn

Ruby: obj.instance_variables
来源：http://jv.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://at.hahajie.cn

================================================================================
来源：http://vg.colortex.cn

H. 异常与错误处理
来源：http://bb.nszjky.cn

================================================================================
来源：http://la.521024.cn

[H01] try / catch 基础
来源：http://rn.9csxet.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sf.szxytkj.cn


<!-- 参考信息 -->