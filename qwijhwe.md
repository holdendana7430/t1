代发 wailian999

[G06] 重写方法
来源：http://wc.shxzukj.cn

Py:   def greet(self): return "admin"
来源：http://ts.huanxung.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qs.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://wg.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://kr.lnxyls.cn

Java: @Override String greet() { return "admin"; }
来源：http://ng.nszjky.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ij.9csxet.cn

Ruby: def greet; "admin"; end
来源：http://sd.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://uh.asd995.cn

[G07] 调用父类方法
来源：http://ai.asd995.cn

Py:   super().greet()
来源：http://xl.haigaiapp.cn

PHP:  parent::greet();
来源：http://dh.bjjhwx.cn

JS:   super.greet();
来源：http://cj.shxzukj.cn

TS:   super.greet();
来源：http://di.wgjwhj.cn

Java: super.greet();
来源：http://ce.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://og.hahajie.cn

Ruby: super
来源：http://fj.521024.cn

C#:   base.Greet();
来源：http://tm.lnxyls.cn

[G08] 静态方法与属性
来源：http://ow.wgjwhj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fg.bjjhwx.cn

PHP:  public static function f() {}
来源：http://es.szxytkj.cn

JS:   static f() {}
来源：http://eb.9csxet.cn

TS:   static f(): void {}
来源：http://fd.lnxyls.cn

Java: static void f() {}
来源：http://dw.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zz.jctech888.com.cn

Ruby: def self.f; end
来源：http://cg.jianghongdianzi.cn

C#:   public static void F() {}
来源：http://cw.szsharing.cn

[G09] 接口 / 抽象类
来源：http://rz.huanxung.cn

Py:   from abc import ABC, abstractmethod
来源：http://rb.asd995.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zo.asd995.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://kq.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://go.521024.cn

Java: interface Shape { double area(); }
来源：http://op.huanxung.cn

Go:   type Shape interface { Area() float64 }
来源：http://ho.lnxyls.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://br.yuexingan06.cn

C#:   interface IShape { double Area(); }
来源：http://xj.521024.cn

[G10] 访问控制
来源：http://ff.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://od.szsharing.cn

PHP:  public / protected / private
来源：http://at.nicolike.cn

JS:   #private 字段；其余公开
来源：http://jp.asd995.cn

TS:   public / protected / private
来源：http://mf.hahajie.cn

Java: public / protected / private / 默认包级
来源：http://pw.haigaiapp.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sl.nicolike.cn

Ruby: public / protected / private
来源：http://jx.9csxet.cn

C#:   public / protected / private / internal
来源：http://cu.yuexingan06.cn

[G11] getter / setter
来源：http://kw.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://wz.newstarts.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://kx.colortex.cn

JS:   get name() { return this._name; }
来源：http://jm.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://ew.9csxet.cn

Java: public String getName() { return name; }
来源：http://oq.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://pv.haigaiapp.cn

Ruby: attr_accessor :name
来源：http://af.colortex.cn

C#:   public string Name { get; set; }
来源：http://vi.huanxung.cn

[G12] 对象转字符串
来源：http://ro.haigaiapp.cn

Py:   def __str__(self): return self.name
来源：http://qj.colortex.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jb.bjjhwx.cn

JS:   toString() { return this.name; }
来源：http://pz.huixiangedu.cn

TS:   toString(): string { return this.name; }
来源：http://pr.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://gb.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mb.bookmarksfly.cn

Ruby: def to_s; @name; end
来源：http://jr.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://tt.chemitech.net.cn

[G13] 判断对象类型
来源：http://kb.gzmigu.cn

Py:   isinstance(u, User)
来源：http://ga.bjjhwx.cn

PHP:  $u instanceof User
来源：http://rz.shtwfgs.cn

JS:   u instanceof User
来源：http://to.shxzskj.cn

TS:   u instanceof User
来源：http://py.wgjwhj.cn

Java: u instanceof User
来源：http://xd.asd995.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hn.asd995.cn

Ruby: u.is_a?(User)
来源：http://do.newstarts.cn

C#:   u is User
来源：http://qg.bookmarksfly.cn

[G14] 数据类 / record
来源：http://wx.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ai.huixinmuqiang.cn

PHP:  // 用 readonly 属性模拟
来源：http://ko.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vu.huixiangedu.cn

TS:   type User = { name: string; age: number };
来源：http://ey.szxytkj.cn

Java: record User(String name, int age) {}
来源：http://kq.9csxet.cn

Go:   type User struct { Name string; Age int }
来源：http://ug.gzmigu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://og.hnjuh.cn

C#:   record User(string Name, int Age);
来源：http://sf.szxytkj.cn

[G15] 枚举
来源：http://tt.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://be.asd995.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://je.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://do.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tn.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://jh.bjjhwx.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://jw.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://nm.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sw.jctech888.com.cn

[G16] 对象转数组 / 字典
来源：http://bl.chemitech.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xw.wgjwhj.cn

PHP:  get_object_vars($obj);
来源：http://gp.asd995.cn

JS:   Object.entries(obj)
来源：http://tv.jianghongdianzi.cn

TS:   Object.entries(obj)
来源：http://tc.wgjwhj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://je.jianghongdianzi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jy.asd995.cn

Ruby: obj.instance_variables
来源：http://xo.asd995.cn

C#:   // 用反射或 System.Text.Json
来源：http://yq.nicolike.cn

================================================================================
来源：http://zi.muxihuayi.cn

H. 异常与错误处理
来源：http://rj.colortex.cn

================================================================================
来源：http://xt.huixiangedu.cn

[H01] try / catch 基础
来源：http://lo.panjiajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://is.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nx.nszjky.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yy.jianghongdianzi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uo.shtwfgs.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nk.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gd.yuexingan06.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pj.huixiangedu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://si.szsharing.cn

[H02] finally / ensure 收尾
来源：http://kc.szxytkj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rw.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sm.hnjuh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tq.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ew.colortex.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bx.colortex.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://kp.hahajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://eo.panjiajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ew.jctech888.com.cn

[H03] 主动抛出异常
来源：http://qn.szxytkj.cn

Py:   raise ValueError("错误信息")
来源：http://nn.yuexingan06.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ph.szxytkj.cn

JS:   throw new Error("错误信息");
来源：http://pt.bookmarksfly.cn

TS:   throw new Error("错误信息");
来源：http://qa.huanxung.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://im.szxytkj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xm.jctech888.com.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wq.521024.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ar.bookmarksfly.cn

[H04] 自定义异常类型
来源：http://ib.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://vx.huixiangedu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bc.asd995.cn

JS:   class MyError extends Error {}
来源：http://pi.muxihuayi.cn

TS:   class MyError extends Error {}
来源：http://rv.lnxyls.cn

Java: class MyException extends RuntimeException {}
来源：http://bv.gzmigu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jo.huanxung.cn

Ruby: class MyError < StandardError; end
来源：http://py.wgjwhj.cn

C#:   class MyException : Exception {}
来源：http://il.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://cd.hahajie.cn

Py:   except ValueError as e:
来源：http://lx.huixiangedu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rm.hnjuh.cn

JS:   if (e instanceof TypeError) {}
来源：http://os.szxytkj.cn

TS:   if (e instanceof TypeError) {}
来源：http://uc.shtwfgs.cn

Java: catch (IOException | SQLException e) {}
来源：http://ln.yuntaijiaju.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ut.gzmigu.cn

Ruby: rescue ArgumentError => e
来源：http://fq.bjjhwx.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wp.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://zx.asd995.cn

Py:   value = d.get("k") or default
来源：http://xv.nicolike.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kf.jctech888.com.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cp.521024.cn

TS:   obj?.a?.b;  d ?? default
来源：http://np.shtwfgs.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mw.nszjky.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ro.colortex.cn

Ruby: d&.dig(:a, :b)
来源：http://yv.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://nu.shtwfgs.cn

[H07] 断言
来源：http://li.asd995.cn

Py:   assert x > 0, "必须为正"
来源：http://pk.asd995.cn

PHP:  assert($x > 0);
来源：http://xk.521024.cn

JS:   console.assert(x > 0);
来源：http://yk.lnxyls.cn

TS:   console.assert(x > 0);
来源：http://hg.shtwfgs.cn

Java: assert x > 0 : "必须为正";
来源：http://ch.jianghongdianzi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jn.colortex.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dg.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://lm.shxzskj.cn

[H08] 获取错误信息与堆栈
来源：http://db.lnxyls.cn

Py:   str(e);  traceback.format_exc()
来源：http://dd.shxzukj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ho.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://bs.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vx.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://fu.jctech888.com.cn

Go:   err.Error()
来源：http://wa.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://iz.jianghongdianzi.cn

C#:   e.Message;  e.StackTrace
来源：http://ue.shtwfgs.cn

[H09] 带错误码的异常
来源：http://jj.hahajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tf.wgjwhj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zi.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ey.huixinmuqiang.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ly.gzmigu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dc.wgjwhj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://yw.huixiangedu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mh.huanxung.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ir.yuntaijiaju.cn

[H10] 资源自动释放
来源：http://oc.szsharing.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ex.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mz.gzmigu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wl.521024.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vn.jianghongdianzi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nh.bookmarksfly.cn

Go:   defer f.Close()
来源：http://zn.panjiajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rw.bjjhwx.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zk.huanxung.cn

================================================================================
来源：http://an.wgjwhj.cn

I. 正则表达式
来源：http://dl.bjjhwx.cn

================================================================================
来源：http://zz.panjiajie.cn

[I01] 判断是否匹配
来源：http://jo.jianghongdianzi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cd.yuntaijiaju.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jg.521024.cn

JS:   /\d+/.test(s)
来源：http://xq.szxytkj.cn

TS:   /\d+/.test(s)
来源：http://ua.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://py.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nr.jctech888.com.cn

Ruby: s.match?(/\d+/)
来源：http://bx.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zo.bookmarksfly.cn

[I02] 提取所有匹配
来源：http://wb.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://yh.9csxet.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hu.wgjwhj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ro.yuexingan06.cn

TS:   s.match(/\d+/g)
来源：http://ck.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://le.nicolike.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ur.yuntaijiaju.cn

Ruby: s.scan(/\d+/)
来源：http://qu.shtwfgs.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qj.shxzukj.cn

[I03] 提取捕获分组
来源：http://xn.shxzskj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fk.wgjwhj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://az.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qk.huanxung.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qa.bjjhwx.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://se.hahajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ll.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://az.yuexingan06.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wg.521024.cn

[I04] 正则替换
来源：http://jo.huanxung.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ib.szsharing.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pe.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ud.colortex.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zt.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lp.yuntaijiaju.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ow.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wy.shtwfgs.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tu.shtwfgs.cn

[I05] 按正则拆分
来源：http://yh.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://iv.yuexingan06.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xm.jctech888.com.cn

JS:   s.split(/\s*,\s*/)
来源：http://sc.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://ud.chemitech.net.cn

Java: s.split("\\s*,\\s*")
来源：http://fn.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ti.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tl.szsharing.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://iu.jctech888.com.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://oa.muxihuayi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://oc.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hn.nszjky.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ju.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://at.colortex.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://el.hahajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rf.bookmarksfly.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ka.colortex.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mf.jctech888.com.cn

[I07] 忽略大小写与多行模式
来源：http://ek.szxytkj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mj.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nt.nicolike.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://us.gzmigu.cn

TS:   /error/gim
来源：http://bc.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cd.shxzukj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vm.hahajie.cn

Ruby: s.scan(/error/i)
来源：http://qg.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://th.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://yf.hnjuh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ia.jianghongdianzi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sx.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ub.bookmarksfly.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://mm.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jc.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fc.lnxyls.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qk.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nx.haigaiapp.cn

================================================================================
来源：http://pi.huanxung.cn

J. 日期与时间
来源：http://xz.huixinmuqiang.cn

================================================================================
来源：http://vo.shxzukj.cn

[J01] 获取当前时间
来源：http://jj.nicolike.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ru.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qc.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://cx.jctech888.com.cn

TS:   new Date();  Date.now()
来源：http://pu.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mf.bjjhwx.cn

Go:   time.Now()
来源：http://kl.hnjuh.cn

Ruby: Time.now
来源：http://py.muxihuayi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://aj.haigaiapp.cn

[J02] 格式化输出
来源：http://bn.521024.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ih.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://cl.521024.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gq.wgjwhj.cn

TS:   d.toISOString()
来源：http://sn.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ql.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vn.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sz.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tz.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://en.panjiajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wt.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://of.shtwfgs.cn

JS:   new Date("2024-01-02")
来源：http://re.asd995.cn

TS:   new Date("2024-01-02")
来源：http://jz.muxihuayi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://nc.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dg.jctech888.com.cn

Ruby: Date.parse("2024-01-02")
来源：http://ct.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uy.huanxung.cn

[J04] 时间戳与日期互转
来源：http://wd.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zu.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qr.panjiajie.cn


<!-- 参考信息 -->