代发 wailian999

Py:   isinstance(u, User)
来源：http://ok.shxzukj.cn

PHP:  $u instanceof User
来源：http://hw.shxzskj.cn

JS:   u instanceof User
来源：http://vm.yuexingan06.cn

TS:   u instanceof User
来源：http://uo.chemitech.net.cn

Java: u instanceof User
来源：http://it.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gk.hahajie.cn

Ruby: u.is_a?(User)
来源：http://xz.bookmarksfly.cn

C#:   u is User
来源：http://mz.jctech888.com.cn

[G14] 数据类 / record
来源：http://go.asd995.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xo.huixinmuqiang.cn

PHP:  // 用 readonly 属性模拟
来源：http://jh.huanxung.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tw.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://fw.haigaiapp.cn

Java: record User(String name, int age) {}
来源：http://xh.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://ce.yuntaijiaju.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://lg.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://gd.bookmarksfly.cn

[G15] 枚举
来源：http://ib.lnxyls.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gv.bookmarksfly.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://re.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://la.newstarts.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://fg.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://bi.newstarts.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ef.shxzskj.cn

Ruby: Color = %i[red green].freeze
来源：http://fv.haigaiapp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sc.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://ln.panjiajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fu.shtwfgs.cn

PHP:  get_object_vars($obj);
来源：http://sb.shtwfgs.cn

JS:   Object.entries(obj)
来源：http://ag.panjiajie.cn

TS:   Object.entries(obj)
来源：http://wh.shtwfgs.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://jz.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gn.shtwfgs.cn

Ruby: obj.instance_variables
来源：http://ix.panjiajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://di.nszjky.cn

================================================================================
来源：http://gw.szxytkj.cn

H. 异常与错误处理
来源：http://vh.9csxet.cn

================================================================================
来源：http://rc.yuntaijiaju.cn

[H01] try / catch 基础
来源：http://iu.lnxyls.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sp.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zb.shtwfgs.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://uk.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ex.jctech888.com.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fl.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uj.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qr.haigaiapp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://am.chemitech.net.cn

[H02] finally / ensure 收尾
来源：http://wv.shtwfgs.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qf.nicolike.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://my.huixinmuqiang.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://lh.szxytkj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zg.szxytkj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qv.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mo.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://td.colortex.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vk.wgjwhj.cn

[H03] 主动抛出异常
来源：http://ce.hahajie.cn

Py:   raise ValueError("错误信息")
来源：http://wr.hahajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nd.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://oj.hahajie.cn

TS:   throw new Error("错误信息");
来源：http://to.szxytkj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://eh.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://yy.panjiajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rn.lnxyls.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rm.bjjhwx.cn

[H04] 自定义异常类型
来源：http://jp.yuntaijiaju.cn

Py:   class MyError(Exception): pass
来源：http://sq.shxzukj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ju.hahajie.cn

JS:   class MyError extends Error {}
来源：http://cq.muxihuayi.cn

TS:   class MyError extends Error {}
来源：http://ir.521024.cn

Java: class MyException extends RuntimeException {}
来源：http://kw.shxzskj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ct.bookmarksfly.cn

Ruby: class MyError < StandardError; end
来源：http://bi.yuexingan06.cn

C#:   class MyException : Exception {}
来源：http://wc.muxihuayi.cn

[H05] 捕获特定类型
来源：http://cv.panjiajie.cn

Py:   except ValueError as e:
来源：http://xf.jianghongdianzi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ab.panjiajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://lt.haigaiapp.cn

TS:   if (e instanceof TypeError) {}
来源：http://xv.panjiajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://wo.shtwfgs.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vk.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://ne.huixinmuqiang.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wk.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://lr.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://os.521024.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bm.bookmarksfly.cn

JS:   obj?.a?.b;  d ?? default
来源：http://dy.jctech888.com.cn

TS:   obj?.a?.b;  d ?? default
来源：http://oy.521024.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dx.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bl.huixiangedu.cn

Ruby: d&.dig(:a, :b)
来源：http://xc.chemitech.net.cn

C#:   obj?.A?.B ?? default
来源：http://dn.wgjwhj.cn

[H07] 断言
来源：http://os.hnjuh.cn

Py:   assert x > 0, "必须为正"
来源：http://oo.521024.cn

PHP:  assert($x > 0);
来源：http://il.yuexingan06.cn

JS:   console.assert(x > 0);
来源：http://lv.szxytkj.cn

TS:   console.assert(x > 0);
来源：http://fi.yuntaijiaju.cn

Java: assert x > 0 : "必须为正";
来源：http://oi.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ii.szxytkj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mc.bookmarksfly.cn

C#:   Debug.Assert(x > 0);
来源：http://pd.jianghongdianzi.cn

[H08] 获取错误信息与堆栈
来源：http://au.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://xd.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wu.521024.cn

JS:   e.message;  e.stack
来源：http://zl.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://cb.bookmarksfly.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zx.hahajie.cn

Go:   err.Error()
来源：http://fx.hnjuh.cn

Ruby: e.message;  e.backtrace
来源：http://el.nszjky.cn

C#:   e.Message;  e.StackTrace
来源：http://iu.jctech888.com.cn

[H09] 带错误码的异常
来源：http://mj.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://le.chemitech.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ti.wgjwhj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ho.panjiajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wp.nicolike.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dq.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qv.gzmigu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ix.bjjhwx.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ss.chemitech.net.cn

[H10] 资源自动释放
来源：http://nu.yuexingan06.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kl.chemitech.net.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fv.jctech888.com.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ky.szsharing.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ip.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://rw.huanxung.cn

Go:   defer f.Close()
来源：http://cp.wgjwhj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mm.jctech888.com.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ox.huixiangedu.cn

================================================================================
来源：http://ck.wgjwhj.cn

I. 正则表达式
来源：http://bt.shxzukj.cn

================================================================================
来源：http://nu.nicolike.cn

[I01] 判断是否匹配
来源：http://bd.wgjwhj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://el.shtwfgs.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qk.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://xc.shtwfgs.cn

TS:   /\d+/.test(s)
来源：http://pv.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ju.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vy.asd995.cn

Ruby: s.match?(/\d+/)
来源：http://fv.jctech888.com.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hr.521024.cn

[I02] 提取所有匹配
来源：http://jt.jctech888.com.cn

Py:   re.findall(r"\d+", s)
来源：http://za.nicolike.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wi.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eo.shxzskj.cn

TS:   s.match(/\d+/g)
来源：http://ib.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://om.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://am.wgjwhj.cn

Ruby: s.scan(/\d+/)
来源：http://so.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://jx.muxihuayi.cn

[I03] 提取捕获分组
来源：http://zh.wgjwhj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nc.521024.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ug.newstarts.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://my.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sj.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wf.muxihuayi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kx.521024.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ta.bookmarksfly.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nc.jianghongdianzi.cn

[I04] 正则替换
来源：http://ji.huanxung.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://qx.shxzskj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qq.yuntaijiaju.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xs.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qv.panjiajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ck.shtwfgs.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tq.panjiajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://io.muxihuayi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wh.huixinmuqiang.cn

[I05] 按正则拆分
来源：http://hm.panjiajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pi.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jd.panjiajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://hz.muxihuayi.cn

TS:   s.split(/\s*,\s*/)
来源：http://cx.hnjuh.cn

Java: s.split("\\s*,\\s*")
来源：http://hv.9csxet.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gk.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://gy.521024.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oy.huanxung.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://am.huanxung.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fl.asd995.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rx.muxihuayi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qr.bookmarksfly.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vy.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://kw.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://so.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gc.521024.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wd.shxzukj.cn

[I07] 忽略大小写与多行模式
来源：http://ra.muxihuayi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qa.szxytkj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ln.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vr.9csxet.cn

TS:   /error/gim
来源：http://zj.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zv.bjjhwx.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ea.chemitech.net.cn

Ruby: s.scan(/error/i)
来源：http://td.shxzukj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pl.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://iz.chemitech.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fy.asd995.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://us.jianghongdianzi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ng.bookmarksfly.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ab.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lt.nszjky.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.huixinmuqiang.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ek.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://np.muxihuayi.cn

================================================================================
来源：http://wv.lnxyls.cn

J. 日期与时间
来源：http://xp.gzmigu.cn

================================================================================
来源：http://pd.hahajie.cn

[J01] 获取当前时间
来源：http://kj.panjiajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ds.shtwfgs.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bt.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://oe.9csxet.cn

TS:   new Date();  Date.now()
来源：http://kh.newstarts.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vo.yuexingan06.cn

Go:   time.Now()
来源：http://kf.muxihuayi.cn

Ruby: Time.now
来源：http://ba.9csxet.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ch.newstarts.cn

[J02] 格式化输出
来源：http://bi.colortex.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xj.nicolike.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qs.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://qv.wgjwhj.cn

TS:   d.toISOString()
来源：http://yr.huixinmuqiang.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fd.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fd.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ii.jianghongdianzi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kh.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://rc.panjiajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://xf.chemitech.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://wu.panjiajie.cn

JS:   new Date("2024-01-02")
来源：http://iz.shxzukj.cn

TS:   new Date("2024-01-02")
来源：http://xf.szxytkj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fb.szsharing.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uy.gzmigu.cn

Ruby: Date.parse("2024-01-02")
来源：http://zi.bookmarksfly.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xn.chemitech.net.cn

[J04] 时间戳与日期互转
来源：http://ty.huixinmuqiang.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://es.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://li.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://pj.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://el.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rq.newstarts.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://in.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ai.huixinmuqiang.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uo.muxihuayi.cn

[J05] 时间加减（加 7 天）
来源：http://zy.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://lb.huixiangedu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ns.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://au.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://lw.asd995.cn

Java: LocalDate.now().plusDays(7)
来源：http://sn.wgjwhj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://dy.521024.cn

Ruby: Time.now + 7 * 86400
来源：http://iq.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ed.asd995.cn

[J06] 计算两时间之差
来源：http://hp.huanxung.cn

Py:   (end - start).total_seconds()
来源：http://zb.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://js.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zq.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sl.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://oj.wgjwhj.cn

Go:   end.Sub(start).Hours()
来源：http://id.huixinmuqiang.cn

Ruby: end - start                 # 返回秒数
来源：http://nk.huanxung.cn

C#:   (end - start).TotalSeconds
来源：http://bs.huanxung.cn

[J07] 比较两个日期
来源：http://gh.asd995.cn

Py:   d1 < d2;  d1 == d2
来源：http://vv.panjiajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gk.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ml.panjiajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cy.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ql.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://va.hnjuh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zc.newstarts.cn

C#:   d1 < d2;  d1 == d2
来源：http://yl.chemitech.net.cn

[J08] 提取年月日与星期
来源：http://sq.hahajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://kk.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://td.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://jt.chemitech.net.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dd.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ec.muxihuayi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://vl.newstarts.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mr.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vq.9csxet.cn

[J09] 时区处理
来源：http://tn.hnjuh.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ev.muxihuayi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://an.nicolike.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kh.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cg.hnjuh.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fn.szxytkj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://td.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zq.muxihuayi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jd.wgjwhj.cn

[J10] 取今天 / 本月第一天
来源：http://ib.jianghongdianzi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://gp.gzmigu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sz.muxihuayi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://tc.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://tp.jctech888.com.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pv.huanxung.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qr.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ds.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qx.haigaiapp.cn

================================================================================
来源：http://rt.colortex.cn

K. JSON 与序列化
来源：http://nc.shxzskj.cn

================================================================================
来源：http://re.huixinmuqiang.cn

[K01] 对象转 JSON 字符串
来源：http://df.huanxung.cn


<!-- 参考信息 -->