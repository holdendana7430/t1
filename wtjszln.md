代发 wailian999

[F01] 读取整个文件
来源：http://gc.shxzskj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lu.jianghongdianzi.cn

PHP:  file_get_contents("a.txt");
来源：http://ku.yuntaijiaju.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lr.bookmarksfly.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://om.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lx.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hx.newstarts.cn

Ruby: File.read("a.txt")
来源：http://lp.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://wj.hahajie.cn

[F02] 逐行读取文件
来源：http://au.521024.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://df.lnxyls.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uo.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jx.haigaiapp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xm.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cq.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ln.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mp.wgjwhj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xz.yuntaijiaju.cn

[F03] 写入文件（覆盖）
来源：http://un.szsharing.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rl.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gb.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zu.haigaiapp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qe.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yh.newstarts.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ll.hahajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://si.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yn.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://qe.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://xm.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yp.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ue.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hb.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fq.bookmarksfly.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rq.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://md.huanxung.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lg.wgjwhj.cn

[F05] 判断文件或目录是否存在
来源：http://id.shtwfgs.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jb.9csxet.cn

PHP:  file_exists("a.txt");
来源：http://mc.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://lb.muxihuayi.cn

TS:   fs.existsSync("a.txt")
来源：http://qy.521024.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://br.hahajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qy.9csxet.cn

Ruby: File.exist?("a.txt")
来源：http://ax.gzmigu.cn

C#:   File.Exists("a.txt")
来源：http://ma.szsharing.cn

[F06] 删除文件
来源：http://as.muxihuayi.cn

Py:   os.remove("a.txt")
来源：http://sl.yuexingan06.cn

PHP:  unlink("a.txt");
来源：http://mf.nszjky.cn

JS:   fs.unlinkSync("a.txt")
来源：http://jx.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://yp.newstarts.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ki.panjiajie.cn

Go:   os.Remove("a.txt")
来源：http://bg.bjjhwx.cn

Ruby: File.delete("a.txt")
来源：http://lr.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://sv.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://dm.nicolike.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jb.hahajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iu.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nl.521024.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xr.nszjky.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ui.newstarts.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ob.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://oj.yuexingan06.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ue.huixiangedu.cn

[F08] 遍历目录
来源：http://nw.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ip.chemitech.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tg.panjiajie.cn

JS:   fs.readdirSync("dir")
来源：http://tt.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://nx.bjjhwx.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hu.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://he.szxytkj.cn

Ruby: Dir.children("dir")
来源：http://bd.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://vj.bookmarksfly.cn

[F09] 获取文件大小
来源：http://fb.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://hb.nszjky.cn

PHP:  filesize("a.txt");
来源：http://ng.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://yr.shxzskj.cn

TS:   fs.statSync("a.txt").size
来源：http://mo.muxihuayi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rj.jctech888.com.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bp.521024.cn

Ruby: File.size("a.txt")
来源：http://bw.nszjky.cn

C#:   new FileInfo("a.txt").Length
来源：http://nt.bjjhwx.cn

[F10] 取文件扩展名 / 文件名
来源：http://rt.bjjhwx.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bw.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oh.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zz.huixinmuqiang.cn

TS:   path.extname("a.txt")
来源：http://ef.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pc.521024.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pk.huixiangedu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dg.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vg.newstarts.cn

[F11] 复制与移动文件
来源：http://wi.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ok.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wd.nicolike.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tt.jctech888.com.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dk.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://tl.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://aa.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dp.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ji.panjiajie.cn

[F12] CSV 读写
来源：http://zm.hnjuh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ur.yuexingan06.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rq.yuexingan06.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cg.szsharing.cn

TS:   // 同上
来源：http://pc.muxihuayi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zf.szsharing.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cr.muxihuayi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hh.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pe.szxytkj.cn

================================================================================
来源：http://us.shxzukj.cn

G. 面向对象
来源：http://nm.nicolike.cn

================================================================================
来源：http://qg.newstarts.cn

[G01] 定义类
来源：http://fb.huanxung.cn

Py:   class User: pass
来源：http://fm.panjiajie.cn

PHP:  class User {}
来源：http://sn.newstarts.cn

JS:   class User {}
来源：http://sa.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://oa.yuexingan06.cn

Java: class User {}
来源：http://vp.521024.cn

Go:   type User struct { Name string }
来源：http://sz.bjjhwx.cn

Ruby: class User; end
来源：http://ua.szxytkj.cn

C#:   class User {}
来源：http://qr.hnjuh.cn

[G02] 构造函数
来源：http://tk.colortex.cn

Py:   def __init__(self, name): self.name = name
来源：http://zb.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://wa.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://rv.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://os.jctech888.com.cn

Java: User(String name) { this.name = name; }
来源：http://vp.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zd.szsharing.cn

Ruby: def initialize(name); @name = name; end
来源：http://xk.shxzskj.cn

C#:   public User(string name) { Name = name; }
来源：http://na.lnxyls.cn

[G03] 实例属性
来源：http://ba.wgjwhj.cn

Py:   self.name = "x"
来源：http://du.szxytkj.cn

PHP:  public string $name = "x";
来源：http://ag.yuexingan06.cn

JS:   this.name = "x";
来源：http://jq.newstarts.cn

TS:   name: string = "x";
来源：http://td.muxihuayi.cn

Java: private String name;
来源：http://mb.nszjky.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wc.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://vd.bjjhwx.cn

C#:   public string Name { get; set; } = "x";
来源：http://be.newstarts.cn

[G04] 定义方法
来源：http://ax.9csxet.cn

Py:   def greet(self): return self.name
来源：http://iu.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://rt.9csxet.cn

JS:   greet() { return this.name; }
来源：http://vk.asd995.cn

TS:   greet(): string { return this.name; }
来源：http://vy.wgjwhj.cn

Java: String greet() { return name; }
来源：http://jv.lnxyls.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wf.shtwfgs.cn

Ruby: def greet; @name; end
来源：http://hd.colortex.cn

C#:   public string Greet() => Name;
来源：http://il.bookmarksfly.cn

[G05] 继承
来源：http://nc.szxytkj.cn

Py:   class Admin(User): pass
来源：http://gj.hahajie.cn

PHP:  class Admin extends User {}
来源：http://rf.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://uy.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://vh.newstarts.cn

Java: class Admin extends User {}
来源：http://bw.szxytkj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ca.nicolike.cn

Ruby: class Admin < User; end
来源：http://et.jctech888.com.cn

C#:   class Admin : User {}
来源：http://lo.yuntaijiaju.cn

[G06] 重写方法
来源：http://ad.shtwfgs.cn

Py:   def greet(self): return "admin"
来源：http://ny.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nk.gzmigu.cn

JS:   greet() { return "admin"; }
来源：http://mu.szxytkj.cn

TS:   greet(): string { return "admin"; }
来源：http://pf.haigaiapp.cn

Java: @Override String greet() { return "admin"; }
来源：http://to.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dr.yuexingan06.cn

Ruby: def greet; "admin"; end
来源：http://vq.shxzukj.cn

C#:   public override string Greet() => "admin";
来源：http://fg.9csxet.cn

[G07] 调用父类方法
来源：http://lc.muxihuayi.cn

Py:   super().greet()
来源：http://iu.nicolike.cn

PHP:  parent::greet();
来源：http://ri.nszjky.cn

JS:   super.greet();
来源：http://aw.shxzskj.cn

TS:   super.greet();
来源：http://dp.jctech888.com.cn

Java: super.greet();
来源：http://jt.huixiangedu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yq.521024.cn

Ruby: super
来源：http://yi.bjjhwx.cn

C#:   base.Greet();
来源：http://vc.szxytkj.cn

[G08] 静态方法与属性
来源：http://fe.muxihuayi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nk.shxzukj.cn

PHP:  public static function f() {}
来源：http://dh.lnxyls.cn

JS:   static f() {}
来源：http://of.huixiangedu.cn

TS:   static f(): void {}
来源：http://ur.huixinmuqiang.cn

Java: static void f() {}
来源：http://up.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cg.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://mv.szsharing.cn

C#:   public static void F() {}
来源：http://gv.huixinmuqiang.cn

[G09] 接口 / 抽象类
来源：http://dc.haigaiapp.cn

Py:   from abc import ABC, abstractmethod
来源：http://lz.huanxung.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nh.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mj.nszjky.cn

TS:   interface Shape { area(): number; }
来源：http://jm.yuntaijiaju.cn

Java: interface Shape { double area(); }
来源：http://yl.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://mf.hnjuh.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gw.nicolike.cn

C#:   interface IShape { double Area(); }
来源：http://ur.gzmigu.cn

[G10] 访问控制
来源：http://xl.9csxet.cn

Py:   约定 _protected / __private（不强制）
来源：http://ea.hahajie.cn

PHP:  public / protected / private
来源：http://uh.jianghongdianzi.cn

JS:   #private 字段；其余公开
来源：http://lw.panjiajie.cn

TS:   public / protected / private
来源：http://ax.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://xu.yuexingan06.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vh.yuntaijiaju.cn

Ruby: public / protected / private
来源：http://ts.bjjhwx.cn

C#:   public / protected / private / internal
来源：http://yd.shxzskj.cn

[G11] getter / setter
来源：http://wk.nszjky.cn

Py:   @property 与 @x.setter
来源：http://ox.chemitech.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lz.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://gr.9csxet.cn

TS:   get name(): string { return this._name; }
来源：http://op.gzmigu.cn

Java: public String getName() { return name; }
来源：http://hj.jianghongdianzi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ic.shxzskj.cn

Ruby: attr_accessor :name
来源：http://ew.chemitech.net.cn

C#:   public string Name { get; set; }
来源：http://qn.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://be.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://oi.9csxet.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vx.521024.cn

JS:   toString() { return this.name; }
来源：http://rc.asd995.cn

TS:   toString(): string { return this.name; }
来源：http://so.hnjuh.cn

Java: @Override public String toString() { return name; }
来源：http://km.hahajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ts.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://zo.521024.cn

C#:   public override string ToString() => Name;
来源：http://dy.colortex.cn

[G13] 判断对象类型
来源：http://tn.huixiangedu.cn

Py:   isinstance(u, User)
来源：http://aj.muxihuayi.cn

PHP:  $u instanceof User
来源：http://gi.chemitech.net.cn

JS:   u instanceof User
来源：http://yy.shtwfgs.cn

TS:   u instanceof User
来源：http://sk.jianghongdianzi.cn

Java: u instanceof User
来源：http://qo.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://om.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://ux.lnxyls.cn

C#:   u is User
来源：http://uc.colortex.cn

[G14] 数据类 / record
来源：http://fr.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://si.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://li.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ij.yuexingan06.cn

TS:   type User = { name: string; age: number };
来源：http://me.hnjuh.cn

Java: record User(String name, int age) {}
来源：http://op.jianghongdianzi.cn

Go:   type User struct { Name string; Age int }
来源：http://nc.asd995.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ug.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://kd.bjjhwx.cn

[G15] 枚举
来源：http://nv.wgjwhj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pb.shxzskj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wj.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fu.wgjwhj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://li.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://wa.hnjuh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kw.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://ku.huixinmuqiang.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hp.shxzskj.cn

[G16] 对象转数组 / 字典
来源：http://sv.panjiajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lv.chemitech.net.cn

PHP:  get_object_vars($obj);
来源：http://wg.shtwfgs.cn

JS:   Object.entries(obj)
来源：http://bg.9csxet.cn

TS:   Object.entries(obj)
来源：http://gc.nicolike.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dj.yuntaijiaju.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gn.lnxyls.cn

Ruby: obj.instance_variables
来源：http://wy.jianghongdianzi.cn

C#:   // 用反射或 System.Text.Json
来源：http://mb.gzmigu.cn

================================================================================
来源：http://zx.lnxyls.cn

H. 异常与错误处理
来源：http://cx.wgjwhj.cn

================================================================================
来源：http://ao.muxihuayi.cn

[H01] try / catch 基础
来源：http://fg.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oz.wgjwhj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vd.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yx.lnxyls.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jk.521024.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://we.nszjky.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://al.521024.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rb.muxihuayi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ak.huixiangedu.cn

[H02] finally / ensure 收尾
来源：http://xd.huanxung.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pb.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jl.szxytkj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bb.nszjky.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gy.hahajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ep.muxihuayi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lj.yuexingan06.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://np.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gn.panjiajie.cn

[H03] 主动抛出异常
来源：http://jr.chemitech.net.cn

Py:   raise ValueError("错误信息")
来源：http://dy.szsharing.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gu.haigaiapp.cn

JS:   throw new Error("错误信息");
来源：http://yv.521024.cn

TS:   throw new Error("错误信息");
来源：http://kn.nicolike.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ad.nicolike.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hf.szxytkj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bg.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wg.huixiangedu.cn

[H04] 自定义异常类型
来源：http://sk.nicolike.cn

Py:   class MyError(Exception): pass
来源：http://np.asd995.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fs.yuntaijiaju.cn

JS:   class MyError extends Error {}
来源：http://gk.9csxet.cn

TS:   class MyError extends Error {}
来源：http://zb.panjiajie.cn

Java: class MyException extends RuntimeException {}
来源：http://ts.bookmarksfly.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rv.huixinmuqiang.cn

Ruby: class MyError < StandardError; end
来源：http://ct.wgjwhj.cn

C#:   class MyException : Exception {}
来源：http://lc.panjiajie.cn

[H05] 捕获特定类型
来源：http://qd.lnxyls.cn

Py:   except ValueError as e:
来源：http://cq.huixiangedu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hb.colortex.cn

JS:   if (e instanceof TypeError) {}
来源：http://kg.yuntaijiaju.cn

TS:   if (e instanceof TypeError) {}
来源：http://wy.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://xr.jianghongdianzi.cn


<!-- 参考信息 -->