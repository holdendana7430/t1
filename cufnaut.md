代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://aj.yuexingan06.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yg.jctech888.com.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iw.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bw.muxihuayi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://to.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dy.jianghongdianzi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ub.nicolike.cn

[F08] 遍历目录
来源：http://ni.huanxung.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qa.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://vx.bjjhwx.cn

JS:   fs.readdirSync("dir")
来源：http://qn.nszjky.cn

TS:   fs.readdirSync("dir")
来源：http://ql.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hu.nicolike.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://an.asd995.cn

Ruby: Dir.children("dir")
来源：http://oo.asd995.cn

C#:   Directory.GetFiles("dir")
来源：http://ef.newstarts.cn

[F09] 获取文件大小
来源：http://nq.szxytkj.cn

Py:   os.path.getsize("a.txt")
来源：http://df.shxzukj.cn

PHP:  filesize("a.txt");
来源：http://gx.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://ej.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://yc.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://qw.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://sc.9csxet.cn

Ruby: File.size("a.txt")
来源：http://tt.nszjky.cn

C#:   new FileInfo("a.txt").Length
来源：http://fv.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://vq.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lq.yuexingan06.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qq.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ab.nicolike.cn

TS:   path.extname("a.txt")
来源：http://yi.nszjky.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mb.muxihuayi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ax.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pe.lnxyls.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fx.huixiangedu.cn

[F11] 复制与移动文件
来源：http://ol.colortex.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ga.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://so.colortex.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sb.haigaiapp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kf.hnjuh.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ix.hahajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tx.colortex.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fo.gzmigu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://tm.lnxyls.cn

[F12] CSV 读写
来源：http://du.huixiangedu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hj.yuntaijiaju.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fe.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uf.muxihuayi.cn

TS:   // 同上
来源：http://ma.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vo.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bq.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wu.szsharing.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yt.hnjuh.cn

================================================================================
来源：http://xg.bookmarksfly.cn

G. 面向对象
来源：http://jm.gzmigu.cn

================================================================================
来源：http://kj.panjiajie.cn

[G01] 定义类
来源：http://sy.hahajie.cn

Py:   class User: pass
来源：http://yt.9csxet.cn

PHP:  class User {}
来源：http://lx.szsharing.cn

JS:   class User {}
来源：http://ba.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://cv.bjjhwx.cn

Java: class User {}
来源：http://jo.colortex.cn

Go:   type User struct { Name string }
来源：http://zl.asd995.cn

Ruby: class User; end
来源：http://mu.521024.cn

C#:   class User {}
来源：http://pc.shxzskj.cn

[G02] 构造函数
来源：http://is.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://oj.shtwfgs.cn

PHP:  public function __construct(public string $name) {}
来源：http://ix.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://ug.yuntaijiaju.cn

TS:   constructor(public name: string) {}
来源：http://br.colortex.cn

Java: User(String name) { this.name = name; }
来源：http://nt.bookmarksfly.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://et.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://ds.chemitech.net.cn

C#:   public User(string name) { Name = name; }
来源：http://yd.lnxyls.cn

[G03] 实例属性
来源：http://lx.gzmigu.cn

Py:   self.name = "x"
来源：http://zz.lnxyls.cn

PHP:  public string $name = "x";
来源：http://kr.szsharing.cn

JS:   this.name = "x";
来源：http://od.szxytkj.cn

TS:   name: string = "x";
来源：http://wl.haigaiapp.cn

Java: private String name;
来源：http://sb.jctech888.com.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hj.shxzukj.cn

Ruby: @name = "x"
来源：http://ft.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://si.huixiangedu.cn

[G04] 定义方法
来源：http://na.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://gl.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pe.chemitech.net.cn

JS:   greet() { return this.name; }
来源：http://fm.bookmarksfly.cn

TS:   greet(): string { return this.name; }
来源：http://cx.huixinmuqiang.cn

Java: String greet() { return name; }
来源：http://zm.lnxyls.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bo.szxytkj.cn

Ruby: def greet; @name; end
来源：http://zs.shxzskj.cn

C#:   public string Greet() => Name;
来源：http://wk.newstarts.cn

[G05] 继承
来源：http://aq.shxzskj.cn

Py:   class Admin(User): pass
来源：http://jk.jianghongdianzi.cn

PHP:  class Admin extends User {}
来源：http://vg.shxzukj.cn

JS:   class Admin extends User {}
来源：http://zr.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://mb.szxytkj.cn

Java: class Admin extends User {}
来源：http://nn.newstarts.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://up.hnjuh.cn

Ruby: class Admin < User; end
来源：http://pb.newstarts.cn

C#:   class Admin : User {}
来源：http://lm.chemitech.net.cn

[G06] 重写方法
来源：http://ta.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://ba.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rf.muxihuayi.cn

JS:   greet() { return "admin"; }
来源：http://ii.bookmarksfly.cn

TS:   greet(): string { return "admin"; }
来源：http://tt.szxytkj.cn

Java: @Override String greet() { return "admin"; }
来源：http://hy.nszjky.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kk.shxzskj.cn

Ruby: def greet; "admin"; end
来源：http://cc.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://uv.lnxyls.cn

[G07] 调用父类方法
来源：http://sv.panjiajie.cn

Py:   super().greet()
来源：http://yr.newstarts.cn

PHP:  parent::greet();
来源：http://vd.huanxung.cn

JS:   super.greet();
来源：http://gs.bjjhwx.cn

TS:   super.greet();
来源：http://ss.jctech888.com.cn

Java: super.greet();
来源：http://vl.muxihuayi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dl.9csxet.cn

Ruby: super
来源：http://wy.9csxet.cn

C#:   base.Greet();
来源：http://pu.chemitech.net.cn

[G08] 静态方法与属性
来源：http://fa.9csxet.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wk.bjjhwx.cn

PHP:  public static function f() {}
来源：http://rv.hahajie.cn

JS:   static f() {}
来源：http://fp.huanxung.cn

TS:   static f(): void {}
来源：http://at.bjjhwx.cn

Java: static void f() {}
来源：http://nh.shtwfgs.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zt.shxzskj.cn

Ruby: def self.f; end
来源：http://el.bjjhwx.cn

C#:   public static void F() {}
来源：http://vm.wgjwhj.cn

[G09] 接口 / 抽象类
来源：http://rh.haigaiapp.cn

Py:   from abc import ABC, abstractmethod
来源：http://iz.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bh.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zf.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://in.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://un.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://xm.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://de.jianghongdianzi.cn

C#:   interface IShape { double Area(); }
来源：http://gk.newstarts.cn

[G10] 访问控制
来源：http://ed.bookmarksfly.cn

Py:   约定 _protected / __private（不强制）
来源：http://sx.panjiajie.cn

PHP:  public / protected / private
来源：http://vf.szxytkj.cn

JS:   #private 字段；其余公开
来源：http://yb.lnxyls.cn

TS:   public / protected / private
来源：http://tx.szxytkj.cn

Java: public / protected / private / 默认包级
来源：http://ih.lnxyls.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fo.jctech888.com.cn

Ruby: public / protected / private
来源：http://kq.szxytkj.cn

C#:   public / protected / private / internal
来源：http://qs.muxihuayi.cn

[G11] getter / setter
来源：http://po.jctech888.com.cn

Py:   @property 与 @x.setter
来源：http://np.chemitech.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ot.huanxung.cn

JS:   get name() { return this._name; }
来源：http://ng.lnxyls.cn

TS:   get name(): string { return this._name; }
来源：http://uv.szxytkj.cn

Java: public String getName() { return name; }
来源：http://yi.huixiangedu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mq.wgjwhj.cn

Ruby: attr_accessor :name
来源：http://or.hahajie.cn

C#:   public string Name { get; set; }
来源：http://vs.jctech888.com.cn

[G12] 对象转字符串
来源：http://aw.huixinmuqiang.cn

Py:   def __str__(self): return self.name
来源：http://ig.huanxung.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xa.bjjhwx.cn

JS:   toString() { return this.name; }
来源：http://lg.panjiajie.cn

TS:   toString(): string { return this.name; }
来源：http://gx.521024.cn

Java: @Override public String toString() { return name; }
来源：http://be.asd995.cn

Go:   func (u User) String() string { return u.Name }
来源：http://oi.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://qv.bjjhwx.cn

C#:   public override string ToString() => Name;
来源：http://lx.gzmigu.cn

[G13] 判断对象类型
来源：http://ed.521024.cn

Py:   isinstance(u, User)
来源：http://zb.asd995.cn

PHP:  $u instanceof User
来源：http://nk.haigaiapp.cn

JS:   u instanceof User
来源：http://jh.shtwfgs.cn

TS:   u instanceof User
来源：http://zc.shxzukj.cn

Java: u instanceof User
来源：http://ai.newstarts.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://an.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://zk.colortex.cn

C#:   u is User
来源：http://bw.shxzukj.cn

[G14] 数据类 / record
来源：http://aw.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fa.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://qy.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gv.newstarts.cn

TS:   type User = { name: string; age: number };
来源：http://wj.yuntaijiaju.cn

Java: record User(String name, int age) {}
来源：http://qy.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://yx.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xq.haigaiapp.cn

C#:   record User(string Name, int Age);
来源：http://iq.bookmarksfly.cn

[G15] 枚举
来源：http://lq.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hd.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kz.szsharing.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ge.nszjky.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mo.9csxet.cn

Java: enum Color { RED, GREEN }
来源：http://nt.shxzukj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zh.521024.cn

Ruby: Color = %i[red green].freeze
来源：http://nk.panjiajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bg.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://cl.shxzskj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://iz.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://ui.shxzukj.cn

JS:   Object.entries(obj)
来源：http://vj.shtwfgs.cn

TS:   Object.entries(obj)
来源：http://by.shxzukj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://km.jctech888.com.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.asd995.cn

Ruby: obj.instance_variables
来源：http://ss.chemitech.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://qd.asd995.cn

================================================================================
来源：http://oi.huixiangedu.cn

H. 异常与错误处理
来源：http://hl.muxihuayi.cn

================================================================================
来源：http://jg.huixinmuqiang.cn

[H01] try / catch 基础
来源：http://kz.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sh.shxzukj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://aa.huanxung.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://er.szxytkj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bk.yuexingan06.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jj.9csxet.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uh.haigaiapp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://me.521024.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qg.nszjky.cn

[H02] finally / ensure 收尾
来源：http://pm.gzmigu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mu.huixinmuqiang.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sd.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zx.hahajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yi.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uc.colortex.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qi.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ai.huixinmuqiang.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jt.yuexingan06.cn

[H03] 主动抛出异常
来源：http://lw.yuntaijiaju.cn

Py:   raise ValueError("错误信息")
来源：http://yu.colortex.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ul.yuntaijiaju.cn

JS:   throw new Error("错误信息");
来源：http://hc.huixiangedu.cn

TS:   throw new Error("错误信息");
来源：http://xe.bjjhwx.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ka.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uz.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://us.bookmarksfly.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dn.shtwfgs.cn

[H04] 自定义异常类型
来源：http://tr.lnxyls.cn

Py:   class MyError(Exception): pass
来源：http://vh.jianghongdianzi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ko.yuexingan06.cn

JS:   class MyError extends Error {}
来源：http://ub.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://tm.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://jr.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mr.szsharing.cn

Ruby: class MyError < StandardError; end
来源：http://lh.521024.cn

C#:   class MyException : Exception {}
来源：http://yh.chemitech.net.cn

[H05] 捕获特定类型
来源：http://wr.shxzukj.cn

Py:   except ValueError as e:
来源：http://ru.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ra.shxzskj.cn

JS:   if (e instanceof TypeError) {}
来源：http://au.521024.cn

TS:   if (e instanceof TypeError) {}
来源：http://zu.hahajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://wq.hnjuh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bg.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://xd.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wx.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://tg.panjiajie.cn

Py:   value = d.get("k") or default
来源：http://xt.bjjhwx.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ey.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ao.colortex.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pp.521024.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hr.nszjky.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rx.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://nl.muxihuayi.cn

C#:   obj?.A?.B ?? default
来源：http://wd.bookmarksfly.cn

[H07] 断言
来源：http://iy.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://qd.nicolike.cn

PHP:  assert($x > 0);
来源：http://jr.shxzukj.cn

JS:   console.assert(x > 0);
来源：http://fi.hnjuh.cn

TS:   console.assert(x > 0);
来源：http://gz.newstarts.cn

Java: assert x > 0 : "必须为正";
来源：http://aa.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mi.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vg.chemitech.net.cn

C#:   Debug.Assert(x > 0);
来源：http://eg.shxzskj.cn

[H08] 获取错误信息与堆栈
来源：http://nk.shxzukj.cn

Py:   str(e);  traceback.format_exc()
来源：http://uf.newstarts.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wt.nszjky.cn

JS:   e.message;  e.stack
来源：http://rt.szxytkj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://on.huixinmuqiang.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xs.shxzukj.cn

Go:   err.Error()
来源：http://bo.lnxyls.cn

Ruby: e.message;  e.backtrace
来源：http://hk.asd995.cn

C#:   e.Message;  e.StackTrace
来源：http://xg.shtwfgs.cn

[H09] 带错误码的异常
来源：http://nz.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zw.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gg.bjjhwx.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://it.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ll.hnjuh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uk.szxytkj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mj.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://je.newstarts.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ny.bookmarksfly.cn

[H10] 资源自动释放
来源：http://jb.shtwfgs.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ry.newstarts.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://iy.wgjwhj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hm.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pp.muxihuayi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oa.lnxyls.cn

Go:   defer f.Close()
来源：http://nv.9csxet.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ft.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://iu.asd995.cn

================================================================================
来源：http://dy.gzmigu.cn

I. 正则表达式
来源：http://vu.bjjhwx.cn

================================================================================
来源：http://nu.shtwfgs.cn

[I01] 判断是否匹配
来源：http://bm.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://po.shxzskj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rc.shxzskj.cn

JS:   /\d+/.test(s)
来源：http://yn.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://xf.szsharing.cn


<!-- 参考信息 -->