代发 wailian999

Ruby: attr_accessor :name
来源：http://hd.hnjuh.cn

C#:   public string Name { get; set; }
来源：http://ko.shxzukj.cn

[G12] 对象转字符串
来源：http://wh.colortex.cn

Py:   def __str__(self): return self.name
来源：http://ux.hnjuh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ev.muxihuayi.cn

JS:   toString() { return this.name; }
来源：http://si.szsharing.cn

TS:   toString(): string { return this.name; }
来源：http://ij.521024.cn

Java: @Override public String toString() { return name; }
来源：http://aa.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ky.9csxet.cn

Ruby: def to_s; @name; end
来源：http://lg.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://lo.bjjhwx.cn

[G13] 判断对象类型
来源：http://vi.9csxet.cn

Py:   isinstance(u, User)
来源：http://du.wgjwhj.cn

PHP:  $u instanceof User
来源：http://jw.huixinmuqiang.cn

JS:   u instanceof User
来源：http://bj.szsharing.cn

TS:   u instanceof User
来源：http://sc.newstarts.cn

Java: u instanceof User
来源：http://kp.shxzskj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://dl.yuexingan06.cn

Ruby: u.is_a?(User)
来源：http://qd.colortex.cn

C#:   u is User
来源：http://zy.521024.cn

[G14] 数据类 / record
来源：http://zx.shtwfgs.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ia.newstarts.cn

PHP:  // 用 readonly 属性模拟
来源：http://ww.9csxet.cn

JS:   // 无内置：普通类或对象字面量
来源：http://tr.bookmarksfly.cn

TS:   type User = { name: string; age: number };
来源：http://ql.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://br.huanxung.cn

Go:   type User struct { Name string; Age int }
来源：http://ey.panjiajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://br.jianghongdianzi.cn

C#:   record User(string Name, int Age);
来源：http://cd.nszjky.cn

[G15] 枚举
来源：http://fj.hnjuh.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gg.lnxyls.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rf.bjjhwx.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ht.bookmarksfly.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ol.bookmarksfly.cn

Java: enum Color { RED, GREEN }
来源：http://oj.hnjuh.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://to.wgjwhj.cn

Ruby: Color = %i[red green].freeze
来源：http://rp.gzmigu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wv.521024.cn

[G16] 对象转数组 / 字典
来源：http://lm.chemitech.net.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vv.chemitech.net.cn

PHP:  get_object_vars($obj);
来源：http://si.nicolike.cn

JS:   Object.entries(obj)
来源：http://qe.nszjky.cn

TS:   Object.entries(obj)
来源：http://tc.szsharing.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://es.szsharing.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zb.9csxet.cn

Ruby: obj.instance_variables
来源：http://bx.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://kj.521024.cn

================================================================================
来源：http://iz.yuexingan06.cn

H. 异常与错误处理
来源：http://sn.panjiajie.cn

================================================================================
来源：http://xa.asd995.cn

[H01] try / catch 基础
来源：http://yx.hahajie.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hb.jctech888.com.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tm.huanxung.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xe.bookmarksfly.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jq.nicolike.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ya.asd995.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://zs.wgjwhj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fp.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gp.9csxet.cn

[H02] finally / ensure 收尾
来源：http://rj.huixinmuqiang.cn

Py:   try: f()⏎finally: cleanup()
来源：http://xh.huixiangedu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://on.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pn.bjjhwx.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jr.asd995.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bg.521024.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://dh.newstarts.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://gg.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://oa.huixiangedu.cn

[H03] 主动抛出异常
来源：http://ch.huixiangedu.cn

Py:   raise ValueError("错误信息")
来源：http://hu.521024.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pt.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://vr.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://ep.jctech888.com.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://iq.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xb.chemitech.net.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fo.yuexingan06.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ry.bookmarksfly.cn

[H04] 自定义异常类型
来源：http://dp.hnjuh.cn

Py:   class MyError(Exception): pass
来源：http://lf.shtwfgs.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vf.521024.cn

JS:   class MyError extends Error {}
来源：http://lq.gzmigu.cn

TS:   class MyError extends Error {}
来源：http://lt.chemitech.net.cn

Java: class MyException extends RuntimeException {}
来源：http://yo.shtwfgs.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mk.jianghongdianzi.cn

Ruby: class MyError < StandardError; end
来源：http://dy.huanxung.cn

C#:   class MyException : Exception {}
来源：http://ii.jianghongdianzi.cn

[H05] 捕获特定类型
来源：http://pa.nicolike.cn

Py:   except ValueError as e:
来源：http://rp.yuexingan06.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rf.huanxung.cn

JS:   if (e instanceof TypeError) {}
来源：http://ek.hnjuh.cn

TS:   if (e instanceof TypeError) {}
来源：http://ud.colortex.cn

Java: catch (IOException | SQLException e) {}
来源：http://ty.huixinmuqiang.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://er.521024.cn

Ruby: rescue ArgumentError => e
来源：http://so.bjjhwx.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ur.hahajie.cn

[H06] 可选值 / 空值安全访问
来源：http://bc.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://lc.hnjuh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ew.wgjwhj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qf.chemitech.net.cn

TS:   obj?.a?.b;  d ?? default
来源：http://lr.shxzskj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://se.nicolike.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://np.shtwfgs.cn

Ruby: d&.dig(:a, :b)
来源：http://oq.521024.cn

C#:   obj?.A?.B ?? default
来源：http://qk.hahajie.cn

[H07] 断言
来源：http://hb.asd995.cn

Py:   assert x > 0, "必须为正"
来源：http://lf.haigaiapp.cn

PHP:  assert($x > 0);
来源：http://ii.szsharing.cn

JS:   console.assert(x > 0);
来源：http://zi.szsharing.cn

TS:   console.assert(x > 0);
来源：http://mw.9csxet.cn

Java: assert x > 0 : "必须为正";
来源：http://pq.shtwfgs.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cv.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://pt.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://tx.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://my.521024.cn

Py:   str(e);  traceback.format_exc()
来源：http://dr.hnjuh.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://od.shtwfgs.cn

JS:   e.message;  e.stack
来源：http://bf.jctech888.com.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ip.muxihuayi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://cs.huixinmuqiang.cn

Go:   err.Error()
来源：http://jn.newstarts.cn

Ruby: e.message;  e.backtrace
来源：http://bx.nszjky.cn

C#:   e.Message;  e.StackTrace
来源：http://mb.asd995.cn

[H09] 带错误码的异常
来源：http://fw.9csxet.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xd.bookmarksfly.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://kb.jianghongdianzi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bz.yuntaijiaju.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sj.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://js.muxihuayi.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mw.szsharing.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yd.shxzskj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://jg.yuntaijiaju.cn

[H10] 资源自动释放
来源：http://cn.muxihuayi.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://iy.jctech888.com.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cw.colortex.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ah.hahajie.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ds.newstarts.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://qn.bjjhwx.cn

Go:   defer f.Close()
来源：http://xq.asd995.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ij.chemitech.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://va.yuntaijiaju.cn

================================================================================
来源：http://tt.yuexingan06.cn

I. 正则表达式
来源：http://hx.nszjky.cn

================================================================================
来源：http://hn.521024.cn

[I01] 判断是否匹配
来源：http://ag.huanxung.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://rm.bjjhwx.cn

PHP:  preg_match('/\d+/', $s);
来源：http://af.nszjky.cn

JS:   /\d+/.test(s)
来源：http://gn.colortex.cn

TS:   /\d+/.test(s)
来源：http://pp.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wj.yuntaijiaju.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://pu.muxihuayi.cn

Ruby: s.match?(/\d+/)
来源：http://sd.hahajie.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://we.yuexingan06.cn

[I02] 提取所有匹配
来源：http://ck.hnjuh.cn

Py:   re.findall(r"\d+", s)
来源：http://oj.nicolike.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bo.huixinmuqiang.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zk.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://xf.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xf.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://es.yuntaijiaju.cn

Ruby: s.scan(/\d+/)
来源：http://av.shxzukj.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qq.jianghongdianzi.cn

[I03] 提取捕获分组
来源：http://fy.huixinmuqiang.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://th.colortex.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://pd.haigaiapp.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://fd.nicolike.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zw.shxzskj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://rq.521024.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hm.szxytkj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://di.huanxung.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://dn.9csxet.cn

[I04] 正则替换
来源：http://we.jianghongdianzi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ca.hnjuh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ty.shxzukj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://gq.chemitech.net.cn

TS:   s.replace(/\d+/g, "#")
来源：http://sr.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ji.panjiajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://qt.bookmarksfly.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://um.huixiangedu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://xf.newstarts.cn

[I05] 按正则拆分
来源：http://rg.jctech888.com.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qj.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cp.chemitech.net.cn

JS:   s.split(/\s*,\s*/)
来源：http://gz.newstarts.cn

TS:   s.split(/\s*,\s*/)
来源：http://rx.muxihuayi.cn

Java: s.split("\\s*,\\s*")
来源：http://hw.521024.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fl.yuexingan06.cn

Ruby: s.split(/\s*,\s*/)
来源：http://av.szsharing.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://oq.haigaiapp.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ps.bjjhwx.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://cr.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wq.wgjwhj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ln.newstarts.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zz.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://zo.colortex.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uu.chemitech.net.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://lc.gzmigu.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://so.lnxyls.cn

[I07] 忽略大小写与多行模式
来源：http://cx.521024.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dq.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://to.shxzskj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://cz.szsharing.cn

TS:   /error/gim
来源：http://iw.hnjuh.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://pa.shtwfgs.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://qr.9csxet.cn

Ruby: s.scan(/error/i)
来源：http://rj.shtwfgs.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oc.bjjhwx.cn

[I08] 贪婪与非贪婪匹配
来源：http://sg.9csxet.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://rn.muxihuayi.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://na.wgjwhj.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ka.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://yv.colortex.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ej.szxytkj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://sa.lnxyls.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ij.huixiangedu.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ii.huanxung.cn

================================================================================
来源：http://xe.hnjuh.cn

J. 日期与时间
来源：http://ew.shtwfgs.cn

================================================================================
来源：http://ks.bookmarksfly.cn

[J01] 获取当前时间
来源：http://qx.gzmigu.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://nm.huanxung.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://by.wgjwhj.cn

JS:   new Date();  Date.now()
来源：http://je.yuexingan06.cn

TS:   new Date();  Date.now()
来源：http://xm.panjiajie.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jc.jctech888.com.cn

Go:   time.Now()
来源：http://fa.bookmarksfly.cn

Ruby: Time.now
来源：http://vg.newstarts.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://co.shtwfgs.cn

[J02] 格式化输出
来源：http://kv.shxzskj.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://an.521024.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://yo.jctech888.com.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://sb.lnxyls.cn

TS:   d.toISOString()
来源：http://nz.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://tr.9csxet.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://pk.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ng.yuntaijiaju.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://bo.asd995.cn

[J03] 字符串解析为日期
来源：http://tp.gzmigu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://gz.yuntaijiaju.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://vl.jctech888.com.cn

JS:   new Date("2024-01-02")
来源：http://lz.jianghongdianzi.cn

TS:   new Date("2024-01-02")
来源：http://gu.newstarts.cn

Java: LocalDate.parse("2024-01-02")
来源：http://gr.521024.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://la.shtwfgs.cn

Ruby: Date.parse("2024-01-02")
来源：http://wa.shxzskj.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ng.wgjwhj.cn

[J04] 时间戳与日期互转
来源：http://vi.hnjuh.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vm.bookmarksfly.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://mx.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://lu.muxihuayi.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://jr.chemitech.net.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oo.jianghongdianzi.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ge.newstarts.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tx.szxytkj.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://om.521024.cn

[J05] 时间加减（加 7 天）
来源：http://oz.muxihuayi.cn

Py:   now + timedelta(days=7)
来源：http://oi.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://jj.shtwfgs.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vk.shtwfgs.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://px.szxytkj.cn

Java: LocalDate.now().plusDays(7)
来源：http://jb.huixiangedu.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://pn.nszjky.cn

Ruby: Time.now + 7 * 86400
来源：http://oa.yuntaijiaju.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ng.nszjky.cn

[J06] 计算两时间之差
来源：http://tb.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://jh.lnxyls.cn

PHP:  $end->diff($start)->days;
来源：http://vf.yuexingan06.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://vr.chemitech.net.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fh.521024.cn

Java: Duration.between(start, end).toSeconds()
来源：http://xn.lnxyls.cn

Go:   end.Sub(start).Hours()
来源：http://kf.hahajie.cn

Ruby: end - start                 # 返回秒数
来源：http://yx.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://mi.bjjhwx.cn

[J07] 比较两个日期
来源：http://zk.9csxet.cn

Py:   d1 < d2;  d1 == d2
来源：http://lt.huixiangedu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://de.haigaiapp.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ov.shtwfgs.cn

TS:   d1.getTime() < d2.getTime()
来源：http://gz.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ki.9csxet.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://sg.muxihuayi.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ij.nszjky.cn

C#:   d1 < d2;  d1 == d2
来源：http://nu.huixinmuqiang.cn

[J08] 提取年月日与星期
来源：http://rg.bookmarksfly.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://go.muxihuayi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lo.bookmarksfly.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://bh.huixiangedu.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ok.hahajie.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gq.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://oj.lnxyls.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wh.jctech888.com.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mk.huixinmuqiang.cn

[J09] 时区处理
来源：http://kh.colortex.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ij.huixinmuqiang.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://vv.jianghongdianzi.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aa.jctech888.com.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cj.bookmarksfly.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://kc.huixinmuqiang.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ue.jianghongdianzi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ej.wgjwhj.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hi.asd995.cn

[J10] 取今天 / 本月第一天
来源：http://fk.nicolike.cn


<!-- 参考信息 -->