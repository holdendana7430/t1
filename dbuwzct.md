代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xa.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hb.jianghongdianzi.cn

Java: enum Color { RED, GREEN }
来源：http://ck.huixinmuqiang.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qd.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://bc.jctech888.com.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qf.szsharing.cn

[G16] 对象转数组 / 字典
来源：http://wm.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lq.newstarts.cn

PHP:  get_object_vars($obj);
来源：http://dx.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://zq.wgjwhj.cn

TS:   Object.entries(obj)
来源：http://bc.hahajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mh.shxzskj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mv.muxihuayi.cn

Ruby: obj.instance_variables
来源：http://ye.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://xu.nicolike.cn

================================================================================
来源：http://fj.colortex.cn

H. 异常与错误处理
来源：http://wq.shtwfgs.cn

================================================================================
来源：http://gw.shxzukj.cn

[H01] try / catch 基础
来源：http://tg.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ln.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bq.nszjky.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wp.haigaiapp.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dd.shxzukj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qe.shxzukj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ff.asd995.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lz.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dt.nszjky.cn

[H02] finally / ensure 收尾
来源：http://ui.bookmarksfly.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zx.huixinmuqiang.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bf.hnjuh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zd.9csxet.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gp.nszjky.cn

Java: try { f(); } finally { cleanup(); }
来源：http://is.newstarts.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ej.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ot.nszjky.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://js.chemitech.net.cn

[H03] 主动抛出异常
来源：http://ru.jctech888.com.cn

Py:   raise ValueError("错误信息")
来源：http://ks.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://my.hnjuh.cn

JS:   throw new Error("错误信息");
来源：http://gm.shxzukj.cn

TS:   throw new Error("错误信息");
来源：http://qk.yuntaijiaju.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://zb.szsharing.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nl.szsharing.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bc.bookmarksfly.cn

C#:   throw new ArgumentException("错误信息");
来源：http://np.chemitech.net.cn

[H04] 自定义异常类型
来源：http://ul.shxzukj.cn

Py:   class MyError(Exception): pass
来源：http://tf.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mz.bjjhwx.cn

JS:   class MyError extends Error {}
来源：http://hf.panjiajie.cn

TS:   class MyError extends Error {}
来源：http://yh.newstarts.cn

Java: class MyException extends RuntimeException {}
来源：http://rh.huixinmuqiang.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rw.521024.cn

Ruby: class MyError < StandardError; end
来源：http://kr.jianghongdianzi.cn

C#:   class MyException : Exception {}
来源：http://xe.9csxet.cn

[H05] 捕获特定类型
来源：http://cf.shxzskj.cn

Py:   except ValueError as e:
来源：http://nd.colortex.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ag.haigaiapp.cn

JS:   if (e instanceof TypeError) {}
来源：http://cr.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://cb.huanxung.cn

Java: catch (IOException | SQLException e) {}
来源：http://eb.haigaiapp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fi.nicolike.cn

Ruby: rescue ArgumentError => e
来源：http://qp.shxzskj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ic.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://aq.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://ik.hnjuh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://pm.nicolike.cn

JS:   obj?.a?.b;  d ?? default
来源：http://db.huixiangedu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bd.jianghongdianzi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fg.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pb.jianghongdianzi.cn

Ruby: d&.dig(:a, :b)
来源：http://fq.gzmigu.cn

C#:   obj?.A?.B ?? default
来源：http://tf.521024.cn

[H07] 断言
来源：http://pu.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://rb.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://bt.gzmigu.cn

JS:   console.assert(x > 0);
来源：http://ji.yuntaijiaju.cn

TS:   console.assert(x > 0);
来源：http://eg.lnxyls.cn

Java: assert x > 0 : "必须为正";
来源：http://eg.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rq.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ri.nicolike.cn

C#:   Debug.Assert(x > 0);
来源：http://wr.chemitech.net.cn

[H08] 获取错误信息与堆栈
来源：http://qf.huixiangedu.cn

Py:   str(e);  traceback.format_exc()
来源：http://gp.wgjwhj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mr.szsharing.cn

JS:   e.message;  e.stack
来源：http://ez.nicolike.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://yg.lnxyls.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xv.hnjuh.cn

Go:   err.Error()
来源：http://hi.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://gn.muxihuayi.cn

C#:   e.Message;  e.StackTrace
来源：http://fp.bjjhwx.cn

[H09] 带错误码的异常
来源：http://ha.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qm.chemitech.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hu.bjjhwx.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://lk.gzmigu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://dw.gzmigu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://am.bjjhwx.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xv.haigaiapp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zp.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xl.colortex.cn

[H10] 资源自动释放
来源：http://yd.lnxyls.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://it.szxytkj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vt.yuexingan06.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://yr.muxihuayi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://bv.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lu.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://gr.shxzskj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yw.gzmigu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sw.huanxung.cn

================================================================================
来源：http://kc.asd995.cn

I. 正则表达式
来源：http://fy.gzmigu.cn

================================================================================
来源：http://pa.shxzskj.cn

[I01] 判断是否匹配
来源：http://bk.panjiajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yl.lnxyls.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tu.huanxung.cn

JS:   /\d+/.test(s)
来源：http://ct.nszjky.cn

TS:   /\d+/.test(s)
来源：http://lh.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://do.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jd.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://zy.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ol.szxytkj.cn

[I02] 提取所有匹配
来源：http://on.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://jd.asd995.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rx.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ha.hnjuh.cn

TS:   s.match(/\d+/g)
来源：http://uw.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cl.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nw.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://pm.szxytkj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xa.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://vw.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://dg.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://sr.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ji.hahajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nr.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://is.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fg.szxytkj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hr.szsharing.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://im.szxytkj.cn

[I04] 正则替换
来源：http://zv.asd995.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sa.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://zv.wgjwhj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hw.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sf.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://yf.gzmigu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bm.shxzukj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mo.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kz.haigaiapp.cn

[I05] 按正则拆分
来源：http://ka.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ua.wgjwhj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qs.huixinmuqiang.cn

JS:   s.split(/\s*,\s*/)
来源：http://se.yuexingan06.cn

TS:   s.split(/\s*,\s*/)
来源：http://zu.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://yd.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://qk.shxzskj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bk.jctech888.com.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ge.haigaiapp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xk.bookmarksfly.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rf.jctech888.com.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pa.nszjky.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fw.jianghongdianzi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vk.yuexingan06.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://le.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://oy.newstarts.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://mm.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dk.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://fx.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vv.asd995.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vp.jianghongdianzi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zm.panjiajie.cn

TS:   /error/gim
来源：http://uc.hahajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zh.asd995.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://om.jianghongdianzi.cn

Ruby: s.scan(/error/i)
来源：http://jq.muxihuayi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ag.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://pj.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ck.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://md.521024.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hu.lnxyls.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://wu.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mt.haigaiapp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://et.9csxet.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mj.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fu.newstarts.cn

================================================================================
来源：http://bw.chemitech.net.cn

J. 日期与时间
来源：http://lr.haigaiapp.cn

================================================================================
来源：http://wm.panjiajie.cn

[J01] 获取当前时间
来源：http://tm.huixinmuqiang.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vq.szxytkj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ng.gzmigu.cn

JS:   new Date();  Date.now()
来源：http://tl.muxihuayi.cn

TS:   new Date();  Date.now()
来源：http://rp.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://oa.nicolike.cn

Go:   time.Now()
来源：http://jh.bjjhwx.cn

Ruby: Time.now
来源：http://bz.huixinmuqiang.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gi.wgjwhj.cn

[J02] 格式化输出
来源：http://pf.jianghongdianzi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ex.bjjhwx.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://wq.shxzskj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://te.bookmarksfly.cn

TS:   d.toISOString()
来源：http://wk.hnjuh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wf.521024.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fu.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fv.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ap.gzmigu.cn

[J03] 字符串解析为日期
来源：http://he.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bk.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zx.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://en.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://ar.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ix.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bp.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://uo.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ff.jianghongdianzi.cn

[J04] 时间戳与日期互转
来源：http://yh.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://oh.huixiangedu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ig.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ek.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dg.hnjuh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://de.jctech888.com.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bk.huixiangedu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://lm.lnxyls.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://dv.hahajie.cn

[J05] 时间加减（加 7 天）
来源：http://nv.huixiangedu.cn

Py:   now + timedelta(days=7)
来源：http://om.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uq.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hv.huixiangedu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hf.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://ss.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oi.yuexingan06.cn

Ruby: Time.now + 7 * 86400
来源：http://hv.jianghongdianzi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://es.newstarts.cn

[J06] 计算两时间之差
来源：http://gg.asd995.cn

Py:   (end - start).total_seconds()
来源：http://hu.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://pd.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ls.panjiajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://us.shxzskj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ak.muxihuayi.cn

Go:   end.Sub(start).Hours()
来源：http://sp.hnjuh.cn

Ruby: end - start                 # 返回秒数
来源：http://cr.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://qn.nszjky.cn

[J07] 比较两个日期
来源：http://xj.huanxung.cn

Py:   d1 < d2;  d1 == d2
来源：http://rd.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bj.shxzskj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rv.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://he.521024.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ys.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lb.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://td.hnjuh.cn

C#:   d1 < d2;  d1 == d2
来源：http://jq.shxzukj.cn

[J08] 提取年月日与星期
来源：http://hc.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xy.panjiajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rq.huanxung.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kf.nszjky.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qe.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://si.huixiangedu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://em.asd995.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zk.szxytkj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pk.gzmigu.cn

[J09] 时区处理
来源：http://vo.shtwfgs.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://pj.nicolike.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bd.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lm.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kg.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zk.jctech888.com.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ve.szsharing.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dt.shxzukj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cm.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://yj.wgjwhj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://za.gzmigu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zx.huanxung.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yw.haigaiapp.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fi.colortex.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cp.yuntaijiaju.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vw.jctech888.com.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jo.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mz.bookmarksfly.cn

================================================================================
来源：http://oq.huixiangedu.cn

K. JSON 与序列化
来源：http://pe.shtwfgs.cn

================================================================================
来源：http://ua.bookmarksfly.cn

[K01] 对象转 JSON 字符串
来源：http://to.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zd.9csxet.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rw.szxytkj.cn

JS:   JSON.stringify(obj)
来源：http://dr.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://id.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jf.asd995.cn

Go:   json.Marshal(obj)
来源：http://ty.bjjhwx.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ru.szxytkj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zt.521024.cn

[K02] JSON 字符串转对象
来源：http://qg.hnjuh.cn

Py:   json.loads(s)
来源：http://gy.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xz.huixinmuqiang.cn

JS:   JSON.parse(s)
来源：http://sc.szsharing.cn

TS:   JSON.parse(s)
来源：http://es.huixiangedu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uk.asd995.cn

Go:   json.Unmarshal(data, &v)
来源：http://ok.bookmarksfly.cn

Ruby: JSON.parse(s)
来源：http://ng.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zp.colortex.cn

[K03] JSON 美化输出（带缩进）
来源：http://zp.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rp.nszjky.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vh.shxzskj.cn


<!-- 参考信息 -->