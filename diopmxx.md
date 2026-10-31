代发 wailian999

JS:   super.greet();
来源：http://dx.panjiajie.cn

TS:   super.greet();
来源：http://rm.shxzskj.cn

Java: super.greet();
来源：http://is.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xg.yuntaijiaju.cn

Ruby: super
来源：http://fa.jianghongdianzi.cn

C#:   base.Greet();
来源：http://qz.wgjwhj.cn

[G08] 静态方法与属性
来源：http://fw.szsharing.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mw.newstarts.cn

PHP:  public static function f() {}
来源：http://gr.chemitech.net.cn

JS:   static f() {}
来源：http://op.asd995.cn

TS:   static f(): void {}
来源：http://jb.bookmarksfly.cn

Java: static void f() {}
来源：http://yu.9csxet.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://wu.shtwfgs.cn

Ruby: def self.f; end
来源：http://xq.wgjwhj.cn

C#:   public static void F() {}
来源：http://le.huixiangedu.cn

[G09] 接口 / 抽象类
来源：http://ym.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://vs.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wo.hahajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ut.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://og.shtwfgs.cn

Java: interface Shape { double area(); }
来源：http://ga.jctech888.com.cn

Go:   type Shape interface { Area() float64 }
来源：http://sx.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://aw.shxzukj.cn

C#:   interface IShape { double Area(); }
来源：http://rn.huixiangedu.cn

[G10] 访问控制
来源：http://rl.huixinmuqiang.cn

Py:   约定 _protected / __private（不强制）
来源：http://bp.panjiajie.cn

PHP:  public / protected / private
来源：http://rs.hnjuh.cn

JS:   #private 字段；其余公开
来源：http://aq.lnxyls.cn

TS:   public / protected / private
来源：http://tl.jctech888.com.cn

Java: public / protected / private / 默认包级
来源：http://xb.panjiajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bs.asd995.cn

Ruby: public / protected / private
来源：http://aj.hnjuh.cn

C#:   public / protected / private / internal
来源：http://ka.yuexingan06.cn

[G11] getter / setter
来源：http://tz.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://gq.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fv.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://yo.muxihuayi.cn

TS:   get name(): string { return this._name; }
来源：http://ge.shxzukj.cn

Java: public String getName() { return name; }
来源：http://hg.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ry.jianghongdianzi.cn

Ruby: attr_accessor :name
来源：http://ts.wgjwhj.cn

C#:   public string Name { get; set; }
来源：http://ui.gzmigu.cn

[G12] 对象转字符串
来源：http://vg.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://in.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sh.szxytkj.cn

JS:   toString() { return this.name; }
来源：http://ig.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://ov.521024.cn

Java: @Override public String toString() { return name; }
来源：http://za.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://aq.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://ci.wgjwhj.cn

C#:   public override string ToString() => Name;
来源：http://pr.newstarts.cn

[G13] 判断对象类型
来源：http://ki.colortex.cn

Py:   isinstance(u, User)
来源：http://xy.shxzskj.cn

PHP:  $u instanceof User
来源：http://qx.szxytkj.cn

JS:   u instanceof User
来源：http://ox.lnxyls.cn

TS:   u instanceof User
来源：http://dq.nszjky.cn

Java: u instanceof User
来源：http://qu.haigaiapp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fb.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://mm.hnjuh.cn

C#:   u is User
来源：http://yi.hahajie.cn

[G14] 数据类 / record
来源：http://xy.yuntaijiaju.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://pj.huanxung.cn

PHP:  // 用 readonly 属性模拟
来源：http://ag.colortex.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vf.haigaiapp.cn

TS:   type User = { name: string; age: number };
来源：http://tj.lnxyls.cn

Java: record User(String name, int age) {}
来源：http://zo.szxytkj.cn

Go:   type User struct { Name string; Age int }
来源：http://bk.huixiangedu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wk.hnjuh.cn

C#:   record User(string Name, int Age);
来源：http://ki.jianghongdianzi.cn

[G15] 枚举
来源：http://qj.haigaiapp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mx.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://an.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xt.haigaiapp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ls.hahajie.cn

Java: enum Color { RED, GREEN }
来源：http://um.chemitech.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zi.bookmarksfly.cn

Ruby: Color = %i[red green].freeze
来源：http://sg.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ew.hnjuh.cn

[G16] 对象转数组 / 字典
来源：http://et.nicolike.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vm.muxihuayi.cn

PHP:  get_object_vars($obj);
来源：http://be.colortex.cn

JS:   Object.entries(obj)
来源：http://nc.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://ub.yuexingan06.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hy.colortex.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kc.chemitech.net.cn

Ruby: obj.instance_variables
来源：http://pd.yuntaijiaju.cn

C#:   // 用反射或 System.Text.Json
来源：http://vj.yuexingan06.cn

================================================================================
来源：http://wl.hnjuh.cn

H. 异常与错误处理
来源：http://ml.bookmarksfly.cn

================================================================================
来源：http://av.nicolike.cn

[H01] try / catch 基础
来源：http://sf.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://of.hnjuh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fj.9csxet.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bq.szxytkj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ko.bookmarksfly.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zj.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yk.yuntaijiaju.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zl.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wy.chemitech.net.cn

[H02] finally / ensure 收尾
来源：http://nf.szxytkj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lm.szsharing.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sn.szxytkj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ma.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vi.shxzukj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lq.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cw.gzmigu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.gzmigu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cn.newstarts.cn

[H03] 主动抛出异常
来源：http://rt.colortex.cn

Py:   raise ValueError("错误信息")
来源：http://hw.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mr.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://ka.shxzukj.cn

TS:   throw new Error("错误信息");
来源：http://gc.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lh.shxzskj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xx.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zd.bookmarksfly.cn

C#:   throw new ArgumentException("错误信息");
来源：http://sb.shxzskj.cn

[H04] 自定义异常类型
来源：http://xa.newstarts.cn

Py:   class MyError(Exception): pass
来源：http://jm.colortex.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dy.newstarts.cn

JS:   class MyError extends Error {}
来源：http://qm.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://zz.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://qb.huixiangedu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wf.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://ml.yuexingan06.cn

C#:   class MyException : Exception {}
来源：http://ng.hahajie.cn

[H05] 捕获特定类型
来源：http://to.muxihuayi.cn

Py:   except ValueError as e:
来源：http://on.shxzskj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uj.lnxyls.cn

JS:   if (e instanceof TypeError) {}
来源：http://xt.chemitech.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://kv.jctech888.com.cn

Java: catch (IOException | SQLException e) {}
来源：http://eq.shtwfgs.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cn.muxihuayi.cn

Ruby: rescue ArgumentError => e
来源：http://tw.asd995.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pn.nszjky.cn

[H06] 可选值 / 空值安全访问
来源：http://fr.haigaiapp.cn

Py:   value = d.get("k") or default
来源：http://em.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://je.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://sl.shxzukj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xe.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wc.muxihuayi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dr.shxzukj.cn

Ruby: d&.dig(:a, :b)
来源：http://ua.newstarts.cn

C#:   obj?.A?.B ?? default
来源：http://rb.yuexingan06.cn

[H07] 断言
来源：http://xk.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://iz.nicolike.cn

PHP:  assert($x > 0);
来源：http://yh.shtwfgs.cn

JS:   console.assert(x > 0);
来源：http://gq.521024.cn

TS:   console.assert(x > 0);
来源：http://fx.wgjwhj.cn

Java: assert x > 0 : "必须为正";
来源：http://hw.nicolike.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ak.9csxet.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lx.newstarts.cn

C#:   Debug.Assert(x > 0);
来源：http://cd.shxzukj.cn

[H08] 获取错误信息与堆栈
来源：http://zd.panjiajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://pq.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://eg.haigaiapp.cn

JS:   e.message;  e.stack
来源：http://sz.nszjky.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yh.huanxung.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uh.bjjhwx.cn

Go:   err.Error()
来源：http://oz.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://ki.shtwfgs.cn

C#:   e.Message;  e.StackTrace
来源：http://qw.haigaiapp.cn

[H09] 带错误码的异常
来源：http://vk.521024.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dh.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ru.szxytkj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zz.shtwfgs.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ve.asd995.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zd.bookmarksfly.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mh.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://td.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ty.jctech888.com.cn

[H10] 资源自动释放
来源：http://fd.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://py.lnxyls.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vx.gzmigu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vm.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bn.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zq.bjjhwx.cn

Go:   defer f.Close()
来源：http://wq.jctech888.com.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xf.shtwfgs.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gd.muxihuayi.cn

================================================================================
来源：http://pb.shxzskj.cn

I. 正则表达式
来源：http://fz.jianghongdianzi.cn

================================================================================
来源：http://fb.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://bw.shxzukj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vd.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://os.jctech888.com.cn

JS:   /\d+/.test(s)
来源：http://dy.shxzukj.cn

TS:   /\d+/.test(s)
来源：http://ne.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zf.nicolike.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://iq.szsharing.cn

Ruby: s.match?(/\d+/)
来源：http://sh.szsharing.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vg.muxihuayi.cn

[I02] 提取所有匹配
来源：http://cf.nicolike.cn

Py:   re.findall(r"\d+", s)
来源：http://qm.huixiangedu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zn.wgjwhj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ep.szsharing.cn

TS:   s.match(/\d+/g)
来源：http://wa.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cl.colortex.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sa.521024.cn

Ruby: s.scan(/\d+/)
来源：http://js.shtwfgs.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vi.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://qv.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ip.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ex.szxytkj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wf.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vg.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vb.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ra.hnjuh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vt.szsharing.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ng.bookmarksfly.cn

[I04] 正则替换
来源：http://hi.huixinmuqiang.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mk.jianghongdianzi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cg.nszjky.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ng.jianghongdianzi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://fu.muxihuayi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ww.chemitech.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://el.yuntaijiaju.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jp.9csxet.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jr.hahajie.cn

[I05] 按正则拆分
来源：http://xj.shxzskj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nn.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gj.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://kh.yuntaijiaju.cn

TS:   s.split(/\s*,\s*/)
来源：http://el.bookmarksfly.cn

Java: s.split("\\s*,\\s*")
来源：http://nv.gzmigu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://uy.newstarts.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ux.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pf.bjjhwx.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zz.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cg.yuexingan06.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uw.muxihuayi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ix.jctech888.com.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lr.hnjuh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yq.huanxung.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rk.wgjwhj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://kr.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ai.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://rn.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nt.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pk.yuexingan06.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xg.colortex.cn

TS:   /error/gim
来源：http://sq.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cs.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qy.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://oc.shtwfgs.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ls.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://py.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://of.gzmigu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gu.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vm.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rs.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qn.hnjuh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oi.lnxyls.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ce.huanxung.cn

================================================================================
来源：http://bh.lnxyls.cn

J. 日期与时间
来源：http://tt.huixinmuqiang.cn

================================================================================
来源：http://rh.gzmigu.cn

[J01] 获取当前时间
来源：http://qo.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cf.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://al.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://mp.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://zu.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wc.newstarts.cn

Go:   time.Now()
来源：http://vm.huixinmuqiang.cn

Ruby: Time.now
来源：http://ta.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mg.9csxet.cn

[J02] 格式化输出
来源：http://na.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kd.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mj.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wo.asd995.cn

TS:   d.toISOString()
来源：http://xw.haigaiapp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ey.chemitech.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ya.bjjhwx.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ir.hnjuh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ck.9csxet.cn

[J03] 字符串解析为日期
来源：http://eu.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lk.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zh.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://jq.asd995.cn

TS:   new Date("2024-01-02")
来源：http://nc.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ua.haigaiapp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uq.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://wp.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gz.newstarts.cn

[J04] 时间戳与日期互转
来源：http://vx.huixiangedu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gx.bjjhwx.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nv.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vf.yuexingan06.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cu.9csxet.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yg.lnxyls.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://or.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wh.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lu.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://kr.bjjhwx.cn

Py:   now + timedelta(days=7)
来源：http://nf.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://qy.newstarts.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tc.nicolike.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kg.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://wr.521024.cn


<!-- 参考信息 -->