代发 wailian999

JS:   get name() { return this._name; }
来源：http://tx.huixinmuqiang.cn

TS:   get name(): string { return this._name; }
来源：http://gi.hnjuh.cn

Java: public String getName() { return name; }
来源：http://rt.hnjuh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://sd.lnxyls.cn

Ruby: attr_accessor :name
来源：http://ct.bookmarksfly.cn

C#:   public string Name { get; set; }
来源：http://bp.bjjhwx.cn

[G12] 对象转字符串
来源：http://vc.yuntaijiaju.cn

Py:   def __str__(self): return self.name
来源：http://to.colortex.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://og.yuntaijiaju.cn

JS:   toString() { return this.name; }
来源：http://fv.muxihuayi.cn

TS:   toString(): string { return this.name; }
来源：http://nf.wgjwhj.cn

Java: @Override public String toString() { return name; }
来源：http://jj.huanxung.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vx.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://xr.newstarts.cn

C#:   public override string ToString() => Name;
来源：http://br.lnxyls.cn

[G13] 判断对象类型
来源：http://pv.nicolike.cn

Py:   isinstance(u, User)
来源：http://rk.9csxet.cn

PHP:  $u instanceof User
来源：http://se.bookmarksfly.cn

JS:   u instanceof User
来源：http://oa.chemitech.net.cn

TS:   u instanceof User
来源：http://wg.521024.cn

Java: u instanceof User
来源：http://cd.huanxung.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ao.shxzskj.cn

Ruby: u.is_a?(User)
来源：http://zw.jctech888.com.cn

C#:   u is User
来源：http://ol.jctech888.com.cn

[G14] 数据类 / record
来源：http://bh.colortex.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wi.haigaiapp.cn

PHP:  // 用 readonly 属性模拟
来源：http://du.bjjhwx.cn

JS:   // 无内置：普通类或对象字面量
来源：http://os.huixiangedu.cn

TS:   type User = { name: string; age: number };
来源：http://hb.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://qe.wgjwhj.cn

Go:   type User struct { Name string; Age int }
来源：http://oa.bjjhwx.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://bk.nszjky.cn

C#:   record User(string Name, int Age);
来源：http://ib.colortex.cn

[G15] 枚举
来源：http://sb.asd995.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bz.bookmarksfly.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xi.lnxyls.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ip.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wx.521024.cn

Java: enum Color { RED, GREEN }
来源：http://ue.jianghongdianzi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rh.yuntaijiaju.cn

Ruby: Color = %i[red green].freeze
来源：http://ti.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://kc.haigaiapp.cn

[G16] 对象转数组 / 字典
来源：http://vk.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ob.huixinmuqiang.cn

PHP:  get_object_vars($obj);
来源：http://dh.shtwfgs.cn

JS:   Object.entries(obj)
来源：http://ag.muxihuayi.cn

TS:   Object.entries(obj)
来源：http://tt.huixinmuqiang.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gy.jctech888.com.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://mk.panjiajie.cn

Ruby: obj.instance_variables
来源：http://yf.shtwfgs.cn

C#:   // 用反射或 System.Text.Json
来源：http://vi.9csxet.cn

================================================================================
来源：http://pi.colortex.cn

H. 异常与错误处理
来源：http://rm.szsharing.cn

================================================================================
来源：http://bd.hahajie.cn

[H01] try / catch 基础
来源：http://qw.huixiangedu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hw.asd995.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://qn.bjjhwx.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ul.9csxet.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yi.asd995.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ws.szxytkj.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ic.bjjhwx.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://of.shxzukj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://kc.huanxung.cn

[H02] finally / ensure 收尾
来源：http://lp.newstarts.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ny.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://gf.wgjwhj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://rx.szxytkj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ys.shtwfgs.cn

Java: try { f(); } finally { cleanup(); }
来源：http://db.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ov.521024.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sc.9csxet.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bj.wgjwhj.cn

[H03] 主动抛出异常
来源：http://yq.hahajie.cn

Py:   raise ValueError("错误信息")
来源：http://xk.hahajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://zp.muxihuayi.cn

JS:   throw new Error("错误信息");
来源：http://dk.chemitech.net.cn

TS:   throw new Error("错误信息");
来源：http://az.newstarts.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://mv.shtwfgs.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cu.wgjwhj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bs.wgjwhj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bq.huixinmuqiang.cn

[H04] 自定义异常类型
来源：http://uz.gzmigu.cn

Py:   class MyError(Exception): pass
来源：http://gt.bookmarksfly.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lb.nszjky.cn

JS:   class MyError extends Error {}
来源：http://iv.huanxung.cn

TS:   class MyError extends Error {}
来源：http://zg.yuntaijiaju.cn

Java: class MyException extends RuntimeException {}
来源：http://rl.szsharing.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://od.panjiajie.cn

Ruby: class MyError < StandardError; end
来源：http://wz.haigaiapp.cn

C#:   class MyException : Exception {}
来源：http://qs.bjjhwx.cn

[H05] 捕获特定类型
来源：http://rc.jianghongdianzi.cn

Py:   except ValueError as e:
来源：http://sh.jianghongdianzi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://dw.9csxet.cn

JS:   if (e instanceof TypeError) {}
来源：http://le.szxytkj.cn

TS:   if (e instanceof TypeError) {}
来源：http://tk.wgjwhj.cn

Java: catch (IOException | SQLException e) {}
来源：http://ym.jianghongdianzi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://bc.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://ss.jianghongdianzi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tv.muxihuayi.cn

[H06] 可选值 / 空值安全访问
来源：http://vh.huanxung.cn

Py:   value = d.get("k") or default
来源：http://zm.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bd.panjiajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ci.asd995.cn

TS:   obj?.a?.b;  d ?? default
来源：http://eq.yuexingan06.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://so.panjiajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://nt.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://rs.521024.cn

C#:   obj?.A?.B ?? default
来源：http://nb.huixinmuqiang.cn

[H07] 断言
来源：http://ab.gzmigu.cn

Py:   assert x > 0, "必须为正"
来源：http://ca.muxihuayi.cn

PHP:  assert($x > 0);
来源：http://pe.chemitech.net.cn

JS:   console.assert(x > 0);
来源：http://kx.panjiajie.cn

TS:   console.assert(x > 0);
来源：http://zc.asd995.cn

Java: assert x > 0 : "必须为正";
来源：http://cu.asd995.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ac.shxzukj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://va.nicolike.cn

C#:   Debug.Assert(x > 0);
来源：http://gn.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://zu.jctech888.com.cn

Py:   str(e);  traceback.format_exc()
来源：http://sb.521024.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://ea.9csxet.cn

JS:   e.message;  e.stack
来源：http://xz.521024.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ak.nicolike.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://xl.bookmarksfly.cn

Go:   err.Error()
来源：http://wb.shtwfgs.cn

Ruby: e.message;  e.backtrace
来源：http://lc.hahajie.cn

C#:   e.Message;  e.StackTrace
来源：http://lt.chemitech.net.cn

[H09] 带错误码的异常
来源：http://uu.yuntaijiaju.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fp.wgjwhj.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://tf.szxytkj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wr.shtwfgs.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://nf.newstarts.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fb.9csxet.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ui.hnjuh.cn

Ruby: raise MyError.new("fail", 500)
来源：http://vz.hahajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://nk.bookmarksfly.cn

[H10] 资源自动释放
来源：http://is.9csxet.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://xu.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://bl.shtwfgs.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hf.bookmarksfly.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ig.hnjuh.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kb.huixinmuqiang.cn

Go:   defer f.Close()
来源：http://cy.huixiangedu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://si.jctech888.com.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qg.huanxung.cn

================================================================================
来源：http://xu.gzmigu.cn

I. 正则表达式
来源：http://hf.yuntaijiaju.cn

================================================================================
来源：http://fk.szxytkj.cn

[I01] 判断是否匹配
来源：http://fo.colortex.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://fe.huixiangedu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://mr.chemitech.net.cn

JS:   /\d+/.test(s)
来源：http://km.wgjwhj.cn

TS:   /\d+/.test(s)
来源：http://im.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://sp.nicolike.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hr.yuntaijiaju.cn

Ruby: s.match?(/\d+/)
来源：http://ce.yuexingan06.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://by.huanxung.cn

[I02] 提取所有匹配
来源：http://zk.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://cc.haigaiapp.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://cm.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dy.shxzukj.cn

TS:   s.match(/\d+/g)
来源：http://om.colortex.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://il.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ej.nszjky.cn

Ruby: s.scan(/\d+/)
来源：http://ro.lnxyls.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://vm.chemitech.net.cn

[I03] 提取捕获分组
来源：http://rv.nicolike.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ui.521024.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ap.bookmarksfly.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ir.hahajie.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://jk.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jf.szxytkj.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ly.asd995.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://gv.shxzukj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hd.hahajie.cn

[I04] 正则替换
来源：http://td.hnjuh.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://jf.asd995.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://cd.hnjuh.cn

JS:   s.replace(/\d+/g, "#")
来源：http://az.huixiangedu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://hd.nszjky.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ld.bjjhwx.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://lm.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://zb.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://qn.gzmigu.cn

[I05] 按正则拆分
来源：http://wk.shxzskj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://py.panjiajie.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vz.shxzskj.cn

JS:   s.split(/\s*,\s*/)
来源：http://ws.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://kw.bjjhwx.cn

Java: s.split("\\s*,\\s*")
来源：http://fm.bjjhwx.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yo.panjiajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://uj.yuexingan06.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://sw.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ok.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ft.haigaiapp.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://zh.chemitech.net.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hr.shxzskj.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://or.nszjky.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://cm.bookmarksfly.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://rd.huixiangedu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jl.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://gp.shtwfgs.cn

[I07] 忽略大小写与多行模式
来源：http://ea.shxzukj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ir.bjjhwx.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://vc.9csxet.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://rd.nicolike.cn

TS:   /error/gim
来源：http://er.colortex.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://kz.yuntaijiaju.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ak.huixinmuqiang.cn

Ruby: s.scan(/error/i)
来源：http://vn.jianghongdianzi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://dd.wgjwhj.cn

[I08] 贪婪与非贪婪匹配
来源：http://md.chemitech.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://xw.521024.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://wf.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://oq.huixinmuqiang.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://av.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cx.521024.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://tn.szsharing.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hb.gzmigu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://js.szsharing.cn

================================================================================
来源：http://ek.haigaiapp.cn

J. 日期与时间
来源：http://sb.szsharing.cn

================================================================================
来源：http://ns.huixinmuqiang.cn

[J01] 获取当前时间
来源：http://se.lnxyls.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://cb.huanxung.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kx.nszjky.cn

JS:   new Date();  Date.now()
来源：http://rq.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://rp.hahajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ew.hahajie.cn

Go:   time.Now()
来源：http://cq.hnjuh.cn

Ruby: Time.now
来源：http://vb.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://dr.chemitech.net.cn

[J02] 格式化输出
来源：http://yy.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vo.bookmarksfly.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ua.haigaiapp.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vx.bookmarksfly.cn

TS:   d.toISOString()
来源：http://rb.bookmarksfly.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hu.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hk.hnjuh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rj.szsharing.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://sf.nszjky.cn

[J03] 字符串解析为日期
来源：http://ia.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://um.bookmarksfly.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://dm.521024.cn

JS:   new Date("2024-01-02")
来源：http://jt.panjiajie.cn

TS:   new Date("2024-01-02")
来源：http://cx.newstarts.cn

Java: LocalDate.parse("2024-01-02")
来源：http://lf.jianghongdianzi.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hj.jianghongdianzi.cn

Ruby: Date.parse("2024-01-02")
来源：http://wz.huanxung.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hf.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://jl.bjjhwx.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ps.muxihuayi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vv.nicolike.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://rr.hahajie.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ml.yuexingan06.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://kz.hnjuh.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://tn.nicolike.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://sv.chemitech.net.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://lm.muxihuayi.cn

[J05] 时间加减（加 7 天）
来源：http://mv.huixiangedu.cn

Py:   now + timedelta(days=7)
来源：http://jc.huanxung.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://kq.muxihuayi.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wn.521024.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://va.huanxung.cn

Java: LocalDate.now().plusDays(7)
来源：http://oa.lnxyls.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://an.jianghongdianzi.cn

Ruby: Time.now + 7 * 86400
来源：http://xz.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://hc.521024.cn

[J06] 计算两时间之差
来源：http://md.nicolike.cn

Py:   (end - start).total_seconds()
来源：http://fu.chemitech.net.cn

PHP:  $end->diff($start)->days;
来源：http://ci.9csxet.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://jt.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yx.9csxet.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hh.jctech888.com.cn

Go:   end.Sub(start).Hours()
来源：http://id.bookmarksfly.cn

Ruby: end - start                 # 返回秒数
来源：http://iz.shtwfgs.cn

C#:   (end - start).TotalSeconds
来源：http://oy.colortex.cn

[J07] 比较两个日期
来源：http://xl.colortex.cn

Py:   d1 < d2;  d1 == d2
来源：http://gt.bjjhwx.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tl.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://qu.huixinmuqiang.cn

TS:   d1.getTime() < d2.getTime()
来源：http://cj.gzmigu.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://um.gzmigu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xu.nszjky.cn

Ruby: d1 < d2;  d1 == d2
来源：http://hx.nicolike.cn

C#:   d1 < d2;  d1 == d2
来源：http://br.panjiajie.cn

[J08] 提取年月日与星期
来源：http://iv.hnjuh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://eh.haigaiapp.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rp.yuntaijiaju.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://om.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://iw.huixinmuqiang.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mj.muxihuayi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gi.szsharing.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ew.chemitech.net.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://rb.gzmigu.cn

[J09] 时区处理
来源：http://sx.nszjky.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://il.huixiangedu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ew.huanxung.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cq.huixinmuqiang.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ei.521024.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://js.shxzukj.cn


<!-- 参考信息 -->