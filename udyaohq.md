代发 wailian999

Py:   isinstance(u, User)
来源：http://oi.wgjwhj.cn

PHP:  $u instanceof User
来源：http://kz.shxzskj.cn

JS:   u instanceof User
来源：http://bk.shxzukj.cn

TS:   u instanceof User
来源：http://wg.nicolike.cn

Java: u instanceof User
来源：http://cz.huixiangedu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://re.9csxet.cn

Ruby: u.is_a?(User)
来源：http://bw.huixinmuqiang.cn

C#:   u is User
来源：http://ii.colortex.cn

[G14] 数据类 / record
来源：http://ym.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vd.bookmarksfly.cn

PHP:  // 用 readonly 属性模拟
来源：http://mo.huanxung.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nh.hnjuh.cn

TS:   type User = { name: string; age: number };
来源：http://ug.hahajie.cn

Java: record User(String name, int age) {}
来源：http://ld.colortex.cn

Go:   type User struct { Name string; Age int }
来源：http://yh.hnjuh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ba.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://aj.huanxung.cn

[G15] 枚举
来源：http://ku.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ea.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wm.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rm.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xe.yuntaijiaju.cn

Java: enum Color { RED, GREEN }
来源：http://zg.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rq.shxzukj.cn

Ruby: Color = %i[red green].freeze
来源：http://wk.shxzukj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ik.shxzskj.cn

[G16] 对象转数组 / 字典
来源：http://br.szxytkj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sd.newstarts.cn

PHP:  get_object_vars($obj);
来源：http://ch.panjiajie.cn

JS:   Object.entries(obj)
来源：http://ra.9csxet.cn

TS:   Object.entries(obj)
来源：http://kk.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://db.nicolike.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ou.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://at.9csxet.cn

C#:   // 用反射或 System.Text.Json
来源：http://mw.shtwfgs.cn

================================================================================
来源：http://yr.hnjuh.cn

H. 异常与错误处理
来源：http://gw.szxytkj.cn

================================================================================
来源：http://vh.gzmigu.cn

[H01] try / catch 基础
来源：http://ag.shxzskj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vf.asd995.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qr.nicolike.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://nf.shxzskj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ae.wgjwhj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://un.szsharing.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ay.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ac.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iu.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://oi.nicolike.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sc.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hy.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hv.muxihuayi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tk.jianghongdianzi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://fm.szxytkj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zm.yuexingan06.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sw.yuntaijiaju.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xj.colortex.cn

[H03] 主动抛出异常
来源：http://vy.shxzukj.cn

Py:   raise ValueError("错误信息")
来源：http://yq.wgjwhj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uh.hnjuh.cn

JS:   throw new Error("错误信息");
来源：http://ox.yuexingan06.cn

TS:   throw new Error("错误信息");
来源：http://mz.9csxet.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://tg.huanxung.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xy.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://um.szsharing.cn

C#:   throw new ArgumentException("错误信息");
来源：http://es.9csxet.cn

[H04] 自定义异常类型
来源：http://dy.nicolike.cn

Py:   class MyError(Exception): pass
来源：http://ek.shxzukj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ef.nicolike.cn

JS:   class MyError extends Error {}
来源：http://kz.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://qq.panjiajie.cn

Java: class MyException extends RuntimeException {}
来源：http://vv.jianghongdianzi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nd.gzmigu.cn

Ruby: class MyError < StandardError; end
来源：http://um.hnjuh.cn

C#:   class MyException : Exception {}
来源：http://pf.shtwfgs.cn

[H05] 捕获特定类型
来源：http://ud.chemitech.net.cn

Py:   except ValueError as e:
来源：http://md.shxzukj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vp.newstarts.cn

JS:   if (e instanceof TypeError) {}
来源：http://pk.521024.cn

TS:   if (e instanceof TypeError) {}
来源：http://kz.panjiajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://ir.yuntaijiaju.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zk.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://dd.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ew.haigaiapp.cn

[H06] 可选值 / 空值安全访问
来源：http://ns.bookmarksfly.cn

Py:   value = d.get("k") or default
来源：http://oi.521024.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vp.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ql.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zl.jianghongdianzi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cy.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://de.yuexingan06.cn

Ruby: d&.dig(:a, :b)
来源：http://ya.huanxung.cn

C#:   obj?.A?.B ?? default
来源：http://bt.huanxung.cn

[H07] 断言
来源：http://nd.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://ad.newstarts.cn

PHP:  assert($x > 0);
来源：http://ll.wgjwhj.cn

JS:   console.assert(x > 0);
来源：http://ae.521024.cn

TS:   console.assert(x > 0);
来源：http://nj.hnjuh.cn

Java: assert x > 0 : "必须为正";
来源：http://xg.jianghongdianzi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kd.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ae.lnxyls.cn

C#:   Debug.Assert(x > 0);
来源：http://xv.9csxet.cn

[H08] 获取错误信息与堆栈
来源：http://xc.huanxung.cn

Py:   str(e);  traceback.format_exc()
来源：http://ig.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bh.lnxyls.cn

JS:   e.message;  e.stack
来源：http://mv.wgjwhj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ha.colortex.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://oa.hahajie.cn

Go:   err.Error()
来源：http://jd.jctech888.com.cn

Ruby: e.message;  e.backtrace
来源：http://ry.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://mr.lnxyls.cn

[H09] 带错误码的异常
来源：http://ya.shxzukj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fz.huanxung.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://zp.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sv.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gs.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ug.colortex.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://or.nszjky.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jx.chemitech.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ad.yuexingan06.cn

[H10] 资源自动释放
来源：http://aa.yuexingan06.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sq.asd995.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cv.jctech888.com.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tv.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ux.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mz.bookmarksfly.cn

Go:   defer f.Close()
来源：http://pc.szxytkj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pc.yuntaijiaju.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://pm.9csxet.cn

================================================================================
来源：http://ev.hnjuh.cn

I. 正则表达式
来源：http://fl.huixinmuqiang.cn

================================================================================
来源：http://mg.huixiangedu.cn

[I01] 判断是否匹配
来源：http://hu.colortex.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cg.shxzukj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://on.nicolike.cn

JS:   /\d+/.test(s)
来源：http://zi.9csxet.cn

TS:   /\d+/.test(s)
来源：http://ip.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yd.huanxung.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://it.bookmarksfly.cn

Ruby: s.match?(/\d+/)
来源：http://jz.huanxung.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vi.hnjuh.cn

[I02] 提取所有匹配
来源：http://gh.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://zb.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ay.bjjhwx.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ac.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://ny.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://el.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mh.521024.cn

Ruby: s.scan(/\d+/)
来源：http://qx.nicolike.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://aw.wgjwhj.cn

[I03] 提取捕获分组
来源：http://le.521024.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bv.jianghongdianzi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pc.nszjky.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uc.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ax.huixiangedu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://co.nszjky.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ha.szxytkj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://yd.huanxung.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fe.szxytkj.cn

[I04] 正则替换
来源：http://tc.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://zp.jctech888.com.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ut.nszjky.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pf.shtwfgs.cn

TS:   s.replace(/\d+/g, "#")
来源：http://da.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kf.huanxung.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bp.jctech888.com.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ui.asd995.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://no.haigaiapp.cn

[I05] 按正则拆分
来源：http://pn.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fc.521024.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xf.bookmarksfly.cn

JS:   s.split(/\s*,\s*/)
来源：http://an.jctech888.com.cn

TS:   s.split(/\s*,\s*/)
来源：http://vt.szxytkj.cn

Java: s.split("\\s*,\\s*")
来源：http://rz.yuntaijiaju.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fb.bjjhwx.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mw.newstarts.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mc.haigaiapp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kl.haigaiapp.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://lz.haigaiapp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sb.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uy.nicolike.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cw.panjiajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uu.muxihuayi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wt.yuexingan06.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dl.521024.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uh.shxzukj.cn

[I07] 忽略大小写与多行模式
来源：http://xf.lnxyls.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ge.huixinmuqiang.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://cj.chemitech.net.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sw.gzmigu.cn

TS:   /error/gim
来源：http://up.yuntaijiaju.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hu.asd995.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sn.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://fq.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://io.colortex.cn

[I08] 贪婪与非贪婪匹配
来源：http://rw.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://di.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ua.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bk.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://qt.hnjuh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://xr.szxytkj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://jx.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ve.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uw.nszjky.cn

================================================================================
来源：http://vh.asd995.cn

J. 日期与时间
来源：http://av.newstarts.cn

================================================================================
来源：http://cv.shxzskj.cn

[J01] 获取当前时间
来源：http://fo.9csxet.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rd.huixinmuqiang.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://nk.wgjwhj.cn

JS:   new Date();  Date.now()
来源：http://nq.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://rf.szxytkj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vy.haigaiapp.cn

Go:   time.Now()
来源：http://jn.shtwfgs.cn

Ruby: Time.now
来源：http://yj.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zy.asd995.cn

[J02] 格式化输出
来源：http://pn.shxzukj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rc.jctech888.com.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ke.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://zz.bookmarksfly.cn

TS:   d.toISOString()
来源：http://ts.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://wh.nicolike.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://op.shtwfgs.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pk.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://xb.shxzukj.cn

[J03] 字符串解析为日期
来源：http://cc.bookmarksfly.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yz.hahajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://aj.shxzskj.cn

JS:   new Date("2024-01-02")
来源：http://wq.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://jc.bjjhwx.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mw.chemitech.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jq.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://mn.jianghongdianzi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lq.nszjky.cn

[J04] 时间戳与日期互转
来源：http://gc.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://pa.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ey.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tm.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://wq.hnjuh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jk.hnjuh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pi.wgjwhj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gw.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yw.nszjky.cn

[J05] 时间加减（加 7 天）
来源：http://dt.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://jg.wgjwhj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cb.521024.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mu.hahajie.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://oq.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://wb.hahajie.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pd.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://ha.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://sc.bjjhwx.cn

[J06] 计算两时间之差
来源：http://kx.panjiajie.cn

Py:   (end - start).total_seconds()
来源：http://sl.jctech888.com.cn

PHP:  $end->diff($start)->days;
来源：http://vj.shtwfgs.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://td.bjjhwx.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fe.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://mv.shxzukj.cn

Go:   end.Sub(start).Hours()
来源：http://kn.haigaiapp.cn

Ruby: end - start                 # 返回秒数
来源：http://iu.szxytkj.cn

C#:   (end - start).TotalSeconds
来源：http://lz.gzmigu.cn

[J07] 比较两个日期
来源：http://mc.chemitech.net.cn

Py:   d1 < d2;  d1 == d2
来源：http://xi.lnxyls.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rb.jctech888.com.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ru.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://bp.newstarts.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gf.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tr.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://cf.bjjhwx.cn

C#:   d1 < d2;  d1 == d2
来源：http://xt.panjiajie.cn

[J08] 提取年月日与星期
来源：http://sm.521024.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yw.huanxung.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://yf.bjjhwx.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://li.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ob.yuexingan06.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zv.521024.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gv.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zc.shtwfgs.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://em.nszjky.cn

[J09] 时区处理
来源：http://zx.jctech888.com.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ss.shxzukj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ao.muxihuayi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fy.szsharing.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sq.yuexingan06.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://zw.bjjhwx.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ld.asd995.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wn.huixinmuqiang.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oc.muxihuayi.cn

[J10] 取今天 / 本月第一天
来源：http://kv.huixiangedu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jb.asd995.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dv.szxytkj.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://fv.colortex.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bz.nicolike.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bz.huixinmuqiang.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gh.panjiajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://um.521024.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wk.gzmigu.cn

================================================================================
来源：http://yn.szsharing.cn

K. JSON 与序列化
来源：http://dj.panjiajie.cn

================================================================================
来源：http://ng.szxytkj.cn

[K01] 对象转 JSON 字符串
来源：http://qb.521024.cn


<!-- 参考信息 -->