代发 wailian999

Ruby: super
来源：http://mj.jianghongdianzi.cn

C#:   base.Greet();
来源：http://sn.jctech888.com.cn

[G08] 静态方法与属性
来源：http://rq.wgjwhj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wo.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://wi.szxytkj.cn

JS:   static f() {}
来源：http://dw.shtwfgs.cn

TS:   static f(): void {}
来源：http://bx.colortex.cn

Java: static void f() {}
来源：http://dt.nicolike.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kk.lnxyls.cn

Ruby: def self.f; end
来源：http://of.muxihuayi.cn

C#:   public static void F() {}
来源：http://pu.panjiajie.cn

[G09] 接口 / 抽象类
来源：http://oj.newstarts.cn

Py:   from abc import ABC, abstractmethod
来源：http://cz.jctech888.com.cn

PHP:  interface Shape { public function area(): float; }
来源：http://um.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://oq.9csxet.cn

TS:   interface Shape { area(): number; }
来源：http://zi.jctech888.com.cn

Java: interface Shape { double area(); }
来源：http://pd.shxzukj.cn

Go:   type Shape interface { Area() float64 }
来源：http://qn.521024.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pn.521024.cn

C#:   interface IShape { double Area(); }
来源：http://gv.chemitech.net.cn

[G10] 访问控制
来源：http://ty.hnjuh.cn

Py:   约定 _protected / __private（不强制）
来源：http://za.chemitech.net.cn

PHP:  public / protected / private
来源：http://hc.chemitech.net.cn

JS:   #private 字段；其余公开
来源：http://xm.gzmigu.cn

TS:   public / protected / private
来源：http://ar.bjjhwx.cn

Java: public / protected / private / 默认包级
来源：http://vy.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sq.gzmigu.cn

Ruby: public / protected / private
来源：http://vv.shxzukj.cn

C#:   public / protected / private / internal
来源：http://va.shtwfgs.cn

[G11] getter / setter
来源：http://ec.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://gw.chemitech.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ip.szsharing.cn

JS:   get name() { return this._name; }
来源：http://sz.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://li.jianghongdianzi.cn

Java: public String getName() { return name; }
来源：http://yn.newstarts.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yp.shxzukj.cn

Ruby: attr_accessor :name
来源：http://av.chemitech.net.cn

C#:   public string Name { get; set; }
来源：http://kq.newstarts.cn

[G12] 对象转字符串
来源：http://ok.shxzskj.cn

Py:   def __str__(self): return self.name
来源：http://ec.chemitech.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://no.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://mm.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://wq.hnjuh.cn

Java: @Override public String toString() { return name; }
来源：http://ja.huixinmuqiang.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lm.shxzukj.cn

Ruby: def to_s; @name; end
来源：http://og.jctech888.com.cn

C#:   public override string ToString() => Name;
来源：http://rx.shtwfgs.cn

[G13] 判断对象类型
来源：http://xc.shtwfgs.cn

Py:   isinstance(u, User)
来源：http://vy.hnjuh.cn

PHP:  $u instanceof User
来源：http://jk.asd995.cn

JS:   u instanceof User
来源：http://lv.colortex.cn

TS:   u instanceof User
来源：http://ku.asd995.cn

Java: u instanceof User
来源：http://by.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ov.nicolike.cn

Ruby: u.is_a?(User)
来源：http://bh.lnxyls.cn

C#:   u is User
来源：http://fh.shxzskj.cn

[G14] 数据类 / record
来源：http://ua.bjjhwx.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xa.muxihuayi.cn

PHP:  // 用 readonly 属性模拟
来源：http://zy.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vs.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://xc.lnxyls.cn

Java: record User(String name, int age) {}
来源：http://wv.muxihuayi.cn

Go:   type User struct { Name string; Age int }
来源：http://gh.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://os.szxytkj.cn

C#:   record User(string Name, int Age);
来源：http://rt.huixinmuqiang.cn

[G15] 枚举
来源：http://ns.hnjuh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qh.shtwfgs.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qi.yuexingan06.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dp.bookmarksfly.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ni.haigaiapp.cn

Java: enum Color { RED, GREEN }
来源：http://hz.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kj.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://ye.jctech888.com.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fe.asd995.cn

[G16] 对象转数组 / 字典
来源：http://ul.huixiangedu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gc.yuexingan06.cn

PHP:  get_object_vars($obj);
来源：http://tk.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://wv.colortex.cn

TS:   Object.entries(obj)
来源：http://ib.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://id.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zv.bookmarksfly.cn

Ruby: obj.instance_variables
来源：http://ug.huixinmuqiang.cn

C#:   // 用反射或 System.Text.Json
来源：http://wr.shtwfgs.cn

================================================================================
来源：http://vx.muxihuayi.cn

H. 异常与错误处理
来源：http://cy.nicolike.cn

================================================================================
来源：http://zr.panjiajie.cn

[H01] try / catch 基础
来源：http://lp.jianghongdianzi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://il.asd995.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://aj.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xt.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://or.yuexingan06.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wh.huanxung.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gz.chemitech.net.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mr.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dw.nicolike.cn

[H02] finally / ensure 收尾
来源：http://ec.nszjky.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ky.shtwfgs.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ww.huanxung.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gr.yuexingan06.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fl.9csxet.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wy.yuexingan06.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jw.newstarts.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mf.huanxung.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yl.newstarts.cn

[H03] 主动抛出异常
来源：http://bg.chemitech.net.cn

Py:   raise ValueError("错误信息")
来源：http://na.hnjuh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gu.asd995.cn

JS:   throw new Error("错误信息");
来源：http://ri.szxytkj.cn

TS:   throw new Error("错误信息");
来源：http://nx.szsharing.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ox.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cn.szxytkj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cu.hahajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ut.newstarts.cn

[H04] 自定义异常类型
来源：http://ny.521024.cn

Py:   class MyError(Exception): pass
来源：http://pd.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sd.nszjky.cn

JS:   class MyError extends Error {}
来源：http://pb.shtwfgs.cn

TS:   class MyError extends Error {}
来源：http://vc.bookmarksfly.cn

Java: class MyException extends RuntimeException {}
来源：http://dm.yuntaijiaju.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mv.haigaiapp.cn

Ruby: class MyError < StandardError; end
来源：http://in.shxzukj.cn

C#:   class MyException : Exception {}
来源：http://eu.nicolike.cn

[H05] 捕获特定类型
来源：http://hu.colortex.cn

Py:   except ValueError as e:
来源：http://zj.bjjhwx.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xn.hahajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://hy.521024.cn

TS:   if (e instanceof TypeError) {}
来源：http://ci.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://qj.huanxung.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pi.muxihuayi.cn

Ruby: rescue ArgumentError => e
来源：http://nb.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kg.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://ae.chemitech.net.cn

Py:   value = d.get("k") or default
来源：http://cs.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://in.lnxyls.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kj.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rz.yuexingan06.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tg.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cm.huixinmuqiang.cn

Ruby: d&.dig(:a, :b)
来源：http://bs.nszjky.cn

C#:   obj?.A?.B ?? default
来源：http://bi.gzmigu.cn

[H07] 断言
来源：http://xm.nszjky.cn

Py:   assert x > 0, "必须为正"
来源：http://ns.hnjuh.cn

PHP:  assert($x > 0);
来源：http://tw.haigaiapp.cn

JS:   console.assert(x > 0);
来源：http://rw.colortex.cn

TS:   console.assert(x > 0);
来源：http://wu.panjiajie.cn

Java: assert x > 0 : "必须为正";
来源：http://ff.lnxyls.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yz.shxzskj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xz.521024.cn

C#:   Debug.Assert(x > 0);
来源：http://pm.haigaiapp.cn

[H08] 获取错误信息与堆栈
来源：http://vs.lnxyls.cn

Py:   str(e);  traceback.format_exc()
来源：http://ay.wgjwhj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lp.jctech888.com.cn

JS:   e.message;  e.stack
来源：http://vm.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rk.hnjuh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wa.colortex.cn

Go:   err.Error()
来源：http://jq.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://wx.nszjky.cn

C#:   e.Message;  e.StackTrace
来源：http://kh.shxzskj.cn

[H09] 带错误码的异常
来源：http://xg.szsharing.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lb.haigaiapp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://vc.yuexingan06.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://no.asd995.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://el.shxzukj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://in.huanxung.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tv.huanxung.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dn.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://eg.szsharing.cn

[H10] 资源自动释放
来源：http://xb.lnxyls.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ep.huixiangedu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zj.huanxung.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wa.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pf.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://no.asd995.cn

Go:   defer f.Close()
来源：http://eq.newstarts.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fe.bookmarksfly.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fx.shtwfgs.cn

================================================================================
来源：http://ib.huixinmuqiang.cn

I. 正则表达式
来源：http://ej.nicolike.cn

================================================================================
来源：http://eu.newstarts.cn

[I01] 判断是否匹配
来源：http://lv.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rp.newstarts.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tc.521024.cn

JS:   /\d+/.test(s)
来源：http://bz.yuntaijiaju.cn

TS:   /\d+/.test(s)
来源：http://gp.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://af.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://iq.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://lt.muxihuayi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mq.shxzskj.cn

[I02] 提取所有匹配
来源：http://hz.jianghongdianzi.cn

Py:   re.findall(r"\d+", s)
来源：http://am.yuntaijiaju.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ri.yuntaijiaju.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ba.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://xu.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cd.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dz.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://tw.huixiangedu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://up.jctech888.com.cn

[I03] 提取捕获分组
来源：http://pk.chemitech.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vp.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yz.bookmarksfly.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yb.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lx.szsharing.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kz.szsharing.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ik.panjiajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bg.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mb.yuntaijiaju.cn

[I04] 正则替换
来源：http://ss.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nk.szxytkj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ih.newstarts.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ou.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ba.lnxyls.cn

Java: s.replaceAll("\\d+", "#")
来源：http://uj.szsharing.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pr.haigaiapp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://eb.shxzukj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lp.bookmarksfly.cn

[I05] 按正则拆分
来源：http://qn.bookmarksfly.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yq.huixinmuqiang.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nr.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://db.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://pf.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://qt.szsharing.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yz.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zp.shxzukj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lq.szsharing.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hl.muxihuayi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nu.asd995.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ev.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xq.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://go.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mw.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lm.521024.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ft.hahajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sm.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://hm.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wz.huanxung.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cj.shxzskj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pt.shxzskj.cn

TS:   /error/gim
来源：http://ll.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://gf.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fl.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://rh.newstarts.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wy.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://sj.muxihuayi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gg.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ye.colortex.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sa.panjiajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hq.yuexingan06.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zq.panjiajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sa.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bg.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wy.asd995.cn

================================================================================
来源：http://xs.huixiangedu.cn

J. 日期与时间
来源：http://ia.gzmigu.cn

================================================================================
来源：http://op.9csxet.cn

[J01] 获取当前时间
来源：http://ez.szsharing.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qj.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ep.wgjwhj.cn

JS:   new Date();  Date.now()
来源：http://wc.bookmarksfly.cn

TS:   new Date();  Date.now()
来源：http://wc.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://au.yuexingan06.cn

Go:   time.Now()
来源：http://jc.panjiajie.cn

Ruby: Time.now
来源：http://ts.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ev.521024.cn

[J02] 格式化输出
来源：http://mc.colortex.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ly.huixinmuqiang.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dw.huixinmuqiang.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jx.lnxyls.cn

TS:   d.toISOString()
来源：http://ui.hahajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dp.521024.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://up.shxzukj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mx.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://aq.szxytkj.cn

[J03] 字符串解析为日期
来源：http://fk.nicolike.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jx.shxzskj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ij.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://yn.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://za.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fx.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tc.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://ww.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ib.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://fj.huixinmuqiang.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sh.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tr.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fj.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sk.haigaiapp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cn.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://kr.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yt.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kg.yuexingan06.cn

[J05] 时间加减（加 7 天）
来源：http://sb.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://mj.huixiangedu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://aw.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://as.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://io.colortex.cn

Java: LocalDate.now().plusDays(7)
来源：http://yb.jianghongdianzi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dc.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://mg.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bz.szsharing.cn

[J06] 计算两时间之差
来源：http://yy.jianghongdianzi.cn


<!-- 参考信息 -->