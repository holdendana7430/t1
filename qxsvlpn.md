代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://vk.hahajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hn.nicolike.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bz.shxzskj.cn

TS:   interface Shape { area(): number; }
来源：http://sr.chemitech.net.cn

Java: interface Shape { double area(); }
来源：http://fq.521024.cn

Go:   type Shape interface { Area() float64 }
来源：http://fx.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ct.colortex.cn

C#:   interface IShape { double Area(); }
来源：http://ww.nicolike.cn

[G10] 访问控制
来源：http://qg.jianghongdianzi.cn

Py:   约定 _protected / __private（不强制）
来源：http://ui.yuexingan06.cn

PHP:  public / protected / private
来源：http://hc.jianghongdianzi.cn

JS:   #private 字段；其余公开
来源：http://sh.muxihuayi.cn

TS:   public / protected / private
来源：http://js.shtwfgs.cn

Java: public / protected / private / 默认包级
来源：http://vt.jctech888.com.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ws.newstarts.cn

Ruby: public / protected / private
来源：http://zo.gzmigu.cn

C#:   public / protected / private / internal
来源：http://ao.lnxyls.cn

[G11] getter / setter
来源：http://xt.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://th.szxytkj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ej.huixinmuqiang.cn

JS:   get name() { return this._name; }
来源：http://vc.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://oi.bookmarksfly.cn

Java: public String getName() { return name; }
来源：http://sg.huanxung.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ix.wgjwhj.cn

Ruby: attr_accessor :name
来源：http://mr.szxytkj.cn

C#:   public string Name { get; set; }
来源：http://rx.panjiajie.cn

[G12] 对象转字符串
来源：http://tj.shtwfgs.cn

Py:   def __str__(self): return self.name
来源：http://fk.huanxung.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jz.shtwfgs.cn

JS:   toString() { return this.name; }
来源：http://vp.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://wc.hnjuh.cn

Java: @Override public String toString() { return name; }
来源：http://pm.asd995.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ne.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://ik.huixiangedu.cn

C#:   public override string ToString() => Name;
来源：http://tf.jianghongdianzi.cn

[G13] 判断对象类型
来源：http://ig.nicolike.cn

Py:   isinstance(u, User)
来源：http://xx.gzmigu.cn

PHP:  $u instanceof User
来源：http://lx.huixinmuqiang.cn

JS:   u instanceof User
来源：http://eh.haigaiapp.cn

TS:   u instanceof User
来源：http://fd.hahajie.cn

Java: u instanceof User
来源：http://hy.shxzukj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ru.szxytkj.cn

Ruby: u.is_a?(User)
来源：http://vp.9csxet.cn

C#:   u is User
来源：http://lv.bookmarksfly.cn

[G14] 数据类 / record
来源：http://cn.jianghongdianzi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kk.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://vy.yuntaijiaju.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zr.bookmarksfly.cn

TS:   type User = { name: string; age: number };
来源：http://uf.szxytkj.cn

Java: record User(String name, int age) {}
来源：http://ne.jianghongdianzi.cn

Go:   type User struct { Name string; Age int }
来源：http://hp.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bt.asd995.cn

C#:   record User(string Name, int Age);
来源：http://ze.huanxung.cn

[G15] 枚举
来源：http://dd.bjjhwx.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vl.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ao.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ss.9csxet.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mr.nszjky.cn

Java: enum Color { RED, GREEN }
来源：http://bn.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oz.huixinmuqiang.cn

Ruby: Color = %i[red green].freeze
来源：http://hu.nicolike.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bf.nszjky.cn

[G16] 对象转数组 / 字典
来源：http://tv.bjjhwx.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rf.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://ih.yuexingan06.cn

JS:   Object.entries(obj)
来源：http://hc.521024.cn

TS:   Object.entries(obj)
来源：http://aj.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vr.jianghongdianzi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hj.nszjky.cn

Ruby: obj.instance_variables
来源：http://uu.nszjky.cn

C#:   // 用反射或 System.Text.Json
来源：http://po.lnxyls.cn

================================================================================
来源：http://mv.szxytkj.cn

H. 异常与错误处理
来源：http://it.huanxung.cn

================================================================================
来源：http://nm.bjjhwx.cn

[H01] try / catch 基础
来源：http://ja.hahajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nf.shtwfgs.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pz.shxzskj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ho.muxihuayi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ou.huixinmuqiang.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lq.shtwfgs.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uw.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vi.huixinmuqiang.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ig.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://hu.huixiangedu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://uw.nszjky.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vn.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pq.nszjky.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ks.nicolike.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qg.gzmigu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vv.panjiajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ws.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pr.hnjuh.cn

[H03] 主动抛出异常
来源：http://by.bookmarksfly.cn

Py:   raise ValueError("错误信息")
来源：http://mk.huixinmuqiang.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ja.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://wy.muxihuayi.cn

TS:   throw new Error("错误信息");
来源：http://fi.szxytkj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qh.haigaiapp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://me.huixiangedu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mg.szxytkj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://og.haigaiapp.cn

[H04] 自定义异常类型
来源：http://qe.gzmigu.cn

Py:   class MyError(Exception): pass
来源：http://ak.huixinmuqiang.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nl.yuntaijiaju.cn

JS:   class MyError extends Error {}
来源：http://my.nszjky.cn

TS:   class MyError extends Error {}
来源：http://kp.bookmarksfly.cn

Java: class MyException extends RuntimeException {}
来源：http://lr.hnjuh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mw.colortex.cn

Ruby: class MyError < StandardError; end
来源：http://kg.shxzukj.cn

C#:   class MyException : Exception {}
来源：http://ay.9csxet.cn

[H05] 捕获特定类型
来源：http://mi.nszjky.cn

Py:   except ValueError as e:
来源：http://yb.jctech888.com.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://cg.colortex.cn

JS:   if (e instanceof TypeError) {}
来源：http://cm.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://it.lnxyls.cn

Java: catch (IOException | SQLException e) {}
来源：http://qy.gzmigu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qq.shxzukj.cn

Ruby: rescue ArgumentError => e
来源：http://rz.huixiangedu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hy.asd995.cn

[H06] 可选值 / 空值安全访问
来源：http://ec.yuntaijiaju.cn

Py:   value = d.get("k") or default
来源：http://ta.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cd.newstarts.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dp.huixiangedu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bg.hahajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qg.yuexingan06.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://us.muxihuayi.cn

Ruby: d&.dig(:a, :b)
来源：http://oe.521024.cn

C#:   obj?.A?.B ?? default
来源：http://tv.huixiangedu.cn

[H07] 断言
来源：http://na.huixinmuqiang.cn

Py:   assert x > 0, "必须为正"
来源：http://bc.jctech888.com.cn

PHP:  assert($x > 0);
来源：http://ds.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://wq.szxytkj.cn

TS:   console.assert(x > 0);
来源：http://wr.shxzukj.cn

Java: assert x > 0 : "必须为正";
来源：http://na.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dz.szxytkj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xp.nszjky.cn

C#:   Debug.Assert(x > 0);
来源：http://ag.huixinmuqiang.cn

[H08] 获取错误信息与堆栈
来源：http://gw.9csxet.cn

Py:   str(e);  traceback.format_exc()
来源：http://jn.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qe.huanxung.cn

JS:   e.message;  e.stack
来源：http://hb.wgjwhj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mf.colortex.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rt.jianghongdianzi.cn

Go:   err.Error()
来源：http://qr.haigaiapp.cn

Ruby: e.message;  e.backtrace
来源：http://wn.shxzukj.cn

C#:   e.Message;  e.StackTrace
来源：http://vl.huixinmuqiang.cn

[H09] 带错误码的异常
来源：http://kv.muxihuayi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hm.nicolike.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ni.9csxet.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oz.nicolike.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wu.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vl.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ml.huixiangedu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fc.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://py.huixiangedu.cn

[H10] 资源自动释放
来源：http://dt.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qa.wgjwhj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bw.wgjwhj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kn.haigaiapp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pk.colortex.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jl.szsharing.cn

Go:   defer f.Close()
来源：http://ab.muxihuayi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wi.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ih.wgjwhj.cn

================================================================================
来源：http://mc.shxzskj.cn

I. 正则表达式
来源：http://sd.shxzskj.cn

================================================================================
来源：http://mx.panjiajie.cn

[I01] 判断是否匹配
来源：http://ov.colortex.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zz.521024.cn

PHP:  preg_match('/\d+/', $s);
来源：http://oh.szxytkj.cn

JS:   /\d+/.test(s)
来源：http://xd.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://gj.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dj.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pp.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://px.hahajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qm.hnjuh.cn

[I02] 提取所有匹配
来源：http://nu.jctech888.com.cn

Py:   re.findall(r"\d+", s)
来源：http://tq.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ku.nszjky.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vq.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://cq.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ai.nicolike.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pk.panjiajie.cn

Ruby: s.scan(/\d+/)
来源：http://af.huixinmuqiang.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gf.yuntaijiaju.cn

[I03] 提取捕获分组
来源：http://xa.wgjwhj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yi.hahajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ef.panjiajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zr.shtwfgs.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wn.yuexingan06.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cx.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qm.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tw.gzmigu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rl.nicolike.cn

[I04] 正则替换
来源：http://tu.gzmigu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xn.hahajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vl.jctech888.com.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zr.panjiajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jw.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sg.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pj.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hc.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tg.yuexingan06.cn

[I05] 按正则拆分
来源：http://kq.haigaiapp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gw.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://re.jctech888.com.cn

JS:   s.split(/\s*,\s*/)
来源：http://gg.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://kk.521024.cn

Java: s.split("\\s*,\\s*")
来源：http://hr.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://de.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pl.szxytkj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qm.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pi.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jh.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dw.bookmarksfly.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yb.huixinmuqiang.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nl.panjiajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sr.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ci.521024.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xf.lnxyls.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://np.yuexingan06.cn

[I07] 忽略大小写与多行模式
来源：http://di.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wr.9csxet.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yk.nicolike.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://id.szsharing.cn

TS:   /error/gim
来源：http://qf.bookmarksfly.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jk.shxzukj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://tw.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://na.hnjuh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vc.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://ux.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wa.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vv.gzmigu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mu.yuexingan06.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ps.huixiangedu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kb.haigaiapp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://eg.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cv.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uc.haigaiapp.cn

================================================================================
来源：http://au.huixiangedu.cn

J. 日期与时间
来源：http://oa.yuntaijiaju.cn

================================================================================
来源：http://uf.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://xn.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yu.colortex.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zn.newstarts.cn

JS:   new Date();  Date.now()
来源：http://oj.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://rw.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dh.nszjky.cn

Go:   time.Now()
来源：http://gl.newstarts.cn

Ruby: Time.now
来源：http://gn.9csxet.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ms.bookmarksfly.cn

[J02] 格式化输出
来源：http://og.bookmarksfly.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lv.huixinmuqiang.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bi.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://nu.shxzukj.cn

TS:   d.toISOString()
来源：http://td.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fd.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kp.colortex.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://eu.521024.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dp.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://bp.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://re.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xh.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://gk.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://ry.jctech888.com.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vf.szxytkj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://eg.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://gm.szxytkj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fb.huixinmuqiang.cn

[J04] 时间戳与日期互转
来源：http://ft.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kn.szxytkj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://tq.lnxyls.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tg.szxytkj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zq.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ts.521024.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ql.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mq.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://iq.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://kz.nszjky.cn

Py:   now + timedelta(days=7)
来源：http://pg.bjjhwx.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://or.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pa.szxytkj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bo.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://ss.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://fq.yuexingan06.cn

Ruby: Time.now + 7 * 86400
来源：http://bs.colortex.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ee.shxzukj.cn

[J06] 计算两时间之差
来源：http://ye.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://kv.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://vh.chemitech.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wf.colortex.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pb.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ai.wgjwhj.cn

Go:   end.Sub(start).Hours()
来源：http://sy.shxzskj.cn

Ruby: end - start                 # 返回秒数
来源：http://rj.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://yg.huixinmuqiang.cn

[J07] 比较两个日期
来源：http://wj.huixinmuqiang.cn

Py:   d1 < d2;  d1 == d2
来源：http://hx.muxihuayi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nz.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ww.bookmarksfly.cn


<!-- 参考信息 -->