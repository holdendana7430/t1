代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://ok.panjiajie.cn

Ruby: def self.f; end
来源：http://np.lnxyls.cn

C#:   public static void F() {}
来源：http://wq.bjjhwx.cn

[G09] 接口 / 抽象类
来源：http://lv.lnxyls.cn

Py:   from abc import ABC, abstractmethod
来源：http://tl.huanxung.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ac.521024.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://pz.yuexingan06.cn

TS:   interface Shape { area(): number; }
来源：http://dl.huanxung.cn

Java: interface Shape { double area(); }
来源：http://gd.9csxet.cn

Go:   type Shape interface { Area() float64 }
来源：http://fz.huixinmuqiang.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://eu.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://cu.asd995.cn

[G10] 访问控制
来源：http://ir.hnjuh.cn

Py:   约定 _protected / __private（不强制）
来源：http://ed.shxzskj.cn

PHP:  public / protected / private
来源：http://iz.asd995.cn

JS:   #private 字段；其余公开
来源：http://qr.nicolike.cn

TS:   public / protected / private
来源：http://wr.hnjuh.cn

Java: public / protected / private / 默认包级
来源：http://tw.shxzskj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://bp.chemitech.net.cn

Ruby: public / protected / private
来源：http://pt.hnjuh.cn

C#:   public / protected / private / internal
来源：http://jm.wgjwhj.cn

[G11] getter / setter
来源：http://xi.szxytkj.cn

Py:   @property 与 @x.setter
来源：http://fq.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://md.shxzskj.cn

JS:   get name() { return this._name; }
来源：http://zz.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://xr.shtwfgs.cn

Java: public String getName() { return name; }
来源：http://zz.yuexingan06.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yg.hahajie.cn

Ruby: attr_accessor :name
来源：http://ko.521024.cn

C#:   public string Name { get; set; }
来源：http://ym.newstarts.cn

[G12] 对象转字符串
来源：http://lg.colortex.cn

Py:   def __str__(self): return self.name
来源：http://wo.szxytkj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ml.szxytkj.cn

JS:   toString() { return this.name; }
来源：http://vl.nszjky.cn

TS:   toString(): string { return this.name; }
来源：http://ax.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://hc.jianghongdianzi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jg.gzmigu.cn

Ruby: def to_s; @name; end
来源：http://ns.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://tz.haigaiapp.cn

[G13] 判断对象类型
来源：http://qr.colortex.cn

Py:   isinstance(u, User)
来源：http://xd.gzmigu.cn

PHP:  $u instanceof User
来源：http://bh.nszjky.cn

JS:   u instanceof User
来源：http://th.nicolike.cn

TS:   u instanceof User
来源：http://bc.jianghongdianzi.cn

Java: u instanceof User
来源：http://se.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tq.jctech888.com.cn

Ruby: u.is_a?(User)
来源：http://ww.muxihuayi.cn

C#:   u is User
来源：http://kp.nszjky.cn

[G14] 数据类 / record
来源：http://tr.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qn.huixinmuqiang.cn

PHP:  // 用 readonly 属性模拟
来源：http://bb.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ch.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://xg.bookmarksfly.cn

Java: record User(String name, int age) {}
来源：http://th.wgjwhj.cn

Go:   type User struct { Name string; Age int }
来源：http://hf.panjiajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pb.521024.cn

C#:   record User(string Name, int Age);
来源：http://hc.shxzskj.cn

[G15] 枚举
来源：http://ce.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://zu.shxzskj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xx.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eq.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cj.bookmarksfly.cn

Java: enum Color { RED, GREEN }
来源：http://ea.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yg.9csxet.cn

Ruby: Color = %i[red green].freeze
来源：http://so.yuexingan06.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ys.jctech888.com.cn

[G16] 对象转数组 / 字典
来源：http://lq.yuntaijiaju.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vs.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://os.hahajie.cn

JS:   Object.entries(obj)
来源：http://pf.jctech888.com.cn

TS:   Object.entries(obj)
来源：http://by.nszjky.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fe.yuexingan06.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.gzmigu.cn

Ruby: obj.instance_variables
来源：http://iu.newstarts.cn

C#:   // 用反射或 System.Text.Json
来源：http://be.shxzskj.cn

================================================================================
来源：http://sn.panjiajie.cn

H. 异常与错误处理
来源：http://ra.yuexingan06.cn

================================================================================
来源：http://iy.hnjuh.cn

[H01] try / catch 基础
来源：http://yx.jianghongdianzi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dz.hnjuh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yv.yuexingan06.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uz.gzmigu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pl.shtwfgs.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cc.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oj.bjjhwx.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ys.muxihuayi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ml.jctech888.com.cn

[H02] finally / ensure 收尾
来源：http://os.yuntaijiaju.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bo.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sr.muxihuayi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://oj.huanxung.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ds.nszjky.cn

Java: try { f(); } finally { cleanup(); }
来源：http://et.colortex.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://np.panjiajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ob.chemitech.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://fs.yuexingan06.cn

[H03] 主动抛出异常
来源：http://pk.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://uq.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ge.huanxung.cn

JS:   throw new Error("错误信息");
来源：http://gy.wgjwhj.cn

TS:   throw new Error("错误信息");
来源：http://hi.wgjwhj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ml.wgjwhj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hi.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rw.lnxyls.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xy.asd995.cn

[H04] 自定义异常类型
来源：http://mx.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://ge.bookmarksfly.cn

PHP:  class MyError extends RuntimeException {}
来源：http://px.colortex.cn

JS:   class MyError extends Error {}
来源：http://lj.colortex.cn

TS:   class MyError extends Error {}
来源：http://ac.haigaiapp.cn

Java: class MyException extends RuntimeException {}
来源：http://ys.chemitech.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://di.9csxet.cn

Ruby: class MyError < StandardError; end
来源：http://ke.shtwfgs.cn

C#:   class MyException : Exception {}
来源：http://qx.shtwfgs.cn

[H05] 捕获特定类型
来源：http://wj.szsharing.cn

Py:   except ValueError as e:
来源：http://lj.szxytkj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bx.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://au.nszjky.cn

TS:   if (e instanceof TypeError) {}
来源：http://sv.haigaiapp.cn

Java: catch (IOException | SQLException e) {}
来源：http://dn.panjiajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://kz.hnjuh.cn

Ruby: rescue ArgumentError => e
来源：http://zz.chemitech.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iw.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://ov.yuntaijiaju.cn

Py:   value = d.get("k") or default
来源：http://sd.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wj.szsharing.cn

JS:   obj?.a?.b;  d ?? default
来源：http://op.colortex.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fa.jianghongdianzi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://we.shtwfgs.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yi.haigaiapp.cn

Ruby: d&.dig(:a, :b)
来源：http://bk.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://zl.szsharing.cn

[H07] 断言
来源：http://md.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://ek.shxzskj.cn

PHP:  assert($x > 0);
来源：http://mv.gzmigu.cn

JS:   console.assert(x > 0);
来源：http://ar.shxzukj.cn

TS:   console.assert(x > 0);
来源：http://kw.nszjky.cn

Java: assert x > 0 : "必须为正";
来源：http://ie.bjjhwx.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xm.nszjky.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xr.yuntaijiaju.cn

C#:   Debug.Assert(x > 0);
来源：http://uf.yuexingan06.cn

[H08] 获取错误信息与堆栈
来源：http://gj.gzmigu.cn

Py:   str(e);  traceback.format_exc()
来源：http://xm.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ay.521024.cn

JS:   e.message;  e.stack
来源：http://zt.hnjuh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://uu.newstarts.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qr.szxytkj.cn

Go:   err.Error()
来源：http://vg.colortex.cn

Ruby: e.message;  e.backtrace
来源：http://pp.asd995.cn

C#:   e.Message;  e.StackTrace
来源：http://ie.hahajie.cn

[H09] 带错误码的异常
来源：http://sf.huixiangedu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nz.newstarts.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zv.szsharing.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jb.nszjky.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yg.shxzukj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ut.szxytkj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gu.asd995.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ra.huixinmuqiang.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://le.muxihuayi.cn

[H10] 资源自动释放
来源：http://vq.yuexingan06.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wb.newstarts.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gi.bookmarksfly.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lf.asd995.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yr.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vd.nicolike.cn

Go:   defer f.Close()
来源：http://br.nszjky.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://or.lnxyls.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fh.lnxyls.cn

================================================================================
来源：http://uo.hahajie.cn

I. 正则表达式
来源：http://ul.shxzskj.cn

================================================================================
来源：http://ir.colortex.cn

[I01] 判断是否匹配
来源：http://er.yuntaijiaju.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ml.muxihuayi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://to.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://wb.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://eo.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://jj.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vl.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://ad.jctech888.com.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xl.yuexingan06.cn

[I02] 提取所有匹配
来源：http://dw.huixinmuqiang.cn

Py:   re.findall(r"\d+", s)
来源：http://bi.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ql.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fb.haigaiapp.cn

TS:   s.match(/\d+/g)
来源：http://rq.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tz.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://et.gzmigu.cn

Ruby: s.scan(/\d+/)
来源：http://ko.shxzukj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://oo.hahajie.cn

[I03] 提取捕获分组
来源：http://vb.chemitech.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://id.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sz.wgjwhj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bc.huanxung.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zt.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gr.yuexingan06.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://az.hnjuh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mn.szsharing.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://tz.jianghongdianzi.cn

[I04] 正则替换
来源：http://pa.asd995.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wf.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ym.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kv.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://gf.yuntaijiaju.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ku.szxytkj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://eu.huixinmuqiang.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ms.chemitech.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fh.hnjuh.cn

[I05] 按正则拆分
来源：http://sj.9csxet.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lt.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ya.521024.cn

JS:   s.split(/\s*,\s*/)
来源：http://su.9csxet.cn

TS:   s.split(/\s*,\s*/)
来源：http://rp.yuntaijiaju.cn

Java: s.split("\\s*,\\s*")
来源：http://qe.nszjky.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://re.shxzskj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ks.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ly.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nw.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fn.shtwfgs.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ja.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ss.hahajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nn.gzmigu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ug.szsharing.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://mo.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ed.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ss.shxzukj.cn

[I07] 忽略大小写与多行模式
来源：http://uo.jianghongdianzi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iw.bjjhwx.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ag.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cc.nicolike.cn

TS:   /error/gim
来源：http://cc.chemitech.net.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mb.szxytkj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://yo.huixiangedu.cn

Ruby: s.scan(/error/i)
来源：http://rh.yuntaijiaju.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://se.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://zc.asd995.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://it.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hd.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dh.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cp.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zf.nicolike.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gw.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yo.huixiangedu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wb.yuntaijiaju.cn

================================================================================
来源：http://ha.panjiajie.cn

J. 日期与时间
来源：http://ac.shxzskj.cn

================================================================================
来源：http://ul.bjjhwx.cn

[J01] 获取当前时间
来源：http://ys.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tf.bjjhwx.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rd.hahajie.cn

JS:   new Date();  Date.now()
来源：http://au.wgjwhj.cn

TS:   new Date();  Date.now()
来源：http://cs.lnxyls.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://uy.shxzskj.cn

Go:   time.Now()
来源：http://pn.yuntaijiaju.cn

Ruby: Time.now
来源：http://eg.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yy.9csxet.cn

[J02] 格式化输出
来源：http://nq.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fh.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mq.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xs.colortex.cn

TS:   d.toISOString()
来源：http://kv.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dr.huixiangedu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wz.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wj.muxihuayi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hu.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://re.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gp.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ao.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://rs.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://vl.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tv.521024.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wr.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://et.bookmarksfly.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://di.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://wh.yuntaijiaju.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://re.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://op.yuexingan06.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ke.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fv.haigaiapp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jv.yuexingan06.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oj.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://uq.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ox.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://xm.521024.cn

Py:   now + timedelta(days=7)
来源：http://rp.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uk.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nf.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ht.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://tb.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qe.newstarts.cn

Ruby: Time.now + 7 * 86400
来源：http://za.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://og.haigaiapp.cn

[J06] 计算两时间之差
来源：http://he.bookmarksfly.cn

Py:   (end - start).total_seconds()
来源：http://rq.newstarts.cn

PHP:  $end->diff($start)->days;
来源：http://iq.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://iu.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qk.chemitech.net.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ja.huixiangedu.cn

Go:   end.Sub(start).Hours()
来源：http://jh.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://wg.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://wp.huanxung.cn


<!-- 参考信息 -->