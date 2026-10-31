代发 wailian999

TS:   constructor(public name: string) {}
来源：http://li.asd995.cn

Java: User(String name) { this.name = name; }
来源：http://rc.9csxet.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://rn.jctech888.com.cn

Ruby: def initialize(name); @name = name; end
来源：http://xn.nszjky.cn

C#:   public User(string name) { Name = name; }
来源：http://qo.lnxyls.cn

[G03] 实例属性
来源：http://lo.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://jb.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://pg.jianghongdianzi.cn

JS:   this.name = "x";
来源：http://pr.shxzukj.cn

TS:   name: string = "x";
来源：http://py.szxytkj.cn

Java: private String name;
来源：http://nc.colortex.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xj.hnjuh.cn

Ruby: @name = "x"
来源：http://ns.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://fq.shxzukj.cn

[G04] 定义方法
来源：http://yc.lnxyls.cn

Py:   def greet(self): return self.name
来源：http://lz.jctech888.com.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wd.nszjky.cn

JS:   greet() { return this.name; }
来源：http://eg.szsharing.cn

TS:   greet(): string { return this.name; }
来源：http://oo.bjjhwx.cn

Java: String greet() { return name; }
来源：http://kj.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://px.yuntaijiaju.cn

Ruby: def greet; @name; end
来源：http://zm.lnxyls.cn

C#:   public string Greet() => Name;
来源：http://ax.haigaiapp.cn

[G05] 继承
来源：http://qk.bookmarksfly.cn

Py:   class Admin(User): pass
来源：http://ct.jianghongdianzi.cn

PHP:  class Admin extends User {}
来源：http://zb.szxytkj.cn

JS:   class Admin extends User {}
来源：http://uu.bjjhwx.cn

TS:   class Admin extends User {}
来源：http://cc.szxytkj.cn

Java: class Admin extends User {}
来源：http://yt.shxzukj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ca.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://wq.yuntaijiaju.cn

C#:   class Admin : User {}
来源：http://xt.jianghongdianzi.cn

[G06] 重写方法
来源：http://by.panjiajie.cn

Py:   def greet(self): return "admin"
来源：http://zy.hnjuh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jk.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://qo.szxytkj.cn

TS:   greet(): string { return "admin"; }
来源：http://yy.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://jj.shtwfgs.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://oo.haigaiapp.cn

Ruby: def greet; "admin"; end
来源：http://qk.yuexingan06.cn

C#:   public override string Greet() => "admin";
来源：http://mz.9csxet.cn

[G07] 调用父类方法
来源：http://ve.bookmarksfly.cn

Py:   super().greet()
来源：http://iw.huixiangedu.cn

PHP:  parent::greet();
来源：http://ni.huanxung.cn

JS:   super.greet();
来源：http://mo.jctech888.com.cn

TS:   super.greet();
来源：http://na.colortex.cn

Java: super.greet();
来源：http://be.panjiajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oz.colortex.cn

Ruby: super
来源：http://uo.szsharing.cn

C#:   base.Greet();
来源：http://yc.shxzskj.cn

[G08] 静态方法与属性
来源：http://ei.521024.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ow.yuexingan06.cn

PHP:  public static function f() {}
来源：http://tr.yuexingan06.cn

JS:   static f() {}
来源：http://gf.huixiangedu.cn

TS:   static f(): void {}
来源：http://wd.lnxyls.cn

Java: static void f() {}
来源：http://ea.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://oq.shxzukj.cn

Ruby: def self.f; end
来源：http://ot.hnjuh.cn

C#:   public static void F() {}
来源：http://by.shtwfgs.cn

[G09] 接口 / 抽象类
来源：http://pq.lnxyls.cn

Py:   from abc import ABC, abstractmethod
来源：http://ue.newstarts.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bd.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qk.chemitech.net.cn

TS:   interface Shape { area(): number; }
来源：http://sb.huixinmuqiang.cn

Java: interface Shape { double area(); }
来源：http://bd.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://on.colortex.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pp.huixiangedu.cn

C#:   interface IShape { double Area(); }
来源：http://ia.nszjky.cn

[G10] 访问控制
来源：http://ao.panjiajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://dr.colortex.cn

PHP:  public / protected / private
来源：http://zr.huanxung.cn

JS:   #private 字段；其余公开
来源：http://lf.asd995.cn

TS:   public / protected / private
来源：http://qt.521024.cn

Java: public / protected / private / 默认包级
来源：http://ic.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yj.panjiajie.cn

Ruby: public / protected / private
来源：http://cw.asd995.cn

C#:   public / protected / private / internal
来源：http://lq.yuntaijiaju.cn

[G11] getter / setter
来源：http://xf.gzmigu.cn

Py:   @property 与 @x.setter
来源：http://fg.newstarts.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ie.gzmigu.cn

JS:   get name() { return this._name; }
来源：http://fu.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://ls.yuntaijiaju.cn

Java: public String getName() { return name; }
来源：http://ve.jianghongdianzi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ze.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://cr.newstarts.cn

C#:   public string Name { get; set; }
来源：http://hr.yuexingan06.cn

[G12] 对象转字符串
来源：http://vb.jianghongdianzi.cn

Py:   def __str__(self): return self.name
来源：http://vi.nicolike.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://au.lnxyls.cn

JS:   toString() { return this.name; }
来源：http://lf.yuexingan06.cn

TS:   toString(): string { return this.name; }
来源：http://va.newstarts.cn

Java: @Override public String toString() { return name; }
来源：http://ju.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lj.bookmarksfly.cn

Ruby: def to_s; @name; end
来源：http://cg.shxzskj.cn

C#:   public override string ToString() => Name;
来源：http://mf.hnjuh.cn

[G13] 判断对象类型
来源：http://gi.huixinmuqiang.cn

Py:   isinstance(u, User)
来源：http://yw.shtwfgs.cn

PHP:  $u instanceof User
来源：http://tn.nszjky.cn

JS:   u instanceof User
来源：http://wy.colortex.cn

TS:   u instanceof User
来源：http://jq.shxzskj.cn

Java: u instanceof User
来源：http://af.bookmarksfly.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://af.bjjhwx.cn

Ruby: u.is_a?(User)
来源：http://kc.panjiajie.cn

C#:   u is User
来源：http://ws.huanxung.cn

[G14] 数据类 / record
来源：http://mt.wgjwhj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ty.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://gl.hahajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gn.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://rz.haigaiapp.cn

Java: record User(String name, int age) {}
来源：http://cs.yuexingan06.cn

Go:   type User struct { Name string; Age int }
来源：http://ao.bjjhwx.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://oz.521024.cn

C#:   record User(string Name, int Age);
来源：http://dc.huixinmuqiang.cn

[G15] 枚举
来源：http://dz.szsharing.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xw.wgjwhj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zn.newstarts.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fe.szxytkj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://is.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://ox.521024.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qy.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://xn.gzmigu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cx.nszjky.cn

[G16] 对象转数组 / 字典
来源：http://au.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dg.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://rt.haigaiapp.cn

JS:   Object.entries(obj)
来源：http://ru.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://pl.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wb.bjjhwx.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ns.521024.cn

Ruby: obj.instance_variables
来源：http://cv.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://vp.hahajie.cn

================================================================================
来源：http://gr.asd995.cn

H. 异常与错误处理
来源：http://nq.jianghongdianzi.cn

================================================================================
来源：http://oc.gzmigu.cn

[H01] try / catch 基础
来源：http://um.colortex.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zx.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jp.szsharing.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wo.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://us.521024.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ah.shxzukj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ed.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sv.yuexingan06.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pr.huixinmuqiang.cn

[H02] finally / ensure 收尾
来源：http://qp.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zf.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://un.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cm.nicolike.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://py.huanxung.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tt.asd995.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ti.shxzukj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://em.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://eg.nicolike.cn

[H03] 主动抛出异常
来源：http://hp.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://vn.hnjuh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tn.shtwfgs.cn

JS:   throw new Error("错误信息");
来源：http://yh.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://fy.nszjky.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://td.haigaiapp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ot.newstarts.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yr.newstarts.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ng.huanxung.cn

[H04] 自定义异常类型
来源：http://ja.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://bk.huixiangedu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jw.9csxet.cn

JS:   class MyError extends Error {}
来源：http://fv.szxytkj.cn

TS:   class MyError extends Error {}
来源：http://aj.bookmarksfly.cn

Java: class MyException extends RuntimeException {}
来源：http://aj.muxihuayi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ks.haigaiapp.cn

Ruby: class MyError < StandardError; end
来源：http://lw.bjjhwx.cn

C#:   class MyException : Exception {}
来源：http://ny.panjiajie.cn

[H05] 捕获特定类型
来源：http://ag.szxytkj.cn

Py:   except ValueError as e:
来源：http://jf.newstarts.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ar.shxzskj.cn

JS:   if (e instanceof TypeError) {}
来源：http://hv.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://og.panjiajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://ss.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pb.521024.cn

Ruby: rescue ArgumentError => e
来源：http://vf.muxihuayi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tw.shxzskj.cn

[H06] 可选值 / 空值安全访问
来源：http://oo.gzmigu.cn

Py:   value = d.get("k") or default
来源：http://jk.shxzukj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lj.hnjuh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lm.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tv.9csxet.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gr.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pv.bjjhwx.cn

Ruby: d&.dig(:a, :b)
来源：http://mn.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://vz.bookmarksfly.cn

[H07] 断言
来源：http://ac.521024.cn

Py:   assert x > 0, "必须为正"
来源：http://sm.panjiajie.cn

PHP:  assert($x > 0);
来源：http://gd.newstarts.cn

JS:   console.assert(x > 0);
来源：http://oc.panjiajie.cn

TS:   console.assert(x > 0);
来源：http://my.bookmarksfly.cn

Java: assert x > 0 : "必须为正";
来源：http://im.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ub.yuexingan06.cn

Ruby: raise "必须为正" unless x > 0
来源：http://po.jctech888.com.cn

C#:   Debug.Assert(x > 0);
来源：http://cs.colortex.cn

[H08] 获取错误信息与堆栈
来源：http://mm.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://fp.colortex.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oe.shxzskj.cn

JS:   e.message;  e.stack
来源：http://ij.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ld.szsharing.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cd.lnxyls.cn

Go:   err.Error()
来源：http://uu.shtwfgs.cn

Ruby: e.message;  e.backtrace
来源：http://gr.521024.cn

C#:   e.Message;  e.StackTrace
来源：http://ld.wgjwhj.cn

[H09] 带错误码的异常
来源：http://vf.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dx.nicolike.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rm.521024.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vn.wgjwhj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gf.huixiangedu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mf.shxzukj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yt.lnxyls.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rl.szsharing.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ul.521024.cn

[H10] 资源自动释放
来源：http://iw.nicolike.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sa.lnxyls.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://af.muxihuayi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xn.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fr.newstarts.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://es.colortex.cn

Go:   defer f.Close()
来源：http://ta.newstarts.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fr.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gs.hnjuh.cn

================================================================================
来源：http://uz.lnxyls.cn

I. 正则表达式
来源：http://lu.gzmigu.cn

================================================================================
来源：http://ru.muxihuayi.cn

[I01] 判断是否匹配
来源：http://im.szxytkj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yz.huixiangedu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gt.gzmigu.cn

JS:   /\d+/.test(s)
来源：http://zp.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://ut.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fj.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gs.szxytkj.cn

Ruby: s.match?(/\d+/)
来源：http://zb.wgjwhj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ht.huanxung.cn

[I02] 提取所有匹配
来源：http://wo.gzmigu.cn

Py:   re.findall(r"\d+", s)
来源：http://jt.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nv.chemitech.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://oq.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://it.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yf.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://om.muxihuayi.cn

Ruby: s.scan(/\d+/)
来源：http://nl.yuntaijiaju.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dd.yuexingan06.cn

[I03] 提取捕获分组
来源：http://fy.bookmarksfly.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://it.szxytkj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://tj.muxihuayi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pz.colortex.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vt.jctech888.com.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://br.shxzukj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dj.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bi.huanxung.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sl.jctech888.com.cn

[I04] 正则替换
来源：http://qd.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://je.asd995.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xs.haigaiapp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vy.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://il.asd995.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ib.hnjuh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hg.haigaiapp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ij.haigaiapp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mz.huanxung.cn

[I05] 按正则拆分
来源：http://og.huixinmuqiang.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zl.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://dd.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://rg.hnjuh.cn

TS:   s.split(/\s*,\s*/)
来源：http://sf.bjjhwx.cn

Java: s.split("\\s*,\\s*")
来源：http://xw.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mz.bjjhwx.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ft.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xp.shxzukj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xx.newstarts.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ky.shxzskj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fa.huixiangedu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nb.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ww.9csxet.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pq.nszjky.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ch.yuexingan06.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jd.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wv.521024.cn

[I07] 忽略大小写与多行模式
来源：http://jh.wgjwhj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mr.huixinmuqiang.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ip.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eq.asd995.cn

TS:   /error/gim
来源：http://hw.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xj.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qc.colortex.cn

Ruby: s.scan(/error/i)
来源：http://hq.521024.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://be.bookmarksfly.cn

[I08] 贪婪与非贪婪匹配
来源：http://qk.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://js.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ph.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yc.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://li.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ip.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wc.asd995.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zn.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fd.lnxyls.cn

================================================================================
来源：http://hz.bjjhwx.cn


<!-- 参考信息 -->