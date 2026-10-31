代发 wailian999

[G06] 重写方法
来源：http://ta.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://gz.huixinmuqiang.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ju.shtwfgs.cn

JS:   greet() { return "admin"; }
来源：http://vx.bjjhwx.cn

TS:   greet(): string { return "admin"; }
来源：http://jt.shxzskj.cn

Java: @Override String greet() { return "admin"; }
来源：http://zw.jctech888.com.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hi.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://da.hnjuh.cn

C#:   public override string Greet() => "admin";
来源：http://io.szxytkj.cn

[G07] 调用父类方法
来源：http://tn.gzmigu.cn

Py:   super().greet()
来源：http://aj.panjiajie.cn

PHP:  parent::greet();
来源：http://pi.haigaiapp.cn

JS:   super.greet();
来源：http://yf.szxytkj.cn

TS:   super.greet();
来源：http://pw.hahajie.cn

Java: super.greet();
来源：http://do.hnjuh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dm.panjiajie.cn

Ruby: super
来源：http://wz.521024.cn

C#:   base.Greet();
来源：http://bq.nicolike.cn

[G08] 静态方法与属性
来源：http://uy.asd995.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cx.asd995.cn

PHP:  public static function f() {}
来源：http://nu.haigaiapp.cn

JS:   static f() {}
来源：http://ky.huixiangedu.cn

TS:   static f(): void {}
来源：http://fa.shxzskj.cn

Java: static void f() {}
来源：http://uq.9csxet.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ze.panjiajie.cn

Ruby: def self.f; end
来源：http://dt.panjiajie.cn

C#:   public static void F() {}
来源：http://az.huixiangedu.cn

[G09] 接口 / 抽象类
来源：http://je.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://hi.yuntaijiaju.cn

PHP:  interface Shape { public function area(): float; }
来源：http://bz.muxihuayi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wq.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://op.yuexingan06.cn

Java: interface Shape { double area(); }
来源：http://ol.9csxet.cn

Go:   type Shape interface { Area() float64 }
来源：http://vm.nszjky.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cm.jctech888.com.cn

C#:   interface IShape { double Area(); }
来源：http://xq.chemitech.net.cn

[G10] 访问控制
来源：http://lp.bjjhwx.cn

Py:   约定 _protected / __private（不强制）
来源：http://jt.shxzskj.cn

PHP:  public / protected / private
来源：http://mz.9csxet.cn

JS:   #private 字段；其余公开
来源：http://fq.haigaiapp.cn

TS:   public / protected / private
来源：http://qo.521024.cn

Java: public / protected / private / 默认包级
来源：http://pf.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://px.521024.cn

Ruby: public / protected / private
来源：http://pl.asd995.cn

C#:   public / protected / private / internal
来源：http://sc.lnxyls.cn

[G11] getter / setter
来源：http://nd.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://rs.huixinmuqiang.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cw.jianghongdianzi.cn

JS:   get name() { return this._name; }
来源：http://cg.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://te.panjiajie.cn

Java: public String getName() { return name; }
来源：http://cw.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hj.nszjky.cn

Ruby: attr_accessor :name
来源：http://za.nszjky.cn

C#:   public string Name { get; set; }
来源：http://wb.chemitech.net.cn

[G12] 对象转字符串
来源：http://dj.nszjky.cn

Py:   def __str__(self): return self.name
来源：http://qu.521024.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mh.hnjuh.cn

JS:   toString() { return this.name; }
来源：http://lt.bookmarksfly.cn

TS:   toString(): string { return this.name; }
来源：http://jv.newstarts.cn

Java: @Override public String toString() { return name; }
来源：http://cu.bookmarksfly.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ie.newstarts.cn

Ruby: def to_s; @name; end
来源：http://ml.jctech888.com.cn

C#:   public override string ToString() => Name;
来源：http://ch.colortex.cn

[G13] 判断对象类型
来源：http://qr.nicolike.cn

Py:   isinstance(u, User)
来源：http://ks.gzmigu.cn

PHP:  $u instanceof User
来源：http://tp.lnxyls.cn

JS:   u instanceof User
来源：http://lx.huixiangedu.cn

TS:   u instanceof User
来源：http://hp.bjjhwx.cn

Java: u instanceof User
来源：http://mn.nszjky.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ox.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://mq.huanxung.cn

C#:   u is User
来源：http://qb.huixiangedu.cn

[G14] 数据类 / record
来源：http://sb.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vk.panjiajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://qf.bjjhwx.cn

JS:   // 无内置：普通类或对象字面量
来源：http://oz.wgjwhj.cn

TS:   type User = { name: string; age: number };
来源：http://kz.bjjhwx.cn

Java: record User(String name, int age) {}
来源：http://zk.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://ea.szsharing.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tm.nicolike.cn

C#:   record User(string Name, int Age);
来源：http://ao.521024.cn

[G15] 枚举
来源：http://qr.wgjwhj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bi.hahajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ez.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hx.huanxung.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ux.bjjhwx.cn

Java: enum Color { RED, GREEN }
来源：http://pz.huixinmuqiang.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vy.colortex.cn

Ruby: Color = %i[red green].freeze
来源：http://zq.szxytkj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sy.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://kp.asd995.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hq.nicolike.cn

PHP:  get_object_vars($obj);
来源：http://rl.hnjuh.cn

JS:   Object.entries(obj)
来源：http://vu.shxzskj.cn

TS:   Object.entries(obj)
来源：http://pi.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://no.bookmarksfly.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nr.lnxyls.cn

Ruby: obj.instance_variables
来源：http://ra.shtwfgs.cn

C#:   // 用反射或 System.Text.Json
来源：http://vh.9csxet.cn

================================================================================
来源：http://vh.hnjuh.cn

H. 异常与错误处理
来源：http://se.9csxet.cn

================================================================================
来源：http://bh.asd995.cn

[H01] try / catch 基础
来源：http://gi.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sy.hnjuh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://av.lnxyls.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uu.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tw.jctech888.com.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jz.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hx.huixiangedu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jn.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tk.9csxet.cn

[H02] finally / ensure 收尾
来源：http://iv.colortex.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ll.bjjhwx.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tw.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ye.szsharing.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nj.asd995.cn

Java: try { f(); } finally { cleanup(); }
来源：http://oa.yuntaijiaju.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pn.gzmigu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bu.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yd.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://xg.wgjwhj.cn

Py:   raise ValueError("错误信息")
来源：http://sl.haigaiapp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kh.nicolike.cn

JS:   throw new Error("错误信息");
来源：http://cl.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://ag.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wk.shxzskj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ac.jctech888.com.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mw.huanxung.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gf.shxzskj.cn

[H04] 自定义异常类型
来源：http://mf.9csxet.cn

Py:   class MyError(Exception): pass
来源：http://yl.9csxet.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yg.huixiangedu.cn

JS:   class MyError extends Error {}
来源：http://ca.yuntaijiaju.cn

TS:   class MyError extends Error {}
来源：http://fj.yuntaijiaju.cn

Java: class MyException extends RuntimeException {}
来源：http://oa.hnjuh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jh.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://kr.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://km.bjjhwx.cn

[H05] 捕获特定类型
来源：http://hc.szsharing.cn

Py:   except ValueError as e:
来源：http://ti.gzmigu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qb.nicolike.cn

JS:   if (e instanceof TypeError) {}
来源：http://cr.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://nv.shtwfgs.cn

Java: catch (IOException | SQLException e) {}
来源：http://wz.shtwfgs.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wo.huixinmuqiang.cn

Ruby: rescue ArgumentError => e
来源：http://jg.hahajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qa.yuntaijiaju.cn

[H06] 可选值 / 空值安全访问
来源：http://rs.hahajie.cn

Py:   value = d.get("k") or default
来源：http://mw.haigaiapp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yy.lnxyls.cn

JS:   obj?.a?.b;  d ?? default
来源：http://um.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yf.bjjhwx.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ww.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://js.haigaiapp.cn

Ruby: d&.dig(:a, :b)
来源：http://wl.nicolike.cn

C#:   obj?.A?.B ?? default
来源：http://iq.panjiajie.cn

[H07] 断言
来源：http://gd.521024.cn

Py:   assert x > 0, "必须为正"
来源：http://by.huanxung.cn

PHP:  assert($x > 0);
来源：http://ul.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://dv.9csxet.cn

TS:   console.assert(x > 0);
来源：http://md.asd995.cn

Java: assert x > 0 : "必须为正";
来源：http://pc.jctech888.com.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ch.bookmarksfly.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kb.hnjuh.cn

C#:   Debug.Assert(x > 0);
来源：http://qu.9csxet.cn

[H08] 获取错误信息与堆栈
来源：http://qj.haigaiapp.cn

Py:   str(e);  traceback.format_exc()
来源：http://dj.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://da.shxzskj.cn

JS:   e.message;  e.stack
来源：http://qd.huixinmuqiang.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://or.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jz.chemitech.net.cn

Go:   err.Error()
来源：http://ap.jctech888.com.cn

Ruby: e.message;  e.backtrace
来源：http://wb.huanxung.cn

C#:   e.Message;  e.StackTrace
来源：http://zw.huixiangedu.cn

[H09] 带错误码的异常
来源：http://jx.9csxet.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mb.hnjuh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zm.nicolike.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://eg.lnxyls.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jc.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hj.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hu.huixiangedu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zu.jctech888.com.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rp.huixiangedu.cn

[H10] 资源自动释放
来源：http://la.lnxyls.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://je.asd995.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jc.hnjuh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kx.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://uw.huixinmuqiang.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oa.bookmarksfly.cn

Go:   defer f.Close()
来源：http://jq.9csxet.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xz.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ey.shtwfgs.cn

================================================================================
来源：http://ox.shtwfgs.cn

I. 正则表达式
来源：http://lm.huixinmuqiang.cn

================================================================================
来源：http://mb.colortex.cn

[I01] 判断是否匹配
来源：http://vw.shtwfgs.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ic.hnjuh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bo.nicolike.cn

JS:   /\d+/.test(s)
来源：http://ne.nicolike.cn

TS:   /\d+/.test(s)
来源：http://zx.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ln.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mv.gzmigu.cn

Ruby: s.match?(/\d+/)
来源：http://xv.huixiangedu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://my.huixiangedu.cn

[I02] 提取所有匹配
来源：http://ag.nicolike.cn

Py:   re.findall(r"\d+", s)
来源：http://hi.shtwfgs.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kb.szsharing.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zo.asd995.cn

TS:   s.match(/\d+/g)
来源：http://xi.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hk.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cr.asd995.cn

Ruby: s.scan(/\d+/)
来源：http://to.lnxyls.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ef.szxytkj.cn

[I03] 提取捕获分组
来源：http://bo.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sf.yuexingan06.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ml.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rf.9csxet.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ky.gzmigu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mi.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fz.panjiajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ct.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://td.lnxyls.cn

[I04] 正则替换
来源：http://dh.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kb.shxzskj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ob.newstarts.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tk.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mv.jctech888.com.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mx.hnjuh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uj.shxzskj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ac.nszjky.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xi.bookmarksfly.cn

[I05] 按正则拆分
来源：http://cj.wgjwhj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cr.yuexingan06.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wl.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://di.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://jw.huixiangedu.cn

Java: s.split("\\s*,\\s*")
来源：http://pz.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cc.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dd.521024.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yl.lnxyls.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nj.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jh.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zg.bjjhwx.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xe.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://za.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jd.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xz.hnjuh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ll.lnxyls.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ef.jctech888.com.cn

[I07] 忽略大小写与多行模式
来源：http://sq.nszjky.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qv.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dd.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bg.newstarts.cn

TS:   /error/gim
来源：http://lc.bookmarksfly.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xv.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.colortex.cn

Ruby: s.scan(/error/i)
来源：http://ul.newstarts.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://et.yuntaijiaju.cn

[I08] 贪婪与非贪婪匹配
来源：http://rs.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vy.521024.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://og.shtwfgs.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jg.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tj.yuexingan06.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gb.jianghongdianzi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xz.shxzukj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nu.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bd.nszjky.cn

================================================================================
来源：http://af.colortex.cn

J. 日期与时间
来源：http://yl.521024.cn

================================================================================
来源：http://kk.asd995.cn

[J01] 获取当前时间
来源：http://qz.shtwfgs.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://xn.jianghongdianzi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cg.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://ny.bookmarksfly.cn

TS:   new Date();  Date.now()
来源：http://qh.newstarts.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://js.9csxet.cn

Go:   time.Now()
来源：http://jj.newstarts.cn

Ruby: Time.now
来源：http://pz.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bw.szsharing.cn

[J02] 格式化输出
来源：http://pi.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tz.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bl.hnjuh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fd.wgjwhj.cn

TS:   d.toISOString()
来源：http://gg.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://oh.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fi.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ox.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://py.szxytkj.cn

[J03] 字符串解析为日期
来源：http://xu.asd995.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pr.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kb.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://nf.colortex.cn

TS:   new Date("2024-01-02")
来源：http://ak.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qg.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kf.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://qd.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://it.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://cs.asd995.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ns.521024.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://db.shtwfgs.cn


<!-- 参考信息 -->