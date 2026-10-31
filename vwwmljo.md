代发 wailian999

Py:   isinstance(u, User)
来源：http://ht.huanxung.cn

PHP:  $u instanceof User
来源：http://qm.bjjhwx.cn

JS:   u instanceof User
来源：http://gw.asd995.cn

TS:   u instanceof User
来源：http://to.hahajie.cn

Java: u instanceof User
来源：http://ly.gzmigu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://uc.shxzukj.cn

Ruby: u.is_a?(User)
来源：http://ij.gzmigu.cn

C#:   u is User
来源：http://er.yuexingan06.cn

[G14] 数据类 / record
来源：http://hv.panjiajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://md.9csxet.cn

PHP:  // 用 readonly 属性模拟
来源：http://di.hnjuh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gb.wgjwhj.cn

TS:   type User = { name: string; age: number };
来源：http://rz.bookmarksfly.cn

Java: record User(String name, int age) {}
来源：http://et.shxzskj.cn

Go:   type User struct { Name string; Age int }
来源：http://sr.huixiangedu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://eh.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://nl.9csxet.cn

[G15] 枚举
来源：http://tk.chemitech.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bg.jianghongdianzi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://tq.gzmigu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qy.huanxung.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ix.521024.cn

Java: enum Color { RED, GREEN }
来源：http://ti.shtwfgs.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ha.newstarts.cn

Ruby: Color = %i[red green].freeze
来源：http://so.hahajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dw.9csxet.cn

[G16] 对象转数组 / 字典
来源：http://qx.asd995.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://dm.hnjuh.cn

PHP:  get_object_vars($obj);
来源：http://ui.jctech888.com.cn

JS:   Object.entries(obj)
来源：http://er.huanxung.cn

TS:   Object.entries(obj)
来源：http://sd.szsharing.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fa.wgjwhj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://py.hnjuh.cn

Ruby: obj.instance_variables
来源：http://ab.lnxyls.cn

C#:   // 用反射或 System.Text.Json
来源：http://dq.shtwfgs.cn

================================================================================
来源：http://gz.muxihuayi.cn

H. 异常与错误处理
来源：http://ex.shxzskj.cn

================================================================================
来源：http://hf.panjiajie.cn

[H01] try / catch 基础
来源：http://hq.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qm.haigaiapp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nd.shtwfgs.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ma.jctech888.com.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tl.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://up.jctech888.com.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jd.yuntaijiaju.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://et.muxihuayi.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xk.521024.cn

[H02] finally / ensure 收尾
来源：http://at.hnjuh.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fn.newstarts.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ti.jctech888.com.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://uh.wgjwhj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://it.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zy.521024.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://on.521024.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kp.huanxung.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://dh.newstarts.cn

[H03] 主动抛出异常
来源：http://gk.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://bm.shxzukj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yp.nicolike.cn

JS:   throw new Error("错误信息");
来源：http://ex.huanxung.cn

TS:   throw new Error("错误信息");
来源：http://ey.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qd.gzmigu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://oa.nicolike.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://pe.lnxyls.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nn.521024.cn

[H04] 自定义异常类型
来源：http://ke.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://bw.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://or.nszjky.cn

JS:   class MyError extends Error {}
来源：http://kx.nszjky.cn

TS:   class MyError extends Error {}
来源：http://nh.chemitech.net.cn

Java: class MyException extends RuntimeException {}
来源：http://rs.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eb.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://av.huixiangedu.cn

C#:   class MyException : Exception {}
来源：http://wh.huixinmuqiang.cn

[H05] 捕获特定类型
来源：http://jo.shxzukj.cn

Py:   except ValueError as e:
来源：http://zb.shxzskj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xl.jianghongdianzi.cn

JS:   if (e instanceof TypeError) {}
来源：http://hq.newstarts.cn

TS:   if (e instanceof TypeError) {}
来源：http://mh.jianghongdianzi.cn

Java: catch (IOException | SQLException e) {}
来源：http://qq.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ay.szsharing.cn

Ruby: rescue ArgumentError => e
来源：http://qf.nicolike.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://rc.chemitech.net.cn

[H06] 可选值 / 空值安全访问
来源：http://ac.muxihuayi.cn

Py:   value = d.get("k") or default
来源：http://ky.huixinmuqiang.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ll.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ks.szsharing.cn

TS:   obj?.a?.b;  d ?? default
来源：http://eq.bookmarksfly.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://er.wgjwhj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ca.chemitech.net.cn

Ruby: d&.dig(:a, :b)
来源：http://pb.yuexingan06.cn

C#:   obj?.A?.B ?? default
来源：http://sa.nicolike.cn

[H07] 断言
来源：http://hj.jctech888.com.cn

Py:   assert x > 0, "必须为正"
来源：http://wm.szsharing.cn

PHP:  assert($x > 0);
来源：http://cs.gzmigu.cn

JS:   console.assert(x > 0);
来源：http://hl.lnxyls.cn

TS:   console.assert(x > 0);
来源：http://rq.huanxung.cn

Java: assert x > 0 : "必须为正";
来源：http://th.szsharing.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://sw.bjjhwx.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ue.shxzskj.cn

C#:   Debug.Assert(x > 0);
来源：http://kg.chemitech.net.cn

[H08] 获取错误信息与堆栈
来源：http://ew.wgjwhj.cn

Py:   str(e);  traceback.format_exc()
来源：http://zs.huanxung.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tp.wgjwhj.cn

JS:   e.message;  e.stack
来源：http://og.shtwfgs.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lz.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://by.muxihuayi.cn

Go:   err.Error()
来源：http://qx.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://ip.chemitech.net.cn

C#:   e.Message;  e.StackTrace
来源：http://fq.gzmigu.cn

[H09] 带错误码的异常
来源：http://gi.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zx.colortex.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qo.bjjhwx.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uy.muxihuayi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ha.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://tn.huixiangedu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rg.huanxung.cn

Ruby: raise MyError.new("fail", 500)
来源：http://gh.shxzukj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://iq.huixinmuqiang.cn

[H10] 资源自动释放
来源：http://il.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://vd.huixinmuqiang.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yx.9csxet.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kh.9csxet.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tr.bjjhwx.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qh.nicolike.cn

Go:   defer f.Close()
来源：http://yx.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://aj.colortex.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gu.szsharing.cn

================================================================================
来源：http://mu.shxzskj.cn

I. 正则表达式
来源：http://nt.haigaiapp.cn

================================================================================
来源：http://nx.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://fw.haigaiapp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yq.newstarts.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dj.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://vx.jctech888.com.cn

TS:   /\d+/.test(s)
来源：http://oz.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vl.colortex.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://xy.haigaiapp.cn

Ruby: s.match?(/\d+/)
来源：http://pq.muxihuayi.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bp.nszjky.cn

[I02] 提取所有匹配
来源：http://zf.gzmigu.cn

Py:   re.findall(r"\d+", s)
来源：http://dg.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yc.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qw.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://lb.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ek.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yn.muxihuayi.cn

Ruby: s.scan(/\d+/)
来源：http://sh.muxihuayi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kt.nicolike.cn

[I03] 提取捕获分组
来源：http://eb.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://iq.nicolike.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hj.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://me.colortex.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wu.huixiangedu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ok.newstarts.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://kb.huixiangedu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nd.shxzskj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lj.9csxet.cn

[I04] 正则替换
来源：http://ns.huixinmuqiang.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vy.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fj.huixiangedu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://nx.hahajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://mo.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qm.wgjwhj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hj.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sc.colortex.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ed.shtwfgs.cn

[I05] 按正则拆分
来源：http://do.huixinmuqiang.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://oy.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tl.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://oz.asd995.cn

TS:   s.split(/\s*,\s*/)
来源：http://fc.yuexingan06.cn

Java: s.split("\\s*,\\s*")
来源：http://zt.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yk.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://xw.panjiajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zt.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zt.huanxung.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://tk.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://kk.shtwfgs.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ul.muxihuayi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://om.shxzskj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zu.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ua.asd995.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.colortex.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ur.jctech888.com.cn

[I07] 忽略大小写与多行模式
来源：http://sf.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tf.jianghongdianzi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ol.521024.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nw.haigaiapp.cn

TS:   /error/gim
来源：http://hw.lnxyls.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bu.hnjuh.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hf.gzmigu.cn

Ruby: s.scan(/error/i)
来源：http://rt.jianghongdianzi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qa.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://rq.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ii.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nz.shxzukj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ez.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vi.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://kt.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gz.jctech888.com.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qu.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://sn.yuntaijiaju.cn

================================================================================
来源：http://sy.shxzskj.cn

J. 日期与时间
来源：http://jv.521024.cn

================================================================================
来源：http://kl.shxzukj.cn

[J01] 获取当前时间
来源：http://yv.huanxung.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hs.newstarts.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sd.asd995.cn

JS:   new Date();  Date.now()
来源：http://sm.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://ne.gzmigu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pu.yuntaijiaju.cn

Go:   time.Now()
来源：http://ag.shxzskj.cn

Ruby: Time.now
来源：http://bp.szsharing.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qc.shxzukj.cn

[J02] 格式化输出
来源：http://lc.yuexingan06.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qr.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://de.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://bn.521024.cn

TS:   d.toISOString()
来源：http://kw.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ya.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vy.jctech888.com.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vi.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ir.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://hv.muxihuayi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ma.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kz.shxzskj.cn

JS:   new Date("2024-01-02")
来源：http://nm.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://pe.hahajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://dk.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tk.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://kl.9csxet.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dq.521024.cn

[J04] 时间戳与日期互转
来源：http://bv.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://qj.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yx.newstarts.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hv.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ri.szxytkj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://do.huanxung.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ol.wgjwhj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nv.muxihuayi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yn.huanxung.cn

[J05] 时间加减（加 7 天）
来源：http://pp.asd995.cn

Py:   now + timedelta(days=7)
来源：http://iq.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xx.haigaiapp.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cm.yuexingan06.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ao.yuntaijiaju.cn

Java: LocalDate.now().plusDays(7)
来源：http://jo.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://la.9csxet.cn

Ruby: Time.now + 7 * 86400
来源：http://hd.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gd.shxzskj.cn

[J06] 计算两时间之差
来源：http://sb.szxytkj.cn

Py:   (end - start).total_seconds()
来源：http://mc.yuntaijiaju.cn

PHP:  $end->diff($start)->days;
来源：http://rp.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ud.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vj.jctech888.com.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dd.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://hk.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://xt.nszjky.cn

C#:   (end - start).TotalSeconds
来源：http://wh.huixiangedu.cn

[J07] 比较两个日期
来源：http://ao.bjjhwx.cn

Py:   d1 < d2;  d1 == d2
来源：http://qr.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://fk.hnjuh.cn

JS:   d1.getTime() < d2.getTime()
来源：http://dt.newstarts.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gp.asd995.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ec.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://if.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wx.yuntaijiaju.cn

C#:   d1 < d2;  d1 == d2
来源：http://ba.szxytkj.cn

[J08] 提取年月日与星期
来源：http://fy.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ql.huanxung.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://be.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rc.bjjhwx.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://mt.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://an.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bq.muxihuayi.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fq.shxzskj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lu.yuexingan06.cn

[J09] 时区处理
来源：http://we.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xa.newstarts.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fp.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lx.newstarts.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jq.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://li.yuexingan06.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pv.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://uu.gzmigu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://su.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://ny.chemitech.net.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ya.nszjky.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://qg.shxzskj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kd.shtwfgs.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xc.shxzskj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://et.haigaiapp.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wz.asd995.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://tj.yuntaijiaju.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xo.wgjwhj.cn

================================================================================
来源：http://ad.yuntaijiaju.cn

K. JSON 与序列化
来源：http://gv.bookmarksfly.cn

================================================================================
来源：http://mm.lnxyls.cn

[K01] 对象转 JSON 字符串
来源：http://cf.szsharing.cn


<!-- 参考信息 -->