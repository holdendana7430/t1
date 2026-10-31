代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ou.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ib.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://jw.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ew.newstarts.cn

[F05] 判断文件或目录是否存在
来源：http://lu.jctech888.com.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://eb.9csxet.cn

PHP:  file_exists("a.txt");
来源：http://hn.asd995.cn

JS:   fs.existsSync("a.txt")
来源：http://nt.yuexingan06.cn

TS:   fs.existsSync("a.txt")
来源：http://vg.muxihuayi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vh.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xe.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://dt.gzmigu.cn

C#:   File.Exists("a.txt")
来源：http://or.huanxung.cn

[F06] 删除文件
来源：http://ki.hahajie.cn

Py:   os.remove("a.txt")
来源：http://va.szxytkj.cn

PHP:  unlink("a.txt");
来源：http://hn.huanxung.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ym.hnjuh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ej.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ht.wgjwhj.cn

Go:   os.Remove("a.txt")
来源：http://si.szsharing.cn

Ruby: File.delete("a.txt")
来源：http://dl.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://so.huanxung.cn

[F07] 创建目录（含多级）
来源：http://ph.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wf.yuexingan06.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xg.bookmarksfly.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://an.nszjky.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://uc.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xw.chemitech.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zv.lnxyls.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tk.nicolike.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kv.huixinmuqiang.cn

[F08] 遍历目录
来源：http://lk.bookmarksfly.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://oy.wgjwhj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sk.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://cl.huixinmuqiang.cn

TS:   fs.readdirSync("dir")
来源：http://vm.shxzukj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sr.gzmigu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vk.newstarts.cn

Ruby: Dir.children("dir")
来源：http://ve.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://vy.shtwfgs.cn

[F09] 获取文件大小
来源：http://zo.huixinmuqiang.cn

Py:   os.path.getsize("a.txt")
来源：http://yp.9csxet.cn

PHP:  filesize("a.txt");
来源：http://kk.hnjuh.cn

JS:   fs.statSync("a.txt").size
来源：http://ot.colortex.cn

TS:   fs.statSync("a.txt").size
来源：http://yc.nszjky.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yv.bookmarksfly.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ek.shxzukj.cn

Ruby: File.size("a.txt")
来源：http://eh.lnxyls.cn

C#:   new FileInfo("a.txt").Length
来源：http://fz.szsharing.cn

[F10] 取文件扩展名 / 文件名
来源：http://de.yuntaijiaju.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zn.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cv.bjjhwx.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lq.hnjuh.cn

TS:   path.extname("a.txt")
来源：http://rp.huixinmuqiang.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hj.9csxet.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ys.yuexingan06.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vj.asd995.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cw.huixiangedu.cn

[F11] 复制与移动文件
来源：http://yf.szsharing.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://oq.szsharing.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dw.yuntaijiaju.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pv.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nu.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ke.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://re.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://we.szsharing.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://df.shxzskj.cn

[F12] CSV 读写
来源：http://dl.bjjhwx.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gd.lnxyls.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://la.bookmarksfly.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ni.bjjhwx.cn

TS:   // 同上
来源：http://rc.yuntaijiaju.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rt.yuexingan06.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gk.hnjuh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://dy.hahajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ht.9csxet.cn

================================================================================
来源：http://uy.chemitech.net.cn

G. 面向对象
来源：http://jq.haigaiapp.cn

================================================================================
来源：http://ab.hnjuh.cn

[G01] 定义类
来源：http://bj.szsharing.cn

Py:   class User: pass
来源：http://zd.9csxet.cn

PHP:  class User {}
来源：http://jz.hahajie.cn

JS:   class User {}
来源：http://px.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://mv.huanxung.cn

Java: class User {}
来源：http://nd.jctech888.com.cn

Go:   type User struct { Name string }
来源：http://sl.newstarts.cn

Ruby: class User; end
来源：http://sl.asd995.cn

C#:   class User {}
来源：http://ko.hnjuh.cn

[G02] 构造函数
来源：http://op.yuexingan06.cn

Py:   def __init__(self, name): self.name = name
来源：http://or.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://we.shxzskj.cn

JS:   constructor(name) { this.name = name; }
来源：http://vx.hahajie.cn

TS:   constructor(public name: string) {}
来源：http://fi.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://ej.panjiajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rg.bjjhwx.cn

Ruby: def initialize(name); @name = name; end
来源：http://rj.shtwfgs.cn

C#:   public User(string name) { Name = name; }
来源：http://wt.nszjky.cn

[G03] 实例属性
来源：http://bt.colortex.cn

Py:   self.name = "x"
来源：http://tw.colortex.cn

PHP:  public string $name = "x";
来源：http://ig.huanxung.cn

JS:   this.name = "x";
来源：http://es.shtwfgs.cn

TS:   name: string = "x";
来源：http://qz.bjjhwx.cn

Java: private String name;
来源：http://wl.jctech888.com.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://uw.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://aj.huixinmuqiang.cn

C#:   public string Name { get; set; } = "x";
来源：http://xx.shtwfgs.cn

[G04] 定义方法
来源：http://ow.shtwfgs.cn

Py:   def greet(self): return self.name
来源：http://sm.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zh.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://pi.huixiangedu.cn

TS:   greet(): string { return this.name; }
来源：http://za.asd995.cn

Java: String greet() { return name; }
来源：http://yz.huixiangedu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hb.bjjhwx.cn

Ruby: def greet; @name; end
来源：http://mh.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://uh.chemitech.net.cn

[G05] 继承
来源：http://id.jctech888.com.cn

Py:   class Admin(User): pass
来源：http://oe.szxytkj.cn

PHP:  class Admin extends User {}
来源：http://ck.asd995.cn

JS:   class Admin extends User {}
来源：http://hj.lnxyls.cn

TS:   class Admin extends User {}
来源：http://qa.muxihuayi.cn

Java: class Admin extends User {}
来源：http://tg.hnjuh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ys.szxytkj.cn

Ruby: class Admin < User; end
来源：http://zc.shxzskj.cn

C#:   class Admin : User {}
来源：http://do.nicolike.cn

[G06] 重写方法
来源：http://ac.shxzukj.cn

Py:   def greet(self): return "admin"
来源：http://fc.hahajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://im.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://rb.shtwfgs.cn

TS:   greet(): string { return "admin"; }
来源：http://vn.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://fg.shtwfgs.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ca.asd995.cn

Ruby: def greet; "admin"; end
来源：http://uz.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://jg.9csxet.cn

[G07] 调用父类方法
来源：http://en.bookmarksfly.cn

Py:   super().greet()
来源：http://ty.shxzskj.cn

PHP:  parent::greet();
来源：http://mb.shxzukj.cn

JS:   super.greet();
来源：http://vd.jianghongdianzi.cn

TS:   super.greet();
来源：http://qw.chemitech.net.cn

Java: super.greet();
来源：http://mj.muxihuayi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eo.panjiajie.cn

Ruby: super
来源：http://mt.521024.cn

C#:   base.Greet();
来源：http://fp.jctech888.com.cn

[G08] 静态方法与属性
来源：http://ls.huanxung.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vu.szsharing.cn

PHP:  public static function f() {}
来源：http://wf.521024.cn

JS:   static f() {}
来源：http://dq.newstarts.cn

TS:   static f(): void {}
来源：http://az.huanxung.cn

Java: static void f() {}
来源：http://sj.panjiajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://oe.521024.cn

Ruby: def self.f; end
来源：http://tl.szxytkj.cn

C#:   public static void F() {}
来源：http://uo.yuntaijiaju.cn

[G09] 接口 / 抽象类
来源：http://sr.jctech888.com.cn

Py:   from abc import ABC, abstractmethod
来源：http://fk.nicolike.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uq.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tt.huixiangedu.cn

TS:   interface Shape { area(): number; }
来源：http://gk.9csxet.cn

Java: interface Shape { double area(); }
来源：http://pp.newstarts.cn

Go:   type Shape interface { Area() float64 }
来源：http://gm.panjiajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ba.huixiangedu.cn

C#:   interface IShape { double Area(); }
来源：http://vg.shxzskj.cn

[G10] 访问控制
来源：http://eb.chemitech.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://ac.shtwfgs.cn

PHP:  public / protected / private
来源：http://np.wgjwhj.cn

JS:   #private 字段；其余公开
来源：http://vj.hnjuh.cn

TS:   public / protected / private
来源：http://vx.colortex.cn

Java: public / protected / private / 默认包级
来源：http://st.shxzukj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bs.nicolike.cn

Ruby: public / protected / private
来源：http://hd.nicolike.cn

C#:   public / protected / private / internal
来源：http://ws.huanxung.cn

[G11] getter / setter
来源：http://dk.gzmigu.cn

Py:   @property 与 @x.setter
来源：http://xc.huixinmuqiang.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tz.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://iu.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://qz.colortex.cn

Java: public String getName() { return name; }
来源：http://ka.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bn.colortex.cn

Ruby: attr_accessor :name
来源：http://ro.nicolike.cn

C#:   public string Name { get; set; }
来源：http://fs.panjiajie.cn

[G12] 对象转字符串
来源：http://mg.nszjky.cn

Py:   def __str__(self): return self.name
来源：http://pl.huixinmuqiang.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qb.521024.cn

JS:   toString() { return this.name; }
来源：http://xg.huixiangedu.cn

TS:   toString(): string { return this.name; }
来源：http://vy.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://bd.shtwfgs.cn

Go:   func (u User) String() string { return u.Name }
来源：http://iv.521024.cn

Ruby: def to_s; @name; end
来源：http://ux.shtwfgs.cn

C#:   public override string ToString() => Name;
来源：http://os.wgjwhj.cn

[G13] 判断对象类型
来源：http://kp.shtwfgs.cn

Py:   isinstance(u, User)
来源：http://sf.huixiangedu.cn

PHP:  $u instanceof User
来源：http://vx.hahajie.cn

JS:   u instanceof User
来源：http://xp.muxihuayi.cn

TS:   u instanceof User
来源：http://rj.panjiajie.cn

Java: u instanceof User
来源：http://ic.shxzukj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sr.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://qn.hahajie.cn

C#:   u is User
来源：http://ve.huixiangedu.cn

[G14] 数据类 / record
来源：http://tc.newstarts.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zk.szsharing.cn

PHP:  // 用 readonly 属性模拟
来源：http://ma.haigaiapp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gl.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://wf.shtwfgs.cn

Java: record User(String name, int age) {}
来源：http://ny.nszjky.cn

Go:   type User struct { Name string; Age int }
来源：http://jn.nicolike.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yg.bookmarksfly.cn

C#:   record User(string Name, int Age);
来源：http://fp.yuexingan06.cn

[G15] 枚举
来源：http://iw.jctech888.com.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ao.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://le.huixinmuqiang.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mi.hnjuh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bm.gzmigu.cn

Java: enum Color { RED, GREEN }
来源：http://iw.hnjuh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rz.bjjhwx.cn

Ruby: Color = %i[red green].freeze
来源：http://um.panjiajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://my.lnxyls.cn

[G16] 对象转数组 / 字典
来源：http://ed.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vr.huixinmuqiang.cn

PHP:  get_object_vars($obj);
来源：http://mu.521024.cn

JS:   Object.entries(obj)
来源：http://kf.gzmigu.cn

TS:   Object.entries(obj)
来源：http://bu.jctech888.com.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://em.colortex.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://li.newstarts.cn

Ruby: obj.instance_variables
来源：http://is.huanxung.cn

C#:   // 用反射或 System.Text.Json
来源：http://al.9csxet.cn

================================================================================
来源：http://ms.hnjuh.cn

H. 异常与错误处理
来源：http://cf.521024.cn

================================================================================
来源：http://ri.muxihuayi.cn

[H01] try / catch 基础
来源：http://au.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ra.yuexingan06.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hu.panjiajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bb.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ds.9csxet.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sw.lnxyls.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tq.haigaiapp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gy.bjjhwx.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fg.asd995.cn

[H02] finally / ensure 收尾
来源：http://ja.colortex.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xi.panjiajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mw.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bn.shxzskj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lu.huixinmuqiang.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wd.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zy.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ii.huixiangedu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sn.gzmigu.cn

[H03] 主动抛出异常
来源：http://up.asd995.cn

Py:   raise ValueError("错误信息")
来源：http://ol.nicolike.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mq.gzmigu.cn

JS:   throw new Error("错误信息");
来源：http://xp.hahajie.cn

TS:   throw new Error("错误信息");
来源：http://dk.hahajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yj.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uz.haigaiapp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hk.shxzukj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nt.huixiangedu.cn

[H04] 自定义异常类型
来源：http://vd.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://sx.shxzukj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wz.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://qa.newstarts.cn

TS:   class MyError extends Error {}
来源：http://ok.yuntaijiaju.cn

Java: class MyException extends RuntimeException {}
来源：http://eq.wgjwhj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sf.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://pu.jctech888.com.cn

C#:   class MyException : Exception {}
来源：http://kx.nszjky.cn

[H05] 捕获特定类型
来源：http://yg.asd995.cn

Py:   except ValueError as e:
来源：http://cy.huanxung.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ge.huanxung.cn

JS:   if (e instanceof TypeError) {}
来源：http://ix.nszjky.cn

TS:   if (e instanceof TypeError) {}
来源：http://nx.panjiajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://qs.huixinmuqiang.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hs.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://lp.chemitech.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nf.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://le.jctech888.com.cn

Py:   value = d.get("k") or default
来源：http://zu.muxihuayi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://dw.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yt.huixinmuqiang.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zs.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dx.huanxung.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://if.gzmigu.cn

Ruby: d&.dig(:a, :b)
来源：http://ic.szsharing.cn

C#:   obj?.A?.B ?? default
来源：http://rb.yuntaijiaju.cn

[H07] 断言
来源：http://mu.lnxyls.cn

Py:   assert x > 0, "必须为正"
来源：http://sf.shxzukj.cn

PHP:  assert($x > 0);
来源：http://nj.szxytkj.cn

JS:   console.assert(x > 0);
来源：http://et.hahajie.cn

TS:   console.assert(x > 0);
来源：http://dc.yuexingan06.cn

Java: assert x > 0 : "必须为正";
来源：http://kr.chemitech.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xv.hahajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xb.hahajie.cn

C#:   Debug.Assert(x > 0);
来源：http://ac.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://fl.nicolike.cn

Py:   str(e);  traceback.format_exc()
来源：http://fe.yuntaijiaju.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ck.shxzskj.cn

JS:   e.message;  e.stack
来源：http://kq.shxzskj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tl.yuntaijiaju.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ty.shtwfgs.cn

Go:   err.Error()
来源：http://wp.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://ol.newstarts.cn

C#:   e.Message;  e.StackTrace
来源：http://iq.bjjhwx.cn

[H09] 带错误码的异常
来源：http://nr.yuntaijiaju.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hv.bookmarksfly.cn


<!-- 参考信息 -->