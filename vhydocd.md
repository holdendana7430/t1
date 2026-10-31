代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ww.huixinmuqiang.cn

Ruby: File.write("a.txt", "hi")
来源：http://rh.szxytkj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ei.bookmarksfly.cn

[F04] 追加写入文件
来源：http://wf.yuntaijiaju.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://os.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ww.colortex.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uz.9csxet.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ad.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://yc.nicolike.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://le.shxzukj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://lh.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rb.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://ml.newstarts.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qc.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://ip.huanxung.cn

JS:   fs.existsSync("a.txt")
来源：http://tj.bjjhwx.cn

TS:   fs.existsSync("a.txt")
来源：http://fq.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hu.shtwfgs.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vn.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://nb.colortex.cn

C#:   File.Exists("a.txt")
来源：http://or.hnjuh.cn

[F06] 删除文件
来源：http://lx.jianghongdianzi.cn

Py:   os.remove("a.txt")
来源：http://kw.haigaiapp.cn

PHP:  unlink("a.txt");
来源：http://zy.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gf.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lk.521024.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fo.yuexingan06.cn

Go:   os.Remove("a.txt")
来源：http://da.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://zl.chemitech.net.cn

C#:   File.Delete("a.txt");
来源：http://dl.nszjky.cn

[F07] 创建目录（含多级）
来源：http://xk.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ay.9csxet.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vx.huanxung.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://du.colortex.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yj.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nj.asd995.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tv.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yt.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wc.huixinmuqiang.cn

[F08] 遍历目录
来源：http://tb.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://sl.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dg.bookmarksfly.cn

JS:   fs.readdirSync("dir")
来源：http://hz.jctech888.com.cn

TS:   fs.readdirSync("dir")
来源：http://yr.9csxet.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wy.yuntaijiaju.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ka.521024.cn

Ruby: Dir.children("dir")
来源：http://il.nicolike.cn

C#:   Directory.GetFiles("dir")
来源：http://fo.chemitech.net.cn

[F09] 获取文件大小
来源：http://lf.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://lw.haigaiapp.cn

PHP:  filesize("a.txt");
来源：http://vp.gzmigu.cn

JS:   fs.statSync("a.txt").size
来源：http://my.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://xl.panjiajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://xe.shxzukj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qo.521024.cn

Ruby: File.size("a.txt")
来源：http://qc.newstarts.cn

C#:   new FileInfo("a.txt").Length
来源：http://lh.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://be.bjjhwx.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wt.huixiangedu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dz.shtwfgs.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yg.shtwfgs.cn

TS:   path.extname("a.txt")
来源：http://vr.9csxet.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://zg.szxytkj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://bc.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ip.muxihuayi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://dd.szsharing.cn

[F11] 复制与移动文件
来源：http://nt.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wh.huanxung.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://un.asd995.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kx.huixiangedu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yw.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://eu.hahajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ea.shxzskj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://av.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wp.jianghongdianzi.cn

[F12] CSV 读写
来源：http://mu.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dv.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ot.gzmigu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rh.bjjhwx.cn

TS:   // 同上
来源：http://xm.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ow.jianghongdianzi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ky.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ab.colortex.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dv.bookmarksfly.cn

================================================================================
来源：http://ry.hahajie.cn

G. 面向对象
来源：http://fh.bookmarksfly.cn

================================================================================
来源：http://zw.chemitech.net.cn

[G01] 定义类
来源：http://xp.newstarts.cn

Py:   class User: pass
来源：http://rs.lnxyls.cn

PHP:  class User {}
来源：http://jl.bookmarksfly.cn

JS:   class User {}
来源：http://ig.huixinmuqiang.cn

TS:   class User { name: string = ""; }
来源：http://sc.huixiangedu.cn

Java: class User {}
来源：http://mc.gzmigu.cn

Go:   type User struct { Name string }
来源：http://jt.hnjuh.cn

Ruby: class User; end
来源：http://vm.bjjhwx.cn

C#:   class User {}
来源：http://md.nicolike.cn

[G02] 构造函数
来源：http://am.chemitech.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://yx.bjjhwx.cn

PHP:  public function __construct(public string $name) {}
来源：http://xp.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://tp.jctech888.com.cn

TS:   constructor(public name: string) {}
来源：http://km.panjiajie.cn

Java: User(String name) { this.name = name; }
来源：http://xx.muxihuayi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bx.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://cg.szxytkj.cn

C#:   public User(string name) { Name = name; }
来源：http://uk.yuexingan06.cn

[G03] 实例属性
来源：http://ao.szsharing.cn

Py:   self.name = "x"
来源：http://us.lnxyls.cn

PHP:  public string $name = "x";
来源：http://tw.hnjuh.cn

JS:   this.name = "x";
来源：http://qh.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://fh.shtwfgs.cn

Java: private String name;
来源：http://ay.huixiangedu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jl.shxzukj.cn

Ruby: @name = "x"
来源：http://jm.haigaiapp.cn

C#:   public string Name { get; set; } = "x";
来源：http://tc.szxytkj.cn

[G04] 定义方法
来源：http://xn.shtwfgs.cn

Py:   def greet(self): return self.name
来源：http://wy.yuexingan06.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bh.chemitech.net.cn

JS:   greet() { return this.name; }
来源：http://lo.521024.cn

TS:   greet(): string { return this.name; }
来源：http://ik.szsharing.cn

Java: String greet() { return name; }
来源：http://id.bjjhwx.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ax.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://ws.bjjhwx.cn

C#:   public string Greet() => Name;
来源：http://av.huixinmuqiang.cn

[G05] 继承
来源：http://fl.shxzukj.cn

Py:   class Admin(User): pass
来源：http://ni.hahajie.cn

PHP:  class Admin extends User {}
来源：http://fw.newstarts.cn

JS:   class Admin extends User {}
来源：http://kq.yuexingan06.cn

TS:   class Admin extends User {}
来源：http://gx.hnjuh.cn

Java: class Admin extends User {}
来源：http://gm.yuntaijiaju.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://js.szxytkj.cn

Ruby: class Admin < User; end
来源：http://pc.gzmigu.cn

C#:   class Admin : User {}
来源：http://hi.jianghongdianzi.cn

[G06] 重写方法
来源：http://ua.huixiangedu.cn

Py:   def greet(self): return "admin"
来源：http://iz.wgjwhj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vm.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://ji.huixinmuqiang.cn

TS:   greet(): string { return "admin"; }
来源：http://cu.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://ez.bjjhwx.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qz.lnxyls.cn

Ruby: def greet; "admin"; end
来源：http://wo.colortex.cn

C#:   public override string Greet() => "admin";
来源：http://hn.jctech888.com.cn

[G07] 调用父类方法
来源：http://cz.szxytkj.cn

Py:   super().greet()
来源：http://ae.yuexingan06.cn

PHP:  parent::greet();
来源：http://bi.521024.cn

JS:   super.greet();
来源：http://ya.colortex.cn

TS:   super.greet();
来源：http://tj.yuntaijiaju.cn

Java: super.greet();
来源：http://nx.muxihuayi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://qf.bookmarksfly.cn

Ruby: super
来源：http://us.szxytkj.cn

C#:   base.Greet();
来源：http://tk.bjjhwx.cn

[G08] 静态方法与属性
来源：http://ej.huixiangedu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lw.haigaiapp.cn

PHP:  public static function f() {}
来源：http://tc.lnxyls.cn

JS:   static f() {}
来源：http://ve.shxzskj.cn

TS:   static f(): void {}
来源：http://fm.szxytkj.cn

Java: static void f() {}
来源：http://ae.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://py.nicolike.cn

Ruby: def self.f; end
来源：http://sc.asd995.cn

C#:   public static void F() {}
来源：http://fq.shtwfgs.cn

[G09] 接口 / 抽象类
来源：http://ca.bookmarksfly.cn

Py:   from abc import ABC, abstractmethod
来源：http://zn.nszjky.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bo.muxihuayi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lq.9csxet.cn

TS:   interface Shape { area(): number; }
来源：http://lz.huixinmuqiang.cn

Java: interface Shape { double area(); }
来源：http://ka.hahajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://lm.huixiangedu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vp.panjiajie.cn

C#:   interface IShape { double Area(); }
来源：http://mn.colortex.cn

[G10] 访问控制
来源：http://gl.jianghongdianzi.cn

Py:   约定 _protected / __private（不强制）
来源：http://rj.shxzukj.cn

PHP:  public / protected / private
来源：http://qe.colortex.cn

JS:   #private 字段；其余公开
来源：http://ne.shxzskj.cn

TS:   public / protected / private
来源：http://zc.nszjky.cn

Java: public / protected / private / 默认包级
来源：http://mw.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dx.lnxyls.cn

Ruby: public / protected / private
来源：http://je.colortex.cn

C#:   public / protected / private / internal
来源：http://nb.muxihuayi.cn

[G11] getter / setter
来源：http://fc.huixiangedu.cn

Py:   @property 与 @x.setter
来源：http://tn.wgjwhj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vj.jianghongdianzi.cn

JS:   get name() { return this._name; }
来源：http://ue.521024.cn

TS:   get name(): string { return this._name; }
来源：http://jr.shtwfgs.cn

Java: public String getName() { return name; }
来源：http://qy.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xf.colortex.cn

Ruby: attr_accessor :name
来源：http://yo.shxzskj.cn

C#:   public string Name { get; set; }
来源：http://rl.huanxung.cn

[G12] 对象转字符串
来源：http://rp.hahajie.cn

Py:   def __str__(self): return self.name
来源：http://bg.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dh.huanxung.cn

JS:   toString() { return this.name; }
来源：http://sb.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://eo.shxzskj.cn

Java: @Override public String toString() { return name; }
来源：http://ce.shtwfgs.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bh.haigaiapp.cn

Ruby: def to_s; @name; end
来源：http://ts.jctech888.com.cn

C#:   public override string ToString() => Name;
来源：http://id.newstarts.cn

[G13] 判断对象类型
来源：http://jn.nszjky.cn

Py:   isinstance(u, User)
来源：http://bv.muxihuayi.cn

PHP:  $u instanceof User
来源：http://al.szxytkj.cn

JS:   u instanceof User
来源：http://dc.9csxet.cn

TS:   u instanceof User
来源：http://ry.huixinmuqiang.cn

Java: u instanceof User
来源：http://vc.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mu.huixiangedu.cn

Ruby: u.is_a?(User)
来源：http://gv.gzmigu.cn

C#:   u is User
来源：http://bh.haigaiapp.cn

[G14] 数据类 / record
来源：http://hg.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kt.huanxung.cn

PHP:  // 用 readonly 属性模拟
来源：http://ps.haigaiapp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wp.bjjhwx.cn

TS:   type User = { name: string; age: number };
来源：http://hr.newstarts.cn

Java: record User(String name, int age) {}
来源：http://lm.huixiangedu.cn

Go:   type User struct { Name string; Age int }
来源：http://qe.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mv.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://gt.shxzskj.cn

[G15] 枚举
来源：http://cm.jctech888.com.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://py.huixiangedu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qj.szxytkj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gp.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ie.szsharing.cn

Java: enum Color { RED, GREEN }
来源：http://lv.gzmigu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zj.bookmarksfly.cn

Ruby: Color = %i[red green].freeze
来源：http://md.jianghongdianzi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wr.shxzukj.cn

[G16] 对象转数组 / 字典
来源：http://yl.huanxung.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bh.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://zt.yuntaijiaju.cn

JS:   Object.entries(obj)
来源：http://zm.huanxung.cn

TS:   Object.entries(obj)
来源：http://gb.muxihuayi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hh.yuntaijiaju.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dp.jctech888.com.cn

Ruby: obj.instance_variables
来源：http://mp.huanxung.cn

C#:   // 用反射或 System.Text.Json
来源：http://ir.bjjhwx.cn

================================================================================
来源：http://ud.bjjhwx.cn

H. 异常与错误处理
来源：http://ls.huanxung.cn

================================================================================
来源：http://ei.huixinmuqiang.cn

[H01] try / catch 基础
来源：http://tm.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://np.yuntaijiaju.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fi.nicolike.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hm.bjjhwx.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pt.wgjwhj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://st.asd995.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fl.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vz.hahajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ne.huixinmuqiang.cn

[H02] finally / ensure 收尾
来源：http://gy.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://cc.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gq.asd995.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://oc.asd995.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zp.shxzukj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://iq.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xh.szsharing.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ct.nszjky.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lw.lnxyls.cn

[H03] 主动抛出异常
来源：http://cb.newstarts.cn

Py:   raise ValueError("错误信息")
来源：http://bu.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jy.gzmigu.cn

JS:   throw new Error("错误信息");
来源：http://ha.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://ps.hahajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zy.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fq.chemitech.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lg.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ya.shxzukj.cn

[H04] 自定义异常类型
来源：http://cq.lnxyls.cn

Py:   class MyError(Exception): pass
来源：http://rt.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yk.hahajie.cn

JS:   class MyError extends Error {}
来源：http://cc.wgjwhj.cn

TS:   class MyError extends Error {}
来源：http://uz.newstarts.cn

Java: class MyException extends RuntimeException {}
来源：http://xj.lnxyls.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ti.nszjky.cn

Ruby: class MyError < StandardError; end
来源：http://ep.wgjwhj.cn

C#:   class MyException : Exception {}
来源：http://rh.szsharing.cn

[H05] 捕获特定类型
来源：http://xd.yuexingan06.cn

Py:   except ValueError as e:
来源：http://um.nszjky.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wq.wgjwhj.cn

JS:   if (e instanceof TypeError) {}
来源：http://ms.newstarts.cn

TS:   if (e instanceof TypeError) {}
来源：http://go.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://fn.huanxung.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sz.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://yj.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ak.521024.cn

[H06] 可选值 / 空值安全访问
来源：http://nk.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://jt.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dd.haigaiapp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nv.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://eq.nicolike.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xz.gzmigu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yp.muxihuayi.cn

Ruby: d&.dig(:a, :b)
来源：http://hd.9csxet.cn

C#:   obj?.A?.B ?? default
来源：http://mk.huanxung.cn

[H07] 断言
来源：http://tz.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://nu.wgjwhj.cn

PHP:  assert($x > 0);
来源：http://ib.yuntaijiaju.cn

JS:   console.assert(x > 0);
来源：http://aw.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://ci.shxzukj.cn

Java: assert x > 0 : "必须为正";
来源：http://nf.muxihuayi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xf.yuexingan06.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lc.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://mj.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://qd.shtwfgs.cn

Py:   str(e);  traceback.format_exc()
来源：http://vj.huixinmuqiang.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rs.hahajie.cn


<!-- 参考信息 -->