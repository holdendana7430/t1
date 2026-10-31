代发 wailian999

Py:   class User: pass
来源：http://li.shtwfgs.cn

PHP:  class User {}
来源：http://pr.yuntaijiaju.cn

JS:   class User {}
来源：http://ak.shtwfgs.cn

TS:   class User { name: string = ""; }
来源：http://xm.szsharing.cn

Java: class User {}
来源：http://xu.asd995.cn

Go:   type User struct { Name string }
来源：http://ki.nszjky.cn

Ruby: class User; end
来源：http://ap.yuntaijiaju.cn

C#:   class User {}
来源：http://go.panjiajie.cn

[G02] 构造函数
来源：http://ua.muxihuayi.cn

Py:   def __init__(self, name): self.name = name
来源：http://li.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://dd.muxihuayi.cn

JS:   constructor(name) { this.name = name; }
来源：http://yv.szsharing.cn

TS:   constructor(public name: string) {}
来源：http://gl.521024.cn

Java: User(String name) { this.name = name; }
来源：http://vc.jianghongdianzi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ko.lnxyls.cn

Ruby: def initialize(name); @name = name; end
来源：http://rc.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://wq.lnxyls.cn

[G03] 实例属性
来源：http://gm.huixiangedu.cn

Py:   self.name = "x"
来源：http://cj.newstarts.cn

PHP:  public string $name = "x";
来源：http://mb.huixiangedu.cn

JS:   this.name = "x";
来源：http://ug.newstarts.cn

TS:   name: string = "x";
来源：http://yh.chemitech.net.cn

Java: private String name;
来源：http://jo.shxzskj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://pz.9csxet.cn

Ruby: @name = "x"
来源：http://ta.szsharing.cn

C#:   public string Name { get; set; } = "x";
来源：http://qq.chemitech.net.cn

[G04] 定义方法
来源：http://jk.yuntaijiaju.cn

Py:   def greet(self): return self.name
来源：http://gb.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://mx.lnxyls.cn

JS:   greet() { return this.name; }
来源：http://me.bjjhwx.cn

TS:   greet(): string { return this.name; }
来源：http://lf.haigaiapp.cn

Java: String greet() { return name; }
来源：http://gt.hnjuh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lc.huanxung.cn

Ruby: def greet; @name; end
来源：http://hu.bjjhwx.cn

C#:   public string Greet() => Name;
来源：http://xr.szsharing.cn

[G05] 继承
来源：http://ps.szxytkj.cn

Py:   class Admin(User): pass
来源：http://tv.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://lv.shxzukj.cn

JS:   class Admin extends User {}
来源：http://vn.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://fs.shxzskj.cn

Java: class Admin extends User {}
来源：http://tu.hnjuh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xs.jctech888.com.cn

Ruby: class Admin < User; end
来源：http://np.gzmigu.cn

C#:   class Admin : User {}
来源：http://yb.shtwfgs.cn

[G06] 重写方法
来源：http://kx.bjjhwx.cn

Py:   def greet(self): return "admin"
来源：http://je.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nz.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://xj.shtwfgs.cn

TS:   greet(): string { return "admin"; }
来源：http://lj.lnxyls.cn

Java: @Override String greet() { return "admin"; }
来源：http://kc.nszjky.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vz.lnxyls.cn

Ruby: def greet; "admin"; end
来源：http://vm.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://jq.haigaiapp.cn

[G07] 调用父类方法
来源：http://vn.shxzskj.cn

Py:   super().greet()
来源：http://iv.shxzskj.cn

PHP:  parent::greet();
来源：http://kz.huixinmuqiang.cn

JS:   super.greet();
来源：http://ui.jianghongdianzi.cn

TS:   super.greet();
来源：http://jp.9csxet.cn

Java: super.greet();
来源：http://ku.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bs.shxzskj.cn

Ruby: super
来源：http://zk.huixiangedu.cn

C#:   base.Greet();
来源：http://ig.jianghongdianzi.cn

[G08] 静态方法与属性
来源：http://lx.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hn.shtwfgs.cn

PHP:  public static function f() {}
来源：http://ox.haigaiapp.cn

JS:   static f() {}
来源：http://ug.chemitech.net.cn

TS:   static f(): void {}
来源：http://ov.panjiajie.cn

Java: static void f() {}
来源：http://tw.wgjwhj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jz.haigaiapp.cn

Ruby: def self.f; end
来源：http://vl.newstarts.cn

C#:   public static void F() {}
来源：http://wn.nszjky.cn

[G09] 接口 / 抽象类
来源：http://tu.hnjuh.cn

Py:   from abc import ABC, abstractmethod
来源：http://pa.jianghongdianzi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dj.shxzskj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://by.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://sv.shtwfgs.cn

Java: interface Shape { double area(); }
来源：http://gq.szxytkj.cn

Go:   type Shape interface { Area() float64 }
来源：http://mr.nszjky.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xv.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://kl.lnxyls.cn

[G10] 访问控制
来源：http://cr.huanxung.cn

Py:   约定 _protected / __private（不强制）
来源：http://db.shtwfgs.cn

PHP:  public / protected / private
来源：http://hz.shxzukj.cn

JS:   #private 字段；其余公开
来源：http://qy.huanxung.cn

TS:   public / protected / private
来源：http://qz.haigaiapp.cn

Java: public / protected / private / 默认包级
来源：http://hw.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://af.huanxung.cn

Ruby: public / protected / private
来源：http://ut.chemitech.net.cn

C#:   public / protected / private / internal
来源：http://xi.shtwfgs.cn

[G11] getter / setter
来源：http://lm.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://dl.huixiangedu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wu.muxihuayi.cn

JS:   get name() { return this._name; }
来源：http://gb.szsharing.cn

TS:   get name(): string { return this._name; }
来源：http://bt.gzmigu.cn

Java: public String getName() { return name; }
来源：http://zt.gzmigu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fl.szxytkj.cn

Ruby: attr_accessor :name
来源：http://mk.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://kb.nicolike.cn

[G12] 对象转字符串
来源：http://zd.shxzukj.cn

Py:   def __str__(self): return self.name
来源：http://yw.521024.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xl.yuexingan06.cn

JS:   toString() { return this.name; }
来源：http://ex.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://lh.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://xa.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qo.szsharing.cn

Ruby: def to_s; @name; end
来源：http://gu.lnxyls.cn

C#:   public override string ToString() => Name;
来源：http://ig.521024.cn

[G13] 判断对象类型
来源：http://gm.bjjhwx.cn

Py:   isinstance(u, User)
来源：http://ww.asd995.cn

PHP:  $u instanceof User
来源：http://zb.yuntaijiaju.cn

JS:   u instanceof User
来源：http://tq.bookmarksfly.cn

TS:   u instanceof User
来源：http://qp.hnjuh.cn

Java: u instanceof User
来源：http://lp.newstarts.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ey.huixiangedu.cn

Ruby: u.is_a?(User)
来源：http://qm.9csxet.cn

C#:   u is User
来源：http://yt.shxzukj.cn

[G14] 数据类 / record
来源：http://et.shxzskj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qg.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://fk.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jw.panjiajie.cn

TS:   type User = { name: string; age: number };
来源：http://ek.nicolike.cn

Java: record User(String name, int age) {}
来源：http://ss.bjjhwx.cn

Go:   type User struct { Name string; Age int }
来源：http://zr.shtwfgs.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qg.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://kc.lnxyls.cn

[G15] 枚举
来源：http://td.shxzskj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hc.chemitech.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vi.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zn.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ga.haigaiapp.cn

Java: enum Color { RED, GREEN }
来源：http://mp.muxihuayi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pl.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://mh.lnxyls.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mg.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://yq.nszjky.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qh.jctech888.com.cn

PHP:  get_object_vars($obj);
来源：http://ry.panjiajie.cn

JS:   Object.entries(obj)
来源：http://ya.huixiangedu.cn

TS:   Object.entries(obj)
来源：http://vh.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jn.panjiajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://oi.shxzukj.cn

Ruby: obj.instance_variables
来源：http://kv.wgjwhj.cn

C#:   // 用反射或 System.Text.Json
来源：http://ko.asd995.cn

================================================================================
来源：http://rj.szsharing.cn

H. 异常与错误处理
来源：http://vm.asd995.cn

================================================================================
来源：http://eo.yuexingan06.cn

[H01] try / catch 基础
来源：http://li.9csxet.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xu.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ql.lnxyls.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fs.szxytkj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zp.yuexingan06.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nz.nszjky.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ts.bjjhwx.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ig.nszjky.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ee.szxytkj.cn

[H02] finally / ensure 收尾
来源：http://bb.haigaiapp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hs.hnjuh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bv.shxzukj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jx.nszjky.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yd.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bj.szsharing.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ij.haigaiapp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mf.shtwfgs.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://kv.nszjky.cn

[H03] 主动抛出异常
来源：http://mx.panjiajie.cn

Py:   raise ValueError("错误信息")
来源：http://zj.yuntaijiaju.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fd.521024.cn

JS:   throw new Error("错误信息");
来源：http://qe.521024.cn

TS:   throw new Error("错误信息");
来源：http://gg.muxihuayi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ns.chemitech.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tc.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yt.wgjwhj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://oq.shxzukj.cn

[H04] 自定义异常类型
来源：http://lv.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://ag.asd995.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sg.lnxyls.cn

JS:   class MyError extends Error {}
来源：http://ul.jianghongdianzi.cn

TS:   class MyError extends Error {}
来源：http://nc.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://fh.hnjuh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lq.hnjuh.cn

Ruby: class MyError < StandardError; end
来源：http://vt.szsharing.cn

C#:   class MyException : Exception {}
来源：http://yw.huixiangedu.cn

[H05] 捕获特定类型
来源：http://ob.shtwfgs.cn

Py:   except ValueError as e:
来源：http://fj.huixinmuqiang.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://oc.jianghongdianzi.cn

JS:   if (e instanceof TypeError) {}
来源：http://dy.huanxung.cn

TS:   if (e instanceof TypeError) {}
来源：http://sa.nicolike.cn

Java: catch (IOException | SQLException e) {}
来源：http://gr.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ea.szsharing.cn

Ruby: rescue ArgumentError => e
来源：http://se.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lp.yuexingan06.cn

[H06] 可选值 / 空值安全访问
来源：http://yw.chemitech.net.cn

Py:   value = d.get("k") or default
来源：http://sg.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nl.szxytkj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wz.yuntaijiaju.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ne.9csxet.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mu.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://je.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://pp.shxzskj.cn

C#:   obj?.A?.B ?? default
来源：http://sl.colortex.cn

[H07] 断言
来源：http://ud.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://qf.colortex.cn

PHP:  assert($x > 0);
来源：http://ws.newstarts.cn

JS:   console.assert(x > 0);
来源：http://wd.asd995.cn

TS:   console.assert(x > 0);
来源：http://zd.panjiajie.cn

Java: assert x > 0 : "必须为正";
来源：http://dz.muxihuayi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zs.bjjhwx.cn

Ruby: raise "必须为正" unless x > 0
来源：http://do.jctech888.com.cn

C#:   Debug.Assert(x > 0);
来源：http://ls.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://nu.newstarts.cn

Py:   str(e);  traceback.format_exc()
来源：http://va.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kr.9csxet.cn

JS:   e.message;  e.stack
来源：http://eh.huanxung.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ih.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zv.hnjuh.cn

Go:   err.Error()
来源：http://mj.szsharing.cn

Ruby: e.message;  e.backtrace
来源：http://oq.nszjky.cn

C#:   e.Message;  e.StackTrace
来源：http://hj.shxzukj.cn

[H09] 带错误码的异常
来源：http://bb.yuntaijiaju.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lh.chemitech.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ga.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ay.shtwfgs.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://te.yuexingan06.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://oi.haigaiapp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cr.newstarts.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ov.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gg.wgjwhj.cn

[H10] 资源自动释放
来源：http://ka.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ve.szsharing.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fw.9csxet.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yl.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qt.shxzukj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ok.shxzukj.cn

Go:   defer f.Close()
来源：http://tk.nicolike.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nl.hahajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jo.chemitech.net.cn

================================================================================
来源：http://ot.wgjwhj.cn

I. 正则表达式
来源：http://oy.asd995.cn

================================================================================
来源：http://hr.wgjwhj.cn

[I01] 判断是否匹配
来源：http://jz.szsharing.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tw.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jc.szxytkj.cn

JS:   /\d+/.test(s)
来源：http://jh.huanxung.cn

TS:   /\d+/.test(s)
来源：http://xe.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nj.colortex.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zr.yuexingan06.cn

Ruby: s.match?(/\d+/)
来源：http://et.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wv.yuntaijiaju.cn

[I02] 提取所有匹配
来源：http://og.gzmigu.cn

Py:   re.findall(r"\d+", s)
来源：http://gy.asd995.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ze.lnxyls.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kw.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://na.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://js.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yv.gzmigu.cn

Ruby: s.scan(/\d+/)
来源：http://le.newstarts.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://as.jctech888.com.cn

[I03] 提取捕获分组
来源：http://qe.hnjuh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rs.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dz.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ym.nszjky.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ju.szsharing.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tj.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://om.yuexingan06.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gm.jianghongdianzi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kc.gzmigu.cn

[I04] 正则替换
来源：http://db.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lw.521024.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qy.panjiajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zd.muxihuayi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://oz.shxzskj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ho.bookmarksfly.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ni.panjiajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bj.chemitech.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ee.lnxyls.cn

[I05] 按正则拆分
来源：http://mh.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tu.haigaiapp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gi.asd995.cn

JS:   s.split(/\s*,\s*/)
来源：http://qs.hnjuh.cn

TS:   s.split(/\s*,\s*/)
来源：http://kq.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://bq.lnxyls.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ab.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ux.521024.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fi.nicolike.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yi.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ac.nszjky.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://il.bjjhwx.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gj.jctech888.com.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://aq.szxytkj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ev.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mu.521024.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ko.bookmarksfly.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ra.haigaiapp.cn

[I07] 忽略大小写与多行模式
来源：http://oi.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ys.bookmarksfly.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://tu.yuexingan06.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yk.haigaiapp.cn

TS:   /error/gim
来源：http://qq.lnxyls.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dd.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ee.9csxet.cn


<!-- 参考信息 -->