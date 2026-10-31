代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://xc.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://zy.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://an.panjiajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wy.wgjwhj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://aa.nszjky.cn

TS:   path.extname("a.txt")
来源：http://sz.haigaiapp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yx.bookmarksfly.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://og.colortex.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wx.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uc.lnxyls.cn

[F11] 复制与移动文件
来源：http://mr.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jm.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ls.lnxyls.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dg.newstarts.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zf.521024.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://jp.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://iz.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ne.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ac.newstarts.cn

[F12] CSV 读写
来源：http://ds.yuntaijiaju.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://aw.shtwfgs.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sx.9csxet.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tu.jianghongdianzi.cn

TS:   // 同上
来源：http://zy.nszjky.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fi.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://re.hnjuh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://as.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://da.panjiajie.cn

================================================================================
来源：http://st.yuntaijiaju.cn

G. 面向对象
来源：http://ny.jianghongdianzi.cn

================================================================================
来源：http://zp.jianghongdianzi.cn

[G01] 定义类
来源：http://fa.shtwfgs.cn

Py:   class User: pass
来源：http://uq.521024.cn

PHP:  class User {}
来源：http://pf.nszjky.cn

JS:   class User {}
来源：http://vw.jctech888.com.cn

TS:   class User { name: string = ""; }
来源：http://fg.bookmarksfly.cn

Java: class User {}
来源：http://nu.wgjwhj.cn

Go:   type User struct { Name string }
来源：http://xg.huanxung.cn

Ruby: class User; end
来源：http://jp.nszjky.cn

C#:   class User {}
来源：http://pa.wgjwhj.cn

[G02] 构造函数
来源：http://jw.hnjuh.cn

Py:   def __init__(self, name): self.name = name
来源：http://yq.huixinmuqiang.cn

PHP:  public function __construct(public string $name) {}
来源：http://xh.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://zj.wgjwhj.cn

TS:   constructor(public name: string) {}
来源：http://ag.szxytkj.cn

Java: User(String name) { this.name = name; }
来源：http://lw.yuntaijiaju.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xp.colortex.cn

Ruby: def initialize(name); @name = name; end
来源：http://jd.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://jd.shxzukj.cn

[G03] 实例属性
来源：http://sf.bjjhwx.cn

Py:   self.name = "x"
来源：http://pb.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://tr.panjiajie.cn

JS:   this.name = "x";
来源：http://fj.lnxyls.cn

TS:   name: string = "x";
来源：http://ip.gzmigu.cn

Java: private String name;
来源：http://uu.shxzskj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://zy.chemitech.net.cn

Ruby: @name = "x"
来源：http://ey.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://ku.shtwfgs.cn

[G04] 定义方法
来源：http://pc.szxytkj.cn

Py:   def greet(self): return self.name
来源：http://ug.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mq.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://zq.bookmarksfly.cn

TS:   greet(): string { return this.name; }
来源：http://wy.haigaiapp.cn

Java: String greet() { return name; }
来源：http://eg.gzmigu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://im.szsharing.cn

Ruby: def greet; @name; end
来源：http://sd.newstarts.cn

C#:   public string Greet() => Name;
来源：http://ke.yuexingan06.cn

[G05] 继承
来源：http://al.szxytkj.cn

Py:   class Admin(User): pass
来源：http://lg.muxihuayi.cn

PHP:  class Admin extends User {}
来源：http://ex.nszjky.cn

JS:   class Admin extends User {}
来源：http://od.wgjwhj.cn

TS:   class Admin extends User {}
来源：http://hm.nszjky.cn

Java: class Admin extends User {}
来源：http://ie.wgjwhj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://aj.panjiajie.cn

Ruby: class Admin < User; end
来源：http://jn.panjiajie.cn

C#:   class Admin : User {}
来源：http://ao.muxihuayi.cn

[G06] 重写方法
来源：http://la.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://fe.jctech888.com.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xj.yuexingan06.cn

JS:   greet() { return "admin"; }
来源：http://as.hnjuh.cn

TS:   greet(): string { return "admin"; }
来源：http://tv.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://ni.newstarts.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qo.nszjky.cn

Ruby: def greet; "admin"; end
来源：http://fg.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://xp.bookmarksfly.cn

[G07] 调用父类方法
来源：http://wv.szsharing.cn

Py:   super().greet()
来源：http://bs.chemitech.net.cn

PHP:  parent::greet();
来源：http://aa.huixiangedu.cn

JS:   super.greet();
来源：http://wu.hnjuh.cn

TS:   super.greet();
来源：http://uf.yuexingan06.cn

Java: super.greet();
来源：http://to.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xn.chemitech.net.cn

Ruby: super
来源：http://hz.yuexingan06.cn

C#:   base.Greet();
来源：http://kr.shxzukj.cn

[G08] 静态方法与属性
来源：http://yp.szxytkj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mt.muxihuayi.cn

PHP:  public static function f() {}
来源：http://fz.gzmigu.cn

JS:   static f() {}
来源：http://pk.panjiajie.cn

TS:   static f(): void {}
来源：http://zk.9csxet.cn

Java: static void f() {}
来源：http://be.9csxet.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://za.wgjwhj.cn

Ruby: def self.f; end
来源：http://ow.wgjwhj.cn

C#:   public static void F() {}
来源：http://wj.bookmarksfly.cn

[G09] 接口 / 抽象类
来源：http://lt.wgjwhj.cn

Py:   from abc import ABC, abstractmethod
来源：http://oe.9csxet.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sx.jianghongdianzi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ir.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://en.jianghongdianzi.cn

Java: interface Shape { double area(); }
来源：http://zt.muxihuayi.cn

Go:   type Shape interface { Area() float64 }
来源：http://dc.huixiangedu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://at.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://et.colortex.cn

[G10] 访问控制
来源：http://wc.yuntaijiaju.cn

Py:   约定 _protected / __private（不强制）
来源：http://dd.haigaiapp.cn

PHP:  public / protected / private
来源：http://qc.521024.cn

JS:   #private 字段；其余公开
来源：http://ld.panjiajie.cn

TS:   public / protected / private
来源：http://gl.nszjky.cn

Java: public / protected / private / 默认包级
来源：http://wt.shxzukj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sp.nicolike.cn

Ruby: public / protected / private
来源：http://vc.lnxyls.cn

C#:   public / protected / private / internal
来源：http://be.newstarts.cn

[G11] getter / setter
来源：http://ah.newstarts.cn

Py:   @property 与 @x.setter
来源：http://sa.szsharing.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wk.jianghongdianzi.cn

JS:   get name() { return this._name; }
来源：http://oi.haigaiapp.cn

TS:   get name(): string { return this._name; }
来源：http://df.bookmarksfly.cn

Java: public String getName() { return name; }
来源：http://zl.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://er.shxzukj.cn

Ruby: attr_accessor :name
来源：http://go.szsharing.cn

C#:   public string Name { get; set; }
来源：http://cr.nicolike.cn

[G12] 对象转字符串
来源：http://cb.newstarts.cn

Py:   def __str__(self): return self.name
来源：http://ur.huixinmuqiang.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://cx.nszjky.cn

JS:   toString() { return this.name; }
来源：http://qg.muxihuayi.cn

TS:   toString(): string { return this.name; }
来源：http://en.9csxet.cn

Java: @Override public String toString() { return name; }
来源：http://zq.muxihuayi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://no.haigaiapp.cn

Ruby: def to_s; @name; end
来源：http://hc.lnxyls.cn

C#:   public override string ToString() => Name;
来源：http://dj.hahajie.cn

[G13] 判断对象类型
来源：http://pn.bookmarksfly.cn

Py:   isinstance(u, User)
来源：http://gl.nszjky.cn

PHP:  $u instanceof User
来源：http://vz.jianghongdianzi.cn

JS:   u instanceof User
来源：http://ry.newstarts.cn

TS:   u instanceof User
来源：http://qa.szxytkj.cn

Java: u instanceof User
来源：http://kg.asd995.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jm.9csxet.cn

Ruby: u.is_a?(User)
来源：http://yo.9csxet.cn

C#:   u is User
来源：http://ek.huixiangedu.cn

[G14] 数据类 / record
来源：http://wr.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mj.colortex.cn

PHP:  // 用 readonly 属性模拟
来源：http://bp.jianghongdianzi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://al.wgjwhj.cn

TS:   type User = { name: string; age: number };
来源：http://et.asd995.cn

Java: record User(String name, int age) {}
来源：http://xx.panjiajie.cn

Go:   type User struct { Name string; Age int }
来源：http://ai.shxzukj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ob.asd995.cn

C#:   record User(string Name, int Age);
来源：http://px.jianghongdianzi.cn

[G15] 枚举
来源：http://nn.newstarts.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pq.gzmigu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jz.9csxet.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xg.shxzukj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iq.jianghongdianzi.cn

Java: enum Color { RED, GREEN }
来源：http://hb.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ob.panjiajie.cn

Ruby: Color = %i[red green].freeze
来源：http://fy.hnjuh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ty.huanxung.cn

[G16] 对象转数组 / 字典
来源：http://ju.huanxung.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zh.shtwfgs.cn

PHP:  get_object_vars($obj);
来源：http://sd.yuexingan06.cn

JS:   Object.entries(obj)
来源：http://jf.szsharing.cn

TS:   Object.entries(obj)
来源：http://ge.lnxyls.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ya.nszjky.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xz.yuntaijiaju.cn

Ruby: obj.instance_variables
来源：http://lq.shtwfgs.cn

C#:   // 用反射或 System.Text.Json
来源：http://cn.colortex.cn

================================================================================
来源：http://tl.nszjky.cn

H. 异常与错误处理
来源：http://ik.wgjwhj.cn

================================================================================
来源：http://my.huixiangedu.cn

[H01] try / catch 基础
来源：http://im.hnjuh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jh.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://po.nszjky.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ij.lnxyls.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://te.huixiangedu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ts.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mn.haigaiapp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://il.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xg.muxihuayi.cn

[H02] finally / ensure 收尾
来源：http://wq.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://cs.shtwfgs.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ek.jctech888.com.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yl.szsharing.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gg.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fo.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://uc.colortex.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jn.newstarts.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dr.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://es.jctech888.com.cn

Py:   raise ValueError("错误信息")
来源：http://bs.521024.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ew.colortex.cn

JS:   throw new Error("错误信息");
来源：http://ho.chemitech.net.cn

TS:   throw new Error("错误信息");
来源：http://cs.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://kd.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ii.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kc.chemitech.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kt.shtwfgs.cn

[H04] 自定义异常类型
来源：http://ax.colortex.cn

Py:   class MyError(Exception): pass
来源：http://be.hnjuh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xv.yuntaijiaju.cn

JS:   class MyError extends Error {}
来源：http://wm.shxzskj.cn

TS:   class MyError extends Error {}
来源：http://wv.shxzskj.cn

Java: class MyException extends RuntimeException {}
来源：http://ya.bookmarksfly.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yc.colortex.cn

Ruby: class MyError < StandardError; end
来源：http://yu.lnxyls.cn

C#:   class MyException : Exception {}
来源：http://ux.hahajie.cn

[H05] 捕获特定类型
来源：http://rd.yuexingan06.cn

Py:   except ValueError as e:
来源：http://jx.nicolike.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://up.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://lu.bjjhwx.cn

TS:   if (e instanceof TypeError) {}
来源：http://wc.nszjky.cn

Java: catch (IOException | SQLException e) {}
来源：http://jq.bjjhwx.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hj.asd995.cn

Ruby: rescue ArgumentError => e
来源：http://hb.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kj.haigaiapp.cn

[H06] 可选值 / 空值安全访问
来源：http://zf.nicolike.cn

Py:   value = d.get("k") or default
来源：http://fu.bjjhwx.cn

PHP:  $v = $d["k"] ?? null;
来源：http://je.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://on.huixinmuqiang.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bs.nicolike.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://el.szsharing.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sa.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://mi.bookmarksfly.cn

C#:   obj?.A?.B ?? default
来源：http://kr.yuexingan06.cn

[H07] 断言
来源：http://lz.9csxet.cn

Py:   assert x > 0, "必须为正"
来源：http://mk.521024.cn

PHP:  assert($x > 0);
来源：http://ua.shxzskj.cn

JS:   console.assert(x > 0);
来源：http://py.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://jn.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://sk.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dh.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xi.panjiajie.cn

C#:   Debug.Assert(x > 0);
来源：http://ne.bjjhwx.cn

[H08] 获取错误信息与堆栈
来源：http://re.shxzskj.cn

Py:   str(e);  traceback.format_exc()
来源：http://br.asd995.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ja.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://nu.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yc.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ip.panjiajie.cn

Go:   err.Error()
来源：http://pj.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://en.hahajie.cn

C#:   e.Message;  e.StackTrace
来源：http://gl.hnjuh.cn

[H09] 带错误码的异常
来源：http://bo.521024.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ga.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vy.shtwfgs.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ct.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ok.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cv.yuexingan06.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zg.shtwfgs.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mw.panjiajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://aj.shxzskj.cn

[H10] 资源自动释放
来源：http://up.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cn.bookmarksfly.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://pq.newstarts.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://li.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yy.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://to.hahajie.cn

Go:   defer f.Close()
来源：http://wi.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tu.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yp.newstarts.cn

================================================================================
来源：http://mi.haigaiapp.cn

I. 正则表达式
来源：http://zd.szsharing.cn

================================================================================
来源：http://pa.huixinmuqiang.cn

[I01] 判断是否匹配
来源：http://ot.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://at.asd995.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mh.yuexingan06.cn

JS:   /\d+/.test(s)
来源：http://wu.szxytkj.cn

TS:   /\d+/.test(s)
来源：http://kr.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mr.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gf.newstarts.cn

Ruby: s.match?(/\d+/)
来源：http://dl.gzmigu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qu.szsharing.cn

[I02] 提取所有匹配
来源：http://hi.panjiajie.cn

Py:   re.findall(r"\d+", s)
来源：http://zk.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mw.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eb.haigaiapp.cn

TS:   s.match(/\d+/g)
来源：http://po.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dy.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://co.asd995.cn

Ruby: s.scan(/\d+/)
来源：http://lp.szxytkj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kn.lnxyls.cn

[I03] 提取捕获分组
来源：http://ab.nszjky.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://om.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vt.hnjuh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fq.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dm.jianghongdianzi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ns.newstarts.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wm.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qa.huixiangedu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iz.asd995.cn

[I04] 正则替换
来源：http://yk.chemitech.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://uz.shtwfgs.cn


<!-- 参考信息 -->