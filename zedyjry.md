代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://if.nszjky.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://te.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eu.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tz.shxzskj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pi.bookmarksfly.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://nc.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qn.521024.cn

[F08] 遍历目录
来源：http://pa.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qq.huixiangedu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ps.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://ke.jctech888.com.cn

TS:   fs.readdirSync("dir")
来源：http://kl.bookmarksfly.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gz.bookmarksfly.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xf.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://ne.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://jj.hahajie.cn

[F09] 获取文件大小
来源：http://ip.jianghongdianzi.cn

Py:   os.path.getsize("a.txt")
来源：http://ta.chemitech.net.cn

PHP:  filesize("a.txt");
来源：http://ul.muxihuayi.cn

JS:   fs.statSync("a.txt").size
来源：http://il.colortex.cn

TS:   fs.statSync("a.txt").size
来源：http://un.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hh.nicolike.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ck.shxzukj.cn

Ruby: File.size("a.txt")
来源：http://by.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://kp.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://hf.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zt.shtwfgs.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bk.wgjwhj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jz.521024.cn

TS:   path.extname("a.txt")
来源：http://hs.shxzukj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oa.bookmarksfly.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://er.newstarts.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://qb.huanxung.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ta.asd995.cn

[F11] 复制与移动文件
来源：http://rz.haigaiapp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://zi.jianghongdianzi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fx.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://re.muxihuayi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jd.panjiajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mj.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://be.hnjuh.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://al.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oi.yuntaijiaju.cn

[F12] CSV 读写
来源：http://hd.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mi.shxzukj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://no.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qp.huixinmuqiang.cn

TS:   // 同上
来源：http://cb.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wn.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vk.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zw.gzmigu.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lk.nszjky.cn

================================================================================
来源：http://cq.huixinmuqiang.cn

G. 面向对象
来源：http://oj.lnxyls.cn

================================================================================
来源：http://rw.yuexingan06.cn

[G01] 定义类
来源：http://ob.yuntaijiaju.cn

Py:   class User: pass
来源：http://zs.nszjky.cn

PHP:  class User {}
来源：http://nd.chemitech.net.cn

JS:   class User {}
来源：http://in.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://ji.shxzskj.cn

Java: class User {}
来源：http://nd.lnxyls.cn

Go:   type User struct { Name string }
来源：http://de.shxzukj.cn

Ruby: class User; end
来源：http://xd.chemitech.net.cn

C#:   class User {}
来源：http://tc.muxihuayi.cn

[G02] 构造函数
来源：http://fl.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://ru.lnxyls.cn

PHP:  public function __construct(public string $name) {}
来源：http://tl.bookmarksfly.cn

JS:   constructor(name) { this.name = name; }
来源：http://nn.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://nw.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://ji.huanxung.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://li.9csxet.cn

Ruby: def initialize(name); @name = name; end
来源：http://bf.hahajie.cn

C#:   public User(string name) { Name = name; }
来源：http://xs.gzmigu.cn

[G03] 实例属性
来源：http://db.gzmigu.cn

Py:   self.name = "x"
来源：http://ky.panjiajie.cn

PHP:  public string $name = "x";
来源：http://pq.chemitech.net.cn

JS:   this.name = "x";
来源：http://vt.panjiajie.cn

TS:   name: string = "x";
来源：http://ja.shxzskj.cn

Java: private String name;
来源：http://lf.colortex.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wi.bjjhwx.cn

Ruby: @name = "x"
来源：http://dd.nszjky.cn

C#:   public string Name { get; set; } = "x";
来源：http://ee.huanxung.cn

[G04] 定义方法
来源：http://pk.huixiangedu.cn

Py:   def greet(self): return self.name
来源：http://ko.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://th.lnxyls.cn

JS:   greet() { return this.name; }
来源：http://ac.bjjhwx.cn

TS:   greet(): string { return this.name; }
来源：http://en.huixiangedu.cn

Java: String greet() { return name; }
来源：http://pc.yuntaijiaju.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kd.hahajie.cn

Ruby: def greet; @name; end
来源：http://ky.huixiangedu.cn

C#:   public string Greet() => Name;
来源：http://ze.chemitech.net.cn

[G05] 继承
来源：http://ut.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://as.bjjhwx.cn

PHP:  class Admin extends User {}
来源：http://px.bookmarksfly.cn

JS:   class Admin extends User {}
来源：http://xn.nszjky.cn

TS:   class Admin extends User {}
来源：http://uj.bookmarksfly.cn

Java: class Admin extends User {}
来源：http://qj.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ss.jctech888.com.cn

Ruby: class Admin < User; end
来源：http://at.bjjhwx.cn

C#:   class Admin : User {}
来源：http://um.bjjhwx.cn

[G06] 重写方法
来源：http://id.haigaiapp.cn

Py:   def greet(self): return "admin"
来源：http://la.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ai.colortex.cn

JS:   greet() { return "admin"; }
来源：http://fx.chemitech.net.cn

TS:   greet(): string { return "admin"; }
来源：http://xx.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://zm.yuexingan06.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mz.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://sd.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://xn.nszjky.cn

[G07] 调用父类方法
来源：http://sk.gzmigu.cn

Py:   super().greet()
来源：http://ca.shxzskj.cn

PHP:  parent::greet();
来源：http://dh.wgjwhj.cn

JS:   super.greet();
来源：http://ma.shxzskj.cn

TS:   super.greet();
来源：http://lg.asd995.cn

Java: super.greet();
来源：http://lw.colortex.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cy.huixiangedu.cn

Ruby: super
来源：http://lh.bjjhwx.cn

C#:   base.Greet();
来源：http://ks.nszjky.cn

[G08] 静态方法与属性
来源：http://dc.yuexingan06.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://km.asd995.cn

PHP:  public static function f() {}
来源：http://nz.nszjky.cn

JS:   static f() {}
来源：http://xy.hahajie.cn

TS:   static f(): void {}
来源：http://rp.hahajie.cn

Java: static void f() {}
来源：http://da.wgjwhj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nr.hahajie.cn

Ruby: def self.f; end
来源：http://zf.chemitech.net.cn

C#:   public static void F() {}
来源：http://fp.shxzukj.cn

[G09] 接口 / 抽象类
来源：http://zy.szsharing.cn

Py:   from abc import ABC, abstractmethod
来源：http://ev.nszjky.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ya.wgjwhj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fw.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://wi.shtwfgs.cn

Java: interface Shape { double area(); }
来源：http://hw.huixiangedu.cn

Go:   type Shape interface { Area() float64 }
来源：http://ic.colortex.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mt.hnjuh.cn

C#:   interface IShape { double Area(); }
来源：http://bc.521024.cn

[G10] 访问控制
来源：http://pa.chemitech.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://fr.nszjky.cn

PHP:  public / protected / private
来源：http://sl.colortex.cn

JS:   #private 字段；其余公开
来源：http://ow.shxzskj.cn

TS:   public / protected / private
来源：http://vg.wgjwhj.cn

Java: public / protected / private / 默认包级
来源：http://vh.bjjhwx.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://in.9csxet.cn

Ruby: public / protected / private
来源：http://df.szxytkj.cn

C#:   public / protected / private / internal
来源：http://zi.jctech888.com.cn

[G11] getter / setter
来源：http://qk.nszjky.cn

Py:   @property 与 @x.setter
来源：http://in.asd995.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://aj.hahajie.cn

JS:   get name() { return this._name; }
来源：http://xp.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://ld.jctech888.com.cn

Java: public String getName() { return name; }
来源：http://ow.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://un.521024.cn

Ruby: attr_accessor :name
来源：http://iv.szsharing.cn

C#:   public string Name { get; set; }
来源：http://jm.lnxyls.cn

[G12] 对象转字符串
来源：http://en.hahajie.cn

Py:   def __str__(self): return self.name
来源：http://vg.521024.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sr.yuexingan06.cn

JS:   toString() { return this.name; }
来源：http://ef.huanxung.cn

TS:   toString(): string { return this.name; }
来源：http://vh.chemitech.net.cn

Java: @Override public String toString() { return name; }
来源：http://ze.yuexingan06.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jq.haigaiapp.cn

Ruby: def to_s; @name; end
来源：http://vk.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://hn.huanxung.cn

[G13] 判断对象类型
来源：http://es.huixiangedu.cn

Py:   isinstance(u, User)
来源：http://zh.hahajie.cn

PHP:  $u instanceof User
来源：http://sd.bjjhwx.cn

JS:   u instanceof User
来源：http://ab.hahajie.cn

TS:   u instanceof User
来源：http://gf.muxihuayi.cn

Java: u instanceof User
来源：http://ku.muxihuayi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://hd.yuntaijiaju.cn

C#:   u is User
来源：http://ny.colortex.cn

[G14] 数据类 / record
来源：http://fs.muxihuayi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://uv.yuntaijiaju.cn

PHP:  // 用 readonly 属性模拟
来源：http://xu.hnjuh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fu.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://gf.521024.cn

Java: record User(String name, int age) {}
来源：http://dd.colortex.cn

Go:   type User struct { Name string; Age int }
来源：http://dc.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rd.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://hd.szxytkj.cn

[G15] 枚举
来源：http://fm.lnxyls.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://os.chemitech.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gw.colortex.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zm.colortex.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mp.shxzskj.cn

Java: enum Color { RED, GREEN }
来源：http://ip.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lq.wgjwhj.cn

Ruby: Color = %i[red green].freeze
来源：http://fi.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kh.shxzukj.cn

[G16] 对象转数组 / 字典
来源：http://aj.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ey.gzmigu.cn

PHP:  get_object_vars($obj);
来源：http://wj.bjjhwx.cn

JS:   Object.entries(obj)
来源：http://sa.chemitech.net.cn

TS:   Object.entries(obj)
来源：http://mz.hnjuh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rn.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://aq.nszjky.cn

Ruby: obj.instance_variables
来源：http://ec.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://xk.szxytkj.cn

================================================================================
来源：http://pe.hahajie.cn

H. 异常与错误处理
来源：http://xl.9csxet.cn

================================================================================
来源：http://ru.hahajie.cn

[H01] try / catch 基础
来源：http://zl.szsharing.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dx.muxihuayi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vy.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://un.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mb.9csxet.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xk.nszjky.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ye.yuexingan06.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gw.haigaiapp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ni.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://jg.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ic.panjiajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fj.shxzukj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bg.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ow.huixinmuqiang.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rb.jctech888.com.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nr.szsharing.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bi.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dw.bjjhwx.cn

[H03] 主动抛出异常
来源：http://qj.hnjuh.cn

Py:   raise ValueError("错误信息")
来源：http://lg.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wk.shtwfgs.cn

JS:   throw new Error("错误信息");
来源：http://cg.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://sd.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gb.colortex.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://au.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ro.wgjwhj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://er.asd995.cn

[H04] 自定义异常类型
来源：http://si.szsharing.cn

Py:   class MyError(Exception): pass
来源：http://md.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://id.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://li.chemitech.net.cn

TS:   class MyError extends Error {}
来源：http://uh.jianghongdianzi.cn

Java: class MyException extends RuntimeException {}
来源：http://qi.9csxet.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qy.yuntaijiaju.cn

Ruby: class MyError < StandardError; end
来源：http://in.bjjhwx.cn

C#:   class MyException : Exception {}
来源：http://wo.bookmarksfly.cn

[H05] 捕获特定类型
来源：http://vl.nszjky.cn

Py:   except ValueError as e:
来源：http://oe.huanxung.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yp.colortex.cn

JS:   if (e instanceof TypeError) {}
来源：http://mi.huanxung.cn

TS:   if (e instanceof TypeError) {}
来源：http://eu.9csxet.cn

Java: catch (IOException | SQLException e) {}
来源：http://kb.haigaiapp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://iw.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://ko.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ei.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://mi.haigaiapp.cn

Py:   value = d.get("k") or default
来源：http://jd.hnjuh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kb.bjjhwx.cn

JS:   obj?.a?.b;  d ?? default
来源：http://aq.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ue.hahajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://od.chemitech.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qy.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://tc.nszjky.cn

C#:   obj?.A?.B ?? default
来源：http://ue.nicolike.cn

[H07] 断言
来源：http://qu.asd995.cn

Py:   assert x > 0, "必须为正"
来源：http://yx.newstarts.cn

PHP:  assert($x > 0);
来源：http://bi.nicolike.cn

JS:   console.assert(x > 0);
来源：http://vg.hnjuh.cn

TS:   console.assert(x > 0);
来源：http://wi.lnxyls.cn

Java: assert x > 0 : "必须为正";
来源：http://ay.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ux.shtwfgs.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ih.bjjhwx.cn

C#:   Debug.Assert(x > 0);
来源：http://ik.newstarts.cn

[H08] 获取错误信息与堆栈
来源：http://pi.nicolike.cn

Py:   str(e);  traceback.format_exc()
来源：http://gk.shxzukj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sl.nicolike.cn

JS:   e.message;  e.stack
来源：http://br.yuntaijiaju.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dc.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dx.jctech888.com.cn

Go:   err.Error()
来源：http://xj.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://gr.shxzukj.cn

C#:   e.Message;  e.StackTrace
来源：http://dp.shxzskj.cn

[H09] 带错误码的异常
来源：http://vz.huixinmuqiang.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xz.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://oz.jianghongdianzi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fg.panjiajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bv.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jt.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bb.yuntaijiaju.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wx.lnxyls.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ur.521024.cn

[H10] 资源自动释放
来源：http://rx.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mu.szsharing.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fj.9csxet.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://no.hahajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ze.9csxet.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hd.gzmigu.cn

Go:   defer f.Close()
来源：http://sk.newstarts.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ig.huixinmuqiang.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://js.shtwfgs.cn

================================================================================
来源：http://fz.huixiangedu.cn

I. 正则表达式
来源：http://vm.huixinmuqiang.cn

================================================================================
来源：http://ua.huixinmuqiang.cn

[I01] 判断是否匹配
来源：http://ge.colortex.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tp.huixiangedu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://eh.colortex.cn

JS:   /\d+/.test(s)
来源：http://ov.chemitech.net.cn

TS:   /\d+/.test(s)
来源：http://nd.gzmigu.cn


<!-- 参考信息 -->