代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://mj.szxytkj.cn

Ruby: def greet; @name; end
来源：http://yc.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://to.nszjky.cn

[G05] 继承
来源：http://nc.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://hy.huanxung.cn

PHP:  class Admin extends User {}
来源：http://pg.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://dk.jctech888.com.cn

TS:   class Admin extends User {}
来源：http://om.haigaiapp.cn

Java: class Admin extends User {}
来源：http://lw.szxytkj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rn.nicolike.cn

Ruby: class Admin < User; end
来源：http://hm.jctech888.com.cn

C#:   class Admin : User {}
来源：http://fl.newstarts.cn

[G06] 重写方法
来源：http://gp.asd995.cn

Py:   def greet(self): return "admin"
来源：http://bv.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nt.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://fq.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://rl.bjjhwx.cn

Java: @Override String greet() { return "admin"; }
来源：http://ja.shtwfgs.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fl.asd995.cn

Ruby: def greet; "admin"; end
来源：http://bf.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://vc.bookmarksfly.cn

[G07] 调用父类方法
来源：http://mp.nicolike.cn

Py:   super().greet()
来源：http://mj.lnxyls.cn

PHP:  parent::greet();
来源：http://gu.jctech888.com.cn

JS:   super.greet();
来源：http://yh.colortex.cn

TS:   super.greet();
来源：http://th.bjjhwx.cn

Java: super.greet();
来源：http://vv.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pm.chemitech.net.cn

Ruby: super
来源：http://yf.huixiangedu.cn

C#:   base.Greet();
来源：http://kp.hahajie.cn

[G08] 静态方法与属性
来源：http://ae.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rt.chemitech.net.cn

PHP:  public static function f() {}
来源：http://md.huixiangedu.cn

JS:   static f() {}
来源：http://tx.lnxyls.cn

TS:   static f(): void {}
来源：http://uq.bookmarksfly.cn

Java: static void f() {}
来源：http://lh.huixiangedu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xo.asd995.cn

Ruby: def self.f; end
来源：http://wn.521024.cn

C#:   public static void F() {}
来源：http://ef.jctech888.com.cn

[G09] 接口 / 抽象类
来源：http://nz.newstarts.cn

Py:   from abc import ABC, abstractmethod
来源：http://ab.newstarts.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qu.bjjhwx.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://in.9csxet.cn

TS:   interface Shape { area(): number; }
来源：http://zm.huixinmuqiang.cn

Java: interface Shape { double area(); }
来源：http://xd.shxzukj.cn

Go:   type Shape interface { Area() float64 }
来源：http://tc.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nm.huixiangedu.cn

C#:   interface IShape { double Area(); }
来源：http://sn.shxzukj.cn

[G10] 访问控制
来源：http://dl.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://sb.nicolike.cn

PHP:  public / protected / private
来源：http://rs.hnjuh.cn

JS:   #private 字段；其余公开
来源：http://qe.bookmarksfly.cn

TS:   public / protected / private
来源：http://ud.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://dp.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://as.haigaiapp.cn

Ruby: public / protected / private
来源：http://df.colortex.cn

C#:   public / protected / private / internal
来源：http://kj.muxihuayi.cn

[G11] getter / setter
来源：http://pl.jctech888.com.cn

Py:   @property 与 @x.setter
来源：http://yf.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ug.colortex.cn

JS:   get name() { return this._name; }
来源：http://yk.muxihuayi.cn

TS:   get name(): string { return this._name; }
来源：http://bn.yuntaijiaju.cn

Java: public String getName() { return name; }
来源：http://ox.yuexingan06.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ke.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://cj.huixinmuqiang.cn

C#:   public string Name { get; set; }
来源：http://cl.colortex.cn

[G12] 对象转字符串
来源：http://eu.haigaiapp.cn

Py:   def __str__(self): return self.name
来源：http://zx.huixinmuqiang.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vj.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://hd.newstarts.cn

TS:   toString(): string { return this.name; }
来源：http://dp.wgjwhj.cn

Java: @Override public String toString() { return name; }
来源：http://nh.newstarts.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ee.wgjwhj.cn

Ruby: def to_s; @name; end
来源：http://fu.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://wi.newstarts.cn

[G13] 判断对象类型
来源：http://dd.gzmigu.cn

Py:   isinstance(u, User)
来源：http://js.wgjwhj.cn

PHP:  $u instanceof User
来源：http://vy.shxzskj.cn

JS:   u instanceof User
来源：http://au.521024.cn

TS:   u instanceof User
来源：http://im.hnjuh.cn

Java: u instanceof User
来源：http://qr.hahajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kj.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://cg.shxzskj.cn

C#:   u is User
来源：http://xn.shtwfgs.cn

[G14] 数据类 / record
来源：http://gz.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ga.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://av.hnjuh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qf.gzmigu.cn

TS:   type User = { name: string; age: number };
来源：http://fr.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://vt.bjjhwx.cn

Go:   type User struct { Name string; Age int }
来源：http://vd.bookmarksfly.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://of.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://qt.shxzskj.cn

[G15] 枚举
来源：http://bz.colortex.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xg.nicolike.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xi.jctech888.com.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ip.bjjhwx.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dp.asd995.cn

Java: enum Color { RED, GREEN }
来源：http://fu.hnjuh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ky.shxzukj.cn

Ruby: Color = %i[red green].freeze
来源：http://uo.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nv.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://zc.panjiajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bp.szxytkj.cn

PHP:  get_object_vars($obj);
来源：http://jj.nicolike.cn

JS:   Object.entries(obj)
来源：http://tq.wgjwhj.cn

TS:   Object.entries(obj)
来源：http://pn.asd995.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mm.szsharing.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://do.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://rb.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://gf.huanxung.cn

================================================================================
来源：http://cy.chemitech.net.cn

H. 异常与错误处理
来源：http://lq.9csxet.cn

================================================================================
来源：http://rk.gzmigu.cn

[H01] try / catch 基础
来源：http://mm.9csxet.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fb.9csxet.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xy.yuntaijiaju.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kh.yuntaijiaju.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ys.jianghongdianzi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zt.asd995.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gx.bjjhwx.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ic.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nd.gzmigu.cn

[H02] finally / ensure 收尾
来源：http://hu.yuntaijiaju.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xm.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fl.szxytkj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jc.hnjuh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://au.jctech888.com.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wc.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rr.muxihuayi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zz.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qs.newstarts.cn

[H03] 主动抛出异常
来源：http://ue.yuexingan06.cn

Py:   raise ValueError("错误信息")
来源：http://cm.szsharing.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://in.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://pa.muxihuayi.cn

TS:   throw new Error("错误信息");
来源：http://ue.szsharing.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gq.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ls.nszjky.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yb.9csxet.cn

C#:   throw new ArgumentException("错误信息");
来源：http://el.newstarts.cn

[H04] 自定义异常类型
来源：http://dq.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://mj.asd995.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ut.lnxyls.cn

JS:   class MyError extends Error {}
来源：http://jn.jianghongdianzi.cn

TS:   class MyError extends Error {}
来源：http://uu.hnjuh.cn

Java: class MyException extends RuntimeException {}
来源：http://ek.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hv.bookmarksfly.cn

Ruby: class MyError < StandardError; end
来源：http://hw.huixinmuqiang.cn

C#:   class MyException : Exception {}
来源：http://pc.nszjky.cn

[H05] 捕获特定类型
来源：http://nq.muxihuayi.cn

Py:   except ValueError as e:
来源：http://mr.chemitech.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gr.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://fn.nszjky.cn

TS:   if (e instanceof TypeError) {}
来源：http://no.jctech888.com.cn

Java: catch (IOException | SQLException e) {}
来源：http://qq.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lo.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://hv.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mf.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://ff.hnjuh.cn

Py:   value = d.get("k") or default
来源：http://dz.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bq.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gm.nicolike.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jg.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://je.szsharing.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bm.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://ym.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://uf.huixinmuqiang.cn

[H07] 断言
来源：http://gg.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://ow.521024.cn

PHP:  assert($x > 0);
来源：http://zm.szxytkj.cn

JS:   console.assert(x > 0);
来源：http://af.shxzskj.cn

TS:   console.assert(x > 0);
来源：http://mi.521024.cn

Java: assert x > 0 : "必须为正";
来源：http://zp.gzmigu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://by.shxzskj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zt.shxzukj.cn

C#:   Debug.Assert(x > 0);
来源：http://nd.yuntaijiaju.cn

[H08] 获取错误信息与堆栈
来源：http://ug.panjiajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://cu.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://el.shtwfgs.cn

JS:   e.message;  e.stack
来源：http://oc.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vv.szsharing.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xc.hahajie.cn

Go:   err.Error()
来源：http://eu.shtwfgs.cn

Ruby: e.message;  e.backtrace
来源：http://wi.nicolike.cn

C#:   e.Message;  e.StackTrace
来源：http://yx.shxzukj.cn

[H09] 带错误码的异常
来源：http://pb.nicolike.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fp.gzmigu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ly.jctech888.com.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qp.lnxyls.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ua.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gz.wgjwhj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://st.asd995.cn

Ruby: raise MyError.new("fail", 500)
来源：http://by.jctech888.com.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qz.9csxet.cn

[H10] 资源自动释放
来源：http://pn.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kq.shxzukj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ae.yuexingan06.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vp.521024.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lr.huixinmuqiang.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fp.nszjky.cn

Go:   defer f.Close()
来源：http://fg.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://go.nicolike.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mo.yuexingan06.cn

================================================================================
来源：http://zg.haigaiapp.cn

I. 正则表达式
来源：http://wx.panjiajie.cn

================================================================================
来源：http://zd.chemitech.net.cn

[I01] 判断是否匹配
来源：http://xd.hahajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ji.9csxet.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ky.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://tj.yuntaijiaju.cn

TS:   /\d+/.test(s)
来源：http://os.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ee.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pt.colortex.cn

Ruby: s.match?(/\d+/)
来源：http://nz.panjiajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nt.muxihuayi.cn

[I02] 提取所有匹配
来源：http://zp.bjjhwx.cn

Py:   re.findall(r"\d+", s)
来源：http://lv.lnxyls.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://op.szsharing.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sa.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://cc.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kv.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rw.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://vt.shxzukj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jb.huixinmuqiang.cn

[I03] 提取捕获分组
来源：http://yk.bjjhwx.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tv.huixinmuqiang.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://md.bookmarksfly.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sy.lnxyls.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://iz.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fc.newstarts.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sx.bookmarksfly.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rn.haigaiapp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bi.chemitech.net.cn

[I04] 正则替换
来源：http://th.szsharing.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wd.hahajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ti.nszjky.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yp.hnjuh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mz.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bs.shxzukj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ce.chemitech.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tl.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yq.bjjhwx.cn

[I05] 按正则拆分
来源：http://ry.haigaiapp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lq.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cp.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://gy.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://ps.bjjhwx.cn

Java: s.split("\\s*,\\s*")
来源：http://xa.huanxung.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bw.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tz.szsharing.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oj.bjjhwx.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tt.asd995.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ww.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pj.colortex.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wa.hahajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xt.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gj.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pm.szxytkj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sn.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gb.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://sk.chemitech.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qw.huixiangedu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mi.hahajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ew.panjiajie.cn

TS:   /error/gim
来源：http://qy.yuexingan06.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hm.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ww.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://ne.chemitech.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tb.huixiangedu.cn

[I08] 贪婪与非贪婪匹配
来源：http://jq.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tz.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sa.shtwfgs.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dj.wgjwhj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pn.asd995.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mq.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zl.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ed.newstarts.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ms.jctech888.com.cn

================================================================================
来源：http://jg.jctech888.com.cn

J. 日期与时间
来源：http://gt.nicolike.cn

================================================================================
来源：http://ys.shtwfgs.cn

[J01] 获取当前时间
来源：http://th.lnxyls.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mn.szsharing.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rj.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://aq.huanxung.cn

TS:   new Date();  Date.now()
来源：http://vg.yuntaijiaju.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rh.wgjwhj.cn

Go:   time.Now()
来源：http://mi.nicolike.cn

Ruby: Time.now
来源：http://ts.hnjuh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hl.szsharing.cn

[J02] 格式化输出
来源：http://ma.huixiangedu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://id.chemitech.net.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vs.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://no.yuntaijiaju.cn

TS:   d.toISOString()
来源：http://lb.haigaiapp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cr.nicolike.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://bh.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rr.9csxet.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nf.yuntaijiaju.cn


<!-- 参考信息 -->