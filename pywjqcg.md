代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://qa.bookmarksfly.cn

Ruby: def self.f; end
来源：http://lz.jctech888.com.cn

C#:   public static void F() {}
来源：http://qq.huixiangedu.cn

[G09] 接口 / 抽象类
来源：http://ls.shxzskj.cn

Py:   from abc import ABC, abstractmethod
来源：http://kq.bjjhwx.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lu.colortex.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zv.chemitech.net.cn

TS:   interface Shape { area(): number; }
来源：http://bt.shtwfgs.cn

Java: interface Shape { double area(); }
来源：http://ug.hahajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://kx.wgjwhj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ha.shxzskj.cn

C#:   interface IShape { double Area(); }
来源：http://eu.yuexingan06.cn

[G10] 访问控制
来源：http://rs.newstarts.cn

Py:   约定 _protected / __private（不强制）
来源：http://sw.colortex.cn

PHP:  public / protected / private
来源：http://de.jianghongdianzi.cn

JS:   #private 字段；其余公开
来源：http://cu.chemitech.net.cn

TS:   public / protected / private
来源：http://tx.jianghongdianzi.cn

Java: public / protected / private / 默认包级
来源：http://dc.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xc.szsharing.cn

Ruby: public / protected / private
来源：http://gk.nszjky.cn

C#:   public / protected / private / internal
来源：http://by.asd995.cn

[G11] getter / setter
来源：http://ok.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://oh.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://do.muxihuayi.cn

JS:   get name() { return this._name; }
来源：http://kv.yuntaijiaju.cn

TS:   get name(): string { return this._name; }
来源：http://gi.bookmarksfly.cn

Java: public String getName() { return name; }
来源：http://et.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lz.shxzskj.cn

Ruby: attr_accessor :name
来源：http://ji.huixinmuqiang.cn

C#:   public string Name { get; set; }
来源：http://mo.shxzukj.cn

[G12] 对象转字符串
来源：http://hu.newstarts.cn

Py:   def __str__(self): return self.name
来源：http://cw.9csxet.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ir.yuexingan06.cn

JS:   toString() { return this.name; }
来源：http://hn.nszjky.cn

TS:   toString(): string { return this.name; }
来源：http://lp.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://og.shtwfgs.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zo.shxzskj.cn

Ruby: def to_s; @name; end
来源：http://yo.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://km.nicolike.cn

[G13] 判断对象类型
来源：http://ls.panjiajie.cn

Py:   isinstance(u, User)
来源：http://ae.wgjwhj.cn

PHP:  $u instanceof User
来源：http://mo.yuntaijiaju.cn

JS:   u instanceof User
来源：http://lh.bookmarksfly.cn

TS:   u instanceof User
来源：http://fb.yuexingan06.cn

Java: u instanceof User
来源：http://xw.yuntaijiaju.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tc.shxzukj.cn

Ruby: u.is_a?(User)
来源：http://wc.jctech888.com.cn

C#:   u is User
来源：http://mj.szsharing.cn

[G14] 数据类 / record
来源：http://tf.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://rw.panjiajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://kg.huanxung.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lg.521024.cn

TS:   type User = { name: string; age: number };
来源：http://mj.9csxet.cn

Java: record User(String name, int age) {}
来源：http://ad.panjiajie.cn

Go:   type User struct { Name string; Age int }
来源：http://em.jctech888.com.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://py.panjiajie.cn

C#:   record User(string Name, int Age);
来源：http://hn.wgjwhj.cn

[G15] 枚举
来源：http://og.bjjhwx.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nr.asd995.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dk.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://be.bjjhwx.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qj.gzmigu.cn

Java: enum Color { RED, GREEN }
来源：http://dp.panjiajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kb.shxzskj.cn

Ruby: Color = %i[red green].freeze
来源：http://xz.panjiajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rz.nszjky.cn

[G16] 对象转数组 / 字典
来源：http://ki.muxihuayi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mk.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://ni.9csxet.cn

JS:   Object.entries(obj)
来源：http://kk.shxzukj.cn

TS:   Object.entries(obj)
来源：http://pb.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vf.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://go.huanxung.cn

Ruby: obj.instance_variables
来源：http://mf.bjjhwx.cn

C#:   // 用反射或 System.Text.Json
来源：http://ld.huixiangedu.cn

================================================================================
来源：http://hc.panjiajie.cn

H. 异常与错误处理
来源：http://pd.gzmigu.cn

================================================================================
来源：http://qz.hnjuh.cn

[H01] try / catch 基础
来源：http://kj.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rz.gzmigu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uk.hahajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lx.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mf.colortex.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wf.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wm.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ss.hnjuh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eh.nicolike.cn

[H02] finally / ensure 收尾
来源：http://tt.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ha.nszjky.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bt.haigaiapp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rb.szxytkj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ha.muxihuayi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bo.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rx.hnjuh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pi.bookmarksfly.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qd.hahajie.cn

[H03] 主动抛出异常
来源：http://ru.yuntaijiaju.cn

Py:   raise ValueError("错误信息")
来源：http://xa.panjiajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pi.huanxung.cn

JS:   throw new Error("错误信息");
来源：http://im.9csxet.cn

TS:   throw new Error("错误信息");
来源：http://uq.jianghongdianzi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hc.jianghongdianzi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kn.huixinmuqiang.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ic.huanxung.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ig.nicolike.cn

[H04] 自定义异常类型
来源：http://xn.9csxet.cn

Py:   class MyError(Exception): pass
来源：http://yc.panjiajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gg.bjjhwx.cn

JS:   class MyError extends Error {}
来源：http://jv.gzmigu.cn

TS:   class MyError extends Error {}
来源：http://uh.chemitech.net.cn

Java: class MyException extends RuntimeException {}
来源：http://ir.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://up.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://wh.9csxet.cn

C#:   class MyException : Exception {}
来源：http://gg.nicolike.cn

[H05] 捕获特定类型
来源：http://hv.nicolike.cn

Py:   except ValueError as e:
来源：http://fb.bookmarksfly.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ia.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://na.hahajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://tn.shxzukj.cn

Java: catch (IOException | SQLException e) {}
来源：http://mp.huanxung.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mi.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://vk.huixiangedu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zx.nszjky.cn

[H06] 可选值 / 空值安全访问
来源：http://si.szsharing.cn

Py:   value = d.get("k") or default
来源：http://nl.haigaiapp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zi.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://uw.shxzskj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://eb.newstarts.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vw.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://uz.nicolike.cn

Ruby: d&.dig(:a, :b)
来源：http://gd.newstarts.cn

C#:   obj?.A?.B ?? default
来源：http://nj.huixiangedu.cn

[H07] 断言
来源：http://tg.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://rb.jianghongdianzi.cn

PHP:  assert($x > 0);
来源：http://ea.nszjky.cn

JS:   console.assert(x > 0);
来源：http://bp.9csxet.cn

TS:   console.assert(x > 0);
来源：http://wp.nszjky.cn

Java: assert x > 0 : "必须为正";
来源：http://ea.newstarts.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ym.szxytkj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hj.panjiajie.cn

C#:   Debug.Assert(x > 0);
来源：http://ux.asd995.cn

[H08] 获取错误信息与堆栈
来源：http://kp.szsharing.cn

Py:   str(e);  traceback.format_exc()
来源：http://ms.bookmarksfly.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sm.colortex.cn

JS:   e.message;  e.stack
来源：http://hj.yuexingan06.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ce.gzmigu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ar.szsharing.cn

Go:   err.Error()
来源：http://qh.hnjuh.cn

Ruby: e.message;  e.backtrace
来源：http://en.chemitech.net.cn

C#:   e.Message;  e.StackTrace
来源：http://ob.jctech888.com.cn

[H09] 带错误码的异常
来源：http://al.shxzukj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dt.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gx.huixinmuqiang.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kq.yuntaijiaju.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ej.szxytkj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tp.hahajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vo.panjiajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pw.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://if.yuexingan06.cn

[H10] 资源自动释放
来源：http://ni.wgjwhj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://et.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ym.hnjuh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gs.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bj.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qv.gzmigu.cn

Go:   defer f.Close()
来源：http://jk.muxihuayi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ne.jianghongdianzi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bn.lnxyls.cn

================================================================================
来源：http://tq.nszjky.cn

I. 正则表达式
来源：http://ba.hnjuh.cn

================================================================================
来源：http://ta.jctech888.com.cn

[I01] 判断是否匹配
来源：http://sv.colortex.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wx.jianghongdianzi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dc.shxzskj.cn

JS:   /\d+/.test(s)
来源：http://kq.muxihuayi.cn

TS:   /\d+/.test(s)
来源：http://dn.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lw.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cg.haigaiapp.cn

Ruby: s.match?(/\d+/)
来源：http://xp.muxihuayi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bw.muxihuayi.cn

[I02] 提取所有匹配
来源：http://gw.jianghongdianzi.cn

Py:   re.findall(r"\d+", s)
来源：http://sw.hnjuh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://td.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jk.jctech888.com.cn

TS:   s.match(/\d+/g)
来源：http://dc.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oc.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ii.521024.cn

Ruby: s.scan(/\d+/)
来源：http://cy.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mb.huixinmuqiang.cn

[I03] 提取捕获分组
来源：http://xz.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tt.9csxet.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://my.szsharing.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kf.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://qm.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ds.9csxet.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wb.huixiangedu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qs.shtwfgs.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pm.panjiajie.cn

[I04] 正则替换
来源：http://mp.hahajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xo.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ly.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://wp.colortex.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bj.bookmarksfly.cn

Java: s.replaceAll("\\d+", "#")
来源：http://eh.gzmigu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fk.gzmigu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hd.panjiajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ct.521024.cn

[I05] 按正则拆分
来源：http://kl.hnjuh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://nw.yuntaijiaju.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fx.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://gh.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://jc.nszjky.cn

Java: s.split("\\s*,\\s*")
来源：http://sk.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vc.yuexingan06.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vo.szxytkj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ul.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jx.huanxung.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://no.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://al.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jq.shxzukj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lq.huixiangedu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kp.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pf.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nb.huixiangedu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ue.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://ol.yuntaijiaju.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fc.szxytkj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vh.nicolike.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ux.huanxung.cn

TS:   /error/gim
来源：http://mj.shxzskj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lb.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wm.szsharing.cn

Ruby: s.scan(/error/i)
来源：http://un.bjjhwx.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xk.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://ct.muxihuayi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fe.nicolike.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cc.hnjuh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sa.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xi.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nv.bjjhwx.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lx.jianghongdianzi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://up.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pu.521024.cn

================================================================================
来源：http://xy.jianghongdianzi.cn

J. 日期与时间
来源：http://tm.newstarts.cn

================================================================================
来源：http://rf.nszjky.cn

[J01] 获取当前时间
来源：http://yc.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yg.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ss.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://fk.asd995.cn

TS:   new Date();  Date.now()
来源：http://uy.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lg.yuexingan06.cn

Go:   time.Now()
来源：http://vs.bookmarksfly.cn

Ruby: Time.now
来源：http://jp.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://he.asd995.cn

[J02] 格式化输出
来源：http://cd.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kr.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hn.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ma.jctech888.com.cn

TS:   d.toISOString()
来源：http://oe.lnxyls.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://zh.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yi.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sf.521024.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lb.newstarts.cn

[J03] 字符串解析为日期
来源：http://mp.asd995.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rr.gzmigu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fj.panjiajie.cn

JS:   new Date("2024-01-02")
来源：http://nf.huixiangedu.cn

TS:   new Date("2024-01-02")
来源：http://xx.hahajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xl.panjiajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gb.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://nz.hnjuh.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ri.shtwfgs.cn

[J04] 时间戳与日期互转
来源：http://xm.hnjuh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://fc.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ta.huixinmuqiang.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pz.bjjhwx.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lu.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://am.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nr.chemitech.net.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qq.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ly.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://ty.asd995.cn

Py:   now + timedelta(days=7)
来源：http://kp.shxzskj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nr.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gu.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hu.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://sh.yuexingan06.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fr.hahajie.cn

Ruby: Time.now + 7 * 86400
来源：http://ih.bookmarksfly.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zy.szsharing.cn

[J06] 计算两时间之差
来源：http://os.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://lo.wgjwhj.cn

PHP:  $end->diff($start)->days;
来源：http://aq.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://en.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gu.haigaiapp.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cv.wgjwhj.cn

Go:   end.Sub(start).Hours()
来源：http://bw.nszjky.cn

Ruby: end - start                 # 返回秒数
来源：http://yo.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://nd.shtwfgs.cn


<!-- 参考信息 -->