代发 wailian999

[G02] 构造函数
来源：http://rg.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://du.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://yk.szsharing.cn

JS:   constructor(name) { this.name = name; }
来源：http://ni.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://rx.asd995.cn

Java: User(String name) { this.name = name; }
来源：http://ta.gzmigu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ui.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://xo.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://fj.chemitech.net.cn

[G03] 实例属性
来源：http://zl.yuexingan06.cn

Py:   self.name = "x"
来源：http://lt.nicolike.cn

PHP:  public string $name = "x";
来源：http://wl.bookmarksfly.cn

JS:   this.name = "x";
来源：http://gc.shtwfgs.cn

TS:   name: string = "x";
来源：http://kj.gzmigu.cn

Java: private String name;
来源：http://dk.bjjhwx.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oe.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://il.szxytkj.cn

C#:   public string Name { get; set; } = "x";
来源：http://zh.huanxung.cn

[G04] 定义方法
来源：http://lk.yuntaijiaju.cn

Py:   def greet(self): return self.name
来源：http://bs.huanxung.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tb.lnxyls.cn

JS:   greet() { return this.name; }
来源：http://lz.shxzskj.cn

TS:   greet(): string { return this.name; }
来源：http://kj.jctech888.com.cn

Java: String greet() { return name; }
来源：http://ux.nicolike.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xt.yuexingan06.cn

Ruby: def greet; @name; end
来源：http://fz.huixinmuqiang.cn

C#:   public string Greet() => Name;
来源：http://lg.panjiajie.cn

[G05] 继承
来源：http://ka.panjiajie.cn

Py:   class Admin(User): pass
来源：http://lc.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://zl.huixiangedu.cn

JS:   class Admin extends User {}
来源：http://us.nicolike.cn

TS:   class Admin extends User {}
来源：http://ew.chemitech.net.cn

Java: class Admin extends User {}
来源：http://mm.hnjuh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://py.nicolike.cn

Ruby: class Admin < User; end
来源：http://ku.hahajie.cn

C#:   class Admin : User {}
来源：http://xh.bjjhwx.cn

[G06] 重写方法
来源：http://at.asd995.cn

Py:   def greet(self): return "admin"
来源：http://kr.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://go.newstarts.cn

JS:   greet() { return "admin"; }
来源：http://kq.haigaiapp.cn

TS:   greet(): string { return "admin"; }
来源：http://nc.colortex.cn

Java: @Override String greet() { return "admin"; }
来源：http://eg.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ww.colortex.cn

Ruby: def greet; "admin"; end
来源：http://ol.hahajie.cn

C#:   public override string Greet() => "admin";
来源：http://ds.nszjky.cn

[G07] 调用父类方法
来源：http://pv.hnjuh.cn

Py:   super().greet()
来源：http://ha.chemitech.net.cn

PHP:  parent::greet();
来源：http://pi.yuntaijiaju.cn

JS:   super.greet();
来源：http://qd.szsharing.cn

TS:   super.greet();
来源：http://vq.shtwfgs.cn

Java: super.greet();
来源：http://gk.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dg.nszjky.cn

Ruby: super
来源：http://zo.hahajie.cn

C#:   base.Greet();
来源：http://xu.shxzskj.cn

[G08] 静态方法与属性
来源：http://ar.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hi.jctech888.com.cn

PHP:  public static function f() {}
来源：http://zs.szsharing.cn

JS:   static f() {}
来源：http://ss.yuntaijiaju.cn

TS:   static f(): void {}
来源：http://gw.jctech888.com.cn

Java: static void f() {}
来源：http://qy.huixiangedu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zc.nicolike.cn

Ruby: def self.f; end
来源：http://ab.hnjuh.cn

C#:   public static void F() {}
来源：http://zo.521024.cn

[G09] 接口 / 抽象类
来源：http://zu.muxihuayi.cn

Py:   from abc import ABC, abstractmethod
来源：http://xn.szxytkj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jp.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yo.jctech888.com.cn

TS:   interface Shape { area(): number; }
来源：http://nx.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://xt.huixinmuqiang.cn

Go:   type Shape interface { Area() float64 }
来源：http://jh.jianghongdianzi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ej.shxzskj.cn

C#:   interface IShape { double Area(); }
来源：http://th.hahajie.cn

[G10] 访问控制
来源：http://ir.jianghongdianzi.cn

Py:   约定 _protected / __private（不强制）
来源：http://lb.panjiajie.cn

PHP:  public / protected / private
来源：http://zq.jianghongdianzi.cn

JS:   #private 字段；其余公开
来源：http://bq.yuntaijiaju.cn

TS:   public / protected / private
来源：http://zw.shxzukj.cn

Java: public / protected / private / 默认包级
来源：http://kv.jctech888.com.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://oa.asd995.cn

Ruby: public / protected / private
来源：http://cl.lnxyls.cn

C#:   public / protected / private / internal
来源：http://nv.bjjhwx.cn

[G11] getter / setter
来源：http://ev.colortex.cn

Py:   @property 与 @x.setter
来源：http://lv.shxzukj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fh.shxzskj.cn

JS:   get name() { return this._name; }
来源：http://ig.hahajie.cn

TS:   get name(): string { return this._name; }
来源：http://ry.nicolike.cn

Java: public String getName() { return name; }
来源：http://cb.szsharing.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qt.nicolike.cn

Ruby: attr_accessor :name
来源：http://ai.bookmarksfly.cn

C#:   public string Name { get; set; }
来源：http://lw.nicolike.cn

[G12] 对象转字符串
来源：http://tl.haigaiapp.cn

Py:   def __str__(self): return self.name
来源：http://ja.lnxyls.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qi.newstarts.cn

JS:   toString() { return this.name; }
来源：http://xx.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://pv.newstarts.cn

Java: @Override public String toString() { return name; }
来源：http://wg.yuntaijiaju.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ic.bjjhwx.cn

Ruby: def to_s; @name; end
来源：http://ke.chemitech.net.cn

C#:   public override string ToString() => Name;
来源：http://rr.muxihuayi.cn

[G13] 判断对象类型
来源：http://it.bjjhwx.cn

Py:   isinstance(u, User)
来源：http://vq.huanxung.cn

PHP:  $u instanceof User
来源：http://jn.bjjhwx.cn

JS:   u instanceof User
来源：http://lc.huixiangedu.cn

TS:   u instanceof User
来源：http://hn.gzmigu.cn

Java: u instanceof User
来源：http://yn.asd995.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kt.521024.cn

Ruby: u.is_a?(User)
来源：http://yd.wgjwhj.cn

C#:   u is User
来源：http://yc.yuexingan06.cn

[G14] 数据类 / record
来源：http://es.chemitech.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gs.lnxyls.cn

PHP:  // 用 readonly 属性模拟
来源：http://ne.hahajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bd.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://rx.bjjhwx.cn

Java: record User(String name, int age) {}
来源：http://nr.hnjuh.cn

Go:   type User struct { Name string; Age int }
来源：http://ba.bjjhwx.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bv.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://kl.szxytkj.cn

[G15] 枚举
来源：http://ry.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sa.521024.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wb.wgjwhj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ei.wgjwhj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jm.wgjwhj.cn

Java: enum Color { RED, GREEN }
来源：http://kd.muxihuayi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://by.huixiangedu.cn

Ruby: Color = %i[red green].freeze
来源：http://nq.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fi.lnxyls.cn

[G16] 对象转数组 / 字典
来源：http://yp.9csxet.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://az.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://ji.hahajie.cn

JS:   Object.entries(obj)
来源：http://va.yuexingan06.cn

TS:   Object.entries(obj)
来源：http://zq.jianghongdianzi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://me.szsharing.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hf.bookmarksfly.cn

Ruby: obj.instance_variables
来源：http://pb.colortex.cn

C#:   // 用反射或 System.Text.Json
来源：http://hn.lnxyls.cn

================================================================================
来源：http://vu.lnxyls.cn

H. 异常与错误处理
来源：http://xe.bookmarksfly.cn

================================================================================
来源：http://et.shxzskj.cn

[H01] try / catch 基础
来源：http://cm.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rv.muxihuayi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yw.gzmigu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fm.chemitech.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ln.haigaiapp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://we.chemitech.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://km.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ye.huixinmuqiang.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kq.shtwfgs.cn

[H02] finally / ensure 收尾
来源：http://wu.newstarts.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qg.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tz.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vk.shxzskj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ra.shxzskj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mx.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zz.jianghongdianzi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mz.yuexingan06.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nj.szxytkj.cn

[H03] 主动抛出异常
来源：http://fd.panjiajie.cn

Py:   raise ValueError("错误信息")
来源：http://oz.szsharing.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nj.bookmarksfly.cn

JS:   throw new Error("错误信息");
来源：http://st.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://nd.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xc.yuntaijiaju.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ec.hahajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mm.shxzskj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://re.asd995.cn

[H04] 自定义异常类型
来源：http://fq.huixinmuqiang.cn

Py:   class MyError(Exception): pass
来源：http://xh.huixiangedu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ak.nicolike.cn

JS:   class MyError extends Error {}
来源：http://ue.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://vm.chemitech.net.cn

Java: class MyException extends RuntimeException {}
来源：http://ob.bjjhwx.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bv.huixinmuqiang.cn

Ruby: class MyError < StandardError; end
来源：http://rs.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://cs.yuntaijiaju.cn

[H05] 捕获特定类型
来源：http://rx.haigaiapp.cn

Py:   except ValueError as e:
来源：http://wg.jianghongdianzi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mp.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://gv.huixinmuqiang.cn

TS:   if (e instanceof TypeError) {}
来源：http://ww.lnxyls.cn

Java: catch (IOException | SQLException e) {}
来源：http://cm.asd995.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://eb.shxzukj.cn

Ruby: rescue ArgumentError => e
来源：http://jy.jianghongdianzi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ia.muxihuayi.cn

[H06] 可选值 / 空值安全访问
来源：http://tk.huixiangedu.cn

Py:   value = d.get("k") or default
来源：http://lu.gzmigu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ki.nszjky.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rm.szsharing.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vi.bookmarksfly.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uv.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wz.newstarts.cn

Ruby: d&.dig(:a, :b)
来源：http://ng.colortex.cn

C#:   obj?.A?.B ?? default
来源：http://kj.szsharing.cn

[H07] 断言
来源：http://cl.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://mx.lnxyls.cn

PHP:  assert($x > 0);
来源：http://zr.shxzskj.cn

JS:   console.assert(x > 0);
来源：http://jv.yuexingan06.cn

TS:   console.assert(x > 0);
来源：http://he.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://dd.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jh.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ek.bjjhwx.cn

C#:   Debug.Assert(x > 0);
来源：http://ss.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://sm.muxihuayi.cn

Py:   str(e);  traceback.format_exc()
来源：http://xp.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oy.haigaiapp.cn

JS:   e.message;  e.stack
来源：http://qo.colortex.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kd.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://en.huixinmuqiang.cn

Go:   err.Error()
来源：http://ck.szxytkj.cn

Ruby: e.message;  e.backtrace
来源：http://vu.hahajie.cn

C#:   e.Message;  e.StackTrace
来源：http://yz.hahajie.cn

[H09] 带错误码的异常
来源：http://bq.9csxet.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://aa.gzmigu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ii.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ih.chemitech.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cc.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lf.asd995.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ws.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ls.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qn.bjjhwx.cn

[H10] 资源自动释放
来源：http://qk.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gi.nszjky.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ge.huixinmuqiang.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ov.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sn.szxytkj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cg.9csxet.cn

Go:   defer f.Close()
来源：http://zc.szxytkj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yy.panjiajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://op.bjjhwx.cn

================================================================================
来源：http://fm.bjjhwx.cn

I. 正则表达式
来源：http://oc.shtwfgs.cn

================================================================================
来源：http://cy.hnjuh.cn

[I01] 判断是否匹配
来源：http://cq.panjiajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ox.huixiangedu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wj.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://cn.yuntaijiaju.cn

TS:   /\d+/.test(s)
来源：http://hv.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sk.huanxung.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wc.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://gb.jctech888.com.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vt.bjjhwx.cn

[I02] 提取所有匹配
来源：http://js.nicolike.cn

Py:   re.findall(r"\d+", s)
来源：http://tt.lnxyls.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qa.jctech888.com.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://kb.nicolike.cn

TS:   s.match(/\d+/g)
来源：http://dg.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vt.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hj.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://om.yuexingan06.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bp.muxihuayi.cn

[I03] 提取捕获分组
来源：http://ac.nszjky.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kq.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rl.newstarts.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pk.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jo.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bg.nicolike.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tb.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dl.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xf.szsharing.cn

[I04] 正则替换
来源：http://kk.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gh.yuexingan06.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ea.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wr.panjiajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wc.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pv.szsharing.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cu.jianghongdianzi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://js.bjjhwx.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fc.muxihuayi.cn

[I05] 按正则拆分
来源：http://bu.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://tu.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://af.521024.cn

JS:   s.split(/\s*,\s*/)
来源：http://zi.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://fm.shtwfgs.cn

Java: s.split("\\s*,\\s*")
来源：http://gp.shxzskj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://au.panjiajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ko.nicolike.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qt.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vt.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hx.hahajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kr.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jm.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xa.colortex.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lo.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fv.nszjky.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hc.newstarts.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yu.521024.cn

[I07] 忽略大小写与多行模式
来源：http://zp.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yn.bjjhwx.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wq.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xt.szxytkj.cn

TS:   /error/gim
来源：http://bz.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wi.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bg.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://sv.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://km.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://gv.huixiangedu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jr.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kb.nicolike.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wv.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://be.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wd.9csxet.cn


<!-- 参考信息 -->