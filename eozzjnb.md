代发 wailian999

Ruby: @name = "x"
来源：http://mi.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://jk.hnjuh.cn

[G04] 定义方法
来源：http://zp.521024.cn

Py:   def greet(self): return self.name
来源：http://sf.huixinmuqiang.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fy.hnjuh.cn

JS:   greet() { return this.name; }
来源：http://gx.panjiajie.cn

TS:   greet(): string { return this.name; }
来源：http://ns.newstarts.cn

Java: String greet() { return name; }
来源：http://ou.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://iz.nszjky.cn

Ruby: def greet; @name; end
来源：http://zf.yuntaijiaju.cn

C#:   public string Greet() => Name;
来源：http://pm.bjjhwx.cn

[G05] 继承
来源：http://xe.szsharing.cn

Py:   class Admin(User): pass
来源：http://rg.asd995.cn

PHP:  class Admin extends User {}
来源：http://jw.shxzukj.cn

JS:   class Admin extends User {}
来源：http://kl.colortex.cn

TS:   class Admin extends User {}
来源：http://me.asd995.cn

Java: class Admin extends User {}
来源：http://kh.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://of.wgjwhj.cn

Ruby: class Admin < User; end
来源：http://tb.jianghongdianzi.cn

C#:   class Admin : User {}
来源：http://ja.asd995.cn

[G06] 重写方法
来源：http://yl.newstarts.cn

Py:   def greet(self): return "admin"
来源：http://ga.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://rz.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://kb.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://zk.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://fl.bjjhwx.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mm.yuexingan06.cn

Ruby: def greet; "admin"; end
来源：http://jn.muxihuayi.cn

C#:   public override string Greet() => "admin";
来源：http://vl.yuexingan06.cn

[G07] 调用父类方法
来源：http://yw.huanxung.cn

Py:   super().greet()
来源：http://ql.jianghongdianzi.cn

PHP:  parent::greet();
来源：http://cx.521024.cn

JS:   super.greet();
来源：http://ty.nszjky.cn

TS:   super.greet();
来源：http://if.huixinmuqiang.cn

Java: super.greet();
来源：http://jy.hahajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://if.lnxyls.cn

Ruby: super
来源：http://oi.asd995.cn

C#:   base.Greet();
来源：http://ma.jctech888.com.cn

[G08] 静态方法与属性
来源：http://lk.shtwfgs.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://an.hahajie.cn

PHP:  public static function f() {}
来源：http://bl.9csxet.cn

JS:   static f() {}
来源：http://vr.huixiangedu.cn

TS:   static f(): void {}
来源：http://ar.gzmigu.cn

Java: static void f() {}
来源：http://kj.colortex.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fp.bjjhwx.cn

Ruby: def self.f; end
来源：http://rl.jianghongdianzi.cn

C#:   public static void F() {}
来源：http://rv.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://qt.gzmigu.cn

Py:   from abc import ABC, abstractmethod
来源：http://me.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://nr.huixiangedu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://sc.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://fc.hahajie.cn

Java: interface Shape { double area(); }
来源：http://fi.bjjhwx.cn

Go:   type Shape interface { Area() float64 }
来源：http://bc.jianghongdianzi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://og.lnxyls.cn

C#:   interface IShape { double Area(); }
来源：http://vv.jianghongdianzi.cn

[G10] 访问控制
来源：http://oq.521024.cn

Py:   约定 _protected / __private（不强制）
来源：http://gl.panjiajie.cn

PHP:  public / protected / private
来源：http://ur.szxytkj.cn

JS:   #private 字段；其余公开
来源：http://ac.bookmarksfly.cn

TS:   public / protected / private
来源：http://gz.yuntaijiaju.cn

Java: public / protected / private / 默认包级
来源：http://po.szsharing.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cx.lnxyls.cn

Ruby: public / protected / private
来源：http://jw.lnxyls.cn

C#:   public / protected / private / internal
来源：http://qg.shxzskj.cn

[G11] getter / setter
来源：http://ez.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://cq.shxzskj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ie.gzmigu.cn

JS:   get name() { return this._name; }
来源：http://kk.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://eg.muxihuayi.cn

Java: public String getName() { return name; }
来源：http://pt.9csxet.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mf.chemitech.net.cn

Ruby: attr_accessor :name
来源：http://jo.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://zp.asd995.cn

[G12] 对象转字符串
来源：http://yw.jianghongdianzi.cn

Py:   def __str__(self): return self.name
来源：http://mh.panjiajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://tc.muxihuayi.cn

JS:   toString() { return this.name; }
来源：http://jj.bjjhwx.cn

TS:   toString(): string { return this.name; }
来源：http://zd.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://oy.shxzskj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://jb.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://zr.9csxet.cn

C#:   public override string ToString() => Name;
来源：http://qw.szxytkj.cn

[G13] 判断对象类型
来源：http://hb.asd995.cn

Py:   isinstance(u, User)
来源：http://hn.haigaiapp.cn

PHP:  $u instanceof User
来源：http://lm.huixiangedu.cn

JS:   u instanceof User
来源：http://gf.wgjwhj.cn

TS:   u instanceof User
来源：http://vv.huanxung.cn

Java: u instanceof User
来源：http://vl.bjjhwx.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://fg.nszjky.cn

Ruby: u.is_a?(User)
来源：http://mh.521024.cn

C#:   u is User
来源：http://qt.lnxyls.cn

[G14] 数据类 / record
来源：http://pb.bookmarksfly.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bg.yuntaijiaju.cn

PHP:  // 用 readonly 属性模拟
来源：http://fi.huanxung.cn

JS:   // 无内置：普通类或对象字面量
来源：http://do.wgjwhj.cn

TS:   type User = { name: string; age: number };
来源：http://rv.yuntaijiaju.cn

Java: record User(String name, int age) {}
来源：http://zg.haigaiapp.cn

Go:   type User struct { Name string; Age int }
来源：http://ga.hahajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://qk.haigaiapp.cn

C#:   record User(string Name, int Age);
来源：http://vl.nicolike.cn

[G15] 枚举
来源：http://ly.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://vw.lnxyls.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pa.yuntaijiaju.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://vp.muxihuayi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://kw.szxytkj.cn

Java: enum Color { RED, GREEN }
来源：http://pn.9csxet.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://td.huixiangedu.cn

Ruby: Color = %i[red green].freeze
来源：http://og.shtwfgs.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bq.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://ik.hahajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bx.9csxet.cn

PHP:  get_object_vars($obj);
来源：http://bo.bjjhwx.cn

JS:   Object.entries(obj)
来源：http://hj.shxzskj.cn

TS:   Object.entries(obj)
来源：http://uy.newstarts.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://fr.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://tu.shxzskj.cn

Ruby: obj.instance_variables
来源：http://ja.szsharing.cn

C#:   // 用反射或 System.Text.Json
来源：http://me.panjiajie.cn

================================================================================
来源：http://bl.lnxyls.cn

H. 异常与错误处理
来源：http://ra.9csxet.cn

================================================================================
来源：http://zu.shxzskj.cn

[H01] try / catch 基础
来源：http://vo.asd995.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zi.huixinmuqiang.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://zk.wgjwhj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dk.szsharing.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://cm.521024.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://jr.hnjuh.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kh.9csxet.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://by.huanxung.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ol.gzmigu.cn

[H02] finally / ensure 收尾
来源：http://mr.panjiajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fl.bjjhwx.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lr.szxytkj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hm.hahajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://jm.muxihuayi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ce.huixinmuqiang.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://bp.nicolike.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://kj.wgjwhj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zc.yuntaijiaju.cn

[H03] 主动抛出异常
来源：http://vi.bjjhwx.cn

Py:   raise ValueError("错误信息")
来源：http://cc.newstarts.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ce.shxzskj.cn

JS:   throw new Error("错误信息");
来源：http://gw.szxytkj.cn

TS:   throw new Error("错误信息");
来源：http://to.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://pa.huixinmuqiang.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://vw.haigaiapp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://eq.jctech888.com.cn

C#:   throw new ArgumentException("错误信息");
来源：http://no.huanxung.cn

[H04] 自定义异常类型
来源：http://bo.lnxyls.cn

Py:   class MyError(Exception): pass
来源：http://xs.huixinmuqiang.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wm.lnxyls.cn

JS:   class MyError extends Error {}
来源：http://dt.bookmarksfly.cn

TS:   class MyError extends Error {}
来源：http://oy.huanxung.cn

Java: class MyException extends RuntimeException {}
来源：http://va.chemitech.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://lr.szsharing.cn

Ruby: class MyError < StandardError; end
来源：http://ie.shxzskj.cn

C#:   class MyException : Exception {}
来源：http://ax.newstarts.cn

[H05] 捕获特定类型
来源：http://nm.hahajie.cn

Py:   except ValueError as e:
来源：http://ut.hahajie.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://bn.shtwfgs.cn

JS:   if (e instanceof TypeError) {}
来源：http://iw.panjiajie.cn

TS:   if (e instanceof TypeError) {}
来源：http://cg.shxzskj.cn

Java: catch (IOException | SQLException e) {}
来源：http://wd.muxihuayi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://dj.shtwfgs.cn

Ruby: rescue ArgumentError => e
来源：http://sw.shxzukj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wc.hahajie.cn

[H06] 可选值 / 空值安全访问
来源：http://dl.haigaiapp.cn

Py:   value = d.get("k") or default
来源：http://vg.yuntaijiaju.cn

PHP:  $v = $d["k"] ?? null;
来源：http://bg.huixinmuqiang.cn

JS:   obj?.a?.b;  d ?? default
来源：http://ar.panjiajie.cn

TS:   obj?.a?.b;  d ?? default
来源：http://sf.hnjuh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://cr.colortex.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://zm.huixinmuqiang.cn

Ruby: d&.dig(:a, :b)
来源：http://re.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://gc.panjiajie.cn

[H07] 断言
来源：http://il.yuntaijiaju.cn

Py:   assert x > 0, "必须为正"
来源：http://fg.nicolike.cn

PHP:  assert($x > 0);
来源：http://wz.nicolike.cn

JS:   console.assert(x > 0);
来源：http://pd.nicolike.cn

TS:   console.assert(x > 0);
来源：http://gc.bjjhwx.cn

Java: assert x > 0 : "必须为正";
来源：http://hs.jianghongdianzi.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://cx.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://hk.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://ul.wgjwhj.cn

[H08] 获取错误信息与堆栈
来源：http://ld.nszjky.cn

Py:   str(e);  traceback.format_exc()
来源：http://to.gzmigu.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://nj.yuntaijiaju.cn

JS:   e.message;  e.stack
来源：http://pz.lnxyls.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://hn.lnxyls.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://er.shtwfgs.cn

Go:   err.Error()
来源：http://dq.szxytkj.cn

Ruby: e.message;  e.backtrace
来源：http://yl.shtwfgs.cn

C#:   e.Message;  e.StackTrace
来源：http://zo.szxytkj.cn

[H09] 带错误码的异常
来源：http://iu.huanxung.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://ld.nszjky.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://jz.jctech888.com.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://jw.shxzskj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sq.nicolike.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://uj.521024.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fg.wgjwhj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://jo.chemitech.net.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ww.haigaiapp.cn

[H10] 资源自动释放
来源：http://bt.nszjky.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://wo.colortex.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hc.nszjky.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://aj.haigaiapp.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://yh.nszjky.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ri.huixiangedu.cn

Go:   defer f.Close()
来源：http://ib.nszjky.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://br.yuexingan06.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://ei.gzmigu.cn

================================================================================
来源：http://rg.shxzukj.cn

I. 正则表达式
来源：http://zy.jctech888.com.cn

================================================================================
来源：http://wl.huanxung.cn

[I01] 判断是否匹配
来源：http://jq.yuexingan06.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://tv.gzmigu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://xa.newstarts.cn

JS:   /\d+/.test(s)
来源：http://zq.chemitech.net.cn

TS:   /\d+/.test(s)
来源：http://pr.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://ad.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://oe.bookmarksfly.cn

Ruby: s.match?(/\d+/)
来源：http://zn.shxzukj.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://bc.asd995.cn

[I02] 提取所有匹配
来源：http://fn.huixinmuqiang.cn

Py:   re.findall(r"\d+", s)
来源：http://ms.asd995.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://vx.muxihuayi.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zr.chemitech.net.cn

TS:   s.match(/\d+/g)
来源：http://az.panjiajie.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://zz.shtwfgs.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://kv.shxzukj.cn

Ruby: s.scan(/\d+/)
来源：http://mu.yuexingan06.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://qx.521024.cn

[I03] 提取捕获分组
来源：http://ag.nszjky.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wh.9csxet.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wn.jctech888.com.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://qo.gzmigu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://ls.huixinmuqiang.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://sf.huixiangedu.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://nv.bjjhwx.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jq.yuntaijiaju.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yv.shxzskj.cn

[I04] 正则替换
来源：http://ak.asd995.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://oj.newstarts.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://jr.huixinmuqiang.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ei.szxytkj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://lc.huanxung.cn

Java: s.replaceAll("\\d+", "#")
来源：http://kt.shxzskj.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://wd.colortex.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ra.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dl.haigaiapp.cn

[I05] 按正则拆分
来源：http://zt.huixinmuqiang.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://iv.lnxyls.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://rh.huixinmuqiang.cn

JS:   s.split(/\s*,\s*/)
来源：http://rf.bookmarksfly.cn

TS:   s.split(/\s*,\s*/)
来源：http://aw.jctech888.com.cn

Java: s.split("\\s*,\\s*")
来源：http://jq.nszjky.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://vy.gzmigu.cn

Ruby: s.split(/\s*,\s*/)
来源：http://wz.yuntaijiaju.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://if.nszjky.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://eo.hahajie.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hy.521024.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://un.nszjky.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://xh.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bd.hnjuh.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wy.jianghongdianzi.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://dw.yuexingan06.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://il.shtwfgs.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://et.bookmarksfly.cn

[I07] 忽略大小写与多行模式
来源：http://jy.muxihuayi.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://jr.shxzukj.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://qz.yuntaijiaju.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dv.jianghongdianzi.cn

TS:   /error/gim
来源：http://iu.asd995.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wl.nszjky.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fh.colortex.cn

Ruby: s.scan(/error/i)
来源：http://og.muxihuayi.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ww.jctech888.com.cn

[I08] 贪婪与非贪婪匹配
来源：http://nf.chemitech.net.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://cc.wgjwhj.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ow.haigaiapp.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://az.wgjwhj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://sx.szsharing.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://tc.huixinmuqiang.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://wg.nicolike.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ai.huanxung.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gt.nszjky.cn

================================================================================
来源：http://js.panjiajie.cn

J. 日期与时间
来源：http://to.shxzskj.cn

================================================================================
来源：http://zk.9csxet.cn

[J01] 获取当前时间
来源：http://rl.jctech888.com.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wq.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sd.szsharing.cn

JS:   new Date();  Date.now()
来源：http://uz.szxytkj.cn

TS:   new Date();  Date.now()
来源：http://ye.shxzskj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://vp.huixinmuqiang.cn

Go:   time.Now()
来源：http://oe.colortex.cn

Ruby: Time.now
来源：http://ds.9csxet.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://qc.newstarts.cn

[J02] 格式化输出
来源：http://ml.nszjky.cn


<!-- 参考信息 -->