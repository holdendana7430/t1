代发 wailian999

[G14] 数据类 / record
来源：http://wi.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cd.521024.cn

PHP:  // 用 readonly 属性模拟
来源：http://eq.yuexingan06.cn

JS:   // 无内置：普通类或对象字面量
来源：http://in.chemitech.net.cn

TS:   type User = { name: string; age: number };
来源：http://pj.huixiangedu.cn

Java: record User(String name, int age) {}
来源：http://gn.wgjwhj.cn

Go:   type User struct { Name string; Age int }
来源：http://ul.nszjky.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ir.lnxyls.cn

C#:   record User(string Name, int Age);
来源：http://xb.newstarts.cn

[G15] 枚举
来源：http://cx.wgjwhj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://is.jianghongdianzi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://mh.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wj.9csxet.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ip.wgjwhj.cn

Java: enum Color { RED, GREEN }
来源：http://hk.gzmigu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://dj.bookmarksfly.cn

Ruby: Color = %i[red green].freeze
来源：http://sa.521024.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kg.nszjky.cn

[G16] 对象转数组 / 字典
来源：http://ez.panjiajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ix.hahajie.cn

PHP:  get_object_vars($obj);
来源：http://tt.huixinmuqiang.cn

JS:   Object.entries(obj)
来源：http://tj.nszjky.cn

TS:   Object.entries(obj)
来源：http://wi.huixinmuqiang.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://vm.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jr.521024.cn

Ruby: obj.instance_variables
来源：http://kj.wgjwhj.cn

C#:   // 用反射或 System.Text.Json
来源：http://tt.asd995.cn

================================================================================
来源：http://ml.wgjwhj.cn

H. 异常与错误处理
来源：http://dt.huixiangedu.cn

================================================================================
来源：http://ah.huanxung.cn

[H01] try / catch 基础
来源：http://wg.hahajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kr.jianghongdianzi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yh.lnxyls.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://gg.nicolike.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cx.huanxung.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nk.jctech888.com.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sb.yuexingan06.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tl.521024.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://um.gzmigu.cn

[H02] finally / ensure 收尾
来源：http://lz.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dz.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://no.jianghongdianzi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ab.yuntaijiaju.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tc.wgjwhj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gw.panjiajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ri.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gp.9csxet.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ly.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://ci.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://kn.newstarts.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gu.huixinmuqiang.cn

JS:   throw new Error("错误信息");
来源：http://sn.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://ca.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://im.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://im.yuexingan06.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vd.nicolike.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rt.szxytkj.cn

[H04] 自定义异常类型
来源：http://zb.lnxyls.cn

Py:   class MyError(Exception): pass
来源：http://tq.hnjuh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://bj.szsharing.cn

JS:   class MyError extends Error {}
来源：http://da.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://kb.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://ry.yuntaijiaju.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vs.521024.cn

Ruby: class MyError < StandardError; end
来源：http://ug.chemitech.net.cn

C#:   class MyException : Exception {}
来源：http://wo.shtwfgs.cn

[H05] 捕获特定类型
来源：http://nr.szsharing.cn

Py:   except ValueError as e:
来源：http://yh.shtwfgs.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ia.shxzskj.cn

JS:   if (e instanceof TypeError) {}
来源：http://tn.9csxet.cn

TS:   if (e instanceof TypeError) {}
来源：http://ii.shxzukj.cn

Java: catch (IOException | SQLException e) {}
来源：http://dr.shtwfgs.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cy.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://vx.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://xy.szsharing.cn

[H06] 可选值 / 空值安全访问
来源：http://dd.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://pf.9csxet.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bk.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://jf.huixiangedu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cr.yuexingan06.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wo.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ba.gzmigu.cn

Ruby: d&.dig(:a, :b)
来源：http://sg.huanxung.cn

C#:   obj?.A?.B ?? default
来源：http://nk.chemitech.net.cn

[H07] 断言
来源：http://oo.wgjwhj.cn

Py:   assert x > 0, "必须为正"
来源：http://ly.hnjuh.cn

PHP:  assert($x > 0);
来源：http://cc.muxihuayi.cn

JS:   console.assert(x > 0);
来源：http://lj.nszjky.cn

TS:   console.assert(x > 0);
来源：http://xj.shxzukj.cn

Java: assert x > 0 : "必须为正";
来源：http://cf.bookmarksfly.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://gc.haigaiapp.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xd.nszjky.cn

C#:   Debug.Assert(x > 0);
来源：http://nj.hnjuh.cn

[H08] 获取错误信息与堆栈
来源：http://ke.colortex.cn

Py:   str(e);  traceback.format_exc()
来源：http://ej.shtwfgs.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://rc.bjjhwx.cn

JS:   e.message;  e.stack
来源：http://dc.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://js.haigaiapp.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://el.panjiajie.cn

Go:   err.Error()
来源：http://ij.muxihuayi.cn

Ruby: e.message;  e.backtrace
来源：http://ty.szsharing.cn

C#:   e.Message;  e.StackTrace
来源：http://uk.colortex.cn

[H09] 带错误码的异常
来源：http://gt.nszjky.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uy.haigaiapp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ci.chemitech.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nv.bookmarksfly.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://tl.hnjuh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://pe.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fd.521024.cn

Ruby: raise MyError.new("fail", 500)
来源：http://af.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zv.nszjky.cn

[H10] 资源自动释放
来源：http://nd.wgjwhj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vn.yuexingan06.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.huixiangedu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mn.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qx.huixinmuqiang.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nn.wgjwhj.cn

Go:   defer f.Close()
来源：http://ug.chemitech.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vs.wgjwhj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wo.shxzukj.cn

================================================================================
来源：http://ts.huixiangedu.cn

I. 正则表达式
来源：http://hi.yuntaijiaju.cn

================================================================================
来源：http://di.yuntaijiaju.cn

[I01] 判断是否匹配
来源：http://cp.shxzskj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tq.hahajie.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hb.newstarts.cn

JS:   /\d+/.test(s)
来源：http://dk.szsharing.cn

TS:   /\d+/.test(s)
来源：http://lp.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ty.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wb.colortex.cn

Ruby: s.match?(/\d+/)
来源：http://pp.jianghongdianzi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bs.panjiajie.cn

[I02] 提取所有匹配
来源：http://et.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://zf.jctech888.com.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ei.gzmigu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ii.nicolike.cn

TS:   s.match(/\d+/g)
来源：http://vi.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://eo.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://iy.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://es.asd995.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kv.huixiangedu.cn

[I03] 提取捕获分组
来源：http://ur.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://my.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ex.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fm.wgjwhj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nx.521024.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://cs.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://aw.hnjuh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gi.shxzskj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mb.panjiajie.cn

[I04] 正则替换
来源：http://od.hahajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ef.shxzukj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://te.9csxet.cn

JS:   s.replace(/\d+/g, "#")
来源：http://sv.shtwfgs.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mh.bjjhwx.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bl.lnxyls.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://do.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wk.huanxung.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qz.bookmarksfly.cn

[I05] 按正则拆分
来源：http://xe.shtwfgs.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://aa.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xd.shxzskj.cn

JS:   s.split(/\s*,\s*/)
来源：http://nv.9csxet.cn

TS:   s.split(/\s*,\s*/)
来源：http://ml.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://jk.chemitech.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://iz.lnxyls.cn

Ruby: s.split(/\s*,\s*/)
来源：http://bx.bjjhwx.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://gq.panjiajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sf.shxzukj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rb.hnjuh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uy.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oy.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pm.chemitech.net.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vs.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sp.panjiajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pi.yuntaijiaju.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fi.bookmarksfly.cn

[I07] 忽略大小写与多行模式
来源：http://zi.muxihuayi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cc.szxytkj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ev.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zp.9csxet.cn

TS:   /error/gim
来源：http://aw.jianghongdianzi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hb.muxihuayi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://cu.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://ry.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://we.shxzskj.cn

[I08] 贪婪与非贪婪匹配
来源：http://dv.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nn.newstarts.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://gp.asd995.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xu.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yt.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ur.521024.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xp.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yu.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xi.nszjky.cn

================================================================================
来源：http://cv.bookmarksfly.cn

J. 日期与时间
来源：http://dx.jianghongdianzi.cn

================================================================================
来源：http://ph.521024.cn

[J01] 获取当前时间
来源：http://vu.lnxyls.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kx.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://bw.9csxet.cn

JS:   new Date();  Date.now()
来源：http://et.panjiajie.cn

TS:   new Date();  Date.now()
来源：http://ha.yuntaijiaju.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fy.muxihuayi.cn

Go:   time.Now()
来源：http://ta.9csxet.cn

Ruby: Time.now
来源：http://qz.shtwfgs.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uu.jianghongdianzi.cn

[J02] 格式化输出
来源：http://nk.shxzskj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zr.bookmarksfly.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qk.asd995.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://os.muxihuayi.cn

TS:   d.toISOString()
来源：http://kc.shxzukj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fd.gzmigu.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zr.huanxung.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vz.muxihuayi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wz.bookmarksfly.cn

[J03] 字符串解析为日期
来源：http://yd.nicolike.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qf.shxzskj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aq.yuntaijiaju.cn

JS:   new Date("2024-01-02")
来源：http://dm.szsharing.cn

TS:   new Date("2024-01-02")
来源：http://kv.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ma.newstarts.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fg.yuntaijiaju.cn

Ruby: Date.parse("2024-01-02")
来源：http://rz.yuntaijiaju.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://gu.szxytkj.cn

[J04] 时间戳与日期互转
来源：http://ru.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://lh.nicolike.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wm.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sk.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yi.chemitech.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qv.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fb.muxihuayi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://xq.lnxyls.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ep.hahajie.cn

[J05] 时间加减（加 7 天）
来源：http://rs.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://oz.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ny.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wl.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://sl.huixinmuqiang.cn

Java: LocalDate.now().plusDays(7)
来源：http://ef.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://eu.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://uf.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qh.huanxung.cn

[J06] 计算两时间之差
来源：http://ou.hahajie.cn

Py:   (end - start).total_seconds()
来源：http://rz.huixinmuqiang.cn

PHP:  $end->diff($start)->days;
来源：http://hm.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zm.yuexingan06.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://jh.huanxung.cn

Java: Duration.between(start, end).toSeconds()
来源：http://nu.gzmigu.cn

Go:   end.Sub(start).Hours()
来源：http://nx.bookmarksfly.cn

Ruby: end - start                 # 返回秒数
来源：http://xa.9csxet.cn

C#:   (end - start).TotalSeconds
来源：http://bp.hnjuh.cn

[J07] 比较两个日期
来源：http://nf.huanxung.cn

Py:   d1 < d2;  d1 == d2
来源：http://ys.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mi.nicolike.cn

JS:   d1.getTime() < d2.getTime()
来源：http://gn.szsharing.cn

TS:   d1.getTime() < d2.getTime()
来源：http://uk.lnxyls.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bb.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xm.yuntaijiaju.cn

Ruby: d1 < d2;  d1 == d2
来源：http://qk.hnjuh.cn

C#:   d1 < d2;  d1 == d2
来源：http://vj.huixinmuqiang.cn

[J08] 提取年月日与星期
来源：http://ag.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fd.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wf.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://da.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yf.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ve.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fh.nicolike.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cp.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lc.yuexingan06.cn

[J09] 时区处理
来源：http://vr.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uj.wgjwhj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://pc.hnjuh.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ea.hnjuh.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fu.wgjwhj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://eu.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qj.huixinmuqiang.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ee.shxzskj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kk.huixinmuqiang.cn

[J10] 取今天 / 本月第一天
来源：http://tl.9csxet.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://kg.9csxet.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tk.haigaiapp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ls.shtwfgs.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ig.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ow.521024.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zm.hnjuh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://it.hnjuh.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://oh.chemitech.net.cn

================================================================================
来源：http://yn.chemitech.net.cn

K. JSON 与序列化
来源：http://ic.jianghongdianzi.cn

================================================================================
来源：http://jh.szsharing.cn

[K01] 对象转 JSON 字符串
来源：http://nl.gzmigu.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://eu.haigaiapp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xd.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://dc.huixiangedu.cn

TS:   JSON.stringify(obj)
来源：http://jt.9csxet.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dn.huixinmuqiang.cn

Go:   json.Marshal(obj)
来源：http://jv.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bo.9csxet.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sy.jctech888.com.cn


<!-- 参考信息 -->