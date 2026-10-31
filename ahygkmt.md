代发 wailian999

Ruby: super
来源：http://vq.huanxung.cn

C#:   base.Greet();
来源：http://ko.9csxet.cn

[G08] 静态方法与属性
来源：http://wc.jctech888.com.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ab.gzmigu.cn

PHP:  public static function f() {}
来源：http://yk.bjjhwx.cn

JS:   static f() {}
来源：http://tk.asd995.cn

TS:   static f(): void {}
来源：http://vi.yuexingan06.cn

Java: static void f() {}
来源：http://sc.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://aj.jctech888.com.cn

Ruby: def self.f; end
来源：http://wd.muxihuayi.cn

C#:   public static void F() {}
来源：http://ry.hnjuh.cn

[G09] 接口 / 抽象类
来源：http://rw.huanxung.cn

Py:   from abc import ABC, abstractmethod
来源：http://di.bookmarksfly.cn

PHP:  interface Shape { public function area(): float; }
来源：http://du.huixinmuqiang.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wc.lnxyls.cn

TS:   interface Shape { area(): number; }
来源：http://we.haigaiapp.cn

Java: interface Shape { double area(); }
来源：http://zj.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://aj.nszjky.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wp.huanxung.cn

C#:   interface IShape { double Area(); }
来源：http://br.shtwfgs.cn

[G10] 访问控制
来源：http://bm.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://ma.szxytkj.cn

PHP:  public / protected / private
来源：http://bm.lnxyls.cn

JS:   #private 字段；其余公开
来源：http://kj.hahajie.cn

TS:   public / protected / private
来源：http://tb.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://tq.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hg.9csxet.cn

Ruby: public / protected / private
来源：http://pj.gzmigu.cn

C#:   public / protected / private / internal
来源：http://qg.9csxet.cn

[G11] getter / setter
来源：http://qm.9csxet.cn

Py:   @property 与 @x.setter
来源：http://lc.521024.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xb.hnjuh.cn

JS:   get name() { return this._name; }
来源：http://hj.huixiangedu.cn

TS:   get name(): string { return this._name; }
来源：http://tp.yuexingan06.cn

Java: public String getName() { return name; }
来源：http://fk.521024.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ut.shxzukj.cn

Ruby: attr_accessor :name
来源：http://ag.panjiajie.cn

C#:   public string Name { get; set; }
来源：http://qt.jianghongdianzi.cn

[G12] 对象转字符串
来源：http://za.gzmigu.cn

Py:   def __str__(self): return self.name
来源：http://cf.huanxung.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ni.9csxet.cn

JS:   toString() { return this.name; }
来源：http://cn.bookmarksfly.cn

TS:   toString(): string { return this.name; }
来源：http://ju.shxzskj.cn

Java: @Override public String toString() { return name; }
来源：http://ge.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kr.huanxung.cn

Ruby: def to_s; @name; end
来源：http://em.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://vt.shtwfgs.cn

[G13] 判断对象类型
来源：http://ty.nszjky.cn

Py:   isinstance(u, User)
来源：http://ib.haigaiapp.cn

PHP:  $u instanceof User
来源：http://lh.gzmigu.cn

JS:   u instanceof User
来源：http://it.9csxet.cn

TS:   u instanceof User
来源：http://he.gzmigu.cn

Java: u instanceof User
来源：http://fs.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ko.szxytkj.cn

Ruby: u.is_a?(User)
来源：http://pv.lnxyls.cn

C#:   u is User
来源：http://uw.szxytkj.cn

[G14] 数据类 / record
来源：http://ni.muxihuayi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bo.shtwfgs.cn

PHP:  // 用 readonly 属性模拟
来源：http://tm.hahajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nd.huixiangedu.cn

TS:   type User = { name: string; age: number };
来源：http://re.colortex.cn

Java: record User(String name, int age) {}
来源：http://xe.chemitech.net.cn

Go:   type User struct { Name string; Age int }
来源：http://bs.chemitech.net.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://sb.newstarts.cn

C#:   record User(string Name, int Age);
来源：http://ef.jctech888.com.cn

[G15] 枚举
来源：http://sn.shtwfgs.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://qf.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://wu.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dt.huixinmuqiang.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://xm.bjjhwx.cn

Java: enum Color { RED, GREEN }
来源：http://eh.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://as.szsharing.cn

Ruby: Color = %i[red green].freeze
来源：http://nn.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://eq.hahajie.cn

[G16] 对象转数组 / 字典
来源：http://ly.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://on.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://sn.bookmarksfly.cn

JS:   Object.entries(obj)
来源：http://ac.9csxet.cn

TS:   Object.entries(obj)
来源：http://fc.shxzukj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cw.521024.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://iw.newstarts.cn

Ruby: obj.instance_variables
来源：http://ey.haigaiapp.cn

C#:   // 用反射或 System.Text.Json
来源：http://nj.jianghongdianzi.cn

================================================================================
来源：http://cu.jctech888.com.cn

H. 异常与错误处理
来源：http://yo.gzmigu.cn

================================================================================
来源：http://gk.jctech888.com.cn

[H01] try / catch 基础
来源：http://cj.nicolike.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jm.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bo.bookmarksfly.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ph.colortex.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://fk.newstarts.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ta.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://tt.9csxet.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qj.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vn.gzmigu.cn

[H02] finally / ensure 收尾
来源：http://ep.yuexingan06.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ss.nszjky.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://wq.shxzukj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mc.9csxet.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qq.szxytkj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ki.asd995.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ut.shxzukj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wa.szsharing.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pq.newstarts.cn

[H03] 主动抛出异常
来源：http://ks.huixiangedu.cn

Py:   raise ValueError("错误信息")
来源：http://av.szxytkj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ys.nszjky.cn

JS:   throw new Error("错误信息");
来源：http://kw.nszjky.cn

TS:   throw new Error("错误信息");
来源：http://hs.haigaiapp.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://wm.yuexingan06.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://xa.lnxyls.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://nw.wgjwhj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gc.hnjuh.cn

[H04] 自定义异常类型
来源：http://en.521024.cn

Py:   class MyError(Exception): pass
来源：http://pa.9csxet.cn

PHP:  class MyError extends RuntimeException {}
来源：http://uf.shxzukj.cn

JS:   class MyError extends Error {}
来源：http://tx.huanxung.cn

TS:   class MyError extends Error {}
来源：http://hp.colortex.cn

Java: class MyException extends RuntimeException {}
来源：http://vj.muxihuayi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://pf.shxzukj.cn

Ruby: class MyError < StandardError; end
来源：http://vt.szsharing.cn

C#:   class MyException : Exception {}
来源：http://ob.huixiangedu.cn

[H05] 捕获特定类型
来源：http://rx.hnjuh.cn

Py:   except ValueError as e:
来源：http://ck.newstarts.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://rx.shtwfgs.cn

JS:   if (e instanceof TypeError) {}
来源：http://tu.hahajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://xt.shtwfgs.cn

Java: catch (IOException | SQLException e) {}
来源：http://hz.jianghongdianzi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://tf.yuexingan06.cn

Ruby: rescue ArgumentError => e
来源：http://gl.muxihuayi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://od.wgjwhj.cn

[H06] 可选值 / 空值安全访问
来源：http://gn.9csxet.cn

Py:   value = d.get("k") or default
来源：http://xm.hahajie.cn

PHP:  $v = $d["k"] ?? null;
来源：http://nc.bookmarksfly.cn

JS:   obj?.a?.b;  d ?? default
来源：http://an.jianghongdianzi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://os.panjiajie.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://am.asd995.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://bu.haigaiapp.cn

Ruby: d&.dig(:a, :b)
来源：http://qd.colortex.cn

C#:   obj?.A?.B ?? default
来源：http://jm.szsharing.cn

[H07] 断言
来源：http://if.huixinmuqiang.cn

Py:   assert x > 0, "必须为正"
来源：http://si.huanxung.cn

PHP:  assert($x > 0);
来源：http://wh.hnjuh.cn

JS:   console.assert(x > 0);
来源：http://ci.shxzskj.cn

TS:   console.assert(x > 0);
来源：http://og.huixiangedu.cn

Java: assert x > 0 : "必须为正";
来源：http://lg.newstarts.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://th.muxihuayi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://uv.lnxyls.cn

C#:   Debug.Assert(x > 0);
来源：http://ex.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://jv.asd995.cn

Py:   str(e);  traceback.format_exc()
来源：http://pm.jianghongdianzi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://bl.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://zq.muxihuayi.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://ok.shtwfgs.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qo.muxihuayi.cn

Go:   err.Error()
来源：http://gl.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://wr.bjjhwx.cn

C#:   e.Message;  e.StackTrace
来源：http://at.yuntaijiaju.cn

[H09] 带错误码的异常
来源：http://wg.yuexingan06.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://xx.huixiangedu.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://qg.yuexingan06.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mo.hnjuh.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hd.asd995.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hf.szxytkj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ov.9csxet.cn

Ruby: raise MyError.new("fail", 500)
来源：http://tv.9csxet.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://oq.jianghongdianzi.cn

[H10] 资源自动释放
来源：http://ul.lnxyls.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://uj.asd995.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://si.bookmarksfly.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://jd.shxzskj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://je.yuntaijiaju.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://oa.nszjky.cn

Go:   defer f.Close()
来源：http://wh.jctech888.com.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://bq.hnjuh.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cm.wgjwhj.cn

================================================================================
来源：http://lo.gzmigu.cn

I. 正则表达式
来源：http://wx.szsharing.cn

================================================================================
来源：http://pv.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://oh.wgjwhj.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://bo.chemitech.net.cn

PHP:  preg_match('/\d+/', $s);
来源：http://yc.szxytkj.cn

JS:   /\d+/.test(s)
来源：http://lz.huixinmuqiang.cn

TS:   /\d+/.test(s)
来源：http://xt.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://eb.panjiajie.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://bp.shxzskj.cn

Ruby: s.match?(/\d+/)
来源：http://ix.colortex.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bp.colortex.cn

[I02] 提取所有匹配
来源：http://vq.shxzukj.cn

Py:   re.findall(r"\d+", s)
来源：http://xp.hahajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://nc.nszjky.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xh.yuntaijiaju.cn

TS:   s.match(/\d+/g)
来源：http://fj.nicolike.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://jk.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pp.panjiajie.cn

Ruby: s.scan(/\d+/)
来源：http://qf.panjiajie.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gd.9csxet.cn

[I03] 提取捕获分组
来源：http://aw.bookmarksfly.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mp.hahajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://qu.yuexingan06.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://il.yuexingan06.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://rw.colortex.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lr.9csxet.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://aw.yuexingan06.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zk.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bj.newstarts.cn

[I04] 正则替换
来源：http://hy.panjiajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://cq.yuntaijiaju.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://fq.nicolike.cn

JS:   s.replace(/\d+/g, "#")
来源：http://xk.huixinmuqiang.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kw.gzmigu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://lc.colortex.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://xx.chemitech.net.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://iz.szsharing.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://fm.yuntaijiaju.cn

[I05] 按正则拆分
来源：http://qc.nicolike.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://du.chemitech.net.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jx.shxzskj.cn

JS:   s.split(/\s*,\s*/)
来源：http://eu.panjiajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://no.colortex.cn

Java: s.split("\\s*,\\s*")
来源：http://vf.9csxet.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ll.nicolike.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ji.huixiangedu.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fq.hnjuh.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zw.jianghongdianzi.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://jq.panjiajie.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://sq.bjjhwx.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://is.nszjky.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gn.haigaiapp.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://dk.hnjuh.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://kc.shxzukj.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://fu.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kj.huixinmuqiang.cn

[I07] 忽略大小写与多行模式
来源：http://kt.nicolike.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://ii.asd995.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://nd.asd995.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://da.nszjky.cn

TS:   /error/gim
来源：http://am.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://do.panjiajie.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fa.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://rf.lnxyls.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ow.huixiangedu.cn

[I08] 贪婪与非贪婪匹配
来源：http://gy.huixinmuqiang.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ds.newstarts.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://bh.gzmigu.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://yc.muxihuayi.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://lx.shtwfgs.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://mq.panjiajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://yj.bookmarksfly.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mg.asd995.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://bk.bookmarksfly.cn

================================================================================
来源：http://jg.szsharing.cn

J. 日期与时间
来源：http://va.jctech888.com.cn

================================================================================
来源：http://ay.asd995.cn

[J01] 获取当前时间
来源：http://qi.bookmarksfly.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://kn.hahajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://uq.nszjky.cn

JS:   new Date();  Date.now()
来源：http://iq.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://bp.bookmarksfly.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://jd.huanxung.cn

Go:   time.Now()
来源：http://mz.muxihuayi.cn

Ruby: Time.now
来源：http://wu.wgjwhj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://du.9csxet.cn

[J02] 格式化输出
来源：http://yb.haigaiapp.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://zb.muxihuayi.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://rn.szsharing.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://df.panjiajie.cn

TS:   d.toISOString()
来源：http://mj.shtwfgs.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://bw.huixinmuqiang.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://li.gzmigu.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://kb.colortex.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://lp.huanxung.cn

[J03] 字符串解析为日期
来源：http://rx.hahajie.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wy.shxzukj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hl.szsharing.cn

JS:   new Date("2024-01-02")
来源：http://en.hahajie.cn

TS:   new Date("2024-01-02")
来源：http://cj.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://vt.shxzskj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://qg.wgjwhj.cn

Ruby: Date.parse("2024-01-02")
来源：http://ty.jctech888.com.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://ws.bookmarksfly.cn

[J04] 时间戳与日期互转
来源：http://gz.haigaiapp.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vn.huixinmuqiang.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://cv.huixinmuqiang.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ew.chemitech.net.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://rx.huixinmuqiang.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://vb.yuexingan06.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hc.colortex.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://kj.jianghongdianzi.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://vy.szxytkj.cn

[J05] 时间加减（加 7 天）
来源：http://mx.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://xv.muxihuayi.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://lk.panjiajie.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ek.shtwfgs.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://zh.hahajie.cn

Java: LocalDate.now().plusDays(7)
来源：http://gz.huanxung.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://kk.asd995.cn

Ruby: Time.now + 7 * 86400
来源：http://or.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://oj.shxzukj.cn

[J06] 计算两时间之差
来源：http://hk.huixinmuqiang.cn


<!-- 参考信息 -->