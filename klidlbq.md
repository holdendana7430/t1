代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://um.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://oo.gzmigu.cn

[F11] 复制与移动文件
来源：http://kw.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uk.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xl.bjjhwx.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vr.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ef.gzmigu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://px.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ga.huanxung.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ti.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://as.hnjuh.cn

[F12] CSV 读写
来源：http://pp.muxihuayi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://tu.colortex.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://jw.haigaiapp.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hn.wgjwhj.cn

TS:   // 同上
来源：http://so.huixiangedu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ei.colortex.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mf.lnxyls.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://gk.huixinmuqiang.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://il.9csxet.cn

================================================================================
来源：http://fr.shxzukj.cn

G. 面向对象
来源：http://dn.shxzukj.cn

================================================================================
来源：http://bl.colortex.cn

[G01] 定义类
来源：http://tf.muxihuayi.cn

Py:   class User: pass
来源：http://zf.szxytkj.cn

PHP:  class User {}
来源：http://fm.muxihuayi.cn

JS:   class User {}
来源：http://dx.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://dx.jctech888.com.cn

Java: class User {}
来源：http://da.szxytkj.cn

Go:   type User struct { Name string }
来源：http://wn.521024.cn

Ruby: class User; end
来源：http://af.bjjhwx.cn

C#:   class User {}
来源：http://dr.shxzukj.cn

[G02] 构造函数
来源：http://pc.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://ce.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://wy.asd995.cn

JS:   constructor(name) { this.name = name; }
来源：http://ts.asd995.cn

TS:   constructor(public name: string) {}
来源：http://kz.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://sj.yuntaijiaju.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fe.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://dx.shtwfgs.cn

C#:   public User(string name) { Name = name; }
来源：http://kk.haigaiapp.cn

[G03] 实例属性
来源：http://zm.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://bg.asd995.cn

PHP:  public string $name = "x";
来源：http://lg.szxytkj.cn

JS:   this.name = "x";
来源：http://wu.nicolike.cn

TS:   name: string = "x";
来源：http://ak.colortex.cn

Java: private String name;
来源：http://db.panjiajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qa.szsharing.cn

Ruby: @name = "x"
来源：http://zi.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://du.colortex.cn

[G04] 定义方法
来源：http://gv.huixiangedu.cn

Py:   def greet(self): return self.name
来源：http://mm.haigaiapp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qu.nicolike.cn

JS:   greet() { return this.name; }
来源：http://al.jctech888.com.cn

TS:   greet(): string { return this.name; }
来源：http://hm.bookmarksfly.cn

Java: String greet() { return name; }
来源：http://pf.nszjky.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vb.haigaiapp.cn

Ruby: def greet; @name; end
来源：http://wk.huixinmuqiang.cn

C#:   public string Greet() => Name;
来源：http://in.hnjuh.cn

[G05] 继承
来源：http://up.panjiajie.cn

Py:   class Admin(User): pass
来源：http://xx.yuntaijiaju.cn

PHP:  class Admin extends User {}
来源：http://ld.jctech888.com.cn

JS:   class Admin extends User {}
来源：http://xy.szxytkj.cn

TS:   class Admin extends User {}
来源：http://nu.lnxyls.cn

Java: class Admin extends User {}
来源：http://ye.shxzukj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://in.shxzukj.cn

Ruby: class Admin < User; end
来源：http://wh.521024.cn

C#:   class Admin : User {}
来源：http://ib.asd995.cn

[G06] 重写方法
来源：http://ta.bookmarksfly.cn

Py:   def greet(self): return "admin"
来源：http://wo.muxihuayi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ux.huixiangedu.cn

JS:   greet() { return "admin"; }
来源：http://tv.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://bi.panjiajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://ci.hnjuh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uq.szxytkj.cn

Ruby: def greet; "admin"; end
来源：http://jq.jctech888.com.cn

C#:   public override string Greet() => "admin";
来源：http://bj.yuexingan06.cn

[G07] 调用父类方法
来源：http://kr.shxzskj.cn

Py:   super().greet()
来源：http://wv.huixiangedu.cn

PHP:  parent::greet();
来源：http://ek.bjjhwx.cn

JS:   super.greet();
来源：http://kg.szxytkj.cn

TS:   super.greet();
来源：http://bh.hahajie.cn

Java: super.greet();
来源：http://gb.jctech888.com.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ql.shxzukj.cn

Ruby: super
来源：http://dl.lnxyls.cn

C#:   base.Greet();
来源：http://jj.panjiajie.cn

[G08] 静态方法与属性
来源：http://rd.szxytkj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://aa.hnjuh.cn

PHP:  public static function f() {}
来源：http://au.asd995.cn

JS:   static f() {}
来源：http://zh.yuntaijiaju.cn

TS:   static f(): void {}
来源：http://uu.nicolike.cn

Java: static void f() {}
来源：http://cc.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ud.9csxet.cn

Ruby: def self.f; end
来源：http://ml.newstarts.cn

C#:   public static void F() {}
来源：http://yx.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://ra.hnjuh.cn

Py:   from abc import ABC, abstractmethod
来源：http://kw.lnxyls.cn

PHP:  interface Shape { public function area(): float; }
来源：http://op.lnxyls.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vu.newstarts.cn

TS:   interface Shape { area(): number; }
来源：http://sr.jctech888.com.cn

Java: interface Shape { double area(); }
来源：http://wo.yuexingan06.cn

Go:   type Shape interface { Area() float64 }
来源：http://ij.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lw.szxytkj.cn

C#:   interface IShape { double Area(); }
来源：http://jj.shxzukj.cn

[G10] 访问控制
来源：http://jf.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://zw.muxihuayi.cn

PHP:  public / protected / private
来源：http://ai.asd995.cn

JS:   #private 字段；其余公开
来源：http://gi.521024.cn

TS:   public / protected / private
来源：http://sx.colortex.cn

Java: public / protected / private / 默认包级
来源：http://kv.nszjky.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://my.shxzukj.cn

Ruby: public / protected / private
来源：http://yt.szsharing.cn

C#:   public / protected / private / internal
来源：http://tt.colortex.cn

[G11] getter / setter
来源：http://ep.colortex.cn

Py:   @property 与 @x.setter
来源：http://fi.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wl.muxihuayi.cn

JS:   get name() { return this._name; }
来源：http://da.hahajie.cn

TS:   get name(): string { return this._name; }
来源：http://lu.bookmarksfly.cn

Java: public String getName() { return name; }
来源：http://wy.hnjuh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nr.shxzskj.cn

Ruby: attr_accessor :name
来源：http://mk.haigaiapp.cn

C#:   public string Name { get; set; }
来源：http://df.szxytkj.cn

[G12] 对象转字符串
来源：http://ox.huixiangedu.cn

Py:   def __str__(self): return self.name
来源：http://nt.chemitech.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gm.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://wp.colortex.cn

TS:   toString(): string { return this.name; }
来源：http://mb.521024.cn

Java: @Override public String toString() { return name; }
来源：http://fs.asd995.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cn.shxzskj.cn

Ruby: def to_s; @name; end
来源：http://jv.chemitech.net.cn

C#:   public override string ToString() => Name;
来源：http://bc.huixiangedu.cn

[G13] 判断对象类型
来源：http://jy.jianghongdianzi.cn

Py:   isinstance(u, User)
来源：http://bb.hnjuh.cn

PHP:  $u instanceof User
来源：http://af.shxzskj.cn

JS:   u instanceof User
来源：http://ou.szsharing.cn

TS:   u instanceof User
来源：http://qf.szsharing.cn

Java: u instanceof User
来源：http://hz.huixiangedu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://py.lnxyls.cn

Ruby: u.is_a?(User)
来源：http://jq.nicolike.cn

C#:   u is User
来源：http://ar.gzmigu.cn

[G14] 数据类 / record
来源：http://ec.panjiajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ey.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://ky.521024.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pw.asd995.cn

TS:   type User = { name: string; age: number };
来源：http://qj.szsharing.cn

Java: record User(String name, int age) {}
来源：http://ki.huanxung.cn

Go:   type User struct { Name string; Age int }
来源：http://mt.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dt.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://oc.wgjwhj.cn

[G15] 枚举
来源：http://vw.haigaiapp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kd.asd995.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qz.huixinmuqiang.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://iz.bjjhwx.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zk.gzmigu.cn

Java: enum Color { RED, GREEN }
来源：http://jf.chemitech.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lf.bjjhwx.cn

Ruby: Color = %i[red green].freeze
来源：http://uj.nszjky.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ri.muxihuayi.cn

[G16] 对象转数组 / 字典
来源：http://or.shxzskj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://le.521024.cn

PHP:  get_object_vars($obj);
来源：http://yi.nicolike.cn

JS:   Object.entries(obj)
来源：http://fs.newstarts.cn

TS:   Object.entries(obj)
来源：http://di.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hp.asd995.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kb.bookmarksfly.cn

Ruby: obj.instance_variables
来源：http://wp.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://ev.521024.cn

================================================================================
来源：http://ob.asd995.cn

H. 异常与错误处理
来源：http://ei.yuexingan06.cn

================================================================================
来源：http://jm.hahajie.cn

[H01] try / catch 基础
来源：http://ti.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qm.lnxyls.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zz.lnxyls.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yy.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://st.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ld.huanxung.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gl.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rz.szxytkj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pe.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://at.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fp.wgjwhj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tv.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://im.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pi.jianghongdianzi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://go.shxzukj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hh.chemitech.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://uo.nszjky.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qg.panjiajie.cn

[H03] 主动抛出异常
来源：http://gr.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://pt.hnjuh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jj.bjjhwx.cn

JS:   throw new Error("错误信息");
来源：http://fn.yuexingan06.cn

TS:   throw new Error("错误信息");
来源：http://ol.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ve.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qm.jctech888.com.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jj.shxzskj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xm.nicolike.cn

[H04] 自定义异常类型
来源：http://gw.shxzskj.cn

Py:   class MyError(Exception): pass
来源：http://ja.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://he.9csxet.cn

JS:   class MyError extends Error {}
来源：http://vi.nicolike.cn

TS:   class MyError extends Error {}
来源：http://yw.lnxyls.cn

Java: class MyException extends RuntimeException {}
来源：http://uc.yuexingan06.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://su.nszjky.cn

Ruby: class MyError < StandardError; end
来源：http://ym.bjjhwx.cn

C#:   class MyException : Exception {}
来源：http://zt.bookmarksfly.cn

[H05] 捕获特定类型
来源：http://tt.haigaiapp.cn

Py:   except ValueError as e:
来源：http://hh.jianghongdianzi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ky.haigaiapp.cn

JS:   if (e instanceof TypeError) {}
来源：http://fa.yuexingan06.cn

TS:   if (e instanceof TypeError) {}
来源：http://wf.521024.cn

Java: catch (IOException | SQLException e) {}
来源：http://uw.nicolike.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tq.bjjhwx.cn

Ruby: rescue ArgumentError => e
来源：http://hd.muxihuayi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jz.yuntaijiaju.cn

[H06] 可选值 / 空值安全访问
来源：http://iv.jctech888.com.cn

Py:   value = d.get("k") or default
来源：http://lc.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ck.bjjhwx.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fb.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gd.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qx.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mm.yuntaijiaju.cn

Ruby: d&.dig(:a, :b)
来源：http://be.szxytkj.cn

C#:   obj?.A?.B ?? default
来源：http://ck.muxihuayi.cn

[H07] 断言
来源：http://zx.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://hu.szsharing.cn

PHP:  assert($x > 0);
来源：http://ag.shtwfgs.cn

JS:   console.assert(x > 0);
来源：http://xx.colortex.cn

TS:   console.assert(x > 0);
来源：http://pv.newstarts.cn

Java: assert x > 0 : "必须为正";
来源：http://qz.hahajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fd.yuntaijiaju.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fq.colortex.cn

C#:   Debug.Assert(x > 0);
来源：http://bp.bjjhwx.cn

[H08] 获取错误信息与堆栈
来源：http://dl.shtwfgs.cn

Py:   str(e);  traceback.format_exc()
来源：http://pe.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cz.521024.cn

JS:   e.message;  e.stack
来源：http://em.asd995.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ya.huanxung.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rc.szxytkj.cn

Go:   err.Error()
来源：http://sa.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://fs.gzmigu.cn

C#:   e.Message;  e.StackTrace
来源：http://tu.szxytkj.cn

[H09] 带错误码的异常
来源：http://sj.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mz.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pk.wgjwhj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://to.shxzskj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pb.asd995.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lz.huanxung.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ux.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vo.yuexingan06.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tj.hnjuh.cn

[H10] 资源自动释放
来源：http://oo.nszjky.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://er.szsharing.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xt.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ym.jianghongdianzi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ym.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xl.gzmigu.cn

Go:   defer f.Close()
来源：http://pb.hnjuh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ua.chemitech.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mc.haigaiapp.cn

================================================================================
来源：http://to.szxytkj.cn

I. 正则表达式
来源：http://kt.muxihuayi.cn

================================================================================
来源：http://lh.szxytkj.cn

[I01] 判断是否匹配
来源：http://ua.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mn.asd995.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ap.521024.cn

JS:   /\d+/.test(s)
来源：http://os.huixiangedu.cn

TS:   /\d+/.test(s)
来源：http://ab.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zy.huanxung.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bw.szsharing.cn

Ruby: s.match?(/\d+/)
来源：http://ib.szxytkj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shxzskj.cn

[I02] 提取所有匹配
来源：http://kh.huanxung.cn

Py:   re.findall(r"\d+", s)
来源：http://ij.colortex.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kl.haigaiapp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hh.haigaiapp.cn

TS:   s.match(/\d+/g)
来源：http://py.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yv.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://te.jianghongdianzi.cn

Ruby: s.scan(/\d+/)
来源：http://rc.huanxung.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hr.9csxet.cn

[I03] 提取捕获分组
来源：http://ok.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fl.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bm.nicolike.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://am.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ja.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rs.bjjhwx.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sm.yuexingan06.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xl.chemitech.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ox.shtwfgs.cn

[I04] 正则替换
来源：http://pz.wgjwhj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tc.asd995.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cw.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wn.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qu.chemitech.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://og.gzmigu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kw.yuntaijiaju.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ap.nszjky.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tv.wgjwhj.cn

[I05] 按正则拆分
来源：http://bu.muxihuayi.cn


<!-- 参考信息 -->