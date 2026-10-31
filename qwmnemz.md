代发 wailian999

JS:   super.greet();
来源：http://xj.jctech888.com.cn

TS:   super.greet();
来源：http://dt.muxihuayi.cn

Java: super.greet();
来源：http://lm.huixiangedu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fo.szsharing.cn

Ruby: super
来源：http://qp.haigaiapp.cn

C#:   base.Greet();
来源：http://kb.hnjuh.cn

[G08] 静态方法与属性
来源：http://sy.asd995.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://tf.szsharing.cn

PHP:  public static function f() {}
来源：http://gp.chemitech.net.cn

JS:   static f() {}
来源：http://vs.jctech888.com.cn

TS:   static f(): void {}
来源：http://rw.shxzukj.cn

Java: static void f() {}
来源：http://sj.colortex.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kr.521024.cn

Ruby: def self.f; end
来源：http://qv.gzmigu.cn

C#:   public static void F() {}
来源：http://qj.bjjhwx.cn

[G09] 接口 / 抽象类
来源：http://eg.huixinmuqiang.cn

Py:   from abc import ABC, abstractmethod
来源：http://jz.huanxung.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mu.lnxyls.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mi.wgjwhj.cn

TS:   interface Shape { area(): number; }
来源：http://qu.colortex.cn

Java: interface Shape { double area(); }
来源：http://af.shxzukj.cn

Go:   type Shape interface { Area() float64 }
来源：http://lb.9csxet.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xb.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://pe.hahajie.cn

[G10] 访问控制
来源：http://dz.huixiangedu.cn

Py:   约定 _protected / __private（不强制）
来源：http://lt.muxihuayi.cn

PHP:  public / protected / private
来源：http://mg.yuexingan06.cn

JS:   #private 字段；其余公开
来源：http://hn.bjjhwx.cn

TS:   public / protected / private
来源：http://rf.shxzukj.cn

Java: public / protected / private / 默认包级
来源：http://tn.9csxet.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://oa.huixiangedu.cn

Ruby: public / protected / private
来源：http://jz.nicolike.cn

C#:   public / protected / private / internal
来源：http://uc.chemitech.net.cn

[G11] getter / setter
来源：http://bw.szxytkj.cn

Py:   @property 与 @x.setter
来源：http://gu.yuntaijiaju.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vm.muxihuayi.cn

JS:   get name() { return this._name; }
来源：http://fq.bookmarksfly.cn

TS:   get name(): string { return this._name; }
来源：http://it.nicolike.cn

Java: public String getName() { return name; }
来源：http://ia.hahajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qz.shxzukj.cn

Ruby: attr_accessor :name
来源：http://qs.szsharing.cn

C#:   public string Name { get; set; }
来源：http://bp.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://pk.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://lh.nicolike.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bc.szxytkj.cn

JS:   toString() { return this.name; }
来源：http://or.huixinmuqiang.cn

TS:   toString(): string { return this.name; }
来源：http://xj.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://qn.gzmigu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sj.asd995.cn

Ruby: def to_s; @name; end
来源：http://mb.9csxet.cn

C#:   public override string ToString() => Name;
来源：http://uk.hnjuh.cn

[G13] 判断对象类型
来源：http://ux.nicolike.cn

Py:   isinstance(u, User)
来源：http://xy.huanxung.cn

PHP:  $u instanceof User
来源：http://px.nicolike.cn

JS:   u instanceof User
来源：http://ae.hnjuh.cn

TS:   u instanceof User
来源：http://wx.9csxet.cn

Java: u instanceof User
来源：http://cy.gzmigu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ll.yuntaijiaju.cn

Ruby: u.is_a?(User)
来源：http://lj.nicolike.cn

C#:   u is User
来源：http://ji.jctech888.com.cn

[G14] 数据类 / record
来源：http://gb.yuntaijiaju.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hv.huixiangedu.cn

PHP:  // 用 readonly 属性模拟
来源：http://je.yuexingan06.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ie.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://ek.hahajie.cn

Java: record User(String name, int age) {}
来源：http://mn.hnjuh.cn

Go:   type User struct { Name string; Age int }
来源：http://ae.hnjuh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pr.huixiangedu.cn

C#:   record User(string Name, int Age);
来源：http://mg.hnjuh.cn

[G15] 枚举
来源：http://qv.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vp.huixiangedu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://po.wgjwhj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zc.haigaiapp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vg.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://sl.haigaiapp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fe.szsharing.cn

Ruby: Color = %i[red green].freeze
来源：http://nq.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lw.9csxet.cn

[G16] 对象转数组 / 字典
来源：http://bt.shxzskj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dl.nszjky.cn

PHP:  get_object_vars($obj);
来源：http://rt.lnxyls.cn

JS:   Object.entries(obj)
来源：http://ma.hnjuh.cn

TS:   Object.entries(obj)
来源：http://ba.haigaiapp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vj.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zh.nszjky.cn

Ruby: obj.instance_variables
来源：http://gs.huanxung.cn

C#:   // 用反射或 System.Text.Json
来源：http://cr.shxzskj.cn

================================================================================
来源：http://fh.shxzskj.cn

H. 异常与错误处理
来源：http://ot.jctech888.com.cn

================================================================================
来源：http://gu.hahajie.cn

[H01] try / catch 基础
来源：http://ez.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yj.nszjky.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pv.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rw.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dh.szsharing.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xs.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ri.huanxung.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://re.jianghongdianzi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lr.asd995.cn

[H02] finally / ensure 收尾
来源：http://zg.muxihuayi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://nu.nicolike.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://kf.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ki.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://uv.muxihuayi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sg.hnjuh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mf.lnxyls.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hw.huixinmuqiang.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xn.hnjuh.cn

[H03] 主动抛出异常
来源：http://yh.shxzukj.cn

Py:   raise ValueError("错误信息")
来源：http://ls.yuntaijiaju.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mo.bjjhwx.cn

JS:   throw new Error("错误信息");
来源：http://hs.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://np.shtwfgs.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tj.colortex.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bp.nicolike.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xo.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qx.chemitech.net.cn

[H04] 自定义异常类型
来源：http://rw.yuntaijiaju.cn

Py:   class MyError(Exception): pass
来源：http://yu.yuntaijiaju.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yh.newstarts.cn

JS:   class MyError extends Error {}
来源：http://bq.huixinmuqiang.cn

TS:   class MyError extends Error {}
来源：http://vt.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://xm.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://qu.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://zm.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://zx.shtwfgs.cn

[H05] 捕获特定类型
来源：http://ol.bjjhwx.cn

Py:   except ValueError as e:
来源：http://hb.bookmarksfly.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ge.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://mk.wgjwhj.cn

TS:   if (e instanceof TypeError) {}
来源：http://ur.chemitech.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://nd.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hq.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://sq.jianghongdianzi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ap.chemitech.net.cn

[H06] 可选值 / 空值安全访问
来源：http://aa.bjjhwx.cn

Py:   value = d.get("k") or default
来源：http://kc.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mf.nszjky.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ke.huanxung.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qs.yuntaijiaju.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mk.nicolike.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lo.jianghongdianzi.cn

Ruby: d&.dig(:a, :b)
来源：http://xd.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://uk.shtwfgs.cn

[H07] 断言
来源：http://xr.huixinmuqiang.cn

Py:   assert x > 0, "必须为正"
来源：http://py.huanxung.cn

PHP:  assert($x > 0);
来源：http://jt.gzmigu.cn

JS:   console.assert(x > 0);
来源：http://hu.bookmarksfly.cn

TS:   console.assert(x > 0);
来源：http://qh.szxytkj.cn

Java: assert x > 0 : "必须为正";
来源：http://em.wgjwhj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ce.haigaiapp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ya.521024.cn

C#:   Debug.Assert(x > 0);
来源：http://qp.jctech888.com.cn

[H08] 获取错误信息与堆栈
来源：http://ur.lnxyls.cn

Py:   str(e);  traceback.format_exc()
来源：http://fm.szxytkj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fi.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://tl.muxihuayi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ik.gzmigu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yf.bjjhwx.cn

Go:   err.Error()
来源：http://sg.hahajie.cn

Ruby: e.message;  e.backtrace
来源：http://tx.nszjky.cn

C#:   e.Message;  e.StackTrace
来源：http://ej.yuexingan06.cn

[H09] 带错误码的异常
来源：http://wa.huixinmuqiang.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://du.newstarts.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gn.shxzukj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yb.nszjky.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yq.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vf.lnxyls.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pv.shxzskj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://if.huixinmuqiang.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vd.asd995.cn

[H10] 资源自动释放
来源：http://ml.yuexingan06.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pp.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bc.bjjhwx.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oi.jctech888.com.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ax.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cx.muxihuayi.cn

Go:   defer f.Close()
来源：http://um.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wz.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lm.muxihuayi.cn

================================================================================
来源：http://na.hnjuh.cn

I. 正则表达式
来源：http://ar.yuexingan06.cn

================================================================================
来源：http://en.shxzukj.cn

[I01] 判断是否匹配
来源：http://ce.jianghongdianzi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ly.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sv.nszjky.cn

JS:   /\d+/.test(s)
来源：http://ay.newstarts.cn

TS:   /\d+/.test(s)
来源：http://zr.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ir.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qe.shtwfgs.cn

Ruby: s.match?(/\d+/)
来源：http://ao.shxzskj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nl.newstarts.cn

[I02] 提取所有匹配
来源：http://rs.panjiajie.cn

Py:   re.findall(r"\d+", s)
来源：http://yi.huixiangedu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://as.muxihuayi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ej.hnjuh.cn

TS:   s.match(/\d+/g)
来源：http://ok.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://na.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gy.bookmarksfly.cn

Ruby: s.scan(/\d+/)
来源：http://ko.shxzukj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://af.huixiangedu.cn

[I03] 提取捕获分组
来源：http://kz.panjiajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vc.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vk.gzmigu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://og.wgjwhj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://it.bjjhwx.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vy.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://se.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mi.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yl.jctech888.com.cn

[I04] 正则替换
来源：http://rf.bjjhwx.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jd.shtwfgs.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sz.shxzskj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xe.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pu.szxytkj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://io.panjiajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kw.szxytkj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gp.yuexingan06.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://us.shxzskj.cn

[I05] 按正则拆分
来源：http://xl.panjiajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://aj.521024.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vf.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://ek.hahajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://hq.asd995.cn

Java: s.split("\\s*,\\s*")
来源：http://rn.szsharing.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nm.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mi.shtwfgs.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hd.521024.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ys.shxzukj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rn.yuexingan06.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ks.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gf.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ql.521024.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zc.huixinmuqiang.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vv.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ka.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gq.newstarts.cn

[I07] 忽略大小写与多行模式
来源：http://jr.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://gb.hahajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vx.9csxet.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oc.shxzukj.cn

TS:   /error/gim
来源：http://um.nszjky.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://eu.jctech888.com.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ho.9csxet.cn

Ruby: s.scan(/error/i)
来源：http://je.jianghongdianzi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yl.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://xb.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ax.yuexingan06.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jc.newstarts.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pz.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ya.hahajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gh.521024.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jx.newstarts.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nm.newstarts.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ol.szsharing.cn

================================================================================
来源：http://lw.szxytkj.cn

J. 日期与时间
来源：http://qs.shtwfgs.cn

================================================================================
来源：http://ik.jctech888.com.cn

[J01] 获取当前时间
来源：http://ui.colortex.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gz.chemitech.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yl.shxzukj.cn

JS:   new Date();  Date.now()
来源：http://mm.nszjky.cn

TS:   new Date();  Date.now()
来源：http://uy.nszjky.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zk.521024.cn

Go:   time.Now()
来源：http://im.yuexingan06.cn

Ruby: Time.now
来源：http://hz.chemitech.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cw.huixiangedu.cn

[J02] 格式化输出
来源：http://iu.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kd.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bl.jianghongdianzi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vi.panjiajie.cn

TS:   d.toISOString()
来源：http://jl.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vn.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://il.nszjky.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vo.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ke.hahajie.cn

[J03] 字符串解析为日期
来源：http://zw.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ke.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ys.521024.cn

JS:   new Date("2024-01-02")
来源：http://yv.jctech888.com.cn

TS:   new Date("2024-01-02")
来源：http://uy.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ug.wgjwhj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nt.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://jf.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wz.nszjky.cn

[J04] 时间戳与日期互转
来源：http://xu.huanxung.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rt.shxzukj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bs.jctech888.com.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zy.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jp.yuexingan06.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xo.chemitech.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://en.jctech888.com.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vg.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uk.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://qn.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://tj.hahajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ay.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ir.nszjky.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ue.huixiangedu.cn

Java: LocalDate.now().plusDays(7)
来源：http://wb.newstarts.cn


<!-- 参考信息 -->