代发 wailian999

Java: interface Shape { double area(); }
来源：http://qc.9csxet.cn

Go:   type Shape interface { Area() float64 }
来源：http://bt.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oy.wgjwhj.cn

C#:   interface IShape { double Area(); }
来源：http://yb.haigaiapp.cn

[G10] 访问控制
来源：http://hy.colortex.cn

Py:   约定 _protected / __private（不强制）
来源：http://ne.chemitech.net.cn

PHP:  public / protected / private
来源：http://uc.huixiangedu.cn

JS:   #private 字段；其余公开
来源：http://dk.shtwfgs.cn

TS:   public / protected / private
来源：http://if.chemitech.net.cn

Java: public / protected / private / 默认包级
来源：http://pw.nicolike.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fz.huixinmuqiang.cn

Ruby: public / protected / private
来源：http://rr.yuntaijiaju.cn

C#:   public / protected / private / internal
来源：http://tt.wgjwhj.cn

[G11] getter / setter
来源：http://xf.huixiangedu.cn

Py:   @property 与 @x.setter
来源：http://gv.wgjwhj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://su.nszjky.cn

JS:   get name() { return this._name; }
来源：http://tp.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://ay.newstarts.cn

Java: public String getName() { return name; }
来源：http://xk.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rg.huixinmuqiang.cn

Ruby: attr_accessor :name
来源：http://mr.bookmarksfly.cn

C#:   public string Name { get; set; }
来源：http://ey.9csxet.cn

[G12] 对象转字符串
来源：http://yd.wgjwhj.cn

Py:   def __str__(self): return self.name
来源：http://xd.huixinmuqiang.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tr.yuntaijiaju.cn

JS:   toString() { return this.name; }
来源：http://ot.chemitech.net.cn

TS:   toString(): string { return this.name; }
来源：http://th.gzmigu.cn

Java: @Override public String toString() { return name; }
来源：http://hq.huanxung.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xb.gzmigu.cn

Ruby: def to_s; @name; end
来源：http://nh.panjiajie.cn

C#:   public override string ToString() => Name;
来源：http://qm.shtwfgs.cn

[G13] 判断对象类型
来源：http://kx.yuntaijiaju.cn

Py:   isinstance(u, User)
来源：http://re.bookmarksfly.cn

PHP:  $u instanceof User
来源：http://fc.muxihuayi.cn

JS:   u instanceof User
来源：http://wo.panjiajie.cn

TS:   u instanceof User
来源：http://pq.szsharing.cn

Java: u instanceof User
来源：http://ye.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sz.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://hx.hahajie.cn

C#:   u is User
来源：http://fk.yuntaijiaju.cn

[G14] 数据类 / record
来源：http://ec.jianghongdianzi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ro.panjiajie.cn

PHP:  // 用 readonly 属性模拟
来源：http://ob.yuntaijiaju.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xz.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://hy.521024.cn

Java: record User(String name, int age) {}
来源：http://cn.huixiangedu.cn

Go:   type User struct { Name string; Age int }
来源：http://co.huixiangedu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nh.szxytkj.cn

C#:   record User(string Name, int Age);
来源：http://fv.szxytkj.cn

[G15] 枚举
来源：http://vu.muxihuayi.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://tf.hahajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ue.shxzukj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://th.haigaiapp.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://sp.shtwfgs.cn

Java: enum Color { RED, GREEN }
来源：http://al.gzmigu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ke.yuexingan06.cn

Ruby: Color = %i[red green].freeze
来源：http://yd.nicolike.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://he.colortex.cn

[G16] 对象转数组 / 字典
来源：http://zy.huixiangedu.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ye.jianghongdianzi.cn

PHP:  get_object_vars($obj);
来源：http://bc.lnxyls.cn

JS:   Object.entries(obj)
来源：http://uz.shxzukj.cn

TS:   Object.entries(obj)
来源：http://gf.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gv.asd995.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://go.asd995.cn

Ruby: obj.instance_variables
来源：http://sa.9csxet.cn

C#:   // 用反射或 System.Text.Json
来源：http://jx.521024.cn

================================================================================
来源：http://dd.szsharing.cn

H. 异常与错误处理
来源：http://sa.panjiajie.cn

================================================================================
来源：http://vx.szsharing.cn

[H01] try / catch 基础
来源：http://bz.colortex.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://fw.shtwfgs.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wv.nszjky.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://py.huixiangedu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://jq.chemitech.net.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tk.nicolike.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iw.muxihuayi.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://la.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://om.huixinmuqiang.cn

[H02] finally / ensure 收尾
来源：http://uc.gzmigu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://yw.bookmarksfly.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://hs.hahajie.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ap.asd995.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://tq.bjjhwx.cn

Java: try { f(); } finally { cleanup(); }
来源：http://sf.huixinmuqiang.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qu.9csxet.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://fp.szxytkj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://es.shxzukj.cn

[H03] 主动抛出异常
来源：http://xg.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://xl.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://nc.hahajie.cn

JS:   throw new Error("错误信息");
来源：http://yz.nszjky.cn

TS:   throw new Error("错误信息");
来源：http://ls.hnjuh.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://yk.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fm.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ha.haigaiapp.cn

C#:   throw new ArgumentException("错误信息");
来源：http://qt.huixinmuqiang.cn

[H04] 自定义异常类型
来源：http://mk.newstarts.cn

Py:   class MyError(Exception): pass
来源：http://jg.huixinmuqiang.cn

PHP:  class MyError extends RuntimeException {}
来源：http://mr.szxytkj.cn

JS:   class MyError extends Error {}
来源：http://iu.szsharing.cn

TS:   class MyError extends Error {}
来源：http://eb.muxihuayi.cn

Java: class MyException extends RuntimeException {}
来源：http://ld.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nz.haigaiapp.cn

Ruby: class MyError < StandardError; end
来源：http://by.huanxung.cn

C#:   class MyException : Exception {}
来源：http://zd.nicolike.cn

[H05] 捕获特定类型
来源：http://aa.yuexingan06.cn

Py:   except ValueError as e:
来源：http://wy.szxytkj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://px.huixinmuqiang.cn

JS:   if (e instanceof TypeError) {}
来源：http://df.muxihuayi.cn

TS:   if (e instanceof TypeError) {}
来源：http://en.nszjky.cn

Java: catch (IOException | SQLException e) {}
来源：http://zq.huixiangedu.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://qw.hahajie.cn

Ruby: rescue ArgumentError => e
来源：http://iy.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ab.shxzukj.cn

[H06] 可选值 / 空值安全访问
来源：http://rr.hahajie.cn

Py:   value = d.get("k") or default
来源：http://nx.9csxet.cn

PHP:  $v = $d["k"] ?? null;
来源：http://hs.jianghongdianzi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://js.hahajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://yz.shxzukj.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://fj.jianghongdianzi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://js.hnjuh.cn

Ruby: d&.dig(:a, :b)
来源：http://ya.yuntaijiaju.cn

C#:   obj?.A?.B ?? default
来源：http://wk.huixiangedu.cn

[H07] 断言
来源：http://qr.bjjhwx.cn

Py:   assert x > 0, "必须为正"
来源：http://pb.9csxet.cn

PHP:  assert($x > 0);
来源：http://ia.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://na.szxytkj.cn

TS:   console.assert(x > 0);
来源：http://ny.szxytkj.cn

Java: assert x > 0 : "必须为正";
来源：http://vx.szxytkj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://tq.jctech888.com.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vr.asd995.cn

C#:   Debug.Assert(x > 0);
来源：http://bd.hahajie.cn

[H08] 获取错误信息与堆栈
来源：http://qr.shxzukj.cn

Py:   str(e);  traceback.format_exc()
来源：http://ns.yuntaijiaju.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://cr.asd995.cn

JS:   e.message;  e.stack
来源：http://ob.gzmigu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qt.szxytkj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qo.bookmarksfly.cn

Go:   err.Error()
来源：http://am.nszjky.cn

Ruby: e.message;  e.backtrace
来源：http://kv.9csxet.cn

C#:   e.Message;  e.StackTrace
来源：http://nq.huixinmuqiang.cn

[H09] 带错误码的异常
来源：http://zf.szsharing.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wn.chemitech.net.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://te.521024.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wi.asd995.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hu.jctech888.com.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://ol.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://kj.bookmarksfly.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ax.hahajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://di.hnjuh.cn

[H10] 资源自动释放
来源：http://av.newstarts.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://hx.jianghongdianzi.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yk.jctech888.com.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://eq.asd995.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ns.asd995.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://zb.yuntaijiaju.cn

Go:   defer f.Close()
来源：http://rd.huixiangedu.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qu.jctech888.com.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ss.muxihuayi.cn

================================================================================
来源：http://cm.shxzukj.cn

I. 正则表达式
来源：http://dh.nicolike.cn

================================================================================
来源：http://kw.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://wc.bjjhwx.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://br.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wx.colortex.cn

JS:   /\d+/.test(s)
来源：http://cp.huixinmuqiang.cn

TS:   /\d+/.test(s)
来源：http://ze.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://et.chemitech.net.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://fn.asd995.cn

Ruby: s.match?(/\d+/)
来源：http://rn.bjjhwx.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gx.shxzukj.cn

[I02] 提取所有匹配
来源：http://hp.muxihuayi.cn

Py:   re.findall(r"\d+", s)
来源：http://nd.shxzukj.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://xc.huanxung.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://em.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://aq.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://or.wgjwhj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rz.9csxet.cn

Ruby: s.scan(/\d+/)
来源：http://lq.haigaiapp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rj.jianghongdianzi.cn

[I03] 提取捕获分组
来源：http://xs.newstarts.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://vm.panjiajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://vz.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://vr.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ni.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wf.jctech888.com.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://bz.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hm.muxihuayi.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://cf.hnjuh.cn

[I04] 正则替换
来源：http://wl.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rh.shxzskj.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://qx.newstarts.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zz.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tk.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ix.jctech888.com.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://oc.haigaiapp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://xf.521024.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://eh.haigaiapp.cn

[I05] 按正则拆分
来源：http://ua.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://qf.huanxung.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qq.muxihuayi.cn

JS:   s.split(/\s*,\s*/)
来源：http://tr.shxzukj.cn

TS:   s.split(/\s*,\s*/)
来源：http://pd.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://rp.haigaiapp.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://yv.bookmarksfly.cn

Ruby: s.split(/\s*,\s*/)
来源：http://zt.jianghongdianzi.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://le.bjjhwx.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ia.yuexingan06.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://dh.newstarts.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://ob.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://kg.lnxyls.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vi.bookmarksfly.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://bs.shtwfgs.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uh.wgjwhj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://wz.huanxung.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://qj.szsharing.cn

[I07] 忽略大小写与多行模式
来源：http://aq.gzmigu.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://df.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://io.szsharing.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://fj.shxzskj.cn

TS:   /error/gim
来源：http://po.hahajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://cp.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://ai.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://ov.lnxyls.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://bs.nszjky.cn

[I08] 贪婪与非贪婪匹配
来源：http://jv.hahajie.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ue.chemitech.net.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://dw.muxihuayi.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ln.hnjuh.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://pf.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cg.nszjky.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fd.shxzskj.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://nr.huixinmuqiang.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://pv.huixinmuqiang.cn

================================================================================
来源：http://lc.bjjhwx.cn

J. 日期与时间
来源：http://md.yuexingan06.cn

================================================================================
来源：http://er.nszjky.cn

[J01] 获取当前时间
来源：http://sy.asd995.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://mh.shtwfgs.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uv.bookmarksfly.cn

JS:   new Date();  Date.now()
来源：http://hu.jianghongdianzi.cn

TS:   new Date();  Date.now()
来源：http://hu.521024.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://eb.colortex.cn

Go:   time.Now()
来源：http://xr.newstarts.cn

Ruby: Time.now
来源：http://st.newstarts.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://sk.521024.cn

[J02] 格式化输出
来源：http://hv.lnxyls.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bg.wgjwhj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://nq.shtwfgs.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://vx.nszjky.cn

TS:   d.toISOString()
来源：http://jn.haigaiapp.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://az.wgjwhj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xk.521024.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://aq.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://pt.hnjuh.cn

[J03] 字符串解析为日期
来源：http://gl.chemitech.net.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://th.huixiangedu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://yp.bjjhwx.cn

JS:   new Date("2024-01-02")
来源：http://dt.521024.cn

TS:   new Date("2024-01-02")
来源：http://ow.yuntaijiaju.cn

Java: LocalDate.parse("2024-01-02")
来源：http://ek.newstarts.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://zu.muxihuayi.cn

Ruby: Date.parse("2024-01-02")
来源：http://rs.haigaiapp.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ys.huixinmuqiang.cn

[J04] 时间戳与日期互转
来源：http://ga.yuntaijiaju.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://de.colortex.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ex.wgjwhj.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://mk.shtwfgs.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://gr.jianghongdianzi.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://sm.huixinmuqiang.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://sn.gzmigu.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://qb.lnxyls.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ci.panjiajie.cn

[J05] 时间加减（加 7 天）
来源：http://dt.nicolike.cn

Py:   now + timedelta(days=7)
来源：http://oe.shtwfgs.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://xq.lnxyls.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://mr.jctech888.com.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://vo.nicolike.cn

Java: LocalDate.now().plusDays(7)
来源：http://vc.jianghongdianzi.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://in.haigaiapp.cn

Ruby: Time.now + 7 * 86400
来源：http://qt.hahajie.cn

C#:   DateTime.Now.AddDays(7)
来源：http://rq.hahajie.cn

[J06] 计算两时间之差
来源：http://gz.shtwfgs.cn

Py:   (end - start).total_seconds()
来源：http://co.yuexingan06.cn

PHP:  $end->diff($start)->days;
来源：http://me.shxzskj.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://xk.shtwfgs.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://fo.hnjuh.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ow.huanxung.cn

Go:   end.Sub(start).Hours()
来源：http://fe.panjiajie.cn

Ruby: end - start                 # 返回秒数
来源：http://ms.hnjuh.cn

C#:   (end - start).TotalSeconds
来源：http://hn.huanxung.cn

[J07] 比较两个日期
来源：http://dq.wgjwhj.cn

Py:   d1 < d2;  d1 == d2
来源：http://dz.chemitech.net.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mo.asd995.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tm.haigaiapp.cn

TS:   d1.getTime() < d2.getTime()
来源：http://pr.muxihuayi.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://yd.nszjky.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gs.bookmarksfly.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tg.muxihuayi.cn


<!-- 参考信息 -->