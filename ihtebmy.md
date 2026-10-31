代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hs.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zv.shxzukj.cn

Java: enum Color { RED, GREEN }
来源：http://pk.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://oh.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://gw.yuexingan06.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://it.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://hx.bjjhwx.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://rq.muxihuayi.cn

PHP:  get_object_vars($obj);
来源：http://tg.colortex.cn

JS:   Object.entries(obj)
来源：http://jq.hahajie.cn

TS:   Object.entries(obj)
来源：http://bx.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ep.jctech888.com.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://du.asd995.cn

Ruby: obj.instance_variables
来源：http://wt.yuntaijiaju.cn

C#:   // 用反射或 System.Text.Json
来源：http://wh.shxzskj.cn

================================================================================
来源：http://ge.bjjhwx.cn

H. 异常与错误处理
来源：http://nr.newstarts.cn

================================================================================
来源：http://jb.gzmigu.cn

[H01] try / catch 基础
来源：http://jy.hahajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://cp.muxihuayi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fi.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gz.panjiajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yc.shxzskj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://py.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ey.yuexingan06.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mo.huixinmuqiang.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bq.hahajie.cn

[H02] finally / ensure 收尾
来源：http://qd.gzmigu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sw.yuntaijiaju.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bb.yuntaijiaju.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yb.chemitech.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://km.9csxet.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yr.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://am.shxzukj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ek.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rg.shxzskj.cn

[H03] 主动抛出异常
来源：http://uu.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://tu.bookmarksfly.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://fw.haigaiapp.cn

JS:   throw new Error("错误信息");
来源：http://vf.jctech888.com.cn

TS:   throw new Error("错误信息");
来源：http://pk.nszjky.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://sf.asd995.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ds.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wv.bjjhwx.cn

C#:   throw new ArgumentException("错误信息");
来源：http://sl.huixiangedu.cn

[H04] 自定义异常类型
来源：http://ej.hnjuh.cn

Py:   class MyError(Exception): pass
来源：http://yy.hahajie.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gu.521024.cn

JS:   class MyError extends Error {}
来源：http://wx.colortex.cn

TS:   class MyError extends Error {}
来源：http://ma.hnjuh.cn

Java: class MyException extends RuntimeException {}
来源：http://jl.jianghongdianzi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ct.jianghongdianzi.cn

Ruby: class MyError < StandardError; end
来源：http://fq.haigaiapp.cn

C#:   class MyException : Exception {}
来源：http://tr.gzmigu.cn

[H05] 捕获特定类型
来源：http://ap.nicolike.cn

Py:   except ValueError as e:
来源：http://ts.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ws.nicolike.cn

JS:   if (e instanceof TypeError) {}
来源：http://sc.chemitech.net.cn

TS:   if (e instanceof TypeError) {}
来源：http://yn.szxytkj.cn

Java: catch (IOException | SQLException e) {}
来源：http://sf.bjjhwx.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xd.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://ml.hahajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hp.newstarts.cn

[H06] 可选值 / 空值安全访问
来源：http://kx.yuntaijiaju.cn

Py:   value = d.get("k") or default
来源：http://rc.nszjky.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sj.chemitech.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ju.asd995.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sc.newstarts.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://zk.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lj.muxihuayi.cn

Ruby: d&.dig(:a, :b)
来源：http://fa.shxzskj.cn

C#:   obj?.A?.B ?? default
来源：http://yk.panjiajie.cn

[H07] 断言
来源：http://am.yuexingan06.cn

Py:   assert x > 0, "必须为正"
来源：http://si.gzmigu.cn

PHP:  assert($x > 0);
来源：http://az.huanxung.cn

JS:   console.assert(x > 0);
来源：http://bh.nszjky.cn

TS:   console.assert(x > 0);
来源：http://hh.shxzukj.cn

Java: assert x > 0 : "必须为正";
来源：http://vn.szxytkj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tn.colortex.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ud.jianghongdianzi.cn

C#:   Debug.Assert(x > 0);
来源：http://mo.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://ob.bjjhwx.cn

Py:   str(e);  traceback.format_exc()
来源：http://nc.huanxung.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://os.szsharing.cn

JS:   e.message;  e.stack
来源：http://pa.chemitech.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gd.colortex.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://oe.newstarts.cn

Go:   err.Error()
来源：http://nv.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://qz.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://or.haigaiapp.cn

[H09] 带错误码的异常
来源：http://gf.jctech888.com.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://yj.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lc.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://al.huixiangedu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nr.yuntaijiaju.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yx.panjiajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sq.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hn.huanxung.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cf.shtwfgs.cn

[H10] 资源自动释放
来源：http://qi.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zp.nszjky.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sa.yuexingan06.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://oi.jianghongdianzi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pv.shxzukj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://lm.huixiangedu.cn

Go:   defer f.Close()
来源：http://kn.hnjuh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ds.9csxet.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ki.jianghongdianzi.cn

================================================================================
来源：http://cg.huixiangedu.cn

I. 正则表达式
来源：http://gi.huixiangedu.cn

================================================================================
来源：http://rf.hahajie.cn

[I01] 判断是否匹配
来源：http://nk.jctech888.com.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nx.shxzukj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nd.gzmigu.cn

JS:   /\d+/.test(s)
来源：http://zy.jianghongdianzi.cn

TS:   /\d+/.test(s)
来源：http://sr.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://at.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pa.9csxet.cn

Ruby: s.match?(/\d+/)
来源：http://ke.huixiangedu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fa.huanxung.cn

[I02] 提取所有匹配
来源：http://wf.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://ze.lnxyls.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qj.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wf.hnjuh.cn

TS:   s.match(/\d+/g)
来源：http://nk.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wv.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ns.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://tf.muxihuayi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ml.yuntaijiaju.cn

[I03] 提取捕获分组
来源：http://sk.panjiajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xm.hnjuh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://zu.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ca.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://lh.yuntaijiaju.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ky.muxihuayi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://va.shtwfgs.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tk.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://aw.asd995.cn

[I04] 正则替换
来源：http://gb.muxihuayi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qx.huixinmuqiang.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wp.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cl.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yr.panjiajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ko.yuexingan06.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tw.yuntaijiaju.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rm.chemitech.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zy.huixiangedu.cn

[I05] 按正则拆分
来源：http://at.shxzukj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ow.haigaiapp.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hk.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://cl.9csxet.cn

TS:   s.split(/\s*,\s*/)
来源：http://tj.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://io.hnjuh.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hx.huixinmuqiang.cn

Ruby: s.split(/\s*,\s*/)
来源：http://at.bjjhwx.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fn.shxzukj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mu.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://st.yuexingan06.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fx.muxihuayi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lp.wgjwhj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xo.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mf.521024.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gq.huanxung.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ut.bjjhwx.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://rm.yuntaijiaju.cn

[I07] 忽略大小写与多行模式
来源：http://lq.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ix.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ai.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://it.haigaiapp.cn

TS:   /error/gim
来源：http://ve.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dp.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wa.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://oe.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://um.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://qk.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://oa.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mx.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yh.shxzskj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tn.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wg.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jf.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ek.gzmigu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nt.szsharing.cn

================================================================================
来源：http://if.asd995.cn

J. 日期与时间
来源：http://li.9csxet.cn

================================================================================
来源：http://yc.bookmarksfly.cn

[J01] 获取当前时间
来源：http://qf.9csxet.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yo.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://tt.wgjwhj.cn

JS:   new Date();  Date.now()
来源：http://rx.shtwfgs.cn

TS:   new Date();  Date.now()
来源：http://xo.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mq.nszjky.cn

Go:   time.Now()
来源：http://ei.bookmarksfly.cn

Ruby: Time.now
来源：http://lo.muxihuayi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rl.newstarts.cn

[J02] 格式化输出
来源：http://nn.gzmigu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ll.huixinmuqiang.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ve.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yk.szsharing.cn

TS:   d.toISOString()
来源：http://ay.jianghongdianzi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rx.lnxyls.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ta.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gk.szxytkj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ue.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://ti.nszjky.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vi.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qi.nszjky.cn

JS:   new Date("2024-01-02")
来源：http://df.nicolike.cn

TS:   new Date("2024-01-02")
来源：http://ri.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gk.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ei.yuntaijiaju.cn

Ruby: Date.parse("2024-01-02")
来源：http://br.yuexingan06.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ig.newstarts.cn

[J04] 时间戳与日期互转
来源：http://pv.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ta.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cs.huixinmuqiang.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ku.bjjhwx.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://vl.haigaiapp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bd.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qt.szxytkj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ti.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://qc.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://wm.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://xm.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nz.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xd.jianghongdianzi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qi.wgjwhj.cn

Java: LocalDate.now().plusDays(7)
来源：http://lf.bookmarksfly.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jx.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://zw.shxzskj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cs.huanxung.cn

[J06] 计算两时间之差
来源：http://xy.bookmarksfly.cn

Py:   (end - start).total_seconds()
来源：http://mc.lnxyls.cn

PHP:  $end->diff($start)->days;
来源：http://ug.521024.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://np.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://qp.shxzskj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cg.gzmigu.cn

Go:   end.Sub(start).Hours()
来源：http://tk.muxihuayi.cn

Ruby: end - start                 # 返回秒数
来源：http://de.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://it.wgjwhj.cn

[J07] 比较两个日期
来源：http://rv.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://sw.colortex.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ms.jianghongdianzi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://if.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yf.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qw.nicolike.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ta.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vl.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://cr.shtwfgs.cn

[J08] 提取年月日与星期
来源：http://dm.colortex.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hk.nszjky.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ly.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qf.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ws.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://re.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pw.panjiajie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wb.nszjky.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hl.yuntaijiaju.cn

[J09] 时区处理
来源：http://ne.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gf.shxzskj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vk.shtwfgs.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sy.jctech888.com.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://de.lnxyls.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kw.jctech888.com.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lz.huixinmuqiang.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jt.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://po.chemitech.net.cn

[J10] 取今天 / 本月第一天
来源：http://gm.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nh.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xr.shxzskj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ga.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tn.huanxung.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uc.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wg.huixinmuqiang.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sp.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yi.shtwfgs.cn

================================================================================
来源：http://ia.yuntaijiaju.cn

K. JSON 与序列化
来源：http://ag.shxzskj.cn

================================================================================
来源：http://sn.panjiajie.cn

[K01] 对象转 JSON 字符串
来源：http://db.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bq.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ge.9csxet.cn

JS:   JSON.stringify(obj)
来源：http://fl.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://hx.bjjhwx.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ff.nicolike.cn

Go:   json.Marshal(obj)
来源：http://gj.colortex.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ve.shxzskj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bz.szsharing.cn

[K02] JSON 字符串转对象
来源：http://tg.jianghongdianzi.cn

Py:   json.loads(s)
来源：http://iq.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qh.yuntaijiaju.cn

JS:   JSON.parse(s)
来源：http://wi.huixinmuqiang.cn

TS:   JSON.parse(s)
来源：http://dk.yuexingan06.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jw.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://xb.yuntaijiaju.cn

Ruby: JSON.parse(s)
来源：http://ap.szxytkj.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://st.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://zw.huixiangedu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ib.panjiajie.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ui.huixinmuqiang.cn


<!-- 参考信息 -->