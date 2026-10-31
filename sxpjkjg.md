代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://yy.jianghongdianzi.cn

[G07] 调用父类方法
来源：http://hy.jctech888.com.cn

Py:   super().greet()
来源：http://ik.shxzukj.cn

PHP:  parent::greet();
来源：http://hg.hahajie.cn

JS:   super.greet();
来源：http://yp.jianghongdianzi.cn

TS:   super.greet();
来源：http://ve.jctech888.com.cn

Java: super.greet();
来源：http://qx.chemitech.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kx.shxzskj.cn

Ruby: super
来源：http://yp.asd995.cn

C#:   base.Greet();
来源：http://fu.jctech888.com.cn

[G08] 静态方法与属性
来源：http://zz.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://oj.9csxet.cn

PHP:  public static function f() {}
来源：http://gk.panjiajie.cn

JS:   static f() {}
来源：http://rt.jctech888.com.cn

TS:   static f(): void {}
来源：http://gu.jctech888.com.cn

Java: static void f() {}
来源：http://tq.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rn.9csxet.cn

Ruby: def self.f; end
来源：http://kz.wgjwhj.cn

C#:   public static void F() {}
来源：http://tu.chemitech.net.cn

[G09] 接口 / 抽象类
来源：http://zp.haigaiapp.cn

Py:   from abc import ABC, abstractmethod
来源：http://zx.huixiangedu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ki.huixiangedu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://oe.yuntaijiaju.cn

TS:   interface Shape { area(): number; }
来源：http://yg.szxytkj.cn

Java: interface Shape { double area(); }
来源：http://tu.9csxet.cn

Go:   type Shape interface { Area() float64 }
来源：http://es.szxytkj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://md.hnjuh.cn

C#:   interface IShape { double Area(); }
来源：http://nc.colortex.cn

[G10] 访问控制
来源：http://jn.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://oy.muxihuayi.cn

PHP:  public / protected / private
来源：http://cq.shtwfgs.cn

JS:   #private 字段；其余公开
来源：http://cg.newstarts.cn

TS:   public / protected / private
来源：http://vl.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://fg.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fi.shxzskj.cn

Ruby: public / protected / private
来源：http://at.bjjhwx.cn

C#:   public / protected / private / internal
来源：http://ii.muxihuayi.cn

[G11] getter / setter
来源：http://nh.nszjky.cn

Py:   @property 与 @x.setter
来源：http://gx.szsharing.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ct.szxytkj.cn

JS:   get name() { return this._name; }
来源：http://vw.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://py.bookmarksfly.cn

Java: public String getName() { return name; }
来源：http://ok.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://oe.yuexingan06.cn

Ruby: attr_accessor :name
来源：http://tf.chemitech.net.cn

C#:   public string Name { get; set; }
来源：http://fa.szsharing.cn

[G12] 对象转字符串
来源：http://xq.wgjwhj.cn

Py:   def __str__(self): return self.name
来源：http://ao.bookmarksfly.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yx.bjjhwx.cn

JS:   toString() { return this.name; }
来源：http://wm.szsharing.cn

TS:   toString(): string { return this.name; }
来源：http://nh.shxzskj.cn

Java: @Override public String toString() { return name; }
来源：http://zn.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jx.chemitech.net.cn

Ruby: def to_s; @name; end
来源：http://ez.nszjky.cn

C#:   public override string ToString() => Name;
来源：http://xu.jianghongdianzi.cn

[G13] 判断对象类型
来源：http://wl.bjjhwx.cn

Py:   isinstance(u, User)
来源：http://ct.asd995.cn

PHP:  $u instanceof User
来源：http://xy.521024.cn

JS:   u instanceof User
来源：http://vx.hnjuh.cn

TS:   u instanceof User
来源：http://oo.bjjhwx.cn

Java: u instanceof User
来源：http://qc.jianghongdianzi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://am.gzmigu.cn

Ruby: u.is_a?(User)
来源：http://cd.panjiajie.cn

C#:   u is User
来源：http://jq.chemitech.net.cn

[G14] 数据类 / record
来源：http://sk.yuntaijiaju.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oh.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://wz.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uo.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://mq.muxihuayi.cn

Java: record User(String name, int age) {}
来源：http://pv.haigaiapp.cn

Go:   type User struct { Name string; Age int }
来源：http://vt.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zh.szxytkj.cn

C#:   record User(string Name, int Age);
来源：http://yn.hnjuh.cn

[G15] 枚举
来源：http://wj.panjiajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pz.asd995.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jn.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lc.haigaiapp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nu.panjiajie.cn

Java: enum Color { RED, GREEN }
来源：http://zb.newstarts.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rd.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://yd.jctech888.com.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tv.hahajie.cn

[G16] 对象转数组 / 字典
来源：http://ry.chemitech.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vt.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://ex.huixinmuqiang.cn

JS:   Object.entries(obj)
来源：http://ur.shxzukj.cn

TS:   Object.entries(obj)
来源：http://kg.nicolike.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mj.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yz.lnxyls.cn

Ruby: obj.instance_variables
来源：http://to.yuexingan06.cn

C#:   // 用反射或 System.Text.Json
来源：http://rp.szxytkj.cn

================================================================================
来源：http://fv.huixiangedu.cn

H. 异常与错误处理
来源：http://km.521024.cn

================================================================================
来源：http://ba.chemitech.net.cn

[H01] try / catch 基础
来源：http://vy.szxytkj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zo.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nw.9csxet.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kn.bjjhwx.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pr.haigaiapp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dh.huanxung.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nr.jianghongdianzi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tg.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ju.9csxet.cn

[H02] finally / ensure 收尾
来源：http://nx.muxihuayi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://nz.newstarts.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hl.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://la.gzmigu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qb.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ga.colortex.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://se.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hi.bjjhwx.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wi.shtwfgs.cn

[H03] 主动抛出异常
来源：http://hi.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://sf.shxzukj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oq.newstarts.cn

JS:   throw new Error("错误信息");
来源：http://rj.haigaiapp.cn

TS:   throw new Error("错误信息");
来源：http://ej.nszjky.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ch.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ms.hahajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hv.gzmigu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ok.asd995.cn

[H04] 自定义异常类型
来源：http://ej.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://yj.bookmarksfly.cn

PHP:  class MyError extends RuntimeException {}
来源：http://li.yuexingan06.cn

JS:   class MyError extends Error {}
来源：http://jk.shtwfgs.cn

TS:   class MyError extends Error {}
来源：http://re.shxzukj.cn

Java: class MyException extends RuntimeException {}
来源：http://ur.jianghongdianzi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fk.shtwfgs.cn

Ruby: class MyError < StandardError; end
来源：http://op.jianghongdianzi.cn

C#:   class MyException : Exception {}
来源：http://mm.szxytkj.cn

[H05] 捕获特定类型
来源：http://ma.nszjky.cn

Py:   except ValueError as e:
来源：http://yb.9csxet.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ae.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://tq.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://at.hahajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://sx.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://iv.yuntaijiaju.cn

Ruby: rescue ArgumentError => e
来源：http://nx.hahajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fj.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://on.szsharing.cn

Py:   value = d.get("k") or default
来源：http://sm.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cd.colortex.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wz.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wn.bjjhwx.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hb.huanxung.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bw.huixinmuqiang.cn

Ruby: d&.dig(:a, :b)
来源：http://my.nicolike.cn

C#:   obj?.A?.B ?? default
来源：http://ep.muxihuayi.cn

[H07] 断言
来源：http://tb.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://rd.jctech888.com.cn

PHP:  assert($x > 0);
来源：http://ka.haigaiapp.cn

JS:   console.assert(x > 0);
来源：http://xz.nszjky.cn

TS:   console.assert(x > 0);
来源：http://uq.haigaiapp.cn

Java: assert x > 0 : "必须为正";
来源：http://jn.hnjuh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ds.bookmarksfly.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vx.colortex.cn

C#:   Debug.Assert(x > 0);
来源：http://rf.hahajie.cn

[H08] 获取错误信息与堆栈
来源：http://di.jianghongdianzi.cn

Py:   str(e);  traceback.format_exc()
来源：http://se.bookmarksfly.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ro.9csxet.cn

JS:   e.message;  e.stack
来源：http://tz.jctech888.com.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://br.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hy.nszjky.cn

Go:   err.Error()
来源：http://ce.colortex.cn

Ruby: e.message;  e.backtrace
来源：http://kn.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://zo.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://vp.yuntaijiaju.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sj.shxzskj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://aj.jianghongdianzi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gc.chemitech.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ra.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://nt.hahajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lo.hnjuh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ap.haigaiapp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cr.shxzukj.cn

[H10] 资源自动释放
来源：http://kr.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dp.asd995.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lr.szxytkj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rt.asd995.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://jl.huanxung.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ji.gzmigu.cn

Go:   defer f.Close()
来源：http://iq.yuexingan06.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fl.jianghongdianzi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oz.yuntaijiaju.cn

================================================================================
来源：http://rn.asd995.cn

I. 正则表达式
来源：http://lu.jianghongdianzi.cn

================================================================================
来源：http://cb.nicolike.cn

[I01] 判断是否匹配
来源：http://zk.szsharing.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kv.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ax.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://mt.hnjuh.cn

TS:   /\d+/.test(s)
来源：http://ru.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ue.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pr.szsharing.cn

Ruby: s.match?(/\d+/)
来源：http://dp.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ro.gzmigu.cn

[I02] 提取所有匹配
来源：http://xk.9csxet.cn

Py:   re.findall(r"\d+", s)
来源：http://sy.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yw.521024.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xl.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://pt.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nz.521024.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xv.huanxung.cn

Ruby: s.scan(/\d+/)
来源：http://yi.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wm.521024.cn

[I03] 提取捕获分组
来源：http://ih.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wh.gzmigu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cd.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sx.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ef.lnxyls.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tt.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xw.bookmarksfly.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fr.chemitech.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sp.lnxyls.cn

[I04] 正则替换
来源：http://ta.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://uv.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vj.shxzskj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vn.gzmigu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jr.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://il.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hq.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://db.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wk.huanxung.cn

[I05] 按正则拆分
来源：http://od.wgjwhj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ys.nicolike.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vm.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://hw.9csxet.cn

TS:   s.split(/\s*,\s*/)
来源：http://ld.muxihuayi.cn

Java: s.split("\\s*,\\s*")
来源：http://dz.hahajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cr.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://my.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ki.9csxet.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mk.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ln.jctech888.com.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bv.huixinmuqiang.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ci.colortex.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sc.huanxung.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dl.lnxyls.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://is.hahajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qh.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sa.colortex.cn

[I07] 忽略大小写与多行模式
来源：http://jm.nszjky.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tr.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wd.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sm.huixinmuqiang.cn

TS:   /error/gim
来源：http://uz.chemitech.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nq.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tf.panjiajie.cn

Ruby: s.scan(/error/i)
来源：http://tb.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bh.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://ua.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ht.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ji.hahajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pf.huixinmuqiang.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zt.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ma.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://aq.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rw.lnxyls.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://px.hnjuh.cn

================================================================================
来源：http://in.newstarts.cn

J. 日期与时间
来源：http://rm.jianghongdianzi.cn

================================================================================
来源：http://mn.szxytkj.cn

[J01] 获取当前时间
来源：http://ue.szxytkj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mm.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ja.9csxet.cn

JS:   new Date();  Date.now()
来源：http://go.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://ap.jianghongdianzi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fq.yuntaijiaju.cn

Go:   time.Now()
来源：http://ei.yuexingan06.cn

Ruby: Time.now
来源：http://kl.colortex.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tk.yuntaijiaju.cn

[J02] 格式化输出
来源：http://tg.jianghongdianzi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://df.yuexingan06.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wa.shtwfgs.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://et.hnjuh.cn

TS:   d.toISOString()
来源：http://db.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ax.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lr.colortex.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dv.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mr.nicolike.cn

[J03] 字符串解析为日期
来源：http://dd.asd995.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qc.hahajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dx.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://gm.shxzskj.cn

TS:   new Date("2024-01-02")
来源：http://oq.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qb.jctech888.com.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ud.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://vv.szsharing.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hr.shxzskj.cn

[J04] 时间戳与日期互转
来源：http://iq.szxytkj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lr.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yk.huanxung.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mb.shxzukj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cn.hnjuh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://aw.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ut.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zo.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://or.newstarts.cn

[J05] 时间加减（加 7 天）
来源：http://lt.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://gf.colortex.cn


<!-- 参考信息 -->