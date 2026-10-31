代发 wailian999

PHP:  public function greet(): string { return $this->name; }
来源：http://qu.yuexingan06.cn

JS:   greet() { return this.name; }
来源：http://bg.lnxyls.cn

TS:   greet(): string { return this.name; }
来源：http://pc.wgjwhj.cn

Java: String greet() { return name; }
来源：http://pg.asd995.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ty.szxytkj.cn

Ruby: def greet; @name; end
来源：http://yj.szxytkj.cn

C#:   public string Greet() => Name;
来源：http://es.szxytkj.cn

[G05] 继承
来源：http://ih.chemitech.net.cn

Py:   class Admin(User): pass
来源：http://ox.jianghongdianzi.cn

PHP:  class Admin extends User {}
来源：http://ic.huixiangedu.cn

JS:   class Admin extends User {}
来源：http://mt.shtwfgs.cn

TS:   class Admin extends User {}
来源：http://qk.bookmarksfly.cn

Java: class Admin extends User {}
来源：http://js.jctech888.com.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://zv.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://eu.panjiajie.cn

C#:   class Admin : User {}
来源：http://ju.521024.cn

[G06] 重写方法
来源：http://vg.shxzukj.cn

Py:   def greet(self): return "admin"
来源：http://zy.wgjwhj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://qw.colortex.cn

JS:   greet() { return "admin"; }
来源：http://za.9csxet.cn

TS:   greet(): string { return "admin"; }
来源：http://eg.yuntaijiaju.cn

Java: @Override String greet() { return "admin"; }
来源：http://ay.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://gh.hnjuh.cn

Ruby: def greet; "admin"; end
来源：http://ih.hnjuh.cn

C#:   public override string Greet() => "admin";
来源：http://hz.hnjuh.cn

[G07] 调用父类方法
来源：http://wm.bookmarksfly.cn

Py:   super().greet()
来源：http://ub.szxytkj.cn

PHP:  parent::greet();
来源：http://eh.yuexingan06.cn

JS:   super.greet();
来源：http://fl.jianghongdianzi.cn

TS:   super.greet();
来源：http://gt.shtwfgs.cn

Java: super.greet();
来源：http://it.shxzukj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://md.huanxung.cn

Ruby: super
来源：http://mh.szsharing.cn

C#:   base.Greet();
来源：http://xa.9csxet.cn

[G08] 静态方法与属性
来源：http://on.jianghongdianzi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ho.wgjwhj.cn

PHP:  public static function f() {}
来源：http://xu.shxzskj.cn

JS:   static f() {}
来源：http://kl.yuexingan06.cn

TS:   static f(): void {}
来源：http://gp.muxihuayi.cn

Java: static void f() {}
来源：http://lj.szxytkj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://qq.gzmigu.cn

Ruby: def self.f; end
来源：http://li.newstarts.cn

C#:   public static void F() {}
来源：http://ol.jianghongdianzi.cn

[G09] 接口 / 抽象类
来源：http://qd.lnxyls.cn

Py:   from abc import ABC, abstractmethod
来源：http://al.bjjhwx.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pr.lnxyls.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://vu.huixiangedu.cn

TS:   interface Shape { area(): number; }
来源：http://ur.wgjwhj.cn

Java: interface Shape { double area(); }
来源：http://gm.haigaiapp.cn

Go:   type Shape interface { Area() float64 }
来源：http://ji.newstarts.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://og.yuntaijiaju.cn

C#:   interface IShape { double Area(); }
来源：http://uk.yuntaijiaju.cn

[G10] 访问控制
来源：http://ux.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://ny.jianghongdianzi.cn

PHP:  public / protected / private
来源：http://li.asd995.cn

JS:   #private 字段；其余公开
来源：http://ps.bookmarksfly.cn

TS:   public / protected / private
来源：http://tu.shxzskj.cn

Java: public / protected / private / 默认包级
来源：http://kk.nszjky.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://vf.szxytkj.cn

Ruby: public / protected / private
来源：http://wv.gzmigu.cn

C#:   public / protected / private / internal
来源：http://gk.nszjky.cn

[G11] getter / setter
来源：http://kb.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://gd.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://df.nicolike.cn

JS:   get name() { return this._name; }
来源：http://gw.wgjwhj.cn

TS:   get name(): string { return this._name; }
来源：http://zw.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://jq.panjiajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://nh.wgjwhj.cn

Ruby: attr_accessor :name
来源：http://mj.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://pu.shxzskj.cn

[G12] 对象转字符串
来源：http://vq.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://sf.asd995.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://aa.yuexingan06.cn

JS:   toString() { return this.name; }
来源：http://yt.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://vt.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://vq.wgjwhj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://zh.haigaiapp.cn

Ruby: def to_s; @name; end
来源：http://ta.nicolike.cn

C#:   public override string ToString() => Name;
来源：http://cs.shxzskj.cn

[G13] 判断对象类型
来源：http://ox.nszjky.cn

Py:   isinstance(u, User)
来源：http://yb.panjiajie.cn

PHP:  $u instanceof User
来源：http://pq.shxzukj.cn

JS:   u instanceof User
来源：http://nl.chemitech.net.cn

TS:   u instanceof User
来源：http://si.wgjwhj.cn

Java: u instanceof User
来源：http://mc.shxzukj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://jm.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://ry.wgjwhj.cn

C#:   u is User
来源：http://fl.521024.cn

[G14] 数据类 / record
来源：http://og.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://bm.jianghongdianzi.cn

PHP:  // 用 readonly 属性模拟
来源：http://ac.shxzskj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://nn.szsharing.cn

TS:   type User = { name: string; age: number };
来源：http://rm.bjjhwx.cn

Java: record User(String name, int age) {}
来源：http://fd.shtwfgs.cn

Go:   type User struct { Name string; Age int }
来源：http://yt.bjjhwx.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://te.panjiajie.cn

C#:   record User(string Name, int Age);
来源：http://lh.521024.cn

[G15] 枚举
来源：http://pq.bookmarksfly.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://bf.shxzukj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://dk.hahajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://eh.newstarts.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mo.hahajie.cn

Java: enum Color { RED, GREEN }
来源：http://wv.szxytkj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rp.huanxung.cn

Ruby: Color = %i[red green].freeze
来源：http://mv.muxihuayi.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://gx.chemitech.net.cn

[G16] 对象转数组 / 字典
来源：http://bs.huanxung.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://tj.huanxung.cn

PHP:  get_object_vars($obj);
来源：http://ii.szxytkj.cn

JS:   Object.entries(obj)
来源：http://mj.asd995.cn

TS:   Object.entries(obj)
来源：http://li.shxzukj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://nq.shxzukj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ai.huixiangedu.cn

Ruby: obj.instance_variables
来源：http://bp.newstarts.cn

C#:   // 用反射或 System.Text.Json
来源：http://lh.bjjhwx.cn

================================================================================
来源：http://gi.chemitech.net.cn

H. 异常与错误处理
来源：http://qu.huixinmuqiang.cn

================================================================================
来源：http://ox.huanxung.cn

[H01] try / catch 基础
来源：http://wk.shtwfgs.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://lw.szxytkj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fh.hahajie.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lm.colortex.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nw.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qs.nicolike.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://xc.szsharing.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ff.chemitech.net.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://up.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://yl.panjiajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fk.521024.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lt.colortex.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ec.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://uk.jctech888.com.cn

Java: try { f(); } finally { cleanup(); }
来源：http://pm.nicolike.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wa.shxzskj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://og.hnjuh.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://hk.huanxung.cn

[H03] 主动抛出异常
来源：http://ib.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://ok.9csxet.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://yy.bjjhwx.cn

JS:   throw new Error("错误信息");
来源：http://pk.szsharing.cn

TS:   throw new Error("错误信息");
来源：http://cx.huixinmuqiang.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://xg.gzmigu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ww.newstarts.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://np.colortex.cn

C#:   throw new ArgumentException("错误信息");
来源：http://mo.yuexingan06.cn

[H04] 自定义异常类型
来源：http://bx.szxytkj.cn

Py:   class MyError(Exception): pass
来源：http://op.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ft.szsharing.cn

JS:   class MyError extends Error {}
来源：http://ex.nicolike.cn

TS:   class MyError extends Error {}
来源：http://sa.huixiangedu.cn

Java: class MyException extends RuntimeException {}
来源：http://dz.gzmigu.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://yd.hnjuh.cn

Ruby: class MyError < StandardError; end
来源：http://kk.shtwfgs.cn

C#:   class MyException : Exception {}
来源：http://ri.shxzukj.cn

[H05] 捕获特定类型
来源：http://lm.jianghongdianzi.cn

Py:   except ValueError as e:
来源：http://hm.szxytkj.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ft.colortex.cn

JS:   if (e instanceof TypeError) {}
来源：http://lc.yuexingan06.cn

TS:   if (e instanceof TypeError) {}
来源：http://xe.muxihuayi.cn

Java: catch (IOException | SQLException e) {}
来源：http://hv.jianghongdianzi.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://vi.gzmigu.cn

Ruby: rescue ArgumentError => e
来源：http://zi.huixiangedu.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://tu.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://dy.szxytkj.cn

Py:   value = d.get("k") or default
来源：http://og.wgjwhj.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ev.muxihuayi.cn

JS:   obj?.a?.b;  d ?? default
来源：http://iv.huanxung.cn

TS:   obj?.a?.b;  d ?? default
来源：http://xz.nszjky.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sp.nszjky.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://dh.panjiajie.cn

Ruby: d&.dig(:a, :b)
来源：http://vv.muxihuayi.cn

C#:   obj?.A?.B ?? default
来源：http://id.hnjuh.cn

[H07] 断言
来源：http://qo.lnxyls.cn

Py:   assert x > 0, "必须为正"
来源：http://yb.jianghongdianzi.cn

PHP:  assert($x > 0);
来源：http://gh.gzmigu.cn

JS:   console.assert(x > 0);
来源：http://ed.lnxyls.cn

TS:   console.assert(x > 0);
来源：http://jz.shtwfgs.cn

Java: assert x > 0 : "必须为正";
来源：http://dc.shxzskj.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://qe.shxzukj.cn

Ruby: raise "必须为正" unless x > 0
来源：http://th.chemitech.net.cn

C#:   Debug.Assert(x > 0);
来源：http://qr.huixinmuqiang.cn

[H08] 获取错误信息与堆栈
来源：http://lm.huixinmuqiang.cn

Py:   str(e);  traceback.format_exc()
来源：http://nq.colortex.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mx.haigaiapp.cn

JS:   e.message;  e.stack
来源：http://hy.bookmarksfly.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://bd.hnjuh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://en.chemitech.net.cn

Go:   err.Error()
来源：http://kn.521024.cn

Ruby: e.message;  e.backtrace
来源：http://ug.nicolike.cn

C#:   e.Message;  e.StackTrace
来源：http://xw.shxzskj.cn

[H09] 带错误码的异常
来源：http://ad.asd995.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://fk.huixinmuqiang.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://if.huixiangedu.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://zi.huixiangedu.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://zm.gzmigu.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hl.huixiangedu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://sd.chemitech.net.cn

Ruby: raise MyError.new("fail", 500)
来源：http://at.panjiajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://ah.newstarts.cn

[H10] 资源自动释放
来源：http://jb.huanxung.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://bq.yuntaijiaju.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://dc.shtwfgs.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://rp.jctech888.com.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://gj.hahajie.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://ia.bookmarksfly.cn

Go:   defer f.Close()
来源：http://tr.wgjwhj.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://vh.huanxung.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xa.panjiajie.cn

================================================================================
来源：http://df.hahajie.cn

I. 正则表达式
来源：http://tb.haigaiapp.cn

================================================================================
来源：http://bi.panjiajie.cn

[I01] 判断是否匹配
来源：http://dp.shtwfgs.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wk.wgjwhj.cn

PHP:  preg_match('/\d+/', $s);
来源：http://wz.asd995.cn

JS:   /\d+/.test(s)
来源：http://xl.jctech888.com.cn

TS:   /\d+/.test(s)
来源：http://mb.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://nd.lnxyls.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://yj.nicolike.cn

Ruby: s.match?(/\d+/)
来源：http://cn.huixinmuqiang.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://ju.bjjhwx.cn

[I02] 提取所有匹配
来源：http://na.9csxet.cn

Py:   re.findall(r"\d+", s)
来源：http://jw.gzmigu.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://zu.colortex.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://br.nicolike.cn

TS:   s.match(/\d+/g)
来源：http://jx.newstarts.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://uw.yuexingan06.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://rc.chemitech.net.cn

Ruby: s.scan(/\d+/)
来源：http://wq.521024.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://fl.jianghongdianzi.cn

[I03] 提取捕获分组
来源：http://pr.szsharing.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://tf.panjiajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wk.shxzskj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://xh.chemitech.net.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yu.szxytkj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://yp.nicolike.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ti.jctech888.com.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://me.lnxyls.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://yc.szsharing.cn

[I04] 正则替换
来源：http://oh.9csxet.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://bd.muxihuayi.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.haigaiapp.cn

JS:   s.replace(/\d+/g, "#")
来源：http://zb.hnjuh.cn

TS:   s.replace(/\d+/g, "#")
来源：http://tb.huixinmuqiang.cn

Java: s.replaceAll("\\d+", "#")
来源：http://mw.colortex.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://fo.hahajie.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sn.asd995.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://jj.muxihuayi.cn

[I05] 按正则拆分
来源：http://aa.huixiangedu.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://gx.gzmigu.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://qu.nszjky.cn

JS:   s.split(/\s*,\s*/)
来源：http://br.gzmigu.cn

TS:   s.split(/\s*,\s*/)
来源：http://vt.wgjwhj.cn

Java: s.split("\\s*,\\s*")
来源：http://bt.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://gu.521024.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sj.shxzskj.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://fk.szxytkj.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://cb.newstarts.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://bw.shxzukj.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://df.shxzskj.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tr.yuexingan06.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://tz.huixinmuqiang.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://nc.bookmarksfly.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ob.gzmigu.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://qh.chemitech.net.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://io.jianghongdianzi.cn

[I07] 忽略大小写与多行模式
来源：http://pg.jctech888.com.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://bt.gzmigu.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ow.nszjky.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ib.haigaiapp.cn

TS:   /error/gim
来源：http://hn.bjjhwx.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://dc.haigaiapp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://vn.bjjhwx.cn

Ruby: s.scan(/error/i)
来源：http://xw.panjiajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://oy.nicolike.cn

[I08] 贪婪与非贪婪匹配
来源：http://yk.colortex.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://fo.lnxyls.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://ob.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://vu.lnxyls.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://xy.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://sj.9csxet.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://qr.9csxet.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://lf.bookmarksfly.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://yp.521024.cn

================================================================================
来源：http://jg.huixinmuqiang.cn

J. 日期与时间
来源：http://ht.haigaiapp.cn

================================================================================
来源：http://kw.colortex.cn

[J01] 获取当前时间
来源：http://xt.yuexingan06.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ic.chemitech.net.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://wa.colortex.cn

JS:   new Date();  Date.now()
来源：http://xa.9csxet.cn

TS:   new Date();  Date.now()
来源：http://ek.haigaiapp.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://cc.yuntaijiaju.cn

Go:   time.Now()
来源：http://um.shtwfgs.cn

Ruby: Time.now
来源：http://od.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://uf.nszjky.cn

[J02] 格式化输出
来源：http://jw.muxihuayi.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://yk.huixiangedu.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://av.9csxet.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://mv.9csxet.cn

TS:   d.toISOString()
来源：http://qr.bjjhwx.cn


<!-- 参考信息 -->