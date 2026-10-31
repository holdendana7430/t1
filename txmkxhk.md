代发 wailian999

Ruby: attr_accessor :name
来源：http://ew.gzmigu.cn

C#:   public string Name { get; set; }
来源：http://se.chemitech.net.cn

[G12] 对象转字符串
来源：http://gn.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://wn.jctech888.com.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rx.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://zj.szsharing.cn

TS:   toString(): string { return this.name; }
来源：http://ni.szsharing.cn

Java: @Override public String toString() { return name; }
来源：http://dz.521024.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mc.shxzskj.cn

Ruby: def to_s; @name; end
来源：http://tb.9csxet.cn

C#:   public override string ToString() => Name;
来源：http://oy.asd995.cn

[G13] 判断对象类型
来源：http://km.bjjhwx.cn

Py:   isinstance(u, User)
来源：http://dp.521024.cn

PHP:  $u instanceof User
来源：http://oa.9csxet.cn

JS:   u instanceof User
来源：http://jc.9csxet.cn

TS:   u instanceof User
来源：http://pw.9csxet.cn

Java: u instanceof User
来源：http://aa.huanxung.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kp.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://xc.lnxyls.cn

C#:   u is User
来源：http://at.muxihuayi.cn

[G14] 数据类 / record
来源：http://lb.huixinmuqiang.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vu.521024.cn

PHP:  // 用 readonly 属性模拟
来源：http://kq.bjjhwx.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pl.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://kt.shtwfgs.cn

Java: record User(String name, int age) {}
来源：http://zw.jianghongdianzi.cn

Go:   type User struct { Name string; Age int }
来源：http://ir.bjjhwx.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://tk.szxytkj.cn

C#:   record User(string Name, int Age);
来源：http://bo.szxytkj.cn

[G15] 枚举
来源：http://xu.chemitech.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://oo.huixiangedu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rc.9csxet.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qs.muxihuayi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://aj.521024.cn

Java: enum Color { RED, GREEN }
来源：http://ec.gzmigu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://fb.yuexingan06.cn

Ruby: Color = %i[red green].freeze
来源：http://xl.hahajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hc.muxihuayi.cn

[G16] 对象转数组 / 字典
来源：http://ft.gzmigu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ju.muxihuayi.cn

PHP:  get_object_vars($obj);
来源：http://oq.hnjuh.cn

JS:   Object.entries(obj)
来源：http://an.yuntaijiaju.cn

TS:   Object.entries(obj)
来源：http://eh.bookmarksfly.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wi.shxzukj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nx.shtwfgs.cn

Ruby: obj.instance_variables
来源：http://kd.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://br.shtwfgs.cn

================================================================================
来源：http://fm.jianghongdianzi.cn

H. 异常与错误处理
来源：http://dd.muxihuayi.cn

================================================================================
来源：http://lm.szsharing.cn

[H01] try / catch 基础
来源：http://iy.muxihuayi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://rq.colortex.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qf.bookmarksfly.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://pw.shtwfgs.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zu.newstarts.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qy.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rw.9csxet.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lr.jctech888.com.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pd.asd995.cn

[H02] finally / ensure 收尾
来源：http://tc.newstarts.cn

Py:   try: f()⏎finally: cleanup()
来源：http://gm.hnjuh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yc.panjiajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vo.haigaiapp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ym.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://eg.hnjuh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lr.bookmarksfly.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sq.muxihuayi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xk.newstarts.cn

[H03] 主动抛出异常
来源：http://hg.bookmarksfly.cn

Py:   raise ValueError("错误信息")
来源：http://id.yuntaijiaju.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sl.nicolike.cn

JS:   throw new Error("错误信息");
来源：http://ba.huixiangedu.cn

TS:   throw new Error("错误信息");
来源：http://ob.jctech888.com.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vr.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gr.bjjhwx.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hh.bookmarksfly.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gy.wgjwhj.cn

[H04] 自定义异常类型
来源：http://oj.521024.cn

Py:   class MyError(Exception): pass
来源：http://gi.yuexingan06.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fm.szsharing.cn

JS:   class MyError extends Error {}
来源：http://pd.colortex.cn

TS:   class MyError extends Error {}
来源：http://ew.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://dw.9csxet.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xn.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://ky.chemitech.net.cn

C#:   class MyException : Exception {}
来源：http://ba.huixiangedu.cn

[H05] 捕获特定类型
来源：http://do.nicolike.cn

Py:   except ValueError as e:
来源：http://wo.shxzukj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ow.szxytkj.cn

JS:   if (e instanceof TypeError) {}
来源：http://sn.yuntaijiaju.cn

TS:   if (e instanceof TypeError) {}
来源：http://ff.gzmigu.cn

Java: catch (IOException | SQLException e) {}
来源：http://da.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xh.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://ky.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pt.bookmarksfly.cn

[H06] 可选值 / 空值安全访问
来源：http://fg.hahajie.cn

Py:   value = d.get("k") or default
来源：http://ya.gzmigu.cn

PHP:  $v = $d["k"] ?? null;
来源：http://vq.haigaiapp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bx.huanxung.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zc.huixinmuqiang.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ok.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://gh.shxzukj.cn

Ruby: d&.dig(:a, :b)
来源：http://cu.jctech888.com.cn

C#:   obj?.A?.B ?? default
来源：http://up.asd995.cn

[H07] 断言
来源：http://oa.szxytkj.cn

Py:   assert x > 0, "必须为正"
来源：http://gq.nicolike.cn

PHP:  assert($x > 0);
来源：http://km.haigaiapp.cn

JS:   console.assert(x > 0);
来源：http://ak.jctech888.com.cn

TS:   console.assert(x > 0);
来源：http://vn.asd995.cn

Java: assert x > 0 : "必须为正";
来源：http://st.nicolike.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pw.szxytkj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vn.haigaiapp.cn

C#:   Debug.Assert(x > 0);
来源：http://ms.521024.cn

[H08] 获取错误信息与堆栈
来源：http://zu.yuntaijiaju.cn

Py:   str(e);  traceback.format_exc()
来源：http://qq.huanxung.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://is.colortex.cn

JS:   e.message;  e.stack
来源：http://ie.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://aa.szxytkj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cj.panjiajie.cn

Go:   err.Error()
来源：http://vs.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://gs.jctech888.com.cn

C#:   e.Message;  e.StackTrace
来源：http://to.panjiajie.cn

[H09] 带错误码的异常
来源：http://pv.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://gm.muxihuayi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://om.hnjuh.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jz.jctech888.com.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mw.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://lr.wgjwhj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tk.lnxyls.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ed.bjjhwx.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://kr.huixinmuqiang.cn

[H10] 资源自动释放
来源：http://qo.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bo.asd995.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://am.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://db.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ie.shxzskj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://bu.yuntaijiaju.cn

Go:   defer f.Close()
来源：http://ms.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://og.huixinmuqiang.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nx.panjiajie.cn

================================================================================
来源：http://sd.hnjuh.cn

I. 正则表达式
来源：http://wy.hnjuh.cn

================================================================================
来源：http://pd.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://oe.gzmigu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fp.szxytkj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rr.colortex.cn

JS:   /\d+/.test(s)
来源：http://pi.9csxet.cn

TS:   /\d+/.test(s)
来源：http://xn.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ex.szsharing.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ki.panjiajie.cn

Ruby: s.match?(/\d+/)
来源：http://wn.jctech888.com.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://zx.huixinmuqiang.cn

[I02] 提取所有匹配
来源：http://mt.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://lg.9csxet.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://yo.haigaiapp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://eb.colortex.cn

TS:   s.match(/\d+/g)
来源：http://al.asd995.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vn.asd995.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qj.asd995.cn

Ruby: s.scan(/\d+/)
来源：http://hk.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hf.gzmigu.cn

[I03] 提取捕获分组
来源：http://rf.nszjky.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vu.521024.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://fj.yuntaijiaju.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://kv.hahajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://py.wgjwhj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dc.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://aw.panjiajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://bb.nszjky.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qt.shxzskj.cn

[I04] 正则替换
来源：http://jd.521024.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://il.huixinmuqiang.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xx.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://qn.hnjuh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yt.yuexingan06.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pv.bjjhwx.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dr.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rv.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qj.shxzukj.cn

[I05] 按正则拆分
来源：http://da.lnxyls.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://jq.wgjwhj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yj.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://dq.shxzukj.cn

TS:   s.split(/\s*,\s*/)
来源：http://hb.huanxung.cn

Java: s.split("\\s*,\\s*")
来源：http://dz.asd995.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://va.hnjuh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://af.newstarts.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://if.haigaiapp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://tz.gzmigu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ia.nszjky.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ix.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yb.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fu.szsharing.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pe.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://fk.shtwfgs.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ow.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fo.hnjuh.cn

[I07] 忽略大小写与多行模式
来源：http://vt.haigaiapp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mk.huanxung.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wi.gzmigu.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qp.huixinmuqiang.cn

TS:   /error/gim
来源：http://cw.haigaiapp.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wf.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://eb.chemitech.net.cn

Ruby: s.scan(/error/i)
来源：http://kg.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://th.jianghongdianzi.cn

[I08] 贪婪与非贪婪匹配
来源：http://xn.521024.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wz.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://xd.muxihuayi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ox.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://us.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nd.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vw.huixinmuqiang.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mo.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ow.hnjuh.cn

================================================================================
来源：http://pu.shtwfgs.cn

J. 日期与时间
来源：http://qd.gzmigu.cn

================================================================================
来源：http://co.9csxet.cn

[J01] 获取当前时间
来源：http://hu.jctech888.com.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ut.huanxung.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ex.colortex.cn

JS:   new Date();  Date.now()
来源：http://qh.shtwfgs.cn

TS:   new Date();  Date.now()
来源：http://ms.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://nz.wgjwhj.cn

Go:   time.Now()
来源：http://di.szsharing.cn

Ruby: Time.now
来源：http://wu.asd995.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uq.bookmarksfly.cn

[J02] 格式化输出
来源：http://xy.hnjuh.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wx.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hn.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://lz.lnxyls.cn

TS:   d.toISOString()
来源：http://zh.szxytkj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://sn.shxzskj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://py.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zt.huixiangedu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://dy.shtwfgs.cn

[J03] 字符串解析为日期
来源：http://wt.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://nm.szsharing.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://kk.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://gy.shxzukj.cn

TS:   new Date("2024-01-02")
来源：http://to.panjiajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qh.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://db.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://jg.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://kf.shxzskj.cn

[J04] 时间戳与日期互转
来源：http://yj.haigaiapp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ll.521024.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://km.gzmigu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cm.colortex.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://we.haigaiapp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ft.shxzskj.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mp.muxihuayi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://zx.huanxung.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://nm.szxytkj.cn

[J05] 时间加减（加 7 天）
来源：http://pt.gzmigu.cn

Py:   now + timedelta(days=7)
来源：http://nl.chemitech.net.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://cm.hahajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://cv.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ns.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://zn.yuexingan06.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://cq.shxzskj.cn

Ruby: Time.now + 7 * 86400
来源：http://qb.huanxung.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dh.asd995.cn

[J06] 计算两时间之差
来源：http://nc.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://mn.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://ey.jctech888.com.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xi.muxihuayi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xf.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://li.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://qs.nszjky.cn

Ruby: end - start                 # 返回秒数
来源：http://xr.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://bg.yuexingan06.cn

[J07] 比较两个日期
来源：http://fo.huanxung.cn

Py:   d1 < d2;  d1 == d2
来源：http://tp.huanxung.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hw.jianghongdianzi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xn.shxzukj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://yr.chemitech.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fc.asd995.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dj.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ws.szsharing.cn

C#:   d1 < d2;  d1 == d2
来源：http://mn.nszjky.cn

[J08] 提取年月日与星期
来源：http://lc.colortex.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vb.szsharing.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://da.lnxyls.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://qb.muxihuayi.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ln.szxytkj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://li.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fo.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://jy.colortex.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zo.jianghongdianzi.cn

[J09] 时区处理
来源：http://zj.lnxyls.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qu.bjjhwx.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fr.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://it.bookmarksfly.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sm.asd995.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kf.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fr.shxzukj.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kk.yuntaijiaju.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://eo.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://bv.shxzskj.cn


<!-- 参考信息 -->