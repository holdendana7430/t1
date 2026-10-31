代发 wailian999

JS:   super.greet();
来源：http://sh.newstarts.cn

TS:   super.greet();
来源：http://cq.shxzukj.cn

Java: super.greet();
来源：http://iq.wgjwhj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hq.wgjwhj.cn

Ruby: super
来源：http://ex.shtwfgs.cn

C#:   base.Greet();
来源：http://ns.gzmigu.cn

[G08] 静态方法与属性
来源：http://ft.gzmigu.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ch.yuntaijiaju.cn

PHP:  public static function f() {}
来源：http://wq.haigaiapp.cn

JS:   static f() {}
来源：http://vy.gzmigu.cn

TS:   static f(): void {}
来源：http://kc.jianghongdianzi.cn

Java: static void f() {}
来源：http://pu.gzmigu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sr.gzmigu.cn

Ruby: def self.f; end
来源：http://ja.panjiajie.cn

C#:   public static void F() {}
来源：http://sg.chemitech.net.cn

[G09] 接口 / 抽象类
来源：http://tz.yuexingan06.cn

Py:   from abc import ABC, abstractmethod
来源：http://jc.yuexingan06.cn

PHP:  interface Shape { public function area(): float; }
来源：http://rv.wgjwhj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sf.gzmigu.cn

TS:   interface Shape { area(): number; }
来源：http://if.szsharing.cn

Java: interface Shape { double area(); }
来源：http://ch.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://ub.yuntaijiaju.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wn.lnxyls.cn

C#:   interface IShape { double Area(); }
来源：http://ax.haigaiapp.cn

[G10] 访问控制
来源：http://hq.panjiajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://de.bjjhwx.cn

PHP:  public / protected / private
来源：http://id.shxzukj.cn

JS:   #private 字段；其余公开
来源：http://kt.muxihuayi.cn

TS:   public / protected / private
来源：http://uk.asd995.cn

Java: public / protected / private / 默认包级
来源：http://px.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jh.chemitech.net.cn

Ruby: public / protected / private
来源：http://wa.hnjuh.cn

C#:   public / protected / private / internal
来源：http://pm.521024.cn

[G11] getter / setter
来源：http://hu.asd995.cn

Py:   @property 与 @x.setter
来源：http://vd.asd995.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fn.hahajie.cn

JS:   get name() { return this._name; }
来源：http://je.shxzukj.cn

TS:   get name(): string { return this._name; }
来源：http://qq.yuntaijiaju.cn

Java: public String getName() { return name; }
来源：http://fl.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://kq.bookmarksfly.cn

Ruby: attr_accessor :name
来源：http://pu.shxzskj.cn

C#:   public string Name { get; set; }
来源：http://mc.szsharing.cn

[G12] 对象转字符串
来源：http://kl.jianghongdianzi.cn

Py:   def __str__(self): return self.name
来源：http://cj.shtwfgs.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ps.huixinmuqiang.cn

JS:   toString() { return this.name; }
来源：http://rb.jianghongdianzi.cn

TS:   toString(): string { return this.name; }
来源：http://id.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://cb.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pi.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://uh.shxzukj.cn

C#:   public override string ToString() => Name;
来源：http://tn.shtwfgs.cn

[G13] 判断对象类型
来源：http://vk.9csxet.cn

Py:   isinstance(u, User)
来源：http://ft.huixinmuqiang.cn

PHP:  $u instanceof User
来源：http://cd.jctech888.com.cn

JS:   u instanceof User
来源：http://td.nicolike.cn

TS:   u instanceof User
来源：http://oh.yuntaijiaju.cn

Java: u instanceof User
来源：http://uj.haigaiapp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ki.colortex.cn

Ruby: u.is_a?(User)
来源：http://au.szxytkj.cn

C#:   u is User
来源：http://zl.panjiajie.cn

[G14] 数据类 / record
来源：http://kp.wgjwhj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bv.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://jw.hahajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kx.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://go.chemitech.net.cn

Java: record User(String name, int age) {}
来源：http://lr.lnxyls.cn

Go:   type User struct { Name string; Age int }
来源：http://tb.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jm.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://ft.huixinmuqiang.cn

[G15] 枚举
来源：http://fu.bjjhwx.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dr.521024.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yw.szxytkj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xh.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://je.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://br.colortex.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ug.521024.cn

Ruby: Color = %i[red green].freeze
来源：http://qh.shtwfgs.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vv.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://iw.asd995.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://re.szxytkj.cn

PHP:  get_object_vars($obj);
来源：http://ih.szxytkj.cn

JS:   Object.entries(obj)
来源：http://kb.huixiangedu.cn

TS:   Object.entries(obj)
来源：http://pn.bjjhwx.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mq.bookmarksfly.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ae.huixinmuqiang.cn

Ruby: obj.instance_variables
来源：http://uj.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://yo.hahajie.cn

================================================================================
来源：http://aw.nicolike.cn

H. 异常与错误处理
来源：http://re.huixinmuqiang.cn

================================================================================
来源：http://th.gzmigu.cn

[H01] try / catch 基础
来源：http://jf.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ob.yuexingan06.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ju.nszjky.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yr.szxytkj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ap.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hu.yuntaijiaju.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sv.shxzukj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gl.asd995.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gv.521024.cn

[H02] finally / ensure 收尾
来源：http://dp.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ox.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zx.muxihuayi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://aa.gzmigu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jb.huixinmuqiang.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gs.hnjuh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://po.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bi.shxzukj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sx.chemitech.net.cn

[H03] 主动抛出异常
来源：http://rz.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://nn.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pn.asd995.cn

JS:   throw new Error("错误信息");
来源：http://mw.yuexingan06.cn

TS:   throw new Error("错误信息");
来源：http://sj.haigaiapp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ku.nszjky.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yp.szxytkj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ke.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://er.newstarts.cn

[H04] 自定义异常类型
来源：http://gx.jctech888.com.cn

Py:   class MyError(Exception): pass
来源：http://sc.jianghongdianzi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gs.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://ki.muxihuayi.cn

TS:   class MyError extends Error {}
来源：http://vi.huanxung.cn

Java: class MyException extends RuntimeException {}
来源：http://dh.nicolike.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lb.jianghongdianzi.cn

Ruby: class MyError < StandardError; end
来源：http://zb.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://vt.yuntaijiaju.cn

[H05] 捕获特定类型
来源：http://tm.hahajie.cn

Py:   except ValueError as e:
来源：http://lg.bjjhwx.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://nq.jianghongdianzi.cn

JS:   if (e instanceof TypeError) {}
来源：http://wj.haigaiapp.cn

TS:   if (e instanceof TypeError) {}
来源：http://ck.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://vu.huixinmuqiang.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rk.szsharing.cn

Ruby: rescue ArgumentError => e
来源：http://cg.huixiangedu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kv.szsharing.cn

[H06] 可选值 / 空值安全访问
来源：http://hb.gzmigu.cn

Py:   value = d.get("k") or default
来源：http://ex.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kc.shtwfgs.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sh.shtwfgs.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ci.9csxet.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ra.nicolike.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://sb.jianghongdianzi.cn

Ruby: d&.dig(:a, :b)
来源：http://sy.521024.cn

C#:   obj?.A?.B ?? default
来源：http://gl.szsharing.cn

[H07] 断言
来源：http://kx.huixinmuqiang.cn

Py:   assert x > 0, "必须为正"
来源：http://mf.bookmarksfly.cn

PHP:  assert($x > 0);
来源：http://xg.huixinmuqiang.cn

JS:   console.assert(x > 0);
来源：http://gr.gzmigu.cn

TS:   console.assert(x > 0);
来源：http://yi.haigaiapp.cn

Java: assert x > 0 : "必须为正";
来源：http://bi.bookmarksfly.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tr.nszjky.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bv.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://mx.nszjky.cn

[H08] 获取错误信息与堆栈
来源：http://as.haigaiapp.cn

Py:   str(e);  traceback.format_exc()
来源：http://zn.yuntaijiaju.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hp.shxzukj.cn

JS:   e.message;  e.stack
来源：http://lb.huixiangedu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://um.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wp.huixinmuqiang.cn

Go:   err.Error()
来源：http://pg.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://ou.jctech888.com.cn

C#:   e.Message;  e.StackTrace
来源：http://cj.lnxyls.cn

[H09] 带错误码的异常
来源：http://zq.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xs.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vl.jctech888.com.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://dz.chemitech.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qv.9csxet.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fl.huixinmuqiang.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://at.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cl.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bs.muxihuayi.cn

[H10] 资源自动释放
来源：http://vx.shxzskj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://re.yuexingan06.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gd.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ex.shtwfgs.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pk.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vr.shxzukj.cn

Go:   defer f.Close()
来源：http://bk.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ya.newstarts.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yl.wgjwhj.cn

================================================================================
来源：http://cg.shtwfgs.cn

I. 正则表达式
来源：http://tk.huixinmuqiang.cn

================================================================================
来源：http://ql.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://xt.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ic.yuntaijiaju.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vs.hnjuh.cn

JS:   /\d+/.test(s)
来源：http://ty.hnjuh.cn

TS:   /\d+/.test(s)
来源：http://hi.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ve.nszjky.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ch.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://ei.chemitech.net.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zj.haigaiapp.cn

[I02] 提取所有匹配
来源：http://ql.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://ey.huanxung.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ru.szsharing.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rc.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://lp.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ci.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dm.bjjhwx.cn

Ruby: s.scan(/\d+/)
来源：http://wa.newstarts.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://io.asd995.cn

[I03] 提取捕获分组
来源：http://ut.nszjky.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nz.521024.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ly.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ch.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kt.colortex.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://da.nszjky.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ct.huanxung.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tk.huixiangedu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mf.9csxet.cn

[I04] 正则替换
来源：http://kz.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://oq.nicolike.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qg.9csxet.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dq.szxytkj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vj.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bh.jianghongdianzi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pb.9csxet.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ng.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xs.nicolike.cn

[I05] 按正则拆分
来源：http://sw.szxytkj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mn.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bx.asd995.cn

JS:   s.split(/\s*,\s*/)
来源：http://rz.hnjuh.cn

TS:   s.split(/\s*,\s*/)
来源：http://cv.huixiangedu.cn

Java: s.split("\\s*,\\s*")
来源：http://pm.shtwfgs.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yb.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ez.shxzukj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ln.hahajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ot.bjjhwx.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zc.szxytkj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fr.huanxung.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uj.asd995.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bp.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://jz.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nd.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jj.521024.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wj.shxzukj.cn

[I07] 忽略大小写与多行模式
来源：http://eb.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hi.shxzskj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vm.bookmarksfly.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://li.panjiajie.cn

TS:   /error/gim
来源：http://dt.yuntaijiaju.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ib.shxzukj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ke.szxytkj.cn

Ruby: s.scan(/error/i)
来源：http://xw.newstarts.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mg.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://di.shxzukj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yl.haigaiapp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qu.bookmarksfly.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dz.nicolike.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cm.asd995.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qx.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gd.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nn.hahajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dh.huixiangedu.cn

================================================================================
来源：http://jg.shtwfgs.cn

J. 日期与时间
来源：http://gq.gzmigu.cn

================================================================================
来源：http://kq.chemitech.net.cn

[J01] 获取当前时间
来源：http://fh.huixinmuqiang.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ci.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ji.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://ac.huanxung.cn

TS:   new Date();  Date.now()
来源：http://ui.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pn.shtwfgs.cn

Go:   time.Now()
来源：http://nc.colortex.cn

Ruby: Time.now
来源：http://rc.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mk.hahajie.cn

[J02] 格式化输出
来源：http://rl.bookmarksfly.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cp.bookmarksfly.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tr.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vm.jctech888.com.cn

TS:   d.toISOString()
来源：http://qi.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xx.yuexingan06.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wa.nszjky.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ei.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lz.bookmarksfly.cn

[J03] 字符串解析为日期
来源：http://re.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tf.jianghongdianzi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nh.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://ml.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://xh.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ci.nszjky.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jd.colortex.cn

Ruby: Date.parse("2024-01-02")
来源：http://kn.huixiangedu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jc.shxzskj.cn

[J04] 时间戳与日期互转
来源：http://hk.huanxung.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zj.lnxyls.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jw.huanxung.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wo.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bs.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oa.nszjky.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jk.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wo.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sp.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://mx.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://aw.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://th.bjjhwx.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lx.chemitech.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://xi.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://iw.panjiajie.cn


<!-- 参考信息 -->