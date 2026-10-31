代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://dr.colortex.cn

[G07] 调用父类方法
来源：http://ag.newstarts.cn

Py:   super().greet()
来源：http://nx.chemitech.net.cn

PHP:  parent::greet();
来源：http://sp.521024.cn

JS:   super.greet();
来源：http://dj.hahajie.cn

TS:   super.greet();
来源：http://rp.jianghongdianzi.cn

Java: super.greet();
来源：http://bg.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://au.hnjuh.cn

Ruby: super
来源：http://fw.yuntaijiaju.cn

C#:   base.Greet();
来源：http://rv.gzmigu.cn

[G08] 静态方法与属性
来源：http://ud.yuexingan06.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fq.gzmigu.cn

PHP:  public static function f() {}
来源：http://pz.huixinmuqiang.cn

JS:   static f() {}
来源：http://vv.lnxyls.cn

TS:   static f(): void {}
来源：http://yr.haigaiapp.cn

Java: static void f() {}
来源：http://fl.jianghongdianzi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://an.huanxung.cn

Ruby: def self.f; end
来源：http://rt.nszjky.cn

C#:   public static void F() {}
来源：http://ut.shxzukj.cn

[G09] 接口 / 抽象类
来源：http://nj.yuntaijiaju.cn

Py:   from abc import ABC, abstractmethod
来源：http://iq.wgjwhj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://mf.jianghongdianzi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://cd.chemitech.net.cn

TS:   interface Shape { area(): number; }
来源：http://pt.panjiajie.cn

Java: interface Shape { double area(); }
来源：http://xm.muxihuayi.cn

Go:   type Shape interface { Area() float64 }
来源：http://dd.szxytkj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bb.jctech888.com.cn

C#:   interface IShape { double Area(); }
来源：http://dl.huixiangedu.cn

[G10] 访问控制
来源：http://uq.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://ko.szsharing.cn

PHP:  public / protected / private
来源：http://tf.nszjky.cn

JS:   #private 字段；其余公开
来源：http://ln.haigaiapp.cn

TS:   public / protected / private
来源：http://ej.bookmarksfly.cn

Java: public / protected / private / 默认包级
来源：http://tc.huanxung.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://oo.asd995.cn

Ruby: public / protected / private
来源：http://cw.lnxyls.cn

C#:   public / protected / private / internal
来源：http://ys.bjjhwx.cn

[G11] getter / setter
来源：http://ut.wgjwhj.cn

Py:   @property 与 @x.setter
来源：http://ka.wgjwhj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://cu.yuexingan06.cn

JS:   get name() { return this._name; }
来源：http://jr.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://vt.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://ep.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://cw.huanxung.cn

Ruby: attr_accessor :name
来源：http://dn.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://mb.muxihuayi.cn

[G12] 对象转字符串
来源：http://hl.asd995.cn

Py:   def __str__(self): return self.name
来源：http://sc.wgjwhj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://od.szxytkj.cn

JS:   toString() { return this.name; }
来源：http://sx.bookmarksfly.cn

TS:   toString(): string { return this.name; }
来源：http://iq.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://tu.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kz.haigaiapp.cn

Ruby: def to_s; @name; end
来源：http://gk.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://li.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://yz.panjiajie.cn

Py:   isinstance(u, User)
来源：http://lg.colortex.cn

PHP:  $u instanceof User
来源：http://zz.muxihuayi.cn

JS:   u instanceof User
来源：http://fx.muxihuayi.cn

TS:   u instanceof User
来源：http://yu.nszjky.cn

Java: u instanceof User
来源：http://ta.haigaiapp.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://br.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://cz.hnjuh.cn

C#:   u is User
来源：http://wp.huixiangedu.cn

[G14] 数据类 / record
来源：http://vj.jianghongdianzi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://iu.9csxet.cn

PHP:  // 用 readonly 属性模拟
来源：http://we.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tb.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://ve.colortex.cn

Java: record User(String name, int age) {}
来源：http://fo.hahajie.cn

Go:   type User struct { Name string; Age int }
来源：http://ch.bookmarksfly.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://il.shtwfgs.cn

C#:   record User(string Name, int Age);
来源：http://zj.jianghongdianzi.cn

[G15] 枚举
来源：http://ut.shxzskj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vv.hahajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://or.huixinmuqiang.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wh.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://va.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://fe.bookmarksfly.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://sc.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://xr.newstarts.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kp.hnjuh.cn

[G16] 对象转数组 / 字典
来源：http://bk.colortex.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wq.asd995.cn

PHP:  get_object_vars($obj);
来源：http://xo.nszjky.cn

JS:   Object.entries(obj)
来源：http://yv.newstarts.cn

TS:   Object.entries(obj)
来源：http://mv.gzmigu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://iy.jctech888.com.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gh.shtwfgs.cn

Ruby: obj.instance_variables
来源：http://po.asd995.cn

C#:   // 用反射或 System.Text.Json
来源：http://mp.shxzukj.cn

================================================================================
来源：http://gk.lnxyls.cn

H. 异常与错误处理
来源：http://jr.muxihuayi.cn

================================================================================
来源：http://nf.asd995.cn

[H01] try / catch 基础
来源：http://ac.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qx.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wl.shxzukj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ca.chemitech.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rb.muxihuayi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xx.9csxet.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mp.muxihuayi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vx.nicolike.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rj.huixiangedu.cn

[H02] finally / ensure 收尾
来源：http://kp.wgjwhj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://iz.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xt.9csxet.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://se.colortex.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gq.nszjky.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ji.huixinmuqiang.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sq.gzmigu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gi.szsharing.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://uj.jianghongdianzi.cn

[H03] 主动抛出异常
来源：http://kv.szxytkj.cn

Py:   raise ValueError("错误信息")
来源：http://sq.nicolike.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fc.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://kd.asd995.cn

TS:   throw new Error("错误信息");
来源：http://ni.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://du.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wt.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cm.huixiangedu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dr.shtwfgs.cn

[H04] 自定义异常类型
来源：http://ov.jianghongdianzi.cn

Py:   class MyError(Exception): pass
来源：http://nz.9csxet.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qx.nicolike.cn

JS:   class MyError extends Error {}
来源：http://qu.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://zn.hnjuh.cn

Java: class MyException extends RuntimeException {}
来源：http://pv.jianghongdianzi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://to.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://sf.chemitech.net.cn

C#:   class MyException : Exception {}
来源：http://hs.muxihuayi.cn

[H05] 捕获特定类型
来源：http://en.szsharing.cn

Py:   except ValueError as e:
来源：http://gh.hahajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ky.nicolike.cn

JS:   if (e instanceof TypeError) {}
来源：http://th.521024.cn

TS:   if (e instanceof TypeError) {}
来源：http://qr.nszjky.cn

Java: catch (IOException | SQLException e) {}
来源：http://vi.asd995.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vj.bookmarksfly.cn

Ruby: rescue ArgumentError => e
来源：http://dd.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wg.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://zx.yuexingan06.cn

Py:   value = d.get("k") or default
来源：http://se.lnxyls.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jo.szxytkj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zv.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sj.huixinmuqiang.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wr.hahajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ul.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://fd.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://dl.chemitech.net.cn

[H07] 断言
来源：http://kt.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://ho.bjjhwx.cn

PHP:  assert($x > 0);
来源：http://su.9csxet.cn

JS:   console.assert(x > 0);
来源：http://sh.521024.cn

TS:   console.assert(x > 0);
来源：http://nn.jianghongdianzi.cn

Java: assert x > 0 : "必须为正";
来源：http://cq.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oa.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mo.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://za.colortex.cn

[H08] 获取错误信息与堆栈
来源：http://kc.szxytkj.cn

Py:   str(e);  traceback.format_exc()
来源：http://yg.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://zq.nszjky.cn

JS:   e.message;  e.stack
来源：http://rj.jctech888.com.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rp.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://af.nszjky.cn

Go:   err.Error()
来源：http://lb.521024.cn

Ruby: e.message;  e.backtrace
来源：http://dq.hahajie.cn

C#:   e.Message;  e.StackTrace
来源：http://dt.yuntaijiaju.cn

[H09] 带错误码的异常
来源：http://xk.jctech888.com.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bn.shtwfgs.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vr.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://je.huixiangedu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ap.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wq.shxzukj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uh.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://je.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://sk.9csxet.cn

[H10] 资源自动释放
来源：http://cj.wgjwhj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://un.yuexingan06.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xx.yuntaijiaju.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kn.521024.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://aw.newstarts.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ls.521024.cn

Go:   defer f.Close()
来源：http://gy.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xo.lnxyls.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jb.wgjwhj.cn

================================================================================
来源：http://wn.shtwfgs.cn

I. 正则表达式
来源：http://xd.wgjwhj.cn

================================================================================
来源：http://jj.szsharing.cn

[I01] 判断是否匹配
来源：http://ft.szsharing.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ui.szxytkj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://by.521024.cn

JS:   /\d+/.test(s)
来源：http://qm.hahajie.cn

TS:   /\d+/.test(s)
来源：http://mz.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://np.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pn.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://gm.9csxet.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ax.muxihuayi.cn

[I02] 提取所有匹配
来源：http://re.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://jd.huixinmuqiang.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qj.wgjwhj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qk.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://wc.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ti.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xe.panjiajie.cn

Ruby: s.scan(/\d+/)
来源：http://mr.lnxyls.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ge.chemitech.net.cn

[I03] 提取捕获分组
来源：http://hf.nszjky.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ia.huixinmuqiang.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ie.hahajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ty.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ki.hahajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://am.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://px.szsharing.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lg.bookmarksfly.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://iu.shtwfgs.cn

[I04] 正则替换
来源：http://ri.jctech888.com.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jg.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ir.huanxung.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ur.huanxung.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ht.jctech888.com.cn

Java: s.replaceAll("\\d+", "#")
来源：http://uj.chemitech.net.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kv.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jr.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lf.lnxyls.cn

[I05] 按正则拆分
来源：http://ds.jianghongdianzi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wt.szxytkj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qj.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://ut.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://ij.chemitech.net.cn

Java: s.split("\\s*,\\s*")
来源：http://mv.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fz.jianghongdianzi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cn.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kv.hahajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ye.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lg.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bb.szxytkj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ud.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ek.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zo.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tz.huixiangedu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zv.bookmarksfly.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gc.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://rf.muxihuayi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jg.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rg.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xy.muxihuayi.cn

TS:   /error/gim
来源：http://gl.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sj.9csxet.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ws.asd995.cn

Ruby: s.scan(/error/i)
来源：http://id.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zz.shxzukj.cn

[I08] 贪婪与非贪婪匹配
来源：http://dl.panjiajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ma.asd995.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zc.nicolike.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xa.huanxung.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://th.shxzukj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ds.asd995.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://iq.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yg.lnxyls.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nt.newstarts.cn

================================================================================
来源：http://ld.nicolike.cn

J. 日期与时间
来源：http://nj.nszjky.cn

================================================================================
来源：http://eq.asd995.cn

[J01] 获取当前时间
来源：http://bl.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ne.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eu.gzmigu.cn

JS:   new Date();  Date.now()
来源：http://rr.wgjwhj.cn

TS:   new Date();  Date.now()
来源：http://kn.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kw.gzmigu.cn

Go:   time.Now()
来源：http://sq.shxzskj.cn

Ruby: Time.now
来源：http://cl.hnjuh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://eq.newstarts.cn

[J02] 格式化输出
来源：http://ze.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ul.colortex.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jo.shxzskj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jc.hnjuh.cn

TS:   d.toISOString()
来源：http://um.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nm.asd995.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sa.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://of.hnjuh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gr.panjiajie.cn

[J03] 字符串解析为日期
来源：http://ue.panjiajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qt.hahajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://tx.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://ws.huanxung.cn

TS:   new Date("2024-01-02")
来源：http://yn.jctech888.com.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yl.bjjhwx.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ur.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://yw.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ge.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://fr.asd995.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pd.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zn.huanxung.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://af.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rt.nszjky.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gz.huixiangedu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gk.hnjuh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://oh.shxzukj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ry.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://xq.gzmigu.cn

Py:   now + timedelta(days=7)
来源：http://dm.wgjwhj.cn


<!-- 参考信息 -->