代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://ks.jctech888.com.cn

Java: record User(String name, int age) {}
来源：http://fg.nszjky.cn

Go:   type User struct { Name string; Age int }
来源：http://zm.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://je.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://gc.huixiangedu.cn

[G15] 枚举
来源：http://uf.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yr.gzmigu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dj.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ld.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://qc.colortex.cn

Java: enum Color { RED, GREEN }
来源：http://tl.nicolike.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bq.huanxung.cn

Ruby: Color = %i[red green].freeze
来源：http://kh.521024.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jp.521024.cn

[G16] 对象转数组 / 字典
来源：http://kb.hnjuh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ta.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://ux.gzmigu.cn

JS:   Object.entries(obj)
来源：http://bj.chemitech.net.cn

TS:   Object.entries(obj)
来源：http://hd.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gr.lnxyls.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://uj.nszjky.cn

Ruby: obj.instance_variables
来源：http://se.colortex.cn

C#:   // 用反射或 System.Text.Json
来源：http://en.lnxyls.cn

================================================================================
来源：http://cr.muxihuayi.cn

H. 异常与错误处理
来源：http://xw.hahajie.cn

================================================================================
来源：http://fu.shtwfgs.cn

[H01] try / catch 基础
来源：http://qp.lnxyls.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sc.szsharing.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cb.shxzskj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sp.gzmigu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jr.colortex.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gx.shtwfgs.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gk.jctech888.com.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zf.haigaiapp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qi.jctech888.com.cn

[H02] finally / ensure 收尾
来源：http://fx.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ud.gzmigu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://or.yuexingan06.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lu.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vy.9csxet.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ra.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ns.asd995.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://il.chemitech.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tc.shxzskj.cn

[H03] 主动抛出异常
来源：http://uk.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://am.521024.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ls.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://zt.bjjhwx.cn

TS:   throw new Error("错误信息");
来源：http://pj.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qk.szsharing.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://as.nicolike.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ux.lnxyls.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nk.gzmigu.cn

[H04] 自定义异常类型
来源：http://tm.colortex.cn

Py:   class MyError(Exception): pass
来源：http://cl.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dr.huixiangedu.cn

JS:   class MyError extends Error {}
来源：http://pj.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://at.panjiajie.cn

Java: class MyException extends RuntimeException {}
来源：http://ai.chemitech.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ri.panjiajie.cn

Ruby: class MyError < StandardError; end
来源：http://xd.nszjky.cn

C#:   class MyException : Exception {}
来源：http://rj.nicolike.cn

[H05] 捕获特定类型
来源：http://kv.szsharing.cn

Py:   except ValueError as e:
来源：http://yt.lnxyls.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fd.szxytkj.cn

JS:   if (e instanceof TypeError) {}
来源：http://vy.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://mm.jianghongdianzi.cn

Java: catch (IOException | SQLException e) {}
来源：http://jt.hnjuh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sw.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://qn.huixiangedu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ts.shxzskj.cn

[H06] 可选值 / 空值安全访问
来源：http://ds.asd995.cn

Py:   value = d.get("k") or default
来源：http://mu.chemitech.net.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tw.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rh.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ks.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ik.yuexingan06.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gg.newstarts.cn

Ruby: d&.dig(:a, :b)
来源：http://zd.jctech888.com.cn

C#:   obj?.A?.B ?? default
来源：http://ae.gzmigu.cn

[H07] 断言
来源：http://ia.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://in.gzmigu.cn

PHP:  assert($x > 0);
来源：http://pe.gzmigu.cn

JS:   console.assert(x > 0);
来源：http://sn.nicolike.cn

TS:   console.assert(x > 0);
来源：http://du.lnxyls.cn

Java: assert x > 0 : "必须为正";
来源：http://iu.gzmigu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://fj.huixinmuqiang.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lh.gzmigu.cn

C#:   Debug.Assert(x > 0);
来源：http://ul.haigaiapp.cn

[H08] 获取错误信息与堆栈
来源：http://fs.yuntaijiaju.cn

Py:   str(e);  traceback.format_exc()
来源：http://hp.nicolike.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sc.jianghongdianzi.cn

JS:   e.message;  e.stack
来源：http://uc.huanxung.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pf.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nr.asd995.cn

Go:   err.Error()
来源：http://lq.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://hx.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://ct.panjiajie.cn

[H09] 带错误码的异常
来源：http://cg.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://oj.nicolike.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gv.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://aa.haigaiapp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qk.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zl.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://of.yuntaijiaju.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xc.newstarts.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://oo.bookmarksfly.cn

[H10] 资源自动释放
来源：http://nx.bjjhwx.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ke.bookmarksfly.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cj.haigaiapp.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tw.huanxung.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tv.nicolike.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sw.shtwfgs.cn

Go:   defer f.Close()
来源：http://ec.nicolike.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://og.panjiajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tj.nszjky.cn

================================================================================
来源：http://ao.szsharing.cn

I. 正则表达式
来源：http://id.bookmarksfly.cn

================================================================================
来源：http://ue.shtwfgs.cn

[I01] 判断是否匹配
来源：http://yx.szsharing.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gn.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zz.bookmarksfly.cn

JS:   /\d+/.test(s)
来源：http://yc.chemitech.net.cn

TS:   /\d+/.test(s)
来源：http://dn.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://uh.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://uw.wgjwhj.cn

Ruby: s.match?(/\d+/)
来源：http://de.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ep.shxzukj.cn

[I02] 提取所有匹配
来源：http://bk.9csxet.cn

Py:   re.findall(r"\d+", s)
来源：http://al.shtwfgs.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vh.szsharing.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://tm.colortex.cn

TS:   s.match(/\d+/g)
来源：http://kp.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://si.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mc.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://ft.haigaiapp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ow.lnxyls.cn

[I03] 提取捕获分组
来源：http://sb.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://xh.huixinmuqiang.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dm.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tb.yuntaijiaju.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wl.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://uz.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wr.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yt.asd995.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rk.colortex.cn

[I04] 正则替换
来源：http://wg.shxzukj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lb.huixinmuqiang.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hj.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qj.huanxung.cn

TS:   s.replace(/\d+/g, "#")
来源：http://nn.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pf.9csxet.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ua.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://gm.shtwfgs.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wj.huixinmuqiang.cn

[I05] 按正则拆分
来源：http://hn.huixiangedu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hk.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hf.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://bv.lnxyls.cn

TS:   s.split(/\s*,\s*/)
来源：http://re.shxzukj.cn

Java: s.split("\\s*,\\s*")
来源：http://tv.newstarts.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://na.shxzskj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bc.muxihuayi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cg.shxzskj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xq.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bj.nicolike.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zy.nicolike.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fy.muxihuayi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lo.chemitech.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sy.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xx.shxzukj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ab.yuntaijiaju.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fd.newstarts.cn

[I07] 忽略大小写与多行模式
来源：http://pe.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ib.szsharing.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zw.nicolike.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kz.shtwfgs.cn

TS:   /error/gim
来源：http://ar.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fd.bookmarksfly.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://dj.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://or.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xi.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://pm.yuexingan06.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://my.bjjhwx.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zm.panjiajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jd.yuntaijiaju.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://va.lnxyls.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ek.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zm.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://to.hnjuh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wu.muxihuayi.cn

================================================================================
来源：http://zo.huixinmuqiang.cn

J. 日期与时间
来源：http://dt.shxzskj.cn

================================================================================
来源：http://js.szsharing.cn

[J01] 获取当前时间
来源：http://ue.newstarts.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://as.shtwfgs.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bc.jianghongdianzi.cn

JS:   new Date();  Date.now()
来源：http://fm.jctech888.com.cn

TS:   new Date();  Date.now()
来源：http://mj.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gc.shxzskj.cn

Go:   time.Now()
来源：http://ec.szxytkj.cn

Ruby: Time.now
来源：http://fr.hahajie.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sf.szxytkj.cn

[J02] 格式化输出
来源：http://fe.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ls.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vi.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ld.muxihuayi.cn

TS:   d.toISOString()
来源：http://pw.asd995.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hm.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ai.shtwfgs.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xe.hnjuh.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zy.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://lw.jctech888.com.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://id.gzmigu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://he.szxytkj.cn

JS:   new Date("2024-01-02")
来源：http://zt.chemitech.net.cn

TS:   new Date("2024-01-02")
来源：http://qe.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cv.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://af.huixinmuqiang.cn

Ruby: Date.parse("2024-01-02")
来源：http://nt.nicolike.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vd.huanxung.cn

[J04] 时间戳与日期互转
来源：http://ie.jctech888.com.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://cd.521024.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sc.521024.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gz.hnjuh.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ul.yuntaijiaju.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nf.huixiangedu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://se.shtwfgs.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://eo.lnxyls.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nk.9csxet.cn

[J05] 时间加减（加 7 天）
来源：http://ji.huixiangedu.cn

Py:   now + timedelta(days=7)
来源：http://jt.bjjhwx.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://zw.muxihuayi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wd.jianghongdianzi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pm.asd995.cn

Java: LocalDate.now().plusDays(7)
来源：http://qi.yuntaijiaju.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vp.szsharing.cn

Ruby: Time.now + 7 * 86400
来源：http://nq.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gv.newstarts.cn

[J06] 计算两时间之差
来源：http://br.yuntaijiaju.cn

Py:   (end - start).total_seconds()
来源：http://dc.hahajie.cn

PHP:  $end->diff($start)->days;
来源：http://sm.jianghongdianzi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://or.jctech888.com.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jl.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ol.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://il.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://eu.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://vq.nszjky.cn

[J07] 比较两个日期
来源：http://ch.muxihuayi.cn

Py:   d1 < d2;  d1 == d2
来源：http://jv.jctech888.com.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rv.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ii.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kj.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ow.gzmigu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gh.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://oo.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://ze.huanxung.cn

[J08] 提取年月日与星期
来源：http://yv.colortex.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wg.gzmigu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zt.shxzukj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nf.panjiajie.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ax.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://fd.gzmigu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://sk.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ot.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ht.wgjwhj.cn

[J09] 时区处理
来源：http://ij.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sl.yuexingan06.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://az.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hv.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ix.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://av.haigaiapp.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xl.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://jm.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hi.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://mc.521024.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://uu.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bh.asd995.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qe.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wb.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://so.szsharing.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qo.bookmarksfly.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nd.yuexingan06.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mk.colortex.cn

================================================================================
来源：http://ro.jctech888.com.cn

K. JSON 与序列化
来源：http://hu.huixiangedu.cn

================================================================================
来源：http://hx.chemitech.net.cn

[K01] 对象转 JSON 字符串
来源：http://pp.haigaiapp.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mu.shtwfgs.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vq.szxytkj.cn

JS:   JSON.stringify(obj)
来源：http://rw.huanxung.cn

TS:   JSON.stringify(obj)
来源：http://xz.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://yq.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://jm.shxzskj.cn

Ruby: obj.to_json                                     // require "json"
来源：http://te.jctech888.com.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ft.nszjky.cn

[K02] JSON 字符串转对象
来源：http://vg.bjjhwx.cn

Py:   json.loads(s)
来源：http://ou.yuexingan06.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gg.asd995.cn

JS:   JSON.parse(s)
来源：http://op.jctech888.com.cn


<!-- 参考信息 -->