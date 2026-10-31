代发 wailian999

C#:   record User(string Name, int Age);
来源：http://kv.bjjhwx.cn

[G15] 枚举
来源：http://jr.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://jn.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cv.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yk.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sj.bjjhwx.cn

Java: enum Color { RED, GREEN }
来源：http://mw.shxzskj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dn.wgjwhj.cn

Ruby: Color = %i[red green].freeze
来源：http://aq.shxzskj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ut.shxzukj.cn

[G16] 对象转数组 / 字典
来源：http://cr.521024.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yn.hahajie.cn

PHP:  get_object_vars($obj);
来源：http://la.hahajie.cn

JS:   Object.entries(obj)
来源：http://nt.huixinmuqiang.cn

TS:   Object.entries(obj)
来源：http://cp.huixinmuqiang.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://te.yuexingan06.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tq.szsharing.cn

Ruby: obj.instance_variables
来源：http://ta.huixinmuqiang.cn

C#:   // 用反射或 System.Text.Json
来源：http://oj.nszjky.cn

================================================================================
来源：http://jc.shtwfgs.cn

H. 异常与错误处理
来源：http://nn.shxzukj.cn

================================================================================
来源：http://tb.yuntaijiaju.cn

[H01] try / catch 基础
来源：http://hz.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dx.nicolike.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nr.nicolike.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ur.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sp.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vx.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://en.shxzukj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ru.hahajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gm.jianghongdianzi.cn

[H02] finally / ensure 收尾
来源：http://yt.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ee.shxzukj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://du.yuexingan06.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yq.wgjwhj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rf.shxzukj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pq.yuntaijiaju.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://kf.shxzskj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mq.nicolike.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tp.gzmigu.cn

[H03] 主动抛出异常
来源：http://yt.newstarts.cn

Py:   raise ValueError("错误信息")
来源：http://bl.bookmarksfly.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://et.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://gm.bookmarksfly.cn

TS:   throw new Error("错误信息");
来源：http://zj.bjjhwx.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dq.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gm.panjiajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wz.asd995.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ir.wgjwhj.cn

[H04] 自定义异常类型
来源：http://iu.shxzskj.cn

Py:   class MyError(Exception): pass
来源：http://zb.shxzukj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ec.szsharing.cn

JS:   class MyError extends Error {}
来源：http://fx.huanxung.cn

TS:   class MyError extends Error {}
来源：http://zx.huanxung.cn

Java: class MyException extends RuntimeException {}
来源：http://gk.colortex.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nb.shtwfgs.cn

Ruby: class MyError < StandardError; end
来源：http://lg.521024.cn

C#:   class MyException : Exception {}
来源：http://qt.521024.cn

[H05] 捕获特定类型
来源：http://jk.lnxyls.cn

Py:   except ValueError as e:
来源：http://ah.yuexingan06.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hd.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://rj.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://gj.huixinmuqiang.cn

Java: catch (IOException | SQLException e) {}
来源：http://yw.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nc.shxzskj.cn

Ruby: rescue ArgumentError => e
来源：http://fn.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qu.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://kz.521024.cn

Py:   value = d.get("k") or default
来源：http://tg.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://al.huixinmuqiang.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rr.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yd.shxzukj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gp.yuexingan06.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ag.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://nv.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://js.hahajie.cn

[H07] 断言
来源：http://on.chemitech.net.cn

Py:   assert x > 0, "必须为正"
来源：http://tm.huixinmuqiang.cn

PHP:  assert($x > 0);
来源：http://tq.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://ef.huanxung.cn

TS:   console.assert(x > 0);
来源：http://mk.hnjuh.cn

Java: assert x > 0 : "必须为正";
来源：http://tl.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dp.szsharing.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zk.huanxung.cn

C#:   Debug.Assert(x > 0);
来源：http://os.jctech888.com.cn

[H08] 获取错误信息与堆栈
来源：http://ra.jianghongdianzi.cn

Py:   str(e);  traceback.format_exc()
来源：http://sb.haigaiapp.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lz.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://fy.wgjwhj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bj.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://sj.huixiangedu.cn

Go:   err.Error()
来源：http://at.szxytkj.cn

Ruby: e.message;  e.backtrace
来源：http://ks.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://ad.521024.cn

[H09] 带错误码的异常
来源：http://tx.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tj.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ik.asd995.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sz.szsharing.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://uf.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://al.chemitech.net.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jy.szxytkj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://zv.newstarts.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://id.bjjhwx.cn

[H10] 资源自动释放
来源：http://gx.521024.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://je.muxihuayi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fr.wgjwhj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rm.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vq.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vd.huixiangedu.cn

Go:   defer f.Close()
来源：http://ua.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tb.bjjhwx.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qa.newstarts.cn

================================================================================
来源：http://db.bjjhwx.cn

I. 正则表达式
来源：http://ao.hahajie.cn

================================================================================
来源：http://oy.newstarts.cn

[I01] 判断是否匹配
来源：http://xt.shxzukj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://un.gzmigu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lf.szxytkj.cn

JS:   /\d+/.test(s)
来源：http://gw.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://rt.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vi.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ok.huixiangedu.cn

Ruby: s.match?(/\d+/)
来源：http://vg.shxzukj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ko.hahajie.cn

[I02] 提取所有匹配
来源：http://bx.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://li.asd995.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://gp.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://em.hnjuh.cn

TS:   s.match(/\d+/g)
来源：http://ak.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fs.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://zb.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://qz.yuexingan06.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ng.colortex.cn

[I03] 提取捕获分组
来源：http://pq.hahajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sp.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://us.muxihuayi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mr.lnxyls.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pg.yuntaijiaju.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oe.szsharing.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xq.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://li.yuexingan06.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rp.bookmarksfly.cn

[I04] 正则替换
来源：http://vh.shxzukj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://mk.nszjky.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kj.521024.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vs.9csxet.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rb.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hm.nicolike.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qg.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://mi.nszjky.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gp.haigaiapp.cn

[I05] 按正则拆分
来源：http://ub.szsharing.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ly.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zn.huixinmuqiang.cn

JS:   s.split(/\s*,\s*/)
来源：http://hj.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://ct.gzmigu.cn

Java: s.split("\\s*,\\s*")
来源：http://so.chemitech.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xp.shxzskj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sk.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cb.newstarts.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://uf.colortex.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ri.yuntaijiaju.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://cs.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tl.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ub.shxzukj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ud.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pe.muxihuayi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gw.panjiajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ls.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://kb.szsharing.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mv.hahajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ty.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pp.muxihuayi.cn

TS:   /error/gim
来源：http://dz.muxihuayi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://se.szsharing.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ls.jianghongdianzi.cn

Ruby: s.scan(/error/i)
来源：http://gl.chemitech.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qm.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://ja.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hl.huixinmuqiang.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ne.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://iv.huanxung.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://be.shtwfgs.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ra.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ru.haigaiapp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pc.lnxyls.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vg.szsharing.cn

================================================================================
来源：http://ey.521024.cn

J. 日期与时间
来源：http://xb.bjjhwx.cn

================================================================================
来源：http://kg.panjiajie.cn

[J01] 获取当前时间
来源：http://by.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rj.newstarts.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vs.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://yj.asd995.cn

TS:   new Date();  Date.now()
来源：http://bg.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://re.lnxyls.cn

Go:   time.Now()
来源：http://xi.panjiajie.cn

Ruby: Time.now
来源：http://ke.panjiajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wi.wgjwhj.cn

[J02] 格式化输出
来源：http://rt.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uu.haigaiapp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://si.9csxet.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://if.muxihuayi.cn

TS:   d.toISOString()
来源：http://lk.shxzukj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://dc.yuexingan06.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mr.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ml.9csxet.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ge.colortex.cn

[J03] 字符串解析为日期
来源：http://qz.chemitech.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wq.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kx.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://yc.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://ce.huanxung.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vz.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xk.huanxung.cn

Ruby: Date.parse("2024-01-02")
来源：http://tm.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lp.hahajie.cn

[J04] 时间戳与日期互转
来源：http://bl.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sc.lnxyls.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://pd.shxzukj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rw.shxzskj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xc.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ae.asd995.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sj.huixiangedu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fw.colortex.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pl.szxytkj.cn

[J05] 时间加减（加 7 天）
来源：http://jb.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://lr.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ll.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sx.panjiajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pm.nszjky.cn

Java: LocalDate.now().plusDays(7)
来源：http://ia.shxzukj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://df.lnxyls.cn

Ruby: Time.now + 7 * 86400
来源：http://yq.lnxyls.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ty.hnjuh.cn

[J06] 计算两时间之差
来源：http://as.newstarts.cn

Py:   (end - start).total_seconds()
来源：http://jg.bjjhwx.cn

PHP:  $end->diff($start)->days;
来源：http://ik.hahajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rh.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sl.521024.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kt.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://na.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://kw.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://ph.szxytkj.cn

[J07] 比较两个日期
来源：http://qb.muxihuayi.cn

Py:   d1 < d2;  d1 == d2
来源：http://en.muxihuayi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dv.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://se.huanxung.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zw.shxzukj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rc.yuexingan06.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dc.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qe.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://bx.huixiangedu.cn

[J08] 提取年月日与星期
来源：http://wp.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ui.hnjuh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qj.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qv.bjjhwx.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hv.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rs.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mc.shtwfgs.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ws.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rw.yuexingan06.cn

[J09] 时区处理
来源：http://ui.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ef.panjiajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gy.gzmigu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ys.shtwfgs.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gv.jctech888.com.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bg.yuntaijiaju.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rh.bookmarksfly.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dd.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oi.bjjhwx.cn

[J10] 取今天 / 本月第一天
来源：http://ys.yuntaijiaju.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://aw.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yg.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://di.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uv.9csxet.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ew.newstarts.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://rc.9csxet.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vp.jctech888.com.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kv.wgjwhj.cn

================================================================================
来源：http://in.jianghongdianzi.cn

K. JSON 与序列化
来源：http://br.jctech888.com.cn

================================================================================
来源：http://cp.huixinmuqiang.cn

[K01] 对象转 JSON 字符串
来源：http://vi.panjiajie.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ni.chemitech.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xc.shxzukj.cn

JS:   JSON.stringify(obj)
来源：http://ez.szsharing.cn

TS:   JSON.stringify(obj)
来源：http://xd.521024.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gl.jctech888.com.cn

Go:   json.Marshal(obj)
来源：http://ym.yuexingan06.cn

Ruby: obj.to_json                                     // require "json"
来源：http://qc.huanxung.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ry.shxzskj.cn

[K02] JSON 字符串转对象
来源：http://fp.bookmarksfly.cn

Py:   json.loads(s)
来源：http://qf.jctech888.com.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://bl.shxzskj.cn

JS:   JSON.parse(s)
来源：http://jb.jianghongdianzi.cn

TS:   JSON.parse(s)
来源：http://hn.shxzukj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hx.shxzukj.cn

Go:   json.Unmarshal(data, &v)
来源：http://fz.nszjky.cn

Ruby: JSON.parse(s)
来源：http://jk.huixiangedu.cn


<!-- 参考信息 -->