代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://ln.wgjwhj.cn

Ruby: def to_s; @name; end
来源：http://nl.asd995.cn

C#:   public override string ToString() => Name;
来源：http://fx.panjiajie.cn

[G13] 判断对象类型
来源：http://bx.jianghongdianzi.cn

Py:   isinstance(u, User)
来源：http://jc.bookmarksfly.cn

PHP:  $u instanceof User
来源：http://ec.yuexingan06.cn

JS:   u instanceof User
来源：http://gp.shtwfgs.cn

TS:   u instanceof User
来源：http://ke.yuexingan06.cn

Java: u instanceof User
来源：http://hs.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xj.newstarts.cn

Ruby: u.is_a?(User)
来源：http://hs.asd995.cn

C#:   u is User
来源：http://mk.nszjky.cn

[G14] 数据类 / record
来源：http://xl.bookmarksfly.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://so.szsharing.cn

PHP:  // 用 readonly 属性模拟
来源：http://bh.asd995.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fr.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://wb.gzmigu.cn

Java: record User(String name, int age) {}
来源：http://wi.shtwfgs.cn

Go:   type User struct { Name string; Age int }
来源：http://lk.muxihuayi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jq.huixinmuqiang.cn

C#:   record User(string Name, int Age);
来源：http://kz.szxytkj.cn

[G15] 枚举
来源：http://gv.bjjhwx.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ou.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rg.9csxet.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ww.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iu.shxzukj.cn

Java: enum Color { RED, GREEN }
来源：http://ut.shxzukj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lw.asd995.cn

Ruby: Color = %i[red green].freeze
来源：http://du.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vf.szxytkj.cn

[G16] 对象转数组 / 字典
来源：http://zq.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ul.wgjwhj.cn

PHP:  get_object_vars($obj);
来源：http://bd.hahajie.cn

JS:   Object.entries(obj)
来源：http://zi.yuexingan06.cn

TS:   Object.entries(obj)
来源：http://sy.gzmigu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ig.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ku.jctech888.com.cn

Ruby: obj.instance_variables
来源：http://ob.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://yj.shtwfgs.cn

================================================================================
来源：http://pt.bjjhwx.cn

H. 异常与错误处理
来源：http://vz.muxihuayi.cn

================================================================================
来源：http://cz.yuexingan06.cn

[H01] try / catch 基础
来源：http://kb.colortex.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://je.nszjky.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xm.huanxung.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ua.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://io.haigaiapp.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://iy.colortex.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://aa.haigaiapp.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bk.shtwfgs.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gx.bookmarksfly.cn

[H02] finally / ensure 收尾
来源：http://wj.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lv.huixinmuqiang.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vp.jianghongdianzi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bz.szxytkj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bt.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://nv.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ro.jianghongdianzi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ax.shxzukj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xe.shxzskj.cn

[H03] 主动抛出异常
来源：http://nl.colortex.cn

Py:   raise ValueError("错误信息")
来源：http://dr.huixinmuqiang.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fo.szsharing.cn

JS:   throw new Error("错误信息");
来源：http://ml.lnxyls.cn

TS:   throw new Error("错误信息");
来源：http://va.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xd.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sf.newstarts.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ci.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ix.gzmigu.cn

[H04] 自定义异常类型
来源：http://kn.yuntaijiaju.cn

Py:   class MyError(Exception): pass
来源：http://pz.yuntaijiaju.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mx.nszjky.cn

JS:   class MyError extends Error {}
来源：http://eu.huixiangedu.cn

TS:   class MyError extends Error {}
来源：http://vl.panjiajie.cn

Java: class MyException extends RuntimeException {}
来源：http://dp.huixiangedu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xn.szsharing.cn

Ruby: class MyError < StandardError; end
来源：http://bu.szxytkj.cn

C#:   class MyException : Exception {}
来源：http://zi.shxzukj.cn

[H05] 捕获特定类型
来源：http://er.nszjky.cn

Py:   except ValueError as e:
来源：http://td.bjjhwx.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ko.panjiajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://tg.asd995.cn

TS:   if (e instanceof TypeError) {}
来源：http://kf.lnxyls.cn

Java: catch (IOException | SQLException e) {}
来源：http://wm.bookmarksfly.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vj.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://hc.jianghongdianzi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sp.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://hr.hnjuh.cn

Py:   value = d.get("k") or default
来源：http://go.bjjhwx.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ap.9csxet.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ob.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tk.chemitech.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gk.nszjky.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xj.nicolike.cn

Ruby: d&.dig(:a, :b)
来源：http://ft.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://lj.bookmarksfly.cn

[H07] 断言
来源：http://xu.huixinmuqiang.cn

Py:   assert x > 0, "必须为正"
来源：http://bw.huixiangedu.cn

PHP:  assert($x > 0);
来源：http://by.jianghongdianzi.cn

JS:   console.assert(x > 0);
来源：http://ig.haigaiapp.cn

TS:   console.assert(x > 0);
来源：http://bl.wgjwhj.cn

Java: assert x > 0 : "必须为正";
来源：http://ym.shxzukj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ng.colortex.cn

Ruby: raise "必须为正" unless x > 0
来源：http://qo.yuntaijiaju.cn

C#:   Debug.Assert(x > 0);
来源：http://cc.9csxet.cn

[H08] 获取错误信息与堆栈
来源：http://il.nicolike.cn

Py:   str(e);  traceback.format_exc()
来源：http://iq.bookmarksfly.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://kw.shxzukj.cn

JS:   e.message;  e.stack
来源：http://qz.colortex.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ol.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qw.521024.cn

Go:   err.Error()
来源：http://nf.bookmarksfly.cn

Ruby: e.message;  e.backtrace
来源：http://lv.nicolike.cn

C#:   e.Message;  e.StackTrace
来源：http://rg.521024.cn

[H09] 带错误码的异常
来源：http://ax.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yl.gzmigu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hd.jianghongdianzi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ns.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gj.lnxyls.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://om.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://az.521024.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zs.newstarts.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yd.shtwfgs.cn

[H10] 资源自动释放
来源：http://tz.bookmarksfly.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hn.huanxung.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dn.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ft.bookmarksfly.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qi.szxytkj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gn.szxytkj.cn

Go:   defer f.Close()
来源：http://ja.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zq.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fl.lnxyls.cn

================================================================================
来源：http://wn.lnxyls.cn

I. 正则表达式
来源：http://aj.chemitech.net.cn

================================================================================
来源：http://xu.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://go.wgjwhj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vz.colortex.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pq.jianghongdianzi.cn

JS:   /\d+/.test(s)
来源：http://fs.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://sc.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://di.newstarts.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hm.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://sw.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fm.colortex.cn

[I02] 提取所有匹配
来源：http://mq.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://yv.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zr.521024.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gl.yuexingan06.cn

TS:   s.match(/\d+/g)
来源：http://ow.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lv.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wu.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://fo.asd995.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ob.shtwfgs.cn

[I03] 提取捕获分组
来源：http://xv.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://co.newstarts.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uw.newstarts.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gr.muxihuayi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xo.newstarts.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ae.muxihuayi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://so.jianghongdianzi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hu.nicolike.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ak.yuntaijiaju.cn

[I04] 正则替换
来源：http://mn.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rm.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ru.wgjwhj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://is.huixiangedu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ph.521024.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bh.jianghongdianzi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sx.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pt.bookmarksfly.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://im.shxzskj.cn

[I05] 按正则拆分
来源：http://dx.yuexingan06.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://lg.bjjhwx.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yl.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://fy.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://qg.newstarts.cn

Java: s.split("\\s*,\\s*")
来源：http://jf.colortex.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://by.asd995.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qk.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://co.panjiajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vf.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mp.bookmarksfly.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lx.yuexingan06.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ru.521024.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://az.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pa.hahajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://tp.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ua.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fj.haigaiapp.cn

[I07] 忽略大小写与多行模式
来源：http://gg.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ee.nszjky.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ne.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wd.shtwfgs.cn

TS:   /error/gim
来源：http://kg.szsharing.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mv.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nb.jctech888.com.cn

Ruby: s.scan(/error/i)
来源：http://sr.521024.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bk.panjiajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://vx.huixinmuqiang.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://il.chemitech.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dh.bjjhwx.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://em.hnjuh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vu.wgjwhj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ro.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kl.panjiajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jc.yuexingan06.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yg.nszjky.cn

================================================================================
来源：http://vm.huixinmuqiang.cn

J. 日期与时间
来源：http://bl.hnjuh.cn

================================================================================
来源：http://py.newstarts.cn

[J01] 获取当前时间
来源：http://it.9csxet.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cv.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ib.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://fa.yuntaijiaju.cn

TS:   new Date();  Date.now()
来源：http://nf.shxzskj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xy.colortex.cn

Go:   time.Now()
来源：http://au.panjiajie.cn

Ruby: Time.now
来源：http://ym.newstarts.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hj.huanxung.cn

[J02] 格式化输出
来源：http://gy.bjjhwx.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ri.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://uc.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ss.haigaiapp.cn

TS:   d.toISOString()
来源：http://jl.shxzskj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://pm.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://go.hnjuh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xj.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zs.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://vv.bookmarksfly.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eg.szxytkj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bv.nicolike.cn

JS:   new Date("2024-01-02")
来源：http://gz.yuntaijiaju.cn

TS:   new Date("2024-01-02")
来源：http://ei.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://iv.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vk.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://jr.nicolike.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ii.huixinmuqiang.cn

[J04] 时间戳与日期互转
来源：http://fb.nszjky.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ng.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pm.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://vg.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zf.bjjhwx.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://le.bookmarksfly.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hn.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://et.hnjuh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vb.wgjwhj.cn

[J05] 时间加减（加 7 天）
来源：http://tp.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://cm.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jn.bookmarksfly.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://tg.shtwfgs.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cc.huixinmuqiang.cn

Java: LocalDate.now().plusDays(7)
来源：http://wa.hahajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zy.shtwfgs.cn

Ruby: Time.now + 7 * 86400
来源：http://gx.colortex.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gj.huixiangedu.cn

[J06] 计算两时间之差
来源：http://md.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://vu.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://vr.nicolike.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://um.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qg.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gg.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://bg.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://ll.shxzukj.cn

C#:   (end - start).TotalSeconds
来源：http://ox.newstarts.cn

[J07] 比较两个日期
来源：http://vy.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://ms.yuntaijiaju.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yo.wgjwhj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zq.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xf.jctech888.com.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ya.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tt.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kj.wgjwhj.cn

C#:   d1 < d2;  d1 == d2
来源：http://du.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://mv.haigaiapp.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tl.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cw.bjjhwx.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fu.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jd.jctech888.com.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rb.yuntaijiaju.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sf.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zp.521024.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ve.nszjky.cn

[J09] 时区处理
来源：http://um.jianghongdianzi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ck.szsharing.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://td.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ic.haigaiapp.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sl.huanxung.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pk.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kj.yuntaijiaju.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xm.nicolike.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://qp.szsharing.cn

[J10] 取今天 / 本月第一天
来源：http://ki.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://na.jctech888.com.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xf.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hd.gzmigu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rr.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rw.9csxet.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zr.gzmigu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nf.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nl.panjiajie.cn


<!-- 参考信息 -->