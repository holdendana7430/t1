代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://tp.szxytkj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sy.hnjuh.cn

[G16] 对象转数组 / 字典
来源：http://op.gzmigu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wz.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://za.panjiajie.cn

JS:   Object.entries(obj)
来源：http://tg.haigaiapp.cn

TS:   Object.entries(obj)
来源：http://bv.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gm.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://wu.haigaiapp.cn

Ruby: obj.instance_variables
来源：http://uf.colortex.cn

C#:   // 用反射或 System.Text.Json
来源：http://ih.9csxet.cn

================================================================================
来源：http://wa.szsharing.cn

H. 异常与错误处理
来源：http://do.haigaiapp.cn

================================================================================
来源：http://ds.nszjky.cn

[H01] try / catch 基础
来源：http://lo.huixiangedu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yh.panjiajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hp.yuntaijiaju.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ag.szsharing.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pi.newstarts.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ms.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rx.huanxung.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ln.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://eh.gzmigu.cn

[H02] finally / ensure 收尾
来源：http://ni.huanxung.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zq.yuexingan06.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cx.bookmarksfly.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cj.nszjky.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cn.wgjwhj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xz.szxytkj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hb.wgjwhj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xl.bookmarksfly.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://kw.newstarts.cn

[H03] 主动抛出异常
来源：http://sg.jianghongdianzi.cn

Py:   raise ValueError("错误信息")
来源：http://qm.asd995.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zi.521024.cn

JS:   throw new Error("错误信息");
来源：http://rj.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://up.szxytkj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hr.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xz.jctech888.com.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://gf.shxzukj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bl.yuntaijiaju.cn

[H04] 自定义异常类型
来源：http://td.shxzskj.cn

Py:   class MyError(Exception): pass
来源：http://tk.jianghongdianzi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ov.lnxyls.cn

JS:   class MyError extends Error {}
来源：http://jy.colortex.cn

TS:   class MyError extends Error {}
来源：http://rr.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://vg.haigaiapp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://aw.9csxet.cn

Ruby: class MyError < StandardError; end
来源：http://jd.haigaiapp.cn

C#:   class MyException : Exception {}
来源：http://aq.9csxet.cn

[H05] 捕获特定类型
来源：http://jx.shtwfgs.cn

Py:   except ValueError as e:
来源：http://un.huanxung.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://my.nszjky.cn

JS:   if (e instanceof TypeError) {}
来源：http://oh.521024.cn

TS:   if (e instanceof TypeError) {}
来源：http://rc.nicolike.cn

Java: catch (IOException | SQLException e) {}
来源：http://us.newstarts.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://yb.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://fy.nicolike.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kr.szxytkj.cn

[H06] 可选值 / 空值安全访问
来源：http://mv.9csxet.cn

Py:   value = d.get("k") or default
来源：http://bv.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mu.lnxyls.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ca.shxzukj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wd.panjiajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qc.bjjhwx.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bc.hnjuh.cn

Ruby: d&.dig(:a, :b)
来源：http://tb.huanxung.cn

C#:   obj?.A?.B ?? default
来源：http://qk.szxytkj.cn

[H07] 断言
来源：http://tn.huixinmuqiang.cn

Py:   assert x > 0, "必须为正"
来源：http://pt.huixinmuqiang.cn

PHP:  assert($x > 0);
来源：http://py.bookmarksfly.cn

JS:   console.assert(x > 0);
来源：http://xq.newstarts.cn

TS:   console.assert(x > 0);
来源：http://ts.szsharing.cn

Java: assert x > 0 : "必须为正";
来源：http://mf.jctech888.com.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ks.hahajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fs.9csxet.cn

C#:   Debug.Assert(x > 0);
来源：http://ab.yuntaijiaju.cn

[H08] 获取错误信息与堆栈
来源：http://vp.hnjuh.cn

Py:   str(e);  traceback.format_exc()
来源：http://kb.panjiajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tb.chemitech.net.cn

JS:   e.message;  e.stack
来源：http://cr.haigaiapp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://of.yuntaijiaju.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zk.shtwfgs.cn

Go:   err.Error()
来源：http://yb.bookmarksfly.cn

Ruby: e.message;  e.backtrace
来源：http://dc.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://xk.jctech888.com.cn

[H09] 带错误码的异常
来源：http://hv.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://aw.chemitech.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://uz.huixiangedu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qm.panjiajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ts.colortex.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hf.bjjhwx.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://rm.huanxung.cn

Ruby: raise MyError.new("fail", 500)
来源：http://us.asd995.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qx.szxytkj.cn

[H10] 资源自动释放
来源：http://vn.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qr.jianghongdianzi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bh.9csxet.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tf.szsharing.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://nr.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wi.asd995.cn

Go:   defer f.Close()
来源：http://me.panjiajie.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://rm.wgjwhj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sj.jctech888.com.cn

================================================================================
来源：http://cj.nicolike.cn

I. 正则表达式
来源：http://nb.yuexingan06.cn

================================================================================
来源：http://sd.huixiangedu.cn

[I01] 判断是否匹配
来源：http://zy.muxihuayi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vg.jianghongdianzi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xm.colortex.cn

JS:   /\d+/.test(s)
来源：http://yu.nicolike.cn

TS:   /\d+/.test(s)
来源：http://ss.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://zi.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ei.9csxet.cn

Ruby: s.match?(/\d+/)
来源：http://kv.9csxet.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dh.jianghongdianzi.cn

[I02] 提取所有匹配
来源：http://ci.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://kc.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wl.shtwfgs.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yg.bjjhwx.cn

TS:   s.match(/\d+/g)
来源：http://tl.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://tl.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yz.hahajie.cn

Ruby: s.scan(/\d+/)
来源：http://ma.521024.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ap.nicolike.cn

[I03] 提取捕获分组
来源：http://mn.nszjky.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zh.szsharing.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://nb.asd995.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://sv.nicolike.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://pe.wgjwhj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ec.huanxung.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://qx.colortex.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qu.jctech888.com.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eb.haigaiapp.cn

[I04] 正则替换
来源：http://un.yuexingan06.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dy.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fp.huixinmuqiang.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ow.hahajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rf.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hm.hnjuh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tu.huanxung.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yp.bjjhwx.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://uo.lnxyls.cn

[I05] 按正则拆分
来源：http://ur.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://fp.nszjky.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://tv.bookmarksfly.cn

JS:   s.split(/\s*,\s*/)
来源：http://cy.yuexingan06.cn

TS:   s.split(/\s*,\s*/)
来源：http://xv.huixinmuqiang.cn

Java: s.split("\\s*,\\s*")
来源：http://sd.nszjky.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://nh.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://pw.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lb.szsharing.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wp.gzmigu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cz.hnjuh.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zg.szxytkj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://di.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yk.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wj.bjjhwx.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://el.newstarts.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://yx.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://da.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://qx.szsharing.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://cp.521024.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lz.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ww.jianghongdianzi.cn

TS:   /error/gim
来源：http://gw.shtwfgs.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://nx.haigaiapp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qm.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://xh.shxzskj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://js.szsharing.cn

[I08] 贪婪与非贪婪匹配
来源：http://nm.huixinmuqiang.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lc.huixiangedu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qx.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://da.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nr.shxzukj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ym.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qz.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://tz.jianghongdianzi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yx.bjjhwx.cn

================================================================================
来源：http://vz.yuntaijiaju.cn

J. 日期与时间
来源：http://fj.bjjhwx.cn

================================================================================
来源：http://qs.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://we.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://qj.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xe.nicolike.cn

JS:   new Date();  Date.now()
来源：http://lf.colortex.cn

TS:   new Date();  Date.now()
来源：http://qc.jctech888.com.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ln.lnxyls.cn

Go:   time.Now()
来源：http://vz.huanxung.cn

Ruby: Time.now
来源：http://mj.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://vy.9csxet.cn

[J02] 格式化输出
来源：http://dw.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sm.nszjky.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dd.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://iq.shxzukj.cn

TS:   d.toISOString()
来源：http://vx.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nk.panjiajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://dq.nicolike.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fu.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cy.shxzukj.cn

[J03] 字符串解析为日期
来源：http://eu.bjjhwx.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tg.gzmigu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fv.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://rd.huanxung.cn

TS:   new Date("2024-01-02")
来源：http://bz.colortex.cn

Java: LocalDate.parse("2024-01-02")
来源：http://th.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://gk.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://ts.wgjwhj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vb.huixiangedu.cn

[J04] 时间戳与日期互转
来源：http://ou.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ft.huixiangedu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fd.nszjky.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zw.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://mm.jctech888.com.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://il.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wv.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://en.muxihuayi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xq.shtwfgs.cn

[J05] 时间加减（加 7 天）
来源：http://ec.newstarts.cn

Py:   now + timedelta(days=7)
来源：http://mg.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jh.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xz.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://by.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://xa.huixinmuqiang.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://of.huixiangedu.cn

Ruby: Time.now + 7 * 86400
来源：http://od.hahajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://bp.shxzskj.cn

[J06] 计算两时间之差
来源：http://rp.jctech888.com.cn

Py:   (end - start).total_seconds()
来源：http://ju.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://jf.gzmigu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nl.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xe.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://gv.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://fn.yuexingan06.cn

Ruby: end - start                 # 返回秒数
来源：http://ow.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://rw.gzmigu.cn

[J07] 比较两个日期
来源：http://qb.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://jp.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://us.9csxet.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ah.hahajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xf.jianghongdianzi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yy.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ef.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://nj.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://rp.521024.cn

[J08] 提取年月日与星期
来源：http://ur.huixiangedu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://jh.szxytkj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://er.9csxet.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bt.yuntaijiaju.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://dn.9csxet.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kr.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ko.shxzukj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ds.hahajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sy.nszjky.cn

[J09] 时区处理
来源：http://nu.chemitech.net.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://jk.colortex.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://tk.yuexingan06.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hr.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ao.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ys.shtwfgs.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://om.bookmarksfly.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fv.lnxyls.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mh.jctech888.com.cn

[J10] 取今天 / 本月第一天
来源：http://sk.muxihuayi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://yo.colortex.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sb.hnjuh.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wv.asd995.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yi.shxzukj.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ih.nszjky.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://oq.nicolike.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sl.bjjhwx.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://te.colortex.cn

================================================================================
来源：http://nx.shxzukj.cn

K. JSON 与序列化
来源：http://kl.shxzukj.cn

================================================================================
来源：http://oq.yuntaijiaju.cn

[K01] 对象转 JSON 字符串
来源：http://rh.shxzukj.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zm.haigaiapp.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://da.huixiangedu.cn

JS:   JSON.stringify(obj)
来源：http://hh.haigaiapp.cn

TS:   JSON.stringify(obj)
来源：http://hs.hahajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ij.asd995.cn

Go:   json.Marshal(obj)
来源：http://qu.huixinmuqiang.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jj.521024.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://hp.szxytkj.cn

[K02] JSON 字符串转对象
来源：http://ot.521024.cn

Py:   json.loads(s)
来源：http://yc.hahajie.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rp.lnxyls.cn

JS:   JSON.parse(s)
来源：http://mx.panjiajie.cn

TS:   JSON.parse(s)
来源：http://qs.shxzukj.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://lo.lnxyls.cn

Go:   json.Unmarshal(data, &v)
来源：http://ns.chemitech.net.cn

Ruby: JSON.parse(s)
来源：http://re.haigaiapp.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tc.wgjwhj.cn

[K03] JSON 美化输出（带缩进）
来源：http://li.521024.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pw.bookmarksfly.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dw.panjiajie.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://po.gzmigu.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lc.bjjhwx.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ku.bjjhwx.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ua.yuntaijiaju.cn


<!-- 参考信息 -->