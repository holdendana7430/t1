代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://kz.nszjky.cn

Ruby: def greet; @name; end
来源：http://ib.colortex.cn

C#:   public string Greet() => Name;
来源：http://ka.yuntaijiaju.cn

[G05] 继承
来源：http://cr.nicolike.cn

Py:   class Admin(User): pass
来源：http://xb.yuexingan06.cn

PHP:  class Admin extends User {}
来源：http://fp.gzmigu.cn

JS:   class Admin extends User {}
来源：http://yg.wgjwhj.cn

TS:   class Admin extends User {}
来源：http://bh.szxytkj.cn

Java: class Admin extends User {}
来源：http://is.huixiangedu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kq.lnxyls.cn

Ruby: class Admin < User; end
来源：http://ur.bookmarksfly.cn

C#:   class Admin : User {}
来源：http://ey.bookmarksfly.cn

[G06] 重写方法
来源：http://ba.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://rt.shxzskj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ou.gzmigu.cn

JS:   greet() { return "admin"; }
来源：http://ta.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://fb.huixiangedu.cn

Java: @Override String greet() { return "admin"; }
来源：http://dx.shxzskj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fb.lnxyls.cn

Ruby: def greet; "admin"; end
来源：http://hv.chemitech.net.cn

C#:   public override string Greet() => "admin";
来源：http://ln.panjiajie.cn

[G07] 调用父类方法
来源：http://cu.gzmigu.cn

Py:   super().greet()
来源：http://qg.colortex.cn

PHP:  parent::greet();
来源：http://af.huixinmuqiang.cn

JS:   super.greet();
来源：http://wd.hahajie.cn

TS:   super.greet();
来源：http://nz.shxzukj.cn

Java: super.greet();
来源：http://he.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kn.nszjky.cn

Ruby: super
来源：http://wi.huixinmuqiang.cn

C#:   base.Greet();
来源：http://we.haigaiapp.cn

[G08] 静态方法与属性
来源：http://dz.asd995.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wq.szxytkj.cn

PHP:  public static function f() {}
来源：http://ye.szxytkj.cn

JS:   static f() {}
来源：http://jz.szsharing.cn

TS:   static f(): void {}
来源：http://mc.huanxung.cn

Java: static void f() {}
来源：http://qs.muxihuayi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ly.nszjky.cn

Ruby: def self.f; end
来源：http://rk.newstarts.cn

C#:   public static void F() {}
来源：http://it.panjiajie.cn

[G09] 接口 / 抽象类
来源：http://jl.yuntaijiaju.cn

Py:   from abc import ABC, abstractmethod
来源：http://zv.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dg.hnjuh.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fx.huixiangedu.cn

TS:   interface Shape { area(): number; }
来源：http://ql.hahajie.cn

Java: interface Shape { double area(); }
来源：http://ws.szsharing.cn

Go:   type Shape interface { Area() float64 }
来源：http://vx.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://vt.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://ft.huixiangedu.cn

[G10] 访问控制
来源：http://wi.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://fr.bookmarksfly.cn

PHP:  public / protected / private
来源：http://ps.chemitech.net.cn

JS:   #private 字段；其余公开
来源：http://sb.521024.cn

TS:   public / protected / private
来源：http://ku.haigaiapp.cn

Java: public / protected / private / 默认包级
来源：http://ov.huixiangedu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://br.newstarts.cn

Ruby: public / protected / private
来源：http://jg.asd995.cn

C#:   public / protected / private / internal
来源：http://aj.huixinmuqiang.cn

[G11] getter / setter
来源：http://cd.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://by.521024.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nl.nicolike.cn

JS:   get name() { return this._name; }
来源：http://gj.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://ue.asd995.cn

Java: public String getName() { return name; }
来源：http://do.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tx.nszjky.cn

Ruby: attr_accessor :name
来源：http://ln.hnjuh.cn

C#:   public string Name { get; set; }
来源：http://la.haigaiapp.cn

[G12] 对象转字符串
来源：http://du.9csxet.cn

Py:   def __str__(self): return self.name
来源：http://yt.newstarts.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dh.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://bp.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://ve.bookmarksfly.cn

Java: @Override public String toString() { return name; }
来源：http://pd.gzmigu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zz.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://yj.bookmarksfly.cn

C#:   public override string ToString() => Name;
来源：http://mi.colortex.cn

[G13] 判断对象类型
来源：http://bs.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://xp.huixinmuqiang.cn

PHP:  $u instanceof User
来源：http://nk.newstarts.cn

JS:   u instanceof User
来源：http://mj.asd995.cn

TS:   u instanceof User
来源：http://iq.nszjky.cn

Java: u instanceof User
来源：http://as.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jp.gzmigu.cn

Ruby: u.is_a?(User)
来源：http://gb.huanxung.cn

C#:   u is User
来源：http://pu.hnjuh.cn

[G14] 数据类 / record
来源：http://ot.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ry.nicolike.cn

PHP:  // 用 readonly 属性模拟
来源：http://ap.shxzskj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ox.huixiangedu.cn

TS:   type User = { name: string; age: number };
来源：http://za.gzmigu.cn

Java: record User(String name, int age) {}
来源：http://av.szxytkj.cn

Go:   type User struct { Name string; Age int }
来源：http://fw.szsharing.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nt.huixiangedu.cn

C#:   record User(string Name, int Age);
来源：http://pq.yuntaijiaju.cn

[G15] 枚举
来源：http://hk.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zi.shxzskj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bo.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yi.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jh.muxihuayi.cn

Java: enum Color { RED, GREEN }
来源：http://vw.chemitech.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yt.bjjhwx.cn

Ruby: Color = %i[red green].freeze
来源：http://nk.hahajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jm.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://yw.huixiangedu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bh.newstarts.cn

PHP:  get_object_vars($obj);
来源：http://ps.newstarts.cn

JS:   Object.entries(obj)
来源：http://kd.jctech888.com.cn

TS:   Object.entries(obj)
来源：http://kb.jianghongdianzi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ab.521024.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wi.szsharing.cn

Ruby: obj.instance_variables
来源：http://pb.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://tz.huixiangedu.cn

================================================================================
来源：http://eo.huixiangedu.cn

H. 异常与错误处理
来源：http://hz.huixiangedu.cn

================================================================================
来源：http://ht.yuexingan06.cn

[H01] try / catch 基础
来源：http://rf.521024.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rj.9csxet.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xr.colortex.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://li.shxzukj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://os.yuexingan06.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vc.wgjwhj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ox.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kf.shtwfgs.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nw.gzmigu.cn

[H02] finally / ensure 收尾
来源：http://sv.huixiangedu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ag.panjiajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qr.gzmigu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ps.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dp.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fx.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ps.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dq.jianghongdianzi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qi.colortex.cn

[H03] 主动抛出异常
来源：http://zt.panjiajie.cn

Py:   raise ValueError("错误信息")
来源：http://uu.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mq.hahajie.cn

JS:   throw new Error("错误信息");
来源：http://uw.huanxung.cn

TS:   throw new Error("错误信息");
来源：http://rt.szsharing.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://np.szxytkj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://st.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vg.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dh.jctech888.com.cn

[H04] 自定义异常类型
来源：http://lf.colortex.cn

Py:   class MyError(Exception): pass
来源：http://ai.huixiangedu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rw.521024.cn

JS:   class MyError extends Error {}
来源：http://ku.nicolike.cn

TS:   class MyError extends Error {}
来源：http://sc.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://da.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sv.colortex.cn

Ruby: class MyError < StandardError; end
来源：http://tj.szsharing.cn

C#:   class MyException : Exception {}
来源：http://pl.wgjwhj.cn

[H05] 捕获特定类型
来源：http://us.nicolike.cn

Py:   except ValueError as e:
来源：http://xk.jianghongdianzi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xx.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://ux.shxzskj.cn

TS:   if (e instanceof TypeError) {}
来源：http://gc.9csxet.cn

Java: catch (IOException | SQLException e) {}
来源：http://gc.gzmigu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ad.shxzskj.cn

Ruby: rescue ArgumentError => e
来源：http://ne.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ia.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://ym.haigaiapp.cn

Py:   value = d.get("k") or default
来源：http://zy.haigaiapp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gx.jctech888.com.cn

JS:   obj?.a?.b;  d ?? default
来源：http://uw.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hx.yuexingan06.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rz.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qz.shtwfgs.cn

Ruby: d&.dig(:a, :b)
来源：http://ap.shxzskj.cn

C#:   obj?.A?.B ?? default
来源：http://xv.haigaiapp.cn

[H07] 断言
来源：http://oi.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://ce.nszjky.cn

PHP:  assert($x > 0);
来源：http://gb.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://qk.huanxung.cn

TS:   console.assert(x > 0);
来源：http://nf.muxihuayi.cn

Java: assert x > 0 : "必须为正";
来源：http://zt.yuexingan06.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lj.nicolike.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fj.huixinmuqiang.cn

C#:   Debug.Assert(x > 0);
来源：http://pf.panjiajie.cn

[H08] 获取错误信息与堆栈
来源：http://ou.9csxet.cn

Py:   str(e);  traceback.format_exc()
来源：http://uq.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tj.huanxung.cn

JS:   e.message;  e.stack
来源：http://hl.panjiajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ti.szxytkj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://aa.nicolike.cn

Go:   err.Error()
来源：http://rs.yuntaijiaju.cn

Ruby: e.message;  e.backtrace
来源：http://ko.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://oq.asd995.cn

[H09] 带错误码的异常
来源：http://ul.shxzukj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mz.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://po.haigaiapp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dy.jianghongdianzi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jr.9csxet.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tg.szxytkj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lk.huixinmuqiang.cn

Ruby: raise MyError.new("fail", 500)
来源：http://io.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://aw.gzmigu.cn

[H10] 资源自动释放
来源：http://dk.chemitech.net.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sq.huixiangedu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lb.szsharing.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ya.bookmarksfly.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://kz.bjjhwx.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zu.huanxung.cn

Go:   defer f.Close()
来源：http://lp.asd995.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qj.newstarts.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bb.hnjuh.cn

================================================================================
来源：http://tm.chemitech.net.cn

I. 正则表达式
来源：http://dp.panjiajie.cn

================================================================================
来源：http://nv.szsharing.cn

[I01] 判断是否匹配
来源：http://by.muxihuayi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ka.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rv.huixiangedu.cn

JS:   /\d+/.test(s)
来源：http://ji.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://yz.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bu.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ol.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://gu.nicolike.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ky.bookmarksfly.cn

[I02] 提取所有匹配
来源：http://jj.gzmigu.cn

Py:   re.findall(r"\d+", s)
来源：http://ym.lnxyls.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oj.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ha.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://im.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bo.521024.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zl.newstarts.cn

Ruby: s.scan(/\d+/)
来源：http://bd.muxihuayi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://an.nicolike.cn

[I03] 提取捕获分组
来源：http://og.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cu.bookmarksfly.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pz.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rd.huixiangedu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tv.yuntaijiaju.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jy.panjiajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sl.nszjky.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kp.9csxet.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eu.521024.cn

[I04] 正则替换
来源：http://lx.yuexingan06.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lz.yuexingan06.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wq.9csxet.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nq.colortex.cn

TS:   s.replace(/\d+/g, "#")
来源：http://es.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jg.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pw.jctech888.com.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ut.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yb.hnjuh.cn

[I05] 按正则拆分
来源：http://dl.hahajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zy.haigaiapp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jx.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://fg.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://qb.chemitech.net.cn

Java: s.split("\\s*,\\s*")
来源：http://zs.shxzskj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kn.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hy.chemitech.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jl.nicolike.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ti.huixiangedu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://an.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tl.521024.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ue.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ui.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://po.521024.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vu.colortex.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ny.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ww.haigaiapp.cn

[I07] 忽略大小写与多行模式
来源：http://qk.yuexingan06.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qc.hnjuh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zi.yuntaijiaju.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://al.jctech888.com.cn

TS:   /error/gim
来源：http://ee.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yg.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xp.521024.cn

Ruby: s.scan(/error/i)
来源：http://mm.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tp.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://wn.521024.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://du.bjjhwx.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kl.asd995.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mn.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://fo.yuexingan06.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fv.asd995.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jh.shxzukj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ra.colortex.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ye.panjiajie.cn

================================================================================
来源：http://nc.gzmigu.cn

J. 日期与时间
来源：http://gs.panjiajie.cn

================================================================================
来源：http://tq.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://rn.muxihuayi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ar.szsharing.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aw.hahajie.cn

JS:   new Date();  Date.now()
来源：http://wa.521024.cn

TS:   new Date();  Date.now()
来源：http://lt.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fr.huixiangedu.cn

Go:   time.Now()
来源：http://mv.bookmarksfly.cn

Ruby: Time.now
来源：http://up.colortex.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cb.huixiangedu.cn

[J02] 格式化输出
来源：http://uj.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jp.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jh.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://rj.wgjwhj.cn

TS:   d.toISOString()
来源：http://te.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wu.shxzskj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gj.colortex.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jx.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cz.shtwfgs.cn


<!-- 参考信息 -->