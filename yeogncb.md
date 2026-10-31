代发 wailian999

[G14] 数据类 / record
来源：http://wx.lnxyls.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://un.521024.cn

PHP:  // 用 readonly 属性模拟
来源：http://lx.haigaiapp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://lr.lnxyls.cn

TS:   type User = { name: string; age: number };
来源：http://et.shxzskj.cn

Java: record User(String name, int age) {}
来源：http://tn.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://sl.hnjuh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vj.haigaiapp.cn

C#:   record User(string Name, int Age);
来源：http://ex.asd995.cn

[G15] 枚举
来源：http://fy.hnjuh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cx.bjjhwx.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jb.nicolike.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bj.szsharing.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mm.521024.cn

Java: enum Color { RED, GREEN }
来源：http://ap.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fx.bjjhwx.cn

Ruby: Color = %i[red green].freeze
来源：http://ed.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ml.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://ej.nszjky.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ao.jctech888.com.cn

PHP:  get_object_vars($obj);
来源：http://pz.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://fu.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://fo.huanxung.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qd.szsharing.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ne.9csxet.cn

Ruby: obj.instance_variables
来源：http://dk.panjiajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://qo.521024.cn

================================================================================
来源：http://nn.huixinmuqiang.cn

H. 异常与错误处理
来源：http://jz.nicolike.cn

================================================================================
来源：http://ab.9csxet.cn

[H01] try / catch 基础
来源：http://wp.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://di.hnjuh.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://vb.haigaiapp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jh.muxihuayi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://da.shtwfgs.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://cm.shxzskj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ip.hahajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ns.gzmigu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fj.huixinmuqiang.cn

[H02] finally / ensure 收尾
来源：http://hl.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jg.muxihuayi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qn.szxytkj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vj.hahajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fe.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lj.521024.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vj.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dm.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wr.shtwfgs.cn

[H03] 主动抛出异常
来源：http://sl.muxihuayi.cn

Py:   raise ValueError("错误信息")
来源：http://kg.yuntaijiaju.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://oc.hnjuh.cn

JS:   throw new Error("错误信息");
来源：http://eq.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://mk.wgjwhj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nh.huixinmuqiang.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jn.gzmigu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://pq.muxihuayi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tv.asd995.cn

[H04] 自定义异常类型
来源：http://hg.shxzukj.cn

Py:   class MyError(Exception): pass
来源：http://nf.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bm.huanxung.cn

JS:   class MyError extends Error {}
来源：http://us.wgjwhj.cn

TS:   class MyError extends Error {}
来源：http://oi.nszjky.cn

Java: class MyException extends RuntimeException {}
来源：http://zx.hnjuh.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nq.wgjwhj.cn

Ruby: class MyError < StandardError; end
来源：http://on.nszjky.cn

C#:   class MyException : Exception {}
来源：http://ql.szsharing.cn

[H05] 捕获特定类型
来源：http://tr.huixinmuqiang.cn

Py:   except ValueError as e:
来源：http://hx.panjiajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gc.muxihuayi.cn

JS:   if (e instanceof TypeError) {}
来源：http://yc.colortex.cn

TS:   if (e instanceof TypeError) {}
来源：http://ur.jctech888.com.cn

Java: catch (IOException | SQLException e) {}
来源：http://kc.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ti.shxzukj.cn

Ruby: rescue ArgumentError => e
来源：http://iw.huixiangedu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vz.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://ox.muxihuayi.cn

Py:   value = d.get("k") or default
来源：http://ls.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yi.bjjhwx.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xp.szxytkj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ev.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wb.szsharing.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xu.hahajie.cn

Ruby: d&.dig(:a, :b)
来源：http://lx.yuntaijiaju.cn

C#:   obj?.A?.B ?? default
来源：http://zv.huixinmuqiang.cn

[H07] 断言
来源：http://qt.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://hn.huixiangedu.cn

PHP:  assert($x > 0);
来源：http://kf.nicolike.cn

JS:   console.assert(x > 0);
来源：http://nd.huixinmuqiang.cn

TS:   console.assert(x > 0);
来源：http://nw.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://jz.yuexingan06.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mv.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zp.nszjky.cn

C#:   Debug.Assert(x > 0);
来源：http://th.bjjhwx.cn

[H08] 获取错误信息与堆栈
来源：http://nn.huanxung.cn

Py:   str(e);  traceback.format_exc()
来源：http://wl.newstarts.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lk.nicolike.cn

JS:   e.message;  e.stack
来源：http://ot.szxytkj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wt.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://jd.chemitech.net.cn

Go:   err.Error()
来源：http://xp.panjiajie.cn

Ruby: e.message;  e.backtrace
来源：http://rf.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://kx.panjiajie.cn

[H09] 带错误码的异常
来源：http://nt.jctech888.com.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ec.huixinmuqiang.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://hh.panjiajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://im.shtwfgs.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fd.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ub.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vx.521024.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qo.yuexingan06.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zv.huixiangedu.cn

[H10] 资源自动释放
来源：http://zq.hnjuh.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mm.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://kd.bookmarksfly.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xe.huanxung.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lv.9csxet.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bd.jctech888.com.cn

Go:   defer f.Close()
来源：http://bk.chemitech.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bf.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ub.bookmarksfly.cn

================================================================================
来源：http://nn.shtwfgs.cn

I. 正则表达式
来源：http://bp.muxihuayi.cn

================================================================================
来源：http://rq.szxytkj.cn

[I01] 判断是否匹配
来源：http://jh.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tj.szsharing.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xe.bjjhwx.cn

JS:   /\d+/.test(s)
来源：http://xb.jctech888.com.cn

TS:   /\d+/.test(s)
来源：http://oc.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ee.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://kb.bookmarksfly.cn

Ruby: s.match?(/\d+/)
来源：http://dr.hnjuh.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cl.wgjwhj.cn

[I02] 提取所有匹配
来源：http://bh.huixinmuqiang.cn

Py:   re.findall(r"\d+", s)
来源：http://fp.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://eo.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rg.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://vg.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://df.521024.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lp.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://di.bjjhwx.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ce.newstarts.cn

[I03] 提取捕获分组
来源：http://py.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://me.huixinmuqiang.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://av.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://oe.bjjhwx.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://vi.jianghongdianzi.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kz.jctech888.com.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://as.shxzukj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mu.newstarts.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pd.panjiajie.cn

[I04] 正则替换
来源：http://gf.newstarts.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dd.bjjhwx.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://rb.nszjky.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fl.9csxet.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ba.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hv.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tt.lnxyls.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://na.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pk.newstarts.cn

[I05] 按正则拆分
来源：http://um.huixinmuqiang.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mb.shtwfgs.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pu.yuexingan06.cn

JS:   s.split(/\s*,\s*/)
来源：http://wg.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://sz.hahajie.cn

Java: s.split("\\s*,\\s*")
来源：http://uo.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sk.shxzskj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bn.hahajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xq.wgjwhj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cx.newstarts.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ev.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jk.hnjuh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zn.huanxung.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lz.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yv.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://xi.shxzukj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://nq.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://eg.521024.cn

[I07] 忽略大小写与多行模式
来源：http://nk.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dh.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hj.colortex.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hy.bjjhwx.cn

TS:   /error/gim
来源：http://pm.bjjhwx.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://eb.asd995.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rt.panjiajie.cn

Ruby: s.scan(/error/i)
来源：http://ia.jctech888.com.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ej.shtwfgs.cn

[I08] 贪婪与非贪婪匹配
来源：http://wg.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://qv.jctech888.com.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://jx.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wf.huixinmuqiang.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://gw.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://af.gzmigu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://oa.colortex.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zn.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://us.hnjuh.cn

================================================================================
来源：http://pj.hnjuh.cn

J. 日期与时间
来源：http://aa.szxytkj.cn

================================================================================
来源：http://na.yuntaijiaju.cn

[J01] 获取当前时间
来源：http://np.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://br.chemitech.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ny.huanxung.cn

JS:   new Date();  Date.now()
来源：http://ig.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://ti.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://is.szxytkj.cn

Go:   time.Now()
来源：http://lq.shtwfgs.cn

Ruby: Time.now
来源：http://by.szxytkj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ae.bjjhwx.cn

[J02] 格式化输出
来源：http://uv.lnxyls.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fm.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pf.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vx.panjiajie.cn

TS:   d.toISOString()
来源：http://ku.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ac.hnjuh.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xa.hnjuh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vq.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dv.newstarts.cn

[J03] 字符串解析为日期
来源：http://kz.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://by.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://qv.nszjky.cn

JS:   new Date("2024-01-02")
来源：http://je.panjiajie.cn

TS:   new Date("2024-01-02")
来源：http://au.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ma.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xh.hahajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://lf.nicolike.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hk.wgjwhj.cn

[J04] 时间戳与日期互转
来源：http://wm.9csxet.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://jx.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://js.szxytkj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://am.huixiangedu.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ek.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ly.shxzukj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pc.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vc.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://el.haigaiapp.cn

[J05] 时间加减（加 7 天）
来源：http://bd.wgjwhj.cn

Py:   now + timedelta(days=7)
来源：http://hk.muxihuayi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://fi.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dc.yuexingan06.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ww.bookmarksfly.cn

Java: LocalDate.now().plusDays(7)
来源：http://lp.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oi.jianghongdianzi.cn

Ruby: Time.now + 7 * 86400
来源：http://wl.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kj.haigaiapp.cn

[J06] 计算两时间之差
来源：http://jr.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://xp.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://fv.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hu.yuntaijiaju.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://cj.521024.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ee.9csxet.cn

Go:   end.Sub(start).Hours()
来源：http://ra.bookmarksfly.cn

Ruby: end - start                 # 返回秒数
来源：http://lw.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://wz.bjjhwx.cn

[J07] 比较两个日期
来源：http://eq.nicolike.cn

Py:   d1 < d2;  d1 == d2
来源：http://xi.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nd.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://yd.wgjwhj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ed.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://iq.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ck.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ht.hnjuh.cn

C#:   d1 < d2;  d1 == d2
来源：http://up.hahajie.cn

[J08] 提取年月日与星期
来源：http://ky.szsharing.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ii.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://et.gzmigu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xg.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cc.hnjuh.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vz.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ic.nicolike.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ku.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zx.yuntaijiaju.cn

[J09] 时区处理
来源：http://re.bookmarksfly.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://sd.huanxung.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sd.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://id.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xo.yuntaijiaju.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pk.nszjky.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mo.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ty.shxzukj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pv.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://to.yuexingan06.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.muxihuayi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://em.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ce.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xo.shxzukj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mj.hahajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xb.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kz.huanxung.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nk.huixiangedu.cn

================================================================================
来源：http://zh.shxzskj.cn

K. JSON 与序列化
来源：http://qf.haigaiapp.cn

================================================================================
来源：http://fo.bjjhwx.cn

[K01] 对象转 JSON 字符串
来源：http://og.huixinmuqiang.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://le.jctech888.com.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://du.asd995.cn

JS:   JSON.stringify(obj)
来源：http://yw.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://mr.wgjwhj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rb.jianghongdianzi.cn

Go:   json.Marshal(obj)
来源：http://gs.haigaiapp.cn

Ruby: obj.to_json                                     // require "json"
来源：http://tl.szsharing.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bw.shxzskj.cn


<!-- 参考信息 -->