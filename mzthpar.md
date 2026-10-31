代发 wailian999

Java: u instanceof User
来源：http://hv.hahajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gh.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://ui.asd995.cn

C#:   u is User
来源：http://up.huanxung.cn

[G14] 数据类 / record
来源：http://vs.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kt.yuntaijiaju.cn

PHP:  // 用 readonly 属性模拟
来源：http://ut.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gt.hnjuh.cn

TS:   type User = { name: string; age: number };
来源：http://rz.nicolike.cn

Java: record User(String name, int age) {}
来源：http://pj.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://ni.nszjky.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://un.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://or.jctech888.com.cn

[G15] 枚举
来源：http://vp.szsharing.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tc.nicolike.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pu.hnjuh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hg.bjjhwx.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sx.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://qx.huanxung.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xs.yuexingan06.cn

Ruby: Color = %i[red green].freeze
来源：http://un.szxytkj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rz.newstarts.cn

[G16] 对象转数组 / 字典
来源：http://xt.szxytkj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://yz.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://qr.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://gr.newstarts.cn

TS:   Object.entries(obj)
来源：http://jw.hnjuh.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yh.newstarts.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://np.bjjhwx.cn

Ruby: obj.instance_variables
来源：http://uc.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://nf.wgjwhj.cn

================================================================================
来源：http://hs.521024.cn

H. 异常与错误处理
来源：http://fq.wgjwhj.cn

================================================================================
来源：http://an.shtwfgs.cn

[H01] try / catch 基础
来源：http://ae.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qm.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wm.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sc.hahajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://he.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xb.chemitech.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bp.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ng.szsharing.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://dk.huanxung.cn

[H02] finally / ensure 收尾
来源：http://dx.shtwfgs.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ce.nszjky.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wm.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zv.9csxet.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ei.jctech888.com.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zh.huixinmuqiang.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pr.gzmigu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kt.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://gq.shxzskj.cn

[H03] 主动抛出异常
来源：http://fs.shxzskj.cn

Py:   raise ValueError("错误信息")
来源：http://az.haigaiapp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jl.yuntaijiaju.cn

JS:   throw new Error("错误信息");
来源：http://kk.chemitech.net.cn

TS:   throw new Error("错误信息");
来源：http://so.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ne.nszjky.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yl.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jx.bjjhwx.cn

C#:   throw new ArgumentException("错误信息");
来源：http://os.muxihuayi.cn

[H04] 自定义异常类型
来源：http://ag.nszjky.cn

Py:   class MyError(Exception): pass
来源：http://tr.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rp.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://ht.newstarts.cn

TS:   class MyError extends Error {}
来源：http://kg.huanxung.cn

Java: class MyException extends RuntimeException {}
来源：http://dt.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gc.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://gr.huanxung.cn

C#:   class MyException : Exception {}
来源：http://nl.yuexingan06.cn

[H05] 捕获特定类型
来源：http://lx.nicolike.cn

Py:   except ValueError as e:
来源：http://ni.shxzukj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wu.gzmigu.cn

JS:   if (e instanceof TypeError) {}
来源：http://mq.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://kv.nicolike.cn

Java: catch (IOException | SQLException e) {}
来源：http://nu.nicolike.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hf.haigaiapp.cn

Ruby: rescue ArgumentError => e
来源：http://in.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://of.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://qg.yuexingan06.cn

Py:   value = d.get("k") or default
来源：http://qf.hnjuh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://my.nszjky.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dt.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ep.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ec.hnjuh.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dq.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://fh.huixiangedu.cn

C#:   obj?.A?.B ?? default
来源：http://ox.huixiangedu.cn

[H07] 断言
来源：http://zi.szsharing.cn

Py:   assert x > 0, "必须为正"
来源：http://am.9csxet.cn

PHP:  assert($x > 0);
来源：http://rf.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://ag.gzmigu.cn

TS:   console.assert(x > 0);
来源：http://gj.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://qr.lnxyls.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://yj.szxytkj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ut.yuntaijiaju.cn

C#:   Debug.Assert(x > 0);
来源：http://hm.panjiajie.cn

[H08] 获取错误信息与堆栈
来源：http://ot.nszjky.cn

Py:   str(e);  traceback.format_exc()
来源：http://cu.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://li.haigaiapp.cn

JS:   e.message;  e.stack
来源：http://mf.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ha.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yn.szsharing.cn

Go:   err.Error()
来源：http://sk.haigaiapp.cn

Ruby: e.message;  e.backtrace
来源：http://zk.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://wv.colortex.cn

[H09] 带错误码的异常
来源：http://sc.szxytkj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wj.9csxet.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ld.yuexingan06.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cj.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nq.shtwfgs.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://eq.bjjhwx.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://xm.colortex.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ot.muxihuayi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gn.asd995.cn

[H10] 资源自动释放
来源：http://hi.hnjuh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://or.bjjhwx.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gc.shxzskj.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rg.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://is.shxzskj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://gr.newstarts.cn

Go:   defer f.Close()
来源：http://ov.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://iu.nicolike.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ax.newstarts.cn

================================================================================
来源：http://if.szxytkj.cn

I. 正则表达式
来源：http://wk.colortex.cn

================================================================================
来源：http://gm.muxihuayi.cn

[I01] 判断是否匹配
来源：http://ru.9csxet.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mz.haigaiapp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://to.jctech888.com.cn

JS:   /\d+/.test(s)
来源：http://gg.huanxung.cn

TS:   /\d+/.test(s)
来源：http://bq.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://id.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://be.wgjwhj.cn

Ruby: s.match?(/\d+/)
来源：http://uj.newstarts.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://kc.bookmarksfly.cn

[I02] 提取所有匹配
来源：http://ts.shxzukj.cn

Py:   re.findall(r"\d+", s)
来源：http://re.szsharing.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pu.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ep.huixinmuqiang.cn

TS:   s.match(/\d+/g)
来源：http://ad.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bt.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ml.haigaiapp.cn

Ruby: s.scan(/\d+/)
来源：http://xk.huixiangedu.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://te.huanxung.cn

[I03] 提取捕获分组
来源：http://on.nicolike.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ma.521024.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xb.chemitech.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wi.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://tr.huixiangedu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ko.panjiajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bb.huixinmuqiang.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cm.9csxet.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xb.bjjhwx.cn

[I04] 正则替换
来源：http://it.huixinmuqiang.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lw.asd995.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://vg.yuexingan06.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kb.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ar.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fl.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dk.hnjuh.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vw.bookmarksfly.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rz.panjiajie.cn

[I05] 按正则拆分
来源：http://mu.huixinmuqiang.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sq.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lb.yuexingan06.cn

JS:   s.split(/\s*,\s*/)
来源：http://ym.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://ik.szsharing.cn

Java: s.split("\\s*,\\s*")
来源：http://cp.hahajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ky.yuexingan06.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ky.yuntaijiaju.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zh.nszjky.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ws.wgjwhj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bz.asd995.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gn.asd995.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gr.chemitech.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nv.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ka.szsharing.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jz.521024.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://bd.panjiajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mm.yuntaijiaju.cn

[I07] 忽略大小写与多行模式
来源：http://wu.yuntaijiaju.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lo.haigaiapp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mw.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cw.wgjwhj.cn

TS:   /error/gim
来源：http://cr.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mh.9csxet.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hu.521024.cn

Ruby: s.scan(/error/i)
来源：http://yt.szxytkj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qp.bjjhwx.cn

[I08] 贪婪与非贪婪匹配
来源：http://ic.panjiajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dw.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pg.panjiajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://iu.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sw.hahajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://un.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://er.huixiangedu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://oj.hahajie.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gd.yuexingan06.cn

================================================================================
来源：http://zw.colortex.cn

J. 日期与时间
来源：http://iv.shxzukj.cn

================================================================================
来源：http://aj.9csxet.cn

[J01] 获取当前时间
来源：http://bb.panjiajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://eq.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wv.shxzukj.cn

JS:   new Date();  Date.now()
来源：http://mj.bookmarksfly.cn

TS:   new Date();  Date.now()
来源：http://vw.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ec.jianghongdianzi.cn

Go:   time.Now()
来源：http://aj.yuntaijiaju.cn

Ruby: Time.now
来源：http://gk.jctech888.com.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://bz.jctech888.com.cn

[J02] 格式化输出
来源：http://sd.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://az.bjjhwx.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hg.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yq.huixiangedu.cn

TS:   d.toISOString()
来源：http://mm.521024.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://xh.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://qc.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hi.gzmigu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cf.muxihuayi.cn

[J03] 字符串解析为日期
来源：http://dk.lnxyls.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nd.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lv.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://xy.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://er.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wd.wgjwhj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uy.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://ha.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://mg.chemitech.net.cn

[J04] 时间戳与日期互转
来源：http://tb.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gs.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://an.jianghongdianzi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://io.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mc.yuntaijiaju.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://js.bookmarksfly.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ls.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zt.9csxet.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xn.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://zh.yuntaijiaju.cn

Py:   now + timedelta(days=7)
来源：http://lf.shxzskj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lo.huixiangedu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://au.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qd.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://xg.panjiajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yq.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://rp.huixiangedu.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dv.nszjky.cn

[J06] 计算两时间之差
来源：http://ee.newstarts.cn

Py:   (end - start).total_seconds()
来源：http://gs.yuntaijiaju.cn

PHP:  $end->diff($start)->days;
来源：http://ot.muxihuayi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cg.9csxet.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tw.shxzskj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dw.shtwfgs.cn

Go:   end.Sub(start).Hours()
来源：http://of.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://uh.hahajie.cn

C#:   (end - start).TotalSeconds
来源：http://jh.shtwfgs.cn

[J07] 比较两个日期
来源：http://tf.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://ie.shtwfgs.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://lw.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cb.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yr.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://al.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ci.szsharing.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fn.yuexingan06.cn

C#:   d1 < d2;  d1 == d2
来源：http://jy.shxzskj.cn

[J08] 提取年月日与星期
来源：http://pl.bookmarksfly.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tg.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mx.huixinmuqiang.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hn.521024.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pi.nicolike.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ce.asd995.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tj.lnxyls.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ki.colortex.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qm.bookmarksfly.cn

[J09] 时区处理
来源：http://nm.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qk.shtwfgs.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ot.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sp.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gs.huixiangedu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://el.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://br.szxytkj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://bv.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vg.hnjuh.cn

[J10] 取今天 / 本月第一天
来源：http://sj.shxzskj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qj.hahajie.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ws.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ia.yuexingan06.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://am.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xa.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qf.hahajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nx.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://we.shtwfgs.cn

================================================================================
来源：http://og.shxzukj.cn

K. JSON 与序列化
来源：http://ff.colortex.cn

================================================================================
来源：http://ny.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://qg.9csxet.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zo.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ok.bookmarksfly.cn

JS:   JSON.stringify(obj)
来源：http://bd.wgjwhj.cn

TS:   JSON.stringify(obj)
来源：http://bu.szxytkj.cn


<!-- 参考信息 -->