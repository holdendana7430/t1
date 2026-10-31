代发 wailian999

JS:   this.name = "x";
来源：http://dv.jianghongdianzi.cn

TS:   name: string = "x";
来源：http://by.szsharing.cn

Java: private String name;
来源：http://iw.newstarts.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://yj.muxihuayi.cn

Ruby: @name = "x"
来源：http://nr.hahajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://ws.hnjuh.cn

[G04] 定义方法
来源：http://fz.newstarts.cn

Py:   def greet(self): return self.name
来源：http://no.lnxyls.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pw.bjjhwx.cn

JS:   greet() { return this.name; }
来源：http://pl.hahajie.cn

TS:   greet(): string { return this.name; }
来源：http://eq.shxzskj.cn

Java: String greet() { return name; }
来源：http://do.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://lu.521024.cn

Ruby: def greet; @name; end
来源：http://bu.huixiangedu.cn

C#:   public string Greet() => Name;
来源：http://cm.szxytkj.cn

[G05] 继承
来源：http://lq.hahajie.cn

Py:   class Admin(User): pass
来源：http://fc.newstarts.cn

PHP:  class Admin extends User {}
来源：http://cj.asd995.cn

JS:   class Admin extends User {}
来源：http://ui.huixinmuqiang.cn

TS:   class Admin extends User {}
来源：http://za.colortex.cn

Java: class Admin extends User {}
来源：http://wp.yuntaijiaju.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://bg.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://wi.huanxung.cn

C#:   class Admin : User {}
来源：http://jf.bookmarksfly.cn

[G06] 重写方法
来源：http://rt.gzmigu.cn

Py:   def greet(self): return "admin"
来源：http://oq.gzmigu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://uy.newstarts.cn

JS:   greet() { return "admin"; }
来源：http://ej.newstarts.cn

TS:   greet(): string { return "admin"; }
来源：http://rc.nicolike.cn

Java: @Override String greet() { return "admin"; }
来源：http://fv.bjjhwx.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://so.huixiangedu.cn

Ruby: def greet; "admin"; end
来源：http://oz.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://po.wgjwhj.cn

[G07] 调用父类方法
来源：http://rg.nicolike.cn

Py:   super().greet()
来源：http://np.szxytkj.cn

PHP:  parent::greet();
来源：http://um.nszjky.cn

JS:   super.greet();
来源：http://dh.haigaiapp.cn

TS:   super.greet();
来源：http://ly.gzmigu.cn

Java: super.greet();
来源：http://tj.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zj.chemitech.net.cn

Ruby: super
来源：http://li.hnjuh.cn

C#:   base.Greet();
来源：http://xa.jctech888.com.cn

[G08] 静态方法与属性
来源：http://bt.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ss.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://iy.muxihuayi.cn

JS:   static f() {}
来源：http://pa.muxihuayi.cn

TS:   static f(): void {}
来源：http://gh.bjjhwx.cn

Java: static void f() {}
来源：http://yh.huixiangedu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bz.colortex.cn

Ruby: def self.f; end
来源：http://ej.lnxyls.cn

C#:   public static void F() {}
来源：http://fh.shtwfgs.cn

[G09] 接口 / 抽象类
来源：http://lm.lnxyls.cn

Py:   from abc import ABC, abstractmethod
来源：http://gi.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jg.newstarts.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://de.yuntaijiaju.cn

TS:   interface Shape { area(): number; }
来源：http://pk.haigaiapp.cn

Java: interface Shape { double area(); }
来源：http://fw.szsharing.cn

Go:   type Shape interface { Area() float64 }
来源：http://hm.huixinmuqiang.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wj.hnjuh.cn

C#:   interface IShape { double Area(); }
来源：http://oi.haigaiapp.cn

[G10] 访问控制
来源：http://zb.gzmigu.cn

Py:   约定 _protected / __private（不强制）
来源：http://jh.wgjwhj.cn

PHP:  public / protected / private
来源：http://ni.shxzskj.cn

JS:   #private 字段；其余公开
来源：http://rq.9csxet.cn

TS:   public / protected / private
来源：http://uf.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://xv.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://on.bookmarksfly.cn

Ruby: public / protected / private
来源：http://rj.bookmarksfly.cn

C#:   public / protected / private / internal
来源：http://bt.huixinmuqiang.cn

[G11] getter / setter
来源：http://xg.bjjhwx.cn

Py:   @property 与 @x.setter
来源：http://bc.shxzskj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lw.chemitech.net.cn

JS:   get name() { return this._name; }
来源：http://tg.hahajie.cn

TS:   get name(): string { return this._name; }
来源：http://mm.szsharing.cn

Java: public String getName() { return name; }
来源：http://hx.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://fc.haigaiapp.cn

Ruby: attr_accessor :name
来源：http://hd.yuexingan06.cn

C#:   public string Name { get; set; }
来源：http://so.colortex.cn

[G12] 对象转字符串
来源：http://yr.huixiangedu.cn

Py:   def __str__(self): return self.name
来源：http://as.521024.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://uj.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://tf.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://hd.huanxung.cn

Java: @Override public String toString() { return name; }
来源：http://pd.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mm.chemitech.net.cn

Ruby: def to_s; @name; end
来源：http://mi.haigaiapp.cn

C#:   public override string ToString() => Name;
来源：http://pl.chemitech.net.cn

[G13] 判断对象类型
来源：http://jg.yuntaijiaju.cn

Py:   isinstance(u, User)
来源：http://af.colortex.cn

PHP:  $u instanceof User
来源：http://nx.szxytkj.cn

JS:   u instanceof User
来源：http://sp.colortex.cn

TS:   u instanceof User
来源：http://xp.newstarts.cn

Java: u instanceof User
来源：http://vj.nicolike.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sy.nszjky.cn

Ruby: u.is_a?(User)
来源：http://hj.colortex.cn

C#:   u is User
来源：http://pd.yuexingan06.cn

[G14] 数据类 / record
来源：http://eh.yuntaijiaju.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://yy.huanxung.cn

PHP:  // 用 readonly 属性模拟
来源：http://wj.muxihuayi.cn

JS:   // 无内置：普通类或对象字面量
来源：http://jg.muxihuayi.cn

TS:   type User = { name: string; age: number };
来源：http://hu.521024.cn

Java: record User(String name, int age) {}
来源：http://sg.hnjuh.cn

Go:   type User struct { Name string; Age int }
来源：http://xq.asd995.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mh.wgjwhj.cn

C#:   record User(string Name, int Age);
来源：http://cm.muxihuayi.cn

[G15] 枚举
来源：http://ea.bjjhwx.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://pr.nicolike.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://qe.521024.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://ix.jianghongdianzi.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jb.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://oy.hahajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ha.asd995.cn

Ruby: Color = %i[red green].freeze
来源：http://ad.colortex.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rg.wgjwhj.cn

[G16] 对象转数组 / 字典
来源：http://xd.nszjky.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://xb.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://ja.shtwfgs.cn

JS:   Object.entries(obj)
来源：http://dy.huixinmuqiang.cn

TS:   Object.entries(obj)
来源：http://kv.newstarts.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://zq.bjjhwx.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bt.9csxet.cn

Ruby: obj.instance_variables
来源：http://hh.huixinmuqiang.cn

C#:   // 用反射或 System.Text.Json
来源：http://hj.yuexingan06.cn

================================================================================
来源：http://qn.jianghongdianzi.cn

H. 异常与错误处理
来源：http://qi.wgjwhj.cn

================================================================================
来源：http://be.hahajie.cn

[H01] try / catch 基础
来源：http://fh.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://vm.colortex.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yy.haigaiapp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://dh.521024.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mc.nszjky.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ie.chemitech.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yl.jctech888.com.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://fd.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://fk.lnxyls.cn

[H02] finally / ensure 收尾
来源：http://xv.jianghongdianzi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://no.jianghongdianzi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://eb.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gm.asd995.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ul.panjiajie.cn

Java: try { f(); } finally { cleanup(); }
来源：http://zm.hahajie.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://qt.bookmarksfly.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.521024.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://tl.shtwfgs.cn

[H03] 主动抛出异常
来源：http://nh.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://fy.newstarts.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://kk.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://qm.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://gj.chemitech.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://uz.gzmigu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://jz.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://te.yuntaijiaju.cn

C#:   throw new ArgumentException("错误信息");
来源：http://oh.hahajie.cn

[H04] 自定义异常类型
来源：http://mt.huanxung.cn

Py:   class MyError(Exception): pass
来源：http://ba.bjjhwx.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ac.nicolike.cn

JS:   class MyError extends Error {}
来源：http://er.hahajie.cn

TS:   class MyError extends Error {}
来源：http://uc.yuntaijiaju.cn

Java: class MyException extends RuntimeException {}
来源：http://hu.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://fs.asd995.cn

Ruby: class MyError < StandardError; end
来源：http://qh.asd995.cn

C#:   class MyException : Exception {}
来源：http://ad.hnjuh.cn

[H05] 捕获特定类型
来源：http://ii.szxytkj.cn

Py:   except ValueError as e:
来源：http://ll.hnjuh.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gc.muxihuayi.cn

JS:   if (e instanceof TypeError) {}
来源：http://vb.szxytkj.cn

TS:   if (e instanceof TypeError) {}
来源：http://pw.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://lc.huanxung.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://rr.yuexingan06.cn

Ruby: rescue ArgumentError => e
来源：http://bm.newstarts.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cd.shtwfgs.cn

[H06] 可选值 / 空值安全访问
来源：http://uo.9csxet.cn

Py:   value = d.get("k") or default
来源：http://eh.szxytkj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://cu.haigaiapp.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wi.hnjuh.cn

TS:   obj?.a?.b;  d ?? default
来源：http://th.haigaiapp.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://aq.hahajie.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://uw.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://bk.9csxet.cn

C#:   obj?.A?.B ?? default
来源：http://kl.nszjky.cn

[H07] 断言
来源：http://nu.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://eg.hnjuh.cn

PHP:  assert($x > 0);
来源：http://pd.huixiangedu.cn

JS:   console.assert(x > 0);
来源：http://ed.hahajie.cn

TS:   console.assert(x > 0);
来源：http://qr.huanxung.cn

Java: assert x > 0 : "必须为正";
来源：http://vu.bookmarksfly.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://xr.hnjuh.cn

Ruby: raise "必须为正" unless x > 0
来源：http://tr.shtwfgs.cn

C#:   Debug.Assert(x > 0);
来源：http://sr.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://ma.panjiajie.cn

Py:   str(e);  traceback.format_exc()
来源：http://je.yuexingan06.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://eg.wgjwhj.cn

JS:   e.message;  e.stack
来源：http://oo.huanxung.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://jt.muxihuayi.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://zu.asd995.cn

Go:   err.Error()
来源：http://sm.bjjhwx.cn

Ruby: e.message;  e.backtrace
来源：http://yf.hahajie.cn

C#:   e.Message;  e.StackTrace
来源：http://sy.hahajie.cn

[H09] 带错误码的异常
来源：http://qb.nicolike.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hy.szsharing.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://pg.chemitech.net.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://pq.haigaiapp.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://pl.gzmigu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://fy.asd995.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fm.9csxet.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ij.bookmarksfly.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://rt.yuexingan06.cn

[H10] 资源自动释放
来源：http://op.jctech888.com.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dj.9csxet.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://nq.huixiangedu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://fu.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ri.shxzskj.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ey.szxytkj.cn

Go:   defer f.Close()
来源：http://ca.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qa.9csxet.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://sw.szxytkj.cn

================================================================================
来源：http://rd.hnjuh.cn

I. 正则表达式
来源：http://ik.asd995.cn

================================================================================
来源：http://fm.muxihuayi.cn

[I01] 判断是否匹配
来源：http://tp.521024.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://sk.colortex.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wv.yuntaijiaju.cn

JS:   /\d+/.test(s)
来源：http://yo.lnxyls.cn

TS:   /\d+/.test(s)
来源：http://fy.gzmigu.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://rq.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://by.nszjky.cn

Ruby: s.match?(/\d+/)
来源：http://kb.lnxyls.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://dx.jianghongdianzi.cn

[I02] 提取所有匹配
来源：http://bh.colortex.cn

Py:   re.findall(r"\d+", s)
来源：http://qp.bookmarksfly.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mh.haigaiapp.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://zo.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://ib.9csxet.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uw.hnjuh.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://ds.colortex.cn

Ruby: s.scan(/\d+/)
来源：http://aq.jctech888.com.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://rc.wgjwhj.cn

[I03] 提取捕获分组
来源：http://fo.huanxung.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://uc.wgjwhj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://kl.hahajie.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zv.hnjuh.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://sk.bookmarksfly.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://ga.newstarts.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ls.newstarts.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://fq.huanxung.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://xi.asd995.cn

[I04] 正则替换
来源：http://lc.haigaiapp.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ws.szsharing.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ji.muxihuayi.cn

JS:   s.replace(/\d+/g, "#")
来源：http://yu.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://yb.9csxet.cn

Java: s.replaceAll("\\d+", "#")
来源：http://nu.jctech888.com.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://kf.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://fr.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://om.colortex.cn

[I05] 按正则拆分
来源：http://bq.yuntaijiaju.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://ma.shxzukj.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vt.nszjky.cn

JS:   s.split(/\s*,\s*/)
来源：http://nv.wgjwhj.cn

TS:   s.split(/\s*,\s*/)
来源：http://jq.shtwfgs.cn

Java: s.split("\\s*,\\s*")
来源：http://fg.szsharing.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://em.huanxung.cn

Ruby: s.split(/\s*,\s*/)
来源：http://hv.huixinmuqiang.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://bn.lnxyls.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://xp.shxzukj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qd.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://rn.haigaiapp.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://gg.huixiangedu.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://qd.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://uw.szxytkj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://yl.huixiangedu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ab.muxihuayi.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://lh.nicolike.cn

[I07] 忽略大小写与多行模式
来源：http://yh.hnjuh.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mx.muxihuayi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://pv.newstarts.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://pu.panjiajie.cn

TS:   /error/gim
来源：http://sv.wgjwhj.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://wt.jianghongdianzi.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://gp.hahajie.cn

Ruby: s.scan(/error/i)
来源：http://vp.yuexingan06.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://zk.wgjwhj.cn

[I08] 贪婪与非贪婪匹配
来源：http://bw.huixinmuqiang.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pu.hahajie.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ir.jctech888.com.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://fi.bookmarksfly.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://av.colortex.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://bo.szxytkj.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://xm.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://zu.nszjky.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://gb.nszjky.cn

================================================================================
来源：http://sx.yuexingan06.cn

J. 日期与时间
来源：http://lh.wgjwhj.cn

================================================================================
来源：http://jk.colortex.cn

[J01] 获取当前时间
来源：http://sh.yuntaijiaju.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://hu.muxihuayi.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wg.nszjky.cn

JS:   new Date();  Date.now()
来源：http://pj.hnjuh.cn

TS:   new Date();  Date.now()
来源：http://gc.huixiangedu.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://xj.haigaiapp.cn


<!-- 参考信息 -->