代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uy.jctech888.com.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://bu.shxzskj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yx.nicolike.cn

[F08] 遍历目录
来源：http://nw.panjiajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ca.huixinmuqiang.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yt.bjjhwx.cn

JS:   fs.readdirSync("dir")
来源：http://ep.9csxet.cn

TS:   fs.readdirSync("dir")
来源：http://nz.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tf.jianghongdianzi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://oj.huixiangedu.cn

Ruby: Dir.children("dir")
来源：http://xo.bookmarksfly.cn

C#:   Directory.GetFiles("dir")
来源：http://pq.panjiajie.cn

[F09] 获取文件大小
来源：http://bo.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://eo.9csxet.cn

PHP:  filesize("a.txt");
来源：http://fb.hahajie.cn

JS:   fs.statSync("a.txt").size
来源：http://tn.9csxet.cn

TS:   fs.statSync("a.txt").size
来源：http://bj.shtwfgs.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wi.szxytkj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ts.bjjhwx.cn

Ruby: File.size("a.txt")
来源：http://tw.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://ax.huixinmuqiang.cn

[F10] 取文件扩展名 / 文件名
来源：http://uw.huixiangedu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ij.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ze.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://nb.colortex.cn

TS:   path.extname("a.txt")
来源：http://kp.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://lj.chemitech.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yi.nszjky.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dl.jianghongdianzi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qy.nszjky.cn

[F11] 复制与移动文件
来源：http://oy.colortex.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dx.newstarts.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rg.yuexingan06.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wr.yuexingan06.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://es.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jt.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://di.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sw.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://zw.jctech888.com.cn

[F12] CSV 读写
来源：http://ii.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://er.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pp.hnjuh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wk.panjiajie.cn

TS:   // 同上
来源：http://vk.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qw.jctech888.com.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fk.hahajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cl.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://od.asd995.cn

================================================================================
来源：http://pq.jctech888.com.cn

G. 面向对象
来源：http://gj.nszjky.cn

================================================================================
来源：http://ng.asd995.cn

[G01] 定义类
来源：http://kv.haigaiapp.cn

Py:   class User: pass
来源：http://uo.panjiajie.cn

PHP:  class User {}
来源：http://kn.muxihuayi.cn

JS:   class User {}
来源：http://gh.huixiangedu.cn

TS:   class User { name: string = ""; }
来源：http://xp.jctech888.com.cn

Java: class User {}
来源：http://is.nicolike.cn

Go:   type User struct { Name string }
来源：http://wj.szxytkj.cn

Ruby: class User; end
来源：http://fk.521024.cn

C#:   class User {}
来源：http://yb.panjiajie.cn

[G02] 构造函数
来源：http://hd.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://ax.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://le.nszjky.cn

JS:   constructor(name) { this.name = name; }
来源：http://ge.nszjky.cn

TS:   constructor(public name: string) {}
来源：http://jn.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://ea.yuexingan06.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ui.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://we.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://hq.wgjwhj.cn

[G03] 实例属性
来源：http://lw.shtwfgs.cn

Py:   self.name = "x"
来源：http://vz.9csxet.cn

PHP:  public string $name = "x";
来源：http://ym.9csxet.cn

JS:   this.name = "x";
来源：http://ar.haigaiapp.cn

TS:   name: string = "x";
来源：http://lc.shxzskj.cn

Java: private String name;
来源：http://om.gzmigu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jy.szsharing.cn

Ruby: @name = "x"
来源：http://hn.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://yb.jctech888.com.cn

[G04] 定义方法
来源：http://sg.gzmigu.cn

Py:   def greet(self): return self.name
来源：http://sf.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ls.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://db.shtwfgs.cn

TS:   greet(): string { return this.name; }
来源：http://sf.shxzskj.cn

Java: String greet() { return name; }
来源：http://ff.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ek.hahajie.cn

Ruby: def greet; @name; end
来源：http://ws.9csxet.cn

C#:   public string Greet() => Name;
来源：http://ky.huanxung.cn

[G05] 继承
来源：http://xe.huixiangedu.cn

Py:   class Admin(User): pass
来源：http://hm.gzmigu.cn

PHP:  class Admin extends User {}
来源：http://au.lnxyls.cn

JS:   class Admin extends User {}
来源：http://hy.shxzukj.cn

TS:   class Admin extends User {}
来源：http://kj.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://qv.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ud.bookmarksfly.cn

Ruby: class Admin < User; end
来源：http://zy.shtwfgs.cn

C#:   class Admin : User {}
来源：http://ik.haigaiapp.cn

[G06] 重写方法
来源：http://gj.shxzukj.cn

Py:   def greet(self): return "admin"
来源：http://po.yuntaijiaju.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dv.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://ma.bjjhwx.cn

TS:   greet(): string { return "admin"; }
来源：http://vs.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://gb.nicolike.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ml.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://kf.huixinmuqiang.cn

C#:   public override string Greet() => "admin";
来源：http://bt.nicolike.cn

[G07] 调用父类方法
来源：http://fm.huanxung.cn

Py:   super().greet()
来源：http://al.huixinmuqiang.cn

PHP:  parent::greet();
来源：http://az.huixinmuqiang.cn

JS:   super.greet();
来源：http://ts.jctech888.com.cn

TS:   super.greet();
来源：http://gl.521024.cn

Java: super.greet();
来源：http://dx.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vh.gzmigu.cn

Ruby: super
来源：http://ir.colortex.cn

C#:   base.Greet();
来源：http://km.hnjuh.cn

[G08] 静态方法与属性
来源：http://lo.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gc.colortex.cn

PHP:  public static function f() {}
来源：http://gg.521024.cn

JS:   static f() {}
来源：http://an.huixinmuqiang.cn

TS:   static f(): void {}
来源：http://sr.yuexingan06.cn

Java: static void f() {}
来源：http://qy.shxzukj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ej.szsharing.cn

Ruby: def self.f; end
来源：http://ao.yuexingan06.cn

C#:   public static void F() {}
来源：http://rg.chemitech.net.cn

[G09] 接口 / 抽象类
来源：http://hi.hnjuh.cn

Py:   from abc import ABC, abstractmethod
来源：http://xy.yuexingan06.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yc.jctech888.com.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://is.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://fn.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://zs.gzmigu.cn

Go:   type Shape interface { Area() float64 }
来源：http://pa.yuntaijiaju.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rg.panjiajie.cn

C#:   interface IShape { double Area(); }
来源：http://km.yuexingan06.cn

[G10] 访问控制
来源：http://ny.nszjky.cn

Py:   约定 _protected / __private（不强制）
来源：http://vt.shxzskj.cn

PHP:  public / protected / private
来源：http://gw.hnjuh.cn

JS:   #private 字段；其余公开
来源：http://ts.panjiajie.cn

TS:   public / protected / private
来源：http://vh.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://pq.chemitech.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://uc.lnxyls.cn

Ruby: public / protected / private
来源：http://zz.521024.cn

C#:   public / protected / private / internal
来源：http://rl.nicolike.cn

[G11] getter / setter
来源：http://lt.yuntaijiaju.cn

Py:   @property 与 @x.setter
来源：http://ew.hahajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jo.bjjhwx.cn

JS:   get name() { return this._name; }
来源：http://ji.9csxet.cn

TS:   get name(): string { return this._name; }
来源：http://wj.nszjky.cn

Java: public String getName() { return name; }
来源：http://do.newstarts.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://db.yuntaijiaju.cn

Ruby: attr_accessor :name
来源：http://rj.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://lp.lnxyls.cn

[G12] 对象转字符串
来源：http://ct.lnxyls.cn

Py:   def __str__(self): return self.name
来源：http://wl.huanxung.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://we.haigaiapp.cn

JS:   toString() { return this.name; }
来源：http://sv.yuexingan06.cn

TS:   toString(): string { return this.name; }
来源：http://zf.lnxyls.cn

Java: @Override public String toString() { return name; }
来源：http://ih.asd995.cn

Go:   func (u User) String() string { return u.Name }
来源：http://uc.jctech888.com.cn

Ruby: def to_s; @name; end
来源：http://re.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://aj.hahajie.cn

[G13] 判断对象类型
来源：http://wu.huixinmuqiang.cn

Py:   isinstance(u, User)
来源：http://ot.shxzukj.cn

PHP:  $u instanceof User
来源：http://jp.newstarts.cn

JS:   u instanceof User
来源：http://zk.huixinmuqiang.cn

TS:   u instanceof User
来源：http://gc.gzmigu.cn

Java: u instanceof User
来源：http://cf.bjjhwx.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qt.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://pu.shxzukj.cn

C#:   u is User
来源：http://gm.nicolike.cn

[G14] 数据类 / record
来源：http://oa.shxzskj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sf.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://ko.yuexingan06.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bh.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://ux.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://zl.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://rb.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uw.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://ja.newstarts.cn

[G15] 枚举
来源：http://zd.chemitech.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zp.szxytkj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vo.nicolike.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gc.lnxyls.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pz.bjjhwx.cn

Java: enum Color { RED, GREEN }
来源：http://sg.haigaiapp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cu.jianghongdianzi.cn

Ruby: Color = %i[red green].freeze
来源：http://xv.hahajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gc.asd995.cn

[G16] 对象转数组 / 字典
来源：http://pa.colortex.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pu.nszjky.cn

PHP:  get_object_vars($obj);
来源：http://hs.haigaiapp.cn

JS:   Object.entries(obj)
来源：http://pf.521024.cn

TS:   Object.entries(obj)
来源：http://zx.szsharing.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tt.521024.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kc.colortex.cn

Ruby: obj.instance_variables
来源：http://ue.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://kj.szxytkj.cn

================================================================================
来源：http://vp.szsharing.cn

H. 异常与错误处理
来源：http://hw.huixinmuqiang.cn

================================================================================
来源：http://il.yuntaijiaju.cn

[H01] try / catch 基础
来源：http://ev.huixiangedu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://en.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lu.yuexingan06.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vj.yuexingan06.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kc.huanxung.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rn.chemitech.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mu.yuexingan06.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vt.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nm.huanxung.cn

[H02] finally / ensure 收尾
来源：http://jw.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gu.hnjuh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tz.bjjhwx.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yq.huanxung.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ep.szsharing.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bd.shxzukj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ge.huixiangedu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tc.9csxet.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hq.szsharing.cn

[H03] 主动抛出异常
来源：http://ys.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://qy.jianghongdianzi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://we.nszjky.cn

JS:   throw new Error("错误信息");
来源：http://ze.yuexingan06.cn

TS:   throw new Error("错误信息");
来源：http://ep.panjiajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qk.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ph.muxihuayi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ao.wgjwhj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ly.shtwfgs.cn

[H04] 自定义异常类型
来源：http://na.yuntaijiaju.cn

Py:   class MyError(Exception): pass
来源：http://di.newstarts.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pg.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://jx.shxzskj.cn

TS:   class MyError extends Error {}
来源：http://dz.bookmarksfly.cn

Java: class MyException extends RuntimeException {}
来源：http://ss.huixiangedu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mj.huanxung.cn

Ruby: class MyError < StandardError; end
来源：http://sh.chemitech.net.cn

C#:   class MyException : Exception {}
来源：http://as.huixinmuqiang.cn

[H05] 捕获特定类型
来源：http://zi.yuexingan06.cn

Py:   except ValueError as e:
来源：http://xb.wgjwhj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uy.hnjuh.cn

JS:   if (e instanceof TypeError) {}
来源：http://xz.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://qt.jianghongdianzi.cn

Java: catch (IOException | SQLException e) {}
来源：http://ml.szsharing.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xm.shxzskj.cn

Ruby: rescue ArgumentError => e
来源：http://sx.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ra.szxytkj.cn

[H06] 可选值 / 空值安全访问
来源：http://ac.yuexingan06.cn

Py:   value = d.get("k") or default
来源：http://zp.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ix.muxihuayi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nc.colortex.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dx.shxzukj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://li.wgjwhj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bj.haigaiapp.cn

Ruby: d&.dig(:a, :b)
来源：http://sj.huanxung.cn

C#:   obj?.A?.B ?? default
来源：http://wz.shxzskj.cn

[H07] 断言
来源：http://dh.shxzskj.cn

Py:   assert x > 0, "必须为正"
来源：http://fp.chemitech.net.cn

PHP:  assert($x > 0);
来源：http://ss.shxzukj.cn

JS:   console.assert(x > 0);
来源：http://il.huixinmuqiang.cn

TS:   console.assert(x > 0);
来源：http://oc.yuntaijiaju.cn

Java: assert x > 0 : "必须为正";
来源：http://gd.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oj.chemitech.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mv.9csxet.cn

C#:   Debug.Assert(x > 0);
来源：http://oh.yuexingan06.cn

[H08] 获取错误信息与堆栈
来源：http://ho.lnxyls.cn

Py:   str(e);  traceback.format_exc()
来源：http://jv.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sm.shxzukj.cn

JS:   e.message;  e.stack
来源：http://wq.colortex.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://am.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cc.shxzukj.cn

Go:   err.Error()
来源：http://um.521024.cn

Ruby: e.message;  e.backtrace
来源：http://xi.panjiajie.cn

C#:   e.Message;  e.StackTrace
来源：http://oi.yuexingan06.cn

[H09] 带错误码的异常
来源：http://yf.nicolike.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kh.wgjwhj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lz.szxytkj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ya.hahajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ox.lnxyls.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pm.haigaiapp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ig.bjjhwx.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xw.nicolike.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mp.jctech888.com.cn

[H10] 资源自动释放
来源：http://wn.nicolike.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ak.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iw.newstarts.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ow.huanxung.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gc.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://au.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://nd.hahajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ht.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nn.chemitech.net.cn

================================================================================
来源：http://tz.bookmarksfly.cn

I. 正则表达式
来源：http://oi.yuntaijiaju.cn

================================================================================
来源：http://yz.jctech888.com.cn

[I01] 判断是否匹配
来源：http://fn.521024.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hi.newstarts.cn

PHP:  preg_match('/\d+/', $s);
来源：http://uy.nszjky.cn

JS:   /\d+/.test(s)
来源：http://pj.9csxet.cn

TS:   /\d+/.test(s)
来源：http://fi.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jl.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mk.521024.cn

Ruby: s.match?(/\d+/)
来源：http://og.panjiajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kq.yuntaijiaju.cn


<!-- 参考信息 -->