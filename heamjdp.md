代发 wailian999

Java: class User {}
来源：http://lc.shtwfgs.cn

Go:   type User struct { Name string }
来源：http://lx.gzmigu.cn

Ruby: class User; end
来源：http://sp.hahajie.cn

C#:   class User {}
来源：http://jz.jctech888.com.cn

[G02] 构造函数
来源：http://ne.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://mh.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://zg.521024.cn

JS:   constructor(name) { this.name = name; }
来源：http://uf.wgjwhj.cn

TS:   constructor(public name: string) {}
来源：http://ko.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://no.haigaiapp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zx.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://so.bookmarksfly.cn

C#:   public User(string name) { Name = name; }
来源：http://st.nicolike.cn

[G03] 实例属性
来源：http://pi.gzmigu.cn

Py:   self.name = "x"
来源：http://sd.bookmarksfly.cn

PHP:  public string $name = "x";
来源：http://mq.hahajie.cn

JS:   this.name = "x";
来源：http://ey.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://xb.huanxung.cn

Java: private String name;
来源：http://ow.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qv.nicolike.cn

Ruby: @name = "x"
来源：http://fw.huixinmuqiang.cn

C#:   public string Name { get; set; } = "x";
来源：http://zz.jctech888.com.cn

[G04] 定义方法
来源：http://ht.nszjky.cn

Py:   def greet(self): return self.name
来源：http://mf.panjiajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pk.huanxung.cn

JS:   greet() { return this.name; }
来源：http://xr.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://gk.gzmigu.cn

Java: String greet() { return name; }
来源：http://ut.panjiajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vc.yuntaijiaju.cn

Ruby: def greet; @name; end
来源：http://ig.bjjhwx.cn

C#:   public string Greet() => Name;
来源：http://ed.jianghongdianzi.cn

[G05] 继承
来源：http://vl.shxzskj.cn

Py:   class Admin(User): pass
来源：http://an.hahajie.cn

PHP:  class Admin extends User {}
来源：http://ml.9csxet.cn

JS:   class Admin extends User {}
来源：http://uo.bjjhwx.cn

TS:   class Admin extends User {}
来源：http://hh.lnxyls.cn

Java: class Admin extends User {}
来源：http://ba.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ac.asd995.cn

Ruby: class Admin < User; end
来源：http://gd.panjiajie.cn

C#:   class Admin : User {}
来源：http://hi.jctech888.com.cn

[G06] 重写方法
来源：http://qp.huixinmuqiang.cn

Py:   def greet(self): return "admin"
来源：http://tn.jctech888.com.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ep.wgjwhj.cn

JS:   greet() { return "admin"; }
来源：http://yc.shtwfgs.cn

TS:   greet(): string { return "admin"; }
来源：http://ak.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://ne.yuexingan06.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wn.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://sl.521024.cn

C#:   public override string Greet() => "admin";
来源：http://tv.nicolike.cn

[G07] 调用父类方法
来源：http://og.yuntaijiaju.cn

Py:   super().greet()
来源：http://tj.colortex.cn

PHP:  parent::greet();
来源：http://cr.szxytkj.cn

JS:   super.greet();
来源：http://dd.bjjhwx.cn

TS:   super.greet();
来源：http://wq.yuexingan06.cn

Java: super.greet();
来源：http://jk.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jf.haigaiapp.cn

Ruby: super
来源：http://eb.haigaiapp.cn

C#:   base.Greet();
来源：http://xp.lnxyls.cn

[G08] 静态方法与属性
来源：http://if.bjjhwx.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vd.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://iv.bjjhwx.cn

JS:   static f() {}
来源：http://sm.shxzskj.cn

TS:   static f(): void {}
来源：http://so.huanxung.cn

Java: static void f() {}
来源：http://ju.jctech888.com.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qf.muxihuayi.cn

Ruby: def self.f; end
来源：http://pd.9csxet.cn

C#:   public static void F() {}
来源：http://rw.shtwfgs.cn

[G09] 接口 / 抽象类
来源：http://br.lnxyls.cn

Py:   from abc import ABC, abstractmethod
来源：http://dt.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dw.haigaiapp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zm.huixiangedu.cn

TS:   interface Shape { area(): number; }
来源：http://qd.shxzukj.cn

Java: interface Shape { double area(); }
来源：http://ww.shxzukj.cn

Go:   type Shape interface { Area() float64 }
来源：http://it.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gw.muxihuayi.cn

C#:   interface IShape { double Area(); }
来源：http://nb.lnxyls.cn

[G10] 访问控制
来源：http://te.yuexingan06.cn

Py:   约定 _protected / __private（不强制）
来源：http://cx.521024.cn

PHP:  public / protected / private
来源：http://ue.colortex.cn

JS:   #private 字段；其余公开
来源：http://qe.hahajie.cn

TS:   public / protected / private
来源：http://qc.gzmigu.cn

Java: public / protected / private / 默认包级
来源：http://ea.lnxyls.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xy.9csxet.cn

Ruby: public / protected / private
来源：http://db.jianghongdianzi.cn

C#:   public / protected / private / internal
来源：http://bk.chemitech.net.cn

[G11] getter / setter
来源：http://ft.nszjky.cn

Py:   @property 与 @x.setter
来源：http://st.bookmarksfly.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fu.9csxet.cn

JS:   get name() { return this._name; }
来源：http://xs.hahajie.cn

TS:   get name(): string { return this._name; }
来源：http://op.jianghongdianzi.cn

Java: public String getName() { return name; }
来源：http://ys.wgjwhj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bv.yuntaijiaju.cn

Ruby: attr_accessor :name
来源：http://ek.newstarts.cn

C#:   public string Name { get; set; }
来源：http://iy.9csxet.cn

[G12] 对象转字符串
来源：http://mf.gzmigu.cn

Py:   def __str__(self): return self.name
来源：http://ba.521024.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ew.haigaiapp.cn

JS:   toString() { return this.name; }
来源：http://ea.haigaiapp.cn

TS:   toString(): string { return this.name; }
来源：http://lv.gzmigu.cn

Java: @Override public String toString() { return name; }
来源：http://mk.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ty.9csxet.cn

Ruby: def to_s; @name; end
来源：http://hu.nicolike.cn

C#:   public override string ToString() => Name;
来源：http://up.9csxet.cn

[G13] 判断对象类型
来源：http://zg.asd995.cn

Py:   isinstance(u, User)
来源：http://ai.gzmigu.cn

PHP:  $u instanceof User
来源：http://yv.gzmigu.cn

JS:   u instanceof User
来源：http://nt.hahajie.cn

TS:   u instanceof User
来源：http://sz.haigaiapp.cn

Java: u instanceof User
来源：http://id.newstarts.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://or.huanxung.cn

Ruby: u.is_a?(User)
来源：http://ng.huixinmuqiang.cn

C#:   u is User
来源：http://au.szsharing.cn

[G14] 数据类 / record
来源：http://gs.hahajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cm.colortex.cn

PHP:  // 用 readonly 属性模拟
来源：http://fn.huixiangedu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vy.newstarts.cn

TS:   type User = { name: string; age: number };
来源：http://ft.szsharing.cn

Java: record User(String name, int age) {}
来源：http://ml.huixiangedu.cn

Go:   type User struct { Name string; Age int }
来源：http://cb.huanxung.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uy.szsharing.cn

C#:   record User(string Name, int Age);
来源：http://ik.asd995.cn

[G15] 枚举
来源：http://zo.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://js.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://io.chemitech.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ev.szxytkj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://no.lnxyls.cn

Java: enum Color { RED, GREEN }
来源：http://te.colortex.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://op.yuexingan06.cn

Ruby: Color = %i[red green].freeze
来源：http://ov.huanxung.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tv.szxytkj.cn

[G16] 对象转数组 / 字典
来源：http://oe.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wb.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://md.nicolike.cn

JS:   Object.entries(obj)
来源：http://qm.huixinmuqiang.cn

TS:   Object.entries(obj)
来源：http://fh.shxzskj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qc.gzmigu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dg.newstarts.cn

Ruby: obj.instance_variables
来源：http://fm.nszjky.cn

C#:   // 用反射或 System.Text.Json
来源：http://fk.yuntaijiaju.cn

================================================================================
来源：http://gs.gzmigu.cn

H. 异常与错误处理
来源：http://ww.newstarts.cn

================================================================================
来源：http://nf.gzmigu.cn

[H01] try / catch 基础
来源：http://ie.szsharing.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wv.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qq.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ed.nicolike.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tw.lnxyls.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zz.colortex.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://th.bookmarksfly.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kj.huixiangedu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xj.huixinmuqiang.cn

[H02] finally / ensure 收尾
来源：http://or.nicolike.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ay.hnjuh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qi.hnjuh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ry.nicolike.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://uh.hnjuh.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cr.jctech888.com.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fd.newstarts.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jh.huixiangedu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ey.chemitech.net.cn

[H03] 主动抛出异常
来源：http://mt.colortex.cn

Py:   raise ValueError("错误信息")
来源：http://sb.colortex.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cu.gzmigu.cn

JS:   throw new Error("错误信息");
来源：http://kd.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://hm.nicolike.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zh.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ou.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kj.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ag.yuexingan06.cn

[H04] 自定义异常类型
来源：http://cs.haigaiapp.cn

Py:   class MyError(Exception): pass
来源：http://hr.newstarts.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wm.bjjhwx.cn

JS:   class MyError extends Error {}
来源：http://zb.huixinmuqiang.cn

TS:   class MyError extends Error {}
来源：http://ly.szsharing.cn

Java: class MyException extends RuntimeException {}
来源：http://zn.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dy.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://pp.huixinmuqiang.cn

C#:   class MyException : Exception {}
来源：http://jc.colortex.cn

[H05] 捕获特定类型
来源：http://dz.bjjhwx.cn

Py:   except ValueError as e:
来源：http://pc.shtwfgs.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://is.bookmarksfly.cn

JS:   if (e instanceof TypeError) {}
来源：http://pg.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://zu.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://yi.hahajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ia.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://yn.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yh.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://gz.asd995.cn

Py:   value = d.get("k") or default
来源：http://tj.jctech888.com.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sg.nicolike.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fn.huixiangedu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ev.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kg.huanxung.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://di.asd995.cn

Ruby: d&.dig(:a, :b)
来源：http://tq.newstarts.cn

C#:   obj?.A?.B ?? default
来源：http://eq.haigaiapp.cn

[H07] 断言
来源：http://jt.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://ej.bookmarksfly.cn

PHP:  assert($x > 0);
来源：http://fy.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://tn.huanxung.cn

TS:   console.assert(x > 0);
来源：http://qi.shxzskj.cn

Java: assert x > 0 : "必须为正";
来源：http://hn.gzmigu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ue.colortex.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uy.nszjky.cn

C#:   Debug.Assert(x > 0);
来源：http://th.huixinmuqiang.cn

[H08] 获取错误信息与堆栈
来源：http://pq.bookmarksfly.cn

Py:   str(e);  traceback.format_exc()
来源：http://pi.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jf.hahajie.cn

JS:   e.message;  e.stack
来源：http://tj.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zm.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cn.jianghongdianzi.cn

Go:   err.Error()
来源：http://mr.huixinmuqiang.cn

Ruby: e.message;  e.backtrace
来源：http://wa.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://sz.haigaiapp.cn

[H09] 带错误码的异常
来源：http://zb.shxzskj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ak.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://np.chemitech.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cf.9csxet.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mn.yuexingan06.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fm.shtwfgs.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xr.jianghongdianzi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kp.bookmarksfly.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://lc.yuexingan06.cn

[H10] 资源自动释放
来源：http://yy.bookmarksfly.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kd.szsharing.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vj.bookmarksfly.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://el.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hw.shxzukj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rz.panjiajie.cn

Go:   defer f.Close()
来源：http://ua.jctech888.com.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ke.lnxyls.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://uq.hahajie.cn

================================================================================
来源：http://qk.shtwfgs.cn

I. 正则表达式
来源：http://ra.jianghongdianzi.cn

================================================================================
来源：http://np.nszjky.cn

[I01] 判断是否匹配
来源：http://vm.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nw.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fp.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://bi.newstarts.cn

TS:   /\d+/.test(s)
来源：http://ql.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ni.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jg.huixiangedu.cn

Ruby: s.match?(/\d+/)
来源：http://an.wgjwhj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://oh.chemitech.net.cn

[I02] 提取所有匹配
来源：http://sh.jctech888.com.cn

Py:   re.findall(r"\d+", s)
来源：http://oh.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nv.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rs.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://yy.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vh.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yq.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://kr.haigaiapp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wu.9csxet.cn

[I03] 提取捕获分组
来源：http://py.shxzskj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kz.gzmigu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zy.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wh.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fu.lnxyls.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kt.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://oo.jianghongdianzi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ew.gzmigu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ry.panjiajie.cn

[I04] 正则替换
来源：http://sz.chemitech.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ui.yuexingan06.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qx.hnjuh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://co.jianghongdianzi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ty.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ls.panjiajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pg.muxihuayi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jl.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://is.shxzukj.cn

[I05] 按正则拆分
来源：http://eq.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ci.jctech888.com.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qk.colortex.cn

JS:   s.split(/\s*,\s*/)
来源：http://to.bookmarksfly.cn

TS:   s.split(/\s*,\s*/)
来源：http://ra.huanxung.cn

Java: s.split("\\s*,\\s*")
来源：http://ai.hahajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dv.huixiangedu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zo.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cb.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nk.yuntaijiaju.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lv.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kt.szsharing.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ah.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zg.asd995.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zh.szsharing.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ps.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dk.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://bz.521024.cn

[I07] 忽略大小写与多行模式
来源：http://fi.wgjwhj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dk.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qw.lnxyls.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jo.panjiajie.cn

TS:   /error/gim
来源：http://he.hnjuh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yf.muxihuayi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cc.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://df.newstarts.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ic.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://ry.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gl.hnjuh.cn


<!-- 参考信息 -->