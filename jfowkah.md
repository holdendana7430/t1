代发 wailian999

Py:   class Admin(User): pass
来源：http://hk.hahajie.cn

PHP:  class Admin extends User {}
来源：http://vb.colortex.cn

JS:   class Admin extends User {}
来源：http://xi.521024.cn

TS:   class Admin extends User {}
来源：http://hq.huanxung.cn

Java: class Admin extends User {}
来源：http://ne.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://pw.hnjuh.cn

Ruby: class Admin < User; end
来源：http://qw.yuntaijiaju.cn

C#:   class Admin : User {}
来源：http://ig.huixinmuqiang.cn

[G06] 重写方法
来源：http://kw.wgjwhj.cn

Py:   def greet(self): return "admin"
来源：http://qa.bookmarksfly.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zz.szxytkj.cn

JS:   greet() { return "admin"; }
来源：http://vm.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://xg.asd995.cn

Java: @Override String greet() { return "admin"; }
来源：http://kc.521024.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ho.szxytkj.cn

Ruby: def greet; "admin"; end
来源：http://oh.hnjuh.cn

C#:   public override string Greet() => "admin";
来源：http://fh.9csxet.cn

[G07] 调用父类方法
来源：http://pi.yuexingan06.cn

Py:   super().greet()
来源：http://gj.haigaiapp.cn

PHP:  parent::greet();
来源：http://er.hnjuh.cn

JS:   super.greet();
来源：http://cm.wgjwhj.cn

TS:   super.greet();
来源：http://ca.shtwfgs.cn

Java: super.greet();
来源：http://kv.colortex.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://im.shtwfgs.cn

Ruby: super
来源：http://mw.shxzskj.cn

C#:   base.Greet();
来源：http://ys.muxihuayi.cn

[G08] 静态方法与属性
来源：http://ai.asd995.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wl.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://cq.shxzukj.cn

JS:   static f() {}
来源：http://cz.huanxung.cn

TS:   static f(): void {}
来源：http://nw.szsharing.cn

Java: static void f() {}
来源：http://py.huanxung.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rs.yuexingan06.cn

Ruby: def self.f; end
来源：http://ct.haigaiapp.cn

C#:   public static void F() {}
来源：http://sa.nszjky.cn

[G09] 接口 / 抽象类
来源：http://nj.newstarts.cn

Py:   from abc import ABC, abstractmethod
来源：http://fu.lnxyls.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ms.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vl.asd995.cn

TS:   interface Shape { area(): number; }
来源：http://vj.9csxet.cn

Java: interface Shape { double area(); }
来源：http://jz.szsharing.cn

Go:   type Shape interface { Area() float64 }
来源：http://df.9csxet.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gu.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://ia.colortex.cn

[G10] 访问控制
来源：http://tm.huixiangedu.cn

Py:   约定 _protected / __private（不强制）
来源：http://bn.jctech888.com.cn

PHP:  public / protected / private
来源：http://lh.bookmarksfly.cn

JS:   #private 字段；其余公开
来源：http://al.huixiangedu.cn

TS:   public / protected / private
来源：http://pn.shxzukj.cn

Java: public / protected / private / 默认包级
来源：http://mv.hahajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jh.panjiajie.cn

Ruby: public / protected / private
来源：http://me.nicolike.cn

C#:   public / protected / private / internal
来源：http://aj.lnxyls.cn

[G11] getter / setter
来源：http://sl.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://mm.521024.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ke.huanxung.cn

JS:   get name() { return this._name; }
来源：http://km.bjjhwx.cn

TS:   get name(): string { return this._name; }
来源：http://sj.colortex.cn

Java: public String getName() { return name; }
来源：http://hy.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ts.lnxyls.cn

Ruby: attr_accessor :name
来源：http://rk.szxytkj.cn

C#:   public string Name { get; set; }
来源：http://ph.521024.cn

[G12] 对象转字符串
来源：http://bz.gzmigu.cn

Py:   def __str__(self): return self.name
来源：http://wi.lnxyls.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gu.gzmigu.cn

JS:   toString() { return this.name; }
来源：http://st.hahajie.cn

TS:   toString(): string { return this.name; }
来源：http://gl.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://lt.chemitech.net.cn

Go:   func (u User) String() string { return u.Name }
来源：http://me.huanxung.cn

Ruby: def to_s; @name; end
来源：http://bg.panjiajie.cn

C#:   public override string ToString() => Name;
来源：http://ud.lnxyls.cn

[G13] 判断对象类型
来源：http://zy.shxzskj.cn

Py:   isinstance(u, User)
来源：http://je.newstarts.cn

PHP:  $u instanceof User
来源：http://eb.hnjuh.cn

JS:   u instanceof User
来源：http://cu.bookmarksfly.cn

TS:   u instanceof User
来源：http://ht.bookmarksfly.cn

Java: u instanceof User
来源：http://sr.shxzskj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://te.nszjky.cn

Ruby: u.is_a?(User)
来源：http://qs.wgjwhj.cn

C#:   u is User
来源：http://hf.haigaiapp.cn

[G14] 数据类 / record
来源：http://qu.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pi.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://jp.shtwfgs.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gy.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://mr.521024.cn

Java: record User(String name, int age) {}
来源：http://gz.chemitech.net.cn

Go:   type User struct { Name string; Age int }
来源：http://pv.muxihuayi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ue.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://tr.shxzskj.cn

[G15] 枚举
来源：http://ra.gzmigu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ne.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kb.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tt.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rr.gzmigu.cn

Java: enum Color { RED, GREEN }
来源：http://bj.bookmarksfly.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mi.shxzukj.cn

Ruby: Color = %i[red green].freeze
来源：http://gi.szxytkj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ws.hnjuh.cn

[G16] 对象转数组 / 字典
来源：http://hd.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ib.gzmigu.cn

PHP:  get_object_vars($obj);
来源：http://wb.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://rt.yuntaijiaju.cn

TS:   Object.entries(obj)
来源：http://bd.muxihuayi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zm.bookmarksfly.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hb.huixiangedu.cn

Ruby: obj.instance_variables
来源：http://qp.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://ov.shtwfgs.cn

================================================================================
来源：http://ai.bjjhwx.cn

H. 异常与错误处理
来源：http://ur.huanxung.cn

================================================================================
来源：http://mb.newstarts.cn

[H01] try / catch 基础
来源：http://do.hnjuh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fj.yuexingan06.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jz.bookmarksfly.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nn.yuexingan06.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oj.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yv.yuexingan06.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://co.jctech888.com.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://rg.wgjwhj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ss.szsharing.cn

[H02] finally / ensure 收尾
来源：http://ue.newstarts.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xk.lnxyls.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://uo.jianghongdianzi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://eo.huanxung.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://sv.huanxung.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lb.huixinmuqiang.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bt.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://no.shtwfgs.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ll.521024.cn

[H03] 主动抛出异常
来源：http://fm.colortex.cn

Py:   raise ValueError("错误信息")
来源：http://fg.wgjwhj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://th.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://sv.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://ds.newstarts.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jr.huanxung.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ju.muxihuayi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yp.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zd.wgjwhj.cn

[H04] 自定义异常类型
来源：http://sf.yuntaijiaju.cn

Py:   class MyError(Exception): pass
来源：http://vd.jianghongdianzi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ds.shxzukj.cn

JS:   class MyError extends Error {}
来源：http://av.wgjwhj.cn

TS:   class MyError extends Error {}
来源：http://if.9csxet.cn

Java: class MyException extends RuntimeException {}
来源：http://bl.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bc.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://hj.szsharing.cn

C#:   class MyException : Exception {}
来源：http://wa.huanxung.cn

[H05] 捕获特定类型
来源：http://rp.hahajie.cn

Py:   except ValueError as e:
来源：http://me.jianghongdianzi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ek.wgjwhj.cn

JS:   if (e instanceof TypeError) {}
来源：http://lk.nicolike.cn

TS:   if (e instanceof TypeError) {}
来源：http://kj.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://bh.9csxet.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://jv.shxzskj.cn

Ruby: rescue ArgumentError => e
来源：http://bk.gzmigu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://bp.yuexingan06.cn

[H06] 可选值 / 空值安全访问
来源：http://sa.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://vg.yuexingan06.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ol.lnxyls.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wj.colortex.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fl.bjjhwx.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sa.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xk.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://rz.521024.cn

C#:   obj?.A?.B ?? default
来源：http://qu.huanxung.cn

[H07] 断言
来源：http://dg.shtwfgs.cn

Py:   assert x > 0, "必须为正"
来源：http://jh.shxzskj.cn

PHP:  assert($x > 0);
来源：http://ru.9csxet.cn

JS:   console.assert(x > 0);
来源：http://hs.szxytkj.cn

TS:   console.assert(x > 0);
来源：http://lh.hnjuh.cn

Java: assert x > 0 : "必须为正";
来源：http://oe.nszjky.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rz.huixiangedu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vm.haigaiapp.cn

C#:   Debug.Assert(x > 0);
来源：http://hg.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://em.bjjhwx.cn

Py:   str(e);  traceback.format_exc()
来源：http://zs.jctech888.com.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tt.newstarts.cn

JS:   e.message;  e.stack
来源：http://rg.gzmigu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://is.jianghongdianzi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fd.colortex.cn

Go:   err.Error()
来源：http://bs.colortex.cn

Ruby: e.message;  e.backtrace
来源：http://js.chemitech.net.cn

C#:   e.Message;  e.StackTrace
来源：http://xk.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://ru.9csxet.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://op.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yt.9csxet.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ez.hnjuh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tb.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://af.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kg.newstarts.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jc.shtwfgs.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rt.wgjwhj.cn

[H10] 资源自动释放
来源：http://as.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://go.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hy.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rn.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ke.bookmarksfly.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ve.muxihuayi.cn

Go:   defer f.Close()
来源：http://fo.colortex.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yj.9csxet.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ph.hnjuh.cn

================================================================================
来源：http://zi.yuexingan06.cn

I. 正则表达式
来源：http://jw.shxzukj.cn

================================================================================
来源：http://hb.gzmigu.cn

[I01] 判断是否匹配
来源：http://pn.muxihuayi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jp.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kt.szsharing.cn

JS:   /\d+/.test(s)
来源：http://xz.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://fq.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kn.9csxet.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sg.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://yw.huixinmuqiang.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cd.521024.cn

[I02] 提取所有匹配
来源：http://qs.huixinmuqiang.cn

Py:   re.findall(r"\d+", s)
来源：http://rd.huixinmuqiang.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ih.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://za.szsharing.cn

TS:   s.match(/\d+/g)
来源：http://ff.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bz.asd995.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vk.bookmarksfly.cn

Ruby: s.scan(/\d+/)
来源：http://xz.lnxyls.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kp.wgjwhj.cn

[I03] 提取捕获分组
来源：http://rp.bookmarksfly.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://er.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ae.gzmigu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fa.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fv.huixiangedu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://eo.jctech888.com.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pl.jianghongdianzi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lm.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pq.panjiajie.cn

[I04] 正则替换
来源：http://df.nszjky.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ay.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://no.nicolike.cn

JS:   s.replace(/\d+/g, "#")
来源：http://tj.muxihuayi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jc.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vi.yuexingan06.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mq.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xe.shxzskj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tt.521024.cn

[I05] 按正则拆分
来源：http://rm.colortex.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xs.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cq.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://zf.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://qj.asd995.cn

Java: s.split("\\s*,\\s*")
来源：http://ew.chemitech.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fc.lnxyls.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gj.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yr.haigaiapp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ff.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ur.yuexingan06.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bj.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rk.asd995.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dx.521024.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://re.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yk.shxzskj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ul.colortex.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lq.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://mo.szsharing.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lp.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://dw.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pr.bookmarksfly.cn

TS:   /error/gim
来源：http://cp.huixinmuqiang.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xp.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dl.jctech888.com.cn

Ruby: s.scan(/error/i)
来源：http://ii.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://go.chemitech.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://ls.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gr.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qb.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://um.521024.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ld.shxzukj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jo.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gj.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wr.huanxung.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vq.jianghongdianzi.cn

================================================================================
来源：http://nr.wgjwhj.cn

J. 日期与时间
来源：http://qq.panjiajie.cn

================================================================================
来源：http://az.bjjhwx.cn

[J01] 获取当前时间
来源：http://ut.panjiajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zh.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zd.nszjky.cn

JS:   new Date();  Date.now()
来源：http://mo.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://zu.newstarts.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kz.9csxet.cn

Go:   time.Now()
来源：http://vk.yuexingan06.cn

Ruby: Time.now
来源：http://yi.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kd.gzmigu.cn

[J02] 格式化输出
来源：http://uv.jianghongdianzi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yo.yuexingan06.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gh.hnjuh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mn.gzmigu.cn

TS:   d.toISOString()
来源：http://ms.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qa.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yi.nszjky.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zi.huixiangedu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ne.hnjuh.cn

[J03] 字符串解析为日期
来源：http://zk.panjiajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lq.asd995.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tx.colortex.cn

JS:   new Date("2024-01-02")
来源：http://sn.muxihuayi.cn


<!-- 参考信息 -->