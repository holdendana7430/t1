代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://ms.gzmigu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://cn.shxzukj.cn

[G16] 对象转数组 / 字典
来源：http://no.huixiangedu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://sv.muxihuayi.cn

PHP:  get_object_vars($obj);
来源：http://zx.haigaiapp.cn

JS:   Object.entries(obj)
来源：http://sm.hnjuh.cn

TS:   Object.entries(obj)
来源：http://cf.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sc.hnjuh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kd.huanxung.cn

Ruby: obj.instance_variables
来源：http://af.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://qx.bjjhwx.cn

================================================================================
来源：http://so.huixinmuqiang.cn

H. 异常与错误处理
来源：http://yb.nicolike.cn

================================================================================
来源：http://ch.panjiajie.cn

[H01] try / catch 基础
来源：http://gf.szxytkj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uv.shtwfgs.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://od.bookmarksfly.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ny.chemitech.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fn.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ei.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://bv.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sv.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sq.huixinmuqiang.cn

[H02] finally / ensure 收尾
来源：http://vu.jctech888.com.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ad.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sb.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hf.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bd.szxytkj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://jl.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gi.wgjwhj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ic.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ph.shxzskj.cn

[H03] 主动抛出异常
来源：http://mp.shtwfgs.cn

Py:   raise ValueError("错误信息")
来源：http://yu.panjiajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qp.hahajie.cn

JS:   throw new Error("错误信息");
来源：http://ti.haigaiapp.cn

TS:   throw new Error("错误信息");
来源：http://gc.haigaiapp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://md.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://af.wgjwhj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xw.9csxet.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qo.szsharing.cn

[H04] 自定义异常类型
来源：http://mj.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://ed.szxytkj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rr.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://lo.nicolike.cn

TS:   class MyError extends Error {}
来源：http://xv.huixiangedu.cn

Java: class MyException extends RuntimeException {}
来源：http://ja.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gm.chemitech.net.cn

Ruby: class MyError < StandardError; end
来源：http://bf.szsharing.cn

C#:   class MyException : Exception {}
来源：http://ck.521024.cn

[H05] 捕获特定类型
来源：http://lu.jianghongdianzi.cn

Py:   except ValueError as e:
来源：http://zz.huixiangedu.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vy.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://kl.jctech888.com.cn

TS:   if (e instanceof TypeError) {}
来源：http://sd.panjiajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://ax.yuntaijiaju.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://su.bookmarksfly.cn

Ruby: rescue ArgumentError => e
来源：http://in.yuexingan06.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ha.bjjhwx.cn

[H06] 可选值 / 空值安全访问
来源：http://gs.9csxet.cn

Py:   value = d.get("k") or default
来源：http://ql.szxytkj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://uu.panjiajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://oe.haigaiapp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ql.haigaiapp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fm.521024.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ru.bookmarksfly.cn

Ruby: d&.dig(:a, :b)
来源：http://np.yuexingan06.cn

C#:   obj?.A?.B ?? default
来源：http://zp.hahajie.cn

[H07] 断言
来源：http://au.hahajie.cn

Py:   assert x > 0, "必须为正"
来源：http://dj.szxytkj.cn

PHP:  assert($x > 0);
来源：http://gk.yuexingan06.cn

JS:   console.assert(x > 0);
来源：http://gy.nszjky.cn

TS:   console.assert(x > 0);
来源：http://rh.jianghongdianzi.cn

Java: assert x > 0 : "必须为正";
来源：http://bx.asd995.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ce.hnjuh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://bi.chemitech.net.cn

C#:   Debug.Assert(x > 0);
来源：http://bx.haigaiapp.cn

[H08] 获取错误信息与堆栈
来源：http://me.szxytkj.cn

Py:   str(e);  traceback.format_exc()
来源：http://cy.shtwfgs.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cb.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://om.shtwfgs.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hv.bjjhwx.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uo.nicolike.cn

Go:   err.Error()
来源：http://jq.colortex.cn

Ruby: e.message;  e.backtrace
来源：http://ef.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://zf.huixiangedu.cn

[H09] 带错误码的异常
来源：http://ea.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jp.hnjuh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qz.bookmarksfly.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://op.shtwfgs.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ox.huixiangedu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gu.nszjky.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://nc.gzmigu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vo.shtwfgs.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://id.nicolike.cn

[H10] 资源自动释放
来源：http://bj.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kt.szsharing.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gg.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bz.lnxyls.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ym.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pd.hahajie.cn

Go:   defer f.Close()
来源：http://ik.yuexingan06.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kj.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hm.huixinmuqiang.cn

================================================================================
来源：http://yy.bookmarksfly.cn

I. 正则表达式
来源：http://rx.yuntaijiaju.cn

================================================================================
来源：http://fm.shxzskj.cn

[I01] 判断是否匹配
来源：http://lk.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yu.yuexingan06.cn

PHP:  preg_match('/\d+/', $s);
来源：http://dx.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://sf.newstarts.cn

TS:   /\d+/.test(s)
来源：http://lg.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hn.nszjky.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ku.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://ls.gzmigu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://tn.shxzukj.cn

[I02] 提取所有匹配
来源：http://mu.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://yp.nszjky.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://th.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ss.szsharing.cn

TS:   s.match(/\d+/g)
来源：http://ad.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tn.huanxung.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://am.gzmigu.cn

Ruby: s.scan(/\d+/)
来源：http://bq.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vj.wgjwhj.cn

[I03] 提取捕获分组
来源：http://na.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nx.hnjuh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xi.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://of.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pc.jctech888.com.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gd.lnxyls.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wc.chemitech.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ne.szsharing.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://wk.yuntaijiaju.cn

[I04] 正则替换
来源：http://hh.newstarts.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sz.wgjwhj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jt.shxzukj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hp.yuexingan06.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ro.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qx.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://vo.huanxung.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ft.bjjhwx.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lj.shxzskj.cn

[I05] 按正则拆分
来源：http://bx.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hw.hahajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://lt.huixinmuqiang.cn

JS:   s.split(/\s*,\s*/)
来源：http://uw.yuexingan06.cn

TS:   s.split(/\s*,\s*/)
来源：http://bl.haigaiapp.cn

Java: s.split("\\s*,\\s*")
来源：http://vo.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yr.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ha.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://uj.yuexingan06.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tv.shxzukj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fj.chemitech.net.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xx.asd995.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sv.muxihuayi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://al.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://vk.shxzskj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pz.asd995.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pz.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wt.szsharing.cn

[I07] 忽略大小写与多行模式
来源：http://wq.haigaiapp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yc.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fc.shxzukj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://jo.gzmigu.cn

TS:   /error/gim
来源：http://bh.nicolike.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ze.shxzukj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jn.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://ii.hahajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://uq.gzmigu.cn

[I08] 贪婪与非贪婪匹配
来源：http://ns.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jt.nszjky.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://cr.huixiangedu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ca.shtwfgs.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ok.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ub.huixiangedu.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://km.hnjuh.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pd.szxytkj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xr.jctech888.com.cn

================================================================================
来源：http://sp.szsharing.cn

J. 日期与时间
来源：http://wa.colortex.cn

================================================================================
来源：http://dl.asd995.cn

[J01] 获取当前时间
来源：http://vw.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://sl.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://up.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://dx.asd995.cn

TS:   new Date();  Date.now()
来源：http://po.hnjuh.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mp.jctech888.com.cn

Go:   time.Now()
来源：http://io.huixiangedu.cn

Ruby: Time.now
来源：http://mf.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pv.chemitech.net.cn

[J02] 格式化输出
来源：http://cf.bjjhwx.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vl.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yh.yuntaijiaju.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wy.521024.cn

TS:   d.toISOString()
来源：http://mj.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://re.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ft.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://gn.nszjky.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vx.szsharing.cn

[J03] 字符串解析为日期
来源：http://tp.newstarts.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qk.muxihuayi.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yg.521024.cn

JS:   new Date("2024-01-02")
来源：http://xo.yuntaijiaju.cn

TS:   new Date("2024-01-02")
来源：http://ad.asd995.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ny.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ir.huixiangedu.cn

Ruby: Date.parse("2024-01-02")
来源：http://fm.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://bi.nicolike.cn

[J04] 时间戳与日期互转
来源：http://az.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sb.panjiajie.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://rq.jctech888.com.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://op.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ba.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qt.lnxyls.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://lm.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mn.huixinmuqiang.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yw.muxihuayi.cn

[J05] 时间加减（加 7 天）
来源：http://xt.bookmarksfly.cn

Py:   now + timedelta(days=7)
来源：http://rf.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yz.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://rx.muxihuayi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dz.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://vr.jctech888.com.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://do.hnjuh.cn

Ruby: Time.now + 7 * 86400
来源：http://jz.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gu.gzmigu.cn

[J06] 计算两时间之差
来源：http://na.521024.cn

Py:   (end - start).total_seconds()
来源：http://wf.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://ky.lnxyls.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cn.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dk.colortex.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qp.huanxung.cn

Go:   end.Sub(start).Hours()
来源：http://fx.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://nf.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://oy.9csxet.cn

[J07] 比较两个日期
来源：http://oi.wgjwhj.cn

Py:   d1 < d2;  d1 == d2
来源：http://hy.chemitech.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kp.wgjwhj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://so.hahajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://oq.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hu.asd995.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ut.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vi.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://jo.huixinmuqiang.cn

[J08] 提取年月日与星期
来源：http://iu.nicolike.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yz.jianghongdianzi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wm.newstarts.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tr.gzmigu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://my.shtwfgs.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sb.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yx.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qq.nicolike.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://so.wgjwhj.cn

[J09] 时区处理
来源：http://qg.colortex.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://vt.shtwfgs.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yy.huanxung.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rk.shxzukj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fd.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mc.huixinmuqiang.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bp.nszjky.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://is.huixinmuqiang.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ko.jianghongdianzi.cn

[J10] 取今天 / 本月第一天
来源：http://ra.szsharing.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rs.haigaiapp.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pe.bjjhwx.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ba.nicolike.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://kh.chemitech.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ax.gzmigu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zy.shxzskj.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xi.szxytkj.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pc.haigaiapp.cn

================================================================================
来源：http://oh.bjjhwx.cn

K. JSON 与序列化
来源：http://yo.hahajie.cn

================================================================================
来源：http://rp.haigaiapp.cn

[K01] 对象转 JSON 字符串
来源：http://sr.asd995.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sf.yuexingan06.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jq.wgjwhj.cn

JS:   JSON.stringify(obj)
来源：http://vh.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://ow.shtwfgs.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cd.hahajie.cn

Go:   json.Marshal(obj)
来源：http://cs.bookmarksfly.cn

Ruby: obj.to_json                                     // require "json"
来源：http://za.gzmigu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bi.haigaiapp.cn

[K02] JSON 字符串转对象
来源：http://ac.521024.cn

Py:   json.loads(s)
来源：http://ld.9csxet.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ay.9csxet.cn

JS:   JSON.parse(s)
来源：http://qk.yuntaijiaju.cn

TS:   JSON.parse(s)
来源：http://ej.newstarts.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lr.colortex.cn

Go:   json.Unmarshal(data, &v)
来源：http://vu.muxihuayi.cn

Ruby: JSON.parse(s)
来源：http://gk.shtwfgs.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tj.colortex.cn

[K03] JSON 美化输出（带缩进）
来源：http://cc.asd995.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bb.jctech888.com.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gb.gzmigu.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pn.nszjky.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://cp.hahajie.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wi.chemitech.net.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gy.lnxyls.cn


<!-- 参考信息 -->