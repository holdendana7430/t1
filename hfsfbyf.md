代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://vt.lnxyls.cn

Java: @Override String greet() { return "admin"; }
来源：http://gw.jctech888.com.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dv.newstarts.cn

Ruby: def greet; "admin"; end
来源：http://iu.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://sh.gzmigu.cn

[G07] 调用父类方法
来源：http://df.colortex.cn

Py:   super().greet()
来源：http://dx.jianghongdianzi.cn

PHP:  parent::greet();
来源：http://dz.jctech888.com.cn

JS:   super.greet();
来源：http://ju.szxytkj.cn

TS:   super.greet();
来源：http://jt.gzmigu.cn

Java: super.greet();
来源：http://wx.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sj.jctech888.com.cn

Ruby: super
来源：http://az.huixinmuqiang.cn

C#:   base.Greet();
来源：http://ck.haigaiapp.cn

[G08] 静态方法与属性
来源：http://rj.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://dx.chemitech.net.cn

PHP:  public static function f() {}
来源：http://hy.szxytkj.cn

JS:   static f() {}
来源：http://gp.hnjuh.cn

TS:   static f(): void {}
来源：http://hq.yuexingan06.cn

Java: static void f() {}
来源：http://nl.gzmigu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://cz.newstarts.cn

Ruby: def self.f; end
来源：http://gn.jctech888.com.cn

C#:   public static void F() {}
来源：http://ax.shxzukj.cn

[G09] 接口 / 抽象类
来源：http://wp.9csxet.cn

Py:   from abc import ABC, abstractmethod
来源：http://gz.asd995.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zf.9csxet.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xz.newstarts.cn

TS:   interface Shape { area(): number; }
来源：http://nb.wgjwhj.cn

Java: interface Shape { double area(); }
来源：http://ji.521024.cn

Go:   type Shape interface { Area() float64 }
来源：http://jg.newstarts.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ea.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://ug.chemitech.net.cn

[G10] 访问控制
来源：http://pk.hnjuh.cn

Py:   约定 _protected / __private（不强制）
来源：http://ea.hnjuh.cn

PHP:  public / protected / private
来源：http://oz.szsharing.cn

JS:   #private 字段；其余公开
来源：http://ym.panjiajie.cn

TS:   public / protected / private
来源：http://qp.huanxung.cn

Java: public / protected / private / 默认包级
来源：http://vl.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cc.colortex.cn

Ruby: public / protected / private
来源：http://wo.gzmigu.cn

C#:   public / protected / private / internal
来源：http://oz.shtwfgs.cn

[G11] getter / setter
来源：http://xv.colortex.cn

Py:   @property 与 @x.setter
来源：http://li.wgjwhj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://rl.szsharing.cn

JS:   get name() { return this._name; }
来源：http://qr.wgjwhj.cn

TS:   get name(): string { return this._name; }
来源：http://qt.huanxung.cn

Java: public String getName() { return name; }
来源：http://us.wgjwhj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mm.bookmarksfly.cn

Ruby: attr_accessor :name
来源：http://ui.colortex.cn

C#:   public string Name { get; set; }
来源：http://cv.bjjhwx.cn

[G12] 对象转字符串
来源：http://rc.muxihuayi.cn

Py:   def __str__(self): return self.name
来源：http://qg.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wz.nszjky.cn

JS:   toString() { return this.name; }
来源：http://cx.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://rw.shxzukj.cn

Java: @Override public String toString() { return name; }
来源：http://ku.yuexingan06.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vg.yuntaijiaju.cn

Ruby: def to_s; @name; end
来源：http://pi.shxzukj.cn

C#:   public override string ToString() => Name;
来源：http://ji.asd995.cn

[G13] 判断对象类型
来源：http://fw.huixinmuqiang.cn

Py:   isinstance(u, User)
来源：http://zo.newstarts.cn

PHP:  $u instanceof User
来源：http://ll.jianghongdianzi.cn

JS:   u instanceof User
来源：http://wo.yuexingan06.cn

TS:   u instanceof User
来源：http://hv.jianghongdianzi.cn

Java: u instanceof User
来源：http://ur.gzmigu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://yt.gzmigu.cn

Ruby: u.is_a?(User)
来源：http://ux.newstarts.cn

C#:   u is User
来源：http://wq.szsharing.cn

[G14] 数据类 / record
来源：http://dz.521024.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cc.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://gh.jctech888.com.cn

JS:   // 无内置：普通类或对象字面量
来源：http://za.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://vu.newstarts.cn

Java: record User(String name, int age) {}
来源：http://dl.nszjky.cn

Go:   type User struct { Name string; Age int }
来源：http://ha.newstarts.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ay.newstarts.cn

C#:   record User(string Name, int Age);
来源：http://xz.haigaiapp.cn

[G15] 枚举
来源：http://zx.asd995.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zx.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bp.shxzukj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ps.haigaiapp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://es.wgjwhj.cn

Java: enum Color { RED, GREEN }
来源：http://gl.szsharing.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://nm.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://tp.wgjwhj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zt.jctech888.com.cn

[G16] 对象转数组 / 字典
来源：http://lt.asd995.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zx.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://av.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://ly.wgjwhj.cn

TS:   Object.entries(obj)
来源：http://qm.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://oe.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fv.hahajie.cn

Ruby: obj.instance_variables
来源：http://on.hnjuh.cn

C#:   // 用反射或 System.Text.Json
来源：http://zh.hahajie.cn

================================================================================
来源：http://nj.jctech888.com.cn

H. 异常与错误处理
来源：http://tj.bjjhwx.cn

================================================================================
来源：http://av.shtwfgs.cn

[H01] try / catch 基础
来源：http://ba.jianghongdianzi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://oa.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jc.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ra.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qk.chemitech.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gu.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tu.gzmigu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uq.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sp.9csxet.cn

[H02] finally / ensure 收尾
来源：http://ra.haigaiapp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sx.shxzukj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://uc.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tk.szxytkj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qi.wgjwhj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lv.muxihuayi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gh.szsharing.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gy.shxzukj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lj.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://pe.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://az.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qh.newstarts.cn

JS:   throw new Error("错误信息");
来源：http://og.panjiajie.cn

TS:   throw new Error("错误信息");
来源：http://nz.521024.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nw.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ed.wgjwhj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gw.shxzskj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fx.szsharing.cn

[H04] 自定义异常类型
来源：http://gy.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://zf.jianghongdianzi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gl.yuntaijiaju.cn

JS:   class MyError extends Error {}
来源：http://ac.nicolike.cn

TS:   class MyError extends Error {}
来源：http://ri.szsharing.cn

Java: class MyException extends RuntimeException {}
来源：http://ce.yuntaijiaju.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yi.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://ll.hahajie.cn

C#:   class MyException : Exception {}
来源：http://fl.nszjky.cn

[H05] 捕获特定类型
来源：http://xp.shxzukj.cn

Py:   except ValueError as e:
来源：http://dk.gzmigu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vw.yuntaijiaju.cn

JS:   if (e instanceof TypeError) {}
来源：http://fv.chemitech.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://zl.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://ve.yuexingan06.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xu.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://lj.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ou.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://ao.hnjuh.cn

Py:   value = d.get("k") or default
来源：http://hs.panjiajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rb.nszjky.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ug.bookmarksfly.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gg.hahajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jj.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wo.chemitech.net.cn

Ruby: d&.dig(:a, :b)
来源：http://zq.newstarts.cn

C#:   obj?.A?.B ?? default
来源：http://ex.9csxet.cn

[H07] 断言
来源：http://ej.shxzskj.cn

Py:   assert x > 0, "必须为正"
来源：http://xl.colortex.cn

PHP:  assert($x > 0);
来源：http://db.lnxyls.cn

JS:   console.assert(x > 0);
来源：http://uh.huanxung.cn

TS:   console.assert(x > 0);
来源：http://vs.jctech888.com.cn

Java: assert x > 0 : "必须为正";
来源：http://tc.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://is.nicolike.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xm.panjiajie.cn

C#:   Debug.Assert(x > 0);
来源：http://pa.bjjhwx.cn

[H08] 获取错误信息与堆栈
来源：http://wj.haigaiapp.cn

Py:   str(e);  traceback.format_exc()
来源：http://ie.yuexingan06.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vd.521024.cn

JS:   e.message;  e.stack
来源：http://sm.muxihuayi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://na.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://up.huixiangedu.cn

Go:   err.Error()
来源：http://ro.szsharing.cn

Ruby: e.message;  e.backtrace
来源：http://pn.nszjky.cn

C#:   e.Message;  e.StackTrace
来源：http://gi.haigaiapp.cn

[H09] 带错误码的异常
来源：http://bz.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://et.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ms.newstarts.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ap.lnxyls.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cg.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://el.9csxet.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mj.gzmigu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mr.chemitech.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ph.gzmigu.cn

[H10] 资源自动释放
来源：http://jb.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ny.jctech888.com.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lo.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://iz.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rk.yuntaijiaju.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wn.asd995.cn

Go:   defer f.Close()
来源：http://so.huixiangedu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vz.chemitech.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mb.9csxet.cn

================================================================================
来源：http://ci.yuexingan06.cn

I. 正则表达式
来源：http://om.521024.cn

================================================================================
来源：http://ws.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://hm.jianghongdianzi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dh.szxytkj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vc.hnjuh.cn

JS:   /\d+/.test(s)
来源：http://za.nszjky.cn

TS:   /\d+/.test(s)
来源：http://gi.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://du.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pb.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://oj.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://il.colortex.cn

[I02] 提取所有匹配
来源：http://tm.nicolike.cn

Py:   re.findall(r"\d+", s)
来源：http://hh.jianghongdianzi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vz.lnxyls.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bj.nszjky.cn

TS:   s.match(/\d+/g)
来源：http://fd.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oj.colortex.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jn.hahajie.cn

Ruby: s.scan(/\d+/)
来源：http://dh.newstarts.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://my.wgjwhj.cn

[I03] 提取捕获分组
来源：http://jw.shtwfgs.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cl.muxihuayi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dh.szsharing.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dv.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fl.szsharing.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cr.yuexingan06.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fh.521024.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ol.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ua.shtwfgs.cn

[I04] 正则替换
来源：http://pa.bjjhwx.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lo.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ne.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ud.huixinmuqiang.cn

TS:   s.replace(/\d+/g, "#")
来源：http://av.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mi.huixinmuqiang.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://yj.haigaiapp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fa.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vj.panjiajie.cn

[I05] 按正则拆分
来源：http://zm.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fl.wgjwhj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kr.colortex.cn

JS:   s.split(/\s*,\s*/)
来源：http://rn.shtwfgs.cn

TS:   s.split(/\s*,\s*/)
来源：http://gl.yuexingan06.cn

Java: s.split("\\s*,\\s*")
来源：http://tb.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://dc.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zo.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jy.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://la.szsharing.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ki.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bt.lnxyls.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vn.wgjwhj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qm.gzmigu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gi.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dg.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gj.yuntaijiaju.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://df.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://pi.colortex.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ws.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xv.jianghongdianzi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fz.shxzukj.cn

TS:   /error/gim
来源：http://rr.jianghongdianzi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://be.newstarts.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sb.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://zw.yuntaijiaju.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ya.huixiangedu.cn

[I08] 贪婪与非贪婪匹配
来源：http://ed.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://do.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fw.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cy.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gz.muxihuayi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://te.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qc.jctech888.com.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lq.panjiajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mi.shxzskj.cn

================================================================================
来源：http://ow.hahajie.cn

J. 日期与时间
来源：http://jb.huixiangedu.cn

================================================================================
来源：http://bb.521024.cn

[J01] 获取当前时间
来源：http://wj.colortex.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qu.huanxung.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zs.huanxung.cn

JS:   new Date();  Date.now()
来源：http://wk.chemitech.net.cn

TS:   new Date();  Date.now()
来源：http://mo.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ga.hnjuh.cn

Go:   time.Now()
来源：http://dl.yuexingan06.cn

Ruby: Time.now
来源：http://fd.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pt.hahajie.cn

[J02] 格式化输出
来源：http://wd.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://il.panjiajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://sw.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xa.panjiajie.cn

TS:   d.toISOString()
来源：http://kx.asd995.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yr.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://cu.hnjuh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nz.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ez.yuntaijiaju.cn

[J03] 字符串解析为日期
来源：http://ld.chemitech.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tf.yuexingan06.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pv.9csxet.cn

JS:   new Date("2024-01-02")
来源：http://wq.shxzskj.cn

TS:   new Date("2024-01-02")
来源：http://ix.huixinmuqiang.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sz.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cq.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://oq.huixiangedu.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tg.jianghongdianzi.cn

[J04] 时间戳与日期互转
来源：http://ii.muxihuayi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nf.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ob.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://xd.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vx.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sn.lnxyls.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sn.colortex.cn


<!-- 参考信息 -->