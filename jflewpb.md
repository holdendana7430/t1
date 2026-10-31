代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://cg.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pl.szsharing.cn

Java: enum Color { RED, GREEN }
来源：http://ih.huixinmuqiang.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ee.bjjhwx.cn

Ruby: Color = %i[red green].freeze
来源：http://fh.asd995.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pa.colortex.cn

[G16] 对象转数组 / 字典
来源：http://id.lnxyls.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tu.bjjhwx.cn

PHP:  get_object_vars($obj);
来源：http://rw.jianghongdianzi.cn

JS:   Object.entries(obj)
来源：http://ib.yuntaijiaju.cn

TS:   Object.entries(obj)
来源：http://wg.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wz.yuntaijiaju.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nw.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://zr.huixinmuqiang.cn

C#:   // 用反射或 System.Text.Json
来源：http://pm.asd995.cn

================================================================================
来源：http://ux.asd995.cn

H. 异常与错误处理
来源：http://zn.panjiajie.cn

================================================================================
来源：http://iy.9csxet.cn

[H01] try / catch 基础
来源：http://ul.colortex.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xx.9csxet.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hk.nszjky.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vt.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ez.asd995.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://io.nszjky.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ks.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ot.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://no.huixiangedu.cn

[H02] finally / ensure 收尾
来源：http://dt.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vo.lnxyls.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://if.hnjuh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://id.huixiangedu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qy.szxytkj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wh.panjiajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yv.shxzukj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vw.yuexingan06.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ii.asd995.cn

[H03] 主动抛出异常
来源：http://dn.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://vt.yuexingan06.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vf.9csxet.cn

JS:   throw new Error("错误信息");
来源：http://xm.nszjky.cn

TS:   throw new Error("错误信息");
来源：http://ep.panjiajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ra.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dl.haigaiapp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vj.jianghongdianzi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://to.shtwfgs.cn

[H04] 自定义异常类型
来源：http://mf.nszjky.cn

Py:   class MyError(Exception): pass
来源：http://no.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mp.szxytkj.cn

JS:   class MyError extends Error {}
来源：http://xp.nszjky.cn

TS:   class MyError extends Error {}
来源：http://fr.colortex.cn

Java: class MyException extends RuntimeException {}
来源：http://uy.lnxyls.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vu.huixinmuqiang.cn

Ruby: class MyError < StandardError; end
来源：http://lv.yuntaijiaju.cn

C#:   class MyException : Exception {}
来源：http://hc.yuexingan06.cn

[H05] 捕获特定类型
来源：http://ft.newstarts.cn

Py:   except ValueError as e:
来源：http://tw.jctech888.com.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://si.shxzskj.cn

JS:   if (e instanceof TypeError) {}
来源：http://pa.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://xz.panjiajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://qg.gzmigu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zh.huanxung.cn

Ruby: rescue ArgumentError => e
来源：http://lc.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://og.chemitech.net.cn

[H06] 可选值 / 空值安全访问
来源：http://vo.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://ef.jctech888.com.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cg.bjjhwx.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bo.jctech888.com.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xl.nszjky.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://vq.szxytkj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ft.nszjky.cn

Ruby: d&.dig(:a, :b)
来源：http://dy.hnjuh.cn

C#:   obj?.A?.B ?? default
来源：http://gl.huanxung.cn

[H07] 断言
来源：http://rx.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://it.szsharing.cn

PHP:  assert($x > 0);
来源：http://kl.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://hv.521024.cn

TS:   console.assert(x > 0);
来源：http://mz.huixiangedu.cn

Java: assert x > 0 : "必须为正";
来源：http://mt.haigaiapp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://px.9csxet.cn

Ruby: raise "必须为正" unless x > 0
来源：http://af.gzmigu.cn

C#:   Debug.Assert(x > 0);
来源：http://dy.shtwfgs.cn

[H08] 获取错误信息与堆栈
来源：http://ng.hnjuh.cn

Py:   str(e);  traceback.format_exc()
来源：http://nw.muxihuayi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mx.bjjhwx.cn

JS:   e.message;  e.stack
来源：http://oi.chemitech.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ga.szxytkj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xf.bjjhwx.cn

Go:   err.Error()
来源：http://ux.szsharing.cn

Ruby: e.message;  e.backtrace
来源：http://ul.haigaiapp.cn

C#:   e.Message;  e.StackTrace
来源：http://ok.huixinmuqiang.cn

[H09] 带错误码的异常
来源：http://xh.szsharing.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lj.colortex.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mk.bookmarksfly.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://gs.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://eo.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xm.gzmigu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sz.jianghongdianzi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ml.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ci.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://er.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fi.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xo.muxihuayi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jy.nszjky.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zw.jianghongdianzi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fs.jianghongdianzi.cn

Go:   defer f.Close()
来源：http://og.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rs.colortex.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sw.jctech888.com.cn

================================================================================
来源：http://bg.shxzskj.cn

I. 正则表达式
来源：http://ky.newstarts.cn

================================================================================
来源：http://do.hnjuh.cn

[I01] 判断是否匹配
来源：http://wn.szxytkj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vv.nszjky.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rn.huanxung.cn

JS:   /\d+/.test(s)
来源：http://yr.szsharing.cn

TS:   /\d+/.test(s)
来源：http://rr.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yp.nszjky.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ox.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://rk.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cm.shxzukj.cn

[I02] 提取所有匹配
来源：http://rx.lnxyls.cn

Py:   re.findall(r"\d+", s)
来源：http://ge.shxzskj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fc.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fh.wgjwhj.cn

TS:   s.match(/\d+/g)
来源：http://vl.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uy.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zu.haigaiapp.cn

Ruby: s.scan(/\d+/)
来源：http://ix.bookmarksfly.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ot.nszjky.cn

[I03] 提取捕获分组
来源：http://sm.szsharing.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ac.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bo.szxytkj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tl.huixiangedu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://de.chemitech.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ie.gzmigu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gm.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ug.huixiangedu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ez.szsharing.cn

[I04] 正则替换
来源：http://pi.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sp.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://px.huixinmuqiang.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pf.nszjky.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xs.muxihuayi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tf.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://nn.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://pf.9csxet.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ff.hahajie.cn

[I05] 按正则拆分
来源：http://aa.shxzskj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ha.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qs.shxzskj.cn

JS:   s.split(/\s*,\s*/)
来源：http://ko.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://gn.jctech888.com.cn

Java: s.split("\\s*,\\s*")
来源：http://jm.jctech888.com.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ug.hnjuh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nc.shtwfgs.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zz.huixinmuqiang.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bk.shtwfgs.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://sb.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ua.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wd.bjjhwx.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uw.hnjuh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wj.shxzskj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ad.huixiangedu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ya.huixiangedu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uj.yuntaijiaju.cn

[I07] 忽略大小写与多行模式
来源：http://ap.gzmigu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fh.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hp.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fv.huanxung.cn

TS:   /error/gim
来源：http://bo.yuntaijiaju.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ce.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cb.huixiangedu.cn

Ruby: s.scan(/error/i)
来源：http://ai.newstarts.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xz.shxzskj.cn

[I08] 贪婪与非贪婪匹配
来源：http://be.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ro.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ou.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yy.521024.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uc.bjjhwx.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nh.huixiangedu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cr.newstarts.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nx.colortex.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://eq.szsharing.cn

================================================================================
来源：http://kl.asd995.cn

J. 日期与时间
来源：http://pa.nszjky.cn

================================================================================
来源：http://fb.shxzukj.cn

[J01] 获取当前时间
来源：http://ai.szxytkj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pi.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://au.shtwfgs.cn

JS:   new Date();  Date.now()
来源：http://mg.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://qi.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ul.jctech888.com.cn

Go:   time.Now()
来源：http://fe.szxytkj.cn

Ruby: Time.now
来源：http://aw.521024.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lw.colortex.cn

[J02] 格式化输出
来源：http://zj.huixinmuqiang.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kl.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hr.colortex.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xw.panjiajie.cn

TS:   d.toISOString()
来源：http://sz.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://is.chemitech.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zt.nicolike.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jp.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ub.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://ut.nicolike.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hk.lnxyls.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ws.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://fn.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://yk.bookmarksfly.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hk.hnjuh.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://vc.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://mz.jctech888.com.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://by.bjjhwx.cn

[J04] 时间戳与日期互转
来源：http://tq.yuntaijiaju.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wi.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xd.nszjky.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yv.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ex.jianghongdianzi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vy.521024.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fv.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://dq.shxzukj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ps.shtwfgs.cn

[J05] 时间加减（加 7 天）
来源：http://mk.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://ot.huixinmuqiang.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ow.huanxung.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wq.huanxung.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ey.muxihuayi.cn

Java: LocalDate.now().plusDays(7)
来源：http://gn.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cv.lnxyls.cn

Ruby: Time.now + 7 * 86400
来源：http://nt.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qo.shxzukj.cn

[J06] 计算两时间之差
来源：http://nc.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://as.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://we.nszjky.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://en.huanxung.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ec.shtwfgs.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ui.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://mh.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://kb.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://cl.newstarts.cn

[J07] 比较两个日期
来源：http://eq.nszjky.cn

Py:   d1 < d2;  d1 == d2
来源：http://um.huanxung.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mk.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yr.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gs.bjjhwx.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://az.shxzukj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lw.chemitech.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ni.yuntaijiaju.cn

C#:   d1 < d2;  d1 == d2
来源：http://bv.wgjwhj.cn

[J08] 提取年月日与星期
来源：http://ma.521024.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wu.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://iu.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://by.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://oa.shxzukj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ts.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ay.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nl.yuntaijiaju.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gh.lnxyls.cn

[J09] 时区处理
来源：http://jp.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://at.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xh.9csxet.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qo.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://om.newstarts.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gl.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sb.newstarts.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yp.yuntaijiaju.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gw.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://vz.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://md.gzmigu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zp.huixiangedu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://od.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tx.asd995.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ki.yuexingan06.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jc.huanxung.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xz.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tc.muxihuayi.cn

================================================================================
来源：http://kr.gzmigu.cn

K. JSON 与序列化
来源：http://qx.haigaiapp.cn

================================================================================
来源：http://vy.yuntaijiaju.cn

[K01] 对象转 JSON 字符串
来源：http://ad.chemitech.net.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ys.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zn.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://da.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://jp.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ck.colortex.cn

Go:   json.Marshal(obj)
来源：http://af.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pc.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hp.chemitech.net.cn

[K02] JSON 字符串转对象
来源：http://vk.nszjky.cn

Py:   json.loads(s)
来源：http://sl.gzmigu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://di.newstarts.cn

JS:   JSON.parse(s)
来源：http://ii.szxytkj.cn

TS:   JSON.parse(s)
来源：http://vs.shxzukj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ji.haigaiapp.cn

Go:   json.Unmarshal(data, &v)
来源：http://kp.9csxet.cn

Ruby: JSON.parse(s)
来源：http://lp.colortex.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hc.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://bd.shxzukj.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sj.szsharing.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jz.huixiangedu.cn


<!-- 参考信息 -->