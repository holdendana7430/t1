代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://zm.shxzukj.cn

Ruby: def greet; @name; end
来源：http://ml.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://qi.nicolike.cn

[G05] 继承
来源：http://yo.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://nv.shtwfgs.cn

PHP:  class Admin extends User {}
来源：http://ww.colortex.cn

JS:   class Admin extends User {}
来源：http://rm.bookmarksfly.cn

TS:   class Admin extends User {}
来源：http://wu.panjiajie.cn

Java: class Admin extends User {}
来源：http://rp.huanxung.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://og.panjiajie.cn

Ruby: class Admin < User; end
来源：http://bq.shtwfgs.cn

C#:   class Admin : User {}
来源：http://ox.shxzskj.cn

[G06] 重写方法
来源：http://jq.colortex.cn

Py:   def greet(self): return "admin"
来源：http://jm.panjiajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fj.hnjuh.cn

JS:   greet() { return "admin"; }
来源：http://dc.hahajie.cn

TS:   greet(): string { return "admin"; }
来源：http://jz.huixinmuqiang.cn

Java: @Override String greet() { return "admin"; }
来源：http://bb.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tn.jianghongdianzi.cn

Ruby: def greet; "admin"; end
来源：http://ll.yuntaijiaju.cn

C#:   public override string Greet() => "admin";
来源：http://ut.nicolike.cn

[G07] 调用父类方法
来源：http://hb.szxytkj.cn

Py:   super().greet()
来源：http://hg.yuexingan06.cn

PHP:  parent::greet();
来源：http://hb.huixinmuqiang.cn

JS:   super.greet();
来源：http://yt.hnjuh.cn

TS:   super.greet();
来源：http://rg.nszjky.cn

Java: super.greet();
来源：http://oh.shtwfgs.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://om.9csxet.cn

Ruby: super
来源：http://fo.huanxung.cn

C#:   base.Greet();
来源：http://sq.shxzukj.cn

[G08] 静态方法与属性
来源：http://iu.9csxet.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://iu.colortex.cn

PHP:  public static function f() {}
来源：http://ri.chemitech.net.cn

JS:   static f() {}
来源：http://us.huanxung.cn

TS:   static f(): void {}
来源：http://bl.hnjuh.cn

Java: static void f() {}
来源：http://mz.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mg.nicolike.cn

Ruby: def self.f; end
来源：http://ii.szsharing.cn

C#:   public static void F() {}
来源：http://jx.newstarts.cn

[G09] 接口 / 抽象类
来源：http://tm.haigaiapp.cn

Py:   from abc import ABC, abstractmethod
来源：http://vx.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nt.jctech888.com.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zw.bookmarksfly.cn

TS:   interface Shape { area(): number; }
来源：http://fm.wgjwhj.cn

Java: interface Shape { double area(); }
来源：http://qh.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://lj.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://in.shtwfgs.cn

C#:   interface IShape { double Area(); }
来源：http://yf.wgjwhj.cn

[G10] 访问控制
来源：http://yw.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://qz.lnxyls.cn

PHP:  public / protected / private
来源：http://qn.lnxyls.cn

JS:   #private 字段；其余公开
来源：http://he.gzmigu.cn

TS:   public / protected / private
来源：http://ym.gzmigu.cn

Java: public / protected / private / 默认包级
来源：http://iq.hnjuh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ee.chemitech.net.cn

Ruby: public / protected / private
来源：http://bg.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://zx.jctech888.com.cn

[G11] getter / setter
来源：http://ti.wgjwhj.cn

Py:   @property 与 @x.setter
来源：http://ht.newstarts.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sa.huanxung.cn

JS:   get name() { return this._name; }
来源：http://nq.muxihuayi.cn

TS:   get name(): string { return this._name; }
来源：http://el.colortex.cn

Java: public String getName() { return name; }
来源：http://ui.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tv.newstarts.cn

Ruby: attr_accessor :name
来源：http://vu.nicolike.cn

C#:   public string Name { get; set; }
来源：http://pf.yuexingan06.cn

[G12] 对象转字符串
来源：http://jb.szsharing.cn

Py:   def __str__(self): return self.name
来源：http://tb.asd995.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jp.yuexingan06.cn

JS:   toString() { return this.name; }
来源：http://cu.jianghongdianzi.cn

TS:   toString(): string { return this.name; }
来源：http://my.gzmigu.cn

Java: @Override public String toString() { return name; }
来源：http://oj.huixinmuqiang.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bn.colortex.cn

Ruby: def to_s; @name; end
来源：http://qj.haigaiapp.cn

C#:   public override string ToString() => Name;
来源：http://qr.bjjhwx.cn

[G13] 判断对象类型
来源：http://ok.szxytkj.cn

Py:   isinstance(u, User)
来源：http://sj.521024.cn

PHP:  $u instanceof User
来源：http://zn.muxihuayi.cn

JS:   u instanceof User
来源：http://dz.lnxyls.cn

TS:   u instanceof User
来源：http://qt.nszjky.cn

Java: u instanceof User
来源：http://jj.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qa.9csxet.cn

Ruby: u.is_a?(User)
来源：http://ow.shxzukj.cn

C#:   u is User
来源：http://pj.shxzskj.cn

[G14] 数据类 / record
来源：http://kj.asd995.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lb.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://th.yuntaijiaju.cn

JS:   // 无内置：普通类或对象字面量
来源：http://go.panjiajie.cn

TS:   type User = { name: string; age: number };
来源：http://fu.yuntaijiaju.cn

Java: record User(String name, int age) {}
来源：http://li.yuexingan06.cn

Go:   type User struct { Name string; Age int }
来源：http://fj.muxihuayi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bl.nicolike.cn

C#:   record User(string Name, int Age);
来源：http://wd.huixiangedu.cn

[G15] 枚举
来源：http://ij.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mi.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fz.szsharing.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zf.muxihuayi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tn.hnjuh.cn

Java: enum Color { RED, GREEN }
来源：http://yu.colortex.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://in.bjjhwx.cn

Ruby: Color = %i[red green].freeze
来源：http://tz.lnxyls.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mn.lnxyls.cn

[G16] 对象转数组 / 字典
来源：http://ic.bookmarksfly.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ld.jianghongdianzi.cn

PHP:  get_object_vars($obj);
来源：http://si.gzmigu.cn

JS:   Object.entries(obj)
来源：http://dc.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://tf.shtwfgs.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xs.jianghongdianzi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ad.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://cw.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://vo.bookmarksfly.cn

================================================================================
来源：http://pg.hahajie.cn

H. 异常与错误处理
来源：http://av.521024.cn

================================================================================
来源：http://zz.hahajie.cn

[H01] try / catch 基础
来源：http://ix.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sj.huixiangedu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ak.chemitech.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lw.lnxyls.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rv.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bz.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yn.gzmigu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ix.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ti.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://wb.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vw.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rw.shtwfgs.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fv.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ru.nicolike.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vo.wgjwhj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zt.shxzukj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wz.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ho.muxihuayi.cn

[H03] 主动抛出异常
来源：http://lb.shxzukj.cn

Py:   raise ValueError("错误信息")
来源：http://gm.chemitech.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wq.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://gk.szxytkj.cn

TS:   throw new Error("错误信息");
来源：http://pt.jianghongdianzi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ml.nszjky.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fz.szsharing.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qk.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tr.yuexingan06.cn

[H04] 自定义异常类型
来源：http://rr.shtwfgs.cn

Py:   class MyError(Exception): pass
来源：http://cc.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rp.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://bb.muxihuayi.cn

TS:   class MyError extends Error {}
来源：http://fh.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://hk.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ds.nicolike.cn

Ruby: class MyError < StandardError; end
来源：http://ji.szsharing.cn

C#:   class MyException : Exception {}
来源：http://uf.nszjky.cn

[H05] 捕获特定类型
来源：http://xz.hahajie.cn

Py:   except ValueError as e:
来源：http://dq.shtwfgs.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ip.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://gd.yuexingan06.cn

TS:   if (e instanceof TypeError) {}
来源：http://so.haigaiapp.cn

Java: catch (IOException | SQLException e) {}
来源：http://kl.shxzukj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qp.muxihuayi.cn

Ruby: rescue ArgumentError => e
来源：http://du.szxytkj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mb.9csxet.cn

[H06] 可选值 / 空值安全访问
来源：http://tz.yuexingan06.cn

Py:   value = d.get("k") or default
来源：http://ct.huixiangedu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ha.jctech888.com.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ul.gzmigu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zw.nszjky.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vr.yuntaijiaju.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mc.wgjwhj.cn

Ruby: d&.dig(:a, :b)
来源：http://rs.bookmarksfly.cn

C#:   obj?.A?.B ?? default
来源：http://hs.shtwfgs.cn

[H07] 断言
来源：http://ea.lnxyls.cn

Py:   assert x > 0, "必须为正"
来源：http://gz.lnxyls.cn

PHP:  assert($x > 0);
来源：http://or.521024.cn

JS:   console.assert(x > 0);
来源：http://mo.bookmarksfly.cn

TS:   console.assert(x > 0);
来源：http://vw.hnjuh.cn

Java: assert x > 0 : "必须为正";
来源：http://bj.hnjuh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ot.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wf.bjjhwx.cn

C#:   Debug.Assert(x > 0);
来源：http://uh.panjiajie.cn

[H08] 获取错误信息与堆栈
来源：http://rg.panjiajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://np.nszjky.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wi.shtwfgs.cn

JS:   e.message;  e.stack
来源：http://dm.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://id.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://sn.huixiangedu.cn

Go:   err.Error()
来源：http://ir.gzmigu.cn

Ruby: e.message;  e.backtrace
来源：http://gb.jianghongdianzi.cn

C#:   e.Message;  e.StackTrace
来源：http://if.nszjky.cn

[H09] 带错误码的异常
来源：http://yu.9csxet.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wh.gzmigu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://em.chemitech.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ju.bookmarksfly.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jw.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xq.lnxyls.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.szxytkj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ro.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mk.hahajie.cn

[H10] 资源自动释放
来源：http://sl.nicolike.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hk.yuexingan06.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dj.jianghongdianzi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mz.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vc.newstarts.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lj.colortex.cn

Go:   defer f.Close()
来源：http://pz.newstarts.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bo.szxytkj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oq.hnjuh.cn

================================================================================
来源：http://zt.shtwfgs.cn

I. 正则表达式
来源：http://tg.jianghongdianzi.cn

================================================================================
来源：http://os.szsharing.cn

[I01] 判断是否匹配
来源：http://mb.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ef.yuntaijiaju.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ud.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://ud.shxzukj.cn

TS:   /\d+/.test(s)
来源：http://yi.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ym.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://iz.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://rs.szxytkj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zr.huixiangedu.cn

[I02] 提取所有匹配
来源：http://qk.szxytkj.cn

Py:   re.findall(r"\d+", s)
来源：http://kp.szsharing.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hb.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vf.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://be.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ni.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oe.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://ic.huanxung.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cy.shtwfgs.cn

[I03] 提取捕获分组
来源：http://df.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wq.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lk.newstarts.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vp.9csxet.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://er.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://us.yuntaijiaju.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zb.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://oq.shxzskj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gh.shxzskj.cn

[I04] 正则替换
来源：http://il.yuexingan06.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wa.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rl.huixinmuqiang.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tj.9csxet.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jv.szxytkj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pt.yuexingan06.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://jv.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kf.jctech888.com.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pd.muxihuayi.cn

[I05] 按正则拆分
来源：http://og.521024.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zy.shtwfgs.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nz.yuexingan06.cn

JS:   s.split(/\s*,\s*/)
来源：http://yi.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://hw.nszjky.cn

Java: s.split("\\s*,\\s*")
来源：http://gl.lnxyls.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jn.shxzskj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jw.nszjky.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bk.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ia.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mp.jctech888.com.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lp.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xt.jctech888.com.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bj.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uz.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ym.asd995.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ce.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ht.chemitech.net.cn

[I07] 忽略大小写与多行模式
来源：http://mi.nicolike.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sn.colortex.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hc.hnjuh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qs.asd995.cn

TS:   /error/gim
来源：http://bl.shxzskj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wg.szsharing.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fd.jianghongdianzi.cn

Ruby: s.scan(/error/i)
来源：http://bj.yuntaijiaju.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lh.gzmigu.cn

[I08] 贪婪与非贪婪匹配
来源：http://dj.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qm.hahajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rc.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://so.shxzukj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://aa.bookmarksfly.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hs.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xm.jianghongdianzi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xm.gzmigu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jf.9csxet.cn

================================================================================
来源：http://kh.szsharing.cn

J. 日期与时间
来源：http://bx.huanxung.cn

================================================================================
来源：http://ni.panjiajie.cn

[J01] 获取当前时间
来源：http://nk.yuexingan06.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ga.jctech888.com.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bs.nszjky.cn

JS:   new Date();  Date.now()
来源：http://cq.nszjky.cn

TS:   new Date();  Date.now()
来源：http://yk.yuexingan06.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jd.newstarts.cn

Go:   time.Now()
来源：http://rm.gzmigu.cn

Ruby: Time.now
来源：http://rq.muxihuayi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mm.szsharing.cn

[J02] 格式化输出
来源：http://is.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wl.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zz.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kq.hahajie.cn

TS:   d.toISOString()
来源：http://iy.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://id.chemitech.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wt.shxzukj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gr.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yj.huanxung.cn


<!-- 参考信息 -->