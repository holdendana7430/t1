代发 wailian999

[G06] 重写方法
来源：http://yj.asd995.cn

Py:   def greet(self): return "admin"
来源：http://ua.jctech888.com.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ix.asd995.cn

JS:   greet() { return "admin"; }
来源：http://nu.hahajie.cn

TS:   greet(): string { return "admin"; }
来源：http://ng.521024.cn

Java: @Override String greet() { return "admin"; }
来源：http://ly.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yw.muxihuayi.cn

Ruby: def greet; "admin"; end
来源：http://mc.szsharing.cn

C#:   public override string Greet() => "admin";
来源：http://yq.shxzskj.cn

[G07] 调用父类方法
来源：http://pa.wgjwhj.cn

Py:   super().greet()
来源：http://op.9csxet.cn

PHP:  parent::greet();
来源：http://dv.jianghongdianzi.cn

JS:   super.greet();
来源：http://vj.yuexingan06.cn

TS:   super.greet();
来源：http://ve.nicolike.cn

Java: super.greet();
来源：http://zr.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ka.nszjky.cn

Ruby: super
来源：http://hr.panjiajie.cn

C#:   base.Greet();
来源：http://rq.huixinmuqiang.cn

[G08] 静态方法与属性
来源：http://pd.chemitech.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ea.bjjhwx.cn

PHP:  public static function f() {}
来源：http://qg.huanxung.cn

JS:   static f() {}
来源：http://xk.shxzukj.cn

TS:   static f(): void {}
来源：http://te.jianghongdianzi.cn

Java: static void f() {}
来源：http://jt.haigaiapp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ef.9csxet.cn

Ruby: def self.f; end
来源：http://at.521024.cn

C#:   public static void F() {}
来源：http://sl.wgjwhj.cn

[G09] 接口 / 抽象类
来源：http://ma.chemitech.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://cf.haigaiapp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ke.wgjwhj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://it.huanxung.cn

TS:   interface Shape { area(): number; }
来源：http://ma.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://tu.521024.cn

Go:   type Shape interface { Area() float64 }
来源：http://sn.huixiangedu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bl.shtwfgs.cn

C#:   interface IShape { double Area(); }
来源：http://cs.hahajie.cn

[G10] 访问控制
来源：http://mv.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://ws.shxzukj.cn

PHP:  public / protected / private
来源：http://ph.yuexingan06.cn

JS:   #private 字段；其余公开
来源：http://ez.hahajie.cn

TS:   public / protected / private
来源：http://xo.newstarts.cn

Java: public / protected / private / 默认包级
来源：http://eq.szsharing.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nm.huanxung.cn

Ruby: public / protected / private
来源：http://wb.521024.cn

C#:   public / protected / private / internal
来源：http://qp.gzmigu.cn

[G11] getter / setter
来源：http://aq.hahajie.cn

Py:   @property 与 @x.setter
来源：http://my.521024.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yk.shxzskj.cn

JS:   get name() { return this._name; }
来源：http://bs.yuntaijiaju.cn

TS:   get name(): string { return this._name; }
来源：http://cx.muxihuayi.cn

Java: public String getName() { return name; }
来源：http://ay.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ix.jctech888.com.cn

Ruby: attr_accessor :name
来源：http://tk.nicolike.cn

C#:   public string Name { get; set; }
来源：http://mt.panjiajie.cn

[G12] 对象转字符串
来源：http://lg.gzmigu.cn

Py:   def __str__(self): return self.name
来源：http://cd.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pm.521024.cn

JS:   toString() { return this.name; }
来源：http://ef.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://um.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://gt.newstarts.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ae.521024.cn

Ruby: def to_s; @name; end
来源：http://vy.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://jb.shtwfgs.cn

[G13] 判断对象类型
来源：http://dr.asd995.cn

Py:   isinstance(u, User)
来源：http://ug.521024.cn

PHP:  $u instanceof User
来源：http://uz.bookmarksfly.cn

JS:   u instanceof User
来源：http://co.newstarts.cn

TS:   u instanceof User
来源：http://or.huixiangedu.cn

Java: u instanceof User
来源：http://aq.chemitech.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kf.yuntaijiaju.cn

Ruby: u.is_a?(User)
来源：http://oa.nszjky.cn

C#:   u is User
来源：http://ob.gzmigu.cn

[G14] 数据类 / record
来源：http://dh.huanxung.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vk.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://rz.chemitech.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pv.shtwfgs.cn

TS:   type User = { name: string; age: number };
来源：http://mb.szxytkj.cn

Java: record User(String name, int age) {}
来源：http://ca.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://we.jianghongdianzi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ym.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://uo.hahajie.cn

[G15] 枚举
来源：http://po.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vm.nicolike.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ig.yuexingan06.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jw.hahajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ja.panjiajie.cn

Java: enum Color { RED, GREEN }
来源：http://jl.haigaiapp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fa.bjjhwx.cn

Ruby: Color = %i[red green].freeze
来源：http://my.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gi.hahajie.cn

[G16] 对象转数组 / 字典
来源：http://xm.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ql.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://iq.colortex.cn

JS:   Object.entries(obj)
来源：http://jz.jctech888.com.cn

TS:   Object.entries(obj)
来源：http://kl.shxzskj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zq.bookmarksfly.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hh.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://db.nszjky.cn

C#:   // 用反射或 System.Text.Json
来源：http://jb.panjiajie.cn

================================================================================
来源：http://gu.colortex.cn

H. 异常与错误处理
来源：http://bi.bookmarksfly.cn

================================================================================
来源：http://ck.bookmarksfly.cn

[H01] try / catch 基础
来源：http://iw.panjiajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hf.nszjky.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ej.nszjky.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jc.haigaiapp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://eq.huixinmuqiang.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pj.nicolike.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hh.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pq.muxihuayi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wc.nicolike.cn

[H02] finally / ensure 收尾
来源：http://qu.huixiangedu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vm.szxytkj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nc.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ts.bjjhwx.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bw.shtwfgs.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tj.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lq.wgjwhj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fy.asd995.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jo.bjjhwx.cn

[H03] 主动抛出异常
来源：http://yj.hnjuh.cn

Py:   raise ValueError("错误信息")
来源：http://jc.bookmarksfly.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xy.colortex.cn

JS:   throw new Error("错误信息");
来源：http://my.bookmarksfly.cn

TS:   throw new Error("错误信息");
来源：http://yv.bjjhwx.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xz.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qm.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vi.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kk.lnxyls.cn

[H04] 自定义异常类型
来源：http://wl.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://ip.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yr.huixiangedu.cn

JS:   class MyError extends Error {}
来源：http://br.wgjwhj.cn

TS:   class MyError extends Error {}
来源：http://rf.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://pg.shxzukj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gt.yuntaijiaju.cn

Ruby: class MyError < StandardError; end
来源：http://hx.colortex.cn

C#:   class MyException : Exception {}
来源：http://jy.yuntaijiaju.cn

[H05] 捕获特定类型
来源：http://ih.yuexingan06.cn

Py:   except ValueError as e:
来源：http://kj.huixinmuqiang.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cs.huixinmuqiang.cn

JS:   if (e instanceof TypeError) {}
来源：http://uj.yuexingan06.cn

TS:   if (e instanceof TypeError) {}
来源：http://qj.hahajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://hz.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fj.521024.cn

Ruby: rescue ArgumentError => e
来源：http://od.jctech888.com.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://aw.shtwfgs.cn

[H06] 可选值 / 空值安全访问
来源：http://oq.yuntaijiaju.cn

Py:   value = d.get("k") or default
来源：http://lk.colortex.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rr.haigaiapp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kn.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cz.yuntaijiaju.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sp.shxzskj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wz.nicolike.cn

Ruby: d&.dig(:a, :b)
来源：http://jr.huixiangedu.cn

C#:   obj?.A?.B ?? default
来源：http://el.jianghongdianzi.cn

[H07] 断言
来源：http://iw.asd995.cn

Py:   assert x > 0, "必须为正"
来源：http://ve.newstarts.cn

PHP:  assert($x > 0);
来源：http://lq.huanxung.cn

JS:   console.assert(x > 0);
来源：http://uw.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://is.hahajie.cn

Java: assert x > 0 : "必须为正";
来源：http://tt.bookmarksfly.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jb.wgjwhj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://am.shxzskj.cn

C#:   Debug.Assert(x > 0);
来源：http://cb.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://sq.newstarts.cn

Py:   str(e);  traceback.format_exc()
来源：http://az.asd995.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fy.lnxyls.cn

JS:   e.message;  e.stack
来源：http://pj.yuntaijiaju.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qs.jctech888.com.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mp.newstarts.cn

Go:   err.Error()
来源：http://wa.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://sv.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://fr.shxzukj.cn

[H09] 带错误码的异常
来源：http://ms.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vu.newstarts.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nx.shxzukj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jx.wgjwhj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://iy.shxzskj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qx.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://oq.lnxyls.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gv.gzmigu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://sm.521024.cn

[H10] 资源自动释放
来源：http://xf.szsharing.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xy.nicolike.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bb.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gm.hnjuh.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tj.szxytkj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://uk.bjjhwx.cn

Go:   defer f.Close()
来源：http://wf.nicolike.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ej.9csxet.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bp.nicolike.cn

================================================================================
来源：http://mt.jianghongdianzi.cn

I. 正则表达式
来源：http://ra.9csxet.cn

================================================================================
来源：http://jg.hnjuh.cn

[I01] 判断是否匹配
来源：http://nh.521024.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ii.lnxyls.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wn.bookmarksfly.cn

JS:   /\d+/.test(s)
来源：http://nu.huanxung.cn

TS:   /\d+/.test(s)
来源：http://fk.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uq.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hd.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://rt.yuntaijiaju.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hl.huixiangedu.cn

[I02] 提取所有匹配
来源：http://jc.wgjwhj.cn

Py:   re.findall(r"\d+", s)
来源：http://da.nicolike.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://aj.lnxyls.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://aa.huixinmuqiang.cn

TS:   s.match(/\d+/g)
来源：http://xb.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ca.hahajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wg.hnjuh.cn

Ruby: s.scan(/\d+/)
来源：http://ja.shxzskj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fk.wgjwhj.cn

[I03] 提取捕获分组
来源：http://nv.wgjwhj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qy.haigaiapp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rx.panjiajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rv.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fi.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yv.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ua.newstarts.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mq.nicolike.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yq.bjjhwx.cn

[I04] 正则替换
来源：http://hb.szsharing.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nl.asd995.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xi.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gr.szsharing.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qi.shxzskj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xz.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://by.haigaiapp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://za.haigaiapp.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ko.bookmarksfly.cn

[I05] 按正则拆分
来源：http://kc.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yn.huixinmuqiang.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nr.newstarts.cn

JS:   s.split(/\s*,\s*/)
来源：http://tq.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://yj.huixinmuqiang.cn

Java: s.split("\\s*,\\s*")
来源：http://lo.szsharing.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lf.yuexingan06.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pc.shtwfgs.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ln.huixiangedu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ru.lnxyls.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kp.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ew.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zb.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qt.hnjuh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rh.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ta.hnjuh.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ou.colortex.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wf.huanxung.cn

[I07] 忽略大小写与多行模式
来源：http://lf.huixiangedu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jc.asd995.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pr.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://aq.521024.cn

TS:   /error/gim
来源：http://rx.hahajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vk.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lk.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://wk.newstarts.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mu.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://pr.shtwfgs.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kg.huixiangedu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qd.colortex.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tn.hnjuh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hy.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cm.shxzskj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wa.wgjwhj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kw.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://th.9csxet.cn

================================================================================
来源：http://ax.nicolike.cn

J. 日期与时间
来源：http://fu.9csxet.cn

================================================================================
来源：http://ca.521024.cn

[J01] 获取当前时间
来源：http://bn.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nv.haigaiapp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ua.lnxyls.cn

JS:   new Date();  Date.now()
来源：http://gl.yuntaijiaju.cn

TS:   new Date();  Date.now()
来源：http://uy.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kj.9csxet.cn

Go:   time.Now()
来源：http://ko.nicolike.cn

Ruby: Time.now
来源：http://tg.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ah.newstarts.cn

[J02] 格式化输出
来源：http://at.bjjhwx.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://en.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://en.gzmigu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ps.lnxyls.cn

TS:   d.toISOString()
来源：http://uv.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cb.haigaiapp.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zt.huanxung.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xl.yuexingan06.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fp.asd995.cn

[J03] 字符串解析为日期
来源：http://wc.nszjky.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ga.chemitech.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zx.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://pq.bjjhwx.cn

TS:   new Date("2024-01-02")
来源：http://sm.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://iu.szxytkj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://nb.shxzskj.cn

Ruby: Date.parse("2024-01-02")
来源：http://jk.9csxet.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nd.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://lb.shtwfgs.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tk.yuntaijiaju.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bn.jctech888.com.cn


<!-- 参考信息 -->