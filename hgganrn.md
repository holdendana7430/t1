代发 wailian999

[G14] 数据类 / record
来源：http://py.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wo.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://si.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://yt.panjiajie.cn

TS:   type User = { name: string; age: number };
来源：http://as.yuntaijiaju.cn

Java: record User(String name, int age) {}
来源：http://gw.bjjhwx.cn

Go:   type User struct { Name string; Age int }
来源：http://ad.yuntaijiaju.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://cc.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://vz.huixiangedu.cn

[G15] 枚举
来源：http://bn.szxytkj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mw.lnxyls.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ij.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xz.huanxung.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sv.shxzskj.cn

Java: enum Color { RED, GREEN }
来源：http://ed.huanxung.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mj.shxzukj.cn

Ruby: Color = %i[red green].freeze
来源：http://zs.9csxet.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oz.nicolike.cn

[G16] 对象转数组 / 字典
来源：http://mc.huixinmuqiang.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ms.muxihuayi.cn

PHP:  get_object_vars($obj);
来源：http://qd.9csxet.cn

JS:   Object.entries(obj)
来源：http://kx.yuntaijiaju.cn

TS:   Object.entries(obj)
来源：http://bj.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ai.hnjuh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://fy.9csxet.cn

Ruby: obj.instance_variables
来源：http://lj.nszjky.cn

C#:   // 用反射或 System.Text.Json
来源：http://oj.bjjhwx.cn

================================================================================
来源：http://gl.yuexingan06.cn

H. 异常与错误处理
来源：http://yo.shxzskj.cn

================================================================================
来源：http://fd.chemitech.net.cn

[H01] try / catch 基础
来源：http://xz.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zw.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fd.huanxung.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qs.chemitech.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lu.panjiajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://za.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://aa.gzmigu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ox.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hj.nszjky.cn

[H02] finally / ensure 收尾
来源：http://oi.muxihuayi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lv.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://up.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://tb.haigaiapp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zp.yuntaijiaju.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sk.panjiajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dd.nszjky.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qf.muxihuayi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://jk.wgjwhj.cn

[H03] 主动抛出异常
来源：http://vq.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://us.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dl.nszjky.cn

JS:   throw new Error("错误信息");
来源：http://ew.shxzukj.cn

TS:   throw new Error("错误信息");
来源：http://ih.yuexingan06.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bg.lnxyls.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hs.huixinmuqiang.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://at.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://us.chemitech.net.cn

[H04] 自定义异常类型
来源：http://mc.yuntaijiaju.cn

Py:   class MyError(Exception): pass
来源：http://ch.chemitech.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://of.asd995.cn

JS:   class MyError extends Error {}
来源：http://ff.asd995.cn

TS:   class MyError extends Error {}
来源：http://ww.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://ug.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cs.szsharing.cn

Ruby: class MyError < StandardError; end
来源：http://kt.szsharing.cn

C#:   class MyException : Exception {}
来源：http://od.huixinmuqiang.cn

[H05] 捕获特定类型
来源：http://om.shtwfgs.cn

Py:   except ValueError as e:
来源：http://jk.nicolike.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wy.szxytkj.cn

JS:   if (e instanceof TypeError) {}
来源：http://hz.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://ge.huanxung.cn

Java: catch (IOException | SQLException e) {}
来源：http://cx.yuntaijiaju.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yo.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://ae.yuntaijiaju.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ab.shtwfgs.cn

[H06] 可选值 / 空值安全访问
来源：http://xf.jctech888.com.cn

Py:   value = d.get("k") or default
来源：http://eg.521024.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jb.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bk.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qv.wgjwhj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pm.yuntaijiaju.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kq.shtwfgs.cn

Ruby: d&.dig(:a, :b)
来源：http://eh.panjiajie.cn

C#:   obj?.A?.B ?? default
来源：http://nq.panjiajie.cn

[H07] 断言
来源：http://ec.huixinmuqiang.cn

Py:   assert x > 0, "必须为正"
来源：http://xb.nicolike.cn

PHP:  assert($x > 0);
来源：http://dw.hahajie.cn

JS:   console.assert(x > 0);
来源：http://nx.hahajie.cn

TS:   console.assert(x > 0);
来源：http://uv.huanxung.cn

Java: assert x > 0 : "必须为正";
来源：http://dh.chemitech.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ke.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://mt.nicolike.cn

C#:   Debug.Assert(x > 0);
来源：http://nr.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://xm.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://yk.yuexingan06.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://iu.haigaiapp.cn

JS:   e.message;  e.stack
来源：http://wr.hnjuh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://uj.colortex.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://eg.colortex.cn

Go:   err.Error()
来源：http://bk.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://yb.gzmigu.cn

C#:   e.Message;  e.StackTrace
来源：http://il.muxihuayi.cn

[H09] 带错误码的异常
来源：http://rx.bookmarksfly.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://kr.szsharing.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://oe.bjjhwx.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qr.shxzskj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zm.lnxyls.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jv.lnxyls.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wp.521024.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yy.hnjuh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://yq.bookmarksfly.cn

[H10] 资源自动释放
来源：http://fe.jianghongdianzi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hj.shtwfgs.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ua.jianghongdianzi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hk.shxzukj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ds.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fo.yuntaijiaju.cn

Go:   defer f.Close()
来源：http://sc.hnjuh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fq.huixinmuqiang.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zo.jctech888.com.cn

================================================================================
来源：http://qq.nicolike.cn

I. 正则表达式
来源：http://hc.shtwfgs.cn

================================================================================
来源：http://oe.colortex.cn

[I01] 判断是否匹配
来源：http://if.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ot.gzmigu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://co.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://fh.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://dk.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qk.colortex.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mn.newstarts.cn

Ruby: s.match?(/\d+/)
来源：http://bf.haigaiapp.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://za.huanxung.cn

[I02] 提取所有匹配
来源：http://fv.521024.cn

Py:   re.findall(r"\d+", s)
来源：http://ts.shxzskj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oz.muxihuayi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://sa.szsharing.cn

TS:   s.match(/\d+/g)
来源：http://qo.yuntaijiaju.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zb.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://gf.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://vw.bookmarksfly.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fl.newstarts.cn

[I03] 提取捕获分组
来源：http://zh.shxzskj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ix.lnxyls.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rk.hahajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kd.huixiangedu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jd.bjjhwx.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dw.wgjwhj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bl.shxzskj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gc.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fn.nszjky.cn

[I04] 正则替换
来源：http://vv.lnxyls.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vh.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lo.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zp.haigaiapp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ep.bookmarksfly.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fe.muxihuayi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mp.shxzskj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ov.jctech888.com.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rn.szsharing.cn

[I05] 按正则拆分
来源：http://vc.bjjhwx.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://be.asd995.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kd.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://ol.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://kb.huixiangedu.cn

Java: s.split("\\s*,\\s*")
来源：http://gn.gzmigu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ky.shtwfgs.cn

Ruby: s.split(/\s*,\s*/)
来源：http://te.bookmarksfly.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sl.szsharing.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://vx.hnjuh.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bp.hahajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ee.szxytkj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cs.newstarts.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fu.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://my.haigaiapp.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://og.gzmigu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://is.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tx.newstarts.cn

[I07] 忽略大小写与多行模式
来源：http://wi.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://np.gzmigu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fn.nicolike.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ol.huanxung.cn

TS:   /error/gim
来源：http://hz.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jn.bookmarksfly.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://aj.521024.cn

Ruby: s.scan(/error/i)
来源：http://aj.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://un.huixinmuqiang.cn

[I08] 贪婪与非贪婪匹配
来源：http://kb.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dz.szsharing.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://oz.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vq.lnxyls.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jn.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ia.hahajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ne.jianghongdianzi.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zn.yuntaijiaju.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tb.huixinmuqiang.cn

================================================================================
来源：http://jc.szxytkj.cn

J. 日期与时间
来源：http://cm.9csxet.cn

================================================================================
来源：http://gt.shxzukj.cn

[J01] 获取当前时间
来源：http://yc.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pr.szxytkj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cs.shtwfgs.cn

JS:   new Date();  Date.now()
来源：http://pg.lnxyls.cn

TS:   new Date();  Date.now()
来源：http://ae.jianghongdianzi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kh.jianghongdianzi.cn

Go:   time.Now()
来源：http://dv.nszjky.cn

Ruby: Time.now
来源：http://fi.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dl.haigaiapp.cn

[J02] 格式化输出
来源：http://lq.haigaiapp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dr.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ti.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zc.szxytkj.cn

TS:   d.toISOString()
来源：http://ej.haigaiapp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://up.yuexingan06.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://az.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uj.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ll.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://cw.521024.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fc.chemitech.net.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vb.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://jg.shxzskj.cn

TS:   new Date("2024-01-02")
来源：http://nz.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://em.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://pi.szxytkj.cn

Ruby: Date.parse("2024-01-02")
来源：http://cl.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ry.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://wt.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yr.huixiangedu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vd.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://re.jctech888.com.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ey.jianghongdianzi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vu.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ec.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xw.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vg.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://mb.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://jl.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sl.nicolike.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pj.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wd.lnxyls.cn

Java: LocalDate.now().plusDays(7)
来源：http://uo.shxzskj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://un.hnjuh.cn

Ruby: Time.now + 7 * 86400
来源：http://nb.bjjhwx.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yj.szxytkj.cn

[J06] 计算两时间之差
来源：http://db.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://za.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://zm.huixinmuqiang.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://oq.gzmigu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vk.hahajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ks.521024.cn

Go:   end.Sub(start).Hours()
来源：http://kc.jianghongdianzi.cn

Ruby: end - start                 # 返回秒数
来源：http://le.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://nr.huanxung.cn

[J07] 比较两个日期
来源：http://kd.521024.cn

Py:   d1 < d2;  d1 == d2
来源：http://op.bookmarksfly.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vh.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xh.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ut.wgjwhj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://sk.shxzskj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://oi.panjiajie.cn

Ruby: d1 < d2;  d1 == d2
来源：http://xc.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://gn.hnjuh.cn

[J08] 提取年月日与星期
来源：http://tw.shtwfgs.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://uq.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://og.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dd.nicolike.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nt.nicolike.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pz.yuntaijiaju.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ym.gzmigu.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fc.hnjuh.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dl.szsharing.cn

[J09] 时区处理
来源：http://lv.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uv.panjiajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nt.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uk.yuntaijiaju.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kh.shxzskj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://db.muxihuayi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ka.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ao.yuexingan06.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fj.lnxyls.cn

[J10] 取今天 / 本月第一天
来源：http://ns.asd995.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vu.shtwfgs.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ab.panjiajie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ac.huixiangedu.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://um.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wy.wgjwhj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qk.shxzukj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sk.gzmigu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pf.nicolike.cn

================================================================================
来源：http://iz.lnxyls.cn

K. JSON 与序列化
来源：http://dg.shtwfgs.cn

================================================================================
来源：http://gy.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://xu.huixiangedu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pn.huanxung.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vh.gzmigu.cn

JS:   JSON.stringify(obj)
来源：http://zn.yuntaijiaju.cn

TS:   JSON.stringify(obj)
来源：http://gc.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rq.521024.cn

Go:   json.Marshal(obj)
来源：http://ia.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://gw.panjiajie.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://es.shxzskj.cn


<!-- 参考信息 -->