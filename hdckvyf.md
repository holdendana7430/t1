代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bu.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tq.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hm.bjjhwx.cn

[F08] 遍历目录
来源：http://vq.shxzukj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tq.wgjwhj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://pp.bjjhwx.cn

JS:   fs.readdirSync("dir")
来源：http://zw.muxihuayi.cn

TS:   fs.readdirSync("dir")
来源：http://mw.nszjky.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yc.huixiangedu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wf.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://uq.hnjuh.cn

C#:   Directory.GetFiles("dir")
来源：http://bz.hnjuh.cn

[F09] 获取文件大小
来源：http://fa.wgjwhj.cn

Py:   os.path.getsize("a.txt")
来源：http://hk.shtwfgs.cn

PHP:  filesize("a.txt");
来源：http://ta.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://fm.jianghongdianzi.cn

TS:   fs.statSync("a.txt").size
来源：http://tn.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nx.nicolike.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://df.huixinmuqiang.cn

Ruby: File.size("a.txt")
来源：http://my.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://he.nszjky.cn

[F10] 取文件扩展名 / 文件名
来源：http://nl.chemitech.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zq.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jz.szxytkj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qf.shxzukj.cn

TS:   path.extname("a.txt")
来源：http://bk.nszjky.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hh.szsharing.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pk.gzmigu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://oa.asd995.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yo.shxzskj.cn

[F11] 复制与移动文件
来源：http://vo.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fm.szsharing.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fo.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jr.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wr.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kg.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qw.huixinmuqiang.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bk.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://by.huixinmuqiang.cn

[F12] CSV 读写
来源：http://nt.nszjky.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jk.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yc.huanxung.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bd.huixiangedu.cn

TS:   // 同上
来源：http://ux.asd995.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wv.jctech888.com.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://iw.hnjuh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hg.newstarts.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yu.panjiajie.cn

================================================================================
来源：http://qb.9csxet.cn

G. 面向对象
来源：http://gn.muxihuayi.cn

================================================================================
来源：http://yr.szsharing.cn

[G01] 定义类
来源：http://yz.huanxung.cn

Py:   class User: pass
来源：http://jb.szsharing.cn

PHP:  class User {}
来源：http://kv.9csxet.cn

JS:   class User {}
来源：http://ca.shxzskj.cn

TS:   class User { name: string = ""; }
来源：http://qd.gzmigu.cn

Java: class User {}
来源：http://qa.colortex.cn

Go:   type User struct { Name string }
来源：http://ls.haigaiapp.cn

Ruby: class User; end
来源：http://wb.panjiajie.cn

C#:   class User {}
来源：http://yj.szxytkj.cn

[G02] 构造函数
来源：http://bs.haigaiapp.cn

Py:   def __init__(self, name): self.name = name
来源：http://ot.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://sj.wgjwhj.cn

JS:   constructor(name) { this.name = name; }
来源：http://gb.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://bz.yuexingan06.cn

Java: User(String name) { this.name = name; }
来源：http://gb.bjjhwx.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ow.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://il.shxzskj.cn

C#:   public User(string name) { Name = name; }
来源：http://xq.521024.cn

[G03] 实例属性
来源：http://cc.huixiangedu.cn

Py:   self.name = "x"
来源：http://bk.hahajie.cn

PHP:  public string $name = "x";
来源：http://px.9csxet.cn

JS:   this.name = "x";
来源：http://af.hnjuh.cn

TS:   name: string = "x";
来源：http://ix.yuntaijiaju.cn

Java: private String name;
来源：http://vr.chemitech.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://as.jctech888.com.cn

Ruby: @name = "x"
来源：http://xb.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://hy.szxytkj.cn

[G04] 定义方法
来源：http://bf.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://gm.shxzukj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wm.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://fe.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://aj.9csxet.cn

Java: String greet() { return name; }
来源：http://ps.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gm.hahajie.cn

Ruby: def greet; @name; end
来源：http://ig.huanxung.cn

C#:   public string Greet() => Name;
来源：http://zs.shxzukj.cn

[G05] 继承
来源：http://la.panjiajie.cn

Py:   class Admin(User): pass
来源：http://qf.bjjhwx.cn

PHP:  class Admin extends User {}
来源：http://op.9csxet.cn

JS:   class Admin extends User {}
来源：http://dj.asd995.cn

TS:   class Admin extends User {}
来源：http://jr.huixinmuqiang.cn

Java: class Admin extends User {}
来源：http://cu.hahajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ug.chemitech.net.cn

Ruby: class Admin < User; end
来源：http://dc.shtwfgs.cn

C#:   class Admin : User {}
来源：http://wi.bjjhwx.cn

[G06] 重写方法
来源：http://vj.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://dl.gzmigu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fz.asd995.cn

JS:   greet() { return "admin"; }
来源：http://hf.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://dt.panjiajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://hm.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jv.shtwfgs.cn

Ruby: def greet; "admin"; end
来源：http://ma.hnjuh.cn

C#:   public override string Greet() => "admin";
来源：http://eg.yuntaijiaju.cn

[G07] 调用父类方法
来源：http://ri.hahajie.cn

Py:   super().greet()
来源：http://da.nszjky.cn

PHP:  parent::greet();
来源：http://zi.szsharing.cn

JS:   super.greet();
来源：http://kw.jctech888.com.cn

TS:   super.greet();
来源：http://sq.yuntaijiaju.cn

Java: super.greet();
来源：http://rt.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ng.hahajie.cn

Ruby: super
来源：http://xt.szxytkj.cn

C#:   base.Greet();
来源：http://wx.jctech888.com.cn

[G08] 静态方法与属性
来源：http://nv.asd995.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bx.9csxet.cn

PHP:  public static function f() {}
来源：http://ik.szxytkj.cn

JS:   static f() {}
来源：http://wr.newstarts.cn

TS:   static f(): void {}
来源：http://lc.szxytkj.cn

Java: static void f() {}
来源：http://yl.521024.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tm.9csxet.cn

Ruby: def self.f; end
来源：http://pz.huanxung.cn

C#:   public static void F() {}
来源：http://dp.bjjhwx.cn

[G09] 接口 / 抽象类
来源：http://cu.bookmarksfly.cn

Py:   from abc import ABC, abstractmethod
来源：http://os.yuexingan06.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yr.asd995.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fu.bookmarksfly.cn

TS:   interface Shape { area(): number; }
来源：http://vk.wgjwhj.cn

Java: interface Shape { double area(); }
来源：http://qs.muxihuayi.cn

Go:   type Shape interface { Area() float64 }
来源：http://hg.9csxet.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://il.huanxung.cn

C#:   interface IShape { double Area(); }
来源：http://tw.huixiangedu.cn

[G10] 访问控制
来源：http://pe.yuntaijiaju.cn

Py:   约定 _protected / __private（不强制）
来源：http://zh.nszjky.cn

PHP:  public / protected / private
来源：http://kx.521024.cn

JS:   #private 字段；其余公开
来源：http://la.asd995.cn

TS:   public / protected / private
来源：http://fk.chemitech.net.cn

Java: public / protected / private / 默认包级
来源：http://uf.colortex.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ee.jctech888.com.cn

Ruby: public / protected / private
来源：http://xo.9csxet.cn

C#:   public / protected / private / internal
来源：http://nw.shtwfgs.cn

[G11] getter / setter
来源：http://vi.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://fm.muxihuayi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ch.bjjhwx.cn

JS:   get name() { return this._name; }
来源：http://iv.nicolike.cn

TS:   get name(): string { return this._name; }
来源：http://sj.haigaiapp.cn

Java: public String getName() { return name; }
来源：http://xy.huanxung.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wl.colortex.cn

Ruby: attr_accessor :name
来源：http://ll.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://qh.panjiajie.cn

[G12] 对象转字符串
来源：http://so.newstarts.cn

Py:   def __str__(self): return self.name
来源：http://ai.bookmarksfly.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gf.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://ba.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://qm.chemitech.net.cn

Java: @Override public String toString() { return name; }
来源：http://ir.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://uu.yuexingan06.cn

Ruby: def to_s; @name; end
来源：http://xs.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://sn.wgjwhj.cn

[G13] 判断对象类型
来源：http://as.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://jv.shxzukj.cn

PHP:  $u instanceof User
来源：http://kv.521024.cn

JS:   u instanceof User
来源：http://eo.newstarts.cn

TS:   u instanceof User
来源：http://cu.asd995.cn

Java: u instanceof User
来源：http://nn.panjiajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pe.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://rp.jianghongdianzi.cn

C#:   u is User
来源：http://zu.jianghongdianzi.cn

[G14] 数据类 / record
来源：http://dp.bookmarksfly.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vz.colortex.cn

PHP:  // 用 readonly 属性模拟
来源：http://ff.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kr.bjjhwx.cn

TS:   type User = { name: string; age: number };
来源：http://vi.shtwfgs.cn

Java: record User(String name, int age) {}
来源：http://us.panjiajie.cn

Go:   type User struct { Name string; Age int }
来源：http://rr.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jb.jctech888.com.cn

C#:   record User(string Name, int Age);
来源：http://pj.lnxyls.cn

[G15] 枚举
来源：http://dz.colortex.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rg.bjjhwx.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ey.panjiajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rf.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pa.nszjky.cn

Java: enum Color { RED, GREEN }
来源：http://rv.nicolike.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kn.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://rr.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nq.newstarts.cn

[G16] 对象转数组 / 字典
来源：http://km.nicolike.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bd.521024.cn

PHP:  get_object_vars($obj);
来源：http://lw.shxzukj.cn

JS:   Object.entries(obj)
来源：http://bd.521024.cn

TS:   Object.entries(obj)
来源：http://gj.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wv.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://eb.panjiajie.cn

Ruby: obj.instance_variables
来源：http://qt.yuntaijiaju.cn

C#:   // 用反射或 System.Text.Json
来源：http://fe.yuexingan06.cn

================================================================================
来源：http://us.chemitech.net.cn

H. 异常与错误处理
来源：http://fi.huanxung.cn

================================================================================
来源：http://mz.shtwfgs.cn

[H01] try / catch 基础
来源：http://tg.huixinmuqiang.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pe.wgjwhj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fl.muxihuayi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kf.lnxyls.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lw.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zz.gzmigu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ez.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kz.shxzskj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://de.huixiangedu.cn

[H02] finally / ensure 收尾
来源：http://qw.huixiangedu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://uw.szsharing.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ec.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xn.hnjuh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xs.hahajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ow.nicolike.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ny.hahajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fn.panjiajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ft.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://ht.huanxung.cn

Py:   raise ValueError("错误信息")
来源：http://dd.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dl.huixiangedu.cn

JS:   throw new Error("错误信息");
来源：http://vt.nszjky.cn

TS:   throw new Error("错误信息");
来源：http://mu.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vt.shxzskj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://eu.bjjhwx.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fl.wgjwhj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ji.lnxyls.cn

[H04] 自定义异常类型
来源：http://go.gzmigu.cn

Py:   class MyError(Exception): pass
来源：http://hi.newstarts.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ni.nicolike.cn

JS:   class MyError extends Error {}
来源：http://xg.colortex.cn

TS:   class MyError extends Error {}
来源：http://ez.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://uf.bjjhwx.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://du.bjjhwx.cn

Ruby: class MyError < StandardError; end
来源：http://kk.szxytkj.cn

C#:   class MyException : Exception {}
来源：http://mi.gzmigu.cn

[H05] 捕获特定类型
来源：http://vr.gzmigu.cn

Py:   except ValueError as e:
来源：http://uh.bookmarksfly.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xq.jctech888.com.cn

JS:   if (e instanceof TypeError) {}
来源：http://li.jianghongdianzi.cn

TS:   if (e instanceof TypeError) {}
来源：http://eu.huanxung.cn

Java: catch (IOException | SQLException e) {}
来源：http://pl.yuexingan06.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hj.lnxyls.cn

Ruby: rescue ArgumentError => e
来源：http://ll.jianghongdianzi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ql.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://yq.chemitech.net.cn

Py:   value = d.get("k") or default
来源：http://to.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gd.chemitech.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ba.yuexingan06.cn

TS:   obj?.a?.b;  d ?? default
来源：http://na.chemitech.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rj.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wo.yuntaijiaju.cn

Ruby: d&.dig(:a, :b)
来源：http://uh.shxzukj.cn

C#:   obj?.A?.B ?? default
来源：http://yu.huixinmuqiang.cn

[H07] 断言
来源：http://or.muxihuayi.cn

Py:   assert x > 0, "必须为正"
来源：http://yc.shtwfgs.cn

PHP:  assert($x > 0);
来源：http://kw.wgjwhj.cn

JS:   console.assert(x > 0);
来源：http://ut.colortex.cn

TS:   console.assert(x > 0);
来源：http://kz.shtwfgs.cn

Java: assert x > 0 : "必须为正";
来源：http://kv.wgjwhj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://np.wgjwhj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nw.jctech888.com.cn

C#:   Debug.Assert(x > 0);
来源：http://ho.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://zg.newstarts.cn

Py:   str(e);  traceback.format_exc()
来源：http://pu.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kr.muxihuayi.cn

JS:   e.message;  e.stack
来源：http://vf.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://iq.yuntaijiaju.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hc.yuntaijiaju.cn

Go:   err.Error()
来源：http://ru.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://hs.haigaiapp.cn

C#:   e.Message;  e.StackTrace
来源：http://wt.huanxung.cn

[H09] 带错误码的异常
来源：http://gn.521024.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ni.huanxung.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hn.shxzskj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ak.nicolike.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zg.nicolike.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ix.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hn.bjjhwx.cn

Ruby: raise MyError.new("fail", 500)
来源：http://uq.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jx.521024.cn

[H10] 资源自动释放
来源：http://eb.521024.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zi.shtwfgs.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tx.hnjuh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bi.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://de.bookmarksfly.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ov.jctech888.com.cn

Go:   defer f.Close()
来源：http://vz.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cq.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ea.haigaiapp.cn

================================================================================
来源：http://xb.yuntaijiaju.cn

I. 正则表达式
来源：http://os.colortex.cn

================================================================================
来源：http://ui.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://vz.huixiangedu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dn.lnxyls.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tu.gzmigu.cn

JS:   /\d+/.test(s)
来源：http://he.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://qe.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rs.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gl.hahajie.cn

Ruby: s.match?(/\d+/)
来源：http://fv.huanxung.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ou.yuexingan06.cn


<!-- 参考信息 -->