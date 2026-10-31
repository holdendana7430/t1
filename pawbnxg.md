代发 wailian999

C#:   record User(string Name, int Age);
来源：http://qb.yuntaijiaju.cn

[G15] 枚举
来源：http://bp.jianghongdianzi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yf.asd995.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ef.gzmigu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vy.szxytkj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://if.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://ks.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ej.huixiangedu.cn

Ruby: Color = %i[red green].freeze
来源：http://sb.9csxet.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xc.newstarts.cn

[G16] 对象转数组 / 字典
来源：http://ay.nicolike.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://py.haigaiapp.cn

PHP:  get_object_vars($obj);
来源：http://wo.lnxyls.cn

JS:   Object.entries(obj)
来源：http://aq.panjiajie.cn

TS:   Object.entries(obj)
来源：http://ez.muxihuayi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gg.szxytkj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bw.chemitech.net.cn

Ruby: obj.instance_variables
来源：http://sb.huanxung.cn

C#:   // 用反射或 System.Text.Json
来源：http://bk.newstarts.cn

================================================================================
来源：http://ek.szxytkj.cn

H. 异常与错误处理
来源：http://zi.newstarts.cn

================================================================================
来源：http://lm.shxzskj.cn

[H01] try / catch 基础
来源：http://xh.521024.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ew.hnjuh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://is.gzmigu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xu.nicolike.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vy.9csxet.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hn.shxzskj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gx.shxzskj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bz.szxytkj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tk.gzmigu.cn

[H02] finally / ensure 收尾
来源：http://fh.bjjhwx.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qj.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://dl.gzmigu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yz.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ar.huanxung.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qk.chemitech.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zn.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wd.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yb.haigaiapp.cn

[H03] 主动抛出异常
来源：http://ok.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://mk.haigaiapp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bx.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://iy.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://su.szsharing.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mj.jianghongdianzi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://eq.panjiajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ax.szxytkj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pn.huanxung.cn

[H04] 自定义异常类型
来源：http://bd.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://es.hnjuh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hp.shxzukj.cn

JS:   class MyError extends Error {}
来源：http://mx.nicolike.cn

TS:   class MyError extends Error {}
来源：http://ze.jctech888.com.cn

Java: class MyException extends RuntimeException {}
来源：http://tm.jianghongdianzi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://md.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://en.muxihuayi.cn

C#:   class MyException : Exception {}
来源：http://jm.9csxet.cn

[H05] 捕获特定类型
来源：http://yf.panjiajie.cn

Py:   except ValueError as e:
来源：http://yh.huanxung.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jg.haigaiapp.cn

JS:   if (e instanceof TypeError) {}
来源：http://qk.9csxet.cn

TS:   if (e instanceof TypeError) {}
来源：http://cu.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://yx.newstarts.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://eg.wgjwhj.cn

Ruby: rescue ArgumentError => e
来源：http://mx.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oh.muxihuayi.cn

[H06] 可选值 / 空值安全访问
来源：http://sa.hnjuh.cn

Py:   value = d.get("k") or default
来源：http://ls.hnjuh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bv.nicolike.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zx.hahajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qe.chemitech.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ye.huanxung.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://el.yuexingan06.cn

Ruby: d&.dig(:a, :b)
来源：http://yz.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://dt.9csxet.cn

[H07] 断言
来源：http://ez.colortex.cn

Py:   assert x > 0, "必须为正"
来源：http://ha.colortex.cn

PHP:  assert($x > 0);
来源：http://lz.newstarts.cn

JS:   console.assert(x > 0);
来源：http://fe.szxytkj.cn

TS:   console.assert(x > 0);
来源：http://zi.shxzskj.cn

Java: assert x > 0 : "必须为正";
来源：http://vn.jianghongdianzi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rt.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xd.jctech888.com.cn

C#:   Debug.Assert(x > 0);
来源：http://bd.shtwfgs.cn

[H08] 获取错误信息与堆栈
来源：http://qb.bookmarksfly.cn

Py:   str(e);  traceback.format_exc()
来源：http://ng.9csxet.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hq.newstarts.cn

JS:   e.message;  e.stack
来源：http://nj.asd995.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ci.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qh.chemitech.net.cn

Go:   err.Error()
来源：http://kl.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://mc.bjjhwx.cn

C#:   e.Message;  e.StackTrace
来源：http://pv.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://fu.shtwfgs.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qs.chemitech.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rt.haigaiapp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qt.panjiajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mh.huanxung.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yt.bjjhwx.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ma.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gc.szsharing.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://sl.chemitech.net.cn

[H10] 资源自动释放
来源：http://dd.wgjwhj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ix.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lk.bookmarksfly.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ug.jctech888.com.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ks.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ja.shxzskj.cn

Go:   defer f.Close()
来源：http://xl.jctech888.com.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hh.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://on.yuntaijiaju.cn

================================================================================
来源：http://kq.asd995.cn

I. 正则表达式
来源：http://py.bookmarksfly.cn

================================================================================
来源：http://ma.yuexingan06.cn

[I01] 判断是否匹配
来源：http://yl.wgjwhj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nk.lnxyls.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ly.521024.cn

JS:   /\d+/.test(s)
来源：http://sd.newstarts.cn

TS:   /\d+/.test(s)
来源：http://yx.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vb.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pb.bookmarksfly.cn

Ruby: s.match?(/\d+/)
来源：http://gd.wgjwhj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kl.colortex.cn

[I02] 提取所有匹配
来源：http://ea.muxihuayi.cn

Py:   re.findall(r"\d+", s)
来源：http://sv.szxytkj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qt.shxzukj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wq.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://gf.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ds.huanxung.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yk.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://pp.hahajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://um.hnjuh.cn

[I03] 提取捕获分组
来源：http://gs.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ih.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jw.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vf.jianghongdianzi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lu.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uf.hahajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ud.bookmarksfly.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ju.chemitech.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nb.jianghongdianzi.cn

[I04] 正则替换
来源：http://gv.lnxyls.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rb.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://je.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xd.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qf.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hi.nszjky.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fk.haigaiapp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rf.9csxet.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fa.panjiajie.cn

[I05] 按正则拆分
来源：http://fd.521024.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://bz.nicolike.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://nx.huixinmuqiang.cn

JS:   s.split(/\s*,\s*/)
来源：http://uw.shxzukj.cn

TS:   s.split(/\s*,\s*/)
来源：http://rk.huixiangedu.cn

Java: s.split("\\s*,\\s*")
来源：http://ai.nicolike.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bc.wgjwhj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vc.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ci.huixiangedu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rg.gzmigu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qb.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lo.lnxyls.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fm.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wf.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sv.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://es.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ej.yuexingan06.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qj.newstarts.cn

[I07] 忽略大小写与多行模式
来源：http://mh.hnjuh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fb.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://es.huanxung.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://lh.nicolike.cn

TS:   /error/gim
来源：http://oo.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://iw.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pp.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://kc.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oc.newstarts.cn

[I08] 贪婪与非贪婪匹配
来源：http://se.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fh.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wd.panjiajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pz.bjjhwx.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xv.huixiangedu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fk.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wg.szxytkj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://aw.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://eb.colortex.cn

================================================================================
来源：http://et.chemitech.net.cn

J. 日期与时间
来源：http://cy.hahajie.cn

================================================================================
来源：http://ge.shxzskj.cn

[J01] 获取当前时间
来源：http://zo.szsharing.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pf.bjjhwx.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zm.szsharing.cn

JS:   new Date();  Date.now()
来源：http://an.yuexingan06.cn

TS:   new Date();  Date.now()
来源：http://mk.szxytkj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cl.huixinmuqiang.cn

Go:   time.Now()
来源：http://nb.haigaiapp.cn

Ruby: Time.now
来源：http://qr.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sf.wgjwhj.cn

[J02] 格式化输出
来源：http://xc.hnjuh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cm.colortex.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fm.yuntaijiaju.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://tc.huanxung.cn

TS:   d.toISOString()
来源：http://hk.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dk.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hu.hnjuh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://me.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iz.panjiajie.cn

[J03] 字符串解析为日期
来源：http://pp.shtwfgs.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://un.yuexingan06.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ci.9csxet.cn

JS:   new Date("2024-01-02")
来源：http://rj.shtwfgs.cn

TS:   new Date("2024-01-02")
来源：http://xt.yuexingan06.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vh.nszjky.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wa.chemitech.net.cn

Ruby: Date.parse("2024-01-02")
来源：http://gr.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ha.wgjwhj.cn

[J04] 时间戳与日期互转
来源：http://dx.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ra.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lo.yuntaijiaju.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://eq.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://fm.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rh.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rp.521024.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zp.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ya.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://gd.asd995.cn

Py:   now + timedelta(days=7)
来源：http://gr.nicolike.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ty.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zw.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hw.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://gh.bookmarksfly.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rs.shxzukj.cn

Ruby: Time.now + 7 * 86400
来源：http://gc.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://an.asd995.cn

[J06] 计算两时间之差
来源：http://bp.asd995.cn

Py:   (end - start).total_seconds()
来源：http://hd.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://gx.hahajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nt.szsharing.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://uz.jctech888.com.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cy.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://vb.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://ds.shxzukj.cn

C#:   (end - start).TotalSeconds
来源：http://qi.huixinmuqiang.cn

[J07] 比较两个日期
来源：http://ox.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://kc.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nc.9csxet.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hk.yuntaijiaju.cn

TS:   d1.getTime() < d2.getTime()
来源：http://uh.chemitech.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://po.yuexingan06.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://br.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://yc.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://fv.newstarts.cn

[J08] 提取年月日与星期
来源：http://rm.lnxyls.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qe.szxytkj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ya.shxzskj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://om.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dv.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bk.huanxung.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bm.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wm.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ro.bookmarksfly.cn

[J09] 时区处理
来源：http://ut.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uu.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rq.bjjhwx.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ec.lnxyls.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ix.jianghongdianzi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://se.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sd.haigaiapp.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yp.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gf.yuntaijiaju.cn

[J10] 取今天 / 本月第一天
来源：http://gj.wgjwhj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jc.jctech888.com.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vk.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qu.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tr.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://vd.huixinmuqiang.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tn.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fb.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://td.panjiajie.cn

================================================================================
来源：http://wx.asd995.cn

K. JSON 与序列化
来源：http://jg.hahajie.cn

================================================================================
来源：http://nl.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://ze.521024.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://re.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pc.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://bc.szxytkj.cn

TS:   JSON.stringify(obj)
来源：http://fo.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hq.hahajie.cn

Go:   json.Marshal(obj)
来源：http://lz.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mk.shxzskj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://no.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://yj.shtwfgs.cn

Py:   json.loads(s)
来源：http://xl.nicolike.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ha.szsharing.cn

JS:   JSON.parse(s)
来源：http://nf.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://lo.521024.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uz.nszjky.cn

Go:   json.Unmarshal(data, &v)
来源：http://lr.jianghongdianzi.cn

Ruby: JSON.parse(s)
来源：http://uf.jianghongdianzi.cn


<!-- 参考信息 -->