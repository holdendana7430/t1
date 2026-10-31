代发 wailian999

[G14] 数据类 / record
来源：http://zu.yuexingan06.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gh.hnjuh.cn

PHP:  // 用 readonly 属性模拟
来源：http://fu.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://dt.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://hh.muxihuayi.cn

Java: record User(String name, int age) {}
来源：http://xi.shxzskj.cn

Go:   type User struct { Name string; Age int }
来源：http://vi.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uu.bjjhwx.cn

C#:   record User(string Name, int Age);
来源：http://ee.szsharing.cn

[G15] 枚举
来源：http://qn.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ne.shtwfgs.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ng.hahajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ma.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pt.bookmarksfly.cn

Java: enum Color { RED, GREEN }
来源：http://ex.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://am.hnjuh.cn

Ruby: Color = %i[red green].freeze
来源：http://kr.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jz.szsharing.cn

[G16] 对象转数组 / 字典
来源：http://jn.hahajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://cw.hnjuh.cn

PHP:  get_object_vars($obj);
来源：http://ys.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://zw.lnxyls.cn

TS:   Object.entries(obj)
来源：http://ps.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://su.shtwfgs.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fa.newstarts.cn

Ruby: obj.instance_variables
来源：http://rw.nicolike.cn

C#:   // 用反射或 System.Text.Json
来源：http://oi.hnjuh.cn

================================================================================
来源：http://fi.yuntaijiaju.cn

H. 异常与错误处理
来源：http://wv.yuntaijiaju.cn

================================================================================
来源：http://qh.9csxet.cn

[H01] try / catch 基础
来源：http://de.huixinmuqiang.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://al.huixinmuqiang.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wx.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ej.bookmarksfly.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://eh.yuexingan06.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fr.szxytkj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iq.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kr.szsharing.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sp.bookmarksfly.cn

[H02] finally / ensure 收尾
来源：http://qv.nicolike.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xb.wgjwhj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://mk.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ic.newstarts.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zj.asd995.cn

Java: try { f(); } finally { cleanup(); }
来源：http://on.newstarts.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://km.huixiangedu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ba.asd995.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lo.shxzukj.cn

[H03] 主动抛出异常
来源：http://os.gzmigu.cn

Py:   raise ValueError("错误信息")
来源：http://bc.wgjwhj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://aq.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://qy.shxzukj.cn

TS:   throw new Error("错误信息");
来源：http://gj.shtwfgs.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hg.gzmigu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://pw.panjiajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://qo.yuexingan06.cn

C#:   throw new ArgumentException("错误信息");
来源：http://yt.yuntaijiaju.cn

[H04] 自定义异常类型
来源：http://pe.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://in.wgjwhj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yr.shxzskj.cn

JS:   class MyError extends Error {}
来源：http://mm.szsharing.cn

TS:   class MyError extends Error {}
来源：http://rp.huanxung.cn

Java: class MyException extends RuntimeException {}
来源：http://am.haigaiapp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ti.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://tv.chemitech.net.cn

C#:   class MyException : Exception {}
来源：http://ac.huixiangedu.cn

[H05] 捕获特定类型
来源：http://es.colortex.cn

Py:   except ValueError as e:
来源：http://zm.muxihuayi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rx.shxzukj.cn

JS:   if (e instanceof TypeError) {}
来源：http://jo.wgjwhj.cn

TS:   if (e instanceof TypeError) {}
来源：http://on.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://lg.huixinmuqiang.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cp.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://yp.9csxet.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ky.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://ir.asd995.cn

Py:   value = d.get("k") or default
来源：http://jh.hnjuh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rm.wgjwhj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://eq.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ry.bookmarksfly.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xx.panjiajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qt.nszjky.cn

Ruby: d&.dig(:a, :b)
来源：http://ax.wgjwhj.cn

C#:   obj?.A?.B ?? default
来源：http://pp.szsharing.cn

[H07] 断言
来源：http://wj.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://hs.hahajie.cn

PHP:  assert($x > 0);
来源：http://bf.nszjky.cn

JS:   console.assert(x > 0);
来源：http://am.colortex.cn

TS:   console.assert(x > 0);
来源：http://vd.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://ht.9csxet.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yh.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vt.bjjhwx.cn

C#:   Debug.Assert(x > 0);
来源：http://ub.shxzskj.cn

[H08] 获取错误信息与堆栈
来源：http://rg.panjiajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://cc.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hl.szxytkj.cn

JS:   e.message;  e.stack
来源：http://nx.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wd.jianghongdianzi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zv.bookmarksfly.cn

Go:   err.Error()
来源：http://ko.muxihuayi.cn

Ruby: e.message;  e.backtrace
来源：http://aq.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://vc.chemitech.net.cn

[H09] 带错误码的异常
来源：http://ef.shxzukj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://px.jctech888.com.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://en.hahajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uu.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gz.huanxung.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yt.521024.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://br.shxzskj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://wl.lnxyls.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gg.muxihuayi.cn

[H10] 资源自动释放
来源：http://rr.szxytkj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rw.haigaiapp.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fq.nszjky.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gn.asd995.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://cn.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nx.jctech888.com.cn

Go:   defer f.Close()
来源：http://cn.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gv.bookmarksfly.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://my.bookmarksfly.cn

================================================================================
来源：http://el.gzmigu.cn

I. 正则表达式
来源：http://pj.lnxyls.cn

================================================================================
来源：http://km.gzmigu.cn

[I01] 判断是否匹配
来源：http://mh.panjiajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vs.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xn.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://ye.hnjuh.cn

TS:   /\d+/.test(s)
来源：http://qh.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://kf.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gk.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://mz.szsharing.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://no.chemitech.net.cn

[I02] 提取所有匹配
来源：http://ll.521024.cn

Py:   re.findall(r"\d+", s)
来源：http://md.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ru.shtwfgs.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yp.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://bt.521024.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rt.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sc.chemitech.net.cn

Ruby: s.scan(/\d+/)
来源：http://pm.gzmigu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gu.haigaiapp.cn

[I03] 提取捕获分组
来源：http://tg.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nz.yuntaijiaju.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qc.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jq.yuntaijiaju.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://do.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gg.yuexingan06.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yr.asd995.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qo.yuntaijiaju.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ic.shxzukj.cn

[I04] 正则替换
来源：http://hr.bjjhwx.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hj.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xc.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yn.huixiangedu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zh.lnxyls.cn

Java: s.replaceAll("\\d+", "#")
来源：http://km.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fm.jianghongdianzi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://db.chemitech.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://kn.shxzskj.cn

[I05] 按正则拆分
来源：http://eh.hnjuh.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://uj.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lg.shtwfgs.cn

JS:   s.split(/\s*,\s*/)
来源：http://mf.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://bx.huanxung.cn

Java: s.split("\\s*,\\s*")
来源：http://kc.szsharing.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ua.muxihuayi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://nd.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ph.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zd.huanxung.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dn.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rd.nszjky.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://es.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jt.yuexingan06.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sq.shxzskj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://lo.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lz.nicolike.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://za.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://du.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ox.wgjwhj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oo.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zw.nicolike.cn

TS:   /error/gim
来源：http://wr.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fm.newstarts.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://mp.hahajie.cn

Ruby: s.scan(/error/i)
来源：http://vj.lnxyls.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zd.shxzskj.cn

[I08] 贪婪与非贪婪匹配
来源：http://eo.yuexingan06.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bo.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://el.chemitech.net.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://uj.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hx.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://fl.asd995.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ay.haigaiapp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ns.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fp.panjiajie.cn

================================================================================
来源：http://kv.nicolike.cn

J. 日期与时间
来源：http://wj.colortex.cn

================================================================================
来源：http://tp.hahajie.cn

[J01] 获取当前时间
来源：http://il.huixinmuqiang.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vr.chemitech.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://aj.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://gx.haigaiapp.cn

TS:   new Date();  Date.now()
来源：http://ak.nicolike.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nc.nicolike.cn

Go:   time.Now()
来源：http://xo.lnxyls.cn

Ruby: Time.now
来源：http://hk.colortex.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tm.muxihuayi.cn

[J02] 格式化输出
来源：http://qs.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jc.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://im.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ou.huixinmuqiang.cn

TS:   d.toISOString()
来源：http://iv.521024.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jd.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jw.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tl.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://ih.szsharing.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xq.lnxyls.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vu.shxzukj.cn

JS:   new Date("2024-01-02")
来源：http://yn.muxihuayi.cn

TS:   new Date("2024-01-02")
来源：http://tc.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ij.nszjky.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://re.bjjhwx.cn

Ruby: Date.parse("2024-01-02")
来源：http://nz.521024.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://so.nszjky.cn

[J04] 时间戳与日期互转
来源：http://kv.bookmarksfly.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jw.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kf.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://jr.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nq.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jz.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qk.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tg.jctech888.com.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ut.shxzukj.cn

[J05] 时间加减（加 7 天）
来源：http://qt.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://ug.panjiajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gj.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xe.szxytkj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://tf.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://ut.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gc.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://fz.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qw.gzmigu.cn

[J06] 计算两时间之差
来源：http://eb.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://bh.hahajie.cn

PHP:  $end->diff($start)->days;
来源：http://lb.huanxung.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eb.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://je.bjjhwx.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lo.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://xs.521024.cn

Ruby: end - start                 # 返回秒数
来源：http://yh.lnxyls.cn

C#:   (end - start).TotalSeconds
来源：http://pv.shtwfgs.cn

[J07] 比较两个日期
来源：http://fe.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://yl.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rr.gzmigu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://jx.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://qt.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://az.shxzskj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sk.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cs.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://fr.huixinmuqiang.cn

[J08] 提取年月日与星期
来源：http://rp.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fa.bookmarksfly.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zh.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dl.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xj.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hn.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ym.shtwfgs.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nx.yuntaijiaju.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pa.9csxet.cn

[J09] 时区处理
来源：http://qv.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://tl.haigaiapp.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ev.chemitech.net.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qc.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zf.huixinmuqiang.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gg.yuexingan06.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ot.yuntaijiaju.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vs.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tu.nszjky.cn

[J10] 取今天 / 本月第一天
来源：http://lx.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sr.huixinmuqiang.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://rx.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://bl.nicolike.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://eg.huixinmuqiang.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ad.panjiajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sq.bjjhwx.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ny.nszjky.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dv.wgjwhj.cn

================================================================================
来源：http://hk.colortex.cn

K. JSON 与序列化
来源：http://xo.9csxet.cn

================================================================================
来源：http://te.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://ly.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yx.wgjwhj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pv.haigaiapp.cn

JS:   JSON.stringify(obj)
来源：http://px.lnxyls.cn

TS:   JSON.stringify(obj)
来源：http://jn.lnxyls.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mx.newstarts.cn

Go:   json.Marshal(obj)
来源：http://ct.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mh.shxzukj.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bz.colortex.cn


<!-- 参考信息 -->