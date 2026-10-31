代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ba.yuexingan06.cn

TS:   path.extname("a.txt")
来源：http://sq.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kk.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sp.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bf.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xg.szxytkj.cn

[F11] 复制与移动文件
来源：http://tk.hahajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yw.wgjwhj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cx.chemitech.net.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bt.colortex.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ba.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pd.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hw.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gj.9csxet.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xg.9csxet.cn

[F12] CSV 读写
来源：http://oc.huixiangedu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://pi.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://vn.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tf.gzmigu.cn

TS:   // 同上
来源：http://ax.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gj.szsharing.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wy.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://me.szsharing.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qz.521024.cn

================================================================================
来源：http://ev.huanxung.cn

G. 面向对象
来源：http://dd.szxytkj.cn

================================================================================
来源：http://tb.gzmigu.cn

[G01] 定义类
来源：http://nn.muxihuayi.cn

Py:   class User: pass
来源：http://ep.shxzukj.cn

PHP:  class User {}
来源：http://md.shxzukj.cn

JS:   class User {}
来源：http://yx.huixiangedu.cn

TS:   class User { name: string = ""; }
来源：http://dh.521024.cn

Java: class User {}
来源：http://mg.haigaiapp.cn

Go:   type User struct { Name string }
来源：http://sm.huixiangedu.cn

Ruby: class User; end
来源：http://ce.gzmigu.cn

C#:   class User {}
来源：http://ql.haigaiapp.cn

[G02] 构造函数
来源：http://ti.panjiajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://pm.yuexingan06.cn

PHP:  public function __construct(public string $name) {}
来源：http://lf.yuntaijiaju.cn

JS:   constructor(name) { this.name = name; }
来源：http://rm.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://yc.wgjwhj.cn

Java: User(String name) { this.name = name; }
来源：http://vu.lnxyls.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pm.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://xo.shxzukj.cn

C#:   public User(string name) { Name = name; }
来源：http://pn.asd995.cn

[G03] 实例属性
来源：http://ku.521024.cn

Py:   self.name = "x"
来源：http://lv.huixinmuqiang.cn

PHP:  public string $name = "x";
来源：http://xw.szsharing.cn

JS:   this.name = "x";
来源：http://is.hnjuh.cn

TS:   name: string = "x";
来源：http://ae.shxzskj.cn

Java: private String name;
来源：http://yr.shxzskj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gl.nicolike.cn

Ruby: @name = "x"
来源：http://vi.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://pd.szxytkj.cn

[G04] 定义方法
来源：http://ty.hnjuh.cn

Py:   def greet(self): return self.name
来源：http://xo.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gr.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://nb.jctech888.com.cn

TS:   greet(): string { return this.name; }
来源：http://fp.jctech888.com.cn

Java: String greet() { return name; }
来源：http://ui.gzmigu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wl.huanxung.cn

Ruby: def greet; @name; end
来源：http://xa.hahajie.cn

C#:   public string Greet() => Name;
来源：http://pu.wgjwhj.cn

[G05] 继承
来源：http://yq.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://xb.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://bd.521024.cn

JS:   class Admin extends User {}
来源：http://mp.shtwfgs.cn

TS:   class Admin extends User {}
来源：http://ol.hahajie.cn

Java: class Admin extends User {}
来源：http://kv.hnjuh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cj.yuntaijiaju.cn

Ruby: class Admin < User; end
来源：http://cn.gzmigu.cn

C#:   class Admin : User {}
来源：http://ho.haigaiapp.cn

[G06] 重写方法
来源：http://ww.panjiajie.cn

Py:   def greet(self): return "admin"
来源：http://vo.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bq.panjiajie.cn

JS:   greet() { return "admin"; }
来源：http://yx.huixiangedu.cn

TS:   greet(): string { return "admin"; }
来源：http://km.bjjhwx.cn

Java: @Override String greet() { return "admin"; }
来源：http://wi.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nu.bookmarksfly.cn

Ruby: def greet; "admin"; end
来源：http://tv.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://ru.haigaiapp.cn

[G07] 调用父类方法
来源：http://ed.haigaiapp.cn

Py:   super().greet()
来源：http://jx.muxihuayi.cn

PHP:  parent::greet();
来源：http://ge.huixiangedu.cn

JS:   super.greet();
来源：http://jp.yuntaijiaju.cn

TS:   super.greet();
来源：http://oy.yuexingan06.cn

Java: super.greet();
来源：http://hc.hahajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ll.szxytkj.cn

Ruby: super
来源：http://wt.huixinmuqiang.cn

C#:   base.Greet();
来源：http://yj.gzmigu.cn

[G08] 静态方法与属性
来源：http://do.bjjhwx.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qc.colortex.cn

PHP:  public static function f() {}
来源：http://of.chemitech.net.cn

JS:   static f() {}
来源：http://ix.yuexingan06.cn

TS:   static f(): void {}
来源：http://ix.jctech888.com.cn

Java: static void f() {}
来源：http://ms.huixiangedu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://tz.jctech888.com.cn

Ruby: def self.f; end
来源：http://gi.gzmigu.cn

C#:   public static void F() {}
来源：http://tv.shxzskj.cn

[G09] 接口 / 抽象类
来源：http://cz.muxihuayi.cn

Py:   from abc import ABC, abstractmethod
来源：http://ve.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pd.9csxet.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://uw.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://qv.szxytkj.cn

Java: interface Shape { double area(); }
来源：http://oj.wgjwhj.cn

Go:   type Shape interface { Area() float64 }
来源：http://kq.colortex.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uc.huixiangedu.cn

C#:   interface IShape { double Area(); }
来源：http://uv.hahajie.cn

[G10] 访问控制
来源：http://nz.panjiajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://wo.newstarts.cn

PHP:  public / protected / private
来源：http://nm.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://to.nszjky.cn

TS:   public / protected / private
来源：http://yd.huanxung.cn

Java: public / protected / private / 默认包级
来源：http://vi.muxihuayi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://aw.szsharing.cn

Ruby: public / protected / private
来源：http://qz.huanxung.cn

C#:   public / protected / private / internal
来源：http://vj.asd995.cn

[G11] getter / setter
来源：http://vg.521024.cn

Py:   @property 与 @x.setter
来源：http://np.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://uz.yuexingan06.cn

JS:   get name() { return this._name; }
来源：http://ka.yuntaijiaju.cn

TS:   get name(): string { return this._name; }
来源：http://rm.wgjwhj.cn

Java: public String getName() { return name; }
来源：http://rf.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://il.nicolike.cn

Ruby: attr_accessor :name
来源：http://eo.colortex.cn

C#:   public string Name { get; set; }
来源：http://io.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://ay.hnjuh.cn

Py:   def __str__(self): return self.name
来源：http://yv.9csxet.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lm.colortex.cn

JS:   toString() { return this.name; }
来源：http://rk.haigaiapp.cn

TS:   toString(): string { return this.name; }
来源：http://po.nszjky.cn

Java: @Override public String toString() { return name; }
来源：http://ix.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xp.shxzskj.cn

Ruby: def to_s; @name; end
来源：http://ov.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://ug.shtwfgs.cn

[G13] 判断对象类型
来源：http://gz.shxzukj.cn

Py:   isinstance(u, User)
来源：http://gh.nicolike.cn

PHP:  $u instanceof User
来源：http://hz.shxzskj.cn

JS:   u instanceof User
来源：http://di.bookmarksfly.cn

TS:   u instanceof User
来源：http://rq.wgjwhj.cn

Java: u instanceof User
来源：http://ss.huanxung.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ks.9csxet.cn

Ruby: u.is_a?(User)
来源：http://oe.shxzskj.cn

C#:   u is User
来源：http://ef.szsharing.cn

[G14] 数据类 / record
来源：http://oy.wgjwhj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://no.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://sb.chemitech.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vp.huixiangedu.cn

TS:   type User = { name: string; age: number };
来源：http://fe.hahajie.cn

Java: record User(String name, int age) {}
来源：http://il.hnjuh.cn

Go:   type User struct { Name string; Age int }
来源：http://xa.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bo.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://mr.hnjuh.cn

[G15] 枚举
来源：http://iy.colortex.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vv.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://la.newstarts.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ab.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dm.jianghongdianzi.cn

Java: enum Color { RED, GREEN }
来源：http://yx.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ks.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://vk.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://aj.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://lu.lnxyls.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://da.gzmigu.cn

PHP:  get_object_vars($obj);
来源：http://bg.shtwfgs.cn

JS:   Object.entries(obj)
来源：http://jl.nicolike.cn

TS:   Object.entries(obj)
来源：http://wi.jctech888.com.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jk.huixiangedu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kj.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://wr.huixinmuqiang.cn

C#:   // 用反射或 System.Text.Json
来源：http://tl.hahajie.cn

================================================================================
来源：http://nl.9csxet.cn

H. 异常与错误处理
来源：http://od.nszjky.cn

================================================================================
来源：http://tc.521024.cn

[H01] try / catch 基础
来源：http://hu.haigaiapp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bo.haigaiapp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bh.szsharing.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qz.szsharing.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gj.shtwfgs.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fq.nicolike.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bx.newstarts.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lr.wgjwhj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ys.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://pm.muxihuayi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://va.yuexingan06.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://at.muxihuayi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://au.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://lz.colortex.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ux.nicolike.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yz.huixiangedu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hf.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jw.nicolike.cn

[H03] 主动抛出异常
来源：http://uj.521024.cn

Py:   raise ValueError("错误信息")
来源：http://fp.521024.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xx.yuntaijiaju.cn

JS:   throw new Error("错误信息");
来源：http://px.huanxung.cn

TS:   throw new Error("错误信息");
来源：http://vw.szsharing.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vo.huanxung.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kx.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hv.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xf.bjjhwx.cn

[H04] 自定义异常类型
来源：http://xo.9csxet.cn

Py:   class MyError(Exception): pass
来源：http://cg.jianghongdianzi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ow.521024.cn

JS:   class MyError extends Error {}
来源：http://yh.newstarts.cn

TS:   class MyError extends Error {}
来源：http://me.panjiajie.cn

Java: class MyException extends RuntimeException {}
来源：http://gr.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xb.huixinmuqiang.cn

Ruby: class MyError < StandardError; end
来源：http://lq.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://la.521024.cn

[H05] 捕获特定类型
来源：http://ld.9csxet.cn

Py:   except ValueError as e:
来源：http://st.jctech888.com.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oa.jianghongdianzi.cn

JS:   if (e instanceof TypeError) {}
来源：http://gt.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://gh.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://id.panjiajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bp.gzmigu.cn

Ruby: rescue ArgumentError => e
来源：http://sx.shxzskj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hg.shtwfgs.cn

[H06] 可选值 / 空值安全访问
来源：http://sx.szsharing.cn

Py:   value = d.get("k") or default
来源：http://mk.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cr.nszjky.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zb.huixinmuqiang.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cm.szsharing.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://so.bjjhwx.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://un.bookmarksfly.cn

Ruby: d&.dig(:a, :b)
来源：http://uz.panjiajie.cn

C#:   obj?.A?.B ?? default
来源：http://lp.yuntaijiaju.cn

[H07] 断言
来源：http://fn.nszjky.cn

Py:   assert x > 0, "必须为正"
来源：http://fw.yuntaijiaju.cn

PHP:  assert($x > 0);
来源：http://qr.shxzukj.cn

JS:   console.assert(x > 0);
来源：http://ra.wgjwhj.cn

TS:   console.assert(x > 0);
来源：http://ui.hahajie.cn

Java: assert x > 0 : "必须为正";
来源：http://vx.bjjhwx.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hm.shxzskj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ht.shxzskj.cn

C#:   Debug.Assert(x > 0);
来源：http://fo.panjiajie.cn

[H08] 获取错误信息与堆栈
来源：http://ai.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://bg.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ls.szxytkj.cn

JS:   e.message;  e.stack
来源：http://ld.shxzskj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gh.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uv.yuntaijiaju.cn

Go:   err.Error()
来源：http://nt.jctech888.com.cn

Ruby: e.message;  e.backtrace
来源：http://rb.yuntaijiaju.cn

C#:   e.Message;  e.StackTrace
来源：http://ae.lnxyls.cn

[H09] 带错误码的异常
来源：http://ph.chemitech.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zi.nicolike.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zy.chemitech.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rz.yuexingan06.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://js.bjjhwx.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rv.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ai.asd995.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xz.huixinmuqiang.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hb.jctech888.com.cn

[H10] 资源自动释放
来源：http://nu.9csxet.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fc.huixiangedu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uo.szxytkj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pn.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bc.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ex.szsharing.cn

Go:   defer f.Close()
来源：http://dj.huixiangedu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://am.szsharing.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nw.huixinmuqiang.cn

================================================================================
来源：http://ly.nicolike.cn

I. 正则表达式
来源：http://xi.gzmigu.cn

================================================================================
来源：http://wq.nszjky.cn

[I01] 判断是否匹配
来源：http://ko.gzmigu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kl.gzmigu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tg.jctech888.com.cn

JS:   /\d+/.test(s)
来源：http://ei.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://lj.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lf.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mm.colortex.cn

Ruby: s.match?(/\d+/)
来源：http://bo.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ce.colortex.cn

[I02] 提取所有匹配
来源：http://jk.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://oq.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gh.chemitech.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://to.nszjky.cn

TS:   s.match(/\d+/g)
来源：http://qw.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oi.yuntaijiaju.cn

Ruby: s.scan(/\d+/)
来源：http://dl.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rv.yuexingan06.cn

[I03] 提取捕获分组
来源：http://zg.hahajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vf.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zx.hahajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jy.huixiangedu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wa.muxihuayi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vq.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://en.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lh.shxzskj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sz.bookmarksfly.cn

[I04] 正则替换
来源：http://hy.nicolike.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://md.521024.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hb.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ej.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://na.jctech888.com.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jh.9csxet.cn


<!-- 参考信息 -->