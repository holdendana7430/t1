代发 wailian999

Java: class Admin extends User {}
来源：http://dd.huanxung.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tp.huanxung.cn

Ruby: class Admin < User; end
来源：http://cj.panjiajie.cn

C#:   class Admin : User {}
来源：http://xp.panjiajie.cn

[G06] 重写方法
来源：http://hk.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://qp.yuexingan06.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://et.9csxet.cn

JS:   greet() { return "admin"; }
来源：http://ao.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://hy.wgjwhj.cn

Java: @Override String greet() { return "admin"; }
来源：http://qh.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ij.9csxet.cn

Ruby: def greet; "admin"; end
来源：http://xw.9csxet.cn

C#:   public override string Greet() => "admin";
来源：http://ub.bookmarksfly.cn

[G07] 调用父类方法
来源：http://pz.hahajie.cn

Py:   super().greet()
来源：http://ew.521024.cn

PHP:  parent::greet();
来源：http://gv.jianghongdianzi.cn

JS:   super.greet();
来源：http://eu.shxzskj.cn

TS:   super.greet();
来源：http://ph.huixiangedu.cn

Java: super.greet();
来源：http://ja.jianghongdianzi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fy.szxytkj.cn

Ruby: super
来源：http://se.yuexingan06.cn

C#:   base.Greet();
来源：http://ae.huanxung.cn

[G08] 静态方法与属性
来源：http://dk.wgjwhj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mb.shxzskj.cn

PHP:  public static function f() {}
来源：http://bk.asd995.cn

JS:   static f() {}
来源：http://aa.9csxet.cn

TS:   static f(): void {}
来源：http://jv.newstarts.cn

Java: static void f() {}
来源：http://oy.nicolike.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ms.gzmigu.cn

Ruby: def self.f; end
来源：http://nw.muxihuayi.cn

C#:   public static void F() {}
来源：http://sa.521024.cn

[G09] 接口 / 抽象类
来源：http://yt.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://xh.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://uy.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://rl.shxzskj.cn

TS:   interface Shape { area(): number; }
来源：http://wv.bjjhwx.cn

Java: interface Shape { double area(); }
来源：http://jy.jctech888.com.cn

Go:   type Shape interface { Area() float64 }
来源：http://ox.huixiangedu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://rk.colortex.cn

C#:   interface IShape { double Area(); }
来源：http://ve.panjiajie.cn

[G10] 访问控制
来源：http://qg.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://uj.shtwfgs.cn

PHP:  public / protected / private
来源：http://wl.panjiajie.cn

JS:   #private 字段；其余公开
来源：http://hl.shtwfgs.cn

TS:   public / protected / private
来源：http://gf.bookmarksfly.cn

Java: public / protected / private / 默认包级
来源：http://nk.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kf.szsharing.cn

Ruby: public / protected / private
来源：http://tw.huixiangedu.cn

C#:   public / protected / private / internal
来源：http://vh.szsharing.cn

[G11] getter / setter
来源：http://iu.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://ll.huixiangedu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://se.panjiajie.cn

JS:   get name() { return this._name; }
来源：http://ot.huanxung.cn

TS:   get name(): string { return this._name; }
来源：http://ud.lnxyls.cn

Java: public String getName() { return name; }
来源：http://sz.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://es.bookmarksfly.cn

Ruby: attr_accessor :name
来源：http://ak.huanxung.cn

C#:   public string Name { get; set; }
来源：http://et.newstarts.cn

[G12] 对象转字符串
来源：http://ta.521024.cn

Py:   def __str__(self): return self.name
来源：http://ap.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tp.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://cv.muxihuayi.cn

TS:   toString(): string { return this.name; }
来源：http://sr.hahajie.cn

Java: @Override public String toString() { return name; }
来源：http://sv.wgjwhj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gs.huanxung.cn

Ruby: def to_s; @name; end
来源：http://ez.chemitech.net.cn

C#:   public override string ToString() => Name;
来源：http://ac.shxzukj.cn

[G13] 判断对象类型
来源：http://hg.huixinmuqiang.cn

Py:   isinstance(u, User)
来源：http://ld.nicolike.cn

PHP:  $u instanceof User
来源：http://fn.yuntaijiaju.cn

JS:   u instanceof User
来源：http://ru.wgjwhj.cn

TS:   u instanceof User
来源：http://tj.huanxung.cn

Java: u instanceof User
来源：http://oa.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://on.shxzskj.cn

Ruby: u.is_a?(User)
来源：http://kv.shxzukj.cn

C#:   u is User
来源：http://lj.wgjwhj.cn

[G14] 数据类 / record
来源：http://kb.muxihuayi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cc.szsharing.cn

PHP:  // 用 readonly 属性模拟
来源：http://lv.asd995.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zn.521024.cn

TS:   type User = { name: string; age: number };
来源：http://fz.hahajie.cn

Java: record User(String name, int age) {}
来源：http://jq.muxihuayi.cn

Go:   type User struct { Name string; Age int }
来源：http://ol.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yy.521024.cn

C#:   record User(string Name, int Age);
来源：http://iw.lnxyls.cn

[G15] 枚举
来源：http://tp.chemitech.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ke.shxzukj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rj.szsharing.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tk.lnxyls.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ud.nszjky.cn

Java: enum Color { RED, GREEN }
来源：http://xk.szsharing.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ww.bjjhwx.cn

Ruby: Color = %i[red green].freeze
来源：http://gx.nszjky.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ql.jctech888.com.cn

[G16] 对象转数组 / 字典
来源：http://lz.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fa.chemitech.net.cn

PHP:  get_object_vars($obj);
来源：http://hk.huixiangedu.cn

JS:   Object.entries(obj)
来源：http://zi.521024.cn

TS:   Object.entries(obj)
来源：http://au.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xu.huixiangedu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://od.521024.cn

Ruby: obj.instance_variables
来源：http://hk.asd995.cn

C#:   // 用反射或 System.Text.Json
来源：http://hl.bookmarksfly.cn

================================================================================
来源：http://dg.haigaiapp.cn

H. 异常与错误处理
来源：http://gi.colortex.cn

================================================================================
来源：http://bj.panjiajie.cn

[H01] try / catch 基础
来源：http://pr.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ph.hnjuh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tn.nicolike.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ou.yuexingan06.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ir.9csxet.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eb.yuexingan06.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jo.szsharing.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://at.gzmigu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sv.yuntaijiaju.cn

[H02] finally / ensure 收尾
来源：http://xm.huanxung.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mp.nicolike.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jb.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pg.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mu.nszjky.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ym.nicolike.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qz.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tl.shtwfgs.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://as.szxytkj.cn

[H03] 主动抛出异常
来源：http://st.gzmigu.cn

Py:   raise ValueError("错误信息")
来源：http://aw.gzmigu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ug.chemitech.net.cn

JS:   throw new Error("错误信息");
来源：http://zm.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://bg.szsharing.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ff.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ob.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nt.hnjuh.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hl.shtwfgs.cn

[H04] 自定义异常类型
来源：http://cn.szsharing.cn

Py:   class MyError(Exception): pass
来源：http://yh.jianghongdianzi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://og.shxzskj.cn

JS:   class MyError extends Error {}
来源：http://qp.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://kw.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://ja.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bh.521024.cn

Ruby: class MyError < StandardError; end
来源：http://mk.nszjky.cn

C#:   class MyException : Exception {}
来源：http://tr.lnxyls.cn

[H05] 捕获特定类型
来源：http://jw.bookmarksfly.cn

Py:   except ValueError as e:
来源：http://kb.hahajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qj.huixiangedu.cn

JS:   if (e instanceof TypeError) {}
来源：http://cb.chemitech.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://bb.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://wa.shxzukj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bi.nicolike.cn

Ruby: rescue ArgumentError => e
来源：http://si.jianghongdianzi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jm.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://qx.yuexingan06.cn

Py:   value = d.get("k") or default
来源：http://dd.lnxyls.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bl.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ca.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rw.shxzukj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uc.szsharing.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ql.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://pi.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://cr.szsharing.cn

[H07] 断言
来源：http://yo.lnxyls.cn

Py:   assert x > 0, "必须为正"
来源：http://jy.huanxung.cn

PHP:  assert($x > 0);
来源：http://rj.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://zb.nszjky.cn

TS:   console.assert(x > 0);
来源：http://tb.nszjky.cn

Java: assert x > 0 : "必须为正";
来源：http://pz.asd995.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tl.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xi.jianghongdianzi.cn

C#:   Debug.Assert(x > 0);
来源：http://ih.panjiajie.cn

[H08] 获取错误信息与堆栈
来源：http://rg.huanxung.cn

Py:   str(e);  traceback.format_exc()
来源：http://sj.lnxyls.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ek.colortex.cn

JS:   e.message;  e.stack
来源：http://tz.colortex.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rp.shtwfgs.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://gj.bookmarksfly.cn

Go:   err.Error()
来源：http://gi.shxzukj.cn

Ruby: e.message;  e.backtrace
来源：http://yo.shxzukj.cn

C#:   e.Message;  e.StackTrace
来源：http://ca.haigaiapp.cn

[H09] 带错误码的异常
来源：http://km.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://el.hahajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dm.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yy.lnxyls.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cv.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ay.yuexingan06.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zp.bookmarksfly.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pe.huixiangedu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jb.szxytkj.cn

[H10] 资源自动释放
来源：http://je.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ky.nicolike.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://em.bookmarksfly.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://sp.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ym.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ax.asd995.cn

Go:   defer f.Close()
来源：http://jj.bjjhwx.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://jj.9csxet.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vx.yuexingan06.cn

================================================================================
来源：http://rk.521024.cn

I. 正则表达式
来源：http://lz.nicolike.cn

================================================================================
来源：http://bd.shxzukj.cn

[I01] 判断是否匹配
来源：http://vl.huixiangedu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ny.bookmarksfly.cn

PHP:  preg_match('/\d+/', $s);
来源：http://af.szxytkj.cn

JS:   /\d+/.test(s)
来源：http://yb.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://ln.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jf.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vj.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://kh.shxzukj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mv.hnjuh.cn

[I02] 提取所有匹配
来源：http://wy.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://em.chemitech.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vd.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vx.gzmigu.cn

TS:   s.match(/\d+/g)
来源：http://kg.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://iw.nicolike.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dc.hahajie.cn

Ruby: s.scan(/\d+/)
来源：http://wq.huixiangedu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rm.huixiangedu.cn

[I03] 提取捕获分组
来源：http://mx.szsharing.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://gl.szsharing.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mg.hnjuh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ed.shtwfgs.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://up.jctech888.com.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yy.jianghongdianzi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zl.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wy.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xm.nicolike.cn

[I04] 正则替换
来源：http://jn.muxihuayi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qs.yuexingan06.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kz.muxihuayi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://is.huixiangedu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vs.szxytkj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vk.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lo.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jn.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xu.jianghongdianzi.cn

[I05] 按正则拆分
来源：http://po.szxytkj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xo.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hu.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://go.hnjuh.cn

TS:   s.split(/\s*,\s*/)
来源：http://bk.nszjky.cn

Java: s.split("\\s*,\\s*")
来源：http://lp.nszjky.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xp.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ck.nszjky.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wg.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kg.shxzukj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bt.asd995.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kd.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lv.nicolike.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://as.szxytkj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gv.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ni.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fr.yuexingan06.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://va.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://gv.nszjky.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ua.hahajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jl.jianghongdianzi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eq.521024.cn

TS:   /error/gim
来源：http://qo.huixinmuqiang.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://so.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xd.jianghongdianzi.cn

Ruby: s.scan(/error/i)
来源：http://hn.szsharing.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://to.szsharing.cn

[I08] 贪婪与非贪婪匹配
来源：http://ml.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nq.chemitech.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ft.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://al.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zb.muxihuayi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bd.shxzukj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hl.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ao.gzmigu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://iy.chemitech.net.cn

================================================================================
来源：http://xm.szxytkj.cn

J. 日期与时间
来源：http://pn.newstarts.cn

================================================================================
来源：http://uc.colortex.cn

[J01] 获取当前时间
来源：http://sp.9csxet.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fb.gzmigu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ro.shxzukj.cn

JS:   new Date();  Date.now()
来源：http://bs.hahajie.cn

TS:   new Date();  Date.now()
来源：http://ns.newstarts.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://do.hahajie.cn

Go:   time.Now()
来源：http://ia.gzmigu.cn

Ruby: Time.now
来源：http://vs.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ql.lnxyls.cn

[J02] 格式化输出
来源：http://bg.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kh.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wx.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cg.muxihuayi.cn

TS:   d.toISOString()
来源：http://pt.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lk.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ul.bjjhwx.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ei.hahajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gb.haigaiapp.cn

[J03] 字符串解析为日期
来源：http://ni.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xf.asd995.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lf.yuntaijiaju.cn

JS:   new Date("2024-01-02")
来源：http://ym.huixinmuqiang.cn

TS:   new Date("2024-01-02")
来源：http://yh.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://du.panjiajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lw.colortex.cn

Ruby: Date.parse("2024-01-02")
来源：http://uz.colortex.cn


<!-- 参考信息 -->