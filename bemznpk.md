代发 wailian999

[G10] 访问控制
来源：http://so.shxzukj.cn

Py:   约定 _protected / __private（不强制）
来源：http://ic.lnxyls.cn

PHP:  public / protected / private
来源：http://uz.colortex.cn

JS:   #private 字段；其余公开
来源：http://lz.wgjwhj.cn

TS:   public / protected / private
来源：http://qq.wgjwhj.cn

Java: public / protected / private / 默认包级
来源：http://fa.shxzukj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://wz.chemitech.net.cn

Ruby: public / protected / private
来源：http://ok.9csxet.cn

C#:   public / protected / private / internal
来源：http://qc.hnjuh.cn

[G11] getter / setter
来源：http://et.9csxet.cn

Py:   @property 与 @x.setter
来源：http://he.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tr.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://nq.bjjhwx.cn

TS:   get name(): string { return this._name; }
来源：http://ui.lnxyls.cn

Java: public String getName() { return name; }
来源：http://og.nicolike.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wd.huixinmuqiang.cn

Ruby: attr_accessor :name
来源：http://ir.colortex.cn

C#:   public string Name { get; set; }
来源：http://hr.huanxung.cn

[G12] 对象转字符串
来源：http://aa.bookmarksfly.cn

Py:   def __str__(self): return self.name
来源：http://bg.szsharing.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zy.hahajie.cn

JS:   toString() { return this.name; }
来源：http://ow.hahajie.cn

TS:   toString(): string { return this.name; }
来源：http://xi.chemitech.net.cn

Java: @Override public String toString() { return name; }
来源：http://ut.shxzukj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://hw.bookmarksfly.cn

Ruby: def to_s; @name; end
来源：http://hy.jctech888.com.cn

C#:   public override string ToString() => Name;
来源：http://sw.hnjuh.cn

[G13] 判断对象类型
来源：http://js.chemitech.net.cn

Py:   isinstance(u, User)
来源：http://gm.521024.cn

PHP:  $u instanceof User
来源：http://pv.huanxung.cn

JS:   u instanceof User
来源：http://fi.hahajie.cn

TS:   u instanceof User
来源：http://pj.hnjuh.cn

Java: u instanceof User
来源：http://di.521024.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fn.jctech888.com.cn

Ruby: u.is_a?(User)
来源：http://ng.muxihuayi.cn

C#:   u is User
来源：http://pp.jctech888.com.cn

[G14] 数据类 / record
来源：http://uo.szxytkj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://eq.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://wu.nszjky.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jl.yuntaijiaju.cn

TS:   type User = { name: string; age: number };
来源：http://iw.hnjuh.cn

Java: record User(String name, int age) {}
来源：http://uh.yuntaijiaju.cn

Go:   type User struct { Name string; Age int }
来源：http://sq.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://yi.shtwfgs.cn

C#:   record User(string Name, int Age);
来源：http://nl.szxytkj.cn

[G15] 枚举
来源：http://xf.szxytkj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://op.chemitech.net.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://xf.shxzskj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jq.nicolike.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kf.shxzskj.cn

Java: enum Color { RED, GREEN }
来源：http://ew.huanxung.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rs.chemitech.net.cn

Ruby: Color = %i[red green].freeze
来源：http://dq.szsharing.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://yo.huixinmuqiang.cn

[G16] 对象转数组 / 字典
来源：http://ed.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://iw.haigaiapp.cn

PHP:  get_object_vars($obj);
来源：http://hk.hnjuh.cn

JS:   Object.entries(obj)
来源：http://hg.huanxung.cn

TS:   Object.entries(obj)
来源：http://ta.lnxyls.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://kl.panjiajie.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ab.colortex.cn

Ruby: obj.instance_variables
来源：http://xg.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://yc.szsharing.cn

================================================================================
来源：http://ze.szsharing.cn

H. 异常与错误处理
来源：http://mm.nicolike.cn

================================================================================
来源：http://cq.huixiangedu.cn

[H01] try / catch 基础
来源：http://xq.gzmigu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://nb.huixinmuqiang.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fc.huixiangedu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zp.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fh.wgjwhj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://zk.muxihuayi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gz.huanxung.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nr.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://yl.newstarts.cn

[H02] finally / ensure 收尾
来源：http://fu.panjiajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pe.nicolike.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lq.9csxet.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nx.szsharing.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qy.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://we.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://od.bookmarksfly.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ll.wgjwhj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://il.huixiangedu.cn

[H03] 主动抛出异常
来源：http://vp.haigaiapp.cn

Py:   raise ValueError("错误信息")
来源：http://oq.yuntaijiaju.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ub.hnjuh.cn

JS:   throw new Error("错误信息");
来源：http://jy.nicolike.cn

TS:   throw new Error("错误信息");
来源：http://ul.newstarts.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://nw.chemitech.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tz.wgjwhj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zs.shtwfgs.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nm.nszjky.cn

[H04] 自定义异常类型
来源：http://lv.shxzukj.cn

Py:   class MyError(Exception): pass
来源：http://kn.hnjuh.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ph.521024.cn

JS:   class MyError extends Error {}
来源：http://vz.huanxung.cn

TS:   class MyError extends Error {}
来源：http://xf.panjiajie.cn

Java: class MyException extends RuntimeException {}
来源：http://cf.wgjwhj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://gs.9csxet.cn

Ruby: class MyError < StandardError; end
来源：http://sd.shxzukj.cn

C#:   class MyException : Exception {}
来源：http://xe.yuntaijiaju.cn

[H05] 捕获特定类型
来源：http://wi.panjiajie.cn

Py:   except ValueError as e:
来源：http://jq.yuexingan06.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wa.bookmarksfly.cn

JS:   if (e instanceof TypeError) {}
来源：http://ri.bookmarksfly.cn

TS:   if (e instanceof TypeError) {}
来源：http://rh.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://qq.colortex.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qu.yuexingan06.cn

Ruby: rescue ArgumentError => e
来源：http://ya.jctech888.com.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://jz.asd995.cn

[H06] 可选值 / 空值安全访问
来源：http://oq.nicolike.cn

Py:   value = d.get("k") or default
来源：http://es.newstarts.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jt.jianghongdianzi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ro.asd995.cn

TS:   obj?.a?.b;  d ?? default
来源：http://qa.panjiajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://tu.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ln.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://wq.asd995.cn

C#:   obj?.A?.B ?? default
来源：http://yr.asd995.cn

[H07] 断言
来源：http://sd.colortex.cn

Py:   assert x > 0, "必须为正"
来源：http://dv.bjjhwx.cn

PHP:  assert($x > 0);
来源：http://dv.chemitech.net.cn

JS:   console.assert(x > 0);
来源：http://uz.bjjhwx.cn

TS:   console.assert(x > 0);
来源：http://ua.szsharing.cn

Java: assert x > 0 : "必须为正";
来源：http://pj.shxzukj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://to.521024.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vl.muxihuayi.cn

C#:   Debug.Assert(x > 0);
来源：http://yn.muxihuayi.cn

[H08] 获取错误信息与堆栈
来源：http://tz.newstarts.cn

Py:   str(e);  traceback.format_exc()
来源：http://pn.wgjwhj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://lj.colortex.cn

JS:   e.message;  e.stack
来源：http://lb.jianghongdianzi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://zn.hnjuh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rb.colortex.cn

Go:   err.Error()
来源：http://ij.hahajie.cn

Ruby: e.message;  e.backtrace
来源：http://sd.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://ui.shxzukj.cn

[H09] 带错误码的异常
来源：http://ak.newstarts.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ec.jctech888.com.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://md.hahajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ao.521024.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://om.hnjuh.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://dr.bookmarksfly.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iz.muxihuayi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fd.shtwfgs.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gm.huixiangedu.cn

[H10] 资源自动释放
来源：http://fz.asd995.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://kr.huixinmuqiang.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ap.yuntaijiaju.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://cr.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://vj.bookmarksfly.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://dk.shxzskj.cn

Go:   defer f.Close()
来源：http://rc.huixinmuqiang.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://lr.wgjwhj.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qp.newstarts.cn

================================================================================
来源：http://ot.jianghongdianzi.cn

I. 正则表达式
来源：http://uh.asd995.cn

================================================================================
来源：http://to.szxytkj.cn

[I01] 判断是否匹配
来源：http://ep.shxzskj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://lw.jctech888.com.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ma.huanxung.cn

JS:   /\d+/.test(s)
来源：http://dj.521024.cn

TS:   /\d+/.test(s)
来源：http://ua.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tt.9csxet.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ny.gzmigu.cn

Ruby: s.match?(/\d+/)
来源：http://oo.huanxung.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://rl.hahajie.cn

[I02] 提取所有匹配
来源：http://np.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://tk.9csxet.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://fu.panjiajie.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://vn.huanxung.cn

TS:   s.match(/\d+/g)
来源：http://pc.nszjky.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sr.nicolike.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://sn.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://ma.9csxet.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://bq.shtwfgs.cn

[I03] 提取捕获分组
来源：http://oh.shxzskj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cn.hnjuh.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gt.nicolike.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ud.nszjky.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://cj.hnjuh.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://vi.asd995.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vc.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pl.nicolike.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zi.yuntaijiaju.cn

[I04] 正则替换
来源：http://cr.chemitech.net.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://xs.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://yb.colortex.cn

JS:   s.replace(/\d+/g, "#")
来源：http://pv.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yd.jianghongdianzi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://vk.muxihuayi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kp.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sn.hahajie.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://an.jctech888.com.cn

[I05] 按正则拆分
来源：http://zb.9csxet.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://vg.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://km.shxzskj.cn

JS:   s.split(/\s*,\s*/)
来源：http://se.nszjky.cn

TS:   s.split(/\s*,\s*/)
来源：http://yg.shxzskj.cn

Java: s.split("\\s*,\\s*")
来源：http://ms.lnxyls.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://sv.shxzskj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://cy.yuntaijiaju.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://mo.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hv.shxzskj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dc.szxytkj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://gh.hahajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jm.huanxung.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qs.wgjwhj.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yz.muxihuayi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qe.panjiajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://gk.shxzukj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ow.bjjhwx.cn

[I07] 忽略大小写与多行模式
来源：http://iq.shtwfgs.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://xd.yuntaijiaju.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oj.yuntaijiaju.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ei.huixiangedu.cn

TS:   /error/gim
来源：http://ll.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://eg.hahajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ch.lnxyls.cn

Ruby: s.scan(/error/i)
来源：http://xr.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hv.9csxet.cn

[I08] 贪婪与非贪婪匹配
来源：http://um.shxzukj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://yo.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://yq.bjjhwx.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mt.jianghongdianzi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://cr.szxytkj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://wz.huanxung.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://td.asd995.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://kt.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://xk.hahajie.cn

================================================================================
来源：http://ee.huanxung.cn

J. 日期与时间
来源：http://nq.hnjuh.cn

================================================================================
来源：http://hj.szxytkj.cn

[J01] 获取当前时间
来源：http://yd.muxihuayi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hq.szsharing.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ko.shtwfgs.cn

JS:   new Date();  Date.now()
来源：http://ho.colortex.cn

TS:   new Date();  Date.now()
来源：http://pz.huixinmuqiang.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://uw.521024.cn

Go:   time.Now()
来源：http://jp.jctech888.com.cn

Ruby: Time.now
来源：http://hv.nicolike.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://fv.huixinmuqiang.cn

[J02] 格式化输出
来源：http://ga.jctech888.com.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yc.colortex.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ub.hahajie.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://fv.jianghongdianzi.cn

TS:   d.toISOString()
来源：http://zq.wgjwhj.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://fu.muxihuayi.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://sw.szxytkj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://cu.huixiangedu.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wr.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://gg.szsharing.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://rm.9csxet.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://nv.hahajie.cn

JS:   new Date("2024-01-02")
来源：http://tl.newstarts.cn

TS:   new Date("2024-01-02")
来源：http://vg.haigaiapp.cn

Java: LocalDate.parse("2024-01-02")
来源：http://if.yuntaijiaju.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://jv.panjiajie.cn

Ruby: Date.parse("2024-01-02")
来源：http://nv.yuntaijiaju.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nw.muxihuayi.cn

[J04] 时间戳与日期互转
来源：http://rw.huixinmuqiang.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ew.newstarts.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ns.muxihuayi.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://id.newstarts.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://tj.panjiajie.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://jj.huixinmuqiang.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://fg.panjiajie.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qp.bookmarksfly.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tu.wgjwhj.cn

[J05] 时间加减（加 7 天）
来源：http://jr.jctech888.com.cn

Py:   now + timedelta(days=7)
来源：http://zl.yuexingan06.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pc.szsharing.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://qo.shxzukj.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://kz.hnjuh.cn

Java: LocalDate.now().plusDays(7)
来源：http://ee.huixinmuqiang.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://li.gzmigu.cn

Ruby: Time.now + 7 * 86400
来源：http://yz.muxihuayi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://ux.chemitech.net.cn

[J06] 计算两时间之差
来源：http://bm.bjjhwx.cn

Py:   (end - start).total_seconds()
来源：http://df.muxihuayi.cn

PHP:  $end->diff($start)->days;
来源：http://no.chemitech.net.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://cs.gzmigu.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fa.nicolike.cn

Java: Duration.between(start, end).toSeconds()
来源：http://rf.bjjhwx.cn

Go:   end.Sub(start).Hours()
来源：http://qd.asd995.cn

Ruby: end - start                 # 返回秒数
来源：http://xz.haigaiapp.cn

C#:   (end - start).TotalSeconds
来源：http://kf.shxzskj.cn

[J07] 比较两个日期
来源：http://se.yuntaijiaju.cn

Py:   d1 < d2;  d1 == d2
来源：http://hk.szxytkj.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ki.shtwfgs.cn

JS:   d1.getTime() < d2.getTime()
来源：http://np.shxzukj.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pn.colortex.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jh.colortex.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://lx.nicolike.cn

Ruby: d1 < d2;  d1 == d2
来源：http://bo.lnxyls.cn

C#:   d1 < d2;  d1 == d2
来源：http://kq.521024.cn

[J08] 提取年月日与星期
来源：http://fz.szsharing.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bv.jianghongdianzi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tc.jctech888.com.cn


<!-- 参考信息 -->