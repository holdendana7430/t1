代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://ru.szsharing.cn

Ruby: def to_s; @name; end
来源：http://cg.jianghongdianzi.cn

C#:   public override string ToString() => Name;
来源：http://la.colortex.cn

[G13] 判断对象类型
来源：http://sx.nicolike.cn

Py:   isinstance(u, User)
来源：http://ac.hahajie.cn

PHP:  $u instanceof User
来源：http://jj.szxytkj.cn

JS:   u instanceof User
来源：http://wb.yuexingan06.cn

TS:   u instanceof User
来源：http://ko.huixinmuqiang.cn

Java: u instanceof User
来源：http://uk.huixiangedu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kd.shtwfgs.cn

Ruby: u.is_a?(User)
来源：http://dt.panjiajie.cn

C#:   u is User
来源：http://sw.szxytkj.cn

[G14] 数据类 / record
来源：http://ei.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://iw.shxzukj.cn

PHP:  // 用 readonly 属性模拟
来源：http://et.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mo.huixinmuqiang.cn

TS:   type User = { name: string; age: number };
来源：http://ye.bjjhwx.cn

Java: record User(String name, int age) {}
来源：http://qr.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://zt.newstarts.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jv.shxzukj.cn

C#:   record User(string Name, int Age);
来源：http://he.huanxung.cn

[G15] 枚举
来源：http://ay.asd995.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://fn.huixiangedu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sq.wgjwhj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gn.muxihuayi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mq.yuntaijiaju.cn

Java: enum Color { RED, GREEN }
来源：http://pz.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tj.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://rg.bookmarksfly.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dt.lnxyls.cn

[G16] 对象转数组 / 字典
来源：http://lu.huixinmuqiang.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rz.szxytkj.cn

PHP:  get_object_vars($obj);
来源：http://km.huixinmuqiang.cn

JS:   Object.entries(obj)
来源：http://cs.jctech888.com.cn

TS:   Object.entries(obj)
来源：http://tv.huixinmuqiang.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xu.yuexingan06.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jm.chemitech.net.cn

Ruby: obj.instance_variables
来源：http://bl.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://hq.jctech888.com.cn

================================================================================
来源：http://um.wgjwhj.cn

H. 异常与错误处理
来源：http://rt.asd995.cn

================================================================================
来源：http://jy.nicolike.cn

[H01] try / catch 基础
来源：http://ys.bjjhwx.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ty.huixiangedu.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ad.shxzskj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dt.haigaiapp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zm.huanxung.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zc.bookmarksfly.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ax.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ca.szsharing.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hn.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://fa.gzmigu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yu.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://im.hnjuh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mo.521024.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fg.bookmarksfly.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xm.szsharing.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cz.szxytkj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hg.gzmigu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ek.shtwfgs.cn

[H03] 主动抛出异常
来源：http://lm.gzmigu.cn

Py:   raise ValueError("错误信息")
来源：http://kf.huixinmuqiang.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://th.jctech888.com.cn

JS:   throw new Error("错误信息");
来源：http://sm.wgjwhj.cn

TS:   throw new Error("错误信息");
来源：http://au.newstarts.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://uo.newstarts.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://za.panjiajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://sd.jianghongdianzi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://uv.bookmarksfly.cn

[H04] 自定义异常类型
来源：http://fp.nszjky.cn

Py:   class MyError(Exception): pass
来源：http://on.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tk.szsharing.cn

JS:   class MyError extends Error {}
来源：http://uy.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://tf.jianghongdianzi.cn

Java: class MyException extends RuntimeException {}
来源：http://sr.haigaiapp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vx.bjjhwx.cn

Ruby: class MyError < StandardError; end
来源：http://sl.newstarts.cn

C#:   class MyException : Exception {}
来源：http://wl.lnxyls.cn

[H05] 捕获特定类型
来源：http://dz.haigaiapp.cn

Py:   except ValueError as e:
来源：http://rz.jctech888.com.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zd.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://ur.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://xj.shxzukj.cn

Java: catch (IOException | SQLException e) {}
来源：http://zf.9csxet.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hs.nicolike.cn

Ruby: rescue ArgumentError => e
来源：http://jc.shxzskj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zg.szsharing.cn

[H06] 可选值 / 空值安全访问
来源：http://qv.haigaiapp.cn

Py:   value = d.get("k") or default
来源：http://lr.shxzukj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ei.lnxyls.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ez.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://eh.yuntaijiaju.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pv.nicolike.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zv.hahajie.cn

Ruby: d&.dig(:a, :b)
来源：http://fm.shxzukj.cn

C#:   obj?.A?.B ?? default
来源：http://yy.jctech888.com.cn

[H07] 断言
来源：http://ib.colortex.cn

Py:   assert x > 0, "必须为正"
来源：http://am.huixinmuqiang.cn

PHP:  assert($x > 0);
来源：http://ln.newstarts.cn

JS:   console.assert(x > 0);
来源：http://eo.huixinmuqiang.cn

TS:   console.assert(x > 0);
来源：http://ue.yuexingan06.cn

Java: assert x > 0 : "必须为正";
来源：http://mf.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vl.shtwfgs.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cn.lnxyls.cn

C#:   Debug.Assert(x > 0);
来源：http://sn.nszjky.cn

[H08] 获取错误信息与堆栈
来源：http://fz.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://vd.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hf.521024.cn

JS:   e.message;  e.stack
来源：http://ac.yuexingan06.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gf.huixinmuqiang.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ee.9csxet.cn

Go:   err.Error()
来源：http://hy.jctech888.com.cn

Ruby: e.message;  e.backtrace
来源：http://yl.muxihuayi.cn

C#:   e.Message;  e.StackTrace
来源：http://xc.jctech888.com.cn

[H09] 带错误码的异常
来源：http://fa.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://eb.nicolike.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://od.nszjky.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jy.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ot.521024.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qt.panjiajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uj.newstarts.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vk.huanxung.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qw.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://xb.bjjhwx.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://eu.bjjhwx.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://op.hahajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mu.haigaiapp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ht.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sj.gzmigu.cn

Go:   defer f.Close()
来源：http://tt.panjiajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bd.szsharing.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hq.nszjky.cn

================================================================================
来源：http://cg.haigaiapp.cn

I. 正则表达式
来源：http://tn.panjiajie.cn

================================================================================
来源：http://og.shtwfgs.cn

[I01] 判断是否匹配
来源：http://si.newstarts.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dz.asd995.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hx.shxzskj.cn

JS:   /\d+/.test(s)
来源：http://od.hahajie.cn

TS:   /\d+/.test(s)
来源：http://dt.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ec.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nc.yuntaijiaju.cn

Ruby: s.match?(/\d+/)
来源：http://mz.newstarts.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ae.lnxyls.cn

[I02] 提取所有匹配
来源：http://pc.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://ie.asd995.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qw.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eo.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://km.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ny.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xy.wgjwhj.cn

Ruby: s.scan(/\d+/)
来源：http://mp.hnjuh.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yg.hnjuh.cn

[I03] 提取捕获分组
来源：http://ss.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ss.9csxet.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fa.szsharing.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bm.wgjwhj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mo.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://do.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gs.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lf.yuntaijiaju.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ka.huixinmuqiang.cn

[I04] 正则替换
来源：http://ss.huixiangedu.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ug.shxzskj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yz.szsharing.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vy.9csxet.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mf.szxytkj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cg.shtwfgs.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oh.shxzskj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://do.lnxyls.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pm.asd995.cn

[I05] 按正则拆分
来源：http://md.szxytkj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sq.shxzskj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kr.newstarts.cn

JS:   s.split(/\s*,\s*/)
来源：http://bg.jianghongdianzi.cn

TS:   s.split(/\s*,\s*/)
来源：http://wz.asd995.cn

Java: s.split("\\s*,\\s*")
来源：http://jf.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gb.panjiajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://es.yuntaijiaju.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://za.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jn.hahajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ie.shxzskj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kl.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oa.chemitech.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rs.nszjky.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ek.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://av.huixinmuqiang.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ac.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ci.huanxung.cn

[I07] 忽略大小写与多行模式
来源：http://ua.wgjwhj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ki.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ex.gzmigu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gm.chemitech.net.cn

TS:   /error/gim
来源：http://pj.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jk.haigaiapp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mr.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://qm.szxytkj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ca.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://dj.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://co.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fv.lnxyls.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cj.bjjhwx.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ke.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vq.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lz.lnxyls.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wq.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wn.nszjky.cn

================================================================================
来源：http://bt.colortex.cn

J. 日期与时间
来源：http://kj.chemitech.net.cn

================================================================================
来源：http://ik.nicolike.cn

[J01] 获取当前时间
来源：http://nx.jianghongdianzi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://am.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ld.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://be.jctech888.com.cn

TS:   new Date();  Date.now()
来源：http://od.newstarts.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kw.521024.cn

Go:   time.Now()
来源：http://en.shxzskj.cn

Ruby: Time.now
来源：http://qa.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ug.haigaiapp.cn

[J02] 格式化输出
来源：http://mn.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fh.nszjky.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://iv.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qz.bookmarksfly.cn

TS:   d.toISOString()
来源：http://mt.asd995.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dh.szsharing.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ty.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fn.muxihuayi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ht.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://gu.shxzukj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wz.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://co.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://vt.yuntaijiaju.cn

TS:   new Date("2024-01-02")
来源：http://ng.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://du.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vc.chemitech.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://mt.huixinmuqiang.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ll.wgjwhj.cn

[J04] 时间戳与日期互转
来源：http://bv.wgjwhj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mv.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://os.jctech888.com.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uj.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://hv.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ye.gzmigu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rz.muxihuayi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nu.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sr.wgjwhj.cn

[J05] 时间加减（加 7 天）
来源：http://xn.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://bo.huixinmuqiang.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hq.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cv.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mg.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://rb.bjjhwx.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zl.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://sj.panjiajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://nl.521024.cn

[J06] 计算两时间之差
来源：http://zw.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://uo.wgjwhj.cn

PHP:  $end->diff($start)->days;
来源：http://vl.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nm.bookmarksfly.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mh.shxzukj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://yd.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://vs.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://px.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://dk.hnjuh.cn

[J07] 比较两个日期
来源：http://hu.asd995.cn

Py:   d1 < d2;  d1 == d2
来源：http://na.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://id.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rt.huanxung.cn

TS:   d1.getTime() < d2.getTime()
来源：http://jw.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oy.haigaiapp.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pt.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mm.chemitech.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://hl.jianghongdianzi.cn

[J08] 提取年月日与星期
来源：http://dg.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ed.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mh.nszjky.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yl.newstarts.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nr.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://py.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gi.521024.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wi.yuntaijiaju.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://az.panjiajie.cn

[J09] 时区处理
来源：http://hd.jctech888.com.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lt.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hx.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ki.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ul.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wa.hahajie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ex.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cq.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ty.huanxung.cn

[J10] 取今天 / 本月第一天
来源：http://bc.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nk.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vm.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wj.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bz.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uk.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qq.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ki.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ke.asd995.cn


<!-- 参考信息 -->