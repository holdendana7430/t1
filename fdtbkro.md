代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hx.wgjwhj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vq.muxihuayi.cn

[F11] 复制与移动文件
来源：http://bt.chemitech.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ni.bjjhwx.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fj.jianghongdianzi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ft.hahajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nt.yuexingan06.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ut.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nj.newstarts.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://em.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://rm.hnjuh.cn

[F12] CSV 读写
来源：http://uc.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kw.bookmarksfly.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xk.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jm.nicolike.cn

TS:   // 同上
来源：http://mh.huixinmuqiang.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hc.bjjhwx.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wg.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ym.shxzskj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fd.9csxet.cn

================================================================================
来源：http://np.chemitech.net.cn

G. 面向对象
来源：http://ex.nicolike.cn

================================================================================
来源：http://vj.shtwfgs.cn

[G01] 定义类
来源：http://pc.muxihuayi.cn

Py:   class User: pass
来源：http://sf.shxzukj.cn

PHP:  class User {}
来源：http://za.lnxyls.cn

JS:   class User {}
来源：http://ov.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://ch.shxzskj.cn

Java: class User {}
来源：http://mh.szsharing.cn

Go:   type User struct { Name string }
来源：http://ds.shxzukj.cn

Ruby: class User; end
来源：http://fc.szxytkj.cn

C#:   class User {}
来源：http://xd.nicolike.cn

[G02] 构造函数
来源：http://iv.yuntaijiaju.cn

Py:   def __init__(self, name): self.name = name
来源：http://nz.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://jc.szsharing.cn

JS:   constructor(name) { this.name = name; }
来源：http://qc.521024.cn

TS:   constructor(public name: string) {}
来源：http://fl.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://bz.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ga.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://if.szsharing.cn

C#:   public User(string name) { Name = name; }
来源：http://of.chemitech.net.cn

[G03] 实例属性
来源：http://jc.hahajie.cn

Py:   self.name = "x"
来源：http://eb.nszjky.cn

PHP:  public string $name = "x";
来源：http://mf.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://lf.shxzukj.cn

TS:   name: string = "x";
来源：http://qw.9csxet.cn

Java: private String name;
来源：http://km.jianghongdianzi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tq.szsharing.cn

Ruby: @name = "x"
来源：http://vk.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://am.gzmigu.cn

[G04] 定义方法
来源：http://iy.gzmigu.cn

Py:   def greet(self): return self.name
来源：http://nw.huixiangedu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ch.jctech888.com.cn

JS:   greet() { return this.name; }
来源：http://ln.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://kt.nszjky.cn

Java: String greet() { return name; }
来源：http://zc.colortex.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mj.haigaiapp.cn

Ruby: def greet; @name; end
来源：http://vv.szxytkj.cn

C#:   public string Greet() => Name;
来源：http://cf.yuntaijiaju.cn

[G05] 继承
来源：http://vr.szsharing.cn

Py:   class Admin(User): pass
来源：http://kk.9csxet.cn

PHP:  class Admin extends User {}
来源：http://zq.szxytkj.cn

JS:   class Admin extends User {}
来源：http://zw.huanxung.cn

TS:   class Admin extends User {}
来源：http://kv.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://ee.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ai.shxzskj.cn

Ruby: class Admin < User; end
来源：http://jm.lnxyls.cn

C#:   class Admin : User {}
来源：http://pv.newstarts.cn

[G06] 重写方法
来源：http://su.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://hl.nszjky.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jy.huixiangedu.cn

JS:   greet() { return "admin"; }
来源：http://vm.huixinmuqiang.cn

TS:   greet(): string { return "admin"; }
来源：http://ms.lnxyls.cn

Java: @Override String greet() { return "admin"; }
来源：http://uz.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qw.huixiangedu.cn

Ruby: def greet; "admin"; end
来源：http://pq.wgjwhj.cn

C#:   public override string Greet() => "admin";
来源：http://jd.hahajie.cn

[G07] 调用父类方法
来源：http://zu.shxzukj.cn

Py:   super().greet()
来源：http://nu.shtwfgs.cn

PHP:  parent::greet();
来源：http://os.jctech888.com.cn

JS:   super.greet();
来源：http://aq.hahajie.cn

TS:   super.greet();
来源：http://rn.shtwfgs.cn

Java: super.greet();
来源：http://bx.huixinmuqiang.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cj.bjjhwx.cn

Ruby: super
来源：http://in.hahajie.cn

C#:   base.Greet();
来源：http://wb.bjjhwx.cn

[G08] 静态方法与属性
来源：http://bf.szxytkj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fl.chemitech.net.cn

PHP:  public static function f() {}
来源：http://tv.shxzukj.cn

JS:   static f() {}
来源：http://qr.shtwfgs.cn

TS:   static f(): void {}
来源：http://ja.shtwfgs.cn

Java: static void f() {}
来源：http://bw.bookmarksfly.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dj.haigaiapp.cn

Ruby: def self.f; end
来源：http://sr.521024.cn

C#:   public static void F() {}
来源：http://nw.jianghongdianzi.cn

[G09] 接口 / 抽象类
来源：http://ax.shxzukj.cn

Py:   from abc import ABC, abstractmethod
来源：http://kj.jianghongdianzi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fo.asd995.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lu.wgjwhj.cn

TS:   interface Shape { area(): number; }
来源：http://ye.haigaiapp.cn

Java: interface Shape { double area(); }
来源：http://go.gzmigu.cn

Go:   type Shape interface { Area() float64 }
来源：http://jm.521024.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://og.shxzukj.cn

C#:   interface IShape { double Area(); }
来源：http://oy.shtwfgs.cn

[G10] 访问控制
来源：http://zt.huixiangedu.cn

Py:   约定 _protected / __private（不强制）
来源：http://vw.huixinmuqiang.cn

PHP:  public / protected / private
来源：http://bd.wgjwhj.cn

JS:   #private 字段；其余公开
来源：http://ty.jianghongdianzi.cn

TS:   public / protected / private
来源：http://ei.shxzskj.cn

Java: public / protected / private / 默认包级
来源：http://ea.shxzskj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ml.hahajie.cn

Ruby: public / protected / private
来源：http://py.huixiangedu.cn

C#:   public / protected / private / internal
来源：http://ec.bookmarksfly.cn

[G11] getter / setter
来源：http://tg.yuntaijiaju.cn

Py:   @property 与 @x.setter
来源：http://cr.chemitech.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://se.shxzskj.cn

JS:   get name() { return this._name; }
来源：http://hq.yuntaijiaju.cn

TS:   get name(): string { return this._name; }
来源：http://lw.newstarts.cn

Java: public String getName() { return name; }
来源：http://ki.haigaiapp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dl.bjjhwx.cn

Ruby: attr_accessor :name
来源：http://oc.nicolike.cn

C#:   public string Name { get; set; }
来源：http://fa.bjjhwx.cn

[G12] 对象转字符串
来源：http://qe.panjiajie.cn

Py:   def __str__(self): return self.name
来源：http://rx.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vk.colortex.cn

JS:   toString() { return this.name; }
来源：http://co.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://au.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://co.nszjky.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xo.yuexingan06.cn

Ruby: def to_s; @name; end
来源：http://oh.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://zh.huanxung.cn

[G13] 判断对象类型
来源：http://xi.chemitech.net.cn

Py:   isinstance(u, User)
来源：http://bg.szxytkj.cn

PHP:  $u instanceof User
来源：http://ml.gzmigu.cn

JS:   u instanceof User
来源：http://rc.nszjky.cn

TS:   u instanceof User
来源：http://li.haigaiapp.cn

Java: u instanceof User
来源：http://ba.haigaiapp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tq.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://zy.shxzskj.cn

C#:   u is User
来源：http://mv.chemitech.net.cn

[G14] 数据类 / record
来源：http://el.asd995.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ue.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://ww.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rg.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://xo.asd995.cn

Java: record User(String name, int age) {}
来源：http://dy.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://gt.bookmarksfly.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wx.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://jm.nicolike.cn

[G15] 枚举
来源：http://pu.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tm.nicolike.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ap.hahajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tu.yuntaijiaju.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xr.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://dx.jianghongdianzi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fh.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://bd.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bs.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://kb.hnjuh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://it.bjjhwx.cn

PHP:  get_object_vars($obj);
来源：http://nn.haigaiapp.cn

JS:   Object.entries(obj)
来源：http://qs.huanxung.cn

TS:   Object.entries(obj)
来源：http://xo.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rp.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fi.hnjuh.cn

Ruby: obj.instance_variables
来源：http://cr.szxytkj.cn

C#:   // 用反射或 System.Text.Json
来源：http://bl.shxzukj.cn

================================================================================
来源：http://ac.shxzskj.cn

H. 异常与错误处理
来源：http://nj.muxihuayi.cn

================================================================================
来源：http://fr.9csxet.cn

[H01] try / catch 基础
来源：http://gq.panjiajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ll.yuntaijiaju.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yr.nicolike.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yn.bjjhwx.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ni.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bi.huixiangedu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vc.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ek.lnxyls.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ei.lnxyls.cn

[H02] finally / ensure 收尾
来源：http://bd.nicolike.cn

Py:   try: f()⏎finally: cleanup()
来源：http://at.huixiangedu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fg.521024.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mm.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nt.shxzukj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://nf.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vn.newstarts.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tq.bjjhwx.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ck.hnjuh.cn

[H03] 主动抛出异常
来源：http://ed.gzmigu.cn

Py:   raise ValueError("错误信息")
来源：http://nq.wgjwhj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zv.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://ht.yuntaijiaju.cn

TS:   throw new Error("错误信息");
来源：http://lp.shtwfgs.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rj.huixinmuqiang.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ax.szxytkj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lk.nicolike.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wk.shxzukj.cn

[H04] 自定义异常类型
来源：http://nb.gzmigu.cn

Py:   class MyError(Exception): pass
来源：http://gr.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uv.muxihuayi.cn

JS:   class MyError extends Error {}
来源：http://uk.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://za.nicolike.cn

Java: class MyException extends RuntimeException {}
来源：http://kr.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ky.huixinmuqiang.cn

Ruby: class MyError < StandardError; end
来源：http://wn.lnxyls.cn

C#:   class MyException : Exception {}
来源：http://yj.haigaiapp.cn

[H05] 捕获特定类型
来源：http://gm.haigaiapp.cn

Py:   except ValueError as e:
来源：http://cd.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fz.wgjwhj.cn

JS:   if (e instanceof TypeError) {}
来源：http://vr.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://ka.shtwfgs.cn

Java: catch (IOException | SQLException e) {}
来源：http://bo.asd995.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bd.shxzukj.cn

Ruby: rescue ArgumentError => e
来源：http://pn.chemitech.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bd.haigaiapp.cn

[H06] 可选值 / 空值安全访问
来源：http://tr.jctech888.com.cn

Py:   value = d.get("k") or default
来源：http://hk.newstarts.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wi.nszjky.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yl.haigaiapp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nh.szsharing.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qx.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ia.jianghongdianzi.cn

Ruby: d&.dig(:a, :b)
来源：http://qw.huixiangedu.cn

C#:   obj?.A?.B ?? default
来源：http://ay.szsharing.cn

[H07] 断言
来源：http://wu.asd995.cn

Py:   assert x > 0, "必须为正"
来源：http://wb.9csxet.cn

PHP:  assert($x > 0);
来源：http://vx.asd995.cn

JS:   console.assert(x > 0);
来源：http://er.szsharing.cn

TS:   console.assert(x > 0);
来源：http://hs.szsharing.cn

Java: assert x > 0 : "必须为正";
来源：http://zj.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nb.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fu.haigaiapp.cn

C#:   Debug.Assert(x > 0);
来源：http://nh.colortex.cn

[H08] 获取错误信息与堆栈
来源：http://nm.shxzskj.cn

Py:   str(e);  traceback.format_exc()
来源：http://jy.9csxet.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://iy.colortex.cn

JS:   e.message;  e.stack
来源：http://tj.jctech888.com.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ze.huixiangedu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ok.huanxung.cn

Go:   err.Error()
来源：http://kg.panjiajie.cn

Ruby: e.message;  e.backtrace
来源：http://xj.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://tf.bjjhwx.cn

[H09] 带错误码的异常
来源：http://he.asd995.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nr.chemitech.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tu.9csxet.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pn.szsharing.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ui.lnxyls.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ko.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kk.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sj.shxzskj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ad.yuexingan06.cn

[H10] 资源自动释放
来源：http://ni.yuntaijiaju.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fg.jianghongdianzi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eg.haigaiapp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bg.shtwfgs.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xr.bookmarksfly.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dn.wgjwhj.cn

Go:   defer f.Close()
来源：http://uy.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cx.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lx.521024.cn

================================================================================
来源：http://py.shxzukj.cn

I. 正则表达式
来源：http://vd.colortex.cn

================================================================================
来源：http://uo.jctech888.com.cn

[I01] 判断是否匹配
来源：http://xo.jianghongdianzi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ed.muxihuayi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ar.shxzskj.cn

JS:   /\d+/.test(s)
来源：http://mh.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://hc.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qr.nszjky.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wh.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://ky.jctech888.com.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ee.newstarts.cn

[I02] 提取所有匹配
来源：http://mr.nszjky.cn

Py:   re.findall(r"\d+", s)
来源：http://gp.szsharing.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ez.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kr.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://bk.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lh.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qg.shxzskj.cn

Ruby: s.scan(/\d+/)
来源：http://ff.haigaiapp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ai.huixiangedu.cn

[I03] 提取捕获分组
来源：http://nh.nicolike.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ts.shxzskj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nt.colortex.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ba.huixiangedu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ju.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wb.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wu.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sm.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://br.asd995.cn

[I04] 正则替换
来源：http://rj.wgjwhj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://te.hnjuh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lo.wgjwhj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fh.szxytkj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sh.yuntaijiaju.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sb.yuexingan06.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ad.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gw.bjjhwx.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tf.nicolike.cn

[I05] 按正则拆分
来源：http://oy.521024.cn


<!-- 参考信息 -->