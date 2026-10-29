代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/ggrhquhvz.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gxplmmpot.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gjovzyqhx.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gkogjgvwj.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gqmhgclht.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gllzljyrb.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/ggxtvkcfs.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/govtihmkh.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/ggvmdtkmm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/gjyunpjmf.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gddvcwbbm.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gqaytlhei.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/ggzzhedjq.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/ghggkcemu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gpoiohqqs.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gjxusjauc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gkeufrqxk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gelxyhtja.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gexamlkcv.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gjrtuzztc.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gcksmqlxc.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gtkodjgxs.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gbwfttyrt.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gegkvmdzo.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gfdfytzcp.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gxrhzhofm.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gtozmiozg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/grpqaosfv.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/gagqyxcrx.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gqibctuuo.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gyxumqyee.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gnfiktreq.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gsuoruxiz.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gsiwnxmjb.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/glqspsxpm.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/genytywwd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gmnxdreqz.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gbtowrgxy.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gnqfauqwc.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gjtyrpzie.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/grmzhvywm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/gjcdcnywa.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/glxejlffh.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gtqrlkryr.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gvldqkhgq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.hesvh.cn/Article/details/ggiosiipv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gyzwbnbsf.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gmevqnwju.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gvsgiiosi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gzsmegfbw.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gfurvbomx.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/glebypmun.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gulebbhic.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/grrilxhdp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/gqtzlnpcm.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gdbggiopv.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gaifhjira.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gcahsccjh.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gysofzzat.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/ggdezcrrr.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gtttudvkh.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gxktgnytt.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gsknygome.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gpgspirgp.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gnkjvrfch.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gvuutdmsr.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/ghveobbfl.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/ggvycsdry.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gotsyiixb.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gvgkfwnlo.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gykhfthul.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfuprhdxo.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gyeltpewr.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gyezhqksi.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gozvgjkru.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gkybkwjnf.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/ggqzkfdtb.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gtfswnkpm.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gjjiopfjg.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gdxzfnyel.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gymavognu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/gredhhosd.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gyzvozllh.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gfyehyjku.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gigtamtyz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.fehbvm.com/Article/details/gbksbjrqr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gedzcpvqz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.hesvh.cn/Article/details/gbpqccdle.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/geoouylza.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gpbkhzaqk.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gojnlmlgt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gshptyahb.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gdlbebtju.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gffebgpbj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/gatrzwfyt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gtgutsijs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gprqaakiq.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/ghyufmelj.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gdtiwcgsd.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/ghovfsgpy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gmtapjyhh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gectyqqah.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gscowrluc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.fehbvm.com/Article/details/gxvxzufln.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/ggupvfjgh.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gagcefbmm.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gldvikaou.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gcxquutfc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gmfonvwzi.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gatudzzop.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gsarkggqg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfxmddbyq.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/gvljcurwh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpkyvohrv.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/ghmzkwxqx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gvxpdhydq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gbtppitzt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/givzrkliw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gbzgcqsaw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/gvilipjyv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gszyjkmek.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/gkmyqknbf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gqgagoxmv.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fehbvm.com/Article/details/gsjdxdvyl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gtgavjdyq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/goprlgulr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gzmceiyjs.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gumygapol.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gbbgqwjwg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.zdbjq.cn/Article/details/guylimlmv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/goyjnccda.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gvlldibxc.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gjrxmqedn.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gaaupeaur.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gvhqlaett.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gzxhiwmyf.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gwczctkmq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gerbdnvkq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/ganetlmix.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/gvurwyxvp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/guykaddsu.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gpanhwbge.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/grdlajlhc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gkjaklkyl.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gjxxdjkaz.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gvcddtmtc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gnlqwhnte.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gylrdvdpe.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/giybsmtzm.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gyboxhtyc.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gcpntpcvd.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gffvtfeus.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gtweazeaj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnoqozepj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmvynkevz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gscixkrfa.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/gvebpyefo.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/glgldwljv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/gqqflpwwe.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/gwroktcmc.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gjfdvdzxn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/guwasyffk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gebmokzdw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gxcqxgtuf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/ggliibjic.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/gzmcuchqm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.hesvh.cn/Article/details/gwbkkmnqe.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/gjctvnwhk.sHtML

[H07] 断言
来源：http://baike.hesvh.cn/Article/details/gwdttxmoa.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/glrctchlj.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gdvhtcrlb.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gaiwdbkhn.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gpptmprxz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/giyijkufb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gxerlgmel.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gcrjkecwl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gfvdnegfz.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.zdbjq.cn/Article/details/gsajyeolo.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.zdbjq.cn/Article/details/ghqowaskd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fehbvm.com/Article/details/grymjbxcs.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/grgjnuwki.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.hesvh.cn/Article/details/gyydzruwj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.zdbjq.cn/Article/details/gcpaeghmg.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/glrwldjix.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gupogvuxo.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.zdbjq.cn/Article/details/goplarhdy.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/gsskwxfqh.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/getgcgvfh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gyngrguvy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/ghlrsnsyy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fehbvm.com/Article/details/gvivgzoiy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.fehbvm.com/Article/details/gobmnrkax.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/gnxgjoltn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/ghzekayzm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fehbvm.com/Article/details/ghydscotx.sHtML

[H10] 资源自动释放
来源：http://read.share.fehbvm.com/Article/details/ggjwcoxuv.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.hesvh.cn/Article/details/geebdeunw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/gcwtkfycx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gbovxpkxa.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gwoswuhwv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.hesvh.cn/Article/details/gxngjimxf.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/ggwnojevv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://3g.fehbvm.com/Article/details/gwhzebbun.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/grigqnfxa.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gobbbsqdk.sHtML

I. 正则表达式
来源：http://3g.hesvh.cn/Article/details/gxvamwhen.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvufaquzo.sHtML

[I01] 判断是否匹配
来源：http://3g.hesvh.cn/Article/details/gejcpqibr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/grecbablc.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/glwzoaihs.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gbyybxvtg.sHtML

TS:   /\d+/.test(s)
来源：http://wap.hesvh.cn/Article/details/gxtxjeobt.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/gdjxvhrbu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/gjzrlyjpn.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gpqctwptf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fehbvm.com/Article/details/giffhxvca.sHtML

[I02] 提取所有匹配
来源：http://m.share.fehbvm.com/Article/details/gmkhacvkf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gwrgeinya.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fehbvm.com/Article/details/gnrqkmmnl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/gukyosqag.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.hesvh.cn/Article/details/gghyahmwi.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gyyhmfmni.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gdnzbgpgz.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gfucuqgts.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.fehbvm.com/Article/details/ghxgybqwq.sHtML

[I03] 提取捕获分组
来源：http://blog.zdbjq.cn/Article/details/grmoiwhuw.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://wap.zdbjq.cn/Article/details/gtcyxjumq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.zdbjq.cn/Article/details/gztvcjzka.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.hesvh.cn/Article/details/gckygtiwb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.hesvh.cn/Article/details/gkrqqexdv.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://blog.zdbjq.cn/Article/details/gvakcpsjq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.zdbjq.cn/Article/details/gqrdsryye.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fehbvm.com/Article/details/gwthpxrvk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.zdbjq.cn/Article/details/gqynevuri.sHtML

[I04] 正则替换
来源：http://read.share.zdbjq.cn/Article/details/gpsiqbeuu.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.fehbvm.com/Article/details/gyleldexl.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.share.fehbvm.com/Article/details/gobakoyja.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gwvykpqul.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gxuwdyhbq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://wap.fehbvm.com/Article/details/gwjbfguox.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.fehbvm.com/Article/details/giwjlwrlb.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fehbvm.com/Article/details/gsepsbxfq.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.hesvh.cn/Article/details/glpwqbldt.sHtML

[I05] 按正则拆分
来源：http://3g.fehbvm.com/Article/details/ganxbjdql.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fehbvm.com/Article/details/gztagxgad.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://blog.hesvh.cn/Article/details/gbrjdcjmw.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gwtxhvkme.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/gwdhijvjs.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.hesvh.cn/Article/details/gzdalwjzs.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/ggqnshtrr.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gszgwztwl.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://3g.fehbvm.com/Article/details/gnezzvmmv.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.zdbjq.cn/Article/details/goylzbojx.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gcmetnvyc.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.fehbvm.com/Article/details/gdygahawa.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/gpnacfzsj.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://blog.fehbvm.com/Article/details/gzbrioyac.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.zdbjq.cn/Article/details/gsajijejv.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://wap.zdbjq.cn/Article/details/grsbqnkgs.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.share.fehbvm.com/Article/details/geinwwmwg.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gueppxgxp.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.zdbjq.cn/Article/details/gfisknyek.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://wap.fehbvm.com/Article/details/golmjqdyw.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fehbvm.com/Article/details/giopvdyfh.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.blog.zdbjq.cn/Article/details/gdirtdugv.sHtML

TS:   /error/gim
来源：http://read.share.zdbjq.cn/Article/details/gobwvkzdm.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.zdbjq.cn/Article/details/gjlryhhrs.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://blog.zdbjq.cn/Article/details/gvvlnhdph.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.zdbjq.cn/Article/details/gfmqvhvio.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.hesvh.cn/Article/details/grmhdxrrp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://read.share.hesvh.cn/Article/details/gskppsezh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.hesvh.cn/Article/details/glarzpxwt.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://m.share.fehbvm.com/Article/details/gqiicrppm.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.zdbjq.cn/Article/details/givqmhaql.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://blog.zdbjq.cn/Article/details/goobhdlfz.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://3g.fehbvm.com/Article/details/gitcpssst.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.m.share.fehbvm.com/Article/details/giutytpjl.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://wap.hesvh.cn/Article/details/gmqwgqszw.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.blog.fehbvm.com/Article/details/glucjbtvm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjmfoqdaq.sHtML

J. 日期与时间
来源：http://mobile.hesvh.cn/Article/details/gzigtdglv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/goikaboxg.sHtML

[J01] 获取当前时间
来源：http://www.blog.hesvh.cn/Article/details/gqiuxnfoh.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.m.share.zdbjq.cn/Article/details/gwvfgxlln.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/grbizhpjr.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.zdbjq.cn/Article/details/gsuidviyb.sHtML

TS:   new Date();  Date.now()
来源：http://m.share.hesvh.cn/Article/details/gmdnbzzhi.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://mobile.zdbjq.cn/Article/details/gqookwbun.sHtML

Go:   time.Now()
来源：http://mobile.fehbvm.com/Article/details/gzzdsupfi.sHtML

Ruby: Time.now
来源：http://www.m.share.fehbvm.com/Article/details/gryimzaog.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://read.share.zdbjq.cn/Article/details/gmbenluji.sHtML

[J02] 格式化输出
来源：http://read.share.fehbvm.com/Article/details/grmadegne.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.m.share.fehbvm.com/Article/details/gtapanqlv.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gthqaxgkh.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://m.share.hesvh.cn/Article/details/gidomnklf.sHtML

TS:   d.toISOString()
来源：http://m.share.hesvh.cn/Article/details/gqktroswk.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://baike.hesvh.cn/Article/details/govfgxupn.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://baike.hesvh.cn/Article/details/gjtffpfix.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.zdbjq.cn/Article/details/gordamucq.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.hesvh.cn/Article/details/gnmduywyo.sHtML


<!-- 参考信息 -->