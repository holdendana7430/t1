代发 wailian999

C#:   public / protected / private / internal
来源：http://pw.szsharing.cn

[G11] getter / setter
来源：http://ok.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://lj.nicolike.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://sp.nicolike.cn

JS:   get name() { return this._name; }
来源：http://ce.nicolike.cn

TS:   get name(): string { return this._name; }
来源：http://xk.hnjuh.cn

Java: public String getName() { return name; }
来源：http://yv.hnjuh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xb.szsharing.cn

Ruby: attr_accessor :name
来源：http://qi.521024.cn

C#:   public string Name { get; set; }
来源：http://ig.huanxung.cn

[G12] 对象转字符串
来源：http://ky.huixinmuqiang.cn

Py:   def __str__(self): return self.name
来源：http://pi.haigaiapp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hh.nicolike.cn

JS:   toString() { return this.name; }
来源：http://od.shxzskj.cn

TS:   toString(): string { return this.name; }
来源：http://tb.9csxet.cn

Java: @Override public String toString() { return name; }
来源：http://ft.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://tv.shxzukj.cn

Ruby: def to_s; @name; end
来源：http://ck.lnxyls.cn

C#:   public override string ToString() => Name;
来源：http://pi.hahajie.cn

[G13] 判断对象类型
来源：http://xs.panjiajie.cn

Py:   isinstance(u, User)
来源：http://le.haigaiapp.cn

PHP:  $u instanceof User
来源：http://zs.newstarts.cn

JS:   u instanceof User
来源：http://sk.panjiajie.cn

TS:   u instanceof User
来源：http://mb.muxihuayi.cn

Java: u instanceof User
来源：http://qc.wgjwhj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wz.jianghongdianzi.cn

Ruby: u.is_a?(User)
来源：http://lr.521024.cn

C#:   u is User
来源：http://fm.yuexingan06.cn

[G14] 数据类 / record
来源：http://vs.huixiangedu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ww.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://ww.huanxung.cn

JS:   // 无内置：普通类或对象字面量
来源：http://gi.huixinmuqiang.cn

TS:   type User = { name: string; age: number };
来源：http://lg.hahajie.cn

Java: record User(String name, int age) {}
来源：http://qn.yuexingan06.cn

Go:   type User struct { Name string; Age int }
来源：http://vl.hahajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hh.shxzukj.cn

C#:   record User(string Name, int Age);
来源：http://by.asd995.cn

[G15] 枚举
来源：http://ah.szxytkj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vg.shtwfgs.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vm.muxihuayi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qz.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ew.hahajie.cn

Java: enum Color { RED, GREEN }
来源：http://wn.jianghongdianzi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://uv.yuexingan06.cn

Ruby: Color = %i[red green].freeze
来源：http://pj.gzmigu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jg.gzmigu.cn

[G16] 对象转数组 / 字典
来源：http://ei.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://eg.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://nn.hahajie.cn

JS:   Object.entries(obj)
来源：http://ya.nszjky.cn

TS:   Object.entries(obj)
来源：http://rz.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tz.huixiangedu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gn.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://yb.lnxyls.cn

C#:   // 用反射或 System.Text.Json
来源：http://os.szsharing.cn

================================================================================
来源：http://bn.shtwfgs.cn

H. 异常与错误处理
来源：http://rz.szxytkj.cn

================================================================================
来源：http://bt.nszjky.cn

[H01] try / catch 基础
来源：http://gd.9csxet.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vq.bookmarksfly.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yj.9csxet.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xp.shxzskj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xw.gzmigu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qu.bjjhwx.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tx.shtwfgs.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yq.hahajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://rz.muxihuayi.cn

[H02] finally / ensure 收尾
来源：http://xq.wgjwhj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wo.asd995.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wx.yuntaijiaju.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qg.haigaiapp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://dt.jianghongdianzi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yw.jianghongdianzi.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vu.shxzskj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ze.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zl.hahajie.cn

[H03] 主动抛出异常
来源：http://eq.nicolike.cn

Py:   raise ValueError("错误信息")
来源：http://ha.asd995.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://bn.huixiangedu.cn

JS:   throw new Error("错误信息");
来源：http://qj.wgjwhj.cn

TS:   throw new Error("错误信息");
来源：http://li.jctech888.com.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ck.bookmarksfly.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ro.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ej.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xk.szsharing.cn

[H04] 自定义异常类型
来源：http://gy.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://oq.yuexingan06.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sl.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://xf.jianghongdianzi.cn

TS:   class MyError extends Error {}
来源：http://ae.szxytkj.cn

Java: class MyException extends RuntimeException {}
来源：http://lk.szxytkj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yf.shtwfgs.cn

Ruby: class MyError < StandardError; end
来源：http://vg.szxytkj.cn

C#:   class MyException : Exception {}
来源：http://oc.newstarts.cn

[H05] 捕获特定类型
来源：http://pr.panjiajie.cn

Py:   except ValueError as e:
来源：http://ii.jianghongdianzi.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mb.chemitech.net.cn

JS:   if (e instanceof TypeError) {}
来源：http://if.muxihuayi.cn

TS:   if (e instanceof TypeError) {}
来源：http://rg.lnxyls.cn

Java: catch (IOException | SQLException e) {}
来源：http://ri.hahajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://re.szsharing.cn

Ruby: rescue ArgumentError => e
来源：http://mz.bookmarksfly.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ck.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://im.newstarts.cn

Py:   value = d.get("k") or default
来源：http://qr.szxytkj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jb.huixiangedu.cn

JS:   obj?.a?.b;  d ?? default
来源：http://vn.hahajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://vm.colortex.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wb.newstarts.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://eg.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://wo.jctech888.com.cn

C#:   obj?.A?.B ?? default
来源：http://lx.bjjhwx.cn

[H07] 断言
来源：http://oe.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://et.hahajie.cn

PHP:  assert($x > 0);
来源：http://cr.bjjhwx.cn

JS:   console.assert(x > 0);
来源：http://rh.panjiajie.cn

TS:   console.assert(x > 0);
来源：http://ce.szxytkj.cn

Java: assert x > 0 : "必须为正";
来源：http://ww.shxzukj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://jg.bjjhwx.cn

Ruby: raise "必须为正" unless x > 0
来源：http://rq.jctech888.com.cn

C#:   Debug.Assert(x > 0);
来源：http://hj.newstarts.cn

[H08] 获取错误信息与堆栈
来源：http://ji.hnjuh.cn

Py:   str(e);  traceback.format_exc()
来源：http://ff.yuexingan06.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hm.hnjuh.cn

JS:   e.message;  e.stack
来源：http://ca.haigaiapp.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://eh.hnjuh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://an.newstarts.cn

Go:   err.Error()
来源：http://dd.huixiangedu.cn

Ruby: e.message;  e.backtrace
来源：http://vb.bookmarksfly.cn

C#:   e.Message;  e.StackTrace
来源：http://tk.wgjwhj.cn

[H09] 带错误码的异常
来源：http://zd.nszjky.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tx.bjjhwx.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mc.huixiangedu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kr.newstarts.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://cw.huixinmuqiang.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://or.newstarts.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ol.521024.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://sc.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://ex.9csxet.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://se.wgjwhj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ek.hnjuh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ol.haigaiapp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://es.szsharing.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ro.nszjky.cn

Go:   defer f.Close()
来源：http://ex.shxzukj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://xl.jianghongdianzi.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://so.hnjuh.cn

================================================================================
来源：http://ao.shtwfgs.cn

I. 正则表达式
来源：http://ji.wgjwhj.cn

================================================================================
来源：http://lc.nicolike.cn

[I01] 判断是否匹配
来源：http://zq.lnxyls.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://yb.nicolike.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ub.shxzskj.cn

JS:   /\d+/.test(s)
来源：http://vy.jctech888.com.cn

TS:   /\d+/.test(s)
来源：http://pn.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ed.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ag.hnjuh.cn

Ruby: s.match?(/\d+/)
来源：http://vt.szxytkj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ap.521024.cn

[I02] 提取所有匹配
来源：http://bh.yuntaijiaju.cn

Py:   re.findall(r"\d+", s)
来源：http://as.shtwfgs.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nj.asd995.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ec.szsharing.cn

TS:   s.match(/\d+/g)
来源：http://pw.jctech888.com.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ml.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://id.hahajie.cn

Ruby: s.scan(/\d+/)
来源：http://op.9csxet.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ko.szxytkj.cn

[I03] 提取捕获分组
来源：http://co.jctech888.com.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://eh.szxytkj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://jy.nicolike.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://jk.bookmarksfly.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://kb.gzmigu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vd.szsharing.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rq.hahajie.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sd.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ee.jctech888.com.cn

[I04] 正则替换
来源：http://bn.jianghongdianzi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://sy.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hn.huanxung.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ms.huixiangedu.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vw.shxzskj.cn

Java: s.replaceAll("\\d+", "#")
来源：http://jr.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ng.huanxung.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://bo.nicolike.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://bt.haigaiapp.cn

[I05] 按正则拆分
来源：http://jq.panjiajie.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ch.shtwfgs.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://fb.hnjuh.cn

JS:   s.split(/\s*,\s*/)
来源：http://oz.jctech888.com.cn

TS:   s.split(/\s*,\s*/)
来源：http://nt.asd995.cn

Java: s.split("\\s*,\\s*")
来源：http://nb.hahajie.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://bd.newstarts.cn

Ruby: s.split(/\s*,\s*/)
来源：http://jy.shxzskj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://kh.bookmarksfly.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qf.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://yt.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://yq.gzmigu.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://iu.nicolike.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wb.bjjhwx.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://gr.wgjwhj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://la.szsharing.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://xj.shxzskj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://fo.nicolike.cn

[I07] 忽略大小写与多行模式
来源：http://ho.gzmigu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mr.lnxyls.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://zf.wgjwhj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://kt.lnxyls.cn

TS:   /error/gim
来源：http://dq.newstarts.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://bd.gzmigu.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ll.huixiangedu.cn

Ruby: s.scan(/error/i)
来源：http://nq.huanxung.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://yr.hnjuh.cn

[I08] 贪婪与非贪婪匹配
来源：http://bh.muxihuayi.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vh.gzmigu.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://tw.asd995.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://re.huixiangedu.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ms.muxihuayi.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://go.panjiajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://lq.wgjwhj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cb.szsharing.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wf.panjiajie.cn

================================================================================
来源：http://ht.huixinmuqiang.cn

J. 日期与时间
来源：http://mu.521024.cn

================================================================================
来源：http://ck.gzmigu.cn

[J01] 获取当前时间
来源：http://ko.chemitech.net.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://er.nicolike.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kn.yuexingan06.cn

JS:   new Date();  Date.now()
来源：http://uo.chemitech.net.cn

TS:   new Date();  Date.now()
来源：http://nf.bjjhwx.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://hg.szxytkj.cn

Go:   time.Now()
来源：http://au.shxzskj.cn

Ruby: Time.now
来源：http://rg.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://du.bookmarksfly.cn

[J02] 格式化输出
来源：http://st.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zi.shxzukj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ol.nszjky.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fo.gzmigu.cn

TS:   d.toISOString()
来源：http://bo.nicolike.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://rk.bjjhwx.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://kb.jctech888.com.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yg.nicolike.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lr.gzmigu.cn

[J03] 字符串解析为日期
来源：http://kf.jianghongdianzi.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ph.hahajie.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pi.bookmarksfly.cn

JS:   new Date("2024-01-02")
来源：http://qz.bjjhwx.cn

TS:   new Date("2024-01-02")
来源：http://tn.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bp.szxytkj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ax.asd995.cn

Ruby: Date.parse("2024-01-02")
来源：http://fs.shtwfgs.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://qz.lnxyls.cn

[J04] 时间戳与日期互转
来源：http://mb.shtwfgs.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vt.9csxet.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://iu.bjjhwx.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://nb.huixinmuqiang.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://yu.huanxung.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://ea.yuntaijiaju.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fx.yuntaijiaju.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://tl.bjjhwx.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://kv.nicolike.cn

[J05] 时间加减（加 7 天）
来源：http://xp.huanxung.cn

Py:   now + timedelta(days=7)
来源：http://yq.szsharing.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://dz.szxytkj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qw.gzmigu.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bi.huixinmuqiang.cn

Java: LocalDate.now().plusDays(7)
来源：http://yh.nszjky.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://xa.szxytkj.cn

Ruby: Time.now + 7 * 86400
来源：http://bm.hnjuh.cn

C#:   DateTime.Now.AddDays(7)
来源：http://cy.szsharing.cn

[J06] 计算两时间之差
来源：http://uk.newstarts.cn

Py:   (end - start).total_seconds()
来源：http://pj.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://uh.asd995.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ji.hnjuh.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://be.521024.cn

Java: Duration.between(start, end).toSeconds()
来源：http://vl.hahajie.cn

Go:   end.Sub(start).Hours()
来源：http://re.hnjuh.cn

Ruby: end - start                 # 返回秒数
来源：http://en.bookmarksfly.cn

C#:   (end - start).TotalSeconds
来源：http://xi.nicolike.cn

[J07] 比较两个日期
来源：http://wq.hahajie.cn

Py:   d1 < d2;  d1 == d2
来源：http://iv.chemitech.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ux.muxihuayi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://fl.newstarts.cn

TS:   d1.getTime() < d2.getTime()
来源：http://we.bjjhwx.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yc.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rx.bjjhwx.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ux.jianghongdianzi.cn

C#:   d1 < d2;  d1 == d2
来源：http://hl.jianghongdianzi.cn

[J08] 提取年月日与星期
来源：http://ju.huanxung.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://pq.hahajie.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xs.gzmigu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xz.haigaiapp.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://fe.chemitech.net.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ff.yuexingan06.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://bn.yuexingan06.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lm.yuexingan06.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://fx.chemitech.net.cn

[J09] 时区处理
来源：http://qb.newstarts.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://kb.gzmigu.cn


<!-- 参考信息 -->