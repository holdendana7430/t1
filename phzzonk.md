代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://vr.szsharing.cn

Ruby: def self.f; end
来源：http://po.nszjky.cn

C#:   public static void F() {}
来源：http://vd.bjjhwx.cn

[G09] 接口 / 抽象类
来源：http://jy.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://wk.jctech888.com.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pr.huixiangedu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://if.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://lu.nicolike.cn

Java: interface Shape { double area(); }
来源：http://vc.lnxyls.cn

Go:   type Shape interface { Area() float64 }
来源：http://lx.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://tz.panjiajie.cn

C#:   interface IShape { double Area(); }
来源：http://uc.szsharing.cn

[G10] 访问控制
来源：http://pp.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://tf.nicolike.cn

PHP:  public / protected / private
来源：http://yu.jctech888.com.cn

JS:   #private 字段；其余公开
来源：http://lc.bjjhwx.cn

TS:   public / protected / private
来源：http://nc.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://gg.huanxung.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://au.9csxet.cn

Ruby: public / protected / private
来源：http://fh.nszjky.cn

C#:   public / protected / private / internal
来源：http://ha.521024.cn

[G11] getter / setter
来源：http://gc.newstarts.cn

Py:   @property 与 @x.setter
来源：http://ep.jianghongdianzi.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gr.shxzskj.cn

JS:   get name() { return this._name; }
来源：http://wb.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://oo.shtwfgs.cn

Java: public String getName() { return name; }
来源：http://jy.bjjhwx.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yg.521024.cn

Ruby: attr_accessor :name
来源：http://xs.hnjuh.cn

C#:   public string Name { get; set; }
来源：http://ku.newstarts.cn

[G12] 对象转字符串
来源：http://yt.jianghongdianzi.cn

Py:   def __str__(self): return self.name
来源：http://td.panjiajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zm.shtwfgs.cn

JS:   toString() { return this.name; }
来源：http://jw.yuexingan06.cn

TS:   toString(): string { return this.name; }
来源：http://qk.jianghongdianzi.cn

Java: @Override public String toString() { return name; }
来源：http://re.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://aw.colortex.cn

Ruby: def to_s; @name; end
来源：http://kz.szsharing.cn

C#:   public override string ToString() => Name;
来源：http://ao.lnxyls.cn

[G13] 判断对象类型
来源：http://vr.colortex.cn

Py:   isinstance(u, User)
来源：http://qd.nszjky.cn

PHP:  $u instanceof User
来源：http://kz.huixiangedu.cn

JS:   u instanceof User
来源：http://ck.haigaiapp.cn

TS:   u instanceof User
来源：http://wu.szsharing.cn

Java: u instanceof User
来源：http://on.yuntaijiaju.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://hx.szsharing.cn

Ruby: u.is_a?(User)
来源：http://cu.lnxyls.cn

C#:   u is User
来源：http://vj.shxzukj.cn

[G14] 数据类 / record
来源：http://il.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ka.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://os.yuexingan06.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pz.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://ul.gzmigu.cn

Java: record User(String name, int age) {}
来源：http://jc.9csxet.cn

Go:   type User struct { Name string; Age int }
来源：http://yk.muxihuayi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nv.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://aq.yuexingan06.cn

[G15] 枚举
来源：http://vh.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vu.asd995.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zf.shxzukj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zx.colortex.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://yh.jctech888.com.cn

Java: enum Color { RED, GREEN }
来源：http://yb.shxzukj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lz.gzmigu.cn

Ruby: Color = %i[red green].freeze
来源：http://sq.bookmarksfly.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://uk.asd995.cn

[G16] 对象转数组 / 字典
来源：http://nv.asd995.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hp.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://vz.nicolike.cn

JS:   Object.entries(obj)
来源：http://qa.gzmigu.cn

TS:   Object.entries(obj)
来源：http://nl.chemitech.net.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ti.jianghongdianzi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ku.huanxung.cn

Ruby: obj.instance_variables
来源：http://yj.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://ma.yuexingan06.cn

================================================================================
来源：http://vz.yuexingan06.cn

H. 异常与错误处理
来源：http://bj.newstarts.cn

================================================================================
来源：http://dt.521024.cn

[H01] try / catch 基础
来源：http://eq.shxzukj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eb.huanxung.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ay.chemitech.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://er.hnjuh.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wz.shxzskj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hp.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gn.jianghongdianzi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gt.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ci.asd995.cn

[H02] finally / ensure 收尾
来源：http://ye.panjiajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gf.yuexingan06.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tj.haigaiapp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ki.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://sc.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://tz.asd995.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hu.bookmarksfly.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ba.bookmarksfly.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fc.huanxung.cn

[H03] 主动抛出异常
来源：http://ol.gzmigu.cn

Py:   raise ValueError("错误信息")
来源：http://pw.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ot.nszjky.cn

JS:   throw new Error("错误信息");
来源：http://pd.jctech888.com.cn

TS:   throw new Error("错误信息");
来源：http://xu.nszjky.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nv.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ax.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jx.gzmigu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://je.chemitech.net.cn

[H04] 自定义异常类型
来源：http://uy.chemitech.net.cn

Py:   class MyError(Exception): pass
来源：http://rt.shxzukj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rh.yuntaijiaju.cn

JS:   class MyError extends Error {}
来源：http://du.asd995.cn

TS:   class MyError extends Error {}
来源：http://qh.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://uj.jianghongdianzi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vh.yuntaijiaju.cn

Ruby: class MyError < StandardError; end
来源：http://iw.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://ps.szsharing.cn

[H05] 捕获特定类型
来源：http://fy.hnjuh.cn

Py:   except ValueError as e:
来源：http://cj.9csxet.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vr.lnxyls.cn

JS:   if (e instanceof TypeError) {}
来源：http://pp.shtwfgs.cn

TS:   if (e instanceof TypeError) {}
来源：http://ei.wgjwhj.cn

Java: catch (IOException | SQLException e) {}
来源：http://kd.jianghongdianzi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cb.jctech888.com.cn

Ruby: rescue ArgumentError => e
来源：http://oo.bookmarksfly.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qz.shxzskj.cn

[H06] 可选值 / 空值安全访问
来源：http://rl.bjjhwx.cn

Py:   value = d.get("k") or default
来源：http://zv.hnjuh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hl.muxihuayi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://cd.yuexingan06.cn

TS:   obj?.a?.b;  d ?? default
来源：http://rc.nszjky.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qn.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tl.bjjhwx.cn

Ruby: d&.dig(:a, :b)
来源：http://eu.9csxet.cn

C#:   obj?.A?.B ?? default
来源：http://bo.muxihuayi.cn

[H07] 断言
来源：http://ha.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://ca.nicolike.cn

PHP:  assert($x > 0);
来源：http://ab.yuntaijiaju.cn

JS:   console.assert(x > 0);
来源：http://cn.wgjwhj.cn

TS:   console.assert(x > 0);
来源：http://sf.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://gx.asd995.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jn.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pu.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://av.asd995.cn

[H08] 获取错误信息与堆栈
来源：http://pk.hnjuh.cn

Py:   str(e);  traceback.format_exc()
来源：http://mz.jctech888.com.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://jd.jianghongdianzi.cn

JS:   e.message;  e.stack
来源：http://eg.jianghongdianzi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ri.newstarts.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uf.bjjhwx.cn

Go:   err.Error()
来源：http://jx.yuntaijiaju.cn

Ruby: e.message;  e.backtrace
来源：http://sc.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://en.chemitech.net.cn

[H09] 带错误码的异常
来源：http://bw.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jc.521024.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://it.nicolike.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yq.yuntaijiaju.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jl.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kg.newstarts.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ee.gzmigu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wy.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dj.jctech888.com.cn

[H10] 资源自动释放
来源：http://ah.wgjwhj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://us.huixinmuqiang.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xd.szxytkj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zt.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ov.yuntaijiaju.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vc.chemitech.net.cn

Go:   defer f.Close()
来源：http://nc.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qk.huanxung.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sp.szxytkj.cn

================================================================================
来源：http://ta.lnxyls.cn

I. 正则表达式
来源：http://wi.colortex.cn

================================================================================
来源：http://nw.nicolike.cn

[I01] 判断是否匹配
来源：http://hp.wgjwhj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://oe.9csxet.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lw.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://wl.nszjky.cn

TS:   /\d+/.test(s)
来源：http://xo.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jn.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cn.gzmigu.cn

Ruby: s.match?(/\d+/)
来源：http://lk.shxzukj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rm.lnxyls.cn

[I02] 提取所有匹配
来源：http://rk.huixinmuqiang.cn

Py:   re.findall(r"\d+", s)
来源：http://gs.hnjuh.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fl.nicolike.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ad.gzmigu.cn

TS:   s.match(/\d+/g)
来源：http://lz.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bf.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vf.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://zj.colortex.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yi.bjjhwx.cn

[I03] 提取捕获分组
来源：http://go.colortex.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ue.szxytkj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://oi.bjjhwx.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://rb.jianghongdianzi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vj.hahajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pj.jctech888.com.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dn.shxzukj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mv.bjjhwx.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ec.newstarts.cn

[I04] 正则替换
来源：http://ru.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nn.szxytkj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://sq.nicolike.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zr.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://li.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nm.huixinmuqiang.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://au.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gj.wgjwhj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://yc.bjjhwx.cn

[I05] 按正则拆分
来源：http://gy.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gm.muxihuayi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cn.nszjky.cn

JS:   s.split(/\s*,\s*/)
来源：http://wb.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://ua.hnjuh.cn

Java: s.split("\\s*,\\s*")
来源：http://ib.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://rw.bookmarksfly.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sc.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://me.shxzskj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sq.newstarts.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xv.gzmigu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pd.hahajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://mu.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zx.yuntaijiaju.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rm.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sc.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mo.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://jc.521024.cn

[I07] 忽略大小写与多行模式
来源：http://yt.huixiangedu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xd.huanxung.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ed.gzmigu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fl.haigaiapp.cn

TS:   /error/gim
来源：http://rw.szsharing.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kw.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ka.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://fe.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vy.bookmarksfly.cn

[I08] 贪婪与非贪婪匹配
来源：http://sr.yuexingan06.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nw.nicolike.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fm.szsharing.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ud.huanxung.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jl.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fk.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zm.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wb.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hk.jctech888.com.cn

================================================================================
来源：http://ys.huixinmuqiang.cn

J. 日期与时间
来源：http://th.szsharing.cn

================================================================================
来源：http://ej.bjjhwx.cn

[J01] 获取当前时间
来源：http://vu.jctech888.com.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wf.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hl.shtwfgs.cn

JS:   new Date();  Date.now()
来源：http://ok.hahajie.cn

TS:   new Date();  Date.now()
来源：http://qz.newstarts.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pj.haigaiapp.cn

Go:   time.Now()
来源：http://xv.newstarts.cn

Ruby: Time.now
来源：http://lq.lnxyls.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mz.huixinmuqiang.cn

[J02] 格式化输出
来源：http://yz.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qe.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gd.szsharing.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dq.colortex.cn

TS:   d.toISOString()
来源：http://uz.asd995.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://lh.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gr.jianghongdianzi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://of.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kd.shxzskj.cn

[J03] 字符串解析为日期
来源：http://jm.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://of.lnxyls.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nw.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://ef.bjjhwx.cn

TS:   new Date("2024-01-02")
来源：http://xd.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tb.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lv.chemitech.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://bx.yuntaijiaju.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xb.huixiangedu.cn

[J04] 时间戳与日期互转
来源：http://fh.jianghongdianzi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ex.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://bk.nszjky.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ve.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cz.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vg.shxzukj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wl.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://aa.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lw.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://rr.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://fj.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ab.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hr.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wp.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://io.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lj.panjiajie.cn

Ruby: Time.now + 7 * 86400
来源：http://ug.haigaiapp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://iq.chemitech.net.cn

[J06] 计算两时间之差
来源：http://sw.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://tp.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://ij.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xo.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://id.gzmigu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hw.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://fv.521024.cn

Ruby: end - start                 # 返回秒数
来源：http://uq.huixiangedu.cn

C#:   (end - start).TotalSeconds
来源：http://bz.huixinmuqiang.cn


<!-- 参考信息 -->