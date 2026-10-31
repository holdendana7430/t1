代发 wailian999

JS:   this.name = "x";
来源：http://yy.muxihuayi.cn

TS:   name: string = "x";
来源：http://vu.yuexingan06.cn

Java: private String name;
来源：http://ss.yuntaijiaju.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ek.521024.cn

Ruby: @name = "x"
来源：http://bx.bookmarksfly.cn

C#:   public string Name { get; set; } = "x";
来源：http://ht.szxytkj.cn

[G04] 定义方法
来源：http://rc.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://kw.hahajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://my.hnjuh.cn

JS:   greet() { return this.name; }
来源：http://ip.shxzukj.cn

TS:   greet(): string { return this.name; }
来源：http://fc.hahajie.cn

Java: String greet() { return name; }
来源：http://qf.huixinmuqiang.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://no.gzmigu.cn

Ruby: def greet; @name; end
来源：http://wo.asd995.cn

C#:   public string Greet() => Name;
来源：http://ep.521024.cn

[G05] 继承
来源：http://np.yuntaijiaju.cn

Py:   class Admin(User): pass
来源：http://sp.huixinmuqiang.cn

PHP:  class Admin extends User {}
来源：http://vt.wgjwhj.cn

JS:   class Admin extends User {}
来源：http://ss.9csxet.cn

TS:   class Admin extends User {}
来源：http://ub.newstarts.cn

Java: class Admin extends User {}
来源：http://fa.huanxung.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qg.chemitech.net.cn

Ruby: class Admin < User; end
来源：http://tn.huixiangedu.cn

C#:   class Admin : User {}
来源：http://hy.panjiajie.cn

[G06] 重写方法
来源：http://fl.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://tm.hahajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vv.panjiajie.cn

JS:   greet() { return "admin"; }
来源：http://xa.hnjuh.cn

TS:   greet(): string { return "admin"; }
来源：http://qw.lnxyls.cn

Java: @Override String greet() { return "admin"; }
来源：http://vg.shtwfgs.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wq.huixinmuqiang.cn

Ruby: def greet; "admin"; end
来源：http://af.shtwfgs.cn

C#:   public override string Greet() => "admin";
来源：http://sa.nicolike.cn

[G07] 调用父类方法
来源：http://sm.521024.cn

Py:   super().greet()
来源：http://qa.huanxung.cn

PHP:  parent::greet();
来源：http://uv.huixinmuqiang.cn

JS:   super.greet();
来源：http://qr.bookmarksfly.cn

TS:   super.greet();
来源：http://bi.nszjky.cn

Java: super.greet();
来源：http://ce.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fo.9csxet.cn

Ruby: super
来源：http://zz.shtwfgs.cn

C#:   base.Greet();
来源：http://on.huixinmuqiang.cn

[G08] 静态方法与属性
来源：http://cy.bjjhwx.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zn.shxzskj.cn

PHP:  public static function f() {}
来源：http://ks.9csxet.cn

JS:   static f() {}
来源：http://yu.nicolike.cn

TS:   static f(): void {}
来源：http://fl.nicolike.cn

Java: static void f() {}
来源：http://mo.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pm.shxzskj.cn

Ruby: def self.f; end
来源：http://fh.nszjky.cn

C#:   public static void F() {}
来源：http://nl.nszjky.cn

[G09] 接口 / 抽象类
来源：http://eh.bjjhwx.cn

Py:   from abc import ABC, abstractmethod
来源：http://pw.szxytkj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://fj.jctech888.com.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://nm.yuntaijiaju.cn

TS:   interface Shape { area(): number; }
来源：http://je.yuexingan06.cn

Java: interface Shape { double area(); }
来源：http://bx.huanxung.cn

Go:   type Shape interface { Area() float64 }
来源：http://fr.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ej.9csxet.cn

C#:   interface IShape { double Area(); }
来源：http://qn.hnjuh.cn

[G10] 访问控制
来源：http://kf.nszjky.cn

Py:   约定 _protected / __private（不强制）
来源：http://og.nicolike.cn

PHP:  public / protected / private
来源：http://xx.yuexingan06.cn

JS:   #private 字段；其余公开
来源：http://bk.gzmigu.cn

TS:   public / protected / private
来源：http://uo.9csxet.cn

Java: public / protected / private / 默认包级
来源：http://ek.shxzukj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lw.lnxyls.cn

Ruby: public / protected / private
来源：http://fu.bookmarksfly.cn

C#:   public / protected / private / internal
来源：http://ok.colortex.cn

[G11] getter / setter
来源：http://zu.9csxet.cn

Py:   @property 与 @x.setter
来源：http://bi.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://wu.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://cj.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://ew.szxytkj.cn

Java: public String getName() { return name; }
来源：http://sd.szsharing.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qm.521024.cn

Ruby: attr_accessor :name
来源：http://fj.shtwfgs.cn

C#:   public string Name { get; set; }
来源：http://zc.chemitech.net.cn

[G12] 对象转字符串
来源：http://yt.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://cx.bjjhwx.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://me.huixinmuqiang.cn

JS:   toString() { return this.name; }
来源：http://zn.huixinmuqiang.cn

TS:   toString(): string { return this.name; }
来源：http://kz.lnxyls.cn

Java: @Override public String toString() { return name; }
来源：http://yf.yuexingan06.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vr.haigaiapp.cn

Ruby: def to_s; @name; end
来源：http://ea.huixiangedu.cn

C#:   public override string ToString() => Name;
来源：http://sz.hahajie.cn

[G13] 判断对象类型
来源：http://ds.wgjwhj.cn

Py:   isinstance(u, User)
来源：http://lh.newstarts.cn

PHP:  $u instanceof User
来源：http://ow.yuexingan06.cn

JS:   u instanceof User
来源：http://po.muxihuayi.cn

TS:   u instanceof User
来源：http://ne.nicolike.cn

Java: u instanceof User
来源：http://ir.panjiajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pk.shxzukj.cn

Ruby: u.is_a?(User)
来源：http://ns.jianghongdianzi.cn

C#:   u is User
来源：http://hn.bookmarksfly.cn

[G14] 数据类 / record
来源：http://gd.nszjky.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ry.szsharing.cn

PHP:  // 用 readonly 属性模拟
来源：http://mz.colortex.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kt.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://pt.yuntaijiaju.cn

Java: record User(String name, int age) {}
来源：http://nv.chemitech.net.cn

Go:   type User struct { Name string; Age int }
来源：http://za.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xq.shxzukj.cn

C#:   record User(string Name, int Age);
来源：http://hm.panjiajie.cn

[G15] 枚举
来源：http://lx.nszjky.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tg.chemitech.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://aj.hahajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mj.hahajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sg.hahajie.cn

Java: enum Color { RED, GREEN }
来源：http://dp.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yq.asd995.cn

Ruby: Color = %i[red green].freeze
来源：http://hi.panjiajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rk.szsharing.cn

[G16] 对象转数组 / 字典
来源：http://ff.muxihuayi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xr.jianghongdianzi.cn

PHP:  get_object_vars($obj);
来源：http://az.nicolike.cn

JS:   Object.entries(obj)
来源：http://cv.muxihuayi.cn

TS:   Object.entries(obj)
来源：http://ie.bjjhwx.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cy.panjiajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jn.huanxung.cn

Ruby: obj.instance_variables
来源：http://id.szxytkj.cn

C#:   // 用反射或 System.Text.Json
来源：http://lf.huixiangedu.cn

================================================================================
来源：http://ch.nszjky.cn

H. 异常与错误处理
来源：http://tc.521024.cn

================================================================================
来源：http://dy.bjjhwx.cn

[H01] try / catch 基础
来源：http://fq.muxihuayi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vh.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ew.jctech888.com.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://im.szsharing.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zi.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pr.shxzukj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://se.bjjhwx.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vp.haigaiapp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ok.asd995.cn

[H02] finally / ensure 收尾
来源：http://po.hnjuh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xz.hnjuh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gu.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://oj.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tx.muxihuayi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://rk.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://tg.lnxyls.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mv.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ff.hnjuh.cn

[H03] 主动抛出异常
来源：http://ac.wgjwhj.cn

Py:   raise ValueError("错误信息")
来源：http://py.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://io.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://lf.nszjky.cn

TS:   throw new Error("错误信息");
来源：http://dy.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://da.huanxung.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hr.jctech888.com.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ia.yuntaijiaju.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rb.lnxyls.cn

[H04] 自定义异常类型
来源：http://dv.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://xx.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://aa.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://qx.szxytkj.cn

TS:   class MyError extends Error {}
来源：http://bg.colortex.cn

Java: class MyException extends RuntimeException {}
来源：http://lh.jctech888.com.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nn.newstarts.cn

Ruby: class MyError < StandardError; end
来源：http://nr.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://tm.shtwfgs.cn

[H05] 捕获特定类型
来源：http://og.huanxung.cn

Py:   except ValueError as e:
来源：http://gv.colortex.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nk.szxytkj.cn

JS:   if (e instanceof TypeError) {}
来源：http://nz.szxytkj.cn

TS:   if (e instanceof TypeError) {}
来源：http://sg.yuntaijiaju.cn

Java: catch (IOException | SQLException e) {}
来源：http://om.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bs.asd995.cn

Ruby: rescue ArgumentError => e
来源：http://st.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gb.shtwfgs.cn

[H06] 可选值 / 空值安全访问
来源：http://yl.huixinmuqiang.cn

Py:   value = d.get("k") or default
来源：http://ic.huixinmuqiang.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fr.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ix.yuexingan06.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ah.huixiangedu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rh.gzmigu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fx.hnjuh.cn

Ruby: d&.dig(:a, :b)
来源：http://dh.hnjuh.cn

C#:   obj?.A?.B ?? default
来源：http://dd.hnjuh.cn

[H07] 断言
来源：http://nw.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://ag.newstarts.cn

PHP:  assert($x > 0);
来源：http://og.bookmarksfly.cn

JS:   console.assert(x > 0);
来源：http://hv.bjjhwx.cn

TS:   console.assert(x > 0);
来源：http://pd.panjiajie.cn

Java: assert x > 0 : "必须为正";
来源：http://qd.bjjhwx.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ja.bjjhwx.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fh.chemitech.net.cn

C#:   Debug.Assert(x > 0);
来源：http://vf.jianghongdianzi.cn

[H08] 获取错误信息与堆栈
来源：http://jg.jctech888.com.cn

Py:   str(e);  traceback.format_exc()
来源：http://em.huixiangedu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bl.shxzskj.cn

JS:   e.message;  e.stack
来源：http://hc.huanxung.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kn.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pa.shxzukj.cn

Go:   err.Error()
来源：http://jh.shxzukj.cn

Ruby: e.message;  e.backtrace
来源：http://dq.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://qf.nszjky.cn

[H09] 带错误码的异常
来源：http://xa.asd995.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rb.panjiajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zb.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uu.huixiangedu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mu.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://bp.colortex.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uf.gzmigu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://to.521024.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ge.panjiajie.cn

[H10] 资源自动释放
来源：http://ml.shxzskj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ju.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ld.bjjhwx.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vs.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wr.colortex.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wx.muxihuayi.cn

Go:   defer f.Close()
来源：http://lm.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://so.lnxyls.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tv.newstarts.cn

================================================================================
来源：http://qk.muxihuayi.cn

I. 正则表达式
来源：http://ia.szsharing.cn

================================================================================
来源：http://tw.szsharing.cn

[I01] 判断是否匹配
来源：http://mk.521024.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gh.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bj.shtwfgs.cn

JS:   /\d+/.test(s)
来源：http://sj.haigaiapp.cn

TS:   /\d+/.test(s)
来源：http://jh.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://db.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cz.gzmigu.cn

Ruby: s.match?(/\d+/)
来源：http://zm.hahajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ik.gzmigu.cn

[I02] 提取所有匹配
来源：http://sd.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://zy.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hm.chemitech.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://oe.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://zu.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rn.9csxet.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://so.9csxet.cn

Ruby: s.scan(/\d+/)
来源：http://nb.gzmigu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zd.shxzskj.cn

[I03] 提取捕获分组
来源：http://fm.bookmarksfly.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hd.hahajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gi.shxzskj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ou.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jr.nszjky.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yd.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xo.huixiangedu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://en.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gs.shtwfgs.cn

[I04] 正则替换
来源：http://eb.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ri.asd995.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pq.9csxet.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pb.huanxung.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ho.bookmarksfly.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zt.jianghongdianzi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ms.newstarts.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jn.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ff.chemitech.net.cn

[I05] 按正则拆分
来源：http://ha.panjiajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ax.asd995.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ev.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://dc.nszjky.cn

TS:   s.split(/\s*,\s*/)
来源：http://pu.gzmigu.cn

Java: s.split("\\s*,\\s*")
来源：http://sn.bjjhwx.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ba.jctech888.com.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ha.nszjky.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ud.hahajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dn.yuntaijiaju.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yn.nszjky.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hg.lnxyls.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tq.szxytkj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://md.chemitech.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vo.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://df.huanxung.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pl.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://no.colortex.cn

[I07] 忽略大小写与多行模式
来源：http://qh.muxihuayi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yi.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ip.szxytkj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ah.huixiangedu.cn

TS:   /error/gim
来源：http://sy.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fg.bookmarksfly.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bb.yuntaijiaju.cn

Ruby: s.scan(/error/i)
来源：http://hc.9csxet.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xm.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://zx.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://os.haigaiapp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ce.jianghongdianzi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://no.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xm.huanxung.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://aj.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://al.muxihuayi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ri.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vv.panjiajie.cn

================================================================================
来源：http://um.asd995.cn

J. 日期与时间
来源：http://gi.jianghongdianzi.cn

================================================================================
来源：http://mq.lnxyls.cn

[J01] 获取当前时间
来源：http://xk.shtwfgs.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fv.jctech888.com.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uo.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://oi.huanxung.cn

TS:   new Date();  Date.now()
来源：http://qt.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ca.shxzukj.cn


<!-- 参考信息 -->