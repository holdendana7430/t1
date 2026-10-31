代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mc.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jc.gzmigu.cn

Java: enum Color { RED, GREEN }
来源：http://ol.asd995.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dh.huixinmuqiang.cn

Ruby: Color = %i[red green].freeze
来源：http://cn.wgjwhj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wx.szxytkj.cn

[G16] 对象转数组 / 字典
来源：http://lk.huixinmuqiang.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ve.wgjwhj.cn

PHP:  get_object_vars($obj);
来源：http://yc.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://jf.nicolike.cn

TS:   Object.entries(obj)
来源：http://qw.asd995.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://of.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://re.shtwfgs.cn

Ruby: obj.instance_variables
来源：http://up.wgjwhj.cn

C#:   // 用反射或 System.Text.Json
来源：http://mo.shtwfgs.cn

================================================================================
来源：http://tq.asd995.cn

H. 异常与错误处理
来源：http://ai.lnxyls.cn

================================================================================
来源：http://aj.yuntaijiaju.cn

[H01] try / catch 基础
来源：http://mg.hnjuh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cd.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://uc.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qz.shxzskj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://os.yuexingan06.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://af.szsharing.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zr.yuntaijiaju.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kh.521024.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ov.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://le.hnjuh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gn.gzmigu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yd.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bu.521024.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://oe.huixinmuqiang.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gr.yuexingan06.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ez.shxzukj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ch.nszjky.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gt.chemitech.net.cn

[H03] 主动抛出异常
来源：http://wy.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://tj.jianghongdianzi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nx.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://em.jctech888.com.cn

TS:   throw new Error("错误信息");
来源：http://jo.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rg.bjjhwx.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ho.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://du.shtwfgs.cn

C#:   throw new ArgumentException("错误信息");
来源：http://hz.gzmigu.cn

[H04] 自定义异常类型
来源：http://do.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://fx.gzmigu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ml.muxihuayi.cn

JS:   class MyError extends Error {}
来源：http://ze.wgjwhj.cn

TS:   class MyError extends Error {}
来源：http://wv.szxytkj.cn

Java: class MyException extends RuntimeException {}
来源：http://mh.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vg.haigaiapp.cn

Ruby: class MyError < StandardError; end
来源：http://lf.panjiajie.cn

C#:   class MyException : Exception {}
来源：http://dq.yuexingan06.cn

[H05] 捕获特定类型
来源：http://xq.muxihuayi.cn

Py:   except ValueError as e:
来源：http://qp.nszjky.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mn.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://dx.huixinmuqiang.cn

TS:   if (e instanceof TypeError) {}
来源：http://yj.9csxet.cn

Java: catch (IOException | SQLException e) {}
来源：http://gk.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mt.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://fi.gzmigu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cz.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://pc.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://ms.muxihuayi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pi.hnjuh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jj.asd995.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wb.shxzukj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://lx.nszjky.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://em.jctech888.com.cn

Ruby: d&.dig(:a, :b)
来源：http://ms.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://rk.panjiajie.cn

[H07] 断言
来源：http://ra.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://hw.nicolike.cn

PHP:  assert($x > 0);
来源：http://yc.yuexingan06.cn

JS:   console.assert(x > 0);
来源：http://ij.newstarts.cn

TS:   console.assert(x > 0);
来源：http://ue.muxihuayi.cn

Java: assert x > 0 : "必须为正";
来源：http://iv.nicolike.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yf.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hp.nszjky.cn

C#:   Debug.Assert(x > 0);
来源：http://ki.yuexingan06.cn

[H08] 获取错误信息与堆栈
来源：http://nm.chemitech.net.cn

Py:   str(e);  traceback.format_exc()
来源：http://li.huanxung.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ac.haigaiapp.cn

JS:   e.message;  e.stack
来源：http://eg.jctech888.com.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://tk.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ye.huixinmuqiang.cn

Go:   err.Error()
来源：http://oj.hnjuh.cn

Ruby: e.message;  e.backtrace
来源：http://ti.muxihuayi.cn

C#:   e.Message;  e.StackTrace
来源：http://lv.9csxet.cn

[H09] 带错误码的异常
来源：http://it.asd995.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nq.nicolike.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nc.shxzskj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://yu.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ni.521024.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zb.nicolike.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://lj.chemitech.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pc.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wp.lnxyls.cn

[H10] 资源自动释放
来源：http://sd.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://tr.shxzukj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://rx.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://su.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://it.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kb.wgjwhj.cn

Go:   defer f.Close()
来源：http://bf.huixinmuqiang.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://km.szsharing.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ee.521024.cn

================================================================================
来源：http://hk.nszjky.cn

I. 正则表达式
来源：http://kw.shtwfgs.cn

================================================================================
来源：http://mu.szsharing.cn

[I01] 判断是否匹配
来源：http://er.hnjuh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tv.shtwfgs.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mh.bjjhwx.cn

JS:   /\d+/.test(s)
来源：http://ww.haigaiapp.cn

TS:   /\d+/.test(s)
来源：http://fi.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xo.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bm.newstarts.cn

Ruby: s.match?(/\d+/)
来源：http://rz.nicolike.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lo.hnjuh.cn

[I02] 提取所有匹配
来源：http://pb.9csxet.cn

Py:   re.findall(r"\d+", s)
来源：http://oa.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://js.bjjhwx.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tz.wgjwhj.cn

TS:   s.match(/\d+/g)
来源：http://zu.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sp.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ph.yuexingan06.cn

Ruby: s.scan(/\d+/)
来源：http://zc.yuexingan06.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tq.jctech888.com.cn

[I03] 提取捕获分组
来源：http://ko.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://kh.wgjwhj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dl.521024.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ph.newstarts.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dj.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pg.bjjhwx.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sr.huanxung.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sl.szsharing.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jd.szxytkj.cn

[I04] 正则替换
来源：http://vw.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xs.bookmarksfly.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wu.bookmarksfly.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zl.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sp.huixiangedu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ax.huixinmuqiang.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xr.haigaiapp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jb.9csxet.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ej.szsharing.cn

[I05] 按正则拆分
来源：http://va.muxihuayi.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wi.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jl.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://ad.nszjky.cn

TS:   s.split(/\s*,\s*/)
来源：http://uc.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://jk.asd995.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mo.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kj.muxihuayi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jb.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://rc.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nb.wgjwhj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hm.panjiajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gp.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tb.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://tk.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kx.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hh.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ay.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://vu.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tc.jianghongdianzi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wf.bjjhwx.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://oi.huixiangedu.cn

TS:   /error/gim
来源：http://ch.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fo.jctech888.com.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bf.bookmarksfly.cn

Ruby: s.scan(/error/i)
来源：http://us.huixiangedu.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qb.nicolike.cn

[I08] 贪婪与非贪婪匹配
来源：http://hx.jianghongdianzi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vw.hnjuh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zm.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xj.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xb.shtwfgs.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lr.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jb.lnxyls.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://no.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uc.jctech888.com.cn

================================================================================
来源：http://vp.521024.cn

J. 日期与时间
来源：http://cb.yuntaijiaju.cn

================================================================================
来源：http://gv.hahajie.cn

[J01] 获取当前时间
来源：http://pw.hnjuh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://sl.shtwfgs.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://eb.9csxet.cn

JS:   new Date();  Date.now()
来源：http://uy.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://ok.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ms.asd995.cn

Go:   time.Now()
来源：http://yo.bookmarksfly.cn

Ruby: Time.now
来源：http://pn.szxytkj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mz.shxzukj.cn

[J02] 格式化输出
来源：http://ev.panjiajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yx.gzmigu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qy.shtwfgs.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fs.colortex.cn

TS:   d.toISOString()
来源：http://ys.shxzukj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bi.newstarts.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gt.nszjky.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pu.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oc.asd995.cn

[J03] 字符串解析为日期
来源：http://yh.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ut.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kh.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://rs.huixiangedu.cn

TS:   new Date("2024-01-02")
来源：http://ab.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ww.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://om.shxzukj.cn

Ruby: Date.parse("2024-01-02")
来源：http://dy.9csxet.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ue.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://ip.nicolike.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://dm.shxzukj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ke.yuexingan06.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://my.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cj.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jq.jianghongdianzi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rz.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://na.yuntaijiaju.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uw.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://im.bjjhwx.cn

Py:   now + timedelta(days=7)
来源：http://po.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ai.newstarts.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rf.chemitech.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rw.bjjhwx.cn

Java: LocalDate.now().plusDays(7)
来源：http://fo.lnxyls.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gh.shxzukj.cn

Ruby: Time.now + 7 * 86400
来源：http://mk.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hn.hnjuh.cn

[J06] 计算两时间之差
来源：http://mf.chemitech.net.cn

Py:   (end - start).total_seconds()
来源：http://ck.nicolike.cn

PHP:  $end->diff($start)->days;
来源：http://gs.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yr.yuntaijiaju.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nl.nszjky.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nu.muxihuayi.cn

Go:   end.Sub(start).Hours()
来源：http://ln.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://kr.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://nq.colortex.cn

[J07] 比较两个日期
来源：http://fq.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://va.nicolike.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bl.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qx.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cc.shxzskj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ai.bookmarksfly.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lc.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wh.haigaiapp.cn

C#:   d1 < d2;  d1 == d2
来源：http://sd.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://fn.jctech888.com.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jw.lnxyls.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nk.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qk.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ol.shxzukj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vj.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://as.haigaiapp.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://op.shxzskj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lq.9csxet.cn

[J09] 时区处理
来源：http://xg.asd995.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vc.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rx.shxzukj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lc.9csxet.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jc.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://oo.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://cd.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dz.521024.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wk.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://zu.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://fi.shtwfgs.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vv.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mj.jianghongdianzi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://iz.huixiangedu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bm.jctech888.com.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dn.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vo.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zp.yuexingan06.cn

================================================================================
来源：http://sm.wgjwhj.cn

K. JSON 与序列化
来源：http://us.haigaiapp.cn

================================================================================
来源：http://zz.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://zo.nicolike.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://er.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pr.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://et.nicolike.cn

TS:   JSON.stringify(obj)
来源：http://to.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://do.lnxyls.cn

Go:   json.Marshal(obj)
来源：http://vw.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://py.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vk.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://tn.521024.cn

Py:   json.loads(s)
来源：http://wm.asd995.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://or.asd995.cn

JS:   JSON.parse(s)
来源：http://kw.nicolike.cn

TS:   JSON.parse(s)
来源：http://ul.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ah.panjiajie.cn

Go:   json.Unmarshal(data, &v)
来源：http://jf.newstarts.cn

Ruby: JSON.parse(s)
来源：http://hs.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://va.gzmigu.cn

[K03] JSON 美化输出（带缩进）
来源：http://uz.lnxyls.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dv.haigaiapp.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oy.colortex.cn


<!-- 参考信息 -->