代发 wailian999

Java: u instanceof User
来源：http://fn.nszjky.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lq.9csxet.cn

Ruby: u.is_a?(User)
来源：http://zj.nszjky.cn

C#:   u is User
来源：http://lq.wgjwhj.cn

[G14] 数据类 / record
来源：http://aj.nszjky.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://up.newstarts.cn

PHP:  // 用 readonly 属性模拟
来源：http://hn.shtwfgs.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wi.gzmigu.cn

TS:   type User = { name: string; age: number };
来源：http://dv.shxzukj.cn

Java: record User(String name, int age) {}
来源：http://lt.huanxung.cn

Go:   type User struct { Name string; Age int }
来源：http://nr.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://th.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://hy.chemitech.net.cn

[G15] 枚举
来源：http://fw.yuntaijiaju.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tw.shtwfgs.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cc.colortex.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sb.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iz.gzmigu.cn

Java: enum Color { RED, GREEN }
来源：http://xj.chemitech.net.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qy.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://fl.gzmigu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mh.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://nf.bookmarksfly.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://so.nszjky.cn

PHP:  get_object_vars($obj);
来源：http://op.shtwfgs.cn

JS:   Object.entries(obj)
来源：http://gd.yuexingan06.cn

TS:   Object.entries(obj)
来源：http://lp.chemitech.net.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://us.yuntaijiaju.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gk.chemitech.net.cn

Ruby: obj.instance_variables
来源：http://tv.huanxung.cn

C#:   // 用反射或 System.Text.Json
来源：http://by.szsharing.cn

================================================================================
来源：http://bs.nicolike.cn

H. 异常与错误处理
来源：http://ls.yuntaijiaju.cn

================================================================================
来源：http://to.huixinmuqiang.cn

[H01] try / catch 基础
来源：http://hn.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ez.newstarts.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ub.huixiangedu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://yk.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xk.huixinmuqiang.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wi.shxzskj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wu.521024.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sr.haigaiapp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cp.jctech888.com.cn

[H02] finally / ensure 收尾
来源：http://mi.shxzukj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zy.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gq.yuntaijiaju.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ip.wgjwhj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rq.hnjuh.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dg.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qp.wgjwhj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://oe.yuntaijiaju.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pa.asd995.cn

[H03] 主动抛出异常
来源：http://vw.bjjhwx.cn

Py:   raise ValueError("错误信息")
来源：http://ah.szsharing.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mi.gzmigu.cn

JS:   throw new Error("错误信息");
来源：http://eh.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://bz.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yz.colortex.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ac.jianghongdianzi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ar.nicolike.cn

C#:   throw new ArgumentException("错误信息");
来源：http://iu.nszjky.cn

[H04] 自定义异常类型
来源：http://sk.bjjhwx.cn

Py:   class MyError(Exception): pass
来源：http://gc.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dk.jianghongdianzi.cn

JS:   class MyError extends Error {}
来源：http://uw.szsharing.cn

TS:   class MyError extends Error {}
来源：http://cx.nszjky.cn

Java: class MyException extends RuntimeException {}
来源：http://jh.huixinmuqiang.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cy.huanxung.cn

Ruby: class MyError < StandardError; end
来源：http://as.9csxet.cn

C#:   class MyException : Exception {}
来源：http://ej.muxihuayi.cn

[H05] 捕获特定类型
来源：http://oq.nicolike.cn

Py:   except ValueError as e:
来源：http://hc.chemitech.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eq.9csxet.cn

JS:   if (e instanceof TypeError) {}
来源：http://qm.hahajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://cw.wgjwhj.cn

Java: catch (IOException | SQLException e) {}
来源：http://cj.521024.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hl.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://vl.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ss.newstarts.cn

[H06] 可选值 / 空值安全访问
来源：http://xa.huixinmuqiang.cn

Py:   value = d.get("k") or default
来源：http://pw.9csxet.cn

PHP:  $v = $d["k"] ?? null;
来源：http://te.wgjwhj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://uo.hahajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://dh.asd995.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xu.shxzukj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tn.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://vm.huixiangedu.cn

C#:   obj?.A?.B ?? default
来源：http://gq.shxzukj.cn

[H07] 断言
来源：http://ap.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://tb.lnxyls.cn

PHP:  assert($x > 0);
来源：http://yy.jctech888.com.cn

JS:   console.assert(x > 0);
来源：http://cr.lnxyls.cn

TS:   console.assert(x > 0);
来源：http://wo.bookmarksfly.cn

Java: assert x > 0 : "必须为正";
来源：http://it.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wc.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xi.shtwfgs.cn

C#:   Debug.Assert(x > 0);
来源：http://ui.panjiajie.cn

[H08] 获取错误信息与堆栈
来源：http://dq.jctech888.com.cn

Py:   str(e);  traceback.format_exc()
来源：http://hk.muxihuayi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ps.huixiangedu.cn

JS:   e.message;  e.stack
来源：http://ti.jianghongdianzi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://mt.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://tq.nicolike.cn

Go:   err.Error()
来源：http://xw.521024.cn

Ruby: e.message;  e.backtrace
来源：http://ek.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://mw.bjjhwx.cn

[H09] 带错误码的异常
来源：http://gd.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tj.bjjhwx.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cm.hahajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rp.yuntaijiaju.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://da.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ex.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hl.gzmigu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fc.bjjhwx.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://la.panjiajie.cn

[H10] 资源自动释放
来源：http://vs.huixinmuqiang.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bh.lnxyls.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vq.bjjhwx.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hy.huixiangedu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xn.haigaiapp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hw.lnxyls.cn

Go:   defer f.Close()
来源：http://gi.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ch.huanxung.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://dn.asd995.cn

================================================================================
来源：http://sv.huixiangedu.cn

I. 正则表达式
来源：http://bb.szsharing.cn

================================================================================
来源：http://tj.huixinmuqiang.cn

[I01] 判断是否匹配
来源：http://rp.9csxet.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ug.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vg.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://iz.jianghongdianzi.cn

TS:   /\d+/.test(s)
来源：http://qk.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ju.nicolike.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rx.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://ch.hahajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fp.huanxung.cn

[I02] 提取所有匹配
来源：http://bj.chemitech.net.cn

Py:   re.findall(r"\d+", s)
来源：http://jo.521024.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://up.hnjuh.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tv.nicolike.cn

TS:   s.match(/\d+/g)
来源：http://be.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dc.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nj.bookmarksfly.cn

Ruby: s.scan(/\d+/)
来源：http://lk.muxihuayi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pa.jianghongdianzi.cn

[I03] 提取捕获分组
来源：http://mj.hnjuh.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jz.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ea.haigaiapp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yk.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vr.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gn.lnxyls.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ci.newstarts.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dj.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vp.muxihuayi.cn

[I04] 正则替换
来源：http://ak.chemitech.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qh.szsharing.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hg.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gu.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ui.jianghongdianzi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://gw.yuexingan06.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://se.jctech888.com.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yy.nszjky.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dp.bookmarksfly.cn

[I05] 按正则拆分
来源：http://eu.hnjuh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yb.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ls.huanxung.cn

JS:   s.split(/\s*,\s*/)
来源：http://hn.panjiajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://wt.521024.cn

Java: s.split("\\s*,\\s*")
来源：http://bk.szsharing.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bo.shxzskj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ph.chemitech.net.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ya.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wh.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://up.nszjky.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hv.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wj.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uh.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bk.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ac.huanxung.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tl.shtwfgs.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dc.nicolike.cn

[I07] 忽略大小写与多行模式
来源：http://kb.chemitech.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://uy.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kp.huixiangedu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sf.gzmigu.cn

TS:   /error/gim
来源：http://zb.hnjuh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bn.9csxet.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ix.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://lr.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ud.panjiajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://gg.muxihuayi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rv.nicolike.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ph.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xa.panjiajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qm.muxihuayi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ik.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mq.huanxung.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fy.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gq.szxytkj.cn

================================================================================
来源：http://ze.chemitech.net.cn

J. 日期与时间
来源：http://we.huixinmuqiang.cn

================================================================================
来源：http://zn.jctech888.com.cn

[J01] 获取当前时间
来源：http://ta.szxytkj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zq.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mz.nszjky.cn

JS:   new Date();  Date.now()
来源：http://sc.521024.cn

TS:   new Date();  Date.now()
来源：http://hk.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fc.lnxyls.cn

Go:   time.Now()
来源：http://ma.huixinmuqiang.cn

Ruby: Time.now
来源：http://bg.nszjky.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rn.shtwfgs.cn

[J02] 格式化输出
来源：http://jm.szxytkj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://it.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://lq.huixinmuqiang.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ln.yuexingan06.cn

TS:   d.toISOString()
来源：http://ru.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fz.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ew.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hf.panjiajie.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vd.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://bw.colortex.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bw.yuexingan06.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://of.chemitech.net.cn

JS:   new Date("2024-01-02")
来源：http://il.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://we.lnxyls.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ad.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ph.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://jl.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://sw.shtwfgs.cn

[J04] 时间戳与日期互转
来源：http://cm.chemitech.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ec.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fk.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sd.panjiajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ev.hnjuh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pd.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xt.nicolike.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://je.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yg.huixiangedu.cn

[J05] 时间加减（加 7 天）
来源：http://cl.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://jy.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sj.newstarts.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://we.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wj.9csxet.cn

Java: LocalDate.now().plusDays(7)
来源：http://de.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jw.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://ki.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ao.huanxung.cn

[J06] 计算两时间之差
来源：http://lp.521024.cn

Py:   (end - start).total_seconds()
来源：http://gm.jianghongdianzi.cn

PHP:  $end->diff($start)->days;
来源：http://ne.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dh.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gk.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ch.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://ay.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://bh.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://nw.szsharing.cn

[J07] 比较两个日期
来源：http://bi.asd995.cn

Py:   d1 < d2;  d1 == d2
来源：http://wa.asd995.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vb.jianghongdianzi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bm.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://fy.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uz.jianghongdianzi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tp.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hb.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://zn.gzmigu.cn

[J08] 提取年月日与星期
来源：http://um.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ix.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zv.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ma.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://am.wgjwhj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://jc.huixinmuqiang.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ee.panjiajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://oy.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gb.muxihuayi.cn

[J09] 时区处理
来源：http://ou.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bx.shxzskj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mi.asd995.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pk.colortex.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zo.wgjwhj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://nr.szsharing.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fc.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://nq.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://do.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://bf.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://wr.szxytkj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rk.newstarts.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://px.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rt.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ox.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://iz.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jt.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://lw.muxihuayi.cn

================================================================================
来源：http://hq.huixiangedu.cn

K. JSON 与序列化
来源：http://xr.nszjky.cn

================================================================================
来源：http://yp.jianghongdianzi.cn

[K01] 对象转 JSON 字符串
来源：http://yw.9csxet.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ge.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ss.nicolike.cn

JS:   JSON.stringify(obj)
来源：http://lp.newstarts.cn

TS:   JSON.stringify(obj)
来源：http://xc.hahajie.cn


<!-- 参考信息 -->