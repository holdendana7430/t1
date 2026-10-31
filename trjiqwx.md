代发 wailian999

[F01] 读取整个文件
来源：http://bv.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ef.szsharing.cn

PHP:  file_get_contents("a.txt");
来源：http://hh.shxzukj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vu.shxzskj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lp.hnjuh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://cy.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://xr.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://gt.9csxet.cn

C#:   File.ReadAllText("a.txt");
来源：http://qm.wgjwhj.cn

[F02] 逐行读取文件
来源：http://pq.nicolike.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ax.colortex.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yh.szxytkj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ml.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lp.newstarts.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gh.lnxyls.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://zh.huixiangedu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lg.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xq.haigaiapp.cn

[F03] 写入文件（覆盖）
来源：http://xj.huanxung.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xi.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qz.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sy.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ox.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dq.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://po.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://xn.gzmigu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://cj.jctech888.com.cn

[F04] 追加写入文件
来源：http://kq.shxzukj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tp.nicolike.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://la.nicolike.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fh.yuntaijiaju.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nj.colortex.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ts.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rx.bookmarksfly.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pj.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://le.jianghongdianzi.cn

[F05] 判断文件或目录是否存在
来源：http://iw.jctech888.com.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wu.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://bk.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://gm.jctech888.com.cn

TS:   fs.existsSync("a.txt")
来源：http://lb.gzmigu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://do.chemitech.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://le.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://ah.yuntaijiaju.cn

C#:   File.Exists("a.txt")
来源：http://iv.gzmigu.cn

[F06] 删除文件
来源：http://sc.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://rc.newstarts.cn

PHP:  unlink("a.txt");
来源：http://ck.nszjky.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nw.shtwfgs.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zv.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jl.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://ef.gzmigu.cn

Ruby: File.delete("a.txt")
来源：http://wi.jianghongdianzi.cn

C#:   File.Delete("a.txt");
来源：http://of.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://js.yuntaijiaju.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jv.wgjwhj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qo.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://as.muxihuayi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mo.asd995.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ke.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jr.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://xn.shtwfgs.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bv.521024.cn

[F08] 遍历目录
来源：http://cu.szxytkj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ya.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://tk.panjiajie.cn

JS:   fs.readdirSync("dir")
来源：http://tl.yuntaijiaju.cn

TS:   fs.readdirSync("dir")
来源：http://iz.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bk.newstarts.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://hy.colortex.cn

Ruby: Dir.children("dir")
来源：http://ku.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://nr.gzmigu.cn

[F09] 获取文件大小
来源：http://qb.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://vo.shxzukj.cn

PHP:  filesize("a.txt");
来源：http://yn.hnjuh.cn

JS:   fs.statSync("a.txt").size
来源：http://zn.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://no.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://aq.yuexingan06.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ei.huixinmuqiang.cn

Ruby: File.size("a.txt")
来源：http://cz.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://jf.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://hp.shxzukj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sn.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://aj.szsharing.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fo.yuntaijiaju.cn

TS:   path.extname("a.txt")
来源：http://sm.muxihuayi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://om.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sc.521024.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gq.lnxyls.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wv.huixiangedu.cn

[F11] 复制与移动文件
来源：http://gs.muxihuayi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fp.yuexingan06.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://um.nicolike.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wv.szsharing.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ck.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hk.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vl.lnxyls.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yo.chemitech.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jc.colortex.cn

[F12] CSV 读写
来源：http://oo.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fz.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qa.jianghongdianzi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hh.haigaiapp.cn

TS:   // 同上
来源：http://zn.gzmigu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dg.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vp.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lv.jianghongdianzi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lj.bookmarksfly.cn

================================================================================
来源：http://gq.shxzskj.cn

G. 面向对象
来源：http://yy.shtwfgs.cn

================================================================================
来源：http://qm.nszjky.cn

[G01] 定义类
来源：http://bs.wgjwhj.cn

Py:   class User: pass
来源：http://lb.nszjky.cn

PHP:  class User {}
来源：http://it.wgjwhj.cn

JS:   class User {}
来源：http://pj.hnjuh.cn

TS:   class User { name: string = ""; }
来源：http://dh.jianghongdianzi.cn

Java: class User {}
来源：http://tx.lnxyls.cn

Go:   type User struct { Name string }
来源：http://iq.yuexingan06.cn

Ruby: class User; end
来源：http://mo.colortex.cn

C#:   class User {}
来源：http://pb.hahajie.cn

[G02] 构造函数
来源：http://wn.bookmarksfly.cn

Py:   def __init__(self, name): self.name = name
来源：http://rl.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://ai.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://wf.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://aj.hahajie.cn

Java: User(String name) { this.name = name; }
来源：http://mz.yuntaijiaju.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lt.muxihuayi.cn

Ruby: def initialize(name); @name = name; end
来源：http://zs.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://yi.szsharing.cn

[G03] 实例属性
来源：http://ni.colortex.cn

Py:   self.name = "x"
来源：http://fb.yuntaijiaju.cn

PHP:  public string $name = "x";
来源：http://bp.muxihuayi.cn

JS:   this.name = "x";
来源：http://on.shxzukj.cn

TS:   name: string = "x";
来源：http://ry.shxzukj.cn

Java: private String name;
来源：http://uq.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lv.hnjuh.cn

Ruby: @name = "x"
来源：http://lj.shxzskj.cn

C#:   public string Name { get; set; } = "x";
来源：http://ef.jianghongdianzi.cn

[G04] 定义方法
来源：http://vs.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://cc.shxzukj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://td.lnxyls.cn

JS:   greet() { return this.name; }
来源：http://ac.shxzskj.cn

TS:   greet(): string { return this.name; }
来源：http://sp.wgjwhj.cn

Java: String greet() { return name; }
来源：http://mx.asd995.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://iw.hnjuh.cn

Ruby: def greet; @name; end
来源：http://oo.9csxet.cn

C#:   public string Greet() => Name;
来源：http://dh.szxytkj.cn

[G05] 继承
来源：http://ra.jctech888.com.cn

Py:   class Admin(User): pass
来源：http://gx.gzmigu.cn

PHP:  class Admin extends User {}
来源：http://rp.521024.cn

JS:   class Admin extends User {}
来源：http://ug.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://pf.nszjky.cn

Java: class Admin extends User {}
来源：http://zl.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nx.lnxyls.cn

Ruby: class Admin < User; end
来源：http://yx.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://ue.nicolike.cn

[G06] 重写方法
来源：http://lm.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://cg.bookmarksfly.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hg.yuexingan06.cn

JS:   greet() { return "admin"; }
来源：http://cw.muxihuayi.cn

TS:   greet(): string { return "admin"; }
来源：http://qc.shxzskj.cn

Java: @Override String greet() { return "admin"; }
来源：http://zh.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ae.huixiangedu.cn

Ruby: def greet; "admin"; end
来源：http://fb.szxytkj.cn

C#:   public override string Greet() => "admin";
来源：http://hc.yuexingan06.cn

[G07] 调用父类方法
来源：http://re.hahajie.cn

Py:   super().greet()
来源：http://mi.hnjuh.cn

PHP:  parent::greet();
来源：http://fk.bookmarksfly.cn

JS:   super.greet();
来源：http://ee.huixiangedu.cn

TS:   super.greet();
来源：http://mj.shtwfgs.cn

Java: super.greet();
来源：http://uc.colortex.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gd.asd995.cn

Ruby: super
来源：http://uf.yuntaijiaju.cn

C#:   base.Greet();
来源：http://rs.bookmarksfly.cn

[G08] 静态方法与属性
来源：http://yg.chemitech.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ve.asd995.cn

PHP:  public static function f() {}
来源：http://hd.newstarts.cn

JS:   static f() {}
来源：http://ib.newstarts.cn

TS:   static f(): void {}
来源：http://uw.yuntaijiaju.cn

Java: static void f() {}
来源：http://vv.shxzskj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qv.9csxet.cn

Ruby: def self.f; end
来源：http://wd.huanxung.cn

C#:   public static void F() {}
来源：http://vl.nicolike.cn

[G09] 接口 / 抽象类
来源：http://xv.nicolike.cn

Py:   from abc import ABC, abstractmethod
来源：http://hb.shtwfgs.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ol.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vi.asd995.cn

TS:   interface Shape { area(): number; }
来源：http://fn.bjjhwx.cn

Java: interface Shape { double area(); }
来源：http://pq.huixinmuqiang.cn

Go:   type Shape interface { Area() float64 }
来源：http://ra.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://eb.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://vu.hnjuh.cn

[G10] 访问控制
来源：http://hm.nicolike.cn

Py:   约定 _protected / __private（不强制）
来源：http://qi.jianghongdianzi.cn

PHP:  public / protected / private
来源：http://gt.yuntaijiaju.cn

JS:   #private 字段；其余公开
来源：http://yp.hahajie.cn

TS:   public / protected / private
来源：http://zd.shxzukj.cn

Java: public / protected / private / 默认包级
来源：http://bf.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yp.huixiangedu.cn

Ruby: public / protected / private
来源：http://ki.yuexingan06.cn

C#:   public / protected / private / internal
来源：http://hs.jctech888.com.cn

[G11] getter / setter
来源：http://yk.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://ww.shtwfgs.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wq.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://wh.521024.cn

TS:   get name(): string { return this._name; }
来源：http://mr.szsharing.cn

Java: public String getName() { return name; }
来源：http://kq.huixiangedu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yc.huixiangedu.cn

Ruby: attr_accessor :name
来源：http://bo.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://vb.jctech888.com.cn

[G12] 对象转字符串
来源：http://ai.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://lc.hnjuh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ro.colortex.cn

JS:   toString() { return this.name; }
来源：http://gu.bjjhwx.cn

TS:   toString(): string { return this.name; }
来源：http://nq.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://ys.521024.cn

Go:   func (u User) String() string { return u.Name }
来源：http://aj.muxihuayi.cn

Ruby: def to_s; @name; end
来源：http://hv.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://gx.chemitech.net.cn

[G13] 判断对象类型
来源：http://la.newstarts.cn

Py:   isinstance(u, User)
来源：http://no.lnxyls.cn

PHP:  $u instanceof User
来源：http://vb.colortex.cn

JS:   u instanceof User
来源：http://zz.szsharing.cn

TS:   u instanceof User
来源：http://ai.shxzskj.cn

Java: u instanceof User
来源：http://hy.huixiangedu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ma.huanxung.cn

Ruby: u.is_a?(User)
来源：http://vm.lnxyls.cn

C#:   u is User
来源：http://ln.huixinmuqiang.cn

[G14] 数据类 / record
来源：http://xp.bookmarksfly.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jh.9csxet.cn

PHP:  // 用 readonly 属性模拟
来源：http://vk.asd995.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mr.asd995.cn

TS:   type User = { name: string; age: number };
来源：http://sx.huixiangedu.cn

Java: record User(String name, int age) {}
来源：http://qm.colortex.cn

Go:   type User struct { Name string; Age int }
来源：http://ik.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jd.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://ja.521024.cn

[G15] 枚举
来源：http://fj.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ie.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nw.shxzukj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cy.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ny.haigaiapp.cn

Java: enum Color { RED, GREEN }
来源：http://iq.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kj.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://ky.521024.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xv.shxzskj.cn

[G16] 对象转数组 / 字典
来源：http://us.newstarts.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tf.shtwfgs.cn

PHP:  get_object_vars($obj);
来源：http://bj.gzmigu.cn

JS:   Object.entries(obj)
来源：http://ld.panjiajie.cn

TS:   Object.entries(obj)
来源：http://yt.hahajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vp.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://sv.yuntaijiaju.cn

Ruby: obj.instance_variables
来源：http://zv.nicolike.cn

C#:   // 用反射或 System.Text.Json
来源：http://uc.yuexingan06.cn

================================================================================
来源：http://gk.wgjwhj.cn

H. 异常与错误处理
来源：http://uj.521024.cn

================================================================================
来源：http://ju.newstarts.cn

[H01] try / catch 基础
来源：http://sl.shxzskj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uv.hnjuh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nl.huixiangedu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://aa.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wx.huanxung.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ox.shxzukj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lg.wgjwhj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nv.huixinmuqiang.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vo.huixiangedu.cn

[H02] finally / ensure 收尾
来源：http://ov.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hf.muxihuayi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xh.hahajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lm.nszjky.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qq.szxytkj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tl.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vh.gzmigu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://eo.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vc.szxytkj.cn

[H03] 主动抛出异常
来源：http://jk.wgjwhj.cn

Py:   raise ValueError("错误信息")
来源：http://ln.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bg.gzmigu.cn

JS:   throw new Error("错误信息");
来源：http://rv.szsharing.cn

TS:   throw new Error("错误信息");
来源：http://dj.panjiajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jz.colortex.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vd.muxihuayi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ms.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://al.9csxet.cn

[H04] 自定义异常类型
来源：http://ud.colortex.cn

Py:   class MyError(Exception): pass
来源：http://hu.chemitech.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bx.gzmigu.cn

JS:   class MyError extends Error {}
来源：http://fy.bookmarksfly.cn

TS:   class MyError extends Error {}
来源：http://oa.asd995.cn

Java: class MyException extends RuntimeException {}
来源：http://qu.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://to.huixiangedu.cn

Ruby: class MyError < StandardError; end
来源：http://xz.hnjuh.cn

C#:   class MyException : Exception {}
来源：http://pl.shxzskj.cn

[H05] 捕获特定类型
来源：http://eq.bjjhwx.cn

Py:   except ValueError as e:
来源：http://od.colortex.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ki.jctech888.com.cn

JS:   if (e instanceof TypeError) {}
来源：http://rv.huanxung.cn

TS:   if (e instanceof TypeError) {}
来源：http://fh.jctech888.com.cn

Java: catch (IOException | SQLException e) {}
来源：http://og.jianghongdianzi.cn


<!-- 参考信息 -->