代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ta.wgjwhj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lx.yuexingan06.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://by.shtwfgs.cn

[F12] CSV 读写
来源：http://uv.shxzskj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rz.nszjky.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://iw.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gh.hahajie.cn

TS:   // 同上
来源：http://fh.panjiajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ig.szsharing.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ce.521024.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://we.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vk.lnxyls.cn

================================================================================
来源：http://ja.bookmarksfly.cn

G. 面向对象
来源：http://gu.lnxyls.cn

================================================================================
来源：http://xk.asd995.cn

[G01] 定义类
来源：http://mi.huixinmuqiang.cn

Py:   class User: pass
来源：http://yt.shxzskj.cn

PHP:  class User {}
来源：http://bx.shtwfgs.cn

JS:   class User {}
来源：http://sd.nicolike.cn

TS:   class User { name: string = ""; }
来源：http://id.jctech888.com.cn

Java: class User {}
来源：http://ne.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://nd.newstarts.cn

Ruby: class User; end
来源：http://nz.jianghongdianzi.cn

C#:   class User {}
来源：http://hi.huanxung.cn

[G02] 构造函数
来源：http://sb.hnjuh.cn

Py:   def __init__(self, name): self.name = name
来源：http://wf.shxzukj.cn

PHP:  public function __construct(public string $name) {}
来源：http://qs.huanxung.cn

JS:   constructor(name) { this.name = name; }
来源：http://km.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://qu.huixiangedu.cn

Java: User(String name) { this.name = name; }
来源：http://vx.chemitech.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fu.colortex.cn

Ruby: def initialize(name); @name = name; end
来源：http://qe.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://rg.bookmarksfly.cn

[G03] 实例属性
来源：http://cf.newstarts.cn

Py:   self.name = "x"
来源：http://gw.lnxyls.cn

PHP:  public string $name = "x";
来源：http://lu.chemitech.net.cn

JS:   this.name = "x";
来源：http://ku.muxihuayi.cn

TS:   name: string = "x";
来源：http://qb.nszjky.cn

Java: private String name;
来源：http://at.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vr.9csxet.cn

Ruby: @name = "x"
来源：http://te.panjiajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://vy.szxytkj.cn

[G04] 定义方法
来源：http://pw.bjjhwx.cn

Py:   def greet(self): return self.name
来源：http://vk.asd995.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cb.yuntaijiaju.cn

JS:   greet() { return this.name; }
来源：http://dc.shxzskj.cn

TS:   greet(): string { return this.name; }
来源：http://qf.colortex.cn

Java: String greet() { return name; }
来源：http://ln.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zx.chemitech.net.cn

Ruby: def greet; @name; end
来源：http://vg.huanxung.cn

C#:   public string Greet() => Name;
来源：http://og.9csxet.cn

[G05] 继承
来源：http://cs.9csxet.cn

Py:   class Admin(User): pass
来源：http://wf.chemitech.net.cn

PHP:  class Admin extends User {}
来源：http://pt.521024.cn

JS:   class Admin extends User {}
来源：http://lc.panjiajie.cn

TS:   class Admin extends User {}
来源：http://pn.huixinmuqiang.cn

Java: class Admin extends User {}
来源：http://vs.newstarts.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zb.9csxet.cn

Ruby: class Admin < User; end
来源：http://ay.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://fv.bjjhwx.cn

[G06] 重写方法
来源：http://xc.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://ob.haigaiapp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gn.huixinmuqiang.cn

JS:   greet() { return "admin"; }
来源：http://mx.yuntaijiaju.cn

TS:   greet(): string { return "admin"; }
来源：http://wn.nicolike.cn

Java: @Override String greet() { return "admin"; }
来源：http://np.bjjhwx.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kg.huixiangedu.cn

Ruby: def greet; "admin"; end
来源：http://zg.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://qu.nicolike.cn

[G07] 调用父类方法
来源：http://xi.jctech888.com.cn

Py:   super().greet()
来源：http://jg.huixinmuqiang.cn

PHP:  parent::greet();
来源：http://ee.521024.cn

JS:   super.greet();
来源：http://tr.muxihuayi.cn

TS:   super.greet();
来源：http://de.szsharing.cn

Java: super.greet();
来源：http://ry.nszjky.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://eu.chemitech.net.cn

Ruby: super
来源：http://ba.muxihuayi.cn

C#:   base.Greet();
来源：http://lo.muxihuayi.cn

[G08] 静态方法与属性
来源：http://jr.jianghongdianzi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nu.gzmigu.cn

PHP:  public static function f() {}
来源：http://uu.521024.cn

JS:   static f() {}
来源：http://yb.panjiajie.cn

TS:   static f(): void {}
来源：http://mk.panjiajie.cn

Java: static void f() {}
来源：http://wd.lnxyls.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ev.gzmigu.cn

Ruby: def self.f; end
来源：http://wn.hnjuh.cn

C#:   public static void F() {}
来源：http://wt.shxzskj.cn

[G09] 接口 / 抽象类
来源：http://kq.shxzukj.cn

Py:   from abc import ABC, abstractmethod
来源：http://gw.9csxet.cn

PHP:  interface Shape { public function area(): float; }
来源：http://il.newstarts.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://it.haigaiapp.cn

TS:   interface Shape { area(): number; }
来源：http://af.chemitech.net.cn

Java: interface Shape { double area(); }
来源：http://uj.gzmigu.cn

Go:   type Shape interface { Area() float64 }
来源：http://jo.newstarts.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nv.panjiajie.cn

C#:   interface IShape { double Area(); }
来源：http://cl.shtwfgs.cn

[G10] 访问控制
来源：http://lx.shxzskj.cn

Py:   约定 _protected / __private（不强制）
来源：http://zc.bookmarksfly.cn

PHP:  public / protected / private
来源：http://st.hahajie.cn

JS:   #private 字段；其余公开
来源：http://vd.huixiangedu.cn

TS:   public / protected / private
来源：http://kj.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://na.jctech888.com.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rr.asd995.cn

Ruby: public / protected / private
来源：http://ts.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://od.colortex.cn

[G11] getter / setter
来源：http://gr.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://ow.huanxung.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fi.szxytkj.cn

JS:   get name() { return this._name; }
来源：http://lq.huanxung.cn

TS:   get name(): string { return this._name; }
来源：http://pv.shtwfgs.cn

Java: public String getName() { return name; }
来源：http://za.9csxet.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://un.shxzukj.cn

Ruby: attr_accessor :name
来源：http://su.shxzskj.cn

C#:   public string Name { get; set; }
来源：http://tq.wgjwhj.cn

[G12] 对象转字符串
来源：http://gx.wgjwhj.cn

Py:   def __str__(self): return self.name
来源：http://lr.huanxung.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fk.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://ev.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://xf.hahajie.cn

Java: @Override public String toString() { return name; }
来源：http://es.asd995.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bv.haigaiapp.cn

Ruby: def to_s; @name; end
来源：http://ep.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://dn.muxihuayi.cn

[G13] 判断对象类型
来源：http://yu.bookmarksfly.cn

Py:   isinstance(u, User)
来源：http://mg.9csxet.cn

PHP:  $u instanceof User
来源：http://cf.newstarts.cn

JS:   u instanceof User
来源：http://qa.lnxyls.cn

TS:   u instanceof User
来源：http://sb.chemitech.net.cn

Java: u instanceof User
来源：http://ui.hnjuh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bm.yuntaijiaju.cn

Ruby: u.is_a?(User)
来源：http://iy.szxytkj.cn

C#:   u is User
来源：http://vg.shxzskj.cn

[G14] 数据类 / record
来源：http://ci.huixinmuqiang.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pz.huixiangedu.cn

PHP:  // 用 readonly 属性模拟
来源：http://ho.colortex.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dj.jctech888.com.cn

TS:   type User = { name: string; age: number };
来源：http://qt.newstarts.cn

Java: record User(String name, int age) {}
来源：http://tr.nszjky.cn

Go:   type User struct { Name string; Age int }
来源：http://fi.huixinmuqiang.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xl.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://nr.haigaiapp.cn

[G15] 枚举
来源：http://cn.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ob.yuntaijiaju.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ys.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xa.szsharing.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sh.huixinmuqiang.cn

Java: enum Color { RED, GREEN }
来源：http://nv.szsharing.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hm.hahajie.cn

Ruby: Color = %i[red green].freeze
来源：http://fe.haigaiapp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lx.huixiangedu.cn

[G16] 对象转数组 / 字典
来源：http://ps.newstarts.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mp.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://gg.yuntaijiaju.cn

JS:   Object.entries(obj)
来源：http://wr.shtwfgs.cn

TS:   Object.entries(obj)
来源：http://eh.szsharing.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yl.newstarts.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://em.colortex.cn

Ruby: obj.instance_variables
来源：http://ux.hnjuh.cn

C#:   // 用反射或 System.Text.Json
来源：http://ie.yuexingan06.cn

================================================================================
来源：http://ye.huixinmuqiang.cn

H. 异常与错误处理
来源：http://ff.lnxyls.cn

================================================================================
来源：http://go.shxzukj.cn

[H01] try / catch 基础
来源：http://ar.jctech888.com.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pu.muxihuayi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dc.lnxyls.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oa.bookmarksfly.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xq.lnxyls.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xu.colortex.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xp.shtwfgs.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pa.szxytkj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ol.shxzskj.cn

[H02] finally / ensure 收尾
来源：http://ey.huixiangedu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xz.nszjky.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nv.haigaiapp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ph.huixiangedu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xs.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pb.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sf.shxzukj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nq.newstarts.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hd.chemitech.net.cn

[H03] 主动抛出异常
来源：http://eq.szxytkj.cn

Py:   raise ValueError("错误信息")
来源：http://jq.9csxet.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sv.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://cq.hahajie.cn

TS:   throw new Error("错误信息");
来源：http://bp.szxytkj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yw.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://we.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qu.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ek.szsharing.cn

[H04] 自定义异常类型
来源：http://ep.muxihuayi.cn

Py:   class MyError(Exception): pass
来源：http://wh.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ce.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://bk.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://pm.jianghongdianzi.cn

Java: class MyException extends RuntimeException {}
来源：http://cf.9csxet.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ot.huixinmuqiang.cn

Ruby: class MyError < StandardError; end
来源：http://bx.szxytkj.cn

C#:   class MyException : Exception {}
来源：http://mw.wgjwhj.cn

[H05] 捕获特定类型
来源：http://ts.newstarts.cn

Py:   except ValueError as e:
来源：http://lr.gzmigu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dh.9csxet.cn

JS:   if (e instanceof TypeError) {}
来源：http://aq.wgjwhj.cn

TS:   if (e instanceof TypeError) {}
来源：http://ks.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://da.yuexingan06.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wf.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://wt.hnjuh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ka.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://al.newstarts.cn

Py:   value = d.get("k") or default
来源：http://aw.szxytkj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pd.nicolike.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sh.shtwfgs.cn

TS:   obj?.a?.b;  d ?? default
来源：http://kk.nszjky.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sk.huanxung.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qp.asd995.cn

Ruby: d&.dig(:a, :b)
来源：http://lh.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://xw.521024.cn

[H07] 断言
来源：http://ce.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://bp.shxzskj.cn

PHP:  assert($x > 0);
来源：http://fw.nszjky.cn

JS:   console.assert(x > 0);
来源：http://iu.muxihuayi.cn

TS:   console.assert(x > 0);
来源：http://le.nszjky.cn

Java: assert x > 0 : "必须为正";
来源：http://pg.wgjwhj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wu.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kh.szxytkj.cn

C#:   Debug.Assert(x > 0);
来源：http://xs.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://in.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://ho.haigaiapp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://af.shxzukj.cn

JS:   e.message;  e.stack
来源：http://ck.nszjky.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zw.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ge.bookmarksfly.cn

Go:   err.Error()
来源：http://qe.shxzukj.cn

Ruby: e.message;  e.backtrace
来源：http://ub.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://ij.shxzskj.cn

[H09] 带错误码的异常
来源：http://jj.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jm.huanxung.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://bj.huixinmuqiang.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://id.haigaiapp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xg.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zx.newstarts.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jv.521024.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gf.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hg.szsharing.cn

[H10] 资源自动释放
来源：http://lo.huixinmuqiang.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pl.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xw.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zf.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ep.colortex.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wr.haigaiapp.cn

Go:   defer f.Close()
来源：http://wz.huixinmuqiang.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jr.wgjwhj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://we.hnjuh.cn

================================================================================
来源：http://gm.asd995.cn

I. 正则表达式
来源：http://dd.newstarts.cn

================================================================================
来源：http://hk.bjjhwx.cn

[I01] 判断是否匹配
来源：http://rk.bjjhwx.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lr.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ia.9csxet.cn

JS:   /\d+/.test(s)
来源：http://sc.szsharing.cn

TS:   /\d+/.test(s)
来源：http://eb.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xg.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ya.huanxung.cn

Ruby: s.match?(/\d+/)
来源：http://ko.colortex.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gd.chemitech.net.cn

[I02] 提取所有匹配
来源：http://so.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://an.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iv.521024.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uf.jctech888.com.cn

TS:   s.match(/\d+/g)
来源：http://qz.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mh.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xv.wgjwhj.cn

Ruby: s.scan(/\d+/)
来源：http://yw.yuntaijiaju.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lt.gzmigu.cn

[I03] 提取捕获分组
来源：http://mu.szxytkj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://op.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ro.haigaiapp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rn.shxzskj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://io.muxihuayi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wx.jianghongdianzi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rj.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lc.bjjhwx.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uz.shtwfgs.cn

[I04] 正则替换
来源：http://wf.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rc.9csxet.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lw.bookmarksfly.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lx.yuntaijiaju.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xf.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qz.jianghongdianzi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wq.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ya.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ko.521024.cn

[I05] 按正则拆分
来源：http://za.haigaiapp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://um.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yu.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://id.jctech888.com.cn

TS:   s.split(/\s*,\s*/)
来源：http://bf.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://iz.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jz.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ay.haigaiapp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pm.jctech888.com.cn


<!-- 参考信息 -->