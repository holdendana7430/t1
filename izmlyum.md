代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://by.shxzukj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ee.haigaiapp.cn

Java: enum Color { RED, GREEN }
来源：http://zo.huixiangedu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://te.shxzskj.cn

Ruby: Color = %i[red green].freeze
来源：http://br.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gj.huanxung.cn

[G16] 对象转数组 / 字典
来源：http://ox.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ay.huanxung.cn

PHP:  get_object_vars($obj);
来源：http://rw.jianghongdianzi.cn

JS:   Object.entries(obj)
来源：http://np.hahajie.cn

TS:   Object.entries(obj)
来源：http://nm.shtwfgs.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ee.huixiangedu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tp.szsharing.cn

Ruby: obj.instance_variables
来源：http://hx.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://ve.szxytkj.cn

================================================================================
来源：http://rk.521024.cn

H. 异常与错误处理
来源：http://pd.9csxet.cn

================================================================================
来源：http://mp.haigaiapp.cn

[H01] try / catch 基础
来源：http://uh.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ut.muxihuayi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ce.yuexingan06.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zk.hnjuh.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hf.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ny.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tz.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yi.hahajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://we.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://aj.bookmarksfly.cn

Py:   try: f()⏎finally: cleanup()
来源：http://eq.yuntaijiaju.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fl.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qo.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://wh.jctech888.com.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dg.yuntaijiaju.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://oi.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://rx.newstarts.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://oe.szsharing.cn

[H03] 主动抛出异常
来源：http://ao.gzmigu.cn

Py:   raise ValueError("错误信息")
来源：http://jq.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cm.nicolike.cn

JS:   throw new Error("错误信息");
来源：http://et.521024.cn

TS:   throw new Error("错误信息");
来源：http://iq.bjjhwx.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://iz.szsharing.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ai.9csxet.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://cb.bookmarksfly.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jp.nicolike.cn

[H04] 自定义异常类型
来源：http://nx.asd995.cn

Py:   class MyError(Exception): pass
来源：http://ig.9csxet.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dn.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://ek.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://hd.newstarts.cn

Java: class MyException extends RuntimeException {}
来源：http://me.lnxyls.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ga.shxzskj.cn

Ruby: class MyError < StandardError; end
来源：http://lu.9csxet.cn

C#:   class MyException : Exception {}
来源：http://iw.huixiangedu.cn

[H05] 捕获特定类型
来源：http://gn.521024.cn

Py:   except ValueError as e:
来源：http://mv.gzmigu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://in.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://ul.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://vq.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://pp.yuntaijiaju.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://gu.shxzskj.cn

Ruby: rescue ArgumentError => e
来源：http://gw.huixinmuqiang.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://iv.asd995.cn

[H06] 可选值 / 空值安全访问
来源：http://bm.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://si.panjiajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bh.szxytkj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ga.colortex.cn

TS:   obj?.a?.b;  d ?? default
来源：http://af.shxzukj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://so.nicolike.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://uo.szsharing.cn

Ruby: d&.dig(:a, :b)
来源：http://lt.panjiajie.cn

C#:   obj?.A?.B ?? default
来源：http://um.huixiangedu.cn

[H07] 断言
来源：http://zi.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://dh.yuntaijiaju.cn

PHP:  assert($x > 0);
来源：http://mr.huixinmuqiang.cn

JS:   console.assert(x > 0);
来源：http://yc.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://hx.shtwfgs.cn

Java: assert x > 0 : "必须为正";
来源：http://my.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ja.jianghongdianzi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ro.huixiangedu.cn

C#:   Debug.Assert(x > 0);
来源：http://jd.panjiajie.cn

[H08] 获取错误信息与堆栈
来源：http://mw.muxihuayi.cn

Py:   str(e);  traceback.format_exc()
来源：http://oy.gzmigu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tu.hahajie.cn

JS:   e.message;  e.stack
来源：http://sf.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://uk.wgjwhj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://mq.szxytkj.cn

Go:   err.Error()
来源：http://jd.jctech888.com.cn

Ruby: e.message;  e.backtrace
来源：http://lh.lnxyls.cn

C#:   e.Message;  e.StackTrace
来源：http://yt.yuntaijiaju.cn

[H09] 带错误码的异常
来源：http://eu.shxzskj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hk.521024.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ka.jctech888.com.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mp.9csxet.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jg.lnxyls.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tw.haigaiapp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wh.hnjuh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://nu.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rl.shxzskj.cn

[H10] 资源自动释放
来源：http://uh.nicolike.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://uy.shxzskj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hu.yuntaijiaju.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jr.nicolike.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ge.bjjhwx.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yy.bookmarksfly.cn

Go:   defer f.Close()
来源：http://gc.bookmarksfly.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ld.jctech888.com.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nd.haigaiapp.cn

================================================================================
来源：http://yh.newstarts.cn

I. 正则表达式
来源：http://du.bookmarksfly.cn

================================================================================
来源：http://uv.huixiangedu.cn

[I01] 判断是否匹配
来源：http://yf.shxzukj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://zx.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://my.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://jj.shtwfgs.cn

TS:   /\d+/.test(s)
来源：http://zu.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zf.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cz.hnjuh.cn

Ruby: s.match?(/\d+/)
来源：http://yy.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xo.hahajie.cn

[I02] 提取所有匹配
来源：http://jr.jianghongdianzi.cn

Py:   re.findall(r"\d+", s)
来源：http://ex.yuexingan06.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vl.yuexingan06.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://up.haigaiapp.cn

TS:   s.match(/\d+/g)
来源：http://km.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ka.hahajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wp.newstarts.cn

Ruby: s.scan(/\d+/)
来源：http://dw.lnxyls.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://yo.nicolike.cn

[I03] 提取捕获分组
来源：http://ll.lnxyls.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dz.newstarts.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yw.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jk.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bj.szsharing.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nl.colortex.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pq.colortex.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qu.huanxung.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yo.hahajie.cn

[I04] 正则替换
来源：http://gb.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ka.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fu.muxihuayi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cl.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vq.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mg.colortex.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://um.chemitech.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bw.huanxung.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://in.shxzskj.cn

[I05] 按正则拆分
来源：http://fw.bookmarksfly.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dp.szxytkj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qh.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://sf.muxihuayi.cn

TS:   s.split(/\s*,\s*/)
来源：http://rg.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://je.gzmigu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bk.bjjhwx.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mx.bjjhwx.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xt.gzmigu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://bc.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://wj.shxzukj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://us.nicolike.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bq.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vg.yuntaijiaju.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xl.jctech888.com.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ko.shxzskj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ii.bookmarksfly.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ur.colortex.cn

[I07] 忽略大小写与多行模式
来源：http://yp.chemitech.net.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rc.huixiangedu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zr.szxytkj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://js.panjiajie.cn

TS:   /error/gim
来源：http://sl.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wj.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://im.asd995.cn

Ruby: s.scan(/error/i)
来源：http://qr.jctech888.com.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qs.nicolike.cn

[I08] 贪婪与非贪婪匹配
来源：http://za.huanxung.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://li.huixiangedu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yu.huixiangedu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zx.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ri.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xb.bjjhwx.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ly.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ow.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://kt.huixinmuqiang.cn

================================================================================
来源：http://ez.panjiajie.cn

J. 日期与时间
来源：http://oi.shxzskj.cn

================================================================================
来源：http://at.huanxung.cn

[J01] 获取当前时间
来源：http://wf.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ts.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fh.jianghongdianzi.cn

JS:   new Date();  Date.now()
来源：http://xu.nicolike.cn

TS:   new Date();  Date.now()
来源：http://mu.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hk.huixinmuqiang.cn

Go:   time.Now()
来源：http://if.szxytkj.cn

Ruby: Time.now
来源：http://pe.huixinmuqiang.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://io.haigaiapp.cn

[J02] 格式化输出
来源：http://ly.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://id.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://tm.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lh.colortex.cn

TS:   d.toISOString()
来源：http://cv.jianghongdianzi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gb.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://as.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ff.szxytkj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://aq.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://xx.huixiangedu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://kw.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://sy.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://lx.bookmarksfly.cn

TS:   new Date("2024-01-02")
来源：http://pn.muxihuayi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://kx.yuexingan06.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gd.huanxung.cn

Ruby: Date.parse("2024-01-02")
来源：http://oj.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://eh.yuexingan06.cn

[J04] 时间戳与日期互转
来源：http://vs.muxihuayi.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://de.huanxung.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kh.huanxung.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://yx.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yw.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yx.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yf.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ty.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hr.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://lh.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://yw.shxzskj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ez.jianghongdianzi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ha.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qy.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://so.shtwfgs.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jc.9csxet.cn

Ruby: Time.now + 7 * 86400
来源：http://yu.shxzskj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ae.shtwfgs.cn

[J06] 计算两时间之差
来源：http://ak.521024.cn

Py:   (end - start).total_seconds()
来源：http://si.9csxet.cn

PHP:  $end->diff($start)->days;
来源：http://uf.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yp.szxytkj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gc.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kb.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://ap.yuntaijiaju.cn

Ruby: end - start                 # 返回秒数
来源：http://sk.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://xe.jianghongdianzi.cn

[J07] 比较两个日期
来源：http://ww.lnxyls.cn

Py:   d1 < d2;  d1 == d2
来源：http://sg.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bd.jctech888.com.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qy.shxzskj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://lu.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hs.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://no.szsharing.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rh.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://yx.huanxung.cn

[J08] 提取年月日与星期
来源：http://sf.bookmarksfly.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hj.jctech888.com.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qq.shxzukj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wo.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://zp.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ca.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gd.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://km.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ft.muxihuayi.cn

[J09] 时区处理
来源：http://ve.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://fh.shtwfgs.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lp.jianghongdianzi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vc.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sp.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lz.chemitech.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xa.yuntaijiaju.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qs.newstarts.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xu.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://ix.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jg.yuntaijiaju.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mt.9csxet.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ey.nicolike.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gr.hahajie.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dj.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xs.colortex.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://po.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vb.shxzskj.cn

================================================================================
来源：http://gl.bookmarksfly.cn

K. JSON 与序列化
来源：http://lz.yuntaijiaju.cn

================================================================================
来源：http://ug.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://tb.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kw.gzmigu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bg.9csxet.cn

JS:   JSON.stringify(obj)
来源：http://lu.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://oe.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nf.nszjky.cn

Go:   json.Marshal(obj)
来源：http://sl.hnjuh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://df.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rf.nicolike.cn

[K02] JSON 字符串转对象
来源：http://bm.gzmigu.cn

Py:   json.loads(s)
来源：http://ft.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kx.colortex.cn

JS:   JSON.parse(s)
来源：http://xx.gzmigu.cn

TS:   JSON.parse(s)
来源：http://nd.haigaiapp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ky.huixinmuqiang.cn

Go:   json.Unmarshal(data, &v)
来源：http://nk.shxzskj.cn

Ruby: JSON.parse(s)
来源：http://xd.hahajie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qv.huixiangedu.cn

[K03] JSON 美化输出（带缩进）
来源：http://wb.huixiangedu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tr.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dp.shxzskj.cn


<!-- 参考信息 -->