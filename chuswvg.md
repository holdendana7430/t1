代发 wailian999

Ruby: @name = "x"
来源：http://lq.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://ab.huixiangedu.cn

[G04] 定义方法
来源：http://px.bookmarksfly.cn

Py:   def greet(self): return self.name
来源：http://ki.haigaiapp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://us.lnxyls.cn

JS:   greet() { return this.name; }
来源：http://nc.colortex.cn

TS:   greet(): string { return this.name; }
来源：http://bk.yuexingan06.cn

Java: String greet() { return name; }
来源：http://bd.shtwfgs.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ix.nszjky.cn

Ruby: def greet; @name; end
来源：http://qa.colortex.cn

C#:   public string Greet() => Name;
来源：http://jl.chemitech.net.cn

[G05] 继承
来源：http://yb.9csxet.cn

Py:   class Admin(User): pass
来源：http://cg.shtwfgs.cn

PHP:  class Admin extends User {}
来源：http://yh.chemitech.net.cn

JS:   class Admin extends User {}
来源：http://cz.521024.cn

TS:   class Admin extends User {}
来源：http://wo.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://cg.colortex.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gs.szsharing.cn

Ruby: class Admin < User; end
来源：http://gy.asd995.cn

C#:   class Admin : User {}
来源：http://ni.shxzskj.cn

[G06] 重写方法
来源：http://si.yuexingan06.cn

Py:   def greet(self): return "admin"
来源：http://up.panjiajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://la.newstarts.cn

JS:   greet() { return "admin"; }
来源：http://vb.nszjky.cn

TS:   greet(): string { return "admin"; }
来源：http://ix.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://tl.bookmarksfly.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fs.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://aa.jctech888.com.cn

C#:   public override string Greet() => "admin";
来源：http://yw.bookmarksfly.cn

[G07] 调用父类方法
来源：http://el.szsharing.cn

Py:   super().greet()
来源：http://ew.panjiajie.cn

PHP:  parent::greet();
来源：http://vq.huixinmuqiang.cn

JS:   super.greet();
来源：http://nu.jctech888.com.cn

TS:   super.greet();
来源：http://vw.hnjuh.cn

Java: super.greet();
来源：http://bt.9csxet.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gy.szsharing.cn

Ruby: super
来源：http://nx.shxzskj.cn

C#:   base.Greet();
来源：http://oq.newstarts.cn

[G08] 静态方法与属性
来源：http://rm.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://al.szsharing.cn

PHP:  public static function f() {}
来源：http://ph.newstarts.cn

JS:   static f() {}
来源：http://qk.shxzskj.cn

TS:   static f(): void {}
来源：http://eu.nicolike.cn

Java: static void f() {}
来源：http://xe.yuntaijiaju.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xn.nszjky.cn

Ruby: def self.f; end
来源：http://rv.muxihuayi.cn

C#:   public static void F() {}
来源：http://uo.chemitech.net.cn

[G09] 接口 / 抽象类
来源：http://nn.bjjhwx.cn

Py:   from abc import ABC, abstractmethod
来源：http://gp.521024.cn

PHP:  interface Shape { public function area(): float; }
来源：http://dt.szxytkj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xz.nszjky.cn

TS:   interface Shape { area(): number; }
来源：http://ug.muxihuayi.cn

Java: interface Shape { double area(); }
来源：http://gd.jctech888.com.cn

Go:   type Shape interface { Area() float64 }
来源：http://mp.huixiangedu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ac.muxihuayi.cn

C#:   interface IShape { double Area(); }
来源：http://bl.jianghongdianzi.cn

[G10] 访问控制
来源：http://yx.jianghongdianzi.cn

Py:   约定 _protected / __private（不强制）
来源：http://qi.muxihuayi.cn

PHP:  public / protected / private
来源：http://oj.wgjwhj.cn

JS:   #private 字段；其余公开
来源：http://wc.panjiajie.cn

TS:   public / protected / private
来源：http://qu.chemitech.net.cn

Java: public / protected / private / 默认包级
来源：http://id.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://su.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://xn.huanxung.cn

C#:   public / protected / private / internal
来源：http://dt.haigaiapp.cn

[G11] getter / setter
来源：http://vs.colortex.cn

Py:   @property 与 @x.setter
来源：http://jy.newstarts.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xz.jianghongdianzi.cn

JS:   get name() { return this._name; }
来源：http://sf.shxzukj.cn

TS:   get name(): string { return this._name; }
来源：http://qv.521024.cn

Java: public String getName() { return name; }
来源：http://wd.jctech888.com.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ac.szxytkj.cn

Ruby: attr_accessor :name
来源：http://pb.shxzskj.cn

C#:   public string Name { get; set; }
来源：http://lo.hnjuh.cn

[G12] 对象转字符串
来源：http://zw.wgjwhj.cn

Py:   def __str__(self): return self.name
来源：http://pq.hahajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://xy.huixinmuqiang.cn

JS:   toString() { return this.name; }
来源：http://ae.szsharing.cn

TS:   toString(): string { return this.name; }
来源：http://lc.jctech888.com.cn

Java: @Override public String toString() { return name; }
来源：http://co.lnxyls.cn

Go:   func (u User) String() string { return u.Name }
来源：http://bd.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://hj.bjjhwx.cn

C#:   public override string ToString() => Name;
来源：http://yh.huixiangedu.cn

[G13] 判断对象类型
来源：http://ji.shxzskj.cn

Py:   isinstance(u, User)
来源：http://co.huixiangedu.cn

PHP:  $u instanceof User
来源：http://cz.521024.cn

JS:   u instanceof User
来源：http://ol.muxihuayi.cn

TS:   u instanceof User
来源：http://ox.gzmigu.cn

Java: u instanceof User
来源：http://kn.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://py.huixinmuqiang.cn

Ruby: u.is_a?(User)
来源：http://jg.nszjky.cn

C#:   u is User
来源：http://cc.wgjwhj.cn

[G14] 数据类 / record
来源：http://oa.haigaiapp.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bf.chemitech.net.cn

PHP:  // 用 readonly 属性模拟
来源：http://fz.shtwfgs.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uk.nszjky.cn

TS:   type User = { name: string; age: number };
来源：http://xq.huixiangedu.cn

Java: record User(String name, int age) {}
来源：http://mt.lnxyls.cn

Go:   type User struct { Name string; Age int }
来源：http://ls.haigaiapp.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://uk.huanxung.cn

C#:   record User(string Name, int Age);
来源：http://ii.521024.cn

[G15] 枚举
来源：http://rz.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://om.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://zo.nicolike.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ah.nszjky.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ah.hnjuh.cn

Java: enum Color { RED, GREEN }
来源：http://ts.huanxung.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.szsharing.cn

Ruby: Color = %i[red green].freeze
来源：http://ar.bjjhwx.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oh.panjiajie.cn

[G16] 对象转数组 / 字典
来源：http://fd.colortex.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ve.panjiajie.cn

PHP:  get_object_vars($obj);
来源：http://wk.bjjhwx.cn

JS:   Object.entries(obj)
来源：http://lp.hahajie.cn

TS:   Object.entries(obj)
来源：http://bl.bjjhwx.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gd.muxihuayi.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://xe.shtwfgs.cn

Ruby: obj.instance_variables
来源：http://xp.nszjky.cn

C#:   // 用反射或 System.Text.Json
来源：http://db.shxzukj.cn

================================================================================
来源：http://cl.newstarts.cn

H. 异常与错误处理
来源：http://mc.gzmigu.cn

================================================================================
来源：http://bj.huixiangedu.cn

[H01] try / catch 基础
来源：http://qu.huanxung.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://tr.wgjwhj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://tc.newstarts.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wi.nszjky.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xy.jctech888.com.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://fw.panjiajie.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://gw.shtwfgs.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fy.colortex.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://xa.huanxung.cn

[H02] finally / ensure 收尾
来源：http://vv.hahajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ii.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://qu.bjjhwx.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://xs.huixiangedu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://nb.yuntaijiaju.cn

Java: try { f(); } finally { cleanup(); }
来源：http://yy.newstarts.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://vj.muxihuayi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://uc.asd995.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://cg.shxzskj.cn

[H03] 主动抛出异常
来源：http://se.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://ma.lnxyls.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yc.huixiangedu.cn

JS:   throw new Error("错误信息");
来源：http://vl.huixinmuqiang.cn

TS:   throw new Error("错误信息");
来源：http://qv.colortex.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lj.hnjuh.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://nt.huixinmuqiang.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://oe.szxytkj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zw.bjjhwx.cn

[H04] 自定义异常类型
来源：http://jp.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://cm.chemitech.net.cn

PHP:  class MyError extends RuntimeException {}
来源：http://fx.yuexingan06.cn

JS:   class MyError extends Error {}
来源：http://aa.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://pj.panjiajie.cn

Java: class MyException extends RuntimeException {}
来源：http://xe.gzmigu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fp.szxytkj.cn

Ruby: class MyError < StandardError; end
来源：http://ox.panjiajie.cn

C#:   class MyException : Exception {}
来源：http://cv.chemitech.net.cn

[H05] 捕获特定类型
来源：http://ai.muxihuayi.cn

Py:   except ValueError as e:
来源：http://zc.szxytkj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wg.panjiajie.cn

JS:   if (e instanceof TypeError) {}
来源：http://lr.szsharing.cn

TS:   if (e instanceof TypeError) {}
来源：http://nt.chemitech.net.cn

Java: catch (IOException | SQLException e) {}
来源：http://yo.wgjwhj.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://zt.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://oz.haigaiapp.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sh.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://uo.521024.cn

Py:   value = d.get("k") or default
来源：http://pn.hnjuh.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ee.shxzskj.cn

JS:   obj?.a?.b;  d ?? default
来源：http://qq.asd995.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zh.shtwfgs.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://uk.szsharing.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://lv.szsharing.cn

Ruby: d&.dig(:a, :b)
来源：http://jr.bookmarksfly.cn

C#:   obj?.A?.B ?? default
来源：http://uw.shxzskj.cn

[H07] 断言
来源：http://qq.szsharing.cn

Py:   assert x > 0, "必须为正"
来源：http://js.9csxet.cn

PHP:  assert($x > 0);
来源：http://gr.9csxet.cn

JS:   console.assert(x > 0);
来源：http://ym.chemitech.net.cn

TS:   console.assert(x > 0);
来源：http://fu.9csxet.cn

Java: assert x > 0 : "必须为正";
来源：http://br.521024.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://et.asd995.cn

Ruby: raise "必须为正" unless x > 0
来源：http://or.newstarts.cn

C#:   Debug.Assert(x > 0);
来源：http://be.521024.cn

[H08] 获取错误信息与堆栈
来源：http://nw.hnjuh.cn

Py:   str(e);  traceback.format_exc()
来源：http://gq.muxihuayi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pi.szsharing.cn

JS:   e.message;  e.stack
来源：http://um.gzmigu.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wa.panjiajie.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bl.9csxet.cn

Go:   err.Error()
来源：http://wr.9csxet.cn

Ruby: e.message;  e.backtrace
来源：http://qg.haigaiapp.cn

C#:   e.Message;  e.StackTrace
来源：http://ut.bookmarksfly.cn

[H09] 带错误码的异常
来源：http://ip.yuntaijiaju.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sa.haigaiapp.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://wy.yuntaijiaju.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://fw.jianghongdianzi.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ot.521024.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mr.yuexingan06.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://pn.jianghongdianzi.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ax.shxzskj.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://pd.newstarts.cn

[H10] 资源自动释放
来源：http://or.panjiajie.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://pz.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nd.gzmigu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mc.muxihuayi.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ne.yuexingan06.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://da.shxzukj.cn

Go:   defer f.Close()
来源：http://yo.asd995.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ni.szsharing.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://yq.yuexingan06.cn

================================================================================
来源：http://ij.bjjhwx.cn

I. 正则表达式
来源：http://af.lnxyls.cn

================================================================================
来源：http://va.huanxung.cn

[I01] 判断是否匹配
来源：http://xs.hahajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ul.yuntaijiaju.cn

PHP:  preg_match('/\d+/', $s);
来源：http://sq.hnjuh.cn

JS:   /\d+/.test(s)
来源：http://du.panjiajie.cn

TS:   /\d+/.test(s)
来源：http://ir.521024.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://fd.jctech888.com.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://sy.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://ae.yuntaijiaju.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fd.muxihuayi.cn

[I02] 提取所有匹配
来源：http://zn.shtwfgs.cn

Py:   re.findall(r"\d+", s)
来源：http://as.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://pd.chemitech.net.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://fu.521024.cn

TS:   s.match(/\d+/g)
来源：http://xo.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://sg.shxzskj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://lj.shtwfgs.cn

Ruby: s.scan(/\d+/)
来源：http://xp.haigaiapp.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ca.muxihuayi.cn

[I03] 提取捕获分组
来源：http://bn.yuntaijiaju.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://yr.lnxyls.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://yt.szxytkj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mk.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://iv.chemitech.net.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jj.shtwfgs.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rw.bookmarksfly.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://pz.szxytkj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://un.gzmigu.cn

[I04] 正则替换
来源：http://pv.bjjhwx.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://gf.asd995.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ul.yuntaijiaju.cn

JS:   s.replace(/\d+/g, "#")
来源：http://hc.szxytkj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://od.jianghongdianzi.cn

Java: s.replaceAll("\\d+", "#")
来源：http://cs.huanxung.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://uc.shxzukj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://cs.shxzskj.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://pb.yuexingan06.cn

[I05] 按正则拆分
来源：http://hf.shxzukj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://wd.bjjhwx.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://jo.huixiangedu.cn

JS:   s.split(/\s*,\s*/)
来源：http://hc.hahajie.cn

TS:   s.split(/\s*,\s*/)
来源：http://cj.huixinmuqiang.cn

Java: s.split("\\s*,\\s*")
来源：http://ie.wgjwhj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://pu.haigaiapp.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ro.newstarts.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wq.shxzskj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://iv.hahajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://aj.shtwfgs.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rh.nszjky.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jp.9csxet.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gn.colortex.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xc.newstarts.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://uy.muxihuayi.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ws.hahajie.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://in.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://mb.shxzskj.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vf.hahajie.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://oe.lnxyls.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://vh.shxzskj.cn

TS:   /error/gim
来源：http://af.hahajie.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://rw.nicolike.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://zz.521024.cn

Ruby: s.scan(/error/i)
来源：http://fw.jctech888.com.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ym.hahajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://er.gzmigu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://uq.colortex.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://rh.hnjuh.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://lu.nszjky.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jg.9csxet.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bl.lnxyls.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://la.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://fd.shtwfgs.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gl.haigaiapp.cn

================================================================================
来源：http://bx.huixiangedu.cn

J. 日期与时间
来源：http://ts.newstarts.cn

================================================================================
来源：http://qw.nszjky.cn

[J01] 获取当前时间
来源：http://nv.lnxyls.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hq.9csxet.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://xc.colortex.cn

JS:   new Date();  Date.now()
来源：http://yp.colortex.cn

TS:   new Date();  Date.now()
来源：http://bq.yuexingan06.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://he.yuntaijiaju.cn

Go:   time.Now()
来源：http://dj.nszjky.cn

Ruby: Time.now
来源：http://dz.gzmigu.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://th.lnxyls.cn

[J02] 格式化输出
来源：http://rm.shtwfgs.cn


<!-- 参考信息 -->