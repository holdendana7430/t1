代发 wailian999

[G14] 数据类 / record
来源：http://lt.hnjuh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tz.hnjuh.cn

PHP:  // 用 readonly 属性模拟
来源：http://br.chemitech.net.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zd.521024.cn

TS:   type User = { name: string; age: number };
来源：http://qq.hahajie.cn

Java: record User(String name, int age) {}
来源：http://se.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://ug.lnxyls.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ni.nicolike.cn

C#:   record User(string Name, int Age);
来源：http://ob.newstarts.cn

[G15] 枚举
来源：http://qp.huixiangedu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xv.bookmarksfly.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rr.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ck.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jw.yuntaijiaju.cn

Java: enum Color { RED, GREEN }
来源：http://qz.bookmarksfly.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hg.newstarts.cn

Ruby: Color = %i[red green].freeze
来源：http://kh.haigaiapp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://nz.nicolike.cn

[G16] 对象转数组 / 字典
来源：http://sk.huixiangedu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lz.nszjky.cn

PHP:  get_object_vars($obj);
来源：http://vt.521024.cn

JS:   Object.entries(obj)
来源：http://wz.haigaiapp.cn

TS:   Object.entries(obj)
来源：http://lk.newstarts.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://dh.jianghongdianzi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://lf.yuntaijiaju.cn

Ruby: obj.instance_variables
来源：http://tc.9csxet.cn

C#:   // 用反射或 System.Text.Json
来源：http://zu.hnjuh.cn

================================================================================
来源：http://ld.nszjky.cn

H. 异常与错误处理
来源：http://ax.9csxet.cn

================================================================================
来源：http://pa.gzmigu.cn

[H01] try / catch 基础
来源：http://bk.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ag.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fx.yuexingan06.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://vm.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qv.colortex.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rp.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yh.521024.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yp.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://aq.lnxyls.cn

[H02] finally / ensure 收尾
来源：http://vb.yuntaijiaju.cn

Py:   try: f()⏎finally: cleanup()
来源：http://lf.asd995.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://bt.521024.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rg.newstarts.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://pr.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yc.asd995.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yq.521024.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kq.shxzskj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ua.newstarts.cn

[H03] 主动抛出异常
来源：http://ak.hnjuh.cn

Py:   raise ValueError("错误信息")
来源：http://ft.wgjwhj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ka.asd995.cn

JS:   throw new Error("错误信息");
来源：http://wl.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://pr.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://dn.jctech888.com.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fr.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ih.shxzskj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vp.hnjuh.cn

[H04] 自定义异常类型
来源：http://tx.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://tr.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rj.nicolike.cn

JS:   class MyError extends Error {}
来源：http://ij.nicolike.cn

TS:   class MyError extends Error {}
来源：http://pf.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://df.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ty.hnjuh.cn

Ruby: class MyError < StandardError; end
来源：http://qx.nicolike.cn

C#:   class MyException : Exception {}
来源：http://cs.nicolike.cn

[H05] 捕获特定类型
来源：http://pd.yuexingan06.cn

Py:   except ValueError as e:
来源：http://kt.muxihuayi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yb.hahajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://mq.huixinmuqiang.cn

TS:   if (e instanceof TypeError) {}
来源：http://ik.panjiajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://pu.hnjuh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://pt.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://xn.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://of.jianghongdianzi.cn

[H06] 可选值 / 空值安全访问
来源：http://mg.hahajie.cn

Py:   value = d.get("k") or default
来源：http://cy.muxihuayi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wz.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://st.yuntaijiaju.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gr.newstarts.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hj.bookmarksfly.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://of.gzmigu.cn

Ruby: d&.dig(:a, :b)
来源：http://jb.bjjhwx.cn

C#:   obj?.A?.B ?? default
来源：http://pv.bjjhwx.cn

[H07] 断言
来源：http://hs.gzmigu.cn

Py:   assert x > 0, "必须为正"
来源：http://ob.bjjhwx.cn

PHP:  assert($x > 0);
来源：http://ha.newstarts.cn

JS:   console.assert(x > 0);
来源：http://mz.bjjhwx.cn

TS:   console.assert(x > 0);
来源：http://kf.9csxet.cn

Java: assert x > 0 : "必须为正";
来源：http://yg.wgjwhj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dr.nszjky.cn

Ruby: raise "必须为正" unless x > 0
来源：http://le.huixinmuqiang.cn

C#:   Debug.Assert(x > 0);
来源：http://uh.hahajie.cn

[H08] 获取错误信息与堆栈
来源：http://mx.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://yb.hahajie.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qt.huixinmuqiang.cn

JS:   e.message;  e.stack
来源：http://uo.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://br.muxihuayi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zj.hnjuh.cn

Go:   err.Error()
来源：http://wq.haigaiapp.cn

Ruby: e.message;  e.backtrace
来源：http://wa.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://zx.nszjky.cn

[H09] 带错误码的异常
来源：http://av.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hf.panjiajie.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gd.chemitech.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://la.hahajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ie.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://jq.newstarts.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qv.shxzskj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://io.huixiangedu.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cd.szsharing.cn

[H10] 资源自动释放
来源：http://qj.lnxyls.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://iv.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://vy.szsharing.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://po.gzmigu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rm.hnjuh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wm.shxzskj.cn

Go:   defer f.Close()
来源：http://nt.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://la.bjjhwx.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ra.wgjwhj.cn

================================================================================
来源：http://xg.szxytkj.cn

I. 正则表达式
来源：http://hr.shxzukj.cn

================================================================================
来源：http://ig.jctech888.com.cn

[I01] 判断是否匹配
来源：http://cy.jianghongdianzi.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ud.shtwfgs.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sf.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://vo.haigaiapp.cn

TS:   /\d+/.test(s)
来源：http://pc.hnjuh.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fe.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ki.huixinmuqiang.cn

Ruby: s.match?(/\d+/)
来源：http://km.nszjky.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://xp.lnxyls.cn

[I02] 提取所有匹配
来源：http://ve.szxytkj.cn

Py:   re.findall(r"\d+", s)
来源：http://ao.yuntaijiaju.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pg.asd995.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xl.gzmigu.cn

TS:   s.match(/\d+/g)
来源：http://zv.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jg.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://jr.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://dy.yuntaijiaju.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ra.lnxyls.cn

[I03] 提取捕获分组
来源：http://pz.colortex.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rq.haigaiapp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yk.szsharing.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ev.shxzskj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ll.bjjhwx.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dw.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://du.shxzskj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tg.wgjwhj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://lr.jianghongdianzi.cn

[I04] 正则替换
来源：http://iv.shxzskj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ok.nicolike.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://se.lnxyls.cn

JS:   s.replace(/\d+/g, "#")
来源：http://am.muxihuayi.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qm.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cn.lnxyls.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://mt.muxihuayi.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://db.chemitech.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fb.nszjky.cn

[I05] 按正则拆分
来源：http://ze.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://cj.nszjky.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hf.asd995.cn

JS:   s.split(/\s*,\s*/)
来源：http://qm.huanxung.cn

TS:   s.split(/\s*,\s*/)
来源：http://ki.lnxyls.cn

Java: s.split("\\s*,\\s*")
来源：http://gz.jctech888.com.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ny.szsharing.cn

Ruby: s.split(/\s*,\s*/)
来源：http://io.shtwfgs.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xr.lnxyls.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nm.huixinmuqiang.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://eo.panjiajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://jk.huixinmuqiang.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ww.jctech888.com.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sz.521024.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zk.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ga.newstarts.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fg.jctech888.com.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vh.hahajie.cn

[I07] 忽略大小写与多行模式
来源：http://fw.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ss.bookmarksfly.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://me.hahajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://sn.jctech888.com.cn

TS:   /error/gim
来源：http://kp.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://vx.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ap.9csxet.cn

Ruby: s.scan(/error/i)
来源：http://rp.chemitech.net.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hw.521024.cn

[I08] 贪婪与非贪婪匹配
来源：http://zh.hnjuh.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://jp.hnjuh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kv.panjiajie.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://sr.shxzskj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://om.shtwfgs.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://rm.haigaiapp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gl.huanxung.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://pq.newstarts.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nc.jctech888.com.cn

================================================================================
来源：http://hw.huanxung.cn

J. 日期与时间
来源：http://df.hnjuh.cn

================================================================================
来源：http://pi.chemitech.net.cn

[J01] 获取当前时间
来源：http://jl.nszjky.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kc.hahajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://yv.huanxung.cn

JS:   new Date();  Date.now()
来源：http://rs.chemitech.net.cn

TS:   new Date();  Date.now()
来源：http://yz.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://su.gzmigu.cn

Go:   time.Now()
来源：http://ni.chemitech.net.cn

Ruby: Time.now
来源：http://re.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xv.haigaiapp.cn

[J02] 格式化输出
来源：http://dh.nicolike.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://tb.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hx.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fy.shxzukj.cn

TS:   d.toISOString()
来源：http://oh.yuntaijiaju.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vh.bookmarksfly.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://rb.bjjhwx.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fk.shxzskj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ls.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://pu.newstarts.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ys.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://fu.huanxung.cn

JS:   new Date("2024-01-02")
来源：http://zg.bjjhwx.cn

TS:   new Date("2024-01-02")
来源：http://ar.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ib.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zs.bjjhwx.cn

Ruby: Date.parse("2024-01-02")
来源：http://iu.521024.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fp.chemitech.net.cn

[J04] 时间戳与日期互转
来源：http://qj.huixinmuqiang.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://yk.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://yj.newstarts.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ku.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ur.panjiajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wb.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gt.hahajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rr.szsharing.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://em.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://tm.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://dt.hahajie.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://hd.wgjwhj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cc.shtwfgs.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gv.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://yn.chemitech.net.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ig.jianghongdianzi.cn

Ruby: Time.now + 7 * 86400
来源：http://rg.nszjky.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kq.jctech888.com.cn

[J06] 计算两时间之差
来源：http://pq.521024.cn

Py:   (end - start).total_seconds()
来源：http://ka.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://lr.haigaiapp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wh.bookmarksfly.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kv.asd995.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xl.haigaiapp.cn

Go:   end.Sub(start).Hours()
来源：http://ou.shxzukj.cn

Ruby: end - start                 # 返回秒数
来源：http://zb.muxihuayi.cn

C#:   (end - start).TotalSeconds
来源：http://iy.chemitech.net.cn

[J07] 比较两个日期
来源：http://sr.newstarts.cn

Py:   d1 < d2;  d1 == d2
来源：http://eo.colortex.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gf.newstarts.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vh.shxzukj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xn.521024.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bj.chemitech.net.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vy.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fw.jctech888.com.cn

C#:   d1 < d2;  d1 == d2
来源：http://wb.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://qo.panjiajie.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rt.panjiajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://py.shxzukj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ks.szsharing.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://bs.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://do.jctech888.com.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yw.wgjwhj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tx.lnxyls.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kz.521024.cn

[J09] 时区处理
来源：http://ol.asd995.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zm.bookmarksfly.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hm.newstarts.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ic.panjiajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ug.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jf.muxihuayi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wr.hnjuh.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://yp.shxzukj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ap.shxzukj.cn

[J10] 取今天 / 本月第一天
来源：http://fg.shxzskj.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://rd.chemitech.net.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fi.bjjhwx.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zd.lnxyls.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ft.jctech888.com.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://em.huixinmuqiang.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uh.hahajie.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kw.9csxet.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bo.lnxyls.cn

================================================================================
来源：http://av.newstarts.cn

K. JSON 与序列化
来源：http://fa.szsharing.cn

================================================================================
来源：http://zk.gzmigu.cn

[K01] 对象转 JSON 字符串
来源：http://ld.bjjhwx.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sw.chemitech.net.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cx.jianghongdianzi.cn

JS:   JSON.stringify(obj)
来源：http://hs.bjjhwx.cn

TS:   JSON.stringify(obj)
来源：http://zg.panjiajie.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xi.chemitech.net.cn

Go:   json.Marshal(obj)
来源：http://rf.jctech888.com.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cn.yuexingan06.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://uc.haigaiapp.cn


<!-- 参考信息 -->