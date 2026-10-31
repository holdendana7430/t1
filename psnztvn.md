代发 wailian999

[G06] 重写方法
来源：http://gr.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://xo.521024.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://iz.yuexingan06.cn

JS:   greet() { return "admin"; }
来源：http://mb.nszjky.cn

TS:   greet(): string { return "admin"; }
来源：http://nb.huixinmuqiang.cn

Java: @Override String greet() { return "admin"; }
来源：http://ei.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://up.szxytkj.cn

Ruby: def greet; "admin"; end
来源：http://aw.asd995.cn

C#:   public override string Greet() => "admin";
来源：http://tr.shtwfgs.cn

[G07] 调用父类方法
来源：http://be.yuexingan06.cn

Py:   super().greet()
来源：http://bk.nicolike.cn

PHP:  parent::greet();
来源：http://zg.szsharing.cn

JS:   super.greet();
来源：http://um.haigaiapp.cn

TS:   super.greet();
来源：http://qx.521024.cn

Java: super.greet();
来源：http://jg.gzmigu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ig.huixinmuqiang.cn

Ruby: super
来源：http://xd.newstarts.cn

C#:   base.Greet();
来源：http://js.szxytkj.cn

[G08] 静态方法与属性
来源：http://qa.jctech888.com.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hc.nicolike.cn

PHP:  public static function f() {}
来源：http://ep.panjiajie.cn

JS:   static f() {}
来源：http://zq.521024.cn

TS:   static f(): void {}
来源：http://te.yuexingan06.cn

Java: static void f() {}
来源：http://xn.asd995.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ic.9csxet.cn

Ruby: def self.f; end
来源：http://yr.huanxung.cn

C#:   public static void F() {}
来源：http://ch.wgjwhj.cn

[G09] 接口 / 抽象类
来源：http://jx.jctech888.com.cn

Py:   from abc import ABC, abstractmethod
来源：http://du.huixinmuqiang.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ed.muxihuayi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pw.szxytkj.cn

TS:   interface Shape { area(): number; }
来源：http://oq.9csxet.cn

Java: interface Shape { double area(); }
来源：http://qo.shxzskj.cn

Go:   type Shape interface { Area() float64 }
来源：http://dd.muxihuayi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wc.shtwfgs.cn

C#:   interface IShape { double Area(); }
来源：http://zk.521024.cn

[G10] 访问控制
来源：http://vz.szsharing.cn

Py:   约定 _protected / __private（不强制）
来源：http://tc.nicolike.cn

PHP:  public / protected / private
来源：http://jt.lnxyls.cn

JS:   #private 字段；其余公开
来源：http://in.huixiangedu.cn

TS:   public / protected / private
来源：http://uz.haigaiapp.cn

Java: public / protected / private / 默认包级
来源：http://eh.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xf.colortex.cn

Ruby: public / protected / private
来源：http://mq.yuexingan06.cn

C#:   public / protected / private / internal
来源：http://iq.hahajie.cn

[G11] getter / setter
来源：http://wp.newstarts.cn

Py:   @property 与 @x.setter
来源：http://ew.hahajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gw.hahajie.cn

JS:   get name() { return this._name; }
来源：http://kt.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://dk.colortex.cn

Java: public String getName() { return name; }
来源：http://pz.wgjwhj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://sc.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://zv.szxytkj.cn

C#:   public string Name { get; set; }
来源：http://pa.shtwfgs.cn

[G12] 对象转字符串
来源：http://ui.hnjuh.cn

Py:   def __str__(self): return self.name
来源：http://tn.asd995.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ae.bjjhwx.cn

JS:   toString() { return this.name; }
来源：http://gi.newstarts.cn

TS:   toString(): string { return this.name; }
来源：http://gu.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://zu.szxytkj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://oq.haigaiapp.cn

Ruby: def to_s; @name; end
来源：http://db.jctech888.com.cn

C#:   public override string ToString() => Name;
来源：http://nb.nicolike.cn

[G13] 判断对象类型
来源：http://dk.shxzukj.cn

Py:   isinstance(u, User)
来源：http://ro.muxihuayi.cn

PHP:  $u instanceof User
来源：http://ad.hahajie.cn

JS:   u instanceof User
来源：http://nc.hahajie.cn

TS:   u instanceof User
来源：http://cr.521024.cn

Java: u instanceof User
来源：http://ml.haigaiapp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vm.colortex.cn

Ruby: u.is_a?(User)
来源：http://ej.szsharing.cn

C#:   u is User
来源：http://us.colortex.cn

[G14] 数据类 / record
来源：http://xi.huixiangedu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jn.nicolike.cn

PHP:  // 用 readonly 属性模拟
来源：http://sa.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://th.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://ha.shtwfgs.cn

Java: record User(String name, int age) {}
来源：http://qd.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://pf.521024.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nd.bjjhwx.cn

C#:   record User(string Name, int Age);
来源：http://yc.shtwfgs.cn

[G15] 枚举
来源：http://lt.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kk.bookmarksfly.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dv.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ud.gzmigu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qc.9csxet.cn

Java: enum Color { RED, GREEN }
来源：http://gy.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oo.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://xl.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uo.huanxung.cn

[G16] 对象转数组 / 字典
来源：http://eq.nszjky.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://js.hnjuh.cn

PHP:  get_object_vars($obj);
来源：http://vt.huixiangedu.cn

JS:   Object.entries(obj)
来源：http://te.szsharing.cn

TS:   Object.entries(obj)
来源：http://hs.lnxyls.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ne.colortex.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ga.colortex.cn

Ruby: obj.instance_variables
来源：http://fv.shxzskj.cn

C#:   // 用反射或 System.Text.Json
来源：http://xb.panjiajie.cn

================================================================================
来源：http://wa.chemitech.net.cn

H. 异常与错误处理
来源：http://mw.colortex.cn

================================================================================
来源：http://ad.hnjuh.cn

[H01] try / catch 基础
来源：http://zj.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pw.gzmigu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zp.shxzukj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jv.jianghongdianzi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mx.wgjwhj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ab.huanxung.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ar.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bc.colortex.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fq.lnxyls.cn

[H02] finally / ensure 收尾
来源：http://yo.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fw.bjjhwx.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yk.shxzskj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wz.chemitech.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yb.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fy.huixinmuqiang.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nf.huixiangedu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tk.gzmigu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wn.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://hc.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://zp.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://is.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://dy.shxzskj.cn

TS:   throw new Error("错误信息");
来源：http://kq.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://eq.gzmigu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ap.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rv.muxihuayi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wh.panjiajie.cn

[H04] 自定义异常类型
来源：http://ki.yuexingan06.cn

Py:   class MyError(Exception): pass
来源：http://rx.wgjwhj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://oo.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://no.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://cj.shxzukj.cn

Java: class MyException extends RuntimeException {}
来源：http://ha.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wp.9csxet.cn

Ruby: class MyError < StandardError; end
来源：http://ap.asd995.cn

C#:   class MyException : Exception {}
来源：http://fb.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://ex.yuntaijiaju.cn

Py:   except ValueError as e:
来源：http://ec.shxzukj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zg.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://yp.yuexingan06.cn

TS:   if (e instanceof TypeError) {}
来源：http://oa.lnxyls.cn

Java: catch (IOException | SQLException e) {}
来源：http://vx.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://po.hnjuh.cn

Ruby: rescue ArgumentError => e
来源：http://ej.bookmarksfly.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://if.shtwfgs.cn

[H06] 可选值 / 空值安全访问
来源：http://rj.panjiajie.cn

Py:   value = d.get("k") or default
来源：http://bw.521024.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ue.colortex.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qk.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mm.newstarts.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://it.bjjhwx.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sa.haigaiapp.cn

Ruby: d&.dig(:a, :b)
来源：http://jq.9csxet.cn

C#:   obj?.A?.B ?? default
来源：http://sc.gzmigu.cn

[H07] 断言
来源：http://qz.huixinmuqiang.cn

Py:   assert x > 0, "必须为正"
来源：http://om.nicolike.cn

PHP:  assert($x > 0);
来源：http://mg.yuntaijiaju.cn

JS:   console.assert(x > 0);
来源：http://cw.colortex.cn

TS:   console.assert(x > 0);
来源：http://xf.bookmarksfly.cn

Java: assert x > 0 : "必须为正";
来源：http://hb.newstarts.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vg.haigaiapp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tb.shxzukj.cn

C#:   Debug.Assert(x > 0);
来源：http://hk.521024.cn

[H08] 获取错误信息与堆栈
来源：http://xt.lnxyls.cn

Py:   str(e);  traceback.format_exc()
来源：http://tl.lnxyls.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mg.nicolike.cn

JS:   e.message;  e.stack
来源：http://ly.nicolike.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fa.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ri.haigaiapp.cn

Go:   err.Error()
来源：http://jr.shtwfgs.cn

Ruby: e.message;  e.backtrace
来源：http://xc.haigaiapp.cn

C#:   e.Message;  e.StackTrace
来源：http://cg.shtwfgs.cn

[H09] 带错误码的异常
来源：http://kz.521024.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vw.nicolike.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://eg.muxihuayi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ld.colortex.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bc.huixiangedu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sx.szsharing.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ka.huanxung.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jo.huanxung.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ld.haigaiapp.cn

[H10] 资源自动释放
来源：http://hy.nicolike.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mb.nszjky.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sk.shtwfgs.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hj.szsharing.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tx.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dd.jianghongdianzi.cn

Go:   defer f.Close()
来源：http://yc.bjjhwx.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lb.huixiangedu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://th.gzmigu.cn

================================================================================
来源：http://kh.shxzskj.cn

I. 正则表达式
来源：http://ht.panjiajie.cn

================================================================================
来源：http://pb.shxzukj.cn

[I01] 判断是否匹配
来源：http://jm.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ee.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://im.bookmarksfly.cn

JS:   /\d+/.test(s)
来源：http://bf.shtwfgs.cn

TS:   /\d+/.test(s)
来源：http://us.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ut.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://td.asd995.cn

Ruby: s.match?(/\d+/)
来源：http://jt.lnxyls.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://js.shxzukj.cn

[I02] 提取所有匹配
来源：http://wz.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://rj.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bg.hnjuh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ct.bjjhwx.cn

TS:   s.match(/\d+/g)
来源：http://ip.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ct.huanxung.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ob.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://pn.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vy.nicolike.cn

[I03] 提取捕获分组
来源：http://gk.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://as.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://we.szxytkj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ho.shxzskj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yl.nszjky.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ja.bjjhwx.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yp.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cb.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bp.huanxung.cn

[I04] 正则替换
来源：http://ah.asd995.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ld.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hd.shxzskj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://af.jianghongdianzi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vt.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cz.shxzukj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rc.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kc.asd995.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bn.hahajie.cn

[I05] 按正则拆分
来源：http://zj.szsharing.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pv.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ef.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://nb.bookmarksfly.cn

TS:   s.split(/\s*,\s*/)
来源：http://mn.yuexingan06.cn

Java: s.split("\\s*,\\s*")
来源：http://pq.jctech888.com.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ds.wgjwhj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tf.hahajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xk.huixinmuqiang.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rv.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://if.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://no.nszjky.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zm.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wl.hnjuh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tm.nszjky.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://es.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bu.lnxyls.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lk.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://pn.yuexingan06.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kt.huanxung.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ez.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://an.huanxung.cn

TS:   /error/gim
来源：http://km.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://we.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tq.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://tp.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dh.szsharing.cn

[I08] 贪婪与非贪婪匹配
来源：http://zm.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hn.huixinmuqiang.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uc.hnjuh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wk.panjiajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://rd.muxihuayi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jk.muxihuayi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://uh.haigaiapp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ig.hnjuh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nx.9csxet.cn

================================================================================
来源：http://xw.chemitech.net.cn

J. 日期与时间
来源：http://zm.bookmarksfly.cn

================================================================================
来源：http://hx.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://uo.jctech888.com.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xn.huanxung.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qg.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://xb.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://jb.nszjky.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pd.hahajie.cn

Go:   time.Now()
来源：http://iz.yuexingan06.cn

Ruby: Time.now
来源：http://qx.colortex.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vi.bookmarksfly.cn

[J02] 格式化输出
来源：http://pp.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jc.huanxung.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kz.colortex.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zc.haigaiapp.cn

TS:   d.toISOString()
来源：http://nn.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yy.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vf.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yv.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zc.shxzukj.cn

[J03] 字符串解析为日期
来源：http://nt.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pq.shtwfgs.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://eg.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://sf.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://na.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://po.newstarts.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cs.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://jq.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kv.newstarts.cn

[J04] 时间戳与日期互转
来源：http://bv.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cm.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sl.nszjky.cn


<!-- 参考信息 -->