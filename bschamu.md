代发 wailian999

C#:   record User(string Name, int Age);
来源：http://af.hahajie.cn

[G15] 枚举
来源：http://xw.chemitech.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cr.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://br.szsharing.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ga.szsharing.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wn.gzmigu.cn

Java: enum Color { RED, GREEN }
来源：http://lv.panjiajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pr.lnxyls.cn

Ruby: Color = %i[red green].freeze
来源：http://nc.shtwfgs.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fo.asd995.cn

[G16] 对象转数组 / 字典
来源：http://xk.hahajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ko.nszjky.cn

PHP:  get_object_vars($obj);
来源：http://op.newstarts.cn

JS:   Object.entries(obj)
来源：http://wd.9csxet.cn

TS:   Object.entries(obj)
来源：http://nq.jianghongdianzi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://pg.panjiajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bb.bookmarksfly.cn

Ruby: obj.instance_variables
来源：http://pd.gzmigu.cn

C#:   // 用反射或 System.Text.Json
来源：http://vp.9csxet.cn

================================================================================
来源：http://pl.szsharing.cn

H. 异常与错误处理
来源：http://ce.wgjwhj.cn

================================================================================
来源：http://yk.szsharing.cn

[H01] try / catch 基础
来源：http://na.chemitech.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fr.panjiajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mt.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tx.panjiajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://au.szsharing.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://eo.wgjwhj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://an.jianghongdianzi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vm.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jx.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://mz.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gh.haigaiapp.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zs.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lx.shxzukj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pr.shtwfgs.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ft.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://br.jianghongdianzi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pz.muxihuayi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ad.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://hr.panjiajie.cn

Py:   raise ValueError("错误信息")
来源：http://lf.haigaiapp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ey.nszjky.cn

JS:   throw new Error("错误信息");
来源：http://bh.huixiangedu.cn

TS:   throw new Error("错误信息");
来源：http://nl.9csxet.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://uq.asd995.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dv.gzmigu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kb.lnxyls.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kg.jianghongdianzi.cn

[H04] 自定义异常类型
来源：http://yo.nszjky.cn

Py:   class MyError(Exception): pass
来源：http://eo.huixiangedu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wq.huixinmuqiang.cn

JS:   class MyError extends Error {}
来源：http://qe.huixiangedu.cn

TS:   class MyError extends Error {}
来源：http://kq.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://ee.nicolike.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uu.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://zq.bjjhwx.cn

C#:   class MyException : Exception {}
来源：http://zo.huanxung.cn

[H05] 捕获特定类型
来源：http://ob.haigaiapp.cn

Py:   except ValueError as e:
来源：http://qi.hahajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ak.hnjuh.cn

JS:   if (e instanceof TypeError) {}
来源：http://mf.haigaiapp.cn

TS:   if (e instanceof TypeError) {}
来源：http://so.jctech888.com.cn

Java: catch (IOException | SQLException e) {}
来源：http://mt.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://je.lnxyls.cn

Ruby: rescue ArgumentError => e
来源：http://zi.szxytkj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vm.nszjky.cn

[H06] 可选值 / 空值安全访问
来源：http://ur.hnjuh.cn

Py:   value = d.get("k") or default
来源：http://cz.bookmarksfly.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lv.bjjhwx.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pw.yuexingan06.cn

TS:   obj?.a?.b;  d ?? default
来源：http://px.521024.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xd.chemitech.net.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://os.newstarts.cn

Ruby: d&.dig(:a, :b)
来源：http://xw.shxzukj.cn

C#:   obj?.A?.B ?? default
来源：http://xm.szxytkj.cn

[H07] 断言
来源：http://wj.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://fz.szxytkj.cn

PHP:  assert($x > 0);
来源：http://sb.huixiangedu.cn

JS:   console.assert(x > 0);
来源：http://mj.colortex.cn

TS:   console.assert(x > 0);
来源：http://he.yuexingan06.cn

Java: assert x > 0 : "必须为正";
来源：http://uv.jianghongdianzi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://us.shtwfgs.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sv.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://rh.shxzskj.cn

[H08] 获取错误信息与堆栈
来源：http://ne.shxzukj.cn

Py:   str(e);  traceback.format_exc()
来源：http://df.hahajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ot.521024.cn

JS:   e.message;  e.stack
来源：http://dv.nicolike.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xr.muxihuayi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ee.asd995.cn

Go:   err.Error()
来源：http://sn.jctech888.com.cn

Ruby: e.message;  e.backtrace
来源：http://gn.wgjwhj.cn

C#:   e.Message;  e.StackTrace
来源：http://ou.jianghongdianzi.cn

[H09] 带错误码的异常
来源：http://yr.bookmarksfly.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://of.huanxung.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dd.nicolike.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://xk.colortex.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jb.muxihuayi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ua.yuexingan06.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ci.521024.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qr.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qg.shxzukj.cn

[H10] 资源自动释放
来源：http://kt.jctech888.com.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qj.shxzskj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://eq.asd995.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://uy.nicolike.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qj.9csxet.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xr.9csxet.cn

Go:   defer f.Close()
来源：http://km.newstarts.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gi.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ix.nicolike.cn

================================================================================
来源：http://lm.bookmarksfly.cn

I. 正则表达式
来源：http://hk.panjiajie.cn

================================================================================
来源：http://be.shtwfgs.cn

[I01] 判断是否匹配
来源：http://mr.bjjhwx.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fo.yuexingan06.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rq.newstarts.cn

JS:   /\d+/.test(s)
来源：http://ho.hahajie.cn

TS:   /\d+/.test(s)
来源：http://nc.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rr.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://rk.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://pe.huixiangedu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://it.haigaiapp.cn

[I02] 提取所有匹配
来源：http://hw.bjjhwx.cn

Py:   re.findall(r"\d+", s)
来源：http://oe.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lg.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://da.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://bo.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nq.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://oh.newstarts.cn

Ruby: s.scan(/\d+/)
来源：http://vj.lnxyls.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ml.asd995.cn

[I03] 提取捕获分组
来源：http://jm.9csxet.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zu.panjiajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zz.chemitech.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://lg.bjjhwx.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sa.nszjky.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cc.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://za.muxihuayi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ga.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://vg.szxytkj.cn

[I04] 正则替换
来源：http://sp.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wb.shtwfgs.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://iu.newstarts.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pw.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ip.wgjwhj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ek.haigaiapp.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://cu.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://on.panjiajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kc.bjjhwx.cn

[I05] 按正则拆分
来源：http://tv.hnjuh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bw.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bu.haigaiapp.cn

JS:   s.split(/\s*,\s*/)
来源：http://vw.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://sk.huixiangedu.cn

Java: s.split("\\s*,\\s*")
来源：http://hu.hnjuh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://td.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tz.lnxyls.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://my.panjiajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xw.gzmigu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://uq.huanxung.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://bk.asd995.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lk.szsharing.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ar.asd995.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qj.shxzskj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pi.nszjky.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ah.521024.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mt.muxihuayi.cn

[I07] 忽略大小写与多行模式
来源：http://sf.szsharing.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sy.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mu.bookmarksfly.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hf.panjiajie.cn

TS:   /error/gim
来源：http://tu.szsharing.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ax.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fe.wgjwhj.cn

Ruby: s.scan(/error/i)
来源：http://eu.bjjhwx.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yu.yuntaijiaju.cn

[I08] 贪婪与非贪婪匹配
来源：http://ux.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cw.haigaiapp.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hm.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kz.bjjhwx.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eh.jctech888.com.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vw.jianghongdianzi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://he.bookmarksfly.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jx.yuntaijiaju.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://im.wgjwhj.cn

================================================================================
来源：http://yt.chemitech.net.cn

J. 日期与时间
来源：http://tv.chemitech.net.cn

================================================================================
来源：http://go.shtwfgs.cn

[J01] 获取当前时间
来源：http://fi.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pa.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ky.lnxyls.cn

JS:   new Date();  Date.now()
来源：http://xl.newstarts.cn

TS:   new Date();  Date.now()
来源：http://ri.9csxet.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qw.panjiajie.cn

Go:   time.Now()
来源：http://rl.shxzskj.cn

Ruby: Time.now
来源：http://kd.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lg.9csxet.cn

[J02] 格式化输出
来源：http://at.shxzskj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xv.hnjuh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fq.521024.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ub.newstarts.cn

TS:   d.toISOString()
来源：http://cm.lnxyls.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sl.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ht.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://no.huixinmuqiang.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xn.asd995.cn

[J03] 字符串解析为日期
来源：http://zf.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mz.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vy.gzmigu.cn

JS:   new Date("2024-01-02")
来源：http://ad.shtwfgs.cn

TS:   new Date("2024-01-02")
来源：http://jf.521024.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qc.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jo.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://yu.chemitech.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jn.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://qr.newstarts.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://co.jianghongdianzi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://um.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yt.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://eg.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://st.yuexingan06.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bs.jianghongdianzi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rb.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fp.hahajie.cn

[J05] 时间加减（加 7 天）
来源：http://hv.jctech888.com.cn

Py:   now + timedelta(days=7)
来源：http://dr.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mn.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://em.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mg.muxihuayi.cn

Java: LocalDate.now().plusDays(7)
来源：http://xd.yuexingan06.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bw.lnxyls.cn

Ruby: Time.now + 7 * 86400
来源：http://zo.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yr.jianghongdianzi.cn

[J06] 计算两时间之差
来源：http://bh.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://sq.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://ng.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://lv.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://aa.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xr.hnjuh.cn

Go:   end.Sub(start).Hours()
来源：http://tp.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://el.shxzukj.cn

C#:   (end - start).TotalSeconds
来源：http://tb.shxzskj.cn

[J07] 比较两个日期
来源：http://fj.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://rn.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ce.bookmarksfly.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ka.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://uh.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vv.shxzskj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gs.chemitech.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sf.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://vv.colortex.cn

[J08] 提取年月日与星期
来源：http://xr.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://re.hahajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nn.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://up.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wn.jctech888.com.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hy.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lv.haigaiapp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wo.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zg.huanxung.cn

[J09] 时区处理
来源：http://sl.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hg.szxytkj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ik.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zt.gzmigu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xf.nicolike.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bl.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nl.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://eg.panjiajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xp.huixiangedu.cn

[J10] 取今天 / 本月第一天
来源：http://jx.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fk.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bk.lnxyls.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lk.hahajie.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://av.shtwfgs.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kx.nszjky.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ys.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ro.nicolike.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://av.hahajie.cn

================================================================================
来源：http://cj.jianghongdianzi.cn

K. JSON 与序列化
来源：http://zk.lnxyls.cn

================================================================================
来源：http://ma.yuntaijiaju.cn

[K01] 对象转 JSON 字符串
来源：http://ir.chemitech.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://td.huixinmuqiang.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rr.yuntaijiaju.cn

JS:   JSON.stringify(obj)
来源：http://ab.521024.cn

TS:   JSON.stringify(obj)
来源：http://eo.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ec.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://zw.wgjwhj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://eg.colortex.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hv.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://kv.shtwfgs.cn

Py:   json.loads(s)
来源：http://nw.lnxyls.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ia.9csxet.cn

JS:   JSON.parse(s)
来源：http://zh.gzmigu.cn

TS:   JSON.parse(s)
来源：http://jy.hahajie.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qr.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://kw.nicolike.cn

Ruby: JSON.parse(s)
来源：http://wq.nszjky.cn


<!-- 参考信息 -->