代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ph.huanxung.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ll.wgjwhj.cn

[F11] 复制与移动文件
来源：http://za.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cm.hnjuh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jv.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pp.huixinmuqiang.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fz.colortex.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ui.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://we.bookmarksfly.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vi.yuntaijiaju.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://gw.nszjky.cn

[F12] CSV 读写
来源：http://fu.colortex.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xu.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ry.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uh.nszjky.cn

TS:   // 同上
来源：http://vx.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rj.521024.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uw.shxzukj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oh.hnjuh.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ie.gzmigu.cn

================================================================================
来源：http://df.shxzukj.cn

G. 面向对象
来源：http://na.asd995.cn

================================================================================
来源：http://kd.9csxet.cn

[G01] 定义类
来源：http://eq.szxytkj.cn

Py:   class User: pass
来源：http://di.hahajie.cn

PHP:  class User {}
来源：http://ly.gzmigu.cn

JS:   class User {}
来源：http://mx.huixiangedu.cn

TS:   class User { name: string = ""; }
来源：http://oa.yuntaijiaju.cn

Java: class User {}
来源：http://kq.huanxung.cn

Go:   type User struct { Name string }
来源：http://kl.lnxyls.cn

Ruby: class User; end
来源：http://ti.9csxet.cn

C#:   class User {}
来源：http://an.chemitech.net.cn

[G02] 构造函数
来源：http://hi.9csxet.cn

Py:   def __init__(self, name): self.name = name
来源：http://av.huanxung.cn

PHP:  public function __construct(public string $name) {}
来源：http://px.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://gh.yuexingan06.cn

TS:   constructor(public name: string) {}
来源：http://tl.huanxung.cn

Java: User(String name) { this.name = name; }
来源：http://cp.shtwfgs.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hn.jianghongdianzi.cn

Ruby: def initialize(name); @name = name; end
来源：http://ui.bjjhwx.cn

C#:   public User(string name) { Name = name; }
来源：http://iy.521024.cn

[G03] 实例属性
来源：http://ri.hahajie.cn

Py:   self.name = "x"
来源：http://ih.jianghongdianzi.cn

PHP:  public string $name = "x";
来源：http://se.yuntaijiaju.cn

JS:   this.name = "x";
来源：http://gq.szsharing.cn

TS:   name: string = "x";
来源：http://sp.newstarts.cn

Java: private String name;
来源：http://af.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://tn.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://wy.jctech888.com.cn

C#:   public string Name { get; set; } = "x";
来源：http://na.szxytkj.cn

[G04] 定义方法
来源：http://xs.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://pw.yuntaijiaju.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bq.szsharing.cn

JS:   greet() { return this.name; }
来源：http://yx.lnxyls.cn

TS:   greet(): string { return this.name; }
来源：http://nf.haigaiapp.cn

Java: String greet() { return name; }
来源：http://op.shxzukj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lb.hahajie.cn

Ruby: def greet; @name; end
来源：http://ns.asd995.cn

C#:   public string Greet() => Name;
来源：http://nx.haigaiapp.cn

[G05] 继承
来源：http://eb.wgjwhj.cn

Py:   class Admin(User): pass
来源：http://it.muxihuayi.cn

PHP:  class Admin extends User {}
来源：http://ol.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://ii.bjjhwx.cn

TS:   class Admin extends User {}
来源：http://ou.shtwfgs.cn

Java: class Admin extends User {}
来源：http://kp.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fk.shtwfgs.cn

Ruby: class Admin < User; end
来源：http://us.shxzukj.cn

C#:   class Admin : User {}
来源：http://oo.hnjuh.cn

[G06] 重写方法
来源：http://dp.huanxung.cn

Py:   def greet(self): return "admin"
来源：http://bk.9csxet.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://of.nicolike.cn

JS:   greet() { return "admin"; }
来源：http://rn.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://ud.hahajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://xk.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ax.shxzskj.cn

Ruby: def greet; "admin"; end
来源：http://it.wgjwhj.cn

C#:   public override string Greet() => "admin";
来源：http://ui.521024.cn

[G07] 调用父类方法
来源：http://ms.colortex.cn

Py:   super().greet()
来源：http://ys.panjiajie.cn

PHP:  parent::greet();
来源：http://by.nicolike.cn

JS:   super.greet();
来源：http://oa.newstarts.cn

TS:   super.greet();
来源：http://nd.gzmigu.cn

Java: super.greet();
来源：http://nv.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zk.szxytkj.cn

Ruby: super
来源：http://rv.yuntaijiaju.cn

C#:   base.Greet();
来源：http://za.521024.cn

[G08] 静态方法与属性
来源：http://qj.nszjky.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hv.hahajie.cn

PHP:  public static function f() {}
来源：http://nz.chemitech.net.cn

JS:   static f() {}
来源：http://xj.huanxung.cn

TS:   static f(): void {}
来源：http://mr.9csxet.cn

Java: static void f() {}
来源：http://tx.9csxet.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://km.szsharing.cn

Ruby: def self.f; end
来源：http://in.asd995.cn

C#:   public static void F() {}
来源：http://uc.huixiangedu.cn

[G09] 接口 / 抽象类
来源：http://vi.9csxet.cn

Py:   from abc import ABC, abstractmethod
来源：http://tf.panjiajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uw.jctech888.com.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kr.colortex.cn

TS:   interface Shape { area(): number; }
来源：http://qw.szsharing.cn

Java: interface Shape { double area(); }
来源：http://fd.panjiajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://pi.jianghongdianzi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sr.jianghongdianzi.cn

C#:   interface IShape { double Area(); }
来源：http://zf.9csxet.cn

[G10] 访问控制
来源：http://pc.jianghongdianzi.cn

Py:   约定 _protected / __private（不强制）
来源：http://kr.szsharing.cn

PHP:  public / protected / private
来源：http://gg.shtwfgs.cn

JS:   #private 字段；其余公开
来源：http://wk.bjjhwx.cn

TS:   public / protected / private
来源：http://xo.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://rk.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qj.chemitech.net.cn

Ruby: public / protected / private
来源：http://eo.newstarts.cn

C#:   public / protected / private / internal
来源：http://kb.chemitech.net.cn

[G11] getter / setter
来源：http://pu.gzmigu.cn

Py:   @property 与 @x.setter
来源：http://or.wgjwhj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dd.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://jt.nszjky.cn

TS:   get name(): string { return this._name; }
来源：http://pb.haigaiapp.cn

Java: public String getName() { return name; }
来源：http://ej.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://uz.jctech888.com.cn

Ruby: attr_accessor :name
来源：http://yj.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://vk.hahajie.cn

[G12] 对象转字符串
来源：http://gn.shxzukj.cn

Py:   def __str__(self): return self.name
来源：http://in.hnjuh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yf.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://dp.521024.cn

TS:   toString(): string { return this.name; }
来源：http://ym.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://uo.gzmigu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rt.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://qs.bjjhwx.cn

C#:   public override string ToString() => Name;
来源：http://iv.wgjwhj.cn

[G13] 判断对象类型
来源：http://hh.jctech888.com.cn

Py:   isinstance(u, User)
来源：http://jy.shxzskj.cn

PHP:  $u instanceof User
来源：http://ah.huanxung.cn

JS:   u instanceof User
来源：http://yk.bjjhwx.cn

TS:   u instanceof User
来源：http://ku.haigaiapp.cn

Java: u instanceof User
来源：http://hb.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://un.szxytkj.cn

Ruby: u.is_a?(User)
来源：http://ov.521024.cn

C#:   u is User
来源：http://sk.haigaiapp.cn

[G14] 数据类 / record
来源：http://oo.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zr.haigaiapp.cn

PHP:  // 用 readonly 属性模拟
来源：http://an.huanxung.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tq.huixinmuqiang.cn

TS:   type User = { name: string; age: number };
来源：http://ab.521024.cn

Java: record User(String name, int age) {}
来源：http://rm.panjiajie.cn

Go:   type User struct { Name string; Age int }
来源：http://cg.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jk.panjiajie.cn

C#:   record User(string Name, int Age);
来源：http://zy.shtwfgs.cn

[G15] 枚举
来源：http://cf.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ht.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sn.huixinmuqiang.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gk.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gm.colortex.cn

Java: enum Color { RED, GREEN }
来源：http://xq.bjjhwx.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xa.shtwfgs.cn

Ruby: Color = %i[red green].freeze
来源：http://cr.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ia.huanxung.cn

[G16] 对象转数组 / 字典
来源：http://oa.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tm.shxzskj.cn

PHP:  get_object_vars($obj);
来源：http://dr.szxytkj.cn

JS:   Object.entries(obj)
来源：http://rs.asd995.cn

TS:   Object.entries(obj)
来源：http://ok.shtwfgs.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kp.huixinmuqiang.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ge.bookmarksfly.cn

Ruby: obj.instance_variables
来源：http://gp.huixiangedu.cn

C#:   // 用反射或 System.Text.Json
来源：http://jk.chemitech.net.cn

================================================================================
来源：http://js.huixinmuqiang.cn

H. 异常与错误处理
来源：http://cu.haigaiapp.cn

================================================================================
来源：http://vb.huixiangedu.cn

[H01] try / catch 基础
来源：http://sq.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fn.nicolike.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vx.panjiajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yd.chemitech.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pz.shxzskj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oj.gzmigu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lo.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uq.wgjwhj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bt.bookmarksfly.cn

[H02] finally / ensure 收尾
来源：http://mg.jianghongdianzi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gg.panjiajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kv.muxihuayi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hm.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fq.yuexingan06.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dm.nszjky.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ry.yuexingan06.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fw.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gq.lnxyls.cn

[H03] 主动抛出异常
来源：http://dz.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://pf.9csxet.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pn.hahajie.cn

JS:   throw new Error("错误信息");
来源：http://jj.jianghongdianzi.cn

TS:   throw new Error("错误信息");
来源：http://cz.panjiajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wb.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://do.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cu.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://uu.colortex.cn

[H04] 自定义异常类型
来源：http://dj.panjiajie.cn

Py:   class MyError(Exception): pass
来源：http://rr.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dp.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://xs.lnxyls.cn

TS:   class MyError extends Error {}
来源：http://xo.nicolike.cn

Java: class MyException extends RuntimeException {}
来源：http://gb.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xf.yuntaijiaju.cn

Ruby: class MyError < StandardError; end
来源：http://za.shxzukj.cn

C#:   class MyException : Exception {}
来源：http://se.jctech888.com.cn

[H05] 捕获特定类型
来源：http://iz.nicolike.cn

Py:   except ValueError as e:
来源：http://bo.wgjwhj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://od.shxzskj.cn

JS:   if (e instanceof TypeError) {}
来源：http://bu.huixinmuqiang.cn

TS:   if (e instanceof TypeError) {}
来源：http://ia.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://qb.9csxet.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://np.haigaiapp.cn

Ruby: rescue ArgumentError => e
来源：http://dy.bookmarksfly.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ps.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://hb.huixiangedu.cn

Py:   value = d.get("k") or default
来源：http://fn.jctech888.com.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mi.haigaiapp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ty.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mf.wgjwhj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ag.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mi.newstarts.cn

Ruby: d&.dig(:a, :b)
来源：http://bp.newstarts.cn

C#:   obj?.A?.B ?? default
来源：http://ks.yuntaijiaju.cn

[H07] 断言
来源：http://tv.521024.cn

Py:   assert x > 0, "必须为正"
来源：http://jq.muxihuayi.cn

PHP:  assert($x > 0);
来源：http://pz.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://kk.yuntaijiaju.cn

TS:   console.assert(x > 0);
来源：http://kk.yuexingan06.cn

Java: assert x > 0 : "必须为正";
来源：http://lj.bookmarksfly.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hc.huanxung.cn

Ruby: raise "必须为正" unless x > 0
来源：http://do.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://gl.jctech888.com.cn

[H08] 获取错误信息与堆栈
来源：http://ll.szsharing.cn

Py:   str(e);  traceback.format_exc()
来源：http://jo.panjiajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://px.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://yb.521024.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xp.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cy.wgjwhj.cn

Go:   err.Error()
来源：http://yj.asd995.cn

Ruby: e.message;  e.backtrace
来源：http://dz.huixinmuqiang.cn

C#:   e.Message;  e.StackTrace
来源：http://fw.muxihuayi.cn

[H09] 带错误码的异常
来源：http://lj.newstarts.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dv.521024.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://eb.haigaiapp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://za.muxihuayi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lr.9csxet.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://st.szxytkj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ko.szsharing.cn

Ruby: raise MyError.new("fail", 500)
来源：http://es.huixiangedu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yj.haigaiapp.cn

[H10] 资源自动释放
来源：http://yc.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vt.yuexingan06.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jm.huanxung.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://es.colortex.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iu.yuntaijiaju.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hc.yuexingan06.cn

Go:   defer f.Close()
来源：http://zu.asd995.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dc.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://og.chemitech.net.cn

================================================================================
来源：http://ry.shtwfgs.cn

I. 正则表达式
来源：http://cf.huixiangedu.cn

================================================================================
来源：http://qy.shtwfgs.cn

[I01] 判断是否匹配
来源：http://gv.shtwfgs.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ya.9csxet.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oj.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://zj.521024.cn

TS:   /\d+/.test(s)
来源：http://mn.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wn.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fv.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://ht.huixiangedu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jm.hahajie.cn

[I02] 提取所有匹配
来源：http://bv.shxzukj.cn

Py:   re.findall(r"\d+", s)
来源：http://gb.colortex.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lu.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rp.szsharing.cn

TS:   s.match(/\d+/g)
来源：http://qj.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lj.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qi.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://mh.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qe.huixinmuqiang.cn

[I03] 提取捕获分组
来源：http://qe.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bb.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cw.9csxet.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fx.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hg.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rp.panjiajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kg.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sf.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lt.yuntaijiaju.cn

[I04] 正则替换
来源：http://en.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zv.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gi.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xd.yuntaijiaju.cn

TS:   s.replace(/\d+/g, "#")
来源：http://dv.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://un.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ly.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jw.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xv.huixiangedu.cn

[I05] 按正则拆分
来源：http://yc.muxihuayi.cn


<!-- 参考信息 -->