代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://yv.shxzukj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gc.nszjky.cn

Java: enum Color { RED, GREEN }
来源：http://ik.521024.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tc.521024.cn

Ruby: Color = %i[red green].freeze
来源：http://jx.szsharing.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jb.nicolike.cn

[G16] 对象转数组 / 字典
来源：http://wl.hnjuh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ja.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://jv.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://vx.nszjky.cn

TS:   Object.entries(obj)
来源：http://ba.jianghongdianzi.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mh.panjiajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tb.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://jg.lnxyls.cn

C#:   // 用反射或 System.Text.Json
来源：http://xu.nicolike.cn

================================================================================
来源：http://lc.jctech888.com.cn

H. 异常与错误处理
来源：http://rd.gzmigu.cn

================================================================================
来源：http://rh.shtwfgs.cn

[H01] try / catch 基础
来源：http://ch.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://yv.huixinmuqiang.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hn.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vn.nicolike.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://tt.9csxet.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://dk.haigaiapp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mx.szxytkj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://su.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nb.9csxet.cn

[H02] finally / ensure 收尾
来源：http://uq.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xo.lnxyls.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://tc.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yo.chemitech.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ik.wgjwhj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mb.asd995.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fp.szxytkj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dr.huixiangedu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rl.huixinmuqiang.cn

[H03] 主动抛出异常
来源：http://cn.521024.cn

Py:   raise ValueError("错误信息")
来源：http://bu.shtwfgs.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hx.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://vx.hnjuh.cn

TS:   throw new Error("错误信息");
来源：http://pq.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yu.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://lo.szxytkj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bv.yuntaijiaju.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pn.newstarts.cn

[H04] 自定义异常类型
来源：http://sl.shxzskj.cn

Py:   class MyError(Exception): pass
来源：http://jr.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wo.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://ou.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://af.newstarts.cn

Java: class MyException extends RuntimeException {}
来源：http://dd.lnxyls.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uy.colortex.cn

Ruby: class MyError < StandardError; end
来源：http://ib.yuexingan06.cn

C#:   class MyException : Exception {}
来源：http://ed.yuntaijiaju.cn

[H05] 捕获特定类型
来源：http://xs.bookmarksfly.cn

Py:   except ValueError as e:
来源：http://tn.huanxung.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pw.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://sl.jianghongdianzi.cn

TS:   if (e instanceof TypeError) {}
来源：http://qq.shtwfgs.cn

Java: catch (IOException | SQLException e) {}
来源：http://ba.huanxung.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ma.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://tz.hahajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hy.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://js.hahajie.cn

Py:   value = d.get("k") or default
来源：http://we.wgjwhj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://fh.shtwfgs.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ik.szxytkj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yz.521024.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rc.panjiajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xr.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://jg.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://pr.bookmarksfly.cn

[H07] 断言
来源：http://ri.bookmarksfly.cn

Py:   assert x > 0, "必须为正"
来源：http://et.bookmarksfly.cn

PHP:  assert($x > 0);
来源：http://nu.nicolike.cn

JS:   console.assert(x > 0);
来源：http://th.chemitech.net.cn

TS:   console.assert(x > 0);
来源：http://tk.huixiangedu.cn

Java: assert x > 0 : "必须为正";
来源：http://gg.bjjhwx.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hb.chemitech.net.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nh.521024.cn

C#:   Debug.Assert(x > 0);
来源：http://xd.haigaiapp.cn

[H08] 获取错误信息与堆栈
来源：http://qy.9csxet.cn

Py:   str(e);  traceback.format_exc()
来源：http://ji.panjiajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tb.bookmarksfly.cn

JS:   e.message;  e.stack
来源：http://lr.haigaiapp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://gf.bookmarksfly.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ca.wgjwhj.cn

Go:   err.Error()
来源：http://to.asd995.cn

Ruby: e.message;  e.backtrace
来源：http://al.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://qi.jctech888.com.cn

[H09] 带错误码的异常
来源：http://ck.hnjuh.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://pn.haigaiapp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yx.521024.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ba.colortex.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://fp.muxihuayi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lg.colortex.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ds.lnxyls.cn

Ruby: raise MyError.new("fail", 500)
来源：http://cg.shxzskj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://wy.newstarts.cn

[H10] 资源自动释放
来源：http://ch.9csxet.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ko.wgjwhj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ap.hnjuh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bc.jianghongdianzi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://oc.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pm.szxytkj.cn

Go:   defer f.Close()
来源：http://fd.huixiangedu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qp.nszjky.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ql.hnjuh.cn

================================================================================
来源：http://er.gzmigu.cn

I. 正则表达式
来源：http://ed.nszjky.cn

================================================================================
来源：http://lu.huixiangedu.cn

[I01] 判断是否匹配
来源：http://hs.wgjwhj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jz.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wa.bjjhwx.cn

JS:   /\d+/.test(s)
来源：http://wt.jctech888.com.cn

TS:   /\d+/.test(s)
来源：http://hr.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://bq.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ia.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://it.yuntaijiaju.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qz.yuntaijiaju.cn

[I02] 提取所有匹配
来源：http://yi.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://ht.nicolike.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nw.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qq.huixiangedu.cn

TS:   s.match(/\d+/g)
来源：http://cl.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mi.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://or.muxihuayi.cn

Ruby: s.scan(/\d+/)
来源：http://ok.haigaiapp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xy.yuexingan06.cn

[I03] 提取捕获分组
来源：http://oi.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rf.szsharing.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ef.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://dv.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gg.szsharing.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nv.gzmigu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ws.colortex.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ar.jianghongdianzi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://pu.shxzskj.cn

[I04] 正则替换
来源：http://ck.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jq.panjiajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dr.jianghongdianzi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://my.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://eo.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qe.szsharing.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ow.szsharing.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://je.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wa.yuexingan06.cn

[I05] 按正则拆分
来源：http://lx.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://et.chemitech.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mb.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://du.lnxyls.cn

TS:   s.split(/\s*,\s*/)
来源：http://bh.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://pb.panjiajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jt.szsharing.cn

Ruby: s.split(/\s*,\s*/)
来源：http://yu.colortex.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rf.huixinmuqiang.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qp.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hr.haigaiapp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yx.shtwfgs.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gb.szsharing.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ht.shxzskj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wt.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://sq.lnxyls.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://cz.newstarts.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gd.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://ez.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wf.hnjuh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ep.panjiajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fn.lnxyls.cn

TS:   /error/gim
来源：http://ic.bookmarksfly.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://fx.521024.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ez.nicolike.cn

Ruby: s.scan(/error/i)
来源：http://wx.9csxet.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://mu.521024.cn

[I08] 贪婪与非贪婪匹配
来源：http://gd.hnjuh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://et.jctech888.com.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zx.asd995.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ho.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ts.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://qo.nicolike.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zu.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://rk.hnjuh.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zx.chemitech.net.cn

================================================================================
来源：http://sd.chemitech.net.cn

J. 日期与时间
来源：http://td.521024.cn

================================================================================
来源：http://ao.haigaiapp.cn

[J01] 获取当前时间
来源：http://we.huixinmuqiang.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ws.521024.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mg.jianghongdianzi.cn

JS:   new Date();  Date.now()
来源：http://ka.nszjky.cn

TS:   new Date();  Date.now()
来源：http://rt.shtwfgs.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ku.huixinmuqiang.cn

Go:   time.Now()
来源：http://ih.nicolike.cn

Ruby: Time.now
来源：http://gx.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://oh.hnjuh.cn

[J02] 格式化输出
来源：http://cv.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ln.huanxung.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fz.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://yn.huixiangedu.cn

TS:   d.toISOString()
来源：http://na.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fr.nszjky.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://og.nszjky.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jx.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ph.haigaiapp.cn

[J03] 字符串解析为日期
来源：http://qu.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://tk.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://zy.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://om.muxihuayi.cn

TS:   new Date("2024-01-02")
来源：http://um.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://il.bjjhwx.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://aq.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://ae.yuntaijiaju.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://oy.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://uv.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yq.nszjky.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://jw.9csxet.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://go.colortex.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://cm.wgjwhj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ff.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wf.szsharing.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wl.hnjuh.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://sd.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://gd.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://je.asd995.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://br.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://do.shtwfgs.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jt.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://ca.shxzskj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yn.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://li.jctech888.com.cn

C#:   DateTime.Now.AddDays(7)
来源：http://mt.newstarts.cn

[J06] 计算两时间之差
来源：http://jk.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://zn.lnxyls.cn

PHP:  $end->diff($start)->days;
来源：http://od.panjiajie.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ue.lnxyls.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bq.shtwfgs.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wv.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://uy.nicolike.cn

Ruby: end - start                 # 返回秒数
来源：http://kf.gzmigu.cn

C#:   (end - start).TotalSeconds
来源：http://vs.nicolike.cn

[J07] 比较两个日期
来源：http://fe.shtwfgs.cn

Py:   d1 < d2;  d1 == d2
来源：http://ff.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hw.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://da.asd995.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wi.huixinmuqiang.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://pt.bjjhwx.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kq.hnjuh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://uv.wgjwhj.cn

C#:   d1 < d2;  d1 == d2
来源：http://je.huanxung.cn

[J08] 提取年月日与星期
来源：http://cs.shxzskj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://la.huixinmuqiang.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oi.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zo.szsharing.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://kf.colortex.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://cj.yuntaijiaju.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pz.bjjhwx.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://dv.huixiangedu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://on.yuntaijiaju.cn

[J09] 时区处理
来源：http://la.huixiangedu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ir.yuntaijiaju.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ji.szsharing.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rb.shxzskj.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xd.huixinmuqiang.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fv.asd995.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://km.shtwfgs.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yi.shxzukj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://dd.gzmigu.cn

[J10] 取今天 / 本月第一天
来源：http://sl.huixinmuqiang.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://oz.huanxung.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tx.nszjky.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kd.jctech888.com.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dq.bookmarksfly.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zy.shtwfgs.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mu.yuntaijiaju.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fp.hahajie.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dc.hnjuh.cn

================================================================================
来源：http://xs.colortex.cn

K. JSON 与序列化
来源：http://gj.asd995.cn

================================================================================
来源：http://ri.huanxung.cn

[K01] 对象转 JSON 字符串
来源：http://hc.lnxyls.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ah.asd995.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xj.nszjky.cn

JS:   JSON.stringify(obj)
来源：http://ak.yuexingan06.cn

TS:   JSON.stringify(obj)
来源：http://mr.jctech888.com.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sf.newstarts.cn

Go:   json.Marshal(obj)
来源：http://ld.huanxung.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ix.gzmigu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://am.lnxyls.cn

[K02] JSON 字符串转对象
来源：http://bd.colortex.cn

Py:   json.loads(s)
来源：http://qb.hnjuh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kv.jctech888.com.cn

JS:   JSON.parse(s)
来源：http://uz.gzmigu.cn

TS:   JSON.parse(s)
来源：http://ny.huanxung.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ww.chemitech.net.cn

Go:   json.Unmarshal(data, &v)
来源：http://qx.colortex.cn

Ruby: JSON.parse(s)
来源：http://kz.9csxet.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nb.huixinmuqiang.cn

[K03] JSON 美化输出（带缩进）
来源：http://wa.huanxung.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ha.lnxyls.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sj.521024.cn


<!-- 参考信息 -->