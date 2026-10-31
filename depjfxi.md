代发 wailian999

Java: class User {}
来源：http://lk.gzmigu.cn

Go:   type User struct { Name string }
来源：http://ip.bookmarksfly.cn

Ruby: class User; end
来源：http://fv.lnxyls.cn

C#:   class User {}
来源：http://ps.asd995.cn

[G02] 构造函数
来源：http://fu.chemitech.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://ut.jianghongdianzi.cn

PHP:  public function __construct(public string $name) {}
来源：http://oh.wgjwhj.cn

JS:   constructor(name) { this.name = name; }
来源：http://qz.shxzskj.cn

TS:   constructor(public name: string) {}
来源：http://kz.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://ne.szsharing.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://me.asd995.cn

Ruby: def initialize(name); @name = name; end
来源：http://jj.jianghongdianzi.cn

C#:   public User(string name) { Name = name; }
来源：http://vz.hahajie.cn

[G03] 实例属性
来源：http://sl.shtwfgs.cn

Py:   self.name = "x"
来源：http://fp.huixinmuqiang.cn

PHP:  public string $name = "x";
来源：http://zi.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://az.bjjhwx.cn

TS:   name: string = "x";
来源：http://tk.shxzukj.cn

Java: private String name;
来源：http://iu.9csxet.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://md.jianghongdianzi.cn

Ruby: @name = "x"
来源：http://jq.lnxyls.cn

C#:   public string Name { get; set; } = "x";
来源：http://qb.szxytkj.cn

[G04] 定义方法
来源：http://jx.yuexingan06.cn

Py:   def greet(self): return self.name
来源：http://ps.jianghongdianzi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ri.lnxyls.cn

JS:   greet() { return this.name; }
来源：http://cs.colortex.cn

TS:   greet(): string { return this.name; }
来源：http://mq.hahajie.cn

Java: String greet() { return name; }
来源：http://av.yuntaijiaju.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hn.shxzukj.cn

Ruby: def greet; @name; end
来源：http://uj.bookmarksfly.cn

C#:   public string Greet() => Name;
来源：http://vl.bookmarksfly.cn

[G05] 继承
来源：http://lu.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://jv.panjiajie.cn

PHP:  class Admin extends User {}
来源：http://tb.haigaiapp.cn

JS:   class Admin extends User {}
来源：http://fh.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://wj.huixiangedu.cn

Java: class Admin extends User {}
来源：http://sx.muxihuayi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://po.huixiangedu.cn

Ruby: class Admin < User; end
来源：http://at.colortex.cn

C#:   class Admin : User {}
来源：http://ed.yuntaijiaju.cn

[G06] 重写方法
来源：http://ok.lnxyls.cn

Py:   def greet(self): return "admin"
来源：http://xp.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://af.haigaiapp.cn

JS:   greet() { return "admin"; }
来源：http://va.shxzskj.cn

TS:   greet(): string { return "admin"; }
来源：http://xk.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://ai.nicolike.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://sc.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://mq.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://fr.hnjuh.cn

[G07] 调用父类方法
来源：http://ih.hahajie.cn

Py:   super().greet()
来源：http://jh.521024.cn

PHP:  parent::greet();
来源：http://rn.bjjhwx.cn

JS:   super.greet();
来源：http://pg.lnxyls.cn

TS:   super.greet();
来源：http://yz.haigaiapp.cn

Java: super.greet();
来源：http://gj.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mb.nszjky.cn

Ruby: super
来源：http://hm.yuexingan06.cn

C#:   base.Greet();
来源：http://ed.nicolike.cn

[G08] 静态方法与属性
来源：http://qg.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qg.bjjhwx.cn

PHP:  public static function f() {}
来源：http://fa.nszjky.cn

JS:   static f() {}
来源：http://kp.yuexingan06.cn

TS:   static f(): void {}
来源：http://xj.chemitech.net.cn

Java: static void f() {}
来源：http://xy.jianghongdianzi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mc.jctech888.com.cn

Ruby: def self.f; end
来源：http://ls.bjjhwx.cn

C#:   public static void F() {}
来源：http://ss.jctech888.com.cn

[G09] 接口 / 抽象类
来源：http://jo.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://sa.nicolike.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zd.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://yu.shxzukj.cn

TS:   interface Shape { area(): number; }
来源：http://rw.yuntaijiaju.cn

Java: interface Shape { double area(); }
来源：http://dp.9csxet.cn

Go:   type Shape interface { Area() float64 }
来源：http://rw.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://se.nszjky.cn

C#:   interface IShape { double Area(); }
来源：http://zg.yuntaijiaju.cn

[G10] 访问控制
来源：http://cj.huanxung.cn

Py:   约定 _protected / __private（不强制）
来源：http://py.huixiangedu.cn

PHP:  public / protected / private
来源：http://xg.muxihuayi.cn

JS:   #private 字段；其余公开
来源：http://qi.nicolike.cn

TS:   public / protected / private
来源：http://nd.wgjwhj.cn

Java: public / protected / private / 默认包级
来源：http://yl.colortex.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ry.bjjhwx.cn

Ruby: public / protected / private
来源：http://af.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://lg.szsharing.cn

[G11] getter / setter
来源：http://gd.shxzukj.cn

Py:   @property 与 @x.setter
来源：http://jm.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yc.panjiajie.cn

JS:   get name() { return this._name; }
来源：http://fp.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://cv.shxzukj.cn

Java: public String getName() { return name; }
来源：http://kj.newstarts.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nb.szxytkj.cn

Ruby: attr_accessor :name
来源：http://rs.chemitech.net.cn

C#:   public string Name { get; set; }
来源：http://ef.huanxung.cn

[G12] 对象转字符串
来源：http://ep.muxihuayi.cn

Py:   def __str__(self): return self.name
来源：http://wb.haigaiapp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fk.huixiangedu.cn

JS:   toString() { return this.name; }
来源：http://cx.yuntaijiaju.cn

TS:   toString(): string { return this.name; }
来源：http://zq.huixiangedu.cn

Java: @Override public String toString() { return name; }
来源：http://xc.szxytkj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ga.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://at.panjiajie.cn

C#:   public override string ToString() => Name;
来源：http://lm.bjjhwx.cn

[G13] 判断对象类型
来源：http://qh.colortex.cn

Py:   isinstance(u, User)
来源：http://bx.newstarts.cn

PHP:  $u instanceof User
来源：http://xn.gzmigu.cn

JS:   u instanceof User
来源：http://od.szxytkj.cn

TS:   u instanceof User
来源：http://mq.wgjwhj.cn

Java: u instanceof User
来源：http://dg.huanxung.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sw.shxzukj.cn

Ruby: u.is_a?(User)
来源：http://ax.colortex.cn

C#:   u is User
来源：http://sh.muxihuayi.cn

[G14] 数据类 / record
来源：http://li.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nt.huixiangedu.cn

PHP:  // 用 readonly 属性模拟
来源：http://wb.jianghongdianzi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gu.haigaiapp.cn

TS:   type User = { name: string; age: number };
来源：http://sc.lnxyls.cn

Java: record User(String name, int age) {}
来源：http://xz.wgjwhj.cn

Go:   type User struct { Name string; Age int }
来源：http://rd.bookmarksfly.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kl.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://df.jianghongdianzi.cn

[G15] 枚举
来源：http://lo.shtwfgs.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gl.wgjwhj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nq.shtwfgs.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xs.jctech888.com.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wa.szsharing.cn

Java: enum Color { RED, GREEN }
来源：http://wm.521024.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tg.bjjhwx.cn

Ruby: Color = %i[red green].freeze
来源：http://gz.newstarts.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ua.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://oj.yuntaijiaju.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://to.asd995.cn

PHP:  get_object_vars($obj);
来源：http://hc.shxzskj.cn

JS:   Object.entries(obj)
来源：http://mp.9csxet.cn

TS:   Object.entries(obj)
来源：http://du.521024.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ph.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ld.asd995.cn

Ruby: obj.instance_variables
来源：http://fy.wgjwhj.cn

C#:   // 用反射或 System.Text.Json
来源：http://gw.jianghongdianzi.cn

================================================================================
来源：http://ou.shxzskj.cn

H. 异常与错误处理
来源：http://dm.lnxyls.cn

================================================================================
来源：http://ja.yuexingan06.cn

[H01] try / catch 基础
来源：http://mh.huixiangedu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://si.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ch.nszjky.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://eq.jctech888.com.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kh.colortex.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tw.colortex.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gd.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zf.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lv.asd995.cn

[H02] finally / ensure 收尾
来源：http://gq.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://la.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vv.521024.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ig.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qd.jctech888.com.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tc.hahajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lu.nszjky.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ax.chemitech.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jb.lnxyls.cn

[H03] 主动抛出异常
来源：http://zh.shtwfgs.cn

Py:   raise ValueError("错误信息")
来源：http://pt.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qq.huixiangedu.cn

JS:   throw new Error("错误信息");
来源：http://mv.bjjhwx.cn

TS:   throw new Error("错误信息");
来源：http://xb.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tj.wgjwhj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ay.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nk.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ux.hnjuh.cn

[H04] 自定义异常类型
来源：http://dd.hnjuh.cn

Py:   class MyError(Exception): pass
来源：http://un.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kx.shxzukj.cn

JS:   class MyError extends Error {}
来源：http://hb.colortex.cn

TS:   class MyError extends Error {}
来源：http://qd.panjiajie.cn

Java: class MyException extends RuntimeException {}
来源：http://hx.jianghongdianzi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ob.wgjwhj.cn

Ruby: class MyError < StandardError; end
来源：http://fc.haigaiapp.cn

C#:   class MyException : Exception {}
来源：http://ll.9csxet.cn

[H05] 捕获特定类型
来源：http://gp.nszjky.cn

Py:   except ValueError as e:
来源：http://if.huixinmuqiang.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jx.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://xd.nicolike.cn

TS:   if (e instanceof TypeError) {}
来源：http://zn.colortex.cn

Java: catch (IOException | SQLException e) {}
来源：http://kg.wgjwhj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://by.huanxung.cn

Ruby: rescue ArgumentError => e
来源：http://lf.huixinmuqiang.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lv.yuexingan06.cn

[H06] 可选值 / 空值安全访问
来源：http://th.newstarts.cn

Py:   value = d.get("k") or default
来源：http://py.newstarts.cn

PHP:  $v = $d["k"] ?? null;
来源：http://od.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hc.haigaiapp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jt.wgjwhj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fe.nszjky.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qi.huixinmuqiang.cn

Ruby: d&.dig(:a, :b)
来源：http://ky.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://zy.colortex.cn

[H07] 断言
来源：http://ac.muxihuayi.cn

Py:   assert x > 0, "必须为正"
来源：http://ov.wgjwhj.cn

PHP:  assert($x > 0);
来源：http://yk.yuntaijiaju.cn

JS:   console.assert(x > 0);
来源：http://fk.asd995.cn

TS:   console.assert(x > 0);
来源：http://gh.jianghongdianzi.cn

Java: assert x > 0 : "必须为正";
来源：http://rm.hnjuh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://uq.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fo.gzmigu.cn

C#:   Debug.Assert(x > 0);
来源：http://fd.haigaiapp.cn

[H08] 获取错误信息与堆栈
来源：http://sy.newstarts.cn

Py:   str(e);  traceback.format_exc()
来源：http://sp.huixinmuqiang.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xo.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://su.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ed.hnjuh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nu.9csxet.cn

Go:   err.Error()
来源：http://gh.haigaiapp.cn

Ruby: e.message;  e.backtrace
来源：http://aj.newstarts.cn

C#:   e.Message;  e.StackTrace
来源：http://kx.hnjuh.cn

[H09] 带错误码的异常
来源：http://vi.panjiajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sw.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xt.nicolike.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zb.hahajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bi.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ey.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wl.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lp.shxzskj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fh.hahajie.cn

[H10] 资源自动释放
来源：http://to.jianghongdianzi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vp.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kh.gzmigu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gv.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jp.yuntaijiaju.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lf.bjjhwx.cn

Go:   defer f.Close()
来源：http://jj.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vv.szxytkj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oa.newstarts.cn

================================================================================
来源：http://pj.hahajie.cn

I. 正则表达式
来源：http://xd.lnxyls.cn

================================================================================
来源：http://ng.huanxung.cn

[I01] 判断是否匹配
来源：http://vh.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qa.szxytkj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://em.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://yq.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://fd.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sg.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vh.yuexingan06.cn

Ruby: s.match?(/\d+/)
来源：http://xf.lnxyls.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://py.hnjuh.cn

[I02] 提取所有匹配
来源：http://ug.asd995.cn

Py:   re.findall(r"\d+", s)
来源：http://hp.szsharing.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ov.huanxung.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cm.haigaiapp.cn

TS:   s.match(/\d+/g)
来源：http://el.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ie.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gf.panjiajie.cn

Ruby: s.scan(/\d+/)
来源：http://pn.haigaiapp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ie.hnjuh.cn

[I03] 提取捕获分组
来源：http://pg.nszjky.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mq.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wk.gzmigu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ku.hahajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rd.newstarts.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ur.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ul.huixiangedu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tp.yuexingan06.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bs.muxihuayi.cn

[I04] 正则替换
来源：http://zq.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://tu.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dk.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fy.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mg.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vx.jctech888.com.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://au.521024.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xo.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rm.huixinmuqiang.cn

[I05] 按正则拆分
来源：http://os.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dh.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pd.shxzskj.cn

JS:   s.split(/\s*,\s*/)
来源：http://xn.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://am.szxytkj.cn

Java: s.split("\\s*,\\s*")
来源：http://df.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vu.shxzskj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qr.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lc.shxzskj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ts.shtwfgs.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pm.bookmarksfly.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fd.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nt.521024.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://th.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xo.nszjky.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zw.szxytkj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bw.jianghongdianzi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fd.yuntaijiaju.cn

[I07] 忽略大小写与多行模式
来源：http://gj.nicolike.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://el.bjjhwx.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dy.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rc.colortex.cn

TS:   /error/gim
来源：http://lp.shxzskj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mi.9csxet.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://se.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://vm.asd995.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rk.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://pk.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ko.szsharing.cn


<!-- 参考信息 -->