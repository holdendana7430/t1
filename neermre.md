代发 wailian999

C#:   public / protected / private / internal
来源：http://uf.panjiajie.cn

[G11] getter / setter
来源：http://iz.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://nh.szsharing.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://at.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://eg.lnxyls.cn

TS:   get name(): string { return this._name; }
来源：http://dx.jianghongdianzi.cn

Java: public String getName() { return name; }
来源：http://zd.huanxung.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gl.haigaiapp.cn

Ruby: attr_accessor :name
来源：http://fu.huanxung.cn

C#:   public string Name { get; set; }
来源：http://er.yuexingan06.cn

[G12] 对象转字符串
来源：http://mv.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://gc.huixiangedu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fp.huanxung.cn

JS:   toString() { return this.name; }
来源：http://uq.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://vp.shxzskj.cn

Java: @Override public String toString() { return name; }
来源：http://gj.bookmarksfly.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sp.muxihuayi.cn

Ruby: def to_s; @name; end
来源：http://zj.colortex.cn

C#:   public override string ToString() => Name;
来源：http://du.jctech888.com.cn

[G13] 判断对象类型
来源：http://xk.colortex.cn

Py:   isinstance(u, User)
来源：http://ps.gzmigu.cn

PHP:  $u instanceof User
来源：http://ez.muxihuayi.cn

JS:   u instanceof User
来源：http://ol.chemitech.net.cn

TS:   u instanceof User
来源：http://rj.huanxung.cn

Java: u instanceof User
来源：http://xm.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cl.hnjuh.cn

Ruby: u.is_a?(User)
来源：http://cs.yuexingan06.cn

C#:   u is User
来源：http://nj.chemitech.net.cn

[G14] 数据类 / record
来源：http://yw.panjiajie.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://xo.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://rx.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://no.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://et.huixiangedu.cn

Java: record User(String name, int age) {}
来源：http://kq.colortex.cn

Go:   type User struct { Name string; Age int }
来源：http://mr.bookmarksfly.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gn.newstarts.cn

C#:   record User(string Name, int Age);
来源：http://fo.huixinmuqiang.cn

[G15] 枚举
来源：http://pt.wgjwhj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kc.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wj.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://fq.newstarts.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cw.panjiajie.cn

Java: enum Color { RED, GREEN }
来源：http://tx.nszjky.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pf.9csxet.cn

Ruby: Color = %i[red green].freeze
来源：http://ng.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lu.yuntaijiaju.cn

[G16] 对象转数组 / 字典
来源：http://gu.huanxung.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pv.shxzskj.cn

PHP:  get_object_vars($obj);
来源：http://yx.chemitech.net.cn

JS:   Object.entries(obj)
来源：http://hy.yuntaijiaju.cn

TS:   Object.entries(obj)
来源：http://zm.shtwfgs.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fm.muxihuayi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ja.9csxet.cn

Ruby: obj.instance_variables
来源：http://cp.lnxyls.cn

C#:   // 用反射或 System.Text.Json
来源：http://gr.huixinmuqiang.cn

================================================================================
来源：http://ol.asd995.cn

H. 异常与错误处理
来源：http://kx.521024.cn

================================================================================
来源：http://ak.asd995.cn

[H01] try / catch 基础
来源：http://or.bjjhwx.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uq.huixinmuqiang.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://pq.szsharing.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://sl.newstarts.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cg.muxihuayi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tb.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ad.wgjwhj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://kd.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ff.hahajie.cn

[H02] finally / ensure 收尾
来源：http://ud.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://uy.huixinmuqiang.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hw.szxytkj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xy.newstarts.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ag.bjjhwx.cn

Java: try { f(); } finally { cleanup(); }
来源：http://lj.chemitech.net.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ew.haigaiapp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hx.huanxung.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pu.szxytkj.cn

[H03] 主动抛出异常
来源：http://td.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://tp.nicolike.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://dm.szxytkj.cn

JS:   throw new Error("错误信息");
来源：http://sl.yuexingan06.cn

TS:   throw new Error("错误信息");
来源：http://ei.jianghongdianzi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vl.shxzskj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mw.panjiajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ov.colortex.cn

C#:   throw new ArgumentException("错误信息");
来源：http://wu.bookmarksfly.cn

[H04] 自定义异常类型
来源：http://kn.huixiangedu.cn

Py:   class MyError(Exception): pass
来源：http://km.wgjwhj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zr.szsharing.cn

JS:   class MyError extends Error {}
来源：http://ay.hnjuh.cn

TS:   class MyError extends Error {}
来源：http://vg.lnxyls.cn

Java: class MyException extends RuntimeException {}
来源：http://if.jctech888.com.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://be.wgjwhj.cn

Ruby: class MyError < StandardError; end
来源：http://zm.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://uf.nszjky.cn

[H05] 捕获特定类型
来源：http://dt.bjjhwx.cn

Py:   except ValueError as e:
来源：http://vg.szsharing.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pv.bjjhwx.cn

JS:   if (e instanceof TypeError) {}
来源：http://ef.jctech888.com.cn

TS:   if (e instanceof TypeError) {}
来源：http://av.yuexingan06.cn

Java: catch (IOException | SQLException e) {}
来源：http://vi.hahajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://sb.jianghongdianzi.cn

Ruby: rescue ArgumentError => e
来源：http://dg.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wm.newstarts.cn

[H06] 可选值 / 空值安全访问
来源：http://pp.bjjhwx.cn

Py:   value = d.get("k") or default
来源：http://io.bookmarksfly.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ad.asd995.cn

JS:   obj?.a?.b;  d ?? default
来源：http://es.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://ze.muxihuayi.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jv.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://kx.szsharing.cn

Ruby: d&.dig(:a, :b)
来源：http://zm.huanxung.cn

C#:   obj?.A?.B ?? default
来源：http://dh.shtwfgs.cn

[H07] 断言
来源：http://qg.muxihuayi.cn

Py:   assert x > 0, "必须为正"
来源：http://de.newstarts.cn

PHP:  assert($x > 0);
来源：http://ba.asd995.cn

JS:   console.assert(x > 0);
来源：http://ni.huanxung.cn

TS:   console.assert(x > 0);
来源：http://bq.9csxet.cn

Java: assert x > 0 : "必须为正";
来源：http://bu.muxihuayi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bz.hnjuh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tf.lnxyls.cn

C#:   Debug.Assert(x > 0);
来源：http://ic.gzmigu.cn

[H08] 获取错误信息与堆栈
来源：http://wp.haigaiapp.cn

Py:   str(e);  traceback.format_exc()
来源：http://iq.yuexingan06.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mg.muxihuayi.cn

JS:   e.message;  e.stack
来源：http://zc.521024.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jy.nszjky.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://nx.yuntaijiaju.cn

Go:   err.Error()
来源：http://fx.huanxung.cn

Ruby: e.message;  e.backtrace
来源：http://bo.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://bx.yuexingan06.cn

[H09] 带错误码的异常
来源：http://fz.hahajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ml.jianghongdianzi.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://ij.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zr.panjiajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://gh.asd995.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zk.gzmigu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fn.haigaiapp.cn

Ruby: raise MyError.new("fail", 500)
来源：http://af.hahajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://if.9csxet.cn

[H10] 资源自动释放
来源：http://fc.huixinmuqiang.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://fy.wgjwhj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://tl.newstarts.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ja.szsharing.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://up.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zx.yuntaijiaju.cn

Go:   defer f.Close()
来源：http://lr.huixiangedu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gf.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://nw.jianghongdianzi.cn

================================================================================
来源：http://jz.shxzukj.cn

I. 正则表达式
来源：http://vp.szxytkj.cn

================================================================================
来源：http://rt.yuexingan06.cn

[I01] 判断是否匹配
来源：http://ld.haigaiapp.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ov.shtwfgs.cn

PHP:  preg_match('/\d+/', $s);
来源：http://lx.bookmarksfly.cn

JS:   /\d+/.test(s)
来源：http://mw.yuntaijiaju.cn

TS:   /\d+/.test(s)
来源：http://so.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://yw.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ul.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://rh.jctech888.com.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://oa.colortex.cn

[I02] 提取所有匹配
来源：http://sb.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://kt.shxzskj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://af.haigaiapp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://gy.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://il.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://dy.szsharing.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ns.lnxyls.cn

Ruby: s.scan(/\d+/)
来源：http://lk.521024.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://um.shtwfgs.cn

[I03] 提取捕获分组
来源：http://tq.bjjhwx.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ei.yuexingan06.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ka.hnjuh.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zs.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xi.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://kt.haigaiapp.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yp.colortex.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sg.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://qz.bookmarksfly.cn

[I04] 正则替换
来源：http://ra.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rc.nicolike.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ax.huixinmuqiang.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ok.szxytkj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://jr.newstarts.cn

Java: s.replaceAll("\\d+", "#")
来源：http://qd.asd995.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://om.nicolike.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xi.wgjwhj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gl.hnjuh.cn

[I05] 按正则拆分
来源：http://dq.shtwfgs.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://yi.nszjky.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://pa.colortex.cn

JS:   s.split(/\s*,\s*/)
来源：http://nq.nszjky.cn

TS:   s.split(/\s*,\s*/)
来源：http://ig.yuntaijiaju.cn

Java: s.split("\\s*,\\s*")
来源：http://km.muxihuayi.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://be.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ah.nszjky.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ti.bjjhwx.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://eg.shtwfgs.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://vi.colortex.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lo.huixinmuqiang.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://un.huanxung.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ar.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bu.nszjky.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ln.panjiajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zq.huixinmuqiang.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://zo.bjjhwx.cn

[I07] 忽略大小写与多行模式
来源：http://nl.wgjwhj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dl.newstarts.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zp.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nz.yuntaijiaju.cn

TS:   /error/gim
来源：http://bf.huanxung.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ut.colortex.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wy.szsharing.cn

Ruby: s.scan(/error/i)
来源：http://os.bookmarksfly.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://qu.huanxung.cn

[I08] 贪婪与非贪婪匹配
来源：http://vr.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vf.yuexingan06.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://te.huixiangedu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tf.bookmarksfly.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ke.huixinmuqiang.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ss.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vw.bjjhwx.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vv.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ew.haigaiapp.cn

================================================================================
来源：http://jc.hnjuh.cn

J. 日期与时间
来源：http://kn.gzmigu.cn

================================================================================
来源：http://lw.yuexingan06.cn

[J01] 获取当前时间
来源：http://mk.jctech888.com.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tk.bjjhwx.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://td.huanxung.cn

JS:   new Date();  Date.now()
来源：http://xs.jctech888.com.cn

TS:   new Date();  Date.now()
来源：http://if.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ys.szsharing.cn

Go:   time.Now()
来源：http://hj.yuexingan06.cn

Ruby: Time.now
来源：http://vl.bookmarksfly.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://gv.huixiangedu.cn

[J02] 格式化输出
来源：http://ps.shtwfgs.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vx.nszjky.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qk.huixiangedu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ce.lnxyls.cn

TS:   d.toISOString()
来源：http://cx.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mt.chemitech.net.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hb.huixiangedu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://iy.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://ww.hahajie.cn

[J03] 字符串解析为日期
来源：http://vm.shxzukj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://qq.gzmigu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shxzukj.cn

JS:   new Date("2024-01-02")
来源：http://nv.bookmarksfly.cn

TS:   new Date("2024-01-02")
来源：http://zk.shxzukj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ou.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://te.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://pd.szxytkj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://lf.nicolike.cn

[J04] 时间戳与日期互转
来源：http://rm.panjiajie.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://sp.jctech888.com.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://gz.panjiajie.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://fc.colortex.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ku.muxihuayi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sl.muxihuayi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://nw.jianghongdianzi.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ax.9csxet.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hb.wgjwhj.cn

[J05] 时间加减（加 7 天）
来源：http://qu.9csxet.cn

Py:   now + timedelta(days=7)
来源：http://bd.shxzskj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://uy.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://gt.shxzskj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dc.nszjky.cn

Java: LocalDate.now().plusDays(7)
来源：http://ru.szsharing.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pp.szxytkj.cn

Ruby: Time.now + 7 * 86400
来源：http://xg.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://xg.gzmigu.cn

[J06] 计算两时间之差
来源：http://ml.huixinmuqiang.cn

Py:   (end - start).total_seconds()
来源：http://fb.hnjuh.cn

PHP:  $end->diff($start)->days;
来源：http://bc.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://kj.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://gi.panjiajie.cn

Java: Duration.between(start, end).toSeconds()
来源：http://td.chemitech.net.cn

Go:   end.Sub(start).Hours()
来源：http://qr.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://el.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://vt.bjjhwx.cn

[J07] 比较两个日期
来源：http://bj.asd995.cn

Py:   d1 < d2;  d1 == d2
来源：http://rh.szsharing.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://br.szxytkj.cn

JS:   d1.getTime() < d2.getTime()
来源：http://pb.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pv.haigaiapp.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://cy.521024.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cs.521024.cn

Ruby: d1 < d2;  d1 == d2
来源：http://kd.asd995.cn

C#:   d1 < d2;  d1 == d2
来源：http://rz.9csxet.cn

[J08] 提取年月日与星期
来源：http://yn.huixinmuqiang.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://is.9csxet.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://cu.wgjwhj.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://az.nicolike.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ec.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://rh.huixinmuqiang.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ln.shxzskj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://so.bjjhwx.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wj.bookmarksfly.cn

[J09] 时区处理
来源：http://ln.wgjwhj.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://op.shtwfgs.cn


<!-- 参考信息 -->