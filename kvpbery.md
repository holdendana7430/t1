代发 wailian999

TS:   public / protected / private
来源：http://oz.wgjwhj.cn

Java: public / protected / private / 默认包级
来源：http://vc.gzmigu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fg.9csxet.cn

Ruby: public / protected / private
来源：http://uf.huixinmuqiang.cn

C#:   public / protected / private / internal
来源：http://su.wgjwhj.cn

[G11] getter / setter
来源：http://if.bjjhwx.cn

Py:   @property 与 @x.setter
来源：http://tz.huanxung.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://bq.colortex.cn

JS:   get name() { return this._name; }
来源：http://sn.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://za.nicolike.cn

Java: public String getName() { return name; }
来源：http://nj.521024.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ks.shxzukj.cn

Ruby: attr_accessor :name
来源：http://qh.wgjwhj.cn

C#:   public string Name { get; set; }
来源：http://uf.gzmigu.cn

[G12] 对象转字符串
来源：http://pt.9csxet.cn

Py:   def __str__(self): return self.name
来源：http://oz.panjiajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fl.muxihuayi.cn

JS:   toString() { return this.name; }
来源：http://id.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://lz.shxzskj.cn

Java: @Override public String toString() { return name; }
来源：http://rj.wgjwhj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tn.nszjky.cn

Ruby: def to_s; @name; end
来源：http://tf.huixiangedu.cn

C#:   public override string ToString() => Name;
来源：http://ik.hahajie.cn

[G13] 判断对象类型
来源：http://qy.9csxet.cn

Py:   isinstance(u, User)
来源：http://to.nszjky.cn

PHP:  $u instanceof User
来源：http://hn.huixiangedu.cn

JS:   u instanceof User
来源：http://hc.bookmarksfly.cn

TS:   u instanceof User
来源：http://ml.chemitech.net.cn

Java: u instanceof User
来源：http://sq.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gn.haigaiapp.cn

Ruby: u.is_a?(User)
来源：http://np.bjjhwx.cn

C#:   u is User
来源：http://mk.newstarts.cn

[G14] 数据类 / record
来源：http://lv.bjjhwx.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://cp.shxzukj.cn

PHP:  // 用 readonly 属性模拟
来源：http://xv.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://oq.haigaiapp.cn

TS:   type User = { name: string; age: number };
来源：http://xm.huanxung.cn

Java: record User(String name, int age) {}
来源：http://cu.newstarts.cn

Go:   type User struct { Name string; Age int }
来源：http://cj.huixinmuqiang.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://ka.lnxyls.cn

C#:   record User(string Name, int Age);
来源：http://zo.shtwfgs.cn

[G15] 枚举
来源：http://qy.shxzskj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pb.haigaiapp.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zp.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://em.huanxung.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://tm.haigaiapp.cn

Java: enum Color { RED, GREEN }
来源：http://he.jianghongdianzi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kl.chemitech.net.cn

Ruby: Color = %i[red green].freeze
来源：http://gg.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://fg.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://jo.hahajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ka.haigaiapp.cn

PHP:  get_object_vars($obj);
来源：http://gb.shxzukj.cn

JS:   Object.entries(obj)
来源：http://lv.jianghongdianzi.cn

TS:   Object.entries(obj)
来源：http://qc.shxzskj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mf.jctech888.com.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://av.bookmarksfly.cn

Ruby: obj.instance_variables
来源：http://jf.lnxyls.cn

C#:   // 用反射或 System.Text.Json
来源：http://ig.bjjhwx.cn

================================================================================
来源：http://pi.chemitech.net.cn

H. 异常与错误处理
来源：http://ze.hnjuh.cn

================================================================================
来源：http://kw.yuexingan06.cn

[H01] try / catch 基础
来源：http://wm.szsharing.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ca.muxihuayi.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jw.shxzskj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ld.muxihuayi.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://uk.yuexingan06.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://vq.chemitech.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://db.bookmarksfly.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jx.huanxung.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yu.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://zn.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://qg.colortex.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://fq.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vt.hahajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nk.shtwfgs.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gn.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://or.gzmigu.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://yo.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hk.wgjwhj.cn

[H03] 主动抛出异常
来源：http://of.hnjuh.cn

Py:   raise ValueError("错误信息")
来源：http://hr.yuexingan06.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kl.521024.cn

JS:   throw new Error("错误信息");
来源：http://xz.muxihuayi.cn

TS:   throw new Error("错误信息");
来源：http://by.huixiangedu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fb.colortex.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cj.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://az.lnxyls.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gc.nszjky.cn

[H04] 自定义异常类型
来源：http://zq.huixinmuqiang.cn

Py:   class MyError(Exception): pass
来源：http://tw.newstarts.cn

PHP:  class MyError extends RuntimeException {}
来源：http://rl.521024.cn

JS:   class MyError extends Error {}
来源：http://sv.asd995.cn

TS:   class MyError extends Error {}
来源：http://pb.nszjky.cn

Java: class MyException extends RuntimeException {}
来源：http://vs.newstarts.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://xs.shxzskj.cn

Ruby: class MyError < StandardError; end
来源：http://wf.shxzskj.cn

C#:   class MyException : Exception {}
来源：http://vs.nszjky.cn

[H05] 捕获特定类型
来源：http://ut.shtwfgs.cn

Py:   except ValueError as e:
来源：http://ac.szxytkj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://yr.panjiajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://xy.szxytkj.cn

TS:   if (e instanceof TypeError) {}
来源：http://ub.hahajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://jw.szxytkj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bm.bookmarksfly.cn

Ruby: rescue ArgumentError => e
来源：http://wq.bookmarksfly.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://va.bookmarksfly.cn

[H06] 可选值 / 空值安全访问
来源：http://np.jctech888.com.cn

Py:   value = d.get("k") or default
来源：http://jh.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hc.colortex.cn

JS:   obj?.a?.b;  d ?? default
来源：http://kl.szxytkj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://jo.szsharing.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sy.haigaiapp.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://hw.huixinmuqiang.cn

Ruby: d&.dig(:a, :b)
来源：http://yy.colortex.cn

C#:   obj?.A?.B ?? default
来源：http://kk.shxzskj.cn

[H07] 断言
来源：http://eo.huixinmuqiang.cn

Py:   assert x > 0, "必须为正"
来源：http://mo.panjiajie.cn

PHP:  assert($x > 0);
来源：http://mh.szxytkj.cn

JS:   console.assert(x > 0);
来源：http://gf.shxzskj.cn

TS:   console.assert(x > 0);
来源：http://mp.huanxung.cn

Java: assert x > 0 : "必须为正";
来源：http://mu.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qz.nszjky.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cx.szsharing.cn

C#:   Debug.Assert(x > 0);
来源：http://ao.shxzskj.cn

[H08] 获取错误信息与堆栈
来源：http://mi.jianghongdianzi.cn

Py:   str(e);  traceback.format_exc()
来源：http://cl.asd995.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ai.hahajie.cn

JS:   e.message;  e.stack
来源：http://bp.hnjuh.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://xv.huixiangedu.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://vx.nszjky.cn

Go:   err.Error()
来源：http://nf.521024.cn

Ruby: e.message;  e.backtrace
来源：http://pf.newstarts.cn

C#:   e.Message;  e.StackTrace
来源：http://eq.asd995.cn

[H09] 带错误码的异常
来源：http://na.jianghongdianzi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://lk.9csxet.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://br.gzmigu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://su.wgjwhj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zm.szsharing.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://qn.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vc.nszjky.cn

Ruby: raise MyError.new("fail", 500)
来源：http://lv.jianghongdianzi.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://uf.shxzukj.cn

[H10] 资源自动释放
来源：http://ps.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ne.bjjhwx.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ze.jianghongdianzi.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://kf.521024.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ur.9csxet.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sc.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://th.nicolike.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ro.shxzskj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://rp.haigaiapp.cn

================================================================================
来源：http://qq.shxzskj.cn

I. 正则表达式
来源：http://cm.huixiangedu.cn

================================================================================
来源：http://ne.haigaiapp.cn

[I01] 判断是否匹配
来源：http://kt.panjiajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ak.huixinmuqiang.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gx.wgjwhj.cn

JS:   /\d+/.test(s)
来源：http://fc.jctech888.com.cn

TS:   /\d+/.test(s)
来源：http://vw.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://dv.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sy.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://ib.nicolike.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ro.shtwfgs.cn

[I02] 提取所有匹配
来源：http://lz.yuexingan06.cn

Py:   re.findall(r"\d+", s)
来源：http://fb.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://at.haigaiapp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://yb.panjiajie.cn

TS:   s.match(/\d+/g)
来源：http://rh.szxytkj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bz.9csxet.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ny.muxihuayi.cn

Ruby: s.scan(/\d+/)
来源：http://td.muxihuayi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sd.shxzukj.cn

[I03] 提取捕获分组
来源：http://uw.haigaiapp.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mh.chemitech.net.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://dv.shxzskj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://nn.shxzukj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://oy.bjjhwx.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ls.lnxyls.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://pr.haigaiapp.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://ae.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://km.szxytkj.cn

[I04] 正则替换
来源：http://zg.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bw.shxzskj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://bv.shxzskj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://en.shxzskj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://pg.hahajie.cn

Java: s.replaceAll("\\d+", "#")
来源：http://hc.bjjhwx.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://bw.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fe.9csxet.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hc.nicolike.cn

[I05] 按正则拆分
来源：http://ho.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://iy.wgjwhj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ze.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://ce.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://eb.asd995.cn

Java: s.split("\\s*,\\s*")
来源：http://ti.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yo.szxytkj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://mc.9csxet.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://lb.wgjwhj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://pf.gzmigu.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://my.jianghongdianzi.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nn.szxytkj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://oj.szsharing.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://uf.nszjky.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://sm.9csxet.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ri.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fd.lnxyls.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://uf.yuntaijiaju.cn

[I07] 忽略大小写与多行模式
来源：http://xt.haigaiapp.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://fc.hahajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xh.nicolike.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vn.yuntaijiaju.cn

TS:   /error/gim
来源：http://ha.muxihuayi.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://zw.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://xe.jianghongdianzi.cn

Ruby: s.scan(/error/i)
来源：http://jw.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://sf.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://gj.szxytkj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wp.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ob.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ac.shxzskj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://go.nszjky.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nj.muxihuayi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://iu.521024.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zl.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vt.nicolike.cn

================================================================================
来源：http://cx.521024.cn

J. 日期与时间
来源：http://yd.bjjhwx.cn

================================================================================
来源：http://ld.newstarts.cn

[J01] 获取当前时间
来源：http://fq.szsharing.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://bp.shxzskj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dl.muxihuayi.cn

JS:   new Date();  Date.now()
来源：http://wr.shtwfgs.cn

TS:   new Date();  Date.now()
来源：http://qe.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://mo.9csxet.cn

Go:   time.Now()
来源：http://ys.huixiangedu.cn

Ruby: Time.now
来源：http://ik.yuntaijiaju.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://yq.huixiangedu.cn

[J02] 格式化输出
来源：http://ix.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xu.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pl.huixinmuqiang.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wx.bjjhwx.cn

TS:   d.toISOString()
来源：http://cp.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fi.nicolike.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://yd.szsharing.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wg.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fu.chemitech.net.cn

[J03] 字符串解析为日期
来源：http://jc.yuntaijiaju.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cu.gzmigu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vw.haigaiapp.cn

JS:   new Date("2024-01-02")
来源：http://tl.muxihuayi.cn

TS:   new Date("2024-01-02")
来源：http://ss.newstarts.cn

Java: LocalDate.parse("2024-01-02")
来源：http://xu.gzmigu.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cz.yuexingan06.cn

Ruby: Date.parse("2024-01-02")
来源：http://bi.jctech888.com.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://fx.haigaiapp.cn

[J04] 时间戳与日期互转
来源：http://xl.huanxung.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vc.hnjuh.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iw.szsharing.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://kt.haigaiapp.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gj.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zn.521024.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zv.nszjky.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ey.521024.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ey.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://bd.hahajie.cn

Py:   now + timedelta(days=7)
来源：http://vq.hnjuh.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://mq.9csxet.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qa.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://fy.jctech888.com.cn

Java: LocalDate.now().plusDays(7)
来源：http://mj.9csxet.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ne.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://dc.lnxyls.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hi.bookmarksfly.cn

[J06] 计算两时间之差
来源：http://qs.shxzskj.cn

Py:   (end - start).total_seconds()
来源：http://sy.9csxet.cn

PHP:  $end->diff($start)->days;
来源：http://dq.bjjhwx.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vk.asd995.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xf.huixinmuqiang.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lk.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://ub.hnjuh.cn

Ruby: end - start                 # 返回秒数
来源：http://zp.yuexingan06.cn

C#:   (end - start).TotalSeconds
来源：http://tg.shtwfgs.cn

[J07] 比较两个日期
来源：http://zs.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://qf.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jy.szsharing.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nk.lnxyls.cn

TS:   d1.getTime() < d2.getTime()
来源：http://zv.szxytkj.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fw.newstarts.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mi.shxzukj.cn

Ruby: d1 < d2;  d1 == d2
来源：http://zl.9csxet.cn

C#:   d1 < d2;  d1 == d2
来源：http://fm.9csxet.cn

[J08] 提取年月日与星期
来源：http://vo.yuexingan06.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vz.nicolike.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://at.yuexingan06.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://fl.szxytkj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jg.haigaiapp.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://lm.huixinmuqiang.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rw.huanxung.cn


<!-- 参考信息 -->