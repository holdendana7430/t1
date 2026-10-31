代发 wailian999

[F01] 读取整个文件
来源：http://mt.szxytkj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://qu.bjjhwx.cn

PHP:  file_get_contents("a.txt");
来源：http://zl.hnjuh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ax.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ba.jianghongdianzi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pm.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dj.bookmarksfly.cn

Ruby: File.read("a.txt")
来源：http://xy.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://ea.wgjwhj.cn

[F02] 逐行读取文件
来源：http://zj.shxzukj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ja.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://to.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qt.jctech888.com.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dk.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vn.521024.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://br.panjiajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://kw.haigaiapp.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://fb.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://nw.9csxet.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dd.shtwfgs.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mw.huixinmuqiang.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://to.haigaiapp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qy.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zv.asd995.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oa.hahajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://jf.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pu.huixinmuqiang.cn

[F04] 追加写入文件
来源：http://fp.huixinmuqiang.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pn.huixiangedu.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://dq.nicolike.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://if.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fx.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://id.jianghongdianzi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mn.yuntaijiaju.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ga.asd995.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yx.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://vk.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://el.szxytkj.cn

PHP:  file_exists("a.txt");
来源：http://tj.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://qk.bjjhwx.cn

TS:   fs.existsSync("a.txt")
来源：http://fg.yuexingan06.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xg.colortex.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tc.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://zs.szxytkj.cn

C#:   File.Exists("a.txt")
来源：http://xl.bjjhwx.cn

[F06] 删除文件
来源：http://vf.szxytkj.cn

Py:   os.remove("a.txt")
来源：http://yu.hnjuh.cn

PHP:  unlink("a.txt");
来源：http://ka.shxzskj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://sm.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gi.521024.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://oi.521024.cn

Go:   os.Remove("a.txt")
来源：http://vq.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://pn.nszjky.cn

C#:   File.Delete("a.txt");
来源：http://gr.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://oj.hahajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gw.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cg.shxzukj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xr.shxzukj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ca.szsharing.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dn.gzmigu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jy.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://as.shxzskj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://om.szxytkj.cn

[F08] 遍历目录
来源：http://ck.szxytkj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://cp.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gh.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://xw.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://lm.wgjwhj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fd.yuntaijiaju.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ru.huanxung.cn

Ruby: Dir.children("dir")
来源：http://xv.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://wa.shxzskj.cn

[F09] 获取文件大小
来源：http://nx.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://vl.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://fm.huixiangedu.cn

JS:   fs.statSync("a.txt").size
来源：http://us.asd995.cn

TS:   fs.statSync("a.txt").size
来源：http://jg.lnxyls.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pu.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fs.yuexingan06.cn

Ruby: File.size("a.txt")
来源：http://am.nicolike.cn

C#:   new FileInfo("a.txt").Length
来源：http://nq.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://sx.gzmigu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ai.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zj.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ba.panjiajie.cn

TS:   path.extname("a.txt")
来源：http://qb.shxzukj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://aq.chemitech.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://aw.9csxet.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cv.shtwfgs.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pi.chemitech.net.cn

[F11] 复制与移动文件
来源：http://yl.newstarts.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yt.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://je.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://km.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cf.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ex.521024.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zf.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rm.yuntaijiaju.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://em.muxihuayi.cn

[F12] CSV 读写
来源：http://vd.szsharing.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tu.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://og.huixiangedu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hw.chemitech.net.cn

TS:   // 同上
来源：http://ul.jianghongdianzi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://av.jianghongdianzi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ow.huixiangedu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qa.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rx.nszjky.cn

================================================================================
来源：http://jy.colortex.cn

G. 面向对象
来源：http://br.asd995.cn

================================================================================
来源：http://fs.9csxet.cn

[G01] 定义类
来源：http://hc.newstarts.cn

Py:   class User: pass
来源：http://te.szxytkj.cn

PHP:  class User {}
来源：http://dq.szxytkj.cn

JS:   class User {}
来源：http://tw.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://cq.newstarts.cn

Java: class User {}
来源：http://rv.haigaiapp.cn

Go:   type User struct { Name string }
来源：http://xn.yuntaijiaju.cn

Ruby: class User; end
来源：http://ey.gzmigu.cn

C#:   class User {}
来源：http://qq.newstarts.cn

[G02] 构造函数
来源：http://ry.gzmigu.cn

Py:   def __init__(self, name): self.name = name
来源：http://xr.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://kt.hnjuh.cn

JS:   constructor(name) { this.name = name; }
来源：http://hy.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://on.hnjuh.cn

Java: User(String name) { this.name = name; }
来源：http://xn.muxihuayi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://az.jianghongdianzi.cn

Ruby: def initialize(name); @name = name; end
来源：http://mf.bjjhwx.cn

C#:   public User(string name) { Name = name; }
来源：http://gq.szxytkj.cn

[G03] 实例属性
来源：http://xn.521024.cn

Py:   self.name = "x"
来源：http://ze.szxytkj.cn

PHP:  public string $name = "x";
来源：http://ej.szxytkj.cn

JS:   this.name = "x";
来源：http://is.shxzukj.cn

TS:   name: string = "x";
来源：http://fg.panjiajie.cn

Java: private String name;
来源：http://cz.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jt.9csxet.cn

Ruby: @name = "x"
来源：http://yi.9csxet.cn

C#:   public string Name { get; set; } = "x";
来源：http://nx.yuntaijiaju.cn

[G04] 定义方法
来源：http://ub.shxzskj.cn

Py:   def greet(self): return self.name
来源：http://lx.jctech888.com.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wg.newstarts.cn

JS:   greet() { return this.name; }
来源：http://bq.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://zu.shtwfgs.cn

Java: String greet() { return name; }
来源：http://ph.yuexingan06.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://oc.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://wm.colortex.cn

C#:   public string Greet() => Name;
来源：http://db.newstarts.cn

[G05] 继承
来源：http://kv.hahajie.cn

Py:   class Admin(User): pass
来源：http://sy.muxihuayi.cn

PHP:  class Admin extends User {}
来源：http://ls.shxzukj.cn

JS:   class Admin extends User {}
来源：http://sj.huanxung.cn

TS:   class Admin extends User {}
来源：http://yi.muxihuayi.cn

Java: class Admin extends User {}
来源：http://qr.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pb.lnxyls.cn

Ruby: class Admin < User; end
来源：http://oy.huixiangedu.cn

C#:   class Admin : User {}
来源：http://od.nicolike.cn

[G06] 重写方法
来源：http://lo.colortex.cn

Py:   def greet(self): return "admin"
来源：http://hl.jctech888.com.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fw.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://ay.huanxung.cn

TS:   greet(): string { return "admin"; }
来源：http://tn.yuntaijiaju.cn

Java: @Override String greet() { return "admin"; }
来源：http://ob.9csxet.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://al.jianghongdianzi.cn

Ruby: def greet; "admin"; end
来源：http://ol.panjiajie.cn

C#:   public override string Greet() => "admin";
来源：http://yh.yuexingan06.cn

[G07] 调用父类方法
来源：http://cs.hahajie.cn

Py:   super().greet()
来源：http://tv.shxzskj.cn

PHP:  parent::greet();
来源：http://zk.shxzskj.cn

JS:   super.greet();
来源：http://kd.bookmarksfly.cn

TS:   super.greet();
来源：http://ic.huixiangedu.cn

Java: super.greet();
来源：http://vo.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tp.huanxung.cn

Ruby: super
来源：http://vl.9csxet.cn

C#:   base.Greet();
来源：http://cd.nicolike.cn

[G08] 静态方法与属性
来源：http://ch.9csxet.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hl.chemitech.net.cn

PHP:  public static function f() {}
来源：http://rp.hahajie.cn

JS:   static f() {}
来源：http://kw.panjiajie.cn

TS:   static f(): void {}
来源：http://eq.nicolike.cn

Java: static void f() {}
来源：http://uk.asd995.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://aa.haigaiapp.cn

Ruby: def self.f; end
来源：http://qa.shxzskj.cn

C#:   public static void F() {}
来源：http://by.jctech888.com.cn

[G09] 接口 / 抽象类
来源：http://tq.shxzskj.cn

Py:   from abc import ABC, abstractmethod
来源：http://hb.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ks.asd995.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mc.yuntaijiaju.cn

TS:   interface Shape { area(): number; }
来源：http://pl.bookmarksfly.cn

Java: interface Shape { double area(); }
来源：http://os.nicolike.cn

Go:   type Shape interface { Area() float64 }
来源：http://my.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://iv.huixiangedu.cn

C#:   interface IShape { double Area(); }
来源：http://oi.newstarts.cn

[G10] 访问控制
来源：http://bu.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://ks.huanxung.cn

PHP:  public / protected / private
来源：http://cb.huixiangedu.cn

JS:   #private 字段；其余公开
来源：http://ne.wgjwhj.cn

TS:   public / protected / private
来源：http://tg.521024.cn

Java: public / protected / private / 默认包级
来源：http://dk.colortex.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rf.asd995.cn

Ruby: public / protected / private
来源：http://fh.chemitech.net.cn

C#:   public / protected / private / internal
来源：http://ac.gzmigu.cn

[G11] getter / setter
来源：http://og.bookmarksfly.cn

Py:   @property 与 @x.setter
来源：http://fa.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tj.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://gq.jctech888.com.cn

TS:   get name(): string { return this._name; }
来源：http://ay.bookmarksfly.cn

Java: public String getName() { return name; }
来源：http://sz.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vi.szsharing.cn

Ruby: attr_accessor :name
来源：http://cq.nicolike.cn

C#:   public string Name { get; set; }
来源：http://vq.jianghongdianzi.cn

[G12] 对象转字符串
来源：http://zp.shtwfgs.cn

Py:   def __str__(self): return self.name
来源：http://nd.szxytkj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gl.haigaiapp.cn

JS:   toString() { return this.name; }
来源：http://yo.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://hl.gzmigu.cn

Java: @Override public String toString() { return name; }
来源：http://yk.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vf.panjiajie.cn

Ruby: def to_s; @name; end
来源：http://ew.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://lo.gzmigu.cn

[G13] 判断对象类型
来源：http://yl.huixiangedu.cn

Py:   isinstance(u, User)
来源：http://vx.yuexingan06.cn

PHP:  $u instanceof User
来源：http://ww.szxytkj.cn

JS:   u instanceof User
来源：http://as.jianghongdianzi.cn

TS:   u instanceof User
来源：http://wj.panjiajie.cn

Java: u instanceof User
来源：http://ma.shxzskj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ip.bjjhwx.cn

Ruby: u.is_a?(User)
来源：http://hm.gzmigu.cn

C#:   u is User
来源：http://lg.szxytkj.cn

[G14] 数据类 / record
来源：http://uc.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bp.huixinmuqiang.cn

PHP:  // 用 readonly 属性模拟
来源：http://uu.szxytkj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wh.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://ef.bookmarksfly.cn

Java: record User(String name, int age) {}
来源：http://uo.shxzskj.cn

Go:   type User struct { Name string; Age int }
来源：http://hu.nszjky.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cv.muxihuayi.cn

C#:   record User(string Name, int Age);
来源：http://sy.szsharing.cn

[G15] 枚举
来源：http://xc.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ug.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fh.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iy.hnjuh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xc.lnxyls.cn

Java: enum Color { RED, GREEN }
来源：http://rb.muxihuayi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://io.asd995.cn

Ruby: Color = %i[red green].freeze
来源：http://ys.hnjuh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zw.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://ab.asd995.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gi.nszjky.cn

PHP:  get_object_vars($obj);
来源：http://vt.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://jn.jctech888.com.cn

TS:   Object.entries(obj)
来源：http://om.shxzskj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zu.bjjhwx.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://sp.szsharing.cn

Ruby: obj.instance_variables
来源：http://xm.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://pm.muxihuayi.cn

================================================================================
来源：http://fo.shxzskj.cn

H. 异常与错误处理
来源：http://pg.huanxung.cn

================================================================================
来源：http://ri.shtwfgs.cn

[H01] try / catch 基础
来源：http://hu.shtwfgs.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ws.jianghongdianzi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yt.asd995.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nd.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oa.wgjwhj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zn.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qe.szxytkj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wc.shtwfgs.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xg.hnjuh.cn

[H02] finally / ensure 收尾
来源：http://lc.9csxet.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zz.lnxyls.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ll.haigaiapp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wb.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qu.nszjky.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vw.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://of.jianghongdianzi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vd.shtwfgs.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hm.gzmigu.cn

[H03] 主动抛出异常
来源：http://mt.huixiangedu.cn

Py:   raise ValueError("错误信息")
来源：http://lt.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tb.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://su.bookmarksfly.cn

TS:   throw new Error("错误信息");
来源：http://jo.yuntaijiaju.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://uq.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oy.haigaiapp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qu.huanxung.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ml.9csxet.cn

[H04] 自定义异常类型
来源：http://le.hnjuh.cn

Py:   class MyError(Exception): pass
来源：http://bg.chemitech.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pc.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://tt.nicolike.cn

TS:   class MyError extends Error {}
来源：http://qe.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://ue.shtwfgs.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sn.hahajie.cn

Ruby: class MyError < StandardError; end
来源：http://ag.hahajie.cn

C#:   class MyException : Exception {}
来源：http://ks.gzmigu.cn

[H05] 捕获特定类型
来源：http://od.szsharing.cn

Py:   except ValueError as e:
来源：http://jy.jianghongdianzi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xy.huixinmuqiang.cn

JS:   if (e instanceof TypeError) {}
来源：http://zi.bjjhwx.cn

TS:   if (e instanceof TypeError) {}
来源：http://vw.huixiangedu.cn

Java: catch (IOException | SQLException e) {}
来源：http://ar.bjjhwx.cn


<!-- 参考信息 -->