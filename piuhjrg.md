代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://nt.haigaiapp.cn

[G07] 调用父类方法
来源：http://nf.panjiajie.cn

Py:   super().greet()
来源：http://zu.gzmigu.cn

PHP:  parent::greet();
来源：http://ly.nszjky.cn

JS:   super.greet();
来源：http://kz.nszjky.cn

TS:   super.greet();
来源：http://tu.shtwfgs.cn

Java: super.greet();
来源：http://xc.huixinmuqiang.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nq.bjjhwx.cn

Ruby: super
来源：http://yi.szxytkj.cn

C#:   base.Greet();
来源：http://vl.wgjwhj.cn

[G08] 静态方法与属性
来源：http://wr.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://or.gzmigu.cn

PHP:  public static function f() {}
来源：http://ez.jianghongdianzi.cn

JS:   static f() {}
来源：http://nx.jctech888.com.cn

TS:   static f(): void {}
来源：http://ng.521024.cn

Java: static void f() {}
来源：http://pa.jctech888.com.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mk.szsharing.cn

Ruby: def self.f; end
来源：http://kl.hnjuh.cn

C#:   public static void F() {}
来源：http://ot.szsharing.cn

[G09] 接口 / 抽象类
来源：http://bg.muxihuayi.cn

Py:   from abc import ABC, abstractmethod
来源：http://gw.szxytkj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://gc.wgjwhj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xi.gzmigu.cn

TS:   interface Shape { area(): number; }
来源：http://do.szxytkj.cn

Java: interface Shape { double area(); }
来源：http://um.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://yi.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cp.panjiajie.cn

C#:   interface IShape { double Area(); }
来源：http://rn.newstarts.cn

[G10] 访问控制
来源：http://eb.szxytkj.cn

Py:   约定 _protected / __private（不强制）
来源：http://dg.lnxyls.cn

PHP:  public / protected / private
来源：http://kb.nszjky.cn

JS:   #private 字段；其余公开
来源：http://qg.gzmigu.cn

TS:   public / protected / private
来源：http://bd.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://nl.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mj.bookmarksfly.cn

Ruby: public / protected / private
来源：http://gu.panjiajie.cn

C#:   public / protected / private / internal
来源：http://ut.9csxet.cn

[G11] getter / setter
来源：http://yk.nicolike.cn

Py:   @property 与 @x.setter
来源：http://gn.szxytkj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://la.szsharing.cn

JS:   get name() { return this._name; }
来源：http://yf.jianghongdianzi.cn

TS:   get name(): string { return this._name; }
来源：http://pa.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://ot.huixiangedu.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hk.gzmigu.cn

Ruby: attr_accessor :name
来源：http://nr.chemitech.net.cn

C#:   public string Name { get; set; }
来源：http://on.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://pi.haigaiapp.cn

Py:   def __str__(self): return self.name
来源：http://qp.huanxung.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://om.yuexingan06.cn

JS:   toString() { return this.name; }
来源：http://vu.panjiajie.cn

TS:   toString(): string { return this.name; }
来源：http://kk.yuexingan06.cn

Java: @Override public String toString() { return name; }
来源：http://zx.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://cq.yuexingan06.cn

Ruby: def to_s; @name; end
来源：http://iv.nicolike.cn

C#:   public override string ToString() => Name;
来源：http://ey.521024.cn

[G13] 判断对象类型
来源：http://uy.huixiangedu.cn

Py:   isinstance(u, User)
来源：http://vj.gzmigu.cn

PHP:  $u instanceof User
来源：http://xt.haigaiapp.cn

JS:   u instanceof User
来源：http://hk.nicolike.cn

TS:   u instanceof User
来源：http://ub.haigaiapp.cn

Java: u instanceof User
来源：http://xs.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ze.newstarts.cn

Ruby: u.is_a?(User)
来源：http://em.bjjhwx.cn

C#:   u is User
来源：http://mn.hnjuh.cn

[G14] 数据类 / record
来源：http://fs.hahajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ml.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://tl.panjiajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ac.bookmarksfly.cn

TS:   type User = { name: string; age: number };
来源：http://te.nicolike.cn

Java: record User(String name, int age) {}
来源：http://fz.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://jy.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cy.9csxet.cn

C#:   record User(string Name, int Age);
来源：http://kv.nszjky.cn

[G15] 枚举
来源：http://jn.huanxung.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vi.nicolike.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ac.nszjky.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://co.colortex.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ea.colortex.cn

Java: enum Color { RED, GREEN }
来源：http://sm.colortex.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ql.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://jd.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ie.shxzukj.cn

[G16] 对象转数组 / 字典
来源：http://si.9csxet.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ji.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://gy.nszjky.cn

JS:   Object.entries(obj)
来源：http://ji.9csxet.cn

TS:   Object.entries(obj)
来源：http://qr.szsharing.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wu.lnxyls.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://js.chemitech.net.cn

Ruby: obj.instance_variables
来源：http://oe.hahajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://ci.shxzukj.cn

================================================================================
来源：http://zc.chemitech.net.cn

H. 异常与错误处理
来源：http://ai.wgjwhj.cn

================================================================================
来源：http://bh.hahajie.cn

[H01] try / catch 基础
来源：http://om.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ax.szxytkj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wi.yuntaijiaju.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vi.szsharing.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cs.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zs.gzmigu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mp.bookmarksfly.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bb.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ud.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://ct.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rl.shxzukj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dq.jctech888.com.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rh.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://po.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ou.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rc.bookmarksfly.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ku.nszjky.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ys.panjiajie.cn

[H03] 主动抛出异常
来源：http://ab.jctech888.com.cn

Py:   raise ValueError("错误信息")
来源：http://xe.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gk.bjjhwx.cn

JS:   throw new Error("错误信息");
来源：http://on.yuexingan06.cn

TS:   throw new Error("错误信息");
来源：http://tp.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xn.jctech888.com.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ny.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jt.szxytkj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kc.colortex.cn

[H04] 自定义异常类型
来源：http://gm.lnxyls.cn

Py:   class MyError(Exception): pass
来源：http://cs.521024.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ij.huixiangedu.cn

JS:   class MyError extends Error {}
来源：http://qf.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://tz.haigaiapp.cn

Java: class MyException extends RuntimeException {}
来源：http://tc.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pr.lnxyls.cn

Ruby: class MyError < StandardError; end
来源：http://hu.shxzukj.cn

C#:   class MyException : Exception {}
来源：http://zn.nszjky.cn

[H05] 捕获特定类型
来源：http://jn.nszjky.cn

Py:   except ValueError as e:
来源：http://hl.lnxyls.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fh.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://wy.haigaiapp.cn

TS:   if (e instanceof TypeError) {}
来源：http://hn.hahajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://gj.bookmarksfly.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zz.bookmarksfly.cn

Ruby: rescue ArgumentError => e
来源：http://jz.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mx.hnjuh.cn

[H06] 可选值 / 空值安全访问
来源：http://bs.wgjwhj.cn

Py:   value = d.get("k") or default
来源：http://wn.nszjky.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ly.haigaiapp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://em.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yt.nszjky.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gg.szxytkj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hw.colortex.cn

Ruby: d&.dig(:a, :b)
来源：http://ar.hnjuh.cn

C#:   obj?.A?.B ?? default
来源：http://yi.bookmarksfly.cn

[H07] 断言
来源：http://xx.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://nq.jctech888.com.cn

PHP:  assert($x > 0);
来源：http://oj.newstarts.cn

JS:   console.assert(x > 0);
来源：http://yu.yuexingan06.cn

TS:   console.assert(x > 0);
来源：http://gr.hnjuh.cn

Java: assert x > 0 : "必须为正";
来源：http://uh.muxihuayi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xd.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ci.bookmarksfly.cn

C#:   Debug.Assert(x > 0);
来源：http://pk.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://kr.lnxyls.cn

Py:   str(e);  traceback.format_exc()
来源：http://ul.szxytkj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cx.colortex.cn

JS:   e.message;  e.stack
来源：http://sm.shtwfgs.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://sl.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://io.hnjuh.cn

Go:   err.Error()
来源：http://xe.wgjwhj.cn

Ruby: e.message;  e.backtrace
来源：http://rg.shxzukj.cn

C#:   e.Message;  e.StackTrace
来源：http://en.521024.cn

[H09] 带错误码的异常
来源：http://vv.shxzukj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wp.szxytkj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jm.huanxung.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sc.hahajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nc.asd995.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mq.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vb.panjiajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://eo.haigaiapp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mk.lnxyls.cn

[H10] 资源自动释放
来源：http://eu.521024.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rl.hnjuh.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tb.huixinmuqiang.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lo.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vq.newstarts.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xr.hahajie.cn

Go:   defer f.Close()
来源：http://kr.huixinmuqiang.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cw.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fr.colortex.cn

================================================================================
来源：http://dy.hahajie.cn

I. 正则表达式
来源：http://bv.nszjky.cn

================================================================================
来源：http://ip.huanxung.cn

[I01] 判断是否匹配
来源：http://sa.haigaiapp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://or.521024.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ey.asd995.cn

JS:   /\d+/.test(s)
来源：http://cl.asd995.cn

TS:   /\d+/.test(s)
来源：http://ul.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bz.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wm.huanxung.cn

Ruby: s.match?(/\d+/)
来源：http://ah.newstarts.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sn.huixiangedu.cn

[I02] 提取所有匹配
来源：http://aa.gzmigu.cn

Py:   re.findall(r"\d+", s)
来源：http://yv.szxytkj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zr.521024.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ez.szxytkj.cn

TS:   s.match(/\d+/g)
来源：http://zg.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://go.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cc.muxihuayi.cn

Ruby: s.scan(/\d+/)
来源：http://ij.asd995.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xf.yuexingan06.cn

[I03] 提取捕获分组
来源：http://vn.nszjky.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rv.huixiangedu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kd.chemitech.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fl.huixiangedu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ox.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ti.bookmarksfly.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cg.shxzskj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qi.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cd.yuntaijiaju.cn

[I04] 正则替换
来源：http://sb.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sq.hnjuh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://eb.huanxung.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xf.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sf.asd995.cn

Java: s.replaceAll("\\d+", "#")
来源：http://eo.gzmigu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oj.wgjwhj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pw.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pi.szxytkj.cn

[I05] 按正则拆分
来源：http://ry.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hk.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jx.lnxyls.cn

JS:   s.split(/\s*,\s*/)
来源：http://oq.shxzukj.cn

TS:   s.split(/\s*,\s*/)
来源：http://yr.huanxung.cn

Java: s.split("\\s*,\\s*")
来源：http://mt.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wv.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://da.bjjhwx.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://pl.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sd.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://st.hnjuh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://mn.newstarts.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mm.shxzukj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ai.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gq.muxihuayi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ta.521024.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lk.bookmarksfly.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gj.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://cr.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qs.bjjhwx.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://we.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lw.521024.cn

TS:   /error/gim
来源：http://hf.chemitech.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ff.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://oa.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://xj.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uc.bjjhwx.cn

[I08] 贪婪与非贪婪匹配
来源：http://yw.panjiajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ht.colortex.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://su.9csxet.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://gk.shxzskj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gy.huanxung.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ah.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zf.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qz.wgjwhj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yz.hnjuh.cn

================================================================================
来源：http://tv.szsharing.cn

J. 日期与时间
来源：http://gd.9csxet.cn

================================================================================
来源：http://xs.newstarts.cn

[J01] 获取当前时间
来源：http://tl.nicolike.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fj.haigaiapp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://no.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://qz.huanxung.cn

TS:   new Date();  Date.now()
来源：http://jm.521024.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dj.panjiajie.cn

Go:   time.Now()
来源：http://at.shxzukj.cn

Ruby: Time.now
来源：http://kk.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nz.huixinmuqiang.cn

[J02] 格式化输出
来源：http://ab.gzmigu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uf.nszjky.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kb.huixinmuqiang.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ii.newstarts.cn

TS:   d.toISOString()
来源：http://ux.hnjuh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vp.yuexingan06.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pu.nszjky.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pb.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xx.huixinmuqiang.cn

[J03] 字符串解析为日期
来源：http://ol.lnxyls.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cv.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tm.muxihuayi.cn

JS:   new Date("2024-01-02")
来源：http://zs.bookmarksfly.cn

TS:   new Date("2024-01-02")
来源：http://pk.huanxung.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xa.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xy.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://ml.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tm.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://eo.szxytkj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zb.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://aj.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ca.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ws.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jf.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ty.muxihuayi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hd.asd995.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fm.shxzukj.cn

[J05] 时间加减（加 7 天）
来源：http://ul.asd995.cn

Py:   now + timedelta(days=7)
来源：http://sv.hahajie.cn


<!-- 参考信息 -->