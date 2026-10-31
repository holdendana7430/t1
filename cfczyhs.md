代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://kk.colortex.cn

[F02] 逐行读取文件
来源：http://rm.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fd.huixinmuqiang.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ws.shxzukj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://du.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wh.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kx.jianghongdianzi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://bt.521024.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://an.szxytkj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qi.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://tu.muxihuayi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ob.jctech888.com.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pr.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hl.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bj.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tu.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gh.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://ov.9csxet.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wf.shxzukj.cn

[F04] 追加写入文件
来源：http://ex.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nd.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tt.9csxet.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wh.yuntaijiaju.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://km.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vs.szxytkj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hl.panjiajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://to.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uf.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://yz.szsharing.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fy.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://za.muxihuayi.cn

JS:   fs.existsSync("a.txt")
来源：http://au.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://hv.chemitech.net.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qf.shxzukj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ev.colortex.cn

Ruby: File.exist?("a.txt")
来源：http://ll.gzmigu.cn

C#:   File.Exists("a.txt")
来源：http://nl.lnxyls.cn

[F06] 删除文件
来源：http://fz.asd995.cn

Py:   os.remove("a.txt")
来源：http://kg.yuexingan06.cn

PHP:  unlink("a.txt");
来源：http://ra.9csxet.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wp.yuntaijiaju.cn

TS:   fs.unlinkSync("a.txt")
来源：http://fs.muxihuayi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lq.newstarts.cn

Go:   os.Remove("a.txt")
来源：http://rs.hahajie.cn

Ruby: File.delete("a.txt")
来源：http://lt.yuntaijiaju.cn

C#:   File.Delete("a.txt");
来源：http://in.shxzskj.cn

[F07] 创建目录（含多级）
来源：http://gs.jctech888.com.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wk.shxzukj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pu.newstarts.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uw.panjiajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cd.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zg.jianghongdianzi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gn.szsharing.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gt.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rl.jianghongdianzi.cn

[F08] 遍历目录
来源：http://pi.szxytkj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tt.chemitech.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bp.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://wi.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://ce.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wo.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nc.hahajie.cn

Ruby: Dir.children("dir")
来源：http://ww.shxzukj.cn

C#:   Directory.GetFiles("dir")
来源：http://yd.nicolike.cn

[F09] 获取文件大小
来源：http://ny.yuntaijiaju.cn

Py:   os.path.getsize("a.txt")
来源：http://tx.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://fi.huixinmuqiang.cn

JS:   fs.statSync("a.txt").size
来源：http://qj.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://ia.9csxet.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qr.yuntaijiaju.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bd.9csxet.cn

Ruby: File.size("a.txt")
来源：http://pp.yuexingan06.cn

C#:   new FileInfo("a.txt").Length
来源：http://ef.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://ax.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wc.bookmarksfly.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://sm.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://xt.jianghongdianzi.cn

TS:   path.extname("a.txt")
来源：http://pf.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ha.szxytkj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kv.huixiangedu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hk.shtwfgs.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bg.huanxung.cn

[F11] 复制与移动文件
来源：http://je.muxihuayi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xj.wgjwhj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mw.huixiangedu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yq.chemitech.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ah.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yv.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://im.szsharing.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fw.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mc.haigaiapp.cn

[F12] CSV 读写
来源：http://sw.huixinmuqiang.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gs.haigaiapp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wk.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fg.huanxung.cn

TS:   // 同上
来源：http://on.szsharing.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ot.jianghongdianzi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uw.jctech888.com.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uw.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wy.jianghongdianzi.cn

================================================================================
来源：http://tk.shxzskj.cn

G. 面向对象
来源：http://am.panjiajie.cn

================================================================================
来源：http://qj.jianghongdianzi.cn

[G01] 定义类
来源：http://vc.shxzukj.cn

Py:   class User: pass
来源：http://hs.szxytkj.cn

PHP:  class User {}
来源：http://vw.huanxung.cn

JS:   class User {}
来源：http://nw.panjiajie.cn

TS:   class User { name: string = ""; }
来源：http://df.9csxet.cn

Java: class User {}
来源：http://ac.nszjky.cn

Go:   type User struct { Name string }
来源：http://fl.muxihuayi.cn

Ruby: class User; end
来源：http://ok.shtwfgs.cn

C#:   class User {}
来源：http://xh.hahajie.cn

[G02] 构造函数
来源：http://hk.jctech888.com.cn

Py:   def __init__(self, name): self.name = name
来源：http://zf.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://ii.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://ah.nicolike.cn

TS:   constructor(public name: string) {}
来源：http://bw.huanxung.cn

Java: User(String name) { this.name = name; }
来源：http://du.szsharing.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pn.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://fb.haigaiapp.cn

C#:   public User(string name) { Name = name; }
来源：http://ux.jctech888.com.cn

[G03] 实例属性
来源：http://sh.yuexingan06.cn

Py:   self.name = "x"
来源：http://sg.nszjky.cn

PHP:  public string $name = "x";
来源：http://id.newstarts.cn

JS:   this.name = "x";
来源：http://nr.asd995.cn

TS:   name: string = "x";
来源：http://ko.szxytkj.cn

Java: private String name;
来源：http://lm.chemitech.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jo.bjjhwx.cn

Ruby: @name = "x"
来源：http://oz.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://fc.bookmarksfly.cn

[G04] 定义方法
来源：http://nt.hnjuh.cn

Py:   def greet(self): return self.name
来源：http://nb.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cl.jctech888.com.cn

JS:   greet() { return this.name; }
来源：http://ho.shxzukj.cn

TS:   greet(): string { return this.name; }
来源：http://lt.jianghongdianzi.cn

Java: String greet() { return name; }
来源：http://sq.huanxung.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ei.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://xz.szsharing.cn

C#:   public string Greet() => Name;
来源：http://zw.yuntaijiaju.cn

[G05] 继承
来源：http://py.newstarts.cn

Py:   class Admin(User): pass
来源：http://yt.nszjky.cn

PHP:  class Admin extends User {}
来源：http://oz.9csxet.cn

JS:   class Admin extends User {}
来源：http://fw.hahajie.cn

TS:   class Admin extends User {}
来源：http://br.hnjuh.cn

Java: class Admin extends User {}
来源：http://vx.yuntaijiaju.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ny.haigaiapp.cn

Ruby: class Admin < User; end
来源：http://ge.9csxet.cn

C#:   class Admin : User {}
来源：http://jq.newstarts.cn

[G06] 重写方法
来源：http://gq.szsharing.cn

Py:   def greet(self): return "admin"
来源：http://qe.gzmigu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zs.huanxung.cn

JS:   greet() { return "admin"; }
来源：http://yl.huanxung.cn

TS:   greet(): string { return "admin"; }
来源：http://jt.shxzukj.cn

Java: @Override String greet() { return "admin"; }
来源：http://xd.9csxet.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uh.shtwfgs.cn

Ruby: def greet; "admin"; end
来源：http://wa.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://xw.muxihuayi.cn

[G07] 调用父类方法
来源：http://vz.haigaiapp.cn

Py:   super().greet()
来源：http://fy.colortex.cn

PHP:  parent::greet();
来源：http://me.szxytkj.cn

JS:   super.greet();
来源：http://sq.gzmigu.cn

TS:   super.greet();
来源：http://ox.huixiangedu.cn

Java: super.greet();
来源：http://zc.bjjhwx.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bg.szsharing.cn

Ruby: super
来源：http://ti.yuexingan06.cn

C#:   base.Greet();
来源：http://dz.bjjhwx.cn

[G08] 静态方法与属性
来源：http://hu.szxytkj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hg.panjiajie.cn

PHP:  public static function f() {}
来源：http://uc.huanxung.cn

JS:   static f() {}
来源：http://yz.yuntaijiaju.cn

TS:   static f(): void {}
来源：http://uz.szsharing.cn

Java: static void f() {}
来源：http://om.wgjwhj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://io.wgjwhj.cn

Ruby: def self.f; end
来源：http://cc.panjiajie.cn

C#:   public static void F() {}
来源：http://qr.nicolike.cn

[G09] 接口 / 抽象类
来源：http://dk.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://jw.shxzukj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mx.jctech888.com.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hb.gzmigu.cn

TS:   interface Shape { area(): number; }
来源：http://dj.nszjky.cn

Java: interface Shape { double area(); }
来源：http://rm.shxzukj.cn

Go:   type Shape interface { Area() float64 }
来源：http://gm.nicolike.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ep.haigaiapp.cn

C#:   interface IShape { double Area(); }
来源：http://lb.panjiajie.cn

[G10] 访问控制
来源：http://vl.newstarts.cn

Py:   约定 _protected / __private（不强制）
来源：http://zb.gzmigu.cn

PHP:  public / protected / private
来源：http://vg.hnjuh.cn

JS:   #private 字段；其余公开
来源：http://yz.huixiangedu.cn

TS:   public / protected / private
来源：http://yx.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://uk.chemitech.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kf.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://lg.colortex.cn

C#:   public / protected / private / internal
来源：http://ss.shxzukj.cn

[G11] getter / setter
来源：http://tl.hahajie.cn

Py:   @property 与 @x.setter
来源：http://jy.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fx.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://bg.nicolike.cn

TS:   get name(): string { return this._name; }
来源：http://tp.huixinmuqiang.cn

Java: public String getName() { return name; }
来源：http://ce.hnjuh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zd.521024.cn

Ruby: attr_accessor :name
来源：http://wh.chemitech.net.cn

C#:   public string Name { get; set; }
来源：http://ma.bjjhwx.cn

[G12] 对象转字符串
来源：http://xs.nszjky.cn

Py:   def __str__(self): return self.name
来源：http://cb.hnjuh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yx.huanxung.cn

JS:   toString() { return this.name; }
来源：http://aw.lnxyls.cn

TS:   toString(): string { return this.name; }
来源：http://kb.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://wg.asd995.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bv.521024.cn

Ruby: def to_s; @name; end
来源：http://vi.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://jj.521024.cn

[G13] 判断对象类型
来源：http://po.yuntaijiaju.cn

Py:   isinstance(u, User)
来源：http://zz.nszjky.cn

PHP:  $u instanceof User
来源：http://bp.huanxung.cn

JS:   u instanceof User
来源：http://cd.yuntaijiaju.cn

TS:   u instanceof User
来源：http://vz.hahajie.cn

Java: u instanceof User
来源：http://ox.shtwfgs.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lj.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://ml.shxzukj.cn

C#:   u is User
来源：http://kg.colortex.cn

[G14] 数据类 / record
来源：http://xh.wgjwhj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bk.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://ay.asd995.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tl.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://gw.haigaiapp.cn

Java: record User(String name, int age) {}
来源：http://sq.521024.cn

Go:   type User struct { Name string; Age int }
来源：http://ql.521024.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gy.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://lj.nszjky.cn

[G15] 枚举
来源：http://fw.newstarts.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ka.521024.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hx.huanxung.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bu.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ro.bjjhwx.cn

Java: enum Color { RED, GREEN }
来源：http://kv.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ku.hnjuh.cn

Ruby: Color = %i[red green].freeze
来源：http://xr.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ja.colortex.cn

[G16] 对象转数组 / 字典
来源：http://yy.panjiajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ck.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://au.haigaiapp.cn

JS:   Object.entries(obj)
来源：http://xr.haigaiapp.cn

TS:   Object.entries(obj)
来源：http://ca.yuexingan06.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ok.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gw.huixiangedu.cn

Ruby: obj.instance_variables
来源：http://yk.9csxet.cn

C#:   // 用反射或 System.Text.Json
来源：http://ar.huixiangedu.cn

================================================================================
来源：http://nj.bjjhwx.cn

H. 异常与错误处理
来源：http://tl.shtwfgs.cn

================================================================================
来源：http://pd.lnxyls.cn

[H01] try / catch 基础
来源：http://pd.hnjuh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pj.yuntaijiaju.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://iy.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pb.haigaiapp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://er.szsharing.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mo.shxzskj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ij.colortex.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ta.huixiangedu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cw.muxihuayi.cn

[H02] finally / ensure 收尾
来源：http://ao.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://di.gzmigu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hm.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jr.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fk.huanxung.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ep.chemitech.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wf.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ds.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vj.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://pb.huanxung.cn

Py:   raise ValueError("错误信息")
来源：http://rz.wgjwhj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bj.szxytkj.cn

JS:   throw new Error("错误信息");
来源：http://oo.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://to.shxzukj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fp.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bf.bookmarksfly.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tu.asd995.cn

C#:   throw new ArgumentException("错误信息");
来源：http://oq.shtwfgs.cn

[H04] 自定义异常类型
来源：http://yh.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://pb.lnxyls.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xy.gzmigu.cn

JS:   class MyError extends Error {}
来源：http://ep.szsharing.cn

TS:   class MyError extends Error {}
来源：http://ct.hahajie.cn

Java: class MyException extends RuntimeException {}
来源：http://nh.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ze.shtwfgs.cn

Ruby: class MyError < StandardError; end
来源：http://yb.chemitech.net.cn

C#:   class MyException : Exception {}
来源：http://dd.wgjwhj.cn

[H05] 捕获特定类型
来源：http://ho.huixinmuqiang.cn

Py:   except ValueError as e:
来源：http://qj.asd995.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ih.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://lh.huixinmuqiang.cn

TS:   if (e instanceof TypeError) {}
来源：http://hy.521024.cn

Java: catch (IOException | SQLException e) {}
来源：http://dj.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gd.bookmarksfly.cn

Ruby: rescue ArgumentError => e
来源：http://yw.521024.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fn.bookmarksfly.cn

[H06] 可选值 / 空值安全访问
来源：http://ie.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://qo.521024.cn

PHP:  $v = $d["k"] ?? null;
来源：http://km.lnxyls.cn

JS:   obj?.a?.b;  d ?? default
来源：http://iz.9csxet.cn

TS:   obj?.a?.b;  d ?? default
来源：http://br.9csxet.cn


<!-- 参考信息 -->