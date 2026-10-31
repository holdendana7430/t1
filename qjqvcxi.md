代发 wailian999

TS:   constructor(public name: string) {}
来源：http://rx.yuntaijiaju.cn

Java: User(String name) { this.name = name; }
来源：http://xy.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://bj.yuexingan06.cn

Ruby: def initialize(name); @name = name; end
来源：http://tt.shxzukj.cn

C#:   public User(string name) { Name = name; }
来源：http://ck.asd995.cn

[G03] 实例属性
来源：http://vf.huixinmuqiang.cn

Py:   self.name = "x"
来源：http://lp.jianghongdianzi.cn

PHP:  public string $name = "x";
来源：http://kx.jctech888.com.cn

JS:   this.name = "x";
来源：http://ff.huanxung.cn

TS:   name: string = "x";
来源：http://mz.521024.cn

Java: private String name;
来源：http://wv.szxytkj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nz.huanxung.cn

Ruby: @name = "x"
来源：http://le.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://vx.nicolike.cn

[G04] 定义方法
来源：http://iz.newstarts.cn

Py:   def greet(self): return self.name
来源：http://kx.jctech888.com.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://kb.jctech888.com.cn

JS:   greet() { return this.name; }
来源：http://cd.huixiangedu.cn

TS:   greet(): string { return this.name; }
来源：http://pi.yuntaijiaju.cn

Java: String greet() { return name; }
来源：http://ib.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vz.chemitech.net.cn

Ruby: def greet; @name; end
来源：http://up.huanxung.cn

C#:   public string Greet() => Name;
来源：http://fd.lnxyls.cn

[G05] 继承
来源：http://ls.9csxet.cn

Py:   class Admin(User): pass
来源：http://pp.yuntaijiaju.cn

PHP:  class Admin extends User {}
来源：http://li.huixinmuqiang.cn

JS:   class Admin extends User {}
来源：http://cf.521024.cn

TS:   class Admin extends User {}
来源：http://ny.yuexingan06.cn

Java: class Admin extends User {}
来源：http://qg.lnxyls.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bv.haigaiapp.cn

Ruby: class Admin < User; end
来源：http://qw.huanxung.cn

C#:   class Admin : User {}
来源：http://qp.asd995.cn

[G06] 重写方法
来源：http://pe.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://zl.huixinmuqiang.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xh.hnjuh.cn

JS:   greet() { return "admin"; }
来源：http://am.shxzukj.cn

TS:   greet(): string { return "admin"; }
来源：http://vk.521024.cn

Java: @Override String greet() { return "admin"; }
来源：http://qt.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://or.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://nh.chemitech.net.cn

C#:   public override string Greet() => "admin";
来源：http://ug.huixinmuqiang.cn

[G07] 调用父类方法
来源：http://bs.yuexingan06.cn

Py:   super().greet()
来源：http://qi.colortex.cn

PHP:  parent::greet();
来源：http://tk.shxzskj.cn

JS:   super.greet();
来源：http://dj.yuexingan06.cn

TS:   super.greet();
来源：http://nq.521024.cn

Java: super.greet();
来源：http://vr.lnxyls.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mz.huanxung.cn

Ruby: super
来源：http://os.newstarts.cn

C#:   base.Greet();
来源：http://su.hahajie.cn

[G08] 静态方法与属性
来源：http://og.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gd.shtwfgs.cn

PHP:  public static function f() {}
来源：http://fz.521024.cn

JS:   static f() {}
来源：http://hk.muxihuayi.cn

TS:   static f(): void {}
来源：http://zx.bookmarksfly.cn

Java: static void f() {}
来源：http://hc.gzmigu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hu.huixiangedu.cn

Ruby: def self.f; end
来源：http://mr.jctech888.com.cn

C#:   public static void F() {}
来源：http://cv.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://km.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://vp.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ld.9csxet.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zv.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://fy.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://ar.jianghongdianzi.cn

Go:   type Shape interface { Area() float64 }
来源：http://au.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ph.shtwfgs.cn

C#:   interface IShape { double Area(); }
来源：http://sk.huixinmuqiang.cn

[G10] 访问控制
来源：http://ni.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://uf.gzmigu.cn

PHP:  public / protected / private
来源：http://se.shxzukj.cn

JS:   #private 字段；其余公开
来源：http://tj.huixiangedu.cn

TS:   public / protected / private
来源：http://vd.asd995.cn

Java: public / protected / private / 默认包级
来源：http://sm.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sq.jctech888.com.cn

Ruby: public / protected / private
来源：http://be.shtwfgs.cn

C#:   public / protected / private / internal
来源：http://hx.shtwfgs.cn

[G11] getter / setter
来源：http://ld.szxytkj.cn

Py:   @property 与 @x.setter
来源：http://mk.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ve.huixinmuqiang.cn

JS:   get name() { return this._name; }
来源：http://ed.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://nz.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://yo.hahajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kv.lnxyls.cn

Ruby: attr_accessor :name
来源：http://fa.gzmigu.cn

C#:   public string Name { get; set; }
来源：http://ui.lnxyls.cn

[G12] 对象转字符串
来源：http://so.huixinmuqiang.cn

Py:   def __str__(self): return self.name
来源：http://py.shtwfgs.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rt.521024.cn

JS:   toString() { return this.name; }
来源：http://hm.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://lt.muxihuayi.cn

Java: @Override public String toString() { return name; }
来源：http://nj.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hy.shxzukj.cn

Ruby: def to_s; @name; end
来源：http://am.nicolike.cn

C#:   public override string ToString() => Name;
来源：http://jf.bookmarksfly.cn

[G13] 判断对象类型
来源：http://zu.szsharing.cn

Py:   isinstance(u, User)
来源：http://sr.shxzukj.cn

PHP:  $u instanceof User
来源：http://zr.chemitech.net.cn

JS:   u instanceof User
来源：http://ws.lnxyls.cn

TS:   u instanceof User
来源：http://hp.muxihuayi.cn

Java: u instanceof User
来源：http://oy.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cg.panjiajie.cn

Ruby: u.is_a?(User)
来源：http://ak.yuexingan06.cn

C#:   u is User
来源：http://qc.newstarts.cn

[G14] 数据类 / record
来源：http://va.wgjwhj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://zr.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://ov.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wk.lnxyls.cn

TS:   type User = { name: string; age: number };
来源：http://rv.huixiangedu.cn

Java: record User(String name, int age) {}
来源：http://yg.huanxung.cn

Go:   type User struct { Name string; Age int }
来源：http://jz.haigaiapp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ic.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://hq.jctech888.com.cn

[G15] 枚举
来源：http://gj.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ge.nicolike.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://il.chemitech.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jy.hnjuh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jr.shxzukj.cn

Java: enum Color { RED, GREEN }
来源：http://js.gzmigu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jy.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://kb.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wa.521024.cn

[G16] 对象转数组 / 字典
来源：http://oo.bjjhwx.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rp.colortex.cn

PHP:  get_object_vars($obj);
来源：http://wk.hnjuh.cn

JS:   Object.entries(obj)
来源：http://rs.panjiajie.cn

TS:   Object.entries(obj)
来源：http://cv.lnxyls.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dh.bjjhwx.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://te.nszjky.cn

Ruby: obj.instance_variables
来源：http://by.lnxyls.cn

C#:   // 用反射或 System.Text.Json
来源：http://wc.shtwfgs.cn

================================================================================
来源：http://of.szxytkj.cn

H. 异常与错误处理
来源：http://dp.nszjky.cn

================================================================================
来源：http://gk.panjiajie.cn

[H01] try / catch 基础
来源：http://qs.jianghongdianzi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zf.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wn.shxzskj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vr.bookmarksfly.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ks.521024.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yi.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gv.gzmigu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ji.huanxung.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dc.chemitech.net.cn

[H02] finally / ensure 收尾
来源：http://vv.nszjky.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dx.colortex.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ih.521024.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xh.bjjhwx.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bb.nicolike.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ny.asd995.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ih.szxytkj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yf.shxzskj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rr.huixinmuqiang.cn

[H03] 主动抛出异常
来源：http://xj.nicolike.cn

Py:   raise ValueError("错误信息")
来源：http://su.yuexingan06.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ep.shxzukj.cn

JS:   throw new Error("错误信息");
来源：http://er.muxihuayi.cn

TS:   throw new Error("错误信息");
来源：http://ow.shxzskj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bp.asd995.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pc.newstarts.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xu.bookmarksfly.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wb.lnxyls.cn

[H04] 自定义异常类型
来源：http://zz.nicolike.cn

Py:   class MyError(Exception): pass
来源：http://sf.huixiangedu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xs.muxihuayi.cn

JS:   class MyError extends Error {}
来源：http://cu.gzmigu.cn

TS:   class MyError extends Error {}
来源：http://ve.jianghongdianzi.cn

Java: class MyException extends RuntimeException {}
来源：http://il.muxihuayi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ih.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://vi.haigaiapp.cn

C#:   class MyException : Exception {}
来源：http://zd.hahajie.cn

[H05] 捕获特定类型
来源：http://by.huixinmuqiang.cn

Py:   except ValueError as e:
来源：http://az.shxzukj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eg.szxytkj.cn

JS:   if (e instanceof TypeError) {}
来源：http://hh.huixiangedu.cn

TS:   if (e instanceof TypeError) {}
来源：http://rb.huixiangedu.cn

Java: catch (IOException | SQLException e) {}
来源：http://hn.jctech888.com.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ou.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://lp.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fr.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://cw.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://di.bookmarksfly.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ob.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vj.huanxung.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jf.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xf.chemitech.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ee.shtwfgs.cn

Ruby: d&.dig(:a, :b)
来源：http://kg.shxzukj.cn

C#:   obj?.A?.B ?? default
来源：http://oi.huanxung.cn

[H07] 断言
来源：http://ic.gzmigu.cn

Py:   assert x > 0, "必须为正"
来源：http://sq.panjiajie.cn

PHP:  assert($x > 0);
来源：http://nk.szsharing.cn

JS:   console.assert(x > 0);
来源：http://pj.hnjuh.cn

TS:   console.assert(x > 0);
来源：http://gt.huanxung.cn

Java: assert x > 0 : "必须为正";
来源：http://gn.haigaiapp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ko.521024.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ya.shxzukj.cn

C#:   Debug.Assert(x > 0);
来源：http://ih.szxytkj.cn

[H08] 获取错误信息与堆栈
来源：http://yf.9csxet.cn

Py:   str(e);  traceback.format_exc()
来源：http://ku.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://js.nszjky.cn

JS:   e.message;  e.stack
来源：http://ju.wgjwhj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vg.nszjky.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rx.bjjhwx.cn

Go:   err.Error()
来源：http://ls.jctech888.com.cn

Ruby: e.message;  e.backtrace
来源：http://ql.bjjhwx.cn

C#:   e.Message;  e.StackTrace
来源：http://bd.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://kw.colortex.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pd.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ay.shxzskj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lc.muxihuayi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zm.nicolike.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gl.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jo.yuntaijiaju.cn

Ruby: raise MyError.new("fail", 500)
来源：http://me.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wj.asd995.cn

[H10] 资源自动释放
来源：http://rc.muxihuayi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xi.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qc.huixinmuqiang.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://af.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://du.newstarts.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vg.nicolike.cn

Go:   defer f.Close()
来源：http://ae.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nn.yuntaijiaju.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hy.wgjwhj.cn

================================================================================
来源：http://fg.newstarts.cn

I. 正则表达式
来源：http://rs.szxytkj.cn

================================================================================
来源：http://ba.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://wd.jianghongdianzi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://iz.szxytkj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fe.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://ma.szsharing.cn

TS:   /\d+/.test(s)
来源：http://nw.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://mm.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://tr.yuexingan06.cn

Ruby: s.match?(/\d+/)
来源：http://nt.shxzskj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mk.hnjuh.cn

[I02] 提取所有匹配
来源：http://jg.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://qz.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://px.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fk.haigaiapp.cn

TS:   s.match(/\d+/g)
来源：http://ul.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cn.9csxet.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zx.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://yf.muxihuayi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nl.hahajie.cn

[I03] 提取捕获分组
来源：http://sl.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ro.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lx.haigaiapp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qw.huanxung.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uf.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xs.newstarts.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bd.newstarts.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://io.huixiangedu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bm.yuntaijiaju.cn

[I04] 正则替换
来源：http://ov.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ht.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eb.shxzskj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zs.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sw.521024.cn

Java: s.replaceAll("\\d+", "#")
来源：http://su.bjjhwx.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ib.gzmigu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://na.panjiajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://di.521024.cn

[I05] 按正则拆分
来源：http://ii.yuexingan06.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ny.521024.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yk.bookmarksfly.cn

JS:   s.split(/\s*,\s*/)
来源：http://ik.shtwfgs.cn

TS:   s.split(/\s*,\s*/)
来源：http://pc.huixiangedu.cn

Java: s.split("\\s*,\\s*")
来源：http://bc.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hq.yuntaijiaju.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ra.yuntaijiaju.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vx.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tf.chemitech.net.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kl.hnjuh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jl.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://io.huixinmuqiang.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://to.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zr.nszjky.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fr.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://md.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cn.huanxung.cn

[I07] 忽略大小写与多行模式
来源：http://ma.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lo.wgjwhj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ky.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ot.chemitech.net.cn

TS:   /error/gim
来源：http://xf.hahajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ny.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zt.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://rs.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://eb.panjiajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://ep.521024.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zf.hahajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bf.jianghongdianzi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ot.panjiajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xd.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bh.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gb.asd995.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gk.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gn.shtwfgs.cn

================================================================================
来源：http://mc.521024.cn


<!-- 参考信息 -->