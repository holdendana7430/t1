代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://id.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://sm.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://pn.jctech888.com.cn

[G05] 继承
来源：http://ch.lnxyls.cn

Py:   class Admin(User): pass
来源：http://oc.szsharing.cn

PHP:  class Admin extends User {}
来源：http://eq.szsharing.cn

JS:   class Admin extends User {}
来源：http://bj.jianghongdianzi.cn

TS:   class Admin extends User {}
来源：http://ga.haigaiapp.cn

Java: class Admin extends User {}
来源：http://iy.hnjuh.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tw.szsharing.cn

Ruby: class Admin < User; end
来源：http://nu.huixiangedu.cn

C#:   class Admin : User {}
来源：http://vn.521024.cn

[G06] 重写方法
来源：http://iu.huixinmuqiang.cn

Py:   def greet(self): return "admin"
来源：http://xz.asd995.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zl.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://va.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://tp.bookmarksfly.cn

Java: @Override String greet() { return "admin"; }
来源：http://ti.muxihuayi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ft.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://fm.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://dt.hnjuh.cn

[G07] 调用父类方法
来源：http://py.muxihuayi.cn

Py:   super().greet()
来源：http://ji.panjiajie.cn

PHP:  parent::greet();
来源：http://ws.bookmarksfly.cn

JS:   super.greet();
来源：http://bk.colortex.cn

TS:   super.greet();
来源：http://le.panjiajie.cn

Java: super.greet();
来源：http://sb.bjjhwx.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uq.nszjky.cn

Ruby: super
来源：http://de.lnxyls.cn

C#:   base.Greet();
来源：http://eu.huixiangedu.cn

[G08] 静态方法与属性
来源：http://wa.gzmigu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ji.yuntaijiaju.cn

PHP:  public static function f() {}
来源：http://tk.yuntaijiaju.cn

JS:   static f() {}
来源：http://qa.colortex.cn

TS:   static f(): void {}
来源：http://xm.huixiangedu.cn

Java: static void f() {}
来源：http://os.bookmarksfly.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xe.nicolike.cn

Ruby: def self.f; end
来源：http://ow.szsharing.cn

C#:   public static void F() {}
来源：http://aa.huixinmuqiang.cn

[G09] 接口 / 抽象类
来源：http://qb.lnxyls.cn

Py:   from abc import ABC, abstractmethod
来源：http://ka.nicolike.cn

PHP:  interface Shape { public function area(): float; }
来源：http://va.yuntaijiaju.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fr.newstarts.cn

TS:   interface Shape { area(): number; }
来源：http://dr.gzmigu.cn

Java: interface Shape { double area(); }
来源：http://id.huixiangedu.cn

Go:   type Shape interface { Area() float64 }
来源：http://ap.nszjky.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sd.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://sp.hnjuh.cn

[G10] 访问控制
来源：http://js.huixinmuqiang.cn

Py:   约定 _protected / __private（不强制）
来源：http://ht.bjjhwx.cn

PHP:  public / protected / private
来源：http://og.szsharing.cn

JS:   #private 字段；其余公开
来源：http://id.jctech888.com.cn

TS:   public / protected / private
来源：http://ni.jctech888.com.cn

Java: public / protected / private / 默认包级
来源：http://ok.shxzukj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dq.yuntaijiaju.cn

Ruby: public / protected / private
来源：http://hr.chemitech.net.cn

C#:   public / protected / private / internal
来源：http://ka.chemitech.net.cn

[G11] getter / setter
来源：http://kc.wgjwhj.cn

Py:   @property 与 @x.setter
来源：http://we.huixiangedu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://uq.nszjky.cn

JS:   get name() { return this._name; }
来源：http://sa.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://gr.gzmigu.cn

Java: public String getName() { return name; }
来源：http://dl.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hf.yuexingan06.cn

Ruby: attr_accessor :name
来源：http://qh.szxytkj.cn

C#:   public string Name { get; set; }
来源：http://uj.nicolike.cn

[G12] 对象转字符串
来源：http://ln.yuntaijiaju.cn

Py:   def __str__(self): return self.name
来源：http://vn.yuntaijiaju.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ab.bookmarksfly.cn

JS:   toString() { return this.name; }
来源：http://yy.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://jb.521024.cn

Java: @Override public String toString() { return name; }
来源：http://zy.jctech888.com.cn

Go:   func (u User) String() string { return u.Name }
来源：http://yp.hahajie.cn

Ruby: def to_s; @name; end
来源：http://zi.shxzskj.cn

C#:   public override string ToString() => Name;
来源：http://sj.huixinmuqiang.cn

[G13] 判断对象类型
来源：http://da.wgjwhj.cn

Py:   isinstance(u, User)
来源：http://hs.nszjky.cn

PHP:  $u instanceof User
来源：http://bs.asd995.cn

JS:   u instanceof User
来源：http://wl.yuexingan06.cn

TS:   u instanceof User
来源：http://yb.huanxung.cn

Java: u instanceof User
来源：http://wr.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cn.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://sd.nicolike.cn

C#:   u is User
来源：http://oz.bookmarksfly.cn

[G14] 数据类 / record
来源：http://eo.huixinmuqiang.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rc.colortex.cn

PHP:  // 用 readonly 属性模拟
来源：http://il.yuexingan06.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dm.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://bl.muxihuayi.cn

Java: record User(String name, int age) {}
来源：http://bi.nszjky.cn

Go:   type User struct { Name string; Age int }
来源：http://mn.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ek.jianghongdianzi.cn

C#:   record User(string Name, int Age);
来源：http://wm.shxzskj.cn

[G15] 枚举
来源：http://dr.szsharing.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rb.hahajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lk.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hw.colortex.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ul.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://vg.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zb.szsharing.cn

Ruby: Color = %i[red green].freeze
来源：http://ks.nszjky.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lu.yuexingan06.cn

[G16] 对象转数组 / 字典
来源：http://bo.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wu.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://fx.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://vr.hnjuh.cn

TS:   Object.entries(obj)
来源：http://va.shtwfgs.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qt.bjjhwx.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ab.hnjuh.cn

Ruby: obj.instance_variables
来源：http://ko.newstarts.cn

C#:   // 用反射或 System.Text.Json
来源：http://zz.huanxung.cn

================================================================================
来源：http://fv.shtwfgs.cn

H. 异常与错误处理
来源：http://yg.jctech888.com.cn

================================================================================
来源：http://qc.hnjuh.cn

[H01] try / catch 基础
来源：http://qb.szsharing.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://si.wgjwhj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pk.shxzskj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sy.szxytkj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gi.chemitech.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yj.szsharing.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ak.haigaiapp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ch.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hx.panjiajie.cn

[H02] finally / ensure 收尾
来源：http://il.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://of.bjjhwx.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ku.nicolike.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zv.wgjwhj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pt.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wh.gzmigu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jo.chemitech.net.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://le.yuntaijiaju.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rr.521024.cn

[H03] 主动抛出异常
来源：http://se.shtwfgs.cn

Py:   raise ValueError("错误信息")
来源：http://kq.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lz.jctech888.com.cn

JS:   throw new Error("错误信息");
来源：http://xq.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://lt.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://be.bjjhwx.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ht.gzmigu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ub.shxzskj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vk.wgjwhj.cn

[H04] 自定义异常类型
来源：http://go.shxzskj.cn

Py:   class MyError(Exception): pass
来源：http://gn.nicolike.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hc.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://mh.panjiajie.cn

TS:   class MyError extends Error {}
来源：http://dx.szxytkj.cn

Java: class MyException extends RuntimeException {}
来源：http://xx.jctech888.com.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gx.hnjuh.cn

Ruby: class MyError < StandardError; end
来源：http://dm.521024.cn

C#:   class MyException : Exception {}
来源：http://ed.chemitech.net.cn

[H05] 捕获特定类型
来源：http://hz.lnxyls.cn

Py:   except ValueError as e:
来源：http://kv.bookmarksfly.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vu.newstarts.cn

JS:   if (e instanceof TypeError) {}
来源：http://xy.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://st.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://xc.521024.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://eg.jctech888.com.cn

Ruby: rescue ArgumentError => e
来源：http://px.9csxet.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nl.yuntaijiaju.cn

[H06] 可选值 / 空值安全访问
来源：http://xq.wgjwhj.cn

Py:   value = d.get("k") or default
来源：http://ff.521024.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wm.chemitech.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kq.nicolike.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sq.hahajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://iz.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://eh.hahajie.cn

Ruby: d&.dig(:a, :b)
来源：http://ec.nszjky.cn

C#:   obj?.A?.B ?? default
来源：http://nj.huixiangedu.cn

[H07] 断言
来源：http://fz.asd995.cn

Py:   assert x > 0, "必须为正"
来源：http://ge.szxytkj.cn

PHP:  assert($x > 0);
来源：http://lr.huanxung.cn

JS:   console.assert(x > 0);
来源：http://kd.yuntaijiaju.cn

TS:   console.assert(x > 0);
来源：http://th.szxytkj.cn

Java: assert x > 0 : "必须为正";
来源：http://cp.hnjuh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kk.colortex.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ka.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://hv.szsharing.cn

[H08] 获取错误信息与堆栈
来源：http://px.huanxung.cn

Py:   str(e);  traceback.format_exc()
来源：http://gy.9csxet.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sz.huixinmuqiang.cn

JS:   e.message;  e.stack
来源：http://nz.shxzskj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zi.huanxung.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zu.jctech888.com.cn

Go:   err.Error()
来源：http://ql.haigaiapp.cn

Ruby: e.message;  e.backtrace
来源：http://bx.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://fy.jianghongdianzi.cn

[H09] 带错误码的异常
来源：http://oo.jianghongdianzi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oe.hahajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jz.shxzskj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ez.szxytkj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rg.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qr.hnjuh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cp.jianghongdianzi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pp.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zk.panjiajie.cn

[H10] 资源自动释放
来源：http://li.lnxyls.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://in.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ut.hahajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ry.chemitech.net.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://di.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zm.szsharing.cn

Go:   defer f.Close()
来源：http://sd.panjiajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cf.9csxet.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fs.jianghongdianzi.cn

================================================================================
来源：http://dn.shxzukj.cn

I. 正则表达式
来源：http://jl.szsharing.cn

================================================================================
来源：http://os.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://wl.9csxet.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yw.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ct.huanxung.cn

JS:   /\d+/.test(s)
来源：http://tj.nicolike.cn

TS:   /\d+/.test(s)
来源：http://tz.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wr.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qo.lnxyls.cn

Ruby: s.match?(/\d+/)
来源：http://kq.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lo.szxytkj.cn

[I02] 提取所有匹配
来源：http://tw.muxihuayi.cn

Py:   re.findall(r"\d+", s)
来源：http://yz.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ek.hnjuh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ut.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://bk.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jz.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qn.hahajie.cn

Ruby: s.scan(/\d+/)
来源：http://bp.jianghongdianzi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://lm.colortex.cn

[I03] 提取捕获分组
来源：http://cp.hahajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lk.lnxyls.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fu.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://aa.shxzukj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fz.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ut.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wt.newstarts.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cr.nicolike.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jw.yuexingan06.cn

[I04] 正则替换
来源：http://wg.bjjhwx.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nk.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kt.shxzskj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dd.gzmigu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sq.szxytkj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ed.shxzukj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dz.panjiajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ov.asd995.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bz.jctech888.com.cn

[I05] 按正则拆分
来源：http://jy.colortex.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ps.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fa.huixinmuqiang.cn

JS:   s.split(/\s*,\s*/)
来源：http://hh.nicolike.cn

TS:   s.split(/\s*,\s*/)
来源：http://bg.shxzukj.cn

Java: s.split("\\s*,\\s*")
来源：http://ad.wgjwhj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://as.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://oy.jianghongdianzi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oj.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ey.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ii.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vw.hahajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ib.bookmarksfly.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ht.shxzskj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://as.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uh.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xy.lnxyls.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xh.asd995.cn

[I07] 忽略大小写与多行模式
来源：http://va.nicolike.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ls.yuexingan06.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pw.muxihuayi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wl.haigaiapp.cn

TS:   /error/gim
来源：http://uw.nszjky.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tr.hnjuh.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ms.521024.cn

Ruby: s.scan(/error/i)
来源：http://es.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ty.colortex.cn

[I08] 贪婪与非贪婪匹配
来源：http://wm.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vi.huixiangedu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bi.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gn.newstarts.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ce.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wz.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zy.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://aa.colortex.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zo.bookmarksfly.cn

================================================================================
来源：http://do.newstarts.cn

J. 日期与时间
来源：http://hf.huixinmuqiang.cn

================================================================================
来源：http://yj.gzmigu.cn

[J01] 获取当前时间
来源：http://qy.panjiajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://js.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tg.shtwfgs.cn

JS:   new Date();  Date.now()
来源：http://wz.panjiajie.cn

TS:   new Date();  Date.now()
来源：http://av.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tr.nicolike.cn

Go:   time.Now()
来源：http://lh.bookmarksfly.cn

Ruby: Time.now
来源：http://tv.szxytkj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qw.shtwfgs.cn

[J02] 格式化输出
来源：http://wm.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yx.nszjky.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rx.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zv.hahajie.cn

TS:   d.toISOString()
来源：http://ao.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ta.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lg.hahajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://it.nszjky.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://no.lnxyls.cn


<!-- 参考信息 -->