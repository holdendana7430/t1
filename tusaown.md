代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jq.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jq.bjjhwx.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ff.asd995.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://co.yuntaijiaju.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sf.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://kz.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wl.gzmigu.cn

[F08] 遍历目录
来源：http://tu.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yk.wgjwhj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ge.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://cg.lnxyls.cn

TS:   fs.readdirSync("dir")
来源：http://pc.muxihuayi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://pr.gzmigu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://zb.huixinmuqiang.cn

Ruby: Dir.children("dir")
来源：http://iy.521024.cn

C#:   Directory.GetFiles("dir")
来源：http://wi.shtwfgs.cn

[F09] 获取文件大小
来源：http://aq.nicolike.cn

Py:   os.path.getsize("a.txt")
来源：http://pd.lnxyls.cn

PHP:  filesize("a.txt");
来源：http://xa.asd995.cn

JS:   fs.statSync("a.txt").size
来源：http://ic.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://ay.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sn.yuexingan06.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ek.muxihuayi.cn

Ruby: File.size("a.txt")
来源：http://sp.nszjky.cn

C#:   new FileInfo("a.txt").Length
来源：http://jf.wgjwhj.cn

[F10] 取文件扩展名 / 文件名
来源：http://lg.bjjhwx.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wc.panjiajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ws.hahajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rp.shxzukj.cn

TS:   path.extname("a.txt")
来源：http://wa.hahajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qj.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vk.yuexingan06.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ip.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ex.huixiangedu.cn

[F11] 复制与移动文件
来源：http://mz.lnxyls.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vl.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://su.szsharing.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fb.muxihuayi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rc.yuexingan06.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jp.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://et.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ys.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qd.haigaiapp.cn

[F12] CSV 读写
来源：http://fb.asd995.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ty.9csxet.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ah.9csxet.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ay.panjiajie.cn

TS:   // 同上
来源：http://yn.muxihuayi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wn.bjjhwx.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ip.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://in.9csxet.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zp.nszjky.cn

================================================================================
来源：http://me.szsharing.cn

G. 面向对象
来源：http://jq.nicolike.cn

================================================================================
来源：http://bx.hnjuh.cn

[G01] 定义类
来源：http://vq.bjjhwx.cn

Py:   class User: pass
来源：http://fm.nicolike.cn

PHP:  class User {}
来源：http://oa.lnxyls.cn

JS:   class User {}
来源：http://tp.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://xs.shxzukj.cn

Java: class User {}
来源：http://xx.wgjwhj.cn

Go:   type User struct { Name string }
来源：http://us.lnxyls.cn

Ruby: class User; end
来源：http://my.asd995.cn

C#:   class User {}
来源：http://ba.bjjhwx.cn

[G02] 构造函数
来源：http://yq.muxihuayi.cn

Py:   def __init__(self, name): self.name = name
来源：http://wv.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://uw.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://vw.hahajie.cn

TS:   constructor(public name: string) {}
来源：http://on.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://an.jianghongdianzi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://my.szsharing.cn

Ruby: def initialize(name); @name = name; end
来源：http://qp.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://pk.bjjhwx.cn

[G03] 实例属性
来源：http://hw.huixiangedu.cn

Py:   self.name = "x"
来源：http://nu.nszjky.cn

PHP:  public string $name = "x";
来源：http://ux.bjjhwx.cn

JS:   this.name = "x";
来源：http://mr.colortex.cn

TS:   name: string = "x";
来源：http://uq.nszjky.cn

Java: private String name;
来源：http://zh.szxytkj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nj.9csxet.cn

Ruby: @name = "x"
来源：http://dk.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://er.panjiajie.cn

[G04] 定义方法
来源：http://rk.nicolike.cn

Py:   def greet(self): return self.name
来源：http://nf.9csxet.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nw.asd995.cn

JS:   greet() { return this.name; }
来源：http://zl.chemitech.net.cn

TS:   greet(): string { return this.name; }
来源：http://qd.newstarts.cn

Java: String greet() { return name; }
来源：http://hx.nicolike.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gu.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://gh.9csxet.cn

C#:   public string Greet() => Name;
来源：http://hn.shxzukj.cn

[G05] 继承
来源：http://ng.bjjhwx.cn

Py:   class Admin(User): pass
来源：http://ac.521024.cn

PHP:  class Admin extends User {}
来源：http://nh.asd995.cn

JS:   class Admin extends User {}
来源：http://dl.panjiajie.cn

TS:   class Admin extends User {}
来源：http://cb.bjjhwx.cn

Java: class Admin extends User {}
来源：http://cv.huixinmuqiang.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xx.shxzukj.cn

Ruby: class Admin < User; end
来源：http://ef.colortex.cn

C#:   class Admin : User {}
来源：http://hh.huixinmuqiang.cn

[G06] 重写方法
来源：http://ph.bookmarksfly.cn

Py:   def greet(self): return "admin"
来源：http://or.hahajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://np.haigaiapp.cn

JS:   greet() { return "admin"; }
来源：http://ck.hnjuh.cn

TS:   greet(): string { return "admin"; }
来源：http://oi.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://rk.huanxung.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ez.colortex.cn

Ruby: def greet; "admin"; end
来源：http://wq.panjiajie.cn

C#:   public override string Greet() => "admin";
来源：http://ve.bjjhwx.cn

[G07] 调用父类方法
来源：http://gh.chemitech.net.cn

Py:   super().greet()
来源：http://es.hahajie.cn

PHP:  parent::greet();
来源：http://sh.szsharing.cn

JS:   super.greet();
来源：http://hv.9csxet.cn

TS:   super.greet();
来源：http://ji.haigaiapp.cn

Java: super.greet();
来源：http://fq.colortex.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pz.jctech888.com.cn

Ruby: super
来源：http://gr.asd995.cn

C#:   base.Greet();
来源：http://tn.nicolike.cn

[G08] 静态方法与属性
来源：http://pp.jianghongdianzi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://we.9csxet.cn

PHP:  public static function f() {}
来源：http://bz.shxzskj.cn

JS:   static f() {}
来源：http://zq.haigaiapp.cn

TS:   static f(): void {}
来源：http://oe.shxzukj.cn

Java: static void f() {}
来源：http://yn.huixiangedu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rn.panjiajie.cn

Ruby: def self.f; end
来源：http://tv.yuexingan06.cn

C#:   public static void F() {}
来源：http://oh.chemitech.net.cn

[G09] 接口 / 抽象类
来源：http://cb.bookmarksfly.cn

Py:   from abc import ABC, abstractmethod
来源：http://cx.yuexingan06.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gz.nicolike.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yuntaijiaju.cn

TS:   interface Shape { area(): number; }
来源：http://md.jianghongdianzi.cn

Java: interface Shape { double area(); }
来源：http://wa.huanxung.cn

Go:   type Shape interface { Area() float64 }
来源：http://as.newstarts.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yk.asd995.cn

C#:   interface IShape { double Area(); }
来源：http://mg.huanxung.cn

[G10] 访问控制
来源：http://ib.bookmarksfly.cn

Py:   约定 _protected / __private（不强制）
来源：http://cd.yuexingan06.cn

PHP:  public / protected / private
来源：http://ov.newstarts.cn

JS:   #private 字段；其余公开
来源：http://gq.shxzskj.cn

TS:   public / protected / private
来源：http://sj.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://lr.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://og.haigaiapp.cn

Ruby: public / protected / private
来源：http://za.lnxyls.cn

C#:   public / protected / private / internal
来源：http://pt.szxytkj.cn

[G11] getter / setter
来源：http://vn.hahajie.cn

Py:   @property 与 @x.setter
来源：http://vv.newstarts.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ol.yuntaijiaju.cn

JS:   get name() { return this._name; }
来源：http://dl.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://pm.521024.cn

Java: public String getName() { return name; }
来源：http://lj.chemitech.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nx.yuntaijiaju.cn

Ruby: attr_accessor :name
来源：http://kk.hahajie.cn

C#:   public string Name { get; set; }
来源：http://ug.hnjuh.cn

[G12] 对象转字符串
来源：http://da.asd995.cn

Py:   def __str__(self): return self.name
来源：http://ey.muxihuayi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lv.huixinmuqiang.cn

JS:   toString() { return this.name; }
来源：http://jc.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://pi.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://vn.yuexingan06.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gv.szsharing.cn

Ruby: def to_s; @name; end
来源：http://kx.newstarts.cn

C#:   public override string ToString() => Name;
来源：http://oc.yuexingan06.cn

[G13] 判断对象类型
来源：http://yx.colortex.cn

Py:   isinstance(u, User)
来源：http://we.huixinmuqiang.cn

PHP:  $u instanceof User
来源：http://fe.szsharing.cn

JS:   u instanceof User
来源：http://bc.colortex.cn

TS:   u instanceof User
来源：http://dk.9csxet.cn

Java: u instanceof User
来源：http://je.szxytkj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ec.yuntaijiaju.cn

Ruby: u.is_a?(User)
来源：http://fg.hnjuh.cn

C#:   u is User
来源：http://bo.bookmarksfly.cn

[G14] 数据类 / record
来源：http://oa.bjjhwx.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yb.9csxet.cn

PHP:  // 用 readonly 属性模拟
来源：http://gt.hahajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://me.newstarts.cn

TS:   type User = { name: string; age: number };
来源：http://ia.huixiangedu.cn

Java: record User(String name, int age) {}
来源：http://ow.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://uu.gzmigu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xo.521024.cn

C#:   record User(string Name, int Age);
来源：http://mb.521024.cn

[G15] 枚举
来源：http://uy.shtwfgs.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://et.shxzskj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mk.haigaiapp.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dl.muxihuayi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yf.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://yg.bjjhwx.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xr.colortex.cn

Ruby: Color = %i[red green].freeze
来源：http://xq.bookmarksfly.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gv.hahajie.cn

[G16] 对象转数组 / 字典
来源：http://uu.gzmigu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wq.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://mq.shxzukj.cn

JS:   Object.entries(obj)
来源：http://zs.haigaiapp.cn

TS:   Object.entries(obj)
来源：http://iw.wgjwhj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xx.9csxet.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wf.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://dt.asd995.cn

C#:   // 用反射或 System.Text.Json
来源：http://pk.jctech888.com.cn

================================================================================
来源：http://qc.bjjhwx.cn

H. 异常与错误处理
来源：http://qr.gzmigu.cn

================================================================================
来源：http://ys.shtwfgs.cn

[H01] try / catch 基础
来源：http://qd.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lt.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lj.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://em.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ec.huanxung.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://go.asd995.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://go.szsharing.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gx.asd995.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zv.szsharing.cn

[H02] finally / ensure 收尾
来源：http://vg.huanxung.cn

Py:   try: f()⏎finally: cleanup()
来源：http://im.9csxet.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://eu.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rg.chemitech.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zx.muxihuayi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gz.lnxyls.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ua.jianghongdianzi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wh.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cq.bjjhwx.cn

[H03] 主动抛出异常
来源：http://ye.muxihuayi.cn

Py:   raise ValueError("错误信息")
来源：http://rj.yuexingan06.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qo.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://xj.hahajie.cn

TS:   throw new Error("错误信息");
来源：http://gj.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vp.gzmigu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://po.bookmarksfly.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ka.jianghongdianzi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://db.shxzukj.cn

[H04] 自定义异常类型
来源：http://ad.nicolike.cn

Py:   class MyError(Exception): pass
来源：http://um.bookmarksfly.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dl.shxzukj.cn

JS:   class MyError extends Error {}
来源：http://il.asd995.cn

TS:   class MyError extends Error {}
来源：http://rq.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://zo.shxzskj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gu.bjjhwx.cn

Ruby: class MyError < StandardError; end
来源：http://gi.nicolike.cn

C#:   class MyException : Exception {}
来源：http://vd.muxihuayi.cn

[H05] 捕获特定类型
来源：http://ts.shtwfgs.cn

Py:   except ValueError as e:
来源：http://me.nicolike.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hj.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://zz.hahajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://rw.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://od.gzmigu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bz.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://oq.bjjhwx.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sa.haigaiapp.cn

[H06] 可选值 / 空值安全访问
来源：http://jq.nszjky.cn

Py:   value = d.get("k") or default
来源：http://vo.gzmigu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wy.bookmarksfly.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rg.shtwfgs.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zc.wgjwhj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cz.szsharing.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hn.newstarts.cn

Ruby: d&.dig(:a, :b)
来源：http://qz.huixiangedu.cn

C#:   obj?.A?.B ?? default
来源：http://an.lnxyls.cn

[H07] 断言
来源：http://vq.jianghongdianzi.cn

Py:   assert x > 0, "必须为正"
来源：http://fj.huixinmuqiang.cn

PHP:  assert($x > 0);
来源：http://nu.yuexingan06.cn

JS:   console.assert(x > 0);
来源：http://mi.wgjwhj.cn

TS:   console.assert(x > 0);
来源：http://pw.9csxet.cn

Java: assert x > 0 : "必须为正";
来源：http://ko.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sx.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://as.bookmarksfly.cn

C#:   Debug.Assert(x > 0);
来源：http://mg.jctech888.com.cn

[H08] 获取错误信息与堆栈
来源：http://at.szsharing.cn

Py:   str(e);  traceback.format_exc()
来源：http://xw.shtwfgs.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nv.huixinmuqiang.cn

JS:   e.message;  e.stack
来源：http://vn.panjiajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rv.newstarts.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ve.hahajie.cn

Go:   err.Error()
来源：http://xj.yuntaijiaju.cn

Ruby: e.message;  e.backtrace
来源：http://bc.jianghongdianzi.cn

C#:   e.Message;  e.StackTrace
来源：http://rc.hahajie.cn

[H09] 带错误码的异常
来源：http://ca.chemitech.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yj.shxzukj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xd.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hg.nicolike.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://oj.bjjhwx.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zq.huixinmuqiang.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ta.colortex.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kj.hnjuh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://td.9csxet.cn

[H10] 资源自动释放
来源：http://yl.nszjky.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ef.jctech888.com.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ci.9csxet.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dx.bookmarksfly.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ok.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sp.bjjhwx.cn

Go:   defer f.Close()
来源：http://qv.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bj.colortex.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rp.huanxung.cn

================================================================================
来源：http://nr.nszjky.cn

I. 正则表达式
来源：http://wh.9csxet.cn

================================================================================
来源：http://dd.muxihuayi.cn

[I01] 判断是否匹配
来源：http://mu.huixinmuqiang.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sh.9csxet.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ls.szsharing.cn

JS:   /\d+/.test(s)
来源：http://ez.9csxet.cn

TS:   /\d+/.test(s)
来源：http://bz.nszjky.cn


<!-- 参考信息 -->