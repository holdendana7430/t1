代发 wailian999

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ft.521024.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yq.shxzukj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ad.huixinmuqiang.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wo.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ph.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://na.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fm.shxzukj.cn

[F08] 遍历目录
来源：http://hc.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ov.nicolike.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://aq.huixiangedu.cn

JS:   fs.readdirSync("dir")
来源：http://rs.yuntaijiaju.cn

TS:   fs.readdirSync("dir")
来源：http://ux.bookmarksfly.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sb.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sk.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://de.huixinmuqiang.cn

C#:   Directory.GetFiles("dir")
来源：http://he.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://db.colortex.cn

Py:   os.path.getsize("a.txt")
来源：http://dr.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://fu.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://sc.szsharing.cn

TS:   fs.statSync("a.txt").size
来源：http://us.colortex.cn

Java: Files.size(Path.of("a.txt"))
来源：http://eg.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ig.chemitech.net.cn

Ruby: File.size("a.txt")
来源：http://qp.yuexingan06.cn

C#:   new FileInfo("a.txt").Length
来源：http://rj.muxihuayi.cn

[F10] 取文件扩展名 / 文件名
来源：http://wa.bjjhwx.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mr.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fg.szsharing.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qk.gzmigu.cn

TS:   path.extname("a.txt")
来源：http://ua.szxytkj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nv.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ml.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eo.521024.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gl.shxzukj.cn

[F11] 复制与移动文件
来源：http://ty.hnjuh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://po.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wz.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oo.bjjhwx.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wz.szxytkj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wo.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sc.wgjwhj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sa.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kn.jianghongdianzi.cn

[F12] CSV 读写
来源：http://rj.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eh.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nt.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oz.gzmigu.cn

TS:   // 同上
来源：http://ws.yuntaijiaju.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://eu.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://rp.jctech888.com.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lq.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dt.huanxung.cn

================================================================================
来源：http://et.huixiangedu.cn

G. 面向对象
来源：http://gd.9csxet.cn

================================================================================
来源：http://xj.shxzskj.cn

[G01] 定义类
来源：http://mz.szxytkj.cn

Py:   class User: pass
来源：http://wa.bjjhwx.cn

PHP:  class User {}
来源：http://qd.haigaiapp.cn

JS:   class User {}
来源：http://mm.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://vz.huixiangedu.cn

Java: class User {}
来源：http://my.jianghongdianzi.cn

Go:   type User struct { Name string }
来源：http://ho.wgjwhj.cn

Ruby: class User; end
来源：http://sx.szsharing.cn

C#:   class User {}
来源：http://xv.huixiangedu.cn

[G02] 构造函数
来源：http://zk.colortex.cn

Py:   def __init__(self, name): self.name = name
来源：http://aj.panjiajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://th.gzmigu.cn

JS:   constructor(name) { this.name = name; }
来源：http://mf.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://yx.shxzukj.cn

Java: User(String name) { this.name = name; }
来源：http://ld.huanxung.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ha.521024.cn

Ruby: def initialize(name); @name = name; end
来源：http://pl.asd995.cn

C#:   public User(string name) { Name = name; }
来源：http://dw.huixiangedu.cn

[G03] 实例属性
来源：http://dz.nszjky.cn

Py:   self.name = "x"
来源：http://jw.nicolike.cn

PHP:  public string $name = "x";
来源：http://qw.bjjhwx.cn

JS:   this.name = "x";
来源：http://ze.hnjuh.cn

TS:   name: string = "x";
来源：http://mx.shxzukj.cn

Java: private String name;
来源：http://ji.shxzukj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oh.gzmigu.cn

Ruby: @name = "x"
来源：http://an.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://qb.huanxung.cn

[G04] 定义方法
来源：http://pi.shtwfgs.cn

Py:   def greet(self): return self.name
来源：http://ec.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://jo.hahajie.cn

JS:   greet() { return this.name; }
来源：http://ul.szsharing.cn

TS:   greet(): string { return this.name; }
来源：http://td.muxihuayi.cn

Java: String greet() { return name; }
来源：http://gi.nicolike.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ql.huixiangedu.cn

Ruby: def greet; @name; end
来源：http://pz.bjjhwx.cn

C#:   public string Greet() => Name;
来源：http://od.bjjhwx.cn

[G05] 继承
来源：http://de.521024.cn

Py:   class Admin(User): pass
来源：http://jt.bookmarksfly.cn

PHP:  class Admin extends User {}
来源：http://lz.jianghongdianzi.cn

JS:   class Admin extends User {}
来源：http://bp.yuntaijiaju.cn

TS:   class Admin extends User {}
来源：http://zs.bookmarksfly.cn

Java: class Admin extends User {}
来源：http://ht.huixiangedu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rb.shxzskj.cn

Ruby: class Admin < User; end
来源：http://vv.9csxet.cn

C#:   class Admin : User {}
来源：http://pv.newstarts.cn

[G06] 重写方法
来源：http://fi.chemitech.net.cn

Py:   def greet(self): return "admin"
来源：http://pa.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mr.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://gv.colortex.cn

TS:   greet(): string { return "admin"; }
来源：http://ps.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://tb.hahajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ko.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://gv.newstarts.cn

C#:   public override string Greet() => "admin";
来源：http://dx.lnxyls.cn

[G07] 调用父类方法
来源：http://jn.huixiangedu.cn

Py:   super().greet()
来源：http://ja.haigaiapp.cn

PHP:  parent::greet();
来源：http://mf.wgjwhj.cn

JS:   super.greet();
来源：http://lm.9csxet.cn

TS:   super.greet();
来源：http://ai.asd995.cn

Java: super.greet();
来源：http://bi.hnjuh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ox.asd995.cn

Ruby: super
来源：http://gn.521024.cn

C#:   base.Greet();
来源：http://te.yuntaijiaju.cn

[G08] 静态方法与属性
来源：http://xm.9csxet.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pa.521024.cn

PHP:  public static function f() {}
来源：http://rr.haigaiapp.cn

JS:   static f() {}
来源：http://mc.yuexingan06.cn

TS:   static f(): void {}
来源：http://th.colortex.cn

Java: static void f() {}
来源：http://hr.lnxyls.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nx.huanxung.cn

Ruby: def self.f; end
来源：http://ub.lnxyls.cn

C#:   public static void F() {}
来源：http://jq.colortex.cn

[G09] 接口 / 抽象类
来源：http://vf.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://ll.jianghongdianzi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lv.huixinmuqiang.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gz.hahajie.cn

TS:   interface Shape { area(): number; }
来源：http://xl.muxihuayi.cn

Java: interface Shape { double area(); }
来源：http://ue.yuexingan06.cn

Go:   type Shape interface { Area() float64 }
来源：http://wr.huixiangedu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tw.shxzskj.cn

C#:   interface IShape { double Area(); }
来源：http://dv.szsharing.cn

[G10] 访问控制
来源：http://ma.jianghongdianzi.cn

Py:   约定 _protected / __private（不强制）
来源：http://xd.wgjwhj.cn

PHP:  public / protected / private
来源：http://oj.szsharing.cn

JS:   #private 字段；其余公开
来源：http://ga.bjjhwx.cn

TS:   public / protected / private
来源：http://up.huixinmuqiang.cn

Java: public / protected / private / 默认包级
来源：http://ln.huanxung.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rn.szxytkj.cn

Ruby: public / protected / private
来源：http://es.panjiajie.cn

C#:   public / protected / private / internal
来源：http://eg.bookmarksfly.cn

[G11] getter / setter
来源：http://pl.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://nv.gzmigu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fr.nszjky.cn

JS:   get name() { return this._name; }
来源：http://ui.bookmarksfly.cn

TS:   get name(): string { return this._name; }
来源：http://ju.shxzukj.cn

Java: public String getName() { return name; }
来源：http://av.yuexingan06.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kb.lnxyls.cn

Ruby: attr_accessor :name
来源：http://km.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://ew.hahajie.cn

[G12] 对象转字符串
来源：http://jc.panjiajie.cn

Py:   def __str__(self): return self.name
来源：http://sj.asd995.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tk.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://eq.hnjuh.cn

TS:   toString(): string { return this.name; }
来源：http://ez.nszjky.cn

Java: @Override public String toString() { return name; }
来源：http://no.asd995.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ws.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://yt.nicolike.cn

C#:   public override string ToString() => Name;
来源：http://ze.hnjuh.cn

[G13] 判断对象类型
来源：http://re.jctech888.com.cn

Py:   isinstance(u, User)
来源：http://ru.colortex.cn

PHP:  $u instanceof User
来源：http://lm.hahajie.cn

JS:   u instanceof User
来源：http://in.colortex.cn

TS:   u instanceof User
来源：http://kc.shxzskj.cn

Java: u instanceof User
来源：http://at.asd995.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fu.nszjky.cn

Ruby: u.is_a?(User)
来源：http://oj.huixiangedu.cn

C#:   u is User
来源：http://cs.newstarts.cn

[G14] 数据类 / record
来源：http://kq.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tg.jianghongdianzi.cn

PHP:  // 用 readonly 属性模拟
来源：http://bi.szsharing.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kr.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://rp.521024.cn

Java: record User(String name, int age) {}
来源：http://mb.szxytkj.cn

Go:   type User struct { Name string; Age int }
来源：http://qd.huixiangedu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://oq.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://il.hahajie.cn

[G15] 枚举
来源：http://dl.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gg.gzmigu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ir.panjiajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ve.colortex.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mc.9csxet.cn

Java: enum Color { RED, GREEN }
来源：http://bd.bjjhwx.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yx.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://ej.hnjuh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nq.jianghongdianzi.cn

[G16] 对象转数组 / 字典
来源：http://nd.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jy.asd995.cn

PHP:  get_object_vars($obj);
来源：http://cl.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://ud.muxihuayi.cn

TS:   Object.entries(obj)
来源：http://ld.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yq.jianghongdianzi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ur.chemitech.net.cn

Ruby: obj.instance_variables
来源：http://rd.nszjky.cn

C#:   // 用反射或 System.Text.Json
来源：http://jc.wgjwhj.cn

================================================================================
来源：http://xt.huixinmuqiang.cn

H. 异常与错误处理
来源：http://gy.gzmigu.cn

================================================================================
来源：http://sr.shxzskj.cn

[H01] try / catch 基础
来源：http://cb.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://im.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bf.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iq.shxzukj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gh.521024.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jf.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oi.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://as.nszjky.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://el.gzmigu.cn

[H02] finally / ensure 收尾
来源：http://ta.shtwfgs.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ny.nszjky.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xa.bookmarksfly.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://da.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yk.huixinmuqiang.cn

Java: try { f(); } finally { cleanup(); }
来源：http://up.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rh.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gp.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lf.jianghongdianzi.cn

[H03] 主动抛出异常
来源：http://qb.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://dm.9csxet.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vz.szxytkj.cn

JS:   throw new Error("错误信息");
来源：http://dp.muxihuayi.cn

TS:   throw new Error("错误信息");
来源：http://yk.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qj.huanxung.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ad.muxihuayi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ez.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ow.szxytkj.cn

[H04] 自定义异常类型
来源：http://yz.panjiajie.cn

Py:   class MyError(Exception): pass
来源：http://zh.huanxung.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yh.gzmigu.cn

JS:   class MyError extends Error {}
来源：http://pe.jianghongdianzi.cn

TS:   class MyError extends Error {}
来源：http://fj.lnxyls.cn

Java: class MyException extends RuntimeException {}
来源：http://sr.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hc.huanxung.cn

Ruby: class MyError < StandardError; end
来源：http://gt.huixinmuqiang.cn

C#:   class MyException : Exception {}
来源：http://gs.shxzukj.cn

[H05] 捕获特定类型
来源：http://nq.haigaiapp.cn

Py:   except ValueError as e:
来源：http://zm.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qv.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://ec.nszjky.cn

TS:   if (e instanceof TypeError) {}
来源：http://si.asd995.cn

Java: catch (IOException | SQLException e) {}
来源：http://tg.jianghongdianzi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mg.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://tb.lnxyls.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oa.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://pm.9csxet.cn

Py:   value = d.get("k") or default
来源：http://hi.shxzukj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mn.muxihuayi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://io.szsharing.cn

TS:   obj?.a?.b;  d ?? default
来源：http://it.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://en.chemitech.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vs.yuexingan06.cn

Ruby: d&.dig(:a, :b)
来源：http://ra.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://sm.haigaiapp.cn

[H07] 断言
来源：http://ys.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://sy.521024.cn

PHP:  assert($x > 0);
来源：http://dx.jianghongdianzi.cn

JS:   console.assert(x > 0);
来源：http://xb.jianghongdianzi.cn

TS:   console.assert(x > 0);
来源：http://ci.asd995.cn

Java: assert x > 0 : "必须为正";
来源：http://dv.nszjky.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qa.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qz.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://hi.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://ff.huixiangedu.cn

Py:   str(e);  traceback.format_exc()
来源：http://qg.shxzukj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yu.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://kv.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kt.szxytkj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jo.wgjwhj.cn

Go:   err.Error()
来源：http://ps.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://jk.haigaiapp.cn

C#:   e.Message;  e.StackTrace
来源：http://ju.nszjky.cn

[H09] 带错误码的异常
来源：http://wc.nszjky.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pw.hnjuh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tz.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uz.yuexingan06.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bv.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cl.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oj.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ij.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hr.shxzskj.cn

[H10] 资源自动释放
来源：http://yj.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ld.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://de.szxytkj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rp.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tm.huanxung.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ia.yuexingan06.cn

Go:   defer f.Close()
来源：http://lp.bookmarksfly.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nc.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ho.yuntaijiaju.cn

================================================================================
来源：http://lw.muxihuayi.cn

I. 正则表达式
来源：http://dk.gzmigu.cn

================================================================================
来源：http://qs.lnxyls.cn

[I01] 判断是否匹配
来源：http://ic.shxzukj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ma.shxzskj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zv.bookmarksfly.cn

JS:   /\d+/.test(s)
来源：http://le.nicolike.cn

TS:   /\d+/.test(s)
来源：http://wi.jctech888.com.cn


<!-- 参考信息 -->