代发 wailian999

Java: u instanceof User
来源：http://zp.nszjky.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ni.chemitech.net.cn

Ruby: u.is_a?(User)
来源：http://mo.chemitech.net.cn

C#:   u is User
来源：http://hr.yuexingan06.cn

[G14] 数据类 / record
来源：http://ax.huixinmuqiang.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bi.lnxyls.cn

PHP:  // 用 readonly 属性模拟
来源：http://aj.yuntaijiaju.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ow.shxzukj.cn

TS:   type User = { name: string; age: number };
来源：http://ve.newstarts.cn

Java: record User(String name, int age) {}
来源：http://bn.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://du.szxytkj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ax.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://ca.9csxet.cn

[G15] 枚举
来源：http://ho.9csxet.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oa.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ph.chemitech.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wk.nszjky.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xz.colortex.cn

Java: enum Color { RED, GREEN }
来源：http://cf.huanxung.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ow.muxihuayi.cn

Ruby: Color = %i[red green].freeze
来源：http://pd.bookmarksfly.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dj.521024.cn

[G16] 对象转数组 / 字典
来源：http://hy.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vw.nszjky.cn

PHP:  get_object_vars($obj);
来源：http://uh.huanxung.cn

JS:   Object.entries(obj)
来源：http://mm.muxihuayi.cn

TS:   Object.entries(obj)
来源：http://er.hnjuh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jf.521024.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gz.szsharing.cn

Ruby: obj.instance_variables
来源：http://va.521024.cn

C#:   // 用反射或 System.Text.Json
来源：http://kb.yuexingan06.cn

================================================================================
来源：http://bm.huixiangedu.cn

H. 异常与错误处理
来源：http://ja.hahajie.cn

================================================================================
来源：http://ro.shtwfgs.cn

[H01] try / catch 基础
来源：http://mt.huixiangedu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ea.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://je.gzmigu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ww.chemitech.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cq.shtwfgs.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qn.9csxet.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zb.yuexingan06.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zy.gzmigu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://js.asd995.cn

[H02] finally / ensure 收尾
来源：http://du.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://di.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://uv.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://va.bjjhwx.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nj.shxzskj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vp.hahajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.panjiajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cd.nicolike.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rs.nszjky.cn

[H03] 主动抛出异常
来源：http://uo.yuexingan06.cn

Py:   raise ValueError("错误信息")
来源：http://yk.bookmarksfly.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oo.colortex.cn

JS:   throw new Error("错误信息");
来源：http://ox.colortex.cn

TS:   throw new Error("错误信息");
来源：http://vl.hahajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://oq.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kx.yuntaijiaju.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mq.chemitech.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://az.9csxet.cn

[H04] 自定义异常类型
来源：http://jm.szsharing.cn

Py:   class MyError(Exception): pass
来源：http://wi.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dj.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://jx.shtwfgs.cn

TS:   class MyError extends Error {}
来源：http://rl.hnjuh.cn

Java: class MyException extends RuntimeException {}
来源：http://kw.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jt.haigaiapp.cn

Ruby: class MyError < StandardError; end
来源：http://jz.yuexingan06.cn

C#:   class MyException : Exception {}
来源：http://xh.shxzskj.cn

[H05] 捕获特定类型
来源：http://aw.panjiajie.cn

Py:   except ValueError as e:
来源：http://tm.szxytkj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xf.shtwfgs.cn

JS:   if (e instanceof TypeError) {}
来源：http://mu.panjiajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://ox.asd995.cn

Java: catch (IOException | SQLException e) {}
来源：http://ee.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hq.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://ue.colortex.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://df.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://wm.asd995.cn

Py:   value = d.get("k") or default
来源：http://wo.9csxet.cn

PHP:  $v = $d["k"] ?? null;
来源：http://sg.hahajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zf.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://il.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://si.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://jv.haigaiapp.cn

Ruby: d&.dig(:a, :b)
来源：http://nw.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://wd.9csxet.cn

[H07] 断言
来源：http://wy.huixiangedu.cn

Py:   assert x > 0, "必须为正"
来源：http://ex.yuntaijiaju.cn

PHP:  assert($x > 0);
来源：http://mi.shxzukj.cn

JS:   console.assert(x > 0);
来源：http://oo.nszjky.cn

TS:   console.assert(x > 0);
来源：http://cx.huixinmuqiang.cn

Java: assert x > 0 : "必须为正";
来源：http://ji.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gy.nicolike.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ve.haigaiapp.cn

C#:   Debug.Assert(x > 0);
来源：http://up.shtwfgs.cn

[H08] 获取错误信息与堆栈
来源：http://av.muxihuayi.cn

Py:   str(e);  traceback.format_exc()
来源：http://el.muxihuayi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rc.szxytkj.cn

JS:   e.message;  e.stack
来源：http://xm.jianghongdianzi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qe.jianghongdianzi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zc.shtwfgs.cn

Go:   err.Error()
来源：http://xm.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://im.huixiangedu.cn

C#:   e.Message;  e.StackTrace
来源：http://fk.shtwfgs.cn

[H09] 带错误码的异常
来源：http://tf.panjiajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xl.yuexingan06.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://cz.wgjwhj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ok.colortex.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://kl.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yd.haigaiapp.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ez.huanxung.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xy.hahajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kt.asd995.cn

[H10] 资源自动释放
来源：http://mg.szxytkj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vr.nszjky.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://no.hahajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ob.yuntaijiaju.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yo.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://xy.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://at.jianghongdianzi.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pu.nicolike.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zs.huanxung.cn

================================================================================
来源：http://kg.bjjhwx.cn

I. 正则表达式
来源：http://gz.yuexingan06.cn

================================================================================
来源：http://vt.nszjky.cn

[I01] 判断是否匹配
来源：http://fd.nszjky.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://en.shtwfgs.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sa.asd995.cn

JS:   /\d+/.test(s)
来源：http://pb.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://te.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ue.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pa.newstarts.cn

Ruby: s.match?(/\d+/)
来源：http://zn.9csxet.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qc.huixiangedu.cn

[I02] 提取所有匹配
来源：http://fa.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://da.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://eh.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://jq.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://uf.bookmarksfly.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://oh.9csxet.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://xn.newstarts.cn

Ruby: s.scan(/\d+/)
来源：http://bg.yuexingan06.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gb.yuexingan06.cn

[I03] 提取捕获分组
来源：http://um.shxzskj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://eu.bjjhwx.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ot.bookmarksfly.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bq.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gf.nszjky.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://no.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ev.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bj.521024.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rb.yuntaijiaju.cn

[I04] 正则替换
来源：http://cs.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://yp.szxytkj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://nj.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gb.huixiangedu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tu.huixiangedu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fk.bookmarksfly.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://eq.hnjuh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://nr.newstarts.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://cw.huixiangedu.cn

[I05] 按正则拆分
来源：http://aq.nszjky.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ws.huixiangedu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ad.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://yz.newstarts.cn

TS:   s.split(/\s*,\s*/)
来源：http://sj.chemitech.net.cn

Java: s.split("\\s*,\\s*")
来源：http://gf.asd995.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://eh.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://kh.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cc.yuexingan06.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jl.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qa.panjiajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vr.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zl.panjiajie.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sf.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ca.jctech888.com.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://iz.521024.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ym.lnxyls.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sk.hahajie.cn

[I07] 忽略大小写与多行模式
来源：http://kj.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jq.shtwfgs.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ya.yuexingan06.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ul.hahajie.cn

TS:   /error/gim
来源：http://ts.colortex.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ae.shxzukj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zk.hahajie.cn

Ruby: s.scan(/error/i)
来源：http://fw.newstarts.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ro.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://gp.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ms.bjjhwx.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://la.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lq.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tj.nicolike.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://aq.bjjhwx.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nm.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ii.gzmigu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ug.nicolike.cn

================================================================================
来源：http://oo.shxzskj.cn

J. 日期与时间
来源：http://ci.jianghongdianzi.cn

================================================================================
来源：http://kw.newstarts.cn

[J01] 获取当前时间
来源：http://vb.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wd.szsharing.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uu.shtwfgs.cn

JS:   new Date();  Date.now()
来源：http://ei.haigaiapp.cn

TS:   new Date();  Date.now()
来源：http://un.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://eu.newstarts.cn

Go:   time.Now()
来源：http://gs.yuexingan06.cn

Ruby: Time.now
来源：http://hf.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ud.nszjky.cn

[J02] 格式化输出
来源：http://ji.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yd.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://bq.yuntaijiaju.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://oi.521024.cn

TS:   d.toISOString()
来源：http://ir.bjjhwx.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://km.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jv.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nh.huixiangedu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yb.haigaiapp.cn

[J03] 字符串解析为日期
来源：http://lk.lnxyls.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tw.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wu.jianghongdianzi.cn

JS:   new Date("2024-01-02")
来源：http://uk.yuexingan06.cn

TS:   new Date("2024-01-02")
来源：http://iu.yuexingan06.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bu.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tg.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://zx.chemitech.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qt.nicolike.cn

[J04] 时间戳与日期互转
来源：http://vp.521024.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://aw.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://qf.nszjky.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://df.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zr.gzmigu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://cm.jianghongdianzi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://md.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://jl.lnxyls.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://km.bookmarksfly.cn

[J05] 时间加减（加 7 天）
来源：http://rg.hnjuh.cn

Py:   now + timedelta(days=7)
来源：http://td.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nu.asd995.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ul.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vu.muxihuayi.cn

Java: LocalDate.now().plusDays(7)
来源：http://fi.bjjhwx.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://rm.hahajie.cn

Ruby: Time.now + 7 * 86400
来源：http://of.shxzskj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dd.asd995.cn

[J06] 计算两时间之差
来源：http://zy.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://fe.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://lj.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jb.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://li.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://oq.jianghongdianzi.cn

Go:   end.Sub(start).Hours()
来源：http://lo.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://fc.chemitech.net.cn

C#:   (end - start).TotalSeconds
来源：http://wm.jianghongdianzi.cn

[J07] 比较两个日期
来源：http://xm.bjjhwx.cn

Py:   d1 < d2;  d1 == d2
来源：http://mk.nicolike.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yb.shxzskj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mi.chemitech.net.cn

TS:   d1.getTime() < d2.getTime()
来源：http://si.hahajie.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cu.521024.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qx.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wq.newstarts.cn

C#:   d1 < d2;  d1 == d2
来源：http://yz.gzmigu.cn

[J08] 提取年月日与星期
来源：http://el.nszjky.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://dv.shxzukj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fw.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tm.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mh.bookmarksfly.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gk.szxytkj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ar.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yx.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://og.nicolike.cn

[J09] 时区处理
来源：http://pv.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://af.yuntaijiaju.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gu.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lb.521024.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bm.szsharing.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sd.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bc.jianghongdianzi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://gp.hnjuh.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fi.panjiajie.cn

[J10] 取今天 / 本月第一天
来源：http://fo.newstarts.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qq.chemitech.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mh.huixiangedu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yc.jianghongdianzi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kz.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://of.szxytkj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://di.muxihuayi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://we.huixinmuqiang.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://if.hahajie.cn

================================================================================
来源：http://mh.shtwfgs.cn

K. JSON 与序列化
来源：http://qe.hahajie.cn

================================================================================
来源：http://ld.huixinmuqiang.cn

[K01] 对象转 JSON 字符串
来源：http://iy.shxzskj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://no.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dz.newstarts.cn

JS:   JSON.stringify(obj)
来源：http://tz.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://ij.huixinmuqiang.cn


<!-- 参考信息 -->