代发 wailian999

TS:   public / protected / private
来源：http://uj.521024.cn

Java: public / protected / private / 默认包级
来源：http://ak.bjjhwx.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vk.szxytkj.cn

Ruby: public / protected / private
来源：http://eb.huixiangedu.cn

C#:   public / protected / private / internal
来源：http://up.huixinmuqiang.cn

[G11] getter / setter
来源：http://to.9csxet.cn

Py:   @property 与 @x.setter
来源：http://sg.colortex.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://uz.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://yg.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://nw.nicolike.cn

Java: public String getName() { return name; }
来源：http://as.hnjuh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ud.gzmigu.cn

Ruby: attr_accessor :name
来源：http://kv.lnxyls.cn

C#:   public string Name { get; set; }
来源：http://ps.haigaiapp.cn

[G12] 对象转字符串
来源：http://mi.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://fk.szxytkj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wn.chemitech.net.cn

JS:   toString() { return this.name; }
来源：http://al.asd995.cn

TS:   toString(): string { return this.name; }
来源：http://dx.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://qz.9csxet.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ap.szsharing.cn

Ruby: def to_s; @name; end
来源：http://ds.nszjky.cn

C#:   public override string ToString() => Name;
来源：http://kb.nszjky.cn

[G13] 判断对象类型
来源：http://ve.chemitech.net.cn

Py:   isinstance(u, User)
来源：http://rk.huixinmuqiang.cn

PHP:  $u instanceof User
来源：http://jy.shxzskj.cn

JS:   u instanceof User
来源：http://ux.bjjhwx.cn

TS:   u instanceof User
来源：http://yb.newstarts.cn

Java: u instanceof User
来源：http://op.colortex.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://vv.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://mh.jianghongdianzi.cn

C#:   u is User
来源：http://ko.hahajie.cn

[G14] 数据类 / record
来源：http://ut.521024.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nl.9csxet.cn

PHP:  // 用 readonly 属性模拟
来源：http://qm.nszjky.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cz.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://wt.newstarts.cn

Java: record User(String name, int age) {}
来源：http://mn.muxihuayi.cn

Go:   type User struct { Name string; Age int }
来源：http://rn.bookmarksfly.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://il.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://po.shxzukj.cn

[G15] 枚举
来源：http://tq.gzmigu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yv.jctech888.com.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pk.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ps.9csxet.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xq.asd995.cn

Java: enum Color { RED, GREEN }
来源：http://id.521024.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ew.chemitech.net.cn

Ruby: Color = %i[red green].freeze
来源：http://si.yuexingan06.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jr.shxzskj.cn

[G16] 对象转数组 / 字典
来源：http://vn.9csxet.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://la.huixinmuqiang.cn

PHP:  get_object_vars($obj);
来源：http://pw.szsharing.cn

JS:   Object.entries(obj)
来源：http://qj.9csxet.cn

TS:   Object.entries(obj)
来源：http://za.bjjhwx.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ej.muxihuayi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yu.wgjwhj.cn

Ruby: obj.instance_variables
来源：http://eb.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://al.newstarts.cn

================================================================================
来源：http://qn.hahajie.cn

H. 异常与错误处理
来源：http://mk.bjjhwx.cn

================================================================================
来源：http://fg.521024.cn

[H01] try / catch 基础
来源：http://cc.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://iq.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://og.jctech888.com.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sz.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ig.haigaiapp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dt.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nf.shxzskj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ec.nszjky.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://lj.nszjky.cn

[H02] finally / ensure 收尾
来源：http://dg.shtwfgs.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rd.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ak.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xx.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://mq.hahajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://me.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ku.asd995.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dt.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ya.shxzukj.cn

[H03] 主动抛出异常
来源：http://dz.huanxung.cn

Py:   raise ValueError("错误信息")
来源：http://xc.wgjwhj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xc.shtwfgs.cn

JS:   throw new Error("错误信息");
来源：http://ik.muxihuayi.cn

TS:   throw new Error("错误信息");
来源：http://bv.jctech888.com.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jo.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nm.bjjhwx.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hw.colortex.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ch.shxzukj.cn

[H04] 自定义异常类型
来源：http://ns.jianghongdianzi.cn

Py:   class MyError(Exception): pass
来源：http://fj.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://jl.muxihuayi.cn

JS:   class MyError extends Error {}
来源：http://dg.szxytkj.cn

TS:   class MyError extends Error {}
来源：http://wi.lnxyls.cn

Java: class MyException extends RuntimeException {}
来源：http://bv.wgjwhj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kp.lnxyls.cn

Ruby: class MyError < StandardError; end
来源：http://hf.shxzukj.cn

C#:   class MyException : Exception {}
来源：http://kk.shxzskj.cn

[H05] 捕获特定类型
来源：http://sv.521024.cn

Py:   except ValueError as e:
来源：http://lm.jianghongdianzi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://qi.shtwfgs.cn

JS:   if (e instanceof TypeError) {}
来源：http://ay.chemitech.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://jn.9csxet.cn

Java: catch (IOException | SQLException e) {}
来源：http://nn.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://eh.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://sn.bjjhwx.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://of.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://ih.yuexingan06.cn

Py:   value = d.get("k") or default
来源：http://lk.bjjhwx.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ai.chemitech.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hp.yuntaijiaju.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gt.shtwfgs.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://am.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://uw.muxihuayi.cn

Ruby: d&.dig(:a, :b)
来源：http://tf.newstarts.cn

C#:   obj?.A?.B ?? default
来源：http://jm.jianghongdianzi.cn

[H07] 断言
来源：http://mv.huanxung.cn

Py:   assert x > 0, "必须为正"
来源：http://fz.shxzskj.cn

PHP:  assert($x > 0);
来源：http://yd.jianghongdianzi.cn

JS:   console.assert(x > 0);
来源：http://op.jianghongdianzi.cn

TS:   console.assert(x > 0);
来源：http://dv.bjjhwx.cn

Java: assert x > 0 : "必须为正";
来源：http://bb.gzmigu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jc.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lw.szxytkj.cn

C#:   Debug.Assert(x > 0);
来源：http://ws.newstarts.cn

[H08] 获取错误信息与堆栈
来源：http://oc.huanxung.cn

Py:   str(e);  traceback.format_exc()
来源：http://cu.wgjwhj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ru.hnjuh.cn

JS:   e.message;  e.stack
来源：http://ca.panjiajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bi.szsharing.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qs.huixinmuqiang.cn

Go:   err.Error()
来源：http://wn.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://zh.huixinmuqiang.cn

C#:   e.Message;  e.StackTrace
来源：http://ad.haigaiapp.cn

[H09] 带错误码的异常
来源：http://pi.hahajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bn.hnjuh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zl.chemitech.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yj.szxytkj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ml.yuntaijiaju.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jw.bjjhwx.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xr.yuntaijiaju.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jz.gzmigu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vf.521024.cn

[H10] 资源自动释放
来源：http://sh.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ov.hahajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nb.9csxet.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xl.muxihuayi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hv.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vy.yuntaijiaju.cn

Go:   defer f.Close()
来源：http://gi.hahajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mu.asd995.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://jp.nszjky.cn

================================================================================
来源：http://qw.yuntaijiaju.cn

I. 正则表达式
来源：http://lm.asd995.cn

================================================================================
来源：http://tp.shxzukj.cn

[I01] 判断是否匹配
来源：http://zp.haigaiapp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ju.521024.cn

PHP:  preg_match('/\d+/', $s);
来源：http://un.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://tx.panjiajie.cn

TS:   /\d+/.test(s)
来源：http://wd.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ym.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://am.nszjky.cn

Ruby: s.match?(/\d+/)
来源：http://mb.yuntaijiaju.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://to.nszjky.cn

[I02] 提取所有匹配
来源：http://an.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://xy.yuntaijiaju.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rq.bjjhwx.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zh.huixiangedu.cn

TS:   s.match(/\d+/g)
来源：http://eh.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cw.nszjky.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ea.521024.cn

Ruby: s.scan(/\d+/)
来源：http://iu.shxzukj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ez.szsharing.cn

[I03] 提取捕获分组
来源：http://wj.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mk.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mc.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xi.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uv.colortex.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fm.yuntaijiaju.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://jc.szsharing.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ho.bookmarksfly.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hh.panjiajie.cn

[I04] 正则替换
来源：http://ti.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rb.haigaiapp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://es.nicolike.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jt.jianghongdianzi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ke.haigaiapp.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vk.jctech888.com.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://rz.haigaiapp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ns.panjiajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cs.9csxet.cn

[I05] 按正则拆分
来源：http://pl.panjiajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dt.yuntaijiaju.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://oj.colortex.cn

JS:   s.split(/\s*,\s*/)
来源：http://ak.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://zs.lnxyls.cn

Java: s.split("\\s*,\\s*")
来源：http://hv.gzmigu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ky.shxzskj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cn.bookmarksfly.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wn.panjiajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rt.bookmarksfly.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pr.newstarts.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nt.szxytkj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bp.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hx.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dz.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uo.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zw.bjjhwx.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tv.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://lf.muxihuayi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ad.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fu.nicolike.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ap.yuntaijiaju.cn

TS:   /error/gim
来源：http://sv.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://qc.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eo.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://cf.nicolike.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://jy.szsharing.cn

[I08] 贪婪与非贪婪匹配
来源：http://is.newstarts.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oj.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zd.nicolike.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ut.lnxyls.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uu.hnjuh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://eu.hnjuh.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qt.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ux.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tw.huixinmuqiang.cn

================================================================================
来源：http://pi.muxihuayi.cn

J. 日期与时间
来源：http://to.szxytkj.cn

================================================================================
来源：http://cj.shxzukj.cn

[J01] 获取当前时间
来源：http://gu.hnjuh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://so.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://up.asd995.cn

JS:   new Date();  Date.now()
来源：http://ee.hahajie.cn

TS:   new Date();  Date.now()
来源：http://zm.chemitech.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ua.yuexingan06.cn

Go:   time.Now()
来源：http://ou.bjjhwx.cn

Ruby: Time.now
来源：http://qf.bjjhwx.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bm.newstarts.cn

[J02] 格式化输出
来源：http://cm.yuexingan06.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wo.szsharing.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://jn.521024.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fv.huanxung.cn

TS:   d.toISOString()
来源：http://eq.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kq.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yb.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yv.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yz.shxzskj.cn

[J03] 字符串解析为日期
来源：http://hk.nicolike.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sc.nicolike.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mb.huixinmuqiang.cn

JS:   new Date("2024-01-02")
来源：http://wi.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://nx.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://of.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cf.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://la.bjjhwx.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xa.shxzukj.cn

[J04] 时间戳与日期互转
来源：http://pm.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zl.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mr.yuexingan06.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bj.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vr.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://od.bookmarksfly.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jm.asd995.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mj.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://bw.asd995.cn

[J05] 时间加减（加 7 天）
来源：http://ez.newstarts.cn

Py:   now + timedelta(days=7)
来源：http://qj.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://rb.huixiangedu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vk.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zl.huixiangedu.cn

Java: LocalDate.now().plusDays(7)
来源：http://bn.yuexingan06.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zt.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://ch.lnxyls.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zu.huixiangedu.cn

[J06] 计算两时间之差
来源：http://th.colortex.cn

Py:   (end - start).total_seconds()
来源：http://tt.shxzskj.cn

PHP:  $end->diff($start)->days;
来源：http://ns.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hj.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zb.wgjwhj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xj.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://lu.wgjwhj.cn

Ruby: end - start                 # 返回秒数
来源：http://zw.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://yq.szsharing.cn

[J07] 比较两个日期
来源：http://za.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://lz.yuntaijiaju.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nn.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ue.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kh.yuexingan06.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://do.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://le.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bk.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://sz.9csxet.cn

[J08] 提取年月日与星期
来源：http://ok.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vx.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://no.huixiangedu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ug.yuntaijiaju.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hp.bjjhwx.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mm.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fo.yuexingan06.cn


<!-- 参考信息 -->