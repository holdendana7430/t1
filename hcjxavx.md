代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://wh.shxzukj.cn

Ruby: obj.instance_variables
来源：http://xf.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://mw.jctech888.com.cn

================================================================================
来源：http://yg.521024.cn

H. 异常与错误处理
来源：http://xl.huixiangedu.cn

================================================================================
来源：http://ad.hnjuh.cn

[H01] try / catch 基础
来源：http://vp.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://bu.newstarts.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ql.colortex.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fu.yuexingan06.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tu.shtwfgs.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://sk.chemitech.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vx.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mr.nicolike.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zs.lnxyls.cn

[H02] finally / ensure 收尾
来源：http://my.gzmigu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://es.shtwfgs.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ql.muxihuayi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kc.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://bk.nicolike.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qh.jctech888.com.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fl.bookmarksfly.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dw.gzmigu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pb.szxytkj.cn

[H03] 主动抛出异常
来源：http://yj.szxytkj.cn

Py:   raise ValueError("错误信息")
来源：http://wi.nszjky.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rl.huixiangedu.cn

JS:   throw new Error("错误信息");
来源：http://vb.nszjky.cn

TS:   throw new Error("错误信息");
来源：http://uh.muxihuayi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yl.bjjhwx.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://kb.gzmigu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://sp.lnxyls.cn

C#:   throw new ArgumentException("错误信息");
来源：http://jm.shxzukj.cn

[H04] 自定义异常类型
来源：http://br.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://cs.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://my.hahajie.cn

JS:   class MyError extends Error {}
来源：http://ox.9csxet.cn

TS:   class MyError extends Error {}
来源：http://zy.bookmarksfly.cn

Java: class MyException extends RuntimeException {}
来源：http://yp.lnxyls.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ph.panjiajie.cn

Ruby: class MyError < StandardError; end
来源：http://tj.panjiajie.cn

C#:   class MyException : Exception {}
来源：http://vp.gzmigu.cn

[H05] 捕获特定类型
来源：http://ty.hnjuh.cn

Py:   except ValueError as e:
来源：http://vo.colortex.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://tu.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://hq.nszjky.cn

TS:   if (e instanceof TypeError) {}
来源：http://gr.huanxung.cn

Java: catch (IOException | SQLException e) {}
来源：http://nm.huanxung.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ds.asd995.cn

Ruby: rescue ArgumentError => e
来源：http://gj.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://to.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://go.bjjhwx.cn

Py:   value = d.get("k") or default
来源：http://bx.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ja.yuexingan06.cn

JS:   obj?.a?.b;  d ?? default
来源：http://lv.hahajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tn.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://qb.shxzukj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://vl.9csxet.cn

Ruby: d&.dig(:a, :b)
来源：http://oq.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://ws.muxihuayi.cn

[H07] 断言
来源：http://jc.colortex.cn

Py:   assert x > 0, "必须为正"
来源：http://ud.shtwfgs.cn

PHP:  assert($x > 0);
来源：http://ei.panjiajie.cn

JS:   console.assert(x > 0);
来源：http://zr.yuexingan06.cn

TS:   console.assert(x > 0);
来源：http://jp.huixinmuqiang.cn

Java: assert x > 0 : "必须为正";
来源：http://gh.newstarts.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://it.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fz.shtwfgs.cn

C#:   Debug.Assert(x > 0);
来源：http://eq.hahajie.cn

[H08] 获取错误信息与堆栈
来源：http://yf.hnjuh.cn

Py:   str(e);  traceback.format_exc()
来源：http://jf.hahajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ls.hnjuh.cn

JS:   e.message;  e.stack
来源：http://tx.szsharing.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ku.9csxet.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bp.shxzskj.cn

Go:   err.Error()
来源：http://wf.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://ic.huixinmuqiang.cn

C#:   e.Message;  e.StackTrace
来源：http://ut.lnxyls.cn

[H09] 带错误码的异常
来源：http://wy.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qb.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://sp.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://od.huixiangedu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://yo.gzmigu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://vq.shxzukj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qw.panjiajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xy.asd995.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tt.szsharing.cn

[H10] 资源自动释放
来源：http://mi.yuexingan06.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zc.shtwfgs.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jr.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gy.jctech888.com.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qu.huixinmuqiang.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zg.lnxyls.cn

Go:   defer f.Close()
来源：http://vg.chemitech.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://eg.521024.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://io.gzmigu.cn

================================================================================
来源：http://od.jctech888.com.cn

I. 正则表达式
来源：http://vg.chemitech.net.cn

================================================================================
来源：http://af.nszjky.cn

[I01] 判断是否匹配
来源：http://ek.szxytkj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bp.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ke.asd995.cn

JS:   /\d+/.test(s)
来源：http://yj.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://bm.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nt.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://li.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://df.gzmigu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rt.huixinmuqiang.cn

[I02] 提取所有匹配
来源：http://ho.bookmarksfly.cn

Py:   re.findall(r"\d+", s)
来源：http://uf.9csxet.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://kg.bjjhwx.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cc.asd995.cn

TS:   s.match(/\d+/g)
来源：http://ns.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ta.hahajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yg.huanxung.cn

Ruby: s.scan(/\d+/)
来源：http://og.bjjhwx.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dv.szxytkj.cn

[I03] 提取捕获分组
来源：http://ii.9csxet.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://oy.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ck.panjiajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://bu.huixiangedu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gf.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ah.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ix.hnjuh.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://vu.asd995.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://oc.huixiangedu.cn

[I04] 正则替换
来源：http://cq.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kt.gzmigu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ld.hahajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cv.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://uo.szxytkj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://fa.huixiangedu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://va.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ab.bookmarksfly.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ro.newstarts.cn

[I05] 按正则拆分
来源：http://ov.newstarts.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://su.huixiangedu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://py.yuexingan06.cn

JS:   s.split(/\s*,\s*/)
来源：http://uv.shtwfgs.cn

TS:   s.split(/\s*,\s*/)
来源：http://pv.huixiangedu.cn

Java: s.split("\\s*,\\s*")
来源：http://mh.jctech888.com.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pe.yuntaijiaju.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zj.shxzskj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lr.asd995.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nz.shtwfgs.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nw.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uj.bjjhwx.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ag.nicolike.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://az.szxytkj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cl.nszjky.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ys.bookmarksfly.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vw.shtwfgs.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gw.shxzskj.cn

[I07] 忽略大小写与多行模式
来源：http://da.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tt.shxzskj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fm.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://xy.muxihuayi.cn

TS:   /error/gim
来源：http://kk.shxzukj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://md.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xo.colortex.cn

Ruby: s.scan(/error/i)
来源：http://xg.szxytkj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qo.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://iu.lnxyls.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://dg.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nx.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://cn.panjiajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://px.colortex.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://iu.wgjwhj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://bv.colortex.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ka.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gy.shtwfgs.cn

================================================================================
来源：http://mt.shtwfgs.cn

J. 日期与时间
来源：http://ar.newstarts.cn

================================================================================
来源：http://yg.jctech888.com.cn

[J01] 获取当前时间
来源：http://sk.haigaiapp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ku.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://qv.bookmarksfly.cn

JS:   new Date();  Date.now()
来源：http://nv.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://hg.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mm.9csxet.cn

Go:   time.Now()
来源：http://xl.colortex.cn

Ruby: Time.now
来源：http://vz.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tb.yuntaijiaju.cn

[J02] 格式化输出
来源：http://us.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zj.panjiajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://un.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://cb.szxytkj.cn

TS:   d.toISOString()
来源：http://lc.521024.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vt.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ci.bjjhwx.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ei.asd995.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fd.jctech888.com.cn

[J03] 字符串解析为日期
来源：http://si.nicolike.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fj.colortex.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://od.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://fv.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://mw.shtwfgs.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gc.chemitech.net.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ed.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://eb.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://vy.huixinmuqiang.cn

[J04] 时间戳与日期互转
来源：http://hb.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mk.huanxung.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://la.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ci.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://pz.nicolike.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ss.lnxyls.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://md.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ut.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jf.yuexingan06.cn

[J05] 时间加减（加 7 天）
来源：http://pw.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://jr.chemitech.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pb.huixiangedu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://eu.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gw.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://as.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zp.huixinmuqiang.cn

Ruby: Time.now + 7 * 86400
来源：http://hd.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dk.yuexingan06.cn

[J06] 计算两时间之差
来源：http://il.lnxyls.cn

Py:   (end - start).total_seconds()
来源：http://sp.huixiangedu.cn

PHP:  $end->diff($start)->days;
来源：http://wt.shxzukj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yj.szsharing.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gz.bjjhwx.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kl.szsharing.cn

Go:   end.Sub(start).Hours()
来源：http://bl.yuexingan06.cn

Ruby: end - start                 # 返回秒数
来源：http://mo.wgjwhj.cn

C#:   (end - start).TotalSeconds
来源：http://pb.haigaiapp.cn

[J07] 比较两个日期
来源：http://aw.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://id.asd995.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://on.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://zr.newstarts.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ea.newstarts.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hahajie.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bf.jctech888.com.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wk.panjiajie.cn

C#:   d1 < d2;  d1 == d2
来源：http://ut.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://sr.chemitech.net.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ij.nszjky.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://to.nszjky.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bv.yuntaijiaju.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kn.szxytkj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vi.nicolike.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://jj.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yw.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://pd.huixinmuqiang.cn

[J09] 时区处理
来源：http://fa.bjjhwx.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ui.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fl.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gp.chemitech.net.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ul.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jr.9csxet.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hc.gzmigu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lc.huixinmuqiang.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fg.yuexingan06.cn

[J10] 取今天 / 本月第一天
来源：http://bt.bookmarksfly.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ap.gzmigu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vm.nicolike.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vo.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sl.muxihuayi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cx.shxzskj.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ss.haigaiapp.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ln.chemitech.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wf.wgjwhj.cn

================================================================================
来源：http://ml.yuntaijiaju.cn

K. JSON 与序列化
来源：http://yt.szxytkj.cn

================================================================================
来源：http://hq.haigaiapp.cn

[K01] 对象转 JSON 字符串
来源：http://ua.hnjuh.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zx.muxihuayi.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bb.shxzukj.cn

JS:   JSON.stringify(obj)
来源：http://ir.gzmigu.cn

TS:   JSON.stringify(obj)
来源：http://lj.shxzskj.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rl.shxzukj.cn

Go:   json.Marshal(obj)
来源：http://zc.9csxet.cn

Ruby: obj.to_json                                     // require "json"
来源：http://uf.newstarts.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gd.huixinmuqiang.cn

[K02] JSON 字符串转对象
来源：http://ci.shxzskj.cn

Py:   json.loads(s)
来源：http://ao.newstarts.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cw.asd995.cn

JS:   JSON.parse(s)
来源：http://hk.huanxung.cn

TS:   JSON.parse(s)
来源：http://ph.jctech888.com.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://iv.hnjuh.cn

Go:   json.Unmarshal(data, &v)
来源：http://ql.chemitech.net.cn

Ruby: JSON.parse(s)
来源：http://gm.newstarts.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sh.jctech888.com.cn

[K03] JSON 美化输出（带缩进）
来源：http://zb.nszjky.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rg.huanxung.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wi.szsharing.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ju.muxihuayi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zc.521024.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sa.nszjky.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cl.haigaiapp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://os.wgjwhj.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qa.colortex.cn

[K04] 读取 JSON 文件
来源：http://pq.hnjuh.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vt.yuexingan06.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yu.chemitech.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bx.muxihuayi.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ud.colortex.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fy.hnjuh.cn


<!-- 参考信息 -->