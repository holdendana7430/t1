代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xl.hahajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zo.bjjhwx.cn

Java: enum Color { RED, GREEN }
来源：http://pi.nicolike.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://le.jianghongdianzi.cn

Ruby: Color = %i[red green].freeze
来源：http://pv.bookmarksfly.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ai.huixiangedu.cn

[G16] 对象转数组 / 字典
来源：http://qa.huixinmuqiang.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hi.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://fh.gzmigu.cn

JS:   Object.entries(obj)
来源：http://ee.9csxet.cn

TS:   Object.entries(obj)
来源：http://tq.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://uc.shxzskj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ok.lnxyls.cn

Ruby: obj.instance_variables
来源：http://qj.gzmigu.cn

C#:   // 用反射或 System.Text.Json
来源：http://ri.521024.cn

================================================================================
来源：http://xp.szsharing.cn

H. 异常与错误处理
来源：http://ux.chemitech.net.cn

================================================================================
来源：http://sa.shtwfgs.cn

[H01] try / catch 基础
来源：http://eu.hnjuh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kk.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fn.shxzskj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xd.muxihuayi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lj.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wn.yuntaijiaju.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pk.bjjhwx.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ua.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pg.shtwfgs.cn

[H02] finally / ensure 收尾
来源：http://og.szxytkj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yp.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xg.newstarts.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mj.chemitech.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://eg.szxytkj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ke.lnxyls.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://df.hahajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kj.shtwfgs.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bw.shtwfgs.cn

[H03] 主动抛出异常
来源：http://bd.bookmarksfly.cn

Py:   raise ValueError("错误信息")
来源：http://nv.haigaiapp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tj.huanxung.cn

JS:   throw new Error("错误信息");
来源：http://jo.szxytkj.cn

TS:   throw new Error("错误信息");
来源：http://kz.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fk.colortex.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gw.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wt.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qz.szxytkj.cn

[H04] 自定义异常类型
来源：http://kt.bjjhwx.cn

Py:   class MyError(Exception): pass
来源：http://mx.521024.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nj.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://ae.chemitech.net.cn

TS:   class MyError extends Error {}
来源：http://iq.lnxyls.cn

Java: class MyException extends RuntimeException {}
来源：http://yv.huixinmuqiang.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fh.jianghongdianzi.cn

Ruby: class MyError < StandardError; end
来源：http://pk.newstarts.cn

C#:   class MyException : Exception {}
来源：http://vm.huixiangedu.cn

[H05] 捕获特定类型
来源：http://vz.hnjuh.cn

Py:   except ValueError as e:
来源：http://fz.yuexingan06.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://eg.jianghongdianzi.cn

JS:   if (e instanceof TypeError) {}
来源：http://no.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://om.521024.cn

Java: catch (IOException | SQLException e) {}
来源：http://fy.nszjky.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cf.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://cr.hnjuh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ia.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://ad.chemitech.net.cn

Py:   value = d.get("k") or default
来源：http://sj.huanxung.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cm.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mh.gzmigu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fz.hnjuh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://nn.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jf.szsharing.cn

Ruby: d&.dig(:a, :b)
来源：http://ub.shtwfgs.cn

C#:   obj?.A?.B ?? default
来源：http://pl.hahajie.cn

[H07] 断言
来源：http://bo.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://ye.wgjwhj.cn

PHP:  assert($x > 0);
来源：http://rw.nicolike.cn

JS:   console.assert(x > 0);
来源：http://yf.haigaiapp.cn

TS:   console.assert(x > 0);
来源：http://ls.jianghongdianzi.cn

Java: assert x > 0 : "必须为正";
来源：http://mm.huixinmuqiang.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lj.bjjhwx.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ec.bookmarksfly.cn

C#:   Debug.Assert(x > 0);
来源：http://cs.haigaiapp.cn

[H08] 获取错误信息与堆栈
来源：http://kt.colortex.cn

Py:   str(e);  traceback.format_exc()
来源：http://js.shxzskj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://oc.szsharing.cn

JS:   e.message;  e.stack
来源：http://lb.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hk.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://js.huixiangedu.cn

Go:   err.Error()
来源：http://dy.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://mw.huixiangedu.cn

C#:   e.Message;  e.StackTrace
来源：http://uc.colortex.cn

[H09] 带错误码的异常
来源：http://gk.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qd.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kk.shxzskj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://my.jianghongdianzi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://on.huixiangedu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xo.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://uy.jianghongdianzi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mf.bjjhwx.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gh.huanxung.cn

[H10] 资源自动释放
来源：http://bb.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ao.jctech888.com.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mv.asd995.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://dt.hnjuh.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sf.haigaiapp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mu.asd995.cn

Go:   defer f.Close()
来源：http://mz.nszjky.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wa.huixinmuqiang.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ab.huixinmuqiang.cn

================================================================================
来源：http://xy.szxytkj.cn

I. 正则表达式
来源：http://io.nszjky.cn

================================================================================
来源：http://ql.szxytkj.cn

[I01] 判断是否匹配
来源：http://ue.521024.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wx.bookmarksfly.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qs.szxytkj.cn

JS:   /\d+/.test(s)
来源：http://xy.colortex.cn

TS:   /\d+/.test(s)
来源：http://ey.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ef.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ga.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://nq.muxihuayi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fe.muxihuayi.cn

[I02] 提取所有匹配
来源：http://yh.521024.cn

Py:   re.findall(r"\d+", s)
来源：http://ur.huanxung.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ur.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://pw.9csxet.cn

TS:   s.match(/\d+/g)
来源：http://wr.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cn.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wc.hahajie.cn

Ruby: s.scan(/\d+/)
来源：http://zv.9csxet.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rq.shxzskj.cn

[I03] 提取捕获分组
来源：http://wv.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cq.nszjky.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fl.colortex.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kj.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wy.chemitech.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://py.gzmigu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hv.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iy.jctech888.com.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gf.huixiangedu.cn

[I04] 正则替换
来源：http://jl.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fj.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ag.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qn.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zm.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://eb.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ul.wgjwhj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yc.yuexingan06.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://py.lnxyls.cn

[I05] 按正则拆分
来源：http://dg.shxzukj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://er.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ts.bookmarksfly.cn

JS:   s.split(/\s*,\s*/)
来源：http://yg.szsharing.cn

TS:   s.split(/\s*,\s*/)
来源：http://el.haigaiapp.cn

Java: s.split("\\s*,\\s*")
来源：http://sb.lnxyls.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://em.jianghongdianzi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fs.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://to.wgjwhj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vi.bjjhwx.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nx.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://du.bjjhwx.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yu.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xn.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wp.hahajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xu.szsharing.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nm.huixinmuqiang.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kg.bookmarksfly.cn

[I07] 忽略大小写与多行模式
来源：http://wr.newstarts.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ci.shxzskj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://iw.hahajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sd.bookmarksfly.cn

TS:   /error/gim
来源：http://qh.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cx.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://pw.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://cz.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sz.newstarts.cn

[I08] 贪婪与非贪婪匹配
来源：http://pk.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xz.szxytkj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zc.gzmigu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qz.chemitech.net.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://bi.shtwfgs.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tt.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://dg.huanxung.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ba.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bw.huixiangedu.cn

================================================================================
来源：http://dk.nicolike.cn

J. 日期与时间
来源：http://ph.huixiangedu.cn

================================================================================
来源：http://ev.colortex.cn

[J01] 获取当前时间
来源：http://sp.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://sv.asd995.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ui.szsharing.cn

JS:   new Date();  Date.now()
来源：http://vu.nszjky.cn

TS:   new Date();  Date.now()
来源：http://ga.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://if.huixiangedu.cn

Go:   time.Now()
来源：http://ah.shxzukj.cn

Ruby: Time.now
来源：http://zo.muxihuayi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sm.yuexingan06.cn

[J02] 格式化输出
来源：http://vo.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bn.shxzskj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bg.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wt.muxihuayi.cn

TS:   d.toISOString()
来源：http://yn.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cv.521024.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://iy.shxzskj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ml.muxihuayi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yo.panjiajie.cn

[J03] 字符串解析为日期
来源：http://vv.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://se.9csxet.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wi.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://ii.szxytkj.cn

TS:   new Date("2024-01-02")
来源：http://rp.shxzukj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://uu.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kn.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://rn.lnxyls.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://wk.521024.cn

[J04] 时间戳与日期互转
来源：http://ae.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://it.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xw.shtwfgs.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fa.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://me.panjiajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://gf.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qh.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sg.nszjky.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wm.muxihuayi.cn

[J05] 时间加减（加 7 天）
来源：http://zy.yuexingan06.cn

Py:   now + timedelta(days=7)
来源：http://wy.jianghongdianzi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nm.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://em.hahajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bp.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://fo.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hk.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://oc.nicolike.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lp.hahajie.cn

[J06] 计算两时间之差
来源：http://ke.shxzukj.cn

Py:   (end - start).total_seconds()
来源：http://sp.huixiangedu.cn

PHP:  $end->diff($start)->days;
来源：http://xs.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fp.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gk.nszjky.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lv.yuntaijiaju.cn

Go:   end.Sub(start).Hours()
来源：http://vc.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://mv.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://qk.yuexingan06.cn

[J07] 比较两个日期
来源：http://jz.shxzukj.cn

Py:   d1 < d2;  d1 == d2
来源：http://vm.shtwfgs.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qa.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bi.jianghongdianzi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kh.chemitech.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fw.panjiajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://fm.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://iw.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://ks.hahajie.cn

[J08] 提取年月日与星期
来源：http://nf.bjjhwx.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cu.nszjky.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rz.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qf.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vw.yuntaijiaju.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://du.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ps.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wd.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vq.nszjky.cn

[J09] 时区处理
来源：http://yn.newstarts.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tf.asd995.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cg.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://di.colortex.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gy.panjiajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kx.huixinmuqiang.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ju.huanxung.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zs.huixiangedu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fe.haigaiapp.cn

[J10] 取今天 / 本月第一天
来源：http://yd.colortex.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qt.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zh.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://pa.szxytkj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ee.wgjwhj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ui.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yx.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rs.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vr.gzmigu.cn

================================================================================
来源：http://lp.nszjky.cn

K. JSON 与序列化
来源：http://yp.bjjhwx.cn

================================================================================
来源：http://ge.newstarts.cn

[K01] 对象转 JSON 字符串
来源：http://sm.9csxet.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://kj.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dq.lnxyls.cn

JS:   JSON.stringify(obj)
来源：http://kv.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://du.lnxyls.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wd.nicolike.cn

Go:   json.Marshal(obj)
来源：http://yw.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uo.huixiangedu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://qv.muxihuayi.cn

[K02] JSON 字符串转对象
来源：http://mp.newstarts.cn

Py:   json.loads(s)
来源：http://pm.szsharing.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://nl.bookmarksfly.cn

JS:   JSON.parse(s)
来源：http://mj.wgjwhj.cn

TS:   JSON.parse(s)
来源：http://ey.nszjky.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rq.jctech888.com.cn

Go:   json.Unmarshal(data, &v)
来源：http://bv.9csxet.cn

Ruby: JSON.parse(s)
来源：http://zb.jianghongdianzi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ib.szsharing.cn

[K03] JSON 美化输出（带缩进）
来源：http://qq.haigaiapp.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://th.hahajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qf.huixinmuqiang.cn


<!-- 参考信息 -->