代发 wailian999

C#:   public / protected / private / internal
来源：http://eh.shtwfgs.cn

[G11] getter / setter
来源：http://nf.shxzskj.cn

Py:   @property 与 @x.setter
来源：http://wf.huixiangedu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://uq.szsharing.cn

JS:   get name() { return this._name; }
来源：http://de.haigaiapp.cn

TS:   get name(): string { return this._name; }
来源：http://rf.huixiangedu.cn

Java: public String getName() { return name; }
来源：http://zk.nicolike.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://dn.shxzskj.cn

Ruby: attr_accessor :name
来源：http://vs.asd995.cn

C#:   public string Name { get; set; }
来源：http://in.gzmigu.cn

[G12] 对象转字符串
来源：http://ev.gzmigu.cn

Py:   def __str__(self): return self.name
来源：http://ts.panjiajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rd.hnjuh.cn

JS:   toString() { return this.name; }
来源：http://br.panjiajie.cn

TS:   toString(): string { return this.name; }
来源：http://dj.asd995.cn

Java: @Override public String toString() { return name; }
来源：http://bq.lnxyls.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hy.521024.cn

Ruby: def to_s; @name; end
来源：http://zz.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://wl.lnxyls.cn

[G13] 判断对象类型
来源：http://ba.asd995.cn

Py:   isinstance(u, User)
来源：http://ly.bookmarksfly.cn

PHP:  $u instanceof User
来源：http://gx.nszjky.cn

JS:   u instanceof User
来源：http://xp.shxzukj.cn

TS:   u instanceof User
来源：http://bx.gzmigu.cn

Java: u instanceof User
来源：http://jk.shtwfgs.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://aw.bjjhwx.cn

Ruby: u.is_a?(User)
来源：http://hf.jianghongdianzi.cn

C#:   u is User
来源：http://ve.bjjhwx.cn

[G14] 数据类 / record
来源：http://yl.yuntaijiaju.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nj.huixiangedu.cn

PHP:  // 用 readonly 属性模拟
来源：http://fq.colortex.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mk.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://jg.9csxet.cn

Java: record User(String name, int age) {}
来源：http://yz.haigaiapp.cn

Go:   type User struct { Name string; Age int }
来源：http://wh.szsharing.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xc.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://ky.9csxet.cn

[G15] 枚举
来源：http://nr.nicolike.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qr.yuntaijiaju.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xs.colortex.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ae.hnjuh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://uk.bjjhwx.cn

Java: enum Color { RED, GREEN }
来源：http://mq.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lg.jctech888.com.cn

Ruby: Color = %i[red green].freeze
来源：http://hf.shxzskj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://lw.nicolike.cn

[G16] 对象转数组 / 字典
来源：http://qd.lnxyls.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vp.huanxung.cn

PHP:  get_object_vars($obj);
来源：http://mx.huixinmuqiang.cn

JS:   Object.entries(obj)
来源：http://pn.huanxung.cn

TS:   Object.entries(obj)
来源：http://yr.bjjhwx.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nv.jianghongdianzi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://nt.colortex.cn

Ruby: obj.instance_variables
来源：http://vl.yuexingan06.cn

C#:   // 用反射或 System.Text.Json
来源：http://qk.shxzskj.cn

================================================================================
来源：http://od.nicolike.cn

H. 异常与错误处理
来源：http://ai.colortex.cn

================================================================================
来源：http://to.shxzukj.cn

[H01] try / catch 基础
来源：http://ka.szxytkj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wn.nicolike.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mw.nszjky.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://do.yuntaijiaju.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xk.szsharing.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bi.haigaiapp.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://qc.jctech888.com.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://at.haigaiapp.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ok.szxytkj.cn

[H02] finally / ensure 收尾
来源：http://fa.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ev.newstarts.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://uz.9csxet.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xv.wgjwhj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zk.bookmarksfly.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vi.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bt.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://lz.wgjwhj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://km.huixinmuqiang.cn

[H03] 主动抛出异常
来源：http://qc.wgjwhj.cn

Py:   raise ValueError("错误信息")
来源：http://cg.nszjky.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://lr.nszjky.cn

JS:   throw new Error("错误信息");
来源：http://gu.chemitech.net.cn

TS:   throw new Error("错误信息");
来源：http://xy.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://sc.jctech888.com.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://in.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ei.newstarts.cn

C#:   throw new ArgumentException("错误信息");
来源：http://tr.shtwfgs.cn

[H04] 自定义异常类型
来源：http://jq.hahajie.cn

Py:   class MyError(Exception): pass
来源：http://uk.bookmarksfly.cn

PHP:  class MyError extends RuntimeException {}
来源：http://xq.jctech888.com.cn

JS:   class MyError extends Error {}
来源：http://ke.nicolike.cn

TS:   class MyError extends Error {}
来源：http://vc.colortex.cn

Java: class MyException extends RuntimeException {}
来源：http://zc.huixiangedu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://rv.jctech888.com.cn

Ruby: class MyError < StandardError; end
来源：http://jy.gzmigu.cn

C#:   class MyException : Exception {}
来源：http://zu.huixiangedu.cn

[H05] 捕获特定类型
来源：http://hl.hahajie.cn

Py:   except ValueError as e:
来源：http://nz.9csxet.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pg.huanxung.cn

JS:   if (e instanceof TypeError) {}
来源：http://nz.hahajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://st.jctech888.com.cn

Java: catch (IOException | SQLException e) {}
来源：http://dh.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://nc.colortex.cn

Ruby: rescue ArgumentError => e
来源：http://mg.chemitech.net.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://dg.hnjuh.cn

[H06] 可选值 / 空值安全访问
来源：http://hf.gzmigu.cn

Py:   value = d.get("k") or default
来源：http://fh.lnxyls.cn

PHP:  $v = $d["k"] ?? null;
来源：http://mx.shxzukj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ai.hnjuh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vi.jctech888.com.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mt.9csxet.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://tf.chemitech.net.cn

Ruby: d&.dig(:a, :b)
来源：http://ob.shtwfgs.cn

C#:   obj?.A?.B ?? default
来源：http://gl.bjjhwx.cn

[H07] 断言
来源：http://us.nszjky.cn

Py:   assert x > 0, "必须为正"
来源：http://xd.panjiajie.cn

PHP:  assert($x > 0);
来源：http://nd.nszjky.cn

JS:   console.assert(x > 0);
来源：http://nu.haigaiapp.cn

TS:   console.assert(x > 0);
来源：http://lk.jianghongdianzi.cn

Java: assert x > 0 : "必须为正";
来源：http://yv.lnxyls.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://lz.9csxet.cn

Ruby: raise "必须为正" unless x > 0
来源：http://nc.lnxyls.cn

C#:   Debug.Assert(x > 0);
来源：http://oq.yuexingan06.cn

[H08] 获取错误信息与堆栈
来源：http://rm.haigaiapp.cn

Py:   str(e);  traceback.format_exc()
来源：http://jy.9csxet.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ip.hahajie.cn

JS:   e.message;  e.stack
来源：http://az.bjjhwx.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://lh.lnxyls.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cd.szxytkj.cn

Go:   err.Error()
来源：http://yi.szsharing.cn

Ruby: e.message;  e.backtrace
来源：http://vx.colortex.cn

C#:   e.Message;  e.StackTrace
来源：http://qp.szxytkj.cn

[H09] 带错误码的异常
来源：http://ey.9csxet.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sk.hnjuh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://my.szxytkj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pa.shxzskj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mn.huixiangedu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://yu.hnjuh.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://jg.szxytkj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://hp.shxzskj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ir.colortex.cn

[H10] 资源自动释放
来源：http://gw.9csxet.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://me.nszjky.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wt.hahajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://nj.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yz.lnxyls.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://pk.chemitech.net.cn

Go:   defer f.Close()
来源：http://mt.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fn.nicolike.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://zp.newstarts.cn

================================================================================
来源：http://en.huanxung.cn

I. 正则表达式
来源：http://lu.gzmigu.cn

================================================================================
来源：http://lg.9csxet.cn

[I01] 判断是否匹配
来源：http://pc.nicolike.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fo.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ne.muxihuayi.cn

JS:   /\d+/.test(s)
来源：http://oo.newstarts.cn

TS:   /\d+/.test(s)
来源：http://lt.lnxyls.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://il.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://jk.bookmarksfly.cn

Ruby: s.match?(/\d+/)
来源：http://fq.lnxyls.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wj.szsharing.cn

[I02] 提取所有匹配
来源：http://hx.nszjky.cn

Py:   re.findall(r"\d+", s)
来源：http://mk.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vb.jctech888.com.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mh.newstarts.cn

TS:   s.match(/\d+/g)
来源：http://de.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mh.nszjky.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://fi.asd995.cn

Ruby: s.scan(/\d+/)
来源：http://zi.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ce.jianghongdianzi.cn

[I03] 提取捕获分组
来源：http://kk.huixinmuqiang.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zy.jctech888.com.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ho.lnxyls.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://tp.jctech888.com.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://bh.nicolike.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sf.lnxyls.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://xf.bookmarksfly.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nk.bjjhwx.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fs.huixiangedu.cn

[I04] 正则替换
来源：http://xw.asd995.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://he.lnxyls.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xu.panjiajie.cn

JS:   s.replace(/\d+/g, "#")
来源：http://cs.nszjky.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sx.chemitech.net.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jp.muxihuayi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oy.panjiajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://go.panjiajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://ww.hahajie.cn

[I05] 按正则拆分
来源：http://px.asd995.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ii.chemitech.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ox.shxzskj.cn

JS:   s.split(/\s*,\s*/)
来源：http://rp.nszjky.cn

TS:   s.split(/\s*,\s*/)
来源：http://an.newstarts.cn

Java: s.split("\\s*,\\s*")
来源：http://ks.gzmigu.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://jb.wgjwhj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ll.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wb.panjiajie.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://kh.hahajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fk.yuntaijiaju.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://pl.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lz.chemitech.net.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qx.huixinmuqiang.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qq.bookmarksfly.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rb.chemitech.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://zs.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hb.9csxet.cn

[I07] 忽略大小写与多行模式
来源：http://bc.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://qi.yuntaijiaju.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fy.muxihuayi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qf.shxzukj.cn

TS:   /error/gim
来源：http://as.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cj.asd995.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fe.jianghongdianzi.cn

Ruby: s.scan(/error/i)
来源：http://vc.shtwfgs.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://gm.bjjhwx.cn

[I08] 贪婪与非贪婪匹配
来源：http://sh.newstarts.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://eq.colortex.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://pz.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://tw.newstarts.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jw.hahajie.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://vl.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kv.bookmarksfly.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://yb.lnxyls.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cm.asd995.cn

================================================================================
来源：http://rf.shxzskj.cn

J. 日期与时间
来源：http://eg.szxytkj.cn

================================================================================
来源：http://st.shxzskj.cn

[J01] 获取当前时间
来源：http://hm.szxytkj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://be.huixiangedu.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://fa.szxytkj.cn

JS:   new Date();  Date.now()
来源：http://bz.bjjhwx.cn

TS:   new Date();  Date.now()
来源：http://dp.jianghongdianzi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vi.szsharing.cn

Go:   time.Now()
来源：http://tr.panjiajie.cn

Ruby: Time.now
来源：http://tm.lnxyls.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://zg.huixinmuqiang.cn

[J02] 格式化输出
来源：http://lt.huanxung.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://pc.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://zs.bjjhwx.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sj.jctech888.com.cn

TS:   d.toISOString()
来源：http://zt.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jj.lnxyls.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://my.newstarts.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sl.haigaiapp.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://vg.haigaiapp.cn

[J03] 字符串解析为日期
来源：http://lk.huixiangedu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ut.szsharing.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://oi.lnxyls.cn

JS:   new Date("2024-01-02")
来源：http://xh.gzmigu.cn

TS:   new Date("2024-01-02")
来源：http://yp.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ui.shtwfgs.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://tk.newstarts.cn

Ruby: Date.parse("2024-01-02")
来源：http://ge.huixinmuqiang.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://rp.shxzskj.cn

[J04] 时间戳与日期互转
来源：http://xv.9csxet.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ld.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://xp.lnxyls.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://me.bookmarksfly.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xu.chemitech.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ie.shtwfgs.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ck.huixiangedu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qg.gzmigu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://jg.lnxyls.cn

[J05] 时间加减（加 7 天）
来源：http://jk.szxytkj.cn

Py:   now + timedelta(days=7)
来源：http://yg.colortex.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xx.shxzskj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ks.huixiangedu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://rx.bookmarksfly.cn

Java: LocalDate.now().plusDays(7)
来源：http://on.szxytkj.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://vz.9csxet.cn

Ruby: Time.now + 7 * 86400
来源：http://iv.nicolike.cn

C#:   DateTime.Now.AddDays(7)
来源：http://dm.jianghongdianzi.cn

[J06] 计算两时间之差
来源：http://xr.nszjky.cn

Py:   (end - start).total_seconds()
来源：http://cr.shxzskj.cn

PHP:  $end->diff($start)->days;
来源：http://bj.szsharing.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jq.muxihuayi.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ho.yuntaijiaju.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qo.gzmigu.cn

Go:   end.Sub(start).Hours()
来源：http://ed.nicolike.cn

Ruby: end - start                 # 返回秒数
来源：http://wq.yuntaijiaju.cn

C#:   (end - start).TotalSeconds
来源：http://sg.huixinmuqiang.cn

[J07] 比较两个日期
来源：http://wk.yuexingan06.cn

Py:   d1 < d2;  d1 == d2
来源：http://yg.colortex.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://na.yuexingan06.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vc.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://xg.hnjuh.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xq.shtwfgs.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wz.haigaiapp.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ou.shxzukj.cn

C#:   d1 < d2;  d1 == d2
来源：http://wo.jctech888.com.cn

[J08] 提取年月日与星期
来源：http://xt.nszjky.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lz.hnjuh.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://kc.haigaiapp.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kg.szxytkj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://sk.nszjky.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sa.szxytkj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gn.shxzukj.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yo.9csxet.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://lw.panjiajie.cn

[J09] 时区处理
来源：http://xb.hahajie.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uz.lnxyls.cn


<!-- 参考信息 -->