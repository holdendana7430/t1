代发 wailian999

C#:   record User(string Name, int Age);
来源：http://vm.bjjhwx.cn

[G15] 枚举
来源：http://xr.newstarts.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ur.gzmigu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gn.chemitech.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tw.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://te.shxzskj.cn

Java: enum Color { RED, GREEN }
来源：http://qf.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://it.panjiajie.cn

Ruby: Color = %i[red green].freeze
来源：http://te.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://iq.colortex.cn

[G16] 对象转数组 / 字典
来源：http://wc.colortex.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cr.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://ey.shtwfgs.cn

JS:   Object.entries(obj)
来源：http://ec.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://da.huixinmuqiang.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xm.bjjhwx.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dt.shtwfgs.cn

Ruby: obj.instance_variables
来源：http://se.lnxyls.cn

C#:   // 用反射或 System.Text.Json
来源：http://pk.muxihuayi.cn

================================================================================
来源：http://ik.yuntaijiaju.cn

H. 异常与错误处理
来源：http://zj.hnjuh.cn

================================================================================
来源：http://ht.jianghongdianzi.cn

[H01] try / catch 基础
来源：http://ep.newstarts.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bl.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lv.hahajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xb.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://oz.muxihuayi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sk.shxzskj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://we.shtwfgs.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qv.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://if.huixinmuqiang.cn

[H02] finally / ensure 收尾
来源：http://pt.bjjhwx.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xy.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sd.asd995.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nq.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fj.yuexingan06.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yg.colortex.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ku.wgjwhj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ld.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ok.haigaiapp.cn

[H03] 主动抛出异常
来源：http://ft.chemitech.net.cn

Py:   raise ValueError("错误信息")
来源：http://cw.9csxet.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vx.yuntaijiaju.cn

JS:   throw new Error("错误信息");
来源：http://xa.muxihuayi.cn

TS:   throw new Error("错误信息");
来源：http://vt.newstarts.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mo.huixinmuqiang.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bd.bjjhwx.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ik.huixiangedu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wf.shtwfgs.cn

[H04] 自定义异常类型
来源：http://sl.muxihuayi.cn

Py:   class MyError(Exception): pass
来源：http://vj.asd995.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mo.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://az.panjiajie.cn

TS:   class MyError extends Error {}
来源：http://ib.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://lj.muxihuayi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ly.lnxyls.cn

Ruby: class MyError < StandardError; end
来源：http://fh.yuntaijiaju.cn

C#:   class MyException : Exception {}
来源：http://wn.lnxyls.cn

[H05] 捕获特定类型
来源：http://ue.lnxyls.cn

Py:   except ValueError as e:
来源：http://qm.hahajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xi.asd995.cn

JS:   if (e instanceof TypeError) {}
来源：http://vd.bjjhwx.cn

TS:   if (e instanceof TypeError) {}
来源：http://pz.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://mm.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sz.lnxyls.cn

Ruby: rescue ArgumentError => e
来源：http://kv.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jf.bookmarksfly.cn

[H06] 可选值 / 空值安全访问
来源：http://af.newstarts.cn

Py:   value = d.get("k") or default
来源：http://kp.bookmarksfly.cn

PHP:  $v = $d["k"] ?? null;
来源：http://my.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wn.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cr.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ux.szsharing.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://iy.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://nu.lnxyls.cn

C#:   obj?.A?.B ?? default
来源：http://db.panjiajie.cn

[H07] 断言
来源：http://tj.521024.cn

Py:   assert x > 0, "必须为正"
来源：http://bq.wgjwhj.cn

PHP:  assert($x > 0);
来源：http://fu.nszjky.cn

JS:   console.assert(x > 0);
来源：http://mz.nszjky.cn

TS:   console.assert(x > 0);
来源：http://cg.huixinmuqiang.cn

Java: assert x > 0 : "必须为正";
来源：http://bx.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://iq.yuntaijiaju.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ko.9csxet.cn

C#:   Debug.Assert(x > 0);
来源：http://fz.shxzskj.cn

[H08] 获取错误信息与堆栈
来源：http://la.shxzukj.cn

Py:   str(e);  traceback.format_exc()
来源：http://ys.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rp.nszjky.cn

JS:   e.message;  e.stack
来源：http://kh.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qv.chemitech.net.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://em.shxzskj.cn

Go:   err.Error()
来源：http://iz.bookmarksfly.cn

Ruby: e.message;  e.backtrace
来源：http://ml.panjiajie.cn

C#:   e.Message;  e.StackTrace
来源：http://qt.yuexingan06.cn

[H09] 带错误码的异常
来源：http://bk.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://vg.gzmigu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wk.muxihuayi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zi.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qo.huanxung.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ol.shtwfgs.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://an.huanxung.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xz.huixinmuqiang.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ak.haigaiapp.cn

[H10] 资源自动释放
来源：http://fp.wgjwhj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cz.lnxyls.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gp.wgjwhj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bf.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ha.9csxet.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sx.huixiangedu.cn

Go:   defer f.Close()
来源：http://af.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rp.huixinmuqiang.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ls.huixiangedu.cn

================================================================================
来源：http://hb.hahajie.cn

I. 正则表达式
来源：http://jo.shtwfgs.cn

================================================================================
来源：http://wa.gzmigu.cn

[I01] 判断是否匹配
来源：http://ps.yuntaijiaju.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tr.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tv.yuexingan06.cn

JS:   /\d+/.test(s)
来源：http://es.shxzukj.cn

TS:   /\d+/.test(s)
来源：http://vk.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pq.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://lt.nszjky.cn

Ruby: s.match?(/\d+/)
来源：http://ff.bjjhwx.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cm.bookmarksfly.cn

[I02] 提取所有匹配
来源：http://ha.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://ct.yuntaijiaju.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ju.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://of.jctech888.com.cn

TS:   s.match(/\d+/g)
来源：http://oh.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ov.nicolike.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xp.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://ap.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ap.bjjhwx.cn

[I03] 提取捕获分组
来源：http://jr.lnxyls.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://lj.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vp.shxzskj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nl.bjjhwx.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pj.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zt.colortex.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xn.hnjuh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://or.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oh.newstarts.cn

[I04] 正则替换
来源：http://zn.shxzskj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ck.jianghongdianzi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://et.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://dn.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pm.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nn.huixiangedu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://pd.shxzskj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://co.shtwfgs.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wl.newstarts.cn

[I05] 按正则拆分
来源：http://hn.colortex.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sm.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ah.nicolike.cn

JS:   s.split(/\s*,\s*/)
来源：http://tr.szsharing.cn

TS:   s.split(/\s*,\s*/)
来源：http://ar.szxytkj.cn

Java: s.split("\\s*,\\s*")
来源：http://vg.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://tp.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yg.newstarts.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://em.szxytkj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://va.shtwfgs.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://md.gzmigu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pa.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://em.colortex.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.9csxet.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zt.nicolike.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gq.shxzskj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ih.hnjuh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ca.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://lh.huixiangedu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://iv.asd995.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hd.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cf.panjiajie.cn

TS:   /error/gim
来源：http://lu.hnjuh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ny.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jl.gzmigu.cn

Ruby: s.scan(/error/i)
来源：http://ld.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ht.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://uc.lnxyls.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ka.huixiangedu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vz.shtwfgs.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wy.shxzskj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://je.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dj.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zj.haigaiapp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oh.huanxung.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ko.szxytkj.cn

================================================================================
来源：http://ck.521024.cn

J. 日期与时间
来源：http://dt.hnjuh.cn

================================================================================
来源：http://gp.lnxyls.cn

[J01] 获取当前时间
来源：http://ma.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ej.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://en.bookmarksfly.cn

JS:   new Date();  Date.now()
来源：http://ad.jctech888.com.cn

TS:   new Date();  Date.now()
来源：http://je.shxzukj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://zx.szxytkj.cn

Go:   time.Now()
来源：http://lf.haigaiapp.cn

Ruby: Time.now
来源：http://ef.chemitech.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dd.nicolike.cn

[J02] 格式化输出
来源：http://ea.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pv.lnxyls.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qk.hnjuh.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zw.hnjuh.cn

TS:   d.toISOString()
来源：http://zm.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://iz.huixiangedu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zl.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ms.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vb.bookmarksfly.cn

[J03] 字符串解析为日期
来源：http://ik.nicolike.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://th.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yj.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://sk.huanxung.cn

TS:   new Date("2024-01-02")
来源：http://dr.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://sy.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zw.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://qc.szsharing.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gk.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://cp.jctech888.com.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pm.521024.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://us.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ia.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nt.bookmarksfly.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://op.521024.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://jd.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://if.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mk.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://il.bjjhwx.cn

Py:   now + timedelta(days=7)
来源：http://ph.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pu.colortex.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vf.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qh.yuntaijiaju.cn

Java: LocalDate.now().plusDays(7)
来源：http://ty.521024.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cl.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://ch.nicolike.cn

C#:   DateTime.Now.AddDays(7)
来源：http://op.nszjky.cn

[J06] 计算两时间之差
来源：http://fe.bookmarksfly.cn

Py:   (end - start).total_seconds()
来源：http://wo.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://fl.bjjhwx.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kj.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://es.521024.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rf.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://wr.gzmigu.cn

Ruby: end - start                 # 返回秒数
来源：http://ui.colortex.cn

C#:   (end - start).TotalSeconds
来源：http://el.szxytkj.cn

[J07] 比较两个日期
来源：http://sy.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://un.szsharing.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://qm.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://bb.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cs.yuntaijiaju.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://un.shtwfgs.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://no.szxytkj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cl.szxytkj.cn

C#:   d1 < d2;  d1 == d2
来源：http://ae.szxytkj.cn

[J08] 提取年月日与星期
来源：http://ls.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ul.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fe.hahajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zl.colortex.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kt.jianghongdianzi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kq.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pj.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://vs.szsharing.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://or.lnxyls.cn

[J09] 时区处理
来源：http://vl.521024.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tb.521024.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fc.yuntaijiaju.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mr.asd995.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://be.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jg.jianghongdianzi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://om.wgjwhj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ar.panjiajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://at.hahajie.cn

[J10] 取今天 / 本月第一天
来源：http://tm.wgjwhj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://zq.shxzukj.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://il.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gn.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fy.9csxet.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kb.huixinmuqiang.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://li.wgjwhj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yi.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fz.shxzukj.cn

================================================================================
来源：http://ok.huixinmuqiang.cn

K. JSON 与序列化
来源：http://gf.asd995.cn

================================================================================
来源：http://dq.shxzskj.cn

[K01] 对象转 JSON 字符串
来源：http://lq.panjiajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ow.newstarts.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pu.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://da.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://ji.yuexingan06.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pg.bookmarksfly.cn

Go:   json.Marshal(obj)
来源：http://zt.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zc.hnjuh.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://iq.gzmigu.cn

[K02] JSON 字符串转对象
来源：http://jd.hahajie.cn

Py:   json.loads(s)
来源：http://cn.muxihuayi.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ks.9csxet.cn

JS:   JSON.parse(s)
来源：http://og.newstarts.cn

TS:   JSON.parse(s)
来源：http://tc.bookmarksfly.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pw.shxzskj.cn

Go:   json.Unmarshal(data, &v)
来源：http://bb.nicolike.cn

Ruby: JSON.parse(s)
来源：http://cb.szsharing.cn


<!-- 参考信息 -->