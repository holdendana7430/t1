代发 wailian999

[G14] 数据类 / record
来源：http://ym.nszjky.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ur.wgjwhj.cn

PHP:  // 用 readonly 属性模拟
来源：http://bx.panjiajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wg.lnxyls.cn

TS:   type User = { name: string; age: number };
来源：http://jl.bookmarksfly.cn

Java: record User(String name, int age) {}
来源：http://qp.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://vx.shtwfgs.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://zw.jctech888.com.cn

C#:   record User(string Name, int Age);
来源：http://lu.yuntaijiaju.cn

[G15] 枚举
来源：http://vu.huixiangedu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://nv.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fd.newstarts.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qr.huixiangedu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hv.asd995.cn

Java: enum Color { RED, GREEN }
来源：http://pl.hahajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://eg.panjiajie.cn

Ruby: Color = %i[red green].freeze
来源：http://on.hnjuh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yb.521024.cn

[G16] 对象转数组 / 字典
来源：http://mg.szxytkj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ds.yuntaijiaju.cn

PHP:  get_object_vars($obj);
来源：http://sj.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://ff.lnxyls.cn

TS:   Object.entries(obj)
来源：http://lx.yuexingan06.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vo.muxihuayi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ko.wgjwhj.cn

Ruby: obj.instance_variables
来源：http://nc.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://jy.jctech888.com.cn

================================================================================
来源：http://vq.chemitech.net.cn

H. 异常与错误处理
来源：http://vu.jctech888.com.cn

================================================================================
来源：http://dg.9csxet.cn

[H01] try / catch 基础
来源：http://vb.chemitech.net.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pi.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nv.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nx.bookmarksfly.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ji.9csxet.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qn.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jn.bookmarksfly.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fm.521024.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ui.521024.cn

[H02] finally / ensure 收尾
来源：http://xr.gzmigu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://re.szsharing.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ph.bjjhwx.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dk.huixinmuqiang.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vm.lnxyls.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fg.521024.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://do.panjiajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ef.wgjwhj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zt.chemitech.net.cn

[H03] 主动抛出异常
来源：http://gr.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://ml.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jq.yuexingan06.cn

JS:   throw new Error("错误信息");
来源：http://zn.nszjky.cn

TS:   throw new Error("错误信息");
来源：http://bd.szxytkj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gk.huixinmuqiang.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sh.newstarts.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yi.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ml.jianghongdianzi.cn

[H04] 自定义异常类型
来源：http://ak.bookmarksfly.cn

Py:   class MyError(Exception): pass
来源：http://kb.nszjky.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qs.asd995.cn

JS:   class MyError extends Error {}
来源：http://sx.shtwfgs.cn

TS:   class MyError extends Error {}
来源：http://uj.yuexingan06.cn

Java: class MyException extends RuntimeException {}
来源：http://ip.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ii.hahajie.cn

Ruby: class MyError < StandardError; end
来源：http://qn.jctech888.com.cn

C#:   class MyException : Exception {}
来源：http://mu.yuexingan06.cn

[H05] 捕获特定类型
来源：http://px.hnjuh.cn

Py:   except ValueError as e:
来源：http://ls.9csxet.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yb.huanxung.cn

JS:   if (e instanceof TypeError) {}
来源：http://tu.shxzukj.cn

TS:   if (e instanceof TypeError) {}
来源：http://qm.panjiajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://eu.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yv.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://zg.jianghongdianzi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wi.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://cq.shxzukj.cn

Py:   value = d.get("k") or default
来源：http://ah.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://lm.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pl.lnxyls.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xm.szsharing.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rg.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hk.shtwfgs.cn

Ruby: d&.dig(:a, :b)
来源：http://om.bookmarksfly.cn

C#:   obj?.A?.B ?? default
来源：http://el.yuexingan06.cn

[H07] 断言
来源：http://xe.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://so.9csxet.cn

PHP:  assert($x > 0);
来源：http://sb.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://ei.9csxet.cn

TS:   console.assert(x > 0);
来源：http://wq.huixiangedu.cn

Java: assert x > 0 : "必须为正";
来源：http://uv.huixinmuqiang.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dl.szsharing.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sd.muxihuayi.cn

C#:   Debug.Assert(x > 0);
来源：http://fu.gzmigu.cn

[H08] 获取错误信息与堆栈
来源：http://hx.wgjwhj.cn

Py:   str(e);  traceback.format_exc()
来源：http://xx.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://dy.wgjwhj.cn

JS:   e.message;  e.stack
来源：http://qu.nicolike.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://kj.bookmarksfly.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.9csxet.cn

Go:   err.Error()
来源：http://ay.newstarts.cn

Ruby: e.message;  e.backtrace
来源：http://uf.wgjwhj.cn

C#:   e.Message;  e.StackTrace
来源：http://kq.nszjky.cn

[H09] 带错误码的异常
来源：http://xi.nicolike.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gx.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qp.nicolike.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hc.jianghongdianzi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qe.hnjuh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://sy.shxzukj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hv.jctech888.com.cn

Ruby: raise MyError.new("fail", 500)
来源：http://do.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ac.huixiangedu.cn

[H10] 资源自动释放
来源：http://co.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gf.shxzskj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ij.lnxyls.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://zn.bookmarksfly.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://fp.szsharing.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ma.hahajie.cn

Go:   defer f.Close()
来源：http://mm.wgjwhj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pw.bjjhwx.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://py.szsharing.cn

================================================================================
来源：http://fx.nszjky.cn

I. 正则表达式
来源：http://oo.huixiangedu.cn

================================================================================
来源：http://xc.lnxyls.cn

[I01] 判断是否匹配
来源：http://em.huixinmuqiang.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jf.jianghongdianzi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://vp.521024.cn

JS:   /\d+/.test(s)
来源：http://vw.huixinmuqiang.cn

TS:   /\d+/.test(s)
来源：http://yb.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vr.colortex.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xa.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://tq.gzmigu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://lg.huanxung.cn

[I02] 提取所有匹配
来源：http://op.asd995.cn

Py:   re.findall(r"\d+", s)
来源：http://ox.huixinmuqiang.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ow.jctech888.com.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ig.521024.cn

TS:   s.match(/\d+/g)
来源：http://wp.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kp.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tl.bjjhwx.cn

Ruby: s.scan(/\d+/)
来源：http://cf.wgjwhj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ip.yuexingan06.cn

[I03] 提取捕获分组
来源：http://tc.huixinmuqiang.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://po.yuntaijiaju.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://bp.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kd.jianghongdianzi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hc.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wc.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sz.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sr.yuexingan06.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fl.hahajie.cn

[I04] 正则替换
来源：http://tx.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bb.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bb.hnjuh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ab.szsharing.cn

TS:   s.replace(/\d+/g, "#")
来源：http://oo.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zq.hnjuh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qq.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ht.panjiajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pq.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://aj.gzmigu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gh.jctech888.com.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ip.shxzukj.cn

JS:   s.split(/\s*,\s*/)
来源：http://jt.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://px.haigaiapp.cn

Java: s.split("\\s*,\\s*")
来源：http://nh.bjjhwx.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vq.muxihuayi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ic.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bx.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://da.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ej.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qf.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eu.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bg.jctech888.com.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vy.huanxung.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qh.huixinmuqiang.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gj.lnxyls.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vk.szsharing.cn

[I07] 忽略大小写与多行模式
来源：http://qn.muxihuayi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mm.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jv.wgjwhj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kj.gzmigu.cn

TS:   /error/gim
来源：http://fr.yuntaijiaju.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ya.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uv.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://sc.bjjhwx.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://kd.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://hu.shxzskj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hu.yuntaijiaju.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://be.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wm.huixinmuqiang.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zh.asd995.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ur.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tn.huixinmuqiang.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mz.huanxung.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://mm.newstarts.cn

================================================================================
来源：http://ng.muxihuayi.cn

J. 日期与时间
来源：http://yh.shtwfgs.cn

================================================================================
来源：http://ka.9csxet.cn

[J01] 获取当前时间
来源：http://bm.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://jj.yuntaijiaju.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sj.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://yd.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://mh.nszjky.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://qv.huixiangedu.cn

Go:   time.Now()
来源：http://nr.hnjuh.cn

Ruby: Time.now
来源：http://te.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://iw.wgjwhj.cn

[J02] 格式化输出
来源：http://qh.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pu.lnxyls.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://kq.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xn.huixiangedu.cn

TS:   d.toISOString()
来源：http://lj.nszjky.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qy.hahajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://at.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gt.chemitech.net.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xn.panjiajie.cn

[J03] 字符串解析为日期
来源：http://lh.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://co.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bm.muxihuayi.cn

JS:   new Date("2024-01-02")
来源：http://yw.muxihuayi.cn

TS:   new Date("2024-01-02")
来源：http://wv.jctech888.com.cn

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://bj.asd995.cn

Ruby: Date.parse("2024-01-02")
来源：http://zw.hahajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://eq.521024.cn

[J04] 时间戳与日期互转
来源：http://tr.bookmarksfly.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vs.nszjky.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sc.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ez.bookmarksfly.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ft.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://li.nszjky.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nd.shtwfgs.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gl.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wv.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://dm.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://kp.shxzskj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://wk.yuexingan06.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wb.nicolike.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bw.yuexingan06.cn

Java: LocalDate.now().plusDays(7)
来源：http://mq.nicolike.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mz.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://bm.colortex.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cn.panjiajie.cn

[J06] 计算两时间之差
来源：http://vu.hnjuh.cn

Py:   (end - start).total_seconds()
来源：http://pu.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://wt.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hi.lnxyls.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hy.huanxung.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rd.yuntaijiaju.cn

Go:   end.Sub(start).Hours()
来源：http://xx.huanxung.cn

Ruby: end - start                 # 返回秒数
来源：http://um.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://ac.gzmigu.cn

[J07] 比较两个日期
来源：http://fv.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://je.wgjwhj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jh.lnxyls.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qq.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cx.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://io.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cl.yuexingan06.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xv.huixinmuqiang.cn

C#:   d1 < d2;  d1 == d2
来源：http://vu.szxytkj.cn

[J08] 提取年月日与星期
来源：http://tg.hahajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ih.huixiangedu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wu.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ug.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://qd.bookmarksfly.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rq.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pg.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zo.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ro.shtwfgs.cn

[J09] 时区处理
来源：http://dp.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ws.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jn.lnxyls.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vo.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qr.gzmigu.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ru.lnxyls.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ok.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fw.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pt.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://po.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ik.huixiangedu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ju.bjjhwx.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rk.chemitech.net.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ny.newstarts.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://uc.nicolike.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fu.huixiangedu.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mo.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://fd.521024.cn

================================================================================
来源：http://df.yuntaijiaju.cn

K. JSON 与序列化
来源：http://co.bookmarksfly.cn

================================================================================
来源：http://tc.muxihuayi.cn

[K01] 对象转 JSON 字符串
来源：http://ps.wgjwhj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mt.shxzukj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sh.lnxyls.cn

JS:   JSON.stringify(obj)
来源：http://ka.shtwfgs.cn

TS:   JSON.stringify(obj)
来源：http://ku.gzmigu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cu.hahajie.cn

Go:   json.Marshal(obj)
来源：http://mz.nszjky.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mk.yuntaijiaju.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://wk.newstarts.cn


<!-- 参考信息 -->