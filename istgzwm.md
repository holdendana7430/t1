代发 wailian999

JS:   this.name = "x";
来源：http://fl.huixiangedu.cn

TS:   name: string = "x";
来源：http://vd.shxzskj.cn

Java: private String name;
来源：http://dl.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mb.szsharing.cn

Ruby: @name = "x"
来源：http://dq.haigaiapp.cn

C#:   public string Name { get; set; } = "x";
来源：http://uo.bookmarksfly.cn

[G04] 定义方法
来源：http://ds.szxytkj.cn

Py:   def greet(self): return self.name
来源：http://qh.nicolike.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://go.huixiangedu.cn

JS:   greet() { return this.name; }
来源：http://mb.bjjhwx.cn

TS:   greet(): string { return this.name; }
来源：http://xl.jianghongdianzi.cn

Java: String greet() { return name; }
来源：http://gp.asd995.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ly.hahajie.cn

Ruby: def greet; @name; end
来源：http://ft.wgjwhj.cn

C#:   public string Greet() => Name;
来源：http://pu.bookmarksfly.cn

[G05] 继承
来源：http://vp.521024.cn

Py:   class Admin(User): pass
来源：http://ck.jianghongdianzi.cn

PHP:  class Admin extends User {}
来源：http://dz.nszjky.cn

JS:   class Admin extends User {}
来源：http://vg.lnxyls.cn

TS:   class Admin extends User {}
来源：http://fo.shtwfgs.cn

Java: class Admin extends User {}
来源：http://az.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jf.szsharing.cn

Ruby: class Admin < User; end
来源：http://yb.lnxyls.cn

C#:   class Admin : User {}
来源：http://so.yuntaijiaju.cn

[G06] 重写方法
来源：http://ci.shxzskj.cn

Py:   def greet(self): return "admin"
来源：http://ge.haigaiapp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jn.9csxet.cn

JS:   greet() { return "admin"; }
来源：http://fz.jianghongdianzi.cn

TS:   greet(): string { return "admin"; }
来源：http://vf.shxzskj.cn

Java: @Override String greet() { return "admin"; }
来源：http://jf.huixiangedu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xo.chemitech.net.cn

Ruby: def greet; "admin"; end
来源：http://qc.yuexingan06.cn

C#:   public override string Greet() => "admin";
来源：http://ln.521024.cn

[G07] 调用父类方法
来源：http://fp.huanxung.cn

Py:   super().greet()
来源：http://or.chemitech.net.cn

PHP:  parent::greet();
来源：http://na.nszjky.cn

JS:   super.greet();
来源：http://mp.yuntaijiaju.cn

TS:   super.greet();
来源：http://jf.9csxet.cn

Java: super.greet();
来源：http://qa.shxzukj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://di.nszjky.cn

Ruby: super
来源：http://ap.hnjuh.cn

C#:   base.Greet();
来源：http://vv.muxihuayi.cn

[G08] 静态方法与属性
来源：http://wj.szxytkj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fa.colortex.cn

PHP:  public static function f() {}
来源：http://ob.bookmarksfly.cn

JS:   static f() {}
来源：http://xu.newstarts.cn

TS:   static f(): void {}
来源：http://zf.gzmigu.cn

Java: static void f() {}
来源：http://pd.muxihuayi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fu.gzmigu.cn

Ruby: def self.f; end
来源：http://hb.gzmigu.cn

C#:   public static void F() {}
来源：http://tm.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://fi.521024.cn

Py:   from abc import ABC, abstractmethod
来源：http://ka.shxzskj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pa.yuexingan06.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://oe.9csxet.cn

TS:   interface Shape { area(): number; }
来源：http://nz.nicolike.cn

Java: interface Shape { double area(); }
来源：http://qe.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://op.szsharing.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dh.panjiajie.cn

C#:   interface IShape { double Area(); }
来源：http://ae.9csxet.cn

[G10] 访问控制
来源：http://yn.szxytkj.cn

Py:   约定 _protected / __private（不强制）
来源：http://pq.asd995.cn

PHP:  public / protected / private
来源：http://uw.yuntaijiaju.cn

JS:   #private 字段；其余公开
来源：http://xe.huanxung.cn

TS:   public / protected / private
来源：http://gi.huanxung.cn

Java: public / protected / private / 默认包级
来源：http://fw.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jd.bjjhwx.cn

Ruby: public / protected / private
来源：http://le.colortex.cn

C#:   public / protected / private / internal
来源：http://eq.hnjuh.cn

[G11] getter / setter
来源：http://cb.shxzukj.cn

Py:   @property 与 @x.setter
来源：http://pj.szsharing.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qj.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://xl.nszjky.cn

TS:   get name(): string { return this._name; }
来源：http://ix.haigaiapp.cn

Java: public String getName() { return name; }
来源：http://qw.szsharing.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pq.gzmigu.cn

Ruby: attr_accessor :name
来源：http://yb.9csxet.cn

C#:   public string Name { get; set; }
来源：http://kp.shxzskj.cn

[G12] 对象转字符串
来源：http://sf.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://zp.chemitech.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fx.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://qn.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://yl.szsharing.cn

Java: @Override public String toString() { return name; }
来源：http://hv.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jr.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://re.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://rs.huixiangedu.cn

[G13] 判断对象类型
来源：http://ej.newstarts.cn

Py:   isinstance(u, User)
来源：http://yk.nicolike.cn

PHP:  $u instanceof User
来源：http://rh.9csxet.cn

JS:   u instanceof User
来源：http://qp.lnxyls.cn

TS:   u instanceof User
来源：http://zk.gzmigu.cn

Java: u instanceof User
来源：http://ja.chemitech.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ss.bjjhwx.cn

Ruby: u.is_a?(User)
来源：http://qj.9csxet.cn

C#:   u is User
来源：http://fp.chemitech.net.cn

[G14] 数据类 / record
来源：http://ro.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bw.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://he.yuexingan06.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sq.haigaiapp.cn

TS:   type User = { name: string; age: number };
来源：http://au.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://ig.lnxyls.cn

Go:   type User struct { Name string; Age int }
来源：http://lx.szsharing.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://du.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://kg.muxihuayi.cn

[G15] 枚举
来源：http://zq.bjjhwx.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://um.bjjhwx.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://la.wgjwhj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bj.bjjhwx.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xu.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://bg.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rv.9csxet.cn

Ruby: Color = %i[red green].freeze
来源：http://ie.hnjuh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ca.nszjky.cn

[G16] 对象转数组 / 字典
来源：http://gq.bookmarksfly.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ie.shxzskj.cn

PHP:  get_object_vars($obj);
来源：http://fg.newstarts.cn

JS:   Object.entries(obj)
来源：http://tu.nszjky.cn

TS:   Object.entries(obj)
来源：http://jm.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://og.newstarts.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://eg.szsharing.cn

Ruby: obj.instance_variables
来源：http://rr.colortex.cn

C#:   // 用反射或 System.Text.Json
来源：http://fy.521024.cn

================================================================================
来源：http://ll.szxytkj.cn

H. 异常与错误处理
来源：http://ha.muxihuayi.cn

================================================================================
来源：http://dw.yuexingan06.cn

[H01] try / catch 基础
来源：http://bf.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wk.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://co.huixiangedu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://th.shxzskj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nx.gzmigu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xk.bookmarksfly.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mq.521024.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ei.asd995.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uu.shxzskj.cn

[H02] finally / ensure 收尾
来源：http://am.bookmarksfly.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xv.gzmigu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vz.9csxet.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vd.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://sy.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lo.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ym.muxihuayi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ny.wgjwhj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ka.newstarts.cn

[H03] 主动抛出异常
来源：http://mn.shxzukj.cn

Py:   raise ValueError("错误信息")
来源：http://mb.hahajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ek.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://cx.asd995.cn

TS:   throw new Error("错误信息");
来源：http://dd.jctech888.com.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://eb.chemitech.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://np.huixiangedu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zq.newstarts.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zu.colortex.cn

[H04] 自定义异常类型
来源：http://zm.szsharing.cn

Py:   class MyError(Exception): pass
来源：http://qm.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nt.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://po.jianghongdianzi.cn

TS:   class MyError extends Error {}
来源：http://cm.shxzskj.cn

Java: class MyException extends RuntimeException {}
来源：http://cy.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lq.panjiajie.cn

Ruby: class MyError < StandardError; end
来源：http://za.jctech888.com.cn

C#:   class MyException : Exception {}
来源：http://cm.nicolike.cn

[H05] 捕获特定类型
来源：http://db.hnjuh.cn

Py:   except ValueError as e:
来源：http://vj.asd995.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pb.lnxyls.cn

JS:   if (e instanceof TypeError) {}
来源：http://bt.bjjhwx.cn

TS:   if (e instanceof TypeError) {}
来源：http://mq.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://fh.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gx.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://cx.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ce.chemitech.net.cn

[H06] 可选值 / 空值安全访问
来源：http://di.lnxyls.cn

Py:   value = d.get("k") or default
来源：http://zy.huixiangedu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zl.521024.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qw.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://oj.nicolike.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mt.9csxet.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://om.yuntaijiaju.cn

Ruby: d&.dig(:a, :b)
来源：http://ph.shtwfgs.cn

C#:   obj?.A?.B ?? default
来源：http://qs.hahajie.cn

[H07] 断言
来源：http://fw.yuntaijiaju.cn

Py:   assert x > 0, "必须为正"
来源：http://io.panjiajie.cn

PHP:  assert($x > 0);
来源：http://ym.chemitech.net.cn

JS:   console.assert(x > 0);
来源：http://py.muxihuayi.cn

TS:   console.assert(x > 0);
来源：http://gb.szsharing.cn

Java: assert x > 0 : "必须为正";
来源：http://pn.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rl.bookmarksfly.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wj.gzmigu.cn

C#:   Debug.Assert(x > 0);
来源：http://uo.jctech888.com.cn

[H08] 获取错误信息与堆栈
来源：http://td.panjiajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://cv.asd995.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fh.wgjwhj.cn

JS:   e.message;  e.stack
来源：http://ml.huixiangedu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://se.chemitech.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ut.bookmarksfly.cn

Go:   err.Error()
来源：http://od.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://uh.hahajie.cn

C#:   e.Message;  e.StackTrace
来源：http://dl.shxzskj.cn

[H09] 带错误码的异常
来源：http://im.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cu.shtwfgs.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://sc.9csxet.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ew.shxzskj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ly.colortex.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xx.newstarts.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yo.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://np.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kk.huixiangedu.cn

[H10] 资源自动释放
来源：http://ti.nicolike.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rm.yuexingan06.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wx.szsharing.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wi.bookmarksfly.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mb.bookmarksfly.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mj.nszjky.cn

Go:   defer f.Close()
来源：http://au.asd995.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vs.nszjky.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ga.yuntaijiaju.cn

================================================================================
来源：http://rx.huixinmuqiang.cn

I. 正则表达式
来源：http://sp.bjjhwx.cn

================================================================================
来源：http://pg.haigaiapp.cn

[I01] 判断是否匹配
来源：http://oo.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://eu.newstarts.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zl.shxzskj.cn

JS:   /\d+/.test(s)
来源：http://xc.huanxung.cn

TS:   /\d+/.test(s)
来源：http://gz.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uh.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://af.shtwfgs.cn

Ruby: s.match?(/\d+/)
来源：http://if.chemitech.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dp.jianghongdianzi.cn

[I02] 提取所有匹配
来源：http://sb.newstarts.cn

Py:   re.findall(r"\d+", s)
来源：http://nx.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ty.panjiajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ey.lnxyls.cn

TS:   s.match(/\d+/g)
来源：http://dk.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mu.nszjky.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ow.yuexingan06.cn

Ruby: s.scan(/\d+/)
来源：http://gs.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://si.huanxung.cn

[I03] 提取捕获分组
来源：http://ft.hahajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rc.9csxet.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wy.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://at.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bn.huixiangedu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kp.yuexingan06.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ya.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ww.shxzskj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pj.521024.cn

[I04] 正则替换
来源：http://ox.wgjwhj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://by.szsharing.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fs.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jr.hnjuh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vi.muxihuayi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://eq.muxihuayi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zf.jctech888.com.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://dd.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pn.wgjwhj.cn

[I05] 按正则拆分
来源：http://qg.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ug.nszjky.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pn.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://jf.bookmarksfly.cn

TS:   s.split(/\s*,\s*/)
来源：http://yw.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://jo.huixiangedu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hb.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zf.muxihuayi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://aw.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zg.newstarts.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ao.szxytkj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sn.huixiangedu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://br.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yg.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cn.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zt.huixiangedu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hx.shxzukj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ol.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://ea.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rx.nszjky.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jt.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xc.hnjuh.cn

TS:   /error/gim
来源：http://up.yuntaijiaju.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ob.szsharing.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pm.shxzskj.cn

Ruby: s.scan(/error/i)
来源：http://rf.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://eh.gzmigu.cn

[I08] 贪婪与非贪婪匹配
来源：http://le.huanxung.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tk.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ze.bookmarksfly.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bw.huanxung.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://iy.yuexingan06.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://px.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wt.newstarts.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://iv.shxzskj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wv.huixinmuqiang.cn

================================================================================
来源：http://rl.jianghongdianzi.cn

J. 日期与时间
来源：http://ru.lnxyls.cn

================================================================================
来源：http://mc.shtwfgs.cn

[J01] 获取当前时间
来源：http://nk.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bs.shtwfgs.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fs.lnxyls.cn

JS:   new Date();  Date.now()
来源：http://bn.newstarts.cn

TS:   new Date();  Date.now()
来源：http://jk.shxzskj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ul.jctech888.com.cn


<!-- 参考信息 -->