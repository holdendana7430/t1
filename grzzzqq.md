代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nr.shtwfgs.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://so.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tl.szsharing.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sg.huanxung.cn

[F05] 判断文件或目录是否存在
来源：http://aj.bookmarksfly.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://od.lnxyls.cn

PHP:  file_exists("a.txt");
来源：http://zy.muxihuayi.cn

JS:   fs.existsSync("a.txt")
来源：http://to.bookmarksfly.cn

TS:   fs.existsSync("a.txt")
来源：http://rd.huanxung.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://iy.521024.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://od.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://jc.shxzukj.cn

C#:   File.Exists("a.txt")
来源：http://hx.yuexingan06.cn

[F06] 删除文件
来源：http://uq.yuexingan06.cn

Py:   os.remove("a.txt")
来源：http://pi.jctech888.com.cn

PHP:  unlink("a.txt");
来源：http://by.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tn.hnjuh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zp.szxytkj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://pq.haigaiapp.cn

Go:   os.Remove("a.txt")
来源：http://tm.gzmigu.cn

Ruby: File.delete("a.txt")
来源：http://cz.huanxung.cn

C#:   File.Delete("a.txt");
来源：http://qq.nicolike.cn

[F07] 创建目录（含多级）
来源：http://ap.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nw.yuexingan06.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wd.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sh.huanxung.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pr.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ns.521024.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fg.wgjwhj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gj.wgjwhj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ee.huixiangedu.cn

[F08] 遍历目录
来源：http://fm.muxihuayi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://je.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://zk.yuexingan06.cn

JS:   fs.readdirSync("dir")
来源：http://kh.huanxung.cn

TS:   fs.readdirSync("dir")
来源：http://ij.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ae.bookmarksfly.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://st.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://dr.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://dd.nicolike.cn

[F09] 获取文件大小
来源：http://pr.lnxyls.cn

Py:   os.path.getsize("a.txt")
来源：http://ng.9csxet.cn

PHP:  filesize("a.txt");
来源：http://dl.bjjhwx.cn

JS:   fs.statSync("a.txt").size
来源：http://ba.szsharing.cn

TS:   fs.statSync("a.txt").size
来源：http://dt.wgjwhj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ak.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yu.shxzskj.cn

Ruby: File.size("a.txt")
来源：http://jt.hahajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://jc.huixinmuqiang.cn

[F10] 取文件扩展名 / 文件名
来源：http://to.nszjky.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://iw.shtwfgs.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://iv.9csxet.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://aw.newstarts.cn

TS:   path.extname("a.txt")
来源：http://gx.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sf.colortex.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ri.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ty.chemitech.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ry.jctech888.com.cn

[F11] 复制与移动文件
来源：http://ny.asd995.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ty.panjiajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vp.newstarts.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wd.bjjhwx.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wa.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://du.colortex.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mo.bookmarksfly.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ex.chemitech.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gj.shtwfgs.cn

[F12] CSV 读写
来源：http://to.shxzukj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ka.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vl.hahajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yo.hnjuh.cn

TS:   // 同上
来源：http://qt.yuntaijiaju.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vg.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ca.asd995.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://sv.nszjky.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://tz.hnjuh.cn

================================================================================
来源：http://sh.nicolike.cn

G. 面向对象
来源：http://jp.huixiangedu.cn

================================================================================
来源：http://ke.shxzukj.cn

[G01] 定义类
来源：http://ok.yuexingan06.cn

Py:   class User: pass
来源：http://pe.huixinmuqiang.cn

PHP:  class User {}
来源：http://ff.gzmigu.cn

JS:   class User {}
来源：http://kn.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://fq.muxihuayi.cn

Java: class User {}
来源：http://qq.9csxet.cn

Go:   type User struct { Name string }
来源：http://ta.shxzukj.cn

Ruby: class User; end
来源：http://xc.bookmarksfly.cn

C#:   class User {}
来源：http://bn.huixinmuqiang.cn

[G02] 构造函数
来源：http://kc.shtwfgs.cn

Py:   def __init__(self, name): self.name = name
来源：http://rk.bjjhwx.cn

PHP:  public function __construct(public string $name) {}
来源：http://kb.huanxung.cn

JS:   constructor(name) { this.name = name; }
来源：http://zh.jctech888.com.cn

TS:   constructor(public name: string) {}
来源：http://jc.szxytkj.cn

Java: User(String name) { this.name = name; }
来源：http://do.muxihuayi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://gw.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://or.chemitech.net.cn

C#:   public User(string name) { Name = name; }
来源：http://vg.muxihuayi.cn

[G03] 实例属性
来源：http://ns.521024.cn

Py:   self.name = "x"
来源：http://ke.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://ip.colortex.cn

JS:   this.name = "x";
来源：http://gq.panjiajie.cn

TS:   name: string = "x";
来源：http://on.szsharing.cn

Java: private String name;
来源：http://pm.chemitech.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qy.haigaiapp.cn

Ruby: @name = "x"
来源：http://ar.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://pe.9csxet.cn

[G04] 定义方法
来源：http://gb.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://lu.jctech888.com.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zi.jianghongdianzi.cn

JS:   greet() { return this.name; }
来源：http://pr.huixinmuqiang.cn

TS:   greet(): string { return this.name; }
来源：http://rg.nszjky.cn

Java: String greet() { return name; }
来源：http://db.shtwfgs.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fv.szxytkj.cn

Ruby: def greet; @name; end
来源：http://wi.gzmigu.cn

C#:   public string Greet() => Name;
来源：http://ix.shtwfgs.cn

[G05] 继承
来源：http://oc.shxzukj.cn

Py:   class Admin(User): pass
来源：http://vq.521024.cn

PHP:  class Admin extends User {}
来源：http://cb.hnjuh.cn

JS:   class Admin extends User {}
来源：http://ek.hahajie.cn

TS:   class Admin extends User {}
来源：http://bm.nszjky.cn

Java: class Admin extends User {}
来源：http://fv.asd995.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rr.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://dx.huixiangedu.cn

C#:   class Admin : User {}
来源：http://cj.chemitech.net.cn

[G06] 重写方法
来源：http://ma.newstarts.cn

Py:   def greet(self): return "admin"
来源：http://yb.panjiajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ph.shxzskj.cn

JS:   greet() { return "admin"; }
来源：http://qg.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://bl.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://kt.huixinmuqiang.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://zs.hahajie.cn

Ruby: def greet; "admin"; end
来源：http://kx.bjjhwx.cn

C#:   public override string Greet() => "admin";
来源：http://hn.shxzskj.cn

[G07] 调用父类方法
来源：http://sa.szxytkj.cn

Py:   super().greet()
来源：http://dy.lnxyls.cn

PHP:  parent::greet();
来源：http://di.yuexingan06.cn

JS:   super.greet();
来源：http://cu.asd995.cn

TS:   super.greet();
来源：http://nz.lnxyls.cn

Java: super.greet();
来源：http://sc.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cn.hnjuh.cn

Ruby: super
来源：http://be.gzmigu.cn

C#:   base.Greet();
来源：http://cl.huixinmuqiang.cn

[G08] 静态方法与属性
来源：http://kj.colortex.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kk.wgjwhj.cn

PHP:  public static function f() {}
来源：http://vy.9csxet.cn

JS:   static f() {}
来源：http://vy.szsharing.cn

TS:   static f(): void {}
来源：http://an.szxytkj.cn

Java: static void f() {}
来源：http://yn.yuexingan06.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://lq.bookmarksfly.cn

Ruby: def self.f; end
来源：http://wp.bjjhwx.cn

C#:   public static void F() {}
来源：http://lj.jctech888.com.cn

[G09] 接口 / 抽象类
来源：http://fa.yuntaijiaju.cn

Py:   from abc import ABC, abstractmethod
来源：http://oq.bjjhwx.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wl.hahajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lo.newstarts.cn

TS:   interface Shape { area(): number; }
来源：http://ji.newstarts.cn

Java: interface Shape { double area(); }
来源：http://rt.9csxet.cn

Go:   type Shape interface { Area() float64 }
来源：http://df.lnxyls.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://re.huanxung.cn

C#:   interface IShape { double Area(); }
来源：http://bj.nszjky.cn

[G10] 访问控制
来源：http://cg.chemitech.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://lu.szsharing.cn

PHP:  public / protected / private
来源：http://ck.lnxyls.cn

JS:   #private 字段；其余公开
来源：http://ld.jianghongdianzi.cn

TS:   public / protected / private
来源：http://aa.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://zk.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pf.shtwfgs.cn

Ruby: public / protected / private
来源：http://li.gzmigu.cn

C#:   public / protected / private / internal
来源：http://ge.hnjuh.cn

[G11] getter / setter
来源：http://id.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://am.shtwfgs.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://go.shtwfgs.cn

JS:   get name() { return this._name; }
来源：http://sm.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://wk.huixiangedu.cn

Java: public String getName() { return name; }
来源：http://ng.9csxet.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ki.haigaiapp.cn

Ruby: attr_accessor :name
来源：http://aw.hahajie.cn

C#:   public string Name { get; set; }
来源：http://ty.lnxyls.cn

[G12] 对象转字符串
来源：http://oc.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://dg.jctech888.com.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nl.haigaiapp.cn

JS:   toString() { return this.name; }
来源：http://ht.chemitech.net.cn

TS:   toString(): string { return this.name; }
来源：http://sx.nszjky.cn

Java: @Override public String toString() { return name; }
来源：http://ez.nszjky.cn

Go:   func (u User) String() string { return u.Name }
来源：http://db.jctech888.com.cn

Ruby: def to_s; @name; end
来源：http://ih.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://ws.bookmarksfly.cn

[G13] 判断对象类型
来源：http://zz.shxzukj.cn

Py:   isinstance(u, User)
来源：http://sh.hnjuh.cn

PHP:  $u instanceof User
来源：http://ld.nicolike.cn

JS:   u instanceof User
来源：http://tu.bookmarksfly.cn

TS:   u instanceof User
来源：http://wg.yuexingan06.cn

Java: u instanceof User
来源：http://lm.521024.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xd.haigaiapp.cn

Ruby: u.is_a?(User)
来源：http://ne.hahajie.cn

C#:   u is User
来源：http://gd.huixinmuqiang.cn

[G14] 数据类 / record
来源：http://yx.hnjuh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://be.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://qw.haigaiapp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ov.chemitech.net.cn

TS:   type User = { name: string; age: number };
来源：http://jz.haigaiapp.cn

Java: record User(String name, int age) {}
来源：http://fd.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://gu.shxzukj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yy.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://gn.chemitech.net.cn

[G15] 枚举
来源：http://cx.lnxyls.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xm.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ih.nszjky.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hw.jctech888.com.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pp.colortex.cn

Java: enum Color { RED, GREEN }
来源：http://pe.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sb.shxzskj.cn

Ruby: Color = %i[red green].freeze
来源：http://od.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://le.newstarts.cn

[G16] 对象转数组 / 字典
来源：http://em.nicolike.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://td.521024.cn

PHP:  get_object_vars($obj);
来源：http://de.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://vi.yuexingan06.cn

TS:   Object.entries(obj)
来源：http://ae.jctech888.com.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cf.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://la.nicolike.cn

Ruby: obj.instance_variables
来源：http://nq.hnjuh.cn

C#:   // 用反射或 System.Text.Json
来源：http://qn.lnxyls.cn

================================================================================
来源：http://fp.521024.cn

H. 异常与错误处理
来源：http://hb.shxzskj.cn

================================================================================
来源：http://cr.9csxet.cn

[H01] try / catch 基础
来源：http://xn.521024.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gk.newstarts.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jw.panjiajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://je.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jq.huixinmuqiang.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zv.szsharing.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sf.shxzskj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nv.huanxung.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oi.chemitech.net.cn

[H02] finally / ensure 收尾
来源：http://wc.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://py.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rm.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ki.bookmarksfly.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yw.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gr.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cm.nszjky.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gn.huixiangedu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://my.huixinmuqiang.cn

[H03] 主动抛出异常
来源：http://yw.yuntaijiaju.cn

Py:   raise ValueError("错误信息")
来源：http://vn.colortex.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gv.shxzskj.cn

JS:   throw new Error("错误信息");
来源：http://ax.bjjhwx.cn

TS:   throw new Error("错误信息");
来源：http://hu.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lf.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qf.yuexingan06.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tn.9csxet.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ek.asd995.cn

[H04] 自定义异常类型
来源：http://jk.jianghongdianzi.cn

Py:   class MyError(Exception): pass
来源：http://xa.wgjwhj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tz.huixiangedu.cn

JS:   class MyError extends Error {}
来源：http://yy.szsharing.cn

TS:   class MyError extends Error {}
来源：http://vh.newstarts.cn

Java: class MyException extends RuntimeException {}
来源：http://pf.lnxyls.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://at.bjjhwx.cn

Ruby: class MyError < StandardError; end
来源：http://br.jianghongdianzi.cn

C#:   class MyException : Exception {}
来源：http://kx.panjiajie.cn

[H05] 捕获特定类型
来源：http://lf.chemitech.net.cn

Py:   except ValueError as e:
来源：http://dl.nszjky.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gr.shxzskj.cn

JS:   if (e instanceof TypeError) {}
来源：http://hh.szxytkj.cn

TS:   if (e instanceof TypeError) {}
来源：http://pf.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://oj.asd995.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lz.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://af.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zq.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://fo.colortex.cn

Py:   value = d.get("k") or default
来源：http://er.bjjhwx.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vl.nicolike.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rg.hahajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ab.panjiajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hv.shxzukj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gs.shtwfgs.cn

Ruby: d&.dig(:a, :b)
来源：http://qw.muxihuayi.cn

C#:   obj?.A?.B ?? default
来源：http://oh.hnjuh.cn

[H07] 断言
来源：http://yz.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://uf.huixiangedu.cn

PHP:  assert($x > 0);
来源：http://jq.gzmigu.cn

JS:   console.assert(x > 0);
来源：http://mo.asd995.cn

TS:   console.assert(x > 0);
来源：http://bf.szsharing.cn

Java: assert x > 0 : "必须为正";
来源：http://bn.asd995.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dd.hahajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qp.colortex.cn

C#:   Debug.Assert(x > 0);
来源：http://gn.521024.cn

[H08] 获取错误信息与堆栈
来源：http://wx.jctech888.com.cn

Py:   str(e);  traceback.format_exc()
来源：http://mb.chemitech.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://he.huixinmuqiang.cn

JS:   e.message;  e.stack
来源：http://ll.jianghongdianzi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://cm.huixiangedu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://da.newstarts.cn

Go:   err.Error()
来源：http://wl.haigaiapp.cn

Ruby: e.message;  e.backtrace
来源：http://lk.nszjky.cn

C#:   e.Message;  e.StackTrace
来源：http://gb.shtwfgs.cn

[H09] 带错误码的异常
来源：http://ai.colortex.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yn.asd995.cn


<!-- 参考信息 -->