代发 wailian999

JS:   get name() { return this._name; }
来源：http://ee.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://hz.asd995.cn

Java: public String getName() { return name; }
来源：http://kb.521024.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xh.huanxung.cn

Ruby: attr_accessor :name
来源：http://tb.nicolike.cn

C#:   public string Name { get; set; }
来源：http://us.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://tr.szxytkj.cn

Py:   def __str__(self): return self.name
来源：http://vb.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://kp.wgjwhj.cn

JS:   toString() { return this.name; }
来源：http://pu.jctech888.com.cn

TS:   toString(): string { return this.name; }
来源：http://dg.huixinmuqiang.cn

Java: @Override public String toString() { return name; }
来源：http://vz.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ww.asd995.cn

Ruby: def to_s; @name; end
来源：http://iq.newstarts.cn

C#:   public override string ToString() => Name;
来源：http://yr.521024.cn

[G13] 判断对象类型
来源：http://mx.szsharing.cn

Py:   isinstance(u, User)
来源：http://ft.shxzukj.cn

PHP:  $u instanceof User
来源：http://zf.szxytkj.cn

JS:   u instanceof User
来源：http://up.chemitech.net.cn

TS:   u instanceof User
来源：http://wd.yuntaijiaju.cn

Java: u instanceof User
来源：http://wv.chemitech.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rh.huixinmuqiang.cn

Ruby: u.is_a?(User)
来源：http://mu.wgjwhj.cn

C#:   u is User
来源：http://rw.gzmigu.cn

[G14] 数据类 / record
来源：http://fd.shxzskj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://oh.huixiangedu.cn

PHP:  // 用 readonly 属性模拟
来源：http://rq.panjiajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://bi.colortex.cn

TS:   type User = { name: string; age: number };
来源：http://pw.huanxung.cn

Java: record User(String name, int age) {}
来源：http://wr.lnxyls.cn

Go:   type User struct { Name string; Age int }
来源：http://xe.huixinmuqiang.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lf.lnxyls.cn

C#:   record User(string Name, int Age);
来源：http://nt.szxytkj.cn

[G15] 枚举
来源：http://mm.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pn.asd995.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xm.huanxung.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zf.gzmigu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ei.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://iu.521024.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kt.colortex.cn

Ruby: Color = %i[red green].freeze
来源：http://xs.nszjky.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nz.huanxung.cn

[G16] 对象转数组 / 字典
来源：http://xp.nszjky.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xw.muxihuayi.cn

PHP:  get_object_vars($obj);
来源：http://ax.huixiangedu.cn

JS:   Object.entries(obj)
来源：http://ez.huixinmuqiang.cn

TS:   Object.entries(obj)
来源：http://xy.huixiangedu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://po.jctech888.com.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ff.bjjhwx.cn

Ruby: obj.instance_variables
来源：http://ic.hnjuh.cn

C#:   // 用反射或 System.Text.Json
来源：http://xl.huixinmuqiang.cn

================================================================================
来源：http://bf.wgjwhj.cn

H. 异常与错误处理
来源：http://ou.wgjwhj.cn

================================================================================
来源：http://mv.9csxet.cn

[H01] try / catch 基础
来源：http://xl.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ch.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qk.huanxung.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zq.muxihuayi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pb.hahajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pa.wgjwhj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://cs.szxytkj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://gu.shxzskj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vi.szxytkj.cn

[H02] finally / ensure 收尾
来源：http://yc.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ry.asd995.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mk.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cg.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ug.wgjwhj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sn.wgjwhj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sb.jctech888.com.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://eg.nicolike.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pw.jctech888.com.cn

[H03] 主动抛出异常
来源：http://rd.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://ko.szsharing.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kk.haigaiapp.cn

JS:   throw new Error("错误信息");
来源：http://bb.9csxet.cn

TS:   throw new Error("错误信息");
来源：http://op.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://iu.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ch.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://sv.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://or.jianghongdianzi.cn

[H04] 自定义异常类型
来源：http://sa.bjjhwx.cn

Py:   class MyError(Exception): pass
来源：http://jw.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yq.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://yi.521024.cn

TS:   class MyError extends Error {}
来源：http://ng.hahajie.cn

Java: class MyException extends RuntimeException {}
来源：http://hi.shxzukj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dv.hnjuh.cn

Ruby: class MyError < StandardError; end
来源：http://fy.hnjuh.cn

C#:   class MyException : Exception {}
来源：http://di.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://hw.haigaiapp.cn

Py:   except ValueError as e:
来源：http://xp.hahajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://lh.haigaiapp.cn

JS:   if (e instanceof TypeError) {}
来源：http://tw.shtwfgs.cn

TS:   if (e instanceof TypeError) {}
来源：http://dh.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://ku.shxzukj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xf.haigaiapp.cn

Ruby: rescue ArgumentError => e
来源：http://sy.9csxet.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nt.newstarts.cn

[H06] 可选值 / 空值安全访问
来源：http://bb.shxzskj.cn

Py:   value = d.get("k") or default
来源：http://mg.hnjuh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nc.haigaiapp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rq.nicolike.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zg.nicolike.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xp.shxzukj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://th.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://op.huixiangedu.cn

C#:   obj?.A?.B ?? default
来源：http://pe.9csxet.cn

[H07] 断言
来源：http://df.shxzskj.cn

Py:   assert x > 0, "必须为正"
来源：http://ou.bjjhwx.cn

PHP:  assert($x > 0);
来源：http://mz.newstarts.cn

JS:   console.assert(x > 0);
来源：http://wd.shxzukj.cn

TS:   console.assert(x > 0);
来源：http://lc.panjiajie.cn

Java: assert x > 0 : "必须为正";
来源：http://pz.haigaiapp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wa.colortex.cn

Ruby: raise "必须为正" unless x > 0
来源：http://wj.bjjhwx.cn

C#:   Debug.Assert(x > 0);
来源：http://we.bjjhwx.cn

[H08] 获取错误信息与堆栈
来源：http://wi.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://px.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bn.huixinmuqiang.cn

JS:   e.message;  e.stack
来源：http://ly.wgjwhj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jq.panjiajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mu.hnjuh.cn

Go:   err.Error()
来源：http://yd.asd995.cn

Ruby: e.message;  e.backtrace
来源：http://qa.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://lb.panjiajie.cn

[H09] 带错误码的异常
来源：http://dv.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nw.colortex.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lt.newstarts.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qg.shtwfgs.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://no.bjjhwx.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dr.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://dh.chemitech.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zl.huixinmuqiang.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rt.huixiangedu.cn

[H10] 资源自动释放
来源：http://va.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://od.jianghongdianzi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ej.521024.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qq.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hp.huixinmuqiang.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://cn.yuntaijiaju.cn

Go:   defer f.Close()
来源：http://lh.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wf.jctech888.com.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zw.521024.cn

================================================================================
来源：http://li.shxzskj.cn

I. 正则表达式
来源：http://cz.jctech888.com.cn

================================================================================
来源：http://tp.chemitech.net.cn

[I01] 判断是否匹配
来源：http://fj.haigaiapp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ui.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://uo.521024.cn

JS:   /\d+/.test(s)
来源：http://iv.shxzskj.cn

TS:   /\d+/.test(s)
来源：http://kk.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fj.nicolike.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://co.yuexingan06.cn

Ruby: s.match?(/\d+/)
来源：http://ow.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bx.huixinmuqiang.cn

[I02] 提取所有匹配
来源：http://kb.yuexingan06.cn

Py:   re.findall(r"\d+", s)
来源：http://mp.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://co.yuntaijiaju.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://de.haigaiapp.cn

TS:   s.match(/\d+/g)
来源：http://hd.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xh.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tm.wgjwhj.cn

Ruby: s.scan(/\d+/)
来源：http://ud.521024.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://cf.shtwfgs.cn

[I03] 提取捕获分组
来源：http://ps.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ex.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ja.bjjhwx.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kx.asd995.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://js.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://us.gzmigu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://um.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wk.shxzukj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ht.jctech888.com.cn

[I04] 正则替换
来源：http://ys.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ex.nicolike.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://he.bookmarksfly.cn

JS:   s.replace(/\d+/g, "#")
来源：http://if.huanxung.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wt.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://to.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ez.muxihuayi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xh.newstarts.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ln.shxzskj.cn

[I05] 按正则拆分
来源：http://fw.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ag.shtwfgs.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jz.jctech888.com.cn

JS:   s.split(/\s*,\s*/)
来源：http://op.szxytkj.cn

TS:   s.split(/\s*,\s*/)
来源：http://er.muxihuayi.cn

Java: s.split("\\s*,\\s*")
来源：http://xm.shxzskj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pl.huixiangedu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gm.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ng.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://va.yuntaijiaju.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ua.yuexingan06.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://tl.bjjhwx.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vz.hahajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uv.yuexingan06.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://if.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sr.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ku.hahajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ef.asd995.cn

[I07] 忽略大小写与多行模式
来源：http://hy.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ii.chemitech.net.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ly.huixinmuqiang.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zp.szsharing.cn

TS:   /error/gim
来源：http://ms.muxihuayi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yk.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qf.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://lu.chemitech.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cb.colortex.cn

[I08] 贪婪与非贪婪匹配
来源：http://nj.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nt.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://np.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tf.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sx.asd995.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ct.colortex.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ve.huixiangedu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hp.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://al.colortex.cn

================================================================================
来源：http://kj.521024.cn

J. 日期与时间
来源：http://jt.9csxet.cn

================================================================================
来源：http://yg.chemitech.net.cn

[J01] 获取当前时间
来源：http://ob.wgjwhj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rn.9csxet.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gm.hahajie.cn

JS:   new Date();  Date.now()
来源：http://tn.haigaiapp.cn

TS:   new Date();  Date.now()
来源：http://dc.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://dy.newstarts.cn

Go:   time.Now()
来源：http://ak.huixiangedu.cn

Ruby: Time.now
来源：http://ai.9csxet.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fs.shtwfgs.cn

[J02] 格式化输出
来源：http://ul.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ae.hnjuh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://og.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yh.nszjky.cn

TS:   d.toISOString()
来源：http://bk.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ys.szsharing.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yt.521024.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oe.9csxet.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nd.hnjuh.cn

[J03] 字符串解析为日期
来源：http://eo.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://zr.szxytkj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jv.shxzukj.cn

JS:   new Date("2024-01-02")
来源：http://ei.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://iy.wgjwhj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dq.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zi.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://sr.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qw.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://vj.lnxyls.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ef.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ci.hahajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nc.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ic.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://le.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ct.hnjuh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ef.nicolike.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tz.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://cm.colortex.cn

Py:   now + timedelta(days=7)
来源：http://de.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://oe.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xr.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://km.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://dy.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://lo.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://cy.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://it.bjjhwx.cn

[J06] 计算两时间之差
来源：http://or.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://jf.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://dw.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oy.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xg.shtwfgs.cn

Java: Duration.between(start, end).toSeconds()
来源：http://oc.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://xw.nszjky.cn

Ruby: end - start                 # 返回秒数
来源：http://yt.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://bp.nicolike.cn

[J07] 比较两个日期
来源：http://py.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://bq.huanxung.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bo.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ul.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sq.jianghongdianzi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pr.gzmigu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://et.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://eo.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://oz.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://tl.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zh.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ch.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ge.jianghongdianzi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uf.panjiajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tk.szxytkj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ie.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cf.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://bp.colortex.cn

[J09] 时区处理
来源：http://rk.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mf.huixinmuqiang.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://el.nszjky.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dj.shtwfgs.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qn.9csxet.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zc.gzmigu.cn


<!-- 参考信息 -->