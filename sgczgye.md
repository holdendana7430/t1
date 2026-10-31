代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://pn.yuntaijiaju.cn

Java: @Override String greet() { return "admin"; }
来源：http://lk.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rp.hahajie.cn

Ruby: def greet; "admin"; end
来源：http://po.hnjuh.cn

C#:   public override string Greet() => "admin";
来源：http://qk.gzmigu.cn

[G07] 调用父类方法
来源：http://ld.bookmarksfly.cn

Py:   super().greet()
来源：http://bk.9csxet.cn

PHP:  parent::greet();
来源：http://wk.huanxung.cn

JS:   super.greet();
来源：http://tr.521024.cn

TS:   super.greet();
来源：http://ad.jianghongdianzi.cn

Java: super.greet();
来源：http://yp.szsharing.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iw.yuntaijiaju.cn

Ruby: super
来源：http://au.nicolike.cn

C#:   base.Greet();
来源：http://qr.jianghongdianzi.cn

[G08] 静态方法与属性
来源：http://ib.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ae.huanxung.cn

PHP:  public static function f() {}
来源：http://qq.haigaiapp.cn

JS:   static f() {}
来源：http://ur.nicolike.cn

TS:   static f(): void {}
来源：http://vl.panjiajie.cn

Java: static void f() {}
来源：http://mv.yuexingan06.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qy.haigaiapp.cn

Ruby: def self.f; end
来源：http://om.huixiangedu.cn

C#:   public static void F() {}
来源：http://lh.bjjhwx.cn

[G09] 接口 / 抽象类
来源：http://yv.gzmigu.cn

Py:   from abc import ABC, abstractmethod
来源：http://oa.haigaiapp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lo.huanxung.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://do.colortex.cn

TS:   interface Shape { area(): number; }
来源：http://rj.chemitech.net.cn

Java: interface Shape { double area(); }
来源：http://qb.lnxyls.cn

Go:   type Shape interface { Area() float64 }
来源：http://qm.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ef.szsharing.cn

C#:   interface IShape { double Area(); }
来源：http://en.yuntaijiaju.cn

[G10] 访问控制
来源：http://bs.9csxet.cn

Py:   约定 _protected / __private（不强制）
来源：http://oa.hahajie.cn

PHP:  public / protected / private
来源：http://qb.panjiajie.cn

JS:   #private 字段；其余公开
来源：http://se.jctech888.com.cn

TS:   public / protected / private
来源：http://xx.jianghongdianzi.cn

Java: public / protected / private / 默认包级
来源：http://vj.hnjuh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://il.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://do.shxzskj.cn

C#:   public / protected / private / internal
来源：http://mh.gzmigu.cn

[G11] getter / setter
来源：http://fe.gzmigu.cn

Py:   @property 与 @x.setter
来源：http://rw.bookmarksfly.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ln.colortex.cn

JS:   get name() { return this._name; }
来源：http://ne.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://xx.szsharing.cn

Java: public String getName() { return name; }
来源：http://lg.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bh.hahajie.cn

Ruby: attr_accessor :name
来源：http://ez.szsharing.cn

C#:   public string Name { get; set; }
来源：http://ta.gzmigu.cn

[G12] 对象转字符串
来源：http://zh.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://sh.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://di.9csxet.cn

JS:   toString() { return this.name; }
来源：http://wm.bjjhwx.cn

TS:   toString(): string { return this.name; }
来源：http://ix.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://cu.lnxyls.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kr.asd995.cn

Ruby: def to_s; @name; end
来源：http://hc.haigaiapp.cn

C#:   public override string ToString() => Name;
来源：http://nk.szsharing.cn

[G13] 判断对象类型
来源：http://pf.hahajie.cn

Py:   isinstance(u, User)
来源：http://td.huixiangedu.cn

PHP:  $u instanceof User
来源：http://sf.huixinmuqiang.cn

JS:   u instanceof User
来源：http://xr.shxzskj.cn

TS:   u instanceof User
来源：http://my.haigaiapp.cn

Java: u instanceof User
来源：http://ms.hahajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://an.yuntaijiaju.cn

Ruby: u.is_a?(User)
来源：http://dt.hahajie.cn

C#:   u is User
来源：http://oz.shxzukj.cn

[G14] 数据类 / record
来源：http://jk.jianghongdianzi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rr.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://px.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://md.yuexingan06.cn

TS:   type User = { name: string; age: number };
来源：http://xf.haigaiapp.cn

Java: record User(String name, int age) {}
来源：http://la.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://xz.hahajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hp.bjjhwx.cn

C#:   record User(string Name, int Age);
来源：http://dj.hahajie.cn

[G15] 枚举
来源：http://ic.haigaiapp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jf.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://uc.asd995.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ym.gzmigu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://au.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://xx.hahajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xp.gzmigu.cn

Ruby: Color = %i[red green].freeze
来源：http://kr.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cb.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://zc.9csxet.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dh.shtwfgs.cn

PHP:  get_object_vars($obj);
来源：http://yc.huanxung.cn

JS:   Object.entries(obj)
来源：http://cb.hahajie.cn

TS:   Object.entries(obj)
来源：http://pr.newstarts.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kv.nicolike.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://in.bjjhwx.cn

Ruby: obj.instance_variables
来源：http://rm.jctech888.com.cn

C#:   // 用反射或 System.Text.Json
来源：http://ul.muxihuayi.cn

================================================================================
来源：http://oj.chemitech.net.cn

H. 异常与错误处理
来源：http://nu.szsharing.cn

================================================================================
来源：http://fm.nszjky.cn

[H01] try / catch 基础
来源：http://rz.bjjhwx.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tg.bjjhwx.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pn.asd995.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ib.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lk.521024.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qq.huixinmuqiang.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sj.bjjhwx.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://co.asd995.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iw.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://ca.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qw.yuntaijiaju.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://po.521024.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pb.huixinmuqiang.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rz.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://nv.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://eb.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gk.newstarts.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jr.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://ip.bookmarksfly.cn

Py:   raise ValueError("错误信息")
来源：http://li.newstarts.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dt.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://ic.bookmarksfly.cn

TS:   throw new Error("错误信息");
来源：http://gs.shtwfgs.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hi.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://te.panjiajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nj.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yp.szxytkj.cn

[H04] 自定义异常类型
来源：http://ge.9csxet.cn

Py:   class MyError(Exception): pass
来源：http://dt.gzmigu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ft.huixiangedu.cn

JS:   class MyError extends Error {}
来源：http://za.chemitech.net.cn

TS:   class MyError extends Error {}
来源：http://ea.newstarts.cn

Java: class MyException extends RuntimeException {}
来源：http://vy.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://td.szxytkj.cn

Ruby: class MyError < StandardError; end
来源：http://gs.nszjky.cn

C#:   class MyException : Exception {}
来源：http://yb.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://cj.panjiajie.cn

Py:   except ValueError as e:
来源：http://in.shxzukj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ec.muxihuayi.cn

JS:   if (e instanceof TypeError) {}
来源：http://pv.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://qa.jianghongdianzi.cn

Java: catch (IOException | SQLException e) {}
来源：http://ke.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://iz.bjjhwx.cn

Ruby: rescue ArgumentError => e
来源：http://ff.bjjhwx.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://gc.nicolike.cn

[H06] 可选值 / 空值安全访问
来源：http://tu.shxzukj.cn

Py:   value = d.get("k") or default
来源：http://sd.gzmigu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lv.hahajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://np.szxytkj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zp.panjiajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qt.wgjwhj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vn.shxzukj.cn

Ruby: d&.dig(:a, :b)
来源：http://tq.yuexingan06.cn

C#:   obj?.A?.B ?? default
来源：http://ry.hahajie.cn

[H07] 断言
来源：http://sc.nszjky.cn

Py:   assert x > 0, "必须为正"
来源：http://ya.nicolike.cn

PHP:  assert($x > 0);
来源：http://bp.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://ro.nszjky.cn

TS:   console.assert(x > 0);
来源：http://ea.bookmarksfly.cn

Java: assert x > 0 : "必须为正";
来源：http://ue.yuexingan06.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xt.yuntaijiaju.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nz.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://zf.9csxet.cn

[H08] 获取错误信息与堆栈
来源：http://tm.bookmarksfly.cn

Py:   str(e);  traceback.format_exc()
来源：http://uf.asd995.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xp.bjjhwx.cn

JS:   e.message;  e.stack
来源：http://if.yuntaijiaju.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vk.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://og.gzmigu.cn

Go:   err.Error()
来源：http://cp.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://nr.nicolike.cn

C#:   e.Message;  e.StackTrace
来源：http://hf.colortex.cn

[H09] 带错误码的异常
来源：http://ts.chemitech.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://du.newstarts.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://fh.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ut.wgjwhj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://st.nicolike.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tq.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hs.szxytkj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dx.szsharing.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ff.nicolike.cn

[H10] 资源自动释放
来源：http://aq.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://az.jctech888.com.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wr.hahajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gd.gzmigu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ku.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qb.shxzukj.cn

Go:   defer f.Close()
来源：http://dx.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sc.chemitech.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zk.shtwfgs.cn

================================================================================
来源：http://dl.szxytkj.cn

I. 正则表达式
来源：http://he.huanxung.cn

================================================================================
来源：http://tt.szxytkj.cn

[I01] 判断是否匹配
来源：http://vk.shxzukj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cj.lnxyls.cn

PHP:  preg_match('/\d+/', $s);
来源：http://my.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://ky.newstarts.cn

TS:   /\d+/.test(s)
来源：http://fl.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yt.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wv.hnjuh.cn

Ruby: s.match?(/\d+/)
来源：http://as.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://is.shxzukj.cn

[I02] 提取所有匹配
来源：http://uz.szxytkj.cn

Py:   re.findall(r"\d+", s)
来源：http://uu.9csxet.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rr.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sl.nszjky.cn

TS:   s.match(/\d+/g)
来源：http://zb.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oi.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sv.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://hj.lnxyls.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zo.shxzskj.cn

[I03] 提取捕获分组
来源：http://mn.chemitech.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ru.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ws.9csxet.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vd.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ng.9csxet.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dy.muxihuayi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ku.yuexingan06.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://xf.haigaiapp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gj.szxytkj.cn

[I04] 正则替换
来源：http://cb.chemitech.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hv.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vh.hnjuh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ee.huixiangedu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wn.jctech888.com.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zi.yuexingan06.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lg.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://os.nszjky.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pi.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://ks.hahajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xv.haigaiapp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://wu.panjiajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://wx.bjjhwx.cn

TS:   s.split(/\s*,\s*/)
来源：http://uq.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://we.9csxet.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qu.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yx.521024.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lm.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sg.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nl.haigaiapp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mj.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dv.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kw.nszjky.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fz.huanxung.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fh.wgjwhj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ua.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rc.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://ku.gzmigu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ik.huixinmuqiang.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://se.lnxyls.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qc.521024.cn

TS:   /error/gim
来源：http://ur.nszjky.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ah.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ir.colortex.cn

Ruby: s.scan(/error/i)
来源：http://vy.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://su.newstarts.cn

[I08] 贪婪与非贪婪匹配
来源：http://zu.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yn.muxihuayi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zq.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ko.bookmarksfly.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ff.szxytkj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cw.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ac.huanxung.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kl.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://er.lnxyls.cn

================================================================================
来源：http://vn.huanxung.cn

J. 日期与时间
来源：http://sr.newstarts.cn

================================================================================
来源：http://nk.colortex.cn

[J01] 获取当前时间
来源：http://zl.nszjky.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qp.huanxung.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rw.nicolike.cn

JS:   new Date();  Date.now()
来源：http://xz.panjiajie.cn

TS:   new Date();  Date.now()
来源：http://ns.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fs.hahajie.cn

Go:   time.Now()
来源：http://ux.huixiangedu.cn

Ruby: Time.now
来源：http://ef.lnxyls.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qb.colortex.cn

[J02] 格式化输出
来源：http://vh.bjjhwx.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cc.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hk.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dk.huixinmuqiang.cn

TS:   d.toISOString()
来源：http://if.jianghongdianzi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ux.yuexingan06.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fs.bjjhwx.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ug.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wi.haigaiapp.cn

[J03] 字符串解析为日期
来源：http://zm.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hg.lnxyls.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fn.szxytkj.cn

JS:   new Date("2024-01-02")
来源：http://xj.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://mf.shxzukj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yh.9csxet.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://es.shtwfgs.cn

Ruby: Date.parse("2024-01-02")
来源：http://yy.szsharing.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mn.hahajie.cn

[J04] 时间戳与日期互转
来源：http://fl.huanxung.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hl.nszjky.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ak.9csxet.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ct.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gk.haigaiapp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pd.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qj.muxihuayi.cn


<!-- 参考信息 -->