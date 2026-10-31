代发 wailian999

Ruby: @name = "x"
来源：http://iw.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://ev.asd995.cn

[G04] 定义方法
来源：http://pi.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://sg.newstarts.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ej.szxytkj.cn

JS:   greet() { return this.name; }
来源：http://zw.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://vg.nszjky.cn

Java: String greet() { return name; }
来源：http://wr.huanxung.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gf.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://lg.9csxet.cn

C#:   public string Greet() => Name;
来源：http://ie.nszjky.cn

[G05] 继承
来源：http://mr.nszjky.cn

Py:   class Admin(User): pass
来源：http://us.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://gq.gzmigu.cn

JS:   class Admin extends User {}
来源：http://rc.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://ke.huixiangedu.cn

Java: class Admin extends User {}
来源：http://ey.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ov.huanxung.cn

Ruby: class Admin < User; end
来源：http://qm.hnjuh.cn

C#:   class Admin : User {}
来源：http://ls.bjjhwx.cn

[G06] 重写方法
来源：http://lf.colortex.cn

Py:   def greet(self): return "admin"
来源：http://qs.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://bi.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://qm.szxytkj.cn

TS:   greet(): string { return "admin"; }
来源：http://je.szxytkj.cn

Java: @Override String greet() { return "admin"; }
来源：http://bn.yuexingan06.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wc.wgjwhj.cn

Ruby: def greet; "admin"; end
来源：http://vb.newstarts.cn

C#:   public override string Greet() => "admin";
来源：http://ie.shtwfgs.cn

[G07] 调用父类方法
来源：http://bb.huanxung.cn

Py:   super().greet()
来源：http://sy.nszjky.cn

PHP:  parent::greet();
来源：http://zq.chemitech.net.cn

JS:   super.greet();
来源：http://sr.newstarts.cn

TS:   super.greet();
来源：http://ud.bookmarksfly.cn

Java: super.greet();
来源：http://sl.muxihuayi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://df.yuntaijiaju.cn

Ruby: super
来源：http://zs.huanxung.cn

C#:   base.Greet();
来源：http://es.jctech888.com.cn

[G08] 静态方法与属性
来源：http://ab.lnxyls.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hi.hahajie.cn

PHP:  public static function f() {}
来源：http://gi.bookmarksfly.cn

JS:   static f() {}
来源：http://cr.chemitech.net.cn

TS:   static f(): void {}
来源：http://bi.bjjhwx.cn

Java: static void f() {}
来源：http://hu.newstarts.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ad.yuexingan06.cn

Ruby: def self.f; end
来源：http://im.jianghongdianzi.cn

C#:   public static void F() {}
来源：http://qr.huixiangedu.cn

[G09] 接口 / 抽象类
来源：http://av.yuntaijiaju.cn

Py:   from abc import ABC, abstractmethod
来源：http://lx.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qy.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lz.chemitech.net.cn

TS:   interface Shape { area(): number; }
来源：http://nu.szxytkj.cn

Java: interface Shape { double area(); }
来源：http://rf.shxzukj.cn

Go:   type Shape interface { Area() float64 }
来源：http://pv.shtwfgs.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mn.shxzukj.cn

C#:   interface IShape { double Area(); }
来源：http://xw.yuexingan06.cn

[G10] 访问控制
来源：http://gq.hnjuh.cn

Py:   约定 _protected / __private（不强制）
来源：http://av.bjjhwx.cn

PHP:  public / protected / private
来源：http://kg.hahajie.cn

JS:   #private 字段；其余公开
来源：http://lz.huixinmuqiang.cn

TS:   public / protected / private
来源：http://el.hahajie.cn

Java: public / protected / private / 默认包级
来源：http://ek.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mb.hnjuh.cn

Ruby: public / protected / private
来源：http://kn.huanxung.cn

C#:   public / protected / private / internal
来源：http://xd.szsharing.cn

[G11] getter / setter
来源：http://gi.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://bo.yuexingan06.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ox.huixiangedu.cn

JS:   get name() { return this._name; }
来源：http://so.huanxung.cn

TS:   get name(): string { return this._name; }
来源：http://px.9csxet.cn

Java: public String getName() { return name; }
来源：http://rk.gzmigu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ts.huixiangedu.cn

Ruby: attr_accessor :name
来源：http://xo.hahajie.cn

C#:   public string Name { get; set; }
来源：http://xm.yuexingan06.cn

[G12] 对象转字符串
来源：http://ky.bookmarksfly.cn

Py:   def __str__(self): return self.name
来源：http://xl.asd995.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://az.shtwfgs.cn

JS:   toString() { return this.name; }
来源：http://ki.szsharing.cn

TS:   toString(): string { return this.name; }
来源：http://rq.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://vp.shtwfgs.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ek.panjiajie.cn

Ruby: def to_s; @name; end
来源：http://ly.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://ad.521024.cn

[G13] 判断对象类型
来源：http://yv.521024.cn

Py:   isinstance(u, User)
来源：http://fg.shtwfgs.cn

PHP:  $u instanceof User
来源：http://yt.wgjwhj.cn

JS:   u instanceof User
来源：http://ng.hahajie.cn

TS:   u instanceof User
来源：http://me.nszjky.cn

Java: u instanceof User
来源：http://rq.shtwfgs.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mv.yuexingan06.cn

Ruby: u.is_a?(User)
来源：http://kj.szsharing.cn

C#:   u is User
来源：http://eq.haigaiapp.cn

[G14] 数据类 / record
来源：http://sj.9csxet.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qb.huixiangedu.cn

PHP:  // 用 readonly 属性模拟
来源：http://dh.colortex.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jn.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://xv.yuexingan06.cn

Java: record User(String name, int age) {}
来源：http://vg.shxzskj.cn

Go:   type User struct { Name string; Age int }
来源：http://ip.bjjhwx.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://kw.9csxet.cn

C#:   record User(string Name, int Age);
来源：http://jj.shtwfgs.cn

[G15] 枚举
来源：http://na.jctech888.com.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ec.newstarts.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wq.muxihuayi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pu.9csxet.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mv.szxytkj.cn

Java: enum Color { RED, GREEN }
来源：http://hf.muxihuayi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fg.colortex.cn

Ruby: Color = %i[red green].freeze
来源：http://zu.jianghongdianzi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gd.newstarts.cn

[G16] 对象转数组 / 字典
来源：http://eo.bookmarksfly.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yf.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://mb.bjjhwx.cn

JS:   Object.entries(obj)
来源：http://sg.hnjuh.cn

TS:   Object.entries(obj)
来源：http://fv.asd995.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jh.newstarts.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dk.huanxung.cn

Ruby: obj.instance_variables
来源：http://ze.lnxyls.cn

C#:   // 用反射或 System.Text.Json
来源：http://et.asd995.cn

================================================================================
来源：http://vw.lnxyls.cn

H. 异常与错误处理
来源：http://iy.haigaiapp.cn

================================================================================
来源：http://rk.huanxung.cn

[H01] try / catch 基础
来源：http://zl.shtwfgs.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zs.huixiangedu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wq.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gz.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qa.bjjhwx.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qw.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://js.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tn.shxzskj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fl.panjiajie.cn

[H02] finally / ensure 收尾
来源：http://ov.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://du.jianghongdianzi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://si.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://km.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qv.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ck.bookmarksfly.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gc.newstarts.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rm.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nj.nszjky.cn

[H03] 主动抛出异常
来源：http://uu.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://ov.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sn.colortex.cn

JS:   throw new Error("错误信息");
来源：http://rf.bjjhwx.cn

TS:   throw new Error("错误信息");
来源：http://qn.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zc.shxzskj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pp.gzmigu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jq.newstarts.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ok.newstarts.cn

[H04] 自定义异常类型
来源：http://tg.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://fw.chemitech.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sw.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://oe.shxzskj.cn

TS:   class MyError extends Error {}
来源：http://ad.colortex.cn

Java: class MyException extends RuntimeException {}
来源：http://wm.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nj.shtwfgs.cn

Ruby: class MyError < StandardError; end
来源：http://jm.nszjky.cn

C#:   class MyException : Exception {}
来源：http://lk.huixiangedu.cn

[H05] 捕获特定类型
来源：http://so.huanxung.cn

Py:   except ValueError as e:
来源：http://vu.panjiajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yn.huanxung.cn

JS:   if (e instanceof TypeError) {}
来源：http://ti.szxytkj.cn

TS:   if (e instanceof TypeError) {}
来源：http://ff.asd995.cn

Java: catch (IOException | SQLException e) {}
来源：http://ir.nicolike.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ir.jctech888.com.cn

Ruby: rescue ArgumentError => e
来源：http://tl.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zw.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://mj.muxihuayi.cn

Py:   value = d.get("k") or default
来源：http://yz.szsharing.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hn.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://yp.huixiangedu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ak.jianghongdianzi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://si.lnxyls.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ka.bjjhwx.cn

Ruby: d&.dig(:a, :b)
来源：http://ti.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://gt.asd995.cn

[H07] 断言
来源：http://gu.gzmigu.cn

Py:   assert x > 0, "必须为正"
来源：http://jk.huixinmuqiang.cn

PHP:  assert($x > 0);
来源：http://wm.lnxyls.cn

JS:   console.assert(x > 0);
来源：http://yn.huixinmuqiang.cn

TS:   console.assert(x > 0);
来源：http://tb.521024.cn

Java: assert x > 0 : "必须为正";
来源：http://pg.hahajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ln.bookmarksfly.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xy.colortex.cn

C#:   Debug.Assert(x > 0);
来源：http://ft.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://ei.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://rq.yuntaijiaju.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://iw.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://xj.haigaiapp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mf.newstarts.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://su.shxzskj.cn

Go:   err.Error()
来源：http://tm.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://vt.asd995.cn

C#:   e.Message;  e.StackTrace
来源：http://qx.haigaiapp.cn

[H09] 带错误码的异常
来源：http://ho.colortex.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ny.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://uk.shxzskj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qr.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hi.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yl.colortex.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ty.szxytkj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dc.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fm.shtwfgs.cn

[H10] 资源自动释放
来源：http://vk.shtwfgs.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rd.chemitech.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://su.shtwfgs.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qu.szxytkj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hr.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tj.szsharing.cn

Go:   defer f.Close()
来源：http://on.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://dt.chemitech.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ua.panjiajie.cn

================================================================================
来源：http://qs.huanxung.cn

I. 正则表达式
来源：http://la.huanxung.cn

================================================================================
来源：http://dl.muxihuayi.cn

[I01] 判断是否匹配
来源：http://ix.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://do.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rd.huixinmuqiang.cn

JS:   /\d+/.test(s)
来源：http://jp.hahajie.cn

TS:   /\d+/.test(s)
来源：http://sb.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qp.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yj.gzmigu.cn

Ruby: s.match?(/\d+/)
来源：http://du.gzmigu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mz.bookmarksfly.cn

[I02] 提取所有匹配
来源：http://fd.muxihuayi.cn

Py:   re.findall(r"\d+", s)
来源：http://xa.huixinmuqiang.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ly.newstarts.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ea.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://ps.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://al.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xu.chemitech.net.cn

Ruby: s.scan(/\d+/)
来源：http://mk.colortex.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ix.huixiangedu.cn

[I03] 提取捕获分组
来源：http://cd.nszjky.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://po.yuexingan06.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wt.bjjhwx.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ah.shxzukj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hc.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bl.hahajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rv.shxzukj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dj.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ar.9csxet.cn

[I04] 正则替换
来源：http://ag.muxihuayi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://io.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jn.muxihuayi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dc.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ol.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ld.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sy.shxzskj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jh.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hn.hahajie.cn

[I05] 按正则拆分
来源：http://bv.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cj.lnxyls.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hg.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://mp.haigaiapp.cn

TS:   s.split(/\s*,\s*/)
来源：http://sr.yuntaijiaju.cn

Java: s.split("\\s*,\\s*")
来源：http://rf.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xg.jctech888.com.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xq.chemitech.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vs.9csxet.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rt.lnxyls.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rc.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qc.bookmarksfly.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oz.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://di.colortex.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nl.haigaiapp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rz.huanxung.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://by.newstarts.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ut.chemitech.net.cn

[I07] 忽略大小写与多行模式
来源：http://bm.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vd.yuexingan06.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bl.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ug.wgjwhj.cn

TS:   /error/gim
来源：http://tu.hahajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sh.muxihuayi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kp.newstarts.cn

Ruby: s.scan(/error/i)
来源：http://qu.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://md.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://wg.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gp.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lq.bookmarksfly.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zu.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ld.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ap.shxzskj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ti.muxihuayi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bd.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yy.shxzukj.cn

================================================================================
来源：http://fy.huixinmuqiang.cn

J. 日期与时间
来源：http://qp.newstarts.cn

================================================================================
来源：http://fx.bjjhwx.cn

[J01] 获取当前时间
来源：http://vj.jianghongdianzi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kf.wgjwhj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fa.521024.cn

JS:   new Date();  Date.now()
来源：http://fa.colortex.cn

TS:   new Date();  Date.now()
来源：http://tu.szxytkj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fa.shtwfgs.cn

Go:   time.Now()
来源：http://lb.szsharing.cn

Ruby: Time.now
来源：http://gw.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vo.colortex.cn

[J02] 格式化输出
来源：http://pg.nszjky.cn


<!-- 参考信息 -->