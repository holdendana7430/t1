代发 wailian999

C#:   public / protected / private / internal
来源：http://rb.chemitech.net.cn

[G11] getter / setter
来源：http://ru.yuexingan06.cn

Py:   @property 与 @x.setter
来源：http://co.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vu.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://lk.bjjhwx.cn

TS:   get name(): string { return this._name; }
来源：http://il.panjiajie.cn

Java: public String getName() { return name; }
来源：http://xf.nszjky.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ze.newstarts.cn

Ruby: attr_accessor :name
来源：http://kn.colortex.cn

C#:   public string Name { get; set; }
来源：http://po.chemitech.net.cn

[G12] 对象转字符串
来源：http://wy.shxzskj.cn

Py:   def __str__(self): return self.name
来源：http://sg.muxihuayi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://qq.521024.cn

JS:   toString() { return this.name; }
来源：http://di.hahajie.cn

TS:   toString(): string { return this.name; }
来源：http://rt.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://ij.jctech888.com.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ca.jianghongdianzi.cn

Ruby: def to_s; @name; end
来源：http://hf.jctech888.com.cn

C#:   public override string ToString() => Name;
来源：http://sm.521024.cn

[G13] 判断对象类型
来源：http://nf.panjiajie.cn

Py:   isinstance(u, User)
来源：http://zx.nszjky.cn

PHP:  $u instanceof User
来源：http://fe.shxzskj.cn

JS:   u instanceof User
来源：http://xi.wgjwhj.cn

TS:   u instanceof User
来源：http://pr.muxihuayi.cn

Java: u instanceof User
来源：http://zm.gzmigu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ap.521024.cn

Ruby: u.is_a?(User)
来源：http://wu.hahajie.cn

C#:   u is User
来源：http://qa.gzmigu.cn

[G14] 数据类 / record
来源：http://er.chemitech.net.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bx.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://vc.gzmigu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://do.bjjhwx.cn

TS:   type User = { name: string; age: number };
来源：http://bc.hahajie.cn

Java: record User(String name, int age) {}
来源：http://nd.muxihuayi.cn

Go:   type User struct { Name string; Age int }
来源：http://qe.huanxung.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cm.colortex.cn

C#:   record User(string Name, int Age);
来源：http://dz.huixinmuqiang.cn

[G15] 枚举
来源：http://hx.bjjhwx.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tq.shxzukj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qn.hahajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vc.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ah.lnxyls.cn

Java: enum Color { RED, GREEN }
来源：http://pf.shtwfgs.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fe.hnjuh.cn

Ruby: Color = %i[red green].freeze
来源：http://wf.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vf.jctech888.com.cn

[G16] 对象转数组 / 字典
来源：http://sf.bookmarksfly.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://el.chemitech.net.cn

PHP:  get_object_vars($obj);
来源：http://wn.nszjky.cn

JS:   Object.entries(obj)
来源：http://zr.szsharing.cn

TS:   Object.entries(obj)
来源：http://gx.hahajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dd.szsharing.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ym.colortex.cn

Ruby: obj.instance_variables
来源：http://rk.521024.cn

C#:   // 用反射或 System.Text.Json
来源：http://gc.chemitech.net.cn

================================================================================
来源：http://nt.bookmarksfly.cn

H. 异常与错误处理
来源：http://co.huixinmuqiang.cn

================================================================================
来源：http://jk.haigaiapp.cn

[H01] try / catch 基础
来源：http://zu.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qb.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ot.bookmarksfly.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://df.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bm.huanxung.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qv.muxihuayi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hc.jianghongdianzi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fe.gzmigu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nw.huixiangedu.cn

[H02] finally / ensure 收尾
来源：http://wb.nicolike.cn

Py:   try: f()⏎finally: cleanup()
来源：http://el.9csxet.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://py.jctech888.com.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ea.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qn.lnxyls.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ux.yuexingan06.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jc.muxihuayi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gm.shtwfgs.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qa.nicolike.cn

[H03] 主动抛出异常
来源：http://sa.panjiajie.cn

Py:   raise ValueError("错误信息")
来源：http://ov.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ra.bjjhwx.cn

JS:   throw new Error("错误信息");
来源：http://by.haigaiapp.cn

TS:   throw new Error("错误信息");
来源：http://ir.newstarts.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://cw.szxytkj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zu.huixinmuqiang.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gi.jianghongdianzi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://dn.shxzskj.cn

[H04] 自定义异常类型
来源：http://sa.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://tx.huixinmuqiang.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zo.colortex.cn

JS:   class MyError extends Error {}
来源：http://ji.shtwfgs.cn

TS:   class MyError extends Error {}
来源：http://oj.szsharing.cn

Java: class MyException extends RuntimeException {}
来源：http://bi.gzmigu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://th.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://xr.wgjwhj.cn

C#:   class MyException : Exception {}
来源：http://bn.shxzukj.cn

[H05] 捕获特定类型
来源：http://tf.haigaiapp.cn

Py:   except ValueError as e:
来源：http://mf.hahajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ds.yuntaijiaju.cn

JS:   if (e instanceof TypeError) {}
来源：http://wn.huixinmuqiang.cn

TS:   if (e instanceof TypeError) {}
来源：http://jb.nszjky.cn

Java: catch (IOException | SQLException e) {}
来源：http://gt.szxytkj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qt.9csxet.cn

Ruby: rescue ArgumentError => e
来源：http://xf.asd995.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hc.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://vh.asd995.cn

Py:   value = d.get("k") or default
来源：http://sz.wgjwhj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sl.szxytkj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rn.gzmigu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://up.huixiangedu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kr.panjiajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dg.yuexingan06.cn

Ruby: d&.dig(:a, :b)
来源：http://gr.newstarts.cn

C#:   obj?.A?.B ?? default
来源：http://hx.hnjuh.cn

[H07] 断言
来源：http://po.gzmigu.cn

Py:   assert x > 0, "必须为正"
来源：http://ax.jianghongdianzi.cn

PHP:  assert($x > 0);
来源：http://sm.huixiangedu.cn

JS:   console.assert(x > 0);
来源：http://ud.nszjky.cn

TS:   console.assert(x > 0);
来源：http://go.bjjhwx.cn

Java: assert x > 0 : "必须为正";
来源：http://lr.bookmarksfly.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xv.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cf.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://yi.huixinmuqiang.cn

[H08] 获取错误信息与堆栈
来源：http://xi.huanxung.cn

Py:   str(e);  traceback.format_exc()
来源：http://nc.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://um.jctech888.com.cn

JS:   e.message;  e.stack
来源：http://gy.muxihuayi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hg.huanxung.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ug.asd995.cn

Go:   err.Error()
来源：http://ke.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://qr.wgjwhj.cn

C#:   e.Message;  e.StackTrace
来源：http://ye.asd995.cn

[H09] 带错误码的异常
来源：http://tt.521024.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fm.hahajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jp.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gq.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uj.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hh.huixinmuqiang.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://na.bookmarksfly.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zo.chemitech.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://mu.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://eo.haigaiapp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://je.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rb.huanxung.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xw.haigaiapp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vr.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ul.nszjky.cn

Go:   defer f.Close()
来源：http://cg.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lo.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hm.colortex.cn

================================================================================
来源：http://ud.jianghongdianzi.cn

I. 正则表达式
来源：http://fc.nicolike.cn

================================================================================
来源：http://wk.szxytkj.cn

[I01] 判断是否匹配
来源：http://wj.hnjuh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ia.9csxet.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hx.9csxet.cn

JS:   /\d+/.test(s)
来源：http://ue.newstarts.cn

TS:   /\d+/.test(s)
来源：http://tf.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ti.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sm.asd995.cn

Ruby: s.match?(/\d+/)
来源：http://zt.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zm.colortex.cn

[I02] 提取所有匹配
来源：http://og.asd995.cn

Py:   re.findall(r"\d+", s)
来源：http://lw.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yr.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ah.nszjky.cn

TS:   s.match(/\d+/g)
来源：http://bz.521024.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gu.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://og.panjiajie.cn

Ruby: s.scan(/\d+/)
来源：http://al.newstarts.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qt.szxytkj.cn

[I03] 提取捕获分组
来源：http://ea.wgjwhj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sm.yuexingan06.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://eg.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://up.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gd.lnxyls.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ce.muxihuayi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://un.521024.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://me.huixiangedu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zi.newstarts.cn

[I04] 正则替换
来源：http://xv.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rp.nicolike.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ag.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xf.hnjuh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ta.yuntaijiaju.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ly.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ha.huanxung.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://eg.lnxyls.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kq.huixinmuqiang.cn

[I05] 按正则拆分
来源：http://zu.huixiangedu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jt.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xv.huixinmuqiang.cn

JS:   s.split(/\s*,\s*/)
来源：http://fj.jctech888.com.cn

TS:   s.split(/\s*,\s*/)
来源：http://ah.szxytkj.cn

Java: s.split("\\s*,\\s*")
来源：http://bu.huanxung.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zr.colortex.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ay.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cz.chemitech.net.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wf.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ac.bjjhwx.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sw.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tm.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ha.hnjuh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fh.yuexingan06.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zf.huixinmuqiang.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nh.yuexingan06.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ds.szxytkj.cn

[I07] 忽略大小写与多行模式
来源：http://lk.hnjuh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ki.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hl.huanxung.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qf.hahajie.cn

TS:   /error/gim
来源：http://tt.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jx.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cc.nszjky.cn

Ruby: s.scan(/error/i)
来源：http://wz.hnjuh.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bi.shxzukj.cn

[I08] 贪婪与非贪婪匹配
来源：http://pr.hnjuh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://aj.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gi.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://iz.wgjwhj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bx.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ty.jctech888.com.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ec.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ww.hahajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://rs.shxzskj.cn

================================================================================
来源：http://de.bjjhwx.cn

J. 日期与时间
来源：http://yw.gzmigu.cn

================================================================================
来源：http://kv.shxzskj.cn

[J01] 获取当前时间
来源：http://vb.szsharing.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://lx.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jm.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://yq.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://lt.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://yo.jctech888.com.cn

Go:   time.Now()
来源：http://yt.huanxung.cn

Ruby: Time.now
来源：http://dl.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tv.asd995.cn

[J02] 格式化输出
来源：http://hm.szsharing.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ka.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tk.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://un.bookmarksfly.cn

TS:   d.toISOString()
来源：http://tp.hnjuh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mk.colortex.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ee.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qy.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fz.shxzskj.cn

[J03] 字符串解析为日期
来源：http://so.yuexingan06.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://at.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qs.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://gc.huixiangedu.cn

TS:   new Date("2024-01-02")
来源：http://jl.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dp.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://yg.chemitech.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://zv.bookmarksfly.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lw.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://ej.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cl.wgjwhj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fo.asd995.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qw.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ew.haigaiapp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mg.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ab.521024.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://md.huixinmuqiang.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yz.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://tx.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://ux.nszjky.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ad.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wf.colortex.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yk.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://lo.shxzskj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yq.9csxet.cn

Ruby: Time.now + 7 * 86400
来源：http://uh.bookmarksfly.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qm.newstarts.cn

[J06] 计算两时间之差
来源：http://pj.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://zn.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://kb.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cy.bookmarksfly.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://to.shxzukj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://st.521024.cn

Go:   end.Sub(start).Hours()
来源：http://gw.shxzskj.cn

Ruby: end - start                 # 返回秒数
来源：http://fu.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://gn.yuexingan06.cn

[J07] 比较两个日期
来源：http://oc.hnjuh.cn

Py:   d1 < d2;  d1 == d2
来源：http://jn.muxihuayi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cn.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vq.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://us.jianghongdianzi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://io.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mn.szxytkj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://po.haigaiapp.cn

C#:   d1 < d2;  d1 == d2
来源：http://oh.yuntaijiaju.cn

[J08] 提取年月日与星期
来源：http://it.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ig.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gy.szxytkj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uw.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://el.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ps.shtwfgs.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mo.nicolike.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mx.huanxung.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ae.9csxet.cn

[J09] 时区处理
来源：http://xw.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ia.hnjuh.cn


<!-- 参考信息 -->