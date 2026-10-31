代发 wailian999

Ruby: attr_accessor :name
来源：http://hl.wgjwhj.cn

C#:   public string Name { get; set; }
来源：http://dw.panjiajie.cn

[G12] 对象转字符串
来源：http://yn.szsharing.cn

Py:   def __str__(self): return self.name
来源：http://zl.hahajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dy.521024.cn

JS:   toString() { return this.name; }
来源：http://ib.chemitech.net.cn

TS:   toString(): string { return this.name; }
来源：http://cf.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://xq.wgjwhj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://to.chemitech.net.cn

Ruby: def to_s; @name; end
来源：http://nk.wgjwhj.cn

C#:   public override string ToString() => Name;
来源：http://qo.shxzukj.cn

[G13] 判断对象类型
来源：http://hy.shxzskj.cn

Py:   isinstance(u, User)
来源：http://th.9csxet.cn

PHP:  $u instanceof User
来源：http://qk.asd995.cn

JS:   u instanceof User
来源：http://tl.szsharing.cn

TS:   u instanceof User
来源：http://ze.huanxung.cn

Java: u instanceof User
来源：http://ho.521024.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xp.nszjky.cn

Ruby: u.is_a?(User)
来源：http://re.wgjwhj.cn

C#:   u is User
来源：http://on.muxihuayi.cn

[G14] 数据类 / record
来源：http://pk.muxihuayi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://jz.muxihuayi.cn

PHP:  // 用 readonly 属性模拟
来源：http://wd.huixiangedu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vp.shtwfgs.cn

TS:   type User = { name: string; age: number };
来源：http://oy.hahajie.cn

Java: record User(String name, int age) {}
来源：http://xe.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://dn.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ld.gzmigu.cn

C#:   record User(string Name, int Age);
来源：http://km.huixiangedu.cn

[G15] 枚举
来源：http://ep.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sw.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pa.hahajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ff.huixiangedu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hg.nszjky.cn

Java: enum Color { RED, GREEN }
来源：http://zd.szsharing.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yb.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://ut.nszjky.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://pc.shxzukj.cn

[G16] 对象转数组 / 字典
来源：http://nx.huixinmuqiang.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://og.huixinmuqiang.cn

PHP:  get_object_vars($obj);
来源：http://bq.shtwfgs.cn

JS:   Object.entries(obj)
来源：http://ww.asd995.cn

TS:   Object.entries(obj)
来源：http://ut.lnxyls.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://om.hnjuh.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://qt.yuexingan06.cn

Ruby: obj.instance_variables
来源：http://gk.9csxet.cn

C#:   // 用反射或 System.Text.Json
来源：http://di.panjiajie.cn

================================================================================
来源：http://on.huixinmuqiang.cn

H. 异常与错误处理
来源：http://wd.nszjky.cn

================================================================================
来源：http://oc.shxzukj.cn

[H01] try / catch 基础
来源：http://rz.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gc.chemitech.net.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kq.hahajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://st.muxihuayi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://md.colortex.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xj.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gn.jianghongdianzi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dv.nicolike.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://iu.huixinmuqiang.cn

[H02] finally / ensure 收尾
来源：http://mq.wgjwhj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://on.nicolike.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ps.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vt.gzmigu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://al.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://nb.panjiajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pa.nszjky.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ls.bookmarksfly.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ox.muxihuayi.cn

[H03] 主动抛出异常
来源：http://en.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://py.asd995.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://gq.muxihuayi.cn

JS:   throw new Error("错误信息");
来源：http://zb.hahajie.cn

TS:   throw new Error("错误信息");
来源：http://cz.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ad.yuntaijiaju.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ic.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://yy.asd995.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vt.muxihuayi.cn

[H04] 自定义异常类型
来源：http://pj.jctech888.com.cn

Py:   class MyError(Exception): pass
来源：http://re.yuntaijiaju.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ob.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://uk.bookmarksfly.cn

TS:   class MyError extends Error {}
来源：http://wt.bookmarksfly.cn

Java: class MyException extends RuntimeException {}
来源：http://og.nszjky.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nk.bookmarksfly.cn

Ruby: class MyError < StandardError; end
来源：http://md.huixinmuqiang.cn

C#:   class MyException : Exception {}
来源：http://wq.szsharing.cn

[H05] 捕获特定类型
来源：http://om.colortex.cn

Py:   except ValueError as e:
来源：http://xm.huixinmuqiang.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://vl.huixinmuqiang.cn

JS:   if (e instanceof TypeError) {}
来源：http://jf.yuexingan06.cn

TS:   if (e instanceof TypeError) {}
来源：http://ng.newstarts.cn

Java: catch (IOException | SQLException e) {}
来源：http://nw.jianghongdianzi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uh.gzmigu.cn

Ruby: rescue ArgumentError => e
来源：http://xg.huanxung.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://aj.newstarts.cn

[H06] 可选值 / 空值安全访问
来源：http://vy.lnxyls.cn

Py:   value = d.get("k") or default
来源：http://tl.newstarts.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ij.yuntaijiaju.cn

JS:   obj?.a?.b;  d ?? default
来源：http://au.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yk.521024.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cd.huixiangedu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ro.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://ym.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://fq.nicolike.cn

[H07] 断言
来源：http://xd.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://ko.chemitech.net.cn

PHP:  assert($x > 0);
来源：http://zl.szxytkj.cn

JS:   console.assert(x > 0);
来源：http://fj.nicolike.cn

TS:   console.assert(x > 0);
来源：http://qt.hnjuh.cn

Java: assert x > 0 : "必须为正";
来源：http://pq.lnxyls.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mv.huixiangedu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://na.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://al.nszjky.cn

[H08] 获取错误信息与堆栈
来源：http://qy.hahajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://dx.jctech888.com.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hv.nszjky.cn

JS:   e.message;  e.stack
来源：http://cc.colortex.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://eu.panjiajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://hf.bookmarksfly.cn

Go:   err.Error()
来源：http://xi.jianghongdianzi.cn

Ruby: e.message;  e.backtrace
来源：http://ma.shxzskj.cn

C#:   e.Message;  e.StackTrace
来源：http://gh.haigaiapp.cn

[H09] 带错误码的异常
来源：http://cq.panjiajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ad.lnxyls.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://lu.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://sd.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mh.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://km.lnxyls.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://cf.panjiajie.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lo.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://tq.wgjwhj.cn

[H10] 资源自动释放
来源：http://nk.szxytkj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hm.wgjwhj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wq.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wl.yuexingan06.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://pz.szsharing.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fb.lnxyls.cn

Go:   defer f.Close()
来源：http://jc.huixinmuqiang.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://sd.nicolike.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mt.nicolike.cn

================================================================================
来源：http://dk.hnjuh.cn

I. 正则表达式
来源：http://pr.shtwfgs.cn

================================================================================
来源：http://kt.asd995.cn

[I01] 判断是否匹配
来源：http://us.9csxet.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tj.yuexingan06.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ih.nicolike.cn

JS:   /\d+/.test(s)
来源：http://kp.asd995.cn

TS:   /\d+/.test(s)
来源：http://ay.huixinmuqiang.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qb.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://un.hnjuh.cn

Ruby: s.match?(/\d+/)
来源：http://kb.shtwfgs.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://sh.muxihuayi.cn

[I02] 提取所有匹配
来源：http://ad.bjjhwx.cn

Py:   re.findall(r"\d+", s)
来源：http://te.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nc.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://cb.huixinmuqiang.cn

TS:   s.match(/\d+/g)
来源：http://dj.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://kj.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ul.wgjwhj.cn

Ruby: s.scan(/\d+/)
来源：http://bq.9csxet.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://iq.9csxet.cn

[I03] 提取捕获分组
来源：http://fc.hahajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mv.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ar.asd995.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://uw.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uv.gzmigu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vc.huixinmuqiang.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vj.shxzskj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fe.yuntaijiaju.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gx.shxzskj.cn

[I04] 正则替换
来源：http://so.szxytkj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ff.szxytkj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://lq.bjjhwx.cn

JS:   s.replace(/\d+/g, "#")
来源：http://jh.panjiajie.cn

TS:   s.replace(/\d+/g, "#")
来源：http://rh.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://es.gzmigu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://am.jctech888.com.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cd.hnjuh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://sd.szsharing.cn

[I05] 按正则拆分
来源：http://vk.panjiajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yi.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ho.yuntaijiaju.cn

JS:   s.split(/\s*,\s*/)
来源：http://sn.szsharing.cn

TS:   s.split(/\s*,\s*/)
来源：http://io.yuntaijiaju.cn

Java: s.split("\\s*,\\s*")
来源：http://zx.gzmigu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://li.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://js.lnxyls.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://do.muxihuayi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://go.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fx.huixinmuqiang.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gu.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gp.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://po.shtwfgs.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://il.yuexingan06.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rp.huixiangedu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://uk.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gn.shxzukj.cn

[I07] 忽略大小写与多行模式
来源：http://kf.bookmarksfly.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qj.hnjuh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vo.wgjwhj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qt.huixiangedu.cn

TS:   /error/gim
来源：http://tq.yuntaijiaju.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rt.szsharing.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://uv.colortex.cn

Ruby: s.scan(/error/i)
来源：http://ge.colortex.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://my.gzmigu.cn

[I08] 贪婪与非贪婪匹配
来源：http://vo.nszjky.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://gv.yuntaijiaju.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mi.muxihuayi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://me.gzmigu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://nh.521024.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ew.haigaiapp.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kd.newstarts.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jk.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uf.jctech888.com.cn

================================================================================
来源：http://ru.shxzskj.cn

J. 日期与时间
来源：http://bz.muxihuayi.cn

================================================================================
来源：http://hj.yuexingan06.cn

[J01] 获取当前时间
来源：http://ye.huanxung.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hl.yuexingan06.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://td.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://nn.huixiangedu.cn

TS:   new Date();  Date.now()
来源：http://hb.wgjwhj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fk.yuexingan06.cn

Go:   time.Now()
来源：http://hn.asd995.cn

Ruby: Time.now
来源：http://ew.newstarts.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://tp.gzmigu.cn

[J02] 格式化输出
来源：http://nd.yuexingan06.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cn.bookmarksfly.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ib.lnxyls.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://su.szxytkj.cn

TS:   d.toISOString()
来源：http://gw.huixiangedu.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ld.lnxyls.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jc.jctech888.com.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uz.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://no.panjiajie.cn

[J03] 字符串解析为日期
来源：http://lb.panjiajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fg.panjiajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cv.nicolike.cn

JS:   new Date("2024-01-02")
来源：http://bw.asd995.cn

TS:   new Date("2024-01-02")
来源：http://he.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://pd.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ls.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://mi.9csxet.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ij.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://qg.hahajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://rx.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://zg.szsharing.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://su.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tp.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mb.huixiangedu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mk.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ue.nicolike.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ny.muxihuayi.cn

[J05] 时间加减（加 7 天）
来源：http://tr.yuntaijiaju.cn

Py:   now + timedelta(days=7)
来源：http://zo.yuntaijiaju.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://oe.yuntaijiaju.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gd.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gs.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://db.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://br.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://gz.shtwfgs.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ne.shxzukj.cn

[J06] 计算两时间之差
来源：http://aa.wgjwhj.cn

Py:   (end - start).total_seconds()
来源：http://uy.panjiajie.cn

PHP:  $end->diff($start)->days;
来源：http://va.wgjwhj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wi.huixiangedu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://aa.szxytkj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://cj.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://vq.shtwfgs.cn

Ruby: end - start                 # 返回秒数
来源：http://oc.huanxung.cn

C#:   (end - start).TotalSeconds
来源：http://xi.jctech888.com.cn

[J07] 比较两个日期
来源：http://os.szxytkj.cn

Py:   d1 < d2;  d1 == d2
来源：http://xj.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ep.jianghongdianzi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nh.bjjhwx.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xs.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mb.muxihuayi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kh.yuntaijiaju.cn

Ruby: d1 < d2;  d1 == d2
来源：http://gi.lnxyls.cn

C#:   d1 < d2;  d1 == d2
来源：http://ho.gzmigu.cn

[J08] 提取年月日与星期
来源：http://at.colortex.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tv.chemitech.net.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://nu.shtwfgs.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fl.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pd.nicolike.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pk.bookmarksfly.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://pc.nicolike.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://gw.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://gk.9csxet.cn

[J09] 时区处理
来源：http://pz.9csxet.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://re.nszjky.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uh.huanxung.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://im.muxihuayi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cw.szxytkj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ct.huanxung.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://co.colortex.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://fs.colortex.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gs.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://ct.shtwfgs.cn


<!-- 参考信息 -->