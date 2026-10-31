代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://ke.asd995.cn

Java: @Override String greet() { return "admin"; }
来源：http://px.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mj.muxihuayi.cn

Ruby: def greet; "admin"; end
来源：http://jp.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://ik.lnxyls.cn

[G07] 调用父类方法
来源：http://se.muxihuayi.cn

Py:   super().greet()
来源：http://bw.shxzukj.cn

PHP:  parent::greet();
来源：http://wn.hnjuh.cn

JS:   super.greet();
来源：http://tq.newstarts.cn

TS:   super.greet();
来源：http://ck.nszjky.cn

Java: super.greet();
来源：http://ss.jctech888.com.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yf.colortex.cn

Ruby: super
来源：http://vf.muxihuayi.cn

C#:   base.Greet();
来源：http://gv.asd995.cn

[G08] 静态方法与属性
来源：http://gv.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://bd.wgjwhj.cn

PHP:  public static function f() {}
来源：http://bm.gzmigu.cn

JS:   static f() {}
来源：http://yn.jianghongdianzi.cn

TS:   static f(): void {}
来源：http://ju.asd995.cn

Java: static void f() {}
来源：http://fc.asd995.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qc.shtwfgs.cn

Ruby: def self.f; end
来源：http://el.asd995.cn

C#:   public static void F() {}
来源：http://dl.bjjhwx.cn

[G09] 接口 / 抽象类
来源：http://fy.asd995.cn

Py:   from abc import ABC, abstractmethod
来源：http://zy.huixiangedu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hk.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pr.muxihuayi.cn

TS:   interface Shape { area(): number; }
来源：http://lu.huanxung.cn

Java: interface Shape { double area(); }
来源：http://cn.panjiajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://ii.huixiangedu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://aw.521024.cn

C#:   interface IShape { double Area(); }
来源：http://ke.9csxet.cn

[G10] 访问控制
来源：http://zf.gzmigu.cn

Py:   约定 _protected / __private（不强制）
来源：http://zt.muxihuayi.cn

PHP:  public / protected / private
来源：http://rp.lnxyls.cn

JS:   #private 字段；其余公开
来源：http://zb.shtwfgs.cn

TS:   public / protected / private
来源：http://fs.huanxung.cn

Java: public / protected / private / 默认包级
来源：http://vt.bookmarksfly.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bw.asd995.cn

Ruby: public / protected / private
来源：http://ur.hnjuh.cn

C#:   public / protected / private / internal
来源：http://ks.asd995.cn

[G11] getter / setter
来源：http://nx.hahajie.cn

Py:   @property 与 @x.setter
来源：http://ku.asd995.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gq.huixinmuqiang.cn

JS:   get name() { return this._name; }
来源：http://hc.muxihuayi.cn

TS:   get name(): string { return this._name; }
来源：http://ok.nszjky.cn

Java: public String getName() { return name; }
来源：http://oj.jctech888.com.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gk.hahajie.cn

Ruby: attr_accessor :name
来源：http://ki.hnjuh.cn

C#:   public string Name { get; set; }
来源：http://dx.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://ni.521024.cn

Py:   def __str__(self): return self.name
来源：http://id.chemitech.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ja.chemitech.net.cn

JS:   toString() { return this.name; }
来源：http://ng.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://iv.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://sj.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ng.9csxet.cn

Ruby: def to_s; @name; end
来源：http://xr.gzmigu.cn

C#:   public override string ToString() => Name;
来源：http://nu.huixinmuqiang.cn

[G13] 判断对象类型
来源：http://mw.szxytkj.cn

Py:   isinstance(u, User)
来源：http://xn.huanxung.cn

PHP:  $u instanceof User
来源：http://bx.muxihuayi.cn

JS:   u instanceof User
来源：http://zu.yuntaijiaju.cn

TS:   u instanceof User
来源：http://fl.gzmigu.cn

Java: u instanceof User
来源：http://iv.bjjhwx.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dr.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://be.lnxyls.cn

C#:   u is User
来源：http://rl.nicolike.cn

[G14] 数据类 / record
来源：http://ly.shxzskj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fy.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://xv.shtwfgs.cn

JS:   // 无内置：普通类或对象字面量
来源：http://iq.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://tk.huixinmuqiang.cn

Java: record User(String name, int age) {}
来源：http://jl.bookmarksfly.cn

Go:   type User struct { Name string; Age int }
来源：http://qy.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sk.panjiajie.cn

C#:   record User(string Name, int Age);
来源：http://gy.haigaiapp.cn

[G15] 枚举
来源：http://qn.chemitech.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wn.wgjwhj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://in.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://or.yuntaijiaju.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ys.9csxet.cn

Java: enum Color { RED, GREEN }
来源：http://yt.521024.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://op.lnxyls.cn

Ruby: Color = %i[red green].freeze
来源：http://fr.gzmigu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://eq.muxihuayi.cn

[G16] 对象转数组 / 字典
来源：http://pk.bjjhwx.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qj.bjjhwx.cn

PHP:  get_object_vars($obj);
来源：http://jl.haigaiapp.cn

JS:   Object.entries(obj)
来源：http://pr.gzmigu.cn

TS:   Object.entries(obj)
来源：http://xi.muxihuayi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bu.szxytkj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hj.huanxung.cn

Ruby: obj.instance_variables
来源：http://rf.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://ve.bjjhwx.cn

================================================================================
来源：http://fu.yuexingan06.cn

H. 异常与错误处理
来源：http://tx.bookmarksfly.cn

================================================================================
来源：http://wm.huixinmuqiang.cn

[H01] try / catch 基础
来源：http://tb.shxzukj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qd.gzmigu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nh.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fu.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xh.shxzskj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cm.shxzukj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dh.jctech888.com.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hn.shxzskj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mj.jctech888.com.cn

[H02] finally / ensure 收尾
来源：http://sk.haigaiapp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rr.bjjhwx.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ew.nicolike.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lr.nicolike.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vq.huixiangedu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tf.yuntaijiaju.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cc.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ie.asd995.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://kw.9csxet.cn

[H03] 主动抛出异常
来源：http://en.hnjuh.cn

Py:   raise ValueError("错误信息")
来源：http://vj.huixiangedu.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://un.szsharing.cn

JS:   throw new Error("错误信息");
来源：http://ky.yuntaijiaju.cn

TS:   throw new Error("错误信息");
来源：http://tl.jctech888.com.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ra.panjiajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ff.jianghongdianzi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dp.yuntaijiaju.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ju.huixiangedu.cn

[H04] 自定义异常类型
来源：http://zr.shtwfgs.cn

Py:   class MyError(Exception): pass
来源：http://de.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fc.jianghongdianzi.cn

JS:   class MyError extends Error {}
来源：http://af.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://vd.lnxyls.cn

Java: class MyException extends RuntimeException {}
来源：http://ft.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ey.9csxet.cn

Ruby: class MyError < StandardError; end
来源：http://mi.yuexingan06.cn

C#:   class MyException : Exception {}
来源：http://kw.nicolike.cn

[H05] 捕获特定类型
来源：http://fm.shxzskj.cn

Py:   except ValueError as e:
来源：http://er.wgjwhj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cn.shtwfgs.cn

JS:   if (e instanceof TypeError) {}
来源：http://gw.yuexingan06.cn

TS:   if (e instanceof TypeError) {}
来源：http://bk.jianghongdianzi.cn

Java: catch (IOException | SQLException e) {}
来源：http://ja.wgjwhj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zg.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://tm.yuexingan06.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sw.521024.cn

[H06] 可选值 / 空值安全访问
来源：http://wg.huanxung.cn

Py:   value = d.get("k") or default
来源：http://li.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ll.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vr.panjiajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://eg.nicolike.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gy.newstarts.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://eu.jctech888.com.cn

Ruby: d&.dig(:a, :b)
来源：http://ji.521024.cn

C#:   obj?.A?.B ?? default
来源：http://lg.newstarts.cn

[H07] 断言
来源：http://ub.gzmigu.cn

Py:   assert x > 0, "必须为正"
来源：http://xf.bookmarksfly.cn

PHP:  assert($x > 0);
来源：http://fp.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://wf.chemitech.net.cn

TS:   console.assert(x > 0);
来源：http://cl.haigaiapp.cn

Java: assert x > 0 : "必须为正";
来源：http://xf.gzmigu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pq.bookmarksfly.cn

Ruby: raise "必须为正" unless x > 0
来源：http://eq.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://mv.hahajie.cn

[H08] 获取错误信息与堆栈
来源：http://zo.newstarts.cn

Py:   str(e);  traceback.format_exc()
来源：http://nk.muxihuayi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://el.jianghongdianzi.cn

JS:   e.message;  e.stack
来源：http://er.muxihuayi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://er.szsharing.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://dq.9csxet.cn

Go:   err.Error()
来源：http://pp.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://vc.bookmarksfly.cn

C#:   e.Message;  e.StackTrace
来源：http://cz.nicolike.cn

[H09] 带错误码的异常
来源：http://vm.chemitech.net.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mq.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qx.wgjwhj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ay.chemitech.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uk.colortex.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tx.newstarts.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tg.chemitech.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ar.yuexingan06.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bf.colortex.cn

[H10] 资源自动释放
来源：http://yd.szxytkj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gu.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ge.huixinmuqiang.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hnjuh.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://os.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cs.lnxyls.cn

Go:   defer f.Close()
来源：http://qj.yuexingan06.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hj.jctech888.com.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cx.huixinmuqiang.cn

================================================================================
来源：http://br.asd995.cn

I. 正则表达式
来源：http://dy.haigaiapp.cn

================================================================================
来源：http://mr.szxytkj.cn

[I01] 判断是否匹配
来源：http://ng.shxzskj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://li.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ca.9csxet.cn

JS:   /\d+/.test(s)
来源：http://gg.muxihuayi.cn

TS:   /\d+/.test(s)
来源：http://it.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ry.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gh.szxytkj.cn

Ruby: s.match?(/\d+/)
来源：http://zn.hahajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://va.yuexingan06.cn

[I02] 提取所有匹配
来源：http://um.huixinmuqiang.cn

Py:   re.findall(r"\d+", s)
来源：http://yw.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jr.muxihuayi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cf.jianghongdianzi.cn

TS:   s.match(/\d+/g)
来源：http://bd.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bt.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rz.shtwfgs.cn

Ruby: s.scan(/\d+/)
来源：http://ig.521024.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oo.newstarts.cn

[I03] 提取捕获分组
来源：http://zh.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jc.jianghongdianzi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://he.shxzskj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://va.colortex.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oq.newstarts.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qc.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dv.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fw.newstarts.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://de.bjjhwx.cn

[I04] 正则替换
来源：http://dy.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ej.shtwfgs.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ic.shxzukj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jh.yuntaijiaju.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qh.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ym.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ay.hnjuh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://eo.yuexingan06.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zp.haigaiapp.cn

[I05] 按正则拆分
来源：http://yb.muxihuayi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://id.szxytkj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ur.hnjuh.cn

JS:   s.split(/\s*,\s*/)
来源：http://dl.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://kd.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://ch.lnxyls.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eg.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cb.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://os.yuexingan06.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://la.bjjhwx.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bc.jctech888.com.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zo.yuexingan06.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hv.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wq.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lk.jctech888.com.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qd.wgjwhj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kr.colortex.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qs.jctech888.com.cn

[I07] 忽略大小写与多行模式
来源：http://qp.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kq.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wd.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uf.szsharing.cn

TS:   /error/gim
来源：http://tz.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kv.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://on.huanxung.cn

Ruby: s.scan(/error/i)
来源：http://ol.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ti.szsharing.cn

[I08] 贪婪与非贪婪匹配
来源：http://ra.nszjky.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uz.huixinmuqiang.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ye.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wd.chemitech.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cc.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ee.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zl.haigaiapp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qk.shxzukj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://qx.yuexingan06.cn

================================================================================
来源：http://sn.bookmarksfly.cn

J. 日期与时间
来源：http://mz.521024.cn

================================================================================
来源：http://hr.wgjwhj.cn

[J01] 获取当前时间
来源：http://ob.521024.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fz.jctech888.com.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yf.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://oo.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://gg.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ij.yuexingan06.cn

Go:   time.Now()
来源：http://bg.chemitech.net.cn

Ruby: Time.now
来源：http://re.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zv.9csxet.cn

[J02] 格式化输出
来源：http://xy.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eu.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lq.szsharing.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hj.hnjuh.cn

TS:   d.toISOString()
来源：http://nm.colortex.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xe.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ji.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://if.hnjuh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://qi.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://fr.lnxyls.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xb.bookmarksfly.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oj.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://vj.szxytkj.cn

TS:   new Date("2024-01-02")
来源：http://rh.shtwfgs.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lo.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pe.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://cn.jctech888.com.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://cf.colortex.cn

[J04] 时间戳与日期互转
来源：http://wi.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vd.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kh.asd995.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ge.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://eq.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://re.szxytkj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fu.521024.cn


<!-- 参考信息 -->