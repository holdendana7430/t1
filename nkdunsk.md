代发 wailian999

Go:   if s == "" {}
来源：http://ab.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://nd.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dy.asd995.cn

[E21] 超长截断加省略号
来源：http://fo.huixinmuqiang.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cl.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hw.haigaiapp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gw.chemitech.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tb.bookmarksfly.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pt.muxihuayi.cn

Go:   // 按 rune 判断长度后截断
来源：http://ix.wgjwhj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ux.huixiangedu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cn.shxzukj.cn

[E22] 字节长度与字符长度
来源：http://xq.521024.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wy.huixinmuqiang.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tz.shxzukj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fr.bjjhwx.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ri.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pa.muxihuayi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://it.shtwfgs.cn

Ruby: s.bytesize;  s.length
来源：http://vx.szsharing.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pw.chemitech.net.cn

================================================================================
来源：http://ue.newstarts.cn

F. 文件与目录
来源：http://lt.huanxung.cn

================================================================================
来源：http://wc.gzmigu.cn

[F01] 读取整个文件
来源：http://if.szxytkj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ne.shxzskj.cn

PHP:  file_get_contents("a.txt");
来源：http://fu.panjiajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gt.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mw.shtwfgs.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zm.hnjuh.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rr.gzmigu.cn

Ruby: File.read("a.txt")
来源：http://ky.bjjhwx.cn

C#:   File.ReadAllText("a.txt");
来源：http://nv.lnxyls.cn

[F02] 逐行读取文件
来源：http://sp.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fw.huixinmuqiang.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://cc.lnxyls.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://no.shxzskj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cg.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://di.szxytkj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://aw.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mr.chemitech.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rh.asd995.cn

[F03] 写入文件（覆盖）
来源：http://cv.szxytkj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ij.panjiajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://kk.szsharing.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wg.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ro.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zr.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mu.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://db.huixiangedu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://eb.hnjuh.cn

[F04] 追加写入文件
来源：http://qs.wgjwhj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fa.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yd.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pd.nicolike.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ys.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://sl.jctech888.com.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ce.newstarts.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://we.nszjky.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gk.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://ue.hnjuh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://eb.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://rz.newstarts.cn

JS:   fs.existsSync("a.txt")
来源：http://ln.asd995.cn

TS:   fs.existsSync("a.txt")
来源：http://ow.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://yq.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://bq.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://sn.gzmigu.cn

C#:   File.Exists("a.txt")
来源：http://pk.nszjky.cn

[F06] 删除文件
来源：http://oh.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://cp.jctech888.com.cn

PHP:  unlink("a.txt");
来源：http://xi.szxytkj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bm.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sa.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://za.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://mc.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://yl.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://fx.szsharing.cn

[F07] 创建目录（含多级）
来源：http://rb.haigaiapp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ru.szxytkj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ln.gzmigu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://km.panjiajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vr.chemitech.net.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://km.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ur.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zg.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.szsharing.cn

[F08] 遍历目录
来源：http://vg.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://co.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qj.nicolike.cn

JS:   fs.readdirSync("dir")
来源：http://eu.jctech888.com.cn

TS:   fs.readdirSync("dir")
来源：http://xe.chemitech.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ec.panjiajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://rw.hahajie.cn

Ruby: Dir.children("dir")
来源：http://nr.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://aa.lnxyls.cn

[F09] 获取文件大小
来源：http://bm.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://jp.hnjuh.cn

PHP:  filesize("a.txt");
来源：http://jo.haigaiapp.cn

JS:   fs.statSync("a.txt").size
来源：http://gn.newstarts.cn

TS:   fs.statSync("a.txt").size
来源：http://xi.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mf.nicolike.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qz.lnxyls.cn

Ruby: File.size("a.txt")
来源：http://we.nicolike.cn

C#:   new FileInfo("a.txt").Length
来源：http://iu.newstarts.cn

[F10] 取文件扩展名 / 文件名
来源：http://ux.shxzukj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vu.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fk.jianghongdianzi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zw.yuntaijiaju.cn

TS:   path.extname("a.txt")
来源：http://xo.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xv.9csxet.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ga.jctech888.com.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qv.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sc.wgjwhj.cn

[F11] 复制与移动文件
来源：http://ds.bookmarksfly.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zx.huanxung.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qh.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://np.muxihuayi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ub.yuexingan06.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rk.colortex.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mq.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pv.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ec.huixinmuqiang.cn

[F12] CSV 读写
来源：http://do.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://is.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kj.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zm.lnxyls.cn

TS:   // 同上
来源：http://zi.shxzukj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hb.jctech888.com.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ny.panjiajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tb.szsharing.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kh.bookmarksfly.cn

================================================================================
来源：http://st.colortex.cn

G. 面向对象
来源：http://qo.yuntaijiaju.cn

================================================================================
来源：http://qx.szsharing.cn

[G01] 定义类
来源：http://lq.yuntaijiaju.cn

Py:   class User: pass
来源：http://qz.nicolike.cn

PHP:  class User {}
来源：http://kb.nicolike.cn

JS:   class User {}
来源：http://ei.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://lb.huixinmuqiang.cn

Java: class User {}
来源：http://yg.hahajie.cn

Go:   type User struct { Name string }
来源：http://ti.hnjuh.cn

Ruby: class User; end
来源：http://qy.521024.cn

C#:   class User {}
来源：http://gm.gzmigu.cn

[G02] 构造函数
来源：http://ff.lnxyls.cn

Py:   def __init__(self, name): self.name = name
来源：http://zu.9csxet.cn

PHP:  public function __construct(public string $name) {}
来源：http://md.gzmigu.cn

JS:   constructor(name) { this.name = name; }
来源：http://ln.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://ik.asd995.cn

Java: User(String name) { this.name = name; }
来源：http://gk.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cc.lnxyls.cn

Ruby: def initialize(name); @name = name; end
来源：http://kp.shxzskj.cn

C#:   public User(string name) { Name = name; }
来源：http://ki.huixiangedu.cn

[G03] 实例属性
来源：http://vc.yuexingan06.cn

Py:   self.name = "x"
来源：http://ez.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://vh.colortex.cn

JS:   this.name = "x";
来源：http://bi.shxzukj.cn

TS:   name: string = "x";
来源：http://dq.jianghongdianzi.cn

Java: private String name;
来源：http://rc.yuexingan06.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ip.nszjky.cn

Ruby: @name = "x"
来源：http://xm.lnxyls.cn

C#:   public string Name { get; set; } = "x";
来源：http://yn.wgjwhj.cn

[G04] 定义方法
来源：http://vf.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://hs.bookmarksfly.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://on.hahajie.cn

JS:   greet() { return this.name; }
来源：http://bu.lnxyls.cn

TS:   greet(): string { return this.name; }
来源：http://co.jianghongdianzi.cn

Java: String greet() { return name; }
来源：http://id.521024.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qn.nszjky.cn

Ruby: def greet; @name; end
来源：http://zi.huanxung.cn

C#:   public string Greet() => Name;
来源：http://he.wgjwhj.cn

[G05] 继承
来源：http://lq.panjiajie.cn

Py:   class Admin(User): pass
来源：http://om.yuntaijiaju.cn

PHP:  class Admin extends User {}
来源：http://ym.muxihuayi.cn

JS:   class Admin extends User {}
来源：http://pr.huixinmuqiang.cn

TS:   class Admin extends User {}
来源：http://pr.muxihuayi.cn

Java: class Admin extends User {}
来源：http://bn.hahajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qa.asd995.cn

Ruby: class Admin < User; end
来源：http://rt.shxzukj.cn

C#:   class Admin : User {}
来源：http://ut.panjiajie.cn

[G06] 重写方法
来源：http://sy.szsharing.cn

Py:   def greet(self): return "admin"
来源：http://cx.huixinmuqiang.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kb.colortex.cn

JS:   greet() { return "admin"; }
来源：http://pr.yuntaijiaju.cn

TS:   greet(): string { return "admin"; }
来源：http://kn.huanxung.cn

Java: @Override String greet() { return "admin"; }
来源：http://wf.521024.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://iq.nszjky.cn

Ruby: def greet; "admin"; end
来源：http://af.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://sk.asd995.cn

[G07] 调用父类方法
来源：http://fn.shxzskj.cn

Py:   super().greet()
来源：http://cb.hahajie.cn

PHP:  parent::greet();
来源：http://lv.9csxet.cn

JS:   super.greet();
来源：http://lo.asd995.cn

TS:   super.greet();
来源：http://pg.bjjhwx.cn

Java: super.greet();
来源：http://kq.bjjhwx.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kp.shtwfgs.cn

Ruby: super
来源：http://mv.szsharing.cn

C#:   base.Greet();
来源：http://jp.bookmarksfly.cn

[G08] 静态方法与属性
来源：http://ig.bookmarksfly.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://os.nszjky.cn

PHP:  public static function f() {}
来源：http://os.haigaiapp.cn

JS:   static f() {}
来源：http://dp.jctech888.com.cn

TS:   static f(): void {}
来源：http://ul.haigaiapp.cn

Java: static void f() {}
来源：http://nt.521024.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xr.gzmigu.cn

Ruby: def self.f; end
来源：http://ji.panjiajie.cn

C#:   public static void F() {}
来源：http://oc.wgjwhj.cn

[G09] 接口 / 抽象类
来源：http://ni.asd995.cn

Py:   from abc import ABC, abstractmethod
来源：http://ao.yuexingan06.cn

PHP:  interface Shape { public function area(): float; }
来源：http://so.hahajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ib.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://km.9csxet.cn

Java: interface Shape { double area(); }
来源：http://og.szsharing.cn

Go:   type Shape interface { Area() float64 }
来源：http://be.9csxet.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://de.jctech888.com.cn

C#:   interface IShape { double Area(); }
来源：http://pm.gzmigu.cn

[G10] 访问控制
来源：http://oa.szsharing.cn

Py:   约定 _protected / __private（不强制）
来源：http://de.panjiajie.cn

PHP:  public / protected / private
来源：http://lg.jianghongdianzi.cn

JS:   #private 字段；其余公开
来源：http://aj.colortex.cn

TS:   public / protected / private
来源：http://rw.colortex.cn

Java: public / protected / private / 默认包级
来源：http://cg.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nl.shtwfgs.cn

Ruby: public / protected / private
来源：http://qo.hahajie.cn

C#:   public / protected / private / internal
来源：http://rz.wgjwhj.cn

[G11] getter / setter
来源：http://js.newstarts.cn

Py:   @property 与 @x.setter
来源：http://ub.shxzskj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://oc.nszjky.cn

JS:   get name() { return this._name; }
来源：http://af.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://zk.yuntaijiaju.cn

Java: public String getName() { return name; }
来源：http://ek.huixinmuqiang.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wa.521024.cn

Ruby: attr_accessor :name
来源：http://fx.shtwfgs.cn

C#:   public string Name { get; set; }
来源：http://ll.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://wl.shtwfgs.cn

Py:   def __str__(self): return self.name
来源：http://pd.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mg.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://bk.jctech888.com.cn

TS:   toString(): string { return this.name; }
来源：http://yu.wgjwhj.cn

Java: @Override public String toString() { return name; }
来源：http://sy.yuexingan06.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gf.muxihuayi.cn

Ruby: def to_s; @name; end
来源：http://yj.shxzskj.cn

C#:   public override string ToString() => Name;
来源：http://rk.wgjwhj.cn

[G13] 判断对象类型
来源：http://fo.hahajie.cn

Py:   isinstance(u, User)
来源：http://lo.gzmigu.cn

PHP:  $u instanceof User
来源：http://qt.muxihuayi.cn

JS:   u instanceof User
来源：http://yv.asd995.cn

TS:   u instanceof User
来源：http://bs.521024.cn

Java: u instanceof User
来源：http://py.shxzskj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zc.9csxet.cn

Ruby: u.is_a?(User)
来源：http://pt.colortex.cn

C#:   u is User
来源：http://wg.hnjuh.cn

[G14] 数据类 / record
来源：http://to.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ss.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://so.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wu.shxzukj.cn

TS:   type User = { name: string; age: number };
来源：http://ju.wgjwhj.cn

Java: record User(String name, int age) {}
来源：http://dl.colortex.cn

Go:   type User struct { Name string; Age int }
来源：http://ha.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tg.szxytkj.cn

C#:   record User(string Name, int Age);
来源：http://fm.wgjwhj.cn

[G15] 枚举
来源：http://tl.yuntaijiaju.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://et.newstarts.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fj.gzmigu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ow.9csxet.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wt.nszjky.cn

Java: enum Color { RED, GREEN }
来源：http://eh.shxzukj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wu.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://tw.shtwfgs.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uz.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://jz.jctech888.com.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ep.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://ax.jctech888.com.cn

JS:   Object.entries(obj)
来源：http://vp.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://qe.yuexingan06.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ws.szsharing.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wu.nicolike.cn

Ruby: obj.instance_variables
来源：http://ad.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://hu.muxihuayi.cn

================================================================================
来源：http://gu.521024.cn

H. 异常与错误处理
来源：http://fi.gzmigu.cn

================================================================================
来源：http://gi.muxihuayi.cn

[H01] try / catch 基础
来源：http://gj.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://db.hnjuh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dj.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dp.shxzukj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kd.chemitech.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iw.bookmarksfly.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zk.shxzskj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fj.nicolike.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hw.huanxung.cn

[H02] finally / ensure 收尾
来源：http://mx.jctech888.com.cn

Py:   try: f()⏎finally: cleanup()
来源：http://nf.nicolike.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bs.huanxung.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ht.wgjwhj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xy.asd995.cn

Java: try { f(); } finally { cleanup(); }
来源：http://oz.wgjwhj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gs.haigaiapp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://iz.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hc.newstarts.cn


<!-- 参考信息 -->