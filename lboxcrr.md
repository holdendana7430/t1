代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://kl.hnjuh.cn

JS:   greet() { return this.name; }
来源：http://gq.lnxyls.cn

TS:   greet(): string { return this.name; }
来源：http://yc.muxihuayi.cn

Java: String greet() { return name; }
来源：http://bt.nicolike.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://oq.shxzukj.cn

Ruby: def greet; @name; end
来源：http://ex.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://iw.panjiajie.cn

[G05] 继承
来源：http://gd.521024.cn

Py:   class Admin(User): pass
来源：http://nk.haigaiapp.cn

PHP:  class Admin extends User {}
来源：http://us.colortex.cn

JS:   class Admin extends User {}
来源：http://sv.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://no.jctech888.com.cn

Java: class Admin extends User {}
来源：http://mp.shxzukj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qs.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://tv.szsharing.cn

C#:   class Admin : User {}
来源：http://zz.colortex.cn

[G06] 重写方法
来源：http://vl.huanxung.cn

Py:   def greet(self): return "admin"
来源：http://ic.yuexingan06.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ml.9csxet.cn

JS:   greet() { return "admin"; }
来源：http://xd.haigaiapp.cn

TS:   greet(): string { return "admin"; }
来源：http://gz.szxytkj.cn

Java: @Override String greet() { return "admin"; }
来源：http://jn.asd995.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://nz.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://xl.chemitech.net.cn

C#:   public override string Greet() => "admin";
来源：http://tj.shxzukj.cn

[G07] 调用父类方法
来源：http://es.jctech888.com.cn

Py:   super().greet()
来源：http://yj.bjjhwx.cn

PHP:  parent::greet();
来源：http://lw.jctech888.com.cn

JS:   super.greet();
来源：http://kg.muxihuayi.cn

TS:   super.greet();
来源：http://vi.9csxet.cn

Java: super.greet();
来源：http://tl.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ep.9csxet.cn

Ruby: super
来源：http://yp.521024.cn

C#:   base.Greet();
来源：http://hd.gzmigu.cn

[G08] 静态方法与属性
来源：http://kj.521024.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qh.szsharing.cn

PHP:  public static function f() {}
来源：http://lz.jctech888.com.cn

JS:   static f() {}
来源：http://xu.szsharing.cn

TS:   static f(): void {}
来源：http://vo.haigaiapp.cn

Java: static void f() {}
来源：http://hp.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fk.shxzskj.cn

Ruby: def self.f; end
来源：http://qg.huixiangedu.cn

C#:   public static void F() {}
来源：http://ma.gzmigu.cn

[G09] 接口 / 抽象类
来源：http://xv.jianghongdianzi.cn

Py:   from abc import ABC, abstractmethod
来源：http://ot.szsharing.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hd.asd995.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xj.colortex.cn

TS:   interface Shape { area(): number; }
来源：http://lh.jianghongdianzi.cn

Java: interface Shape { double area(); }
来源：http://bl.shtwfgs.cn

Go:   type Shape interface { Area() float64 }
来源：http://oc.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://no.shxzukj.cn

C#:   interface IShape { double Area(); }
来源：http://zh.wgjwhj.cn

[G10] 访问控制
来源：http://qb.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://co.gzmigu.cn

PHP:  public / protected / private
来源：http://we.hnjuh.cn

JS:   #private 字段；其余公开
来源：http://vf.gzmigu.cn

TS:   public / protected / private
来源：http://xo.huanxung.cn

Java: public / protected / private / 默认包级
来源：http://pq.szsharing.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://br.9csxet.cn

Ruby: public / protected / private
来源：http://yo.yuexingan06.cn

C#:   public / protected / private / internal
来源：http://oe.hahajie.cn

[G11] getter / setter
来源：http://pn.szxytkj.cn

Py:   @property 与 @x.setter
来源：http://vg.wgjwhj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bw.nszjky.cn

JS:   get name() { return this._name; }
来源：http://ad.jianghongdianzi.cn

TS:   get name(): string { return this._name; }
来源：http://th.bookmarksfly.cn

Java: public String getName() { return name; }
来源：http://jq.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xx.asd995.cn

Ruby: attr_accessor :name
来源：http://ar.panjiajie.cn

C#:   public string Name { get; set; }
来源：http://ei.hnjuh.cn

[G12] 对象转字符串
来源：http://cg.nszjky.cn

Py:   def __str__(self): return self.name
来源：http://yh.jctech888.com.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pb.521024.cn

JS:   toString() { return this.name; }
来源：http://bh.haigaiapp.cn

TS:   toString(): string { return this.name; }
来源：http://ou.hnjuh.cn

Java: @Override public String toString() { return name; }
来源：http://gl.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qs.muxihuayi.cn

Ruby: def to_s; @name; end
来源：http://vb.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://np.szsharing.cn

[G13] 判断对象类型
来源：http://nq.colortex.cn

Py:   isinstance(u, User)
来源：http://yf.asd995.cn

PHP:  $u instanceof User
来源：http://ee.yuexingan06.cn

JS:   u instanceof User
来源：http://tz.nicolike.cn

TS:   u instanceof User
来源：http://cn.lnxyls.cn

Java: u instanceof User
来源：http://gg.shtwfgs.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lj.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://xf.jctech888.com.cn

C#:   u is User
来源：http://jd.nicolike.cn

[G14] 数据类 / record
来源：http://mt.yuntaijiaju.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sn.huanxung.cn

PHP:  // 用 readonly 属性模拟
来源：http://mn.szxytkj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mv.muxihuayi.cn

TS:   type User = { name: string; age: number };
来源：http://ib.jctech888.com.cn

Java: record User(String name, int age) {}
来源：http://if.wgjwhj.cn

Go:   type User struct { Name string; Age int }
来源：http://eg.szsharing.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tn.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://ew.yuexingan06.cn

[G15] 枚举
来源：http://md.wgjwhj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ke.szxytkj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hl.newstarts.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yr.chemitech.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eq.hahajie.cn

Java: enum Color { RED, GREEN }
来源：http://of.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ej.521024.cn

Ruby: Color = %i[red green].freeze
来源：http://kn.nicolike.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cj.521024.cn

[G16] 对象转数组 / 字典
来源：http://hs.colortex.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ho.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://kd.huixiangedu.cn

JS:   Object.entries(obj)
来源：http://tn.huanxung.cn

TS:   Object.entries(obj)
来源：http://nh.shxzskj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vu.yuntaijiaju.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mt.nicolike.cn

Ruby: obj.instance_variables
来源：http://if.hahajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://xs.jctech888.com.cn

================================================================================
来源：http://uq.huixinmuqiang.cn

H. 异常与错误处理
来源：http://bj.yuexingan06.cn

================================================================================
来源：http://dm.chemitech.net.cn

[H01] try / catch 基础
来源：http://lo.colortex.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yl.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bu.huixiangedu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://is.huixiangedu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cs.jianghongdianzi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://oh.shxzskj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yd.9csxet.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qr.521024.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hr.9csxet.cn

[H02] finally / ensure 收尾
来源：http://eb.panjiajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://kb.yuexingan06.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://np.shxzukj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pw.asd995.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ri.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fu.bookmarksfly.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fo.hnjuh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://zq.szsharing.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hk.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://sy.bookmarksfly.cn

Py:   raise ValueError("错误信息")
来源：http://mn.asd995.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://do.colortex.cn

JS:   throw new Error("错误信息");
来源：http://oa.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://xy.bjjhwx.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ew.gzmigu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://am.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ik.huanxung.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rw.huanxung.cn

[H04] 自定义异常类型
来源：http://ax.521024.cn

Py:   class MyError(Exception): pass
来源：http://pn.chemitech.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://pi.szxytkj.cn

JS:   class MyError extends Error {}
来源：http://nj.jianghongdianzi.cn

TS:   class MyError extends Error {}
来源：http://kl.nszjky.cn

Java: class MyException extends RuntimeException {}
来源：http://wy.chemitech.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zm.yuntaijiaju.cn

Ruby: class MyError < StandardError; end
来源：http://jr.haigaiapp.cn

C#:   class MyException : Exception {}
来源：http://nw.lnxyls.cn

[H05] 捕获特定类型
来源：http://zd.lnxyls.cn

Py:   except ValueError as e:
来源：http://fj.gzmigu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zf.hnjuh.cn

JS:   if (e instanceof TypeError) {}
来源：http://ou.jctech888.com.cn

TS:   if (e instanceof TypeError) {}
来源：http://of.huixiangedu.cn

Java: catch (IOException | SQLException e) {}
来源：http://ol.szsharing.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ho.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://ug.chemitech.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oe.521024.cn

[H06] 可选值 / 空值安全访问
来源：http://qz.jianghongdianzi.cn

Py:   value = d.get("k") or default
来源：http://ap.nszjky.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nu.lnxyls.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kr.colortex.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vw.yuexingan06.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cq.szsharing.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wv.gzmigu.cn

Ruby: d&.dig(:a, :b)
来源：http://qe.bookmarksfly.cn

C#:   obj?.A?.B ?? default
来源：http://fr.haigaiapp.cn

[H07] 断言
来源：http://nt.9csxet.cn

Py:   assert x > 0, "必须为正"
来源：http://uj.panjiajie.cn

PHP:  assert($x > 0);
来源：http://sy.9csxet.cn

JS:   console.assert(x > 0);
来源：http://ht.szsharing.cn

TS:   console.assert(x > 0);
来源：http://ui.asd995.cn

Java: assert x > 0 : "必须为正";
来源：http://mr.bookmarksfly.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hb.shxzukj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ld.wgjwhj.cn

C#:   Debug.Assert(x > 0);
来源：http://lq.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://xl.szsharing.cn

Py:   str(e);  traceback.format_exc()
来源：http://gk.yuntaijiaju.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vr.asd995.cn

JS:   e.message;  e.stack
来源：http://bu.shtwfgs.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dx.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://iu.huixinmuqiang.cn

Go:   err.Error()
来源：http://nb.bookmarksfly.cn

Ruby: e.message;  e.backtrace
来源：http://qy.huixiangedu.cn

C#:   e.Message;  e.StackTrace
来源：http://ym.yuntaijiaju.cn

[H09] 带错误码的异常
来源：http://ka.shxzukj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kx.shtwfgs.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fd.asd995.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ac.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wp.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ge.szxytkj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iv.panjiajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://oa.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://la.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://pp.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wu.chemitech.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zg.jctech888.com.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cu.huanxung.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://en.hnjuh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jw.bookmarksfly.cn

Go:   defer f.Close()
来源：http://qe.muxihuayi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://io.wgjwhj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rz.9csxet.cn

================================================================================
来源：http://kb.haigaiapp.cn

I. 正则表达式
来源：http://rs.bookmarksfly.cn

================================================================================
来源：http://ej.shtwfgs.cn

[I01] 判断是否匹配
来源：http://pq.shxzskj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mz.asd995.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ic.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://ur.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://hy.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qh.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ml.lnxyls.cn

Ruby: s.match?(/\d+/)
来源：http://vo.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kn.shxzukj.cn

[I02] 提取所有匹配
来源：http://pt.bjjhwx.cn

Py:   re.findall(r"\d+", s)
来源：http://fw.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://iw.huanxung.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fp.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://xy.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ci.nicolike.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ud.huanxung.cn

Ruby: s.scan(/\d+/)
来源：http://ke.bjjhwx.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ne.9csxet.cn

[I03] 提取捕获分组
来源：http://yj.hnjuh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://br.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hh.asd995.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cp.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ga.asd995.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zy.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tv.yuexingan06.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ew.bookmarksfly.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ef.muxihuayi.cn

[I04] 正则替换
来源：http://wp.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ju.panjiajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sp.gzmigu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pg.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://di.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fu.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jg.hnjuh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://db.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ka.wgjwhj.cn

[I05] 按正则拆分
来源：http://fl.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ry.chemitech.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wm.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://qj.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://by.nszjky.cn

Java: s.split("\\s*,\\s*")
来源：http://dr.jianghongdianzi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ea.asd995.cn

Ruby: s.split(/\s*,\s*/)
来源：http://uh.shxzskj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lm.shxzukj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pv.bjjhwx.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bx.shtwfgs.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://em.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gv.muxihuayi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ws.muxihuayi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sa.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yw.colortex.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cv.huixinmuqiang.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ed.huanxung.cn

[I07] 忽略大小写与多行模式
来源：http://fy.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mo.huanxung.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://es.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://tf.szxytkj.cn

TS:   /error/gim
来源：http://he.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bq.521024.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hs.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://bj.shtwfgs.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ia.newstarts.cn

[I08] 贪婪与非贪婪匹配
来源：http://an.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gp.bjjhwx.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xq.muxihuayi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ax.chemitech.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hk.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mk.shxzskj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fs.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cn.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gy.asd995.cn

================================================================================
来源：http://pk.szsharing.cn

J. 日期与时间
来源：http://xo.521024.cn

================================================================================
来源：http://jp.521024.cn

[J01] 获取当前时间
来源：http://oz.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ga.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vq.asd995.cn

JS:   new Date();  Date.now()
来源：http://fi.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://nt.gzmigu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sj.chemitech.net.cn

Go:   time.Now()
来源：http://hu.hahajie.cn

Ruby: Time.now
来源：http://db.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dn.muxihuayi.cn

[J02] 格式化输出
来源：http://ux.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ue.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ia.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://up.jianghongdianzi.cn

TS:   d.toISOString()
来源：http://zl.hnjuh.cn


<!-- 参考信息 -->