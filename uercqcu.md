代发 wailian999

JS:   get name() { return this._name; }
来源：http://vl.bookmarksfly.cn

TS:   get name(): string { return this._name; }
来源：http://ox.nicolike.cn

Java: public String getName() { return name; }
来源：http://oo.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://up.shtwfgs.cn

Ruby: attr_accessor :name
来源：http://wh.haigaiapp.cn

C#:   public string Name { get; set; }
来源：http://ql.jianghongdianzi.cn

[G12] 对象转字符串
来源：http://jb.521024.cn

Py:   def __str__(self): return self.name
来源：http://ng.haigaiapp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gg.yuexingan06.cn

JS:   toString() { return this.name; }
来源：http://ez.newstarts.cn

TS:   toString(): string { return this.name; }
来源：http://dg.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://ce.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rj.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://tb.nicolike.cn

C#:   public override string ToString() => Name;
来源：http://jq.hnjuh.cn

[G13] 判断对象类型
来源：http://bo.521024.cn

Py:   isinstance(u, User)
来源：http://bg.hnjuh.cn

PHP:  $u instanceof User
来源：http://qg.haigaiapp.cn

JS:   u instanceof User
来源：http://lz.jianghongdianzi.cn

TS:   u instanceof User
来源：http://hx.panjiajie.cn

Java: u instanceof User
来源：http://hl.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rj.haigaiapp.cn

Ruby: u.is_a?(User)
来源：http://ik.colortex.cn

C#:   u is User
来源：http://wy.chemitech.net.cn

[G14] 数据类 / record
来源：http://ux.9csxet.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lo.colortex.cn

PHP:  // 用 readonly 属性模拟
来源：http://zq.asd995.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ag.wgjwhj.cn

TS:   type User = { name: string; age: number };
来源：http://ve.asd995.cn

Java: record User(String name, int age) {}
来源：http://yh.asd995.cn

Go:   type User struct { Name string; Age int }
来源：http://zx.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dm.szxytkj.cn

C#:   record User(string Name, int Age);
来源：http://ga.szsharing.cn

[G15] 枚举
来源：http://dl.asd995.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rn.gzmigu.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bw.szsharing.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jf.shxzukj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://by.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://rl.nicolike.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://gv.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://gd.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jo.szsharing.cn

[G16] 对象转数组 / 字典
来源：http://ua.hnjuh.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jz.shtwfgs.cn

PHP:  get_object_vars($obj);
来源：http://mh.asd995.cn

JS:   Object.entries(obj)
来源：http://eq.shxzskj.cn

TS:   Object.entries(obj)
来源：http://ob.haigaiapp.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ht.szxytkj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://sd.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://ya.lnxyls.cn

C#:   // 用反射或 System.Text.Json
来源：http://dz.colortex.cn

================================================================================
来源：http://qv.huixinmuqiang.cn

H. 异常与错误处理
来源：http://qc.nszjky.cn

================================================================================
来源：http://dj.yuexingan06.cn

[H01] try / catch 基础
来源：http://lc.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tj.szxytkj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ox.chemitech.net.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://az.bookmarksfly.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://lp.hahajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qp.chemitech.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://js.huanxung.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ug.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ob.gzmigu.cn

[H02] finally / ensure 收尾
来源：http://gs.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rp.gzmigu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gb.nszjky.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bx.huixiangedu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://hb.asd995.cn

Java: try { f(); } finally { cleanup(); }
来源：http://va.szsharing.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ty.shxzukj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ou.colortex.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ok.colortex.cn

[H03] 主动抛出异常
来源：http://ma.hnjuh.cn

Py:   raise ValueError("错误信息")
来源：http://qw.shtwfgs.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ip.shtwfgs.cn

JS:   throw new Error("错误信息");
来源：http://ch.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://qz.chemitech.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ri.szsharing.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mo.colortex.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://xp.szxytkj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ly.newstarts.cn

[H04] 自定义异常类型
来源：http://gm.huixinmuqiang.cn

Py:   class MyError(Exception): pass
来源：http://ct.shxzukj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tn.shxzukj.cn

JS:   class MyError extends Error {}
来源：http://ng.szxytkj.cn

TS:   class MyError extends Error {}
来源：http://oj.colortex.cn

Java: class MyException extends RuntimeException {}
来源：http://rz.shtwfgs.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ry.haigaiapp.cn

Ruby: class MyError < StandardError; end
来源：http://qy.nszjky.cn

C#:   class MyException : Exception {}
来源：http://gy.hahajie.cn

[H05] 捕获特定类型
来源：http://em.bookmarksfly.cn

Py:   except ValueError as e:
来源：http://kh.haigaiapp.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wx.bookmarksfly.cn

JS:   if (e instanceof TypeError) {}
来源：http://ev.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://zo.huixinmuqiang.cn

Java: catch (IOException | SQLException e) {}
来源：http://ei.chemitech.net.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ho.newstarts.cn

Ruby: rescue ArgumentError => e
来源：http://fx.szsharing.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://fy.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://wx.bookmarksfly.cn

Py:   value = d.get("k") or default
来源：http://wc.muxihuayi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xj.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hu.nicolike.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ve.szsharing.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://py.jctech888.com.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qf.haigaiapp.cn

Ruby: d&.dig(:a, :b)
来源：http://hd.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://ia.szxytkj.cn

[H07] 断言
来源：http://ha.yuexingan06.cn

Py:   assert x > 0, "必须为正"
来源：http://jv.lnxyls.cn

PHP:  assert($x > 0);
来源：http://af.bookmarksfly.cn

JS:   console.assert(x > 0);
来源：http://ai.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://ua.chemitech.net.cn

Java: assert x > 0 : "必须为正";
来源：http://cg.nicolike.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://dl.nszjky.cn

Ruby: raise "必须为正" unless x > 0
来源：http://fs.jctech888.com.cn

C#:   Debug.Assert(x > 0);
来源：http://db.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://vc.szsharing.cn

Py:   str(e);  traceback.format_exc()
来源：http://me.nicolike.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://fz.wgjwhj.cn

JS:   e.message;  e.stack
来源：http://bi.gzmigu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ek.nszjky.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ie.huanxung.cn

Go:   err.Error()
来源：http://sq.521024.cn

Ruby: e.message;  e.backtrace
来源：http://sm.hnjuh.cn

C#:   e.Message;  e.StackTrace
来源：http://mk.asd995.cn

[H09] 带错误码的异常
来源：http://po.haigaiapp.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lt.muxihuayi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pq.shxzskj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ow.bjjhwx.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://xo.huixiangedu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kr.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bt.yuntaijiaju.cn

Ruby: raise MyError.new("fail", 500)
来源：http://qd.nicolike.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://um.newstarts.cn

[H10] 资源自动释放
来源：http://hg.jctech888.com.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://qm.nicolike.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://si.hnjuh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://qe.521024.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://tb.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pz.hnjuh.cn

Go:   defer f.Close()
来源：http://mn.szsharing.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://yf.haigaiapp.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vr.colortex.cn

================================================================================
来源：http://tl.bookmarksfly.cn

I. 正则表达式
来源：http://tj.newstarts.cn

================================================================================
来源：http://um.jctech888.com.cn

[I01] 判断是否匹配
来源：http://al.szxytkj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yv.shxzskj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ql.jianghongdianzi.cn

JS:   /\d+/.test(s)
来源：http://gz.hahajie.cn

TS:   /\d+/.test(s)
来源：http://cr.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dv.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ho.9csxet.cn

Ruby: s.match?(/\d+/)
来源：http://nk.szsharing.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://og.haigaiapp.cn

[I02] 提取所有匹配
来源：http://bb.newstarts.cn

Py:   re.findall(r"\d+", s)
来源：http://wu.huixinmuqiang.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://oq.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://qf.jctech888.com.cn

TS:   s.match(/\d+/g)
来源：http://wp.muxihuayi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rg.newstarts.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bk.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://be.shxzskj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mp.muxihuayi.cn

[I03] 提取捕获分组
来源：http://fl.lnxyls.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ks.yuntaijiaju.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://rf.muxihuayi.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wz.yuntaijiaju.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hl.colortex.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://bm.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ep.gzmigu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uw.bjjhwx.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://gk.haigaiapp.cn

[I04] 正则替换
来源：http://xo.hahajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://dr.colortex.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kl.asd995.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hv.bjjhwx.cn

TS:   s.replace(/\d+/g, "#")
来源：http://qb.jianghongdianzi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://bw.lnxyls.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://tx.9csxet.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vw.bjjhwx.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://en.shxzukj.cn

[I05] 按正则拆分
来源：http://rb.asd995.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gv.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ol.szxytkj.cn

JS:   s.split(/\s*,\s*/)
来源：http://uc.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://je.huixinmuqiang.cn

Java: s.split("\\s*,\\s*")
来源：http://sy.chemitech.net.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vd.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wx.jianghongdianzi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yz.lnxyls.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ui.9csxet.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://el.shxzukj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pz.huanxung.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oo.colortex.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://fa.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rq.yuntaijiaju.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://cj.jianghongdianzi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ae.jianghongdianzi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qe.colortex.cn

[I07] 忽略大小写与多行模式
来源：http://yp.hahajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://yt.shxzskj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://eh.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yd.newstarts.cn

TS:   /error/gim
来源：http://li.szsharing.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hn.haigaiapp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qr.yuexingan06.cn

Ruby: s.scan(/error/i)
来源：http://jz.hahajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://wh.shtwfgs.cn

[I08] 贪婪与非贪婪匹配
来源：http://ah.muxihuayi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uf.jianghongdianzi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wg.colortex.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zv.yuntaijiaju.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://eh.hnjuh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bv.shxzskj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lk.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hq.9csxet.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bj.yuntaijiaju.cn

================================================================================
来源：http://ww.wgjwhj.cn

J. 日期与时间
来源：http://er.panjiajie.cn

================================================================================
来源：http://zw.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://pf.bjjhwx.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ku.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://vy.jianghongdianzi.cn

JS:   new Date();  Date.now()
来源：http://gh.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://ev.huanxung.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fi.bjjhwx.cn

Go:   time.Now()
来源：http://bo.shxzskj.cn

Ruby: Time.now
来源：http://gt.9csxet.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://cy.hnjuh.cn

[J02] 格式化输出
来源：http://gw.lnxyls.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jm.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qw.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ow.yuntaijiaju.cn

TS:   d.toISOString()
来源：http://rt.shxzukj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ji.jctech888.com.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://ui.nszjky.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://nu.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://yb.jctech888.com.cn

[J03] 字符串解析为日期
来源：http://sh.asd995.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hk.9csxet.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pk.shxzukj.cn

JS:   new Date("2024-01-02")
来源：http://qz.haigaiapp.cn

TS:   new Date("2024-01-02")
来源：http://bu.shtwfgs.cn

Java: LocalDate.parse("2024-01-02")
来源：http://al.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://kf.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://ht.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://br.yuntaijiaju.cn

[J04] 时间戳与日期互转
来源：http://pz.szsharing.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://nr.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://il.huixinmuqiang.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://cy.521024.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://sr.9csxet.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bn.nicolike.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://px.lnxyls.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://co.yuntaijiaju.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://px.shxzukj.cn

[J05] 时间加减（加 7 天）
来源：http://gh.chemitech.net.cn

Py:   now + timedelta(days=7)
来源：http://zw.9csxet.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sb.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pz.newstarts.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dh.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://mp.bjjhwx.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://qs.jctech888.com.cn

Ruby: Time.now + 7 * 86400
来源：http://mj.asd995.cn

C#:   DateTime.Now.AddDays(7)
来源：http://uo.shxzskj.cn

[J06] 计算两时间之差
来源：http://qk.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://ak.wgjwhj.cn

PHP:  $end->diff($start)->days;
来源：http://lz.gzmigu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ck.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ve.jianghongdianzi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hj.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://rm.yuntaijiaju.cn

Ruby: end - start                 # 返回秒数
来源：http://vx.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://nw.yuntaijiaju.cn

[J07] 比较两个日期
来源：http://xl.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://yi.newstarts.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yc.jianghongdianzi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pa.9csxet.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sw.521024.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://po.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xv.bookmarksfly.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tm.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://qb.yuntaijiaju.cn

[J08] 提取年月日与星期
来源：http://pb.shxzukj.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sc.bookmarksfly.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://jq.nszjky.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yv.wgjwhj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yy.newstarts.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://se.huixinmuqiang.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yq.yuntaijiaju.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://pu.gzmigu.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tn.jctech888.com.cn

[J09] 时区处理
来源：http://gq.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ua.521024.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://yz.szxytkj.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vb.huixiangedu.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ii.shtwfgs.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://vr.szxytkj.cn


<!-- 参考信息 -->