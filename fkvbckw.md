代发 wailian999

Java: u instanceof User
来源：http://ve.chemitech.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bg.panjiajie.cn

Ruby: u.is_a?(User)
来源：http://vk.szsharing.cn

C#:   u is User
来源：http://hy.521024.cn

[G14] 数据类 / record
来源：http://vv.hnjuh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hh.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://qc.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mj.yuexingan06.cn

TS:   type User = { name: string; age: number };
来源：http://lg.szsharing.cn

Java: record User(String name, int age) {}
来源：http://gy.chemitech.net.cn

Go:   type User struct { Name string; Age int }
来源：http://yo.hahajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gg.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://tt.shtwfgs.cn

[G15] 枚举
来源：http://vd.huanxung.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://le.newstarts.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://di.bjjhwx.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hn.hnjuh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://eb.bjjhwx.cn

Java: enum Color { RED, GREEN }
来源：http://by.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ug.shtwfgs.cn

Ruby: Color = %i[red green].freeze
来源：http://wy.9csxet.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hb.jianghongdianzi.cn

[G16] 对象转数组 / 字典
来源：http://qu.shxzskj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ma.panjiajie.cn

PHP:  get_object_vars($obj);
来源：http://xn.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://xb.szxytkj.cn

TS:   Object.entries(obj)
来源：http://ea.huixiangedu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xr.shtwfgs.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ue.muxihuayi.cn

Ruby: obj.instance_variables
来源：http://kv.jctech888.com.cn

C#:   // 用反射或 System.Text.Json
来源：http://kh.hahajie.cn

================================================================================
来源：http://py.gzmigu.cn

H. 异常与错误处理
来源：http://pd.huanxung.cn

================================================================================
来源：http://gx.muxihuayi.cn

[H01] try / catch 基础
来源：http://su.haigaiapp.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kd.asd995.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jn.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://co.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wb.wgjwhj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bk.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://pp.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://xf.huixinmuqiang.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ld.huanxung.cn

[H02] finally / ensure 收尾
来源：http://cu.bjjhwx.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gh.yuntaijiaju.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yd.szxytkj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://az.gzmigu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xb.shtwfgs.cn

Java: try { f(); } finally { cleanup(); }
来源：http://af.shxzukj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zi.asd995.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tc.huixiangedu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jt.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://lg.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://ws.asd995.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://me.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://sp.szxytkj.cn

TS:   throw new Error("错误信息");
来源：http://fw.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lz.chemitech.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ym.jctech888.com.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://lg.jianghongdianzi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gi.bjjhwx.cn

[H04] 自定义异常类型
来源：http://ha.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://dv.szsharing.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ne.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://sg.nszjky.cn

TS:   class MyError extends Error {}
来源：http://lu.shxzskj.cn

Java: class MyException extends RuntimeException {}
来源：http://ql.huixinmuqiang.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fm.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://bv.hahajie.cn

C#:   class MyException : Exception {}
来源：http://wb.bjjhwx.cn

[H05] 捕获特定类型
来源：http://fe.newstarts.cn

Py:   except ValueError as e:
来源：http://yu.huixiangedu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://te.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://ia.nicolike.cn

TS:   if (e instanceof TypeError) {}
来源：http://ji.hahajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://xc.hahajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fm.bjjhwx.cn

Ruby: rescue ArgumentError => e
来源：http://eh.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fy.panjiajie.cn

[H06] 可选值 / 空值安全访问
来源：http://gj.asd995.cn

Py:   value = d.get("k") or default
来源：http://pf.newstarts.cn

PHP:  $v = $d["k"] ?? null;
来源：http://gg.szsharing.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ah.wgjwhj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bd.wgjwhj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://yn.huixinmuqiang.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wv.shxzskj.cn

Ruby: d&.dig(:a, :b)
来源：http://vv.hahajie.cn

C#:   obj?.A?.B ?? default
来源：http://bo.521024.cn

[H07] 断言
来源：http://ur.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://cq.shtwfgs.cn

PHP:  assert($x > 0);
来源：http://aq.szsharing.cn

JS:   console.assert(x > 0);
来源：http://tk.lnxyls.cn

TS:   console.assert(x > 0);
来源：http://bu.asd995.cn

Java: assert x > 0 : "必须为正";
来源：http://hx.nicolike.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ih.yuexingan06.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ou.shxzukj.cn

C#:   Debug.Assert(x > 0);
来源：http://ax.gzmigu.cn

[H08] 获取错误信息与堆栈
来源：http://ek.jianghongdianzi.cn

Py:   str(e);  traceback.format_exc()
来源：http://kl.9csxet.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ej.szxytkj.cn

JS:   e.message;  e.stack
来源：http://ys.hahajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ai.huixinmuqiang.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://kh.nszjky.cn

Go:   err.Error()
来源：http://rf.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://ep.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://fz.521024.cn

[H09] 带错误码的异常
来源：http://ha.bookmarksfly.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sv.shtwfgs.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kz.521024.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ce.nicolike.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sa.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pr.nszjky.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hx.asd995.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mh.huixiangedu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://xl.haigaiapp.cn

[H10] 资源自动释放
来源：http://nr.muxihuayi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cv.jianghongdianzi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ra.hnjuh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qq.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://sg.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ar.lnxyls.cn

Go:   defer f.Close()
来源：http://ky.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ay.panjiajie.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zq.shxzskj.cn

================================================================================
来源：http://ii.colortex.cn

I. 正则表达式
来源：http://qp.chemitech.net.cn

================================================================================
来源：http://uw.haigaiapp.cn

[I01] 判断是否匹配
来源：http://cy.panjiajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jw.huixiangedu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://fj.jianghongdianzi.cn

JS:   /\d+/.test(s)
来源：http://gp.yuntaijiaju.cn

TS:   /\d+/.test(s)
来源：http://er.bjjhwx.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ov.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://vk.huixiangedu.cn

Ruby: s.match?(/\d+/)
来源：http://bn.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ni.haigaiapp.cn

[I02] 提取所有匹配
来源：http://my.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://yd.jctech888.com.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ho.newstarts.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zz.szsharing.cn

TS:   s.match(/\d+/g)
来源：http://fk.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://gv.hahajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ix.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://dt.newstarts.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sd.hnjuh.cn

[I03] 提取捕获分组
来源：http://rh.shtwfgs.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://qd.hnjuh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://js.huixinmuqiang.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kh.nicolike.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yp.nszjky.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oa.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vw.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://dy.jctech888.com.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gc.jctech888.com.cn

[I04] 正则替换
来源：http://va.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wz.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://gy.wgjwhj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ow.shtwfgs.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yo.jianghongdianzi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zc.nicolike.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tx.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://oe.asd995.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://il.haigaiapp.cn

[I05] 按正则拆分
来源：http://oe.szxytkj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fe.chemitech.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ve.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://ug.panjiajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://mw.lnxyls.cn

Java: s.split("\\s*,\\s*")
来源：http://oc.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ql.szsharing.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bg.huanxung.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xa.bjjhwx.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xr.hahajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hn.shtwfgs.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ql.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bw.jctech888.com.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rt.gzmigu.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://el.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://na.szsharing.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dc.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ek.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://xm.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://go.hnjuh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pl.newstarts.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ca.gzmigu.cn

TS:   /error/gim
来源：http://pf.lnxyls.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kg.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bk.jianghongdianzi.cn

Ruby: s.scan(/error/i)
来源：http://ef.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xj.nicolike.cn

[I08] 贪婪与非贪婪匹配
来源：http://sd.wgjwhj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hm.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://uu.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sb.lnxyls.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tg.colortex.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wg.bjjhwx.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vs.shxzukj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qw.wgjwhj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wu.bookmarksfly.cn

================================================================================
来源：http://yd.colortex.cn

J. 日期与时间
来源：http://wh.huixiangedu.cn

================================================================================
来源：http://xs.haigaiapp.cn

[J01] 获取当前时间
来源：http://mm.haigaiapp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rl.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ua.asd995.cn

JS:   new Date();  Date.now()
来源：http://mc.gzmigu.cn

TS:   new Date();  Date.now()
来源：http://tb.huanxung.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jj.wgjwhj.cn

Go:   time.Now()
来源：http://kd.huanxung.cn

Ruby: Time.now
来源：http://mc.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cl.newstarts.cn

[J02] 格式化输出
来源：http://aq.bookmarksfly.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qo.haigaiapp.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://oj.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zo.jianghongdianzi.cn

TS:   d.toISOString()
来源：http://vv.521024.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jh.nicolike.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ci.yuexingan06.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ss.chemitech.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://an.asd995.cn

[J03] 字符串解析为日期
来源：http://cw.jctech888.com.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wx.shxzskj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fx.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://qv.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://yr.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://cz.9csxet.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ap.hahajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://bn.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://px.jianghongdianzi.cn

[J04] 时间戳与日期互转
来源：http://tu.nszjky.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://bw.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ef.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://br.huixinmuqiang.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lj.hahajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ru.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bn.haigaiapp.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qh.9csxet.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://et.yuntaijiaju.cn

[J05] 时间加减（加 7 天）
来源：http://el.panjiajie.cn

Py:   now + timedelta(days=7)
来源：http://gv.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uk.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fm.huixiangedu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cm.panjiajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://wc.hahajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://nm.muxihuayi.cn

Ruby: Time.now + 7 * 86400
来源：http://hr.bookmarksfly.cn

C#:   DateTime.Now.AddDays(7)
来源：http://li.9csxet.cn

[J06] 计算两时间之差
来源：http://jo.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://ek.yuntaijiaju.cn

PHP:  $end->diff($start)->days;
来源：http://cz.yuntaijiaju.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://df.bookmarksfly.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://rt.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cl.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://ru.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://fe.bjjhwx.cn

C#:   (end - start).TotalSeconds
来源：http://nv.huixinmuqiang.cn

[J07] 比较两个日期
来源：http://av.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://mj.asd995.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ku.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://mf.shxzukj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xc.bjjhwx.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kh.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hw.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xa.yuntaijiaju.cn

C#:   d1 < d2;  d1 == d2
来源：http://hk.huanxung.cn

[J08] 提取年月日与星期
来源：http://qt.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://zj.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xv.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://uo.jianghongdianzi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://we.szxytkj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://be.newstarts.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kf.lnxyls.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tc.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fp.muxihuayi.cn

[J09] 时区处理
来源：http://nc.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yn.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jc.shtwfgs.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://nn.huanxung.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yp.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ee.muxihuayi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sp.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://se.haigaiapp.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ui.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://gg.bjjhwx.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://xk.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cj.yuexingan06.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://en.huixinmuqiang.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bx.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://il.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zp.newstarts.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ee.bjjhwx.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bo.huanxung.cn

================================================================================
来源：http://rv.jctech888.com.cn

K. JSON 与序列化
来源：http://ii.lnxyls.cn

================================================================================
来源：http://mt.huixinmuqiang.cn

[K01] 对象转 JSON 字符串
来源：http://do.muxihuayi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fb.szxytkj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uq.gzmigu.cn

JS:   JSON.stringify(obj)
来源：http://ub.shxzskj.cn

TS:   JSON.stringify(obj)
来源：http://ms.asd995.cn


<!-- 参考信息 -->