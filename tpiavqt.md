代发 wailian999

TS:   public / protected / private
来源：http://cl.bookmarksfly.cn

Java: public / protected / private / 默认包级
来源：http://ul.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rs.bjjhwx.cn

Ruby: public / protected / private
来源：http://if.521024.cn

C#:   public / protected / private / internal
来源：http://cn.szsharing.cn

[G11] getter / setter
来源：http://ln.szsharing.cn

Py:   @property 与 @x.setter
来源：http://gi.colortex.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yz.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://bs.jctech888.com.cn

TS:   get name(): string { return this._name; }
来源：http://yz.asd995.cn

Java: public String getName() { return name; }
来源：http://fm.huixinmuqiang.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bq.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://cf.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://bp.hahajie.cn

[G12] 对象转字符串
来源：http://fp.bjjhwx.cn

Py:   def __str__(self): return self.name
来源：http://cw.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vd.huanxung.cn

JS:   toString() { return this.name; }
来源：http://vo.bookmarksfly.cn

TS:   toString(): string { return this.name; }
来源：http://uf.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://gm.lnxyls.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ra.huanxung.cn

Ruby: def to_s; @name; end
来源：http://cc.gzmigu.cn

C#:   public override string ToString() => Name;
来源：http://mz.shtwfgs.cn

[G13] 判断对象类型
来源：http://rf.chemitech.net.cn

Py:   isinstance(u, User)
来源：http://mb.newstarts.cn

PHP:  $u instanceof User
来源：http://ti.gzmigu.cn

JS:   u instanceof User
来源：http://ab.panjiajie.cn

TS:   u instanceof User
来源：http://ft.wgjwhj.cn

Java: u instanceof User
来源：http://lb.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ih.huanxung.cn

Ruby: u.is_a?(User)
来源：http://st.szxytkj.cn

C#:   u is User
来源：http://do.huixinmuqiang.cn

[G14] 数据类 / record
来源：http://fl.lnxyls.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kx.newstarts.cn

PHP:  // 用 readonly 属性模拟
来源：http://qo.bookmarksfly.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ye.shtwfgs.cn

TS:   type User = { name: string; age: number };
来源：http://qe.gzmigu.cn

Java: record User(String name, int age) {}
来源：http://vk.yuexingan06.cn

Go:   type User struct { Name string; Age int }
来源：http://uy.9csxet.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uq.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://kn.lnxyls.cn

[G15] 枚举
来源：http://sp.shxzskj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dm.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ho.panjiajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wp.jctech888.com.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://nx.gzmigu.cn

Java: enum Color { RED, GREEN }
来源：http://gq.nszjky.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vy.chemitech.net.cn

Ruby: Color = %i[red green].freeze
来源：http://mm.newstarts.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hj.nicolike.cn

[G16] 对象转数组 / 字典
来源：http://ah.huixinmuqiang.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://la.lnxyls.cn

PHP:  get_object_vars($obj);
来源：http://df.gzmigu.cn

JS:   Object.entries(obj)
来源：http://mq.bjjhwx.cn

TS:   Object.entries(obj)
来源：http://pn.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://th.szsharing.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ui.haigaiapp.cn

Ruby: obj.instance_variables
来源：http://xq.huixiangedu.cn

C#:   // 用反射或 System.Text.Json
来源：http://ge.szsharing.cn

================================================================================
来源：http://wc.hahajie.cn

H. 异常与错误处理
来源：http://as.yuexingan06.cn

================================================================================
来源：http://ck.shxzskj.cn

[H01] try / catch 基础
来源：http://zd.521024.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jz.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://db.shxzskj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ei.colortex.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://za.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hd.wgjwhj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://od.yuexingan06.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hs.szsharing.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gq.nicolike.cn

[H02] finally / ensure 收尾
来源：http://yq.hahajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pd.chemitech.net.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://iy.asd995.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://bo.huanxung.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xt.chemitech.net.cn

Java: try { f(); } finally { cleanup(); }
来源：http://qy.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mj.hnjuh.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://mp.colortex.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pu.nszjky.cn

[H03] 主动抛出异常
来源：http://bo.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://jm.huixinmuqiang.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ry.yuexingan06.cn

JS:   throw new Error("错误信息");
来源：http://gk.wgjwhj.cn

TS:   throw new Error("错误信息");
来源：http://cj.szsharing.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ve.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fx.szsharing.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bk.shxzskj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fj.wgjwhj.cn

[H04] 自定义异常类型
来源：http://fs.newstarts.cn

Py:   class MyError(Exception): pass
来源：http://xh.colortex.cn

PHP:  class MyError extends RuntimeException {}
来源：http://nf.gzmigu.cn

JS:   class MyError extends Error {}
来源：http://sd.bookmarksfly.cn

TS:   class MyError extends Error {}
来源：http://dq.bjjhwx.cn

Java: class MyException extends RuntimeException {}
来源：http://ud.gzmigu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mp.huixinmuqiang.cn

Ruby: class MyError < StandardError; end
来源：http://fz.newstarts.cn

C#:   class MyException : Exception {}
来源：http://vu.szxytkj.cn

[H05] 捕获特定类型
来源：http://yp.huixiangedu.cn

Py:   except ValueError as e:
来源：http://uc.shtwfgs.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gn.yuexingan06.cn

JS:   if (e instanceof TypeError) {}
来源：http://bd.yuntaijiaju.cn

TS:   if (e instanceof TypeError) {}
来源：http://cq.shtwfgs.cn

Java: catch (IOException | SQLException e) {}
来源：http://ez.shxzskj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ql.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://eq.muxihuayi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ms.huixiangedu.cn

[H06] 可选值 / 空值安全访问
来源：http://fl.huixiangedu.cn

Py:   value = d.get("k") or default
来源：http://wb.nicolike.cn

PHP:  $v = $d["k"] ?? null;
来源：http://xl.haigaiapp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ii.huixiangedu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mz.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ee.yuexingan06.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://yu.shxzskj.cn

Ruby: d&.dig(:a, :b)
来源：http://wo.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://dn.shxzukj.cn

[H07] 断言
来源：http://nq.nszjky.cn

Py:   assert x > 0, "必须为正"
来源：http://gs.huixinmuqiang.cn

PHP:  assert($x > 0);
来源：http://eb.szxytkj.cn

JS:   console.assert(x > 0);
来源：http://jp.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://qd.shxzukj.cn

Java: assert x > 0 : "必须为正";
来源：http://ws.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jb.gzmigu.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rb.jianghongdianzi.cn

C#:   Debug.Assert(x > 0);
来源：http://os.jctech888.com.cn

[H08] 获取错误信息与堆栈
来源：http://bg.nszjky.cn

Py:   str(e);  traceback.format_exc()
来源：http://ej.bookmarksfly.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ug.muxihuayi.cn

JS:   e.message;  e.stack
来源：http://xy.huixinmuqiang.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://dv.hahajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zt.wgjwhj.cn

Go:   err.Error()
来源：http://oh.haigaiapp.cn

Ruby: e.message;  e.backtrace
来源：http://wc.haigaiapp.cn

C#:   e.Message;  e.StackTrace
来源：http://st.chemitech.net.cn

[H09] 带错误码的异常
来源：http://cg.muxihuayi.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://zk.asd995.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wt.521024.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://si.colortex.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://rh.asd995.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yb.hahajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://tf.bjjhwx.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ux.panjiajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://et.szxytkj.cn

[H10] 资源自动释放
来源：http://nw.colortex.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pf.asd995.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://jv.huixinmuqiang.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://he.shtwfgs.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ow.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yi.asd995.cn

Go:   defer f.Close()
来源：http://kl.hnjuh.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kr.szsharing.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xy.lnxyls.cn

================================================================================
来源：http://pr.chemitech.net.cn

I. 正则表达式
来源：http://wx.bookmarksfly.cn

================================================================================
来源：http://rw.szsharing.cn

[I01] 判断是否匹配
来源：http://rj.chemitech.net.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vh.9csxet.cn

PHP:  preg_match('/\d+/', $s);
来源：http://gk.panjiajie.cn

JS:   /\d+/.test(s)
来源：http://sw.newstarts.cn

TS:   /\d+/.test(s)
来源：http://ui.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fv.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ho.jctech888.com.cn

Ruby: s.match?(/\d+/)
来源：http://af.shxzukj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bt.asd995.cn

[I02] 提取所有匹配
来源：http://lq.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://af.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://lo.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://se.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://pc.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zx.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wl.hahajie.cn

Ruby: s.scan(/\d+/)
来源：http://ti.bookmarksfly.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://aj.asd995.cn

[I03] 提取捕获分组
来源：http://tf.nicolike.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://fy.haigaiapp.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ef.chemitech.net.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cg.nicolike.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://of.9csxet.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://gh.hnjuh.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ux.chemitech.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jn.yuntaijiaju.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jl.gzmigu.cn

[I04] 正则替换
来源：http://pg.huixinmuqiang.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jz.colortex.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://kw.szxytkj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pa.shtwfgs.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ah.chemitech.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cn.nszjky.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ul.huanxung.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ms.bjjhwx.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ge.shtwfgs.cn

[I05] 按正则拆分
来源：http://do.yuexingan06.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xf.colortex.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ze.huanxung.cn

JS:   s.split(/\s*,\s*/)
来源：http://qm.colortex.cn

TS:   s.split(/\s*,\s*/)
来源：http://va.yuntaijiaju.cn

Java: s.split("\\s*,\\s*")
来源：http://bl.szxytkj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://xa.nicolike.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dx.bjjhwx.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://xi.asd995.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://dw.asd995.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bg.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://fg.shtwfgs.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bm.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wk.9csxet.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://eu.gzmigu.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://pg.jctech888.com.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lz.hnjuh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://yf.bjjhwx.cn

[I07] 忽略大小写与多行模式
来源：http://zr.huixiangedu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://is.yuntaijiaju.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://xy.hahajie.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://yj.hnjuh.cn

TS:   /error/gim
来源：http://ht.521024.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://ah.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://he.521024.cn

Ruby: s.scan(/error/i)
来源：http://xs.bookmarksfly.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://tw.gzmigu.cn

[I08] 贪婪与非贪婪匹配
来源：http://qr.bjjhwx.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lx.panjiajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://kd.muxihuayi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://xi.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zd.newstarts.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://td.wgjwhj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://gs.521024.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://qj.lnxyls.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ny.bookmarksfly.cn

================================================================================
来源：http://ty.panjiajie.cn

J. 日期与时间
来源：http://xx.jctech888.com.cn

================================================================================
来源：http://ew.haigaiapp.cn

[J01] 获取当前时间
来源：http://yl.521024.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://tb.9csxet.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://dz.lnxyls.cn

JS:   new Date();  Date.now()
来源：http://qi.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://mo.huanxung.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://gg.nszjky.cn

Go:   time.Now()
来源：http://je.hnjuh.cn

Ruby: Time.now
来源：http://fo.asd995.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://pl.shxzukj.cn

[J02] 格式化输出
来源：http://xu.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://db.panjiajie.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xx.nicolike.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ud.shtwfgs.cn

TS:   d.toISOString()
来源：http://am.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://uj.yuntaijiaju.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://zb.bjjhwx.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sn.jctech888.com.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fv.huixinmuqiang.cn

[J03] 字符串解析为日期
来源：http://px.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://lp.hahajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://os.yuexingan06.cn

JS:   new Date("2024-01-02")
来源：http://oa.yuntaijiaju.cn

TS:   new Date("2024-01-02")
来源：http://hr.panjiajie.cn

Java: LocalDate.parse("2024-01-02")
来源：http://fr.lnxyls.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tj.521024.cn

Ruby: Date.parse("2024-01-02")
来源：http://rm.muxihuayi.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ru.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://ge.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ab.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://en.szsharing.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://tz.colortex.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://nc.colortex.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ru.huixiangedu.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://zo.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://vs.shtwfgs.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://eu.shxzskj.cn

[J05] 时间加减（加 7 天）
来源：http://bp.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://ms.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lu.huixiangedu.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://aa.yuntaijiaju.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://nm.bookmarksfly.cn

Java: LocalDate.now().plusDays(7)
来源：http://wj.newstarts.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zw.lnxyls.cn

Ruby: Time.now + 7 * 86400
来源：http://ze.9csxet.cn

C#:   DateTime.Now.AddDays(7)
来源：http://px.jianghongdianzi.cn

[J06] 计算两时间之差
来源：http://cj.chemitech.net.cn

Py:   (end - start).total_seconds()
来源：http://hg.yuexingan06.cn

PHP:  $end->diff($start)->days;
来源：http://if.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jm.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://sw.szsharing.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rm.yuntaijiaju.cn

Go:   end.Sub(start).Hours()
来源：http://li.jctech888.com.cn

Ruby: end - start                 # 返回秒数
来源：http://qv.huixinmuqiang.cn

C#:   (end - start).TotalSeconds
来源：http://lz.huanxung.cn

[J07] 比较两个日期
来源：http://iz.9csxet.cn

Py:   d1 < d2;  d1 == d2
来源：http://jy.chemitech.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://gc.bjjhwx.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ed.gzmigu.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ro.newstarts.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ct.hnjuh.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jo.lnxyls.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ny.muxihuayi.cn

C#:   d1 < d2;  d1 == d2
来源：http://bi.wgjwhj.cn

[J08] 提取年月日与星期
来源：http://fy.jianghongdianzi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rq.jctech888.com.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rv.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rg.huixinmuqiang.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fi.gzmigu.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://iy.hnjuh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://rj.huixinmuqiang.cn


<!-- 参考信息 -->