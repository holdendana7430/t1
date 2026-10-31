代发 wailian999

Ruby: attr_accessor :name
来源：http://xs.nicolike.cn

C#:   public string Name { get; set; }
来源：http://ef.chemitech.net.cn

[G12] 对象转字符串
来源：http://zz.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://vj.huixinmuqiang.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://lt.asd995.cn

JS:   toString() { return this.name; }
来源：http://qf.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://xo.shxzskj.cn

Java: @Override public String toString() { return name; }
来源：http://oc.muxihuayi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xq.jctech888.com.cn

Ruby: def to_s; @name; end
来源：http://td.gzmigu.cn

C#:   public override string ToString() => Name;
来源：http://wc.shtwfgs.cn

[G13] 判断对象类型
来源：http://ki.bjjhwx.cn

Py:   isinstance(u, User)
来源：http://in.jianghongdianzi.cn

PHP:  $u instanceof User
来源：http://xr.huixiangedu.cn

JS:   u instanceof User
来源：http://hv.muxihuayi.cn

TS:   u instanceof User
来源：http://cz.yuexingan06.cn

Java: u instanceof User
来源：http://pa.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wh.lnxyls.cn

Ruby: u.is_a?(User)
来源：http://yv.nszjky.cn

C#:   u is User
来源：http://db.szxytkj.cn

[G14] 数据类 / record
来源：http://zl.asd995.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://dp.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://qx.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://th.lnxyls.cn

TS:   type User = { name: string; age: number };
来源：http://rn.muxihuayi.cn

Java: record User(String name, int age) {}
来源：http://uc.yuexingan06.cn

Go:   type User struct { Name string; Age int }
来源：http://vl.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jo.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://pd.huixiangedu.cn

[G15] 枚举
来源：http://og.muxihuayi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ec.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ln.bookmarksfly.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jg.szxytkj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gu.hahajie.cn

Java: enum Color { RED, GREEN }
来源：http://vz.huanxung.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://zw.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://vt.hnjuh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qw.jctech888.com.cn

[G16] 对象转数组 / 字典
来源：http://lk.chemitech.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bp.hnjuh.cn

PHP:  get_object_vars($obj);
来源：http://wj.hnjuh.cn

JS:   Object.entries(obj)
来源：http://aj.lnxyls.cn

TS:   Object.entries(obj)
来源：http://ap.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yu.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ut.shxzukj.cn

Ruby: obj.instance_variables
来源：http://tr.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://yn.chemitech.net.cn

================================================================================
来源：http://su.yuntaijiaju.cn

H. 异常与错误处理
来源：http://ob.panjiajie.cn

================================================================================
来源：http://pz.wgjwhj.cn

[H01] try / catch 基础
来源：http://jy.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zk.nszjky.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wy.wgjwhj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xe.bjjhwx.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://dj.9csxet.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://st.haigaiapp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wv.colortex.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ar.szsharing.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cx.yuexingan06.cn

[H02] finally / ensure 收尾
来源：http://jq.bookmarksfly.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ui.gzmigu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fd.521024.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mk.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://en.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://uw.521024.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://gw.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ov.colortex.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pv.szsharing.cn

[H03] 主动抛出异常
来源：http://nu.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://iy.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://tv.shtwfgs.cn

JS:   throw new Error("错误信息");
来源：http://ar.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://fk.huixiangedu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lo.nszjky.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ll.hnjuh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nl.newstarts.cn

C#:   throw new ArgumentException("错误信息");
来源：http://az.nicolike.cn

[H04] 自定义异常类型
来源：http://yo.newstarts.cn

Py:   class MyError(Exception): pass
来源：http://ix.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yg.huixinmuqiang.cn

JS:   class MyError extends Error {}
来源：http://sq.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://lc.jctech888.com.cn

Java: class MyException extends RuntimeException {}
来源：http://yp.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vm.521024.cn

Ruby: class MyError < StandardError; end
来源：http://om.bookmarksfly.cn

C#:   class MyException : Exception {}
来源：http://hn.newstarts.cn

[H05] 捕获特定类型
来源：http://lu.yuexingan06.cn

Py:   except ValueError as e:
来源：http://qf.jctech888.com.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xa.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://cf.haigaiapp.cn

TS:   if (e instanceof TypeError) {}
来源：http://mt.nicolike.cn

Java: catch (IOException | SQLException e) {}
来源：http://jq.haigaiapp.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://be.lnxyls.cn

Ruby: rescue ArgumentError => e
来源：http://ia.muxihuayi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jx.yuexingan06.cn

[H06] 可选值 / 空值安全访问
来源：http://nr.wgjwhj.cn

Py:   value = d.get("k") or default
来源：http://uw.panjiajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ha.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hv.nicolike.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fx.chemitech.net.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pu.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cu.hnjuh.cn

Ruby: d&.dig(:a, :b)
来源：http://fy.colortex.cn

C#:   obj?.A?.B ?? default
来源：http://nq.yuntaijiaju.cn

[H07] 断言
来源：http://ul.9csxet.cn

Py:   assert x > 0, "必须为正"
来源：http://mw.wgjwhj.cn

PHP:  assert($x > 0);
来源：http://cn.muxihuayi.cn

JS:   console.assert(x > 0);
来源：http://zf.colortex.cn

TS:   console.assert(x > 0);
来源：http://kz.huixiangedu.cn

Java: assert x > 0 : "必须为正";
来源：http://te.asd995.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wk.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://lm.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://bl.nicolike.cn

[H08] 获取错误信息与堆栈
来源：http://fx.shxzukj.cn

Py:   str(e);  traceback.format_exc()
来源：http://sp.szxytkj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ns.muxihuayi.cn

JS:   e.message;  e.stack
来源：http://cq.jianghongdianzi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ud.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://wt.hahajie.cn

Go:   err.Error()
来源：http://nh.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://eo.yuntaijiaju.cn

C#:   e.Message;  e.StackTrace
来源：http://sc.jctech888.com.cn

[H09] 带错误码的异常
来源：http://tp.haigaiapp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://px.shtwfgs.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kk.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ja.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wy.bookmarksfly.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://do.szsharing.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bo.yuexingan06.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ik.bjjhwx.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uq.huixiangedu.cn

[H10] 资源自动释放
来源：http://ak.shxzskj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://up.huanxung.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xl.yuexingan06.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://pa.jianghongdianzi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ci.chemitech.net.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mn.nicolike.cn

Go:   defer f.Close()
来源：http://hx.yuntaijiaju.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://it.newstarts.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://bn.9csxet.cn

================================================================================
来源：http://kj.panjiajie.cn

I. 正则表达式
来源：http://th.asd995.cn

================================================================================
来源：http://co.wgjwhj.cn

[I01] 判断是否匹配
来源：http://qr.jctech888.com.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hk.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://jn.nicolike.cn

JS:   /\d+/.test(s)
来源：http://qj.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://mn.521024.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://of.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ux.colortex.cn

Ruby: s.match?(/\d+/)
来源：http://pm.bookmarksfly.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://eg.521024.cn

[I02] 提取所有匹配
来源：http://yb.huixiangedu.cn

Py:   re.findall(r"\d+", s)
来源：http://xm.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://dr.jctech888.com.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://rv.haigaiapp.cn

TS:   s.match(/\d+/g)
来源：http://qg.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://nf.szxytkj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fs.gzmigu.cn

Ruby: s.scan(/\d+/)
来源：http://pj.huanxung.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nd.lnxyls.cn

[I03] 提取捕获分组
来源：http://lo.huixinmuqiang.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://si.yuntaijiaju.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://cu.colortex.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ap.huixinmuqiang.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://it.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vm.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://zc.huixiangedu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ha.yuexingan06.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jw.hnjuh.cn

[I04] 正则替换
来源：http://cs.bjjhwx.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sl.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ub.shxzskj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://kk.huixiangedu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://km.muxihuayi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://rq.yuexingan06.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tp.yuntaijiaju.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xz.szxytkj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fu.jctech888.com.cn

[I05] 按正则拆分
来源：http://eq.szsharing.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vt.yuntaijiaju.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ew.shtwfgs.cn

JS:   s.split(/\s*,\s*/)
来源：http://fb.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://qn.szsharing.cn

Java: s.split("\\s*,\\s*")
来源：http://pu.huixiangedu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ov.jianghongdianzi.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qc.haigaiapp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xd.szsharing.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://jz.bookmarksfly.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ls.asd995.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://dn.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nh.colortex.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pj.hahajie.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://pk.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://za.panjiajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gv.bookmarksfly.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gr.bookmarksfly.cn

[I07] 忽略大小写与多行模式
来源：http://al.nicolike.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://sq.jianghongdianzi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lt.huanxung.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ns.wgjwhj.cn

TS:   /error/gim
来源：http://th.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://xy.nszjky.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ea.chemitech.net.cn

Ruby: s.scan(/error/i)
来源：http://au.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wv.nszjky.cn

[I08] 贪婪与非贪婪匹配
来源：http://yr.szsharing.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bs.bookmarksfly.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zd.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xc.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://uq.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nb.bookmarksfly.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xc.szxytkj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bo.muxihuayi.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://lf.colortex.cn

================================================================================
来源：http://en.newstarts.cn

J. 日期与时间
来源：http://ft.szxytkj.cn

================================================================================
来源：http://oc.asd995.cn

[J01] 获取当前时间
来源：http://ui.haigaiapp.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ue.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gu.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://ks.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://to.muxihuayi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mr.yuntaijiaju.cn

Go:   time.Now()
来源：http://jz.huixinmuqiang.cn

Ruby: Time.now
来源：http://ji.jianghongdianzi.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gj.shxzskj.cn

[J02] 格式化输出
来源：http://dm.yuexingan06.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://qf.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yf.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://kr.huixinmuqiang.cn

TS:   d.toISOString()
来源：http://xx.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gv.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ub.huanxung.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rn.yuexingan06.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://aw.shxzskj.cn

[J03] 字符串解析为日期
来源：http://vm.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://df.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://cd.521024.cn

JS:   new Date("2024-01-02")
来源：http://xi.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://nw.muxihuayi.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ou.szxytkj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qu.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://up.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://zp.huixinmuqiang.cn

[J04] 时间戳与日期互转
来源：http://ne.yuexingan06.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://np.yuntaijiaju.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cr.szsharing.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://qq.jianghongdianzi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sq.haigaiapp.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ao.hnjuh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://rf.huanxung.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ng.wgjwhj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jo.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://gw.shxzukj.cn

Py:   now + timedelta(days=7)
来源：http://io.bookmarksfly.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://ld.hahajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dm.szsharing.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://pb.bjjhwx.cn

Java: LocalDate.now().plusDays(7)
来源：http://il.gzmigu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uf.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://dq.chemitech.net.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cx.colortex.cn

[J06] 计算两时间之差
来源：http://is.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://ff.jianghongdianzi.cn

PHP:  $end->diff($start)->days;
来源：http://hd.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://js.lnxyls.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://vx.shxzskj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vg.gzmigu.cn

Go:   end.Sub(start).Hours()
来源：http://br.shxzskj.cn

Ruby: end - start                 # 返回秒数
来源：http://hf.huanxung.cn

C#:   (end - start).TotalSeconds
来源：http://zx.lnxyls.cn

[J07] 比较两个日期
来源：http://nm.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://mi.hahajie.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tn.yuntaijiaju.cn

JS:   d1.getTime() < d2.getTime()
来源：http://am.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gc.chemitech.net.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://au.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://st.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://du.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://pa.huanxung.cn

[J08] 提取年月日与星期
来源：http://bh.bookmarksfly.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yx.shxzskj.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fu.szsharing.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cq.colortex.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hq.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://qn.nszjky.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nc.huixinmuqiang.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ek.yuntaijiaju.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vx.jctech888.com.cn

[J09] 时区处理
来源：http://nb.szsharing.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://du.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://us.shxzskj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xv.bjjhwx.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gh.9csxet.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://sn.yuntaijiaju.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mj.9csxet.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://js.9csxet.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://yp.gzmigu.cn

[J10] 取今天 / 本月第一天
来源：http://tm.hnjuh.cn


<!-- 参考信息 -->