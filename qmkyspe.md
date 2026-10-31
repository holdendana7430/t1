代发 wailian999

JS:   get name() { return this._name; }
来源：http://im.9csxet.cn

TS:   get name(): string { return this._name; }
来源：http://dv.nicolike.cn

Java: public String getName() { return name; }
来源：http://xs.colortex.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://by.jianghongdianzi.cn

Ruby: attr_accessor :name
来源：http://uz.nicolike.cn

C#:   public string Name { get; set; }
来源：http://hs.gzmigu.cn

[G12] 对象转字符串
来源：http://ns.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://bx.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jf.lnxyls.cn

JS:   toString() { return this.name; }
来源：http://ho.chemitech.net.cn

TS:   toString(): string { return this.name; }
来源：http://by.hnjuh.cn

Java: @Override public String toString() { return name; }
来源：http://gb.hahajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zy.newstarts.cn

Ruby: def to_s; @name; end
来源：http://vq.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://zr.haigaiapp.cn

[G13] 判断对象类型
来源：http://cq.wgjwhj.cn

Py:   isinstance(u, User)
来源：http://mi.muxihuayi.cn

PHP:  $u instanceof User
来源：http://od.yuexingan06.cn

JS:   u instanceof User
来源：http://wz.yuntaijiaju.cn

TS:   u instanceof User
来源：http://lp.hahajie.cn

Java: u instanceof User
来源：http://pw.szxytkj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kp.nicolike.cn

Ruby: u.is_a?(User)
来源：http://om.muxihuayi.cn

C#:   u is User
来源：http://gq.colortex.cn

[G14] 数据类 / record
来源：http://al.shtwfgs.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gl.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://gj.szsharing.cn

JS:   // 无内置：普通类或对象字面量
来源：http://fq.gzmigu.cn

TS:   type User = { name: string; age: number };
来源：http://yo.521024.cn

Java: record User(String name, int age) {}
来源：http://to.haigaiapp.cn

Go:   type User struct { Name string; Age int }
来源：http://tt.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vn.jctech888.com.cn

C#:   record User(string Name, int Age);
来源：http://qt.haigaiapp.cn

[G15] 枚举
来源：http://tb.hnjuh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qb.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://nq.newstarts.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qf.gzmigu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mi.lnxyls.cn

Java: enum Color { RED, GREEN }
来源：http://ni.521024.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ru.huanxung.cn

Ruby: Color = %i[red green].freeze
来源：http://yp.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yb.hahajie.cn

[G16] 对象转数组 / 字典
来源：http://cy.asd995.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pv.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://mx.asd995.cn

JS:   Object.entries(obj)
来源：http://ez.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://ju.521024.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ys.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://il.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://bq.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://ib.panjiajie.cn

================================================================================
来源：http://oo.yuntaijiaju.cn

H. 异常与错误处理
来源：http://wp.bjjhwx.cn

================================================================================
来源：http://ox.huixinmuqiang.cn

[H01] try / catch 基础
来源：http://ny.shtwfgs.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ax.szxytkj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ec.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://fv.huanxung.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lr.huanxung.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://nl.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ov.huanxung.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ru.wgjwhj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jh.panjiajie.cn

[H02] finally / ensure 收尾
来源：http://ux.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wx.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pl.huanxung.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yb.gzmigu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://uf.chemitech.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://dq.521024.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://hb.gzmigu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://dn.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://xe.szxytkj.cn

[H03] 主动抛出异常
来源：http://yq.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://ho.521024.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xd.asd995.cn

JS:   throw new Error("错误信息");
来源：http://fm.shxzukj.cn

TS:   throw new Error("错误信息");
来源：http://ev.panjiajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yf.huixiangedu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hi.hnjuh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vi.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://kb.asd995.cn

[H04] 自定义异常类型
来源：http://jb.asd995.cn

Py:   class MyError(Exception): pass
来源：http://vs.9csxet.cn

PHP:  class MyError extends RuntimeException {}
来源：http://qk.huixiangedu.cn

JS:   class MyError extends Error {}
来源：http://ra.muxihuayi.cn

TS:   class MyError extends Error {}
来源：http://on.huanxung.cn

Java: class MyException extends RuntimeException {}
来源：http://ty.wgjwhj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://sh.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://fc.nicolike.cn

C#:   class MyException : Exception {}
来源：http://jy.hnjuh.cn

[H05] 捕获特定类型
来源：http://ax.nicolike.cn

Py:   except ValueError as e:
来源：http://bs.hahajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://zd.asd995.cn

JS:   if (e instanceof TypeError) {}
来源：http://vw.gzmigu.cn

TS:   if (e instanceof TypeError) {}
来源：http://da.huanxung.cn

Java: catch (IOException | SQLException e) {}
来源：http://be.9csxet.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://fu.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://vl.shxzskj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://nn.nicolike.cn

[H06] 可选值 / 空值安全访问
来源：http://of.asd995.cn

Py:   value = d.get("k") or default
来源：http://wp.jctech888.com.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ec.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xd.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zl.hahajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://kj.nszjky.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://rg.nszjky.cn

Ruby: d&.dig(:a, :b)
来源：http://tm.haigaiapp.cn

C#:   obj?.A?.B ?? default
来源：http://ty.chemitech.net.cn

[H07] 断言
来源：http://rz.haigaiapp.cn

Py:   assert x > 0, "必须为正"
来源：http://fu.hnjuh.cn

PHP:  assert($x > 0);
来源：http://mt.shxzukj.cn

JS:   console.assert(x > 0);
来源：http://pu.huanxung.cn

TS:   console.assert(x > 0);
来源：http://kq.newstarts.cn

Java: assert x > 0 : "必须为正";
来源：http://bv.yuntaijiaju.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://od.bookmarksfly.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ac.hahajie.cn

C#:   Debug.Assert(x > 0);
来源：http://ot.521024.cn

[H08] 获取错误信息与堆栈
来源：http://ea.wgjwhj.cn

Py:   str(e);  traceback.format_exc()
来源：http://dp.yuntaijiaju.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://py.huixinmuqiang.cn

JS:   e.message;  e.stack
来源：http://yy.9csxet.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://vo.521024.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://yk.shxzukj.cn

Go:   err.Error()
来源：http://lm.muxihuayi.cn

Ruby: e.message;  e.backtrace
来源：http://wp.szxytkj.cn

C#:   e.Message;  e.StackTrace
来源：http://wg.yuntaijiaju.cn

[H09] 带错误码的异常
来源：http://ja.gzmigu.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://uk.huanxung.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://yx.colortex.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://nl.huixinmuqiang.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zj.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rn.huanxung.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qm.lnxyls.cn

Ruby: raise MyError.new("fail", 500)
来源：http://sj.szsharing.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zf.shxzukj.cn

[H10] 资源自动释放
来源：http://lw.szxytkj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://tl.wgjwhj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hc.lnxyls.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nr.shtwfgs.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vl.shxzukj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sx.hahajie.cn

Go:   defer f.Close()
来源：http://aj.nicolike.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://zt.shxzukj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ny.shtwfgs.cn

================================================================================
来源：http://xw.newstarts.cn

I. 正则表达式
来源：http://gw.bookmarksfly.cn

================================================================================
来源：http://rx.wgjwhj.cn

[I01] 判断是否匹配
来源：http://xh.shxzskj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vg.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lb.yuexingan06.cn

JS:   /\d+/.test(s)
来源：http://ym.haigaiapp.cn

TS:   /\d+/.test(s)
来源：http://bh.shtwfgs.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lq.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fk.bjjhwx.cn

Ruby: s.match?(/\d+/)
来源：http://wn.lnxyls.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bf.huanxung.cn

[I02] 提取所有匹配
来源：http://aq.yuexingan06.cn

Py:   re.findall(r"\d+", s)
来源：http://kx.nicolike.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xq.bjjhwx.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hd.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://jr.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://fy.nszjky.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://qc.huixiangedu.cn

Ruby: s.scan(/\d+/)
来源：http://gb.huanxung.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gm.newstarts.cn

[I03] 提取捕获分组
来源：http://dp.huixiangedu.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ss.shxzukj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mj.9csxet.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gf.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kp.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mn.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://wp.shxzukj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hn.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ah.colortex.cn

[I04] 正则替换
来源：http://qf.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://kv.huixiangedu.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ux.bookmarksfly.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pw.haigaiapp.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xi.asd995.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hk.hnjuh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://li.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://do.bookmarksfly.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://vw.shtwfgs.cn

[I05] 按正则拆分
来源：http://dn.9csxet.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dk.hnjuh.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xn.hnjuh.cn

JS:   s.split(/\s*,\s*/)
来源：http://gi.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://kh.huixiangedu.cn

Java: s.split("\\s*,\\s*")
来源：http://eb.nszjky.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://oz.newstarts.cn

Ruby: s.split(/\s*,\s*/)
来源：http://be.nicolike.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://zk.asd995.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cv.bookmarksfly.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://al.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://qt.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gs.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oz.newstarts.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qs.szsharing.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://zc.yuexingan06.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fr.szsharing.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://wa.chemitech.net.cn

[I07] 忽略大小写与多行模式
来源：http://uq.yuntaijiaju.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://np.huanxung.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ks.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vn.lnxyls.cn

TS:   /error/gim
来源：http://ww.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dg.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gu.colortex.cn

Ruby: s.scan(/error/i)
来源：http://kv.newstarts.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://cw.muxihuayi.cn

[I08] 贪婪与非贪婪匹配
来源：http://ji.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lu.chemitech.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://as.newstarts.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://re.wgjwhj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://vf.jctech888.com.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://il.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://nt.haigaiapp.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://bm.shxzukj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ye.bjjhwx.cn

================================================================================
来源：http://wh.newstarts.cn

J. 日期与时间
来源：http://cc.huixinmuqiang.cn

================================================================================
来源：http://cw.lnxyls.cn

[J01] 获取当前时间
来源：http://hp.huixiangedu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ah.haigaiapp.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fq.huixiangedu.cn

JS:   new Date();  Date.now()
来源：http://cy.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://gr.shxzskj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://rk.huanxung.cn

Go:   time.Now()
来源：http://ay.asd995.cn

Ruby: Time.now
来源：http://nt.521024.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://da.wgjwhj.cn

[J02] 格式化输出
来源：http://ni.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vr.huanxung.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://gd.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sd.yuntaijiaju.cn

TS:   d.toISOString()
来源：http://pg.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://us.hahajie.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://jj.haigaiapp.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://so.huanxung.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://tp.jianghongdianzi.cn

[J03] 字符串解析为日期
来源：http://pd.shtwfgs.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://bx.huixinmuqiang.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xt.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://rx.nicolike.cn

TS:   new Date("2024-01-02")
来源：http://mj.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://de.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ge.bookmarksfly.cn

Ruby: Date.parse("2024-01-02")
来源：http://io.szxytkj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dv.521024.cn

[J04] 时间戳与日期互转
来源：http://tm.lnxyls.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hf.asd995.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ou.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://gd.yuntaijiaju.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://dh.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://mq.haigaiapp.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://xi.bjjhwx.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://gh.shxzskj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vh.huanxung.cn

[J05] 时间加减（加 7 天）
来源：http://zt.newstarts.cn

Py:   now + timedelta(days=7)
来源：http://ed.521024.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xj.newstarts.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hn.huixinmuqiang.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://eu.newstarts.cn

Java: LocalDate.now().plusDays(7)
来源：http://on.haigaiapp.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://wf.jianghongdianzi.cn

Ruby: Time.now + 7 * 86400
来源：http://px.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://zm.jctech888.com.cn

[J06] 计算两时间之差
来源：http://wc.yuntaijiaju.cn

Py:   (end - start).total_seconds()
来源：http://nn.bookmarksfly.cn

PHP:  $end->diff($start)->days;
来源：http://wc.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://va.shxzukj.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tn.bjjhwx.cn

Java: Duration.between(start, end).toSeconds()
来源：http://la.yuexingan06.cn

Go:   end.Sub(start).Hours()
来源：http://dr.bjjhwx.cn

Ruby: end - start                 # 返回秒数
来源：http://hj.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://zu.9csxet.cn

[J07] 比较两个日期
来源：http://mj.bookmarksfly.cn

Py:   d1 < d2;  d1 == d2
来源：http://ek.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://un.521024.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ao.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ja.jctech888.com.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bs.huixinmuqiang.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://um.colortex.cn

Ruby: d1 < d2;  d1 == d2
来源：http://rv.hnjuh.cn

C#:   d1 < d2;  d1 == d2
来源：http://ab.bjjhwx.cn

[J08] 提取年月日与星期
来源：http://ry.9csxet.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qv.yuntaijiaju.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eg.jctech888.com.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nq.szxytkj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jf.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ky.9csxet.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lm.colortex.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://cd.jianghongdianzi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://um.panjiajie.cn

[J09] 时区处理
来源：http://gq.jctech888.com.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zz.shtwfgs.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xk.panjiajie.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://da.shtwfgs.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ps.9csxet.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jy.panjiajie.cn


<!-- 参考信息 -->