代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://iy.huixinmuqiang.cn

Java: record User(String name, int age) {}
来源：http://fu.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://gz.szsharing.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ku.jianghongdianzi.cn

C#:   record User(string Name, int Age);
来源：http://je.jctech888.com.cn

[G15] 枚举
来源：http://vw.shxzskj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pj.shtwfgs.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nh.asd995.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pk.hahajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ra.nszjky.cn

Java: enum Color { RED, GREEN }
来源：http://rp.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://aq.muxihuayi.cn

Ruby: Color = %i[red green].freeze
来源：http://bw.yuexingan06.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sl.shxzskj.cn

[G16] 对象转数组 / 字典
来源：http://op.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hx.jctech888.com.cn

PHP:  get_object_vars($obj);
来源：http://vz.huanxung.cn

JS:   Object.entries(obj)
来源：http://mo.panjiajie.cn

TS:   Object.entries(obj)
来源：http://tr.gzmigu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wh.muxihuayi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hb.gzmigu.cn

Ruby: obj.instance_variables
来源：http://ay.gzmigu.cn

C#:   // 用反射或 System.Text.Json
来源：http://qu.colortex.cn

================================================================================
来源：http://lr.9csxet.cn

H. 异常与错误处理
来源：http://th.jctech888.com.cn

================================================================================
来源：http://qi.szsharing.cn

[H01] try / catch 基础
来源：http://dr.huixinmuqiang.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wj.9csxet.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kw.yuexingan06.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://kr.panjiajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yo.huixinmuqiang.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://gw.szsharing.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://jy.muxihuayi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://zb.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sp.huanxung.cn

[H02] finally / ensure 收尾
来源：http://ki.jianghongdianzi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://px.colortex.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://zf.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nb.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cl.jianghongdianzi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://af.muxihuayi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://cu.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ah.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yn.521024.cn

[H03] 主动抛出异常
来源：http://lp.chemitech.net.cn

Py:   raise ValueError("错误信息")
来源：http://rn.hahajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hi.colortex.cn

JS:   throw new Error("错误信息");
来源：http://lm.jctech888.com.cn

TS:   throw new Error("错误信息");
来源：http://zr.panjiajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://je.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cf.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://jz.newstarts.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vy.muxihuayi.cn

[H04] 自定义异常类型
来源：http://vd.jctech888.com.cn

Py:   class MyError(Exception): pass
来源：http://ww.shxzukj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kw.colortex.cn

JS:   class MyError extends Error {}
来源：http://el.huanxung.cn

TS:   class MyError extends Error {}
来源：http://cx.huixiangedu.cn

Java: class MyException extends RuntimeException {}
来源：http://gj.yuexingan06.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rp.haigaiapp.cn

Ruby: class MyError < StandardError; end
来源：http://aa.lnxyls.cn

C#:   class MyException : Exception {}
来源：http://hq.lnxyls.cn

[H05] 捕获特定类型
来源：http://wl.newstarts.cn

Py:   except ValueError as e:
来源：http://lu.bjjhwx.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gc.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://tj.asd995.cn

TS:   if (e instanceof TypeError) {}
来源：http://ge.9csxet.cn

Java: catch (IOException | SQLException e) {}
来源：http://ox.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ht.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://mw.nszjky.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hf.huanxung.cn

[H06] 可选值 / 空值安全访问
来源：http://tp.nicolike.cn

Py:   value = d.get("k") or default
来源：http://sj.szxytkj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://iv.bookmarksfly.cn

JS:   obj?.a?.b;  d ?? default
来源：http://id.bookmarksfly.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ho.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kc.nszjky.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://by.hahajie.cn

Ruby: d&.dig(:a, :b)
来源：http://ot.huanxung.cn

C#:   obj?.A?.B ?? default
来源：http://ik.muxihuayi.cn

[H07] 断言
来源：http://bv.yuexingan06.cn

Py:   assert x > 0, "必须为正"
来源：http://gl.chemitech.net.cn

PHP:  assert($x > 0);
来源：http://ek.huixiangedu.cn

JS:   console.assert(x > 0);
来源：http://pe.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://pi.lnxyls.cn

Java: assert x > 0 : "必须为正";
来源：http://am.shxzukj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://oj.nszjky.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bw.muxihuayi.cn

C#:   Debug.Assert(x > 0);
来源：http://yc.bjjhwx.cn

[H08] 获取错误信息与堆栈
来源：http://av.colortex.cn

Py:   str(e);  traceback.format_exc()
来源：http://rl.huanxung.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nm.panjiajie.cn

JS:   e.message;  e.stack
来源：http://vw.yuntaijiaju.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://rv.huanxung.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ps.colortex.cn

Go:   err.Error()
来源：http://oa.shxzskj.cn

Ruby: e.message;  e.backtrace
来源：http://ro.yuntaijiaju.cn

C#:   e.Message;  e.StackTrace
来源：http://ke.shtwfgs.cn

[H09] 带错误码的异常
来源：http://er.colortex.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://rr.521024.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nj.bjjhwx.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kl.huixinmuqiang.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ik.nszjky.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wh.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kp.panjiajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://at.haigaiapp.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qd.hahajie.cn

[H10] 资源自动释放
来源：http://gg.jianghongdianzi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rs.9csxet.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sy.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cy.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://zd.huixinmuqiang.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dv.szsharing.cn

Go:   defer f.Close()
来源：http://dh.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rn.jianghongdianzi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cf.muxihuayi.cn

================================================================================
来源：http://qh.nszjky.cn

I. 正则表达式
来源：http://wz.muxihuayi.cn

================================================================================
来源：http://xh.yuexingan06.cn

[I01] 判断是否匹配
来源：http://ak.szsharing.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ua.muxihuayi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://aq.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://js.hnjuh.cn

TS:   /\d+/.test(s)
来源：http://cd.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://xe.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mr.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://gf.nicolike.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cv.nicolike.cn

[I02] 提取所有匹配
来源：http://ri.shxzskj.cn

Py:   re.findall(r"\d+", s)
来源：http://jd.szsharing.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://qc.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cl.szxytkj.cn

TS:   s.match(/\d+/g)
来源：http://gf.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ot.9csxet.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://vm.yuexingan06.cn

Ruby: s.scan(/\d+/)
来源：http://ts.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://kr.huanxung.cn

[I03] 提取捕获分组
来源：http://bb.gzmigu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ep.lnxyls.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qp.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nu.huixinmuqiang.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ym.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ox.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://eo.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://kv.shxzskj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xt.nszjky.cn

[I04] 正则替换
来源：http://sm.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hm.szsharing.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bv.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cd.lnxyls.cn

TS:   s.replace(/\d+/g, "#")
来源：http://cg.gzmigu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bt.huixiangedu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ga.haigaiapp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yd.shxzukj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://rg.panjiajie.cn

[I05] 按正则拆分
来源：http://uu.bookmarksfly.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gb.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ep.colortex.cn

JS:   s.split(/\s*,\s*/)
来源：http://vk.jctech888.com.cn

TS:   s.split(/\s*,\s*/)
来源：http://sk.hnjuh.cn

Java: s.split("\\s*,\\s*")
来源：http://qd.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://or.asd995.cn

Ruby: s.split(/\s*,\s*/)
来源：http://vh.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ty.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://gr.szsharing.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://pa.huixiangedu.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hk.colortex.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qw.newstarts.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://cu.newstarts.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://er.bjjhwx.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fc.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vo.hnjuh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://dn.asd995.cn

[I07] 忽略大小写与多行模式
来源：http://kc.haigaiapp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://rg.jianghongdianzi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://rc.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yt.huixinmuqiang.cn

TS:   /error/gim
来源：http://hq.bjjhwx.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ql.9csxet.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://kq.colortex.cn

Ruby: s.scan(/error/i)
来源：http://ss.hahajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://pf.wgjwhj.cn

[I08] 贪婪与非贪婪匹配
来源：http://yz.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kw.szsharing.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xx.huanxung.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xt.huixinmuqiang.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jj.huanxung.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ze.521024.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ph.yuntaijiaju.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ko.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://py.521024.cn

================================================================================
来源：http://pa.wgjwhj.cn

J. 日期与时间
来源：http://hy.wgjwhj.cn

================================================================================
来源：http://va.hnjuh.cn

[J01] 获取当前时间
来源：http://yu.9csxet.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://id.newstarts.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jw.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://kp.hahajie.cn

TS:   new Date();  Date.now()
来源：http://hn.chemitech.net.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ue.lnxyls.cn

Go:   time.Now()
来源：http://xf.521024.cn

Ruby: Time.now
来源：http://jj.lnxyls.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://es.lnxyls.cn

[J02] 格式化输出
来源：http://up.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bu.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://po.asd995.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://dl.huixinmuqiang.cn

TS:   d.toISOString()
来源：http://nu.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jb.hahajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rn.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://if.nszjky.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ez.yuexingan06.cn

[J03] 字符串解析为日期
来源：http://hc.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://yg.jctech888.com.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://jo.newstarts.cn

JS:   new Date("2024-01-02")
来源：http://iv.shtwfgs.cn

TS:   new Date("2024-01-02")
来源：http://vo.yuexingan06.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ai.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ve.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://ic.bjjhwx.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://it.9csxet.cn

[J04] 时间戳与日期互转
来源：http://cs.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rr.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iv.szsharing.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qv.shtwfgs.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://au.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yh.chemitech.net.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ae.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nt.newstarts.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ih.shxzskj.cn

[J05] 时间加减（加 7 天）
来源：http://ux.nicolike.cn

Py:   now + timedelta(days=7)
来源：http://sg.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dr.nszjky.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://jd.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bh.muxihuayi.cn

Java: LocalDate.now().plusDays(7)
来源：http://vn.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ja.shxzskj.cn

Ruby: Time.now + 7 * 86400
来源：http://bh.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gw.shxzukj.cn

[J06] 计算两时间之差
来源：http://fg.chemitech.net.cn

Py:   (end - start).total_seconds()
来源：http://pz.yuexingan06.cn

PHP:  $end->diff($start)->days;
来源：http://gl.bookmarksfly.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mo.hahajie.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://th.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lp.muxihuayi.cn

Go:   end.Sub(start).Hours()
来源：http://ej.huanxung.cn

Ruby: end - start                 # 返回秒数
来源：http://ys.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://vq.521024.cn

[J07] 比较两个日期
来源：http://xu.szsharing.cn

Py:   d1 < d2;  d1 == d2
来源：http://yx.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bj.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vg.nszjky.cn

TS:   d1.getTime() < d2.getTime()
来源：http://up.shtwfgs.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pd.shxzukj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ge.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://sw.hnjuh.cn

C#:   d1 < d2;  d1 == d2
来源：http://gq.bookmarksfly.cn

[J08] 提取年月日与星期
来源：http://xn.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xy.szxytkj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cp.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ep.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hw.shxzukj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://es.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uv.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://us.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vw.shxzskj.cn

[J09] 时区处理
来源：http://lo.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cu.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://gk.9csxet.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yc.jctech888.com.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lv.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://my.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://gc.shxzukj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ay.jianghongdianzi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mt.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://aq.hnjuh.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bn.jianghongdianzi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kx.521024.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://rp.nszjky.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wn.hnjuh.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jb.hahajie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sq.bjjhwx.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vm.bjjhwx.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jf.muxihuayi.cn

================================================================================
来源：http://cy.shxzukj.cn

K. JSON 与序列化
来源：http://rj.lnxyls.cn

================================================================================
来源：http://ii.yuntaijiaju.cn

[K01] 对象转 JSON 字符串
来源：http://rc.jianghongdianzi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://la.szsharing.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pp.muxihuayi.cn

JS:   JSON.stringify(obj)
来源：http://sf.bookmarksfly.cn

TS:   JSON.stringify(obj)
来源：http://zx.bookmarksfly.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ww.szsharing.cn

Go:   json.Marshal(obj)
来源：http://qc.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jc.bookmarksfly.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ys.521024.cn

[K02] JSON 字符串转对象
来源：http://ug.yuexingan06.cn

Py:   json.loads(s)
来源：http://yv.nszjky.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dl.colortex.cn

JS:   JSON.parse(s)
来源：http://fq.shxzukj.cn


<!-- 参考信息 -->