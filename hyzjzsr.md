代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://gh.521024.cn

JS:   greet() { return this.name; }
来源：http://kz.shxzukj.cn

TS:   greet(): string { return this.name; }
来源：http://up.szxytkj.cn

Java: String greet() { return name; }
来源：http://pc.panjiajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vs.asd995.cn

Ruby: def greet; @name; end
来源：http://ff.yuexingan06.cn

C#:   public string Greet() => Name;
来源：http://tl.gzmigu.cn

[G05] 继承
来源：http://qq.wgjwhj.cn

Py:   class Admin(User): pass
来源：http://ff.szsharing.cn

PHP:  class Admin extends User {}
来源：http://mk.colortex.cn

JS:   class Admin extends User {}
来源：http://xd.jianghongdianzi.cn

TS:   class Admin extends User {}
来源：http://ln.shxzskj.cn

Java: class Admin extends User {}
来源：http://fz.nicolike.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zv.yuntaijiaju.cn

Ruby: class Admin < User; end
来源：http://td.colortex.cn

C#:   class Admin : User {}
来源：http://fw.jianghongdianzi.cn

[G06] 重写方法
来源：http://wx.shxzukj.cn

Py:   def greet(self): return "admin"
来源：http://uy.colortex.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jy.9csxet.cn

JS:   greet() { return "admin"; }
来源：http://ju.jianghongdianzi.cn

TS:   greet(): string { return "admin"; }
来源：http://fb.bookmarksfly.cn

Java: @Override String greet() { return "admin"; }
来源：http://or.bookmarksfly.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://us.wgjwhj.cn

Ruby: def greet; "admin"; end
来源：http://pu.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://hy.521024.cn

[G07] 调用父类方法
来源：http://pd.szxytkj.cn

Py:   super().greet()
来源：http://ln.hnjuh.cn

PHP:  parent::greet();
来源：http://as.shxzukj.cn

JS:   super.greet();
来源：http://il.yuntaijiaju.cn

TS:   super.greet();
来源：http://ii.jianghongdianzi.cn

Java: super.greet();
来源：http://ob.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gx.gzmigu.cn

Ruby: super
来源：http://dn.yuntaijiaju.cn

C#:   base.Greet();
来源：http://rp.bookmarksfly.cn

[G08] 静态方法与属性
来源：http://re.colortex.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://rg.nicolike.cn

PHP:  public static function f() {}
来源：http://hl.szxytkj.cn

JS:   static f() {}
来源：http://ed.yuexingan06.cn

TS:   static f(): void {}
来源：http://sx.lnxyls.cn

Java: static void f() {}
来源：http://kc.colortex.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nd.521024.cn

Ruby: def self.f; end
来源：http://db.chemitech.net.cn

C#:   public static void F() {}
来源：http://ic.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://ua.huixiangedu.cn

Py:   from abc import ABC, abstractmethod
来源：http://wk.521024.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dl.wgjwhj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vl.lnxyls.cn

TS:   interface Shape { area(): number; }
来源：http://ee.bookmarksfly.cn

Java: interface Shape { double area(); }
来源：http://vq.bookmarksfly.cn

Go:   type Shape interface { Area() float64 }
来源：http://qy.haigaiapp.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tf.yuexingan06.cn

C#:   interface IShape { double Area(); }
来源：http://dx.asd995.cn

[G10] 访问控制
来源：http://jg.jianghongdianzi.cn

Py:   约定 _protected / __private（不强制）
来源：http://hs.bookmarksfly.cn

PHP:  public / protected / private
来源：http://zu.huanxung.cn

JS:   #private 字段；其余公开
来源：http://mt.shxzskj.cn

TS:   public / protected / private
来源：http://tz.hnjuh.cn

Java: public / protected / private / 默认包级
来源：http://hq.bjjhwx.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xr.panjiajie.cn

Ruby: public / protected / private
来源：http://xy.yuntaijiaju.cn

C#:   public / protected / private / internal
来源：http://yv.szxytkj.cn

[G11] getter / setter
来源：http://fq.nicolike.cn

Py:   @property 与 @x.setter
来源：http://mt.bookmarksfly.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://km.szsharing.cn

JS:   get name() { return this._name; }
来源：http://nw.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://lr.shtwfgs.cn

Java: public String getName() { return name; }
来源：http://jm.hnjuh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fi.9csxet.cn

Ruby: attr_accessor :name
来源：http://de.nszjky.cn

C#:   public string Name { get; set; }
来源：http://cs.asd995.cn

[G12] 对象转字符串
来源：http://kw.panjiajie.cn

Py:   def __str__(self): return self.name
来源：http://hn.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vi.muxihuayi.cn

JS:   toString() { return this.name; }
来源：http://fe.yuntaijiaju.cn

TS:   toString(): string { return this.name; }
来源：http://ct.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://wx.lnxyls.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lw.nicolike.cn

Ruby: def to_s; @name; end
来源：http://pt.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://ul.huixiangedu.cn

[G13] 判断对象类型
来源：http://wd.haigaiapp.cn

Py:   isinstance(u, User)
来源：http://rg.huixinmuqiang.cn

PHP:  $u instanceof User
来源：http://yv.shxzskj.cn

JS:   u instanceof User
来源：http://ya.newstarts.cn

TS:   u instanceof User
来源：http://ux.jctech888.com.cn

Java: u instanceof User
来源：http://uh.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rc.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://ap.hahajie.cn

C#:   u is User
来源：http://fq.asd995.cn

[G14] 数据类 / record
来源：http://bc.shxzskj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yw.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://ks.szxytkj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://oa.chemitech.net.cn

TS:   type User = { name: string; age: number };
来源：http://dw.bookmarksfly.cn

Java: record User(String name, int age) {}
来源：http://vb.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://ek.haigaiapp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rh.521024.cn

C#:   record User(string Name, int Age);
来源：http://uu.gzmigu.cn

[G15] 枚举
来源：http://yt.shtwfgs.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://au.jianghongdianzi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fj.nszjky.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ob.shxzukj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lz.bookmarksfly.cn

Java: enum Color { RED, GREEN }
来源：http://ge.szxytkj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dx.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://an.9csxet.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://df.huanxung.cn

[G16] 对象转数组 / 字典
来源：http://av.newstarts.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xz.jctech888.com.cn

PHP:  get_object_vars($obj);
来源：http://yt.newstarts.cn

JS:   Object.entries(obj)
来源：http://nz.chemitech.net.cn

TS:   Object.entries(obj)
来源：http://sh.newstarts.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yv.szxytkj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cl.hnjuh.cn

Ruby: obj.instance_variables
来源：http://co.huixiangedu.cn

C#:   // 用反射或 System.Text.Json
来源：http://oy.521024.cn

================================================================================
来源：http://rw.szxytkj.cn

H. 异常与错误处理
来源：http://ch.hahajie.cn

================================================================================
来源：http://sw.chemitech.net.cn

[H01] try / catch 基础
来源：http://xc.hnjuh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eo.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qq.hahajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://cv.shtwfgs.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://op.521024.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://au.gzmigu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cd.szxytkj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zo.shtwfgs.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://oo.huanxung.cn

[H02] finally / ensure 收尾
来源：http://ph.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ae.huixiangedu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://td.shxzukj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ur.nszjky.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ei.szsharing.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ft.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bl.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gn.asd995.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cw.szxytkj.cn

[H03] 主动抛出异常
来源：http://af.asd995.cn

Py:   raise ValueError("错误信息")
来源：http://vg.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hi.szxytkj.cn

JS:   throw new Error("错误信息");
来源：http://ja.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://tq.panjiajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zs.haigaiapp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ar.newstarts.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://na.muxihuayi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rk.lnxyls.cn

[H04] 自定义异常类型
来源：http://iq.huixinmuqiang.cn

Py:   class MyError(Exception): pass
来源：http://eu.szsharing.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gj.shxzskj.cn

JS:   class MyError extends Error {}
来源：http://cn.huixinmuqiang.cn

TS:   class MyError extends Error {}
来源：http://rb.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://ng.bjjhwx.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gu.nicolike.cn

Ruby: class MyError < StandardError; end
来源：http://fb.huixinmuqiang.cn

C#:   class MyException : Exception {}
来源：http://bk.szxytkj.cn

[H05] 捕获特定类型
来源：http://ki.jctech888.com.cn

Py:   except ValueError as e:
来源：http://du.muxihuayi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ih.yuntaijiaju.cn

JS:   if (e instanceof TypeError) {}
来源：http://ud.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://vg.nicolike.cn

Java: catch (IOException | SQLException e) {}
来源：http://mn.shtwfgs.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://oh.gzmigu.cn

Ruby: rescue ArgumentError => e
来源：http://ee.wgjwhj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jl.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://hd.asd995.cn

Py:   value = d.get("k") or default
来源：http://jw.newstarts.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ec.lnxyls.cn

JS:   obj?.a?.b;  d ?? default
来源：http://di.yuntaijiaju.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yy.lnxyls.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mj.hahajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ij.bookmarksfly.cn

Ruby: d&.dig(:a, :b)
来源：http://vt.bjjhwx.cn

C#:   obj?.A?.B ?? default
来源：http://fx.bookmarksfly.cn

[H07] 断言
来源：http://sg.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://hz.huanxung.cn

PHP:  assert($x > 0);
来源：http://gr.9csxet.cn

JS:   console.assert(x > 0);
来源：http://rs.haigaiapp.cn

TS:   console.assert(x > 0);
来源：http://kc.huanxung.cn

Java: assert x > 0 : "必须为正";
来源：http://gj.newstarts.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pe.bookmarksfly.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ii.panjiajie.cn

C#:   Debug.Assert(x > 0);
来源：http://bp.colortex.cn

[H08] 获取错误信息与堆栈
来源：http://pa.huixiangedu.cn

Py:   str(e);  traceback.format_exc()
来源：http://wh.huixinmuqiang.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://om.asd995.cn

JS:   e.message;  e.stack
来源：http://so.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qw.newstarts.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ye.gzmigu.cn

Go:   err.Error()
来源：http://yv.bookmarksfly.cn

Ruby: e.message;  e.backtrace
来源：http://cs.shtwfgs.cn

C#:   e.Message;  e.StackTrace
来源：http://xs.nicolike.cn

[H09] 带错误码的异常
来源：http://qv.9csxet.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qn.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://oi.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zn.huixiangedu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yz.colortex.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ml.jctech888.com.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yt.521024.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yv.jctech888.com.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://aw.lnxyls.cn

[H10] 资源自动释放
来源：http://bo.hnjuh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kv.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ls.shxzskj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ti.jctech888.com.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uf.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ir.newstarts.cn

Go:   defer f.Close()
来源：http://ik.bookmarksfly.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://nv.9csxet.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://is.bookmarksfly.cn

================================================================================
来源：http://jj.panjiajie.cn

I. 正则表达式
来源：http://ts.shxzukj.cn

================================================================================
来源：http://zm.yuexingan06.cn

[I01] 判断是否匹配
来源：http://fh.shxzskj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zg.yuntaijiaju.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kl.nicolike.cn

JS:   /\d+/.test(s)
来源：http://zs.shtwfgs.cn

TS:   /\d+/.test(s)
来源：http://jt.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dy.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uj.9csxet.cn

Ruby: s.match?(/\d+/)
来源：http://gm.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fb.muxihuayi.cn

[I02] 提取所有匹配
来源：http://uo.nicolike.cn

Py:   re.findall(r"\d+", s)
来源：http://zg.colortex.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zs.lnxyls.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ow.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://ql.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://es.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zo.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://yg.gzmigu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iy.shtwfgs.cn

[I03] 提取捕获分组
来源：http://no.lnxyls.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://af.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bp.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://te.521024.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://eu.asd995.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jw.shxzskj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mt.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ye.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ff.hnjuh.cn

[I04] 正则替换
来源：http://lh.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yo.wgjwhj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ox.szsharing.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yu.huixiangedu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://th.lnxyls.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gt.bjjhwx.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zi.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tv.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bc.szsharing.cn

[I05] 按正则拆分
来源：http://wp.szxytkj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fk.chemitech.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pb.hnjuh.cn

JS:   s.split(/\s*,\s*/)
来源：http://yr.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://qu.nszjky.cn

Java: s.split("\\s*,\\s*")
来源：http://uh.hahajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uq.muxihuayi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bd.szxytkj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gv.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xg.muxihuayi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lj.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xf.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wp.chemitech.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tp.panjiajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ot.huixinmuqiang.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qm.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xu.shxzukj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ps.colortex.cn

[I07] 忽略大小写与多行模式
来源：http://nb.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://im.bjjhwx.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kn.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dw.yuntaijiaju.cn

TS:   /error/gim
来源：http://qt.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gb.9csxet.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uj.chemitech.net.cn

Ruby: s.scan(/error/i)
来源：http://jg.bjjhwx.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ey.szsharing.cn

[I08] 贪婪与非贪婪匹配
来源：http://ig.huixiangedu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zl.chemitech.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fj.shxzskj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ib.bookmarksfly.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jj.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://je.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eo.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rw.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ml.lnxyls.cn

================================================================================
来源：http://rg.colortex.cn

J. 日期与时间
来源：http://yy.9csxet.cn

================================================================================
来源：http://pr.muxihuayi.cn

[J01] 获取当前时间
来源：http://kd.jctech888.com.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ts.szsharing.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nq.hahajie.cn

JS:   new Date();  Date.now()
来源：http://oy.nszjky.cn

TS:   new Date();  Date.now()
来源：http://yi.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qz.yuexingan06.cn

Go:   time.Now()
来源：http://dk.huixinmuqiang.cn

Ruby: Time.now
来源：http://hu.lnxyls.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ki.wgjwhj.cn

[J02] 格式化输出
来源：http://pn.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lh.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bm.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zy.wgjwhj.cn

TS:   d.toISOString()
来源：http://oj.hahajie.cn


<!-- 参考信息 -->