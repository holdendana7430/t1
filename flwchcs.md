代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kw.asd995.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zz.9csxet.cn

[F11] 复制与移动文件
来源：http://cc.haigaiapp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nc.huixiangedu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qk.newstarts.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://de.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://df.yuexingan06.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rr.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://eg.hahajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yk.asd995.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qj.newstarts.cn

[F12] CSV 读写
来源：http://us.shxzskj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ar.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://is.haigaiapp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://jr.hnjuh.cn

TS:   // 同上
来源：http://lv.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oc.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ku.521024.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rh.hahajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sr.shtwfgs.cn

================================================================================
来源：http://au.shxzskj.cn

G. 面向对象
来源：http://kr.wgjwhj.cn

================================================================================
来源：http://bz.yuntaijiaju.cn

[G01] 定义类
来源：http://wg.newstarts.cn

Py:   class User: pass
来源：http://ji.asd995.cn

PHP:  class User {}
来源：http://og.shxzskj.cn

JS:   class User {}
来源：http://hp.colortex.cn

TS:   class User { name: string = ""; }
来源：http://dh.bookmarksfly.cn

Java: class User {}
来源：http://hp.shxzukj.cn

Go:   type User struct { Name string }
来源：http://eh.shxzskj.cn

Ruby: class User; end
来源：http://tk.huixinmuqiang.cn

C#:   class User {}
来源：http://nu.9csxet.cn

[G02] 构造函数
来源：http://wa.bookmarksfly.cn

Py:   def __init__(self, name): self.name = name
来源：http://gk.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://tm.shxzskj.cn

JS:   constructor(name) { this.name = name; }
来源：http://fs.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://ng.huixiangedu.cn

Java: User(String name) { this.name = name; }
来源：http://oh.newstarts.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pk.jianghongdianzi.cn

Ruby: def initialize(name); @name = name; end
来源：http://kt.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://dv.panjiajie.cn

[G03] 实例属性
来源：http://rh.huixinmuqiang.cn

Py:   self.name = "x"
来源：http://oi.szsharing.cn

PHP:  public string $name = "x";
来源：http://kl.yuexingan06.cn

JS:   this.name = "x";
来源：http://uh.9csxet.cn

TS:   name: string = "x";
来源：http://ot.yuntaijiaju.cn

Java: private String name;
来源：http://ca.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yz.muxihuayi.cn

Ruby: @name = "x"
来源：http://nu.shxzskj.cn

C#:   public string Name { get; set; } = "x";
来源：http://qs.shxzukj.cn

[G04] 定义方法
来源：http://sg.colortex.cn

Py:   def greet(self): return self.name
来源：http://xr.lnxyls.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fh.jctech888.com.cn

JS:   greet() { return this.name; }
来源：http://ey.jctech888.com.cn

TS:   greet(): string { return this.name; }
来源：http://hs.huanxung.cn

Java: String greet() { return name; }
来源：http://cz.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://et.chemitech.net.cn

Ruby: def greet; @name; end
来源：http://rp.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://wi.nszjky.cn

[G05] 继承
来源：http://hj.yuntaijiaju.cn

Py:   class Admin(User): pass
来源：http://gx.bookmarksfly.cn

PHP:  class Admin extends User {}
来源：http://ay.lnxyls.cn

JS:   class Admin extends User {}
来源：http://vd.huanxung.cn

TS:   class Admin extends User {}
来源：http://go.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://op.muxihuayi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lh.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://xa.hahajie.cn

C#:   class Admin : User {}
来源：http://dk.shtwfgs.cn

[G06] 重写方法
来源：http://vz.haigaiapp.cn

Py:   def greet(self): return "admin"
来源：http://zs.9csxet.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ft.haigaiapp.cn

JS:   greet() { return "admin"; }
来源：http://ji.hahajie.cn

TS:   greet(): string { return "admin"; }
来源：http://ok.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://fc.521024.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ah.nszjky.cn

Ruby: def greet; "admin"; end
来源：http://xe.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://cj.gzmigu.cn

[G07] 调用父类方法
来源：http://sr.huixiangedu.cn

Py:   super().greet()
来源：http://xy.muxihuayi.cn

PHP:  parent::greet();
来源：http://ha.bjjhwx.cn

JS:   super.greet();
来源：http://mu.shxzskj.cn

TS:   super.greet();
来源：http://mu.szxytkj.cn

Java: super.greet();
来源：http://zn.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sf.gzmigu.cn

Ruby: super
来源：http://jj.hnjuh.cn

C#:   base.Greet();
来源：http://uf.jctech888.com.cn

[G08] 静态方法与属性
来源：http://kb.huixinmuqiang.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dx.shxzukj.cn

PHP:  public static function f() {}
来源：http://rd.asd995.cn

JS:   static f() {}
来源：http://yi.nszjky.cn

TS:   static f(): void {}
来源：http://tl.chemitech.net.cn

Java: static void f() {}
来源：http://py.huixiangedu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wm.nszjky.cn

Ruby: def self.f; end
来源：http://gi.bookmarksfly.cn

C#:   public static void F() {}
来源：http://lt.huixiangedu.cn

[G09] 接口 / 抽象类
来源：http://rn.chemitech.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://ia.9csxet.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jq.521024.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lt.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://uy.shxzukj.cn

Java: interface Shape { double area(); }
来源：http://vn.lnxyls.cn

Go:   type Shape interface { Area() float64 }
来源：http://qt.yuntaijiaju.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tu.szxytkj.cn

C#:   interface IShape { double Area(); }
来源：http://lj.panjiajie.cn

[G10] 访问控制
来源：http://ne.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://ur.9csxet.cn

PHP:  public / protected / private
来源：http://pc.szxytkj.cn

JS:   #private 字段；其余公开
来源：http://vb.newstarts.cn

TS:   public / protected / private
来源：http://im.hnjuh.cn

Java: public / protected / private / 默认包级
来源：http://nq.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sj.szsharing.cn

Ruby: public / protected / private
来源：http://we.shxzskj.cn

C#:   public / protected / private / internal
来源：http://gm.jianghongdianzi.cn

[G11] getter / setter
来源：http://jm.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://jg.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://oc.hahajie.cn

JS:   get name() { return this._name; }
来源：http://es.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://od.bjjhwx.cn

Java: public String getName() { return name; }
来源：http://ae.hnjuh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ax.nicolike.cn

Ruby: attr_accessor :name
来源：http://ta.panjiajie.cn

C#:   public string Name { get; set; }
来源：http://qt.huixiangedu.cn

[G12] 对象转字符串
来源：http://qt.wgjwhj.cn

Py:   def __str__(self): return self.name
来源：http://ng.muxihuayi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xh.muxihuayi.cn

JS:   toString() { return this.name; }
来源：http://rw.huixiangedu.cn

TS:   toString(): string { return this.name; }
来源：http://od.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://bb.chemitech.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ne.haigaiapp.cn

Ruby: def to_s; @name; end
来源：http://ik.huixinmuqiang.cn

C#:   public override string ToString() => Name;
来源：http://vk.shxzskj.cn

[G13] 判断对象类型
来源：http://yk.chemitech.net.cn

Py:   isinstance(u, User)
来源：http://yk.colortex.cn

PHP:  $u instanceof User
来源：http://ey.haigaiapp.cn

JS:   u instanceof User
来源：http://db.szsharing.cn

TS:   u instanceof User
来源：http://rm.haigaiapp.cn

Java: u instanceof User
来源：http://po.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xd.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://vj.shxzukj.cn

C#:   u is User
来源：http://cn.haigaiapp.cn

[G14] 数据类 / record
来源：http://xo.9csxet.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jh.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://dv.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sf.gzmigu.cn

TS:   type User = { name: string; age: number };
来源：http://ue.yuexingan06.cn

Java: record User(String name, int age) {}
来源：http://sc.wgjwhj.cn

Go:   type User struct { Name string; Age int }
来源：http://rk.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xo.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://lv.huixinmuqiang.cn

[G15] 枚举
来源：http://tz.szxytkj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xl.huixiangedu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pb.huanxung.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ix.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://us.muxihuayi.cn

Java: enum Color { RED, GREEN }
来源：http://bl.gzmigu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://su.huixinmuqiang.cn

Ruby: Color = %i[red green].freeze
来源：http://gs.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lu.muxihuayi.cn

[G16] 对象转数组 / 字典
来源：http://od.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bn.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://px.shtwfgs.cn

JS:   Object.entries(obj)
来源：http://tk.lnxyls.cn

TS:   Object.entries(obj)
来源：http://rq.wgjwhj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gs.shtwfgs.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vn.hahajie.cn

Ruby: obj.instance_variables
来源：http://kp.chemitech.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://wf.huixiangedu.cn

================================================================================
来源：http://jt.panjiajie.cn

H. 异常与错误处理
来源：http://ps.panjiajie.cn

================================================================================
来源：http://sz.9csxet.cn

[H01] try / catch 基础
来源：http://hm.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zv.nszjky.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tf.yuntaijiaju.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nx.colortex.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://as.shxzskj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yt.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lk.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yu.nszjky.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xb.nszjky.cn

[H02] finally / ensure 收尾
来源：http://se.bjjhwx.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gi.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ko.haigaiapp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hy.bjjhwx.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://br.asd995.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xz.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cb.szxytkj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hj.colortex.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wh.jctech888.com.cn

[H03] 主动抛出异常
来源：http://af.nicolike.cn

Py:   raise ValueError("错误信息")
来源：http://qz.yuexingan06.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ey.bjjhwx.cn

JS:   throw new Error("错误信息");
来源：http://wk.jianghongdianzi.cn

TS:   throw new Error("错误信息");
来源：http://rn.newstarts.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mw.huanxung.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yy.nicolike.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://oi.yuntaijiaju.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yv.nszjky.cn

[H04] 自定义异常类型
来源：http://sp.9csxet.cn

Py:   class MyError(Exception): pass
来源：http://tn.yuntaijiaju.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rr.newstarts.cn

JS:   class MyError extends Error {}
来源：http://io.jianghongdianzi.cn

TS:   class MyError extends Error {}
来源：http://le.huixiangedu.cn

Java: class MyException extends RuntimeException {}
来源：http://nj.newstarts.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rw.nszjky.cn

Ruby: class MyError < StandardError; end
来源：http://pv.yuntaijiaju.cn

C#:   class MyException : Exception {}
来源：http://aa.nicolike.cn

[H05] 捕获特定类型
来源：http://hp.yuexingan06.cn

Py:   except ValueError as e:
来源：http://vb.panjiajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qf.hnjuh.cn

JS:   if (e instanceof TypeError) {}
来源：http://dr.nicolike.cn

TS:   if (e instanceof TypeError) {}
来源：http://dh.szxytkj.cn

Java: catch (IOException | SQLException e) {}
来源：http://xj.panjiajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jc.muxihuayi.cn

Ruby: rescue ArgumentError => e
来源：http://rg.hahajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yk.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://wp.nicolike.cn

Py:   value = d.get("k") or default
来源：http://gx.bjjhwx.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fc.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qs.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mi.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gn.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rh.bjjhwx.cn

Ruby: d&.dig(:a, :b)
来源：http://pt.szsharing.cn

C#:   obj?.A?.B ?? default
来源：http://ay.jianghongdianzi.cn

[H07] 断言
来源：http://hp.szsharing.cn

Py:   assert x > 0, "必须为正"
来源：http://jm.lnxyls.cn

PHP:  assert($x > 0);
来源：http://yv.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://fu.nicolike.cn

TS:   console.assert(x > 0);
来源：http://co.9csxet.cn

Java: assert x > 0 : "必须为正";
来源：http://hb.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lq.hnjuh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ir.gzmigu.cn

C#:   Debug.Assert(x > 0);
来源：http://rg.yuntaijiaju.cn

[H08] 获取错误信息与堆栈
来源：http://gc.yuntaijiaju.cn

Py:   str(e);  traceback.format_exc()
来源：http://gt.muxihuayi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yw.muxihuayi.cn

JS:   e.message;  e.stack
来源：http://hs.szsharing.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mo.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ja.huixinmuqiang.cn

Go:   err.Error()
来源：http://vg.huanxung.cn

Ruby: e.message;  e.backtrace
来源：http://zy.nicolike.cn

C#:   e.Message;  e.StackTrace
来源：http://zd.huixinmuqiang.cn

[H09] 带错误码的异常
来源：http://di.nszjky.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oy.huanxung.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vt.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ec.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ef.muxihuayi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ct.nicolike.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hi.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ok.haigaiapp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ha.hahajie.cn

[H10] 资源自动释放
来源：http://yn.bjjhwx.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wy.hahajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yg.bjjhwx.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fw.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ol.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.shxzukj.cn

Go:   defer f.Close()
来源：http://xb.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gu.huanxung.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gr.521024.cn

================================================================================
来源：http://tm.yuexingan06.cn

I. 正则表达式
来源：http://pe.lnxyls.cn

================================================================================
来源：http://mk.huanxung.cn

[I01] 判断是否匹配
来源：http://ro.shxzukj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zl.haigaiapp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sm.wgjwhj.cn

JS:   /\d+/.test(s)
来源：http://iv.521024.cn

TS:   /\d+/.test(s)
来源：http://av.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kv.9csxet.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lr.huixiangedu.cn

Ruby: s.match?(/\d+/)
来源：http://jx.gzmigu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ic.lnxyls.cn

[I02] 提取所有匹配
来源：http://ki.huixinmuqiang.cn

Py:   re.findall(r"\d+", s)
来源：http://pb.szsharing.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lx.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vk.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://wg.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zh.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dq.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://lo.shxzukj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lf.panjiajie.cn

[I03] 提取捕获分组
来源：http://fv.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wh.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://go.panjiajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hd.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ss.muxihuayi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ge.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zc.lnxyls.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xr.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qs.nszjky.cn

[I04] 正则替换
来源：http://gk.nszjky.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mt.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ob.haigaiapp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://eq.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wj.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dl.yuntaijiaju.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wg.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://af.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qn.shxzskj.cn

[I05] 按正则拆分
来源：http://ro.bookmarksfly.cn


<!-- 参考信息 -->