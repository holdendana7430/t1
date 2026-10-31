代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xt.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gj.shtwfgs.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xu.bookmarksfly.cn

[F12] CSV 读写
来源：http://jz.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://dk.shtwfgs.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lv.bjjhwx.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://rr.szsharing.cn

TS:   // 同上
来源：http://ef.shxzukj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ig.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cn.bookmarksfly.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wj.szxytkj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fw.newstarts.cn

================================================================================
来源：http://sg.shtwfgs.cn

G. 面向对象
来源：http://kv.yuntaijiaju.cn

================================================================================
来源：http://gx.haigaiapp.cn

[G01] 定义类
来源：http://og.nszjky.cn

Py:   class User: pass
来源：http://sy.chemitech.net.cn

PHP:  class User {}
来源：http://az.gzmigu.cn

JS:   class User {}
来源：http://dt.newstarts.cn

TS:   class User { name: string = ""; }
来源：http://ih.szsharing.cn

Java: class User {}
来源：http://vv.lnxyls.cn

Go:   type User struct { Name string }
来源：http://mk.lnxyls.cn

Ruby: class User; end
来源：http://cn.yuexingan06.cn

C#:   class User {}
来源：http://di.jianghongdianzi.cn

[G02] 构造函数
来源：http://mp.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://qq.szsharing.cn

PHP:  public function __construct(public string $name) {}
来源：http://rm.nicolike.cn

JS:   constructor(name) { this.name = name; }
来源：http://hc.panjiajie.cn

TS:   constructor(public name: string) {}
来源：http://tj.shtwfgs.cn

Java: User(String name) { this.name = name; }
来源：http://di.shtwfgs.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tu.huanxung.cn

Ruby: def initialize(name); @name = name; end
来源：http://oq.hahajie.cn

C#:   public User(string name) { Name = name; }
来源：http://oi.hnjuh.cn

[G03] 实例属性
来源：http://sz.bjjhwx.cn

Py:   self.name = "x"
来源：http://na.colortex.cn

PHP:  public string $name = "x";
来源：http://mw.asd995.cn

JS:   this.name = "x";
来源：http://pu.chemitech.net.cn

TS:   name: string = "x";
来源：http://je.huixinmuqiang.cn

Java: private String name;
来源：http://mc.asd995.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ew.wgjwhj.cn

Ruby: @name = "x"
来源：http://ot.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://xt.9csxet.cn

[G04] 定义方法
来源：http://hm.nicolike.cn

Py:   def greet(self): return self.name
来源：http://au.jctech888.com.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tw.szsharing.cn

JS:   greet() { return this.name; }
来源：http://jm.yuntaijiaju.cn

TS:   greet(): string { return this.name; }
来源：http://hy.huanxung.cn

Java: String greet() { return name; }
来源：http://qt.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://dq.colortex.cn

Ruby: def greet; @name; end
来源：http://dk.yuexingan06.cn

C#:   public string Greet() => Name;
来源：http://bm.muxihuayi.cn

[G05] 继承
来源：http://ux.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://zq.colortex.cn

PHP:  class Admin extends User {}
来源：http://ec.shxzukj.cn

JS:   class Admin extends User {}
来源：http://oa.hnjuh.cn

TS:   class Admin extends User {}
来源：http://fw.chemitech.net.cn

Java: class Admin extends User {}
来源：http://xa.huixiangedu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rc.hnjuh.cn

Ruby: class Admin < User; end
来源：http://ik.bjjhwx.cn

C#:   class Admin : User {}
来源：http://qc.asd995.cn

[G06] 重写方法
来源：http://vk.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://mq.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pf.wgjwhj.cn

JS:   greet() { return "admin"; }
来源：http://gl.nicolike.cn

TS:   greet(): string { return "admin"; }
来源：http://lt.gzmigu.cn

Java: @Override String greet() { return "admin"; }
来源：http://yq.haigaiapp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uj.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://vz.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://ar.panjiajie.cn

[G07] 调用父类方法
来源：http://zq.lnxyls.cn

Py:   super().greet()
来源：http://jp.jianghongdianzi.cn

PHP:  parent::greet();
来源：http://pc.hahajie.cn

JS:   super.greet();
来源：http://va.huixinmuqiang.cn

TS:   super.greet();
来源：http://od.gzmigu.cn

Java: super.greet();
来源：http://vc.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ra.panjiajie.cn

Ruby: super
来源：http://xd.huixiangedu.cn

C#:   base.Greet();
来源：http://kw.hahajie.cn

[G08] 静态方法与属性
来源：http://ny.lnxyls.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://sk.shxzukj.cn

PHP:  public static function f() {}
来源：http://wn.9csxet.cn

JS:   static f() {}
来源：http://vi.jctech888.com.cn

TS:   static f(): void {}
来源：http://wg.hnjuh.cn

Java: static void f() {}
来源：http://gp.haigaiapp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://uh.521024.cn

Ruby: def self.f; end
来源：http://rb.yuexingan06.cn

C#:   public static void F() {}
来源：http://iz.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://bo.szsharing.cn

Py:   from abc import ABC, abstractmethod
来源：http://zg.lnxyls.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pq.bookmarksfly.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sl.huixiangedu.cn

TS:   interface Shape { area(): number; }
来源：http://pg.shxzskj.cn

Java: interface Shape { double area(); }
来源：http://we.nicolike.cn

Go:   type Shape interface { Area() float64 }
来源：http://kd.newstarts.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vc.shxzukj.cn

C#:   interface IShape { double Area(); }
来源：http://rx.shxzukj.cn

[G10] 访问控制
来源：http://xg.szxytkj.cn

Py:   约定 _protected / __private（不强制）
来源：http://hn.jctech888.com.cn

PHP:  public / protected / private
来源：http://nx.chemitech.net.cn

JS:   #private 字段；其余公开
来源：http://tf.asd995.cn

TS:   public / protected / private
来源：http://ad.colortex.cn

Java: public / protected / private / 默认包级
来源：http://hv.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mi.newstarts.cn

Ruby: public / protected / private
来源：http://ak.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://vy.haigaiapp.cn

[G11] getter / setter
来源：http://ff.521024.cn

Py:   @property 与 @x.setter
来源：http://sl.panjiajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ov.huixinmuqiang.cn

JS:   get name() { return this._name; }
来源：http://xz.nicolike.cn

TS:   get name(): string { return this._name; }
来源：http://vu.muxihuayi.cn

Java: public String getName() { return name; }
来源：http://aw.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://as.huanxung.cn

Ruby: attr_accessor :name
来源：http://yl.chemitech.net.cn

C#:   public string Name { get; set; }
来源：http://qx.shtwfgs.cn

[G12] 对象转字符串
来源：http://hn.haigaiapp.cn

Py:   def __str__(self): return self.name
来源：http://cb.9csxet.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tc.yuexingan06.cn

JS:   toString() { return this.name; }
来源：http://on.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://ds.hahajie.cn

Java: @Override public String toString() { return name; }
来源：http://vh.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tb.bookmarksfly.cn

Ruby: def to_s; @name; end
来源：http://pv.colortex.cn

C#:   public override string ToString() => Name;
来源：http://bi.hnjuh.cn

[G13] 判断对象类型
来源：http://xz.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://iu.colortex.cn

PHP:  $u instanceof User
来源：http://uh.shxzskj.cn

JS:   u instanceof User
来源：http://wc.nszjky.cn

TS:   u instanceof User
来源：http://zl.gzmigu.cn

Java: u instanceof User
来源：http://hs.szxytkj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://yd.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://ae.haigaiapp.cn

C#:   u is User
来源：http://ra.muxihuayi.cn

[G14] 数据类 / record
来源：http://on.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bi.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://li.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mh.shxzskj.cn

TS:   type User = { name: string; age: number };
来源：http://ru.huixiangedu.cn

Java: record User(String name, int age) {}
来源：http://ch.hahajie.cn

Go:   type User struct { Name string; Age int }
来源：http://qd.shxzukj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cg.jctech888.com.cn

C#:   record User(string Name, int Age);
来源：http://sx.muxihuayi.cn

[G15] 枚举
来源：http://jw.szxytkj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vk.lnxyls.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yq.huanxung.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ex.haigaiapp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gq.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://sh.szxytkj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://do.colortex.cn

Ruby: Color = %i[red green].freeze
来源：http://xc.szxytkj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fe.shtwfgs.cn

[G16] 对象转数组 / 字典
来源：http://yk.9csxet.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qq.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://tu.9csxet.cn

JS:   Object.entries(obj)
来源：http://ie.lnxyls.cn

TS:   Object.entries(obj)
来源：http://ik.hahajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ge.huixiangedu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tx.hahajie.cn

Ruby: obj.instance_variables
来源：http://ao.bjjhwx.cn

C#:   // 用反射或 System.Text.Json
来源：http://uc.9csxet.cn

================================================================================
来源：http://dx.hnjuh.cn

H. 异常与错误处理
来源：http://lm.colortex.cn

================================================================================
来源：http://ko.chemitech.net.cn

[H01] try / catch 基础
来源：http://vg.shxzukj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nl.jianghongdianzi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ib.yuntaijiaju.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ck.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gt.huixinmuqiang.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ad.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://te.chemitech.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kz.haigaiapp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ls.szxytkj.cn

[H02] finally / ensure 收尾
来源：http://wm.shxzukj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bw.gzmigu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://uv.hahajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ns.chemitech.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ut.jianghongdianzi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lg.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://kw.haigaiapp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pu.gzmigu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wi.bjjhwx.cn

[H03] 主动抛出异常
来源：http://li.hahajie.cn

Py:   raise ValueError("错误信息")
来源：http://hl.nszjky.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vp.yuntaijiaju.cn

JS:   throw new Error("错误信息");
来源：http://ma.nszjky.cn

TS:   throw new Error("错误信息");
来源：http://pv.jctech888.com.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bg.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sf.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vp.lnxyls.cn

C#:   throw new ArgumentException("错误信息");
来源：http://me.szsharing.cn

[H04] 自定义异常类型
来源：http://ei.huixiangedu.cn

Py:   class MyError(Exception): pass
来源：http://ui.shtwfgs.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gs.bookmarksfly.cn

JS:   class MyError extends Error {}
来源：http://qu.panjiajie.cn

TS:   class MyError extends Error {}
来源：http://mx.asd995.cn

Java: class MyException extends RuntimeException {}
来源：http://dr.521024.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://la.lnxyls.cn

Ruby: class MyError < StandardError; end
来源：http://jp.lnxyls.cn

C#:   class MyException : Exception {}
来源：http://zj.hnjuh.cn

[H05] 捕获特定类型
来源：http://xt.panjiajie.cn

Py:   except ValueError as e:
来源：http://jp.chemitech.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://aw.shtwfgs.cn

JS:   if (e instanceof TypeError) {}
来源：http://na.yuntaijiaju.cn

TS:   if (e instanceof TypeError) {}
来源：http://jz.huixinmuqiang.cn

Java: catch (IOException | SQLException e) {}
来源：http://ia.hnjuh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jz.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://mg.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://za.muxihuayi.cn

[H06] 可选值 / 空值安全访问
来源：http://ln.bookmarksfly.cn

Py:   value = d.get("k") or default
来源：http://er.huixiangedu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kk.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hb.szsharing.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gs.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://al.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ra.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://il.bookmarksfly.cn

C#:   obj?.A?.B ?? default
来源：http://at.chemitech.net.cn

[H07] 断言
来源：http://gx.jctech888.com.cn

Py:   assert x > 0, "必须为正"
来源：http://kj.bookmarksfly.cn

PHP:  assert($x > 0);
来源：http://nx.9csxet.cn

JS:   console.assert(x > 0);
来源：http://fz.nicolike.cn

TS:   console.assert(x > 0);
来源：http://wc.lnxyls.cn

Java: assert x > 0 : "必须为正";
来源：http://gk.hahajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zu.shxzskj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://we.jianghongdianzi.cn

C#:   Debug.Assert(x > 0);
来源：http://do.bookmarksfly.cn

[H08] 获取错误信息与堆栈
来源：http://if.huixiangedu.cn

Py:   str(e);  traceback.format_exc()
来源：http://ai.9csxet.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hf.muxihuayi.cn

JS:   e.message;  e.stack
来源：http://ed.chemitech.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mr.szxytkj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://in.nicolike.cn

Go:   err.Error()
来源：http://jl.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://lh.huixinmuqiang.cn

C#:   e.Message;  e.StackTrace
来源：http://pd.shtwfgs.cn

[H09] 带错误码的异常
来源：http://sy.huixinmuqiang.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uq.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pa.szxytkj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://da.yuntaijiaju.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zu.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hp.lnxyls.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jd.9csxet.cn

Ruby: raise MyError.new("fail", 500)
来源：http://co.chemitech.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vj.nicolike.cn

[H10] 资源自动释放
来源：http://ds.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bc.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tt.lnxyls.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lv.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mm.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uj.haigaiapp.cn

Go:   defer f.Close()
来源：http://ww.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zw.szxytkj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qd.hnjuh.cn

================================================================================
来源：http://am.haigaiapp.cn

I. 正则表达式
来源：http://se.szxytkj.cn

================================================================================
来源：http://ny.colortex.cn

[I01] 判断是否匹配
来源：http://bg.wgjwhj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://za.haigaiapp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wa.yuexingan06.cn

JS:   /\d+/.test(s)
来源：http://eb.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://yp.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jc.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://la.haigaiapp.cn

Ruby: s.match?(/\d+/)
来源：http://vg.yuntaijiaju.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fn.lnxyls.cn

[I02] 提取所有匹配
来源：http://gv.yuexingan06.cn

Py:   re.findall(r"\d+", s)
来源：http://wu.521024.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vj.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qa.jctech888.com.cn

TS:   s.match(/\d+/g)
来源：http://fq.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bu.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://py.yuexingan06.cn

Ruby: s.scan(/\d+/)
来源：http://pw.yuexingan06.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gs.jianghongdianzi.cn

[I03] 提取捕获分组
来源：http://nu.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vm.szsharing.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wd.muxihuayi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pi.wgjwhj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yr.muxihuayi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cs.jctech888.com.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yg.shxzskj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pr.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bo.lnxyls.cn

[I04] 正则替换
来源：http://eb.asd995.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://pu.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wf.hnjuh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tt.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ux.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://eb.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gw.shxzukj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ga.asd995.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://by.huixiangedu.cn

[I05] 按正则拆分
来源：http://eh.haigaiapp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wy.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pn.521024.cn

JS:   s.split(/\s*,\s*/)
来源：http://af.haigaiapp.cn

TS:   s.split(/\s*,\s*/)
来源：http://ih.nicolike.cn

Java: s.split("\\s*,\\s*")
来源：http://wm.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gf.hnjuh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ev.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tj.haigaiapp.cn


<!-- 参考信息 -->