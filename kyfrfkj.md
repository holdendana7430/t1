代发 wailian999

[G06] 重写方法
来源：http://sw.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://cm.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://wr.9csxet.cn

JS:   greet() { return "admin"; }
来源：http://cv.huixiangedu.cn

TS:   greet(): string { return "admin"; }
来源：http://tw.nszjky.cn

Java: @Override String greet() { return "admin"; }
来源：http://pj.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://jz.szxytkj.cn

Ruby: def greet; "admin"; end
来源：http://uw.panjiajie.cn

C#:   public override string Greet() => "admin";
来源：http://vm.bookmarksfly.cn

[G07] 调用父类方法
来源：http://wk.yuntaijiaju.cn

Py:   super().greet()
来源：http://qc.szsharing.cn

PHP:  parent::greet();
来源：http://sq.muxihuayi.cn

JS:   super.greet();
来源：http://pr.huixinmuqiang.cn

TS:   super.greet();
来源：http://jm.huanxung.cn

Java: super.greet();
来源：http://jq.szxytkj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nr.wgjwhj.cn

Ruby: super
来源：http://of.wgjwhj.cn

C#:   base.Greet();
来源：http://uf.haigaiapp.cn

[G08] 静态方法与属性
来源：http://hk.chemitech.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ca.yuexingan06.cn

PHP:  public static function f() {}
来源：http://pi.szxytkj.cn

JS:   static f() {}
来源：http://rs.szxytkj.cn

TS:   static f(): void {}
来源：http://ef.colortex.cn

Java: static void f() {}
来源：http://nw.hnjuh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ot.521024.cn

Ruby: def self.f; end
来源：http://rg.szxytkj.cn

C#:   public static void F() {}
来源：http://tf.nicolike.cn

[G09] 接口 / 抽象类
来源：http://ez.muxihuayi.cn

Py:   from abc import ABC, abstractmethod
来源：http://mu.nszjky.cn

PHP:  interface Shape { public function area(): float; }
来源：http://md.yuexingan06.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bk.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://jx.hahajie.cn

Java: interface Shape { double area(); }
来源：http://at.szxytkj.cn

Go:   type Shape interface { Area() float64 }
来源：http://lz.colortex.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://on.nszjky.cn

C#:   interface IShape { double Area(); }
来源：http://rf.huixiangedu.cn

[G10] 访问控制
来源：http://ws.9csxet.cn

Py:   约定 _protected / __private（不强制）
来源：http://lc.shxzskj.cn

PHP:  public / protected / private
来源：http://ve.shtwfgs.cn

JS:   #private 字段；其余公开
来源：http://nl.nszjky.cn

TS:   public / protected / private
来源：http://cr.newstarts.cn

Java: public / protected / private / 默认包级
来源：http://sl.lnxyls.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lw.bookmarksfly.cn

Ruby: public / protected / private
来源：http://sz.huixiangedu.cn

C#:   public / protected / private / internal
来源：http://is.szxytkj.cn

[G11] getter / setter
来源：http://gx.huanxung.cn

Py:   @property 与 @x.setter
来源：http://ig.wgjwhj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dy.nszjky.cn

JS:   get name() { return this._name; }
来源：http://xi.hahajie.cn

TS:   get name(): string { return this._name; }
来源：http://rs.haigaiapp.cn

Java: public String getName() { return name; }
来源：http://kb.hnjuh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ks.asd995.cn

Ruby: attr_accessor :name
来源：http://be.haigaiapp.cn

C#:   public string Name { get; set; }
来源：http://qz.panjiajie.cn

[G12] 对象转字符串
来源：http://vw.shxzukj.cn

Py:   def __str__(self): return self.name
来源：http://ep.szxytkj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zi.shtwfgs.cn

JS:   toString() { return this.name; }
来源：http://aa.panjiajie.cn

TS:   toString(): string { return this.name; }
来源：http://xh.shxzukj.cn

Java: @Override public String toString() { return name; }
来源：http://hy.yuexingan06.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pp.gzmigu.cn

Ruby: def to_s; @name; end
来源：http://nw.chemitech.net.cn

C#:   public override string ToString() => Name;
来源：http://ti.hahajie.cn

[G13] 判断对象类型
来源：http://ry.huanxung.cn

Py:   isinstance(u, User)
来源：http://sn.nszjky.cn

PHP:  $u instanceof User
来源：http://td.huixiangedu.cn

JS:   u instanceof User
来源：http://fw.9csxet.cn

TS:   u instanceof User
来源：http://vx.gzmigu.cn

Java: u instanceof User
来源：http://zm.hnjuh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ui.hahajie.cn

Ruby: u.is_a?(User)
来源：http://mp.huanxung.cn

C#:   u is User
来源：http://lz.9csxet.cn

[G14] 数据类 / record
来源：http://jf.9csxet.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://we.muxihuayi.cn

PHP:  // 用 readonly 属性模拟
来源：http://uh.shxzukj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://np.wgjwhj.cn

TS:   type User = { name: string; age: number };
来源：http://pg.shxzukj.cn

Java: record User(String name, int age) {}
来源：http://cc.asd995.cn

Go:   type User struct { Name string; Age int }
来源：http://zf.huixiangedu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ly.hahajie.cn

C#:   record User(string Name, int Age);
来源：http://ga.muxihuayi.cn

[G15] 枚举
来源：http://os.chemitech.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ne.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://oq.chemitech.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://nd.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xy.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://pw.nicolike.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://se.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://nw.haigaiapp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://he.jianghongdianzi.cn

[G16] 对象转数组 / 字典
来源：http://pp.shtwfgs.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rz.asd995.cn

PHP:  get_object_vars($obj);
来源：http://bb.gzmigu.cn

JS:   Object.entries(obj)
来源：http://vc.haigaiapp.cn

TS:   Object.entries(obj)
来源：http://br.haigaiapp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tj.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qf.shxzukj.cn

Ruby: obj.instance_variables
来源：http://xh.nicolike.cn

C#:   // 用反射或 System.Text.Json
来源：http://kp.jianghongdianzi.cn

================================================================================
来源：http://oa.huixinmuqiang.cn

H. 异常与错误处理
来源：http://no.hahajie.cn

================================================================================
来源：http://vp.lnxyls.cn

[H01] try / catch 基础
来源：http://ep.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tn.newstarts.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dh.haigaiapp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mh.panjiajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ql.huixinmuqiang.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mx.lnxyls.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lj.bjjhwx.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ww.jctech888.com.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jr.asd995.cn

[H02] finally / ensure 收尾
来源：http://vl.colortex.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pv.shxzukj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gj.shxzskj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ei.szsharing.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bk.huanxung.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wu.newstarts.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xd.panjiajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oj.chemitech.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sy.huixiangedu.cn

[H03] 主动抛出异常
来源：http://xc.bjjhwx.cn

Py:   raise ValueError("错误信息")
来源：http://lj.521024.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://di.gzmigu.cn

JS:   throw new Error("错误信息");
来源：http://xh.muxihuayi.cn

TS:   throw new Error("错误信息");
来源：http://xh.szxytkj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://se.haigaiapp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hf.szxytkj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jp.szxytkj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jm.panjiajie.cn

[H04] 自定义异常类型
来源：http://lg.huixinmuqiang.cn

Py:   class MyError(Exception): pass
来源：http://jj.nszjky.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hg.jianghongdianzi.cn

JS:   class MyError extends Error {}
来源：http://hj.newstarts.cn

TS:   class MyError extends Error {}
来源：http://tj.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://gj.bookmarksfly.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ub.szsharing.cn

Ruby: class MyError < StandardError; end
来源：http://bp.colortex.cn

C#:   class MyException : Exception {}
来源：http://ls.asd995.cn

[H05] 捕获特定类型
来源：http://jl.muxihuayi.cn

Py:   except ValueError as e:
来源：http://oo.huixinmuqiang.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://sd.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://gw.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://go.szsharing.cn

Java: catch (IOException | SQLException e) {}
来源：http://of.newstarts.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nf.huanxung.cn

Ruby: rescue ArgumentError => e
来源：http://zd.jctech888.com.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ux.huixinmuqiang.cn

[H06] 可选值 / 空值安全访问
来源：http://zl.chemitech.net.cn

Py:   value = d.get("k") or default
来源：http://op.9csxet.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kj.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://uk.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pj.shtwfgs.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vv.lnxyls.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nw.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://rt.bjjhwx.cn

C#:   obj?.A?.B ?? default
来源：http://fq.szsharing.cn

[H07] 断言
来源：http://gp.colortex.cn

Py:   assert x > 0, "必须为正"
来源：http://ds.shxzskj.cn

PHP:  assert($x > 0);
来源：http://cp.nicolike.cn

JS:   console.assert(x > 0);
来源：http://aq.9csxet.cn

TS:   console.assert(x > 0);
来源：http://aj.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://qd.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wy.shxzskj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://at.szxytkj.cn

C#:   Debug.Assert(x > 0);
来源：http://kl.newstarts.cn

[H08] 获取错误信息与堆栈
来源：http://yo.szxytkj.cn

Py:   str(e);  traceback.format_exc()
来源：http://ky.bookmarksfly.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cj.huixinmuqiang.cn

JS:   e.message;  e.stack
来源：http://pw.yuntaijiaju.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jr.huixinmuqiang.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hi.wgjwhj.cn

Go:   err.Error()
来源：http://ty.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://bh.lnxyls.cn

C#:   e.Message;  e.StackTrace
来源：http://pk.wgjwhj.cn

[H09] 带错误码的异常
来源：http://vh.newstarts.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kn.haigaiapp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://in.yuexingan06.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hf.gzmigu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dy.colortex.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zr.szsharing.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wc.szsharing.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gq.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mj.muxihuayi.cn

[H10] 资源自动释放
来源：http://ny.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zh.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ao.yuntaijiaju.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ws.shxzskj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nd.haigaiapp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kw.szxytkj.cn

Go:   defer f.Close()
来源：http://ao.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qs.yuexingan06.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zr.asd995.cn

================================================================================
来源：http://dn.shxzukj.cn

I. 正则表达式
来源：http://nd.shtwfgs.cn

================================================================================
来源：http://jt.nszjky.cn

[I01] 判断是否匹配
来源：http://oh.jctech888.com.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fr.hnjuh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://aw.asd995.cn

JS:   /\d+/.test(s)
来源：http://sv.9csxet.cn

TS:   /\d+/.test(s)
来源：http://ea.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lx.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fh.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://gz.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xy.bjjhwx.cn

[I02] 提取所有匹配
来源：http://lg.gzmigu.cn

Py:   re.findall(r"\d+", s)
来源：http://bi.colortex.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rt.yuntaijiaju.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mm.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://xi.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ep.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vx.chemitech.net.cn

Ruby: s.scan(/\d+/)
来源：http://fb.bookmarksfly.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ro.bjjhwx.cn

[I03] 提取捕获分组
来源：http://si.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cd.wgjwhj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bd.yuexingan06.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mk.9csxet.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://iw.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zj.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://tw.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ic.colortex.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wd.jianghongdianzi.cn

[I04] 正则替换
来源：http://pr.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nr.wgjwhj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lc.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ft.wgjwhj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qp.gzmigu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://wb.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kd.chemitech.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://af.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qs.huixinmuqiang.cn

[I05] 按正则拆分
来源：http://vu.bookmarksfly.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ey.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://eo.shxzskj.cn

JS:   s.split(/\s*,\s*/)
来源：http://ww.szxytkj.cn

TS:   s.split(/\s*,\s*/)
来源：http://wx.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://me.wgjwhj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pm.huixinmuqiang.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rz.yuexingan06.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xt.jctech888.com.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vt.yuntaijiaju.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rm.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://eg.bjjhwx.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wh.asd995.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://id.wgjwhj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kn.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ij.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cx.colortex.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cw.nszjky.cn

[I07] 忽略大小写与多行模式
来源：http://dj.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ic.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mr.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bc.nszjky.cn

TS:   /error/gim
来源：http://sk.hnjuh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uo.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ee.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://jg.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vt.gzmigu.cn

[I08] 贪婪与非贪婪匹配
来源：http://hk.panjiajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://zw.hahajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://is.nicolike.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fh.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xx.lnxyls.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rk.521024.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ya.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oj.yuexingan06.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://za.9csxet.cn

================================================================================
来源：http://oj.wgjwhj.cn

J. 日期与时间
来源：http://wd.9csxet.cn

================================================================================
来源：http://rr.panjiajie.cn

[J01] 获取当前时间
来源：http://yn.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zw.hahajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://le.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://kn.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://ns.521024.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://it.shxzukj.cn

Go:   time.Now()
来源：http://mx.haigaiapp.cn

Ruby: Time.now
来源：http://ev.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nj.huixinmuqiang.cn

[J02] 格式化输出
来源：http://qq.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qf.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hd.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zm.asd995.cn

TS:   d.toISOString()
来源：http://bu.haigaiapp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tu.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://oj.hnjuh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qs.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kp.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://zg.bjjhwx.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lq.9csxet.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lv.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://yy.521024.cn

TS:   new Date("2024-01-02")
来源：http://xm.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ot.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mp.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://cj.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jq.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://qc.chemitech.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xu.bjjhwx.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xo.shtwfgs.cn


<!-- 参考信息 -->