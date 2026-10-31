代发 wailian999

C#:   public / protected / private / internal
来源：http://tn.wgjwhj.cn

[G11] getter / setter
来源：http://cb.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://zm.szxytkj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ux.nicolike.cn

JS:   get name() { return this._name; }
来源：http://cs.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://zr.shtwfgs.cn

Java: public String getName() { return name; }
来源：http://zx.huanxung.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gl.colortex.cn

Ruby: attr_accessor :name
来源：http://iz.lnxyls.cn

C#:   public string Name { get; set; }
来源：http://ih.521024.cn

[G12] 对象转字符串
来源：http://ym.521024.cn

Py:   def __str__(self): return self.name
来源：http://tk.nicolike.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://da.521024.cn

JS:   toString() { return this.name; }
来源：http://nk.chemitech.net.cn

TS:   toString(): string { return this.name; }
来源：http://ef.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://qh.asd995.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jy.newstarts.cn

Ruby: def to_s; @name; end
来源：http://sq.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://kb.lnxyls.cn

[G13] 判断对象类型
来源：http://tw.huanxung.cn

Py:   isinstance(u, User)
来源：http://yh.panjiajie.cn

PHP:  $u instanceof User
来源：http://aq.haigaiapp.cn

JS:   u instanceof User
来源：http://ht.chemitech.net.cn

TS:   u instanceof User
来源：http://fi.colortex.cn

Java: u instanceof User
来源：http://ng.hahajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://zu.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://cl.bookmarksfly.cn

C#:   u is User
来源：http://ur.szxytkj.cn

[G14] 数据类 / record
来源：http://ky.jctech888.com.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://np.hnjuh.cn

PHP:  // 用 readonly 属性模拟
来源：http://kk.hnjuh.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qc.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://kw.521024.cn

Java: record User(String name, int age) {}
来源：http://oh.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://mo.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yq.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://px.huanxung.cn

[G15] 枚举
来源：http://od.gzmigu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://os.huanxung.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fh.szxytkj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gk.9csxet.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lp.yuntaijiaju.cn

Java: enum Color { RED, GREEN }
来源：http://md.lnxyls.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://pe.huixinmuqiang.cn

Ruby: Color = %i[red green].freeze
来源：http://im.bookmarksfly.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://om.asd995.cn

[G16] 对象转数组 / 字典
来源：http://gw.jctech888.com.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zv.shxzskj.cn

PHP:  get_object_vars($obj);
来源：http://lb.muxihuayi.cn

JS:   Object.entries(obj)
来源：http://tc.muxihuayi.cn

TS:   Object.entries(obj)
来源：http://bz.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://eh.huanxung.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://el.nszjky.cn

Ruby: obj.instance_variables
来源：http://sz.newstarts.cn

C#:   // 用反射或 System.Text.Json
来源：http://da.9csxet.cn

================================================================================
来源：http://yc.bjjhwx.cn

H. 异常与错误处理
来源：http://gw.huixinmuqiang.cn

================================================================================
来源：http://rj.shtwfgs.cn

[H01] try / catch 基础
来源：http://ui.bookmarksfly.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gr.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wn.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://qc.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zq.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lc.jianghongdianzi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vp.521024.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://tz.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://uz.shxzskj.cn

[H02] finally / ensure 收尾
来源：http://ds.muxihuayi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rb.szsharing.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jj.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://vp.szxytkj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://cz.yuntaijiaju.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pj.huanxung.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://lc.bookmarksfly.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://do.huanxung.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://as.shtwfgs.cn

[H03] 主动抛出异常
来源：http://dp.asd995.cn

Py:   raise ValueError("错误信息")
来源：http://ax.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kf.asd995.cn

JS:   throw new Error("错误信息");
来源：http://kb.nszjky.cn

TS:   throw new Error("错误信息");
来源：http://pq.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ef.shxzskj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gf.hnjuh.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://hg.wgjwhj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://vs.panjiajie.cn

[H04] 自定义异常类型
来源：http://ak.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://ks.huixinmuqiang.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lt.9csxet.cn

JS:   class MyError extends Error {}
来源：http://hz.colortex.cn

TS:   class MyError extends Error {}
来源：http://vn.wgjwhj.cn

Java: class MyException extends RuntimeException {}
来源：http://fh.yuntaijiaju.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://kb.hahajie.cn

Ruby: class MyError < StandardError; end
来源：http://hy.muxihuayi.cn

C#:   class MyException : Exception {}
来源：http://up.chemitech.net.cn

[H05] 捕获特定类型
来源：http://os.jctech888.com.cn

Py:   except ValueError as e:
来源：http://te.chemitech.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rz.bookmarksfly.cn

JS:   if (e instanceof TypeError) {}
来源：http://md.shtwfgs.cn

TS:   if (e instanceof TypeError) {}
来源：http://va.521024.cn

Java: catch (IOException | SQLException e) {}
来源：http://hn.bjjhwx.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://uw.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://rw.yuntaijiaju.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wc.haigaiapp.cn

[H06] 可选值 / 空值安全访问
来源：http://jb.panjiajie.cn

Py:   value = d.get("k") or default
来源：http://li.muxihuayi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hl.szxytkj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bb.nicolike.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qd.gzmigu.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://pq.hahajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zz.9csxet.cn

Ruby: d&.dig(:a, :b)
来源：http://ac.jctech888.com.cn

C#:   obj?.A?.B ?? default
来源：http://xv.gzmigu.cn

[H07] 断言
来源：http://vy.jianghongdianzi.cn

Py:   assert x > 0, "必须为正"
来源：http://lr.huanxung.cn

PHP:  assert($x > 0);
来源：http://rg.hahajie.cn

JS:   console.assert(x > 0);
来源：http://hn.bookmarksfly.cn

TS:   console.assert(x > 0);
来源：http://lu.shxzskj.cn

Java: assert x > 0 : "必须为正";
来源：http://rc.shxzukj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pa.huixinmuqiang.cn

Ruby: raise "必须为正" unless x > 0
来源：http://ai.panjiajie.cn

C#:   Debug.Assert(x > 0);
来源：http://ic.yuexingan06.cn

[H08] 获取错误信息与堆栈
来源：http://pg.shxzskj.cn

Py:   str(e);  traceback.format_exc()
来源：http://bi.shxzukj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://tj.shxzukj.cn

JS:   e.message;  e.stack
来源：http://zi.asd995.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hm.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ja.huixinmuqiang.cn

Go:   err.Error()
来源：http://tk.gzmigu.cn

Ruby: e.message;  e.backtrace
来源：http://sx.jianghongdianzi.cn

C#:   e.Message;  e.StackTrace
来源：http://qv.szsharing.cn

[H09] 带错误码的异常
来源：http://zd.szsharing.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ho.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://um.bjjhwx.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://qa.huanxung.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zr.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://cs.521024.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://qr.colortex.cn

Ruby: raise MyError.new("fail", 500)
来源：http://dd.hnjuh.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ob.hnjuh.cn

[H10] 资源自动释放
来源：http://nd.haigaiapp.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mo.nicolike.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yl.panjiajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://lo.lnxyls.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mo.huanxung.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hy.lnxyls.cn

Go:   defer f.Close()
来源：http://df.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://fv.jianghongdianzi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mk.panjiajie.cn

================================================================================
来源：http://vt.nszjky.cn

I. 正则表达式
来源：http://jy.gzmigu.cn

================================================================================
来源：http://qe.lnxyls.cn

[I01] 判断是否匹配
来源：http://hw.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://qu.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://hi.9csxet.cn

JS:   /\d+/.test(s)
来源：http://bb.9csxet.cn

TS:   /\d+/.test(s)
来源：http://nj.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hw.newstarts.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ch.szxytkj.cn

Ruby: s.match?(/\d+/)
来源：http://fz.asd995.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ev.nszjky.cn

[I02] 提取所有匹配
来源：http://ei.huanxung.cn

Py:   re.findall(r"\d+", s)
来源：http://on.9csxet.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ty.jianghongdianzi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://be.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://fh.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hq.gzmigu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hw.gzmigu.cn

Ruby: s.scan(/\d+/)
来源：http://cc.521024.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sy.shtwfgs.cn

[I03] 提取捕获分组
来源：http://mo.szxytkj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ka.panjiajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yk.szsharing.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wq.jianghongdianzi.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://gb.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ks.chemitech.net.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mi.huixiangedu.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fz.newstarts.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://fz.shxzukj.cn

[I04] 正则替换
来源：http://op.jianghongdianzi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jb.yuexingan06.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://do.nszjky.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zb.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hv.shtwfgs.cn

Java: s.replaceAll("\\d+", "#")
来源：http://dk.panjiajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ws.panjiajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://vv.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://zp.shxzukj.cn

[I05] 按正则拆分
来源：http://il.panjiajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://pc.jctech888.com.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://ct.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://jq.szxytkj.cn

TS:   s.split(/\s*,\s*/)
来源：http://wa.jianghongdianzi.cn

Java: s.split("\\s*,\\s*")
来源：http://rz.hahajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fx.bookmarksfly.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wu.jctech888.com.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://tt.9csxet.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ux.szxytkj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dg.szsharing.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://xc.9csxet.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wd.gzmigu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://lj.lnxyls.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://rq.shxzukj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://te.bjjhwx.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hd.colortex.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://tg.gzmigu.cn

[I07] 忽略大小写与多行模式
来源：http://xg.wgjwhj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://tu.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jc.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://qs.hnjuh.cn

TS:   /error/gim
来源：http://nd.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jq.haigaiapp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ok.521024.cn

Ruby: s.scan(/error/i)
来源：http://da.muxihuayi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://df.bookmarksfly.cn

[I08] 贪婪与非贪婪匹配
来源：http://ql.newstarts.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://bk.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yz.521024.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://bg.521024.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://zf.jianghongdianzi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://dp.yuexingan06.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://af.bookmarksfly.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://av.shxzukj.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gj.muxihuayi.cn

================================================================================
来源：http://md.nszjky.cn

J. 日期与时间
来源：http://yb.jianghongdianzi.cn

================================================================================
来源：http://gn.bjjhwx.cn

[J01] 获取当前时间
来源：http://rp.huanxung.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://rt.shtwfgs.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://pu.panjiajie.cn

JS:   new Date();  Date.now()
来源：http://ve.huixinmuqiang.cn

TS:   new Date();  Date.now()
来源：http://lt.yuntaijiaju.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fw.hnjuh.cn

Go:   time.Now()
来源：http://rx.lnxyls.cn

Ruby: Time.now
来源：http://wa.haigaiapp.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ut.521024.cn

[J02] 格式化输出
来源：http://da.lnxyls.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://en.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pm.521024.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hm.panjiajie.cn

TS:   d.toISOString()
来源：http://mj.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://mp.huanxung.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mz.panjiajie.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://fd.bjjhwx.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://iy.hahajie.cn

[J03] 字符串解析为日期
来源：http://ow.huanxung.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://df.nszjky.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mt.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://ml.wgjwhj.cn

TS:   new Date("2024-01-02")
来源：http://xc.huixiangedu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://na.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://lp.colortex.cn

Ruby: Date.parse("2024-01-02")
来源：http://ay.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://dy.asd995.cn

[J04] 时间戳与日期互转
来源：http://ay.chemitech.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://zf.huixiangedu.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://to.huixiangedu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ya.nicolike.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://zn.521024.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sz.jctech888.com.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gq.shxzukj.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://fa.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://uo.huixinmuqiang.cn

[J05] 时间加减（加 7 天）
来源：http://ev.shtwfgs.cn

Py:   now + timedelta(days=7)
来源：http://gt.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kv.asd995.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://pi.colortex.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://jd.bjjhwx.cn

Java: LocalDate.now().plusDays(7)
来源：http://ue.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xq.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://kv.521024.cn

C#:   DateTime.Now.AddDays(7)
来源：http://yw.hnjuh.cn

[J06] 计算两时间之差
来源：http://ej.lnxyls.cn

Py:   (end - start).total_seconds()
来源：http://wb.yuntaijiaju.cn

PHP:  $end->diff($start)->days;
来源：http://yb.huixiangedu.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://tm.nszjky.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wn.yuntaijiaju.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jb.colortex.cn

Go:   end.Sub(start).Hours()
来源：http://tm.9csxet.cn

Ruby: end - start                 # 返回秒数
来源：http://vc.chemitech.net.cn

C#:   (end - start).TotalSeconds
来源：http://en.yuntaijiaju.cn

[J07] 比较两个日期
来源：http://de.haigaiapp.cn

Py:   d1 < d2;  d1 == d2
来源：http://cl.9csxet.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dc.asd995.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vd.szxytkj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://af.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qx.shxzskj.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vk.huixinmuqiang.cn

Ruby: d1 < d2;  d1 == d2
来源：http://at.huixiangedu.cn

C#:   d1 < d2;  d1 == d2
来源：http://wi.521024.cn

[J08] 提取年月日与星期
来源：http://jc.muxihuayi.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://tx.9csxet.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gn.huanxung.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://av.szxytkj.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nh.shxzukj.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://uw.wgjwhj.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://yh.9csxet.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fz.panjiajie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mt.muxihuayi.cn

[J09] 时区处理
来源：http://zv.haigaiapp.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ir.bjjhwx.cn


<!-- 参考信息 -->