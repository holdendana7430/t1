代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wx.colortex.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kj.hahajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zd.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://uz.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://kk.nszjky.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://on.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://ne.huixinmuqiang.cn

JS:   fs.existsSync("a.txt")
来源：http://jl.9csxet.cn

TS:   fs.existsSync("a.txt")
来源：http://ze.szxytkj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jl.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://vo.huixinmuqiang.cn

Ruby: File.exist?("a.txt")
来源：http://wr.chemitech.net.cn

C#:   File.Exists("a.txt")
来源：http://rq.szsharing.cn

[F06] 删除文件
来源：http://kc.yuexingan06.cn

Py:   os.remove("a.txt")
来源：http://sx.wgjwhj.cn

PHP:  unlink("a.txt");
来源：http://xw.haigaiapp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wj.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://oh.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mz.521024.cn

Go:   os.Remove("a.txt")
来源：http://he.huixiangedu.cn

Ruby: File.delete("a.txt")
来源：http://ep.9csxet.cn

C#:   File.Delete("a.txt");
来源：http://po.nicolike.cn

[F07] 创建目录（含多级）
来源：http://we.wgjwhj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ke.haigaiapp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nm.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wb.hnjuh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vu.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://dk.chemitech.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zz.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nz.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bg.huanxung.cn

[F08] 遍历目录
来源：http://yt.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xf.hnjuh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://la.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://dq.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://dr.9csxet.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qt.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fr.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://xs.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://ei.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://pi.521024.cn

Py:   os.path.getsize("a.txt")
来源：http://nt.lnxyls.cn

PHP:  filesize("a.txt");
来源：http://pn.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://yp.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://zr.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bd.muxihuayi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://oh.haigaiapp.cn

Ruby: File.size("a.txt")
来源：http://oj.huixiangedu.cn

C#:   new FileInfo("a.txt").Length
来源：http://ft.jctech888.com.cn

[F10] 取文件扩展名 / 文件名
来源：http://uj.yuexingan06.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rn.jctech888.com.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kp.bookmarksfly.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hl.szsharing.cn

TS:   path.extname("a.txt")
来源：http://kt.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://dg.asd995.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ez.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bp.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ob.yuntaijiaju.cn

[F11] 复制与移动文件
来源：http://uf.shxzukj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sr.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nf.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rv.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ms.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rd.szxytkj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qn.shtwfgs.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://eu.shxzukj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qi.asd995.cn

[F12] CSV 读写
来源：http://kl.nicolike.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mk.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zj.huanxung.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oo.9csxet.cn

TS:   // 同上
来源：http://yh.muxihuayi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://kz.yuexingan06.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://la.shxzskj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hc.huixinmuqiang.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://za.wgjwhj.cn

================================================================================
来源：http://ei.nicolike.cn

G. 面向对象
来源：http://id.gzmigu.cn

================================================================================
来源：http://ji.nszjky.cn

[G01] 定义类
来源：http://mj.chemitech.net.cn

Py:   class User: pass
来源：http://tg.panjiajie.cn

PHP:  class User {}
来源：http://wc.shtwfgs.cn

JS:   class User {}
来源：http://di.huixinmuqiang.cn

TS:   class User { name: string = ""; }
来源：http://yf.lnxyls.cn

Java: class User {}
来源：http://yw.shxzukj.cn

Go:   type User struct { Name string }
来源：http://ki.huixinmuqiang.cn

Ruby: class User; end
来源：http://hs.wgjwhj.cn

C#:   class User {}
来源：http://kq.panjiajie.cn

[G02] 构造函数
来源：http://up.colortex.cn

Py:   def __init__(self, name): self.name = name
来源：http://ua.shtwfgs.cn

PHP:  public function __construct(public string $name) {}
来源：http://kz.gzmigu.cn

JS:   constructor(name) { this.name = name; }
来源：http://zu.bookmarksfly.cn

TS:   constructor(public name: string) {}
来源：http://cr.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://jd.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://us.jctech888.com.cn

Ruby: def initialize(name); @name = name; end
来源：http://on.bjjhwx.cn

C#:   public User(string name) { Name = name; }
来源：http://js.wgjwhj.cn

[G03] 实例属性
来源：http://mz.huanxung.cn

Py:   self.name = "x"
来源：http://jn.hahajie.cn

PHP:  public string $name = "x";
来源：http://py.hnjuh.cn

JS:   this.name = "x";
来源：http://jt.asd995.cn

TS:   name: string = "x";
来源：http://bv.huixiangedu.cn

Java: private String name;
来源：http://th.szxytkj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://th.haigaiapp.cn

Ruby: @name = "x"
来源：http://nr.huixinmuqiang.cn

C#:   public string Name { get; set; } = "x";
来源：http://to.chemitech.net.cn

[G04] 定义方法
来源：http://ev.panjiajie.cn

Py:   def greet(self): return self.name
来源：http://ph.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bl.colortex.cn

JS:   greet() { return this.name; }
来源：http://al.yuntaijiaju.cn

TS:   greet(): string { return this.name; }
来源：http://sf.chemitech.net.cn

Java: String greet() { return name; }
来源：http://mb.gzmigu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nx.newstarts.cn

Ruby: def greet; @name; end
来源：http://ao.szsharing.cn

C#:   public string Greet() => Name;
来源：http://yq.huanxung.cn

[G05] 继承
来源：http://kl.9csxet.cn

Py:   class Admin(User): pass
来源：http://zy.szxytkj.cn

PHP:  class Admin extends User {}
来源：http://pb.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://qz.shxzukj.cn

TS:   class Admin extends User {}
来源：http://mk.bookmarksfly.cn

Java: class Admin extends User {}
来源：http://fz.chemitech.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mt.yuntaijiaju.cn

Ruby: class Admin < User; end
来源：http://dl.lnxyls.cn

C#:   class Admin : User {}
来源：http://wf.jctech888.com.cn

[G06] 重写方法
来源：http://kv.jctech888.com.cn

Py:   def greet(self): return "admin"
来源：http://zp.yuntaijiaju.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xc.gzmigu.cn

JS:   greet() { return "admin"; }
来源：http://nx.hahajie.cn

TS:   greet(): string { return "admin"; }
来源：http://ef.yuntaijiaju.cn

Java: @Override String greet() { return "admin"; }
来源：http://ha.bookmarksfly.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ss.jianghongdianzi.cn

Ruby: def greet; "admin"; end
来源：http://yz.newstarts.cn

C#:   public override string Greet() => "admin";
来源：http://nk.jctech888.com.cn

[G07] 调用父类方法
来源：http://wm.muxihuayi.cn

Py:   super().greet()
来源：http://yk.shtwfgs.cn

PHP:  parent::greet();
来源：http://wr.szxytkj.cn

JS:   super.greet();
来源：http://pv.panjiajie.cn

TS:   super.greet();
来源：http://yg.521024.cn

Java: super.greet();
来源：http://pb.szsharing.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ez.hahajie.cn

Ruby: super
来源：http://lq.jianghongdianzi.cn

C#:   base.Greet();
来源：http://kf.huixinmuqiang.cn

[G08] 静态方法与属性
来源：http://ja.hahajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gs.shxzukj.cn

PHP:  public static function f() {}
来源：http://cq.huixiangedu.cn

JS:   static f() {}
来源：http://dw.521024.cn

TS:   static f(): void {}
来源：http://nj.hahajie.cn

Java: static void f() {}
来源：http://aa.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xm.9csxet.cn

Ruby: def self.f; end
来源：http://he.nicolike.cn

C#:   public static void F() {}
来源：http://ns.wgjwhj.cn

[G09] 接口 / 抽象类
来源：http://fl.jctech888.com.cn

Py:   from abc import ABC, abstractmethod
来源：http://xw.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ux.nicolike.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mj.gzmigu.cn

TS:   interface Shape { area(): number; }
来源：http://za.bjjhwx.cn

Java: interface Shape { double area(); }
来源：http://lk.lnxyls.cn

Go:   type Shape interface { Area() float64 }
来源：http://lh.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fy.szsharing.cn

C#:   interface IShape { double Area(); }
来源：http://ky.gzmigu.cn

[G10] 访问控制
来源：http://cn.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://ga.gzmigu.cn

PHP:  public / protected / private
来源：http://cj.521024.cn

JS:   #private 字段；其余公开
来源：http://in.gzmigu.cn

TS:   public / protected / private
来源：http://cw.jianghongdianzi.cn

Java: public / protected / private / 默认包级
来源：http://oz.muxihuayi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jr.nszjky.cn

Ruby: public / protected / private
来源：http://dm.lnxyls.cn

C#:   public / protected / private / internal
来源：http://wu.9csxet.cn

[G11] getter / setter
来源：http://yp.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://vu.huixiangedu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ro.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://es.jctech888.com.cn

TS:   get name(): string { return this._name; }
来源：http://va.hahajie.cn

Java: public String getName() { return name; }
来源：http://pn.panjiajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ub.szsharing.cn

Ruby: attr_accessor :name
来源：http://xr.szxytkj.cn

C#:   public string Name { get; set; }
来源：http://bp.bookmarksfly.cn

[G12] 对象转字符串
来源：http://zg.jctech888.com.cn

Py:   def __str__(self): return self.name
来源：http://yz.colortex.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dv.szxytkj.cn

JS:   toString() { return this.name; }
来源：http://hy.asd995.cn

TS:   toString(): string { return this.name; }
来源：http://kt.nicolike.cn

Java: @Override public String toString() { return name; }
来源：http://ul.521024.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qq.newstarts.cn

Ruby: def to_s; @name; end
来源：http://fd.bookmarksfly.cn

C#:   public override string ToString() => Name;
来源：http://pp.9csxet.cn

[G13] 判断对象类型
来源：http://ss.hahajie.cn

Py:   isinstance(u, User)
来源：http://ce.lnxyls.cn

PHP:  $u instanceof User
来源：http://ni.hnjuh.cn

JS:   u instanceof User
来源：http://dk.shtwfgs.cn

TS:   u instanceof User
来源：http://lg.newstarts.cn

Java: u instanceof User
来源：http://df.yuntaijiaju.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mt.521024.cn

Ruby: u.is_a?(User)
来源：http://ns.nicolike.cn

C#:   u is User
来源：http://sk.huanxung.cn

[G14] 数据类 / record
来源：http://yw.wgjwhj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://am.hahajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://nz.hnjuh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://je.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://uz.szsharing.cn

Java: record User(String name, int age) {}
来源：http://zo.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://bv.nicolike.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://na.hnjuh.cn

C#:   record User(string Name, int Age);
来源：http://np.hnjuh.cn

[G15] 枚举
来源：http://jn.szsharing.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fj.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bg.shtwfgs.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qw.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rq.huixinmuqiang.cn

Java: enum Color { RED, GREEN }
来源：http://lw.shxzukj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gc.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://xx.yuexingan06.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jf.nszjky.cn

[G16] 对象转数组 / 字典
来源：http://ks.colortex.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ew.newstarts.cn

PHP:  get_object_vars($obj);
来源：http://xn.lnxyls.cn

JS:   Object.entries(obj)
来源：http://ao.huixiangedu.cn

TS:   Object.entries(obj)
来源：http://nl.newstarts.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://th.panjiajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://aj.muxihuayi.cn

Ruby: obj.instance_variables
来源：http://zh.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://fo.huixinmuqiang.cn

================================================================================
来源：http://dh.huixinmuqiang.cn

H. 异常与错误处理
来源：http://wk.colortex.cn

================================================================================
来源：http://qo.colortex.cn

[H01] try / catch 基础
来源：http://ji.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vp.huixiangedu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ik.jianghongdianzi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tq.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zx.szxytkj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cb.szsharing.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ab.colortex.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oq.szsharing.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pi.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://ob.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ii.szxytkj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wb.521024.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hj.hnjuh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://om.asd995.cn

Java: try { f(); } finally { cleanup(); }
来源：http://os.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://aa.jctech888.com.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nx.yuntaijiaju.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cl.huixiangedu.cn

[H03] 主动抛出异常
来源：http://uh.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://oc.hnjuh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qy.huanxung.cn

JS:   throw new Error("错误信息");
来源：http://qo.szxytkj.cn

TS:   throw new Error("错误信息");
来源：http://zi.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yg.hnjuh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lr.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vo.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://no.nicolike.cn

[H04] 自定义异常类型
来源：http://rw.szsharing.cn

Py:   class MyError(Exception): pass
来源：http://zz.chemitech.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gx.colortex.cn

JS:   class MyError extends Error {}
来源：http://wn.nszjky.cn

TS:   class MyError extends Error {}
来源：http://in.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://bh.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ev.haigaiapp.cn

Ruby: class MyError < StandardError; end
来源：http://dy.haigaiapp.cn

C#:   class MyException : Exception {}
来源：http://bc.haigaiapp.cn

[H05] 捕获特定类型
来源：http://ti.521024.cn

Py:   except ValueError as e:
来源：http://nn.shxzskj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jv.hahajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://zm.bjjhwx.cn

TS:   if (e instanceof TypeError) {}
来源：http://dz.szxytkj.cn

Java: catch (IOException | SQLException e) {}
来源：http://zg.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tj.huixinmuqiang.cn

Ruby: rescue ArgumentError => e
来源：http://md.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ig.521024.cn

[H06] 可选值 / 空值安全访问
来源：http://fj.yuexingan06.cn

Py:   value = d.get("k") or default
来源：http://ne.wgjwhj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ly.chemitech.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://uz.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hx.hnjuh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zv.shxzukj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rb.hnjuh.cn

Ruby: d&.dig(:a, :b)
来源：http://vq.chemitech.net.cn

C#:   obj?.A?.B ?? default
来源：http://xd.huixinmuqiang.cn

[H07] 断言
来源：http://bk.jianghongdianzi.cn

Py:   assert x > 0, "必须为正"
来源：http://gk.bjjhwx.cn

PHP:  assert($x > 0);
来源：http://gp.9csxet.cn

JS:   console.assert(x > 0);
来源：http://yt.hahajie.cn

TS:   console.assert(x > 0);
来源：http://pk.jianghongdianzi.cn

Java: assert x > 0 : "必须为正";
来源：http://mp.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://to.huixinmuqiang.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fe.szsharing.cn

C#:   Debug.Assert(x > 0);
来源：http://iz.yuntaijiaju.cn

[H08] 获取错误信息与堆栈
来源：http://mt.bjjhwx.cn

Py:   str(e);  traceback.format_exc()
来源：http://an.panjiajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zq.newstarts.cn

JS:   e.message;  e.stack
来源：http://lo.jctech888.com.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ae.hnjuh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zp.szxytkj.cn

Go:   err.Error()
来源：http://rj.panjiajie.cn

Ruby: e.message;  e.backtrace
来源：http://qj.hahajie.cn

C#:   e.Message;  e.StackTrace
来源：http://nr.muxihuayi.cn

[H09] 带错误码的异常
来源：http://bd.nicolike.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ik.muxihuayi.cn


<!-- 参考信息 -->