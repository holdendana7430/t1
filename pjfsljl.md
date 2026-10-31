代发 wailian999

Ruby: attr_accessor :name
来源：http://yo.bookmarksfly.cn

C#:   public string Name { get; set; }
来源：http://ck.shxzukj.cn

[G12] 对象转字符串
来源：http://bs.jianghongdianzi.cn

Py:   def __str__(self): return self.name
来源：http://ia.nicolike.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mc.asd995.cn

JS:   toString() { return this.name; }
来源：http://bq.hnjuh.cn

TS:   toString(): string { return this.name; }
来源：http://jd.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://hr.newstarts.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zr.521024.cn

Ruby: def to_s; @name; end
来源：http://dj.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://zd.huixinmuqiang.cn

[G13] 判断对象类型
来源：http://dj.nszjky.cn

Py:   isinstance(u, User)
来源：http://yd.shtwfgs.cn

PHP:  $u instanceof User
来源：http://ki.asd995.cn

JS:   u instanceof User
来源：http://pd.newstarts.cn

TS:   u instanceof User
来源：http://fz.haigaiapp.cn

Java: u instanceof User
来源：http://fz.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://he.asd995.cn

Ruby: u.is_a?(User)
来源：http://gu.shxzukj.cn

C#:   u is User
来源：http://mi.huanxung.cn

[G14] 数据类 / record
来源：http://bu.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kt.hnjuh.cn

PHP:  // 用 readonly 属性模拟
来源：http://eq.huixiangedu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hm.nicolike.cn

TS:   type User = { name: string; age: number };
来源：http://po.huanxung.cn

Java: record User(String name, int age) {}
来源：http://ew.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://qy.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ff.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://fo.jianghongdianzi.cn

[G15] 枚举
来源：http://fg.yuexingan06.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qm.yuntaijiaju.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bx.nszjky.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sy.szsharing.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ra.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://xh.huixiangedu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://se.nszjky.cn

Ruby: Color = %i[red green].freeze
来源：http://ya.jianghongdianzi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ag.newstarts.cn

[G16] 对象转数组 / 字典
来源：http://wr.huixiangedu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qh.bjjhwx.cn

PHP:  get_object_vars($obj);
来源：http://dk.bjjhwx.cn

JS:   Object.entries(obj)
来源：http://kk.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://hq.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://of.9csxet.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://jy.hnjuh.cn

Ruby: obj.instance_variables
来源：http://xw.bookmarksfly.cn

C#:   // 用反射或 System.Text.Json
来源：http://bp.9csxet.cn

================================================================================
来源：http://bx.wgjwhj.cn

H. 异常与错误处理
来源：http://pr.shxzskj.cn

================================================================================
来源：http://xf.asd995.cn

[H01] try / catch 基础
来源：http://df.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ov.wgjwhj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kj.huixiangedu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ni.lnxyls.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://sj.jctech888.com.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fe.shxzskj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://dz.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://re.shxzskj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iy.shtwfgs.cn

[H02] finally / ensure 收尾
来源：http://in.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wr.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wp.shxzskj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://dw.shxzukj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gh.szsharing.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ro.nicolike.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://jw.muxihuayi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gk.nicolike.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://nc.521024.cn

[H03] 主动抛出异常
来源：http://mf.yuntaijiaju.cn

Py:   raise ValueError("错误信息")
来源：http://zh.nicolike.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ri.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://yu.jctech888.com.cn

TS:   throw new Error("错误信息");
来源：http://jv.nicolike.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://oa.jianghongdianzi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://to.nicolike.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kb.gzmigu.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zg.lnxyls.cn

[H04] 自定义异常类型
来源：http://ml.panjiajie.cn

Py:   class MyError(Exception): pass
来源：http://jz.hnjuh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ll.szsharing.cn

JS:   class MyError extends Error {}
来源：http://et.yuntaijiaju.cn

TS:   class MyError extends Error {}
来源：http://qp.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://ta.huixiangedu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rl.wgjwhj.cn

Ruby: class MyError < StandardError; end
来源：http://il.huixinmuqiang.cn

C#:   class MyException : Exception {}
来源：http://ds.nicolike.cn

[H05] 捕获特定类型
来源：http://ud.szsharing.cn

Py:   except ValueError as e:
来源：http://gu.nszjky.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pv.521024.cn

JS:   if (e instanceof TypeError) {}
来源：http://ro.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://th.haigaiapp.cn

Java: catch (IOException | SQLException e) {}
来源：http://bt.bjjhwx.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wm.szxytkj.cn

Ruby: rescue ArgumentError => e
来源：http://ti.lnxyls.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oj.szsharing.cn

[H06] 可选值 / 空值安全访问
来源：http://gj.huixiangedu.cn

Py:   value = d.get("k") or default
来源：http://la.jianghongdianzi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://yc.panjiajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://zm.haigaiapp.cn

TS:   obj?.a?.b;  d ?? default
来源：http://oj.521024.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://dr.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bo.jctech888.com.cn

Ruby: d&.dig(:a, :b)
来源：http://ok.chemitech.net.cn

C#:   obj?.A?.B ?? default
来源：http://cp.wgjwhj.cn

[H07] 断言
来源：http://ow.jianghongdianzi.cn

Py:   assert x > 0, "必须为正"
来源：http://en.9csxet.cn

PHP:  assert($x > 0);
来源：http://iy.newstarts.cn

JS:   console.assert(x > 0);
来源：http://vh.huixinmuqiang.cn

TS:   console.assert(x > 0);
来源：http://ue.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://nr.hahajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://eu.wgjwhj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kz.gzmigu.cn

C#:   Debug.Assert(x > 0);
来源：http://yt.szsharing.cn

[H08] 获取错误信息与堆栈
来源：http://ql.haigaiapp.cn

Py:   str(e);  traceback.format_exc()
来源：http://wq.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://db.521024.cn

JS:   e.message;  e.stack
来源：http://op.nszjky.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wr.shtwfgs.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qs.hnjuh.cn

Go:   err.Error()
来源：http://oc.colortex.cn

Ruby: e.message;  e.backtrace
来源：http://lq.panjiajie.cn

C#:   e.Message;  e.StackTrace
来源：http://ps.shtwfgs.cn

[H09] 带错误码的异常
来源：http://hm.lnxyls.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://td.chemitech.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://uk.bookmarksfly.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://uj.yuexingan06.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wu.nicolike.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://oy.nicolike.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gm.haigaiapp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://xi.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://li.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://vf.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://gj.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://lr.gzmigu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mg.szxytkj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://eq.9csxet.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zh.huixiangedu.cn

Go:   defer f.Close()
来源：http://im.huixinmuqiang.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hc.shxzukj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://gl.asd995.cn

================================================================================
来源：http://od.bjjhwx.cn

I. 正则表达式
来源：http://ky.panjiajie.cn

================================================================================
来源：http://lq.asd995.cn

[I01] 判断是否匹配
来源：http://yu.newstarts.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yx.huanxung.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xn.szsharing.cn

JS:   /\d+/.test(s)
来源：http://gi.521024.cn

TS:   /\d+/.test(s)
来源：http://to.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yu.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://zt.haigaiapp.cn

Ruby: s.match?(/\d+/)
来源：http://ia.huixinmuqiang.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://pb.huixiangedu.cn

[I02] 提取所有匹配
来源：http://ou.nicolike.cn

Py:   re.findall(r"\d+", s)
来源：http://xr.nicolike.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lk.bjjhwx.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://uo.colortex.cn

TS:   s.match(/\d+/g)
来源：http://el.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hahajie.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://nd.bookmarksfly.cn

Ruby: s.scan(/\d+/)
来源：http://rr.nszjky.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ww.wgjwhj.cn

[I03] 提取捕获分组
来源：http://up.9csxet.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sa.szxytkj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://xc.521024.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nr.hahajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ae.huixiangedu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://el.yuntaijiaju.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://dh.haigaiapp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://tt.newstarts.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://rl.huixinmuqiang.cn

[I04] 正则替换
来源：http://wd.shxzukj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://lj.shtwfgs.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fp.yuntaijiaju.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gm.gzmigu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zk.gzmigu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ww.huixinmuqiang.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://hg.asd995.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://jy.wgjwhj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://wm.yuexingan06.cn

[I05] 按正则拆分
来源：http://gp.shtwfgs.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ns.szsharing.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vn.nszjky.cn

JS:   s.split(/\s*,\s*/)
来源：http://gw.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://xp.huixiangedu.cn

Java: s.split("\\s*,\\s*")
来源：http://ht.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sm.hnjuh.cn

Ruby: s.split(/\s*,\s*/)
来源：http://co.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hf.shxzukj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jb.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ho.yuexingan06.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://eu.huanxung.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gb.szxytkj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://yo.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ss.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ou.muxihuayi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xt.9csxet.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zc.newstarts.cn

[I07] 忽略大小写与多行模式
来源：http://fz.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://zd.gzmigu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://kr.haigaiapp.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://wq.haigaiapp.cn

TS:   /error/gim
来源：http://zp.muxihuayi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wu.521024.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ex.9csxet.cn

Ruby: s.scan(/error/i)
来源：http://er.yuntaijiaju.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://em.gzmigu.cn

[I08] 贪婪与非贪婪匹配
来源：http://bz.huanxung.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://tn.huixiangedu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bi.9csxet.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://dq.huanxung.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vz.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yj.szsharing.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zw.shxzukj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ui.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://jd.szxytkj.cn

================================================================================
来源：http://uw.hnjuh.cn

J. 日期与时间
来源：http://fr.szxytkj.cn

================================================================================
来源：http://vp.muxihuayi.cn

[J01] 获取当前时间
来源：http://qv.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://yn.wgjwhj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dl.521024.cn

JS:   new Date();  Date.now()
来源：http://nn.nicolike.cn

TS:   new Date();  Date.now()
来源：http://gz.jianghongdianzi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://op.nicolike.cn

Go:   time.Now()
来源：http://gi.9csxet.cn

Ruby: Time.now
来源：http://hi.huanxung.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ez.wgjwhj.cn

[J02] 格式化输出
来源：http://dw.hahajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lj.asd995.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://dk.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://jp.bjjhwx.cn

TS:   d.toISOString()
来源：http://ak.huanxung.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gi.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://nl.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mw.shxzukj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bg.hahajie.cn

[J03] 字符串解析为日期
来源：http://xt.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://eh.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ce.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://sq.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://zu.shtwfgs.cn

Java: LocalDate.parse("2024-01-02")
来源：http://tq.haigaiapp.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qx.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://ca.bjjhwx.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://si.jianghongdianzi.cn

[J04] 时间戳与日期互转
来源：http://xz.shxzskj.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://wt.shtwfgs.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sd.shxzskj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wg.szsharing.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ou.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sq.haigaiapp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://bk.bookmarksfly.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ho.yuexingan06.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pi.jctech888.com.cn

[J05] 时间加减（加 7 天）
来源：http://gw.jctech888.com.cn

Py:   now + timedelta(days=7)
来源：http://wr.jctech888.com.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://yj.hahajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xy.hnjuh.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wj.yuexingan06.cn

Java: LocalDate.now().plusDays(7)
来源：http://mo.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://na.nicolike.cn

Ruby: Time.now + 7 * 86400
来源：http://fh.shxzskj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://al.wgjwhj.cn

[J06] 计算两时间之差
来源：http://mu.nicolike.cn

Py:   (end - start).total_seconds()
来源：http://wq.gzmigu.cn

PHP:  $end->diff($start)->days;
来源：http://sd.huixinmuqiang.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nl.bookmarksfly.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://em.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://sg.wgjwhj.cn

Go:   end.Sub(start).Hours()
来源：http://bv.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://dq.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://va.huixiangedu.cn

[J07] 比较两个日期
来源：http://yp.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://kp.jctech888.com.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hr.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://cq.hnjuh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://za.bookmarksfly.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://wk.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dt.9csxet.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jv.521024.cn

C#:   d1 < d2;  d1 == d2
来源：http://tz.szsharing.cn

[J08] 提取年月日与星期
来源：http://df.wgjwhj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ey.hnjuh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mn.shxzukj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wx.jctech888.com.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wh.lnxyls.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ns.nszjky.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://us.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fq.newstarts.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ue.asd995.cn

[J09] 时区处理
来源：http://hh.haigaiapp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ec.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fx.bookmarksfly.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wj.jctech888.com.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vh.hahajie.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mh.huixiangedu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://aa.huixiangedu.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://qs.chemitech.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yc.haigaiapp.cn

[J10] 取今天 / 本月第一天
来源：http://xq.wgjwhj.cn


<!-- 参考信息 -->