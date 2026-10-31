代发 wailian999

Ruby: super
来源：http://ub.hnjuh.cn

C#:   base.Greet();
来源：http://qt.lnxyls.cn

[G08] 静态方法与属性
来源：http://xi.huanxung.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zb.bjjhwx.cn

PHP:  public static function f() {}
来源：http://nj.521024.cn

JS:   static f() {}
来源：http://jz.panjiajie.cn

TS:   static f(): void {}
来源：http://hp.szxytkj.cn

Java: static void f() {}
来源：http://uf.nicolike.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fd.colortex.cn

Ruby: def self.f; end
来源：http://zr.yuexingan06.cn

C#:   public static void F() {}
来源：http://xh.huixinmuqiang.cn

[G09] 接口 / 抽象类
来源：http://mh.huixinmuqiang.cn

Py:   from abc import ABC, abstractmethod
来源：http://ua.shtwfgs.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wf.jctech888.com.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://fo.hahajie.cn

TS:   interface Shape { area(): number; }
来源：http://gr.bjjhwx.cn

Java: interface Shape { double area(); }
来源：http://cm.yuexingan06.cn

Go:   type Shape interface { Area() float64 }
来源：http://te.yuntaijiaju.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://zh.colortex.cn

C#:   interface IShape { double Area(); }
来源：http://kd.yuexingan06.cn

[G10] 访问控制
来源：http://uo.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://dm.jianghongdianzi.cn

PHP:  public / protected / private
来源：http://ab.jctech888.com.cn

JS:   #private 字段；其余公开
来源：http://ig.muxihuayi.cn

TS:   public / protected / private
来源：http://hj.huixiangedu.cn

Java: public / protected / private / 默认包级
来源：http://zb.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qu.hnjuh.cn

Ruby: public / protected / private
来源：http://pq.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://oa.szxytkj.cn

[G11] getter / setter
来源：http://fb.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://ff.jctech888.com.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ew.szxytkj.cn

JS:   get name() { return this._name; }
来源：http://of.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://av.shxzskj.cn

Java: public String getName() { return name; }
来源：http://bd.hahajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mu.yuexingan06.cn

Ruby: attr_accessor :name
来源：http://zh.shxzskj.cn

C#:   public string Name { get; set; }
来源：http://ct.bookmarksfly.cn

[G12] 对象转字符串
来源：http://ps.yuexingan06.cn

Py:   def __str__(self): return self.name
来源：http://ly.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tk.colortex.cn

JS:   toString() { return this.name; }
来源：http://ki.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://sx.hnjuh.cn

Java: @Override public String toString() { return name; }
来源：http://ot.huixinmuqiang.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ld.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://ku.jianghongdianzi.cn

C#:   public override string ToString() => Name;
来源：http://pk.shxzukj.cn

[G13] 判断对象类型
来源：http://uw.gzmigu.cn

Py:   isinstance(u, User)
来源：http://yw.shxzskj.cn

PHP:  $u instanceof User
来源：http://dg.haigaiapp.cn

JS:   u instanceof User
来源：http://kq.asd995.cn

TS:   u instanceof User
来源：http://be.521024.cn

Java: u instanceof User
来源：http://ks.jianghongdianzi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ke.nicolike.cn

Ruby: u.is_a?(User)
来源：http://aa.shtwfgs.cn

C#:   u is User
来源：http://ma.chemitech.net.cn

[G14] 数据类 / record
来源：http://bj.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xh.yuntaijiaju.cn

PHP:  // 用 readonly 属性模拟
来源：http://en.521024.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cd.huanxung.cn

TS:   type User = { name: string; age: number };
来源：http://ir.hahajie.cn

Java: record User(String name, int age) {}
来源：http://nv.nszjky.cn

Go:   type User struct { Name string; Age int }
来源：http://az.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lc.haigaiapp.cn

C#:   record User(string Name, int Age);
来源：http://fi.yuntaijiaju.cn

[G15] 枚举
来源：http://qm.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wf.jianghongdianzi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nw.jctech888.com.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ix.haigaiapp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://da.bookmarksfly.cn

Java: enum Color { RED, GREEN }
来源：http://nv.yuntaijiaju.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zx.huixinmuqiang.cn

Ruby: Color = %i[red green].freeze
来源：http://cl.lnxyls.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ze.lnxyls.cn

[G16] 对象转数组 / 字典
来源：http://sk.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zq.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://tl.jianghongdianzi.cn

JS:   Object.entries(obj)
来源：http://oj.asd995.cn

TS:   Object.entries(obj)
来源：http://jy.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wh.hnjuh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://an.nszjky.cn

Ruby: obj.instance_variables
来源：http://hd.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://dt.huixinmuqiang.cn

================================================================================
来源：http://ao.panjiajie.cn

H. 异常与错误处理
来源：http://gx.szxytkj.cn

================================================================================
来源：http://az.wgjwhj.cn

[H01] try / catch 基础
来源：http://ac.muxihuayi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qj.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://er.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xy.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qw.yuexingan06.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gi.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yt.haigaiapp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jv.bjjhwx.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://do.huixiangedu.cn

[H02] finally / ensure 收尾
来源：http://dt.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qb.asd995.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fr.yuntaijiaju.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://iv.shxzukj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hv.9csxet.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fv.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ak.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tp.yuexingan06.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xh.huixinmuqiang.cn

[H03] 主动抛出异常
来源：http://bw.yuntaijiaju.cn

Py:   raise ValueError("错误信息")
来源：http://qt.hnjuh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tq.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://vt.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://qz.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ue.szxytkj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rc.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wn.hahajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jn.yuexingan06.cn

[H04] 自定义异常类型
来源：http://kp.panjiajie.cn

Py:   class MyError(Exception): pass
来源：http://zj.wgjwhj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bg.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://oz.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://ku.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://sy.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vf.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://up.panjiajie.cn

C#:   class MyException : Exception {}
来源：http://qd.yuexingan06.cn

[H05] 捕获特定类型
来源：http://wi.huixiangedu.cn

Py:   except ValueError as e:
来源：http://ti.wgjwhj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qw.shxzskj.cn

JS:   if (e instanceof TypeError) {}
来源：http://pq.huanxung.cn

TS:   if (e instanceof TypeError) {}
来源：http://ii.bookmarksfly.cn

Java: catch (IOException | SQLException e) {}
来源：http://or.panjiajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gs.yuexingan06.cn

Ruby: rescue ArgumentError => e
来源：http://is.jctech888.com.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ne.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://iq.521024.cn

Py:   value = d.get("k") or default
来源：http://mo.lnxyls.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ex.nszjky.cn

JS:   obj?.a?.b;  d ?? default
来源：http://nh.hnjuh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wk.huixiangedu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mj.jctech888.com.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ll.jctech888.com.cn

Ruby: d&.dig(:a, :b)
来源：http://um.huanxung.cn

C#:   obj?.A?.B ?? default
来源：http://kw.muxihuayi.cn

[H07] 断言
来源：http://sy.bjjhwx.cn

Py:   assert x > 0, "必须为正"
来源：http://zb.huixinmuqiang.cn

PHP:  assert($x > 0);
来源：http://mt.lnxyls.cn

JS:   console.assert(x > 0);
来源：http://fm.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://ct.yuexingan06.cn

Java: assert x > 0 : "必须为正";
来源：http://cl.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ue.yuexingan06.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xi.hahajie.cn

C#:   Debug.Assert(x > 0);
来源：http://zk.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://vf.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://rr.nicolike.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lw.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://wz.yuexingan06.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yo.newstarts.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://co.lnxyls.cn

Go:   err.Error()
来源：http://dh.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://mz.jctech888.com.cn

C#:   e.Message;  e.StackTrace
来源：http://fi.9csxet.cn

[H09] 带错误码的异常
来源：http://tu.521024.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oy.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zd.lnxyls.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://et.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jm.shxzskj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wa.gzmigu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ih.asd995.cn

Ruby: raise MyError.new("fail", 500)
来源：http://am.huixinmuqiang.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://st.szsharing.cn

[H10] 资源自动释放
来源：http://hk.szsharing.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ci.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://qg.9csxet.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oj.szsharing.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ap.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hp.9csxet.cn

Go:   defer f.Close()
来源：http://it.yuexingan06.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tq.bjjhwx.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ix.panjiajie.cn

================================================================================
来源：http://nf.szxytkj.cn

I. 正则表达式
来源：http://zu.yuexingan06.cn

================================================================================
来源：http://pi.9csxet.cn

[I01] 判断是否匹配
来源：http://by.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oj.newstarts.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ki.bjjhwx.cn

JS:   /\d+/.test(s)
来源：http://cf.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://dw.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jk.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gf.haigaiapp.cn

Ruby: s.match?(/\d+/)
来源：http://zw.huixinmuqiang.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://nr.haigaiapp.cn

[I02] 提取所有匹配
来源：http://cj.nicolike.cn

Py:   re.findall(r"\d+", s)
来源：http://gv.jianghongdianzi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nm.bookmarksfly.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mb.colortex.cn

TS:   s.match(/\d+/g)
来源：http://kh.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://pq.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://aj.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://st.yuexingan06.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://eh.shtwfgs.cn

[I03] 提取捕获分组
来源：http://vl.yuexingan06.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lo.bookmarksfly.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ig.yuexingan06.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wl.9csxet.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://it.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eo.szxytkj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://de.huixiangedu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qt.bookmarksfly.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kk.asd995.cn

[I04] 正则替换
来源：http://zi.asd995.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qx.szxytkj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jd.muxihuayi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wi.gzmigu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wk.shxzskj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://me.shtwfgs.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ld.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yd.hahajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ad.nszjky.cn

[I05] 按正则拆分
来源：http://ys.szxytkj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://od.haigaiapp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vx.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://ma.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://rb.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://jm.huixiangedu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bg.panjiajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ry.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://id.huixiangedu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vc.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xj.muxihuayi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ji.asd995.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zp.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wg.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fo.muxihuayi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://nz.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ts.yuntaijiaju.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jn.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://tp.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lj.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://os.newstarts.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pq.szxytkj.cn

TS:   /error/gim
来源：http://xu.huixinmuqiang.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qx.yuexingan06.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ul.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://fu.jianghongdianzi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hs.nszjky.cn

[I08] 贪婪与非贪婪匹配
来源：http://ye.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ze.colortex.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pd.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pj.gzmigu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zf.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qn.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mr.newstarts.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ez.hahajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sv.9csxet.cn

================================================================================
来源：http://ej.asd995.cn

J. 日期与时间
来源：http://as.shxzukj.cn

================================================================================
来源：http://lj.shtwfgs.cn

[J01] 获取当前时间
来源：http://dw.jianghongdianzi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://di.bookmarksfly.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ca.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://bx.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://uc.szxytkj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://af.jianghongdianzi.cn

Go:   time.Now()
来源：http://qq.jctech888.com.cn

Ruby: Time.now
来源：http://it.colortex.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ne.wgjwhj.cn

[J02] 格式化输出
来源：http://gh.hnjuh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ea.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lt.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ws.shtwfgs.cn

TS:   d.toISOString()
来源：http://pz.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fv.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ge.panjiajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dz.huixinmuqiang.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://in.shxzskj.cn

[J03] 字符串解析为日期
来源：http://uf.521024.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ee.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nt.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://ne.muxihuayi.cn

TS:   new Date("2024-01-02")
来源：http://er.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://if.haigaiapp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hb.colortex.cn

Ruby: Date.parse("2024-01-02")
来源：http://io.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jw.huixiangedu.cn

[J04] 时间戳与日期互转
来源：http://md.nicolike.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bc.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iv.szsharing.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ua.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wl.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qn.jctech888.com.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ch.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ja.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://du.shtwfgs.cn

[J05] 时间加减（加 7 天）
来源：http://dp.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://md.huixinmuqiang.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vz.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://kh.szxytkj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pn.colortex.cn

Java: LocalDate.now().plusDays(7)
来源：http://ma.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zr.hnjuh.cn

Ruby: Time.now + 7 * 86400
来源：http://qx.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://th.shxzukj.cn

[J06] 计算两时间之差
来源：http://ot.colortex.cn


<!-- 参考信息 -->