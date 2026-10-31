代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://by.shtwfgs.cn

TS:   path.extname("a.txt")
来源：http://kz.bookmarksfly.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jz.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gw.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ih.asd995.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cq.shxzukj.cn

[F11] 复制与移动文件
来源：http://ob.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jq.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oc.szxytkj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aq.haigaiapp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xk.chemitech.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xn.szxytkj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nb.haigaiapp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://as.521024.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dp.nicolike.cn

[F12] CSV 读写
来源：http://yz.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://cp.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ha.newstarts.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://va.nicolike.cn

TS:   // 同上
来源：http://fp.hahajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gd.shxzskj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hj.panjiajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://qw.colortex.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bl.huanxung.cn

================================================================================
来源：http://cb.hnjuh.cn

G. 面向对象
来源：http://pr.huixinmuqiang.cn

================================================================================
来源：http://aa.szsharing.cn

[G01] 定义类
来源：http://uq.huixiangedu.cn

Py:   class User: pass
来源：http://kh.hnjuh.cn

PHP:  class User {}
来源：http://hr.9csxet.cn

JS:   class User {}
来源：http://ve.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://pe.shtwfgs.cn

Java: class User {}
来源：http://fo.wgjwhj.cn

Go:   type User struct { Name string }
来源：http://fu.9csxet.cn

Ruby: class User; end
来源：http://jj.jctech888.com.cn

C#:   class User {}
来源：http://nr.gzmigu.cn

[G02] 构造函数
来源：http://hx.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://uf.hahajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://dy.shtwfgs.cn

JS:   constructor(name) { this.name = name; }
来源：http://yz.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://lx.huixinmuqiang.cn

Java: User(String name) { this.name = name; }
来源：http://yq.gzmigu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zf.jianghongdianzi.cn

Ruby: def initialize(name); @name = name; end
来源：http://rm.huixinmuqiang.cn

C#:   public User(string name) { Name = name; }
来源：http://ra.bjjhwx.cn

[G03] 实例属性
来源：http://ep.gzmigu.cn

Py:   self.name = "x"
来源：http://of.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://by.nszjky.cn

JS:   this.name = "x";
来源：http://ez.szxytkj.cn

TS:   name: string = "x";
来源：http://yh.haigaiapp.cn

Java: private String name;
来源：http://wp.nszjky.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wm.muxihuayi.cn

Ruby: @name = "x"
来源：http://oq.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://nt.szsharing.cn

[G04] 定义方法
来源：http://xx.shxzukj.cn

Py:   def greet(self): return self.name
来源：http://pv.shxzskj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vm.newstarts.cn

JS:   greet() { return this.name; }
来源：http://zv.yuntaijiaju.cn

TS:   greet(): string { return this.name; }
来源：http://kv.nszjky.cn

Java: String greet() { return name; }
来源：http://gp.shxzukj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wx.shtwfgs.cn

Ruby: def greet; @name; end
来源：http://wl.colortex.cn

C#:   public string Greet() => Name;
来源：http://rc.nszjky.cn

[G05] 继承
来源：http://jh.hnjuh.cn

Py:   class Admin(User): pass
来源：http://lu.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://ux.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://pa.szxytkj.cn

TS:   class Admin extends User {}
来源：http://ct.lnxyls.cn

Java: class Admin extends User {}
来源：http://zg.shxzukj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ii.szxytkj.cn

Ruby: class Admin < User; end
来源：http://xs.jianghongdianzi.cn

C#:   class Admin : User {}
来源：http://lo.shtwfgs.cn

[G06] 重写方法
来源：http://ul.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://lu.nszjky.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jk.szxytkj.cn

JS:   greet() { return "admin"; }
来源：http://yz.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://gc.wgjwhj.cn

Java: @Override String greet() { return "admin"; }
来源：http://jv.shxzukj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nf.huixiangedu.cn

Ruby: def greet; "admin"; end
来源：http://vd.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://qo.muxihuayi.cn

[G07] 调用父类方法
来源：http://bw.bjjhwx.cn

Py:   super().greet()
来源：http://hy.shxzskj.cn

PHP:  parent::greet();
来源：http://fs.lnxyls.cn

JS:   super.greet();
来源：http://lm.lnxyls.cn

TS:   super.greet();
来源：http://ko.shtwfgs.cn

Java: super.greet();
来源：http://pz.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nw.gzmigu.cn

Ruby: super
来源：http://ml.panjiajie.cn

C#:   base.Greet();
来源：http://tw.muxihuayi.cn

[G08] 静态方法与属性
来源：http://lb.huanxung.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vl.newstarts.cn

PHP:  public static function f() {}
来源：http://kj.nszjky.cn

JS:   static f() {}
来源：http://tp.9csxet.cn

TS:   static f(): void {}
来源：http://tk.gzmigu.cn

Java: static void f() {}
来源：http://gl.hnjuh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fh.huanxung.cn

Ruby: def self.f; end
来源：http://mn.huixinmuqiang.cn

C#:   public static void F() {}
来源：http://zf.yuexingan06.cn

[G09] 接口 / 抽象类
来源：http://pd.huixiangedu.cn

Py:   from abc import ABC, abstractmethod
来源：http://wh.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vc.newstarts.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ca.yuntaijiaju.cn

TS:   interface Shape { area(): number; }
来源：http://ob.szsharing.cn

Java: interface Shape { double area(); }
来源：http://gk.jianghongdianzi.cn

Go:   type Shape interface { Area() float64 }
来源：http://oe.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cg.newstarts.cn

C#:   interface IShape { double Area(); }
来源：http://hx.lnxyls.cn

[G10] 访问控制
来源：http://zz.colortex.cn

Py:   约定 _protected / __private（不强制）
来源：http://hy.shxzskj.cn

PHP:  public / protected / private
来源：http://vw.colortex.cn

JS:   #private 字段；其余公开
来源：http://or.shtwfgs.cn

TS:   public / protected / private
来源：http://rd.shtwfgs.cn

Java: public / protected / private / 默认包级
来源：http://qz.haigaiapp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ns.521024.cn

Ruby: public / protected / private
来源：http://cc.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://mi.muxihuayi.cn

[G11] getter / setter
来源：http://kn.gzmigu.cn

Py:   @property 与 @x.setter
来源：http://yv.yuexingan06.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hs.haigaiapp.cn

JS:   get name() { return this._name; }
来源：http://ei.bjjhwx.cn

TS:   get name(): string { return this._name; }
来源：http://nh.yuntaijiaju.cn

Java: public String getName() { return name; }
来源：http://sh.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jt.szsharing.cn

Ruby: attr_accessor :name
来源：http://qy.521024.cn

C#:   public string Name { get; set; }
来源：http://py.nszjky.cn

[G12] 对象转字符串
来源：http://ow.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://it.bookmarksfly.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ux.gzmigu.cn

JS:   toString() { return this.name; }
来源：http://zu.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://iv.nszjky.cn

Java: @Override public String toString() { return name; }
来源：http://id.9csxet.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hr.asd995.cn

Ruby: def to_s; @name; end
来源：http://nd.shtwfgs.cn

C#:   public override string ToString() => Name;
来源：http://lc.bookmarksfly.cn

[G13] 判断对象类型
来源：http://ig.chemitech.net.cn

Py:   isinstance(u, User)
来源：http://ax.szxytkj.cn

PHP:  $u instanceof User
来源：http://ue.shxzukj.cn

JS:   u instanceof User
来源：http://nn.shtwfgs.cn

TS:   u instanceof User
来源：http://rx.9csxet.cn

Java: u instanceof User
来源：http://as.haigaiapp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sr.chemitech.net.cn

Ruby: u.is_a?(User)
来源：http://ib.huixinmuqiang.cn

C#:   u is User
来源：http://ly.lnxyls.cn

[G14] 数据类 / record
来源：http://ri.bjjhwx.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cl.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://ca.gzmigu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://el.bjjhwx.cn

TS:   type User = { name: string; age: number };
来源：http://bt.hnjuh.cn

Java: record User(String name, int age) {}
来源：http://mi.9csxet.cn

Go:   type User struct { Name string; Age int }
来源：http://at.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://al.panjiajie.cn

C#:   record User(string Name, int Age);
来源：http://jo.hahajie.cn

[G15] 枚举
来源：http://gr.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kr.yuntaijiaju.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vv.nicolike.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dt.lnxyls.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lq.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://rs.hnjuh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yb.hahajie.cn

Ruby: Color = %i[red green].freeze
来源：http://hr.asd995.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bx.shtwfgs.cn

[G16] 对象转数组 / 字典
来源：http://ek.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oy.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://ms.nszjky.cn

JS:   Object.entries(obj)
来源：http://vl.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://rn.szsharing.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gp.szsharing.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pw.shxzskj.cn

Ruby: obj.instance_variables
来源：http://mu.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://vt.wgjwhj.cn

================================================================================
来源：http://ao.gzmigu.cn

H. 异常与错误处理
来源：http://nl.521024.cn

================================================================================
来源：http://fq.nicolike.cn

[H01] try / catch 基础
来源：http://uz.szsharing.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vy.newstarts.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zo.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lx.bookmarksfly.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xa.hahajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://el.bookmarksfly.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sd.yuexingan06.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jp.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ay.szsharing.cn

[H02] finally / ensure 收尾
来源：http://tl.shxzukj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lg.huixinmuqiang.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://de.shxzukj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nu.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pb.lnxyls.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ri.colortex.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sy.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oa.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jb.chemitech.net.cn

[H03] 主动抛出异常
来源：http://iz.szxytkj.cn

Py:   raise ValueError("错误信息")
来源：http://ql.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kn.yuexingan06.cn

JS:   throw new Error("错误信息");
来源：http://zu.huanxung.cn

TS:   throw new Error("错误信息");
来源：http://ms.huixiangedu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://oq.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uw.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://em.chemitech.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ap.yuexingan06.cn

[H04] 自定义异常类型
来源：http://wg.szsharing.cn

Py:   class MyError(Exception): pass
来源：http://kl.asd995.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hb.yuntaijiaju.cn

JS:   class MyError extends Error {}
来源：http://mp.gzmigu.cn

TS:   class MyError extends Error {}
来源：http://sq.lnxyls.cn

Java: class MyException extends RuntimeException {}
来源：http://df.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pu.9csxet.cn

Ruby: class MyError < StandardError; end
来源：http://tr.lnxyls.cn

C#:   class MyException : Exception {}
来源：http://vh.9csxet.cn

[H05] 捕获特定类型
来源：http://mq.chemitech.net.cn

Py:   except ValueError as e:
来源：http://vd.shxzukj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bd.nicolike.cn

JS:   if (e instanceof TypeError) {}
来源：http://fb.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://ib.szxytkj.cn

Java: catch (IOException | SQLException e) {}
来源：http://kf.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bx.bookmarksfly.cn

Ruby: rescue ArgumentError => e
来源：http://cm.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oe.newstarts.cn

[H06] 可选值 / 空值安全访问
来源：http://ou.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://cn.nicolike.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qk.newstarts.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ru.nicolike.cn

TS:   obj?.a?.b;  d ?? default
来源：http://by.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mt.shtwfgs.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ql.shtwfgs.cn

Ruby: d&.dig(:a, :b)
来源：http://yz.yuntaijiaju.cn

C#:   obj?.A?.B ?? default
来源：http://oc.bookmarksfly.cn

[H07] 断言
来源：http://tf.bjjhwx.cn

Py:   assert x > 0, "必须为正"
来源：http://zs.asd995.cn

PHP:  assert($x > 0);
来源：http://yn.hahajie.cn

JS:   console.assert(x > 0);
来源：http://vm.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://nt.shxzskj.cn

Java: assert x > 0 : "必须为正";
来源：http://mw.huanxung.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pl.wgjwhj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jc.521024.cn

C#:   Debug.Assert(x > 0);
来源：http://gf.9csxet.cn

[H08] 获取错误信息与堆栈
来源：http://wq.bjjhwx.cn

Py:   str(e);  traceback.format_exc()
来源：http://le.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gm.muxihuayi.cn

JS:   e.message;  e.stack
来源：http://jq.panjiajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yc.jctech888.com.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fr.huixiangedu.cn

Go:   err.Error()
来源：http://ra.szxytkj.cn

Ruby: e.message;  e.backtrace
来源：http://rl.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://fw.9csxet.cn

[H09] 带错误码的异常
来源：http://dz.jianghongdianzi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cb.chemitech.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ew.shxzskj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ep.szsharing.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kj.huixiangedu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jv.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ro.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nw.nicolike.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lh.colortex.cn

[H10] 资源自动释放
来源：http://db.chemitech.net.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pd.nicolike.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fh.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cf.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vm.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zc.asd995.cn

Go:   defer f.Close()
来源：http://qq.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ll.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://go.jctech888.com.cn

================================================================================
来源：http://ys.newstarts.cn

I. 正则表达式
来源：http://pl.shtwfgs.cn

================================================================================
来源：http://jw.huixinmuqiang.cn

[I01] 判断是否匹配
来源：http://yz.hahajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dj.shtwfgs.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sm.huixinmuqiang.cn

JS:   /\d+/.test(s)
来源：http://bv.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://va.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zg.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://et.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://xq.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uj.huanxung.cn

[I02] 提取所有匹配
来源：http://jl.newstarts.cn

Py:   re.findall(r"\d+", s)
来源：http://zo.jianghongdianzi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yo.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xj.huixiangedu.cn

TS:   s.match(/\d+/g)
来源：http://nj.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gr.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://js.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://wg.jianghongdianzi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kr.muxihuayi.cn

[I03] 提取捕获分组
来源：http://cm.shxzskj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fp.521024.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pi.jianghongdianzi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hl.colortex.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://on.haigaiapp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kr.gzmigu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cm.newstarts.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yb.yuntaijiaju.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oj.9csxet.cn

[I04] 正则替换
来源：http://vj.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ak.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yl.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://rg.panjiajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ky.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cg.yuntaijiaju.cn


<!-- 参考信息 -->