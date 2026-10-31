代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://cg.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://af.hnjuh.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://as.panjiajie.cn

Go:   os.Remove("a.txt")
来源：http://bk.521024.cn

Ruby: File.delete("a.txt")
来源：http://kj.yuexingan06.cn

C#:   File.Delete("a.txt");
来源：http://co.haigaiapp.cn

[F07] 创建目录（含多级）
来源：http://tl.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ws.shtwfgs.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gg.hnjuh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dg.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ht.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xf.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ht.gzmigu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zb.yuexingan06.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yu.nicolike.cn

[F08] 遍历目录
来源：http://rj.jctech888.com.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ag.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://rc.nszjky.cn

JS:   fs.readdirSync("dir")
来源：http://tn.nicolike.cn

TS:   fs.readdirSync("dir")
来源：http://cu.shxzskj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fj.jctech888.com.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vh.colortex.cn

Ruby: Dir.children("dir")
来源：http://jv.shxzukj.cn

C#:   Directory.GetFiles("dir")
来源：http://yq.huanxung.cn

[F09] 获取文件大小
来源：http://qv.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://yq.huixinmuqiang.cn

PHP:  filesize("a.txt");
来源：http://sh.huixinmuqiang.cn

JS:   fs.statSync("a.txt").size
来源：http://qd.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://cm.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://cp.colortex.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://qd.nszjky.cn

Ruby: File.size("a.txt")
来源：http://qk.shxzukj.cn

C#:   new FileInfo("a.txt").Length
来源：http://hg.hnjuh.cn

[F10] 取文件扩展名 / 文件名
来源：http://zn.jctech888.com.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rc.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ib.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://oc.jianghongdianzi.cn

TS:   path.extname("a.txt")
来源：http://fu.colortex.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nb.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lk.gzmigu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fq.nszjky.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fk.huixinmuqiang.cn

[F11] 复制与移动文件
来源：http://pm.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cw.gzmigu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ik.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hy.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jk.szxytkj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uh.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kb.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ia.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ky.colortex.cn

[F12] CSV 读写
来源：http://fk.shxzukj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://rt.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://rb.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pc.gzmigu.cn

TS:   // 同上
来源：http://yl.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rq.haigaiapp.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ri.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mb.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jv.hahajie.cn

================================================================================
来源：http://bc.gzmigu.cn

G. 面向对象
来源：http://rn.hnjuh.cn

================================================================================
来源：http://re.gzmigu.cn

[G01] 定义类
来源：http://nh.shxzukj.cn

Py:   class User: pass
来源：http://kg.yuexingan06.cn

PHP:  class User {}
来源：http://ap.jctech888.com.cn

JS:   class User {}
来源：http://mm.colortex.cn

TS:   class User { name: string = ""; }
来源：http://gw.nszjky.cn

Java: class User {}
来源：http://dq.szsharing.cn

Go:   type User struct { Name string }
来源：http://so.huixiangedu.cn

Ruby: class User; end
来源：http://rn.nicolike.cn

C#:   class User {}
来源：http://bj.colortex.cn

[G02] 构造函数
来源：http://vs.huixinmuqiang.cn

Py:   def __init__(self, name): self.name = name
来源：http://wf.yuexingan06.cn

PHP:  public function __construct(public string $name) {}
来源：http://vh.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://ef.yuexingan06.cn

TS:   constructor(public name: string) {}
来源：http://hd.colortex.cn

Java: User(String name) { this.name = name; }
来源：http://vv.newstarts.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nt.bjjhwx.cn

Ruby: def initialize(name); @name = name; end
来源：http://ui.muxihuayi.cn

C#:   public User(string name) { Name = name; }
来源：http://gg.huanxung.cn

[G03] 实例属性
来源：http://et.szsharing.cn

Py:   self.name = "x"
来源：http://jm.yuexingan06.cn

PHP:  public string $name = "x";
来源：http://kl.szsharing.cn

JS:   this.name = "x";
来源：http://lu.lnxyls.cn

TS:   name: string = "x";
来源：http://ii.huanxung.cn

Java: private String name;
来源：http://op.huixiangedu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://we.nicolike.cn

Ruby: @name = "x"
来源：http://if.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://bs.nicolike.cn

[G04] 定义方法
来源：http://za.bookmarksfly.cn

Py:   def greet(self): return self.name
来源：http://fr.panjiajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mv.jctech888.com.cn

JS:   greet() { return this.name; }
来源：http://np.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://ih.521024.cn

Java: String greet() { return name; }
来源：http://gl.lnxyls.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wx.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://mh.colortex.cn

C#:   public string Greet() => Name;
来源：http://jo.bookmarksfly.cn

[G05] 继承
来源：http://va.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://bg.szxytkj.cn

PHP:  class Admin extends User {}
来源：http://fs.nszjky.cn

JS:   class Admin extends User {}
来源：http://xr.521024.cn

TS:   class Admin extends User {}
来源：http://ja.haigaiapp.cn

Java: class Admin extends User {}
来源：http://xh.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hr.9csxet.cn

Ruby: class Admin < User; end
来源：http://jh.colortex.cn

C#:   class Admin : User {}
来源：http://mb.shxzukj.cn

[G06] 重写方法
来源：http://tn.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://te.yuexingan06.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fl.hnjuh.cn

JS:   greet() { return "admin"; }
来源：http://qn.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://kn.szxytkj.cn

Java: @Override String greet() { return "admin"; }
来源：http://rs.yuexingan06.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dr.huixinmuqiang.cn

Ruby: def greet; "admin"; end
来源：http://zd.yuntaijiaju.cn

C#:   public override string Greet() => "admin";
来源：http://bw.newstarts.cn

[G07] 调用父类方法
来源：http://cp.chemitech.net.cn

Py:   super().greet()
来源：http://ny.shxzskj.cn

PHP:  parent::greet();
来源：http://jq.asd995.cn

JS:   super.greet();
来源：http://se.yuexingan06.cn

TS:   super.greet();
来源：http://hl.9csxet.cn

Java: super.greet();
来源：http://ki.chemitech.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sy.yuexingan06.cn

Ruby: super
来源：http://xw.szsharing.cn

C#:   base.Greet();
来源：http://qj.jianghongdianzi.cn

[G08] 静态方法与属性
来源：http://lz.panjiajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gd.9csxet.cn

PHP:  public static function f() {}
来源：http://oc.shxzskj.cn

JS:   static f() {}
来源：http://jw.chemitech.net.cn

TS:   static f(): void {}
来源：http://rf.hnjuh.cn

Java: static void f() {}
来源：http://oz.asd995.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pf.yuntaijiaju.cn

Ruby: def self.f; end
来源：http://kz.9csxet.cn

C#:   public static void F() {}
来源：http://cq.muxihuayi.cn

[G09] 接口 / 抽象类
来源：http://jp.bookmarksfly.cn

Py:   from abc import ABC, abstractmethod
来源：http://hp.wgjwhj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mw.hahajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://in.nszjky.cn

TS:   interface Shape { area(): number; }
来源：http://zm.szsharing.cn

Java: interface Shape { double area(); }
来源：http://to.panjiajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://jz.521024.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zs.szsharing.cn

C#:   interface IShape { double Area(); }
来源：http://bf.nszjky.cn

[G10] 访问控制
来源：http://lv.colortex.cn

Py:   约定 _protected / __private（不强制）
来源：http://qo.jctech888.com.cn

PHP:  public / protected / private
来源：http://gt.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://ut.wgjwhj.cn

TS:   public / protected / private
来源：http://yu.chemitech.net.cn

Java: public / protected / private / 默认包级
来源：http://cc.hnjuh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://pj.hnjuh.cn

Ruby: public / protected / private
来源：http://dy.szxytkj.cn

C#:   public / protected / private / internal
来源：http://ma.bjjhwx.cn

[G11] getter / setter
来源：http://po.wgjwhj.cn

Py:   @property 与 @x.setter
来源：http://du.chemitech.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rw.shtwfgs.cn

JS:   get name() { return this._name; }
来源：http://bp.shxzukj.cn

TS:   get name(): string { return this._name; }
来源：http://gq.jianghongdianzi.cn

Java: public String getName() { return name; }
来源：http://vo.nicolike.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ht.nicolike.cn

Ruby: attr_accessor :name
来源：http://sm.lnxyls.cn

C#:   public string Name { get; set; }
来源：http://gx.gzmigu.cn

[G12] 对象转字符串
来源：http://xn.bjjhwx.cn

Py:   def __str__(self): return self.name
来源：http://xu.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xc.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://jw.haigaiapp.cn

TS:   toString(): string { return this.name; }
来源：http://zv.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://ci.huixinmuqiang.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wj.shxzukj.cn

Ruby: def to_s; @name; end
来源：http://lq.lnxyls.cn

C#:   public override string ToString() => Name;
来源：http://fb.shtwfgs.cn

[G13] 判断对象类型
来源：http://hd.hnjuh.cn

Py:   isinstance(u, User)
来源：http://da.chemitech.net.cn

PHP:  $u instanceof User
来源：http://dv.521024.cn

JS:   u instanceof User
来源：http://ng.huanxung.cn

TS:   u instanceof User
来源：http://ue.szsharing.cn

Java: u instanceof User
来源：http://qr.gzmigu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ot.lnxyls.cn

Ruby: u.is_a?(User)
来源：http://ft.nicolike.cn

C#:   u is User
来源：http://ap.bookmarksfly.cn

[G14] 数据类 / record
来源：http://vi.yuntaijiaju.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ad.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://bd.shtwfgs.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rq.szxytkj.cn

TS:   type User = { name: string; age: number };
来源：http://bx.szsharing.cn

Java: record User(String name, int age) {}
来源：http://lx.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://ik.huixiangedu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wn.shxzukj.cn

C#:   record User(string Name, int Age);
来源：http://um.yuntaijiaju.cn

[G15] 枚举
来源：http://sv.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://av.yuntaijiaju.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ct.shxzukj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ka.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zy.huixinmuqiang.cn

Java: enum Color { RED, GREEN }
来源：http://fh.colortex.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fc.gzmigu.cn

Ruby: Color = %i[red green].freeze
来源：http://or.yuexingan06.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yz.colortex.cn

[G16] 对象转数组 / 字典
来源：http://tb.szxytkj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ne.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://mb.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://sl.szsharing.cn

TS:   Object.entries(obj)
来源：http://kc.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fj.szxytkj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://eu.wgjwhj.cn

Ruby: obj.instance_variables
来源：http://lp.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://zc.gzmigu.cn

================================================================================
来源：http://ez.haigaiapp.cn

H. 异常与错误处理
来源：http://tm.521024.cn

================================================================================
来源：http://nj.nicolike.cn

[H01] try / catch 基础
来源：http://ie.huixiangedu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://su.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xw.shtwfgs.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qi.szsharing.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bw.newstarts.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vo.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xm.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ej.521024.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dn.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://nd.panjiajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vx.newstarts.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vv.jctech888.com.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lf.hahajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gd.asd995.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gw.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://oq.haigaiapp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bq.colortex.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ie.gzmigu.cn

[H03] 主动抛出异常
来源：http://vm.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://kv.panjiajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pt.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://ev.asd995.cn

TS:   throw new Error("错误信息");
来源：http://um.szxytkj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://cq.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fj.nszjky.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yi.colortex.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pv.bookmarksfly.cn

[H04] 自定义异常类型
来源：http://ao.szsharing.cn

Py:   class MyError(Exception): pass
来源：http://cd.colortex.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zv.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://au.shtwfgs.cn

TS:   class MyError extends Error {}
来源：http://yy.huanxung.cn

Java: class MyException extends RuntimeException {}
来源：http://yy.muxihuayi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zh.huanxung.cn

Ruby: class MyError < StandardError; end
来源：http://hi.hnjuh.cn

C#:   class MyException : Exception {}
来源：http://va.nicolike.cn

[H05] 捕获特定类型
来源：http://gr.huanxung.cn

Py:   except ValueError as e:
来源：http://qr.chemitech.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gk.shtwfgs.cn

JS:   if (e instanceof TypeError) {}
来源：http://lb.newstarts.cn

TS:   if (e instanceof TypeError) {}
来源：http://aw.nszjky.cn

Java: catch (IOException | SQLException e) {}
来源：http://or.asd995.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ve.chemitech.net.cn

Ruby: rescue ArgumentError => e
来源：http://ae.9csxet.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jw.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://kh.panjiajie.cn

Py:   value = d.get("k") or default
来源：http://mu.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xj.panjiajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cr.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bc.huixinmuqiang.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sc.huanxung.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pk.lnxyls.cn

Ruby: d&.dig(:a, :b)
来源：http://gl.nicolike.cn

C#:   obj?.A?.B ?? default
来源：http://dm.haigaiapp.cn

[H07] 断言
来源：http://bn.szsharing.cn

Py:   assert x > 0, "必须为正"
来源：http://qe.huanxung.cn

PHP:  assert($x > 0);
来源：http://zh.521024.cn

JS:   console.assert(x > 0);
来源：http://yf.521024.cn

TS:   console.assert(x > 0);
来源：http://pj.jctech888.com.cn

Java: assert x > 0 : "必须为正";
来源：http://hq.wgjwhj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://di.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gu.hnjuh.cn

C#:   Debug.Assert(x > 0);
来源：http://ya.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://xl.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://nc.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sa.huixinmuqiang.cn

JS:   e.message;  e.stack
来源：http://im.jctech888.com.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qo.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xq.szsharing.cn

Go:   err.Error()
来源：http://wm.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://pq.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://ri.szsharing.cn

[H09] 带错误码的异常
来源：http://oz.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dn.nicolike.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gg.huixiangedu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wy.szxytkj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dy.colortex.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vo.szxytkj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xs.lnxyls.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ic.nicolike.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rk.huixiangedu.cn

[H10] 资源自动释放
来源：http://um.huixiangedu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://tw.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xn.wgjwhj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ac.szxytkj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gt.nicolike.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rb.wgjwhj.cn

Go:   defer f.Close()
来源：http://uy.jctech888.com.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ut.huixiangedu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ox.bookmarksfly.cn


<!-- 参考信息 -->