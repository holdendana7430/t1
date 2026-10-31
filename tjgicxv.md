代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://oz.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tc.jianghongdianzi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://oo.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vt.jianghongdianzi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yp.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://fo.wgjwhj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gf.colortex.cn

[F04] 追加写入文件
来源：http://rg.colortex.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zb.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mq.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ed.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://he.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://rn.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cz.szxytkj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qa.muxihuayi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lv.nicolike.cn

[F05] 判断文件或目录是否存在
来源：http://pp.bookmarksfly.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rc.panjiajie.cn

PHP:  file_exists("a.txt");
来源：http://wh.521024.cn

JS:   fs.existsSync("a.txt")
来源：http://ux.chemitech.net.cn

TS:   fs.existsSync("a.txt")
来源：http://uf.asd995.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jv.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ss.bjjhwx.cn

Ruby: File.exist?("a.txt")
来源：http://cy.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://cx.gzmigu.cn

[F06] 删除文件
来源：http://ge.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://hr.asd995.cn

PHP:  unlink("a.txt");
来源：http://na.521024.cn

JS:   fs.unlinkSync("a.txt")
来源：http://su.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ci.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://gn.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://sy.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://hs.shtwfgs.cn

C#:   File.Delete("a.txt");
来源：http://nb.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://kh.colortex.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rl.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wi.panjiajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kj.9csxet.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xc.gzmigu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zr.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bw.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rn.shtwfgs.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qe.szxytkj.cn

[F08] 遍历目录
来源：http://lx.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jp.shxzskj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lz.newstarts.cn

JS:   fs.readdirSync("dir")
来源：http://rh.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://pm.huixinmuqiang.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mp.bookmarksfly.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qk.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://yw.shtwfgs.cn

C#:   Directory.GetFiles("dir")
来源：http://di.gzmigu.cn

[F09] 获取文件大小
来源：http://kq.muxihuayi.cn

Py:   os.path.getsize("a.txt")
来源：http://tw.lnxyls.cn

PHP:  filesize("a.txt");
来源：http://te.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://st.yuexingan06.cn

TS:   fs.statSync("a.txt").size
来源：http://yw.szsharing.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ju.shtwfgs.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rl.haigaiapp.cn

Ruby: File.size("a.txt")
来源：http://wg.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://ld.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://kz.wgjwhj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://yp.colortex.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yc.521024.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ia.asd995.cn

TS:   path.extname("a.txt")
来源：http://dz.gzmigu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wd.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vo.521024.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ot.muxihuayi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zf.yuntaijiaju.cn

[F11] 复制与移动文件
来源：http://kq.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gn.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ut.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zr.szsharing.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ue.yuntaijiaju.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://re.lnxyls.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kt.asd995.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://qy.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fk.haigaiapp.cn

[F12] CSV 读写
来源：http://fk.shxzskj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ga.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ck.bookmarksfly.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gl.9csxet.cn

TS:   // 同上
来源：http://hh.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pj.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kn.bookmarksfly.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tn.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tf.hahajie.cn

================================================================================
来源：http://lb.huanxung.cn

G. 面向对象
来源：http://ix.huanxung.cn

================================================================================
来源：http://sp.szsharing.cn

[G01] 定义类
来源：http://gf.shtwfgs.cn

Py:   class User: pass
来源：http://kw.yuntaijiaju.cn

PHP:  class User {}
来源：http://fu.szsharing.cn

JS:   class User {}
来源：http://lo.panjiajie.cn

TS:   class User { name: string = ""; }
来源：http://zq.szsharing.cn

Java: class User {}
来源：http://vv.wgjwhj.cn

Go:   type User struct { Name string }
来源：http://az.asd995.cn

Ruby: class User; end
来源：http://ef.9csxet.cn

C#:   class User {}
来源：http://wa.lnxyls.cn

[G02] 构造函数
来源：http://hn.szxytkj.cn

Py:   def __init__(self, name): self.name = name
来源：http://hk.9csxet.cn

PHP:  public function __construct(public string $name) {}
来源：http://qc.jianghongdianzi.cn

JS:   constructor(name) { this.name = name; }
来源：http://eq.yuexingan06.cn

TS:   constructor(public name: string) {}
来源：http://gl.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://fi.muxihuayi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sj.shxzskj.cn

Ruby: def initialize(name); @name = name; end
来源：http://wb.521024.cn

C#:   public User(string name) { Name = name; }
来源：http://zo.shxzskj.cn

[G03] 实例属性
来源：http://bu.hahajie.cn

Py:   self.name = "x"
来源：http://bv.szsharing.cn

PHP:  public string $name = "x";
来源：http://qx.bookmarksfly.cn

JS:   this.name = "x";
来源：http://wm.yuexingan06.cn

TS:   name: string = "x";
来源：http://gj.huanxung.cn

Java: private String name;
来源：http://yf.panjiajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ro.wgjwhj.cn

Ruby: @name = "x"
来源：http://ae.shxzukj.cn

C#:   public string Name { get; set; } = "x";
来源：http://fx.asd995.cn

[G04] 定义方法
来源：http://bm.newstarts.cn

Py:   def greet(self): return self.name
来源：http://br.shxzukj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zy.521024.cn

JS:   greet() { return this.name; }
来源：http://yk.newstarts.cn

TS:   greet(): string { return this.name; }
来源：http://hf.huixiangedu.cn

Java: String greet() { return name; }
来源：http://py.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tq.hnjuh.cn

Ruby: def greet; @name; end
来源：http://od.hahajie.cn

C#:   public string Greet() => Name;
来源：http://vr.muxihuayi.cn

[G05] 继承
来源：http://ya.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://go.panjiajie.cn

PHP:  class Admin extends User {}
来源：http://up.colortex.cn

JS:   class Admin extends User {}
来源：http://br.asd995.cn

TS:   class Admin extends User {}
来源：http://da.lnxyls.cn

Java: class Admin extends User {}
来源：http://bf.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pl.yuexingan06.cn

Ruby: class Admin < User; end
来源：http://ov.521024.cn

C#:   class Admin : User {}
来源：http://iq.hahajie.cn

[G06] 重写方法
来源：http://hp.newstarts.cn

Py:   def greet(self): return "admin"
来源：http://dq.huanxung.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://si.haigaiapp.cn

JS:   greet() { return "admin"; }
来源：http://iu.bjjhwx.cn

TS:   greet(): string { return "admin"; }
来源：http://xa.szxytkj.cn

Java: @Override String greet() { return "admin"; }
来源：http://oi.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kj.9csxet.cn

Ruby: def greet; "admin"; end
来源：http://wt.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://mu.huixinmuqiang.cn

[G07] 调用父类方法
来源：http://ld.nicolike.cn

Py:   super().greet()
来源：http://it.chemitech.net.cn

PHP:  parent::greet();
来源：http://yb.chemitech.net.cn

JS:   super.greet();
来源：http://bh.shxzskj.cn

TS:   super.greet();
来源：http://zn.panjiajie.cn

Java: super.greet();
来源：http://mh.shxzukj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zy.jianghongdianzi.cn

Ruby: super
来源：http://bv.9csxet.cn

C#:   base.Greet();
来源：http://xb.bjjhwx.cn

[G08] 静态方法与属性
来源：http://pr.colortex.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ep.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://yw.jctech888.com.cn

JS:   static f() {}
来源：http://aa.nicolike.cn

TS:   static f(): void {}
来源：http://np.szsharing.cn

Java: static void f() {}
来源：http://ju.shtwfgs.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mp.haigaiapp.cn

Ruby: def self.f; end
来源：http://nj.colortex.cn

C#:   public static void F() {}
来源：http://ku.jianghongdianzi.cn

[G09] 接口 / 抽象类
来源：http://yk.9csxet.cn

Py:   from abc import ABC, abstractmethod
来源：http://mo.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pd.huanxung.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pt.chemitech.net.cn

TS:   interface Shape { area(): number; }
来源：http://et.jctech888.com.cn

Java: interface Shape { double area(); }
来源：http://rb.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://xf.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yt.newstarts.cn

C#:   interface IShape { double Area(); }
来源：http://ig.lnxyls.cn

[G10] 访问控制
来源：http://cy.jianghongdianzi.cn

Py:   约定 _protected / __private（不强制）
来源：http://ui.yuntaijiaju.cn

PHP:  public / protected / private
来源：http://gt.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://qx.muxihuayi.cn

TS:   public / protected / private
来源：http://ld.nszjky.cn

Java: public / protected / private / 默认包级
来源：http://yz.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gy.bookmarksfly.cn

Ruby: public / protected / private
来源：http://su.shtwfgs.cn

C#:   public / protected / private / internal
来源：http://bp.jctech888.com.cn

[G11] getter / setter
来源：http://ig.newstarts.cn

Py:   @property 与 @x.setter
来源：http://pj.shxzskj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yh.panjiajie.cn

JS:   get name() { return this._name; }
来源：http://ua.szsharing.cn

TS:   get name(): string { return this._name; }
来源：http://rz.9csxet.cn

Java: public String getName() { return name; }
来源：http://om.hnjuh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wb.hahajie.cn

Ruby: attr_accessor :name
来源：http://yo.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://cq.521024.cn

[G12] 对象转字符串
来源：http://bx.huixinmuqiang.cn

Py:   def __str__(self): return self.name
来源：http://kn.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wf.nicolike.cn

JS:   toString() { return this.name; }
来源：http://jh.haigaiapp.cn

TS:   toString(): string { return this.name; }
来源：http://fv.huixinmuqiang.cn

Java: @Override public String toString() { return name; }
来源：http://mt.shtwfgs.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zy.wgjwhj.cn

Ruby: def to_s; @name; end
来源：http://xb.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://ii.521024.cn

[G13] 判断对象类型
来源：http://yj.szxytkj.cn

Py:   isinstance(u, User)
来源：http://zi.bjjhwx.cn

PHP:  $u instanceof User
来源：http://pu.panjiajie.cn

JS:   u instanceof User
来源：http://iy.huixinmuqiang.cn

TS:   u instanceof User
来源：http://ex.szxytkj.cn

Java: u instanceof User
来源：http://me.shxzukj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cl.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://ba.asd995.cn

C#:   u is User
来源：http://bv.bjjhwx.cn

[G14] 数据类 / record
来源：http://pu.shtwfgs.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ay.521024.cn

PHP:  // 用 readonly 属性模拟
来源：http://ze.hahajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sm.colortex.cn

TS:   type User = { name: string; age: number };
来源：http://yq.chemitech.net.cn

Java: record User(String name, int age) {}
来源：http://fk.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://ot.huanxung.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://lx.nszjky.cn

[G15] 枚举
来源：http://jw.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mq.shtwfgs.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xp.huanxung.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ze.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ow.asd995.cn

Java: enum Color { RED, GREEN }
来源：http://uh.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rz.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://bg.521024.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bx.shtwfgs.cn

[G16] 对象转数组 / 字典
来源：http://je.shtwfgs.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qi.muxihuayi.cn

PHP:  get_object_vars($obj);
来源：http://iq.hnjuh.cn

JS:   Object.entries(obj)
来源：http://hj.jctech888.com.cn

TS:   Object.entries(obj)
来源：http://nf.szsharing.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ys.yuexingan06.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://za.huixiangedu.cn

Ruby: obj.instance_variables
来源：http://gm.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://yc.chemitech.net.cn

================================================================================
来源：http://jm.shxzskj.cn

H. 异常与错误处理
来源：http://nd.nicolike.cn

================================================================================
来源：http://qy.nicolike.cn

[H01] try / catch 基础
来源：http://tg.shxzskj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ic.panjiajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mv.jianghongdianzi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zu.shtwfgs.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dn.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hu.bookmarksfly.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hy.9csxet.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bz.hnjuh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bj.chemitech.net.cn

[H02] finally / ensure 收尾
来源：http://qr.bjjhwx.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ip.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xg.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ww.haigaiapp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zx.nicolike.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lv.huixiangedu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://aj.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://su.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qw.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://nv.bjjhwx.cn

Py:   raise ValueError("错误信息")
来源：http://iy.shxzukj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bh.haigaiapp.cn

JS:   throw new Error("错误信息");
来源：http://qb.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://bj.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rl.szxytkj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://if.jctech888.com.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kr.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ie.haigaiapp.cn

[H04] 自定义异常类型
来源：http://eq.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://lj.newstarts.cn

PHP:  class MyError extends RuntimeException {}
来源：http://iw.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://nq.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://xi.9csxet.cn

Java: class MyException extends RuntimeException {}
来源：http://xe.huixiangedu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hu.hnjuh.cn

Ruby: class MyError < StandardError; end
来源：http://pr.colortex.cn

C#:   class MyException : Exception {}
来源：http://lr.521024.cn

[H05] 捕获特定类型
来源：http://tv.nicolike.cn

Py:   except ValueError as e:
来源：http://cu.gzmigu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jv.lnxyls.cn

JS:   if (e instanceof TypeError) {}
来源：http://aw.szxytkj.cn

TS:   if (e instanceof TypeError) {}
来源：http://mb.nicolike.cn

Java: catch (IOException | SQLException e) {}
来源：http://zt.nicolike.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://in.bookmarksfly.cn

Ruby: rescue ArgumentError => e
来源：http://jw.nicolike.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ng.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://uf.shxzukj.cn

Py:   value = d.get("k") or default
来源：http://yu.521024.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rh.jctech888.com.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ii.huanxung.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vu.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ch.lnxyls.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yh.9csxet.cn

Ruby: d&.dig(:a, :b)
来源：http://tk.gzmigu.cn

C#:   obj?.A?.B ?? default
来源：http://zi.9csxet.cn

[H07] 断言
来源：http://ot.huanxung.cn

Py:   assert x > 0, "必须为正"
来源：http://ff.yuntaijiaju.cn

PHP:  assert($x > 0);
来源：http://bn.szxytkj.cn

JS:   console.assert(x > 0);
来源：http://og.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://bv.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://yr.gzmigu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://il.chemitech.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nk.yuntaijiaju.cn


<!-- 参考信息 -->