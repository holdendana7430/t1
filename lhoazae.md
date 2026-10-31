代发 wailian999

Java: class Admin extends User {}
来源：http://cw.nszjky.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://us.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://ik.muxihuayi.cn

C#:   class Admin : User {}
来源：http://cs.yuexingan06.cn

[G06] 重写方法
来源：http://bl.szsharing.cn

Py:   def greet(self): return "admin"
来源：http://ml.wgjwhj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://nj.bjjhwx.cn

JS:   greet() { return "admin"; }
来源：http://yt.bookmarksfly.cn

TS:   greet(): string { return "admin"; }
来源：http://mv.lnxyls.cn

Java: @Override String greet() { return "admin"; }
来源：http://gu.shtwfgs.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pc.wgjwhj.cn

Ruby: def greet; "admin"; end
来源：http://yd.colortex.cn

C#:   public override string Greet() => "admin";
来源：http://ri.jctech888.com.cn

[G07] 调用父类方法
来源：http://cl.bookmarksfly.cn

Py:   super().greet()
来源：http://ry.shtwfgs.cn

PHP:  parent::greet();
来源：http://rk.szxytkj.cn

JS:   super.greet();
来源：http://ta.yuexingan06.cn

TS:   super.greet();
来源：http://zs.nicolike.cn

Java: super.greet();
来源：http://rp.colortex.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://oo.9csxet.cn

Ruby: super
来源：http://iy.9csxet.cn

C#:   base.Greet();
来源：http://fr.9csxet.cn

[G08] 静态方法与属性
来源：http://ka.yuexingan06.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kc.muxihuayi.cn

PHP:  public static function f() {}
来源：http://ci.newstarts.cn

JS:   static f() {}
来源：http://iu.yuntaijiaju.cn

TS:   static f(): void {}
来源：http://lw.newstarts.cn

Java: static void f() {}
来源：http://no.shxzskj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://vz.huixinmuqiang.cn

Ruby: def self.f; end
来源：http://rw.yuntaijiaju.cn

C#:   public static void F() {}
来源：http://ck.nszjky.cn

[G09] 接口 / 抽象类
来源：http://vl.huixinmuqiang.cn

Py:   from abc import ABC, abstractmethod
来源：http://ej.shxzskj.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vw.9csxet.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ic.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://ts.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://le.wgjwhj.cn

Go:   type Shape interface { Area() float64 }
来源：http://mg.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://jn.szsharing.cn

C#:   interface IShape { double Area(); }
来源：http://ct.bjjhwx.cn

[G10] 访问控制
来源：http://bu.szsharing.cn

Py:   约定 _protected / __private（不强制）
来源：http://cc.shxzskj.cn

PHP:  public / protected / private
来源：http://zd.newstarts.cn

JS:   #private 字段；其余公开
来源：http://zv.yuntaijiaju.cn

TS:   public / protected / private
来源：http://uu.wgjwhj.cn

Java: public / protected / private / 默认包级
来源：http://ra.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mf.huanxung.cn

Ruby: public / protected / private
来源：http://zq.nszjky.cn

C#:   public / protected / private / internal
来源：http://rf.panjiajie.cn

[G11] getter / setter
来源：http://lv.nszjky.cn

Py:   @property 与 @x.setter
来源：http://xg.wgjwhj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://gk.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://op.muxihuayi.cn

TS:   get name(): string { return this._name; }
来源：http://cl.panjiajie.cn

Java: public String getName() { return name; }
来源：http://eb.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tp.hahajie.cn

Ruby: attr_accessor :name
来源：http://ue.hahajie.cn

C#:   public string Name { get; set; }
来源：http://vo.shtwfgs.cn

[G12] 对象转字符串
来源：http://bs.yuexingan06.cn

Py:   def __str__(self): return self.name
来源：http://ol.521024.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://al.shxzukj.cn

JS:   toString() { return this.name; }
来源：http://sx.huixinmuqiang.cn

TS:   toString(): string { return this.name; }
来源：http://sa.hahajie.cn

Java: @Override public String toString() { return name; }
来源：http://il.nszjky.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ah.jctech888.com.cn

Ruby: def to_s; @name; end
来源：http://hc.hahajie.cn

C#:   public override string ToString() => Name;
来源：http://ls.nszjky.cn

[G13] 判断对象类型
来源：http://if.huanxung.cn

Py:   isinstance(u, User)
来源：http://cm.yuntaijiaju.cn

PHP:  $u instanceof User
来源：http://nc.muxihuayi.cn

JS:   u instanceof User
来源：http://di.huixinmuqiang.cn

TS:   u instanceof User
来源：http://xi.jianghongdianzi.cn

Java: u instanceof User
来源：http://mq.gzmigu.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xt.szxytkj.cn

Ruby: u.is_a?(User)
来源：http://bm.huixinmuqiang.cn

C#:   u is User
来源：http://yx.szsharing.cn

[G14] 数据类 / record
来源：http://nv.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ny.huixiangedu.cn

PHP:  // 用 readonly 属性模拟
来源：http://ix.bjjhwx.cn

JS:   // 无内置：普通类或对象字面量
来源：http://vi.521024.cn

TS:   type User = { name: string; age: number };
来源：http://he.nszjky.cn

Java: record User(String name, int age) {}
来源：http://jz.chemitech.net.cn

Go:   type User struct { Name string; Age int }
来源：http://zr.521024.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://go.nszjky.cn

C#:   record User(string Name, int Age);
来源：http://sh.shxzskj.cn

[G15] 枚举
来源：http://oy.shxzukj.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cu.shxzskj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://pt.hahajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xq.huixinmuqiang.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://to.szxytkj.cn

Java: enum Color { RED, GREEN }
来源：http://fw.shtwfgs.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://kk.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://fs.szsharing.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bd.jianghongdianzi.cn

[G16] 对象转数组 / 字典
来源：http://fq.colortex.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://qe.shxzukj.cn

PHP:  get_object_vars($obj);
来源：http://ll.hnjuh.cn

JS:   Object.entries(obj)
来源：http://iv.haigaiapp.cn

TS:   Object.entries(obj)
来源：http://zf.shxzukj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gy.haigaiapp.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pa.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://ui.jctech888.com.cn

C#:   // 用反射或 System.Text.Json
来源：http://ry.hahajie.cn

================================================================================
来源：http://fc.shxzukj.cn

H. 异常与错误处理
来源：http://fy.yuexingan06.cn

================================================================================
来源：http://jq.hnjuh.cn

[H01] try / catch 基础
来源：http://yf.huixiangedu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dd.nszjky.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://fu.lnxyls.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://zn.huixiangedu.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ld.yuntaijiaju.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ki.newstarts.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ye.szxytkj.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://nl.wgjwhj.cn

[H02] finally / ensure 收尾
来源：http://lh.521024.cn

Py:   try: f()⏎finally: cleanup()
来源：http://me.muxihuayi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://cl.asd995.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yl.shxzskj.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://rk.asd995.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ef.hnjuh.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ve.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ph.szsharing.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://no.wgjwhj.cn

[H03] 主动抛出异常
来源：http://id.colortex.cn

Py:   raise ValueError("错误信息")
来源：http://ek.bookmarksfly.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rd.jianghongdianzi.cn

JS:   throw new Error("错误信息");
来源：http://wa.shxzskj.cn

TS:   throw new Error("错误信息");
来源：http://hk.hahajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://fv.colortex.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://fq.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rp.9csxet.cn

C#:   throw new ArgumentException("错误信息");
来源：http://bl.gzmigu.cn

[H04] 自定义异常类型
来源：http://mp.chemitech.net.cn

Py:   class MyError(Exception): pass
来源：http://on.lnxyls.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zu.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://ox.asd995.cn

TS:   class MyError extends Error {}
来源：http://bw.shxzskj.cn

Java: class MyException extends RuntimeException {}
来源：http://ik.chemitech.net.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://cw.huixiangedu.cn

Ruby: class MyError < StandardError; end
来源：http://ro.hahajie.cn

C#:   class MyException : Exception {}
来源：http://dz.yuntaijiaju.cn

[H05] 捕获特定类型
来源：http://fr.haigaiapp.cn

Py:   except ValueError as e:
来源：http://cg.chemitech.net.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ge.shxzskj.cn

JS:   if (e instanceof TypeError) {}
来源：http://gp.yuexingan06.cn

TS:   if (e instanceof TypeError) {}
来源：http://nb.hnjuh.cn

Java: catch (IOException | SQLException e) {}
来源：http://ov.hahajie.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://if.panjiajie.cn

Ruby: rescue ArgumentError => e
来源：http://iw.9csxet.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://sy.huanxung.cn

[H06] 可选值 / 空值安全访问
来源：http://he.wgjwhj.cn

Py:   value = d.get("k") or default
来源：http://ye.521024.cn

PHP:  $v = $d["k"] ?? null;
来源：http://us.huanxung.cn

JS:   obj?.a?.b;  d ?? default
来源：http://mx.shxzukj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://cg.hnjuh.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hb.yuexingan06.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://qg.bookmarksfly.cn

Ruby: d&.dig(:a, :b)
来源：http://br.jianghongdianzi.cn

C#:   obj?.A?.B ?? default
来源：http://zv.huixiangedu.cn

[H07] 断言
来源：http://kn.colortex.cn

Py:   assert x > 0, "必须为正"
来源：http://ze.hnjuh.cn

PHP:  assert($x > 0);
来源：http://er.szxytkj.cn

JS:   console.assert(x > 0);
来源：http://sz.szsharing.cn

TS:   console.assert(x > 0);
来源：http://yr.yuexingan06.cn

Java: assert x > 0 : "必须为正";
来源：http://he.panjiajie.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://un.panjiajie.cn

Ruby: raise "必须为正" unless x > 0
来源：http://zx.shxzskj.cn

C#:   Debug.Assert(x > 0);
来源：http://tf.lnxyls.cn

[H08] 获取错误信息与堆栈
来源：http://jl.huixiangedu.cn

Py:   str(e);  traceback.format_exc()
来源：http://km.muxihuayi.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://pq.wgjwhj.cn

JS:   e.message;  e.stack
来源：http://yu.shxzukj.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://qq.shxzukj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://em.huanxung.cn

Go:   err.Error()
来源：http://ln.yuexingan06.cn

Ruby: e.message;  e.backtrace
来源：http://mg.yuexingan06.cn

C#:   e.Message;  e.StackTrace
来源：http://lz.lnxyls.cn

[H09] 带错误码的异常
来源：http://lx.lnxyls.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://cd.hnjuh.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://nv.muxihuayi.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://kh.chemitech.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://sa.huanxung.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://oa.huixiangedu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://bu.gzmigu.cn

Ruby: raise MyError.new("fail", 500)
来源：http://fd.huanxung.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vn.huixiangedu.cn

[H10] 资源自动释放
来源：http://ld.gzmigu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://dp.gzmigu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yr.yuexingan06.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mv.wgjwhj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://xd.521024.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://sv.muxihuayi.cn

Go:   defer f.Close()
来源：http://np.huanxung.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ng.chemitech.net.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://kv.jctech888.com.cn

================================================================================
来源：http://cm.bookmarksfly.cn

I. 正则表达式
来源：http://kf.asd995.cn

================================================================================
来源：http://oz.9csxet.cn

[I01] 判断是否匹配
来源：http://ow.hnjuh.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mu.jianghongdianzi.cn

PHP:  preg_match('/\d+/', $s);
来源：http://om.szsharing.cn

JS:   /\d+/.test(s)
来源：http://fb.shxzukj.cn

TS:   /\d+/.test(s)
来源：http://lc.jianghongdianzi.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://tt.521024.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://nh.nszjky.cn

Ruby: s.match?(/\d+/)
来源：http://sj.yuexingan06.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://iv.521024.cn

[I02] 提取所有匹配
来源：http://op.muxihuayi.cn

Py:   re.findall(r"\d+", s)
来源：http://ln.muxihuayi.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rm.szsharing.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://xy.muxihuayi.cn

TS:   s.match(/\d+/g)
来源：http://iw.huixiangedu.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://xc.nicolike.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://bd.gzmigu.cn

Ruby: s.scan(/\d+/)
来源：http://yu.shtwfgs.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://ol.nszjky.cn

[I03] 提取捕获分组
来源：http://wg.bookmarksfly.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://ng.wgjwhj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gs.huanxung.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://cb.szxytkj.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xt.gzmigu.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://lb.jctech888.com.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rl.lnxyls.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://uj.wgjwhj.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://bj.szsharing.cn

[I04] 正则替换
来源：http://ev.nszjky.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://ed.shtwfgs.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://ty.shtwfgs.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ul.nicolike.cn

TS:   s.replace(/\d+/g, "#")
来源：http://vh.yuexingan06.cn

Java: s.replaceAll("\\d+", "#")
来源：http://go.hahajie.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ql.shtwfgs.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ra.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gl.huanxung.cn

[I05] 按正则拆分
来源：http://uu.shxzskj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://hl.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://gb.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://nc.haigaiapp.cn

TS:   s.split(/\s*,\s*/)
来源：http://xp.shxzukj.cn

Java: s.split("\\s*,\\s*")
来源：http://eo.shxzukj.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://is.szsharing.cn

Ruby: s.split(/\s*,\s*/)
来源：http://rk.lnxyls.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://jy.yuntaijiaju.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yf.lnxyls.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://kw.shtwfgs.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wm.huanxung.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://up.yuntaijiaju.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://bf.huixinmuqiang.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://up.huanxung.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wv.nicolike.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://it.bookmarksfly.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://ag.hnjuh.cn

[I07] 忽略大小写与多行模式
来源：http://wo.9csxet.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://if.jctech888.com.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://fj.szxytkj.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nd.chemitech.net.cn

TS:   /error/gim
来源：http://vm.9csxet.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://os.wgjwhj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://wi.haigaiapp.cn

Ruby: s.scan(/error/i)
来源：http://yu.huixinmuqiang.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://fc.szxytkj.cn

[I08] 贪婪与非贪婪匹配
来源：http://lk.huixiangedu.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://ld.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://du.nszjky.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://ja.shxzukj.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://oa.chemitech.net.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://el.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://kz.chemitech.net.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xs.nicolike.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://uv.nicolike.cn

================================================================================
来源：http://gc.huanxung.cn

J. 日期与时间
来源：http://oh.haigaiapp.cn

================================================================================
来源：http://ou.newstarts.cn

[J01] 获取当前时间
来源：http://cx.jianghongdianzi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vz.hnjuh.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://lu.gzmigu.cn

JS:   new Date();  Date.now()
来源：http://hn.wgjwhj.cn

TS:   new Date();  Date.now()
来源：http://qd.9csxet.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://ct.521024.cn

Go:   time.Now()
来源：http://dw.huixiangedu.cn

Ruby: Time.now
来源：http://hp.hnjuh.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ft.wgjwhj.cn

[J02] 格式化输出
来源：http://lo.huixiangedu.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ba.wgjwhj.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://pb.bookmarksfly.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gb.shtwfgs.cn

TS:   d.toISOString()
来源：http://cb.chemitech.net.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://nl.shxzskj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://vx.yuntaijiaju.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://vg.lnxyls.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://fv.yuexingan06.cn

[J03] 字符串解析为日期
来源：http://to.szxytkj.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://jm.nszjky.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://en.wgjwhj.cn

JS:   new Date("2024-01-02")
来源：http://gq.hnjuh.cn

TS:   new Date("2024-01-02")
来源：http://ly.nicolike.cn

Java: LocalDate.parse("2024-01-02")
来源：http://zr.521024.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://xc.jctech888.com.cn

Ruby: Date.parse("2024-01-02")
来源：http://tt.colortex.cn


<!-- 参考信息 -->