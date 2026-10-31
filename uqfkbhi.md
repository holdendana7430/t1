代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mb.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://vm.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tb.asd995.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dn.nszjky.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ci.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fz.muxihuayi.cn

[F11] 复制与移动文件
来源：http://pj.haigaiapp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pr.lnxyls.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ic.nszjky.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ai.szsharing.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ab.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bj.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rt.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ja.huixiangedu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ds.9csxet.cn

[F12] CSV 读写
来源：http://ls.szsharing.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ij.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ur.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nk.wgjwhj.cn

TS:   // 同上
来源：http://ae.shtwfgs.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rz.lnxyls.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://of.szxytkj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eu.9csxet.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://er.bookmarksfly.cn

================================================================================
来源：http://oh.chemitech.net.cn

G. 面向对象
来源：http://zy.szxytkj.cn

================================================================================
来源：http://ie.jianghongdianzi.cn

[G01] 定义类
来源：http://gh.yuexingan06.cn

Py:   class User: pass
来源：http://ve.chemitech.net.cn

PHP:  class User {}
来源：http://dd.newstarts.cn

JS:   class User {}
来源：http://ef.colortex.cn

TS:   class User { name: string = ""; }
来源：http://ll.jctech888.com.cn

Java: class User {}
来源：http://ft.haigaiapp.cn

Go:   type User struct { Name string }
来源：http://jc.yuntaijiaju.cn

Ruby: class User; end
来源：http://wl.jianghongdianzi.cn

C#:   class User {}
来源：http://sy.asd995.cn

[G02] 构造函数
来源：http://mu.9csxet.cn

Py:   def __init__(self, name): self.name = name
来源：http://mj.lnxyls.cn

PHP:  public function __construct(public string $name) {}
来源：http://st.yuntaijiaju.cn

JS:   constructor(name) { this.name = name; }
来源：http://xl.jctech888.com.cn

TS:   constructor(public name: string) {}
来源：http://ga.muxihuayi.cn

Java: User(String name) { this.name = name; }
来源：http://mv.haigaiapp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lz.jianghongdianzi.cn

Ruby: def initialize(name); @name = name; end
来源：http://wi.nicolike.cn

C#:   public User(string name) { Name = name; }
来源：http://ys.panjiajie.cn

[G03] 实例属性
来源：http://uv.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://qi.nszjky.cn

PHP:  public string $name = "x";
来源：http://bu.nicolike.cn

JS:   this.name = "x";
来源：http://cj.lnxyls.cn

TS:   name: string = "x";
来源：http://ti.szxytkj.cn

Java: private String name;
来源：http://zf.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pe.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://vn.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://cm.asd995.cn

[G04] 定义方法
来源：http://zy.yuexingan06.cn

Py:   def greet(self): return self.name
来源：http://bf.szxytkj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cg.huixiangedu.cn

JS:   greet() { return this.name; }
来源：http://wn.huixinmuqiang.cn

TS:   greet(): string { return this.name; }
来源：http://au.huixinmuqiang.cn

Java: String greet() { return name; }
来源：http://pi.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://il.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://cm.yuexingan06.cn

C#:   public string Greet() => Name;
来源：http://me.asd995.cn

[G05] 继承
来源：http://rb.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://yw.yuexingan06.cn

PHP:  class Admin extends User {}
来源：http://be.newstarts.cn

JS:   class Admin extends User {}
来源：http://to.colortex.cn

TS:   class Admin extends User {}
来源：http://dj.hnjuh.cn

Java: class Admin extends User {}
来源：http://zn.huixinmuqiang.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ok.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://sy.asd995.cn

C#:   class Admin : User {}
来源：http://im.huixinmuqiang.cn

[G06] 重写方法
来源：http://di.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://fy.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yo.haigaiapp.cn

JS:   greet() { return "admin"; }
来源：http://ur.chemitech.net.cn

TS:   greet(): string { return "admin"; }
来源：http://py.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://gm.hahajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://di.haigaiapp.cn

Ruby: def greet; "admin"; end
来源：http://iu.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://ve.yuexingan06.cn

[G07] 调用父类方法
来源：http://us.yuexingan06.cn

Py:   super().greet()
来源：http://jd.wgjwhj.cn

PHP:  parent::greet();
来源：http://ac.huixiangedu.cn

JS:   super.greet();
来源：http://fn.9csxet.cn

TS:   super.greet();
来源：http://pz.yuntaijiaju.cn

Java: super.greet();
来源：http://yv.hnjuh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cn.nszjky.cn

Ruby: super
来源：http://ep.hnjuh.cn

C#:   base.Greet();
来源：http://sc.huixiangedu.cn

[G08] 静态方法与属性
来源：http://ur.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://th.jianghongdianzi.cn

PHP:  public static function f() {}
来源：http://bw.colortex.cn

JS:   static f() {}
来源：http://in.asd995.cn

TS:   static f(): void {}
来源：http://ww.yuexingan06.cn

Java: static void f() {}
来源：http://bt.wgjwhj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yr.panjiajie.cn

Ruby: def self.f; end
来源：http://un.huixinmuqiang.cn

C#:   public static void F() {}
来源：http://sk.9csxet.cn

[G09] 接口 / 抽象类
来源：http://ef.huixiangedu.cn

Py:   from abc import ABC, abstractmethod
来源：http://qk.shxzukj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xv.huanxung.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://oc.newstarts.cn

TS:   interface Shape { area(): number; }
来源：http://ss.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://ku.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://dw.colortex.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rd.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://wp.nicolike.cn

[G10] 访问控制
来源：http://uj.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://ia.szxytkj.cn

PHP:  public / protected / private
来源：http://ar.jianghongdianzi.cn

JS:   #private 字段；其余公开
来源：http://yb.huanxung.cn

TS:   public / protected / private
来源：http://kc.nszjky.cn

Java: public / protected / private / 默认包级
来源：http://no.gzmigu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://uy.gzmigu.cn

Ruby: public / protected / private
来源：http://ld.shxzskj.cn

C#:   public / protected / private / internal
来源：http://wc.jctech888.com.cn

[G11] getter / setter
来源：http://mk.9csxet.cn

Py:   @property 与 @x.setter
来源：http://vr.huixinmuqiang.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qm.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://tf.bjjhwx.cn

TS:   get name(): string { return this._name; }
来源：http://if.haigaiapp.cn

Java: public String getName() { return name; }
来源：http://sc.nszjky.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dg.yuntaijiaju.cn

Ruby: attr_accessor :name
来源：http://cz.nicolike.cn

C#:   public string Name { get; set; }
来源：http://kb.szsharing.cn

[G12] 对象转字符串
来源：http://mr.szsharing.cn

Py:   def __str__(self): return self.name
来源：http://rc.haigaiapp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sj.muxihuayi.cn

JS:   toString() { return this.name; }
来源：http://he.nszjky.cn

TS:   toString(): string { return this.name; }
来源：http://zl.hnjuh.cn

Java: @Override public String toString() { return name; }
来源：http://yc.521024.cn

Go:   func (u User) String() string { return u.Name }
来源：http://yr.hahajie.cn

Ruby: def to_s; @name; end
来源：http://xb.lnxyls.cn

C#:   public override string ToString() => Name;
来源：http://kr.9csxet.cn

[G13] 判断对象类型
来源：http://zv.chemitech.net.cn

Py:   isinstance(u, User)
来源：http://vx.colortex.cn

PHP:  $u instanceof User
来源：http://jq.yuexingan06.cn

JS:   u instanceof User
来源：http://vc.bookmarksfly.cn

TS:   u instanceof User
来源：http://th.521024.cn

Java: u instanceof User
来源：http://zb.asd995.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ld.colortex.cn

Ruby: u.is_a?(User)
来源：http://hj.szsharing.cn

C#:   u is User
来源：http://kk.hahajie.cn

[G14] 数据类 / record
来源：http://xo.lnxyls.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wk.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://mq.bjjhwx.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ov.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://hh.521024.cn

Java: record User(String name, int age) {}
来源：http://fb.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://rr.yuntaijiaju.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nt.jctech888.com.cn

C#:   record User(string Name, int Age);
来源：http://ex.muxihuayi.cn

[G15] 枚举
来源：http://uv.asd995.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ai.huixiangedu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://su.szsharing.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vt.wgjwhj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cx.huixinmuqiang.cn

Java: enum Color { RED, GREEN }
来源：http://lv.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gs.huanxung.cn

Ruby: Color = %i[red green].freeze
来源：http://ww.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vr.haigaiapp.cn

[G16] 对象转数组 / 字典
来源：http://nl.hnjuh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xo.wgjwhj.cn

PHP:  get_object_vars($obj);
来源：http://ug.huixinmuqiang.cn

JS:   Object.entries(obj)
来源：http://lp.szxytkj.cn

TS:   Object.entries(obj)
来源：http://gi.muxihuayi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jx.szxytkj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://sr.jctech888.com.cn

Ruby: obj.instance_variables
来源：http://ci.wgjwhj.cn

C#:   // 用反射或 System.Text.Json
来源：http://iy.lnxyls.cn

================================================================================
来源：http://ht.hnjuh.cn

H. 异常与错误处理
来源：http://xq.shxzskj.cn

================================================================================
来源：http://jg.huixiangedu.cn

[H01] try / catch 基础
来源：http://ce.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ha.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ws.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://np.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nu.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yc.lnxyls.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tw.haigaiapp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gk.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ii.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://ba.wgjwhj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://eg.hnjuh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hg.hnjuh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ql.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ak.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wc.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://iu.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kq.bookmarksfly.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ib.huixiangedu.cn

[H03] 主动抛出异常
来源：http://oa.bookmarksfly.cn

Py:   raise ValueError("错误信息")
来源：http://nx.panjiajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ev.yuntaijiaju.cn

JS:   throw new Error("错误信息");
来源：http://rs.yuexingan06.cn

TS:   throw new Error("错误信息");
来源：http://qw.521024.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dp.jctech888.com.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ai.newstarts.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ee.wgjwhj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pu.521024.cn

[H04] 自定义异常类型
来源：http://hd.gzmigu.cn

Py:   class MyError(Exception): pass
来源：http://vc.panjiajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mc.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://ov.muxihuayi.cn

TS:   class MyError extends Error {}
来源：http://mg.yuntaijiaju.cn

Java: class MyException extends RuntimeException {}
来源：http://qa.hnjuh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iq.newstarts.cn

Ruby: class MyError < StandardError; end
来源：http://tf.9csxet.cn

C#:   class MyException : Exception {}
来源：http://mu.chemitech.net.cn

[H05] 捕获特定类型
来源：http://mk.bjjhwx.cn

Py:   except ValueError as e:
来源：http://ul.nicolike.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jd.huixiangedu.cn

JS:   if (e instanceof TypeError) {}
来源：http://zg.nszjky.cn

TS:   if (e instanceof TypeError) {}
来源：http://oq.wgjwhj.cn

Java: catch (IOException | SQLException e) {}
来源：http://mt.hnjuh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kr.shxzukj.cn

Ruby: rescue ArgumentError => e
来源：http://ch.muxihuayi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nr.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://rw.huanxung.cn

Py:   value = d.get("k") or default
来源：http://ya.yuexingan06.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ce.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sd.jctech888.com.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tk.nicolike.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rl.wgjwhj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://an.shxzskj.cn

Ruby: d&.dig(:a, :b)
来源：http://si.colortex.cn

C#:   obj?.A?.B ?? default
来源：http://tp.muxihuayi.cn

[H07] 断言
来源：http://ie.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://jh.9csxet.cn

PHP:  assert($x > 0);
来源：http://pg.wgjwhj.cn

JS:   console.assert(x > 0);
来源：http://wx.haigaiapp.cn

TS:   console.assert(x > 0);
来源：http://ty.yuexingan06.cn

Java: assert x > 0 : "必须为正";
来源：http://se.chemitech.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oz.huixinmuqiang.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ni.yuntaijiaju.cn

C#:   Debug.Assert(x > 0);
来源：http://mp.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://qm.jctech888.com.cn

Py:   str(e);  traceback.format_exc()
来源：http://ab.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wj.shxzukj.cn

JS:   e.message;  e.stack
来源：http://vo.shxzukj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mx.yuntaijiaju.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ux.yuntaijiaju.cn

Go:   err.Error()
来源：http://cb.nicolike.cn

Ruby: e.message;  e.backtrace
来源：http://wi.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://jx.shtwfgs.cn

[H09] 带错误码的异常
来源：http://ta.newstarts.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lg.huixinmuqiang.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cg.newstarts.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://me.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yd.shxzukj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yl.huixiangedu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ea.huixinmuqiang.cn

Ruby: raise MyError.new("fail", 500)
来源：http://bc.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lx.nszjky.cn

[H10] 资源自动释放
来源：http://zj.chemitech.net.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://tw.newstarts.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://no.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rh.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gb.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mi.newstarts.cn

Go:   defer f.Close()
来源：http://wy.panjiajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pl.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ns.huixiangedu.cn

================================================================================
来源：http://bc.nicolike.cn

I. 正则表达式
来源：http://qx.nszjky.cn

================================================================================
来源：http://jh.haigaiapp.cn

[I01] 判断是否匹配
来源：http://kt.szsharing.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lc.shxzskj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sr.szsharing.cn

JS:   /\d+/.test(s)
来源：http://im.huanxung.cn

TS:   /\d+/.test(s)
来源：http://vr.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ar.9csxet.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://os.hahajie.cn

Ruby: s.match?(/\d+/)
来源：http://nn.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wl.newstarts.cn

[I02] 提取所有匹配
来源：http://fc.huanxung.cn

Py:   re.findall(r"\d+", s)
来源：http://rz.shtwfgs.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cz.bjjhwx.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vf.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://oz.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rf.huanxung.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xn.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://qw.newstarts.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ao.chemitech.net.cn

[I03] 提取捕获分组
来源：http://oj.szsharing.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nd.newstarts.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fq.gzmigu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vc.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ls.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ym.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mz.lnxyls.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ef.yuexingan06.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uf.shxzskj.cn

[I04] 正则替换
来源：http://vl.jianghongdianzi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hr.hnjuh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://be.shxzukj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://on.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lu.yuexingan06.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yr.jctech888.com.cn


<!-- 参考信息 -->