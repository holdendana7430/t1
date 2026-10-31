代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ow.shxzukj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xb.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lq.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://gk.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rx.huixinmuqiang.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fn.shtwfgs.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mn.wgjwhj.cn

[F12] CSV 读写
来源：http://oi.gzmigu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mz.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nh.yuexingan06.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hp.muxihuayi.cn

TS:   // 同上
来源：http://vg.szsharing.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ds.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qt.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xe.bookmarksfly.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bd.bookmarksfly.cn

================================================================================
来源：http://qy.shtwfgs.cn

G. 面向对象
来源：http://zn.lnxyls.cn

================================================================================
来源：http://qc.huixiangedu.cn

[G01] 定义类
来源：http://ya.bookmarksfly.cn

Py:   class User: pass
来源：http://an.yuexingan06.cn

PHP:  class User {}
来源：http://lz.shtwfgs.cn

JS:   class User {}
来源：http://en.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://kd.gzmigu.cn

Java: class User {}
来源：http://jt.szxytkj.cn

Go:   type User struct { Name string }
来源：http://lg.nszjky.cn

Ruby: class User; end
来源：http://qx.panjiajie.cn

C#:   class User {}
来源：http://sj.panjiajie.cn

[G02] 构造函数
来源：http://jm.huanxung.cn

Py:   def __init__(self, name): self.name = name
来源：http://gy.nicolike.cn

PHP:  public function __construct(public string $name) {}
来源：http://xc.newstarts.cn

JS:   constructor(name) { this.name = name; }
来源：http://fl.jctech888.com.cn

TS:   constructor(public name: string) {}
来源：http://ty.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://mi.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fw.nicolike.cn

Ruby: def initialize(name); @name = name; end
来源：http://iu.jctech888.com.cn

C#:   public User(string name) { Name = name; }
来源：http://dm.panjiajie.cn

[G03] 实例属性
来源：http://hx.bjjhwx.cn

Py:   self.name = "x"
来源：http://go.haigaiapp.cn

PHP:  public string $name = "x";
来源：http://tw.nszjky.cn

JS:   this.name = "x";
来源：http://ni.gzmigu.cn

TS:   name: string = "x";
来源：http://un.hnjuh.cn

Java: private String name;
来源：http://ec.jctech888.com.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jp.lnxyls.cn

Ruby: @name = "x"
来源：http://sn.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://ju.bookmarksfly.cn

[G04] 定义方法
来源：http://fb.521024.cn

Py:   def greet(self): return self.name
来源：http://fj.jianghongdianzi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ea.nszjky.cn

JS:   greet() { return this.name; }
来源：http://co.asd995.cn

TS:   greet(): string { return this.name; }
来源：http://eg.hnjuh.cn

Java: String greet() { return name; }
来源：http://wq.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://oc.colortex.cn

Ruby: def greet; @name; end
来源：http://nk.huixiangedu.cn

C#:   public string Greet() => Name;
来源：http://ll.9csxet.cn

[G05] 继承
来源：http://ge.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://ek.huixinmuqiang.cn

PHP:  class Admin extends User {}
来源：http://cn.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://mb.panjiajie.cn

TS:   class Admin extends User {}
来源：http://bj.newstarts.cn

Java: class Admin extends User {}
来源：http://hk.shxzukj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ww.wgjwhj.cn

Ruby: class Admin < User; end
来源：http://hq.shtwfgs.cn

C#:   class Admin : User {}
来源：http://dz.hahajie.cn

[G06] 重写方法
来源：http://pj.bjjhwx.cn

Py:   def greet(self): return "admin"
来源：http://wb.hahajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rh.asd995.cn

JS:   greet() { return "admin"; }
来源：http://yf.haigaiapp.cn

TS:   greet(): string { return "admin"; }
来源：http://jb.shtwfgs.cn

Java: @Override String greet() { return "admin"; }
来源：http://ha.9csxet.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fz.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://ar.yuexingan06.cn

C#:   public override string Greet() => "admin";
来源：http://ir.jianghongdianzi.cn

[G07] 调用父类方法
来源：http://bv.jianghongdianzi.cn

Py:   super().greet()
来源：http://pq.szxytkj.cn

PHP:  parent::greet();
来源：http://yw.jianghongdianzi.cn

JS:   super.greet();
来源：http://yk.9csxet.cn

TS:   super.greet();
来源：http://wy.nicolike.cn

Java: super.greet();
来源：http://qd.jctech888.com.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tu.shtwfgs.cn

Ruby: super
来源：http://zv.gzmigu.cn

C#:   base.Greet();
来源：http://bq.panjiajie.cn

[G08] 静态方法与属性
来源：http://hu.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nv.nicolike.cn

PHP:  public static function f() {}
来源：http://cm.shtwfgs.cn

JS:   static f() {}
来源：http://rs.shtwfgs.cn

TS:   static f(): void {}
来源：http://tj.newstarts.cn

Java: static void f() {}
来源：http://pk.muxihuayi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qh.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://on.asd995.cn

C#:   public static void F() {}
来源：http://zp.szsharing.cn

[G09] 接口 / 抽象类
来源：http://re.wgjwhj.cn

Py:   from abc import ABC, abstractmethod
来源：http://zs.huixiangedu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vo.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zg.wgjwhj.cn

TS:   interface Shape { area(): number; }
来源：http://pc.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://lz.hnjuh.cn

Go:   type Shape interface { Area() float64 }
来源：http://sn.nszjky.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xi.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://yw.yuntaijiaju.cn

[G10] 访问控制
来源：http://li.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://nb.haigaiapp.cn

PHP:  public / protected / private
来源：http://ms.panjiajie.cn

JS:   #private 字段；其余公开
来源：http://ac.nicolike.cn

TS:   public / protected / private
来源：http://ok.wgjwhj.cn

Java: public / protected / private / 默认包级
来源：http://ij.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wl.nszjky.cn

Ruby: public / protected / private
来源：http://mt.newstarts.cn

C#:   public / protected / private / internal
来源：http://mz.szsharing.cn

[G11] getter / setter
来源：http://nh.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://fn.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://oe.colortex.cn

JS:   get name() { return this._name; }
来源：http://ba.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://at.huixiangedu.cn

Java: public String getName() { return name; }
来源：http://vk.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kf.panjiajie.cn

Ruby: attr_accessor :name
来源：http://qb.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://uz.jianghongdianzi.cn

[G12] 对象转字符串
来源：http://zm.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://fw.shxzskj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://me.szsharing.cn

JS:   toString() { return this.name; }
来源：http://qf.bjjhwx.cn

TS:   toString(): string { return this.name; }
来源：http://ij.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://zq.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bt.gzmigu.cn

Ruby: def to_s; @name; end
来源：http://od.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://qu.hnjuh.cn

[G13] 判断对象类型
来源：http://ll.shxzskj.cn

Py:   isinstance(u, User)
来源：http://bk.szsharing.cn

PHP:  $u instanceof User
来源：http://ma.yuexingan06.cn

JS:   u instanceof User
来源：http://vk.gzmigu.cn

TS:   u instanceof User
来源：http://kr.hnjuh.cn

Java: u instanceof User
来源：http://sb.nszjky.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zz.asd995.cn

Ruby: u.is_a?(User)
来源：http://ke.9csxet.cn

C#:   u is User
来源：http://fq.panjiajie.cn

[G14] 数据类 / record
来源：http://dk.shxzskj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ku.521024.cn

PHP:  // 用 readonly 属性模拟
来源：http://pi.szxytkj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ir.huixiangedu.cn

TS:   type User = { name: string; age: number };
来源：http://tp.haigaiapp.cn

Java: record User(String name, int age) {}
来源：http://au.bookmarksfly.cn

Go:   type User struct { Name string; Age int }
来源：http://gx.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fb.haigaiapp.cn

C#:   record User(string Name, int Age);
来源：http://vh.yuntaijiaju.cn

[G15] 枚举
来源：http://zr.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://if.bookmarksfly.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ri.muxihuayi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xr.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kk.szxytkj.cn

Java: enum Color { RED, GREEN }
来源：http://wt.huixiangedu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hs.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://ia.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nc.haigaiapp.cn

[G16] 对象转数组 / 字典
来源：http://tg.bookmarksfly.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://aa.gzmigu.cn

PHP:  get_object_vars($obj);
来源：http://oj.lnxyls.cn

JS:   Object.entries(obj)
来源：http://ox.gzmigu.cn

TS:   Object.entries(obj)
来源：http://vf.521024.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fp.jctech888.com.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ft.newstarts.cn

Ruby: obj.instance_variables
来源：http://uc.521024.cn

C#:   // 用反射或 System.Text.Json
来源：http://fo.jctech888.com.cn

================================================================================
来源：http://ik.gzmigu.cn

H. 异常与错误处理
来源：http://jf.jctech888.com.cn

================================================================================
来源：http://sv.colortex.cn

[H01] try / catch 基础
来源：http://ht.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vf.panjiajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dg.hahajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pu.jctech888.com.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sc.9csxet.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://et.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fw.muxihuayi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tw.haigaiapp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gz.asd995.cn

[H02] finally / ensure 收尾
来源：http://ow.hnjuh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ic.gzmigu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ws.shxzukj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cx.huixiangedu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ub.chemitech.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sr.muxihuayi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zd.szxytkj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hc.huanxung.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://as.newstarts.cn

[H03] 主动抛出异常
来源：http://it.bjjhwx.cn

Py:   raise ValueError("错误信息")
来源：http://oq.bookmarksfly.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://je.colortex.cn

JS:   throw new Error("错误信息");
来源：http://kg.yuntaijiaju.cn

TS:   throw new Error("错误信息");
来源：http://rd.szxytkj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yd.asd995.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qo.nicolike.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lf.shxzukj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bs.jctech888.com.cn

[H04] 自定义异常类型
来源：http://hi.lnxyls.cn

Py:   class MyError(Exception): pass
来源：http://xw.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ig.9csxet.cn

JS:   class MyError extends Error {}
来源：http://eq.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://uf.9csxet.cn

Java: class MyException extends RuntimeException {}
来源：http://kg.521024.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hi.nszjky.cn

Ruby: class MyError < StandardError; end
来源：http://co.jianghongdianzi.cn

C#:   class MyException : Exception {}
来源：http://tm.gzmigu.cn

[H05] 捕获特定类型
来源：http://nc.hnjuh.cn

Py:   except ValueError as e:
来源：http://ja.hnjuh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zk.newstarts.cn

JS:   if (e instanceof TypeError) {}
来源：http://rj.shtwfgs.cn

TS:   if (e instanceof TypeError) {}
来源：http://xc.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://gh.nicolike.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nd.521024.cn

Ruby: rescue ArgumentError => e
来源：http://kn.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dk.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://bh.huixinmuqiang.cn

Py:   value = d.get("k") or default
来源：http://qc.shxzskj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lm.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nb.huanxung.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wz.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ub.muxihuayi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fo.nszjky.cn

Ruby: d&.dig(:a, :b)
来源：http://uu.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://ec.szsharing.cn

[H07] 断言
来源：http://rz.yuntaijiaju.cn

Py:   assert x > 0, "必须为正"
来源：http://lq.hahajie.cn

PHP:  assert($x > 0);
来源：http://ci.yuexingan06.cn

JS:   console.assert(x > 0);
来源：http://wm.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://ot.szxytkj.cn

Java: assert x > 0 : "必须为正";
来源：http://qu.haigaiapp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eq.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pg.colortex.cn

C#:   Debug.Assert(x > 0);
来源：http://rg.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://wq.panjiajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://af.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pw.9csxet.cn

JS:   e.message;  e.stack
来源：http://yj.yuntaijiaju.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jd.muxihuayi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fm.shtwfgs.cn

Go:   err.Error()
来源：http://rz.gzmigu.cn

Ruby: e.message;  e.backtrace
来源：http://qf.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://yv.szsharing.cn

[H09] 带错误码的异常
来源：http://jr.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vx.hnjuh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nw.panjiajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zm.nicolike.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wx.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pm.panjiajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gb.bookmarksfly.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gi.haigaiapp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dx.jctech888.com.cn

[H10] 资源自动释放
来源：http://nk.huixiangedu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://iy.9csxet.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://af.jianghongdianzi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pe.shxzskj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jb.bjjhwx.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ci.shxzukj.cn

Go:   defer f.Close()
来源：http://mh.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ji.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uf.huixinmuqiang.cn

================================================================================
来源：http://gb.yuexingan06.cn

I. 正则表达式
来源：http://ro.haigaiapp.cn

================================================================================
来源：http://mm.shtwfgs.cn

[I01] 判断是否匹配
来源：http://wi.huixinmuqiang.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xw.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ho.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://lu.shtwfgs.cn

TS:   /\d+/.test(s)
来源：http://rn.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lt.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kc.bookmarksfly.cn

Ruby: s.match?(/\d+/)
来源：http://xr.9csxet.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vp.szsharing.cn

[I02] 提取所有匹配
来源：http://kp.lnxyls.cn

Py:   re.findall(r"\d+", s)
来源：http://zf.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://tp.jctech888.com.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ac.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://yl.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://af.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vu.wgjwhj.cn

Ruby: s.scan(/\d+/)
来源：http://qd.asd995.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lk.521024.cn

[I03] 提取捕获分组
来源：http://jp.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fp.gzmigu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ss.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zb.shxzukj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://am.hahajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rq.newstarts.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zw.asd995.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pp.chemitech.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zb.muxihuayi.cn

[I04] 正则替换
来源：http://ls.nicolike.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://km.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gl.panjiajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ux.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fo.521024.cn

Java: s.replaceAll("\\d+", "#")
来源：http://is.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hp.panjiajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yn.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wt.nicolike.cn

[I05] 按正则拆分
来源：http://yd.hahajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://io.nszjky.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yl.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://vo.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://ym.szsharing.cn


<!-- 参考信息 -->