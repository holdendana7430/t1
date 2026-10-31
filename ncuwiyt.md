代发 wailian999

Py:   class Admin(User): pass
来源：http://ob.jianghongdianzi.cn

PHP:  class Admin extends User {}
来源：http://fh.521024.cn

JS:   class Admin extends User {}
来源：http://tu.huixiangedu.cn

TS:   class Admin extends User {}
来源：http://mz.shxzukj.cn

Java: class Admin extends User {}
来源：http://qz.jctech888.com.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ex.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://pz.haigaiapp.cn

C#:   class Admin : User {}
来源：http://qj.szsharing.cn

[G06] 重写方法
来源：http://ww.huanxung.cn

Py:   def greet(self): return "admin"
来源：http://tv.huanxung.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://oy.asd995.cn

JS:   greet() { return "admin"; }
来源：http://dd.jianghongdianzi.cn

TS:   greet(): string { return "admin"; }
来源：http://tu.yuntaijiaju.cn

Java: @Override String greet() { return "admin"; }
来源：http://an.huixiangedu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nx.9csxet.cn

Ruby: def greet; "admin"; end
来源：http://fl.wgjwhj.cn

C#:   public override string Greet() => "admin";
来源：http://mr.yuntaijiaju.cn

[G07] 调用父类方法
来源：http://jw.9csxet.cn

Py:   super().greet()
来源：http://yw.huanxung.cn

PHP:  parent::greet();
来源：http://st.yuntaijiaju.cn

JS:   super.greet();
来源：http://gf.hnjuh.cn

TS:   super.greet();
来源：http://nb.lnxyls.cn

Java: super.greet();
来源：http://fv.wgjwhj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jl.chemitech.net.cn

Ruby: super
来源：http://xe.muxihuayi.cn

C#:   base.Greet();
来源：http://sr.yuexingan06.cn

[G08] 静态方法与属性
来源：http://pr.shtwfgs.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lt.asd995.cn

PHP:  public static function f() {}
来源：http://zf.muxihuayi.cn

JS:   static f() {}
来源：http://fo.szxytkj.cn

TS:   static f(): void {}
来源：http://ki.shxzukj.cn

Java: static void f() {}
来源：http://on.hnjuh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://jt.yuexingan06.cn

Ruby: def self.f; end
来源：http://rm.szsharing.cn

C#:   public static void F() {}
来源：http://rg.chemitech.net.cn

[G09] 接口 / 抽象类
来源：http://lj.9csxet.cn

Py:   from abc import ABC, abstractmethod
来源：http://mh.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gr.yuexingan06.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://th.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://uu.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://ij.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://xx.huixiangedu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pv.nicolike.cn

C#:   interface IShape { double Area(); }
来源：http://iy.shxzukj.cn

[G10] 访问控制
来源：http://gr.huixiangedu.cn

Py:   约定 _protected / __private（不强制）
来源：http://bf.9csxet.cn

PHP:  public / protected / private
来源：http://lt.hnjuh.cn

JS:   #private 字段；其余公开
来源：http://px.nicolike.cn

TS:   public / protected / private
来源：http://te.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://jw.yuexingan06.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cc.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://sy.bookmarksfly.cn

C#:   public / protected / private / internal
来源：http://ge.szsharing.cn

[G11] getter / setter
来源：http://jg.bjjhwx.cn

Py:   @property 与 @x.setter
来源：http://on.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://zl.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://rs.lnxyls.cn

TS:   get name(): string { return this._name; }
来源：http://uv.hahajie.cn

Java: public String getName() { return name; }
来源：http://uu.yuexingan06.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bl.lnxyls.cn

Ruby: attr_accessor :name
来源：http://ms.newstarts.cn

C#:   public string Name { get; set; }
来源：http://ya.shxzskj.cn

[G12] 对象转字符串
来源：http://at.jctech888.com.cn

Py:   def __str__(self): return self.name
来源：http://qv.huixinmuqiang.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://uq.yuexingan06.cn

JS:   toString() { return this.name; }
来源：http://px.huanxung.cn

TS:   toString(): string { return this.name; }
来源：http://rh.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://de.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xq.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://qy.haigaiapp.cn

C#:   public override string ToString() => Name;
来源：http://jr.colortex.cn

[G13] 判断对象类型
来源：http://ss.wgjwhj.cn

Py:   isinstance(u, User)
来源：http://bg.szsharing.cn

PHP:  $u instanceof User
来源：http://sn.huanxung.cn

JS:   u instanceof User
来源：http://ss.szsharing.cn

TS:   u instanceof User
来源：http://ps.nszjky.cn

Java: u instanceof User
来源：http://an.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dw.nicolike.cn

Ruby: u.is_a?(User)
来源：http://iz.huixiangedu.cn

C#:   u is User
来源：http://mw.haigaiapp.cn

[G14] 数据类 / record
来源：http://ba.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://aw.szsharing.cn

PHP:  // 用 readonly 属性模拟
来源：http://oy.haigaiapp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uv.szxytkj.cn

TS:   type User = { name: string; age: number };
来源：http://zn.huanxung.cn

Java: record User(String name, int age) {}
来源：http://jy.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://yn.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mm.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://mi.shtwfgs.cn

[G15] 枚举
来源：http://rk.hnjuh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ym.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kj.gzmigu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xq.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ng.hahajie.cn

Java: enum Color { RED, GREEN }
来源：http://dh.shxzukj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rz.shxzskj.cn

Ruby: Color = %i[red green].freeze
来源：http://hk.hnjuh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rw.muxihuayi.cn

[G16] 对象转数组 / 字典
来源：http://un.wgjwhj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zi.huanxung.cn

PHP:  get_object_vars($obj);
来源：http://gy.jctech888.com.cn

JS:   Object.entries(obj)
来源：http://gh.hahajie.cn

TS:   Object.entries(obj)
来源：http://wy.huixinmuqiang.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dj.muxihuayi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ps.9csxet.cn

Ruby: obj.instance_variables
来源：http://ix.jctech888.com.cn

C#:   // 用反射或 System.Text.Json
来源：http://ar.bookmarksfly.cn

================================================================================
来源：http://vq.nicolike.cn

H. 异常与错误处理
来源：http://uv.colortex.cn

================================================================================
来源：http://dn.huixiangedu.cn

[H01] try / catch 基础
来源：http://rr.huixiangedu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xv.shtwfgs.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tc.huanxung.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wa.huixiangedu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zb.hahajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tq.yuntaijiaju.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zf.szxytkj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qv.jctech888.com.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ek.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://bs.newstarts.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ee.hnjuh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yc.bjjhwx.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pt.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://kc.jianghongdianzi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://im.chemitech.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ju.gzmigu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xk.wgjwhj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rq.521024.cn

[H03] 主动抛出异常
来源：http://dh.muxihuayi.cn

Py:   raise ValueError("错误信息")
来源：http://jc.yuntaijiaju.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qu.hnjuh.cn

JS:   throw new Error("错误信息");
来源：http://gg.hnjuh.cn

TS:   throw new Error("错误信息");
来源：http://ku.haigaiapp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://cb.szsharing.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oe.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ln.huanxung.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dd.chemitech.net.cn

[H04] 自定义异常类型
来源：http://sr.huixiangedu.cn

Py:   class MyError(Exception): pass
来源：http://qb.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://za.szxytkj.cn

JS:   class MyError extends Error {}
来源：http://dc.huanxung.cn

TS:   class MyError extends Error {}
来源：http://mz.521024.cn

Java: class MyException extends RuntimeException {}
来源：http://df.bjjhwx.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://al.wgjwhj.cn

Ruby: class MyError < StandardError; end
来源：http://ud.shxzskj.cn

C#:   class MyException : Exception {}
来源：http://oa.asd995.cn

[H05] 捕获特定类型
来源：http://lt.lnxyls.cn

Py:   except ValueError as e:
来源：http://ug.hahajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gg.huixinmuqiang.cn

JS:   if (e instanceof TypeError) {}
来源：http://lh.9csxet.cn

TS:   if (e instanceof TypeError) {}
来源：http://qy.huixiangedu.cn

Java: catch (IOException | SQLException e) {}
来源：http://nk.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sd.yuntaijiaju.cn

Ruby: rescue ArgumentError => e
来源：http://mg.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lc.haigaiapp.cn

[H06] 可选值 / 空值安全访问
来源：http://ti.bjjhwx.cn

Py:   value = d.get("k") or default
来源：http://kf.nicolike.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lf.haigaiapp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pn.jctech888.com.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ur.huixiangedu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cy.shtwfgs.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://co.wgjwhj.cn

Ruby: d&.dig(:a, :b)
来源：http://kv.bookmarksfly.cn

C#:   obj?.A?.B ?? default
来源：http://un.huixiangedu.cn

[H07] 断言
来源：http://wf.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://sp.521024.cn

PHP:  assert($x > 0);
来源：http://he.colortex.cn

JS:   console.assert(x > 0);
来源：http://bn.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://zx.szsharing.cn

Java: assert x > 0 : "必须为正";
来源：http://zk.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ky.hahajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kw.bjjhwx.cn

C#:   Debug.Assert(x > 0);
来源：http://sb.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://gf.huixiangedu.cn

Py:   str(e);  traceback.format_exc()
来源：http://qf.huanxung.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fq.lnxyls.cn

JS:   e.message;  e.stack
来源：http://bm.shxzukj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xg.panjiajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yu.chemitech.net.cn

Go:   err.Error()
来源：http://vv.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://tn.huixiangedu.cn

C#:   e.Message;  e.StackTrace
来源：http://by.asd995.cn

[H09] 带错误码的异常
来源：http://db.shxzukj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gv.bjjhwx.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lm.shxzskj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ge.hnjuh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yb.szsharing.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lf.bookmarksfly.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fa.9csxet.cn

Ruby: raise MyError.new("fail", 500)
来源：http://or.lnxyls.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mg.hnjuh.cn

[H10] 资源自动释放
来源：http://oe.nicolike.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vt.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ko.shxzukj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yo.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qj.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://st.lnxyls.cn

Go:   defer f.Close()
来源：http://ny.huixiangedu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qn.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kx.nicolike.cn

================================================================================
来源：http://vz.huanxung.cn

I. 正则表达式
来源：http://du.szsharing.cn

================================================================================
来源：http://jx.hnjuh.cn

[I01] 判断是否匹配
来源：http://km.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xb.9csxet.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rv.szxytkj.cn

JS:   /\d+/.test(s)
来源：http://aw.muxihuayi.cn

TS:   /\d+/.test(s)
来源：http://he.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dc.nszjky.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://le.bookmarksfly.cn

Ruby: s.match?(/\d+/)
来源：http://gp.jctech888.com.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vd.shxzskj.cn

[I02] 提取所有匹配
来源：http://eo.jianghongdianzi.cn

Py:   re.findall(r"\d+", s)
来源：http://ks.521024.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fz.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cv.jianghongdianzi.cn

TS:   s.match(/\d+/g)
来源：http://je.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yp.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tn.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://ze.muxihuayi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xk.muxihuayi.cn

[I03] 提取捕获分组
来源：http://ae.wgjwhj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kp.shtwfgs.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zx.nicolike.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ah.521024.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ry.newstarts.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fa.shxzskj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ri.asd995.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qr.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dj.hnjuh.cn

[I04] 正则替换
来源：http://fl.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bh.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fy.szsharing.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ce.hahajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://al.huixiangedu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nx.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://gv.yuntaijiaju.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pk.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bg.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://bl.szsharing.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://iy.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tp.huanxung.cn

JS:   s.split(/\s*,\s*/)
来源：http://mk.newstarts.cn

TS:   s.split(/\s*,\s*/)
来源：http://qv.yuexingan06.cn

Java: s.split("\\s*,\\s*")
来源：http://pt.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cx.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bl.shxzukj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://go.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wi.szsharing.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kp.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://we.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bn.nicolike.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hy.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ln.lnxyls.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fo.szsharing.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bb.asd995.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zr.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://ur.newstarts.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rg.yuexingan06.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gs.panjiajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://iu.gzmigu.cn

TS:   /error/gim
来源：http://ks.szsharing.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kg.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pl.521024.cn

Ruby: s.scan(/error/i)
来源：http://es.asd995.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://rg.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://kq.huixinmuqiang.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jc.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yj.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wc.wgjwhj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gt.colortex.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rg.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dv.jianghongdianzi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jw.gzmigu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jv.jctech888.com.cn

================================================================================
来源：http://ag.huixinmuqiang.cn

J. 日期与时间
来源：http://id.newstarts.cn

================================================================================
来源：http://mb.panjiajie.cn

[J01] 获取当前时间
来源：http://zm.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mo.bjjhwx.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://te.newstarts.cn

JS:   new Date();  Date.now()
来源：http://vz.bjjhwx.cn

TS:   new Date();  Date.now()
来源：http://bo.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://by.muxihuayi.cn

Go:   time.Now()
来源：http://jn.bjjhwx.cn

Ruby: Time.now
来源：http://rt.hnjuh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ql.nszjky.cn

[J02] 格式化输出
来源：http://ot.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zv.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://po.9csxet.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zd.haigaiapp.cn

TS:   d.toISOString()
来源：http://ra.szsharing.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lj.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hn.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ll.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xc.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://td.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ks.huixinmuqiang.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lt.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://sh.panjiajie.cn


<!-- 参考信息 -->