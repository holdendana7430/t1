代发 wailian999

Java: class Admin extends User {}
来源：http://cu.nszjky.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jm.shtwfgs.cn

Ruby: class Admin < User; end
来源：http://ep.bookmarksfly.cn

C#:   class Admin : User {}
来源：http://jr.9csxet.cn

[G06] 重写方法
来源：http://yb.huixinmuqiang.cn

Py:   def greet(self): return "admin"
来源：http://nh.yuexingan06.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ip.521024.cn

JS:   greet() { return "admin"; }
来源：http://qv.gzmigu.cn

TS:   greet(): string { return "admin"; }
来源：http://vw.muxihuayi.cn

Java: @Override String greet() { return "admin"; }
来源：http://mk.shtwfgs.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ge.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://wc.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://es.muxihuayi.cn

[G07] 调用父类方法
来源：http://gi.huixiangedu.cn

Py:   super().greet()
来源：http://di.521024.cn

PHP:  parent::greet();
来源：http://dl.huanxung.cn

JS:   super.greet();
来源：http://mf.hnjuh.cn

TS:   super.greet();
来源：http://ds.huixinmuqiang.cn

Java: super.greet();
来源：http://ea.bookmarksfly.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zj.jianghongdianzi.cn

Ruby: super
来源：http://xo.bookmarksfly.cn

C#:   base.Greet();
来源：http://op.colortex.cn

[G08] 静态方法与属性
来源：http://nb.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vz.huixinmuqiang.cn

PHP:  public static function f() {}
来源：http://cu.9csxet.cn

JS:   static f() {}
来源：http://ly.bjjhwx.cn

TS:   static f(): void {}
来源：http://qm.asd995.cn

Java: static void f() {}
来源：http://on.chemitech.net.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fk.shxzukj.cn

Ruby: def self.f; end
来源：http://fz.nszjky.cn

C#:   public static void F() {}
来源：http://es.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://de.bookmarksfly.cn

Py:   from abc import ABC, abstractmethod
来源：http://ih.asd995.cn

PHP:  interface Shape { public function area(): float; }
来源：http://vl.bookmarksfly.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ic.jctech888.com.cn

TS:   interface Shape { area(): number; }
来源：http://yt.colortex.cn

Java: interface Shape { double area(); }
来源：http://ni.hnjuh.cn

Go:   type Shape interface { Area() float64 }
来源：http://vq.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ek.shxzskj.cn

C#:   interface IShape { double Area(); }
来源：http://or.yuntaijiaju.cn

[G10] 访问控制
来源：http://np.shtwfgs.cn

Py:   约定 _protected / __private（不强制）
来源：http://mj.asd995.cn

PHP:  public / protected / private
来源：http://qg.szsharing.cn

JS:   #private 字段；其余公开
来源：http://go.nicolike.cn

TS:   public / protected / private
来源：http://dt.shtwfgs.cn

Java: public / protected / private / 默认包级
来源：http://zm.panjiajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://gl.gzmigu.cn

Ruby: public / protected / private
来源：http://ig.gzmigu.cn

C#:   public / protected / private / internal
来源：http://zs.szxytkj.cn

[G11] getter / setter
来源：http://cw.huixinmuqiang.cn

Py:   @property 与 @x.setter
来源：http://jm.newstarts.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yy.huixinmuqiang.cn

JS:   get name() { return this._name; }
来源：http://gg.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://hm.9csxet.cn

Java: public String getName() { return name; }
来源：http://tc.bookmarksfly.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://lw.newstarts.cn

Ruby: attr_accessor :name
来源：http://cs.huixiangedu.cn

C#:   public string Name { get; set; }
来源：http://de.szsharing.cn

[G12] 对象转字符串
来源：http://or.wgjwhj.cn

Py:   def __str__(self): return self.name
来源：http://tv.jctech888.com.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vi.bjjhwx.cn

JS:   toString() { return this.name; }
来源：http://fn.yuntaijiaju.cn

TS:   toString(): string { return this.name; }
来源：http://me.jianghongdianzi.cn

Java: @Override public String toString() { return name; }
来源：http://gx.521024.cn

Go:   func (u User) String() string { return u.Name }
来源：http://wc.asd995.cn

Ruby: def to_s; @name; end
来源：http://bq.panjiajie.cn

C#:   public override string ToString() => Name;
来源：http://rx.yuexingan06.cn

[G13] 判断对象类型
来源：http://ma.szxytkj.cn

Py:   isinstance(u, User)
来源：http://cq.lnxyls.cn

PHP:  $u instanceof User
来源：http://pc.szsharing.cn

JS:   u instanceof User
来源：http://vj.521024.cn

TS:   u instanceof User
来源：http://kv.muxihuayi.cn

Java: u instanceof User
来源：http://zq.jianghongdianzi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://rv.shxzukj.cn

Ruby: u.is_a?(User)
来源：http://kb.gzmigu.cn

C#:   u is User
来源：http://tm.chemitech.net.cn

[G14] 数据类 / record
来源：http://fs.nicolike.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://eo.colortex.cn

PHP:  // 用 readonly 属性模拟
来源：http://tx.panjiajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ev.bjjhwx.cn

TS:   type User = { name: string; age: number };
来源：http://qj.gzmigu.cn

Java: record User(String name, int age) {}
来源：http://sy.521024.cn

Go:   type User struct { Name string; Age int }
来源：http://bv.bookmarksfly.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wt.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://th.huixiangedu.cn

[G15] 枚举
来源：http://qk.huixiangedu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://rk.shxzukj.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://kz.hnjuh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://rx.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vc.szxytkj.cn

Java: enum Color { RED, GREEN }
来源：http://wj.nszjky.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://vg.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://zw.521024.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oz.bjjhwx.cn

[G16] 对象转数组 / 字典
来源：http://ap.shxzskj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://od.yuntaijiaju.cn

PHP:  get_object_vars($obj);
来源：http://hb.jctech888.com.cn

JS:   Object.entries(obj)
来源：http://in.haigaiapp.cn

TS:   Object.entries(obj)
来源：http://ma.shtwfgs.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ma.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://vu.9csxet.cn

Ruby: obj.instance_variables
来源：http://ph.521024.cn

C#:   // 用反射或 System.Text.Json
来源：http://qs.hahajie.cn

================================================================================
来源：http://gc.hnjuh.cn

H. 异常与错误处理
来源：http://et.asd995.cn

================================================================================
来源：http://ax.bookmarksfly.cn

[H01] try / catch 基础
来源：http://rm.9csxet.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://eo.haigaiapp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://et.szxytkj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://te.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://nb.asd995.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://tk.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://nx.lnxyls.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://uh.yuexingan06.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hj.yuntaijiaju.cn

[H02] finally / ensure 收尾
来源：http://rz.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://pg.gzmigu.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://yr.lnxyls.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://kt.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zw.521024.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ux.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://mq.haigaiapp.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://da.shxzukj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://bv.bjjhwx.cn

[H03] 主动抛出异常
来源：http://nx.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://ah.shxzukj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pt.yuntaijiaju.cn

JS:   throw new Error("错误信息");
来源：http://nz.jianghongdianzi.cn

TS:   throw new Error("错误信息");
来源：http://fc.bookmarksfly.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://gt.hahajie.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://gb.huixinmuqiang.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://sg.szxytkj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://fm.jianghongdianzi.cn

[H04] 自定义异常类型
来源：http://xg.hahajie.cn

Py:   class MyError(Exception): pass
来源：http://wx.szsharing.cn

PHP:  class MyError extends RuntimeException {}
来源：http://va.jctech888.com.cn

JS:   class MyError extends Error {}
来源：http://sx.jianghongdianzi.cn

TS:   class MyError extends Error {}
来源：http://li.huanxung.cn

Java: class MyException extends RuntimeException {}
来源：http://ji.panjiajie.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://bf.huanxung.cn

Ruby: class MyError < StandardError; end
来源：http://sg.yuexingan06.cn

C#:   class MyException : Exception {}
来源：http://ds.yuntaijiaju.cn

[H05] 捕获特定类型
来源：http://yg.newstarts.cn

Py:   except ValueError as e:
来源：http://bm.jctech888.com.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ni.huanxung.cn

JS:   if (e instanceof TypeError) {}
来源：http://ys.colortex.cn

TS:   if (e instanceof TypeError) {}
来源：http://yd.panjiajie.cn

Java: catch (IOException | SQLException e) {}
来源：http://zb.asd995.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://su.nszjky.cn

Ruby: rescue ArgumentError => e
来源：http://wg.bookmarksfly.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wm.gzmigu.cn

[H06] 可选值 / 空值安全访问
来源：http://bw.shtwfgs.cn

Py:   value = d.get("k") or default
来源：http://mq.haigaiapp.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ba.nicolike.cn

JS:   obj?.a?.b;  d ?? default
来源：http://xc.muxihuayi.cn

TS:   obj?.a?.b;  d ?? default
来源：http://fo.521024.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://ld.muxihuayi.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://ev.bookmarksfly.cn

Ruby: d&.dig(:a, :b)
来源：http://vo.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://do.521024.cn

[H07] 断言
来源：http://gm.nszjky.cn

Py:   assert x > 0, "必须为正"
来源：http://rd.9csxet.cn

PHP:  assert($x > 0);
来源：http://os.colortex.cn

JS:   console.assert(x > 0);
来源：http://yw.gzmigu.cn

TS:   console.assert(x > 0);
来源：http://ow.9csxet.cn

Java: assert x > 0 : "必须为正";
来源：http://tf.haigaiapp.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://nh.huanxung.cn

Ruby: raise "必须为正" unless x > 0
来源：http://dq.yuexingan06.cn

C#:   Debug.Assert(x > 0);
来源：http://fi.huanxung.cn

[H08] 获取错误信息与堆栈
来源：http://fh.lnxyls.cn

Py:   str(e);  traceback.format_exc()
来源：http://fo.lnxyls.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://qh.lnxyls.cn

JS:   e.message;  e.stack
来源：http://ej.nicolike.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://wr.shxzskj.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://qw.haigaiapp.cn

Go:   err.Error()
来源：http://ci.huanxung.cn

Ruby: e.message;  e.backtrace
来源：http://gx.shxzukj.cn

C#:   e.Message;  e.StackTrace
来源：http://na.lnxyls.cn

[H09] 带错误码的异常
来源：http://yg.bookmarksfly.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tc.521024.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://mg.wgjwhj.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://vc.shxzukj.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://ei.haigaiapp.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://rs.hahajie.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://iw.wgjwhj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://io.asd995.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://px.huixinmuqiang.cn

[H10] 资源自动释放
来源：http://kb.shtwfgs.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://ld.panjiajie.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://yu.hnjuh.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://xv.shxzskj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://lj.jctech888.com.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://kf.shxzskj.cn

Go:   defer f.Close()
来源：http://kb.lnxyls.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://gh.jctech888.com.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://lc.muxihuayi.cn

================================================================================
来源：http://aq.hahajie.cn

I. 正则表达式
来源：http://wo.bookmarksfly.cn

================================================================================
来源：http://it.colortex.cn

[I01] 判断是否匹配
来源：http://at.gzmigu.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://ek.newstarts.cn

PHP:  preg_match('/\d+/', $s);
来源：http://bp.521024.cn

JS:   /\d+/.test(s)
来源：http://gr.huanxung.cn

TS:   /\d+/.test(s)
来源：http://vi.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://pz.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://ae.bookmarksfly.cn

Ruby: s.match?(/\d+/)
来源：http://it.jctech888.com.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://fu.521024.cn

[I02] 提取所有匹配
来源：http://db.haigaiapp.cn

Py:   re.findall(r"\d+", s)
来源：http://py.nicolike.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uf.nszjky.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://nl.bookmarksfly.cn

TS:   s.match(/\d+/g)
来源：http://vq.szsharing.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://qm.shxzukj.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://pg.huixinmuqiang.cn

Ruby: s.scan(/\d+/)
来源：http://vy.lnxyls.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://gw.colortex.cn

[I03] 提取捕获分组
来源：http://xe.muxihuayi.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://zx.hahajie.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://gs.huixiangedu.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ay.yuntaijiaju.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://zr.9csxet.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://nx.yuntaijiaju.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://yq.chemitech.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://zs.hahajie.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hm.chemitech.net.cn

[I04] 正则替换
来源：http://oc.hahajie.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://fa.521024.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://es.wgjwhj.cn

JS:   s.replace(/\d+/g, "#")
来源：http://fm.newstarts.cn

TS:   s.replace(/\d+/g, "#")
来源：http://kl.nicolike.cn

Java: s.replaceAll("\\d+", "#")
来源：http://sk.newstarts.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://ed.shxzukj.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://sh.hnjuh.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://gv.lnxyls.cn

[I05] 按正则拆分
来源：http://ts.chemitech.net.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://if.yuexingan06.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cn.gzmigu.cn

JS:   s.split(/\s*,\s*/)
来源：http://qx.szsharing.cn

TS:   s.split(/\s*,\s*/)
来源：http://qv.9csxet.cn

Java: s.split("\\s*,\\s*")
来源：http://pi.huanxung.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://so.hahajie.cn

Ruby: s.split(/\s*,\s*/)
来源：http://dk.hnjuh.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ew.jianghongdianzi.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://zm.shxzukj.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://qq.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://oq.panjiajie.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://sb.bookmarksfly.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://jx.newstarts.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://fi.szsharing.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://ly.bookmarksfly.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://km.wgjwhj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://kt.panjiajie.cn

[I07] 忽略大小写与多行模式
来源：http://ko.asd995.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://as.haigaiapp.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ou.jctech888.com.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://ah.yuntaijiaju.cn

TS:   /error/gim
来源：http://zk.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://tz.shxzukj.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://lc.521024.cn

Ruby: s.scan(/error/i)
来源：http://nl.jctech888.com.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://ql.haigaiapp.cn

[I08] 贪婪与非贪婪匹配
来源：http://hj.shxzskj.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://lk.jctech888.com.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://th.yuexingan06.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://qv.szsharing.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://ni.shxzukj.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://lo.shtwfgs.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://fq.bookmarksfly.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://xt.jctech888.com.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://th.yuexingan06.cn

================================================================================
来源：http://st.haigaiapp.cn

J. 日期与时间
来源：http://gl.shtwfgs.cn

================================================================================
来源：http://wi.szxytkj.cn

[J01] 获取当前时间
来源：http://zg.shxzskj.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://vf.szsharing.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://ou.jctech888.com.cn

JS:   new Date();  Date.now()
来源：http://fj.shxzukj.cn

TS:   new Date();  Date.now()
来源：http://ry.9csxet.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://lk.panjiajie.cn

Go:   time.Now()
来源：http://hn.szxytkj.cn

Ruby: Time.now
来源：http://ux.shxzukj.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://ci.haigaiapp.cn

[J02] 格式化输出
来源：http://bb.colortex.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bl.bjjhwx.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://fx.szxytkj.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://pg.szsharing.cn

TS:   d.toISOString()
来源：http://nl.huixinmuqiang.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://jo.wgjwhj.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://tv.huanxung.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://rm.huixinmuqiang.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://um.521024.cn

[J03] 字符串解析为日期
来源：http://vx.521024.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://ec.huanxung.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://pi.9csxet.cn

JS:   new Date("2024-01-02")
来源：http://yy.521024.cn

TS:   new Date("2024-01-02")
来源：http://ro.shxzskj.cn

Java: LocalDate.parse("2024-01-02")
来源：http://mw.szxytkj.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://sf.9csxet.cn

Ruby: Date.parse("2024-01-02")
来源：http://hq.huixinmuqiang.cn


<!-- 参考信息 -->