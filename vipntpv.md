代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://es.gzmigu.cn

Ruby: def greet; @name; end
来源：http://yf.521024.cn

C#:   public string Greet() => Name;
来源：http://ee.shtwfgs.cn

[G05] 继承
来源：http://cl.gzmigu.cn

Py:   class Admin(User): pass
来源：http://jq.lnxyls.cn

PHP:  class Admin extends User {}
来源：http://vs.chemitech.net.cn

JS:   class Admin extends User {}
来源：http://ir.bookmarksfly.cn

TS:   class Admin extends User {}
来源：http://ys.colortex.cn

Java: class Admin extends User {}
来源：http://mi.shxzukj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yy.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://sa.9csxet.cn

C#:   class Admin : User {}
来源：http://fb.bookmarksfly.cn

[G06] 重写方法
来源：http://om.huixinmuqiang.cn

Py:   def greet(self): return "admin"
来源：http://ed.asd995.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://uo.521024.cn

JS:   greet() { return "admin"; }
来源：http://uy.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://ne.huixiangedu.cn

Java: @Override String greet() { return "admin"; }
来源：http://ss.gzmigu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tv.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://vf.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://xj.gzmigu.cn

[G07] 调用父类方法
来源：http://ks.huixiangedu.cn

Py:   super().greet()
来源：http://yb.yuntaijiaju.cn

PHP:  parent::greet();
来源：http://ku.huanxung.cn

JS:   super.greet();
来源：http://gr.huixiangedu.cn

TS:   super.greet();
来源：http://ec.lnxyls.cn

Java: super.greet();
来源：http://oa.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ce.shxzukj.cn

Ruby: super
来源：http://vq.lnxyls.cn

C#:   base.Greet();
来源：http://mm.panjiajie.cn

[G08] 静态方法与属性
来源：http://wp.bookmarksfly.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://an.yuntaijiaju.cn

PHP:  public static function f() {}
来源：http://jo.bookmarksfly.cn

JS:   static f() {}
来源：http://xy.szxytkj.cn

TS:   static f(): void {}
来源：http://ez.lnxyls.cn

Java: static void f() {}
来源：http://vf.9csxet.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ze.huixinmuqiang.cn

Ruby: def self.f; end
来源：http://nb.colortex.cn

C#:   public static void F() {}
来源：http://nu.gzmigu.cn

[G09] 接口 / 抽象类
来源：http://gk.huixiangedu.cn

Py:   from abc import ABC, abstractmethod
来源：http://et.521024.cn

PHP:  interface Shape { public function area(): float; }
来源：http://tx.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lo.huixinmuqiang.cn

TS:   interface Shape { area(): number; }
来源：http://vb.huixinmuqiang.cn

Java: interface Shape { double area(); }
来源：http://xk.9csxet.cn

Go:   type Shape interface { Area() float64 }
来源：http://us.shxzukj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rc.wgjwhj.cn

C#:   interface IShape { double Area(); }
来源：http://hl.colortex.cn

[G10] 访问控制
来源：http://vm.wgjwhj.cn

Py:   约定 _protected / __private（不强制）
来源：http://sx.szsharing.cn

PHP:  public / protected / private
来源：http://zv.9csxet.cn

JS:   #private 字段；其余公开
来源：http://yb.newstarts.cn

TS:   public / protected / private
来源：http://qd.521024.cn

Java: public / protected / private / 默认包级
来源：http://dk.yuexingan06.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bh.shxzskj.cn

Ruby: public / protected / private
来源：http://wi.shxzskj.cn

C#:   public / protected / private / internal
来源：http://wa.9csxet.cn

[G11] getter / setter
来源：http://do.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://sm.szxytkj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pb.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://wu.shtwfgs.cn

TS:   get name(): string { return this._name; }
来源：http://kr.yuntaijiaju.cn

Java: public String getName() { return name; }
来源：http://kg.huixiangedu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ug.newstarts.cn

Ruby: attr_accessor :name
来源：http://vb.jctech888.com.cn

C#:   public string Name { get; set; }
来源：http://cv.hnjuh.cn

[G12] 对象转字符串
来源：http://ur.asd995.cn

Py:   def __str__(self): return self.name
来源：http://up.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://oe.jianghongdianzi.cn

JS:   toString() { return this.name; }
来源：http://gr.colortex.cn

TS:   toString(): string { return this.name; }
来源：http://mt.jctech888.com.cn

Java: @Override public String toString() { return name; }
来源：http://qf.newstarts.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ny.hahajie.cn

Ruby: def to_s; @name; end
来源：http://ow.chemitech.net.cn

C#:   public override string ToString() => Name;
来源：http://eq.colortex.cn

[G13] 判断对象类型
来源：http://yw.9csxet.cn

Py:   isinstance(u, User)
来源：http://lc.szsharing.cn

PHP:  $u instanceof User
来源：http://pq.newstarts.cn

JS:   u instanceof User
来源：http://lk.shxzukj.cn

TS:   u instanceof User
来源：http://lp.huixiangedu.cn

Java: u instanceof User
来源：http://wg.hahajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://uq.chemitech.net.cn

Ruby: u.is_a?(User)
来源：http://rs.bookmarksfly.cn

C#:   u is User
来源：http://gv.yuexingan06.cn

[G14] 数据类 / record
来源：http://io.huanxung.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ol.shtwfgs.cn

PHP:  // 用 readonly 属性模拟
来源：http://ob.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xk.haigaiapp.cn

TS:   type User = { name: string; age: number };
来源：http://rr.bookmarksfly.cn

Java: record User(String name, int age) {}
来源：http://iu.bjjhwx.cn

Go:   type User struct { Name string; Age int }
来源：http://vm.newstarts.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qx.bookmarksfly.cn

C#:   record User(string Name, int Age);
来源：http://uh.lnxyls.cn

[G15] 枚举
来源：http://gh.colortex.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xz.521024.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vw.bjjhwx.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ld.haigaiapp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wt.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://cg.szxytkj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tl.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://sz.panjiajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qm.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://nh.muxihuayi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://es.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://la.szxytkj.cn

JS:   Object.entries(obj)
来源：http://qe.yuexingan06.cn

TS:   Object.entries(obj)
来源：http://kh.nszjky.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ux.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hk.nicolike.cn

Ruby: obj.instance_variables
来源：http://mz.gzmigu.cn

C#:   // 用反射或 System.Text.Json
来源：http://ho.hnjuh.cn

================================================================================
来源：http://cf.9csxet.cn

H. 异常与错误处理
来源：http://uj.shxzukj.cn

================================================================================
来源：http://ts.colortex.cn

[H01] try / catch 基础
来源：http://vc.szxytkj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://go.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cu.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://aq.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gc.521024.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sn.asd995.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://le.newstarts.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wj.bjjhwx.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lr.panjiajie.cn

[H02] finally / ensure 收尾
来源：http://yi.huixiangedu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://kr.shtwfgs.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://we.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://iz.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://iq.lnxyls.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mm.nszjky.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yv.colortex.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://us.shxzukj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xi.szsharing.cn

[H03] 主动抛出异常
来源：http://fs.panjiajie.cn

Py:   raise ValueError("错误信息")
来源：http://hk.521024.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bg.haigaiapp.cn

JS:   throw new Error("错误信息");
来源：http://ry.huixiangedu.cn

TS:   throw new Error("错误信息");
来源：http://vp.bjjhwx.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mv.wgjwhj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pc.huixiangedu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://aj.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://lt.bjjhwx.cn

[H04] 自定义异常类型
来源：http://eh.nicolike.cn

Py:   class MyError(Exception): pass
来源：http://uw.szxytkj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bv.gzmigu.cn

JS:   class MyError extends Error {}
来源：http://xo.muxihuayi.cn

TS:   class MyError extends Error {}
来源：http://in.yuntaijiaju.cn

Java: class MyException extends RuntimeException {}
来源：http://lu.521024.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ka.shtwfgs.cn

Ruby: class MyError < StandardError; end
来源：http://sh.huixinmuqiang.cn

C#:   class MyException : Exception {}
来源：http://mc.asd995.cn

[H05] 捕获特定类型
来源：http://ag.nszjky.cn

Py:   except ValueError as e:
来源：http://kl.lnxyls.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xz.nszjky.cn

JS:   if (e instanceof TypeError) {}
来源：http://fq.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://pn.colortex.cn

Java: catch (IOException | SQLException e) {}
来源：http://ol.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nm.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://en.colortex.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fo.newstarts.cn

[H06] 可选值 / 空值安全访问
来源：http://lx.yuexingan06.cn

Py:   value = d.get("k") or default
来源：http://hn.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rf.chemitech.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gg.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qr.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://di.chemitech.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ro.wgjwhj.cn

Ruby: d&.dig(:a, :b)
来源：http://fh.hnjuh.cn

C#:   obj?.A?.B ?? default
来源：http://sk.jianghongdianzi.cn

[H07] 断言
来源：http://pn.9csxet.cn

Py:   assert x > 0, "必须为正"
来源：http://cn.hahajie.cn

PHP:  assert($x > 0);
来源：http://fi.newstarts.cn

JS:   console.assert(x > 0);
来源：http://xp.hnjuh.cn

TS:   console.assert(x > 0);
来源：http://uq.yuntaijiaju.cn

Java: assert x > 0 : "必须为正";
来源：http://cr.huanxung.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ud.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://og.muxihuayi.cn

C#:   Debug.Assert(x > 0);
来源：http://xs.shtwfgs.cn

[H08] 获取错误信息与堆栈
来源：http://nv.shxzskj.cn

Py:   str(e);  traceback.format_exc()
来源：http://xq.lnxyls.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xi.bjjhwx.cn

JS:   e.message;  e.stack
来源：http://ox.nszjky.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jv.shtwfgs.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uc.nicolike.cn

Go:   err.Error()
来源：http://wb.yuntaijiaju.cn

Ruby: e.message;  e.backtrace
来源：http://sf.chemitech.net.cn

C#:   e.Message;  e.StackTrace
来源：http://vm.jctech888.com.cn

[H09] 带错误码的异常
来源：http://dm.muxihuayi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ct.nicolike.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ct.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mo.huixiangedu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nx.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ch.huixiangedu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gw.9csxet.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xu.bjjhwx.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ni.haigaiapp.cn

[H10] 资源自动释放
来源：http://dz.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://et.huixiangedu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://de.szxytkj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eq.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ik.shtwfgs.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yn.shxzukj.cn

Go:   defer f.Close()
来源：http://uq.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yr.jianghongdianzi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zb.szsharing.cn

================================================================================
来源：http://vb.szsharing.cn

I. 正则表达式
来源：http://sk.panjiajie.cn

================================================================================
来源：http://gr.lnxyls.cn

[I01] 判断是否匹配
来源：http://ty.szxytkj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wk.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vp.521024.cn

JS:   /\d+/.test(s)
来源：http://wn.lnxyls.cn

TS:   /\d+/.test(s)
来源：http://hv.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tw.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mp.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://jt.nszjky.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bt.shxzukj.cn

[I02] 提取所有匹配
来源：http://ll.wgjwhj.cn

Py:   re.findall(r"\d+", s)
来源：http://zj.hnjuh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gd.nszjky.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ci.nszjky.cn

TS:   s.match(/\d+/g)
来源：http://bf.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hx.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://om.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://lb.shxzukj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ts.huixiangedu.cn

[I03] 提取捕获分组
来源：http://ni.huanxung.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tj.nszjky.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ns.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ao.yuntaijiaju.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qd.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tl.shxzskj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://me.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zm.jctech888.com.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://uh.huanxung.cn

[I04] 正则替换
来源：http://ub.nszjky.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rg.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bu.yuntaijiaju.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ic.haigaiapp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wz.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vg.shxzukj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://db.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://tv.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yt.panjiajie.cn

[I05] 按正则拆分
来源：http://dq.huixiangedu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fu.huixinmuqiang.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://um.9csxet.cn

JS:   s.split(/\s*,\s*/)
来源：http://dj.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://xt.yuexingan06.cn

Java: s.split("\\s*,\\s*")
来源：http://do.chemitech.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lm.asd995.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ln.szxytkj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ta.asd995.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ut.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kz.shtwfgs.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://so.yuexingan06.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://en.chemitech.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vs.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nf.huanxung.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mi.gzmigu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xz.bjjhwx.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://nz.newstarts.cn

[I07] 忽略大小写与多行模式
来源：http://bf.haigaiapp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qq.shxzskj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gd.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ah.asd995.cn

TS:   /error/gim
来源：http://ed.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cy.yuntaijiaju.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ek.jctech888.com.cn

Ruby: s.scan(/error/i)
来源：http://et.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oa.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://xv.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pn.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hv.gzmigu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jg.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bt.bookmarksfly.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mx.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sr.9csxet.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hu.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://go.huanxung.cn

================================================================================
来源：http://jv.wgjwhj.cn

J. 日期与时间
来源：http://ml.shtwfgs.cn

================================================================================
来源：http://ro.bookmarksfly.cn

[J01] 获取当前时间
来源：http://kv.wgjwhj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kj.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ns.wgjwhj.cn

JS:   new Date();  Date.now()
来源：http://ew.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://mf.jianghongdianzi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kj.szxytkj.cn

Go:   time.Now()
来源：http://so.colortex.cn

Ruby: Time.now
来源：http://gm.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ww.bookmarksfly.cn

[J02] 格式化输出
来源：http://lw.szxytkj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eh.yuexingan06.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://in.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sg.colortex.cn

TS:   d.toISOString()
来源：http://vo.hnjuh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nx.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ef.bookmarksfly.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uo.9csxet.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sx.hahajie.cn


<!-- 参考信息 -->