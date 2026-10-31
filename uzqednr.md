代发 wailian999

Ruby: s.lines
来源：http://fb.chemitech.net.cn

C#:   s.Split('\n')
来源：http://ql.9csxet.cn

[E20] 判断字符串是否为空
来源：http://ou.muxihuayi.cn

Py:   if not s:
来源：http://ys.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ln.huixinmuqiang.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ey.haigaiapp.cn

TS:   if (s === "") {}
来源：http://lz.jianghongdianzi.cn

Java: if (s.isEmpty()) {}
来源：http://dc.asd995.cn

Go:   if s == "" {}
来源：http://in.panjiajie.cn

Ruby: if s.empty?
来源：http://id.asd995.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xs.szsharing.cn

[E21] 超长截断加省略号
来源：http://oc.shtwfgs.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://we.yuexingan06.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://op.wgjwhj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vz.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://az.bookmarksfly.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://si.haigaiapp.cn

Go:   // 按 rune 判断长度后截断
来源：http://kq.hahajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gq.szxytkj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dk.nicolike.cn

[E22] 字节长度与字符长度
来源：http://bq.muxihuayi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://cz.bjjhwx.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jn.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://cc.huixiangedu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cg.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ja.chemitech.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mq.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://ia.chemitech.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ad.hahajie.cn

================================================================================
来源：http://jh.muxihuayi.cn

F. 文件与目录
来源：http://gn.asd995.cn

================================================================================
来源：http://oe.shtwfgs.cn

[F01] 读取整个文件
来源：http://bx.colortex.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ak.colortex.cn

PHP:  file_get_contents("a.txt");
来源：http://uk.szxytkj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://to.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uf.chemitech.net.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mr.yuexingan06.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vp.521024.cn

Ruby: File.read("a.txt")
来源：http://kl.hnjuh.cn

C#:   File.ReadAllText("a.txt");
来源：http://um.shxzskj.cn

[F02] 逐行读取文件
来源：http://cz.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oe.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ei.yuntaijiaju.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://na.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gv.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rp.shxzukj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://un.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xk.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lg.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://ky.colortex.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xk.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bj.nszjky.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://di.szsharing.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gg.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xw.huixinmuqiang.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xq.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://lz.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ao.shtwfgs.cn

[F04] 追加写入文件
来源：http://rj.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hr.haigaiapp.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://bq.hahajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ms.9csxet.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ca.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gh.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kk.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pi.bjjhwx.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ax.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://iv.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qo.colortex.cn

PHP:  file_exists("a.txt");
来源：http://uf.9csxet.cn

JS:   fs.existsSync("a.txt")
来源：http://xa.gzmigu.cn

TS:   fs.existsSync("a.txt")
来源：http://yy.yuexingan06.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://cx.bookmarksfly.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rv.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://xm.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://ke.haigaiapp.cn

[F06] 删除文件
来源：http://pg.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://zj.colortex.cn

PHP:  unlink("a.txt");
来源：http://cf.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://se.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xb.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://kc.wgjwhj.cn

Go:   os.Remove("a.txt")
来源：http://vn.lnxyls.cn

Ruby: File.delete("a.txt")
来源：http://gs.wgjwhj.cn

C#:   File.Delete("a.txt");
来源：http://dd.wgjwhj.cn

[F07] 创建目录（含多级）
来源：http://pj.nszjky.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kh.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uy.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jn.huanxung.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lb.wgjwhj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ea.521024.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nk.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ih.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zi.muxihuayi.cn

[F08] 遍历目录
来源：http://hp.colortex.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://bf.wgjwhj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://du.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://yx.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://wv.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gw.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://af.nszjky.cn

Ruby: Dir.children("dir")
来源：http://uc.newstarts.cn

C#:   Directory.GetFiles("dir")
来源：http://gm.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://du.chemitech.net.cn

Py:   os.path.getsize("a.txt")
来源：http://kd.asd995.cn

PHP:  filesize("a.txt");
来源：http://nl.bookmarksfly.cn

JS:   fs.statSync("a.txt").size
来源：http://xk.wgjwhj.cn

TS:   fs.statSync("a.txt").size
来源：http://sz.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mv.jctech888.com.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pz.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://na.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://sl.newstarts.cn

[F10] 取文件扩展名 / 文件名
来源：http://ce.bookmarksfly.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mc.huixiangedu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yy.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://me.gzmigu.cn

TS:   path.extname("a.txt")
来源：http://uy.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cq.muxihuayi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zm.szsharing.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gm.bjjhwx.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mv.521024.cn

[F11] 复制与移动文件
来源：http://gp.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xq.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bw.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qi.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qe.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mm.gzmigu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zs.jctech888.com.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yf.lnxyls.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ff.chemitech.net.cn

[F12] CSV 读写
来源：http://vi.bjjhwx.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ha.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zm.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mv.shxzukj.cn

TS:   // 同上
来源：http://vc.nszjky.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tv.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ys.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://te.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qp.muxihuayi.cn

================================================================================
来源：http://fa.jctech888.com.cn

G. 面向对象
来源：http://wp.szxytkj.cn

================================================================================
来源：http://bj.szxytkj.cn

[G01] 定义类
来源：http://et.haigaiapp.cn

Py:   class User: pass
来源：http://vb.szxytkj.cn

PHP:  class User {}
来源：http://ij.hahajie.cn

JS:   class User {}
来源：http://fc.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://wj.szxytkj.cn

Java: class User {}
来源：http://ye.jianghongdianzi.cn

Go:   type User struct { Name string }
来源：http://oy.wgjwhj.cn

Ruby: class User; end
来源：http://up.jctech888.com.cn

C#:   class User {}
来源：http://ok.huixinmuqiang.cn

[G02] 构造函数
来源：http://nw.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://uq.huixinmuqiang.cn

PHP:  public function __construct(public string $name) {}
来源：http://du.panjiajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://qt.szxytkj.cn

TS:   constructor(public name: string) {}
来源：http://qx.nicolike.cn

Java: User(String name) { this.name = name; }
来源：http://em.bookmarksfly.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ts.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://om.huixinmuqiang.cn

C#:   public User(string name) { Name = name; }
来源：http://xg.szsharing.cn

[G03] 实例属性
来源：http://pt.huanxung.cn

Py:   self.name = "x"
来源：http://kt.nszjky.cn

PHP:  public string $name = "x";
来源：http://jf.wgjwhj.cn

JS:   this.name = "x";
来源：http://rp.szsharing.cn

TS:   name: string = "x";
来源：http://ng.chemitech.net.cn

Java: private String name;
来源：http://nq.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qp.huixiangedu.cn

Ruby: @name = "x"
来源：http://ex.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://xa.bjjhwx.cn

[G04] 定义方法
来源：http://ft.lnxyls.cn

Py:   def greet(self): return self.name
来源：http://os.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ss.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://mx.huixiangedu.cn

TS:   greet(): string { return this.name; }
来源：http://ct.bjjhwx.cn

Java: String greet() { return name; }
来源：http://ny.shtwfgs.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xs.shxzskj.cn

Ruby: def greet; @name; end
来源：http://hp.jctech888.com.cn

C#:   public string Greet() => Name;
来源：http://vo.bjjhwx.cn

[G05] 继承
来源：http://kr.newstarts.cn

Py:   class Admin(User): pass
来源：http://gf.asd995.cn

PHP:  class Admin extends User {}
来源：http://wt.colortex.cn

JS:   class Admin extends User {}
来源：http://et.huanxung.cn

TS:   class Admin extends User {}
来源：http://gz.asd995.cn

Java: class Admin extends User {}
来源：http://xc.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ok.nicolike.cn

Ruby: class Admin < User; end
来源：http://go.colortex.cn

C#:   class Admin : User {}
来源：http://ml.huixinmuqiang.cn

[G06] 重写方法
来源：http://ca.panjiajie.cn

Py:   def greet(self): return "admin"
来源：http://rs.bjjhwx.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ga.gzmigu.cn

JS:   greet() { return "admin"; }
来源：http://xw.bookmarksfly.cn

TS:   greet(): string { return "admin"; }
来源：http://ct.asd995.cn

Java: @Override String greet() { return "admin"; }
来源：http://ym.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rj.szxytkj.cn

Ruby: def greet; "admin"; end
来源：http://xs.asd995.cn

C#:   public override string Greet() => "admin";
来源：http://no.huixinmuqiang.cn

[G07] 调用父类方法
来源：http://jz.521024.cn

Py:   super().greet()
来源：http://xn.9csxet.cn

PHP:  parent::greet();
来源：http://jt.szxytkj.cn

JS:   super.greet();
来源：http://pt.lnxyls.cn

TS:   super.greet();
来源：http://mt.wgjwhj.cn

Java: super.greet();
来源：http://wy.lnxyls.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bj.9csxet.cn

Ruby: super
来源：http://fh.szxytkj.cn

C#:   base.Greet();
来源：http://qs.hahajie.cn

[G08] 静态方法与属性
来源：http://nl.bjjhwx.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://py.huanxung.cn

PHP:  public static function f() {}
来源：http://oa.jctech888.com.cn

JS:   static f() {}
来源：http://lb.yuntaijiaju.cn

TS:   static f(): void {}
来源：http://az.shtwfgs.cn

Java: static void f() {}
来源：http://br.521024.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cg.hahajie.cn

Ruby: def self.f; end
来源：http://kn.asd995.cn

C#:   public static void F() {}
来源：http://bg.shxzukj.cn

[G09] 接口 / 抽象类
来源：http://bv.huanxung.cn

Py:   from abc import ABC, abstractmethod
来源：http://al.gzmigu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dg.huixiangedu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sh.9csxet.cn

TS:   interface Shape { area(): number; }
来源：http://qi.chemitech.net.cn

Java: interface Shape { double area(); }
来源：http://yj.shtwfgs.cn

Go:   type Shape interface { Area() float64 }
来源：http://yj.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ja.newstarts.cn

C#:   interface IShape { double Area(); }
来源：http://cz.szxytkj.cn

[G10] 访问控制
来源：http://tu.nszjky.cn

Py:   约定 _protected / __private（不强制）
来源：http://rw.newstarts.cn

PHP:  public / protected / private
来源：http://rm.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://tt.huixiangedu.cn

TS:   public / protected / private
来源：http://ku.shxzskj.cn

Java: public / protected / private / 默认包级
来源：http://yy.huixiangedu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://on.haigaiapp.cn

Ruby: public / protected / private
来源：http://ze.asd995.cn

C#:   public / protected / private / internal
来源：http://wp.nicolike.cn

[G11] getter / setter
来源：http://vu.9csxet.cn

Py:   @property 与 @x.setter
来源：http://ws.nicolike.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://of.newstarts.cn

JS:   get name() { return this._name; }
来源：http://vt.lnxyls.cn

TS:   get name(): string { return this._name; }
来源：http://up.shtwfgs.cn

Java: public String getName() { return name; }
来源：http://hz.huixiangedu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dv.huixinmuqiang.cn

Ruby: attr_accessor :name
来源：http://vk.nszjky.cn

C#:   public string Name { get; set; }
来源：http://ry.huixiangedu.cn

[G12] 对象转字符串
来源：http://hy.panjiajie.cn

Py:   def __str__(self): return self.name
来源：http://tu.newstarts.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dw.szxytkj.cn

JS:   toString() { return this.name; }
来源：http://jn.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://cb.huanxung.cn

Java: @Override public String toString() { return name; }
来源：http://eh.jctech888.com.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tw.huanxung.cn

Ruby: def to_s; @name; end
来源：http://mi.bjjhwx.cn

C#:   public override string ToString() => Name;
来源：http://uh.bjjhwx.cn

[G13] 判断对象类型
来源：http://md.chemitech.net.cn

Py:   isinstance(u, User)
来源：http://on.muxihuayi.cn

PHP:  $u instanceof User
来源：http://oy.chemitech.net.cn

JS:   u instanceof User
来源：http://au.9csxet.cn

TS:   u instanceof User
来源：http://iw.hahajie.cn

Java: u instanceof User
来源：http://dm.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://yi.asd995.cn

Ruby: u.is_a?(User)
来源：http://aq.yuntaijiaju.cn

C#:   u is User
来源：http://zx.hnjuh.cn

[G14] 数据类 / record
来源：http://ul.yuntaijiaju.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nr.521024.cn

PHP:  // 用 readonly 属性模拟
来源：http://cd.hahajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kz.szxytkj.cn

TS:   type User = { name: string; age: number };
来源：http://lv.huanxung.cn

Java: record User(String name, int age) {}
来源：http://fx.hnjuh.cn

Go:   type User struct { Name string; Age int }
来源：http://km.haigaiapp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ui.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://bi.chemitech.net.cn

[G15] 枚举
来源：http://hf.lnxyls.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jq.chemitech.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://co.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ii.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yl.jctech888.com.cn

Java: enum Color { RED, GREEN }
来源：http://yk.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ar.jianghongdianzi.cn

Ruby: Color = %i[red green].freeze
来源：http://rr.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://eq.shtwfgs.cn

[G16] 对象转数组 / 字典
来源：http://up.lnxyls.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ct.shtwfgs.cn

PHP:  get_object_vars($obj);
来源：http://fr.jianghongdianzi.cn

JS:   Object.entries(obj)
来源：http://uu.szxytkj.cn

TS:   Object.entries(obj)
来源：http://mm.nszjky.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uu.bjjhwx.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ib.wgjwhj.cn

Ruby: obj.instance_variables
来源：http://ho.521024.cn

C#:   // 用反射或 System.Text.Json
来源：http://gv.huanxung.cn

================================================================================
来源：http://ao.shtwfgs.cn

H. 异常与错误处理
来源：http://gh.haigaiapp.cn

================================================================================
来源：http://xm.panjiajie.cn

[H01] try / catch 基础
来源：http://wt.shtwfgs.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tt.jianghongdianzi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nu.colortex.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wi.yuntaijiaju.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vu.szsharing.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ty.yuexingan06.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lz.bookmarksfly.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uy.colortex.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lr.chemitech.net.cn

[H02] finally / ensure 收尾
来源：http://lz.521024.cn


<!-- 参考信息 -->