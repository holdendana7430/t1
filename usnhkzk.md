代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yo.lnxyls.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yj.jctech888.com.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mg.yuntaijiaju.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fo.gzmigu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://um.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ty.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jf.bookmarksfly.cn

[F12] CSV 读写
来源：http://ph.bjjhwx.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://np.shtwfgs.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jw.yuntaijiaju.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uo.muxihuayi.cn

TS:   // 同上
来源：http://py.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fw.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://jm.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gx.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qh.9csxet.cn

================================================================================
来源：http://aj.9csxet.cn

G. 面向对象
来源：http://hl.yuntaijiaju.cn

================================================================================
来源：http://on.huixiangedu.cn

[G01] 定义类
来源：http://zh.szxytkj.cn

Py:   class User: pass
来源：http://ih.jctech888.com.cn

PHP:  class User {}
来源：http://sg.haigaiapp.cn

JS:   class User {}
来源：http://fq.szxytkj.cn

TS:   class User { name: string = ""; }
来源：http://mx.gzmigu.cn

Java: class User {}
来源：http://vl.yuntaijiaju.cn

Go:   type User struct { Name string }
来源：http://le.szxytkj.cn

Ruby: class User; end
来源：http://dt.yuntaijiaju.cn

C#:   class User {}
来源：http://ik.newstarts.cn

[G02] 构造函数
来源：http://ok.chemitech.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://ge.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://rd.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://mz.haigaiapp.cn

TS:   constructor(public name: string) {}
来源：http://ar.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://mw.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rk.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://yn.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://cq.lnxyls.cn

[G03] 实例属性
来源：http://qm.wgjwhj.cn

Py:   self.name = "x"
来源：http://ez.haigaiapp.cn

PHP:  public string $name = "x";
来源：http://br.huixiangedu.cn

JS:   this.name = "x";
来源：http://dw.colortex.cn

TS:   name: string = "x";
来源：http://iz.szsharing.cn

Java: private String name;
来源：http://cu.nszjky.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xe.9csxet.cn

Ruby: @name = "x"
来源：http://nj.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://nf.bjjhwx.cn

[G04] 定义方法
来源：http://ej.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://xj.wgjwhj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bh.nicolike.cn

JS:   greet() { return this.name; }
来源：http://vq.chemitech.net.cn

TS:   greet(): string { return this.name; }
来源：http://mf.9csxet.cn

Java: String greet() { return name; }
来源：http://wi.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tt.gzmigu.cn

Ruby: def greet; @name; end
来源：http://dd.jianghongdianzi.cn

C#:   public string Greet() => Name;
来源：http://hb.nicolike.cn

[G05] 继承
来源：http://iy.huanxung.cn

Py:   class Admin(User): pass
来源：http://zi.muxihuayi.cn

PHP:  class Admin extends User {}
来源：http://fo.huanxung.cn

JS:   class Admin extends User {}
来源：http://lw.newstarts.cn

TS:   class Admin extends User {}
来源：http://sh.huixiangedu.cn

Java: class Admin extends User {}
来源：http://ts.nicolike.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ze.gzmigu.cn

Ruby: class Admin < User; end
来源：http://wc.shtwfgs.cn

C#:   class Admin : User {}
来源：http://ua.colortex.cn

[G06] 重写方法
来源：http://hy.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://lq.shtwfgs.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xg.shtwfgs.cn

JS:   greet() { return "admin"; }
来源：http://gi.shxzukj.cn

TS:   greet(): string { return "admin"; }
来源：http://fk.bookmarksfly.cn

Java: @Override String greet() { return "admin"; }
来源：http://ep.huixinmuqiang.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vd.muxihuayi.cn

Ruby: def greet; "admin"; end
来源：http://gk.wgjwhj.cn

C#:   public override string Greet() => "admin";
来源：http://ay.nszjky.cn

[G07] 调用父类方法
来源：http://tp.jianghongdianzi.cn

Py:   super().greet()
来源：http://wt.muxihuayi.cn

PHP:  parent::greet();
来源：http://qa.bookmarksfly.cn

JS:   super.greet();
来源：http://kk.huixinmuqiang.cn

TS:   super.greet();
来源：http://uw.newstarts.cn

Java: super.greet();
来源：http://ly.bookmarksfly.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://in.hahajie.cn

Ruby: super
来源：http://fd.haigaiapp.cn

C#:   base.Greet();
来源：http://wo.lnxyls.cn

[G08] 静态方法与属性
来源：http://av.jianghongdianzi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ym.szsharing.cn

PHP:  public static function f() {}
来源：http://py.szxytkj.cn

JS:   static f() {}
来源：http://ye.jctech888.com.cn

TS:   static f(): void {}
来源：http://uo.huanxung.cn

Java: static void f() {}
来源：http://oc.asd995.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ql.huixiangedu.cn

Ruby: def self.f; end
来源：http://yi.muxihuayi.cn

C#:   public static void F() {}
来源：http://pr.szsharing.cn

[G09] 接口 / 抽象类
来源：http://td.yuexingan06.cn

Py:   from abc import ABC, abstractmethod
来源：http://ld.huixinmuqiang.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ht.jianghongdianzi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://gi.newstarts.cn

TS:   interface Shape { area(): number; }
来源：http://de.szsharing.cn

Java: interface Shape { double area(); }
来源：http://bk.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://ue.asd995.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dy.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://gt.huixinmuqiang.cn

[G10] 访问控制
来源：http://lu.yuexingan06.cn

Py:   约定 _protected / __private（不强制）
来源：http://rh.colortex.cn

PHP:  public / protected / private
来源：http://ts.gzmigu.cn

JS:   #private 字段；其余公开
来源：http://yt.chemitech.net.cn

TS:   public / protected / private
来源：http://kz.shtwfgs.cn

Java: public / protected / private / 默认包级
来源：http://jb.chemitech.net.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://re.nicolike.cn

Ruby: public / protected / private
来源：http://ux.colortex.cn

C#:   public / protected / private / internal
来源：http://sb.jctech888.com.cn

[G11] getter / setter
来源：http://sy.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://py.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://us.nszjky.cn

JS:   get name() { return this._name; }
来源：http://zo.hahajie.cn

TS:   get name(): string { return this._name; }
来源：http://jl.hnjuh.cn

Java: public String getName() { return name; }
来源：http://lo.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lg.gzmigu.cn

Ruby: attr_accessor :name
来源：http://on.chemitech.net.cn

C#:   public string Name { get; set; }
来源：http://yb.asd995.cn

[G12] 对象转字符串
来源：http://ey.asd995.cn

Py:   def __str__(self): return self.name
来源：http://ky.shtwfgs.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lf.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://mr.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://pw.lnxyls.cn

Java: @Override public String toString() { return name; }
来源：http://no.shxzukj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qm.shtwfgs.cn

Ruby: def to_s; @name; end
来源：http://me.jctech888.com.cn

C#:   public override string ToString() => Name;
来源：http://pk.huixiangedu.cn

[G13] 判断对象类型
来源：http://xg.muxihuayi.cn

Py:   isinstance(u, User)
来源：http://ut.jctech888.com.cn

PHP:  $u instanceof User
来源：http://rp.jianghongdianzi.cn

JS:   u instanceof User
来源：http://iu.yuntaijiaju.cn

TS:   u instanceof User
来源：http://vu.asd995.cn

Java: u instanceof User
来源：http://ti.panjiajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dc.szsharing.cn

Ruby: u.is_a?(User)
来源：http://jn.haigaiapp.cn

C#:   u is User
来源：http://qg.huanxung.cn

[G14] 数据类 / record
来源：http://yq.9csxet.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ma.huixinmuqiang.cn

PHP:  // 用 readonly 属性模拟
来源：http://cz.gzmigu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rg.shxzskj.cn

TS:   type User = { name: string; age: number };
来源：http://hw.szxytkj.cn

Java: record User(String name, int age) {}
来源：http://nr.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://gz.huixinmuqiang.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ie.lnxyls.cn

C#:   record User(string Name, int Age);
来源：http://bb.shxzukj.cn

[G15] 枚举
来源：http://ox.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hh.shtwfgs.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ay.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wv.shxzukj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://od.szsharing.cn

Java: enum Color { RED, GREEN }
来源：http://ce.bjjhwx.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ju.chemitech.net.cn

Ruby: Color = %i[red green].freeze
来源：http://wb.jianghongdianzi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ic.huanxung.cn

[G16] 对象转数组 / 字典
来源：http://cd.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ty.panjiajie.cn

PHP:  get_object_vars($obj);
来源：http://rd.shxzskj.cn

JS:   Object.entries(obj)
来源：http://zb.szsharing.cn

TS:   Object.entries(obj)
来源：http://oz.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yz.szsharing.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wi.hnjuh.cn

Ruby: obj.instance_variables
来源：http://zn.wgjwhj.cn

C#:   // 用反射或 System.Text.Json
来源：http://uv.panjiajie.cn

================================================================================
来源：http://xp.yuntaijiaju.cn

H. 异常与错误处理
来源：http://fx.szxytkj.cn

================================================================================
来源：http://ev.shtwfgs.cn

[H01] try / catch 基础
来源：http://wu.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mz.colortex.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sr.yuexingan06.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sa.lnxyls.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nc.jctech888.com.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://kj.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yy.szxytkj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ta.lnxyls.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zn.hnjuh.cn

[H02] finally / ensure 收尾
来源：http://tq.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://eb.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cy.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rx.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wy.jianghongdianzi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://of.newstarts.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rw.gzmigu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zi.wgjwhj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lq.shtwfgs.cn

[H03] 主动抛出异常
来源：http://hc.yuexingan06.cn

Py:   raise ValueError("错误信息")
来源：http://ko.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xa.szsharing.cn

JS:   throw new Error("错误信息");
来源：http://hh.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://ic.huanxung.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://do.jctech888.com.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://se.huixinmuqiang.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://do.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ha.yuexingan06.cn

[H04] 自定义异常类型
来源：http://bd.hahajie.cn

Py:   class MyError(Exception): pass
来源：http://go.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bw.jctech888.com.cn

JS:   class MyError extends Error {}
来源：http://ym.nicolike.cn

TS:   class MyError extends Error {}
来源：http://kz.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://ed.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://un.shxzskj.cn

Ruby: class MyError < StandardError; end
来源：http://ww.521024.cn

C#:   class MyException : Exception {}
来源：http://ul.bookmarksfly.cn

[H05] 捕获特定类型
来源：http://ar.newstarts.cn

Py:   except ValueError as e:
来源：http://pl.9csxet.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ai.9csxet.cn

JS:   if (e instanceof TypeError) {}
来源：http://wy.huanxung.cn

TS:   if (e instanceof TypeError) {}
来源：http://uf.asd995.cn

Java: catch (IOException | SQLException e) {}
来源：http://na.bjjhwx.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rt.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://fo.colortex.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qh.szxytkj.cn

[H06] 可选值 / 空值安全访问
来源：http://bj.huanxung.cn

Py:   value = d.get("k") or default
来源：http://tt.bookmarksfly.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ev.yuexingan06.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ib.bookmarksfly.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xq.shtwfgs.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ml.bjjhwx.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nj.bjjhwx.cn

Ruby: d&.dig(:a, :b)
来源：http://wu.bookmarksfly.cn

C#:   obj?.A?.B ?? default
来源：http://uv.newstarts.cn

[H07] 断言
来源：http://dm.nszjky.cn

Py:   assert x > 0, "必须为正"
来源：http://gr.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://lf.yuexingan06.cn

JS:   console.assert(x > 0);
来源：http://tc.szsharing.cn

TS:   console.assert(x > 0);
来源：http://bq.bjjhwx.cn

Java: assert x > 0 : "必须为正";
来源：http://gn.haigaiapp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bi.huixiangedu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yq.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://xl.yuntaijiaju.cn

[H08] 获取错误信息与堆栈
来源：http://fj.szxytkj.cn

Py:   str(e);  traceback.format_exc()
来源：http://tk.huixinmuqiang.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rl.nszjky.cn

JS:   e.message;  e.stack
来源：http://ul.huixinmuqiang.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lc.yuexingan06.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rb.huixiangedu.cn

Go:   err.Error()
来源：http://as.haigaiapp.cn

Ruby: e.message;  e.backtrace
来源：http://qa.nicolike.cn

C#:   e.Message;  e.StackTrace
来源：http://eo.9csxet.cn

[H09] 带错误码的异常
来源：http://zm.haigaiapp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ee.colortex.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vy.asd995.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://tu.shtwfgs.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pm.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jn.panjiajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kb.newstarts.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qt.huanxung.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://sn.muxihuayi.cn

[H10] 资源自动释放
来源：http://xs.521024.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://uk.chemitech.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gz.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ee.shtwfgs.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mf.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fg.shtwfgs.cn

Go:   defer f.Close()
来源：http://ah.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uw.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hn.bookmarksfly.cn

================================================================================
来源：http://of.9csxet.cn

I. 正则表达式
来源：http://ar.huixiangedu.cn

================================================================================
来源：http://tf.bjjhwx.cn

[I01] 判断是否匹配
来源：http://ms.wgjwhj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://na.haigaiapp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sb.huanxung.cn

JS:   /\d+/.test(s)
来源：http://hr.colortex.cn

TS:   /\d+/.test(s)
来源：http://fo.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qy.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sj.9csxet.cn

Ruby: s.match?(/\d+/)
来源：http://ao.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://no.shtwfgs.cn

[I02] 提取所有匹配
来源：http://vv.nicolike.cn

Py:   re.findall(r"\d+", s)
来源：http://ba.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gb.bjjhwx.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mw.jianghongdianzi.cn

TS:   s.match(/\d+/g)
来源：http://wg.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mf.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bq.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://ls.shtwfgs.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wy.yuntaijiaju.cn

[I03] 提取捕获分组
来源：http://kd.huixinmuqiang.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bo.haigaiapp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tn.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ds.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://my.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sb.jctech888.com.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qd.newstarts.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ua.huixiangedu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uv.szxytkj.cn

[I04] 正则替换
来源：http://fd.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gj.nicolike.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zb.shxzskj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pk.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tt.gzmigu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://eu.shtwfgs.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qg.huixiangedu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xp.colortex.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://re.huixinmuqiang.cn

[I05] 按正则拆分
来源：http://af.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ct.521024.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jc.huanxung.cn

JS:   s.split(/\s*,\s*/)
来源：http://tz.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://ei.szsharing.cn


<!-- 参考信息 -->