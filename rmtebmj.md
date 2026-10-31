代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://mv.bookmarksfly.cn

JS:   toString() { return this.name; }
来源：http://ap.huixiangedu.cn

TS:   toString(): string { return this.name; }
来源：http://cn.lnxyls.cn

Java: @Override public String toString() { return name; }
来源：http://wo.szxytkj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://oh.wgjwhj.cn

Ruby: def to_s; @name; end
来源：http://ck.nszjky.cn

C#:   public override string ToString() => Name;
来源：http://mh.muxihuayi.cn

[G13] 判断对象类型
来源：http://yy.chemitech.net.cn

Py:   isinstance(u, User)
来源：http://ds.shxzukj.cn

PHP:  $u instanceof User
来源：http://tm.wgjwhj.cn

JS:   u instanceof User
来源：http://nq.shxzukj.cn

TS:   u instanceof User
来源：http://uj.huanxung.cn

Java: u instanceof User
来源：http://ud.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gm.hnjuh.cn

Ruby: u.is_a?(User)
来源：http://ej.nicolike.cn

C#:   u is User
来源：http://fn.bookmarksfly.cn

[G14] 数据类 / record
来源：http://no.bjjhwx.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nx.huanxung.cn

PHP:  // 用 readonly 属性模拟
来源：http://ud.521024.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nb.huixinmuqiang.cn

TS:   type User = { name: string; age: number };
来源：http://xo.9csxet.cn

Java: record User(String name, int age) {}
来源：http://bv.nszjky.cn

Go:   type User struct { Name string; Age int }
来源：http://df.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yn.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://sk.haigaiapp.cn

[G15] 枚举
来源：http://fo.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://aa.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ed.nicolike.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vu.jctech888.com.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wn.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://uv.bookmarksfly.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vt.huixiangedu.cn

Ruby: Color = %i[red green].freeze
来源：http://yt.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ub.lnxyls.cn

[G16] 对象转数组 / 字典
来源：http://ne.521024.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wi.asd995.cn

PHP:  get_object_vars($obj);
来源：http://lq.jctech888.com.cn

JS:   Object.entries(obj)
来源：http://ba.nszjky.cn

TS:   Object.entries(obj)
来源：http://wx.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://qs.shxzskj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xj.huixinmuqiang.cn

Ruby: obj.instance_variables
来源：http://rs.nicolike.cn

C#:   // 用反射或 System.Text.Json
来源：http://lu.shxzukj.cn

================================================================================
来源：http://dj.521024.cn

H. 异常与错误处理
来源：http://nj.newstarts.cn

================================================================================
来源：http://ab.hnjuh.cn

[H01] try / catch 基础
来源：http://ut.hahajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://qk.huanxung.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wi.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mt.colortex.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://bu.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hy.chemitech.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tx.colortex.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fd.huanxung.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zb.asd995.cn

[H02] finally / ensure 收尾
来源：http://rq.9csxet.cn

Py:   try: f()⏎finally: cleanup()
来源：http://zp.9csxet.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://vn.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hm.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rd.wgjwhj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zp.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nr.521024.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://bb.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hf.asd995.cn

[H03] 主动抛出异常
来源：http://rd.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://vu.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yk.newstarts.cn

JS:   throw new Error("错误信息");
来源：http://aa.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://kz.yuntaijiaju.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rd.szxytkj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://au.bookmarksfly.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ck.shxzskj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tr.huixiangedu.cn

[H04] 自定义异常类型
来源：http://sk.panjiajie.cn

Py:   class MyError(Exception): pass
来源：http://pq.521024.cn

PHP:  class MyError extends RuntimeException {}
来源：http://hb.shtwfgs.cn

JS:   class MyError extends Error {}
来源：http://ud.521024.cn

TS:   class MyError extends Error {}
来源：http://aq.shxzukj.cn

Java: class MyException extends RuntimeException {}
来源：http://hm.asd995.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nb.szsharing.cn

Ruby: class MyError < StandardError; end
来源：http://xy.shxzukj.cn

C#:   class MyException : Exception {}
来源：http://ed.bookmarksfly.cn

[H05] 捕获特定类型
来源：http://et.jctech888.com.cn

Py:   except ValueError as e:
来源：http://fq.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ij.huixinmuqiang.cn

JS:   if (e instanceof TypeError) {}
来源：http://ke.hahajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://sc.bjjhwx.cn

Java: catch (IOException | SQLException e) {}
来源：http://aj.gzmigu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vy.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://ju.bookmarksfly.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://yc.shxzskj.cn

[H06] 可选值 / 空值安全访问
来源：http://wt.huanxung.cn

Py:   value = d.get("k") or default
来源：http://er.hnjuh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://qh.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://up.newstarts.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tn.shxzukj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://km.shxzukj.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bh.huixinmuqiang.cn

Ruby: d&.dig(:a, :b)
来源：http://sq.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://ut.colortex.cn

[H07] 断言
来源：http://pl.yuexingan06.cn

Py:   assert x > 0, "必须为正"
来源：http://tm.yuntaijiaju.cn

PHP:  assert($x > 0);
来源：http://kr.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://rb.newstarts.cn

TS:   console.assert(x > 0);
来源：http://tm.wgjwhj.cn

Java: assert x > 0 : "必须为正";
来源：http://tf.muxihuayi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nh.bookmarksfly.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tw.newstarts.cn

C#:   Debug.Assert(x > 0);
来源：http://he.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://mn.huanxung.cn

Py:   str(e);  traceback.format_exc()
来源：http://bd.shtwfgs.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tk.shtwfgs.cn

JS:   e.message;  e.stack
来源：http://hf.colortex.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://un.panjiajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ef.shtwfgs.cn

Go:   err.Error()
来源：http://ls.lnxyls.cn

Ruby: e.message;  e.backtrace
来源：http://qx.lnxyls.cn

C#:   e.Message;  e.StackTrace
来源：http://sf.hahajie.cn

[H09] 带错误码的异常
来源：http://qv.yuntaijiaju.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://dm.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kz.9csxet.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cu.muxihuayi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://le.jianghongdianzi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mp.gzmigu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vk.wgjwhj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xp.huixinmuqiang.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qc.huixiangedu.cn

[H10] 资源自动释放
来源：http://pi.shtwfgs.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ms.szsharing.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://er.jctech888.com.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ta.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://rh.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ry.yuntaijiaju.cn

Go:   defer f.Close()
来源：http://ty.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kc.colortex.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://tz.chemitech.net.cn

================================================================================
来源：http://sb.shxzukj.cn

I. 正则表达式
来源：http://po.muxihuayi.cn

================================================================================
来源：http://ht.haigaiapp.cn

[I01] 判断是否匹配
来源：http://kf.521024.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mh.shtwfgs.cn

PHP:  preg_match('/\d+/', $s);
来源：http://qj.hahajie.cn

JS:   /\d+/.test(s)
来源：http://rx.lnxyls.cn

TS:   /\d+/.test(s)
来源：http://yb.521024.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qr.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bb.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://jx.wgjwhj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dx.huanxung.cn

[I02] 提取所有匹配
来源：http://ur.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://xm.huanxung.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zw.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dw.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://ij.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ym.nicolike.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://cg.shxzskj.cn

Ruby: s.scan(/\d+/)
来源：http://pd.yuntaijiaju.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ze.chemitech.net.cn

[I03] 提取捕获分组
来源：http://tt.szsharing.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sh.hnjuh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rv.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://yn.shxzukj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cu.colortex.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://qj.newstarts.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://lg.9csxet.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://my.bookmarksfly.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ex.newstarts.cn

[I04] 正则替换
来源：http://ev.colortex.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://il.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ho.huixinmuqiang.cn

JS:   s.replace(/\d+/g, "#")
来源：http://lo.colortex.cn

TS:   s.replace(/\d+/g, "#")
来源：http://om.panjiajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://tw.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ac.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://po.chemitech.net.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vz.bjjhwx.cn

[I05] 按正则拆分
来源：http://ea.chemitech.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vt.shtwfgs.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://al.nszjky.cn

JS:   s.split(/\s*,\s*/)
来源：http://sq.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://np.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://jl.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xw.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://am.nszjky.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ut.yuexingan06.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sx.yuntaijiaju.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://rg.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fw.yuntaijiaju.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iu.szxytkj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://td.nszjky.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yx.shxzskj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://iw.yuntaijiaju.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ld.yuexingan06.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://vr.jctech888.com.cn

[I07] 忽略大小写与多行模式
来源：http://im.nszjky.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ew.jianghongdianzi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mj.yuexingan06.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://zn.colortex.cn

TS:   /error/gim
来源：http://uf.panjiajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dm.huixiangedu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lu.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://mo.wgjwhj.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://xq.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://bq.huixinmuqiang.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mc.szsharing.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://of.bookmarksfly.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jk.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ea.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://or.yuntaijiaju.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://rr.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://gu.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://zf.yuexingan06.cn

================================================================================
来源：http://ej.jctech888.com.cn

J. 日期与时间
来源：http://bz.wgjwhj.cn

================================================================================
来源：http://ft.panjiajie.cn

[J01] 获取当前时间
来源：http://qf.panjiajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ob.huanxung.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cl.szsharing.cn

JS:   new Date();  Date.now()
来源：http://ng.nszjky.cn

TS:   new Date();  Date.now()
来源：http://ps.9csxet.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ss.asd995.cn

Go:   time.Now()
来源：http://za.muxihuayi.cn

Ruby: Time.now
来源：http://hu.szxytkj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cw.gzmigu.cn

[J02] 格式化输出
来源：http://rr.asd995.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uv.shtwfgs.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rh.panjiajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mi.hnjuh.cn

TS:   d.toISOString()
来源：http://qg.hnjuh.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ga.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nr.jianghongdianzi.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qf.shtwfgs.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://kn.huixiangedu.cn

[J03] 字符串解析为日期
来源：http://dg.jctech888.com.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://dq.bjjhwx.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kw.521024.cn

JS:   new Date("2024-01-02")
来源：http://jx.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://lr.yuexingan06.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xi.huixinmuqiang.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hd.colortex.cn

Ruby: Date.parse("2024-01-02")
来源：http://dh.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qc.shtwfgs.cn

[J04] 时间戳与日期互转
来源：http://bp.gzmigu.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vp.shxzukj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://lv.bjjhwx.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gf.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ma.bookmarksfly.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://xm.panjiajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://oc.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://il.lnxyls.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ux.shtwfgs.cn

[J05] 时间加减（加 7 天）
来源：http://cs.521024.cn

Py:   now + timedelta(days=7)
来源：http://ne.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lz.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ta.jianghongdianzi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vp.haigaiapp.cn

Java: LocalDate.now().plusDays(7)
来源：http://wn.bookmarksfly.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zh.hahajie.cn

Ruby: Time.now + 7 * 86400
来源：http://fo.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ei.lnxyls.cn

[J06] 计算两时间之差
来源：http://la.szsharing.cn

Py:   (end - start).total_seconds()
来源：http://ep.yuexingan06.cn

PHP:  $end->diff($start)->days;
来源：http://se.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://rh.nicolike.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dt.bookmarksfly.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sx.newstarts.cn

Go:   end.Sub(start).Hours()
来源：http://gs.colortex.cn

Ruby: end - start                 # 返回秒数
来源：http://mx.huanxung.cn

C#:   (end - start).TotalSeconds
来源：http://oh.521024.cn

[J07] 比较两个日期
来源：http://wr.shxzskj.cn

Py:   d1 < d2;  d1 == d2
来源：http://kp.jianghongdianzi.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ay.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ho.muxihuayi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ta.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tp.wgjwhj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://nj.szsharing.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bx.gzmigu.cn

C#:   d1 < d2;  d1 == d2
来源：http://ih.nszjky.cn

[J08] 提取年月日与星期
来源：http://at.huixiangedu.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pt.newstarts.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://bm.colortex.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ke.lnxyls.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://cj.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tg.gzmigu.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://da.chemitech.net.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bv.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jh.haigaiapp.cn

[J09] 时区处理
来源：http://jh.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ya.shxzskj.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zh.haigaiapp.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fu.huanxung.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lj.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://xv.shxzukj.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lk.asd995.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ke.shxzukj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://tt.shtwfgs.cn

[J10] 取今天 / 本月第一天
来源：http://ft.nszjky.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://aa.yuexingan06.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ik.newstarts.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jq.bookmarksfly.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ib.panjiajie.cn


<!-- 参考信息 -->