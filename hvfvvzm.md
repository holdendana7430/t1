代发 wailian999

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qt.szxytkj.cn

Go:   // 按 rune 判断长度后截断
来源：http://oj.panjiajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jk.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://bw.hnjuh.cn

[E22] 字节长度与字符长度
来源：http://ma.yuntaijiaju.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://og.hahajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wi.hahajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://yk.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dx.521024.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mc.jianghongdianzi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mr.szsharing.cn

Ruby: s.bytesize;  s.length
来源：http://zf.wgjwhj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fg.huixiangedu.cn

================================================================================
来源：http://ll.wgjwhj.cn

F. 文件与目录
来源：http://md.521024.cn

================================================================================
来源：http://zg.9csxet.cn

[F01] 读取整个文件
来源：http://ln.newstarts.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uh.panjiajie.cn

PHP:  file_get_contents("a.txt");
来源：http://re.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zs.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ww.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nr.shxzskj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oq.hnjuh.cn

Ruby: File.read("a.txt")
来源：http://zq.hnjuh.cn

C#:   File.ReadAllText("a.txt");
来源：http://bd.muxihuayi.cn

[F02] 逐行读取文件
来源：http://sh.gzmigu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ni.hahajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gt.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vg.nszjky.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hl.asd995.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ka.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://at.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lh.nicolike.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ob.nszjky.cn

[F03] 写入文件（覆盖）
来源：http://dq.gzmigu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://bv.gzmigu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ql.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tq.szsharing.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pu.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dh.szsharing.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://se.shxzskj.cn

Ruby: File.write("a.txt", "hi")
来源：http://pc.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pi.nicolike.cn

[F04] 追加写入文件
来源：http://oo.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://od.shxzskj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zw.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.9csxet.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ti.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lh.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://th.shxzskj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yh.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rn.yuntaijiaju.cn

[F05] 判断文件或目录是否存在
来源：http://kp.shtwfgs.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gk.huixiangedu.cn

PHP:  file_exists("a.txt");
来源：http://nm.wgjwhj.cn

JS:   fs.existsSync("a.txt")
来源：http://cr.chemitech.net.cn

TS:   fs.existsSync("a.txt")
来源：http://gg.colortex.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gm.wgjwhj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wz.yuexingan06.cn

Ruby: File.exist?("a.txt")
来源：http://xd.shxzukj.cn

C#:   File.Exists("a.txt")
来源：http://km.szxytkj.cn

[F06] 删除文件
来源：http://rl.hahajie.cn

Py:   os.remove("a.txt")
来源：http://dq.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://ib.nszjky.cn

JS:   fs.unlinkSync("a.txt")
来源：http://dw.colortex.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yt.shxzukj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fv.nszjky.cn

Go:   os.Remove("a.txt")
来源：http://iy.asd995.cn

Ruby: File.delete("a.txt")
来源：http://ue.yuntaijiaju.cn

C#:   File.Delete("a.txt");
来源：http://kt.newstarts.cn

[F07] 创建目录（含多级）
来源：http://tp.colortex.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ta.huixinmuqiang.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wl.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jb.bjjhwx.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jm.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ec.colortex.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bm.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ke.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://tq.shtwfgs.cn

[F08] 遍历目录
来源：http://ku.bookmarksfly.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ep.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oc.huixinmuqiang.cn

JS:   fs.readdirSync("dir")
来源：http://na.chemitech.net.cn

TS:   fs.readdirSync("dir")
来源：http://gp.nszjky.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ut.haigaiapp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pa.panjiajie.cn

Ruby: Dir.children("dir")
来源：http://sb.bookmarksfly.cn

C#:   Directory.GetFiles("dir")
来源：http://oz.shxzskj.cn

[F09] 获取文件大小
来源：http://vh.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://oq.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://ez.asd995.cn

JS:   fs.statSync("a.txt").size
来源：http://ei.9csxet.cn

TS:   fs.statSync("a.txt").size
来源：http://tt.nszjky.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fq.jctech888.com.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://eb.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://oo.shxzukj.cn

C#:   new FileInfo("a.txt").Length
来源：http://wo.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://qw.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ng.muxihuayi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://np.nszjky.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://pl.huixinmuqiang.cn

TS:   path.extname("a.txt")
来源：http://kx.hnjuh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dk.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://jc.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://al.hahajie.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wl.chemitech.net.cn

[F11] 复制与移动文件
来源：http://uo.jianghongdianzi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gq.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gn.9csxet.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wh.szsharing.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://le.huixiangedu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mo.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bk.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://va.szxytkj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cf.szsharing.cn

[F12] CSV 读写
来源：http://gm.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xv.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qu.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dl.lnxyls.cn

TS:   // 同上
来源：http://dv.shxzukj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fh.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ok.jctech888.com.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cm.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://uj.huixinmuqiang.cn

================================================================================
来源：http://ak.gzmigu.cn

G. 面向对象
来源：http://pk.nicolike.cn

================================================================================
来源：http://xd.lnxyls.cn

[G01] 定义类
来源：http://nd.huixiangedu.cn

Py:   class User: pass
来源：http://yn.jctech888.com.cn

PHP:  class User {}
来源：http://zz.9csxet.cn

JS:   class User {}
来源：http://hd.shtwfgs.cn

TS:   class User { name: string = ""; }
来源：http://ub.muxihuayi.cn

Java: class User {}
来源：http://us.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://jt.szsharing.cn

Ruby: class User; end
来源：http://hh.szsharing.cn

C#:   class User {}
来源：http://zn.newstarts.cn

[G02] 构造函数
来源：http://ae.gzmigu.cn

Py:   def __init__(self, name): self.name = name
来源：http://ue.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://oe.nszjky.cn

JS:   constructor(name) { this.name = name; }
来源：http://zu.gzmigu.cn

TS:   constructor(public name: string) {}
来源：http://al.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://dm.newstarts.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rp.colortex.cn

Ruby: def initialize(name); @name = name; end
来源：http://sc.shxzukj.cn

C#:   public User(string name) { Name = name; }
来源：http://nb.gzmigu.cn

[G03] 实例属性
来源：http://py.asd995.cn

Py:   self.name = "x"
来源：http://eo.yuntaijiaju.cn

PHP:  public string $name = "x";
来源：http://mx.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://ks.haigaiapp.cn

TS:   name: string = "x";
来源：http://pm.hahajie.cn

Java: private String name;
来源：http://uh.chemitech.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bn.asd995.cn

Ruby: @name = "x"
来源：http://mr.jianghongdianzi.cn

C#:   public string Name { get; set; } = "x";
来源：http://hk.wgjwhj.cn

[G04] 定义方法
来源：http://ze.bookmarksfly.cn

Py:   def greet(self): return self.name
来源：http://xs.haigaiapp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://lk.lnxyls.cn

JS:   greet() { return this.name; }
来源：http://yq.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://gn.lnxyls.cn

Java: String greet() { return name; }
来源：http://mh.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cl.szsharing.cn

Ruby: def greet; @name; end
来源：http://zh.huanxung.cn

C#:   public string Greet() => Name;
来源：http://jj.bookmarksfly.cn

[G05] 继承
来源：http://ps.szxytkj.cn

Py:   class Admin(User): pass
来源：http://lt.szxytkj.cn

PHP:  class Admin extends User {}
来源：http://du.gzmigu.cn

JS:   class Admin extends User {}
来源：http://qt.asd995.cn

TS:   class Admin extends User {}
来源：http://fj.colortex.cn

Java: class Admin extends User {}
来源：http://ec.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://td.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://bl.panjiajie.cn

C#:   class Admin : User {}
来源：http://pr.haigaiapp.cn

[G06] 重写方法
来源：http://mi.colortex.cn

Py:   def greet(self): return "admin"
来源：http://cy.9csxet.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ln.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://ei.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://zp.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://kv.hnjuh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vg.bookmarksfly.cn

Ruby: def greet; "admin"; end
来源：http://yn.huixiangedu.cn

C#:   public override string Greet() => "admin";
来源：http://zw.yuexingan06.cn

[G07] 调用父类方法
来源：http://vl.colortex.cn

Py:   super().greet()
来源：http://fs.huixiangedu.cn

PHP:  parent::greet();
来源：http://sy.bjjhwx.cn

JS:   super.greet();
来源：http://oe.shtwfgs.cn

TS:   super.greet();
来源：http://hx.hnjuh.cn

Java: super.greet();
来源：http://st.shxzukj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://de.shtwfgs.cn

Ruby: super
来源：http://ll.shxzukj.cn

C#:   base.Greet();
来源：http://on.huixinmuqiang.cn

[G08] 静态方法与属性
来源：http://tv.gzmigu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uo.bjjhwx.cn

PHP:  public static function f() {}
来源：http://xl.jctech888.com.cn

JS:   static f() {}
来源：http://io.shxzskj.cn

TS:   static f(): void {}
来源：http://ox.chemitech.net.cn

Java: static void f() {}
来源：http://rb.haigaiapp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kr.chemitech.net.cn

Ruby: def self.f; end
来源：http://jy.bookmarksfly.cn

C#:   public static void F() {}
来源：http://vm.shxzskj.cn

[G09] 接口 / 抽象类
来源：http://wb.yuntaijiaju.cn

Py:   from abc import ABC, abstractmethod
来源：http://jq.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ii.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://se.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://bl.szsharing.cn

Java: interface Shape { double area(); }
来源：http://jw.newstarts.cn

Go:   type Shape interface { Area() float64 }
来源：http://lq.asd995.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://at.bjjhwx.cn

C#:   interface IShape { double Area(); }
来源：http://gs.hahajie.cn

[G10] 访问控制
来源：http://zz.shxzukj.cn

Py:   约定 _protected / __private（不强制）
来源：http://gj.colortex.cn

PHP:  public / protected / private
来源：http://aw.szxytkj.cn

JS:   #private 字段；其余公开
来源：http://hh.yuntaijiaju.cn

TS:   public / protected / private
来源：http://aq.huixinmuqiang.cn

Java: public / protected / private / 默认包级
来源：http://pr.shxzukj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rl.shtwfgs.cn

Ruby: public / protected / private
来源：http://sj.bookmarksfly.cn

C#:   public / protected / private / internal
来源：http://wv.bjjhwx.cn

[G11] getter / setter
来源：http://rt.shxzukj.cn

Py:   @property 与 @x.setter
来源：http://oq.jianghongdianzi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://et.jianghongdianzi.cn

JS:   get name() { return this._name; }
来源：http://hg.panjiajie.cn

TS:   get name(): string { return this._name; }
来源：http://sw.huanxung.cn

Java: public String getName() { return name; }
来源：http://mm.gzmigu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ml.lnxyls.cn

Ruby: attr_accessor :name
来源：http://wr.hnjuh.cn

C#:   public string Name { get; set; }
来源：http://ec.newstarts.cn

[G12] 对象转字符串
来源：http://qw.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://wj.bjjhwx.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://we.9csxet.cn

JS:   toString() { return this.name; }
来源：http://uh.asd995.cn

TS:   toString(): string { return this.name; }
来源：http://lb.shxzukj.cn

Java: @Override public String toString() { return name; }
来源：http://gb.colortex.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vi.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://jy.gzmigu.cn

C#:   public override string ToString() => Name;
来源：http://bs.yuexingan06.cn

[G13] 判断对象类型
来源：http://wj.szxytkj.cn

Py:   isinstance(u, User)
来源：http://mg.muxihuayi.cn

PHP:  $u instanceof User
来源：http://ps.yuntaijiaju.cn

JS:   u instanceof User
来源：http://eg.gzmigu.cn

TS:   u instanceof User
来源：http://rf.jianghongdianzi.cn

Java: u instanceof User
来源：http://ny.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zk.panjiajie.cn

Ruby: u.is_a?(User)
来源：http://vs.bjjhwx.cn

C#:   u is User
来源：http://fl.haigaiapp.cn

[G14] 数据类 / record
来源：http://yb.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ju.hnjuh.cn

PHP:  // 用 readonly 属性模拟
来源：http://gf.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fj.gzmigu.cn

TS:   type User = { name: string; age: number };
来源：http://do.gzmigu.cn

Java: record User(String name, int age) {}
来源：http://dd.huanxung.cn

Go:   type User struct { Name string; Age int }
来源：http://le.szxytkj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://an.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://hx.haigaiapp.cn

[G15] 枚举
来源：http://jd.shtwfgs.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pd.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ol.szsharing.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://al.muxihuayi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lc.szxytkj.cn

Java: enum Color { RED, GREEN }
来源：http://jd.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uf.lnxyls.cn

Ruby: Color = %i[red green].freeze
来源：http://aw.521024.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ib.colortex.cn

[G16] 对象转数组 / 字典
来源：http://fm.colortex.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zi.asd995.cn

PHP:  get_object_vars($obj);
来源：http://wk.yuntaijiaju.cn

JS:   Object.entries(obj)
来源：http://sj.lnxyls.cn

TS:   Object.entries(obj)
来源：http://nq.muxihuayi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pt.hnjuh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wf.chemitech.net.cn

Ruby: obj.instance_variables
来源：http://zg.nicolike.cn

C#:   // 用反射或 System.Text.Json
来源：http://do.jctech888.com.cn

================================================================================
来源：http://hm.chemitech.net.cn

H. 异常与错误处理
来源：http://yi.muxihuayi.cn

================================================================================
来源：http://hu.panjiajie.cn

[H01] try / catch 基础
来源：http://cv.muxihuayi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tt.wgjwhj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fz.muxihuayi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sf.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uh.bookmarksfly.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zw.shxzskj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zi.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gj.gzmigu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sa.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://xp.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://aj.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wn.jianghongdianzi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ps.hahajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mg.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dz.yuexingan06.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://uc.shxzskj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://uh.chemitech.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hv.muxihuayi.cn

[H03] 主动抛出异常
来源：http://bd.hahajie.cn

Py:   raise ValueError("错误信息")
来源：http://hr.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kh.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://sk.jctech888.com.cn

TS:   throw new Error("错误信息");
来源：http://mu.newstarts.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jd.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kb.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tu.huixiangedu.cn


<!-- 参考信息 -->