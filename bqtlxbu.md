代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hl.huixiangedu.cn

TS:   path.extname("a.txt")
来源：http://uf.asd995.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cs.lnxyls.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://or.szsharing.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://lg.lnxyls.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zo.shxzskj.cn

[F11] 复制与移动文件
来源：http://wh.lnxyls.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shxzukj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fy.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dq.panjiajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://le.muxihuayi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hw.newstarts.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://zc.jctech888.com.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vm.bjjhwx.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://vy.wgjwhj.cn

[F12] CSV 读写
来源：http://bt.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lu.9csxet.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vo.newstarts.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cf.colortex.cn

TS:   // 同上
来源：http://ly.yuexingan06.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oa.bjjhwx.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bg.szxytkj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eo.chemitech.net.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zg.bookmarksfly.cn

================================================================================
来源：http://vi.bjjhwx.cn

G. 面向对象
来源：http://bf.shxzskj.cn

================================================================================
来源：http://xi.chemitech.net.cn

[G01] 定义类
来源：http://zl.jctech888.com.cn

Py:   class User: pass
来源：http://pu.panjiajie.cn

PHP:  class User {}
来源：http://sj.szxytkj.cn

JS:   class User {}
来源：http://lr.nicolike.cn

TS:   class User { name: string = ""; }
来源：http://yf.colortex.cn

Java: class User {}
来源：http://ak.9csxet.cn

Go:   type User struct { Name string }
来源：http://tj.muxihuayi.cn

Ruby: class User; end
来源：http://hc.newstarts.cn

C#:   class User {}
来源：http://jt.szxytkj.cn

[G02] 构造函数
来源：http://qf.yuntaijiaju.cn

Py:   def __init__(self, name): self.name = name
来源：http://zm.lnxyls.cn

PHP:  public function __construct(public string $name) {}
来源：http://wn.huanxung.cn

JS:   constructor(name) { this.name = name; }
来源：http://um.9csxet.cn

TS:   constructor(public name: string) {}
来源：http://iu.wgjwhj.cn

Java: User(String name) { this.name = name; }
来源：http://on.bookmarksfly.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wc.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://vq.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://jz.521024.cn

[G03] 实例属性
来源：http://dw.huanxung.cn

Py:   self.name = "x"
来源：http://ol.shxzskj.cn

PHP:  public string $name = "x";
来源：http://tp.asd995.cn

JS:   this.name = "x";
来源：http://to.wgjwhj.cn

TS:   name: string = "x";
来源：http://fz.huanxung.cn

Java: private String name;
来源：http://ll.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qr.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://ry.bjjhwx.cn

C#:   public string Name { get; set; } = "x";
来源：http://ak.jianghongdianzi.cn

[G04] 定义方法
来源：http://ut.shxzskj.cn

Py:   def greet(self): return self.name
来源：http://gi.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kl.newstarts.cn

JS:   greet() { return this.name; }
来源：http://am.huixiangedu.cn

TS:   greet(): string { return this.name; }
来源：http://ew.szsharing.cn

Java: String greet() { return name; }
来源：http://iv.huixinmuqiang.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ks.chemitech.net.cn

Ruby: def greet; @name; end
来源：http://iu.huixiangedu.cn

C#:   public string Greet() => Name;
来源：http://ix.muxihuayi.cn

[G05] 继承
来源：http://ff.521024.cn

Py:   class Admin(User): pass
来源：http://za.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://si.nicolike.cn

JS:   class Admin extends User {}
来源：http://gx.9csxet.cn

TS:   class Admin extends User {}
来源：http://cu.hnjuh.cn

Java: class Admin extends User {}
来源：http://fv.nicolike.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ui.shxzskj.cn

Ruby: class Admin < User; end
来源：http://jj.haigaiapp.cn

C#:   class Admin : User {}
来源：http://nn.jctech888.com.cn

[G06] 重写方法
来源：http://nx.bookmarksfly.cn

Py:   def greet(self): return "admin"
来源：http://sv.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rm.colortex.cn

JS:   greet() { return "admin"; }
来源：http://nt.shtwfgs.cn

TS:   greet(): string { return "admin"; }
来源：http://ma.shtwfgs.cn

Java: @Override String greet() { return "admin"; }
来源：http://hp.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qu.yuntaijiaju.cn

Ruby: def greet; "admin"; end
来源：http://si.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://fk.yuexingan06.cn

[G07] 调用父类方法
来源：http://sf.panjiajie.cn

Py:   super().greet()
来源：http://wb.chemitech.net.cn

PHP:  parent::greet();
来源：http://gp.9csxet.cn

JS:   super.greet();
来源：http://rt.shxzskj.cn

TS:   super.greet();
来源：http://dx.szsharing.cn

Java: super.greet();
来源：http://ts.hnjuh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ri.colortex.cn

Ruby: super
来源：http://oi.521024.cn

C#:   base.Greet();
来源：http://bk.huixiangedu.cn

[G08] 静态方法与属性
来源：http://vy.panjiajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bp.yuntaijiaju.cn

PHP:  public static function f() {}
来源：http://yz.yuexingan06.cn

JS:   static f() {}
来源：http://nd.hnjuh.cn

TS:   static f(): void {}
来源：http://hk.9csxet.cn

Java: static void f() {}
来源：http://sq.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zy.panjiajie.cn

Ruby: def self.f; end
来源：http://rx.bjjhwx.cn

C#:   public static void F() {}
来源：http://gq.nszjky.cn

[G09] 接口 / 抽象类
来源：http://uj.wgjwhj.cn

Py:   from abc import ABC, abstractmethod
来源：http://aj.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bc.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mq.9csxet.cn

TS:   interface Shape { area(): number; }
来源：http://wp.nicolike.cn

Java: interface Shape { double area(); }
来源：http://ti.gzmigu.cn

Go:   type Shape interface { Area() float64 }
来源：http://du.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ff.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://vi.gzmigu.cn

[G10] 访问控制
来源：http://iw.jianghongdianzi.cn

Py:   约定 _protected / __private（不强制）
来源：http://ei.hahajie.cn

PHP:  public / protected / private
来源：http://ks.szsharing.cn

JS:   #private 字段；其余公开
来源：http://gt.panjiajie.cn

TS:   public / protected / private
来源：http://fd.shtwfgs.cn

Java: public / protected / private / 默认包级
来源：http://rt.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yb.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://si.lnxyls.cn

C#:   public / protected / private / internal
来源：http://nj.hnjuh.cn

[G11] getter / setter
来源：http://cm.wgjwhj.cn

Py:   @property 与 @x.setter
来源：http://vo.huixinmuqiang.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ri.szxytkj.cn

JS:   get name() { return this._name; }
来源：http://vl.bjjhwx.cn

TS:   get name(): string { return this._name; }
来源：http://kz.muxihuayi.cn

Java: public String getName() { return name; }
来源：http://ol.huanxung.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://aj.colortex.cn

Ruby: attr_accessor :name
来源：http://cy.chemitech.net.cn

C#:   public string Name { get; set; }
来源：http://hz.yuexingan06.cn

[G12] 对象转字符串
来源：http://jz.huixiangedu.cn

Py:   def __str__(self): return self.name
来源：http://wf.jctech888.com.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wq.bjjhwx.cn

JS:   toString() { return this.name; }
来源：http://qx.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://vc.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://yx.jctech888.com.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nv.jctech888.com.cn

Ruby: def to_s; @name; end
来源：http://iy.panjiajie.cn

C#:   public override string ToString() => Name;
来源：http://td.haigaiapp.cn

[G13] 判断对象类型
来源：http://lx.bjjhwx.cn

Py:   isinstance(u, User)
来源：http://fx.shxzukj.cn

PHP:  $u instanceof User
来源：http://fc.wgjwhj.cn

JS:   u instanceof User
来源：http://sh.yuntaijiaju.cn

TS:   u instanceof User
来源：http://mu.huixiangedu.cn

Java: u instanceof User
来源：http://vw.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fn.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://zd.newstarts.cn

C#:   u is User
来源：http://jh.yuexingan06.cn

[G14] 数据类 / record
来源：http://kt.muxihuayi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bv.chemitech.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://cw.jianghongdianzi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qv.jctech888.com.cn

TS:   type User = { name: string; age: number };
来源：http://vo.colortex.cn

Java: record User(String name, int age) {}
来源：http://ou.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://jc.haigaiapp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fw.huixinmuqiang.cn

C#:   record User(string Name, int Age);
来源：http://al.shxzskj.cn

[G15] 枚举
来源：http://fs.lnxyls.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dm.haigaiapp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yh.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nx.shxzukj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fj.521024.cn

Java: enum Color { RED, GREEN }
来源：http://iu.hnjuh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wq.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://by.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://eq.huanxung.cn

[G16] 对象转数组 / 字典
来源：http://eq.shxzskj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jf.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://lr.yuntaijiaju.cn

JS:   Object.entries(obj)
来源：http://ch.shtwfgs.cn

TS:   Object.entries(obj)
来源：http://vm.shxzukj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sv.huixiangedu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ha.shxzukj.cn

Ruby: obj.instance_variables
来源：http://yp.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://hx.huixinmuqiang.cn

================================================================================
来源：http://vu.haigaiapp.cn

H. 异常与错误处理
来源：http://xk.hahajie.cn

================================================================================
来源：http://oa.nszjky.cn

[H01] try / catch 基础
来源：http://oc.huixiangedu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cc.nicolike.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ao.szsharing.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ss.jctech888.com.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://va.hahajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oi.bjjhwx.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gj.huixinmuqiang.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pv.szsharing.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ft.jianghongdianzi.cn

[H02] finally / ensure 收尾
来源：http://mc.szxytkj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pi.newstarts.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ey.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://iu.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://eg.huixinmuqiang.cn

Java: try { f(); } finally { cleanup(); }
来源：http://re.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xi.huixiangedu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vl.gzmigu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yv.szsharing.cn

[H03] 主动抛出异常
来源：http://ym.szxytkj.cn

Py:   raise ValueError("错误信息")
来源：http://pj.haigaiapp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gu.yuntaijiaju.cn

JS:   throw new Error("错误信息");
来源：http://ak.szsharing.cn

TS:   throw new Error("错误信息");
来源：http://mq.chemitech.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ai.szsharing.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vv.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ft.bjjhwx.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gj.jianghongdianzi.cn

[H04] 自定义异常类型
来源：http://qo.colortex.cn

Py:   class MyError(Exception): pass
来源：http://ro.jianghongdianzi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vt.hahajie.cn

JS:   class MyError extends Error {}
来源：http://bi.huanxung.cn

TS:   class MyError extends Error {}
来源：http://at.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://hf.shtwfgs.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wg.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://va.chemitech.net.cn

C#:   class MyException : Exception {}
来源：http://gd.gzmigu.cn

[H05] 捕获特定类型
来源：http://xt.nicolike.cn

Py:   except ValueError as e:
来源：http://zw.nszjky.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hu.lnxyls.cn

JS:   if (e instanceof TypeError) {}
来源：http://sd.chemitech.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://br.colortex.cn

Java: catch (IOException | SQLException e) {}
来源：http://gh.lnxyls.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wi.huixinmuqiang.cn

Ruby: rescue ArgumentError => e
来源：http://sl.bjjhwx.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wo.shxzskj.cn

[H06] 可选值 / 空值安全访问
来源：http://sc.jctech888.com.cn

Py:   value = d.get("k") or default
来源：http://lf.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vt.jctech888.com.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mt.bookmarksfly.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jl.521024.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://id.lnxyls.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sk.nszjky.cn

Ruby: d&.dig(:a, :b)
来源：http://fp.9csxet.cn

C#:   obj?.A?.B ?? default
来源：http://fp.szsharing.cn

[H07] 断言
来源：http://pm.9csxet.cn

Py:   assert x > 0, "必须为正"
来源：http://yc.szsharing.cn

PHP:  assert($x > 0);
来源：http://fg.haigaiapp.cn

JS:   console.assert(x > 0);
来源：http://tb.jianghongdianzi.cn

TS:   console.assert(x > 0);
来源：http://wd.muxihuayi.cn

Java: assert x > 0 : "必须为正";
来源：http://bu.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jl.shtwfgs.cn

Ruby: raise "必须为正" unless x > 0
来源：http://je.9csxet.cn

C#:   Debug.Assert(x > 0);
来源：http://qz.newstarts.cn

[H08] 获取错误信息与堆栈
来源：http://jr.bjjhwx.cn

Py:   str(e);  traceback.format_exc()
来源：http://vd.huanxung.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dd.jianghongdianzi.cn

JS:   e.message;  e.stack
来源：http://xt.jctech888.com.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tb.gzmigu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ux.shxzskj.cn

Go:   err.Error()
来源：http://wc.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://mp.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://ga.szsharing.cn

[H09] 带错误码的异常
来源：http://va.shtwfgs.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mw.wgjwhj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ta.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cm.haigaiapp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lq.521024.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kd.bookmarksfly.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pg.nszjky.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sd.wgjwhj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lg.521024.cn

[H10] 资源自动释放
来源：http://xp.muxihuayi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vv.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gv.hahajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oa.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ka.9csxet.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dt.lnxyls.cn

Go:   defer f.Close()
来源：http://bj.bjjhwx.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tq.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fd.lnxyls.cn

================================================================================
来源：http://ff.shxzukj.cn

I. 正则表达式
来源：http://au.asd995.cn

================================================================================
来源：http://ge.muxihuayi.cn

[I01] 判断是否匹配
来源：http://jf.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://iv.hnjuh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jm.newstarts.cn

JS:   /\d+/.test(s)
来源：http://sz.hahajie.cn

TS:   /\d+/.test(s)
来源：http://yg.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hx.nicolike.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sm.yuexingan06.cn

Ruby: s.match?(/\d+/)
来源：http://uy.huanxung.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bg.yuntaijiaju.cn

[I02] 提取所有匹配
来源：http://yk.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://fy.haigaiapp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ey.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ys.szsharing.cn

TS:   s.match(/\d+/g)
来源：http://jz.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xf.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ys.huanxung.cn

Ruby: s.scan(/\d+/)
来源：http://vf.huixinmuqiang.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gd.huixiangedu.cn

[I03] 提取捕获分组
来源：http://ti.szxytkj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ir.jianghongdianzi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kw.9csxet.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://aa.huixiangedu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://su.9csxet.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dy.szxytkj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ha.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://br.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://at.colortex.cn

[I04] 正则替换
来源：http://cg.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jp.szsharing.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bf.jianghongdianzi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ln.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ph.yuntaijiaju.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yb.bookmarksfly.cn


<!-- 参考信息 -->