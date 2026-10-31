代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://ym.nicolike.cn

Java: @Override String greet() { return "admin"; }
来源：http://xw.haigaiapp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rw.jianghongdianzi.cn

Ruby: def greet; "admin"; end
来源：http://sv.yuexingan06.cn

C#:   public override string Greet() => "admin";
来源：http://yk.bookmarksfly.cn

[G07] 调用父类方法
来源：http://ie.521024.cn

Py:   super().greet()
来源：http://jn.szxytkj.cn

PHP:  parent::greet();
来源：http://kc.szxytkj.cn

JS:   super.greet();
来源：http://le.jianghongdianzi.cn

TS:   super.greet();
来源：http://ud.jctech888.com.cn

Java: super.greet();
来源：http://rv.szxytkj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pr.hnjuh.cn

Ruby: super
来源：http://yj.bjjhwx.cn

C#:   base.Greet();
来源：http://as.9csxet.cn

[G08] 静态方法与属性
来源：http://ga.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eq.yuntaijiaju.cn

PHP:  public static function f() {}
来源：http://ji.lnxyls.cn

JS:   static f() {}
来源：http://zf.haigaiapp.cn

TS:   static f(): void {}
来源：http://ri.hahajie.cn

Java: static void f() {}
来源：http://yz.muxihuayi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://dy.hnjuh.cn

Ruby: def self.f; end
来源：http://qd.asd995.cn

C#:   public static void F() {}
来源：http://jc.yuexingan06.cn

[G09] 接口 / 抽象类
来源：http://ig.wgjwhj.cn

Py:   from abc import ABC, abstractmethod
来源：http://kd.huixiangedu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ee.lnxyls.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://td.shxzukj.cn

TS:   interface Shape { area(): number; }
来源：http://vb.szxytkj.cn

Java: interface Shape { double area(); }
来源：http://of.521024.cn

Go:   type Shape interface { Area() float64 }
来源：http://ac.szsharing.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oi.huanxung.cn

C#:   interface IShape { double Area(); }
来源：http://gq.huixiangedu.cn

[G10] 访问控制
来源：http://ts.gzmigu.cn

Py:   约定 _protected / __private（不强制）
来源：http://ho.newstarts.cn

PHP:  public / protected / private
来源：http://bv.huixiangedu.cn

JS:   #private 字段；其余公开
来源：http://pv.szxytkj.cn

TS:   public / protected / private
来源：http://wp.bjjhwx.cn

Java: public / protected / private / 默认包级
来源：http://wi.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xi.gzmigu.cn

Ruby: public / protected / private
来源：http://pi.hahajie.cn

C#:   public / protected / private / internal
来源：http://mj.gzmigu.cn

[G11] getter / setter
来源：http://ex.521024.cn

Py:   @property 与 @x.setter
来源：http://ah.nicolike.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dx.jianghongdianzi.cn

JS:   get name() { return this._name; }
来源：http://lu.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://bo.huanxung.cn

Java: public String getName() { return name; }
来源：http://dl.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hn.asd995.cn

Ruby: attr_accessor :name
来源：http://ay.lnxyls.cn

C#:   public string Name { get; set; }
来源：http://fs.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://qe.gzmigu.cn

Py:   def __str__(self): return self.name
来源：http://kf.wgjwhj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rq.bookmarksfly.cn

JS:   toString() { return this.name; }
来源：http://zz.newstarts.cn

TS:   toString(): string { return this.name; }
来源：http://ez.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://fr.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hw.jctech888.com.cn

Ruby: def to_s; @name; end
来源：http://cp.shtwfgs.cn

C#:   public override string ToString() => Name;
来源：http://pa.nicolike.cn

[G13] 判断对象类型
来源：http://ps.nszjky.cn

Py:   isinstance(u, User)
来源：http://st.huixiangedu.cn

PHP:  $u instanceof User
来源：http://yk.muxihuayi.cn

JS:   u instanceof User
来源：http://cl.huixiangedu.cn

TS:   u instanceof User
来源：http://tl.asd995.cn

Java: u instanceof User
来源：http://yi.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qc.hahajie.cn

Ruby: u.is_a?(User)
来源：http://qv.newstarts.cn

C#:   u is User
来源：http://xl.huixiangedu.cn

[G14] 数据类 / record
来源：http://ec.nszjky.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sn.haigaiapp.cn

PHP:  // 用 readonly 属性模拟
来源：http://rz.nszjky.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tw.wgjwhj.cn

TS:   type User = { name: string; age: number };
来源：http://np.muxihuayi.cn

Java: record User(String name, int age) {}
来源：http://az.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://gp.shtwfgs.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cs.asd995.cn

C#:   record User(string Name, int Age);
来源：http://zd.huixiangedu.cn

[G15] 枚举
来源：http://cj.muxihuayi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bo.shxzukj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nr.wgjwhj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ax.shxzskj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rm.huixinmuqiang.cn

Java: enum Color { RED, GREEN }
来源：http://ac.521024.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ww.shxzukj.cn

Ruby: Color = %i[red green].freeze
来源：http://kd.newstarts.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ts.haigaiapp.cn

[G16] 对象转数组 / 字典
来源：http://qg.bookmarksfly.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hc.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://lv.asd995.cn

JS:   Object.entries(obj)
来源：http://un.jctech888.com.cn

TS:   Object.entries(obj)
来源：http://zk.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bv.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mi.asd995.cn

Ruby: obj.instance_variables
来源：http://qk.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://rv.muxihuayi.cn

================================================================================
来源：http://vh.shxzukj.cn

H. 异常与错误处理
来源：http://tm.yuntaijiaju.cn

================================================================================
来源：http://ha.shtwfgs.cn

[H01] try / catch 基础
来源：http://rl.nszjky.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vd.muxihuayi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jy.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vx.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jz.9csxet.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jt.bookmarksfly.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://in.yuntaijiaju.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qp.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rz.bookmarksfly.cn

[H02] finally / ensure 收尾
来源：http://ln.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jd.nicolike.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://uc.jctech888.com.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://fr.shxzskj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jc.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gq.szxytkj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lo.bjjhwx.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xt.huixinmuqiang.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qv.bjjhwx.cn

[H03] 主动抛出异常
来源：http://in.huixiangedu.cn

Py:   raise ValueError("错误信息")
来源：http://gx.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://og.szxytkj.cn

JS:   throw new Error("错误信息");
来源：http://gu.521024.cn

TS:   throw new Error("错误信息");
来源：http://be.jctech888.com.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ze.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://eg.bjjhwx.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ou.521024.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yq.szsharing.cn

[H04] 自定义异常类型
来源：http://pc.jctech888.com.cn

Py:   class MyError(Exception): pass
来源：http://qy.hnjuh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ll.colortex.cn

JS:   class MyError extends Error {}
来源：http://nh.shtwfgs.cn

TS:   class MyError extends Error {}
来源：http://fy.gzmigu.cn

Java: class MyException extends RuntimeException {}
来源：http://qc.chemitech.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ib.shxzskj.cn

Ruby: class MyError < StandardError; end
来源：http://ug.szxytkj.cn

C#:   class MyException : Exception {}
来源：http://ld.yuexingan06.cn

[H05] 捕获特定类型
来源：http://nd.szsharing.cn

Py:   except ValueError as e:
来源：http://hy.yuexingan06.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ho.yuntaijiaju.cn

JS:   if (e instanceof TypeError) {}
来源：http://tv.nszjky.cn

TS:   if (e instanceof TypeError) {}
来源：http://ge.newstarts.cn

Java: catch (IOException | SQLException e) {}
来源：http://te.9csxet.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mo.huixinmuqiang.cn

Ruby: rescue ArgumentError => e
来源：http://ou.yuntaijiaju.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://lt.nicolike.cn

[H06] 可选值 / 空值安全访问
来源：http://tl.jctech888.com.cn

Py:   value = d.get("k") or default
来源：http://tk.hnjuh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vi.hahajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pd.panjiajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://de.nszjky.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jm.asd995.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ht.chemitech.net.cn

Ruby: d&.dig(:a, :b)
来源：http://pp.nicolike.cn

C#:   obj?.A?.B ?? default
来源：http://fg.huanxung.cn

[H07] 断言
来源：http://sv.szsharing.cn

Py:   assert x > 0, "必须为正"
来源：http://hf.colortex.cn

PHP:  assert($x > 0);
来源：http://yj.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://ac.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://ow.yuexingan06.cn

Java: assert x > 0 : "必须为正";
来源：http://tn.gzmigu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ef.bjjhwx.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zj.muxihuayi.cn

C#:   Debug.Assert(x > 0);
来源：http://kz.huixinmuqiang.cn

[H08] 获取错误信息与堆栈
来源：http://mf.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://qe.huanxung.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hi.lnxyls.cn

JS:   e.message;  e.stack
来源：http://wm.shxzskj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://to.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tk.jctech888.com.cn

Go:   err.Error()
来源：http://id.hahajie.cn

Ruby: e.message;  e.backtrace
来源：http://tz.huixiangedu.cn

C#:   e.Message;  e.StackTrace
来源：http://ma.szxytkj.cn

[H09] 带错误码的异常
来源：http://ud.nszjky.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nm.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://uw.huixiangedu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ey.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ns.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fg.nicolike.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xa.huixinmuqiang.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yy.jctech888.com.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gi.colortex.cn

[H10] 资源自动释放
来源：http://je.shtwfgs.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sy.9csxet.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dh.jianghongdianzi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://su.jianghongdianzi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ou.huixinmuqiang.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ai.huanxung.cn

Go:   defer f.Close()
来源：http://ca.hnjuh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tp.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cb.huixiangedu.cn

================================================================================
来源：http://pz.yuntaijiaju.cn

I. 正则表达式
来源：http://qo.bjjhwx.cn

================================================================================
来源：http://ev.panjiajie.cn

[I01] 判断是否匹配
来源：http://jk.shtwfgs.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fn.haigaiapp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vl.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://db.hnjuh.cn

TS:   /\d+/.test(s)
来源：http://da.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kk.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mq.gzmigu.cn

Ruby: s.match?(/\d+/)
来源：http://ij.panjiajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qp.muxihuayi.cn

[I02] 提取所有匹配
来源：http://cf.asd995.cn

Py:   re.findall(r"\d+", s)
来源：http://is.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yx.panjiajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ln.nicolike.cn

TS:   s.match(/\d+/g)
来源：http://xk.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ki.nszjky.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://po.shxzskj.cn

Ruby: s.scan(/\d+/)
来源：http://ri.huixiangedu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sj.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://fx.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bc.yuexingan06.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qh.asd995.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ux.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tp.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kb.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ml.newstarts.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://rj.jctech888.com.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jo.hnjuh.cn

[I04] 正则替换
来源：http://di.bjjhwx.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://oq.hnjuh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tq.haigaiapp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mc.yuntaijiaju.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rr.yuntaijiaju.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hc.colortex.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ad.szsharing.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xi.shxzukj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xg.521024.cn

[I05] 按正则拆分
来源：http://eb.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lt.colortex.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lj.shxzskj.cn

JS:   s.split(/\s*,\s*/)
来源：http://tm.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://km.shxzukj.cn

Java: s.split("\\s*,\\s*")
来源：http://yb.szsharing.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bs.newstarts.cn

Ruby: s.split(/\s*,\s*/)
来源：http://il.yuntaijiaju.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ps.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bx.muxihuayi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ex.panjiajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sg.nicolike.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ht.jctech888.com.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sh.asd995.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nb.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oi.haigaiapp.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xl.colortex.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sm.bookmarksfly.cn

[I07] 忽略大小写与多行模式
来源：http://in.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hs.colortex.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sz.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rb.newstarts.cn

TS:   /error/gim
来源：http://bf.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ap.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gh.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://ry.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://re.nicolike.cn

[I08] 贪婪与非贪婪匹配
来源：http://bd.lnxyls.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qp.gzmigu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jo.hnjuh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://rz.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sq.lnxyls.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cw.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ot.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ov.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hd.yuntaijiaju.cn

================================================================================
来源：http://oc.huanxung.cn

J. 日期与时间
来源：http://yb.szxytkj.cn

================================================================================
来源：http://ke.haigaiapp.cn

[J01] 获取当前时间
来源：http://kq.haigaiapp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://av.szxytkj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://na.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://zc.newstarts.cn

TS:   new Date();  Date.now()
来源：http://hu.newstarts.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ek.9csxet.cn

Go:   time.Now()
来源：http://vl.wgjwhj.cn

Ruby: Time.now
来源：http://rs.asd995.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fm.jianghongdianzi.cn

[J02] 格式化输出
来源：http://hh.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hc.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://we.shxzskj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vt.nicolike.cn

TS:   d.toISOString()
来源：http://cd.jianghongdianzi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mb.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nn.hahajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hl.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cn.huanxung.cn

[J03] 字符串解析为日期
来源：http://do.newstarts.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ip.jianghongdianzi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wi.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://if.shtwfgs.cn

TS:   new Date("2024-01-02")
来源：http://fj.szsharing.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ub.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wq.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://mp.nicolike.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ib.wgjwhj.cn

[J04] 时间戳与日期互转
来源：http://ph.huixinmuqiang.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://eg.wgjwhj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wt.nszjky.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zg.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ul.hahajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nx.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fo.hnjuh.cn


<!-- 参考信息 -->