代发 wailian999

Ruby: super
来源：http://fe.bjjhwx.cn

C#:   base.Greet();
来源：http://zm.9csxet.cn

[G08] 静态方法与属性
来源：http://js.hnjuh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ug.huanxung.cn

PHP:  public static function f() {}
来源：http://pk.nszjky.cn

JS:   static f() {}
来源：http://ku.haigaiapp.cn

TS:   static f(): void {}
来源：http://wx.bjjhwx.cn

Java: static void f() {}
来源：http://fx.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://hw.wgjwhj.cn

Ruby: def self.f; end
来源：http://mi.huixinmuqiang.cn

C#:   public static void F() {}
来源：http://tt.nicolike.cn

[G09] 接口 / 抽象类
来源：http://mm.nicolike.cn

Py:   from abc import ABC, abstractmethod
来源：http://nw.panjiajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vm.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://wr.bjjhwx.cn

TS:   interface Shape { area(): number; }
来源：http://iz.wgjwhj.cn

Java: interface Shape { double area(); }
来源：http://bs.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://lp.yuexingan06.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ms.huixiangedu.cn

C#:   interface IShape { double Area(); }
来源：http://oh.panjiajie.cn

[G10] 访问控制
来源：http://xj.jctech888.com.cn

Py:   约定 _protected / __private（不强制）
来源：http://fr.lnxyls.cn

PHP:  public / protected / private
来源：http://kg.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://tm.chemitech.net.cn

TS:   public / protected / private
来源：http://xe.gzmigu.cn

Java: public / protected / private / 默认包级
来源：http://zq.shxzskj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lp.szxytkj.cn

Ruby: public / protected / private
来源：http://bi.shtwfgs.cn

C#:   public / protected / private / internal
来源：http://fx.yuexingan06.cn

[G11] getter / setter
来源：http://rm.bookmarksfly.cn

Py:   @property 与 @x.setter
来源：http://ty.521024.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hw.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://oj.9csxet.cn

TS:   get name(): string { return this._name; }
来源：http://vh.shxzukj.cn

Java: public String getName() { return name; }
来源：http://vr.panjiajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://zz.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://xx.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://uw.newstarts.cn

[G12] 对象转字符串
来源：http://ll.521024.cn

Py:   def __str__(self): return self.name
来源：http://wo.jianghongdianzi.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://gq.huixiangedu.cn

JS:   toString() { return this.name; }
来源：http://wv.521024.cn

TS:   toString(): string { return this.name; }
来源：http://iq.jctech888.com.cn

Java: @Override public String toString() { return name; }
来源：http://tx.9csxet.cn

Go:   func (u User) String() string { return u.Name }
来源：http://nj.gzmigu.cn

Ruby: def to_s; @name; end
来源：http://mr.bookmarksfly.cn

C#:   public override string ToString() => Name;
来源：http://lz.szxytkj.cn

[G13] 判断对象类型
来源：http://vv.jctech888.com.cn

Py:   isinstance(u, User)
来源：http://kt.nicolike.cn

PHP:  $u instanceof User
来源：http://iu.colortex.cn

JS:   u instanceof User
来源：http://sv.shxzukj.cn

TS:   u instanceof User
来源：http://au.shxzskj.cn

Java: u instanceof User
来源：http://az.newstarts.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xa.asd995.cn

Ruby: u.is_a?(User)
来源：http://df.huanxung.cn

C#:   u is User
来源：http://zb.yuexingan06.cn

[G14] 数据类 / record
来源：http://zw.szxytkj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kp.colortex.cn

PHP:  // 用 readonly 属性模拟
来源：http://hc.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://hp.yuexingan06.cn

TS:   type User = { name: string; age: number };
来源：http://gx.hnjuh.cn

Java: record User(String name, int age) {}
来源：http://pz.szxytkj.cn

Go:   type User struct { Name string; Age int }
来源：http://rl.521024.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dj.huixinmuqiang.cn

C#:   record User(string Name, int Age);
来源：http://fp.shtwfgs.cn

[G15] 枚举
来源：http://kz.chemitech.net.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://dw.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://vt.wgjwhj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lv.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://gq.jctech888.com.cn

Java: enum Color { RED, GREEN }
来源：http://sf.muxihuayi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://xh.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://qb.nicolike.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oc.jianghongdianzi.cn

[G16] 对象转数组 / 字典
来源：http://si.yuexingan06.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ie.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://uf.yuexingan06.cn

JS:   Object.entries(obj)
来源：http://aw.jianghongdianzi.cn

TS:   Object.entries(obj)
来源：http://bm.panjiajie.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ka.muxihuayi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://am.9csxet.cn

Ruby: obj.instance_variables
来源：http://mr.jianghongdianzi.cn

C#:   // 用反射或 System.Text.Json
来源：http://lp.huixiangedu.cn

================================================================================
来源：http://ai.shxzukj.cn

H. 异常与错误处理
来源：http://uk.jianghongdianzi.cn

================================================================================
来源：http://zp.yuexingan06.cn

[H01] try / catch 基础
来源：http://hi.shxzukj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://aj.shxzukj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://ml.9csxet.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rd.yuexingan06.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cx.521024.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://an.yuexingan06.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nq.yuntaijiaju.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://aa.huixiangedu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://vp.hahajie.cn

[H02] finally / ensure 收尾
来源：http://gk.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ud.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pz.szsharing.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sy.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vq.huixinmuqiang.cn

Java: try { f(); } finally { cleanup(); }
来源：http://gd.newstarts.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zf.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://xw.panjiajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pq.jctech888.com.cn

[H03] 主动抛出异常
来源：http://jg.gzmigu.cn

Py:   raise ValueError("错误信息")
来源：http://vi.asd995.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sy.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://xj.colortex.cn

TS:   throw new Error("错误信息");
来源：http://ca.chemitech.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fm.huixinmuqiang.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://rp.jianghongdianzi.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://tv.nszjky.cn

C#:   throw new ArgumentException("错误信息");
来源：http://pi.huixiangedu.cn

[H04] 自定义异常类型
来源：http://ie.jctech888.com.cn

Py:   class MyError(Exception): pass
来源：http://re.jianghongdianzi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://lz.huixinmuqiang.cn

JS:   class MyError extends Error {}
来源：http://ql.shxzukj.cn

TS:   class MyError extends Error {}
来源：http://vp.jianghongdianzi.cn

Java: class MyException extends RuntimeException {}
来源：http://az.muxihuayi.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://uu.lnxyls.cn

Ruby: class MyError < StandardError; end
来源：http://ya.jctech888.com.cn

C#:   class MyException : Exception {}
来源：http://qy.asd995.cn

[H05] 捕获特定类型
来源：http://oj.nszjky.cn

Py:   except ValueError as e:
来源：http://uc.521024.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hg.shxzskj.cn

JS:   if (e instanceof TypeError) {}
来源：http://bu.shxzskj.cn

TS:   if (e instanceof TypeError) {}
来源：http://pa.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://vg.hnjuh.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zy.yuexingan06.cn

Ruby: rescue ArgumentError => e
来源：http://kh.jianghongdianzi.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://pm.haigaiapp.cn

[H06] 可选值 / 空值安全访问
来源：http://cx.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://yt.shtwfgs.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cw.haigaiapp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bc.bookmarksfly.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xe.yuexingan06.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://jy.gzmigu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ur.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://mn.nicolike.cn

C#:   obj?.A?.B ?? default
来源：http://ix.bjjhwx.cn

[H07] 断言
来源：http://zn.huixinmuqiang.cn

Py:   assert x > 0, "必须为正"
来源：http://ib.szsharing.cn

PHP:  assert($x > 0);
来源：http://bm.huixiangedu.cn

JS:   console.assert(x > 0);
来源：http://ep.huixinmuqiang.cn

TS:   console.assert(x > 0);
来源：http://qk.shxzskj.cn

Java: assert x > 0 : "必须为正";
来源：http://vz.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wn.shxzukj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://vv.shxzukj.cn

C#:   Debug.Assert(x > 0);
来源：http://qr.huixinmuqiang.cn

[H08] 获取错误信息与堆栈
来源：http://tx.shtwfgs.cn

Py:   str(e);  traceback.format_exc()
来源：http://hz.wgjwhj.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mz.yuexingan06.cn

JS:   e.message;  e.stack
来源：http://yy.521024.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://na.muxihuayi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://ae.nszjky.cn

Go:   err.Error()
来源：http://qh.lnxyls.cn

Ruby: e.message;  e.backtrace
来源：http://th.yuntaijiaju.cn

C#:   e.Message;  e.StackTrace
来源：http://vm.colortex.cn

[H09] 带错误码的异常
来源：http://gq.bjjhwx.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://or.9csxet.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://gv.newstarts.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://ip.hahajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pm.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://kh.yuntaijiaju.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ci.nicolike.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fl.colortex.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://gy.szxytkj.cn

[H10] 资源自动释放
来源：http://ef.chemitech.net.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://jv.wgjwhj.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ph.9csxet.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hl.gzmigu.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xe.nicolike.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://fn.haigaiapp.cn

Go:   defer f.Close()
来源：http://gx.shtwfgs.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ts.nszjky.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mi.shxzukj.cn

================================================================================
来源：http://gq.yuexingan06.cn

I. 正则表达式
来源：http://fk.huixiangedu.cn

================================================================================
来源：http://mp.gzmigu.cn

[I01] 判断是否匹配
来源：http://ih.hahajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sc.huixiangedu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://ec.haigaiapp.cn

JS:   /\d+/.test(s)
来源：http://sx.bjjhwx.cn

TS:   /\d+/.test(s)
来源：http://gn.chemitech.net.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ia.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jctech888.com.cn

Ruby: s.match?(/\d+/)
来源：http://ko.shxzukj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://op.yuntaijiaju.cn

[I02] 提取所有匹配
来源：http://le.jianghongdianzi.cn

Py:   re.findall(r"\d+", s)
来源：http://ai.huixiangedu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://bz.bookmarksfly.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://te.colortex.cn

TS:   s.match(/\d+/g)
来源：http://wq.521024.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hd.521024.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://tb.bjjhwx.cn

Ruby: s.scan(/\d+/)
来源：http://st.yuexingan06.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://sc.bjjhwx.cn

[I03] 提取捕获分组
来源：http://qn.yuexingan06.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sy.szxytkj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://ze.shtwfgs.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wo.szsharing.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://up.huanxung.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://zx.panjiajie.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://fq.bookmarksfly.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://sx.panjiajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://sf.szxytkj.cn

[I04] 正则替换
来源：http://qx.shtwfgs.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://wf.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hp.nszjky.cn

JS:   s.replace(/\d+/g, "#")
来源：http://sl.521024.cn

TS:   s.replace(/\d+/g, "#")
来源：http://xo.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pl.hnjuh.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://zy.wgjwhj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://rn.gzmigu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://tw.nicolike.cn

[I05] 按正则拆分
来源：http://at.colortex.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://xa.jctech888.com.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://bg.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://ru.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://ds.bjjhwx.cn

Java: s.split("\\s*,\\s*")
来源：http://me.jctech888.com.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ha.bookmarksfly.cn

Ruby: s.split(/\s*,\s*/)
来源：http://qg.bjjhwx.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://vb.szsharing.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ew.nicolike.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://fw.nszjky.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uz.szsharing.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hr.bookmarksfly.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tp.yuntaijiaju.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uj.chemitech.net.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hu.bookmarksfly.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://we.hnjuh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://pd.wgjwhj.cn

[I07] 忽略大小写与多行模式
来源：http://hv.szsharing.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hj.panjiajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://gj.bookmarksfly.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://up.yuntaijiaju.cn

TS:   /error/gim
来源：http://bz.hahajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://oj.521024.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://jz.muxihuayi.cn

Ruby: s.scan(/error/i)
来源：http://pf.521024.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ht.gzmigu.cn

[I08] 贪婪与非贪婪匹配
来源：http://li.huanxung.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ze.hahajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://vh.colortex.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://jr.haigaiapp.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xk.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://cd.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fn.jctech888.com.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ys.haigaiapp.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://up.panjiajie.cn

================================================================================
来源：http://bs.chemitech.net.cn

J. 日期与时间
来源：http://vb.szxytkj.cn

================================================================================
来源：http://jx.huixiangedu.cn

[J01] 获取当前时间
来源：http://eo.szxytkj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://il.panjiajie.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://in.chemitech.net.cn

JS:   new Date();  Date.now()
来源：http://zc.yuexingan06.cn

TS:   new Date();  Date.now()
来源：http://ei.jianghongdianzi.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lo.521024.cn

Go:   time.Now()
来源：http://qb.yuntaijiaju.cn

Ruby: Time.now
来源：http://gc.colortex.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ij.muxihuayi.cn

[J02] 格式化输出
来源：http://ib.9csxet.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://sf.hnjuh.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://qr.shxzukj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wd.asd995.cn

TS:   d.toISOString()
来源：http://kq.jctech888.com.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://vk.nicolike.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://wd.hnjuh.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://mq.jianghongdianzi.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://rr.szxytkj.cn

[J03] 字符串解析为日期
来源：http://lq.huixiangedu.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://cx.gzmigu.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://gj.shxzskj.cn

JS:   new Date("2024-01-02")
来源：http://zu.nicolike.cn

TS:   new Date("2024-01-02")
来源：http://jh.chemitech.net.cn

Java: LocalDate.parse("2024-01-02")
来源：http://qw.panjiajie.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://uw.haigaiapp.cn

Ruby: Date.parse("2024-01-02")
来源：http://et.colortex.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://uc.panjiajie.cn

[J04] 时间戳与日期互转
来源：http://rh.huanxung.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ec.yuexingan06.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://vm.chemitech.net.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://zm.huixinmuqiang.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://xz.lnxyls.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://oj.hahajie.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://gd.9csxet.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wz.panjiajie.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ns.colortex.cn

[J05] 时间加减（加 7 天）
来源：http://ch.haigaiapp.cn

Py:   now + timedelta(days=7)
来源：http://qy.lnxyls.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://gk.shxzukj.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://ln.jianghongdianzi.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://qz.chemitech.net.cn

Java: LocalDate.now().plusDays(7)
来源：http://fb.colortex.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://ym.chemitech.net.cn

Ruby: Time.now + 7 * 86400
来源：http://zy.szxytkj.cn

C#:   DateTime.Now.AddDays(7)
来源：http://fv.jctech888.com.cn

[J06] 计算两时间之差
来源：http://tr.colortex.cn


<!-- 参考信息 -->