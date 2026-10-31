代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://nb.szxytkj.cn

[G07] 调用父类方法
来源：http://ll.bookmarksfly.cn

Py:   super().greet()
来源：http://jc.wgjwhj.cn

PHP:  parent::greet();
来源：http://ce.panjiajie.cn

JS:   super.greet();
来源：http://gi.gzmigu.cn

TS:   super.greet();
来源：http://pl.huixiangedu.cn

Java: super.greet();
来源：http://re.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hx.hnjuh.cn

Ruby: super
来源：http://cs.huixinmuqiang.cn

C#:   base.Greet();
来源：http://ts.shtwfgs.cn

[G08] 静态方法与属性
来源：http://tk.shxzukj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ec.huixinmuqiang.cn

PHP:  public static function f() {}
来源：http://jz.shtwfgs.cn

JS:   static f() {}
来源：http://bh.jianghongdianzi.cn

TS:   static f(): void {}
来源：http://ha.chemitech.net.cn

Java: static void f() {}
来源：http://hq.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://nh.nszjky.cn

Ruby: def self.f; end
来源：http://vb.hnjuh.cn

C#:   public static void F() {}
来源：http://vh.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://fm.shtwfgs.cn

Py:   from abc import ABC, abstractmethod
来源：http://mn.lnxyls.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wz.szxytkj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xd.chemitech.net.cn

TS:   interface Shape { area(): number; }
来源：http://vi.nicolike.cn

Java: interface Shape { double area(); }
来源：http://lp.huanxung.cn

Go:   type Shape interface { Area() float64 }
来源：http://ha.nszjky.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oz.hahajie.cn

C#:   interface IShape { double Area(); }
来源：http://ki.nicolike.cn

[G10] 访问控制
来源：http://qf.gzmigu.cn

Py:   约定 _protected / __private（不强制）
来源：http://ak.gzmigu.cn

PHP:  public / protected / private
来源：http://cb.haigaiapp.cn

JS:   #private 字段；其余公开
来源：http://hg.bjjhwx.cn

TS:   public / protected / private
来源：http://la.newstarts.cn

Java: public / protected / private / 默认包级
来源：http://co.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sl.yuntaijiaju.cn

Ruby: public / protected / private
来源：http://qj.yuexingan06.cn

C#:   public / protected / private / internal
来源：http://zg.hnjuh.cn

[G11] getter / setter
来源：http://al.521024.cn

Py:   @property 与 @x.setter
来源：http://br.9csxet.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://vf.szsharing.cn

JS:   get name() { return this._name; }
来源：http://hj.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://rq.nicolike.cn

Java: public String getName() { return name; }
来源：http://wz.szxytkj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://jd.wgjwhj.cn

Ruby: attr_accessor :name
来源：http://sd.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://of.asd995.cn

[G12] 对象转字符串
来源：http://jm.521024.cn

Py:   def __str__(self): return self.name
来源：http://cx.nicolike.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ll.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://rs.jctech888.com.cn

TS:   toString(): string { return this.name; }
来源：http://ml.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://mp.haigaiapp.cn

Go:   func (u User) String() string { return u.Name }
来源：http://yb.wgjwhj.cn

Ruby: def to_s; @name; end
来源：http://zk.lnxyls.cn

C#:   public override string ToString() => Name;
来源：http://vi.huixiangedu.cn

[G13] 判断对象类型
来源：http://nq.jianghongdianzi.cn

Py:   isinstance(u, User)
来源：http://cd.jctech888.com.cn

PHP:  $u instanceof User
来源：http://gd.huixinmuqiang.cn

JS:   u instanceof User
来源：http://de.shtwfgs.cn

TS:   u instanceof User
来源：http://dm.shxzukj.cn

Java: u instanceof User
来源：http://aq.bjjhwx.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ql.bjjhwx.cn

Ruby: u.is_a?(User)
来源：http://gh.9csxet.cn

C#:   u is User
来源：http://hm.muxihuayi.cn

[G14] 数据类 / record
来源：http://zp.521024.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://el.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://yj.nicolike.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ya.jctech888.com.cn

TS:   type User = { name: string; age: number };
来源：http://bs.huixiangedu.cn

Java: record User(String name, int age) {}
来源：http://su.521024.cn

Go:   type User struct { Name string; Age int }
来源：http://jm.hnjuh.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://su.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://yg.jianghongdianzi.cn

[G15] 枚举
来源：http://vk.hahajie.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kf.asd995.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://fq.chemitech.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://qu.hnjuh.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://et.yuntaijiaju.cn

Java: enum Color { RED, GREEN }
来源：http://ig.jctech888.com.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rc.muxihuayi.cn

Ruby: Color = %i[red green].freeze
来源：http://rb.gzmigu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vd.shxzskj.cn

[G16] 对象转数组 / 字典
来源：http://nj.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://im.shxzskj.cn

PHP:  get_object_vars($obj);
来源：http://sq.jctech888.com.cn

JS:   Object.entries(obj)
来源：http://sk.nicolike.cn

TS:   Object.entries(obj)
来源：http://hh.huanxung.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://sb.chemitech.net.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://st.huanxung.cn

Ruby: obj.instance_variables
来源：http://ck.colortex.cn

C#:   // 用反射或 System.Text.Json
来源：http://eg.haigaiapp.cn

================================================================================
来源：http://sj.jianghongdianzi.cn

H. 异常与错误处理
来源：http://ke.shtwfgs.cn

================================================================================
来源：http://bp.szxytkj.cn

[H01] try / catch 基础
来源：http://lp.szxytkj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zk.panjiajie.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://dn.huixiangedu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ps.bookmarksfly.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://td.szxytkj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://ro.chemitech.net.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ne.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://yz.szsharing.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://me.jianghongdianzi.cn

[H02] finally / ensure 收尾
来源：http://vi.panjiajie.cn

Py:   try: f()⏎finally: cleanup()
来源：http://aw.szxytkj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://un.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://pc.bjjhwx.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://px.huanxung.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ce.shxzukj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yh.jianghongdianzi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://tx.asd995.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ey.nszjky.cn

[H03] 主动抛出异常
来源：http://pd.9csxet.cn

Py:   raise ValueError("错误信息")
来源：http://my.yuntaijiaju.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://sl.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://qv.colortex.cn

TS:   throw new Error("错误信息");
来源：http://dz.nicolike.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qy.nicolike.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bu.bookmarksfly.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://db.chemitech.net.cn

C#:   throw new ArgumentException("错误信息");
来源：http://gb.muxihuayi.cn

[H04] 自定义异常类型
来源：http://of.newstarts.cn

Py:   class MyError(Exception): pass
来源：http://ay.huixinmuqiang.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yh.haigaiapp.cn

JS:   class MyError extends Error {}
来源：http://as.nicolike.cn

TS:   class MyError extends Error {}
来源：http://yv.gzmigu.cn

Java: class MyException extends RuntimeException {}
来源：http://dx.shxzukj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ch.huixinmuqiang.cn

Ruby: class MyError < StandardError; end
来源：http://sn.colortex.cn

C#:   class MyException : Exception {}
来源：http://nv.colortex.cn

[H05] 捕获特定类型
来源：http://ge.shxzskj.cn

Py:   except ValueError as e:
来源：http://dr.yuntaijiaju.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://xf.szsharing.cn

JS:   if (e instanceof TypeError) {}
来源：http://xu.szxytkj.cn

TS:   if (e instanceof TypeError) {}
来源：http://ok.asd995.cn

Java: catch (IOException | SQLException e) {}
来源：http://gm.yuntaijiaju.cn

Go:   errors.Is(err, os.ErrNotExist)
来源：http://ml.shxzukj.cn

Ruby: rescue ArgumentError => e
来源：http://bh.szxytkj.cn

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ee.lnxyls.cn

[H06] 可选值 / 空值安全访问
来源：http://oi.newstarts.cn

Py:   value = d.get("k") or default
来源：http://zn.nszjky.cn

PHP:  $v = $d["k"] ?? null;
来源：http://ns.chemitech.net.cn

JS:   obj?.a?.b;  d ?? default
来源：http://bn.huixiangedu.cn

TS:   obj?.a?.b;  d ?? default
来源：http://pc.9csxet.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://om.gzmigu.cn

Go:   if v, ok := m["k"]; ok { }
来源：http://fv.521024.cn

Ruby: d&.dig(:a, :b)
来源：http://zw.huixinmuqiang.cn

C#:   obj?.A?.B ?? default
来源：http://bz.muxihuayi.cn

[H07] 断言
来源：http://pu.panjiajie.cn

Py:   assert x > 0, "必须为正"
来源：http://jd.jctech888.com.cn

PHP:  assert($x > 0);
来源：http://of.hahajie.cn

JS:   console.assert(x > 0);
来源：http://ge.shtwfgs.cn

TS:   console.assert(x > 0);
来源：http://xv.shxzukj.cn

Java: assert x > 0 : "必须为正";
来源：http://ku.9csxet.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://ue.lnxyls.cn

Ruby: raise "必须为正" unless x > 0
来源：http://gr.lnxyls.cn

C#:   Debug.Assert(x > 0);
来源：http://bu.huixiangedu.cn

[H08] 获取错误信息与堆栈
来源：http://ik.jianghongdianzi.cn

Py:   str(e);  traceback.format_exc()
来源：http://yd.bjjhwx.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://yr.nicolike.cn

JS:   e.message;  e.stack
来源：http://of.huanxung.cn

TS:   e instanceof Error ? e.message : String(e)
来源：http://or.shtwfgs.cn

Java: e.getMessage();  e.printStackTrace()
来源：http://bz.panjiajie.cn

Go:   err.Error()
来源：http://lw.chemitech.net.cn

Ruby: e.message;  e.backtrace
来源：http://vq.shtwfgs.cn

C#:   e.Message;  e.StackTrace
来源：http://xs.panjiajie.cn

[H09] 带错误码的异常
来源：http://zc.hahajie.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wb.yuntaijiaju.cn

PHP:  throw new RuntimeException("fail", 500);
来源：http://sc.yuexingan06.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://od.lnxyls.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://qe.panjiajie.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://xs.gzmigu.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://fc.shxzukj.cn

Ruby: raise MyError.new("fail", 500)
来源：http://ez.panjiajie.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://vv.yuexingan06.cn

[H10] 资源自动释放
来源：http://ow.chemitech.net.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://rl.huixiangedu.cn

PHP:  // 无 with：在 finally 里 fclose()
来源：http://zl.gzmigu.cn

JS:   // 无 with：在 finally 里关闭句柄
来源：http://na.szxytkj.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://qi.jianghongdianzi.cn

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://to.shxzskj.cn

Go:   defer f.Close()
来源：http://am.jctech888.com.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://qb.nszjky.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://cp.bjjhwx.cn

================================================================================
来源：http://ks.nicolike.cn

I. 正则表达式
来源：http://cy.shxzukj.cn

================================================================================
来源：http://jv.bookmarksfly.cn

[I01] 判断是否匹配
来源：http://vq.panjiajie.cn

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://uj.gzmigu.cn

PHP:  preg_match('/\d+/', $s);
来源：http://tg.nszjky.cn

JS:   /\d+/.test(s)
来源：http://mj.shxzukj.cn

TS:   /\d+/.test(s)
来源：http://ap.yuexingan06.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://me.huixinmuqiang.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hh.huanxung.cn

Ruby: s.match?(/\d+/)
来源：http://fk.gzmigu.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://gb.szxytkj.cn

[I02] 提取所有匹配
来源：http://rv.9csxet.cn

Py:   re.findall(r"\d+", s)
来源：http://ws.bjjhwx.cn

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://uz.newstarts.cn

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://ig.lnxyls.cn

TS:   s.match(/\d+/g)
来源：http://wv.huanxung.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://bv.bookmarksfly.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://eg.szsharing.cn

Ruby: s.scan(/\d+/)
来源：http://tw.szsharing.cn

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://dd.chemitech.net.cn

[I03] 提取捕获分组
来源：http://qg.shxzukj.cn

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://cb.muxihuayi.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wj.shxzukj.cn

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://ia.huixiangedu.cn

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hb.shxzukj.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://jm.huixinmuqiang.cn

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://my.chemitech.net.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://jz.huixinmuqiang.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://zb.yuexingan06.cn

[I04] 正则替换
来源：http://kp.bookmarksfly.cn

Py:   re.sub(r"\d+", "#", s)
来源：http://vh.hnjuh.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wn.nszjky.cn

JS:   s.replace(/\d+/g, "#")
来源：http://vk.asd995.cn

TS:   s.replace(/\d+/g, "#")
来源：http://on.huixiangedu.cn

Java: s.replaceAll("\\d+", "#")
来源：http://pq.nicolike.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://io.haigaiapp.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://hv.9csxet.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://av.shxzukj.cn

[I05] 按正则拆分
来源：http://bs.shxzskj.cn

Py:   re.split(r"\s*,\s*", s)
来源：http://dx.9csxet.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://yz.hahajie.cn

JS:   s.split(/\s*,\s*/)
来源：http://lb.shxzskj.cn

TS:   s.split(/\s*,\s*/)
来源：http://ou.hnjuh.cn

Java: s.split("\\s*,\\s*")
来源：http://fr.asd995.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://us.bookmarksfly.cn

Ruby: s.split(/\s*,\s*/)
来源：http://ej.nszjky.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://cp.huixiangedu.cn

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://sc.shtwfgs.cn

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://ym.lnxyls.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://km.muxihuayi.cn

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://dt.muxihuayi.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://rg.yuntaijiaju.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://xs.shxzskj.cn

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qq.huanxung.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://vz.szxytkj.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://cw.asd995.cn

[I07] 忽略大小写与多行模式
来源：http://yh.huixinmuqiang.cn

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://eu.jianghongdianzi.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://jc.shtwfgs.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hu.nicolike.cn

TS:   /error/gim
来源：http://rf.jctech888.com.cn

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://jm.huixinmuqiang.cn

Go:   regexp.MustCompile(`(?im)error`)
来源：http://re.jianghongdianzi.cn

Ruby: s.scan(/error/i)
来源：http://qm.hahajie.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lz.hahajie.cn

[I08] 贪婪与非贪婪匹配
来源：http://ez.huixinmuqiang.cn

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://sd.9csxet.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://qa.yuntaijiaju.cn

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://np.asd995.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://je.huanxung.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://zn.panjiajie.cn

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://zc.gzmigu.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hi.lnxyls.cn

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://cu.bookmarksfly.cn

================================================================================
来源：http://mj.huixinmuqiang.cn

J. 日期与时间
来源：http://dh.huixinmuqiang.cn

================================================================================
来源：http://au.panjiajie.cn

[J01] 获取当前时间
来源：http://fy.hahajie.cn

Py:   datetime.now();  datetime.now(UTC)
来源：http://ok.newstarts.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://es.huixinmuqiang.cn

JS:   new Date();  Date.now()
来源：http://ax.jctech888.com.cn

TS:   new Date();  Date.now()
来源：http://lz.wgjwhj.cn

Java: LocalDateTime.now();  Instant.now()
来源：http://pv.huixiangedu.cn

Go:   time.Now()
来源：http://qj.jctech888.com.cn

Ruby: Time.now
来源：http://yc.9csxet.cn

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://kn.huixiangedu.cn

[J02] 格式化输出
来源：http://ap.bjjhwx.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ro.9csxet.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://xk.muxihuayi.cn

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://ku.wgjwhj.cn

TS:   d.toISOString()
来源：http://dp.muxihuayi.cn

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://ns.colortex.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://xs.shxzukj.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://ey.bookmarksfly.cn

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://si.lnxyls.cn

[J03] 字符串解析为日期
来源：http://su.huixinmuqiang.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://wy.shxzskj.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://rs.nicolike.cn

JS:   new Date("2024-01-02")
来源：http://vn.huixinmuqiang.cn

TS:   new Date("2024-01-02")
来源：http://hv.gzmigu.cn

Java: LocalDate.parse("2024-01-02")
来源：http://bx.nszjky.cn

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://fv.lnxyls.cn

Ruby: Date.parse("2024-01-02")
来源：http://fx.panjiajie.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://il.hnjuh.cn

[J04] 时间戳与日期互转
来源：http://nn.chemitech.net.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://vd.shxzskj.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://sa.huixiangedu.cn

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://he.colortex.cn

TS:   Math.floor(Date.now() / 1000)
来源：http://ag.hnjuh.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://bn.jctech888.com.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://wp.yuexingan06.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://ny.huixiangedu.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://yp.shtwfgs.cn

[J05] 时间加减（加 7 天）
来源：http://vf.shxzskj.cn

Py:   now + timedelta(days=7)
来源：http://kr.wgjwhj.cn


<!-- 参考信息 -->