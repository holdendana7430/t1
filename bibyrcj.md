代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://im.jctech888.com.cn

Java: record User(String name, int age) {}
来源：http://pn.9csxet.cn

Go:   type User struct { Name string; Age int }
来源：http://ta.nicolike.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qe.jianghongdianzi.cn

C#:   record User(string Name, int Age);
来源：http://ms.lnxyls.cn

[G15] 枚举
来源：http://zv.panjiajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oj.szxytkj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://yy.9csxet.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tm.lnxyls.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kp.shxzukj.cn

Java: enum Color { RED, GREEN }
来源：http://rq.szsharing.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fm.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://xh.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jn.shtwfgs.cn

[G16] 对象转数组 / 字典
来源：http://vb.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://nt.huanxung.cn

PHP:  get_object_vars($obj);
来源：http://qr.9csxet.cn

JS:   Object.entries(obj)
来源：http://pr.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://ec.shxzskj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lg.huixiangedu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dt.huanxung.cn

Ruby: obj.instance_variables
来源：http://og.521024.cn

C#:   // 用反射或 System.Text.Json
来源：http://bf.shxzukj.cn

================================================================================
来源：http://ck.shxzukj.cn

H. 异常与错误处理
来源：http://uo.chemitech.net.cn

================================================================================
来源：http://ix.chemitech.net.cn

[H01] try / catch 基础
来源：http://qc.jianghongdianzi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dt.newstarts.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lc.huixiangedu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zz.szxytkj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jo.521024.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sd.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://da.yuexingan06.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://bo.bjjhwx.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uw.jianghongdianzi.cn

[H02] finally / ensure 收尾
来源：http://en.9csxet.cn

Py:   try: f()⏎finally: cleanup()
来源：http://mg.muxihuayi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ce.szxytkj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qs.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://of.yuexingan06.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bv.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pj.szxytkj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://al.gzmigu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yq.jctech888.com.cn

[H03] 主动抛出异常
来源：http://bc.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://hj.muxihuayi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://se.bookmarksfly.cn

JS:   throw new Error("错误信息");
来源：http://rc.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://dr.szxytkj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://kd.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ar.9csxet.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xu.huixiangedu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://sd.lnxyls.cn

[H04] 自定义异常类型
来源：http://iw.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://oj.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mx.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://pc.yuexingan06.cn

TS:   class MyError extends Error {}
来源：http://ep.hahajie.cn

Java: class MyException extends RuntimeException {}
来源：http://ee.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lx.szxytkj.cn

Ruby: class MyError < StandardError; end
来源：http://uw.muxihuayi.cn

C#:   class MyException : Exception {}
来源：http://sb.bjjhwx.cn

[H05] 捕获特定类型
来源：http://oi.hnjuh.cn

Py:   except ValueError as e:
来源：http://ez.hnjuh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yb.szsharing.cn

JS:   if (e instanceof TypeError) {}
来源：http://is.shxzskj.cn

TS:   if (e instanceof TypeError) {}
来源：http://qb.chemitech.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://ry.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ij.szsharing.cn

Ruby: rescue ArgumentError => e
来源：http://tt.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xt.bjjhwx.cn

[H06] 可选值 / 空值安全访问
来源：http://zj.shxzskj.cn

Py:   value = d.get("k") or default
来源：http://su.asd995.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xs.szsharing.cn

JS:   obj?.a?.b;  d ?? default
来源：http://fh.yuexingan06.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lz.yuexingan06.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://xd.9csxet.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jk.muxihuayi.cn

Ruby: d&.dig(:a, :b)
来源：http://yn.9csxet.cn

C#:   obj?.A?.B ?? default
来源：http://wc.yuntaijiaju.cn

[H07] 断言
来源：http://fc.colortex.cn

Py:   assert x > 0, "必须为正"
来源：http://ri.szxytkj.cn

PHP:  assert($x > 0);
来源：http://wv.szxytkj.cn

JS:   console.assert(x > 0);
来源：http://ei.shxzukj.cn

TS:   console.assert(x > 0);
来源：http://dn.yuntaijiaju.cn

Java: assert x > 0 : "必须为正";
来源：http://no.asd995.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xa.nszjky.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cy.panjiajie.cn

C#:   Debug.Assert(x > 0);
来源：http://lt.huixiangedu.cn

[H08] 获取错误信息与堆栈
来源：http://vm.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://lr.szxytkj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://av.newstarts.cn

JS:   e.message;  e.stack
来源：http://on.asd995.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://iz.shxzskj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uc.nszjky.cn

Go:   err.Error()
来源：http://ec.haigaiapp.cn

Ruby: e.message;  e.backtrace
来源：http://fx.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://ro.yuntaijiaju.cn

[H09] 带错误码的异常
来源：http://it.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pt.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qt.haigaiapp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uu.huixiangedu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fn.shxzskj.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qi.haigaiapp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fa.colortex.cn

Ruby: raise MyError.new("fail", 500)
来源：http://kx.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://sz.bookmarksfly.cn

[H10] 资源自动释放
来源：http://zw.huixiangedu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wi.shxzukj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dq.newstarts.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://vy.shtwfgs.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yf.jianghongdianzi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fu.asd995.cn

Go:   defer f.Close()
来源：http://kc.muxihuayi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://cv.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xe.9csxet.cn

================================================================================
来源：http://bj.szsharing.cn

I. 正则表达式
来源：http://ss.9csxet.cn

================================================================================
来源：http://qr.shtwfgs.cn

[I01] 判断是否匹配
来源：http://ga.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://nw.huixiangedu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zn.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://oi.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://ja.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zz.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wt.chemitech.net.cn

Ruby: s.match?(/\d+/)
来源：http://tm.shxzskj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yr.bjjhwx.cn

[I02] 提取所有匹配
来源：http://pe.nszjky.cn

Py:   re.findall(r"\d+", s)
来源：http://hc.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rt.bookmarksfly.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yx.wgjwhj.cn

TS:   s.match(/\d+/g)
来源：http://pk.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oo.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://dq.yuntaijiaju.cn

Ruby: s.scan(/\d+/)
来源：http://wi.gzmigu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pd.hahajie.cn

[I03] 提取捕获分组
来源：http://go.shtwfgs.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vw.szsharing.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ga.bookmarksfly.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bw.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oy.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xn.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://de.panjiajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ba.bookmarksfly.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xi.huixinmuqiang.cn

[I04] 正则替换
来源：http://un.yuexingan06.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://od.9csxet.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lg.szxytkj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jp.hahajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nq.szxytkj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://iw.hnjuh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://la.szxytkj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ph.huanxung.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ea.asd995.cn

[I05] 按正则拆分
来源：http://ak.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ko.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ka.bookmarksfly.cn

JS:   s.split(/\s*,\s*/)
来源：http://mn.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://jw.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://ui.szsharing.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yp.hnjuh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://by.gzmigu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mf.nszjky.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nb.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gq.yuexingan06.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yx.bookmarksfly.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qa.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ta.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ma.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://li.huixinmuqiang.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wy.lnxyls.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oq.jctech888.com.cn

[I07] 忽略大小写与多行模式
来源：http://sa.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sw.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xn.nicolike.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ol.bjjhwx.cn

TS:   /error/gim
来源：http://ef.panjiajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wf.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dg.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://qi.asd995.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sr.chemitech.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://ed.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rn.jctech888.com.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://md.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cc.bjjhwx.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ab.asd995.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mr.huixiangedu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jt.panjiajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fg.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bu.jianghongdianzi.cn

================================================================================
来源：http://mm.huixiangedu.cn

J. 日期与时间
来源：http://ah.nicolike.cn

================================================================================
来源：http://qw.shxzukj.cn

[J01] 获取当前时间
来源：http://nb.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://sp.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fv.haigaiapp.cn

JS:   new Date();  Date.now()
来源：http://ey.bjjhwx.cn

TS:   new Date();  Date.now()
来源：http://pd.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://al.chemitech.net.cn

Go:   time.Now()
来源：http://vy.yuexingan06.cn

Ruby: Time.now
来源：http://wk.521024.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wz.shxzukj.cn

[J02] 格式化输出
来源：http://sn.gzmigu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tj.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qk.shxzskj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uh.panjiajie.cn

TS:   d.toISOString()
来源：http://ws.521024.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hu.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fc.shxzukj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bj.lnxyls.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ri.gzmigu.cn

[J03] 字符串解析为日期
来源：http://aw.newstarts.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sl.shxzskj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pk.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://ps.panjiajie.cn

TS:   new Date("2024-01-02")
来源：http://ti.hahajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wc.nszjky.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://oa.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://iz.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qa.shxzukj.cn

[J04] 时间戳与日期互转
来源：http://bt.nicolike.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://is.wgjwhj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ie.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hb.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://we.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zn.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://yw.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://po.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ua.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://qp.nicolike.cn

Py:   now + timedelta(days=7)
来源：http://iv.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://om.nszjky.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://zi.chemitech.net.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bk.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://gn.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://co.bookmarksfly.cn

Ruby: Time.now + 7 * 86400
来源：http://mp.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://uf.szsharing.cn

[J06] 计算两时间之差
来源：http://ht.newstarts.cn

Py:   (end - start).total_seconds()
来源：http://sc.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://fz.muxihuayi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://fc.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bo.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://el.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://of.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://uo.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://yi.lnxyls.cn

[J07] 比较两个日期
来源：http://jh.muxihuayi.cn

Py:   d1 < d2;  d1 == d2
来源：http://ki.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kb.9csxet.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ip.521024.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ck.panjiajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cu.nszjky.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tm.bookmarksfly.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fn.gzmigu.cn

C#:   d1 < d2;  d1 == d2
来源：http://vy.chemitech.net.cn

[J08] 提取年月日与星期
来源：http://fw.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dr.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://js.newstarts.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kh.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bp.nszjky.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yu.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ff.lnxyls.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ob.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mc.szsharing.cn

[J09] 时区处理
来源：http://el.gzmigu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jt.chemitech.net.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ip.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qv.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://we.jctech888.com.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://if.wgjwhj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bs.muxihuayi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dw.521024.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tj.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://ir.shtwfgs.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://sh.521024.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ch.hahajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://od.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pz.9csxet.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oj.bjjhwx.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vz.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kd.shtwfgs.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wj.yuntaijiaju.cn

================================================================================
来源：http://gq.szxytkj.cn

K. JSON 与序列化
来源：http://np.colortex.cn

================================================================================
来源：http://vf.yuntaijiaju.cn

[K01] 对象转 JSON 字符串
来源：http://tn.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://gk.bjjhwx.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nv.shxzukj.cn

JS:   JSON.stringify(obj)
来源：http://ms.chemitech.net.cn

TS:   JSON.stringify(obj)
来源：http://ln.huixiangedu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yz.9csxet.cn

Go:   json.Marshal(obj)
来源：http://oq.hnjuh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://th.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ad.shxzukj.cn

[K02] JSON 字符串转对象
来源：http://rn.hahajie.cn

Py:   json.loads(s)
来源：http://zu.gzmigu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ja.hahajie.cn

JS:   JSON.parse(s)
来源：http://dz.asd995.cn


<!-- 参考信息 -->