代发 wailian999

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ir.bookmarksfly.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kx.hnjuh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://rg.shxzskj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dq.huixiangedu.cn

================================================================================
来源：http://tp.jctech888.com.cn

G. 面向对象
来源：http://ca.9csxet.cn

================================================================================
来源：http://bv.bjjhwx.cn

[G01] 定义类
来源：http://my.nszjky.cn

Py:   class User: pass
来源：http://ba.nszjky.cn

PHP:  class User {}
来源：http://ir.shtwfgs.cn

JS:   class User {}
来源：http://um.hnjuh.cn

TS:   class User { name: string = ""; }
来源：http://ku.yuexingan06.cn

Java: class User {}
来源：http://px.hahajie.cn

Go:   type User struct { Name string }
来源：http://my.shxzskj.cn

Ruby: class User; end
来源：http://ur.yuexingan06.cn

C#:   class User {}
来源：http://np.newstarts.cn

[G02] 构造函数
来源：http://os.chemitech.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://ax.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://qu.lnxyls.cn

JS:   constructor(name) { this.name = name; }
来源：http://ln.nicolike.cn

TS:   constructor(public name: string) {}
来源：http://gs.szsharing.cn

Java: User(String name) { this.name = name; }
来源：http://lx.szsharing.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iu.bookmarksfly.cn

Ruby: def initialize(name); @name = name; end
来源：http://ub.haigaiapp.cn

C#:   public User(string name) { Name = name; }
来源：http://uc.yuntaijiaju.cn

[G03] 实例属性
来源：http://pn.hahajie.cn

Py:   self.name = "x"
来源：http://jr.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://yu.asd995.cn

JS:   this.name = "x";
来源：http://xh.gzmigu.cn

TS:   name: string = "x";
来源：http://dk.gzmigu.cn

Java: private String name;
来源：http://ae.9csxet.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://et.yuexingan06.cn

Ruby: @name = "x"
来源：http://al.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://hz.shxzukj.cn

[G04] 定义方法
来源：http://gk.shtwfgs.cn

Py:   def greet(self): return self.name
来源：http://kk.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bb.jctech888.com.cn

JS:   greet() { return this.name; }
来源：http://ub.lnxyls.cn

TS:   greet(): string { return this.name; }
来源：http://ux.gzmigu.cn

Java: String greet() { return name; }
来源：http://gw.lnxyls.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bh.bookmarksfly.cn

Ruby: def greet; @name; end
来源：http://ih.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://lo.asd995.cn

[G05] 继承
来源：http://sg.panjiajie.cn

Py:   class Admin(User): pass
来源：http://yf.nicolike.cn

PHP:  class Admin extends User {}
来源：http://sa.huixinmuqiang.cn

JS:   class Admin extends User {}
来源：http://vm.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://rq.wgjwhj.cn

Java: class Admin extends User {}
来源：http://fr.szxytkj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://em.panjiajie.cn

Ruby: class Admin < User; end
来源：http://st.asd995.cn

C#:   class Admin : User {}
来源：http://qb.asd995.cn

[G06] 重写方法
来源：http://pv.jianghongdianzi.cn

Py:   def greet(self): return "admin"
来源：http://us.bjjhwx.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yv.shtwfgs.cn

JS:   greet() { return "admin"; }
来源：http://nh.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://fx.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://dh.huanxung.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://se.shtwfgs.cn

Ruby: def greet; "admin"; end
来源：http://id.gzmigu.cn

C#:   public override string Greet() => "admin";
来源：http://yv.521024.cn

[G07] 调用父类方法
来源：http://em.nszjky.cn

Py:   super().greet()
来源：http://zt.hnjuh.cn

PHP:  parent::greet();
来源：http://te.shxzskj.cn

JS:   super.greet();
来源：http://gh.nszjky.cn

TS:   super.greet();
来源：http://js.shxzukj.cn

Java: super.greet();
来源：http://av.521024.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jg.haigaiapp.cn

Ruby: super
来源：http://de.bjjhwx.cn

C#:   base.Greet();
来源：http://ft.yuntaijiaju.cn

[G08] 静态方法与属性
来源：http://dp.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bq.nszjky.cn

PHP:  public static function f() {}
来源：http://pq.shxzskj.cn

JS:   static f() {}
来源：http://sx.hnjuh.cn

TS:   static f(): void {}
来源：http://zi.huixinmuqiang.cn

Java: static void f() {}
来源：http://qv.yuntaijiaju.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hl.huixinmuqiang.cn

Ruby: def self.f; end
来源：http://bz.szxytkj.cn

C#:   public static void F() {}
来源：http://vi.huixinmuqiang.cn

[G09] 接口 / 抽象类
来源：http://lc.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://fy.huixiangedu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xx.szsharing.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zs.521024.cn

TS:   interface Shape { area(): number; }
来源：http://kb.yuntaijiaju.cn

Java: interface Shape { double area(); }
来源：http://ue.huixinmuqiang.cn

Go:   type Shape interface { Area() float64 }
来源：http://gl.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zr.nszjky.cn

C#:   interface IShape { double Area(); }
来源：http://uo.huixinmuqiang.cn

[G10] 访问控制
来源：http://lx.huixiangedu.cn

Py:   约定 _protected / __private（不强制）
来源：http://nb.nicolike.cn

PHP:  public / protected / private
来源：http://pm.521024.cn

JS:   #private 字段；其余公开
来源：http://er.9csxet.cn

TS:   public / protected / private
来源：http://vj.asd995.cn

Java: public / protected / private / 默认包级
来源：http://zw.nicolike.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hg.nszjky.cn

Ruby: public / protected / private
来源：http://ir.huixiangedu.cn

C#:   public / protected / private / internal
来源：http://sr.521024.cn

[G11] getter / setter
来源：http://vg.521024.cn

Py:   @property 与 @x.setter
来源：http://jf.huanxung.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cj.nicolike.cn

JS:   get name() { return this._name; }
来源：http://gq.521024.cn

TS:   get name(): string { return this._name; }
来源：http://cz.hnjuh.cn

Java: public String getName() { return name; }
来源：http://rk.yuexingan06.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wg.bjjhwx.cn

Ruby: attr_accessor :name
来源：http://yj.newstarts.cn

C#:   public string Name { get; set; }
来源：http://ej.szxytkj.cn

[G12] 对象转字符串
来源：http://hg.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://mt.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://um.bookmarksfly.cn

JS:   toString() { return this.name; }
来源：http://pc.shxzukj.cn

TS:   toString(): string { return this.name; }
来源：http://yn.nszjky.cn

Java: @Override public String toString() { return name; }
来源：http://rt.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nu.szsharing.cn

Ruby: def to_s; @name; end
来源：http://ar.jctech888.com.cn

C#:   public override string ToString() => Name;
来源：http://ca.asd995.cn

[G13] 判断对象类型
来源：http://aw.muxihuayi.cn

Py:   isinstance(u, User)
来源：http://fo.bookmarksfly.cn

PHP:  $u instanceof User
来源：http://rg.szsharing.cn

JS:   u instanceof User
来源：http://ux.chemitech.net.cn

TS:   u instanceof User
来源：http://kb.newstarts.cn

Java: u instanceof User
来源：http://hr.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mz.huixinmuqiang.cn

Ruby: u.is_a?(User)
来源：http://be.asd995.cn

C#:   u is User
来源：http://ew.jianghongdianzi.cn

[G14] 数据类 / record
来源：http://qv.muxihuayi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cl.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://kx.szxytkj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://yp.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://sk.hnjuh.cn

Java: record User(String name, int age) {}
来源：http://yw.bjjhwx.cn

Go:   type User struct { Name string; Age int }
来源：http://qa.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pr.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://ip.wgjwhj.cn

[G15] 枚举
来源：http://ve.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://eb.shxzskj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wy.colortex.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nf.newstarts.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kz.haigaiapp.cn

Java: enum Color { RED, GREEN }
来源：http://tu.yuntaijiaju.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gr.szsharing.cn

Ruby: Color = %i[red green].freeze
来源：http://nn.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ow.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://ns.gzmigu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oq.hnjuh.cn

PHP:  get_object_vars($obj);
来源：http://mv.9csxet.cn

JS:   Object.entries(obj)
来源：http://ou.jianghongdianzi.cn

TS:   Object.entries(obj)
来源：http://uj.haigaiapp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cs.huixinmuqiang.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gd.newstarts.cn

Ruby: obj.instance_variables
来源：http://eg.hnjuh.cn

C#:   // 用反射或 System.Text.Json
来源：http://zk.nicolike.cn

================================================================================
来源：http://ar.huixinmuqiang.cn

H. 异常与错误处理
来源：http://rn.nicolike.cn

================================================================================
来源：http://zf.jctech888.com.cn

[H01] try / catch 基础
来源：http://uf.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ma.jianghongdianzi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kf.chemitech.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ok.shxzukj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hc.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://st.huixiangedu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nv.szsharing.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gx.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nu.nszjky.cn

[H02] finally / ensure 收尾
来源：http://hy.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zr.asd995.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vf.jctech888.com.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dy.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ot.muxihuayi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fp.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gb.nszjky.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://jt.shxzukj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fk.haigaiapp.cn

[H03] 主动抛出异常
来源：http://fs.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://hf.nszjky.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ri.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://wy.chemitech.net.cn

TS:   throw new Error("错误信息");
来源：http://el.yuexingan06.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rl.wgjwhj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ot.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lu.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://sc.muxihuayi.cn

[H04] 自定义异常类型
来源：http://ee.muxihuayi.cn

Py:   class MyError(Exception): pass
来源：http://xh.huixinmuqiang.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jn.lnxyls.cn

JS:   class MyError extends Error {}
来源：http://gh.huanxung.cn

TS:   class MyError extends Error {}
来源：http://cb.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://nq.521024.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hi.szxytkj.cn

Ruby: class MyError < StandardError; end
来源：http://nk.9csxet.cn

C#:   class MyException : Exception {}
来源：http://xw.shxzskj.cn

[H05] 捕获特定类型
来源：http://dt.jianghongdianzi.cn

Py:   except ValueError as e:
来源：http://ua.9csxet.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://di.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://cw.wgjwhj.cn

TS:   if (e instanceof TypeError) {}
来源：http://vs.haigaiapp.cn

Java: catch (IOException | SQLException e) {}
来源：http://cs.yuntaijiaju.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ab.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://er.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ph.huixinmuqiang.cn

[H06] 可选值 / 空值安全访问
来源：http://lj.yuexingan06.cn

Py:   value = d.get("k") or default
来源：http://al.szxytkj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sg.panjiajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ta.panjiajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://eu.haigaiapp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://du.shtwfgs.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://in.chemitech.net.cn

Ruby: d&.dig(:a, :b)
来源：http://kt.chemitech.net.cn

C#:   obj?.A?.B ?? default
来源：http://jh.shxzukj.cn

[H07] 断言
来源：http://gv.9csxet.cn

Py:   assert x > 0, "必须为正"
来源：http://js.huixiangedu.cn

PHP:  assert($x > 0);
来源：http://zu.nicolike.cn

JS:   console.assert(x > 0);
来源：http://bm.gzmigu.cn

TS:   console.assert(x > 0);
来源：http://bc.shxzukj.cn

Java: assert x > 0 : "必须为正";
来源：http://zq.wgjwhj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uj.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ax.bjjhwx.cn

C#:   Debug.Assert(x > 0);
来源：http://xv.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://zn.huixiangedu.cn

Py:   str(e);  traceback.format_exc()
来源：http://ny.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://it.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://ql.szxytkj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ac.shxzskj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dt.hnjuh.cn

Go:   err.Error()
来源：http://hj.colortex.cn

Ruby: e.message;  e.backtrace
来源：http://py.newstarts.cn

C#:   e.Message;  e.StackTrace
来源：http://yn.panjiajie.cn

[H09] 带错误码的异常
来源：http://zj.shxzukj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://go.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://in.jctech888.com.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ou.panjiajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hl.bjjhwx.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mm.521024.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ez.shtwfgs.cn

Ruby: raise MyError.new("fail", 500)
来源：http://we.szsharing.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xs.haigaiapp.cn

[H10] 资源自动释放
来源：http://zl.shtwfgs.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gs.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xq.yuexingan06.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mm.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dt.szsharing.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rd.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://qq.chemitech.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://oi.gzmigu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gd.lnxyls.cn

================================================================================
来源：http://xq.huixiangedu.cn

I. 正则表达式
来源：http://dv.nszjky.cn

================================================================================
来源：http://if.newstarts.cn

[I01] 判断是否匹配
来源：http://rn.colortex.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cz.lnxyls.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tb.gzmigu.cn

JS:   /\d+/.test(s)
来源：http://gp.chemitech.net.cn

TS:   /\d+/.test(s)
来源：http://wa.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rw.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://li.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://mu.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ah.shtwfgs.cn

[I02] 提取所有匹配
来源：http://ik.panjiajie.cn

Py:   re.findall(r"\d+", s)
来源：http://cw.szxytkj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lh.wgjwhj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://en.yuexingan06.cn

TS:   s.match(/\d+/g)
来源：http://qp.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nc.hahajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tc.shtwfgs.cn

Ruby: s.scan(/\d+/)
来源：http://db.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ca.jianghongdianzi.cn

[I03] 提取捕获分组
来源：http://jz.hahajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://pi.wgjwhj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uu.colortex.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://aa.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dp.szsharing.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zy.szxytkj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ve.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lh.bjjhwx.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dn.szsharing.cn

[I04] 正则替换
来源：http://jx.chemitech.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fo.wgjwhj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wz.huanxung.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fs.bookmarksfly.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yq.szsharing.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nc.gzmigu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ft.wgjwhj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://th.huanxung.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yz.bookmarksfly.cn

[I05] 按正则拆分
来源：http://jp.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://py.shxzskj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://od.lnxyls.cn

JS:   s.split(/\s*,\s*/)
来源：http://wx.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://yh.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://me.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ub.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rv.szsharing.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://nu.szsharing.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://no.chemitech.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ic.szsharing.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pf.gzmigu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zk.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uo.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tj.newstarts.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cc.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vb.yuntaijiaju.cn


<!-- 参考信息 -->