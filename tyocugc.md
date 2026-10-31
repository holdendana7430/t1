代发 wailian999

Ruby: attr_accessor :name
来源：http://uz.jctech888.com.cn

C#:   public string Name { get; set; }
来源：http://dr.521024.cn

[G12] 对象转字符串
来源：http://jx.haigaiapp.cn

Py:   def __str__(self): return self.name
来源：http://uh.szsharing.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://oz.colortex.cn

JS:   toString() { return this.name; }
来源：http://jc.newstarts.cn

TS:   toString(): string { return this.name; }
来源：http://va.hnjuh.cn

Java: @Override public String toString() { return name; }
来源：http://wz.jianghongdianzi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://la.shxzukj.cn

Ruby: def to_s; @name; end
来源：http://lp.huixinmuqiang.cn

C#:   public override string ToString() => Name;
来源：http://fg.nszjky.cn

[G13] 判断对象类型
来源：http://tf.newstarts.cn

Py:   isinstance(u, User)
来源：http://rx.chemitech.net.cn

PHP:  $u instanceof User
来源：http://pr.9csxet.cn

JS:   u instanceof User
来源：http://ym.shtwfgs.cn

TS:   u instanceof User
来源：http://pu.hahajie.cn

Java: u instanceof User
来源：http://lu.asd995.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jg.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://vf.szxytkj.cn

C#:   u is User
来源：http://vj.bookmarksfly.cn

[G14] 数据类 / record
来源：http://qk.9csxet.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ia.colortex.cn

PHP:  // 用 readonly 属性模拟
来源：http://uo.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://oz.asd995.cn

TS:   type User = { name: string; age: number };
来源：http://vo.huanxung.cn

Java: record User(String name, int age) {}
来源：http://hq.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://fj.bookmarksfly.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sv.huixinmuqiang.cn

C#:   record User(string Name, int Age);
来源：http://sk.9csxet.cn

[G15] 枚举
来源：http://bx.asd995.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gc.521024.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hx.shtwfgs.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jg.bjjhwx.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://if.gzmigu.cn

Java: enum Color { RED, GREEN }
来源：http://mm.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tt.gzmigu.cn

Ruby: Color = %i[red green].freeze
来源：http://vx.yuntaijiaju.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ob.newstarts.cn

[G16] 对象转数组 / 字典
来源：http://ga.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qg.gzmigu.cn

PHP:  get_object_vars($obj);
来源：http://xe.panjiajie.cn

JS:   Object.entries(obj)
来源：http://kq.hnjuh.cn

TS:   Object.entries(obj)
来源：http://cm.huixinmuqiang.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ow.szsharing.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ka.bookmarksfly.cn

Ruby: obj.instance_variables
来源：http://ke.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://gb.gzmigu.cn

================================================================================
来源：http://pk.szxytkj.cn

H. 异常与错误处理
来源：http://fq.nicolike.cn

================================================================================
来源：http://yb.huanxung.cn

[H01] try / catch 基础
来源：http://zy.panjiajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jk.colortex.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://xb.asd995.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xc.huixiangedu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uo.huixiangedu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ma.szsharing.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://oj.szsharing.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jm.szsharing.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://au.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://am.lnxyls.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bj.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ig.yuexingan06.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ws.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://re.shxzukj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://cv.jctech888.com.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qg.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kr.nicolike.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pg.shtwfgs.cn

[H03] 主动抛出异常
来源：http://ob.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://ln.jctech888.com.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kk.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://bo.bjjhwx.cn

TS:   throw new Error("错误信息");
来源：http://rg.nszjky.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://em.521024.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fo.szxytkj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://sv.huanxung.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gn.gzmigu.cn

[H04] 自定义异常类型
来源：http://bm.hahajie.cn

Py:   class MyError(Exception): pass
来源：http://en.yuexingan06.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gh.szsharing.cn

JS:   class MyError extends Error {}
来源：http://hk.szsharing.cn

TS:   class MyError extends Error {}
来源：http://fa.huanxung.cn

Java: class MyException extends RuntimeException {}
来源：http://rr.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zy.nszjky.cn

Ruby: class MyError < StandardError; end
来源：http://jr.bjjhwx.cn

C#:   class MyException : Exception {}
来源：http://bd.yuntaijiaju.cn

[H05] 捕获特定类型
来源：http://lz.bjjhwx.cn

Py:   except ValueError as e:
来源：http://pj.huanxung.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://kr.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://gh.newstarts.cn

TS:   if (e instanceof TypeError) {}
来源：http://lw.haigaiapp.cn

Java: catch (IOException | SQLException e) {}
来源：http://yi.szsharing.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://lq.muxihuayi.cn

Ruby: rescue ArgumentError => e
来源：http://ut.521024.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://vl.bookmarksfly.cn

[H06] 可选值 / 空值安全访问
来源：http://lb.wgjwhj.cn

Py:   value = d.get("k") or default
来源：http://xp.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://tu.wgjwhj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://rf.bjjhwx.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ja.yuexingan06.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ae.lnxyls.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://mv.bjjhwx.cn

Ruby: d&.dig(:a, :b)
来源：http://xc.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://jn.szsharing.cn

[H07] 断言
来源：http://yu.nicolike.cn

Py:   assert x > 0, "必须为正"
来源：http://dd.jianghongdianzi.cn

PHP:  assert($x > 0);
来源：http://ip.lnxyls.cn

JS:   console.assert(x > 0);
来源：http://iw.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://ie.yuntaijiaju.cn

Java: assert x > 0 : "必须为正";
来源：http://lt.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lg.huanxung.cn

Ruby: raise "必须为正" unless x > 0
来源：http://kq.shxzskj.cn

C#:   Debug.Assert(x > 0);
来源：http://ox.hahajie.cn

[H08] 获取错误信息与堆栈
来源：http://pp.shxzukj.cn

Py:   str(e);  traceback.format_exc()
来源：http://gd.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://sy.szsharing.cn

JS:   e.message;  e.stack
来源：http://az.asd995.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pr.gzmigu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://uk.chemitech.net.cn

Go:   err.Error()
来源：http://bt.521024.cn

Ruby: e.message;  e.backtrace
来源：http://pa.gzmigu.cn

C#:   e.Message;  e.StackTrace
来源：http://ky.muxihuayi.cn

[H09] 带错误码的异常
来源：http://yx.huixiangedu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ok.nicolike.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gb.huixiangedu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nb.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ve.jianghongdianzi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://us.nicolike.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://gp.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ke.szsharing.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://bf.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://jp.shtwfgs.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://cj.newstarts.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://gd.hnjuh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ax.panjiajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gw.haigaiapp.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pi.colortex.cn

Go:   defer f.Close()
来源：http://td.chemitech.net.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://so.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://oh.bookmarksfly.cn

================================================================================
来源：http://uu.haigaiapp.cn

I. 正则表达式
来源：http://hb.nszjky.cn

================================================================================
来源：http://hz.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://lt.huixiangedu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://jp.haigaiapp.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gl.521024.cn

JS:   /\d+/.test(s)
来源：http://fp.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://qu.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://vs.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yb.jctech888.com.cn

Ruby: s.match?(/\d+/)
来源：http://xu.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ss.asd995.cn

[I02] 提取所有匹配
来源：http://mn.lnxyls.cn

Py:   re.findall(r"\d+", s)
来源：http://ls.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dz.huixiangedu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fb.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://mk.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fc.nszjky.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lw.szxytkj.cn

Ruby: s.scan(/\d+/)
来源：http://gc.asd995.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://to.colortex.cn

[I03] 提取捕获分组
来源：http://wf.yuexingan06.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rp.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://uk.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jc.colortex.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sf.lnxyls.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://dk.bjjhwx.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://cc.nicolike.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qn.haigaiapp.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sx.huanxung.cn

[I04] 正则替换
来源：http://kn.nicolike.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fs.jianghongdianzi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://th.hnjuh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fu.bookmarksfly.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ur.hnjuh.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cl.szsharing.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qj.yuexingan06.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ky.bookmarksfly.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://id.yuexingan06.cn

[I05] 按正则拆分
来源：http://sh.panjiajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://li.jianghongdianzi.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jg.szsharing.cn

JS:   s.split(/\s*,\s*/)
来源：http://qf.jctech888.com.cn

TS:   s.split(/\s*,\s*/)
来源：http://bs.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://zs.wgjwhj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sd.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://lu.bjjhwx.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bo.szsharing.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ej.jctech888.com.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cd.asd995.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://et.hnjuh.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wy.hnjuh.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oq.newstarts.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://ae.yuexingan06.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://te.chemitech.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lg.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://oj.colortex.cn

[I07] 忽略大小写与多行模式
来源：http://ya.newstarts.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://oh.nszjky.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://yb.nicolike.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vp.szxytkj.cn

TS:   /error/gim
来源：http://hr.nszjky.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ls.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hj.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://jr.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lz.521024.cn

[I08] 贪婪与非贪婪匹配
来源：http://zx.521024.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vv.shxzskj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wj.huixiangedu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://pj.9csxet.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xa.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zo.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ko.haigaiapp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ya.521024.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ml.gzmigu.cn

================================================================================
来源：http://zl.shxzukj.cn

J. 日期与时间
来源：http://vz.gzmigu.cn

================================================================================
来源：http://mo.huixiangedu.cn

[J01] 获取当前时间
来源：http://xh.shtwfgs.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ei.hahajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://zo.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://nu.shtwfgs.cn

TS:   new Date();  Date.now()
来源：http://zx.gzmigu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://wd.jianghongdianzi.cn

Go:   time.Now()
来源：http://ym.bjjhwx.cn

Ruby: Time.now
来源：http://rz.521024.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ao.huixinmuqiang.cn

[J02] 格式化输出
来源：http://mj.wgjwhj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ql.bjjhwx.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://os.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://od.hnjuh.cn

TS:   d.toISOString()
来源：http://bs.szsharing.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://kn.shxzskj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xl.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://dy.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sy.nszjky.cn

[J03] 字符串解析为日期
来源：http://ia.muxihuayi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hs.hnjuh.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://bu.hnjuh.cn

JS:   new Date("2024-01-02")
来源：http://ig.nszjky.cn

TS:   new Date("2024-01-02")
来源：http://zf.jianghongdianzi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://er.shxzukj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://po.huixiangedu.cn

Ruby: Date.parse("2024-01-02")
来源：http://ql.shxzukj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lc.shtwfgs.cn

[J04] 时间戳与日期互转
来源：http://rc.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://kf.huixiangedu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vb.newstarts.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zd.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://id.asd995.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zl.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://iq.shxzukj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://iz.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://xd.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://rt.gzmigu.cn

Py:   now + timedelta(days=7)
来源：http://ms.shtwfgs.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ex.hahajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wt.9csxet.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hh.nszjky.cn

Java: LocalDate.now().plusDays(7)
来源：http://lb.wgjwhj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zd.panjiajie.cn

Ruby: Time.now + 7 * 86400
来源：http://ce.newstarts.cn

C#:   DateTime.Now.AddDays(7)
来源：http://lz.yuntaijiaju.cn

[J06] 计算两时间之差
来源：http://wq.colortex.cn

Py:   (end - start).total_seconds()
来源：http://xf.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://di.szxytkj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nn.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://zn.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qh.asd995.cn

Go:   end.Sub(start).Hours()
来源：http://ix.shxzskj.cn

Ruby: end - start                 # 返回秒数
来源：http://fa.huixinmuqiang.cn

C#:   (end - start).TotalSeconds
来源：http://wq.huanxung.cn

[J07] 比较两个日期
来源：http://jz.asd995.cn

Py:   d1 < d2;  d1 == d2
来源：http://fz.521024.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mj.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pz.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zy.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://vy.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lu.jianghongdianzi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gs.szsharing.cn

C#:   d1 < d2;  d1 == d2
来源：http://dj.gzmigu.cn

[J08] 提取年月日与星期
来源：http://kv.yuntaijiaju.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mm.bookmarksfly.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mw.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://je.shxzukj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xi.nicolike.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yz.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ry.shxzskj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mj.shxzukj.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fl.jctech888.com.cn

[J09] 时区处理
来源：http://dd.huanxung.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://bq.hnjuh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sb.521024.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jk.nicolike.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ot.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gs.gzmigu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qa.szsharing.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kq.bjjhwx.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pv.bookmarksfly.cn

[J10] 取今天 / 本月第一天
来源：http://qh.haigaiapp.cn


<!-- 参考信息 -->