代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://ke.yuntaijiaju.cn

[G03] 实例属性
来源：http://dy.szxytkj.cn

Py:   self.name = "x"
来源：http://bi.521024.cn

PHP:  public string $name = "x";
来源：http://ld.gzmigu.cn

JS:   this.name = "x";
来源：http://lq.shxzskj.cn

TS:   name: string = "x";
来源：http://oc.haigaiapp.cn

Java: private String name;
来源：http://zt.shxzskj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dl.huanxung.cn

Ruby: @name = "x"
来源：http://qn.hahajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://cn.huanxung.cn

[G04] 定义方法
来源：http://cn.huanxung.cn

Py:   def greet(self): return self.name
来源：http://yp.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fg.wgjwhj.cn

JS:   greet() { return this.name; }
来源：http://pe.newstarts.cn

TS:   greet(): string { return this.name; }
来源：http://wr.panjiajie.cn

Java: String greet() { return name; }
来源：http://mj.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yu.wgjwhj.cn

Ruby: def greet; @name; end
来源：http://xb.szxytkj.cn

C#:   public string Greet() => Name;
来源：http://ay.hahajie.cn

[G05] 继承
来源：http://hm.shxzskj.cn

Py:   class Admin(User): pass
来源：http://wz.huixiangedu.cn

PHP:  class Admin extends User {}
来源：http://yq.huanxung.cn

JS:   class Admin extends User {}
来源：http://ic.jianghongdianzi.cn

TS:   class Admin extends User {}
来源：http://lm.nicolike.cn

Java: class Admin extends User {}
来源：http://tk.gzmigu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xr.newstarts.cn

Ruby: class Admin < User; end
来源：http://ly.nicolike.cn

C#:   class Admin : User {}
来源：http://ok.huixiangedu.cn

[G06] 重写方法
来源：http://hw.jctech888.com.cn

Py:   def greet(self): return "admin"
来源：http://yf.szxytkj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hy.nszjky.cn

JS:   greet() { return "admin"; }
来源：http://mw.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://pn.bookmarksfly.cn

Java: @Override String greet() { return "admin"; }
来源：http://sf.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kr.bookmarksfly.cn

Ruby: def greet; "admin"; end
来源：http://oo.hnjuh.cn

C#:   public override string Greet() => "admin";
来源：http://dr.huanxung.cn

[G07] 调用父类方法
来源：http://mu.asd995.cn

Py:   super().greet()
来源：http://os.hnjuh.cn

PHP:  parent::greet();
来源：http://fv.newstarts.cn

JS:   super.greet();
来源：http://dt.bjjhwx.cn

TS:   super.greet();
来源：http://yt.hnjuh.cn

Java: super.greet();
来源：http://mq.asd995.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://cq.hnjuh.cn

Ruby: super
来源：http://pz.huanxung.cn

C#:   base.Greet();
来源：http://zr.bookmarksfly.cn

[G08] 静态方法与属性
来源：http://ji.huanxung.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vz.nicolike.cn

PHP:  public static function f() {}
来源：http://aw.gzmigu.cn

JS:   static f() {}
来源：http://tt.bjjhwx.cn

TS:   static f(): void {}
来源：http://xu.hnjuh.cn

Java: static void f() {}
来源：http://mf.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bf.shtwfgs.cn

Ruby: def self.f; end
来源：http://fa.9csxet.cn

C#:   public static void F() {}
来源：http://ek.szsharing.cn

[G09] 接口 / 抽象类
来源：http://cf.wgjwhj.cn

Py:   from abc import ABC, abstractmethod
来源：http://ye.szsharing.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ji.hnjuh.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qv.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://av.newstarts.cn

Java: interface Shape { double area(); }
来源：http://or.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://wg.newstarts.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://iz.shxzskj.cn

C#:   interface IShape { double Area(); }
来源：http://ek.jianghongdianzi.cn

[G10] 访问控制
来源：http://jx.bjjhwx.cn

Py:   约定 _protected / __private（不强制）
来源：http://ln.yuntaijiaju.cn

PHP:  public / protected / private
来源：http://sn.asd995.cn

JS:   #private 字段；其余公开
来源：http://au.lnxyls.cn

TS:   public / protected / private
来源：http://al.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://hy.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://km.gzmigu.cn

Ruby: public / protected / private
来源：http://bn.asd995.cn

C#:   public / protected / private / internal
来源：http://us.shtwfgs.cn

[G11] getter / setter
来源：http://lt.hahajie.cn

Py:   @property 与 @x.setter
来源：http://yr.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vu.asd995.cn

JS:   get name() { return this._name; }
来源：http://jt.hahajie.cn

TS:   get name(): string { return this._name; }
来源：http://gq.521024.cn

Java: public String getName() { return name; }
来源：http://xd.yuntaijiaju.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bk.huanxung.cn

Ruby: attr_accessor :name
来源：http://kb.haigaiapp.cn

C#:   public string Name { get; set; }
来源：http://ee.szxytkj.cn

[G12] 对象转字符串
来源：http://pg.521024.cn

Py:   def __str__(self): return self.name
来源：http://if.yuntaijiaju.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wh.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://ce.asd995.cn

TS:   toString(): string { return this.name; }
来源：http://zd.521024.cn

Java: @Override public String toString() { return name; }
来源：http://jv.wgjwhj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ct.haigaiapp.cn

Ruby: def to_s; @name; end
来源：http://ak.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://pg.9csxet.cn

[G13] 判断对象类型
来源：http://yy.shxzskj.cn

Py:   isinstance(u, User)
来源：http://nc.huanxung.cn

PHP:  $u instanceof User
来源：http://sb.521024.cn

JS:   u instanceof User
来源：http://ff.yuntaijiaju.cn

TS:   u instanceof User
来源：http://tg.gzmigu.cn

Java: u instanceof User
来源：http://xj.jianghongdianzi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://as.huixiangedu.cn

Ruby: u.is_a?(User)
来源：http://hr.colortex.cn

C#:   u is User
来源：http://ix.huixinmuqiang.cn

[G14] 数据类 / record
来源：http://em.521024.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kr.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://zv.bjjhwx.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gg.huixinmuqiang.cn

TS:   type User = { name: string; age: number };
来源：http://sh.colortex.cn

Java: record User(String name, int age) {}
来源：http://lj.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://fx.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cw.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://th.bjjhwx.cn

[G15] 枚举
来源：http://yz.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yi.lnxyls.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kk.yuntaijiaju.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bz.huixiangedu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://er.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://mt.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rw.bookmarksfly.cn

Ruby: Color = %i[red green].freeze
来源：http://lv.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kr.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://bd.panjiajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oq.szxytkj.cn

PHP:  get_object_vars($obj);
来源：http://bn.yuntaijiaju.cn

JS:   Object.entries(obj)
来源：http://un.9csxet.cn

TS:   Object.entries(obj)
来源：http://uz.nicolike.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vj.szxytkj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qn.szxytkj.cn

Ruby: obj.instance_variables
来源：http://yf.szxytkj.cn

C#:   // 用反射或 System.Text.Json
来源：http://vm.asd995.cn

================================================================================
来源：http://fs.jianghongdianzi.cn

H. 异常与错误处理
来源：http://md.chemitech.net.cn

================================================================================
来源：http://ax.hnjuh.cn

[H01] try / catch 基础
来源：http://sz.muxihuayi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oz.szxytkj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pu.jctech888.com.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qt.bookmarksfly.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rp.colortex.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://my.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gr.yuntaijiaju.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mv.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nv.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://zr.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mg.huixiangedu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fs.haigaiapp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ra.nicolike.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bt.colortex.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yx.colortex.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vr.wgjwhj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gi.colortex.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://au.haigaiapp.cn

[H03] 主动抛出异常
来源：http://tx.chemitech.net.cn

Py:   raise ValueError("错误信息")
来源：http://zu.9csxet.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fg.asd995.cn

JS:   throw new Error("错误信息");
来源：http://yx.yuntaijiaju.cn

TS:   throw new Error("错误信息");
来源：http://gc.muxihuayi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ii.haigaiapp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yd.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tp.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://sq.colortex.cn

[H04] 自定义异常类型
来源：http://ni.nszjky.cn

Py:   class MyError(Exception): pass
来源：http://wf.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://oo.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://xo.huixinmuqiang.cn

TS:   class MyError extends Error {}
来源：http://sv.yuntaijiaju.cn

Java: class MyException extends RuntimeException {}
来源：http://qn.nicolike.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xf.colortex.cn

Ruby: class MyError < StandardError; end
来源：http://tz.hnjuh.cn

C#:   class MyException : Exception {}
来源：http://se.yuexingan06.cn

[H05] 捕获特定类型
来源：http://so.shxzukj.cn

Py:   except ValueError as e:
来源：http://sa.lnxyls.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xb.hnjuh.cn

JS:   if (e instanceof TypeError) {}
来源：http://qy.wgjwhj.cn

TS:   if (e instanceof TypeError) {}
来源：http://cv.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://ot.haigaiapp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xq.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://hc.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gc.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://eo.hahajie.cn

Py:   value = d.get("k") or default
来源：http://dw.bjjhwx.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yn.shtwfgs.cn

JS:   obj?.a?.b;  d ?? default
来源：http://te.hahajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rm.jianghongdianzi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://do.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lw.yuexingan06.cn

Ruby: d&.dig(:a, :b)
来源：http://ti.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://bo.shxzukj.cn

[H07] 断言
来源：http://xc.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://ac.nszjky.cn

PHP:  assert($x > 0);
来源：http://ek.huixinmuqiang.cn

JS:   console.assert(x > 0);
来源：http://za.521024.cn

TS:   console.assert(x > 0);
来源：http://jz.gzmigu.cn

Java: assert x > 0 : "必须为正";
来源：http://wj.shxzukj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xu.hnjuh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fg.haigaiapp.cn

C#:   Debug.Assert(x > 0);
来源：http://ah.szsharing.cn

[H08] 获取错误信息与堆栈
来源：http://vp.9csxet.cn

Py:   str(e);  traceback.format_exc()
来源：http://xt.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://be.jianghongdianzi.cn

JS:   e.message;  e.stack
来源：http://kj.shxzukj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kv.jianghongdianzi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gw.shxzskj.cn

Go:   err.Error()
来源：http://ds.jctech888.com.cn

Ruby: e.message;  e.backtrace
来源：http://ih.huanxung.cn

C#:   e.Message;  e.StackTrace
来源：http://ug.huixiangedu.cn

[H09] 带错误码的异常
来源：http://vg.bookmarksfly.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://up.muxihuayi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zq.asd995.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ht.newstarts.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mh.shxzskj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qe.huanxung.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zq.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dk.wgjwhj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bw.yuexingan06.cn

[H10] 资源自动释放
来源：http://vw.521024.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://nl.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xn.huixinmuqiang.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ai.huixiangedu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://md.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oi.bookmarksfly.cn

Go:   defer f.Close()
来源：http://ek.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gu.yuntaijiaju.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wr.shxzukj.cn

================================================================================
来源：http://kw.shxzukj.cn

I. 正则表达式
来源：http://kj.szsharing.cn

================================================================================
来源：http://sj.muxihuayi.cn

[I01] 判断是否匹配
来源：http://ly.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wi.hnjuh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tz.jianghongdianzi.cn

JS:   /\d+/.test(s)
来源：http://hb.hnjuh.cn

TS:   /\d+/.test(s)
来源：http://qo.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xb.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qs.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://tt.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wg.panjiajie.cn

[I02] 提取所有匹配
来源：http://wk.muxihuayi.cn

Py:   re.findall(r"\d+", s)
来源：http://rs.lnxyls.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://au.asd995.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rj.hnjuh.cn

TS:   s.match(/\d+/g)
来源：http://jq.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yp.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://av.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://du.newstarts.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://la.chemitech.net.cn

[I03] 提取捕获分组
来源：http://km.jianghongdianzi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xc.szxytkj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ba.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cd.shxzskj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rw.9csxet.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hi.panjiajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://is.shxzskj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ib.newstarts.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gb.9csxet.cn

[I04] 正则替换
来源：http://ro.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yk.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ek.huixinmuqiang.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fl.szsharing.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ax.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sp.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zu.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kr.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lx.haigaiapp.cn

[I05] 按正则拆分
来源：http://zx.hahajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pj.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tr.asd995.cn

JS:   s.split(/\s*,\s*/)
来源：http://ir.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://mh.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://wx.asd995.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hv.muxihuayi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xs.chemitech.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zz.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mh.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ie.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nu.lnxyls.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tt.wgjwhj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ho.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qg.newstarts.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bi.hnjuh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lj.newstarts.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cm.huanxung.cn

[I07] 忽略大小写与多行模式
来源：http://xx.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://da.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gg.yuexingan06.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.asd995.cn

TS:   /error/gim
来源：http://to.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mp.521024.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://os.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://tk.bookmarksfly.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qu.shxzskj.cn

[I08] 贪婪与非贪婪匹配
来源：http://jr.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://os.gzmigu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xt.shxzskj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rg.huixinmuqiang.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dr.jctech888.com.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yb.jianghongdianzi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yu.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lm.gzmigu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://su.lnxyls.cn

================================================================================
来源：http://wd.yuexingan06.cn

J. 日期与时间
来源：http://jj.hahajie.cn

================================================================================
来源：http://ba.yuntaijiaju.cn

[J01] 获取当前时间
来源：http://fu.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ba.shtwfgs.cn


<!-- 参考信息 -->