代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://nv.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://uu.521024.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ur.shtwfgs.cn

Ruby: def greet; "admin"; end
来源：http://ju.huanxung.cn

C#:   public override string Greet() => "admin";
来源：http://mn.jianghongdianzi.cn

[G07] 调用父类方法
来源：http://lj.shxzukj.cn

Py:   super().greet()
来源：http://gv.newstarts.cn

PHP:  parent::greet();
来源：http://ia.nicolike.cn

JS:   super.greet();
来源：http://gf.gzmigu.cn

TS:   super.greet();
来源：http://te.jianghongdianzi.cn

Java: super.greet();
来源：http://my.bookmarksfly.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tw.521024.cn

Ruby: super
来源：http://kl.haigaiapp.cn

C#:   base.Greet();
来源：http://tm.szxytkj.cn

[G08] 静态方法与属性
来源：http://pp.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hl.shtwfgs.cn

PHP:  public static function f() {}
来源：http://oh.huanxung.cn

JS:   static f() {}
来源：http://zi.muxihuayi.cn

TS:   static f(): void {}
来源：http://gl.hnjuh.cn

Java: static void f() {}
来源：http://fm.shtwfgs.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://rm.muxihuayi.cn

Ruby: def self.f; end
来源：http://pv.huixinmuqiang.cn

C#:   public static void F() {}
来源：http://dm.gzmigu.cn

[G09] 接口 / 抽象类
来源：http://wh.huixinmuqiang.cn

Py:   from abc import ABC, abstractmethod
来源：http://wh.yuntaijiaju.cn

PHP:  interface Shape { public function area(): float; }
来源：http://oc.jctech888.com.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://px.huixinmuqiang.cn

TS:   interface Shape { area(): number; }
来源：http://mz.colortex.cn

Java: interface Shape { double area(); }
来源：http://mf.chemitech.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://fq.colortex.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pv.yuexingan06.cn

C#:   interface IShape { double Area(); }
来源：http://xp.shxzukj.cn

[G10] 访问控制
来源：http://lk.chemitech.net.cn

Py:   约定 _protected / __private（不强制）
来源：http://bq.521024.cn

PHP:  public / protected / private
来源：http://ib.szxytkj.cn

JS:   #private 字段；其余公开
来源：http://na.jctech888.com.cn

TS:   public / protected / private
来源：http://sz.shxzukj.cn

Java: public / protected / private / 默认包级
来源：http://kd.lnxyls.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ti.shxzskj.cn

Ruby: public / protected / private
来源：http://fu.hahajie.cn

C#:   public / protected / private / internal
来源：http://ur.gzmigu.cn

[G11] getter / setter
来源：http://za.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://st.521024.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ed.huixiangedu.cn

JS:   get name() { return this._name; }
来源：http://uq.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://up.9csxet.cn

Java: public String getName() { return name; }
来源：http://od.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qo.newstarts.cn

Ruby: attr_accessor :name
来源：http://kc.9csxet.cn

C#:   public string Name { get; set; }
来源：http://bk.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://lw.huixinmuqiang.cn

Py:   def __str__(self): return self.name
来源：http://ih.shtwfgs.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gs.colortex.cn

JS:   toString() { return this.name; }
来源：http://jl.nszjky.cn

TS:   toString(): string { return this.name; }
来源：http://kw.huixinmuqiang.cn

Java: @Override public String toString() { return name; }
来源：http://ga.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vp.yuntaijiaju.cn

Ruby: def to_s; @name; end
来源：http://ax.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://rw.yuntaijiaju.cn

[G13] 判断对象类型
来源：http://em.chemitech.net.cn

Py:   isinstance(u, User)
来源：http://zo.bookmarksfly.cn

PHP:  $u instanceof User
来源：http://kt.shtwfgs.cn

JS:   u instanceof User
来源：http://od.lnxyls.cn

TS:   u instanceof User
来源：http://go.shxzskj.cn

Java: u instanceof User
来源：http://iy.asd995.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://pm.asd995.cn

Ruby: u.is_a?(User)
来源：http://eb.shxzukj.cn

C#:   u is User
来源：http://as.shxzskj.cn

[G14] 数据类 / record
来源：http://hh.muxihuayi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://aj.nicolike.cn

PHP:  // 用 readonly 属性模拟
来源：http://hn.yuntaijiaju.cn

JS:   // 无内置：普通类或对象字面量
来源：http://eu.asd995.cn

TS:   type User = { name: string; age: number };
来源：http://tf.huanxung.cn

Java: record User(String name, int age) {}
来源：http://gz.wgjwhj.cn

Go:   type User struct { Name string; Age int }
来源：http://yr.muxihuayi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cr.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://td.huanxung.cn

[G15] 枚举
来源：http://cp.haigaiapp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nk.shxzukj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yv.huanxung.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://al.bookmarksfly.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qc.panjiajie.cn

Java: enum Color { RED, GREEN }
来源：http://my.panjiajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yf.bjjhwx.cn

Ruby: Color = %i[red green].freeze
来源：http://kg.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://do.hnjuh.cn

[G16] 对象转数组 / 字典
来源：http://pq.szxytkj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://oz.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://mw.wgjwhj.cn

JS:   Object.entries(obj)
来源：http://zl.hahajie.cn

TS:   Object.entries(obj)
来源：http://by.nszjky.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://go.colortex.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zw.chemitech.net.cn

Ruby: obj.instance_variables
来源：http://kx.gzmigu.cn

C#:   // 用反射或 System.Text.Json
来源：http://kx.gzmigu.cn

================================================================================
来源：http://zo.szsharing.cn

H. 异常与错误处理
来源：http://at.panjiajie.cn

================================================================================
来源：http://fd.bjjhwx.cn

[H01] try / catch 基础
来源：http://rd.haigaiapp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://df.huixiangedu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dd.yuexingan06.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rn.gzmigu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ck.szxytkj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rq.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lk.colortex.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yi.asd995.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gg.521024.cn

[H02] finally / ensure 收尾
来源：http://ip.yuntaijiaju.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mq.szxytkj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xa.yuexingan06.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zv.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://na.9csxet.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qe.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://id.shxzukj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hx.bjjhwx.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bu.asd995.cn

[H03] 主动抛出异常
来源：http://mk.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://ce.521024.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://it.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://yt.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://sc.szsharing.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qv.nicolike.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sp.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://sl.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vv.521024.cn

[H04] 自定义异常类型
来源：http://ui.gzmigu.cn

Py:   class MyError(Exception): pass
来源：http://nz.jianghongdianzi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ey.jianghongdianzi.cn

JS:   class MyError extends Error {}
来源：http://ex.colortex.cn

TS:   class MyError extends Error {}
来源：http://oz.szxytkj.cn

Java: class MyException extends RuntimeException {}
来源：http://dl.huixinmuqiang.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xe.bjjhwx.cn

Ruby: class MyError < StandardError; end
来源：http://jo.colortex.cn

C#:   class MyException : Exception {}
来源：http://bj.jctech888.com.cn

[H05] 捕获特定类型
来源：http://rz.colortex.cn

Py:   except ValueError as e:
来源：http://mp.szxytkj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vp.szsharing.cn

JS:   if (e instanceof TypeError) {}
来源：http://ss.panjiajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://ru.szxytkj.cn

Java: catch (IOException | SQLException e) {}
来源：http://yd.asd995.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ff.hnjuh.cn

Ruby: rescue ArgumentError => e
来源：http://ae.shxzskj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vm.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://wx.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://oe.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sk.nszjky.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ty.huanxung.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vp.521024.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gc.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vs.yuntaijiaju.cn

Ruby: d&.dig(:a, :b)
来源：http://wg.newstarts.cn

C#:   obj?.A?.B ?? default
来源：http://dp.colortex.cn

[H07] 断言
来源：http://zz.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://io.szsharing.cn

PHP:  assert($x > 0);
来源：http://sk.lnxyls.cn

JS:   console.assert(x > 0);
来源：http://do.bookmarksfly.cn

TS:   console.assert(x > 0);
来源：http://qx.szxytkj.cn

Java: assert x > 0 : "必须为正";
来源：http://pd.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://re.shxzskj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://yu.shxzskj.cn

C#:   Debug.Assert(x > 0);
来源：http://nh.haigaiapp.cn

[H08] 获取错误信息与堆栈
来源：http://xh.nszjky.cn

Py:   str(e);  traceback.format_exc()
来源：http://kf.gzmigu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nd.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://sm.szxytkj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ob.shxzskj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://sp.huanxung.cn

Go:   err.Error()
来源：http://kz.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://gt.asd995.cn

C#:   e.Message;  e.StackTrace
来源：http://bq.asd995.cn

[H09] 带错误码的异常
来源：http://bb.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gd.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ol.shxzukj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vv.panjiajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bj.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://da.lnxyls.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jh.nszjky.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vo.shtwfgs.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://if.muxihuayi.cn

[H10] 资源自动释放
来源：http://ak.muxihuayi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vb.shtwfgs.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://py.yuntaijiaju.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rt.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zt.jianghongdianzi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rz.shxzskj.cn

Go:   defer f.Close()
来源：http://dp.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yf.shxzukj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hl.521024.cn

================================================================================
来源：http://xv.nszjky.cn

I. 正则表达式
来源：http://ha.nicolike.cn

================================================================================
来源：http://ty.szsharing.cn

[I01] 判断是否匹配
来源：http://xq.gzmigu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://at.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://kj.szsharing.cn

JS:   /\d+/.test(s)
来源：http://vw.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://uw.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zj.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hd.szxytkj.cn

Ruby: s.match?(/\d+/)
来源：http://mg.newstarts.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xl.yuntaijiaju.cn

[I02] 提取所有匹配
来源：http://km.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://yi.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uq.shtwfgs.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ei.nszjky.cn

TS:   s.match(/\d+/g)
来源：http://is.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ho.nszjky.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sr.muxihuayi.cn

Ruby: s.scan(/\d+/)
来源：http://aj.hnjuh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hn.szsharing.cn

[I03] 提取捕获分组
来源：http://ru.bjjhwx.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uk.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lx.bookmarksfly.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kr.lnxyls.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vh.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jm.bjjhwx.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mq.asd995.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://at.yuntaijiaju.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hb.huixinmuqiang.cn

[I04] 正则替换
来源：http://rq.lnxyls.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hl.panjiajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hk.gzmigu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ku.huixiangedu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qw.szxytkj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yv.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dq.521024.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bs.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sr.521024.cn

[I05] 按正则拆分
来源：http://ih.521024.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://kv.huixinmuqiang.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hy.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://bc.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://la.shtwfgs.cn

Java: s.split("\\s*,\\s*")
来源：http://gr.asd995.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ve.chemitech.net.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dt.jctech888.com.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jf.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nu.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vh.gzmigu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oy.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hf.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tk.huixinmuqiang.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tq.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tn.szxytkj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lw.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://do.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://qg.nicolike.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yq.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://li.huanxung.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uy.panjiajie.cn

TS:   /error/gim
来源：http://dn.muxihuayi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xq.521024.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mk.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://wb.jianghongdianzi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kk.nicolike.cn

[I08] 贪婪与非贪婪匹配
来源：http://oc.shtwfgs.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kd.521024.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wn.gzmigu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zo.huanxung.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gx.bookmarksfly.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yu.muxihuayi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ge.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yt.yuexingan06.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ws.chemitech.net.cn

================================================================================
来源：http://xw.huixinmuqiang.cn

J. 日期与时间
来源：http://kb.hnjuh.cn

================================================================================
来源：http://ec.muxihuayi.cn

[J01] 获取当前时间
来源：http://mv.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cm.9csxet.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mx.gzmigu.cn

JS:   new Date();  Date.now()
来源：http://uh.newstarts.cn

TS:   new Date();  Date.now()
来源：http://ro.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://bf.huixiangedu.cn

Go:   time.Now()
来源：http://pp.gzmigu.cn

Ruby: Time.now
来源：http://sj.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://aa.bjjhwx.cn

[J02] 格式化输出
来源：http://ly.521024.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xn.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gz.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jl.bjjhwx.cn

TS:   d.toISOString()
来源：http://ci.asd995.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lm.shxzukj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dd.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vu.lnxyls.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://mk.colortex.cn

[J03] 字符串解析为日期
来源：http://vb.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eh.huixinmuqiang.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://az.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://ua.nicolike.cn

TS:   new Date("2024-01-02")
来源：http://oh.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fm.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ts.nicolike.cn

Ruby: Date.parse("2024-01-02")
来源：http://wl.yuntaijiaju.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://le.521024.cn

[J04] 时间戳与日期互转
来源：http://gq.huixinmuqiang.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://xo.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pi.szsharing.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wa.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cx.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://do.bjjhwx.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xa.huixiangedu.cn


<!-- 参考信息 -->