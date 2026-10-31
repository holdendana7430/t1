代发 wailian999

PHP:  get_object_vars($obj);
来源：http://rx.nicolike.cn

JS:   Object.entries(obj)
来源：http://cj.huixiangedu.cn

TS:   Object.entries(obj)
来源：http://ss.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ok.bjjhwx.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hh.panjiajie.cn

Ruby: obj.instance_variables
来源：http://dt.szxytkj.cn

C#:   // 用反射或 System.Text.Json
来源：http://pb.chemitech.net.cn

================================================================================
来源：http://jj.jianghongdianzi.cn

H. 异常与错误处理
来源：http://nj.jianghongdianzi.cn

================================================================================
来源：http://fo.yuntaijiaju.cn

[H01] try / catch 基础
来源：http://sf.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mo.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://iu.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vo.bookmarksfly.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ia.shtwfgs.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yx.shxzukj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nv.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yl.wgjwhj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hu.nszjky.cn

[H02] finally / ensure 收尾
来源：http://bq.jctech888.com.cn

Py:   try: f()⏎finally: cleanup()
来源：http://kk.bjjhwx.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yr.521024.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cz.shxzukj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nv.nszjky.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yj.chemitech.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rk.shxzskj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vz.yuntaijiaju.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://df.chemitech.net.cn

[H03] 主动抛出异常
来源：http://jq.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://fi.hnjuh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yd.yuntaijiaju.cn

JS:   throw new Error("错误信息");
来源：http://xc.wgjwhj.cn

TS:   throw new Error("错误信息");
来源：http://bj.nszjky.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ox.haigaiapp.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dy.chemitech.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zl.521024.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ce.nszjky.cn

[H04] 自定义异常类型
来源：http://yy.szsharing.cn

Py:   class MyError(Exception): pass
来源：http://fl.jianghongdianzi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bj.jctech888.com.cn

JS:   class MyError extends Error {}
来源：http://vo.yuexingan06.cn

TS:   class MyError extends Error {}
来源：http://ym.nszjky.cn

Java: class MyException extends RuntimeException {}
来源：http://ot.shxzukj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://dl.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://pg.shxzskj.cn

C#:   class MyException : Exception {}
来源：http://ca.shxzukj.cn

[H05] 捕获特定类型
来源：http://ba.asd995.cn

Py:   except ValueError as e:
来源：http://ia.newstarts.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://uj.panjiajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://hq.yuntaijiaju.cn

TS:   if (e instanceof TypeError) {}
来源：http://po.9csxet.cn

Java: catch (IOException | SQLException e) {}
来源：http://dw.yuntaijiaju.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bn.lnxyls.cn

Ruby: rescue ArgumentError => e
来源：http://il.shxzskj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ob.huanxung.cn

[H06] 可选值 / 空值安全访问
来源：http://xr.huixiangedu.cn

Py:   value = d.get("k") or default
来源：http://qq.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://zh.nszjky.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hr.nicolike.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ws.hahajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://eb.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://md.bookmarksfly.cn

Ruby: d&.dig(:a, :b)
来源：http://zp.lnxyls.cn

C#:   obj?.A?.B ?? default
来源：http://om.521024.cn

[H07] 断言
来源：http://yz.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://dw.szxytkj.cn

PHP:  assert($x > 0);
来源：http://sp.wgjwhj.cn

JS:   console.assert(x > 0);
来源：http://ei.gzmigu.cn

TS:   console.assert(x > 0);
来源：http://xm.huixiangedu.cn

Java: assert x > 0 : "必须为正";
来源：http://ts.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zq.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zf.colortex.cn

C#:   Debug.Assert(x > 0);
来源：http://ry.nicolike.cn

[H08] 获取错误信息与堆栈
来源：http://aa.jianghongdianzi.cn

Py:   str(e);  traceback.format_exc()
来源：http://pj.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sp.haigaiapp.cn

JS:   e.message;  e.stack
来源：http://lx.muxihuayi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qn.szxytkj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ze.shtwfgs.cn

Go:   err.Error()
来源：http://wn.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://hm.asd995.cn

C#:   e.Message;  e.StackTrace
来源：http://rj.szsharing.cn

[H09] 带错误码的异常
来源：http://ee.huixinmuqiang.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dr.colortex.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://dr.jctech888.com.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vr.yuexingan06.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://bf.yuntaijiaju.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ib.bookmarksfly.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bz.hahajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ap.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://dr.jctech888.com.cn

[H10] 资源自动释放
来源：http://qw.shxzukj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xe.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ij.muxihuayi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pr.hnjuh.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oe.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mb.bjjhwx.cn

Go:   defer f.Close()
来源：http://sz.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sl.nszjky.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wk.szsharing.cn

================================================================================
来源：http://am.huanxung.cn

I. 正则表达式
来源：http://ro.panjiajie.cn

================================================================================
来源：http://ov.gzmigu.cn

[I01] 判断是否匹配
来源：http://tf.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kt.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tn.yuexingan06.cn

JS:   /\d+/.test(s)
来源：http://sq.shxzukj.cn

TS:   /\d+/.test(s)
来源：http://qa.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nh.asd995.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ww.yuexingan06.cn

Ruby: s.match?(/\d+/)
来源：http://nk.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://se.bjjhwx.cn

[I02] 提取所有匹配
来源：http://oc.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://ck.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jq.gzmigu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hj.huixiangedu.cn

TS:   s.match(/\d+/g)
来源：http://up.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jp.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ea.bjjhwx.cn

Ruby: s.scan(/\d+/)
来源：http://gr.szxytkj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ob.bookmarksfly.cn

[I03] 提取捕获分组
来源：http://ux.panjiajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fq.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wm.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mp.shxzskj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wv.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dz.colortex.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nd.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dc.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yv.szxytkj.cn

[I04] 正则替换
来源：http://fk.yuntaijiaju.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fp.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://js.szsharing.cn

JS:   s.replace(/\d+/g, "#")
来源：http://od.huixinmuqiang.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xu.muxihuayi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ha.huanxung.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://sp.shxzukj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rr.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lc.jctech888.com.cn

[I05] 按正则拆分
来源：http://fg.szxytkj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ku.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qa.huanxung.cn

JS:   s.split(/\s*,\s*/)
来源：http://uj.yuexingan06.cn

TS:   s.split(/\s*,\s*/)
来源：http://np.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://hj.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bs.yuexingan06.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dx.jianghongdianzi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rf.hahajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://co.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ju.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kq.lnxyls.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yo.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ea.chemitech.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://lv.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://bd.jianghongdianzi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uo.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rs.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://kb.newstarts.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://kx.huixiangedu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cy.wgjwhj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xv.jctech888.com.cn

TS:   /error/gim
来源：http://yh.bookmarksfly.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://py.yuntaijiaju.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rx.shxzskj.cn

Ruby: s.scan(/error/i)
来源：http://bo.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oq.shtwfgs.cn

[I08] 贪婪与非贪婪匹配
来源：http://av.chemitech.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yf.muxihuayi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cz.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uy.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://il.hahajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://gu.hahajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wq.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bv.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jw.yuntaijiaju.cn

================================================================================
来源：http://jw.yuexingan06.cn

J. 日期与时间
来源：http://vi.lnxyls.cn

================================================================================
来源：http://hk.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://cl.9csxet.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://zi.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pc.huanxung.cn

JS:   new Date();  Date.now()
来源：http://vo.shtwfgs.cn

TS:   new Date();  Date.now()
来源：http://rg.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mf.bookmarksfly.cn

Go:   time.Now()
来源：http://ce.chemitech.net.cn

Ruby: Time.now
来源：http://cq.jianghongdianzi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zy.panjiajie.cn

[J02] 格式化输出
来源：http://oi.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nu.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yp.newstarts.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qb.yuexingan06.cn

TS:   d.toISOString()
来源：http://ay.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qv.colortex.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pn.shtwfgs.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rq.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://as.haigaiapp.cn

[J03] 字符串解析为日期
来源：http://fh.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eh.huixinmuqiang.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ee.chemitech.net.cn

JS:   new Date("2024-01-02")
来源：http://tj.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://xv.shxzukj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hx.hahajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wf.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://rf.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jd.newstarts.cn

[J04] 时间戳与日期互转
来源：http://ct.shxzukj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://er.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ze.szsharing.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mq.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://bq.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zr.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mw.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://aj.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mb.shxzukj.cn

[J05] 时间加减（加 7 天）
来源：http://oi.gzmigu.cn

Py:   now + timedelta(days=7)
来源：http://ut.hahajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wr.hnjuh.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ln.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mg.bookmarksfly.cn

Java: LocalDate.now().plusDays(7)
来源：http://hh.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gf.wgjwhj.cn

Ruby: Time.now + 7 * 86400
来源：http://le.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://wa.szxytkj.cn

[J06] 计算两时间之差
来源：http://mp.521024.cn

Py:   (end - start).total_seconds()
来源：http://bj.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://ez.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rm.521024.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xz.shtwfgs.cn

Java: Duration.between(start, end).toSeconds()
来源：http://in.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://kn.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://tu.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://yg.haigaiapp.cn

[J07] 比较两个日期
来源：http://xx.panjiajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://cn.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nf.bjjhwx.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gu.huanxung.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nm.bjjhwx.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ub.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xt.shxzskj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://eo.shxzskj.cn

C#:   d1 < d2;  d1 == d2
来源：http://mx.yuexingan06.cn

[J08] 提取年月日与星期
来源：http://it.huixiangedu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ex.wgjwhj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://no.muxihuayi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vd.newstarts.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vo.521024.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://oa.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yh.521024.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gb.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dm.lnxyls.cn

[J09] 时区处理
来源：http://dh.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://li.yuntaijiaju.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ou.yuexingan06.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kg.nszjky.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zg.colortex.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vk.hnjuh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ft.hahajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hu.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mp.gzmigu.cn

[J10] 取今天 / 本月第一天
来源：http://qo.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hw.panjiajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://am.huixinmuqiang.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lu.gzmigu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kj.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ig.yuexingan06.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jy.newstarts.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lr.huixiangedu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://vs.colortex.cn

================================================================================
来源：http://zv.szxytkj.cn

K. JSON 与序列化
来源：http://ea.newstarts.cn

================================================================================
来源：http://oi.shxzukj.cn

[K01] 对象转 JSON 字符串
来源：http://ly.shtwfgs.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bt.hahajie.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fs.bjjhwx.cn

JS:   JSON.stringify(obj)
来源：http://wr.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://rk.bookmarksfly.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bg.huixiangedu.cn

Go:   json.Marshal(obj)
来源：http://bo.szsharing.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ct.nszjky.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fr.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://ox.9csxet.cn

Py:   json.loads(s)
来源：http://yt.szxytkj.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ut.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://zu.jianghongdianzi.cn

TS:   JSON.parse(s)
来源：http://bm.gzmigu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nt.yuntaijiaju.cn

Go:   json.Unmarshal(data, &v)
来源：http://cd.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://tt.yuexingan06.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://gm.newstarts.cn

[K03] JSON 美化输出（带缩进）
来源：http://vs.yuexingan06.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://or.yuexingan06.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zz.jctech888.com.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yi.shtwfgs.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tm.huixiangedu.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ru.panjiajie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://js.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gz.colortex.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://nt.huixinmuqiang.cn

[K04] 读取 JSON 文件
来源：http://xy.hahajie.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rx.bjjhwx.cn


<!-- 参考信息 -->