代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://lr.haigaiapp.cn

[G03] 实例属性
来源：http://zk.haigaiapp.cn

Py:   self.name = "x"
来源：http://jj.bjjhwx.cn

PHP:  public string $name = "x";
来源：http://oi.szsharing.cn

JS:   this.name = "x";
来源：http://pg.shxzukj.cn

TS:   name: string = "x";
来源：http://yj.haigaiapp.cn

Java: private String name;
来源：http://dp.panjiajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://oc.nicolike.cn

Ruby: @name = "x"
来源：http://an.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://vm.colortex.cn

[G04] 定义方法
来源：http://kf.asd995.cn

Py:   def greet(self): return self.name
来源：http://hr.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://co.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://zx.jctech888.com.cn

TS:   greet(): string { return this.name; }
来源：http://je.521024.cn

Java: String greet() { return name; }
来源：http://hf.szsharing.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ak.bookmarksfly.cn

Ruby: def greet; @name; end
来源：http://ti.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://vn.shxzskj.cn

[G05] 继承
来源：http://rr.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://zi.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://eb.szxytkj.cn

JS:   class Admin extends User {}
来源：http://iq.chemitech.net.cn

TS:   class Admin extends User {}
来源：http://gk.chemitech.net.cn

Java: class Admin extends User {}
来源：http://rb.huixinmuqiang.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tj.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://xa.haigaiapp.cn

C#:   class Admin : User {}
来源：http://kv.panjiajie.cn

[G06] 重写方法
来源：http://av.panjiajie.cn

Py:   def greet(self): return "admin"
来源：http://cd.haigaiapp.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cy.521024.cn

JS:   greet() { return "admin"; }
来源：http://iv.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://bt.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://wq.521024.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ys.shtwfgs.cn

Ruby: def greet; "admin"; end
来源：http://vh.shtwfgs.cn

C#:   public override string Greet() => "admin";
来源：http://su.hahajie.cn

[G07] 调用父类方法
来源：http://kk.shtwfgs.cn

Py:   super().greet()
来源：http://cq.bjjhwx.cn

PHP:  parent::greet();
来源：http://uf.nszjky.cn

JS:   super.greet();
来源：http://ym.shxzskj.cn

TS:   super.greet();
来源：http://ri.panjiajie.cn

Java: super.greet();
来源：http://yo.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://da.shtwfgs.cn

Ruby: super
来源：http://iu.nicolike.cn

C#:   base.Greet();
来源：http://iq.hahajie.cn

[G08] 静态方法与属性
来源：http://wb.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ve.panjiajie.cn

PHP:  public static function f() {}
来源：http://bk.asd995.cn

JS:   static f() {}
来源：http://bi.colortex.cn

TS:   static f(): void {}
来源：http://yt.yuntaijiaju.cn

Java: static void f() {}
来源：http://dg.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bv.huixinmuqiang.cn

Ruby: def self.f; end
来源：http://ju.huixinmuqiang.cn

C#:   public static void F() {}
来源：http://ds.chemitech.net.cn

[G09] 接口 / 抽象类
来源：http://rr.nicolike.cn

Py:   from abc import ABC, abstractmethod
来源：http://gv.jctech888.com.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bd.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lw.jctech888.com.cn

TS:   interface Shape { area(): number; }
来源：http://fc.shxzukj.cn

Java: interface Shape { double area(); }
来源：http://if.huanxung.cn

Go:   type Shape interface { Area() float64 }
来源：http://qr.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ul.szxytkj.cn

C#:   interface IShape { double Area(); }
来源：http://ot.nicolike.cn

[G10] 访问控制
来源：http://kg.huixinmuqiang.cn

Py:   约定 _protected / __private（不强制）
来源：http://mc.yuexingan06.cn

PHP:  public / protected / private
来源：http://jm.gzmigu.cn

JS:   #private 字段；其余公开
来源：http://pc.jianghongdianzi.cn

TS:   public / protected / private
来源：http://nj.shxzukj.cn

Java: public / protected / private / 默认包级
来源：http://fb.yuexingan06.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nc.haigaiapp.cn

Ruby: public / protected / private
来源：http://dz.gzmigu.cn

C#:   public / protected / private / internal
来源：http://zh.yuexingan06.cn

[G11] getter / setter
来源：http://mo.muxihuayi.cn

Py:   @property 与 @x.setter
来源：http://qs.szsharing.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hn.shxzskj.cn

JS:   get name() { return this._name; }
来源：http://hx.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://zh.jianghongdianzi.cn

Java: public String getName() { return name; }
来源：http://mn.haigaiapp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ox.shxzukj.cn

Ruby: attr_accessor :name
来源：http://pg.yuntaijiaju.cn

C#:   public string Name { get; set; }
来源：http://ia.yuexingan06.cn

[G12] 对象转字符串
来源：http://ov.521024.cn

Py:   def __str__(self): return self.name
来源：http://bj.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ii.yuntaijiaju.cn

JS:   toString() { return this.name; }
来源：http://ca.panjiajie.cn

TS:   toString(): string { return this.name; }
来源：http://rp.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://rj.lnxyls.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hf.shtwfgs.cn

Ruby: def to_s; @name; end
来源：http://qk.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://el.colortex.cn

[G13] 判断对象类型
来源：http://qv.jctech888.com.cn

Py:   isinstance(u, User)
来源：http://vk.huanxung.cn

PHP:  $u instanceof User
来源：http://oh.newstarts.cn

JS:   u instanceof User
来源：http://ua.shxzukj.cn

TS:   u instanceof User
来源：http://is.muxihuayi.cn

Java: u instanceof User
来源：http://yc.shxzukj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mk.chemitech.net.cn

Ruby: u.is_a?(User)
来源：http://mj.huixinmuqiang.cn

C#:   u is User
来源：http://tj.gzmigu.cn

[G14] 数据类 / record
来源：http://km.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qe.yuntaijiaju.cn

PHP:  // 用 readonly 属性模拟
来源：http://wc.shxzukj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://di.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://km.gzmigu.cn

Java: record User(String name, int age) {}
来源：http://hq.haigaiapp.cn

Go:   type User struct { Name string; Age int }
来源：http://uv.521024.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uh.panjiajie.cn

C#:   record User(string Name, int Age);
来源：http://ys.hahajie.cn

[G15] 枚举
来源：http://mc.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ag.9csxet.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://te.muxihuayi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://oa.yuntaijiaju.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bd.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://bb.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://eb.newstarts.cn

Ruby: Color = %i[red green].freeze
来源：http://qn.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ba.jctech888.com.cn

[G16] 对象转数组 / 字典
来源：http://hb.shxzskj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qu.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://av.shxzukj.cn

JS:   Object.entries(obj)
来源：http://vs.muxihuayi.cn

TS:   Object.entries(obj)
来源：http://xq.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tr.lnxyls.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mj.shxzukj.cn

Ruby: obj.instance_variables
来源：http://pj.bjjhwx.cn

C#:   // 用反射或 System.Text.Json
来源：http://wd.jianghongdianzi.cn

================================================================================
来源：http://gh.521024.cn

H. 异常与错误处理
来源：http://ru.hahajie.cn

================================================================================
来源：http://ck.panjiajie.cn

[H01] try / catch 基础
来源：http://ja.huixinmuqiang.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uy.bjjhwx.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://te.panjiajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pg.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wy.huixiangedu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jh.muxihuayi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jr.huanxung.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kj.asd995.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gv.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://uw.szxytkj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://az.muxihuayi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vd.bjjhwx.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rs.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fm.shtwfgs.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wv.asd995.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://so.bookmarksfly.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://je.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pa.hnjuh.cn

[H03] 主动抛出异常
来源：http://wi.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://iy.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dw.nicolike.cn

JS:   throw new Error("错误信息");
来源：http://ub.szsharing.cn

TS:   throw new Error("错误信息");
来源：http://ir.hahajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rv.szsharing.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lr.haigaiapp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fb.newstarts.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ry.panjiajie.cn

[H04] 自定义异常类型
来源：http://dl.newstarts.cn

Py:   class MyError(Exception): pass
来源：http://yi.9csxet.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tm.shxzskj.cn

JS:   class MyError extends Error {}
来源：http://hb.nszjky.cn

TS:   class MyError extends Error {}
来源：http://ab.chemitech.net.cn

Java: class MyException extends RuntimeException {}
来源：http://ks.huixiangedu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://os.nicolike.cn

Ruby: class MyError < StandardError; end
来源：http://ji.huixiangedu.cn

C#:   class MyException : Exception {}
来源：http://dq.hahajie.cn

[H05] 捕获特定类型
来源：http://rx.szxytkj.cn

Py:   except ValueError as e:
来源：http://gu.muxihuayi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tr.shxzskj.cn

JS:   if (e instanceof TypeError) {}
来源：http://et.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://nq.yuntaijiaju.cn

Java: catch (IOException | SQLException e) {}
来源：http://ug.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cf.nicolike.cn

Ruby: rescue ArgumentError => e
来源：http://cu.bookmarksfly.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ul.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://dl.jianghongdianzi.cn

Py:   value = d.get("k") or default
来源：http://eq.yuexingan06.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fk.haigaiapp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bh.yuexingan06.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zr.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ni.szsharing.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mq.jctech888.com.cn

Ruby: d&.dig(:a, :b)
来源：http://ti.panjiajie.cn

C#:   obj?.A?.B ?? default
来源：http://hw.lnxyls.cn

[H07] 断言
来源：http://fb.jianghongdianzi.cn

Py:   assert x > 0, "必须为正"
来源：http://xc.shtwfgs.cn

PHP:  assert($x > 0);
来源：http://ax.wgjwhj.cn

JS:   console.assert(x > 0);
来源：http://cw.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://pb.shxzskj.cn

Java: assert x > 0 : "必须为正";
来源：http://re.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jx.huanxung.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zw.bjjhwx.cn

C#:   Debug.Assert(x > 0);
来源：http://wy.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://nq.huanxung.cn

Py:   str(e);  traceback.format_exc()
来源：http://pl.jctech888.com.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xi.newstarts.cn

JS:   e.message;  e.stack
来源：http://sb.lnxyls.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vm.shtwfgs.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dj.gzmigu.cn

Go:   err.Error()
来源：http://bs.szxytkj.cn

Ruby: e.message;  e.backtrace
来源：http://fg.bjjhwx.cn

C#:   e.Message;  e.StackTrace
来源：http://nx.bjjhwx.cn

[H09] 带错误码的异常
来源：http://uz.yuntaijiaju.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sf.wgjwhj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yw.chemitech.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fx.lnxyls.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rb.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ag.szsharing.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cq.shxzskj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://do.haigaiapp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wf.muxihuayi.cn

[H10] 资源自动释放
来源：http://nu.muxihuayi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cx.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gg.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sb.szsharing.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://us.hnjuh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lf.shtwfgs.cn

Go:   defer f.Close()
来源：http://qz.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://up.szxytkj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fr.nszjky.cn

================================================================================
来源：http://bm.newstarts.cn

I. 正则表达式
来源：http://kg.muxihuayi.cn

================================================================================
来源：http://wi.nszjky.cn

[I01] 判断是否匹配
来源：http://zi.wgjwhj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xy.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zx.nicolike.cn

JS:   /\d+/.test(s)
来源：http://la.asd995.cn

TS:   /\d+/.test(s)
来源：http://qh.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bq.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wx.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://ob.shxzukj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ym.wgjwhj.cn

[I02] 提取所有匹配
来源：http://gb.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://cm.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wd.521024.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gy.wgjwhj.cn

TS:   s.match(/\d+/g)
来源：http://fx.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nj.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vi.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://eo.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dq.9csxet.cn

[I03] 提取捕获分组
来源：http://ln.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mj.newstarts.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ob.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://eo.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zs.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://py.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bs.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://so.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pm.shxzukj.cn

[I04] 正则替换
来源：http://mf.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yb.yuexingan06.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dd.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zd.hnjuh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://st.szsharing.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vm.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://im.nszjky.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zn.shxzukj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wz.huixinmuqiang.cn

[I05] 按正则拆分
来源：http://zj.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yl.yuexingan06.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gs.lnxyls.cn

JS:   s.split(/\s*,\s*/)
来源：http://mk.szsharing.cn

TS:   s.split(/\s*,\s*/)
来源：http://rw.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://rv.jctech888.com.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ph.muxihuayi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cv.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ls.wgjwhj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qt.szsharing.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ds.nszjky.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hn.jianghongdianzi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fi.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ea.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gh.jctech888.com.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://aq.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xu.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mj.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://ka.haigaiapp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://my.shxzukj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lp.panjiajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rf.nszjky.cn

TS:   /error/gim
来源：http://iy.shxzskj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hu.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bk.hnjuh.cn

Ruby: s.scan(/error/i)
来源：http://go.huanxung.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://da.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://ca.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lh.hahajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lz.9csxet.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wj.gzmigu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ek.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://pg.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rx.huanxung.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yw.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://do.haigaiapp.cn

================================================================================
来源：http://mc.asd995.cn

J. 日期与时间
来源：http://eo.yuexingan06.cn

================================================================================
来源：http://hg.gzmigu.cn

[J01] 获取当前时间
来源：http://jt.haigaiapp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fa.nicolike.cn


<!-- 参考信息 -->