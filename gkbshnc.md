代发 wailian999

JS:   super.greet();
来源：http://zp.jianghongdianzi.cn

TS:   super.greet();
来源：http://vi.panjiajie.cn

Java: super.greet();
来源：http://qb.huixiangedu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pr.nszjky.cn

Ruby: super
来源：http://cj.yuexingan06.cn

C#:   base.Greet();
来源：http://qu.521024.cn

[G08] 静态方法与属性
来源：http://qn.hnjuh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jy.huanxung.cn

PHP:  public static function f() {}
来源：http://xk.521024.cn

JS:   static f() {}
来源：http://hc.bookmarksfly.cn

TS:   static f(): void {}
来源：http://mg.shtwfgs.cn

Java: static void f() {}
来源：http://ug.colortex.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cn.colortex.cn

Ruby: def self.f; end
来源：http://hc.huanxung.cn

C#:   public static void F() {}
来源：http://nt.muxihuayi.cn

[G09] 接口 / 抽象类
来源：http://rf.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://tn.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qi.huixiangedu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rp.szxytkj.cn

TS:   interface Shape { area(): number; }
来源：http://cd.lnxyls.cn

Java: interface Shape { double area(); }
来源：http://rb.asd995.cn

Go:   type Shape interface { Area() float64 }
来源：http://as.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ep.bjjhwx.cn

C#:   interface IShape { double Area(); }
来源：http://yv.huixinmuqiang.cn

[G10] 访问控制
来源：http://qm.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://dk.newstarts.cn

PHP:  public / protected / private
来源：http://mh.shtwfgs.cn

JS:   #private 字段；其余公开
来源：http://kq.shtwfgs.cn

TS:   public / protected / private
来源：http://md.hnjuh.cn

Java: public / protected / private / 默认包级
来源：http://gw.panjiajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ov.nszjky.cn

Ruby: public / protected / private
来源：http://bk.huanxung.cn

C#:   public / protected / private / internal
来源：http://fn.newstarts.cn

[G11] getter / setter
来源：http://db.huanxung.cn

Py:   @property 与 @x.setter
来源：http://oc.nicolike.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ks.shxzukj.cn

JS:   get name() { return this._name; }
来源：http://gs.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://nw.colortex.cn

Java: public String getName() { return name; }
来源：http://pq.wgjwhj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lt.huanxung.cn

Ruby: attr_accessor :name
来源：http://sy.jctech888.com.cn

C#:   public string Name { get; set; }
来源：http://qf.newstarts.cn

[G12] 对象转字符串
来源：http://jy.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://ny.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://oq.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://rj.colortex.cn

TS:   toString(): string { return this.name; }
来源：http://wd.huixiangedu.cn

Java: @Override public String toString() { return name; }
来源：http://le.lnxyls.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qs.panjiajie.cn

Ruby: def to_s; @name; end
来源：http://en.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://aa.bjjhwx.cn

[G13] 判断对象类型
来源：http://pa.hahajie.cn

Py:   isinstance(u, User)
来源：http://xg.szsharing.cn

PHP:  $u instanceof User
来源：http://ks.huanxung.cn

JS:   u instanceof User
来源：http://wv.lnxyls.cn

TS:   u instanceof User
来源：http://xk.9csxet.cn

Java: u instanceof User
来源：http://gl.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rq.colortex.cn

Ruby: u.is_a?(User)
来源：http://rx.muxihuayi.cn

C#:   u is User
来源：http://qb.lnxyls.cn

[G14] 数据类 / record
来源：http://iv.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://so.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://pz.haigaiapp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mz.szxytkj.cn

TS:   type User = { name: string; age: number };
来源：http://iu.newstarts.cn

Java: record User(String name, int age) {}
来源：http://uc.521024.cn

Go:   type User struct { Name string; Age int }
来源：http://fa.hnjuh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ct.bookmarksfly.cn

C#:   record User(string Name, int Age);
来源：http://mn.hnjuh.cn

[G15] 枚举
来源：http://zr.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ew.bjjhwx.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vv.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ag.huanxung.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kk.haigaiapp.cn

Java: enum Color { RED, GREEN }
来源：http://bs.shtwfgs.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gt.hahajie.cn

Ruby: Color = %i[red green].freeze
来源：http://uk.521024.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://di.newstarts.cn

[G16] 对象转数组 / 字典
来源：http://lh.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ht.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://mi.hnjuh.cn

JS:   Object.entries(obj)
来源：http://xd.shxzskj.cn

TS:   Object.entries(obj)
来源：http://qd.asd995.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qs.panjiajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zc.jctech888.com.cn

Ruby: obj.instance_variables
来源：http://jj.gzmigu.cn

C#:   // 用反射或 System.Text.Json
来源：http://dd.newstarts.cn

================================================================================
来源：http://ku.yuexingan06.cn

H. 异常与错误处理
来源：http://aa.huanxung.cn

================================================================================
来源：http://ir.chemitech.net.cn

[H01] try / catch 基础
来源：http://zu.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://in.yuexingan06.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ml.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sd.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uf.huixiangedu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gc.9csxet.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gy.shxzskj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vg.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qf.521024.cn

[H02] finally / ensure 收尾
来源：http://cz.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ai.nszjky.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ya.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://di.huixiangedu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tj.szxytkj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://za.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xk.bookmarksfly.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rq.nszjky.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bv.hnjuh.cn

[H03] 主动抛出异常
来源：http://ng.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://pi.hahajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kl.newstarts.cn

JS:   throw new Error("错误信息");
来源：http://hm.asd995.cn

TS:   throw new Error("错误信息");
来源：http://nc.huixiangedu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://li.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mz.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://le.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kx.hnjuh.cn

[H04] 自定义异常类型
来源：http://jm.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://eh.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yv.huanxung.cn

JS:   class MyError extends Error {}
来源：http://ru.shxzskj.cn

TS:   class MyError extends Error {}
来源：http://va.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://dh.hnjuh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://it.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://xd.hahajie.cn

C#:   class MyException : Exception {}
来源：http://mo.9csxet.cn

[H05] 捕获特定类型
来源：http://zx.szsharing.cn

Py:   except ValueError as e:
来源：http://nh.nszjky.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://au.yuntaijiaju.cn

JS:   if (e instanceof TypeError) {}
来源：http://vr.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://kk.huixiangedu.cn

Java: catch (IOException | SQLException e) {}
来源：http://sf.bookmarksfly.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://of.szsharing.cn

Ruby: rescue ArgumentError => e
来源：http://lo.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wy.szxytkj.cn

[H06] 可选值 / 空值安全访问
来源：http://ym.panjiajie.cn

Py:   value = d.get("k") or default
来源：http://vp.shxzskj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://st.newstarts.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mz.hnjuh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tm.shxzukj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://md.9csxet.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ub.jianghongdianzi.cn

Ruby: d&.dig(:a, :b)
来源：http://cf.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://ds.colortex.cn

[H07] 断言
来源：http://be.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://pb.newstarts.cn

PHP:  assert($x > 0);
来源：http://xn.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://ju.yuexingan06.cn

TS:   console.assert(x > 0);
来源：http://jh.huanxung.cn

Java: assert x > 0 : "必须为正";
来源：http://eb.newstarts.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ku.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gt.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://fr.haigaiapp.cn

[H08] 获取错误信息与堆栈
来源：http://zx.szsharing.cn

Py:   str(e);  traceback.format_exc()
来源：http://qo.shxzukj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cv.shxzukj.cn

JS:   e.message;  e.stack
来源：http://gr.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bj.9csxet.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://as.szsharing.cn

Go:   err.Error()
来源：http://dj.bookmarksfly.cn

Ruby: e.message;  e.backtrace
来源：http://vz.newstarts.cn

C#:   e.Message;  e.StackTrace
来源：http://ln.huanxung.cn

[H09] 带错误码的异常
来源：http://nh.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zb.jctech888.com.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ob.bjjhwx.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ga.newstarts.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ze.shxzukj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ef.huixiangedu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zx.szxytkj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pj.nicolike.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://iq.haigaiapp.cn

[H10] 资源自动释放
来源：http://wx.szxytkj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rg.newstarts.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cp.yuexingan06.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eg.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://eh.shxzukj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xr.hnjuh.cn

Go:   defer f.Close()
来源：http://fw.muxihuayi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ex.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fg.shtwfgs.cn

================================================================================
来源：http://mc.szxytkj.cn

I. 正则表达式
来源：http://bb.hahajie.cn

================================================================================
来源：http://uj.nicolike.cn

[I01] 判断是否匹配
来源：http://fv.shxzukj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xy.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ug.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://sl.wgjwhj.cn

TS:   /\d+/.test(s)
来源：http://ps.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wl.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jv.szsharing.cn

Ruby: s.match?(/\d+/)
来源：http://cf.lnxyls.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fc.chemitech.net.cn

[I02] 提取所有匹配
来源：http://ph.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://dn.521024.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uk.bjjhwx.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://iu.szxytkj.cn

TS:   s.match(/\d+/g)
来源：http://gx.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xv.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://eu.muxihuayi.cn

Ruby: s.scan(/\d+/)
来源：http://ub.yuexingan06.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qg.jctech888.com.cn

[I03] 提取捕获分组
来源：http://iz.colortex.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ja.hnjuh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zx.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qh.shxzukj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ns.521024.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://th.panjiajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ow.bookmarksfly.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fc.jctech888.com.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bw.shxzskj.cn

[I04] 正则替换
来源：http://px.chemitech.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ji.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ty.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ye.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ai.szsharing.cn

Java: s.replaceAll("\\d+", "#")
来源：http://uf.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wj.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pf.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cv.haigaiapp.cn

[I05] 按正则拆分
来源：http://sa.9csxet.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://en.huixinmuqiang.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://uz.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://zh.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://rq.huixinmuqiang.cn

Java: s.split("\\s*,\\s*")
来源：http://hi.hahajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ub.asd995.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qw.muxihuayi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://it.huixinmuqiang.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://aq.hnjuh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.szsharing.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nw.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qy.muxihuayi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nu.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zi.521024.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rf.huanxung.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ux.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zn.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://or.haigaiapp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bk.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sj.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gf.huanxung.cn

TS:   /error/gim
来源：http://iz.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qp.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ay.shxzukj.cn

Ruby: s.scan(/error/i)
来源：http://oj.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mu.bjjhwx.cn

[I08] 贪婪与非贪婪匹配
来源：http://vy.huixiangedu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vl.newstarts.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qg.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fp.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pk.panjiajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rw.hnjuh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qx.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cw.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rv.szsharing.cn

================================================================================
来源：http://sg.jctech888.com.cn

J. 日期与时间
来源：http://et.szsharing.cn

================================================================================
来源：http://mg.szsharing.cn

[J01] 获取当前时间
来源：http://zd.lnxyls.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jf.shxzskj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://se.wgjwhj.cn

JS:   new Date();  Date.now()
来源：http://hh.lnxyls.cn

TS:   new Date();  Date.now()
来源：http://bl.nszjky.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gz.bjjhwx.cn

Go:   time.Now()
来源：http://tn.asd995.cn

Ruby: Time.now
来源：http://cq.521024.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pk.chemitech.net.cn

[J02] 格式化输出
来源：http://vb.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dg.wgjwhj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lm.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://av.huixiangedu.cn

TS:   d.toISOString()
来源：http://gm.huanxung.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tj.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ws.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tm.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gn.szsharing.cn

[J03] 字符串解析为日期
来源：http://th.jctech888.com.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ms.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bh.panjiajie.cn

JS:   new Date("2024-01-02")
来源：http://wh.muxihuayi.cn

TS:   new Date("2024-01-02")
来源：http://dv.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tr.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pi.nicolike.cn

Ruby: Date.parse("2024-01-02")
来源：http://nf.szxytkj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qc.huixinmuqiang.cn

[J04] 时间戳与日期互转
来源：http://pi.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eh.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://dw.nszjky.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://eu.bjjhwx.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://li.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cx.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hs.hnjuh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://eg.szxytkj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ux.hnjuh.cn

[J05] 时间加减（加 7 天）
来源：http://ub.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://ld.521024.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lp.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nk.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://il.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://tv.wgjwhj.cn


<!-- 参考信息 -->