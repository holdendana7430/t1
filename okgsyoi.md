代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://ek.huanxung.cn

Java: record User(String name, int age) {}
来源：http://zz.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://eq.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lz.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://iw.panjiajie.cn

[G15] 枚举
来源：http://nf.hnjuh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xx.shxzukj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mi.shxzskj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vf.chemitech.net.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fl.lnxyls.cn

Java: enum Color { RED, GREEN }
来源：http://ls.nszjky.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wk.huixiangedu.cn

Ruby: Color = %i[red green].freeze
来源：http://bo.hnjuh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zl.muxihuayi.cn

[G16] 对象转数组 / 字典
来源：http://sz.bookmarksfly.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jn.shxzskj.cn

PHP:  get_object_vars($obj);
来源：http://mv.colortex.cn

JS:   Object.entries(obj)
来源：http://em.shxzukj.cn

TS:   Object.entries(obj)
来源：http://ka.newstarts.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gu.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pl.bjjhwx.cn

Ruby: obj.instance_variables
来源：http://qc.shtwfgs.cn

C#:   // 用反射或 System.Text.Json
来源：http://ik.newstarts.cn

================================================================================
来源：http://nk.yuexingan06.cn

H. 异常与错误处理
来源：http://vn.asd995.cn

================================================================================
来源：http://oc.haigaiapp.cn

[H01] try / catch 基础
来源：http://bz.hnjuh.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fo.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://og.jctech888.com.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vo.szsharing.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://to.szsharing.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dq.lnxyls.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zf.szsharing.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://os.szxytkj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jt.yuntaijiaju.cn

[H02] finally / ensure 收尾
来源：http://xw.hnjuh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ip.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://te.szxytkj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zp.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ip.huanxung.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sx.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://xk.panjiajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ly.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cp.hnjuh.cn

[H03] 主动抛出异常
来源：http://ah.shtwfgs.cn

Py:   raise ValueError("错误信息")
来源：http://hn.yuexingan06.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bd.9csxet.cn

JS:   throw new Error("错误信息");
来源：http://kx.panjiajie.cn

TS:   throw new Error("错误信息");
来源：http://wu.muxihuayi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yp.asd995.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sf.shxzukj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wi.huixiangedu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pi.hahajie.cn

[H04] 自定义异常类型
来源：http://kw.9csxet.cn

Py:   class MyError(Exception): pass
来源：http://yn.shtwfgs.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wv.jctech888.com.cn

JS:   class MyError extends Error {}
来源：http://xb.nicolike.cn

TS:   class MyError extends Error {}
来源：http://cm.asd995.cn

Java: class MyException extends RuntimeException {}
来源：http://lo.chemitech.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://er.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://qe.muxihuayi.cn

C#:   class MyException : Exception {}
来源：http://qe.bookmarksfly.cn

[H05] 捕获特定类型
来源：http://ze.nicolike.cn

Py:   except ValueError as e:
来源：http://iw.nicolike.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kl.haigaiapp.cn

JS:   if (e instanceof TypeError) {}
来源：http://un.shtwfgs.cn

TS:   if (e instanceof TypeError) {}
来源：http://hx.asd995.cn

Java: catch (IOException | SQLException e) {}
来源：http://xl.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://iu.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://nl.asd995.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://qi.chemitech.net.cn

[H06] 可选值 / 空值安全访问
来源：http://kh.muxihuayi.cn

Py:   value = d.get("k") or default
来源：http://qu.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lg.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vr.hnjuh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yc.nicolike.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mb.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://pq.huixinmuqiang.cn

Ruby: d&.dig(:a, :b)
来源：http://ym.szsharing.cn

C#:   obj?.A?.B ?? default
来源：http://jz.lnxyls.cn

[H07] 断言
来源：http://gx.muxihuayi.cn

Py:   assert x > 0, "必须为正"
来源：http://rw.shtwfgs.cn

PHP:  assert($x > 0);
来源：http://ng.yuntaijiaju.cn

JS:   console.assert(x > 0);
来源：http://ok.huanxung.cn

TS:   console.assert(x > 0);
来源：http://qv.haigaiapp.cn

Java: assert x > 0 : "必须为正";
来源：http://jc.gzmigu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://vp.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bk.haigaiapp.cn

C#:   Debug.Assert(x > 0);
来源：http://ks.huixinmuqiang.cn

[H08] 获取错误信息与堆栈
来源：http://yn.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://kx.shtwfgs.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gh.jctech888.com.cn

JS:   e.message;  e.stack
来源：http://uh.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xv.nszjky.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bh.gzmigu.cn

Go:   err.Error()
来源：http://rv.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://mq.yuntaijiaju.cn

C#:   e.Message;  e.StackTrace
来源：http://om.chemitech.net.cn

[H09] 带错误码的异常
来源：http://pg.yuntaijiaju.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oc.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cl.hahajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://di.hahajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vl.lnxyls.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vw.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ey.haigaiapp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ax.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ex.haigaiapp.cn

[H10] 资源自动释放
来源：http://zs.bookmarksfly.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vd.shxzskj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://uu.muxihuayi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nw.huixiangedu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://om.panjiajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bg.muxihuayi.cn

Go:   defer f.Close()
来源：http://ip.yuexingan06.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ws.huixiangedu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://eu.9csxet.cn

================================================================================
来源：http://ab.chemitech.net.cn

I. 正则表达式
来源：http://cc.yuntaijiaju.cn

================================================================================
来源：http://ww.nicolike.cn

[I01] 判断是否匹配
来源：http://bw.jctech888.com.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://dc.shxzskj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vl.jianghongdianzi.cn

JS:   /\d+/.test(s)
来源：http://eo.nszjky.cn

TS:   /\d+/.test(s)
来源：http://iu.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ww.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oq.newstarts.cn

Ruby: s.match?(/\d+/)
来源：http://kc.szxytkj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cp.newstarts.cn

[I02] 提取所有匹配
来源：http://lq.panjiajie.cn

Py:   re.findall(r"\d+", s)
来源：http://nf.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wl.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ob.colortex.cn

TS:   s.match(/\d+/g)
来源：http://fj.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fg.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kk.chemitech.net.cn

Ruby: s.scan(/\d+/)
来源：http://nd.shxzukj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ln.lnxyls.cn

[I03] 提取捕获分组
来源：http://eb.huixinmuqiang.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wj.huanxung.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wl.hnjuh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nb.nszjky.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wu.nszjky.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qi.shxzskj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rs.shxzskj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ao.chemitech.net.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://kk.9csxet.cn

[I04] 正则替换
来源：http://eq.newstarts.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yq.chemitech.net.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://du.hnjuh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ka.hahajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://wo.yuexingan06.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qx.jianghongdianzi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lm.gzmigu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://kh.jctech888.com.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rw.haigaiapp.cn

[I05] 按正则拆分
来源：http://sz.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://zz.jctech888.com.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yw.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://zw.yuexingan06.cn

TS:   s.split(/\s*,\s*/)
来源：http://un.521024.cn

Java: s.split("\\s*,\\s*")
来源：http://wh.haigaiapp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://mh.jctech888.com.cn

Ruby: s.split(/\s*,\s*/)
来源：http://tx.muxihuayi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bx.yuntaijiaju.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://lz.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ke.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nv.nicolike.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hn.jctech888.com.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ua.9csxet.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ii.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xy.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ho.yuntaijiaju.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ty.muxihuayi.cn

[I07] 忽略大小写与多行模式
来源：http://tr.huanxung.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bf.huixiangedu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jf.yuexingan06.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://er.shxzskj.cn

TS:   /error/gim
来源：http://ta.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pm.chemitech.net.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mh.hnjuh.cn

Ruby: s.scan(/error/i)
来源：http://py.lnxyls.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wr.gzmigu.cn

[I08] 贪婪与非贪婪匹配
来源：http://pv.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nn.chemitech.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nj.colortex.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ta.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lh.colortex.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ss.jctech888.com.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mx.jianghongdianzi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oq.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bp.newstarts.cn

================================================================================
来源：http://nb.shtwfgs.cn

J. 日期与时间
来源：http://pk.nszjky.cn

================================================================================
来源：http://ly.9csxet.cn

[J01] 获取当前时间
来源：http://zg.hnjuh.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kl.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://rb.lnxyls.cn

JS:   new Date();  Date.now()
来源：http://lb.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://ek.colortex.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://tc.haigaiapp.cn

Go:   time.Now()
来源：http://it.shxzskj.cn

Ruby: Time.now
来源：http://kk.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://rj.szxytkj.cn

[J02] 格式化输出
来源：http://ez.521024.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sl.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gh.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yu.hnjuh.cn

TS:   d.toISOString()
来源：http://cs.huixinmuqiang.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jw.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qu.muxihuayi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://to.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://gs.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://jt.shxzskj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xh.huixiangedu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zi.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://fh.lnxyls.cn

TS:   new Date("2024-01-02")
来源：http://dq.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xm.9csxet.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zd.hahajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://ym.nszjky.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gv.szsharing.cn

[J04] 时间戳与日期互转
来源：http://ui.nicolike.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ey.bjjhwx.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yx.bjjhwx.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://bh.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ft.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://iw.yuexingan06.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gn.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://yb.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sf.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://rj.asd995.cn

Py:   now + timedelta(days=7)
来源：http://ff.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hl.nszjky.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xu.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://yz.shtwfgs.cn

Java: LocalDate.now().plusDays(7)
来源：http://bq.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dl.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://dr.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ww.shtwfgs.cn

[J06] 计算两时间之差
来源：http://zi.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://en.shtwfgs.cn

PHP:  $end->diff($start)->days;
来源：http://pb.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mi.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://li.newstarts.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sb.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://jr.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://ug.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://da.szsharing.cn

[J07] 比较两个日期
来源：http://za.shtwfgs.cn

Py:   d1 < d2;  d1 == d2
来源：http://li.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://re.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fo.nicolike.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kt.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://rr.lnxyls.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yd.huixiangedu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mz.wgjwhj.cn

C#:   d1 < d2;  d1 == d2
来源：http://ms.szxytkj.cn

[J08] 提取年月日与星期
来源：http://hw.szxytkj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ri.huanxung.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dq.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xz.yuntaijiaju.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wo.jctech888.com.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://xe.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tp.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lt.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jz.hahajie.cn

[J09] 时区处理
来源：http://an.asd995.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bv.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oa.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://he.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yp.bjjhwx.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ga.shxzskj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fb.panjiajie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cv.panjiajie.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xm.huixinmuqiang.cn

[J10] 取今天 / 本月第一天
来源：http://ff.muxihuayi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vu.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pg.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ti.wgjwhj.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ay.lnxyls.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mj.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zu.muxihuayi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vz.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://io.bjjhwx.cn

================================================================================
来源：http://tj.yuexingan06.cn

K. JSON 与序列化
来源：http://tw.asd995.cn

================================================================================
来源：http://sq.jianghongdianzi.cn

[K01] 对象转 JSON 字符串
来源：http://ni.szxytkj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tw.huixiangedu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://de.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://bd.newstarts.cn

TS:   JSON.stringify(obj)
来源：http://sm.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ff.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://js.huixinmuqiang.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pc.bjjhwx.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://nz.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://mq.wgjwhj.cn

Py:   json.loads(s)
来源：http://er.yuntaijiaju.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mt.asd995.cn

JS:   JSON.parse(s)
来源：http://yq.hahajie.cn


<!-- 参考信息 -->