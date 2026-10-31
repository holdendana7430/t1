代发 wailian999

JS:   get name() { return this._name; }
来源：http://li.hnjuh.cn

TS:   get name(): string { return this._name; }
来源：http://cl.szsharing.cn

Java: public String getName() { return name; }
来源：http://by.huixinmuqiang.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://to.yuexingan06.cn

Ruby: attr_accessor :name
来源：http://ro.nicolike.cn

C#:   public string Name { get; set; }
来源：http://eu.newstarts.cn

[G12] 对象转字符串
来源：http://wh.lnxyls.cn

Py:   def __str__(self): return self.name
来源：http://jd.szsharing.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mx.colortex.cn

JS:   toString() { return this.name; }
来源：http://ey.nszjky.cn

TS:   toString(): string { return this.name; }
来源：http://rb.yuexingan06.cn

Java: @Override public String toString() { return name; }
来源：http://yp.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nb.9csxet.cn

Ruby: def to_s; @name; end
来源：http://ye.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://mw.bookmarksfly.cn

[G13] 判断对象类型
来源：http://gx.hnjuh.cn

Py:   isinstance(u, User)
来源：http://jx.shxzskj.cn

PHP:  $u instanceof User
来源：http://gx.huixinmuqiang.cn

JS:   u instanceof User
来源：http://dp.szsharing.cn

TS:   u instanceof User
来源：http://rf.newstarts.cn

Java: u instanceof User
来源：http://yg.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lw.huixinmuqiang.cn

Ruby: u.is_a?(User)
来源：http://pb.wgjwhj.cn

C#:   u is User
来源：http://zo.shxzskj.cn

[G14] 数据类 / record
来源：http://av.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ez.nicolike.cn

PHP:  // 用 readonly 属性模拟
来源：http://av.huixinmuqiang.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fw.bookmarksfly.cn

TS:   type User = { name: string; age: number };
来源：http://jy.gzmigu.cn

Java: record User(String name, int age) {}
来源：http://rx.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://qn.huixiangedu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xq.lnxyls.cn

C#:   record User(string Name, int Age);
来源：http://gc.jianghongdianzi.cn

[G15] 枚举
来源：http://vx.panjiajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ft.jctech888.com.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ru.chemitech.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ze.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wi.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://zj.huixiangedu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qf.jianghongdianzi.cn

Ruby: Color = %i[red green].freeze
来源：http://zh.wgjwhj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yw.chemitech.net.cn

[G16] 对象转数组 / 字典
来源：http://ws.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wn.bjjhwx.cn

PHP:  get_object_vars($obj);
来源：http://gr.szsharing.cn

JS:   Object.entries(obj)
来源：http://wd.9csxet.cn

TS:   Object.entries(obj)
来源：http://da.shxzskj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ni.hahajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://yp.huixiangedu.cn

Ruby: obj.instance_variables
来源：http://sr.bjjhwx.cn

C#:   // 用反射或 System.Text.Json
来源：http://lp.hahajie.cn

================================================================================
来源：http://tt.newstarts.cn

H. 异常与错误处理
来源：http://qr.szxytkj.cn

================================================================================
来源：http://di.jctech888.com.cn

[H01] try / catch 基础
来源：http://pj.szsharing.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ni.hahajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zs.szsharing.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mu.yuexingan06.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://od.huanxung.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mv.bookmarksfly.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gf.szxytkj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://oc.gzmigu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uf.asd995.cn

[H02] finally / ensure 收尾
来源：http://rl.jctech888.com.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sh.nszjky.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://iw.bjjhwx.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://oy.shxzukj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qg.hnjuh.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kf.szsharing.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://eb.colortex.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ru.chemitech.net.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://so.shxzukj.cn

[H03] 主动抛出异常
来源：http://mb.hnjuh.cn

Py:   raise ValueError("错误信息")
来源：http://kp.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xu.muxihuayi.cn

JS:   throw new Error("错误信息");
来源：http://zr.huixiangedu.cn

TS:   throw new Error("错误信息");
来源：http://xc.wgjwhj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qe.yuntaijiaju.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gl.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://it.newstarts.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nk.muxihuayi.cn

[H04] 自定义异常类型
来源：http://uj.haigaiapp.cn

Py:   class MyError(Exception): pass
来源：http://rt.colortex.cn

PHP:  class MyError extends RuntimeException {}
来源：http://md.huixinmuqiang.cn

JS:   class MyError extends Error {}
来源：http://iq.muxihuayi.cn

TS:   class MyError extends Error {}
来源：http://fm.nicolike.cn

Java: class MyException extends RuntimeException {}
来源：http://hw.hahajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://jz.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://tu.shxzukj.cn

C#:   class MyException : Exception {}
来源：http://gu.newstarts.cn

[H05] 捕获特定类型
来源：http://mk.wgjwhj.cn

Py:   except ValueError as e:
来源：http://hj.jctech888.com.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://fp.panjiajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://hb.panjiajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://ce.chemitech.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://zh.9csxet.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://cp.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://fd.hnjuh.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://st.9csxet.cn

[H06] 可选值 / 空值安全访问
来源：http://ms.shxzukj.cn

Py:   value = d.get("k") or default
来源：http://xc.huixinmuqiang.cn

PHP:  $v = $d["k"] ?? null;
来源：http://wy.hnjuh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://tw.gzmigu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ej.shtwfgs.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mw.gzmigu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://co.jianghongdianzi.cn

Ruby: d&.dig(:a, :b)
来源：http://xb.gzmigu.cn

C#:   obj?.A?.B ?? default
来源：http://uq.bjjhwx.cn

[H07] 断言
来源：http://up.muxihuayi.cn

Py:   assert x > 0, "必须为正"
来源：http://dq.shtwfgs.cn

PHP:  assert($x > 0);
来源：http://hv.yuexingan06.cn

JS:   console.assert(x > 0);
来源：http://jr.haigaiapp.cn

TS:   console.assert(x > 0);
来源：http://ff.szxytkj.cn

Java: assert x > 0 : "必须为正";
来源：http://rj.huixiangedu.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bz.colortex.cn

Ruby: raise "必须为正" unless x > 0
来源：http://sn.hnjuh.cn

C#:   Debug.Assert(x > 0);
来源：http://mb.nszjky.cn

[H08] 获取错误信息与堆栈
来源：http://sl.colortex.cn

Py:   str(e);  traceback.format_exc()
来源：http://an.shxzskj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bi.521024.cn

JS:   e.message;  e.stack
来源：http://jo.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lk.szsharing.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://pf.bjjhwx.cn

Go:   err.Error()
来源：http://km.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://jb.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://hf.szsharing.cn

[H09] 带错误码的异常
来源：http://nv.muxihuayi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nm.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tw.shxzskj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ya.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zd.hahajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rc.shxzskj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fo.hnjuh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://un.szxytkj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ld.szxytkj.cn

[H10] 资源自动释放
来源：http://hy.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jm.9csxet.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://an.9csxet.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qc.hahajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ci.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://iy.lnxyls.cn

Go:   defer f.Close()
来源：http://oc.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://eb.gzmigu.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://fs.shtwfgs.cn

================================================================================
来源：http://ka.bjjhwx.cn

I. 正则表达式
来源：http://zj.shxzukj.cn

================================================================================
来源：http://kk.gzmigu.cn

[I01] 判断是否匹配
来源：http://fe.colortex.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://xv.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bo.521024.cn

JS:   /\d+/.test(s)
来源：http://we.yuntaijiaju.cn

TS:   /\d+/.test(s)
来源：http://ab.521024.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gc.bjjhwx.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ho.szsharing.cn

Ruby: s.match?(/\d+/)
来源：http://hh.shxzskj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://yo.nszjky.cn

[I02] 提取所有匹配
来源：http://wx.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://hf.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wr.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ki.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://ey.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yf.521024.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nx.jianghongdianzi.cn

Ruby: s.scan(/\d+/)
来源：http://op.newstarts.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://av.szxytkj.cn

[I03] 提取捕获分组
来源：http://lg.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ns.hahajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ic.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pd.asd995.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sa.521024.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://fm.muxihuayi.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vy.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://za.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gh.szxytkj.cn

[I04] 正则替换
来源：http://ow.nicolike.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ci.bookmarksfly.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wi.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://mc.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://la.521024.cn

Java: s.replaceAll("\\d+", "#")
来源：http://aa.colortex.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xc.szsharing.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zh.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://so.asd995.cn

[I05] 按正则拆分
来源：http://cf.shtwfgs.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://sj.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://kg.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://up.nicolike.cn

TS:   s.split(/\s*,\s*/)
来源：http://fp.wgjwhj.cn

Java: s.split("\\s*,\\s*")
来源：http://pl.bookmarksfly.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://er.shxzukj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ig.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://rp.colortex.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://px.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zj.szxytkj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gp.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://by.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ov.asd995.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zl.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pw.9csxet.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://oc.hahajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ut.nicolike.cn

[I07] 忽略大小写与多行模式
来源：http://op.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://so.huixinmuqiang.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xr.bookmarksfly.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cx.nicolike.cn

TS:   /error/gim
来源：http://yt.bookmarksfly.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://yg.nszjky.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ij.huanxung.cn

Ruby: s.scan(/error/i)
来源：http://sd.jctech888.com.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oa.chemitech.net.cn

[I08] 贪婪与非贪婪匹配
来源：http://xj.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wd.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hj.colortex.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://at.newstarts.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yr.hahajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vp.521024.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hg.shtwfgs.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zq.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://nd.chemitech.net.cn

================================================================================
来源：http://ef.shtwfgs.cn

J. 日期与时间
来源：http://qv.newstarts.cn

================================================================================
来源：http://oj.muxihuayi.cn

[J01] 获取当前时间
来源：http://ma.huixinmuqiang.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ja.asd995.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://jf.bjjhwx.cn

JS:   new Date();  Date.now()
来源：http://ke.521024.cn

TS:   new Date();  Date.now()
来源：http://zn.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mb.9csxet.cn

Go:   time.Now()
来源：http://lp.hnjuh.cn

Ruby: Time.now
来源：http://js.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wt.jianghongdianzi.cn

[J02] 格式化输出
来源：http://re.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sj.nszjky.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nd.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ep.chemitech.net.cn

TS:   d.toISOString()
来源：http://mm.hahajie.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ke.yuexingan06.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ak.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dd.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://cp.shxzukj.cn

[J03] 字符串解析为日期
来源：http://vd.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://sy.hnjuh.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://lq.521024.cn

JS:   new Date("2024-01-02")
来源：http://gr.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://fi.shxzukj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://da.szxytkj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://dx.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://un.yuexingan06.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://jp.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://dt.nicolike.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sb.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://nt.haigaiapp.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zk.asd995.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://th.huixiangedu.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://pf.colortex.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://um.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hj.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kw.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://nb.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://st.521024.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://tu.chemitech.net.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://sc.lnxyls.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://md.gzmigu.cn

Java: LocalDate.now().plusDays(7)
来源：http://gu.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://px.huanxung.cn

Ruby: Time.now + 7 * 86400
来源：http://tt.haigaiapp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://kp.nszjky.cn

[J06] 计算两时间之差
来源：http://rj.newstarts.cn

Py:   (end - start).total_seconds()
来源：http://wx.huanxung.cn

PHP:  $end->diff($start)->days;
来源：http://zo.nszjky.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xy.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://as.huixiangedu.cn

Java: Duration.between(start, end).toSeconds()
来源：http://kh.muxihuayi.cn

Go:   end.Sub(start).Hours()
来源：http://tn.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://sg.521024.cn

C#:   (end - start).TotalSeconds
来源：http://kg.jianghongdianzi.cn

[J07] 比较两个日期
来源：http://zn.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://oq.huixinmuqiang.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://om.asd995.cn

JS:   d1.getTime() < d2.getTime()
来源：http://if.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gs.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uu.shxzskj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pc.gzmigu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://oa.yuntaijiaju.cn

C#:   d1 < d2;  d1 == d2
来源：http://zl.shxzskj.cn

[J08] 提取年月日与星期
来源：http://sl.nszjky.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gw.hahajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ej.hnjuh.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://as.shtwfgs.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://le.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://za.bjjhwx.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://go.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pu.colortex.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xq.nicolike.cn

[J09] 时区处理
来源：http://rb.yuexingan06.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rw.9csxet.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ea.hahajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ik.hahajie.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xe.haigaiapp.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qe.muxihuayi.cn


<!-- 参考信息 -->