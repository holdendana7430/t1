代发 wailian999

Java: u instanceof User
来源：http://uz.huanxung.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xm.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://or.shtwfgs.cn

C#:   u is User
来源：http://ug.521024.cn

[G14] 数据类 / record
来源：http://cn.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://se.haigaiapp.cn

PHP:  // 用 readonly 属性模拟
来源：http://ix.yuexingan06.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pr.bjjhwx.cn

TS:   type User = { name: string; age: number };
来源：http://yf.shxzskj.cn

Java: record User(String name, int age) {}
来源：http://rr.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://gi.yuexingan06.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gv.shxzukj.cn

C#:   record User(string Name, int Age);
来源：http://re.colortex.cn

[G15] 枚举
来源：http://sa.hahajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cx.nicolike.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://gm.szsharing.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rj.nicolike.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://dn.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://mh.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://na.hahajie.cn

Ruby: Color = %i[red green].freeze
来源：http://mv.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wn.shtwfgs.cn

[G16] 对象转数组 / 字典
来源：http://uv.521024.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ef.szxytkj.cn

PHP:  get_object_vars($obj);
来源：http://fl.asd995.cn

JS:   Object.entries(obj)
来源：http://yd.huixinmuqiang.cn

TS:   Object.entries(obj)
来源：http://zf.nszjky.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mv.shtwfgs.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vd.yuntaijiaju.cn

Ruby: obj.instance_variables
来源：http://np.gzmigu.cn

C#:   // 用反射或 System.Text.Json
来源：http://vy.yuntaijiaju.cn

================================================================================
来源：http://mh.gzmigu.cn

H. 异常与错误处理
来源：http://er.lnxyls.cn

================================================================================
来源：http://hy.szxytkj.cn

[H01] try / catch 基础
来源：http://lv.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://pd.muxihuayi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ce.gzmigu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://jh.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qm.huixinmuqiang.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fe.nicolike.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hl.jctech888.com.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lt.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vr.hnjuh.cn

[H02] finally / ensure 收尾
来源：http://bw.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://hf.shtwfgs.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ce.shtwfgs.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gr.bjjhwx.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nq.9csxet.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xi.szsharing.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nq.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://cw.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://qw.jctech888.com.cn

[H03] 主动抛出异常
来源：http://rh.bjjhwx.cn

Py:   raise ValueError("错误信息")
来源：http://cc.jianghongdianzi.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qi.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://sa.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://vg.newstarts.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bz.shxzskj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jp.chemitech.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://mx.shxzskj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://io.muxihuayi.cn

[H04] 自定义异常类型
来源：http://oe.hnjuh.cn

Py:   class MyError(Exception): pass
来源：http://oo.newstarts.cn

PHP:  class MyError extends RuntimeException {}
来源：http://dg.521024.cn

JS:   class MyError extends Error {}
来源：http://oy.bjjhwx.cn

TS:   class MyError extends Error {}
来源：http://vu.newstarts.cn

Java: class MyException extends RuntimeException {}
来源：http://tb.shxzukj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fs.muxihuayi.cn

Ruby: class MyError < StandardError; end
来源：http://oj.huanxung.cn

C#:   class MyException : Exception {}
来源：http://cu.9csxet.cn

[H05] 捕获特定类型
来源：http://ek.yuexingan06.cn

Py:   except ValueError as e:
来源：http://qk.bjjhwx.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xq.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://jp.jianghongdianzi.cn

TS:   if (e instanceof TypeError) {}
来源：http://mp.shtwfgs.cn

Java: catch (IOException | SQLException e) {}
来源：http://qd.asd995.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fy.nicolike.cn

Ruby: rescue ArgumentError => e
来源：http://mn.gzmigu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tu.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://uq.521024.cn

Py:   value = d.get("k") or default
来源：http://xs.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vd.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://na.shxzskj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://wo.wgjwhj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mw.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yj.bjjhwx.cn

Ruby: d&.dig(:a, :b)
来源：http://zf.huanxung.cn

C#:   obj?.A?.B ?? default
来源：http://xg.shxzukj.cn

[H07] 断言
来源：http://lm.jianghongdianzi.cn

Py:   assert x > 0, "必须为正"
来源：http://vs.wgjwhj.cn

PHP:  assert($x > 0);
来源：http://tq.hahajie.cn

JS:   console.assert(x > 0);
来源：http://sc.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://qj.hnjuh.cn

Java: assert x > 0 : "必须为正";
来源：http://sc.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hx.9csxet.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kc.colortex.cn

C#:   Debug.Assert(x > 0);
来源：http://zl.huixinmuqiang.cn

[H08] 获取错误信息与堆栈
来源：http://wd.lnxyls.cn

Py:   str(e);  traceback.format_exc()
来源：http://lz.szsharing.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ux.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://ud.chemitech.net.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lt.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://oq.jianghongdianzi.cn

Go:   err.Error()
来源：http://rc.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://jq.jianghongdianzi.cn

C#:   e.Message;  e.StackTrace
来源：http://oz.lnxyls.cn

[H09] 带错误码的异常
来源：http://bf.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dr.shtwfgs.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://se.szxytkj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://rp.huixinmuqiang.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ek.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mp.yuexingan06.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hl.shtwfgs.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pb.nicolike.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://av.colortex.cn

[H10] 资源自动释放
来源：http://dr.haigaiapp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mm.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ha.yuntaijiaju.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hf.szxytkj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://dq.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://tj.muxihuayi.cn

Go:   defer f.Close()
来源：http://zg.nszjky.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://pf.newstarts.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rm.colortex.cn

================================================================================
来源：http://yd.gzmigu.cn

I. 正则表达式
来源：http://kc.jctech888.com.cn

================================================================================
来源：http://co.huanxung.cn

[I01] 判断是否匹配
来源：http://nj.szxytkj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bn.asd995.cn

PHP:  preg_match('/\d+/', $s);
来源：http://zc.lnxyls.cn

JS:   /\d+/.test(s)
来源：http://sh.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://be.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hf.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://od.szsharing.cn

Ruby: s.match?(/\d+/)
来源：http://vm.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mq.yuexingan06.cn

[I02] 提取所有匹配
来源：http://ez.szxytkj.cn

Py:   re.findall(r"\d+", s)
来源：http://wi.chemitech.net.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://jw.9csxet.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yx.9csxet.cn

TS:   s.match(/\d+/g)
来源：http://ub.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://un.muxihuayi.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://yb.gzmigu.cn

Ruby: s.scan(/\d+/)
来源：http://gb.521024.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bg.521024.cn

[I03] 提取捕获分组
来源：http://tr.asd995.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ep.jianghongdianzi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pg.szxytkj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wv.jianghongdianzi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sf.chemitech.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tn.muxihuayi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://uk.jianghongdianzi.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://lx.gzmigu.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rn.wgjwhj.cn

[I04] 正则替换
来源：http://dz.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bm.panjiajie.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tk.nszjky.cn

JS:   s.replace(/\d+/g, "#")
来源：http://uk.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://aj.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pc.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bc.huixiangedu.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://lg.yuexingan06.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pq.bjjhwx.cn

[I05] 按正则拆分
来源：http://cf.huixiangedu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://by.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pt.9csxet.cn

JS:   s.split(/\s*,\s*/)
来源：http://kh.yuexingan06.cn

TS:   s.split(/\s*,\s*/)
来源：http://oy.huanxung.cn

Java: s.split("\\s*,\\s*")
来源：http://tx.newstarts.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wv.9csxet.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jo.yuntaijiaju.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vl.yuexingan06.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://nk.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qa.huanxung.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ip.huixinmuqiang.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sz.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://np.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://st.panjiajie.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://vc.szxytkj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wd.asd995.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tn.hahajie.cn

[I07] 忽略大小写与多行模式
来源：http://ph.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wl.nszjky.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wn.hahajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zd.szsharing.cn

TS:   /error/gim
来源：http://uz.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://lt.jctech888.com.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://sy.521024.cn

Ruby: s.scan(/error/i)
来源：http://qc.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://vq.asd995.cn

[I08] 贪婪与非贪婪匹配
来源：http://gc.newstarts.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yk.521024.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ao.szsharing.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://kg.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vn.shxzskj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://eq.jctech888.com.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ls.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://po.yuexingan06.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ep.yuntaijiaju.cn

================================================================================
来源：http://qf.nicolike.cn

J. 日期与时间
来源：http://ul.shxzukj.cn

================================================================================
来源：http://ol.chemitech.net.cn

[J01] 获取当前时间
来源：http://mt.yuexingan06.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cb.huanxung.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vw.shxzukj.cn

JS:   new Date();  Date.now()
来源：http://mt.colortex.cn

TS:   new Date();  Date.now()
来源：http://zp.szxytkj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lw.gzmigu.cn

Go:   time.Now()
来源：http://ov.9csxet.cn

Ruby: Time.now
来源：http://wc.shxzskj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://lq.lnxyls.cn

[J02] 格式化输出
来源：http://fs.newstarts.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://si.hnjuh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ar.9csxet.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kc.nicolike.cn

TS:   d.toISOString()
来源：http://uv.huanxung.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://yt.shxzskj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://lt.asd995.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fz.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bf.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://pu.9csxet.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qw.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bu.asd995.cn

JS:   new Date("2024-01-02")
来源：http://jv.shxzskj.cn

TS:   new Date("2024-01-02")
来源：http://dj.521024.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tr.huanxung.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://wr.nicolike.cn

Ruby: Date.parse("2024-01-02")
来源：http://xu.chemitech.net.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://xq.shxzukj.cn

[J04] 时间戳与日期互转
来源：http://sj.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vr.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ct.jctech888.com.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tp.wgjwhj.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://if.hnjuh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ne.hnjuh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xq.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://nb.haigaiapp.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://fa.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://oi.huixinmuqiang.cn

Py:   now + timedelta(days=7)
来源：http://wk.haigaiapp.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ru.huixiangedu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sm.szxytkj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mo.huixiangedu.cn

Java: LocalDate.now().plusDays(7)
来源：http://iw.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ik.yuntaijiaju.cn

Ruby: Time.now + 7 * 86400
来源：http://kk.panjiajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gn.huanxung.cn

[J06] 计算两时间之差
来源：http://yw.bookmarksfly.cn

Py:   (end - start).total_seconds()
来源：http://ri.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://fp.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://yk.huanxung.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ff.bookmarksfly.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qy.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://ia.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://qh.newstarts.cn

C#:   (end - start).TotalSeconds
来源：http://km.nszjky.cn

[J07] 比较两个日期
来源：http://lq.9csxet.cn

Py:   d1 < d2;  d1 == d2
来源：http://wu.nszjky.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://bq.colortex.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hh.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cb.9csxet.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://in.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sw.wgjwhj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ym.bookmarksfly.cn

C#:   d1 < d2;  d1 == d2
来源：http://uc.nicolike.cn

[J08] 提取年月日与星期
来源：http://mo.jianghongdianzi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ut.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://di.panjiajie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fi.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ld.bookmarksfly.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://up.panjiajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ck.jctech888.com.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lb.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xy.gzmigu.cn

[J09] 时区处理
来源：http://re.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mo.yuntaijiaju.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://wi.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://up.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bo.newstarts.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://av.bookmarksfly.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xv.shxzskj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://dn.chemitech.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vy.haigaiapp.cn

[J10] 取今天 / 本月第一天
来源：http://xc.huixiangedu.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://li.bookmarksfly.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yu.gzmigu.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oj.muxihuayi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ie.gzmigu.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ui.chemitech.net.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://vj.yuexingan06.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kg.lnxyls.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rt.nicolike.cn

================================================================================
来源：http://zf.9csxet.cn

K. JSON 与序列化
来源：http://fw.yuntaijiaju.cn

================================================================================
来源：http://ce.521024.cn

[K01] 对象转 JSON 字符串
来源：http://dh.yuexingan06.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qc.hnjuh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://td.hnjuh.cn

JS:   JSON.stringify(obj)
来源：http://vl.nszjky.cn

TS:   JSON.stringify(obj)
来源：http://mr.nszjky.cn


<!-- 参考信息 -->