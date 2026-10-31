代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ah.shxzskj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hk.huixiangedu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ys.jianghongdianzi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://jx.hahajie.cn

================================================================================
来源：http://be.nszjky.cn

G. 面向对象
来源：http://aj.jianghongdianzi.cn

================================================================================
来源：http://qp.jctech888.com.cn

[G01] 定义类
来源：http://mw.lnxyls.cn

Py:   class User: pass
来源：http://py.newstarts.cn

PHP:  class User {}
来源：http://mj.nicolike.cn

JS:   class User {}
来源：http://hd.bjjhwx.cn

TS:   class User { name: string = ""; }
来源：http://kd.bjjhwx.cn

Java: class User {}
来源：http://qj.szsharing.cn

Go:   type User struct { Name string }
来源：http://tf.panjiajie.cn

Ruby: class User; end
来源：http://ng.lnxyls.cn

C#:   class User {}
来源：http://jf.shtwfgs.cn

[G02] 构造函数
来源：http://wi.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://ub.jctech888.com.cn

PHP:  public function __construct(public string $name) {}
来源：http://gv.9csxet.cn

JS:   constructor(name) { this.name = name; }
来源：http://gk.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://kl.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://wu.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lr.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://xk.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://tn.szsharing.cn

[G03] 实例属性
来源：http://df.nicolike.cn

Py:   self.name = "x"
来源：http://nh.colortex.cn

PHP:  public string $name = "x";
来源：http://uy.newstarts.cn

JS:   this.name = "x";
来源：http://ls.yuexingan06.cn

TS:   name: string = "x";
来源：http://bn.shxzskj.cn

Java: private String name;
来源：http://ae.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lb.521024.cn

Ruby: @name = "x"
来源：http://wd.bookmarksfly.cn

C#:   public string Name { get; set; } = "x";
来源：http://wy.lnxyls.cn

[G04] 定义方法
来源：http://eo.panjiajie.cn

Py:   def greet(self): return self.name
来源：http://ez.huixinmuqiang.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ao.huanxung.cn

JS:   greet() { return this.name; }
来源：http://et.521024.cn

TS:   greet(): string { return this.name; }
来源：http://qa.9csxet.cn

Java: String greet() { return name; }
来源：http://jo.lnxyls.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qb.nicolike.cn

Ruby: def greet; @name; end
来源：http://tz.panjiajie.cn

C#:   public string Greet() => Name;
来源：http://kx.bjjhwx.cn

[G05] 继承
来源：http://wx.huanxung.cn

Py:   class Admin(User): pass
来源：http://ge.nicolike.cn

PHP:  class Admin extends User {}
来源：http://bv.newstarts.cn

JS:   class Admin extends User {}
来源：http://dx.shxzukj.cn

TS:   class Admin extends User {}
来源：http://rl.shtwfgs.cn

Java: class Admin extends User {}
来源：http://wo.yuexingan06.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dc.hnjuh.cn

Ruby: class Admin < User; end
来源：http://jz.jctech888.com.cn

C#:   class Admin : User {}
来源：http://jz.huixinmuqiang.cn

[G06] 重写方法
来源：http://lg.wgjwhj.cn

Py:   def greet(self): return "admin"
来源：http://xg.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zj.huixinmuqiang.cn

JS:   greet() { return "admin"; }
来源：http://ha.muxihuayi.cn

TS:   greet(): string { return "admin"; }
来源：http://hl.nszjky.cn

Java: @Override String greet() { return "admin"; }
来源：http://wc.jctech888.com.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://aw.huixinmuqiang.cn

Ruby: def greet; "admin"; end
来源：http://xz.asd995.cn

C#:   public override string Greet() => "admin";
来源：http://kt.jctech888.com.cn

[G07] 调用父类方法
来源：http://cn.colortex.cn

Py:   super().greet()
来源：http://wq.jctech888.com.cn

PHP:  parent::greet();
来源：http://da.jctech888.com.cn

JS:   super.greet();
来源：http://ao.asd995.cn

TS:   super.greet();
来源：http://ov.shxzskj.cn

Java: super.greet();
来源：http://yw.jctech888.com.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ak.huanxung.cn

Ruby: super
来源：http://hv.hnjuh.cn

C#:   base.Greet();
来源：http://lo.bookmarksfly.cn

[G08] 静态方法与属性
来源：http://tb.gzmigu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zr.hahajie.cn

PHP:  public static function f() {}
来源：http://bs.shxzskj.cn

JS:   static f() {}
来源：http://ec.shxzukj.cn

TS:   static f(): void {}
来源：http://eb.bjjhwx.cn

Java: static void f() {}
来源：http://yv.wgjwhj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kb.9csxet.cn

Ruby: def self.f; end
来源：http://ep.bookmarksfly.cn

C#:   public static void F() {}
来源：http://sa.bjjhwx.cn

[G09] 接口 / 抽象类
来源：http://cg.muxihuayi.cn

Py:   from abc import ABC, abstractmethod
来源：http://gy.panjiajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kv.huixinmuqiang.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pk.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://ro.hnjuh.cn

Java: interface Shape { double area(); }
来源：http://uu.gzmigu.cn

Go:   type Shape interface { Area() float64 }
来源：http://wf.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bs.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://vv.huanxung.cn

[G10] 访问控制
来源：http://jd.huanxung.cn

Py:   约定 _protected / __private（不强制）
来源：http://mb.szsharing.cn

PHP:  public / protected / private
来源：http://jc.yuexingan06.cn

JS:   #private 字段；其余公开
来源：http://dq.jianghongdianzi.cn

TS:   public / protected / private
来源：http://aw.colortex.cn

Java: public / protected / private / 默认包级
来源：http://jt.huanxung.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cb.hahajie.cn

Ruby: public / protected / private
来源：http://ah.shxzskj.cn

C#:   public / protected / private / internal
来源：http://ml.shxzskj.cn

[G11] getter / setter
来源：http://od.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://tj.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://uz.colortex.cn

JS:   get name() { return this._name; }
来源：http://ww.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://nf.9csxet.cn

Java: public String getName() { return name; }
来源：http://zk.panjiajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yv.lnxyls.cn

Ruby: attr_accessor :name
来源：http://ip.hnjuh.cn

C#:   public string Name { get; set; }
来源：http://uf.bjjhwx.cn

[G12] 对象转字符串
来源：http://vk.haigaiapp.cn

Py:   def __str__(self): return self.name
来源：http://yn.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xv.chemitech.net.cn

JS:   toString() { return this.name; }
来源：http://ni.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://zt.bookmarksfly.cn

Java: @Override public String toString() { return name; }
来源：http://pr.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nq.yuexingan06.cn

Ruby: def to_s; @name; end
来源：http://eo.newstarts.cn

C#:   public override string ToString() => Name;
来源：http://dl.panjiajie.cn

[G13] 判断对象类型
来源：http://wg.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://xw.bjjhwx.cn

PHP:  $u instanceof User
来源：http://ex.jianghongdianzi.cn

JS:   u instanceof User
来源：http://sk.shtwfgs.cn

TS:   u instanceof User
来源：http://na.hnjuh.cn

Java: u instanceof User
来源：http://zy.hnjuh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xo.hnjuh.cn

Ruby: u.is_a?(User)
来源：http://gq.jctech888.com.cn

C#:   u is User
来源：http://nr.521024.cn

[G14] 数据类 / record
来源：http://st.huixinmuqiang.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dd.huixiangedu.cn

PHP:  // 用 readonly 属性模拟
来源：http://ak.szxytkj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cw.huixinmuqiang.cn

TS:   type User = { name: string; age: number };
来源：http://ld.521024.cn

Java: record User(String name, int age) {}
来源：http://jt.hahajie.cn

Go:   type User struct { Name string; Age int }
来源：http://kn.nicolike.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://py.nicolike.cn

C#:   record User(string Name, int Age);
来源：http://kv.shxzskj.cn

[G15] 枚举
来源：http://qk.shxzskj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://at.asd995.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://af.nszjky.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jo.szxytkj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nv.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://qb.jianghongdianzi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vd.muxihuayi.cn

Ruby: Color = %i[red green].freeze
来源：http://or.bookmarksfly.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cr.nszjky.cn

[G16] 对象转数组 / 字典
来源：http://mo.szxytkj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xd.shxzskj.cn

PHP:  get_object_vars($obj);
来源：http://cr.szxytkj.cn

JS:   Object.entries(obj)
来源：http://rl.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://bf.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jx.hnjuh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jg.chemitech.net.cn

Ruby: obj.instance_variables
来源：http://ft.gzmigu.cn

C#:   // 用反射或 System.Text.Json
来源：http://lv.huixiangedu.cn

================================================================================
来源：http://qq.lnxyls.cn

H. 异常与错误处理
来源：http://qt.newstarts.cn

================================================================================
来源：http://bn.muxihuayi.cn

[H01] try / catch 基础
来源：http://dt.huixinmuqiang.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://md.lnxyls.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tx.shxzskj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oc.lnxyls.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://we.shtwfgs.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lz.9csxet.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ir.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kt.wgjwhj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hj.newstarts.cn

[H02] finally / ensure 收尾
来源：http://bl.shxzukj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://md.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pn.9csxet.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nw.newstarts.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://md.shxzskj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://by.yuntaijiaju.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ef.panjiajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hm.muxihuayi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://kx.nicolike.cn

[H03] 主动抛出异常
来源：http://kb.huixiangedu.cn

Py:   raise ValueError("错误信息")
来源：http://re.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://et.bookmarksfly.cn

JS:   throw new Error("错误信息");
来源：http://pn.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://pq.shxzukj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zj.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rs.gzmigu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ca.bjjhwx.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tv.nszjky.cn

[H04] 自定义异常类型
来源：http://ib.jianghongdianzi.cn

Py:   class MyError(Exception): pass
来源：http://tk.chemitech.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ts.colortex.cn

JS:   class MyError extends Error {}
来源：http://wy.nszjky.cn

TS:   class MyError extends Error {}
来源：http://li.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://rv.bjjhwx.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sw.panjiajie.cn

Ruby: class MyError < StandardError; end
来源：http://bc.shtwfgs.cn

C#:   class MyException : Exception {}
来源：http://ae.yuexingan06.cn

[H05] 捕获特定类型
来源：http://nr.jctech888.com.cn

Py:   except ValueError as e:
来源：http://wz.huixiangedu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zm.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://ku.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://wu.lnxyls.cn

Java: catch (IOException | SQLException e) {}
来源：http://st.szxytkj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xy.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://pz.jianghongdianzi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sp.nicolike.cn

[H06] 可选值 / 空值安全访问
来源：http://jm.9csxet.cn

Py:   value = d.get("k") or default
来源：http://zt.bjjhwx.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mu.szxytkj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://la.shtwfgs.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yj.newstarts.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gz.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ls.9csxet.cn

Ruby: d&.dig(:a, :b)
来源：http://fa.huixiangedu.cn

C#:   obj?.A?.B ?? default
来源：http://xh.hnjuh.cn

[H07] 断言
来源：http://cl.bjjhwx.cn

Py:   assert x > 0, "必须为正"
来源：http://kf.shtwfgs.cn

PHP:  assert($x > 0);
来源：http://eb.gzmigu.cn

JS:   console.assert(x > 0);
来源：http://hy.muxihuayi.cn

TS:   console.assert(x > 0);
来源：http://od.nszjky.cn

Java: assert x > 0 : "必须为正";
来源：http://vm.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lf.hnjuh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jc.colortex.cn

C#:   Debug.Assert(x > 0);
来源：http://be.gzmigu.cn

[H08] 获取错误信息与堆栈
来源：http://kq.shtwfgs.cn

Py:   str(e);  traceback.format_exc()
来源：http://ue.yuntaijiaju.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uq.huanxung.cn

JS:   e.message;  e.stack
来源：http://sy.szxytkj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mh.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://va.wgjwhj.cn

Go:   err.Error()
来源：http://ap.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://zu.nszjky.cn

C#:   e.Message;  e.StackTrace
来源：http://my.9csxet.cn

[H09] 带错误码的异常
来源：http://ju.chemitech.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mq.hahajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mu.lnxyls.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ti.hnjuh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sg.nicolike.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://di.gzmigu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sq.shxzskj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://eb.wgjwhj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://st.wgjwhj.cn

[H10] 资源自动释放
来源：http://hv.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qu.bookmarksfly.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zf.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ob.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lh.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nx.hahajie.cn

Go:   defer f.Close()
来源：http://rx.521024.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ei.szxytkj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pc.muxihuayi.cn

================================================================================
来源：http://ro.hnjuh.cn

I. 正则表达式
来源：http://kz.hnjuh.cn

================================================================================
来源：http://ui.jctech888.com.cn

[I01] 判断是否匹配
来源：http://gb.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tr.jianghongdianzi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vi.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://sq.huixiangedu.cn

TS:   /\d+/.test(s)
来源：http://oa.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bi.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jy.gzmigu.cn

Ruby: s.match?(/\d+/)
来源：http://we.huixiangedu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qj.haigaiapp.cn

[I02] 提取所有匹配
来源：http://wj.asd995.cn

Py:   re.findall(r"\d+", s)
来源：http://ox.chemitech.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ym.huixiangedu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yc.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://af.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oq.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ed.9csxet.cn

Ruby: s.scan(/\d+/)
来源：http://at.szsharing.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vu.huanxung.cn

[I03] 提取捕获分组
来源：http://qv.wgjwhj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cd.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jg.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fo.nszjky.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gm.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gn.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hr.hnjuh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pc.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ra.asd995.cn

[I04] 正则替换
来源：http://px.nicolike.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://et.shxzskj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://et.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ns.bookmarksfly.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mw.colortex.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wb.bjjhwx.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kk.haigaiapp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ob.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ys.szsharing.cn

[I05] 按正则拆分
来源：http://sq.szxytkj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sq.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yu.huixinmuqiang.cn

JS:   s.split(/\s*,\s*/)
来源：http://bl.yuexingan06.cn

TS:   s.split(/\s*,\s*/)
来源：http://bg.gzmigu.cn

Java: s.split("\\s*,\\s*")
来源：http://ad.huixiangedu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ly.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hn.nicolike.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zx.nszjky.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xu.gzmigu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vf.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vf.huixinmuqiang.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lg.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ie.huixiangedu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qu.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pz.wgjwhj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nc.asd995.cn


<!-- 参考信息 -->