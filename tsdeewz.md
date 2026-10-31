代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://yn.muxihuayi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ya.panjiajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ef.huixiangedu.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ik.bookmarksfly.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://lv.shxzskj.cn

Go:   // 按 rune 判断长度后截断
来源：http://on.nicolike.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://sl.shxzukj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://nk.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://kf.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://my.haigaiapp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://nt.hahajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nh.colortex.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ty.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nf.muxihuayi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qj.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://hs.muxihuayi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://by.hahajie.cn

================================================================================
来源：http://pq.szxytkj.cn

F. 文件与目录
来源：http://ie.panjiajie.cn

================================================================================
来源：http://mb.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://hv.gzmigu.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tc.haigaiapp.cn

PHP:  file_get_contents("a.txt");
来源：http://kz.yuntaijiaju.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zm.gzmigu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vv.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://rc.asd995.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oi.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://mw.yuexingan06.cn

C#:   File.ReadAllText("a.txt");
来源：http://ig.huixinmuqiang.cn

[F02] 逐行读取文件
来源：http://zu.shxzukj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rd.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://xz.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ec.haigaiapp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://tl.shxzskj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://aw.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hf.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ga.huixinmuqiang.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pi.colortex.cn

[F03] 写入文件（覆盖）
来源：http://ty.asd995.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hk.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://os.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lg.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rl.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xv.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vz.huixinmuqiang.cn

Ruby: File.write("a.txt", "hi")
来源：http://kl.huixinmuqiang.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qp.yuntaijiaju.cn

[F04] 追加写入文件
来源：http://vx.wgjwhj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ca.gzmigu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pc.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jx.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vr.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pf.hahajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gm.asd995.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pb.asd995.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kg.yuntaijiaju.cn

[F05] 判断文件或目录是否存在
来源：http://wu.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nk.nszjky.cn

PHP:  file_exists("a.txt");
来源：http://vh.shtwfgs.cn

JS:   fs.existsSync("a.txt")
来源：http://vv.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://oy.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fp.nszjky.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://dv.muxihuayi.cn

Ruby: File.exist?("a.txt")
来源：http://hc.yuntaijiaju.cn

C#:   File.Exists("a.txt")
来源：http://gq.panjiajie.cn

[F06] 删除文件
来源：http://kj.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://yb.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://aj.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wh.9csxet.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ua.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oj.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://hx.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://ji.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://kt.huanxung.cn

[F07] 创建目录（含多级）
来源：http://zm.shxzukj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://tk.huixinmuqiang.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://od.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jp.bookmarksfly.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cp.huanxung.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://km.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jo.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ag.521024.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ha.huixinmuqiang.cn

[F08] 遍历目录
来源：http://nb.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ly.shxzskj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ht.huanxung.cn

JS:   fs.readdirSync("dir")
来源：http://cv.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://hq.yuexingan06.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ar.bjjhwx.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qy.hahajie.cn

Ruby: Dir.children("dir")
来源：http://lq.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://oc.bjjhwx.cn

[F09] 获取文件大小
来源：http://qq.chemitech.net.cn

Py:   os.path.getsize("a.txt")
来源：http://qb.shxzskj.cn

PHP:  filesize("a.txt");
来源：http://en.newstarts.cn

JS:   fs.statSync("a.txt").size
来源：http://rk.jianghongdianzi.cn

TS:   fs.statSync("a.txt").size
来源：http://yv.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hj.haigaiapp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bf.huanxung.cn

Ruby: File.size("a.txt")
来源：http://zr.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://rp.lnxyls.cn

[F10] 取文件扩展名 / 文件名
来源：http://lb.haigaiapp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ev.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dj.521024.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hh.nszjky.cn

TS:   path.extname("a.txt")
来源：http://ed.haigaiapp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xq.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bt.nicolike.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xh.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mc.shxzukj.cn

[F11] 复制与移动文件
来源：http://lw.nicolike.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zv.lnxyls.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://og.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cu.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tz.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://cx.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ke.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mb.521024.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bg.asd995.cn

[F12] CSV 读写
来源：http://gj.shxzskj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qa.lnxyls.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dx.chemitech.net.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jl.panjiajie.cn

TS:   // 同上
来源：http://xv.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ev.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cd.shxzskj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zo.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pz.huixiangedu.cn

================================================================================
来源：http://dn.haigaiapp.cn

G. 面向对象
来源：http://ng.muxihuayi.cn

================================================================================
来源：http://ep.jctech888.com.cn

[G01] 定义类
来源：http://ev.bookmarksfly.cn

Py:   class User: pass
来源：http://qk.haigaiapp.cn

PHP:  class User {}
来源：http://bh.colortex.cn

JS:   class User {}
来源：http://oc.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://lg.newstarts.cn

Java: class User {}
来源：http://ci.hnjuh.cn

Go:   type User struct { Name string }
来源：http://jw.yuntaijiaju.cn

Ruby: class User; end
来源：http://jr.newstarts.cn

C#:   class User {}
来源：http://nh.szsharing.cn

[G02] 构造函数
来源：http://wm.panjiajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://yx.yuexingan06.cn

PHP:  public function __construct(public string $name) {}
来源：http://gr.huanxung.cn

JS:   constructor(name) { this.name = name; }
来源：http://cq.shxzskj.cn

TS:   constructor(public name: string) {}
来源：http://yc.szsharing.cn

Java: User(String name) { this.name = name; }
来源：http://dc.nszjky.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xo.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://oc.shxzukj.cn

C#:   public User(string name) { Name = name; }
来源：http://xo.nszjky.cn

[G03] 实例属性
来源：http://mg.szxytkj.cn

Py:   self.name = "x"
来源：http://yy.bjjhwx.cn

PHP:  public string $name = "x";
来源：http://ea.colortex.cn

JS:   this.name = "x";
来源：http://nx.yuexingan06.cn

TS:   name: string = "x";
来源：http://ta.gzmigu.cn

Java: private String name;
来源：http://du.szxytkj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hy.asd995.cn

Ruby: @name = "x"
来源：http://ww.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://zo.newstarts.cn

[G04] 定义方法
来源：http://jl.huanxung.cn

Py:   def greet(self): return self.name
来源：http://dt.colortex.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ow.muxihuayi.cn

JS:   greet() { return this.name; }
来源：http://ot.bjjhwx.cn

TS:   greet(): string { return this.name; }
来源：http://te.huixiangedu.cn

Java: String greet() { return name; }
来源：http://kj.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xq.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://mi.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://br.colortex.cn

[G05] 继承
来源：http://xk.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://uz.asd995.cn

PHP:  class Admin extends User {}
来源：http://db.gzmigu.cn

JS:   class Admin extends User {}
来源：http://gj.521024.cn

TS:   class Admin extends User {}
来源：http://ok.asd995.cn

Java: class Admin extends User {}
来源：http://wc.nicolike.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lt.shxzukj.cn

Ruby: class Admin < User; end
来源：http://zy.lnxyls.cn

C#:   class Admin : User {}
来源：http://ku.szsharing.cn

[G06] 重写方法
来源：http://mb.521024.cn

Py:   def greet(self): return "admin"
来源：http://rb.yuexingan06.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://za.chemitech.net.cn

JS:   greet() { return "admin"; }
来源：http://ox.bookmarksfly.cn

TS:   greet(): string { return "admin"; }
来源：http://qa.shxzskj.cn

Java: @Override String greet() { return "admin"; }
来源：http://lb.9csxet.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ys.bookmarksfly.cn

Ruby: def greet; "admin"; end
来源：http://pc.hnjuh.cn

C#:   public override string Greet() => "admin";
来源：http://hs.wgjwhj.cn

[G07] 调用父类方法
来源：http://os.muxihuayi.cn

Py:   super().greet()
来源：http://ow.nicolike.cn

PHP:  parent::greet();
来源：http://xl.chemitech.net.cn

JS:   super.greet();
来源：http://li.nszjky.cn

TS:   super.greet();
来源：http://bd.nszjky.cn

Java: super.greet();
来源：http://hc.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nq.shxzskj.cn

Ruby: super
来源：http://px.gzmigu.cn

C#:   base.Greet();
来源：http://of.muxihuayi.cn

[G08] 静态方法与属性
来源：http://pf.muxihuayi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://co.521024.cn

PHP:  public static function f() {}
来源：http://qa.nicolike.cn

JS:   static f() {}
来源：http://jj.yuexingan06.cn

TS:   static f(): void {}
来源：http://jc.nicolike.cn

Java: static void f() {}
来源：http://pu.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://oc.nszjky.cn

Ruby: def self.f; end
来源：http://oz.huanxung.cn

C#:   public static void F() {}
来源：http://cq.szsharing.cn

[G09] 接口 / 抽象类
来源：http://sz.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://az.9csxet.cn

PHP:  interface Shape { public function area(): float; }
来源：http://iy.newstarts.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zb.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://vm.muxihuayi.cn

Java: interface Shape { double area(); }
来源：http://wa.jctech888.com.cn

Go:   type Shape interface { Area() float64 }
来源：http://ki.huixinmuqiang.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ym.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://xk.huixinmuqiang.cn

[G10] 访问控制
来源：http://px.colortex.cn

Py:   约定 _protected / __private（不强制）
来源：http://ce.yuexingan06.cn

PHP:  public / protected / private
来源：http://qs.jianghongdianzi.cn

JS:   #private 字段；其余公开
来源：http://fv.lnxyls.cn

TS:   public / protected / private
来源：http://hb.shxzukj.cn

Java: public / protected / private / 默认包级
来源：http://xp.yuexingan06.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fj.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://xo.hahajie.cn

C#:   public / protected / private / internal
来源：http://ec.jianghongdianzi.cn

[G11] getter / setter
来源：http://ng.wgjwhj.cn

Py:   @property 与 @x.setter
来源：http://oh.colortex.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://df.bjjhwx.cn

JS:   get name() { return this._name; }
来源：http://vc.huanxung.cn

TS:   get name(): string { return this._name; }
来源：http://zp.9csxet.cn

Java: public String getName() { return name; }
来源：http://iw.jctech888.com.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kh.huixiangedu.cn

Ruby: attr_accessor :name
来源：http://im.colortex.cn

C#:   public string Name { get; set; }
来源：http://ye.huanxung.cn

[G12] 对象转字符串
来源：http://mn.panjiajie.cn

Py:   def __str__(self): return self.name
来源：http://jy.bjjhwx.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gs.asd995.cn

JS:   toString() { return this.name; }
来源：http://va.hahajie.cn

TS:   toString(): string { return this.name; }
来源：http://gf.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://cb.shtwfgs.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nj.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://rw.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://bw.hahajie.cn

[G13] 判断对象类型
来源：http://li.gzmigu.cn

Py:   isinstance(u, User)
来源：http://lf.colortex.cn

PHP:  $u instanceof User
来源：http://fs.yuexingan06.cn

JS:   u instanceof User
来源：http://zf.muxihuayi.cn

TS:   u instanceof User
来源：http://aa.jctech888.com.cn

Java: u instanceof User
来源：http://bb.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ml.colortex.cn

Ruby: u.is_a?(User)
来源：http://cv.nicolike.cn

C#:   u is User
来源：http://jh.bookmarksfly.cn

[G14] 数据类 / record
来源：http://lu.nszjky.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://eh.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://cm.panjiajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gh.newstarts.cn

TS:   type User = { name: string; age: number };
来源：http://bl.huixiangedu.cn

Java: record User(String name, int age) {}
来源：http://oa.shxzskj.cn

Go:   type User struct { Name string; Age int }
来源：http://nx.bookmarksfly.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jv.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://rz.shxzukj.cn

[G15] 枚举
来源：http://oh.shtwfgs.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kn.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ih.haigaiapp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yk.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tr.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://fg.yuntaijiaju.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://iy.muxihuayi.cn

Ruby: Color = %i[red green].freeze
来源：http://uh.asd995.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://be.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://vu.szxytkj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bk.muxihuayi.cn

PHP:  get_object_vars($obj);
来源：http://dm.huixinmuqiang.cn

JS:   Object.entries(obj)
来源：http://gr.muxihuayi.cn

TS:   Object.entries(obj)
来源：http://oq.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nd.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pn.9csxet.cn

Ruby: obj.instance_variables
来源：http://kt.jianghongdianzi.cn

C#:   // 用反射或 System.Text.Json
来源：http://ni.shxzskj.cn

================================================================================
来源：http://vt.hahajie.cn

H. 异常与错误处理
来源：http://pe.jianghongdianzi.cn

================================================================================
来源：http://xg.nicolike.cn

[H01] try / catch 基础
来源：http://uu.shxzukj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oz.panjiajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sm.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yq.chemitech.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nq.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bc.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://im.szxytkj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jb.shtwfgs.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zz.hnjuh.cn

[H02] finally / ensure 收尾
来源：http://ni.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zn.newstarts.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ez.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://uc.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hw.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ny.lnxyls.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tc.hnjuh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kr.chemitech.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ud.huixinmuqiang.cn

[H03] 主动抛出异常
来源：http://ym.bookmarksfly.cn

Py:   raise ValueError("错误信息")
来源：http://dq.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ey.shxzskj.cn

JS:   throw new Error("错误信息");
来源：http://bq.szsharing.cn


<!-- 参考信息 -->