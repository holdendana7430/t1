代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sq.huixiangedu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uc.szsharing.cn

Java: enum Color { RED, GREEN }
来源：http://ij.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qz.panjiajie.cn

Ruby: Color = %i[red green].freeze
来源：http://tx.hahajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ws.lnxyls.cn

[G16] 对象转数组 / 字典
来源：http://bw.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://we.yuntaijiaju.cn

PHP:  get_object_vars($obj);
来源：http://ma.521024.cn

JS:   Object.entries(obj)
来源：http://ae.hahajie.cn

TS:   Object.entries(obj)
来源：http://rk.szsharing.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ri.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yz.gzmigu.cn

Ruby: obj.instance_variables
来源：http://jn.hnjuh.cn

C#:   // 用反射或 System.Text.Json
来源：http://jm.521024.cn

================================================================================
来源：http://fe.huanxung.cn

H. 异常与错误处理
来源：http://fs.bookmarksfly.cn

================================================================================
来源：http://ew.newstarts.cn

[H01] try / catch 基础
来源：http://iy.jctech888.com.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uu.shtwfgs.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zz.jctech888.com.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vk.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yk.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bi.huanxung.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uv.huanxung.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ns.colortex.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rj.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://fy.huixiangedu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fd.szxytkj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://iw.muxihuayi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vk.bookmarksfly.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fn.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://wq.szxytkj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vr.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yi.shxzukj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://kj.wgjwhj.cn

[H03] 主动抛出异常
来源：http://vb.panjiajie.cn

Py:   raise ValueError("错误信息")
来源：http://iz.shtwfgs.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://by.szsharing.cn

JS:   throw new Error("错误信息");
来源：http://qm.chemitech.net.cn

TS:   throw new Error("错误信息");
来源：http://lo.9csxet.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ah.jctech888.com.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zv.hahajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xz.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tf.haigaiapp.cn

[H04] 自定义异常类型
来源：http://ff.asd995.cn

Py:   class MyError(Exception): pass
来源：http://dp.newstarts.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dw.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://sk.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://jp.szsharing.cn

Java: class MyException extends RuntimeException {}
来源：http://cz.huixiangedu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rz.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://bs.muxihuayi.cn

C#:   class MyException : Exception {}
来源：http://gu.szsharing.cn

[H05] 捕获特定类型
来源：http://us.nicolike.cn

Py:   except ValueError as e:
来源：http://mm.muxihuayi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://jw.huixinmuqiang.cn

JS:   if (e instanceof TypeError) {}
来源：http://cu.yuexingan06.cn

TS:   if (e instanceof TypeError) {}
来源：http://wp.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://bq.huixinmuqiang.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rw.jctech888.com.cn

Ruby: rescue ArgumentError => e
来源：http://aq.jianghongdianzi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hj.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://wf.hahajie.cn

Py:   value = d.get("k") or default
来源：http://kh.wgjwhj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qn.bookmarksfly.cn

JS:   obj?.a?.b;  d ?? default
来源：http://gy.huanxung.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cx.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ow.szxytkj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mh.huixinmuqiang.cn

Ruby: d&.dig(:a, :b)
来源：http://wr.yuexingan06.cn

C#:   obj?.A?.B ?? default
来源：http://pz.yuntaijiaju.cn

[H07] 断言
来源：http://ui.gzmigu.cn

Py:   assert x > 0, "必须为正"
来源：http://of.jianghongdianzi.cn

PHP:  assert($x > 0);
来源：http://kw.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://lp.hnjuh.cn

TS:   console.assert(x > 0);
来源：http://vi.shxzukj.cn

Java: assert x > 0 : "必须为正";
来源：http://nv.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hv.szxytkj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://jz.colortex.cn

C#:   Debug.Assert(x > 0);
来源：http://dx.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://aw.colortex.cn

Py:   str(e);  traceback.format_exc()
来源：http://uw.colortex.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lb.bjjhwx.cn

JS:   e.message;  e.stack
来源：http://kb.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://iw.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rx.yuntaijiaju.cn

Go:   err.Error()
来源：http://cr.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://sc.muxihuayi.cn

C#:   e.Message;  e.StackTrace
来源：http://gh.gzmigu.cn

[H09] 带错误码的异常
来源：http://ec.lnxyls.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://bc.szsharing.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jp.jctech888.com.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jo.szxytkj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mc.wgjwhj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kf.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xg.bookmarksfly.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kl.shtwfgs.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rq.szxytkj.cn

[H10] 资源自动释放
来源：http://jo.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ts.huanxung.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sj.szxytkj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ox.huanxung.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://li.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hs.huixiangedu.cn

Go:   defer f.Close()
来源：http://ii.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zo.muxihuayi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qx.jianghongdianzi.cn

================================================================================
来源：http://oz.hahajie.cn

I. 正则表达式
来源：http://xe.hnjuh.cn

================================================================================
来源：http://mh.hahajie.cn

[I01] 判断是否匹配
来源：http://xt.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ca.gzmigu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ui.bookmarksfly.cn

JS:   /\d+/.test(s)
来源：http://kz.hahajie.cn

TS:   /\d+/.test(s)
来源：http://py.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yh.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ot.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://yk.panjiajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lq.asd995.cn

[I02] 提取所有匹配
来源：http://bw.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://ji.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ev.asd995.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zi.yuexingan06.cn

TS:   s.match(/\d+/g)
来源：http://ec.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lo.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bd.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://ze.haigaiapp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://uh.hahajie.cn

[I03] 提取捕获分组
来源：http://fx.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wh.yuexingan06.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xi.hahajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sg.huixiangedu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://dt.asd995.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dj.szsharing.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://of.chemitech.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yv.haigaiapp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lx.bjjhwx.cn

[I04] 正则替换
来源：http://ag.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dk.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dv.bookmarksfly.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ml.shtwfgs.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pn.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://xp.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vo.szxytkj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ve.chemitech.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ms.szxytkj.cn

[I05] 按正则拆分
来源：http://oz.haigaiapp.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sj.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xb.bookmarksfly.cn

JS:   s.split(/\s*,\s*/)
来源：http://wc.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://gj.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://og.bookmarksfly.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zq.asd995.cn

Ruby: s.split(/\s*,\s*/)
来源：http://fc.jctech888.com.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bq.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zn.asd995.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yi.muxihuayi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sy.521024.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ij.asd995.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nh.gzmigu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xg.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yb.wgjwhj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://tr.huixiangedu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fb.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://ce.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nl.jianghongdianzi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ax.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://bv.szxytkj.cn

TS:   /error/gim
来源：http://zh.shxzskj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zh.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xy.colortex.cn

Ruby: s.scan(/error/i)
来源：http://px.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vk.szsharing.cn

[I08] 贪婪与非贪婪匹配
来源：http://fi.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gq.newstarts.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ug.szxytkj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://us.nicolike.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://js.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://jm.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bn.521024.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://di.chemitech.net.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yc.szxytkj.cn

================================================================================
来源：http://na.huanxung.cn

J. 日期与时间
来源：http://do.9csxet.cn

================================================================================
来源：http://he.jianghongdianzi.cn

[J01] 获取当前时间
来源：http://kh.huixiangedu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ne.wgjwhj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pg.shtwfgs.cn

JS:   new Date();  Date.now()
来源：http://ob.9csxet.cn

TS:   new Date();  Date.now()
来源：http://ss.colortex.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://sd.huixiangedu.cn

Go:   time.Now()
来源：http://hr.gzmigu.cn

Ruby: Time.now
来源：http://ly.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nv.shxzskj.cn

[J02] 格式化输出
来源：http://fj.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://um.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ex.jianghongdianzi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sy.bookmarksfly.cn

TS:   d.toISOString()
来源：http://uh.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://le.szsharing.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rn.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yl.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hf.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://qi.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fs.newstarts.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qr.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://sz.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://ie.newstarts.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bv.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://at.asd995.cn

Ruby: Date.parse("2024-01-02")
来源：http://nx.521024.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ib.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://ft.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://iv.hahajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yo.lnxyls.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://uu.bjjhwx.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tu.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://lm.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://vg.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sn.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ow.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://hg.huixinmuqiang.cn

Py:   now + timedelta(days=7)
来源：http://nz.yuntaijiaju.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ew.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://va.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://le.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://qk.muxihuayi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zg.lnxyls.cn

Ruby: Time.now + 7 * 86400
来源：http://zx.nicolike.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mj.newstarts.cn

[J06] 计算两时间之差
来源：http://px.newstarts.cn

Py:   (end - start).total_seconds()
来源：http://od.huixiangedu.cn

PHP:  $end->diff($start)->days;
来源：http://zz.bookmarksfly.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yn.wgjwhj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://pj.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ao.gzmigu.cn

Go:   end.Sub(start).Hours()
来源：http://da.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://pj.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://cp.huanxung.cn

[J07] 比较两个日期
来源：http://vd.huixinmuqiang.cn

Py:   d1 < d2;  d1 == d2
来源：http://ph.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tt.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qe.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://rb.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gg.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nv.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qi.haigaiapp.cn

C#:   d1 < d2;  d1 == d2
来源：http://ro.nicolike.cn

[J08] 提取年月日与星期
来源：http://de.hahajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vd.jctech888.com.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xn.gzmigu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cn.bookmarksfly.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ni.jianghongdianzi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hg.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wb.wgjwhj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qq.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mz.nicolike.cn

[J09] 时区处理
来源：http://oo.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ou.shxzskj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://df.yuexingan06.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://li.nszjky.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jj.jianghongdianzi.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ul.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ra.panjiajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xk.jctech888.com.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xx.gzmigu.cn

[J10] 取今天 / 本月第一天
来源：http://cx.hahajie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xl.hahajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kd.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sh.chemitech.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ua.bjjhwx.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ex.shxzukj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xp.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cx.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hs.nicolike.cn

================================================================================
来源：http://kw.gzmigu.cn

K. JSON 与序列化
来源：http://cb.huanxung.cn

================================================================================
来源：http://dq.colortex.cn

[K01] 对象转 JSON 字符串
来源：http://um.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zh.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wv.lnxyls.cn

JS:   JSON.stringify(obj)
来源：http://me.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://hs.chemitech.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ee.hahajie.cn

Go:   json.Marshal(obj)
来源：http://bf.nicolike.cn

Ruby: obj.to_json                                     // require "json"
来源：http://au.shxzskj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cg.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://ej.haigaiapp.cn

Py:   json.loads(s)
来源：http://fv.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hi.huixiangedu.cn

JS:   JSON.parse(s)
来源：http://hh.9csxet.cn

TS:   JSON.parse(s)
来源：http://md.huixiangedu.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ed.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://bg.colortex.cn

Ruby: JSON.parse(s)
来源：http://jx.huixinmuqiang.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rg.szxytkj.cn

[K03] JSON 美化输出（带缩进）
来源：http://be.huixinmuqiang.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dn.colortex.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wd.huanxung.cn


<!-- 参考信息 -->