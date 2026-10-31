代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ep.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gg.haigaiapp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qr.wgjwhj.cn

[F12] CSV 读写
来源：http://oc.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gu.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://uf.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yy.yuexingan06.cn

TS:   // 同上
来源：http://ui.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ba.muxihuayi.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ey.szxytkj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mr.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://yv.szsharing.cn

================================================================================
来源：http://jy.jctech888.com.cn

G. 面向对象
来源：http://ux.hahajie.cn

================================================================================
来源：http://ae.huixinmuqiang.cn

[G01] 定义类
来源：http://ie.huixiangedu.cn

Py:   class User: pass
来源：http://ah.hahajie.cn

PHP:  class User {}
来源：http://fo.bjjhwx.cn

JS:   class User {}
来源：http://li.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://bs.yuntaijiaju.cn

Java: class User {}
来源：http://bc.chemitech.net.cn

Go:   type User struct { Name string }
来源：http://ag.bookmarksfly.cn

Ruby: class User; end
来源：http://bi.jianghongdianzi.cn

C#:   class User {}
来源：http://bs.hahajie.cn

[G02] 构造函数
来源：http://lu.szsharing.cn

Py:   def __init__(self, name): self.name = name
来源：http://bq.huixiangedu.cn

PHP:  public function __construct(public string $name) {}
来源：http://fx.huanxung.cn

JS:   constructor(name) { this.name = name; }
来源：http://gz.shxzukj.cn

TS:   constructor(public name: string) {}
来源：http://zp.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://kv.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fu.shxzukj.cn

Ruby: def initialize(name); @name = name; end
来源：http://sx.nicolike.cn

C#:   public User(string name) { Name = name; }
来源：http://il.gzmigu.cn

[G03] 实例属性
来源：http://do.haigaiapp.cn

Py:   self.name = "x"
来源：http://gn.asd995.cn

PHP:  public string $name = "x";
来源：http://gu.szsharing.cn

JS:   this.name = "x";
来源：http://wh.yuexingan06.cn

TS:   name: string = "x";
来源：http://rm.shxzukj.cn

Java: private String name;
来源：http://uf.yuntaijiaju.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gn.yuntaijiaju.cn

Ruby: @name = "x"
来源：http://cx.bookmarksfly.cn

C#:   public string Name { get; set; } = "x";
来源：http://lw.nicolike.cn

[G04] 定义方法
来源：http://op.colortex.cn

Py:   def greet(self): return self.name
来源：http://ux.shxzukj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gx.gzmigu.cn

JS:   greet() { return this.name; }
来源：http://ye.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://ld.bookmarksfly.cn

Java: String greet() { return name; }
来源：http://wq.huanxung.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://aj.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://nk.521024.cn

C#:   public string Greet() => Name;
来源：http://fg.panjiajie.cn

[G05] 继承
来源：http://wu.lnxyls.cn

Py:   class Admin(User): pass
来源：http://fw.bookmarksfly.cn

PHP:  class Admin extends User {}
来源：http://xt.huixinmuqiang.cn

JS:   class Admin extends User {}
来源：http://np.colortex.cn

TS:   class Admin extends User {}
来源：http://fi.huanxung.cn

Java: class Admin extends User {}
来源：http://sz.huixinmuqiang.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ge.hnjuh.cn

Ruby: class Admin < User; end
来源：http://cf.szsharing.cn

C#:   class Admin : User {}
来源：http://ce.hahajie.cn

[G06] 重写方法
来源：http://uk.panjiajie.cn

Py:   def greet(self): return "admin"
来源：http://vv.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://na.huanxung.cn

JS:   greet() { return "admin"; }
来源：http://iw.lnxyls.cn

TS:   greet(): string { return "admin"; }
来源：http://ej.wgjwhj.cn

Java: @Override String greet() { return "admin"; }
来源：http://ve.newstarts.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://su.nicolike.cn

Ruby: def greet; "admin"; end
来源：http://do.panjiajie.cn

C#:   public override string Greet() => "admin";
来源：http://is.lnxyls.cn

[G07] 调用父类方法
来源：http://ob.haigaiapp.cn

Py:   super().greet()
来源：http://gh.nicolike.cn

PHP:  parent::greet();
来源：http://wu.bookmarksfly.cn

JS:   super.greet();
来源：http://hc.yuntaijiaju.cn

TS:   super.greet();
来源：http://la.huanxung.cn

Java: super.greet();
来源：http://mh.huixiangedu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rv.nicolike.cn

Ruby: super
来源：http://ym.newstarts.cn

C#:   base.Greet();
来源：http://mm.wgjwhj.cn

[G08] 静态方法与属性
来源：http://ke.huixiangedu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dw.wgjwhj.cn

PHP:  public static function f() {}
来源：http://wa.hnjuh.cn

JS:   static f() {}
来源：http://jy.huixinmuqiang.cn

TS:   static f(): void {}
来源：http://pl.jianghongdianzi.cn

Java: static void f() {}
来源：http://dx.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://us.9csxet.cn

Ruby: def self.f; end
来源：http://ta.huixinmuqiang.cn

C#:   public static void F() {}
来源：http://hj.asd995.cn

[G09] 接口 / 抽象类
来源：http://qc.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://pd.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bd.jianghongdianzi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lz.hahajie.cn

TS:   interface Shape { area(): number; }
来源：http://yd.bookmarksfly.cn

Java: interface Shape { double area(); }
来源：http://qy.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://fg.shtwfgs.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mx.bjjhwx.cn

C#:   interface IShape { double Area(); }
来源：http://ew.szxytkj.cn

[G10] 访问控制
来源：http://pe.hnjuh.cn

Py:   约定 _protected / __private（不强制）
来源：http://tb.wgjwhj.cn

PHP:  public / protected / private
来源：http://kl.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://ed.huixinmuqiang.cn

TS:   public / protected / private
来源：http://wz.lnxyls.cn

Java: public / protected / private / 默认包级
来源：http://uf.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pv.huanxung.cn

Ruby: public / protected / private
来源：http://hy.huixinmuqiang.cn

C#:   public / protected / private / internal
来源：http://cs.muxihuayi.cn

[G11] getter / setter
来源：http://zl.wgjwhj.cn

Py:   @property 与 @x.setter
来源：http://kk.huixinmuqiang.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dh.haigaiapp.cn

JS:   get name() { return this._name; }
来源：http://xp.shtwfgs.cn

TS:   get name(): string { return this._name; }
来源：http://tz.nszjky.cn

Java: public String getName() { return name; }
来源：http://bl.huixinmuqiang.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ox.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://fn.newstarts.cn

C#:   public string Name { get; set; }
来源：http://ex.szxytkj.cn

[G12] 对象转字符串
来源：http://ra.newstarts.cn

Py:   def __str__(self): return self.name
来源：http://pv.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gp.9csxet.cn

JS:   toString() { return this.name; }
来源：http://rt.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://qh.shxzskj.cn

Java: @Override public String toString() { return name; }
来源：http://vy.shtwfgs.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lz.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://uz.shxzukj.cn

C#:   public override string ToString() => Name;
来源：http://jp.shxzskj.cn

[G13] 判断对象类型
来源：http://za.jianghongdianzi.cn

Py:   isinstance(u, User)
来源：http://eo.haigaiapp.cn

PHP:  $u instanceof User
来源：http://tg.yuntaijiaju.cn

JS:   u instanceof User
来源：http://ib.lnxyls.cn

TS:   u instanceof User
来源：http://rc.huixiangedu.cn

Java: u instanceof User
来源：http://af.asd995.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://am.panjiajie.cn

Ruby: u.is_a?(User)
来源：http://sn.shxzukj.cn

C#:   u is User
来源：http://bb.nszjky.cn

[G14] 数据类 / record
来源：http://ed.hahajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vl.newstarts.cn

PHP:  // 用 readonly 属性模拟
来源：http://kg.yuntaijiaju.cn

JS:   // 无内置：普通类或对象字面量
来源：http://of.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://dg.9csxet.cn

Java: record User(String name, int age) {}
来源：http://dq.szxytkj.cn

Go:   type User struct { Name string; Age int }
来源：http://bq.lnxyls.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kp.huixiangedu.cn

C#:   record User(string Name, int Age);
来源：http://oe.shtwfgs.cn

[G15] 枚举
来源：http://cy.szxytkj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vo.yuntaijiaju.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fr.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dz.huixiangedu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lt.szxytkj.cn

Java: enum Color { RED, GREEN }
来源：http://ub.newstarts.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ge.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://vt.bookmarksfly.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zd.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://ad.szxytkj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ti.hnjuh.cn

PHP:  get_object_vars($obj);
来源：http://sp.yuexingan06.cn

JS:   Object.entries(obj)
来源：http://cc.gzmigu.cn

TS:   Object.entries(obj)
来源：http://vt.asd995.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jc.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ye.hahajie.cn

Ruby: obj.instance_variables
来源：http://dz.huixinmuqiang.cn

C#:   // 用反射或 System.Text.Json
来源：http://ih.shxzukj.cn

================================================================================
来源：http://rs.yuexingan06.cn

H. 异常与错误处理
来源：http://ha.huixinmuqiang.cn

================================================================================
来源：http://ji.bookmarksfly.cn

[H01] try / catch 基础
来源：http://fm.hahajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vp.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gn.colortex.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://at.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yo.colortex.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rg.shxzskj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ho.hahajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ei.yuexingan06.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://op.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://sf.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ad.colortex.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rw.521024.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bm.wgjwhj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ia.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zp.hahajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://py.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qd.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ds.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://yj.colortex.cn

Py:   raise ValueError("错误信息")
来源：http://ib.shtwfgs.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://on.yuntaijiaju.cn

JS:   throw new Error("错误信息");
来源：http://bo.chemitech.net.cn

TS:   throw new Error("错误信息");
来源：http://gd.shxzskj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://og.huixinmuqiang.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ui.huixiangedu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ne.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pf.hahajie.cn

[H04] 自定义异常类型
来源：http://ll.newstarts.cn

Py:   class MyError(Exception): pass
来源：http://ah.colortex.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xj.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://bb.huixiangedu.cn

TS:   class MyError extends Error {}
来源：http://so.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://ue.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rb.huixiangedu.cn

Ruby: class MyError < StandardError; end
来源：http://gc.szxytkj.cn

C#:   class MyException : Exception {}
来源：http://eb.lnxyls.cn

[H05] 捕获特定类型
来源：http://ev.asd995.cn

Py:   except ValueError as e:
来源：http://vj.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mu.panjiajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://gy.muxihuayi.cn

TS:   if (e instanceof TypeError) {}
来源：http://zp.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://fc.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dx.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://gp.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gf.haigaiapp.cn

[H06] 可选值 / 空值安全访问
来源：http://mh.lnxyls.cn

Py:   value = d.get("k") or default
来源：http://qk.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kk.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wz.huixiangedu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://nh.hahajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mj.yuntaijiaju.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ds.jianghongdianzi.cn

Ruby: d&.dig(:a, :b)
来源：http://th.lnxyls.cn

C#:   obj?.A?.B ?? default
来源：http://ir.yuexingan06.cn

[H07] 断言
来源：http://me.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://fz.szsharing.cn

PHP:  assert($x > 0);
来源：http://sl.hahajie.cn

JS:   console.assert(x > 0);
来源：http://st.521024.cn

TS:   console.assert(x > 0);
来源：http://ip.haigaiapp.cn

Java: assert x > 0 : "必须为正";
来源：http://za.bjjhwx.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wc.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xo.shxzskj.cn

C#:   Debug.Assert(x > 0);
来源：http://yv.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://tp.huanxung.cn

Py:   str(e);  traceback.format_exc()
来源：http://ua.shtwfgs.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bx.muxihuayi.cn

JS:   e.message;  e.stack
来源：http://fq.asd995.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vk.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dz.gzmigu.cn

Go:   err.Error()
来源：http://sx.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://dz.hahajie.cn

C#:   e.Message;  e.StackTrace
来源：http://qa.lnxyls.cn

[H09] 带错误码的异常
来源：http://cu.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kc.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mq.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ar.szxytkj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kz.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yg.hahajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mr.newstarts.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ox.nicolike.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lb.hnjuh.cn

[H10] 资源自动释放
来源：http://vi.jianghongdianzi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bt.shtwfgs.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ek.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oz.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yo.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://of.shtwfgs.cn

Go:   defer f.Close()
来源：http://tm.yuexingan06.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bm.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tv.shxzukj.cn

================================================================================
来源：http://jv.wgjwhj.cn

I. 正则表达式
来源：http://dg.szxytkj.cn

================================================================================
来源：http://tb.szxytkj.cn

[I01] 判断是否匹配
来源：http://ex.yuntaijiaju.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jb.jianghongdianzi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tf.szsharing.cn

JS:   /\d+/.test(s)
来源：http://wd.asd995.cn

TS:   /\d+/.test(s)
来源：http://sc.521024.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ob.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pp.bookmarksfly.cn

Ruby: s.match?(/\d+/)
来源：http://jm.shxzskj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hq.szxytkj.cn

[I02] 提取所有匹配
来源：http://kn.huanxung.cn

Py:   re.findall(r"\d+", s)
来源：http://cg.shxzskj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fu.huixiangedu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://je.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://us.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ic.nszjky.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dl.9csxet.cn

Ruby: s.scan(/\d+/)
来源：http://ip.9csxet.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jf.bjjhwx.cn

[I03] 提取捕获分组
来源：http://fs.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yh.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cu.bjjhwx.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cp.shtwfgs.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sw.haigaiapp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mo.yuexingan06.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dx.jianghongdianzi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xe.jianghongdianzi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wg.asd995.cn

[I04] 正则替换
来源：http://ss.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://oi.521024.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sm.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rh.yuexingan06.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qu.szsharing.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ul.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ml.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rr.lnxyls.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xy.bookmarksfly.cn

[I05] 按正则拆分
来源：http://pm.wgjwhj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://re.jctech888.com.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ex.jianghongdianzi.cn

JS:   s.split(/\s*,\s*/)
来源：http://hv.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://hj.nicolike.cn

Java: s.split("\\s*,\\s*")
来源：http://ne.huanxung.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vg.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qz.hahajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://af.lnxyls.cn


<!-- 参考信息 -->