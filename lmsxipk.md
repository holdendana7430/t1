代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://ft.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://ko.asd995.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://dl.asd995.cn

Ruby: def greet; "admin"; end
来源：http://ml.panjiajie.cn

C#:   public override string Greet() => "admin";
来源：http://br.yuntaijiaju.cn

[G07] 调用父类方法
来源：http://dn.panjiajie.cn

Py:   super().greet()
来源：http://rx.gzmigu.cn

PHP:  parent::greet();
来源：http://vp.hnjuh.cn

JS:   super.greet();
来源：http://rt.bookmarksfly.cn

TS:   super.greet();
来源：http://lx.9csxet.cn

Java: super.greet();
来源：http://tu.huanxung.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://up.muxihuayi.cn

Ruby: super
来源：http://tj.muxihuayi.cn

C#:   base.Greet();
来源：http://ph.wgjwhj.cn

[G08] 静态方法与属性
来源：http://jx.shtwfgs.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://yp.9csxet.cn

PHP:  public static function f() {}
来源：http://mt.jianghongdianzi.cn

JS:   static f() {}
来源：http://sa.newstarts.cn

TS:   static f(): void {}
来源：http://hg.yuexingan06.cn

Java: static void f() {}
来源：http://ec.9csxet.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ij.521024.cn

Ruby: def self.f; end
来源：http://gv.nszjky.cn

C#:   public static void F() {}
来源：http://dq.shxzskj.cn

[G09] 接口 / 抽象类
来源：http://rh.huixiangedu.cn

Py:   from abc import ABC, abstractmethod
来源：http://ox.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pn.wgjwhj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://jq.wgjwhj.cn

TS:   interface Shape { area(): number; }
来源：http://ar.hahajie.cn

Java: interface Shape { double area(); }
来源：http://jl.huanxung.cn

Go:   type Shape interface { Area() float64 }
来源：http://rq.panjiajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://op.9csxet.cn

C#:   interface IShape { double Area(); }
来源：http://ii.nicolike.cn

[G10] 访问控制
来源：http://oi.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://to.bookmarksfly.cn

PHP:  public / protected / private
来源：http://xt.asd995.cn

JS:   #private 字段；其余公开
来源：http://wk.szsharing.cn

TS:   public / protected / private
来源：http://bs.huixiangedu.cn

Java: public / protected / private / 默认包级
来源：http://sv.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://az.colortex.cn

Ruby: public / protected / private
来源：http://ot.haigaiapp.cn

C#:   public / protected / private / internal
来源：http://iu.jianghongdianzi.cn

[G11] getter / setter
来源：http://gm.colortex.cn

Py:   @property 与 @x.setter
来源：http://zi.huanxung.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://do.asd995.cn

JS:   get name() { return this._name; }
来源：http://gt.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://jz.yuexingan06.cn

Java: public String getName() { return name; }
来源：http://sm.chemitech.net.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://he.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://iq.nszjky.cn

C#:   public string Name { get; set; }
来源：http://ju.hahajie.cn

[G12] 对象转字符串
来源：http://pu.jianghongdianzi.cn

Py:   def __str__(self): return self.name
来源：http://wt.hahajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pp.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://mn.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://xt.muxihuayi.cn

Java: @Override public String toString() { return name; }
来源：http://dz.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ds.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://wc.szxytkj.cn

C#:   public override string ToString() => Name;
来源：http://dm.bjjhwx.cn

[G13] 判断对象类型
来源：http://qk.shxzukj.cn

Py:   isinstance(u, User)
来源：http://ax.huixinmuqiang.cn

PHP:  $u instanceof User
来源：http://aj.huixiangedu.cn

JS:   u instanceof User
来源：http://bn.asd995.cn

TS:   u instanceof User
来源：http://ug.huanxung.cn

Java: u instanceof User
来源：http://bw.huixiangedu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://py.szsharing.cn

Ruby: u.is_a?(User)
来源：http://jn.shxzskj.cn

C#:   u is User
来源：http://hx.huixinmuqiang.cn

[G14] 数据类 / record
来源：http://za.panjiajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ok.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://lh.shxzukj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://rl.huanxung.cn

TS:   type User = { name: string; age: number };
来源：http://uu.hahajie.cn

Java: record User(String name, int age) {}
来源：http://zs.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://iy.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cm.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://sv.hahajie.cn

[G15] 枚举
来源：http://zb.hnjuh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://as.9csxet.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sb.nicolike.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ot.muxihuayi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cb.bookmarksfly.cn

Java: enum Color { RED, GREEN }
来源：http://ix.jianghongdianzi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://st.shxzskj.cn

Ruby: Color = %i[red green].freeze
来源：http://do.yuexingan06.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xm.newstarts.cn

[G16] 对象转数组 / 字典
来源：http://md.hnjuh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sv.yuntaijiaju.cn

PHP:  get_object_vars($obj);
来源：http://zy.9csxet.cn

JS:   Object.entries(obj)
来源：http://ov.haigaiapp.cn

TS:   Object.entries(obj)
来源：http://ut.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dz.newstarts.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://za.huixiangedu.cn

Ruby: obj.instance_variables
来源：http://or.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://sv.hnjuh.cn

================================================================================
来源：http://xe.colortex.cn

H. 异常与错误处理
来源：http://eg.hnjuh.cn

================================================================================
来源：http://wd.colortex.cn

[H01] try / catch 基础
来源：http://nj.haigaiapp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://on.szxytkj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gv.gzmigu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bn.szsharing.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rr.muxihuayi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://up.jctech888.com.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://fz.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ri.haigaiapp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://im.szsharing.cn

[H02] finally / ensure 收尾
来源：http://ny.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://cr.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bn.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lb.huixiangedu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fk.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kj.szxytkj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fd.shxzukj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lc.panjiajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dx.yuexingan06.cn

[H03] 主动抛出异常
来源：http://te.szxytkj.cn

Py:   raise ValueError("错误信息")
来源：http://jk.panjiajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pa.521024.cn

JS:   throw new Error("错误信息");
来源：http://aw.asd995.cn

TS:   throw new Error("错误信息");
来源：http://oe.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vo.colortex.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bx.shtwfgs.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://is.nszjky.cn

C#:   throw new ArgumentException("错误信息");
来源：http://oh.asd995.cn

[H04] 自定义异常类型
来源：http://ay.hnjuh.cn

Py:   class MyError(Exception): pass
来源：http://va.newstarts.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mr.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://kh.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://yp.colortex.cn

Java: class MyException extends RuntimeException {}
来源：http://gt.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wi.yuexingan06.cn

Ruby: class MyError < StandardError; end
来源：http://nn.yuntaijiaju.cn

C#:   class MyException : Exception {}
来源：http://dt.huixiangedu.cn

[H05] 捕获特定类型
来源：http://az.hahajie.cn

Py:   except ValueError as e:
来源：http://zp.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ni.colortex.cn

JS:   if (e instanceof TypeError) {}
来源：http://yq.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://fb.haigaiapp.cn

Java: catch (IOException | SQLException e) {}
来源：http://ai.nicolike.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kd.muxihuayi.cn

Ruby: rescue ArgumentError => e
来源：http://fm.huixinmuqiang.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wv.szxytkj.cn

[H06] 可选值 / 空值安全访问
来源：http://ba.huanxung.cn

Py:   value = d.get("k") or default
来源：http://tb.yuexingan06.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pu.wgjwhj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://df.gzmigu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vk.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sd.nicolike.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mz.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://gj.huanxung.cn

C#:   obj?.A?.B ?? default
来源：http://tp.yuexingan06.cn

[H07] 断言
来源：http://mz.asd995.cn

Py:   assert x > 0, "必须为正"
来源：http://ew.hahajie.cn

PHP:  assert($x > 0);
来源：http://ep.huanxung.cn

JS:   console.assert(x > 0);
来源：http://or.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://sv.bjjhwx.cn

Java: assert x > 0 : "必须为正";
来源：http://aa.jctech888.com.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qm.colortex.cn

Ruby: raise "必须为正" unless x > 0
来源：http://px.chemitech.net.cn

C#:   Debug.Assert(x > 0);
来源：http://ud.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://ad.shtwfgs.cn

Py:   str(e);  traceback.format_exc()
来源：http://bq.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rr.521024.cn

JS:   e.message;  e.stack
来源：http://gg.shtwfgs.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wu.colortex.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pf.yuntaijiaju.cn

Go:   err.Error()
来源：http://tr.huixinmuqiang.cn

Ruby: e.message;  e.backtrace
来源：http://ce.hahajie.cn

C#:   e.Message;  e.StackTrace
来源：http://tw.huanxung.cn

[H09] 带错误码的异常
来源：http://sv.shtwfgs.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rf.szsharing.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wt.521024.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rh.chemitech.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nq.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rq.huanxung.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pg.hnjuh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jn.asd995.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bm.huixinmuqiang.cn

[H10] 资源自动释放
来源：http://jf.chemitech.net.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ex.bjjhwx.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ds.bjjhwx.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ne.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sp.szsharing.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://db.jctech888.com.cn

Go:   defer f.Close()
来源：http://rb.huixinmuqiang.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://px.hahajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fs.szsharing.cn

================================================================================
来源：http://fk.newstarts.cn

I. 正则表达式
来源：http://na.hahajie.cn

================================================================================
来源：http://yk.huanxung.cn

[I01] 判断是否匹配
来源：http://je.panjiajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fz.shxzukj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://eq.shxzskj.cn

JS:   /\d+/.test(s)
来源：http://ss.9csxet.cn

TS:   /\d+/.test(s)
来源：http://he.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kg.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kx.haigaiapp.cn

Ruby: s.match?(/\d+/)
来源：http://uj.9csxet.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ks.chemitech.net.cn

[I02] 提取所有匹配
来源：http://bd.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://nt.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xb.asd995.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://az.jctech888.com.cn

TS:   s.match(/\d+/g)
来源：http://hm.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://va.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ff.yuexingan06.cn

Ruby: s.scan(/\d+/)
来源：http://lv.shxzskj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wh.huanxung.cn

[I03] 提取捕获分组
来源：http://ja.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://md.nszjky.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xi.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dm.colortex.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jo.jianghongdianzi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kd.nszjky.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wq.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cg.bjjhwx.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lc.hahajie.cn

[I04] 正则替换
来源：http://wf.jianghongdianzi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lq.hnjuh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://pk.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zv.szsharing.cn

TS:   s.replace(/\d+/g, "#")
来源：http://aq.chemitech.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ed.jianghongdianzi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ex.hnjuh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ev.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://my.shxzukj.cn

[I05] 按正则拆分
来源：http://ar.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://he.asd995.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://no.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://ct.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://mk.chemitech.net.cn

Java: s.split("\\s*,\\s*")
来源：http://ew.huixiangedu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wy.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rh.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://au.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ty.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rv.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zh.huixiangedu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oz.nicolike.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ph.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pj.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sn.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vi.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cz.newstarts.cn

[I07] 忽略大小写与多行模式
来源：http://mq.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tc.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zu.lnxyls.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ik.newstarts.cn

TS:   /error/gim
来源：http://sm.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wq.lnxyls.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jm.huixiangedu.cn

Ruby: s.scan(/error/i)
来源：http://pr.bjjhwx.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bb.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://bs.muxihuayi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oa.chemitech.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zu.9csxet.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bk.huanxung.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sa.szxytkj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fz.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ci.wgjwhj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://iq.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ab.newstarts.cn

================================================================================
来源：http://rl.521024.cn

J. 日期与时间
来源：http://dq.jianghongdianzi.cn

================================================================================
来源：http://ps.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://ox.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://fl.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gu.hnjuh.cn

JS:   new Date();  Date.now()
来源：http://zg.jctech888.com.cn

TS:   new Date();  Date.now()
来源：http://oh.521024.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://aj.9csxet.cn

Go:   time.Now()
来源：http://ma.nicolike.cn

Ruby: Time.now
来源：http://td.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qr.chemitech.net.cn

[J02] 格式化输出
来源：http://uh.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xh.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://th.newstarts.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ge.szxytkj.cn

TS:   d.toISOString()
来源：http://wf.szxytkj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bx.nicolike.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nl.jianghongdianzi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yy.wgjwhj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://de.9csxet.cn

[J03] 字符串解析为日期
来源：http://oc.bookmarksfly.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ps.asd995.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sk.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://wj.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://uy.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://yh.521024.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ig.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://qs.lnxyls.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bf.colortex.cn

[J04] 时间戳与日期互转
来源：http://vs.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ix.hahajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jv.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zj.yuexingan06.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sk.shxzukj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ar.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lh.bjjhwx.cn


<!-- 参考信息 -->