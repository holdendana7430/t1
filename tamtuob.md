代发 wailian999

JS:   get name() { return this._name; }
来源：http://cc.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://by.asd995.cn

Java: public String getName() { return name; }
来源：http://qi.yuexingan06.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zt.9csxet.cn

Ruby: attr_accessor :name
来源：http://sk.colortex.cn

C#:   public string Name { get; set; }
来源：http://qu.bookmarksfly.cn

[G12] 对象转字符串
来源：http://zv.hahajie.cn

Py:   def __str__(self): return self.name
来源：http://on.muxihuayi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wu.yuexingan06.cn

JS:   toString() { return this.name; }
来源：http://kz.nszjky.cn

TS:   toString(): string { return this.name; }
来源：http://mh.jianghongdianzi.cn

Java: @Override public String toString() { return name; }
来源：http://mc.huixinmuqiang.cn

Go:   func (u User) String() string { return u.Name }
来源：http://er.nicolike.cn

Ruby: def to_s; @name; end
来源：http://ac.huixiangedu.cn

C#:   public override string ToString() => Name;
来源：http://kn.bjjhwx.cn

[G13] 判断对象类型
来源：http://zm.nszjky.cn

Py:   isinstance(u, User)
来源：http://tf.huixinmuqiang.cn

PHP:  $u instanceof User
来源：http://vu.huixinmuqiang.cn

JS:   u instanceof User
来源：http://uz.bookmarksfly.cn

TS:   u instanceof User
来源：http://zk.colortex.cn

Java: u instanceof User
来源：http://bu.muxihuayi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://qa.szxytkj.cn

Ruby: u.is_a?(User)
来源：http://ix.hnjuh.cn

C#:   u is User
来源：http://gy.szxytkj.cn

[G14] 数据类 / record
来源：http://yr.bjjhwx.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://lp.lnxyls.cn

PHP:  // 用 readonly 属性模拟
来源：http://bl.yuntaijiaju.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mt.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://un.huanxung.cn

Java: record User(String name, int age) {}
来源：http://qn.panjiajie.cn

Go:   type User struct { Name string; Age int }
来源：http://vt.shxzskj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ha.huixinmuqiang.cn

C#:   record User(string Name, int Age);
来源：http://bh.haigaiapp.cn

[G15] 枚举
来源：http://xf.bjjhwx.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vu.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vr.gzmigu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gs.szsharing.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://oy.colortex.cn

Java: enum Color { RED, GREEN }
来源：http://er.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cw.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://we.huixinmuqiang.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://dk.szxytkj.cn

[G16] 对象转数组 / 字典
来源：http://pl.szxytkj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mk.521024.cn

PHP:  get_object_vars($obj);
来源：http://id.huanxung.cn

JS:   Object.entries(obj)
来源：http://ef.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://bv.nszjky.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zl.jianghongdianzi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://kj.hahajie.cn

Ruby: obj.instance_variables
来源：http://un.huixiangedu.cn

C#:   // 用反射或 System.Text.Json
来源：http://ud.521024.cn

================================================================================
来源：http://lz.hnjuh.cn

H. 异常与错误处理
来源：http://nc.yuntaijiaju.cn

================================================================================
来源：http://na.wgjwhj.cn

[H01] try / catch 基础
来源：http://fj.wgjwhj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://xq.shtwfgs.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://nz.muxihuayi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rx.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://kx.jianghongdianzi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ys.hahajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rd.huixiangedu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yw.haigaiapp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vv.szxytkj.cn

[H02] finally / ensure 收尾
来源：http://lf.szxytkj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://jj.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ko.huanxung.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gr.bjjhwx.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ca.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qv.szsharing.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://fd.yuexingan06.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lk.shxzukj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zg.9csxet.cn

[H03] 主动抛出异常
来源：http://pu.muxihuayi.cn

Py:   raise ValueError("错误信息")
来源：http://xd.nicolike.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://cf.yuntaijiaju.cn

JS:   throw new Error("错误信息");
来源：http://qp.shxzskj.cn

TS:   throw new Error("错误信息");
来源：http://lg.shxzskj.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ki.huixinmuqiang.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://qf.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ue.szxytkj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qi.szxytkj.cn

[H04] 自定义异常类型
来源：http://dc.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://dx.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://oz.huixinmuqiang.cn

JS:   class MyError extends Error {}
来源：http://pg.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://uv.nszjky.cn

Java: class MyException extends RuntimeException {}
来源：http://jb.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yh.hnjuh.cn

Ruby: class MyError < StandardError; end
来源：http://tv.bjjhwx.cn

C#:   class MyException : Exception {}
来源：http://kw.shxzukj.cn

[H05] 捕获特定类型
来源：http://qa.bjjhwx.cn

Py:   except ValueError as e:
来源：http://dy.newstarts.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://or.nicolike.cn

JS:   if (e instanceof TypeError) {}
来源：http://ti.jctech888.com.cn

TS:   if (e instanceof TypeError) {}
来源：http://xb.jianghongdianzi.cn

Java: catch (IOException | SQLException e) {}
来源：http://en.szsharing.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://iv.yuntaijiaju.cn

Ruby: rescue ArgumentError => e
来源：http://fn.bjjhwx.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://kh.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://jk.nszjky.cn

Py:   value = d.get("k") or default
来源：http://co.panjiajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rl.gzmigu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wi.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xg.hnjuh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://am.panjiajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zv.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://fv.huixiangedu.cn

C#:   obj?.A?.B ?? default
来源：http://fc.shxzukj.cn

[H07] 断言
来源：http://mt.huanxung.cn

Py:   assert x > 0, "必须为正"
来源：http://bk.nszjky.cn

PHP:  assert($x > 0);
来源：http://ga.bookmarksfly.cn

JS:   console.assert(x > 0);
来源：http://is.huixiangedu.cn

TS:   console.assert(x > 0);
来源：http://co.nicolike.cn

Java: assert x > 0 : "必须为正";
来源：http://av.chemitech.net.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://rm.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zo.colortex.cn

C#:   Debug.Assert(x > 0);
来源：http://ht.bookmarksfly.cn

[H08] 获取错误信息与堆栈
来源：http://rr.huanxung.cn

Py:   str(e);  traceback.format_exc()
来源：http://yr.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yp.521024.cn

JS:   e.message;  e.stack
来源：http://yz.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://pm.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://me.asd995.cn

Go:   err.Error()
来源：http://mv.jctech888.com.cn

Ruby: e.message;  e.backtrace
来源：http://jq.chemitech.net.cn

C#:   e.Message;  e.StackTrace
来源：http://aw.nszjky.cn

[H09] 带错误码的异常
来源：http://fr.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://jv.colortex.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://rs.jianghongdianzi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cd.asd995.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ed.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yl.bjjhwx.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://zz.newstarts.cn

Ruby: raise MyError.new("fail", 500)
来源：http://mt.nszjky.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ng.bookmarksfly.cn

[H10] 资源自动释放
来源：http://kp.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rq.wgjwhj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://my.9csxet.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ee.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://iu.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://nf.huixiangedu.cn

Go:   defer f.Close()
来源：http://as.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://td.nszjky.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qs.shxzukj.cn

================================================================================
来源：http://zt.huixiangedu.cn

I. 正则表达式
来源：http://pe.9csxet.cn

================================================================================
来源：http://wm.hnjuh.cn

[I01] 判断是否匹配
来源：http://xi.hahajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://eg.gzmigu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://rn.jctech888.com.cn

JS:   /\d+/.test(s)
来源：http://qk.gzmigu.cn

TS:   /\d+/.test(s)
来源：http://bw.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://gd.jianghongdianzi.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bt.shtwfgs.cn

Ruby: s.match?(/\d+/)
来源：http://vh.shxzukj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://cm.haigaiapp.cn

[I02] 提取所有匹配
来源：http://pt.hahajie.cn

Py:   re.findall(r"\d+", s)
来源：http://uc.colortex.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ho.szxytkj.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://da.panjiajie.cn

TS:   s.match(/\d+/g)
来源：http://pa.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://yj.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rk.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://co.szsharing.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gn.huixiangedu.cn

[I03] 提取捕获分组
来源：http://sk.nszjky.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://bl.newstarts.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ha.9csxet.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gv.haigaiapp.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yj.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ir.shxzukj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vp.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ql.shxzukj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bd.hnjuh.cn

[I04] 正则替换
来源：http://ca.shxzskj.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.haigaiapp.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dd.newstarts.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ji.huixinmuqiang.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xb.colortex.cn

Java: s.replaceAll("\\d+", "#")
来源：http://js.shxzukj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fx.szsharing.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://wl.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ge.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://wc.szsharing.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ym.lnxyls.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rs.yuexingan06.cn

JS:   s.split(/\s*,\s*/)
来源：http://df.521024.cn

TS:   s.split(/\s*,\s*/)
来源：http://jw.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://st.szsharing.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wr.bookmarksfly.cn

Ruby: s.split(/\s*,\s*/)
来源：http://it.panjiajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fs.yuntaijiaju.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qs.muxihuayi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://zo.yuntaijiaju.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hx.jctech888.com.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://us.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tt.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hb.shxzskj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ae.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vl.nszjky.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ib.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://ze.panjiajie.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ra.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ig.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://gn.jctech888.com.cn

TS:   /error/gim
来源：http://fc.nicolike.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mk.newstarts.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bi.jctech888.com.cn

Ruby: s.scan(/error/i)
来源：http://ns.nszjky.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lb.huanxung.cn

[I08] 贪婪与非贪婪匹配
来源：http://nd.bookmarksfly.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bt.asd995.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hf.521024.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://zq.hahajie.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://av.jctech888.com.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mr.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://cy.hahajie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://dv.colortex.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://na.yuntaijiaju.cn

================================================================================
来源：http://eq.szsharing.cn

J. 日期与时间
来源：http://gm.szxytkj.cn

================================================================================
来源：http://ch.gzmigu.cn

[J01] 获取当前时间
来源：http://ak.panjiajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ep.shxzskj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xs.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://vo.hahajie.cn

TS:   new Date();  Date.now()
来源：http://de.colortex.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://to.muxihuayi.cn

Go:   time.Now()
来源：http://fp.muxihuayi.cn

Ruby: Time.now
来源：http://ua.chemitech.net.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ak.bookmarksfly.cn

[J02] 格式化输出
来源：http://nb.panjiajie.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cg.hahajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qq.newstarts.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ao.muxihuayi.cn

TS:   d.toISOString()
来源：http://mg.asd995.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ak.asd995.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tn.9csxet.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hk.szxytkj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://da.wgjwhj.cn

[J03] 字符串解析为日期
来源：http://fi.chemitech.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qc.bookmarksfly.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://te.nszjky.cn

JS:   new Date("2024-01-02")
来源：http://zc.9csxet.cn

TS:   new Date("2024-01-02")
来源：http://it.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ud.colortex.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hs.newstarts.cn

Ruby: Date.parse("2024-01-02")
来源：http://fc.9csxet.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://tj.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://db.huixinmuqiang.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ie.gzmigu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://kd.szsharing.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ez.huixinmuqiang.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ht.yuntaijiaju.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://yw.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://qg.hnjuh.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ct.muxihuayi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vl.gzmigu.cn

[J05] 时间加减（加 7 天）
来源：http://au.lnxyls.cn

Py:   now + timedelta(days=7)
来源：http://rz.gzmigu.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://nr.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://lk.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://ba.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://pj.9csxet.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hp.szsharing.cn

Ruby: Time.now + 7 * 86400
来源：http://lw.haigaiapp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rk.nszjky.cn

[J06] 计算两时间之差
来源：http://va.huixiangedu.cn

Py:   (end - start).total_seconds()
来源：http://pi.9csxet.cn

PHP:  $end->diff($start)->days;
来源：http://wi.nszjky.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://gx.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://eg.nicolike.cn

Java: Duration.between(start, end).toSeconds()
来源：http://wj.huixinmuqiang.cn

Go:   end.Sub(start).Hours()
来源：http://sc.chemitech.net.cn

Ruby: end - start                 # 返回秒数
来源：http://vd.jianghongdianzi.cn

C#:   (end - start).TotalSeconds
来源：http://dh.hnjuh.cn

[J07] 比较两个日期
来源：http://zt.huixiangedu.cn

Py:   d1 < d2;  d1 == d2
来源：http://qh.shtwfgs.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://pc.bjjhwx.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qb.hahajie.cn

TS:   d1.getTime() < d2.getTime()
来源：http://kk.szsharing.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://lc.szsharing.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zx.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ne.newstarts.cn

C#:   d1 < d2;  d1 == d2
来源：http://zc.jianghongdianzi.cn

[J08] 提取年月日与星期
来源：http://bb.szsharing.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://cf.shtwfgs.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zu.newstarts.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://vn.shxzskj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ug.asd995.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zg.jianghongdianzi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://py.nszjky.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nv.huixinmuqiang.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fm.wgjwhj.cn

[J09] 时区处理
来源：http://bp.shxzukj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rf.jctech888.com.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://td.gzmigu.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uo.huanxung.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ty.shxzukj.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://at.szxytkj.cn


<!-- 参考信息 -->