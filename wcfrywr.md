代发 wailian999

C#:   File.Exists("a.txt")
来源：http://jd.shxzskj.cn

[F06] 删除文件
来源：http://ua.nicolike.cn

Py:   os.remove("a.txt")
来源：http://fb.huanxung.cn

PHP:  unlink("a.txt");
来源：http://rq.nicolike.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ce.newstarts.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lp.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://so.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://xi.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://fg.szsharing.cn

C#:   File.Delete("a.txt");
来源：http://ib.wgjwhj.cn

[F07] 创建目录（含多级）
来源：http://nl.jianghongdianzi.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rr.huixiangedu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://us.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xo.bjjhwx.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ha.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://at.szsharing.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://eo.colortex.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zw.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ze.haigaiapp.cn

[F08] 遍历目录
来源：http://ru.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hl.wgjwhj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ww.hahajie.cn

JS:   fs.readdirSync("dir")
来源：http://jy.asd995.cn

TS:   fs.readdirSync("dir")
来源：http://vr.nicolike.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ok.huixiangedu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nq.huixinmuqiang.cn

Ruby: Dir.children("dir")
来源：http://es.colortex.cn

C#:   Directory.GetFiles("dir")
来源：http://ak.shxzukj.cn

[F09] 获取文件大小
来源：http://cj.hnjuh.cn

Py:   os.path.getsize("a.txt")
来源：http://hh.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://hk.hnjuh.cn

JS:   fs.statSync("a.txt").size
来源：http://sb.haigaiapp.cn

TS:   fs.statSync("a.txt").size
来源：http://wm.yuexingan06.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vm.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ju.chemitech.net.cn

Ruby: File.size("a.txt")
来源：http://yq.gzmigu.cn

C#:   new FileInfo("a.txt").Length
来源：http://xb.haigaiapp.cn

[F10] 取文件扩展名 / 文件名
来源：http://si.lnxyls.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wq.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vv.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ji.wgjwhj.cn

TS:   path.extname("a.txt")
来源：http://mw.jianghongdianzi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://gj.szxytkj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://al.panjiajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://is.nszjky.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ra.chemitech.net.cn

[F11] 复制与移动文件
来源：http://ro.colortex.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://tm.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://me.yuntaijiaju.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zg.haigaiapp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yi.chemitech.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ko.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bd.asd995.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pr.szsharing.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tq.yuexingan06.cn

[F12] CSV 读写
来源：http://gg.panjiajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ee.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://li.jctech888.com.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://da.huixinmuqiang.cn

TS:   // 同上
来源：http://mp.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://re.bookmarksfly.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vz.panjiajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zs.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://og.shxzukj.cn

================================================================================
来源：http://oi.lnxyls.cn

G. 面向对象
来源：http://vd.nszjky.cn

================================================================================
来源：http://kt.nicolike.cn

[G01] 定义类
来源：http://td.nszjky.cn

Py:   class User: pass
来源：http://xh.wgjwhj.cn

PHP:  class User {}
来源：http://zi.huixinmuqiang.cn

JS:   class User {}
来源：http://ep.colortex.cn

TS:   class User { name: string = ""; }
来源：http://xx.shxzskj.cn

Java: class User {}
来源：http://sm.hnjuh.cn

Go:   type User struct { Name string }
来源：http://xi.bjjhwx.cn

Ruby: class User; end
来源：http://vf.szxytkj.cn

C#:   class User {}
来源：http://nv.yuexingan06.cn

[G02] 构造函数
来源：http://lr.chemitech.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://yk.gzmigu.cn

PHP:  public function __construct(public string $name) {}
来源：http://fv.jctech888.com.cn

JS:   constructor(name) { this.name = name; }
来源：http://ft.lnxyls.cn

TS:   constructor(public name: string) {}
来源：http://bt.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://mw.jianghongdianzi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://jv.huanxung.cn

Ruby: def initialize(name); @name = name; end
来源：http://hc.nszjky.cn

C#:   public User(string name) { Name = name; }
来源：http://va.jctech888.com.cn

[G03] 实例属性
来源：http://hu.521024.cn

Py:   self.name = "x"
来源：http://uv.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://ej.colortex.cn

JS:   this.name = "x";
来源：http://sx.shxzukj.cn

TS:   name: string = "x";
来源：http://cx.huixiangedu.cn

Java: private String name;
来源：http://ng.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ji.gzmigu.cn

Ruby: @name = "x"
来源：http://ti.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://hv.newstarts.cn

[G04] 定义方法
来源：http://re.bjjhwx.cn

Py:   def greet(self): return self.name
来源：http://xw.lnxyls.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://md.panjiajie.cn

JS:   greet() { return this.name; }
来源：http://sj.jctech888.com.cn

TS:   greet(): string { return this.name; }
来源：http://wh.nszjky.cn

Java: String greet() { return name; }
来源：http://dx.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vp.asd995.cn

Ruby: def greet; @name; end
来源：http://qs.huanxung.cn

C#:   public string Greet() => Name;
来源：http://hn.jianghongdianzi.cn

[G05] 继承
来源：http://vz.newstarts.cn

Py:   class Admin(User): pass
来源：http://rq.wgjwhj.cn

PHP:  class Admin extends User {}
来源：http://dx.huixinmuqiang.cn

JS:   class Admin extends User {}
来源：http://yu.521024.cn

TS:   class Admin extends User {}
来源：http://em.lnxyls.cn

Java: class Admin extends User {}
来源：http://vz.nszjky.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dh.szsharing.cn

Ruby: class Admin < User; end
来源：http://bx.shxzukj.cn

C#:   class Admin : User {}
来源：http://et.haigaiapp.cn

[G06] 重写方法
来源：http://qh.szsharing.cn

Py:   def greet(self): return "admin"
来源：http://wo.bookmarksfly.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hc.nicolike.cn

JS:   greet() { return "admin"; }
来源：http://cx.haigaiapp.cn

TS:   greet(): string { return "admin"; }
来源：http://ev.szxytkj.cn

Java: @Override String greet() { return "admin"; }
来源：http://ae.huixinmuqiang.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lp.lnxyls.cn

Ruby: def greet; "admin"; end
来源：http://qo.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://vp.shxzukj.cn

[G07] 调用父类方法
来源：http://hk.9csxet.cn

Py:   super().greet()
来源：http://wb.newstarts.cn

PHP:  parent::greet();
来源：http://vt.hnjuh.cn

JS:   super.greet();
来源：http://ec.bjjhwx.cn

TS:   super.greet();
来源：http://if.szxytkj.cn

Java: super.greet();
来源：http://ia.bjjhwx.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zt.shtwfgs.cn

Ruby: super
来源：http://nv.bjjhwx.cn

C#:   base.Greet();
来源：http://lw.szsharing.cn

[G08] 静态方法与属性
来源：http://pe.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vl.gzmigu.cn

PHP:  public static function f() {}
来源：http://qz.gzmigu.cn

JS:   static f() {}
来源：http://xq.bjjhwx.cn

TS:   static f(): void {}
来源：http://xj.colortex.cn

Java: static void f() {}
来源：http://kp.haigaiapp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fb.huixiangedu.cn

Ruby: def self.f; end
来源：http://co.bjjhwx.cn

C#:   public static void F() {}
来源：http://cx.huixinmuqiang.cn

[G09] 接口 / 抽象类
来源：http://ao.yuexingan06.cn

Py:   from abc import ABC, abstractmethod
来源：http://hy.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://la.huixiangedu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yo.lnxyls.cn

TS:   interface Shape { area(): number; }
来源：http://uu.521024.cn

Java: interface Shape { double area(); }
来源：http://cu.huanxung.cn

Go:   type Shape interface { Area() float64 }
来源：http://dk.panjiajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sz.haigaiapp.cn

C#:   interface IShape { double Area(); }
来源：http://gm.muxihuayi.cn

[G10] 访问控制
来源：http://qj.wgjwhj.cn

Py:   约定 _protected / __private（不强制）
来源：http://di.9csxet.cn

PHP:  public / protected / private
来源：http://yg.colortex.cn

JS:   #private 字段；其余公开
来源：http://sx.yuntaijiaju.cn

TS:   public / protected / private
来源：http://ze.yuntaijiaju.cn

Java: public / protected / private / 默认包级
来源：http://xx.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rl.bjjhwx.cn

Ruby: public / protected / private
来源：http://kk.huixiangedu.cn

C#:   public / protected / private / internal
来源：http://dh.szsharing.cn

[G11] getter / setter
来源：http://fi.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://mn.shxzukj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yx.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://dm.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://kn.521024.cn

Java: public String getName() { return name; }
来源：http://ru.muxihuayi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cx.shtwfgs.cn

Ruby: attr_accessor :name
来源：http://mc.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://ym.panjiajie.cn

[G12] 对象转字符串
来源：http://je.521024.cn

Py:   def __str__(self): return self.name
来源：http://bp.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xs.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://bf.szsharing.cn

TS:   toString(): string { return this.name; }
来源：http://jc.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://xj.colortex.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wz.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://oi.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://vh.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://ck.shxzukj.cn

Py:   isinstance(u, User)
来源：http://og.bookmarksfly.cn

PHP:  $u instanceof User
来源：http://pf.lnxyls.cn

JS:   u instanceof User
来源：http://mr.jianghongdianzi.cn

TS:   u instanceof User
来源：http://iw.asd995.cn

Java: u instanceof User
来源：http://ce.muxihuayi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wj.lnxyls.cn

Ruby: u.is_a?(User)
来源：http://zs.panjiajie.cn

C#:   u is User
来源：http://xt.szxytkj.cn

[G14] 数据类 / record
来源：http://sd.huixinmuqiang.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sh.lnxyls.cn

PHP:  // 用 readonly 属性模拟
来源：http://ap.chemitech.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gw.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://vc.szxytkj.cn

Java: record User(String name, int age) {}
来源：http://fg.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://sn.newstarts.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fb.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://kq.yuntaijiaju.cn

[G15] 枚举
来源：http://pt.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ds.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ak.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fi.wgjwhj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pm.gzmigu.cn

Java: enum Color { RED, GREEN }
来源：http://lq.huixiangedu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lu.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://wj.yuexingan06.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nt.shxzskj.cn

[G16] 对象转数组 / 字典
来源：http://qp.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tb.gzmigu.cn

PHP:  get_object_vars($obj);
来源：http://oj.lnxyls.cn

JS:   Object.entries(obj)
来源：http://ep.nicolike.cn

TS:   Object.entries(obj)
来源：http://mi.jctech888.com.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://af.colortex.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wk.shtwfgs.cn

Ruby: obj.instance_variables
来源：http://su.asd995.cn

C#:   // 用反射或 System.Text.Json
来源：http://gs.asd995.cn

================================================================================
来源：http://fr.huixiangedu.cn

H. 异常与错误处理
来源：http://rv.haigaiapp.cn

================================================================================
来源：http://vi.gzmigu.cn

[H01] try / catch 基础
来源：http://ak.colortex.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dv.huixinmuqiang.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vq.muxihuayi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gl.hahajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sp.gzmigu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sr.szxytkj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ug.huixiangedu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dr.szsharing.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vx.newstarts.cn

[H02] finally / ensure 收尾
来源：http://qc.huixiangedu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xe.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nj.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kz.szsharing.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fg.yuexingan06.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rd.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mg.muxihuayi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ih.huixinmuqiang.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yu.9csxet.cn

[H03] 主动抛出异常
来源：http://hj.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://ti.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gz.yuexingan06.cn

JS:   throw new Error("错误信息");
来源：http://ji.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://sa.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gj.wgjwhj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dg.bjjhwx.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gr.yuexingan06.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xk.521024.cn

[H04] 自定义异常类型
来源：http://np.szsharing.cn

Py:   class MyError(Exception): pass
来源：http://rm.bookmarksfly.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sg.bjjhwx.cn

JS:   class MyError extends Error {}
来源：http://aq.yuntaijiaju.cn

TS:   class MyError extends Error {}
来源：http://di.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://ni.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ei.hahajie.cn

Ruby: class MyError < StandardError; end
来源：http://kq.wgjwhj.cn

C#:   class MyException : Exception {}
来源：http://xz.haigaiapp.cn

[H05] 捕获特定类型
来源：http://vr.bjjhwx.cn

Py:   except ValueError as e:
来源：http://sd.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oh.szxytkj.cn

JS:   if (e instanceof TypeError) {}
来源：http://yd.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://gn.newstarts.cn

Java: catch (IOException | SQLException e) {}
来源：http://ip.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mq.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://kz.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ey.9csxet.cn

[H06] 可选值 / 空值安全访问
来源：http://fs.yuexingan06.cn

Py:   value = d.get("k") or default
来源：http://bk.asd995.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mf.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nt.huixinmuqiang.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vp.asd995.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nm.hahajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nq.nszjky.cn

Ruby: d&.dig(:a, :b)
来源：http://co.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://md.hnjuh.cn

[H07] 断言
来源：http://od.jctech888.com.cn

Py:   assert x > 0, "必须为正"
来源：http://xm.shxzskj.cn

PHP:  assert($x > 0);
来源：http://tb.521024.cn

JS:   console.assert(x > 0);
来源：http://ia.shxzskj.cn

TS:   console.assert(x > 0);
来源：http://wp.gzmigu.cn

Java: assert x > 0 : "必须为正";
来源：http://jm.yuntaijiaju.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mb.yuexingan06.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hc.huixinmuqiang.cn

C#:   Debug.Assert(x > 0);
来源：http://wj.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://uf.haigaiapp.cn

Py:   str(e);  traceback.format_exc()
来源：http://in.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://we.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://fo.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://oa.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jx.9csxet.cn

Go:   err.Error()
来源：http://nv.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://so.nszjky.cn

C#:   e.Message;  e.StackTrace
来源：http://ep.yuntaijiaju.cn

[H09] 带错误码的异常
来源：http://ri.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ad.bjjhwx.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mx.huanxung.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ts.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://oa.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pn.huixiangedu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ve.bjjhwx.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xr.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zs.shxzskj.cn

[H10] 资源自动释放
来源：http://dv.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mc.jctech888.com.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nd.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ft.shtwfgs.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hi.jianghongdianzi.cn


<!-- 参考信息 -->