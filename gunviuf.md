代发 wailian999

Ruby: @name = "x"
来源：http://ns.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://rs.huixiangedu.cn

[G04] 定义方法
来源：http://dn.yuntaijiaju.cn

Py:   def greet(self): return self.name
来源：http://wa.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sk.huanxung.cn

JS:   greet() { return this.name; }
来源：http://qu.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://ta.muxihuayi.cn

Java: String greet() { return name; }
来源：http://dx.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://aj.nicolike.cn

Ruby: def greet; @name; end
来源：http://mb.nicolike.cn

C#:   public string Greet() => Name;
来源：http://cl.huanxung.cn

[G05] 继承
来源：http://bz.lnxyls.cn

Py:   class Admin(User): pass
来源：http://pl.shtwfgs.cn

PHP:  class Admin extends User {}
来源：http://nk.lnxyls.cn

JS:   class Admin extends User {}
来源：http://jp.hahajie.cn

TS:   class Admin extends User {}
来源：http://qg.shtwfgs.cn

Java: class Admin extends User {}
来源：http://xl.huixiangedu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zs.wgjwhj.cn

Ruby: class Admin < User; end
来源：http://os.haigaiapp.cn

C#:   class Admin : User {}
来源：http://fm.gzmigu.cn

[G06] 重写方法
来源：http://dh.9csxet.cn

Py:   def greet(self): return "admin"
来源：http://ug.hnjuh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gb.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://el.lnxyls.cn

TS:   greet(): string { return "admin"; }
来源：http://om.colortex.cn

Java: @Override String greet() { return "admin"; }
来源：http://ji.shxzskj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gi.jianghongdianzi.cn

Ruby: def greet; "admin"; end
来源：http://jk.huanxung.cn

C#:   public override string Greet() => "admin";
来源：http://ow.huanxung.cn

[G07] 调用父类方法
来源：http://dk.shtwfgs.cn

Py:   super().greet()
来源：http://dv.hnjuh.cn

PHP:  parent::greet();
来源：http://oh.lnxyls.cn

JS:   super.greet();
来源：http://qg.wgjwhj.cn

TS:   super.greet();
来源：http://ka.shtwfgs.cn

Java: super.greet();
来源：http://my.bookmarksfly.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ci.lnxyls.cn

Ruby: super
来源：http://ra.newstarts.cn

C#:   base.Greet();
来源：http://fm.yuntaijiaju.cn

[G08] 静态方法与属性
来源：http://qy.haigaiapp.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ml.huixiangedu.cn

PHP:  public static function f() {}
来源：http://av.panjiajie.cn

JS:   static f() {}
来源：http://us.shxzukj.cn

TS:   static f(): void {}
来源：http://fn.jianghongdianzi.cn

Java: static void f() {}
来源：http://na.shtwfgs.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://og.jctech888.com.cn

Ruby: def self.f; end
来源：http://eh.yuntaijiaju.cn

C#:   public static void F() {}
来源：http://rb.szsharing.cn

[G09] 接口 / 抽象类
来源：http://wf.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://fy.chemitech.net.cn

PHP:  interface Shape { public function area(): float; }
来源：http://iq.haigaiapp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://my.huanxung.cn

TS:   interface Shape { area(): number; }
来源：http://tm.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://nd.yuexingan06.cn

Go:   type Shape interface { Area() float64 }
来源：http://zv.panjiajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://dc.nszjky.cn

C#:   interface IShape { double Area(); }
来源：http://lt.yuexingan06.cn

[G10] 访问控制
来源：http://ez.newstarts.cn

Py:   约定 _protected / __private（不强制）
来源：http://rm.jctech888.com.cn

PHP:  public / protected / private
来源：http://yy.szsharing.cn

JS:   #private 字段；其余公开
来源：http://dp.9csxet.cn

TS:   public / protected / private
来源：http://hi.yuntaijiaju.cn

Java: public / protected / private / 默认包级
来源：http://km.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bj.huanxung.cn

Ruby: public / protected / private
来源：http://xh.521024.cn

C#:   public / protected / private / internal
来源：http://il.muxihuayi.cn

[G11] getter / setter
来源：http://nd.hahajie.cn

Py:   @property 与 @x.setter
来源：http://ju.bookmarksfly.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://on.szxytkj.cn

JS:   get name() { return this._name; }
来源：http://pb.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://dp.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://ln.szxytkj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mi.panjiajie.cn

Ruby: attr_accessor :name
来源：http://zr.nicolike.cn

C#:   public string Name { get; set; }
来源：http://tu.szsharing.cn

[G12] 对象转字符串
来源：http://jx.shxzukj.cn

Py:   def __str__(self): return self.name
来源：http://gb.hahajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ew.bjjhwx.cn

JS:   toString() { return this.name; }
来源：http://dv.bookmarksfly.cn

TS:   toString(): string { return this.name; }
来源：http://mx.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://jm.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jh.wgjwhj.cn

Ruby: def to_s; @name; end
来源：http://qo.521024.cn

C#:   public override string ToString() => Name;
来源：http://ir.gzmigu.cn

[G13] 判断对象类型
来源：http://ms.bjjhwx.cn

Py:   isinstance(u, User)
来源：http://ba.panjiajie.cn

PHP:  $u instanceof User
来源：http://cg.huixiangedu.cn

JS:   u instanceof User
来源：http://pq.asd995.cn

TS:   u instanceof User
来源：http://ag.shxzskj.cn

Java: u instanceof User
来源：http://ac.bookmarksfly.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://du.panjiajie.cn

Ruby: u.is_a?(User)
来源：http://hl.gzmigu.cn

C#:   u is User
来源：http://el.yuexingan06.cn

[G14] 数据类 / record
来源：http://eu.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jj.muxihuayi.cn

PHP:  // 用 readonly 属性模拟
来源：http://dd.huixiangedu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cx.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://do.asd995.cn

Java: record User(String name, int age) {}
来源：http://mn.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://fp.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://st.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://tu.wgjwhj.cn

[G15] 枚举
来源：http://ai.szxytkj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://lp.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bs.shxzukj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://kp.bookmarksfly.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nu.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://ue.huixinmuqiang.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ve.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://nn.huanxung.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://me.nszjky.cn

[G16] 对象转数组 / 字典
来源：http://sd.hnjuh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://om.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://zd.colortex.cn

JS:   Object.entries(obj)
来源：http://cx.asd995.cn

TS:   Object.entries(obj)
来源：http://ox.521024.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yr.shtwfgs.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fu.shtwfgs.cn

Ruby: obj.instance_variables
来源：http://kn.jctech888.com.cn

C#:   // 用反射或 System.Text.Json
来源：http://zq.lnxyls.cn

================================================================================
来源：http://yh.gzmigu.cn

H. 异常与错误处理
来源：http://zc.asd995.cn

================================================================================
来源：http://cp.shtwfgs.cn

[H01] try / catch 基础
来源：http://tb.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sa.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jo.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mz.bookmarksfly.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kh.huanxung.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fy.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wh.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kv.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qp.jianghongdianzi.cn

[H02] finally / ensure 收尾
来源：http://og.bjjhwx.cn

Py:   try: f()⏎finally: cleanup()
来源：http://li.asd995.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://if.shtwfgs.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kw.nicolike.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ww.huixinmuqiang.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wd.hahajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yc.hahajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://nx.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ms.521024.cn

[H03] 主动抛出异常
来源：http://og.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://ex.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lh.bjjhwx.cn

JS:   throw new Error("错误信息");
来源：http://zg.huanxung.cn

TS:   throw new Error("错误信息");
来源：http://qt.bjjhwx.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vt.jctech888.com.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vv.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ft.521024.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tj.haigaiapp.cn

[H04] 自定义异常类型
来源：http://xx.asd995.cn

Py:   class MyError(Exception): pass
来源：http://aq.newstarts.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rx.szsharing.cn

JS:   class MyError extends Error {}
来源：http://pf.asd995.cn

TS:   class MyError extends Error {}
来源：http://mu.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://ej.hahajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ao.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://uf.huanxung.cn

C#:   class MyException : Exception {}
来源：http://nv.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://md.newstarts.cn

Py:   except ValueError as e:
来源：http://lr.lnxyls.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ur.yuntaijiaju.cn

JS:   if (e instanceof TypeError) {}
来源：http://oc.haigaiapp.cn

TS:   if (e instanceof TypeError) {}
来源：http://li.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://wv.haigaiapp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fe.shxzskj.cn

Ruby: rescue ArgumentError => e
来源：http://xz.huixiangedu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zi.chemitech.net.cn

[H06] 可选值 / 空值安全访问
来源：http://ln.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://rc.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bz.wgjwhj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pf.shtwfgs.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rv.hahajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ej.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dt.szsharing.cn

Ruby: d&.dig(:a, :b)
来源：http://us.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://mv.muxihuayi.cn

[H07] 断言
来源：http://hs.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://dn.9csxet.cn

PHP:  assert($x > 0);
来源：http://eq.hahajie.cn

JS:   console.assert(x > 0);
来源：http://mi.bookmarksfly.cn

TS:   console.assert(x > 0);
来源：http://rq.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://lw.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wm.haigaiapp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rt.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://of.newstarts.cn

[H08] 获取错误信息与堆栈
来源：http://eh.wgjwhj.cn

Py:   str(e);  traceback.format_exc()
来源：http://ym.asd995.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pc.jianghongdianzi.cn

JS:   e.message;  e.stack
来源：http://td.yuntaijiaju.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sr.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hn.panjiajie.cn

Go:   err.Error()
来源：http://vm.521024.cn

Ruby: e.message;  e.backtrace
来源：http://hx.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://fx.shxzukj.cn

[H09] 带错误码的异常
来源：http://tz.colortex.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yw.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zm.panjiajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hy.nicolike.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pz.521024.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rw.9csxet.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nw.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://if.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rc.jctech888.com.cn

[H10] 资源自动释放
来源：http://il.521024.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://oj.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gj.bjjhwx.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oa.jianghongdianzi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bq.newstarts.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gr.haigaiapp.cn

Go:   defer f.Close()
来源：http://pz.9csxet.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://iv.gzmigu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xl.bjjhwx.cn

================================================================================
来源：http://uw.wgjwhj.cn

I. 正则表达式
来源：http://ec.lnxyls.cn

================================================================================
来源：http://to.lnxyls.cn

[I01] 判断是否匹配
来源：http://cv.yuntaijiaju.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://as.newstarts.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ak.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://pp.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://ak.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qq.nszjky.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hq.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://mj.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ay.huixiangedu.cn

[I02] 提取所有匹配
来源：http://pr.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://db.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vc.521024.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nr.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://ty.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dt.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yf.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://yn.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://zf.newstarts.cn

[I03] 提取捕获分组
来源：http://vi.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nl.jianghongdianzi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kv.hnjuh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dq.bjjhwx.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jq.bjjhwx.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://el.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dw.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hh.shxzukj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ph.hnjuh.cn

[I04] 正则替换
来源：http://wm.muxihuayi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gw.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xn.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ra.colortex.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lh.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://re.muxihuayi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kc.huixinmuqiang.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xj.shtwfgs.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xq.haigaiapp.cn

[I05] 按正则拆分
来源：http://vf.shxzukj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jq.huixinmuqiang.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zb.colortex.cn

JS:   s.split(/\s*,\s*/)
来源：http://ki.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://fh.shtwfgs.cn

Java: s.split("\\s*,\\s*")
来源：http://kc.lnxyls.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://kg.muxihuayi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mo.yuntaijiaju.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zf.panjiajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bz.shxzukj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hu.szsharing.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wo.jianghongdianzi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xh.huixinmuqiang.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xb.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hv.bjjhwx.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zp.jianghongdianzi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://sk.jctech888.com.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ir.szxytkj.cn

[I07] 忽略大小写与多行模式
来源：http://ef.huixiangedu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nh.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gx.hnjuh.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://in.yuntaijiaju.cn

TS:   /error/gim
来源：http://na.yuntaijiaju.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hb.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tc.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://us.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zj.yuexingan06.cn

[I08] 贪婪与非贪婪匹配
来源：http://au.asd995.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tm.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bt.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qo.nicolike.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tw.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ul.shxzskj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://so.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wh.hnjuh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qi.wgjwhj.cn

================================================================================
来源：http://ga.lnxyls.cn

J. 日期与时间
来源：http://zb.yuexingan06.cn

================================================================================
来源：http://oq.jctech888.com.cn

[J01] 获取当前时间
来源：http://xz.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://sl.lnxyls.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xs.bjjhwx.cn

JS:   new Date();  Date.now()
来源：http://ei.9csxet.cn

TS:   new Date();  Date.now()
来源：http://vy.haigaiapp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mj.shtwfgs.cn

Go:   time.Now()
来源：http://rb.huanxung.cn

Ruby: Time.now
来源：http://wi.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fn.hnjuh.cn

[J02] 格式化输出
来源：http://ft.9csxet.cn


<!-- 参考信息 -->