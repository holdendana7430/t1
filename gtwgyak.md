代发 wailian999

Java: class Admin extends User {}
来源：http://ye.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://gg.newstarts.cn

Ruby: class Admin < User; end
来源：http://jp.nszjky.cn

C#:   class Admin : User {}
来源：http://ij.shxzukj.cn

[G06] 重写方法
来源：http://ge.shxzskj.cn

Py:   def greet(self): return "admin"
来源：http://wg.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fm.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://ym.haigaiapp.cn

TS:   greet(): string { return "admin"; }
来源：http://sa.9csxet.cn

Java: @Override String greet() { return "admin"; }
来源：http://nh.newstarts.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://se.yuexingan06.cn

Ruby: def greet; "admin"; end
来源：http://gz.hahajie.cn

C#:   public override string Greet() => "admin";
来源：http://cu.shxzskj.cn

[G07] 调用父类方法
来源：http://al.521024.cn

Py:   super().greet()
来源：http://wg.lnxyls.cn

PHP:  parent::greet();
来源：http://ou.huanxung.cn

JS:   super.greet();
来源：http://nf.shxzskj.cn

TS:   super.greet();
来源：http://pp.gzmigu.cn

Java: super.greet();
来源：http://tr.colortex.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://sz.szsharing.cn

Ruby: super
来源：http://zd.hnjuh.cn

C#:   base.Greet();
来源：http://hw.szxytkj.cn

[G08] 静态方法与属性
来源：http://wb.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ff.521024.cn

PHP:  public static function f() {}
来源：http://cf.lnxyls.cn

JS:   static f() {}
来源：http://ol.yuexingan06.cn

TS:   static f(): void {}
来源：http://xg.jctech888.com.cn

Java: static void f() {}
来源：http://ox.szsharing.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kc.yuntaijiaju.cn

Ruby: def self.f; end
来源：http://ea.shtwfgs.cn

C#:   public static void F() {}
来源：http://md.9csxet.cn

[G09] 接口 / 抽象类
来源：http://cc.muxihuayi.cn

Py:   from abc import ABC, abstractmethod
来源：http://ky.szsharing.cn

PHP:  interface Shape { public function area(): float; }
来源：http://an.nicolike.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zk.nicolike.cn

TS:   interface Shape { area(): number; }
来源：http://ir.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://jt.nicolike.cn

Go:   type Shape interface { Area() float64 }
来源：http://ju.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fi.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://cf.nszjky.cn

[G10] 访问控制
来源：http://wu.huanxung.cn

Py:   约定 _protected / __private（不强制）
来源：http://wj.bookmarksfly.cn

PHP:  public / protected / private
来源：http://ys.yuexingan06.cn

JS:   #private 字段；其余公开
来源：http://wz.asd995.cn

TS:   public / protected / private
来源：http://my.shxzukj.cn

Java: public / protected / private / 默认包级
来源：http://to.muxihuayi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hu.jianghongdianzi.cn

Ruby: public / protected / private
来源：http://vx.yuntaijiaju.cn

C#:   public / protected / private / internal
来源：http://pq.muxihuayi.cn

[G11] getter / setter
来源：http://ys.szsharing.cn

Py:   @property 与 @x.setter
来源：http://zw.yuntaijiaju.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dg.hahajie.cn

JS:   get name() { return this._name; }
来源：http://ua.bookmarksfly.cn

TS:   get name(): string { return this._name; }
来源：http://wj.muxihuayi.cn

Java: public String getName() { return name; }
来源：http://ww.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://bx.shxzukj.cn

Ruby: attr_accessor :name
来源：http://an.gzmigu.cn

C#:   public string Name { get; set; }
来源：http://vs.bjjhwx.cn

[G12] 对象转字符串
来源：http://gy.nicolike.cn

Py:   def __str__(self): return self.name
来源：http://ef.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://hl.huixinmuqiang.cn

JS:   toString() { return this.name; }
来源：http://bi.gzmigu.cn

TS:   toString(): string { return this.name; }
来源：http://bf.szsharing.cn

Java: @Override public String toString() { return name; }
来源：http://ev.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://pc.shxzskj.cn

Ruby: def to_s; @name; end
来源：http://yh.asd995.cn

C#:   public override string ToString() => Name;
来源：http://xi.huanxung.cn

[G13] 判断对象类型
来源：http://xw.colortex.cn

Py:   isinstance(u, User)
来源：http://rz.wgjwhj.cn

PHP:  $u instanceof User
来源：http://vq.wgjwhj.cn

JS:   u instanceof User
来源：http://xw.bjjhwx.cn

TS:   u instanceof User
来源：http://oj.521024.cn

Java: u instanceof User
来源：http://dp.newstarts.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lw.colortex.cn

Ruby: u.is_a?(User)
来源：http://hn.hahajie.cn

C#:   u is User
来源：http://wb.shxzukj.cn

[G14] 数据类 / record
来源：http://pj.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://du.szsharing.cn

PHP:  // 用 readonly 属性模拟
来源：http://gj.shxzukj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qn.newstarts.cn

TS:   type User = { name: string; age: number };
来源：http://tj.jianghongdianzi.cn

Java: record User(String name, int age) {}
来源：http://mr.muxihuayi.cn

Go:   type User struct { Name string; Age int }
来源：http://zh.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fw.yuntaijiaju.cn

C#:   record User(string Name, int Age);
来源：http://pn.szxytkj.cn

[G15] 枚举
来源：http://we.huixinmuqiang.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kl.hnjuh.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://sv.jctech888.com.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://pv.szxytkj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://rw.huanxung.cn

Java: enum Color { RED, GREEN }
来源：http://dp.gzmigu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qw.hnjuh.cn

Ruby: Color = %i[red green].freeze
来源：http://od.shtwfgs.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://rk.bookmarksfly.cn

[G16] 对象转数组 / 字典
来源：http://xw.hahajie.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zh.hnjuh.cn

PHP:  get_object_vars($obj);
来源：http://rq.shxzukj.cn

JS:   Object.entries(obj)
来源：http://ek.asd995.cn

TS:   Object.entries(obj)
来源：http://vy.huixiangedu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://lk.gzmigu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://iv.hahajie.cn

Ruby: obj.instance_variables
来源：http://dz.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://dy.yuntaijiaju.cn

================================================================================
来源：http://xh.yuntaijiaju.cn

H. 异常与错误处理
来源：http://qn.hahajie.cn

================================================================================
来源：http://yz.9csxet.cn

[H01] try / catch 基础
来源：http://dq.lnxyls.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://sk.shxzukj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://bn.521024.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://de.wgjwhj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nx.asd995.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ub.huanxung.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://iw.colortex.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yz.yuntaijiaju.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sl.szxytkj.cn

[H02] finally / ensure 收尾
来源：http://ha.huanxung.cn

Py:   try: f()⏎finally: cleanup()
来源：http://vy.jianghongdianzi.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://th.muxihuayi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://qh.bjjhwx.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://as.szxytkj.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bs.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://oy.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ij.huanxung.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yk.shtwfgs.cn

[H03] 主动抛出异常
来源：http://ed.bookmarksfly.cn

Py:   raise ValueError("错误信息")
来源：http://bs.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qr.nszjky.cn

JS:   throw new Error("错误信息");
来源：http://wr.jctech888.com.cn

TS:   throw new Error("错误信息");
来源：http://uh.lnxyls.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://db.newstarts.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://zy.shxzskj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://ly.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fr.chemitech.net.cn

[H04] 自定义异常类型
来源：http://cx.huixinmuqiang.cn

Py:   class MyError(Exception): pass
来源：http://zg.muxihuayi.cn

PHP:  class MyError extends RuntimeException {}
来源：http://vg.wgjwhj.cn

JS:   class MyError extends Error {}
来源：http://uq.szsharing.cn

TS:   class MyError extends Error {}
来源：http://je.jianghongdianzi.cn

Java: class MyException extends RuntimeException {}
来源：http://fv.haigaiapp.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ag.bookmarksfly.cn

Ruby: class MyError < StandardError; end
来源：http://jc.szxytkj.cn

C#:   class MyException : Exception {}
来源：http://cb.wgjwhj.cn

[H05] 捕获特定类型
来源：http://nt.9csxet.cn

Py:   except ValueError as e:
来源：http://wb.colortex.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://pr.shtwfgs.cn

JS:   if (e instanceof TypeError) {}
来源：http://ko.yuexingan06.cn

TS:   if (e instanceof TypeError) {}
来源：http://gc.szxytkj.cn

Java: catch (IOException | SQLException e) {}
来源：http://vk.shtwfgs.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://io.asd995.cn

Ruby: rescue ArgumentError => e
来源：http://ei.shtwfgs.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ne.colortex.cn

[H06] 可选值 / 空值安全访问
来源：http://vk.muxihuayi.cn

Py:   value = d.get("k") or default
来源：http://hc.muxihuayi.cn

PHP:  $v = $d["k"] ?? null;
来源：http://jq.panjiajie.cn

JS:   obj?.a?.b;  d ?? default
来源：http://pa.shxzskj.cn

TS:   obj?.a?.b;  d ?? default
来源：http://mt.huanxung.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://bz.lnxyls.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://cc.szxytkj.cn

Ruby: d&.dig(:a, :b)
来源：http://da.bookmarksfly.cn

C#:   obj?.A?.B ?? default
来源：http://oy.yuntaijiaju.cn

[H07] 断言
来源：http://dc.szsharing.cn

Py:   assert x > 0, "必须为正"
来源：http://ls.jianghongdianzi.cn

PHP:  assert($x > 0);
来源：http://ii.shxzskj.cn

JS:   console.assert(x > 0);
来源：http://nd.gzmigu.cn

TS:   console.assert(x > 0);
来源：http://xb.bookmarksfly.cn

Java: assert x > 0 : "必须为正";
来源：http://yj.colortex.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://pj.9csxet.cn

Ruby: raise "必须为正" unless x > 0
来源：http://eb.bookmarksfly.cn

C#:   Debug.Assert(x > 0);
来源：http://nu.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://ke.muxihuayi.cn

Py:   str(e);  traceback.format_exc()
来源：http://si.lnxyls.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://xc.gzmigu.cn

JS:   e.message;  e.stack
来源：http://xc.colortex.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://nt.hnjuh.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://rl.bookmarksfly.cn

Go:   err.Error()
来源：http://ar.shxzukj.cn

Ruby: e.message;  e.backtrace
来源：http://nj.shtwfgs.cn

C#:   e.Message;  e.StackTrace
来源：http://nj.asd995.cn

[H09] 带错误码的异常
来源：http://mq.yuntaijiaju.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://sg.huixinmuqiang.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://xy.panjiajie.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://cc.panjiajie.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://oy.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://gn.wgjwhj.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://ru.huixinmuqiang.cn

Ruby: raise MyError.new("fail", 500)
来源：http://yr.yuntaijiaju.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://zi.muxihuayi.cn

[H10] 资源自动释放
来源：http://xi.bookmarksfly.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://sd.bookmarksfly.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://ss.hahajie.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://gc.hnjuh.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qi.szsharing.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hb.521024.cn

Go:   defer f.Close()
来源：http://hj.haigaiapp.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://ed.bjjhwx.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://de.haigaiapp.cn

================================================================================
来源：http://cj.gzmigu.cn

I. 正则表达式
来源：http://ji.nicolike.cn

================================================================================
来源：http://hl.jianghongdianzi.cn

[I01] 判断是否匹配
来源：http://ne.asd995.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ac.colortex.cn

PHP:  preg_match('/\d+/', $s);
来源：http://md.bookmarksfly.cn

JS:   /\d+/.test(s)
来源：http://xr.bookmarksfly.cn

TS:   /\d+/.test(s)
来源：http://zi.shxzskj.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://lg.haigaiapp.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://po.shxzukj.cn

Ruby: s.match?(/\d+/)
来源：http://wf.521024.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fz.haigaiapp.cn

[I02] 提取所有匹配
来源：http://ld.szxytkj.cn

Py:   re.findall(r"\d+", s)
来源：http://nf.panjiajie.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wv.gzmigu.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://so.wgjwhj.cn

TS:   s.match(/\d+/g)
来源：http://nj.wgjwhj.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://ji.huixiangedu.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://or.jctech888.com.cn

Ruby: s.scan(/\d+/)
来源：http://ia.newstarts.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mc.szsharing.cn

[I03] 提取捕获分组
来源：http://ji.chemitech.net.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mr.shxzskj.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://md.bjjhwx.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ng.521024.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://yg.panjiajie.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://xt.huixinmuqiang.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://vm.yuntaijiaju.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://nx.hnjuh.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hw.shxzukj.cn

[I04] 正则替换
来源：http://cz.jianghongdianzi.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://rc.shtwfgs.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://xz.gzmigu.cn

JS:   s.replace(/\d+/g, "#")
来源：http://ls.shxzukj.cn

TS:   s.replace(/\d+/g, "#")
来源：http://bf.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://zk.nicolike.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ew.bjjhwx.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://yi.huanxung.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mv.haigaiapp.cn

[I05] 按正则拆分
来源：http://ix.shxzukj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://mv.shtwfgs.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://xf.9csxet.cn

JS:   s.split(/\s*,\s*/)
来源：http://nx.nicolike.cn

TS:   s.split(/\s*,\s*/)
来源：http://dd.newstarts.cn

Java: s.split("\\s*,\\s*")
来源：http://py.nszjky.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://ya.shxzskj.cn

Ruby: s.split(/\s*,\s*/)
来源：http://sk.asd995.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://yw.jctech888.com.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://yv.yuntaijiaju.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://xn.asd995.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://nl.yuexingan06.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vn.newstarts.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://ze.jianghongdianzi.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://yp.szsharing.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://jz.hahajie.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://rg.hnjuh.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mz.bjjhwx.cn

[I07] 忽略大小写与多行模式
来源：http://uy.nszjky.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://vj.9csxet.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://bb.newstarts.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://on.newstarts.cn

TS:   /error/gim
来源：http://zs.lnxyls.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://sd.haigaiapp.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://fj.shtwfgs.cn

Ruby: s.scan(/error/i)
来源：http://nh.9csxet.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lz.huanxung.cn

[I08] 贪婪与非贪婪匹配
来源：http://eh.jctech888.com.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://vv.shtwfgs.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://zd.huixinmuqiang.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wl.yuexingan06.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://tm.gzmigu.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://ab.chemitech.net.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zn.yuexingan06.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://ml.newstarts.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://dn.bjjhwx.cn

================================================================================
来源：http://pa.nszjky.cn

J. 日期与时间
来源：http://eo.shtwfgs.cn

================================================================================
来源：http://de.huixiangedu.cn

[J01] 获取当前时间
来源：http://qn.muxihuayi.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://wo.nszjky.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://cl.shxzskj.cn

JS:   new Date();  Date.now()
来源：http://be.shxzskj.cn

TS:   new Date();  Date.now()
来源：http://wv.asd995.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://fy.gzmigu.cn

Go:   time.Now()
来源：http://xc.jctech888.com.cn

Ruby: Time.now
来源：http://ss.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://xc.szsharing.cn

[J02] 格式化输出
来源：http://as.bookmarksfly.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://uf.newstarts.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://ju.gzmigu.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://xb.shxzukj.cn

TS:   d.toISOString()
来源：http://ex.yuexingan06.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cx.shtwfgs.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hg.jctech888.com.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://es.wgjwhj.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hw.bjjhwx.cn

[J03] 字符串解析为日期
来源：http://xp.hnjuh.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://us.wgjwhj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://xb.chemitech.net.cn

JS:   new Date("2024-01-02")
来源：http://rz.bookmarksfly.cn

TS:   new Date("2024-01-02")
来源：http://ha.shtwfgs.cn

Java: LocalDate.parse("2024-01-02")
来源：http://it.newstarts.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://cc.huixiangedu.cn

Ruby: Date.parse("2024-01-02")
来源：http://th.gzmigu.cn


<!-- 参考信息 -->