代发 wailian999

TS:   constructor(public name: string) {}
来源：http://sp.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://zh.nszjky.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dt.asd995.cn

Ruby: def initialize(name); @name = name; end
来源：http://iy.shtwfgs.cn

C#:   public User(string name) { Name = name; }
来源：http://ht.wgjwhj.cn

[G03] 实例属性
来源：http://xk.huixiangedu.cn

Py:   self.name = "x"
来源：http://th.lnxyls.cn

PHP:  public string $name = "x";
来源：http://bh.shxzukj.cn

JS:   this.name = "x";
来源：http://ff.gzmigu.cn

TS:   name: string = "x";
来源：http://ig.jianghongdianzi.cn

Java: private String name;
来源：http://lq.9csxet.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fa.newstarts.cn

Ruby: @name = "x"
来源：http://sf.yuntaijiaju.cn

C#:   public string Name { get; set; } = "x";
来源：http://xq.shxzukj.cn

[G04] 定义方法
来源：http://ya.521024.cn

Py:   def greet(self): return self.name
来源：http://pf.panjiajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fs.jianghongdianzi.cn

JS:   greet() { return this.name; }
来源：http://ji.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://zs.asd995.cn

Java: String greet() { return name; }
来源：http://vq.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://va.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://pz.shxzskj.cn

C#:   public string Greet() => Name;
来源：http://hb.9csxet.cn

[G05] 继承
来源：http://xb.gzmigu.cn

Py:   class Admin(User): pass
来源：http://dg.hahajie.cn

PHP:  class Admin extends User {}
来源：http://tp.bjjhwx.cn

JS:   class Admin extends User {}
来源：http://zr.nszjky.cn

TS:   class Admin extends User {}
来源：http://co.yuexingan06.cn

Java: class Admin extends User {}
来源：http://pr.szxytkj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dl.szxytkj.cn

Ruby: class Admin < User; end
来源：http://gc.yuntaijiaju.cn

C#:   class Admin : User {}
来源：http://fn.yuntaijiaju.cn

[G06] 重写方法
来源：http://zp.521024.cn

Py:   def greet(self): return "admin"
来源：http://az.haigaiapp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ue.jianghongdianzi.cn

JS:   greet() { return "admin"; }
来源：http://jz.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://sp.yuexingan06.cn

Java: @Override String greet() { return "admin"; }
来源：http://ni.gzmigu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qc.shxzskj.cn

Ruby: def greet; "admin"; end
来源：http://pk.jctech888.com.cn

C#:   public override string Greet() => "admin";
来源：http://lf.haigaiapp.cn

[G07] 调用父类方法
来源：http://dl.hnjuh.cn

Py:   super().greet()
来源：http://yc.521024.cn

PHP:  parent::greet();
来源：http://lk.panjiajie.cn

JS:   super.greet();
来源：http://xa.wgjwhj.cn

TS:   super.greet();
来源：http://py.hnjuh.cn

Java: super.greet();
来源：http://qu.huixiangedu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bt.lnxyls.cn

Ruby: super
来源：http://bx.szsharing.cn

C#:   base.Greet();
来源：http://pu.huixiangedu.cn

[G08] 静态方法与属性
来源：http://rq.bjjhwx.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ia.gzmigu.cn

PHP:  public static function f() {}
来源：http://ys.nszjky.cn

JS:   static f() {}
来源：http://rm.huixinmuqiang.cn

TS:   static f(): void {}
来源：http://nq.lnxyls.cn

Java: static void f() {}
来源：http://wo.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ca.chemitech.net.cn

Ruby: def self.f; end
来源：http://re.chemitech.net.cn

C#:   public static void F() {}
来源：http://um.nicolike.cn

[G09] 接口 / 抽象类
来源：http://zg.yuntaijiaju.cn

Py:   from abc import ABC, abstractmethod
来源：http://wq.yuntaijiaju.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wp.jianghongdianzi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sq.huixiangedu.cn

TS:   interface Shape { area(): number; }
来源：http://xq.huanxung.cn

Java: interface Shape { double area(); }
来源：http://vj.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://en.nszjky.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mx.muxihuayi.cn

C#:   interface IShape { double Area(); }
来源：http://sq.bookmarksfly.cn

[G10] 访问控制
来源：http://dg.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://mu.jianghongdianzi.cn

PHP:  public / protected / private
来源：http://wc.haigaiapp.cn

JS:   #private 字段；其余公开
来源：http://kb.yuntaijiaju.cn

TS:   public / protected / private
来源：http://hw.shxzukj.cn

Java: public / protected / private / 默认包级
来源：http://lj.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fz.yuexingan06.cn

Ruby: public / protected / private
来源：http://tk.gzmigu.cn

C#:   public / protected / private / internal
来源：http://fa.bjjhwx.cn

[G11] getter / setter
来源：http://zm.bookmarksfly.cn

Py:   @property 与 @x.setter
来源：http://do.huixiangedu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fg.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://kw.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://ix.panjiajie.cn

Java: public String getName() { return name; }
来源：http://yu.haigaiapp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qb.jianghongdianzi.cn

Ruby: attr_accessor :name
来源：http://br.huixinmuqiang.cn

C#:   public string Name { get; set; }
来源：http://xa.hnjuh.cn

[G12] 对象转字符串
来源：http://lo.haigaiapp.cn

Py:   def __str__(self): return self.name
来源：http://tu.9csxet.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ij.newstarts.cn

JS:   toString() { return this.name; }
来源：http://sv.yuntaijiaju.cn

TS:   toString(): string { return this.name; }
来源：http://dv.nszjky.cn

Java: @Override public String toString() { return name; }
来源：http://ll.newstarts.cn

Go:   func (u User) String() string { return u.Name }
来源：http://iu.hahajie.cn

Ruby: def to_s; @name; end
来源：http://ld.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://pk.chemitech.net.cn

[G13] 判断对象类型
来源：http://fy.yuntaijiaju.cn

Py:   isinstance(u, User)
来源：http://wf.hahajie.cn

PHP:  $u instanceof User
来源：http://pu.shtwfgs.cn

JS:   u instanceof User
来源：http://iw.chemitech.net.cn

TS:   u instanceof User
来源：http://qt.wgjwhj.cn

Java: u instanceof User
来源：http://di.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://em.yuntaijiaju.cn

Ruby: u.is_a?(User)
来源：http://ji.shxzukj.cn

C#:   u is User
来源：http://zb.shxzskj.cn

[G14] 数据类 / record
来源：http://al.yuntaijiaju.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://us.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://fc.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ar.hnjuh.cn

TS:   type User = { name: string; age: number };
来源：http://vu.shxzukj.cn

Java: record User(String name, int age) {}
来源：http://fh.lnxyls.cn

Go:   type User struct { Name string; Age int }
来源：http://yq.521024.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sp.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://mr.huixiangedu.cn

[G15] 枚举
来源：http://jb.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rz.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://es.huanxung.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xx.nszjky.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ld.huixiangedu.cn

Java: enum Color { RED, GREEN }
来源：http://uy.hahajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xh.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://hr.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://by.shxzskj.cn

[G16] 对象转数组 / 字典
来源：http://dw.521024.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yc.nicolike.cn

PHP:  get_object_vars($obj);
来源：http://ij.bjjhwx.cn

JS:   Object.entries(obj)
来源：http://ti.9csxet.cn

TS:   Object.entries(obj)
来源：http://qs.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tu.panjiajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://uc.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://fj.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://ve.lnxyls.cn

================================================================================
来源：http://ks.bjjhwx.cn

H. 异常与错误处理
来源：http://jh.shxzukj.cn

================================================================================
来源：http://re.huixiangedu.cn

[H01] try / catch 基础
来源：http://ry.jctech888.com.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qs.huixinmuqiang.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ms.jctech888.com.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yp.jctech888.com.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ld.bjjhwx.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ez.shxzskj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zx.jctech888.com.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nv.colortex.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://it.jctech888.com.cn

[H02] finally / ensure 收尾
来源：http://rk.szxytkj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yk.gzmigu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jy.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ds.gzmigu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://df.jianghongdianzi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ng.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mn.szxytkj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lz.colortex.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qy.9csxet.cn

[H03] 主动抛出异常
来源：http://wx.newstarts.cn

Py:   raise ValueError("错误信息")
来源：http://yo.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bx.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://qw.muxihuayi.cn

TS:   throw new Error("错误信息");
来源：http://nb.521024.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zs.huanxung.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hx.huixiangedu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ol.newstarts.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ng.asd995.cn

[H04] 自定义异常类型
来源：http://hm.yuexingan06.cn

Py:   class MyError(Exception): pass
来源：http://vn.colortex.cn

PHP:  class MyError extends RuntimeException {}
来源：http://al.yuexingan06.cn

JS:   class MyError extends Error {}
来源：http://rk.szsharing.cn

TS:   class MyError extends Error {}
来源：http://rx.haigaiapp.cn

Java: class MyException extends RuntimeException {}
来源：http://vy.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cd.colortex.cn

Ruby: class MyError < StandardError; end
来源：http://ps.shtwfgs.cn

C#:   class MyException : Exception {}
来源：http://dm.huixinmuqiang.cn

[H05] 捕获特定类型
来源：http://lm.shxzukj.cn

Py:   except ValueError as e:
来源：http://ct.huixiangedu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tm.colortex.cn

JS:   if (e instanceof TypeError) {}
来源：http://kz.huixinmuqiang.cn

TS:   if (e instanceof TypeError) {}
来源：http://id.haigaiapp.cn

Java: catch (IOException | SQLException e) {}
来源：http://kj.haigaiapp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qq.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://hv.wgjwhj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ni.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://jg.521024.cn

Py:   value = d.get("k") or default
来源：http://ou.gzmigu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xq.panjiajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pz.hnjuh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://uc.bookmarksfly.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rl.lnxyls.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qk.haigaiapp.cn

Ruby: d&.dig(:a, :b)
来源：http://jz.nszjky.cn

C#:   obj?.A?.B ?? default
来源：http://pi.huixiangedu.cn

[H07] 断言
来源：http://kg.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://js.shxzskj.cn

PHP:  assert($x > 0);
来源：http://nx.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://dt.asd995.cn

TS:   console.assert(x > 0);
来源：http://nz.hahajie.cn

Java: assert x > 0 : "必须为正";
来源：http://iu.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ib.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hu.jctech888.com.cn

C#:   Debug.Assert(x > 0);
来源：http://np.yuexingan06.cn

[H08] 获取错误信息与堆栈
来源：http://fz.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://fd.9csxet.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gb.nszjky.cn

JS:   e.message;  e.stack
来源：http://wq.hnjuh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mp.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jq.hnjuh.cn

Go:   err.Error()
来源：http://al.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://qg.shtwfgs.cn

C#:   e.Message;  e.StackTrace
来源：http://wy.hnjuh.cn

[H09] 带错误码的异常
来源：http://ph.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qf.521024.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mm.huanxung.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nb.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pc.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ej.nszjky.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qr.huanxung.cn

Ruby: raise MyError.new("fail", 500)
来源：http://am.chemitech.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vk.colortex.cn

[H10] 资源自动释放
来源：http://ah.newstarts.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cu.hnjuh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uj.yuntaijiaju.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://av.9csxet.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xc.newstarts.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ay.szxytkj.cn

Go:   defer f.Close()
来源：http://cq.szxytkj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dx.szxytkj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yj.chemitech.net.cn

================================================================================
来源：http://oq.jctech888.com.cn

I. 正则表达式
来源：http://sx.521024.cn

================================================================================
来源：http://db.huanxung.cn

[I01] 判断是否匹配
来源：http://hk.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sc.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ar.nszjky.cn

JS:   /\d+/.test(s)
来源：http://ya.newstarts.cn

TS:   /\d+/.test(s)
来源：http://xj.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ej.newstarts.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gy.gzmigu.cn

Ruby: s.match?(/\d+/)
来源：http://gm.chemitech.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://jf.huixiangedu.cn

[I02] 提取所有匹配
来源：http://dw.9csxet.cn

Py:   re.findall(r"\d+", s)
来源：http://qg.yuntaijiaju.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gg.nszjky.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ru.huixinmuqiang.cn

TS:   s.match(/\d+/g)
来源：http://nc.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pn.asd995.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ew.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://yc.jianghongdianzi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qv.muxihuayi.cn

[I03] 提取捕获分组
来源：http://ha.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yk.newstarts.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gs.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ze.bjjhwx.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://om.9csxet.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ze.nicolike.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zr.asd995.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ih.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qm.huanxung.cn

[I04] 正则替换
来源：http://pw.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://oa.nicolike.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xj.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dh.huixinmuqiang.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jc.szsharing.cn

Java: s.replaceAll("\\d+", "#")
来源：http://al.nszjky.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wv.szsharing.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cu.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://aw.szxytkj.cn

[I05] 按正则拆分
来源：http://rd.bookmarksfly.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ni.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tg.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://hz.muxihuayi.cn

TS:   s.split(/\s*,\s*/)
来源：http://cz.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://zy.nszjky.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hs.bjjhwx.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lw.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tm.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rb.bjjhwx.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sk.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nq.huixiangedu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bs.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bf.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zf.nszjky.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tz.nszjky.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://an.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rm.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://wv.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wx.haigaiapp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lo.gzmigu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://te.asd995.cn

TS:   /error/gim
来源：http://ge.muxihuayi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zf.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gh.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://ok.yuntaijiaju.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zo.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://gs.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xh.colortex.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xh.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zw.yuntaijiaju.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oh.jctech888.com.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://od.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xn.newstarts.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ue.hnjuh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hl.nszjky.cn

================================================================================
来源：http://fj.9csxet.cn


<!-- 参考信息 -->