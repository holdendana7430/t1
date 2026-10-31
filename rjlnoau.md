代发 wailian999

TS:   constructor(public name: string) {}
来源：http://vp.shxzukj.cn

Java: User(String name) { this.name = name; }
来源：http://ok.bookmarksfly.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zg.colortex.cn

Ruby: def initialize(name); @name = name; end
来源：http://xa.huixinmuqiang.cn

C#:   public User(string name) { Name = name; }
来源：http://as.muxihuayi.cn

[G03] 实例属性
来源：http://pb.chemitech.net.cn

Py:   self.name = "x"
来源：http://ey.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://db.chemitech.net.cn

JS:   this.name = "x";
来源：http://ho.colortex.cn

TS:   name: string = "x";
来源：http://eh.panjiajie.cn

Java: private String name;
来源：http://jj.newstarts.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://no.shxzskj.cn

Ruby: @name = "x"
来源：http://os.gzmigu.cn

C#:   public string Name { get; set; } = "x";
来源：http://vr.hnjuh.cn

[G04] 定义方法
来源：http://yr.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://tn.9csxet.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://cs.521024.cn

JS:   greet() { return this.name; }
来源：http://ye.jianghongdianzi.cn

TS:   greet(): string { return this.name; }
来源：http://pb.nicolike.cn

Java: String greet() { return name; }
来源：http://uy.bookmarksfly.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cs.colortex.cn

Ruby: def greet; @name; end
来源：http://kg.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://xg.bookmarksfly.cn

[G05] 继承
来源：http://nf.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://hw.asd995.cn

PHP:  class Admin extends User {}
来源：http://qx.shxzukj.cn

JS:   class Admin extends User {}
来源：http://oj.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://dg.wgjwhj.cn

Java: class Admin extends User {}
来源：http://ek.bjjhwx.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://do.yuntaijiaju.cn

Ruby: class Admin < User; end
来源：http://xd.asd995.cn

C#:   class Admin : User {}
来源：http://as.521024.cn

[G06] 重写方法
来源：http://jp.shxzskj.cn

Py:   def greet(self): return "admin"
来源：http://kw.bjjhwx.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nh.yuntaijiaju.cn

JS:   greet() { return "admin"; }
来源：http://ng.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://rm.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://ox.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fr.szxytkj.cn

Ruby: def greet; "admin"; end
来源：http://tz.shtwfgs.cn

C#:   public override string Greet() => "admin";
来源：http://vn.huanxung.cn

[G07] 调用父类方法
来源：http://jt.huanxung.cn

Py:   super().greet()
来源：http://qa.huanxung.cn

PHP:  parent::greet();
来源：http://yh.shtwfgs.cn

JS:   super.greet();
来源：http://nd.asd995.cn

TS:   super.greet();
来源：http://ck.bjjhwx.cn

Java: super.greet();
来源：http://lg.gzmigu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mq.gzmigu.cn

Ruby: super
来源：http://cw.szxytkj.cn

C#:   base.Greet();
来源：http://gd.yuntaijiaju.cn

[G08] 静态方法与属性
来源：http://ga.muxihuayi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nw.yuexingan06.cn

PHP:  public static function f() {}
来源：http://br.huanxung.cn

JS:   static f() {}
来源：http://qu.yuntaijiaju.cn

TS:   static f(): void {}
来源：http://va.yuexingan06.cn

Java: static void f() {}
来源：http://yw.asd995.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://oz.huixiangedu.cn

Ruby: def self.f; end
来源：http://za.bookmarksfly.cn

C#:   public static void F() {}
来源：http://lp.muxihuayi.cn

[G09] 接口 / 抽象类
来源：http://sn.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://uk.shxzukj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kc.newstarts.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ko.hahajie.cn

TS:   interface Shape { area(): number; }
来源：http://sy.wgjwhj.cn

Java: interface Shape { double area(); }
来源：http://hh.huixinmuqiang.cn

Go:   type Shape interface { Area() float64 }
来源：http://kq.muxihuayi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ou.colortex.cn

C#:   interface IShape { double Area(); }
来源：http://it.jctech888.com.cn

[G10] 访问控制
来源：http://kk.gzmigu.cn

Py:   约定 _protected / __private（不强制）
来源：http://ko.bookmarksfly.cn

PHP:  public / protected / private
来源：http://cx.lnxyls.cn

JS:   #private 字段；其余公开
来源：http://zg.szsharing.cn

TS:   public / protected / private
来源：http://og.bjjhwx.cn

Java: public / protected / private / 默认包级
来源：http://st.panjiajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qh.huixiangedu.cn

Ruby: public / protected / private
来源：http://mn.bjjhwx.cn

C#:   public / protected / private / internal
来源：http://tq.yuexingan06.cn

[G11] getter / setter
来源：http://cg.shxzukj.cn

Py:   @property 与 @x.setter
来源：http://vw.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lf.9csxet.cn

JS:   get name() { return this._name; }
来源：http://ct.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://gd.huixiangedu.cn

Java: public String getName() { return name; }
来源：http://xn.panjiajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qo.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://hj.huixinmuqiang.cn

C#:   public string Name { get; set; }
来源：http://ax.shtwfgs.cn

[G12] 对象转字符串
来源：http://eu.muxihuayi.cn

Py:   def __str__(self): return self.name
来源：http://ls.huixinmuqiang.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vm.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://rm.hahajie.cn

TS:   toString(): string { return this.name; }
来源：http://qd.huixiangedu.cn

Java: @Override public String toString() { return name; }
来源：http://uc.bookmarksfly.cn

Go:   func (u User) String() string { return u.Name }
来源：http://he.jctech888.com.cn

Ruby: def to_s; @name; end
来源：http://xh.wgjwhj.cn

C#:   public override string ToString() => Name;
来源：http://es.muxihuayi.cn

[G13] 判断对象类型
来源：http://au.nszjky.cn

Py:   isinstance(u, User)
来源：http://zp.szxytkj.cn

PHP:  $u instanceof User
来源：http://ly.haigaiapp.cn

JS:   u instanceof User
来源：http://wq.szxytkj.cn

TS:   u instanceof User
来源：http://zz.huixiangedu.cn

Java: u instanceof User
来源：http://qk.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://to.nszjky.cn

Ruby: u.is_a?(User)
来源：http://qm.bookmarksfly.cn

C#:   u is User
来源：http://rv.shxzskj.cn

[G14] 数据类 / record
来源：http://wg.huixinmuqiang.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ml.shtwfgs.cn

PHP:  // 用 readonly 属性模拟
来源：http://jl.yuexingan06.cn

JS:   // 无内置：普通类或对象字面量
来源：http://up.huixiangedu.cn

TS:   type User = { name: string; age: number };
来源：http://vb.bjjhwx.cn

Java: record User(String name, int age) {}
来源：http://li.yuexingan06.cn

Go:   type User struct { Name string; Age int }
来源：http://qj.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kf.szsharing.cn

C#:   record User(string Name, int Age);
来源：http://bh.chemitech.net.cn

[G15] 枚举
来源：http://ay.yuexingan06.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gc.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xy.szxytkj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yn.nszjky.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zs.asd995.cn

Java: enum Color { RED, GREEN }
来源：http://uv.nicolike.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mu.521024.cn

Ruby: Color = %i[red green].freeze
来源：http://yc.panjiajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gf.lnxyls.cn

[G16] 对象转数组 / 字典
来源：http://ve.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ob.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://mm.nszjky.cn

JS:   Object.entries(obj)
来源：http://ru.colortex.cn

TS:   Object.entries(obj)
来源：http://mo.521024.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fn.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://km.wgjwhj.cn

Ruby: obj.instance_variables
来源：http://nr.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://ub.yuexingan06.cn

================================================================================
来源：http://sw.szsharing.cn

H. 异常与错误处理
来源：http://an.hnjuh.cn

================================================================================
来源：http://bl.jctech888.com.cn

[H01] try / catch 基础
来源：http://qw.hahajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gu.muxihuayi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pe.yuntaijiaju.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dv.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uc.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://el.huixiangedu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mq.9csxet.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xf.szxytkj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uj.yuntaijiaju.cn

[H02] finally / ensure 收尾
来源：http://ca.newstarts.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gj.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ih.asd995.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://af.gzmigu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://po.bjjhwx.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gb.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rc.jctech888.com.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://aw.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nu.szsharing.cn

[H03] 主动抛出异常
来源：http://zz.wgjwhj.cn

Py:   raise ValueError("错误信息")
来源：http://hx.hnjuh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qd.yuntaijiaju.cn

JS:   throw new Error("错误信息");
来源：http://jz.521024.cn

TS:   throw new Error("错误信息");
来源：http://in.wgjwhj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://uf.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ta.newstarts.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ip.shxzskj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qt.521024.cn

[H04] 自定义异常类型
来源：http://pk.szsharing.cn

Py:   class MyError(Exception): pass
来源：http://jm.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://si.newstarts.cn

JS:   class MyError extends Error {}
来源：http://uj.wgjwhj.cn

TS:   class MyError extends Error {}
来源：http://yi.jianghongdianzi.cn

Java: class MyException extends RuntimeException {}
来源：http://ub.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zb.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://yi.nicolike.cn

C#:   class MyException : Exception {}
来源：http://tg.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://mx.shtwfgs.cn

Py:   except ValueError as e:
来源：http://wd.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yu.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://nm.9csxet.cn

TS:   if (e instanceof TypeError) {}
来源：http://wt.asd995.cn

Java: catch (IOException | SQLException e) {}
来源：http://si.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fk.wgjwhj.cn

Ruby: rescue ArgumentError => e
来源：http://mu.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ch.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://bc.bookmarksfly.cn

Py:   value = d.get("k") or default
来源：http://pm.bjjhwx.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rx.chemitech.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qa.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://is.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vz.gzmigu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xu.huixinmuqiang.cn

Ruby: d&.dig(:a, :b)
来源：http://md.shtwfgs.cn

C#:   obj?.A?.B ?? default
来源：http://rp.nszjky.cn

[H07] 断言
来源：http://wu.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://hw.hahajie.cn

PHP:  assert($x > 0);
来源：http://mk.yuexingan06.cn

JS:   console.assert(x > 0);
来源：http://xe.panjiajie.cn

TS:   console.assert(x > 0);
来源：http://cj.muxihuayi.cn

Java: assert x > 0 : "必须为正";
来源：http://dg.wgjwhj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dt.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jy.newstarts.cn

C#:   Debug.Assert(x > 0);
来源：http://nq.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://iu.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://ck.huixinmuqiang.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ra.newstarts.cn

JS:   e.message;  e.stack
来源：http://rn.jianghongdianzi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ir.jianghongdianzi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tv.521024.cn

Go:   err.Error()
来源：http://cw.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://qw.bookmarksfly.cn

C#:   e.Message;  e.StackTrace
来源：http://ou.szxytkj.cn

[H09] 带错误码的异常
来源：http://xq.chemitech.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pb.szsharing.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ev.szxytkj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zb.9csxet.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nz.hnjuh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qa.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xe.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jx.huixinmuqiang.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dm.yuexingan06.cn

[H10] 资源自动释放
来源：http://ip.521024.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bh.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kw.asd995.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ln.chemitech.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lv.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pz.asd995.cn

Go:   defer f.Close()
来源：http://we.chemitech.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://uy.wgjwhj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lv.yuntaijiaju.cn

================================================================================
来源：http://ua.521024.cn

I. 正则表达式
来源：http://rn.haigaiapp.cn

================================================================================
来源：http://ov.huixinmuqiang.cn

[I01] 判断是否匹配
来源：http://bq.huixiangedu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mj.huixiangedu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zv.521024.cn

JS:   /\d+/.test(s)
来源：http://dt.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://eb.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bl.9csxet.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yz.521024.cn

Ruby: s.match?(/\d+/)
来源：http://pc.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vh.shtwfgs.cn

[I02] 提取所有匹配
来源：http://ex.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://hu.chemitech.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yh.szsharing.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dc.bjjhwx.cn

TS:   s.match(/\d+/g)
来源：http://wx.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bb.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wv.haigaiapp.cn

Ruby: s.scan(/\d+/)
来源：http://aq.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kz.521024.cn

[I03] 提取捕获分组
来源：http://ki.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ad.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fp.asd995.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://il.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mb.chemitech.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ng.newstarts.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wy.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pb.yuntaijiaju.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zb.chemitech.net.cn

[I04] 正则替换
来源：http://za.muxihuayi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://av.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gy.shxzukj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ni.huixinmuqiang.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jq.bookmarksfly.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xc.gzmigu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://py.521024.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gp.chemitech.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dx.huanxung.cn

[I05] 按正则拆分
来源：http://xx.shtwfgs.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fv.yuntaijiaju.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nl.haigaiapp.cn

JS:   s.split(/\s*,\s*/)
来源：http://tq.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://sv.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://yb.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bg.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wm.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ge.yuexingan06.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://la.gzmigu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cu.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uw.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zi.huanxung.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ct.asd995.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xb.jctech888.com.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yc.yuexingan06.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ms.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://to.nicolike.cn

[I07] 忽略大小写与多行模式
来源：http://uf.gzmigu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://so.bjjhwx.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ju.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://od.haigaiapp.cn

TS:   /error/gim
来源：http://kz.hahajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ad.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hu.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://wv.jctech888.com.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tx.521024.cn

[I08] 贪婪与非贪婪匹配
来源：http://vm.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vv.newstarts.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mh.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pf.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pr.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://eh.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xg.colortex.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yk.huanxung.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jo.szsharing.cn

================================================================================
来源：http://mo.colortex.cn


<!-- 参考信息 -->