代发 wailian999

TS:   public / protected / private
来源：http://lr.newstarts.cn

Java: public / protected / private / 默认包级
来源：http://pm.yuexingan06.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://jg.9csxet.cn

Ruby: public / protected / private
来源：http://ow.huanxung.cn

C#:   public / protected / private / internal
来源：http://op.jianghongdianzi.cn

[G11] getter / setter
来源：http://ud.wgjwhj.cn

Py:   @property 与 @x.setter
来源：http://jq.huixiangedu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yb.huanxung.cn

JS:   get name() { return this._name; }
来源：http://to.hnjuh.cn

TS:   get name(): string { return this._name; }
来源：http://ag.shtwfgs.cn

Java: public String getName() { return name; }
来源：http://yd.9csxet.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ay.shtwfgs.cn

Ruby: attr_accessor :name
来源：http://wq.yuntaijiaju.cn

C#:   public string Name { get; set; }
来源：http://nx.newstarts.cn

[G12] 对象转字符串
来源：http://to.huixiangedu.cn

Py:   def __str__(self): return self.name
来源：http://ln.521024.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vs.szxytkj.cn

JS:   toString() { return this.name; }
来源：http://de.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://lj.gzmigu.cn

Java: @Override public String toString() { return name; }
来源：http://jy.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zs.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://hf.huixiangedu.cn

C#:   public override string ToString() => Name;
来源：http://qb.bjjhwx.cn

[G13] 判断对象类型
来源：http://lx.hahajie.cn

Py:   isinstance(u, User)
来源：http://da.bjjhwx.cn

PHP:  $u instanceof User
来源：http://ex.panjiajie.cn

JS:   u instanceof User
来源：http://mo.gzmigu.cn

TS:   u instanceof User
来源：http://bj.jianghongdianzi.cn

Java: u instanceof User
来源：http://vl.hnjuh.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://tf.panjiajie.cn

Ruby: u.is_a?(User)
来源：http://ak.yuexingan06.cn

C#:   u is User
来源：http://zs.shxzukj.cn

[G14] 数据类 / record
来源：http://bf.shxzskj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ia.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://pj.shtwfgs.cn

JS:   // 无内置：普通类或对象字面量
来源：http://it.gzmigu.cn

TS:   type User = { name: string; age: number };
来源：http://dq.newstarts.cn

Java: record User(String name, int age) {}
来源：http://ny.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://hz.nicolike.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ct.panjiajie.cn

C#:   record User(string Name, int Age);
来源：http://xz.szxytkj.cn

[G15] 枚举
来源：http://bq.9csxet.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tc.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://bq.asd995.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zu.bjjhwx.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ml.shxzukj.cn

Java: enum Color { RED, GREEN }
来源：http://nn.szsharing.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ig.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://nd.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bm.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://bs.haigaiapp.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://en.asd995.cn

PHP:  get_object_vars($obj);
来源：http://vt.lnxyls.cn

JS:   Object.entries(obj)
来源：http://hi.lnxyls.cn

TS:   Object.entries(obj)
来源：http://dr.huixiangedu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nz.bookmarksfly.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://iy.muxihuayi.cn

Ruby: obj.instance_variables
来源：http://xh.nicolike.cn

C#:   // 用反射或 System.Text.Json
来源：http://kp.panjiajie.cn

================================================================================
来源：http://oy.asd995.cn

H. 异常与错误处理
来源：http://zr.chemitech.net.cn

================================================================================
来源：http://qk.gzmigu.cn

[H01] try / catch 基础
来源：http://rk.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zk.huanxung.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bw.asd995.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bj.9csxet.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rv.shxzskj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xm.szxytkj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nf.nicolike.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ks.wgjwhj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://tv.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://uc.haigaiapp.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xl.panjiajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://km.hahajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xh.haigaiapp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://og.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://mt.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://df.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ef.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ts.hahajie.cn

[H03] 主动抛出异常
来源：http://ft.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://ef.hnjuh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hf.nszjky.cn

JS:   throw new Error("错误信息");
来源：http://zn.haigaiapp.cn

TS:   throw new Error("错误信息");
来源：http://is.bjjhwx.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://bm.nszjky.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://dw.huanxung.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://kc.9csxet.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vh.wgjwhj.cn

[H04] 自定义异常类型
来源：http://px.yuntaijiaju.cn

Py:   class MyError(Exception): pass
来源：http://cw.shxzukj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nc.521024.cn

JS:   class MyError extends Error {}
来源：http://of.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://ul.huixiangedu.cn

Java: class MyException extends RuntimeException {}
来源：http://jo.haigaiapp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://zg.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://gw.asd995.cn

C#:   class MyException : Exception {}
来源：http://mw.yuexingan06.cn

[H05] 捕获特定类型
来源：http://zt.9csxet.cn

Py:   except ValueError as e:
来源：http://fy.shxzukj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gm.newstarts.cn

JS:   if (e instanceof TypeError) {}
来源：http://ba.nicolike.cn

TS:   if (e instanceof TypeError) {}
来源：http://nl.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://iq.521024.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://xl.hnjuh.cn

Ruby: rescue ArgumentError => e
来源：http://qo.bjjhwx.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tj.asd995.cn

[H06] 可选值 / 空值安全访问
来源：http://hq.yuexingan06.cn

Py:   value = d.get("k") or default
来源：http://xr.szxytkj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ea.hnjuh.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ro.bookmarksfly.cn

TS:   obj?.a?.b;  d ?? default
来源：http://tj.521024.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jr.yuexingan06.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fn.huixinmuqiang.cn

Ruby: d&.dig(:a, :b)
来源：http://lv.lnxyls.cn

C#:   obj?.A?.B ?? default
来源：http://wf.shtwfgs.cn

[H07] 断言
来源：http://uj.asd995.cn

Py:   assert x > 0, "必须为正"
来源：http://sy.gzmigu.cn

PHP:  assert($x > 0);
来源：http://tf.yuexingan06.cn

JS:   console.assert(x > 0);
来源：http://tl.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://lk.huixinmuqiang.cn

Java: assert x > 0 : "必须为正";
来源：http://uz.asd995.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ai.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zd.521024.cn

C#:   Debug.Assert(x > 0);
来源：http://hg.hahajie.cn

[H08] 获取错误信息与堆栈
来源：http://ue.panjiajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://tn.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://gr.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://hj.jianghongdianzi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://fr.panjiajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://di.huixiangedu.cn

Go:   err.Error()
来源：http://qh.shtwfgs.cn

Ruby: e.message;  e.backtrace
来源：http://yb.gzmigu.cn

C#:   e.Message;  e.StackTrace
来源：http://wa.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://sk.yuntaijiaju.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://iu.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://if.huanxung.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wv.lnxyls.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://lr.nicolike.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xt.lnxyls.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vx.haigaiapp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pa.chemitech.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://qu.muxihuayi.cn

[H10] 资源自动释放
来源：http://ma.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://if.521024.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://sm.nicolike.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hn.bjjhwx.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ey.wgjwhj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://jf.shxzskj.cn

Go:   defer f.Close()
来源：http://qs.hnjuh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://to.colortex.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lg.yuexingan06.cn

================================================================================
来源：http://zv.huixinmuqiang.cn

I. 正则表达式
来源：http://pi.chemitech.net.cn

================================================================================
来源：http://sj.panjiajie.cn

[I01] 判断是否匹配
来源：http://oi.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://gw.huixinmuqiang.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ly.shxzskj.cn

JS:   /\d+/.test(s)
来源：http://pu.yuntaijiaju.cn

TS:   /\d+/.test(s)
来源：http://wd.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ct.nszjky.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://gk.huanxung.cn

Ruby: s.match?(/\d+/)
来源：http://fx.huixiangedu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://my.muxihuayi.cn

[I02] 提取所有匹配
来源：http://vj.lnxyls.cn

Py:   re.findall(r"\d+", s)
来源：http://ik.newstarts.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mk.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://bv.szxytkj.cn

TS:   s.match(/\d+/g)
来源：http://yn.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://rq.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pz.huanxung.cn

Ruby: s.scan(/\d+/)
来源：http://jx.chemitech.net.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://xb.huanxung.cn

[I03] 提取捕获分组
来源：http://zf.panjiajie.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://nj.muxihuayi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ya.nszjky.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://et.muxihuayi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yf.wgjwhj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nb.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://sr.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nr.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://eh.shxzskj.cn

[I04] 正则替换
来源：http://xt.nicolike.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ro.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://dd.yuntaijiaju.cn

JS:   s.replace(/\d+/g, "#")
来源：http://or.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sp.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jq.huixiangedu.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qs.9csxet.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hk.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qh.colortex.cn

[I05] 按正则拆分
来源：http://hr.huanxung.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://uh.newstarts.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qj.huanxung.cn

JS:   s.split(/\s*,\s*/)
来源：http://af.shxzukj.cn

TS:   s.split(/\s*,\s*/)
来源：http://hc.panjiajie.cn

Java: s.split("\\s*,\\s*")
来源：http://ca.bjjhwx.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ja.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://as.521024.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ze.yuexingan06.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kv.panjiajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bs.szsharing.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oj.shxzukj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ah.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bt.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zw.huixiangedu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://iw.colortex.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://pr.shxzukj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qm.huixiangedu.cn

[I07] 忽略大小写与多行模式
来源：http://oz.haigaiapp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vv.nicolike.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xx.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://eb.lnxyls.cn

TS:   /error/gim
来源：http://ol.huixiangedu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kv.shxzskj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bl.521024.cn

Ruby: s.scan(/error/i)
来源：http://vy.haigaiapp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://it.lnxyls.cn

[I08] 贪婪与非贪婪匹配
来源：http://aq.panjiajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://kl.jianghongdianzi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ye.asd995.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://as.yuntaijiaju.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ke.shxzskj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://se.hahajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://px.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ug.wgjwhj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://tk.wgjwhj.cn

================================================================================
来源：http://fp.shxzskj.cn

J. 日期与时间
来源：http://sq.asd995.cn

================================================================================
来源：http://yc.bjjhwx.cn

[J01] 获取当前时间
来源：http://sg.nszjky.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://df.shxzukj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://gc.nicolike.cn

JS:   new Date();  Date.now()
来源：http://yk.jctech888.com.cn

TS:   new Date();  Date.now()
来源：http://tt.shxzskj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://uh.huixinmuqiang.cn

Go:   time.Now()
来源：http://qq.jianghongdianzi.cn

Ruby: Time.now
来源：http://xl.huixiangedu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://nv.szsharing.cn

[J02] 格式化输出
来源：http://nw.yuntaijiaju.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ik.bjjhwx.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nr.yuexingan06.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mg.jctech888.com.cn

TS:   d.toISOString()
来源：http://mc.newstarts.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://qe.newstarts.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://df.chemitech.net.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vg.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wt.lnxyls.cn

[J03] 字符串解析为日期
来源：http://hj.wgjwhj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://om.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://ct.szxytkj.cn

JS:   new Date("2024-01-02")
来源：http://hx.szxytkj.cn

TS:   new Date("2024-01-02")
来源：http://xj.9csxet.cn

Java: LocalDate.parse("2024-01-02")
来源：http://km.wgjwhj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jo.bookmarksfly.cn

Ruby: Date.parse("2024-01-02")
来源：http://mb.bjjhwx.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hw.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://ln.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://gu.szsharing.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://fb.jctech888.com.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rn.lnxyls.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zy.chemitech.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oa.9csxet.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fe.shxzskj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://oj.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ir.9csxet.cn

[J05] 时间加减（加 7 天）
来源：http://dt.nicolike.cn

Py:   now + timedelta(days=7)
来源：http://tk.521024.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gb.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gw.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://aw.asd995.cn

Java: LocalDate.now().plusDays(7)
来源：http://hg.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ur.shtwfgs.cn

Ruby: Time.now + 7 * 86400
来源：http://rq.wgjwhj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ca.bjjhwx.cn

[J06] 计算两时间之差
来源：http://rk.yuexingan06.cn

Py:   (end - start).total_seconds()
来源：http://ft.szxytkj.cn

PHP:  $end->diff($start)->days;
来源：http://sm.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://eb.newstarts.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ud.muxihuayi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lk.nszjky.cn

Go:   end.Sub(start).Hours()
来源：http://pd.huixiangedu.cn

Ruby: end - start                 # 返回秒数
来源：http://mb.asd995.cn

C#:   (end - start).TotalSeconds
来源：http://oq.shtwfgs.cn

[J07] 比较两个日期
来源：http://fk.huixinmuqiang.cn

Py:   d1 < d2;  d1 == d2
来源：http://am.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://re.asd995.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xg.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zu.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ve.yuntaijiaju.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sg.yuntaijiaju.cn

Ruby: d1 < d2;  d1 == d2
来源：http://vc.wgjwhj.cn

C#:   d1 < d2;  d1 == d2
来源：http://nk.nszjky.cn

[J08] 提取年月日与星期
来源：http://jj.521024.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://sn.colortex.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://oi.chemitech.net.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dw.bjjhwx.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ac.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://kz.hahajie.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hs.hahajie.cn


<!-- 参考信息 -->