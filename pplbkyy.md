代发 wailian999

Java: class User {}
来源：http://hn.shxzskj.cn

Go:   type User struct { Name string }
来源：http://bv.yuntaijiaju.cn

Ruby: class User; end
来源：http://nb.panjiajie.cn

C#:   class User {}
来源：http://qk.hahajie.cn

[G02] 构造函数
来源：http://zv.yuexingan06.cn

Py:   def __init__(self, name): self.name = name
来源：http://vx.lnxyls.cn

PHP:  public function __construct(public string $name) {}
来源：http://pk.hahajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://lt.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://sl.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://cu.huanxung.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ub.nszjky.cn

Ruby: def initialize(name); @name = name; end
来源：http://zq.jctech888.com.cn

C#:   public User(string name) { Name = name; }
来源：http://kl.huixinmuqiang.cn

[G03] 实例属性
来源：http://hy.szxytkj.cn

Py:   self.name = "x"
来源：http://jz.colortex.cn

PHP:  public string $name = "x";
来源：http://ev.lnxyls.cn

JS:   this.name = "x";
来源：http://qf.chemitech.net.cn

TS:   name: string = "x";
来源：http://pe.huixiangedu.cn

Java: private String name;
来源：http://up.haigaiapp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://bo.jctech888.com.cn

Ruby: @name = "x"
来源：http://rj.shxzukj.cn

C#:   public string Name { get; set; } = "x";
来源：http://uy.shxzukj.cn

[G04] 定义方法
来源：http://iv.bjjhwx.cn

Py:   def greet(self): return self.name
来源：http://wr.huixiangedu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fi.bjjhwx.cn

JS:   greet() { return this.name; }
来源：http://rh.huanxung.cn

TS:   greet(): string { return this.name; }
来源：http://gp.huixinmuqiang.cn

Java: String greet() { return name; }
来源：http://pv.shxzukj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ii.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://py.521024.cn

C#:   public string Greet() => Name;
来源：http://wb.colortex.cn

[G05] 继承
来源：http://aj.521024.cn

Py:   class Admin(User): pass
来源：http://nk.muxihuayi.cn

PHP:  class Admin extends User {}
来源：http://ft.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://rt.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://rg.huixinmuqiang.cn

Java: class Admin extends User {}
来源：http://jn.huanxung.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qq.521024.cn

Ruby: class Admin < User; end
来源：http://cp.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://fj.521024.cn

[G06] 重写方法
来源：http://nz.chemitech.net.cn

Py:   def greet(self): return "admin"
来源：http://zk.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yi.muxihuayi.cn

JS:   greet() { return "admin"; }
来源：http://nc.nicolike.cn

TS:   greet(): string { return "admin"; }
来源：http://fh.nicolike.cn

Java: @Override String greet() { return "admin"; }
来源：http://sk.chemitech.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dt.asd995.cn

Ruby: def greet; "admin"; end
来源：http://go.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://ji.yuexingan06.cn

[G07] 调用父类方法
来源：http://lp.huixinmuqiang.cn

Py:   super().greet()
来源：http://ev.lnxyls.cn

PHP:  parent::greet();
来源：http://td.nicolike.cn

JS:   super.greet();
来源：http://wf.newstarts.cn

TS:   super.greet();
来源：http://cr.shtwfgs.cn

Java: super.greet();
来源：http://am.szsharing.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tt.gzmigu.cn

Ruby: super
来源：http://jc.yuntaijiaju.cn

C#:   base.Greet();
来源：http://ll.shxzukj.cn

[G08] 静态方法与属性
来源：http://ij.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uj.wgjwhj.cn

PHP:  public static function f() {}
来源：http://vr.haigaiapp.cn

JS:   static f() {}
来源：http://xn.jctech888.com.cn

TS:   static f(): void {}
来源：http://jq.nicolike.cn

Java: static void f() {}
来源：http://mu.nicolike.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zh.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://nr.newstarts.cn

C#:   public static void F() {}
来源：http://nw.huanxung.cn

[G09] 接口 / 抽象类
来源：http://ir.521024.cn

Py:   from abc import ABC, abstractmethod
来源：http://ny.huanxung.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bd.gzmigu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nl.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://lz.bjjhwx.cn

Java: interface Shape { double area(); }
来源：http://ql.shxzukj.cn

Go:   type Shape interface { Area() float64 }
来源：http://rg.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tg.9csxet.cn

C#:   interface IShape { double Area(); }
来源：http://we.haigaiapp.cn

[G10] 访问控制
来源：http://xw.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://jc.nszjky.cn

PHP:  public / protected / private
来源：http://hu.jctech888.com.cn

JS:   #private 字段；其余公开
来源：http://vw.nicolike.cn

TS:   public / protected / private
来源：http://zc.gzmigu.cn

Java: public / protected / private / 默认包级
来源：http://ib.colortex.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gw.shtwfgs.cn

Ruby: public / protected / private
来源：http://qq.shxzukj.cn

C#:   public / protected / private / internal
来源：http://wd.yuntaijiaju.cn

[G11] getter / setter
来源：http://dv.wgjwhj.cn

Py:   @property 与 @x.setter
来源：http://ql.521024.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gz.szxytkj.cn

JS:   get name() { return this._name; }
来源：http://pz.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://sv.shxzskj.cn

Java: public String getName() { return name; }
来源：http://bw.521024.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yp.panjiajie.cn

Ruby: attr_accessor :name
来源：http://tb.newstarts.cn

C#:   public string Name { get; set; }
来源：http://ad.jctech888.com.cn

[G12] 对象转字符串
来源：http://fp.huixinmuqiang.cn

Py:   def __str__(self): return self.name
来源：http://wn.newstarts.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kj.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://ht.newstarts.cn

TS:   toString(): string { return this.name; }
来源：http://zl.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://ex.bookmarksfly.cn

Go:   func (u User) String() string { return u.Name }
来源：http://eu.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://no.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://db.bjjhwx.cn

[G13] 判断对象类型
来源：http://qa.shxzukj.cn

Py:   isinstance(u, User)
来源：http://ia.newstarts.cn

PHP:  $u instanceof User
来源：http://aw.yuexingan06.cn

JS:   u instanceof User
来源：http://mf.shxzukj.cn

TS:   u instanceof User
来源：http://pk.chemitech.net.cn

Java: u instanceof User
来源：http://hb.bookmarksfly.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ue.szxytkj.cn

Ruby: u.is_a?(User)
来源：http://sm.shxzukj.cn

C#:   u is User
来源：http://br.colortex.cn

[G14] 数据类 / record
来源：http://zf.asd995.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jm.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://ej.szxytkj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jl.shxzskj.cn

TS:   type User = { name: string; age: number };
来源：http://bd.nicolike.cn

Java: record User(String name, int age) {}
来源：http://nv.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://tq.hnjuh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bh.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://sh.asd995.cn

[G15] 枚举
来源：http://iz.wgjwhj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ll.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ou.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ae.nicolike.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lv.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://aj.haigaiapp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ic.chemitech.net.cn

Ruby: Color = %i[red green].freeze
来源：http://hc.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wc.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://jr.szxytkj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ks.yuntaijiaju.cn

PHP:  get_object_vars($obj);
来源：http://ta.yuntaijiaju.cn

JS:   Object.entries(obj)
来源：http://gb.shxzukj.cn

TS:   Object.entries(obj)
来源：http://np.shxzukj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qf.nicolike.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wj.9csxet.cn

Ruby: obj.instance_variables
来源：http://ip.521024.cn

C#:   // 用反射或 System.Text.Json
来源：http://cp.bjjhwx.cn

================================================================================
来源：http://ot.bookmarksfly.cn

H. 异常与错误处理
来源：http://bs.bookmarksfly.cn

================================================================================
来源：http://fe.shxzukj.cn

[H01] try / catch 基础
来源：http://eh.szxytkj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://va.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dp.haigaiapp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yx.9csxet.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sw.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tu.shxzskj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sz.huixinmuqiang.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xs.huanxung.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sa.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://wc.huanxung.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ho.huixinmuqiang.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kv.bookmarksfly.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lb.haigaiapp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yb.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ld.panjiajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://oj.jianghongdianzi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://px.huanxung.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sr.muxihuayi.cn

[H03] 主动抛出异常
来源：http://sj.szxytkj.cn

Py:   raise ValueError("错误信息")
来源：http://wy.bookmarksfly.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tr.521024.cn

JS:   throw new Error("错误信息");
来源：http://ak.nszjky.cn

TS:   throw new Error("错误信息");
来源：http://qh.shxzukj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pc.newstarts.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rg.nszjky.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fh.colortex.cn

C#:   throw new ArgumentException("错误信息");
来源：http://er.panjiajie.cn

[H04] 自定义异常类型
来源：http://xk.jctech888.com.cn

Py:   class MyError(Exception): pass
来源：http://xu.panjiajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fk.jianghongdianzi.cn

JS:   class MyError extends Error {}
来源：http://mr.huanxung.cn

TS:   class MyError extends Error {}
来源：http://hj.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://go.huixiangedu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qx.bjjhwx.cn

Ruby: class MyError < StandardError; end
来源：http://th.yuexingan06.cn

C#:   class MyException : Exception {}
来源：http://bn.lnxyls.cn

[H05] 捕获特定类型
来源：http://vb.szsharing.cn

Py:   except ValueError as e:
来源：http://kb.nicolike.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ru.haigaiapp.cn

JS:   if (e instanceof TypeError) {}
来源：http://mu.521024.cn

TS:   if (e instanceof TypeError) {}
来源：http://wt.hahajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://az.gzmigu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://es.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://bw.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qa.szxytkj.cn

[H06] 可选值 / 空值安全访问
来源：http://lp.chemitech.net.cn

Py:   value = d.get("k") or default
来源：http://ck.muxihuayi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mv.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yj.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cj.nicolike.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ay.lnxyls.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://br.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://na.lnxyls.cn

C#:   obj?.A?.B ?? default
来源：http://lm.shxzukj.cn

[H07] 断言
来源：http://lw.shtwfgs.cn

Py:   assert x > 0, "必须为正"
来源：http://sa.hahajie.cn

PHP:  assert($x > 0);
来源：http://vq.gzmigu.cn

JS:   console.assert(x > 0);
来源：http://eg.yuntaijiaju.cn

TS:   console.assert(x > 0);
来源：http://wg.gzmigu.cn

Java: assert x > 0 : "必须为正";
来源：http://ub.asd995.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xk.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kk.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://is.yuntaijiaju.cn

[H08] 获取错误信息与堆栈
来源：http://ry.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://nt.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://at.huanxung.cn

JS:   e.message;  e.stack
来源：http://tb.hnjuh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nt.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vo.newstarts.cn

Go:   err.Error()
来源：http://rw.hahajie.cn

Ruby: e.message;  e.backtrace
来源：http://ld.shxzukj.cn

C#:   e.Message;  e.StackTrace
来源：http://ch.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://qe.chemitech.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tt.yuexingan06.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dq.wgjwhj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zz.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://aj.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ae.szxytkj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ku.shxzskj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jh.bookmarksfly.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ly.gzmigu.cn

[H10] 资源自动释放
来源：http://jg.9csxet.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wq.bookmarksfly.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ov.shxzskj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nx.huanxung.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://if.hnjuh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lv.shxzskj.cn

Go:   defer f.Close()
来源：http://ow.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ko.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bp.hahajie.cn

================================================================================
来源：http://nt.yuexingan06.cn

I. 正则表达式
来源：http://ad.asd995.cn

================================================================================
来源：http://py.newstarts.cn

[I01] 判断是否匹配
来源：http://ju.bookmarksfly.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xu.asd995.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rr.gzmigu.cn

JS:   /\d+/.test(s)
来源：http://ht.lnxyls.cn

TS:   /\d+/.test(s)
来源：http://kq.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://oi.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xw.huanxung.cn

Ruby: s.match?(/\d+/)
来源：http://tx.jctech888.com.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gk.chemitech.net.cn

[I02] 提取所有匹配
来源：http://fp.panjiajie.cn

Py:   re.findall(r"\d+", s)
来源：http://lx.yuntaijiaju.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bq.jctech888.com.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jb.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://bu.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mj.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gh.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://pu.wgjwhj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tv.colortex.cn

[I03] 提取捕获分组
来源：http://vr.nicolike.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tl.jianghongdianzi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wu.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lw.huixinmuqiang.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kt.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rm.gzmigu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qi.newstarts.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rp.szsharing.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://um.panjiajie.cn

[I04] 正则替换
来源：http://en.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rc.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://we.panjiajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ok.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xc.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lk.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lu.jianghongdianzi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://td.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gl.newstarts.cn

[I05] 按正则拆分
来源：http://wq.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gh.chemitech.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vo.bookmarksfly.cn

JS:   s.split(/\s*,\s*/)
来源：http://jx.szxytkj.cn

TS:   s.split(/\s*,\s*/)
来源：http://jh.bjjhwx.cn

Java: s.split("\\s*,\\s*")
来源：http://nf.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wj.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nh.nszjky.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kn.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://db.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qh.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jf.nicolike.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hc.jctech888.com.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lr.asd995.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dp.yuexingan06.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ql.wgjwhj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hh.lnxyls.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mr.asd995.cn

[I07] 忽略大小写与多行模式
来源：http://xz.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qr.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://at.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ow.haigaiapp.cn

TS:   /error/gim
来源：http://la.hnjuh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fe.yuexingan06.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yw.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://rj.jianghongdianzi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xk.shxzukj.cn

[I08] 贪婪与非贪婪匹配
来源：http://oc.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kq.bjjhwx.cn


<!-- 参考信息 -->