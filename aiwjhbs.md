代发 wailian999

Java: u instanceof User
来源：http://mo.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tk.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://ll.bookmarksfly.cn

C#:   u is User
来源：http://bp.newstarts.cn

[G14] 数据类 / record
来源：http://bf.shtwfgs.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qb.jctech888.com.cn

PHP:  // 用 readonly 属性模拟
来源：http://lg.szxytkj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ju.asd995.cn

TS:   type User = { name: string; age: number };
来源：http://fx.521024.cn

Java: record User(String name, int age) {}
来源：http://bx.szxytkj.cn

Go:   type User struct { Name string; Age int }
来源：http://ls.szsharing.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://et.nszjky.cn

C#:   record User(string Name, int Age);
来源：http://ib.haigaiapp.cn

[G15] 枚举
来源：http://ch.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tx.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://oq.asd995.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mj.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://an.asd995.cn

Java: enum Color { RED, GREEN }
来源：http://yr.haigaiapp.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wr.chemitech.net.cn

Ruby: Color = %i[red green].freeze
来源：http://vx.szxytkj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tf.chemitech.net.cn

[G16] 对象转数组 / 字典
来源：http://tt.nszjky.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://st.shxzskj.cn

PHP:  get_object_vars($obj);
来源：http://ap.haigaiapp.cn

JS:   Object.entries(obj)
来源：http://jl.huixiangedu.cn

TS:   Object.entries(obj)
来源：http://is.muxihuayi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mj.yuexingan06.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zi.colortex.cn

Ruby: obj.instance_variables
来源：http://tc.521024.cn

C#:   // 用反射或 System.Text.Json
来源：http://rg.9csxet.cn

================================================================================
来源：http://ad.szsharing.cn

H. 异常与错误处理
来源：http://xf.jctech888.com.cn

================================================================================
来源：http://fg.wgjwhj.cn

[H01] try / catch 基础
来源：http://gp.bjjhwx.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://da.shtwfgs.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hc.yuexingan06.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zu.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://io.lnxyls.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bs.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://eb.szsharing.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://du.gzmigu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ud.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://wq.shxzukj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://og.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qx.hnjuh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hq.521024.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pi.nszjky.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gm.bookmarksfly.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jk.muxihuayi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ef.huixinmuqiang.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ih.bjjhwx.cn

[H03] 主动抛出异常
来源：http://ua.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://hd.chemitech.net.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wx.szsharing.cn

JS:   throw new Error("错误信息");
来源：http://er.huanxung.cn

TS:   throw new Error("错误信息");
来源：http://wm.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ai.szsharing.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jg.hahajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hv.jianghongdianzi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gj.shtwfgs.cn

[H04] 自定义异常类型
来源：http://ox.yuntaijiaju.cn

Py:   class MyError(Exception): pass
来源：http://qa.nszjky.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zp.wgjwhj.cn

JS:   class MyError extends Error {}
来源：http://oh.chemitech.net.cn

TS:   class MyError extends Error {}
来源：http://bk.chemitech.net.cn

Java: class MyException extends RuntimeException {}
来源：http://jh.hahajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ba.huanxung.cn

Ruby: class MyError < StandardError; end
来源：http://tu.521024.cn

C#:   class MyException : Exception {}
来源：http://ct.shtwfgs.cn

[H05] 捕获特定类型
来源：http://il.asd995.cn

Py:   except ValueError as e:
来源：http://pe.asd995.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gn.nszjky.cn

JS:   if (e instanceof TypeError) {}
来源：http://rv.lnxyls.cn

TS:   if (e instanceof TypeError) {}
来源：http://fv.huanxung.cn

Java: catch (IOException | SQLException e) {}
来源：http://ob.bookmarksfly.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tb.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://up.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oo.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://pq.szsharing.cn

Py:   value = d.get("k") or default
来源：http://xb.jctech888.com.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ge.newstarts.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vg.gzmigu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://hw.yuexingan06.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tq.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://th.shxzskj.cn

Ruby: d&.dig(:a, :b)
来源：http://wm.521024.cn

C#:   obj?.A?.B ?? default
来源：http://bw.9csxet.cn

[H07] 断言
来源：http://no.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://pu.shxzukj.cn

PHP:  assert($x > 0);
来源：http://oo.haigaiapp.cn

JS:   console.assert(x > 0);
来源：http://no.521024.cn

TS:   console.assert(x > 0);
来源：http://yi.bookmarksfly.cn

Java: assert x > 0 : "必须为正";
来源：http://ki.yuexingan06.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jb.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cw.shxzukj.cn

C#:   Debug.Assert(x > 0);
来源：http://an.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://dy.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://yt.yuexingan06.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://uf.muxihuayi.cn

JS:   e.message;  e.stack
来源：http://xm.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ye.9csxet.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tj.9csxet.cn

Go:   err.Error()
来源：http://iw.yuntaijiaju.cn

Ruby: e.message;  e.backtrace
来源：http://lw.yuntaijiaju.cn

C#:   e.Message;  e.StackTrace
来源：http://sb.szxytkj.cn

[H09] 带错误码的异常
来源：http://yc.huixiangedu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jr.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pm.yuexingan06.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hv.wgjwhj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uk.shxzskj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://os.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pr.gzmigu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ig.hnjuh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://hg.newstarts.cn

[H10] 资源自动释放
来源：http://ey.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cw.huixinmuqiang.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hi.gzmigu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ph.jianghongdianzi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cg.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hr.nszjky.cn

Go:   defer f.Close()
来源：http://xc.521024.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ji.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dn.yuexingan06.cn

================================================================================
来源：http://yr.huanxung.cn

I. 正则表达式
来源：http://ga.gzmigu.cn

================================================================================
来源：http://vc.shtwfgs.cn

[I01] 判断是否匹配
来源：http://zy.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rz.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wc.shxzskj.cn

JS:   /\d+/.test(s)
来源：http://bb.hahajie.cn

TS:   /\d+/.test(s)
来源：http://rt.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pg.hahajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bb.asd995.cn

Ruby: s.match?(/\d+/)
来源：http://nz.huixinmuqiang.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ak.gzmigu.cn

[I02] 提取所有匹配
来源：http://vv.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://fh.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yd.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fp.jianghongdianzi.cn

TS:   s.match(/\d+/g)
来源：http://rm.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bw.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://py.huanxung.cn

Ruby: s.scan(/\d+/)
来源：http://xe.newstarts.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ta.colortex.cn

[I03] 提取捕获分组
来源：http://xm.shxzskj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cu.hnjuh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yi.panjiajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://id.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pp.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tg.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xt.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ww.colortex.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kr.huixiangedu.cn

[I04] 正则替换
来源：http://sw.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xa.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tw.gzmigu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pl.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xn.chemitech.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://no.521024.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bx.521024.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://uq.hnjuh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bd.asd995.cn

[I05] 按正则拆分
来源：http://gj.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wv.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fu.hnjuh.cn

JS:   s.split(/\s*,\s*/)
来源：http://bg.jctech888.com.cn

TS:   s.split(/\s*,\s*/)
来源：http://ky.szsharing.cn

Java: s.split("\\s*,\\s*")
来源：http://jv.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fn.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jl.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jo.nicolike.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ew.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cm.haigaiapp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ze.huanxung.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ku.szxytkj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dg.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wb.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xy.newstarts.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zj.shxzukj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ma.haigaiapp.cn

[I07] 忽略大小写与多行模式
来源：http://vr.wgjwhj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qd.hahajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://sb.nicolike.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ih.asd995.cn

TS:   /error/gim
来源：http://rs.colortex.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pr.hnjuh.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dn.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://ms.chemitech.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://iu.newstarts.cn

[I08] 贪婪与非贪婪匹配
来源：http://pt.panjiajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xr.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hn.panjiajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ai.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tn.asd995.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://hw.newstarts.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ia.szxytkj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hi.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vo.colortex.cn

================================================================================
来源：http://zm.9csxet.cn

J. 日期与时间
来源：http://qz.nicolike.cn

================================================================================
来源：http://ik.huanxung.cn

[J01] 获取当前时间
来源：http://nv.wgjwhj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://dg.hahajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://or.9csxet.cn

JS:   new Date();  Date.now()
来源：http://bu.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://ht.haigaiapp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rj.huixinmuqiang.cn

Go:   time.Now()
来源：http://ad.9csxet.cn

Ruby: Time.now
来源：http://qx.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wx.yuexingan06.cn

[J02] 格式化输出
来源：http://me.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://oe.haigaiapp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xj.huanxung.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ud.gzmigu.cn

TS:   d.toISOString()
来源：http://zy.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ou.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rd.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gf.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dl.szxytkj.cn

[J03] 字符串解析为日期
来源：http://nz.panjiajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jm.huixiangedu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vt.szxytkj.cn

JS:   new Date("2024-01-02")
来源：http://ca.colortex.cn

TS:   new Date("2024-01-02")
来源：http://he.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mt.chemitech.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ay.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://rl.bookmarksfly.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hi.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://gw.9csxet.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://na.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://af.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pa.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lu.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gi.hnjuh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wq.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://aw.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tk.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://yk.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://bx.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wi.asd995.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rz.haigaiapp.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tf.9csxet.cn

Java: LocalDate.now().plusDays(7)
来源：http://lw.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zr.9csxet.cn

Ruby: Time.now + 7 * 86400
来源：http://kh.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xk.wgjwhj.cn

[J06] 计算两时间之差
来源：http://pp.shxzskj.cn

Py:   (end - start).total_seconds()
来源：http://db.haigaiapp.cn

PHP:  $end->diff($start)->days;
来源：http://zn.bookmarksfly.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mz.haigaiapp.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xm.muxihuayi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://zu.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://qw.hnjuh.cn

Ruby: end - start                 # 返回秒数
来源：http://se.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://xt.huanxung.cn

[J07] 比较两个日期
来源：http://lz.hnjuh.cn

Py:   d1 < d2;  d1 == d2
来源：http://ua.nicolike.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://il.nszjky.cn

JS:   d1.getTime() < d2.getTime()
来源：http://st.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rn.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kx.nszjky.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dq.szxytkj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vk.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://fb.wgjwhj.cn

[J08] 提取年月日与星期
来源：http://mp.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fx.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tv.huixiangedu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://be.chemitech.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lm.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gc.muxihuayi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qp.szxytkj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ou.nszjky.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://at.9csxet.cn

[J09] 时区处理
来源：http://sg.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xv.hahajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ku.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ef.hnjuh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nk.jctech888.com.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zc.szxytkj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wb.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://in.521024.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jx.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://vl.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://de.newstarts.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zm.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oz.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kp.yuexingan06.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://tk.muxihuayi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pc.huixinmuqiang.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mq.bookmarksfly.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://co.muxihuayi.cn

================================================================================
来源：http://vp.yuexingan06.cn

K. JSON 与序列化
来源：http://bi.huixiangedu.cn

================================================================================
来源：http://kz.9csxet.cn

[K01] 对象转 JSON 字符串
来源：http://zd.nszjky.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ar.huixiangedu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xi.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://cp.panjiajie.cn

TS:   JSON.stringify(obj)
来源：http://zp.hahajie.cn


<!-- 参考信息 -->