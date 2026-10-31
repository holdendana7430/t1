代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://fv.chemitech.net.cn

[G07] 调用父类方法
来源：http://nj.wgjwhj.cn

Py:   super().greet()
来源：http://un.asd995.cn

PHP:  parent::greet();
来源：http://ou.hahajie.cn

JS:   super.greet();
来源：http://jg.shxzukj.cn

TS:   super.greet();
来源：http://tc.jianghongdianzi.cn

Java: super.greet();
来源：http://it.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fq.asd995.cn

Ruby: super
来源：http://rj.bookmarksfly.cn

C#:   base.Greet();
来源：http://nl.haigaiapp.cn

[G08] 静态方法与属性
来源：http://ho.chemitech.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vu.shxzukj.cn

PHP:  public static function f() {}
来源：http://dt.jianghongdianzi.cn

JS:   static f() {}
来源：http://je.521024.cn

TS:   static f(): void {}
来源：http://la.gzmigu.cn

Java: static void f() {}
来源：http://io.yuexingan06.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bs.colortex.cn

Ruby: def self.f; end
来源：http://lg.gzmigu.cn

C#:   public static void F() {}
来源：http://tf.bookmarksfly.cn

[G09] 接口 / 抽象类
来源：http://hd.huixinmuqiang.cn

Py:   from abc import ABC, abstractmethod
来源：http://fe.jctech888.com.cn

PHP:  interface Shape { public function area(): float; }
来源：http://sf.gzmigu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pc.shxzskj.cn

TS:   interface Shape { area(): number; }
来源：http://ti.bookmarksfly.cn

Java: interface Shape { double area(); }
来源：http://py.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://bp.asd995.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nc.shxzskj.cn

C#:   interface IShape { double Area(); }
来源：http://fx.shtwfgs.cn

[G10] 访问控制
来源：http://iu.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://dn.chemitech.net.cn

PHP:  public / protected / private
来源：http://rq.hnjuh.cn

JS:   #private 字段；其余公开
来源：http://iw.asd995.cn

TS:   public / protected / private
来源：http://dk.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://gh.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ms.newstarts.cn

Ruby: public / protected / private
来源：http://gh.huanxung.cn

C#:   public / protected / private / internal
来源：http://uj.asd995.cn

[G11] getter / setter
来源：http://be.muxihuayi.cn

Py:   @property 与 @x.setter
来源：http://fx.hnjuh.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://df.yuexingan06.cn

JS:   get name() { return this._name; }
来源：http://ph.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://tg.huixinmuqiang.cn

Java: public String getName() { return name; }
来源：http://yu.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ln.shxzukj.cn

Ruby: attr_accessor :name
来源：http://dd.jianghongdianzi.cn

C#:   public string Name { get; set; }
来源：http://bd.szxytkj.cn

[G12] 对象转字符串
来源：http://ho.yuexingan06.cn

Py:   def __str__(self): return self.name
来源：http://ft.9csxet.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ny.chemitech.net.cn

JS:   toString() { return this.name; }
来源：http://lc.lnxyls.cn

TS:   toString(): string { return this.name; }
来源：http://ef.lnxyls.cn

Java: @Override public String toString() { return name; }
来源：http://qz.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://la.wgjwhj.cn

Ruby: def to_s; @name; end
来源：http://lx.colortex.cn

C#:   public override string ToString() => Name;
来源：http://st.szxytkj.cn

[G13] 判断对象类型
来源：http://bt.newstarts.cn

Py:   isinstance(u, User)
来源：http://ps.nicolike.cn

PHP:  $u instanceof User
来源：http://lu.shxzukj.cn

JS:   u instanceof User
来源：http://cz.bookmarksfly.cn

TS:   u instanceof User
来源：http://gx.muxihuayi.cn

Java: u instanceof User
来源：http://nl.hnjuh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ja.521024.cn

Ruby: u.is_a?(User)
来源：http://by.shxzskj.cn

C#:   u is User
来源：http://gk.huixinmuqiang.cn

[G14] 数据类 / record
来源：http://sl.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ph.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://ya.hnjuh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hy.yuexingan06.cn

TS:   type User = { name: string; age: number };
来源：http://zf.lnxyls.cn

Java: record User(String name, int age) {}
来源：http://ah.chemitech.net.cn

Go:   type User struct { Name string; Age int }
来源：http://ds.hnjuh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tz.panjiajie.cn

C#:   record User(string Name, int Age);
来源：http://ec.szxytkj.cn

[G15] 枚举
来源：http://wz.chemitech.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hp.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ou.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yc.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yu.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://dj.nicolike.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pq.bookmarksfly.cn

Ruby: Color = %i[red green].freeze
来源：http://aa.hahajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rs.yuntaijiaju.cn

[G16] 对象转数组 / 字典
来源：http://fe.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sr.jctech888.com.cn

PHP:  get_object_vars($obj);
来源：http://ij.bjjhwx.cn

JS:   Object.entries(obj)
来源：http://sy.panjiajie.cn

TS:   Object.entries(obj)
来源：http://fs.hnjuh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://rb.shxzukj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gr.gzmigu.cn

Ruby: obj.instance_variables
来源：http://bt.521024.cn

C#:   // 用反射或 System.Text.Json
来源：http://cz.wgjwhj.cn

================================================================================
来源：http://pf.shxzukj.cn

H. 异常与错误处理
来源：http://td.szsharing.cn

================================================================================
来源：http://ej.521024.cn

[H01] try / catch 基础
来源：http://wm.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://it.yuexingan06.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mo.szsharing.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://op.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://to.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pr.yuntaijiaju.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ip.gzmigu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zt.wgjwhj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jr.bookmarksfly.cn

[H02] finally / ensure 收尾
来源：http://rk.9csxet.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yf.jianghongdianzi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nq.jianghongdianzi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tx.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://yn.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ef.hnjuh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mz.yuntaijiaju.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ku.muxihuayi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bj.haigaiapp.cn

[H03] 主动抛出异常
来源：http://rf.gzmigu.cn

Py:   raise ValueError("错误信息")
来源：http://kd.hnjuh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://df.nicolike.cn

JS:   throw new Error("错误信息");
来源：http://gu.chemitech.net.cn

TS:   throw new Error("错误信息");
来源：http://cg.jctech888.com.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ny.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tz.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ve.huixiangedu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://cy.shxzskj.cn

[H04] 自定义异常类型
来源：http://tl.gzmigu.cn

Py:   class MyError(Exception): pass
来源：http://qf.9csxet.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rb.gzmigu.cn

JS:   class MyError extends Error {}
来源：http://sv.panjiajie.cn

TS:   class MyError extends Error {}
来源：http://cy.shxzskj.cn

Java: class MyException extends RuntimeException {}
来源：http://qv.bookmarksfly.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cb.yuntaijiaju.cn

Ruby: class MyError < StandardError; end
来源：http://hm.newstarts.cn

C#:   class MyException : Exception {}
来源：http://lx.nszjky.cn

[H05] 捕获特定类型
来源：http://zk.haigaiapp.cn

Py:   except ValueError as e:
来源：http://vm.asd995.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://al.hahajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://tq.wgjwhj.cn

TS:   if (e instanceof TypeError) {}
来源：http://nh.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://wl.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xg.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://cq.wgjwhj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://da.yuntaijiaju.cn

[H06] 可选值 / 空值安全访问
来源：http://zy.huixiangedu.cn

Py:   value = d.get("k") or default
来源：http://yz.huixiangedu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pc.hnjuh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xn.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rm.jianghongdianzi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fr.shxzukj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://eh.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://mp.hnjuh.cn

C#:   obj?.A?.B ?? default
来源：http://ni.chemitech.net.cn

[H07] 断言
来源：http://xb.jianghongdianzi.cn

Py:   assert x > 0, "必须为正"
来源：http://ro.huanxung.cn

PHP:  assert($x > 0);
来源：http://gr.lnxyls.cn

JS:   console.assert(x > 0);
来源：http://ml.szxytkj.cn

TS:   console.assert(x > 0);
来源：http://tq.hahajie.cn

Java: assert x > 0 : "必须为正";
来源：http://ho.jctech888.com.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ox.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xa.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://em.nszjky.cn

[H08] 获取错误信息与堆栈
来源：http://vp.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://ee.chemitech.net.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pg.521024.cn

JS:   e.message;  e.stack
来源：http://kc.gzmigu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hn.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tm.asd995.cn

Go:   err.Error()
来源：http://hs.yuntaijiaju.cn

Ruby: e.message;  e.backtrace
来源：http://do.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://qu.chemitech.net.cn

[H09] 带错误码的异常
来源：http://ym.shxzukj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hk.hahajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vo.huixiangedu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yc.lnxyls.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mj.huixiangedu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gp.wgjwhj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jy.newstarts.cn

Ruby: raise MyError.new("fail", 500)
来源：http://of.lnxyls.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ec.huanxung.cn

[H10] 资源自动释放
来源：http://xa.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ql.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qz.huanxung.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qh.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sq.haigaiapp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mh.hahajie.cn

Go:   defer f.Close()
来源：http://mw.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gv.hahajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ii.hnjuh.cn

================================================================================
来源：http://fc.shxzukj.cn

I. 正则表达式
来源：http://hw.shxzukj.cn

================================================================================
来源：http://so.hnjuh.cn

[I01] 判断是否匹配
来源：http://iw.shtwfgs.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xs.haigaiapp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kr.huixinmuqiang.cn

JS:   /\d+/.test(s)
来源：http://ay.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://bu.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ld.9csxet.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://av.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://he.hahajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gv.hahajie.cn

[I02] 提取所有匹配
来源：http://oq.panjiajie.cn

Py:   re.findall(r"\d+", s)
来源：http://st.hnjuh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://da.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://by.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://ph.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tu.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://js.panjiajie.cn

Ruby: s.scan(/\d+/)
来源：http://fh.huixinmuqiang.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iy.9csxet.cn

[I03] 提取捕获分组
来源：http://yd.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cr.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ws.szsharing.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dp.521024.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ix.muxihuayi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zn.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://os.yuexingan06.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ib.wgjwhj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cv.asd995.cn

[I04] 正则替换
来源：http://xl.jctech888.com.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zu.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://im.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://oe.muxihuayi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ex.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wd.szsharing.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uc.chemitech.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yu.shtwfgs.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ng.haigaiapp.cn

[I05] 按正则拆分
来源：http://xk.muxihuayi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://uj.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ds.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://aw.chemitech.net.cn

TS:   s.split(/\s*,\s*/)
来源：http://td.shtwfgs.cn

Java: s.split("\\s*,\\s*")
来源：http://dv.gzmigu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eg.szsharing.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gw.nicolike.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pb.shtwfgs.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xh.hnjuh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vn.newstarts.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tx.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://re.asd995.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xy.szxytkj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cs.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fq.hnjuh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://je.newstarts.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vs.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://ni.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://br.haigaiapp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nq.shxzskj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zq.muxihuayi.cn

TS:   /error/gim
来源：http://st.muxihuayi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://is.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oa.521024.cn

Ruby: s.scan(/error/i)
来源：http://yq.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sn.colortex.cn

[I08] 贪婪与非贪婪匹配
来源：http://dj.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zm.jctech888.com.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://eu.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qe.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dx.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mm.bjjhwx.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wy.newstarts.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ao.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tp.nszjky.cn

================================================================================
来源：http://pg.panjiajie.cn

J. 日期与时间
来源：http://uw.bjjhwx.cn

================================================================================
来源：http://zt.bjjhwx.cn

[J01] 获取当前时间
来源：http://dy.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fi.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sz.jianghongdianzi.cn

JS:   new Date();  Date.now()
来源：http://pd.bjjhwx.cn

TS:   new Date();  Date.now()
来源：http://fr.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://af.bookmarksfly.cn

Go:   time.Now()
来源：http://je.huixinmuqiang.cn

Ruby: Time.now
来源：http://oq.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ce.szsharing.cn

[J02] 格式化输出
来源：http://tt.lnxyls.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dr.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bi.yuntaijiaju.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fp.nicolike.cn

TS:   d.toISOString()
来源：http://kw.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qv.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kq.521024.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://em.szxytkj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cq.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://ai.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jc.bookmarksfly.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pm.shxzskj.cn

JS:   new Date("2024-01-02")
来源：http://va.jctech888.com.cn

TS:   new Date("2024-01-02")
来源：http://op.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fn.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fe.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://ub.bookmarksfly.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bd.huanxung.cn

[J04] 时间戳与日期互转
来源：http://ws.shtwfgs.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fr.szxytkj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bf.newstarts.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wz.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bh.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yc.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://cn.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tz.yuntaijiaju.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qg.hahajie.cn

[J05] 时间加减（加 7 天）
来源：http://jv.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://hg.gzmigu.cn


<!-- 参考信息 -->