代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tj.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xd.shtwfgs.cn

[F11] 复制与移动文件
来源：http://bk.szsharing.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://pc.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qk.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lh.jctech888.com.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qr.9csxet.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lz.szsharing.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uq.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pj.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qr.szxytkj.cn

[F12] CSV 读写
来源：http://ca.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pv.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ix.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pt.gzmigu.cn

TS:   // 同上
来源：http://wb.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wm.huanxung.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ba.huixiangedu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://su.bookmarksfly.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gb.hahajie.cn

================================================================================
来源：http://zd.jianghongdianzi.cn

G. 面向对象
来源：http://yg.jianghongdianzi.cn

================================================================================
来源：http://jy.jianghongdianzi.cn

[G01] 定义类
来源：http://bf.521024.cn

Py:   class User: pass
来源：http://rh.hnjuh.cn

PHP:  class User {}
来源：http://vy.huixiangedu.cn

JS:   class User {}
来源：http://ew.colortex.cn

TS:   class User { name: string = ""; }
来源：http://jm.shtwfgs.cn

Java: class User {}
来源：http://mr.newstarts.cn

Go:   type User struct { Name string }
来源：http://nc.huixiangedu.cn

Ruby: class User; end
来源：http://gj.lnxyls.cn

C#:   class User {}
来源：http://rk.huixiangedu.cn

[G02] 构造函数
来源：http://xy.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://vm.lnxyls.cn

PHP:  public function __construct(public string $name) {}
来源：http://gw.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://fy.shxzukj.cn

TS:   constructor(public name: string) {}
来源：http://un.szxytkj.cn

Java: User(String name) { this.name = name; }
来源：http://ly.yuntaijiaju.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://me.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://ro.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://se.jctech888.com.cn

[G03] 实例属性
来源：http://on.asd995.cn

Py:   self.name = "x"
来源：http://fv.nszjky.cn

PHP:  public string $name = "x";
来源：http://il.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://vu.shxzukj.cn

TS:   name: string = "x";
来源：http://xn.yuexingan06.cn

Java: private String name;
来源：http://zh.huixiangedu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nx.hnjuh.cn

Ruby: @name = "x"
来源：http://vp.shxzskj.cn

C#:   public string Name { get; set; } = "x";
来源：http://bk.huixinmuqiang.cn

[G04] 定义方法
来源：http://ys.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://lf.szxytkj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://es.jianghongdianzi.cn

JS:   greet() { return this.name; }
来源：http://sg.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://lf.wgjwhj.cn

Java: String greet() { return name; }
来源：http://tx.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fr.haigaiapp.cn

Ruby: def greet; @name; end
来源：http://er.hnjuh.cn

C#:   public string Greet() => Name;
来源：http://wt.gzmigu.cn

[G05] 继承
来源：http://se.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://vd.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://pe.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://yy.szsharing.cn

TS:   class Admin extends User {}
来源：http://pe.muxihuayi.cn

Java: class Admin extends User {}
来源：http://tk.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kw.asd995.cn

Ruby: class Admin < User; end
来源：http://ht.muxihuayi.cn

C#:   class Admin : User {}
来源：http://qt.gzmigu.cn

[G06] 重写方法
来源：http://ye.huixiangedu.cn

Py:   def greet(self): return "admin"
来源：http://po.bookmarksfly.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sb.newstarts.cn

JS:   greet() { return "admin"; }
来源：http://we.bookmarksfly.cn

TS:   greet(): string { return "admin"; }
来源：http://uj.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://uz.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ud.shtwfgs.cn

Ruby: def greet; "admin"; end
来源：http://tt.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://hk.bjjhwx.cn

[G07] 调用父类方法
来源：http://qq.huixiangedu.cn

Py:   super().greet()
来源：http://pm.shxzskj.cn

PHP:  parent::greet();
来源：http://qd.yuntaijiaju.cn

JS:   super.greet();
来源：http://ee.hnjuh.cn

TS:   super.greet();
来源：http://dv.huixinmuqiang.cn

Java: super.greet();
来源：http://qc.bjjhwx.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mu.jctech888.com.cn

Ruby: super
来源：http://ko.muxihuayi.cn

C#:   base.Greet();
来源：http://sf.nicolike.cn

[G08] 静态方法与属性
来源：http://ez.bjjhwx.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yp.yuntaijiaju.cn

PHP:  public static function f() {}
来源：http://fa.bookmarksfly.cn

JS:   static f() {}
来源：http://ud.shxzskj.cn

TS:   static f(): void {}
来源：http://cx.szxytkj.cn

Java: static void f() {}
来源：http://rm.huixiangedu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ga.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://rx.hahajie.cn

C#:   public static void F() {}
来源：http://kp.9csxet.cn

[G09] 接口 / 抽象类
来源：http://se.wgjwhj.cn

Py:   from abc import ABC, abstractmethod
来源：http://kw.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://yr.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fc.gzmigu.cn

TS:   interface Shape { area(): number; }
来源：http://qw.colortex.cn

Java: interface Shape { double area(); }
来源：http://km.panjiajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://qq.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xb.bjjhwx.cn

C#:   interface IShape { double Area(); }
来源：http://mu.hnjuh.cn

[G10] 访问控制
来源：http://qv.szxytkj.cn

Py:   约定 _protected / __private（不强制）
来源：http://kc.haigaiapp.cn

PHP:  public / protected / private
来源：http://kf.9csxet.cn

JS:   #private 字段；其余公开
来源：http://fm.bjjhwx.cn

TS:   public / protected / private
来源：http://tl.haigaiapp.cn

Java: public / protected / private / 默认包级
来源：http://wv.jctech888.com.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://tx.hnjuh.cn

Ruby: public / protected / private
来源：http://ge.szxytkj.cn

C#:   public / protected / private / internal
来源：http://ie.lnxyls.cn

[G11] getter / setter
来源：http://li.newstarts.cn

Py:   @property 与 @x.setter
来源：http://ih.yuntaijiaju.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fb.szxytkj.cn

JS:   get name() { return this._name; }
来源：http://md.jctech888.com.cn

TS:   get name(): string { return this._name; }
来源：http://vh.haigaiapp.cn

Java: public String getName() { return name; }
来源：http://ah.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cw.haigaiapp.cn

Ruby: attr_accessor :name
来源：http://rr.panjiajie.cn

C#:   public string Name { get; set; }
来源：http://sm.lnxyls.cn

[G12] 对象转字符串
来源：http://ke.panjiajie.cn

Py:   def __str__(self): return self.name
来源：http://gq.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sc.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://tf.jctech888.com.cn

TS:   toString(): string { return this.name; }
来源：http://fd.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://bz.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cd.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://be.colortex.cn

C#:   public override string ToString() => Name;
来源：http://gb.hahajie.cn

[G13] 判断对象类型
来源：http://qy.bookmarksfly.cn

Py:   isinstance(u, User)
来源：http://jj.hnjuh.cn

PHP:  $u instanceof User
来源：http://hh.chemitech.net.cn

JS:   u instanceof User
来源：http://oj.colortex.cn

TS:   u instanceof User
来源：http://zl.shxzukj.cn

Java: u instanceof User
来源：http://zv.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fw.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://wx.chemitech.net.cn

C#:   u is User
来源：http://at.colortex.cn

[G14] 数据类 / record
来源：http://il.chemitech.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://so.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://vv.huixinmuqiang.cn

JS:   // 无内置：普通类或对象字面量
来源：http://os.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://zi.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://xi.yuexingan06.cn

Go:   type User struct { Name string; Age int }
来源：http://nk.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dr.huixiangedu.cn

C#:   record User(string Name, int Age);
来源：http://fv.9csxet.cn

[G15] 枚举
来源：http://pd.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sw.nicolike.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://st.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wj.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wl.panjiajie.cn

Java: enum Color { RED, GREEN }
来源：http://fo.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nj.hnjuh.cn

Ruby: Color = %i[red green].freeze
来源：http://iu.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uz.muxihuayi.cn

[G16] 对象转数组 / 字典
来源：http://kt.bookmarksfly.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ts.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://aa.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://mx.9csxet.cn

TS:   Object.entries(obj)
来源：http://td.gzmigu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dt.asd995.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ir.asd995.cn

Ruby: obj.instance_variables
来源：http://cs.newstarts.cn

C#:   // 用反射或 System.Text.Json
来源：http://mf.lnxyls.cn

================================================================================
来源：http://ao.muxihuayi.cn

H. 异常与错误处理
来源：http://gg.colortex.cn

================================================================================
来源：http://zu.asd995.cn

[H01] try / catch 基础
来源：http://cs.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sq.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ms.chemitech.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yy.shxzskj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mn.szxytkj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fc.9csxet.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rt.gzmigu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jx.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zy.bookmarksfly.cn

[H02] finally / ensure 收尾
来源：http://ec.szxytkj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ax.jianghongdianzi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tv.muxihuayi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bp.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ms.yuexingan06.cn

Java: try { f(); } finally { cleanup(); }
来源：http://nv.nszjky.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ev.lnxyls.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tp.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mn.shtwfgs.cn

[H03] 主动抛出异常
来源：http://ud.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://qd.shtwfgs.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qe.nszjky.cn

JS:   throw new Error("错误信息");
来源：http://og.521024.cn

TS:   throw new Error("错误信息");
来源：http://ul.bjjhwx.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mc.wgjwhj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://je.chemitech.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://be.521024.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hr.shtwfgs.cn

[H04] 自定义异常类型
来源：http://em.jctech888.com.cn

Py:   class MyError(Exception): pass
来源：http://rr.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ig.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://or.huixinmuqiang.cn

TS:   class MyError extends Error {}
来源：http://jw.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://in.wgjwhj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://id.lnxyls.cn

Ruby: class MyError < StandardError; end
来源：http://pa.jianghongdianzi.cn

C#:   class MyException : Exception {}
来源：http://hy.jctech888.com.cn

[H05] 捕获特定类型
来源：http://ji.huixinmuqiang.cn

Py:   except ValueError as e:
来源：http://as.lnxyls.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hp.lnxyls.cn

JS:   if (e instanceof TypeError) {}
来源：http://sq.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://aw.shxzskj.cn

Java: catch (IOException | SQLException e) {}
来源：http://hv.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ny.lnxyls.cn

Ruby: rescue ArgumentError => e
来源：http://ez.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bo.huixinmuqiang.cn

[H06] 可选值 / 空值安全访问
来源：http://zg.shxzskj.cn

Py:   value = d.get("k") or default
来源：http://sp.shxzskj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vf.szsharing.cn

JS:   obj?.a?.b;  d ?? default
来源：http://na.haigaiapp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lm.lnxyls.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yn.hnjuh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vc.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://ty.shxzskj.cn

C#:   obj?.A?.B ?? default
来源：http://lv.szxytkj.cn

[H07] 断言
来源：http://np.shtwfgs.cn

Py:   assert x > 0, "必须为正"
来源：http://ta.bjjhwx.cn

PHP:  assert($x > 0);
来源：http://xl.yuntaijiaju.cn

JS:   console.assert(x > 0);
来源：http://ru.jianghongdianzi.cn

TS:   console.assert(x > 0);
来源：http://go.huanxung.cn

Java: assert x > 0 : "必须为正";
来源：http://zo.yuexingan06.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vf.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dg.gzmigu.cn

C#:   Debug.Assert(x > 0);
来源：http://zy.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://eu.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://vk.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yw.nszjky.cn

JS:   e.message;  e.stack
来源：http://dg.chemitech.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rg.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jc.gzmigu.cn

Go:   err.Error()
来源：http://kf.szsharing.cn

Ruby: e.message;  e.backtrace
来源：http://bk.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://zd.nszjky.cn

[H09] 带错误码的异常
来源：http://uu.chemitech.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lx.hnjuh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yi.shxzskj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qo.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nl.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yh.huixinmuqiang.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bs.hnjuh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pa.wgjwhj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ub.haigaiapp.cn

[H10] 资源自动释放
来源：http://rl.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ii.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mm.szxytkj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uu.szxytkj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nd.huanxung.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://si.wgjwhj.cn

Go:   defer f.Close()
来源：http://mm.nszjky.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kz.panjiajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vl.nszjky.cn

================================================================================
来源：http://dz.muxihuayi.cn

I. 正则表达式
来源：http://kj.huanxung.cn

================================================================================
来源：http://jj.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://hh.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sj.yuexingan06.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tg.521024.cn

JS:   /\d+/.test(s)
来源：http://ol.521024.cn

TS:   /\d+/.test(s)
来源：http://we.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://cr.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wi.huanxung.cn

Ruby: s.match?(/\d+/)
来源：http://iu.muxihuayi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ub.shxzukj.cn

[I02] 提取所有匹配
来源：http://ki.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://qx.asd995.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ai.shxzukj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rv.colortex.cn

TS:   s.match(/\d+/g)
来源：http://ne.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tz.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cc.asd995.cn

Ruby: s.scan(/\d+/)
来源：http://hs.shxzskj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fo.huanxung.cn

[I03] 提取捕获分组
来源：http://pv.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ww.huixinmuqiang.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vw.521024.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oj.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ee.hnjuh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kh.huixinmuqiang.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oi.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sy.yuexingan06.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dp.shxzskj.cn

[I04] 正则替换
来源：http://il.shxzukj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tj.nicolike.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ea.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ef.shtwfgs.cn

TS:   s.replace(/\d+/g, "#")
来源：http://iv.lnxyls.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ni.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wg.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ut.wgjwhj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wb.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://fs.9csxet.cn


<!-- 参考信息 -->