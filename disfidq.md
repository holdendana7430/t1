代发 wailian999

TS:   public / protected / private
来源：http://xh.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://ms.hnjuh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sl.szxytkj.cn

Ruby: public / protected / private
来源：http://vz.9csxet.cn

C#:   public / protected / private / internal
来源：http://qv.huanxung.cn

[G11] getter / setter
来源：http://tb.szsharing.cn

Py:   @property 与 @x.setter
来源：http://rr.shtwfgs.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://pu.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://eq.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://qp.colortex.cn

Java: public String getName() { return name; }
来源：http://he.yuexingan06.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fw.jctech888.com.cn

Ruby: attr_accessor :name
来源：http://im.wgjwhj.cn

C#:   public string Name { get; set; }
来源：http://it.521024.cn

[G12] 对象转字符串
来源：http://sd.szxytkj.cn

Py:   def __str__(self): return self.name
来源：http://fs.yuntaijiaju.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://pp.bookmarksfly.cn

JS:   toString() { return this.name; }
来源：http://nq.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://iu.huixinmuqiang.cn

Java: @Override public String toString() { return name; }
来源：http://gz.asd995.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ur.hnjuh.cn

Ruby: def to_s; @name; end
来源：http://qp.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://hg.nszjky.cn

[G13] 判断对象类型
来源：http://yg.wgjwhj.cn

Py:   isinstance(u, User)
来源：http://kp.jctech888.com.cn

PHP:  $u instanceof User
来源：http://qf.shxzukj.cn

JS:   u instanceof User
来源：http://qb.shtwfgs.cn

TS:   u instanceof User
来源：http://hl.shxzukj.cn

Java: u instanceof User
来源：http://tb.521024.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://in.colortex.cn

Ruby: u.is_a?(User)
来源：http://my.szsharing.cn

C#:   u is User
来源：http://tj.bjjhwx.cn

[G14] 数据类 / record
来源：http://cm.nszjky.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tj.bjjhwx.cn

PHP:  // 用 readonly 属性模拟
来源：http://ip.jctech888.com.cn

JS:   // 无内置：普通类或对象字面量
来源：http://cx.9csxet.cn

TS:   type User = { name: string; age: number };
来源：http://zl.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://iq.gzmigu.cn

Go:   type User struct { Name string; Age int }
来源：http://wy.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uc.bjjhwx.cn

C#:   record User(string Name, int Age);
来源：http://ek.panjiajie.cn

[G15] 枚举
来源：http://tg.bjjhwx.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ns.nszjky.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qt.szsharing.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ep.wgjwhj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://df.nicolike.cn

Java: enum Color { RED, GREEN }
来源：http://js.colortex.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://cr.521024.cn

Ruby: Color = %i[red green].freeze
来源：http://hf.asd995.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ry.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://du.jctech888.com.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://gl.asd995.cn

PHP:  get_object_vars($obj);
来源：http://vw.jianghongdianzi.cn

JS:   Object.entries(obj)
来源：http://qm.asd995.cn

TS:   Object.entries(obj)
来源：http://ra.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xx.gzmigu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zf.hnjuh.cn

Ruby: obj.instance_variables
来源：http://vw.9csxet.cn

C#:   // 用反射或 System.Text.Json
来源：http://mg.asd995.cn

================================================================================
来源：http://lo.haigaiapp.cn

H. 异常与错误处理
来源：http://wb.yuntaijiaju.cn

================================================================================
来源：http://co.muxihuayi.cn

[H01] try / catch 基础
来源：http://xq.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://su.wgjwhj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qh.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tb.hahajie.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zt.wgjwhj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://rx.bjjhwx.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://sl.hahajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://pv.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://bf.asd995.cn

[H02] finally / ensure 收尾
来源：http://zg.shtwfgs.cn

Py:   try: f()⏎finally: cleanup()
来源：http://sn.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://rx.yuntaijiaju.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ls.jianghongdianzi.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xo.shtwfgs.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bj.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ec.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hp.gzmigu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bl.nszjky.cn

[H03] 主动抛出异常
来源：http://vg.bookmarksfly.cn

Py:   raise ValueError("错误信息")
来源：http://cs.huanxung.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ck.nicolike.cn

JS:   throw new Error("错误信息");
来源：http://bt.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://ps.haigaiapp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://js.jianghongdianzi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zo.szxytkj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://vi.chemitech.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://aa.bookmarksfly.cn

[H04] 自定义异常类型
来源：http://se.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://ys.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gs.shxzskj.cn

JS:   class MyError extends Error {}
来源：http://mj.muxihuayi.cn

TS:   class MyError extends Error {}
来源：http://py.jianghongdianzi.cn

Java: class MyException extends RuntimeException {}
来源：http://bg.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vl.huixiangedu.cn

Ruby: class MyError < StandardError; end
来源：http://ip.hnjuh.cn

C#:   class MyException : Exception {}
来源：http://ed.asd995.cn

[H05] 捕获特定类型
来源：http://qe.szsharing.cn

Py:   except ValueError as e:
来源：http://hh.yuntaijiaju.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wi.colortex.cn

JS:   if (e instanceof TypeError) {}
来源：http://ok.panjiajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://mt.huanxung.cn

Java: catch (IOException | SQLException e) {}
来源：http://xv.yuexingan06.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nx.huixiangedu.cn

Ruby: rescue ArgumentError => e
来源：http://fg.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jn.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://wt.newstarts.cn

Py:   value = d.get("k") or default
来源：http://ub.jctech888.com.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cf.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://hl.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://bf.haigaiapp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mz.szsharing.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://xj.haigaiapp.cn

Ruby: d&.dig(:a, :b)
来源：http://jl.nszjky.cn

C#:   obj?.A?.B ?? default
来源：http://mr.gzmigu.cn

[H07] 断言
来源：http://wb.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://db.jctech888.com.cn

PHP:  assert($x > 0);
来源：http://cb.hahajie.cn

JS:   console.assert(x > 0);
来源：http://zp.bookmarksfly.cn

TS:   console.assert(x > 0);
来源：http://ly.colortex.cn

Java: assert x > 0 : "必须为正";
来源：http://je.muxihuayi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ju.newstarts.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uv.yuntaijiaju.cn

C#:   Debug.Assert(x > 0);
来源：http://ww.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://xp.muxihuayi.cn

Py:   str(e);  traceback.format_exc()
来源：http://wd.wgjwhj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tr.hahajie.cn

JS:   e.message;  e.stack
来源：http://xu.newstarts.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lv.asd995.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ec.bjjhwx.cn

Go:   err.Error()
来源：http://si.asd995.cn

Ruby: e.message;  e.backtrace
来源：http://mj.huanxung.cn

C#:   e.Message;  e.StackTrace
来源：http://rh.muxihuayi.cn

[H09] 带错误码的异常
来源：http://ws.yuntaijiaju.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://eb.colortex.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xg.haigaiapp.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ce.szsharing.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hm.bjjhwx.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cr.jianghongdianzi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tf.huixiangedu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hc.hahajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://sw.bookmarksfly.cn

[H10] 资源自动释放
来源：http://jj.hahajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pd.nicolike.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://oi.szsharing.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://tq.bookmarksfly.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mu.colortex.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://co.bookmarksfly.cn

Go:   defer f.Close()
来源：http://sy.jctech888.com.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fe.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://un.shxzskj.cn

================================================================================
来源：http://xu.wgjwhj.cn

I. 正则表达式
来源：http://yi.asd995.cn

================================================================================
来源：http://dp.nszjky.cn

[I01] 判断是否匹配
来源：http://pb.gzmigu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bj.yuntaijiaju.cn

PHP:  preg_match('/\d+/', $s);
来源：http://pc.shxzukj.cn

JS:   /\d+/.test(s)
来源：http://uv.colortex.cn

TS:   /\d+/.test(s)
来源：http://gy.haigaiapp.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ni.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://za.jianghongdianzi.cn

Ruby: s.match?(/\d+/)
来源：http://mz.hahajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rd.colortex.cn

[I02] 提取所有匹配
来源：http://xl.yuexingan06.cn

Py:   re.findall(r"\d+", s)
来源：http://pk.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uw.hahajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hl.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://lh.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ha.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fe.hahajie.cn

Ruby: s.scan(/\d+/)
来源：http://xj.szxytkj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ww.asd995.cn

[I03] 提取捕获分组
来源：http://fw.szsharing.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://rw.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jk.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://gd.huixiangedu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://uw.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://tm.nszjky.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ng.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fx.bookmarksfly.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://it.bjjhwx.cn

[I04] 正则替换
来源：http://mm.jctech888.com.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://nw.yuexingan06.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mz.521024.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xb.gzmigu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ki.szsharing.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pn.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ww.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sf.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://lb.chemitech.net.cn

[I05] 按正则拆分
来源：http://om.huixinmuqiang.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://id.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rm.bjjhwx.cn

JS:   s.split(/\s*,\s*/)
来源：http://zf.huixinmuqiang.cn

TS:   s.split(/\s*,\s*/)
来源：http://vp.bookmarksfly.cn

Java: s.split("\\s*,\\s*")
来源：http://rt.jianghongdianzi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://cp.nszjky.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ku.wgjwhj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://qc.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wj.colortex.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dw.asd995.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ah.muxihuayi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://as.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dg.nicolike.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yq.yuexingan06.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gz.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://dm.bookmarksfly.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hn.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://si.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qi.hnjuh.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://lr.9csxet.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://uz.szsharing.cn

TS:   /error/gim
来源：http://eb.szxytkj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://uv.huanxung.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://nu.gzmigu.cn

Ruby: s.scan(/error/i)
来源：http://ec.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://el.hahajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://rt.yuntaijiaju.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://nm.huixinmuqiang.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://br.nicolike.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hu.shxzskj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jp.shxzukj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://yf.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://ol.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yf.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://fl.nicolike.cn

================================================================================
来源：http://vk.shtwfgs.cn

J. 日期与时间
来源：http://dv.wgjwhj.cn

================================================================================
来源：http://qd.haigaiapp.cn

[J01] 获取当前时间
来源：http://gj.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cg.gzmigu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wa.yuntaijiaju.cn

JS:   new Date();  Date.now()
来源：http://ln.shtwfgs.cn

TS:   new Date();  Date.now()
来源：http://gp.szsharing.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://kr.haigaiapp.cn

Go:   time.Now()
来源：http://cl.hahajie.cn

Ruby: Time.now
来源：http://nh.lnxyls.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mx.szxytkj.cn

[J02] 格式化输出
来源：http://ry.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://jo.yuntaijiaju.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yr.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://no.yuexingan06.cn

TS:   d.toISOString()
来源：http://jj.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mo.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kl.huixiangedu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bl.yuexingan06.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://nm.nszjky.cn

[J03] 字符串解析为日期
来源：http://vg.newstarts.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://vv.521024.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pm.huixiangedu.cn

JS:   new Date("2024-01-02")
来源：http://jt.huixinmuqiang.cn

TS:   new Date("2024-01-02")
来源：http://dh.hnjuh.cn

Java: LocalDate.parse("2024-01-02")
来源：http://wt.bookmarksfly.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zz.bjjhwx.cn

Ruby: Date.parse("2024-01-02")
来源：http://tm.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ny.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://mx.asd995.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hm.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ls.hnjuh.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://sw.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gj.hahajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://qh.huixiangedu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://uy.huixinmuqiang.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://te.jianghongdianzi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://mu.szsharing.cn

[J05] 时间加减（加 7 天）
来源：http://ag.huixiangedu.cn

Py:   now + timedelta(days=7)
来源：http://ru.szxytkj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://vb.yuexingan06.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://dg.wgjwhj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zc.panjiajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://fy.hnjuh.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://yc.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://ui.nicolike.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dn.shxzskj.cn

[J06] 计算两时间之差
来源：http://hb.muxihuayi.cn

Py:   (end - start).total_seconds()
来源：http://os.hahajie.cn

PHP:  $end->diff($start)->days;
来源：http://vj.szsharing.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://om.jianghongdianzi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mh.shxzskj.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ay.shxzskj.cn

Go:   end.Sub(start).Hours()
来源：http://ue.wgjwhj.cn

Ruby: end - start                 # 返回秒数
来源：http://cq.szsharing.cn

C#:   (end - start).TotalSeconds
来源：http://xf.shxzukj.cn

[J07] 比较两个日期
来源：http://jo.gzmigu.cn

Py:   d1 < d2;  d1 == d2
来源：http://sj.huanxung.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ud.panjiajie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://hq.huixiangedu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://nd.huixiangedu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ts.szxytkj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dv.huixiangedu.cn

Ruby: d1 < d2;  d1 == d2
来源：http://fj.shtwfgs.cn

C#:   d1 < d2;  d1 == d2
来源：http://iu.szxytkj.cn

[J08] 提取年月日与星期
来源：http://rs.newstarts.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wg.newstarts.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://vc.newstarts.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://um.yuexingan06.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://yh.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uy.szsharing.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hx.jctech888.com.cn


<!-- 参考信息 -->