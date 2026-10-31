代发 wailian999

Java: u instanceof User
来源：http://ym.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ig.huanxung.cn

Ruby: u.is_a?(User)
来源：http://qg.huixinmuqiang.cn

C#:   u is User
来源：http://vi.yuexingan06.cn

[G14] 数据类 / record
来源：http://di.nszjky.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xl.haigaiapp.cn

PHP:  // 用 readonly 属性模拟
来源：http://ho.gzmigu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://kr.shxzskj.cn

TS:   type User = { name: string; age: number };
来源：http://bi.huixiangedu.cn

Java: record User(String name, int age) {}
来源：http://mm.asd995.cn

Go:   type User struct { Name string; Age int }
来源：http://fa.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ay.shxzukj.cn

C#:   record User(string Name, int Age);
来源：http://hr.gzmigu.cn

[G15] 枚举
来源：http://xl.hnjuh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ou.gzmigu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xb.gzmigu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bc.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pj.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://we.panjiajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://un.9csxet.cn

Ruby: Color = %i[red green].freeze
来源：http://dd.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fy.shxzukj.cn

[G16] 对象转数组 / 字典
来源：http://lg.hahajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qh.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://cd.colortex.cn

JS:   Object.entries(obj)
来源：http://gw.newstarts.cn

TS:   Object.entries(obj)
来源：http://dl.haigaiapp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yk.colortex.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://va.lnxyls.cn

Ruby: obj.instance_variables
来源：http://xe.asd995.cn

C#:   // 用反射或 System.Text.Json
来源：http://ez.newstarts.cn

================================================================================
来源：http://vs.panjiajie.cn

H. 异常与错误处理
来源：http://qf.gzmigu.cn

================================================================================
来源：http://tp.shxzukj.cn

[H01] try / catch 基础
来源：http://hy.panjiajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://er.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tw.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nl.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://on.szxytkj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ns.szxytkj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nk.gzmigu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fg.nszjky.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://df.521024.cn

[H02] finally / ensure 收尾
来源：http://yb.bookmarksfly.cn

Py:   try: f()⏎finally: cleanup()
来源：http://si.muxihuayi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cd.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hp.szsharing.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vl.9csxet.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ty.jctech888.com.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mg.huixiangedu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bt.huixiangedu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dh.hahajie.cn

[H03] 主动抛出异常
来源：http://hu.yuexingan06.cn

Py:   raise ValueError("错误信息")
来源：http://ks.nicolike.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cv.bookmarksfly.cn

JS:   throw new Error("错误信息");
来源：http://sd.jianghongdianzi.cn

TS:   throw new Error("错误信息");
来源：http://iw.newstarts.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://oc.hnjuh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://js.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vm.newstarts.cn

C#:   throw new ArgumentException("错误信息");
来源：http://iy.chemitech.net.cn

[H04] 自定义异常类型
来源：http://gg.muxihuayi.cn

Py:   class MyError(Exception): pass
来源：http://hx.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://au.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://db.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://px.newstarts.cn

Java: class MyException extends RuntimeException {}
来源：http://pw.huixinmuqiang.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fd.huixiangedu.cn

Ruby: class MyError < StandardError; end
来源：http://lq.shxzskj.cn

C#:   class MyException : Exception {}
来源：http://le.szsharing.cn

[H05] 捕获特定类型
来源：http://nu.panjiajie.cn

Py:   except ValueError as e:
来源：http://wg.muxihuayi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bb.szxytkj.cn

JS:   if (e instanceof TypeError) {}
来源：http://vy.panjiajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://if.panjiajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://va.hahajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hx.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://no.yuexingan06.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://zk.huanxung.cn

[H06] 可选值 / 空值安全访问
来源：http://ay.shxzskj.cn

Py:   value = d.get("k") or default
来源：http://yr.szsharing.cn

PHP:  $v = $d["k"] ?? null;
来源：http://kl.521024.cn

JS:   obj?.a?.b;  d ?? default
来源：http://js.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://iu.521024.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://gu.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://em.huixinmuqiang.cn

Ruby: d&.dig(:a, :b)
来源：http://vn.shtwfgs.cn

C#:   obj?.A?.B ?? default
来源：http://jm.jctech888.com.cn

[H07] 断言
来源：http://co.shxzskj.cn

Py:   assert x > 0, "必须为正"
来源：http://ig.nicolike.cn

PHP:  assert($x > 0);
来源：http://fk.nicolike.cn

JS:   console.assert(x > 0);
来源：http://zj.nicolike.cn

TS:   console.assert(x > 0);
来源：http://nr.shtwfgs.cn

Java: assert x > 0 : "必须为正";
来源：http://de.9csxet.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jb.nszjky.cn

Ruby: raise "必须为正" unless x > 0
来源：http://xh.wgjwhj.cn

C#:   Debug.Assert(x > 0);
来源：http://bu.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://kp.wgjwhj.cn

Py:   str(e);  traceback.format_exc()
来源：http://hj.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mn.jctech888.com.cn

JS:   e.message;  e.stack
来源：http://pa.panjiajie.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bh.huanxung.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://la.521024.cn

Go:   err.Error()
来源：http://bh.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://ep.szsharing.cn

C#:   e.Message;  e.StackTrace
来源：http://tk.hahajie.cn

[H09] 带错误码的异常
来源：http://aq.asd995.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dn.gzmigu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yd.shtwfgs.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ym.hahajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://av.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ps.panjiajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rk.colortex.cn

Ruby: raise MyError.new("fail", 500)
来源：http://rf.muxihuayi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://fp.szxytkj.cn

[H10] 资源自动释放
来源：http://fn.huixinmuqiang.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ry.huixinmuqiang.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dn.huixinmuqiang.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fv.newstarts.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zw.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://vm.jctech888.com.cn

Go:   defer f.Close()
来源：http://cn.bjjhwx.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xf.szsharing.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://my.hahajie.cn

================================================================================
来源：http://cb.nicolike.cn

I. 正则表达式
来源：http://ba.haigaiapp.cn

================================================================================
来源：http://rm.521024.cn

[I01] 判断是否匹配
来源：http://xz.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://aj.jianghongdianzi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dc.huixiangedu.cn

JS:   /\d+/.test(s)
来源：http://ue.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://wz.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fz.nszjky.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bs.szsharing.cn

Ruby: s.match?(/\d+/)
来源：http://hb.panjiajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ja.szsharing.cn

[I02] 提取所有匹配
来源：http://wk.huixinmuqiang.cn

Py:   re.findall(r"\d+", s)
来源：http://fw.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dn.shtwfgs.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mj.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://tu.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://lu.hahajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://uq.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://sp.wgjwhj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ai.muxihuayi.cn

[I03] 提取捕获分组
来源：http://ih.nicolike.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://li.gzmigu.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dh.gzmigu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hp.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jj.yuntaijiaju.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ju.jctech888.com.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://aw.jianghongdianzi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://cv.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://nz.wgjwhj.cn

[I04] 正则替换
来源：http://sz.chemitech.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fs.yuexingan06.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ar.jianghongdianzi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fg.szxytkj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xh.shxzukj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rn.yuexingan06.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://se.newstarts.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fz.jctech888.com.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tb.szsharing.cn

[I05] 按正则拆分
来源：http://nq.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rg.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://zf.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://dt.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://pq.wgjwhj.cn

Java: s.split("\\s*,\\s*")
来源：http://rw.haigaiapp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://zt.shxzskj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ha.haigaiapp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tj.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sz.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gj.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://vk.szxytkj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rg.bjjhwx.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ep.yuntaijiaju.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gj.wgjwhj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rh.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ij.huixiangedu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uy.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://ta.nszjky.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://lk.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ra.hahajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ko.jianghongdianzi.cn

TS:   /error/gim
来源：http://we.colortex.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rr.colortex.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zr.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://rs.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ms.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://iv.haigaiapp.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sf.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://sd.colortex.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qz.lnxyls.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vb.haigaiapp.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ji.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wj.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bp.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yd.wgjwhj.cn

================================================================================
来源：http://lp.chemitech.net.cn

J. 日期与时间
来源：http://yn.bookmarksfly.cn

================================================================================
来源：http://es.chemitech.net.cn

[J01] 获取当前时间
来源：http://yu.nszjky.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://gt.gzmigu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://by.huixinmuqiang.cn

JS:   new Date();  Date.now()
来源：http://no.bjjhwx.cn

TS:   new Date();  Date.now()
来源：http://eh.huixinmuqiang.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vk.huanxung.cn

Go:   time.Now()
来源：http://kt.yuexingan06.cn

Ruby: Time.now
来源：http://za.chemitech.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://za.asd995.cn

[J02] 格式化输出
来源：http://ow.colortex.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pp.bookmarksfly.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qe.wgjwhj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://uf.nszjky.cn

TS:   d.toISOString()
来源：http://ny.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ru.jianghongdianzi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://gs.wgjwhj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bs.jianghongdianzi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sp.huanxung.cn

[J03] 字符串解析为日期
来源：http://dl.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hp.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cg.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://wx.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://bc.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ub.asd995.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xp.asd995.cn

Ruby: Date.parse("2024-01-02")
来源：http://os.jctech888.com.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nk.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://yf.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://th.yuntaijiaju.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sf.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sg.jianghongdianzi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ps.shtwfgs.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://fs.wgjwhj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qf.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://cm.hahajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hc.bjjhwx.cn

[J05] 时间加减（加 7 天）
来源：http://dm.bookmarksfly.cn

Py:   now + timedelta(days=7)
来源：http://qt.haigaiapp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ti.jctech888.com.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pz.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bv.9csxet.cn

Java: LocalDate.now().plusDays(7)
来源：http://uh.shxzskj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wy.panjiajie.cn

Ruby: Time.now + 7 * 86400
来源：http://yz.panjiajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://em.yuexingan06.cn

[J06] 计算两时间之差
来源：http://xe.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://rz.521024.cn

PHP:  $end->diff($start)->days;
来源：http://gk.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://qs.gzmigu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://aj.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://bv.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://vl.shxzukj.cn

Ruby: end - start                 # 返回秒数
来源：http://fb.chemitech.net.cn

C#:   (end - start).TotalSeconds
来源：http://dm.newstarts.cn

[J07] 比较两个日期
来源：http://ku.hnjuh.cn

Py:   d1 < d2;  d1 == d2
来源：http://lc.shxzskj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bz.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cm.bookmarksfly.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ro.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gn.shxzukj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rd.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pf.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://gs.asd995.cn

[J08] 提取年月日与星期
来源：http://dv.huixinmuqiang.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ei.521024.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://he.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ok.huanxung.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kn.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rd.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fb.9csxet.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qk.bookmarksfly.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ua.shxzukj.cn

[J09] 时区处理
来源：http://bb.shxzskj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://us.hahajie.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://eg.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yd.yuexingan06.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://pd.colortex.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jd.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://jh.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://hu.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gd.shxzskj.cn

[J10] 取今天 / 本月第一天
来源：http://sw.nszjky.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tg.lnxyls.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dc.521024.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rt.newstarts.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ww.haigaiapp.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ff.huixinmuqiang.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tj.asd995.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kx.lnxyls.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jy.szsharing.cn

================================================================================
来源：http://in.newstarts.cn

K. JSON 与序列化
来源：http://ea.huixiangedu.cn

================================================================================
来源：http://wb.jctech888.com.cn

[K01] 对象转 JSON 字符串
来源：http://rl.yuexingan06.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xk.shxzskj.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://du.szsharing.cn

JS:   JSON.stringify(obj)
来源：http://hw.jianghongdianzi.cn

TS:   JSON.stringify(obj)
来源：http://zr.lnxyls.cn


<!-- 参考信息 -->