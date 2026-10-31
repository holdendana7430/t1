代发 wailian999

Ruby: super
来源：http://uk.lnxyls.cn

C#:   base.Greet();
来源：http://ce.hahajie.cn

[G08] 静态方法与属性
来源：http://td.nszjky.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://op.9csxet.cn

PHP:  public static function f() {}
来源：http://mb.muxihuayi.cn

JS:   static f() {}
来源：http://nv.asd995.cn

TS:   static f(): void {}
来源：http://ls.hahajie.cn

Java: static void f() {}
来源：http://ib.huanxung.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yj.huixinmuqiang.cn

Ruby: def self.f; end
来源：http://gl.yuntaijiaju.cn

C#:   public static void F() {}
来源：http://tm.newstarts.cn

[G09] 接口 / 抽象类
来源：http://nj.yuexingan06.cn

Py:   from abc import ABC, abstractmethod
来源：http://eu.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sp.jianghongdianzi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pl.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://iy.yuexingan06.cn

Java: interface Shape { double area(); }
来源：http://hy.huanxung.cn

Go:   type Shape interface { Area() float64 }
来源：http://wg.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oz.shtwfgs.cn

C#:   interface IShape { double Area(); }
来源：http://tv.hnjuh.cn

[G10] 访问控制
来源：http://dh.jianghongdianzi.cn

Py:   约定 _protected / __private（不强制）
来源：http://qy.shxzukj.cn

PHP:  public / protected / private
来源：http://xr.asd995.cn

JS:   #private 字段；其余公开
来源：http://vh.gzmigu.cn

TS:   public / protected / private
来源：http://im.chemitech.net.cn

Java: public / protected / private / 默认包级
来源：http://re.panjiajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ew.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://pg.hnjuh.cn

C#:   public / protected / private / internal
来源：http://nm.shtwfgs.cn

[G11] getter / setter
来源：http://zq.newstarts.cn

Py:   @property 与 @x.setter
来源：http://ku.huixinmuqiang.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://og.szsharing.cn

JS:   get name() { return this._name; }
来源：http://on.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://ip.shxzskj.cn

Java: public String getName() { return name; }
来源：http://yx.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rj.hnjuh.cn

Ruby: attr_accessor :name
来源：http://mh.wgjwhj.cn

C#:   public string Name { get; set; }
来源：http://ys.jctech888.com.cn

[G12] 对象转字符串
来源：http://ig.wgjwhj.cn

Py:   def __str__(self): return self.name
来源：http://uo.bjjhwx.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ml.muxihuayi.cn

JS:   toString() { return this.name; }
来源：http://mg.521024.cn

TS:   toString(): string { return this.name; }
来源：http://lg.yuexingan06.cn

Java: @Override public String toString() { return name; }
来源：http://ve.yuexingan06.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zj.muxihuayi.cn

Ruby: def to_s; @name; end
来源：http://bn.lnxyls.cn

C#:   public override string ToString() => Name;
来源：http://vp.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://zm.muxihuayi.cn

Py:   isinstance(u, User)
来源：http://uh.muxihuayi.cn

PHP:  $u instanceof User
来源：http://oc.521024.cn

JS:   u instanceof User
来源：http://pg.szsharing.cn

TS:   u instanceof User
来源：http://pb.panjiajie.cn

Java: u instanceof User
来源：http://pa.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wu.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://vf.yuexingan06.cn

C#:   u is User
来源：http://yn.szsharing.cn

[G14] 数据类 / record
来源：http://yp.newstarts.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://iq.hahajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://yx.jianghongdianzi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://is.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://ne.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://qm.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://xz.nszjky.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vy.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://en.bookmarksfly.cn

[G15] 枚举
来源：http://nu.huixiangedu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jl.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qp.jctech888.com.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://co.lnxyls.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mq.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://mx.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tg.wgjwhj.cn

Ruby: Color = %i[red green].freeze
来源：http://zy.huixinmuqiang.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yy.muxihuayi.cn

[G16] 对象转数组 / 字典
来源：http://is.lnxyls.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://uk.jctech888.com.cn

PHP:  get_object_vars($obj);
来源：http://wq.szsharing.cn

JS:   Object.entries(obj)
来源：http://ya.newstarts.cn

TS:   Object.entries(obj)
来源：http://is.newstarts.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kn.muxihuayi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zv.newstarts.cn

Ruby: obj.instance_variables
来源：http://ok.huanxung.cn

C#:   // 用反射或 System.Text.Json
来源：http://gl.bjjhwx.cn

================================================================================
来源：http://pu.huixinmuqiang.cn

H. 异常与错误处理
来源：http://oo.shtwfgs.cn

================================================================================
来源：http://hr.newstarts.cn

[H01] try / catch 基础
来源：http://cd.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xf.nszjky.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hh.huixiangedu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://iv.hahajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pj.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vt.nicolike.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mu.shxzukj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rl.colortex.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kd.colortex.cn

[H02] finally / ensure 收尾
来源：http://kv.haigaiapp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://tn.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xf.huixinmuqiang.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://wi.huanxung.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ui.szxytkj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://nl.jctech888.com.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sp.asd995.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qb.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://om.huanxung.cn

[H03] 主动抛出异常
来源：http://qh.nicolike.cn

Py:   raise ValueError("错误信息")
来源：http://ay.shtwfgs.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dr.shtwfgs.cn

JS:   throw new Error("错误信息");
来源：http://vc.wgjwhj.cn

TS:   throw new Error("错误信息");
来源：http://et.yuntaijiaju.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://sd.huixiangedu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://et.chemitech.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qi.asd995.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yf.huixinmuqiang.cn

[H04] 自定义异常类型
来源：http://bb.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://gq.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xb.nicolike.cn

JS:   class MyError extends Error {}
来源：http://vo.szsharing.cn

TS:   class MyError extends Error {}
来源：http://la.shxzskj.cn

Java: class MyException extends RuntimeException {}
来源：http://qq.shtwfgs.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hc.szxytkj.cn

Ruby: class MyError < StandardError; end
来源：http://xk.chemitech.net.cn

C#:   class MyException : Exception {}
来源：http://wa.9csxet.cn

[H05] 捕获特定类型
来源：http://iv.lnxyls.cn

Py:   except ValueError as e:
来源：http://us.hnjuh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kx.huixiangedu.cn

JS:   if (e instanceof TypeError) {}
来源：http://xo.hahajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://ec.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://ye.jianghongdianzi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mp.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://yk.bjjhwx.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vr.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://dq.jctech888.com.cn

Py:   value = d.get("k") or default
来源：http://nf.bjjhwx.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lo.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tc.lnxyls.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cq.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ym.yuexingan06.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ng.shxzukj.cn

Ruby: d&.dig(:a, :b)
来源：http://no.chemitech.net.cn

C#:   obj?.A?.B ?? default
来源：http://bz.jianghongdianzi.cn

[H07] 断言
来源：http://gw.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://gb.yuntaijiaju.cn

PHP:  assert($x > 0);
来源：http://xx.bookmarksfly.cn

JS:   console.assert(x > 0);
来源：http://dp.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://nq.bookmarksfly.cn

Java: assert x > 0 : "必须为正";
来源：http://sx.hnjuh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://db.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zx.colortex.cn

C#:   Debug.Assert(x > 0);
来源：http://qq.newstarts.cn

[H08] 获取错误信息与堆栈
来源：http://vw.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://qe.bookmarksfly.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qi.chemitech.net.cn

JS:   e.message;  e.stack
来源：http://ua.szxytkj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ql.hnjuh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jl.nicolike.cn

Go:   err.Error()
来源：http://er.szxytkj.cn

Ruby: e.message;  e.backtrace
来源：http://js.hahajie.cn

C#:   e.Message;  e.StackTrace
来源：http://gc.521024.cn

[H09] 带错误码的异常
来源：http://zu.chemitech.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rt.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tf.jianghongdianzi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uc.yuexingan06.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kt.521024.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ok.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xo.nszjky.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ho.gzmigu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://il.newstarts.cn

[H10] 资源自动释放
来源：http://wo.yuntaijiaju.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pi.huixiangedu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vi.jctech888.com.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tu.jctech888.com.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://el.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wd.newstarts.cn

Go:   defer f.Close()
来源：http://zv.gzmigu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lz.gzmigu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bk.shxzskj.cn

================================================================================
来源：http://yr.colortex.cn

I. 正则表达式
来源：http://et.colortex.cn

================================================================================
来源：http://jh.lnxyls.cn

[I01] 判断是否匹配
来源：http://xl.szxytkj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gv.haigaiapp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gm.lnxyls.cn

JS:   /\d+/.test(s)
来源：http://nx.panjiajie.cn

TS:   /\d+/.test(s)
来源：http://rs.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pj.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hq.yuexingan06.cn

Ruby: s.match?(/\d+/)
来源：http://vv.yuntaijiaju.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://uc.newstarts.cn

[I02] 提取所有匹配
来源：http://vj.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://bc.chemitech.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bj.huanxung.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hx.colortex.cn

TS:   s.match(/\d+/g)
来源：http://yw.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xi.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ji.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://ax.bookmarksfly.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qv.lnxyls.cn

[I03] 提取捕获分组
来源：http://yo.lnxyls.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qc.9csxet.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qy.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yq.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://up.bjjhwx.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mm.yuntaijiaju.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yt.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sa.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ht.newstarts.cn

[I04] 正则替换
来源：http://rl.huixinmuqiang.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://um.colortex.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tt.9csxet.cn

JS:   s.replace(/\d+/g, "#")
来源：http://uh.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rd.jianghongdianzi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://to.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dc.huixiangedu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uj.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mb.chemitech.net.cn

[I05] 按正则拆分
来源：http://nb.shxzukj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nx.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kj.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://ry.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://em.chemitech.net.cn

Java: s.split("\\s*,\\s*")
来源：http://ke.huixinmuqiang.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vk.bookmarksfly.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gh.szxytkj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jr.521024.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uu.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sb.gzmigu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ob.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://at.asd995.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rz.9csxet.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xg.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://az.newstarts.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rf.huixinmuqiang.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sr.yuexingan06.cn

[I07] 忽略大小写与多行模式
来源：http://oa.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://pp.nszjky.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qp.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ej.huixinmuqiang.cn

TS:   /error/gim
来源：http://hn.nszjky.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kv.szxytkj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://is.521024.cn

Ruby: s.scan(/error/i)
来源：http://gp.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ha.9csxet.cn

[I08] 贪婪与非贪婪匹配
来源：http://ia.asd995.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tg.muxihuayi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cg.bookmarksfly.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://du.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tl.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kf.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://iv.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ps.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://eg.szxytkj.cn

================================================================================
来源：http://gt.521024.cn

J. 日期与时间
来源：http://mx.lnxyls.cn

================================================================================
来源：http://tf.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://ha.hnjuh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nz.hahajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bv.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://yi.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://ss.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hd.bookmarksfly.cn

Go:   time.Now()
来源：http://pk.wgjwhj.cn

Ruby: Time.now
来源：http://ci.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ma.gzmigu.cn

[J02] 格式化输出
来源：http://my.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kx.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wk.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://da.szxytkj.cn

TS:   d.toISOString()
来源：http://bm.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qs.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dc.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xg.huixiangedu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yf.shxzukj.cn

[J03] 字符串解析为日期
来源：http://bv.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rn.yuexingan06.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ds.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://sm.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://mr.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://jq.lnxyls.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ob.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://by.jctech888.com.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ev.newstarts.cn

[J04] 时间戳与日期互转
来源：http://us.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dr.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://eq.huixiangedu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rn.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hw.yuexingan06.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mg.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kw.shtwfgs.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vp.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zn.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://jx.asd995.cn

Py:   now + timedelta(days=7)
来源：http://gc.huixiangedu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nv.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hd.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://md.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://xp.bookmarksfly.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cd.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://bs.hahajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ic.szsharing.cn

[J06] 计算两时间之差
来源：http://aa.gzmigu.cn


<!-- 参考信息 -->