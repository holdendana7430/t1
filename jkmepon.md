代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://xt.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://mw.panjiajie.cn

C#:   public static void F() {}
来源：http://ig.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://in.jctech888.com.cn

Py:   from abc import ABC, abstractmethod
来源：http://jf.bookmarksfly.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jv.nszjky.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qn.bookmarksfly.cn

TS:   interface Shape { area(): number; }
来源：http://xs.muxihuayi.cn

Java: interface Shape { double area(); }
来源：http://ne.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://jk.szxytkj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lm.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://fl.nicolike.cn

[G10] 访问控制
来源：http://pf.jianghongdianzi.cn

Py:   约定 _protected / __private（不强制）
来源：http://sy.wgjwhj.cn

PHP:  public / protected / private
来源：http://vj.shxzskj.cn

JS:   #private 字段；其余公开
来源：http://in.haigaiapp.cn

TS:   public / protected / private
来源：http://km.huixiangedu.cn

Java: public / protected / private / 默认包级
来源：http://be.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sp.shxzukj.cn

Ruby: public / protected / private
来源：http://aa.panjiajie.cn

C#:   public / protected / private / internal
来源：http://ut.521024.cn

[G11] getter / setter
来源：http://lb.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://rq.panjiajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://kf.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://sk.yuntaijiaju.cn

TS:   get name(): string { return this._name; }
来源：http://di.9csxet.cn

Java: public String getName() { return name; }
来源：http://xr.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ca.lnxyls.cn

Ruby: attr_accessor :name
来源：http://uh.521024.cn

C#:   public string Name { get; set; }
来源：http://gm.shxzskj.cn

[G12] 对象转字符串
来源：http://md.shxzukj.cn

Py:   def __str__(self): return self.name
来源：http://fa.hahajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://nr.haigaiapp.cn

JS:   toString() { return this.name; }
来源：http://cp.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://uk.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://lg.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vx.jianghongdianzi.cn

Ruby: def to_s; @name; end
来源：http://vh.jianghongdianzi.cn

C#:   public override string ToString() => Name;
来源：http://ek.shtwfgs.cn

[G13] 判断对象类型
来源：http://cb.muxihuayi.cn

Py:   isinstance(u, User)
来源：http://mm.bookmarksfly.cn

PHP:  $u instanceof User
来源：http://jv.521024.cn

JS:   u instanceof User
来源：http://lm.asd995.cn

TS:   u instanceof User
来源：http://vv.521024.cn

Java: u instanceof User
来源：http://xa.521024.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nd.newstarts.cn

Ruby: u.is_a?(User)
来源：http://xc.hnjuh.cn

C#:   u is User
来源：http://yt.muxihuayi.cn

[G14] 数据类 / record
来源：http://oj.hahajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lh.chemitech.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://xc.yuntaijiaju.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vv.szxytkj.cn

TS:   type User = { name: string; age: number };
来源：http://my.shxzskj.cn

Java: record User(String name, int age) {}
来源：http://ms.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://ss.shtwfgs.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hr.huixinmuqiang.cn

C#:   record User(string Name, int Age);
来源：http://zs.newstarts.cn

[G15] 枚举
来源：http://ve.newstarts.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zl.jianghongdianzi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jl.wgjwhj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zm.gzmigu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jw.wgjwhj.cn

Java: enum Color { RED, GREEN }
来源：http://ik.chemitech.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lv.yuexingan06.cn

Ruby: Color = %i[red green].freeze
来源：http://ek.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ke.9csxet.cn

[G16] 对象转数组 / 字典
来源：http://xq.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eu.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://mk.9csxet.cn

JS:   Object.entries(obj)
来源：http://xo.haigaiapp.cn

TS:   Object.entries(obj)
来源：http://wr.yuexingan06.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qf.yuntaijiaju.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zf.nszjky.cn

Ruby: obj.instance_variables
来源：http://km.jctech888.com.cn

C#:   // 用反射或 System.Text.Json
来源：http://hq.asd995.cn

================================================================================
来源：http://cv.lnxyls.cn

H. 异常与错误处理
来源：http://jr.shxzskj.cn

================================================================================
来源：http://ce.shtwfgs.cn

[H01] try / catch 基础
来源：http://iy.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ey.huixinmuqiang.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nk.huanxung.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ef.szxytkj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://in.panjiajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uu.jctech888.com.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tg.shxzukj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ju.shtwfgs.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ba.lnxyls.cn

[H02] finally / ensure 收尾
来源：http://jg.newstarts.cn

Py:   try: f()⏎finally: cleanup()
来源：http://nv.szxytkj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gw.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://jq.hnjuh.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gy.wgjwhj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ha.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bp.huixiangedu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lg.jianghongdianzi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qa.shxzskj.cn

[H03] 主动抛出异常
来源：http://jn.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://uz.chemitech.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wv.muxihuayi.cn

JS:   throw new Error("错误信息");
来源：http://bj.colortex.cn

TS:   throw new Error("错误信息");
来源：http://ft.szxytkj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mq.wgjwhj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pb.szsharing.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hd.huixinmuqiang.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gy.shxzukj.cn

[H04] 自定义异常类型
来源：http://wz.panjiajie.cn

Py:   class MyError(Exception): pass
来源：http://lk.shtwfgs.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xo.muxihuayi.cn

JS:   class MyError extends Error {}
来源：http://ul.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://hc.chemitech.net.cn

Java: class MyException extends RuntimeException {}
来源：http://cf.hnjuh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zk.shtwfgs.cn

Ruby: class MyError < StandardError; end
来源：http://tx.huixiangedu.cn

C#:   class MyException : Exception {}
来源：http://ft.bjjhwx.cn

[H05] 捕获特定类型
来源：http://ss.yuexingan06.cn

Py:   except ValueError as e:
来源：http://il.muxihuayi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qf.yuntaijiaju.cn

JS:   if (e instanceof TypeError) {}
来源：http://or.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://ja.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://cg.jianghongdianzi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ye.asd995.cn

Ruby: rescue ArgumentError => e
来源：http://qj.bjjhwx.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tc.chemitech.net.cn

[H06] 可选值 / 空值安全访问
来源：http://kq.chemitech.net.cn

Py:   value = d.get("k") or default
来源：http://by.huixinmuqiang.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xm.shtwfgs.cn

JS:   obj?.a?.b;  d ?? default
来源：http://md.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ci.szxytkj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cx.hnjuh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nx.haigaiapp.cn

Ruby: d&.dig(:a, :b)
来源：http://qd.muxihuayi.cn

C#:   obj?.A?.B ?? default
来源：http://og.huixiangedu.cn

[H07] 断言
来源：http://cy.gzmigu.cn

Py:   assert x > 0, "必须为正"
来源：http://io.shtwfgs.cn

PHP:  assert($x > 0);
来源：http://cy.colortex.cn

JS:   console.assert(x > 0);
来源：http://ls.szxytkj.cn

TS:   console.assert(x > 0);
来源：http://xv.lnxyls.cn

Java: assert x > 0 : "必须为正";
来源：http://nb.chemitech.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gu.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ss.haigaiapp.cn

C#:   Debug.Assert(x > 0);
来源：http://hw.haigaiapp.cn

[H08] 获取错误信息与堆栈
来源：http://oq.nszjky.cn

Py:   str(e);  traceback.format_exc()
来源：http://vb.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tk.hahajie.cn

JS:   e.message;  e.stack
来源：http://su.szxytkj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hs.shtwfgs.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mn.nszjky.cn

Go:   err.Error()
来源：http://ei.shxzukj.cn

Ruby: e.message;  e.backtrace
来源：http://hi.newstarts.cn

C#:   e.Message;  e.StackTrace
来源：http://nb.huanxung.cn

[H09] 带错误码的异常
来源：http://tv.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ie.huixinmuqiang.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ut.shxzukj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rf.jianghongdianzi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hw.nicolike.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qp.hnjuh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jz.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xp.huanxung.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pm.huixiangedu.cn

[H10] 资源自动释放
来源：http://ya.nszjky.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vy.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hf.haigaiapp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kc.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://il.9csxet.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wv.panjiajie.cn

Go:   defer f.Close()
来源：http://uh.nszjky.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://za.hahajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rr.haigaiapp.cn

================================================================================
来源：http://zm.nicolike.cn

I. 正则表达式
来源：http://la.hahajie.cn

================================================================================
来源：http://ly.haigaiapp.cn

[I01] 判断是否匹配
来源：http://rc.shxzskj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ak.hnjuh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oi.newstarts.cn

JS:   /\d+/.test(s)
来源：http://bo.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://bj.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sg.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://qc.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://cs.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hx.bookmarksfly.cn

[I02] 提取所有匹配
来源：http://uu.wgjwhj.cn

Py:   re.findall(r"\d+", s)
来源：http://yx.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ho.bjjhwx.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wc.gzmigu.cn

TS:   s.match(/\d+/g)
来源：http://kj.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jb.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fu.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://aq.jianghongdianzi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://an.haigaiapp.cn

[I03] 提取捕获分组
来源：http://dj.jianghongdianzi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iz.hnjuh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zh.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ct.521024.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://fy.haigaiapp.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ec.nszjky.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rp.huanxung.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pm.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qi.haigaiapp.cn

[I04] 正则替换
来源：http://yy.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://me.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ft.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qi.yuntaijiaju.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xe.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kk.jianghongdianzi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cv.521024.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xu.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://br.colortex.cn

[I05] 按正则拆分
来源：http://dk.nszjky.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mp.colortex.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lf.bookmarksfly.cn

JS:   s.split(/\s*,\s*/)
来源：http://ha.panjiajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://ef.huanxung.cn

Java: s.split("\\s*,\\s*")
来源：http://dn.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hy.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pu.bookmarksfly.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cm.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vs.szsharing.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mu.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ev.gzmigu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jl.jctech888.com.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ab.huixiangedu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bj.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cr.muxihuayi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cg.hnjuh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ih.haigaiapp.cn

[I07] 忽略大小写与多行模式
来源：http://sd.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yz.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vu.chemitech.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jz.huixinmuqiang.cn

TS:   /error/gim
来源：http://va.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kr.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dl.521024.cn

Ruby: s.scan(/error/i)
来源：http://wv.nicolike.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qm.wgjwhj.cn

[I08] 贪婪与非贪婪匹配
来源：http://cu.chemitech.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://un.hnjuh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ul.shxzskj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fy.nicolike.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://kp.shtwfgs.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://he.521024.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cm.newstarts.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fc.panjiajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://po.huixinmuqiang.cn

================================================================================
来源：http://ri.shxzskj.cn

J. 日期与时间
来源：http://wp.szsharing.cn

================================================================================
来源：http://nc.wgjwhj.cn

[J01] 获取当前时间
来源：http://fi.521024.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://oh.jctech888.com.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hr.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://th.bookmarksfly.cn

TS:   new Date();  Date.now()
来源：http://ec.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jv.jianghongdianzi.cn

Go:   time.Now()
来源：http://zu.shxzukj.cn

Ruby: Time.now
来源：http://bj.newstarts.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gx.shxzukj.cn

[J02] 格式化输出
来源：http://ed.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fv.gzmigu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kp.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cg.shxzukj.cn

TS:   d.toISOString()
来源：http://kb.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://em.szxytkj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ub.521024.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yf.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vs.hnjuh.cn

[J03] 字符串解析为日期
来源：http://le.muxihuayi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dl.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zt.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://dg.colortex.cn

TS:   new Date("2024-01-02")
来源：http://py.jianghongdianzi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qy.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://af.huixinmuqiang.cn

Ruby: Date.parse("2024-01-02")
来源：http://ze.szsharing.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vb.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://jh.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://tl.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mn.jctech888.com.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://dt.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ug.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pj.nszjky.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ve.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wy.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://po.521024.cn

[J05] 时间加减（加 7 天）
来源：http://yz.bjjhwx.cn

Py:   now + timedelta(days=7)
来源：http://un.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wi.nszjky.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ac.jianghongdianzi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ly.jianghongdianzi.cn

Java: LocalDate.now().plusDays(7)
来源：http://kg.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mt.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://kd.panjiajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ub.gzmigu.cn

[J06] 计算两时间之差
来源：http://fl.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://cx.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://wm.shxzskj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nm.nicolike.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wb.shtwfgs.cn

Java: Duration.between(start, end).toSeconds()
来源：http://tf.yuexingan06.cn

Go:   end.Sub(start).Hours()
来源：http://ez.bookmarksfly.cn

Ruby: end - start                 # 返回秒数
来源：http://ea.lnxyls.cn

C#:   (end - start).TotalSeconds
来源：http://xg.521024.cn


<!-- 参考信息 -->