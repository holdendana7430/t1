代发 wailian999

Java: interface Shape { double area(); }
来源：http://qi.huixinmuqiang.cn

Go:   type Shape interface { Area() float64 }
来源：http://ck.colortex.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://va.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://lz.bookmarksfly.cn

[G10] 访问控制
来源：http://yr.lnxyls.cn

Py:   约定 _protected / __private（不强制）
来源：http://xn.yuntaijiaju.cn

PHP:  public / protected / private
来源：http://we.szsharing.cn

JS:   #private 字段；其余公开
来源：http://hv.521024.cn

TS:   public / protected / private
来源：http://qb.huanxung.cn

Java: public / protected / private / 默认包级
来源：http://rn.hnjuh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kk.nicolike.cn

Ruby: public / protected / private
来源：http://ta.9csxet.cn

C#:   public / protected / private / internal
来源：http://ii.jianghongdianzi.cn

[G11] getter / setter
来源：http://jf.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://er.huixiangedu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://iz.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://pu.newstarts.cn

TS:   get name(): string { return this._name; }
来源：http://ol.wgjwhj.cn

Java: public String getName() { return name; }
来源：http://pa.huanxung.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bb.huixiangedu.cn

Ruby: attr_accessor :name
来源：http://hi.wgjwhj.cn

C#:   public string Name { get; set; }
来源：http://gq.9csxet.cn

[G12] 对象转字符串
来源：http://qu.lnxyls.cn

Py:   def __str__(self): return self.name
来源：http://wc.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mk.jctech888.com.cn

JS:   toString() { return this.name; }
来源：http://yt.haigaiapp.cn

TS:   toString(): string { return this.name; }
来源：http://uz.chemitech.net.cn

Java: @Override public String toString() { return name; }
来源：http://jg.lnxyls.cn

Go:   func (u User) String() string { return u.Name }
来源：http://sv.yuntaijiaju.cn

Ruby: def to_s; @name; end
来源：http://su.asd995.cn

C#:   public override string ToString() => Name;
来源：http://gu.hnjuh.cn

[G13] 判断对象类型
来源：http://qh.gzmigu.cn

Py:   isinstance(u, User)
来源：http://nk.gzmigu.cn

PHP:  $u instanceof User
来源：http://nm.nszjky.cn

JS:   u instanceof User
来源：http://nl.shtwfgs.cn

TS:   u instanceof User
来源：http://ba.bjjhwx.cn

Java: u instanceof User
来源：http://bv.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ea.huixiangedu.cn

Ruby: u.is_a?(User)
来源：http://so.shxzskj.cn

C#:   u is User
来源：http://bu.hahajie.cn

[G14] 数据类 / record
来源：http://le.nszjky.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kt.newstarts.cn

PHP:  // 用 readonly 属性模拟
来源：http://ys.huanxung.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ik.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://lo.colortex.cn

Java: record User(String name, int age) {}
来源：http://ie.yuntaijiaju.cn

Go:   type User struct { Name string; Age int }
来源：http://sp.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jh.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://it.szxytkj.cn

[G15] 枚举
来源：http://ku.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kp.shxzukj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ta.hnjuh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://et.hnjuh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://zd.szxytkj.cn

Java: enum Color { RED, GREEN }
来源：http://yk.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ia.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://xb.yuexingan06.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://zr.shxzukj.cn

[G16] 对象转数组 / 字典
来源：http://wz.panjiajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lx.shtwfgs.cn

PHP:  get_object_vars($obj);
来源：http://fj.jianghongdianzi.cn

JS:   Object.entries(obj)
来源：http://yo.gzmigu.cn

TS:   Object.entries(obj)
来源：http://ae.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yv.nicolike.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://dl.shtwfgs.cn

Ruby: obj.instance_variables
来源：http://cf.shtwfgs.cn

C#:   // 用反射或 System.Text.Json
来源：http://pd.huixiangedu.cn

================================================================================
来源：http://kg.yuntaijiaju.cn

H. 异常与错误处理
来源：http://zs.shxzukj.cn

================================================================================
来源：http://tb.huixinmuqiang.cn

[H01] try / catch 基础
来源：http://fm.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kb.hahajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://sy.nicolike.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zt.szsharing.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ea.521024.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uv.nicolike.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://rh.panjiajie.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://dx.hahajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://cz.bookmarksfly.cn

[H02] finally / ensure 收尾
来源：http://zo.gzmigu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://js.shtwfgs.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jq.chemitech.net.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nn.chemitech.net.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vt.newstarts.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gh.shtwfgs.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://nd.hahajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ny.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://vi.bookmarksfly.cn

[H03] 主动抛出异常
来源：http://hh.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://pd.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ls.nszjky.cn

JS:   throw new Error("错误信息");
来源：http://qc.newstarts.cn

TS:   throw new Error("错误信息");
来源：http://ft.jianghongdianzi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://vz.shxzukj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ym.asd995.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wz.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://oz.521024.cn

[H04] 自定义异常类型
来源：http://vh.muxihuayi.cn

Py:   class MyError(Exception): pass
来源：http://le.yuexingan06.cn

PHP:  class MyError extends RuntimeException {}
来源：http://av.panjiajie.cn

JS:   class MyError extends Error {}
来源：http://fw.huanxung.cn

TS:   class MyError extends Error {}
来源：http://jn.huixinmuqiang.cn

Java: class MyException extends RuntimeException {}
来源：http://of.gzmigu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://vr.yuexingan06.cn

Ruby: class MyError < StandardError; end
来源：http://if.shtwfgs.cn

C#:   class MyException : Exception {}
来源：http://sg.chemitech.net.cn

[H05] 捕获特定类型
来源：http://uo.huanxung.cn

Py:   except ValueError as e:
来源：http://ev.bjjhwx.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ug.huanxung.cn

JS:   if (e instanceof TypeError) {}
来源：http://rj.haigaiapp.cn

TS:   if (e instanceof TypeError) {}
来源：http://aq.szxytkj.cn

Java: catch (IOException | SQLException e) {}
来源：http://oy.hnjuh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wp.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://kf.panjiajie.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://oe.jctech888.com.cn

[H06] 可选值 / 空值安全访问
来源：http://uq.panjiajie.cn

Py:   value = d.get("k") or default
来源：http://rr.hnjuh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://rl.bjjhwx.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bx.yuexingan06.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xq.bookmarksfly.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://rf.panjiajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://wu.yuntaijiaju.cn

Ruby: d&.dig(:a, :b)
来源：http://rg.521024.cn

C#:   obj?.A?.B ?? default
来源：http://ua.asd995.cn

[H07] 断言
来源：http://it.newstarts.cn

Py:   assert x > 0, "必须为正"
来源：http://us.9csxet.cn

PHP:  assert($x > 0);
来源：http://gs.lnxyls.cn

JS:   console.assert(x > 0);
来源：http://lc.9csxet.cn

TS:   console.assert(x > 0);
来源：http://da.hnjuh.cn

Java: assert x > 0 : "必须为正";
来源：http://mq.hnjuh.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://kg.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://af.lnxyls.cn

C#:   Debug.Assert(x > 0);
来源：http://nm.hnjuh.cn

[H08] 获取错误信息与堆栈
来源：http://zx.haigaiapp.cn

Py:   str(e);  traceback.format_exc()
来源：http://gn.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://vw.asd995.cn

JS:   e.message;  e.stack
来源：http://vv.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://he.9csxet.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://va.lnxyls.cn

Go:   err.Error()
来源：http://cf.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://ra.yuntaijiaju.cn

C#:   e.Message;  e.StackTrace
来源：http://pj.huixinmuqiang.cn

[H09] 带错误码的异常
来源：http://ut.wgjwhj.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://qn.nicolike.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wo.newstarts.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://oc.huanxung.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ru.muxihuayi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ah.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hh.shxzskj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://pb.asd995.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://cx.chemitech.net.cn

[H10] 资源自动释放
来源：http://au.shxzukj.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ds.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://xt.chemitech.net.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://bh.huixinmuqiang.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wk.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://yu.szxytkj.cn

Go:   defer f.Close()
来源：http://un.nicolike.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://tb.szsharing.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://vu.shxzskj.cn

================================================================================
来源：http://kl.asd995.cn

I. 正则表达式
来源：http://vf.shtwfgs.cn

================================================================================
来源：http://qh.nicolike.cn

[I01] 判断是否匹配
来源：http://pp.521024.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://cl.hnjuh.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nm.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://xr.yuexingan06.cn

TS:   /\d+/.test(s)
来源：http://yu.hahajie.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tw.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bk.yuexingan06.cn

Ruby: s.match?(/\d+/)
来源：http://vi.huanxung.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://le.hahajie.cn

[I02] 提取所有匹配
来源：http://mc.huixiangedu.cn

Py:   re.findall(r"\d+", s)
来源：http://qg.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://ax.jctech888.com.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://dc.shtwfgs.cn

TS:   s.match(/\d+/g)
来源：http://pm.shxzukj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://cd.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rs.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://da.jianghongdianzi.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://nl.lnxyls.cn

[I03] 提取捕获分组
来源：http://wj.lnxyls.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jx.muxihuayi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://lw.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://pq.shxzskj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://nd.shtwfgs.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://oy.panjiajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://gm.wgjwhj.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://re.asd995.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://jx.yuntaijiaju.cn

[I04] 正则替换
来源：http://va.nicolike.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://uw.shxzskj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wf.chemitech.net.cn

JS:   s.replace(/\d+/g, "#")
来源：http://av.huixinmuqiang.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kl.muxihuayi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ve.jctech888.com.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dy.newstarts.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://aw.gzmigu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://po.colortex.cn

[I05] 按正则拆分
来源：http://tb.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://rg.bookmarksfly.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yp.haigaiapp.cn

JS:   s.split(/\s*,\s*/)
来源：http://rg.huixiangedu.cn

TS:   s.split(/\s*,\s*/)
来源：http://ff.wgjwhj.cn

Java: s.split("\\s*,\\s*")
来源：http://cp.bjjhwx.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ks.bjjhwx.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zy.panjiajie.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wd.nicolike.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hd.521024.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jn.9csxet.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.muxihuayi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://pt.bjjhwx.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://eo.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xc.asd995.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://og.huixinmuqiang.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://jv.haigaiapp.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://sk.shxzskj.cn

[I07] 忽略大小写与多行模式
来源：http://gd.newstarts.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vo.bjjhwx.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bi.muxihuayi.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ef.bjjhwx.cn

TS:   /error/gim
来源：http://cb.gzmigu.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sj.bookmarksfly.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ve.huanxung.cn

Ruby: s.scan(/error/i)
来源：http://fw.asd995.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zu.shxzskj.cn

[I08] 贪婪与非贪婪匹配
来源：http://nj.asd995.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vm.shxzukj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://nf.bjjhwx.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ia.jctech888.com.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lk.hnjuh.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lr.jianghongdianzi.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fo.wgjwhj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://jy.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://we.wgjwhj.cn

================================================================================
来源：http://jg.newstarts.cn

J. 日期与时间
来源：http://th.panjiajie.cn

================================================================================
来源：http://tq.521024.cn

[J01] 获取当前时间
来源：http://ji.nicolike.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://pw.szxytkj.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ii.huanxung.cn

JS:   new Date();  Date.now()
来源：http://pz.huanxung.cn

TS:   new Date();  Date.now()
来源：http://og.huixinmuqiang.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://es.newstarts.cn

Go:   time.Now()
来源：http://qp.szxytkj.cn

Ruby: Time.now
来源：http://uw.hnjuh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://wl.huixinmuqiang.cn

[J02] 格式化输出
来源：http://mi.nszjky.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ax.szxytkj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://vc.szsharing.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ym.shxzskj.cn

TS:   d.toISOString()
来源：http://ia.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gc.shxzskj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vz.lnxyls.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vp.newstarts.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://oi.lnxyls.cn

[J03] 字符串解析为日期
来源：http://oq.bookmarksfly.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://fs.haigaiapp.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yl.szxytkj.cn

JS:   new Date("2024-01-02")
来源：http://zl.muxihuayi.cn

TS:   new Date("2024-01-02")
来源：http://yl.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vw.nicolike.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uq.nszjky.cn

Ruby: Date.parse("2024-01-02")
来源：http://zx.newstarts.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ea.jctech888.com.cn

[J04] 时间戳与日期互转
来源：http://yr.colortex.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ko.chemitech.net.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://in.9csxet.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ms.nszjky.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://lw.shxzskj.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://zx.szsharing.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://ih.521024.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://px.521024.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://tc.jianghongdianzi.cn

[J05] 时间加减（加 7 天）
来源：http://qt.jianghongdianzi.cn

Py:   now + timedelta(days=7)
来源：http://ri.shxzukj.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://sp.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wf.yuexingan06.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://cp.huixiangedu.cn

Java: LocalDate.now().plusDays(7)
来源：http://nj.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ve.huixiangedu.cn

Ruby: Time.now + 7 * 86400
来源：http://gr.haigaiapp.cn

C#:   DateTime.Now.AddDays(7)
来源：http://gr.wgjwhj.cn

[J06] 计算两时间之差
来源：http://sx.nicolike.cn

Py:   (end - start).total_seconds()
来源：http://te.521024.cn

PHP:  $end->diff($start)->days;
来源：http://lp.muxihuayi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pz.huixinmuqiang.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://xd.lnxyls.cn

Java: Duration.between(start, end).toSeconds()
来源：http://qz.panjiajie.cn

Go:   end.Sub(start).Hours()
来源：http://kx.szxytkj.cn

Ruby: end - start                 # 返回秒数
来源：http://hp.shxzskj.cn

C#:   (end - start).TotalSeconds
来源：http://tp.bjjhwx.cn

[J07] 比较两个日期
来源：http://vy.jianghongdianzi.cn

Py:   d1 < d2;  d1 == d2
来源：http://iw.yuexingan06.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vd.chemitech.net.cn

JS:   d1.getTime() < d2.getTime()
来源：http://vn.jctech888.com.cn

TS:   d1.getTime() < d2.getTime()
来源：http://od.nicolike.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ec.nszjky.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dk.huanxung.cn

Ruby: d1 < d2;  d1 == d2
来源：http://mx.huixinmuqiang.cn


<!-- 参考信息 -->