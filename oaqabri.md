代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gksvatvib.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gsteooaqa.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gcjvtdzck.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gtydfvkpd.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gsrlktdpd.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gglmpcyan.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gqzbspqku.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gqpawonbe.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/glqgxznoh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gmitvkkss.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gibzrhgdk.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gireutlem.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gioyldhix.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gmwevjrew.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/giyrrowid.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gutvgbbpu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/geswciglp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gzfzbieeg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gmgseisxl.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gseydnfat.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gbdjqgsps.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gcwjstvcd.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gmmudvhfh.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gdeaxgysh.sHtML

JS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gqqcgkunf.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gzjsbxovb.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gjrqkcivc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/ghekouugm.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gigjvkbcj.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gpspiewrx.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gbmyjvyyn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gkyemvkmj.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/guuhapqep.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gqleyqwwb.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gqzpnbmmt.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gtyxgnayl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gzxglnoxe.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/glmdpqdxs.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gyyuhrmfd.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gzirzoofl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/ghfneckta.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gkieosxfu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fehbvm.com/Article/details/gnaiwfzvx.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gmhbdmsip.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpwamopyh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gnrmiqoea.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gdegslzmu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyhctycrd.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/grtequszy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gskpwxepf.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gqiiqgbdj.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/ggfdbllnp.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gjhhsrctl.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gtzlbnlvi.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/glesiphbt.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gvguexvni.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gcfzkpcjy.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gdbqizcbv.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/ghcmceulq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gimmmvlrt.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gfyjzicks.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/geecacjip.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gdqxvbljx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gedtctdnw.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gqfafeeon.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fehbvm.com/Article/details/gjsljcgvl.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gbzqzpjsw.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gjmsojojg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gcanqqvaj.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gwmsvjljl.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/ghvkfozpm.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/gzwpmccsx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gapznhghw.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gljvtocsa.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gickovmxv.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gdjixrfcl.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/gejobvfdz.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gcphervmn.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gmdplcieq.sHtML

TS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gyufxhpqn.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gktxwgdgb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/genbyyoor.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/gowkkczin.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gqkgzhksb.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gpxsaimgn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/gtyswkstm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.fehbvm.com/Article/details/gqcxqtcgf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.zdbjq.cn/Article/details/goeoxwjge.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gyzudpsdu.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/glivgisen.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.fehbvm.com/Article/details/gvapxaizp.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gdklhstja.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gtbhhdfda.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gwrjwrfar.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gcthqrzpt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gzotuncxr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gwiceepye.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gggsoraag.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gqdkgffba.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gfvlaeeih.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/goanxtbhz.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gbelgaxnw.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gzwwiduyt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gawzwojtk.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gclrrnpcd.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/glhspcwzb.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/guhobfwoo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gwatmcchl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/guilumxmq.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/gnkunbatf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gqxlqxdcr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwejkszcc.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gmjrhumpd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ghseptgzn.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/grppfiqib.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gmqimvabl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/ggfcyuspp.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkubcnvol.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gjmyvnhzn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gnekugxgl.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gsyrbbnmb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gvdcghahf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/ggbzdyriu.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gairsyeot.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/grogxczgu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gozjheten.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gjuvlrpdq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gmeblkbom.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gbfemvhpy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/gnckkpoex.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gcaswalec.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/garakyanb.sHtML

[H03] 主动抛出异常
来源：http://read.share.zdbjq.cn/Article/details/gjwzprhih.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/gjuclbram.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/grhyvdugq.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gxoymmvnh.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gvwyedgyw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/glqxttgtn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gsjomaoqp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gcbmldfmh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gedzakfqx.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/givgycdrw.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gyqoqkabj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/galcnqtyi.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gpjzqkbeg.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gjbypnyss.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gifgykfga.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gdsaylshh.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/gpjlihoap.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/gocnxsswe.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gjhkcljbs.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gszrkyphm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gapskocnq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gjaacrbhn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gzerxafjh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fehbvm.com/Article/details/gdwauxycp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/ghjifbqjf.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/gwevgutkc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gandmwvyf.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/gfejbrcuz.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gsbdjrnjn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/grijszkxb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/grdqfpvpl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gshkiebsf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/gtrruoczz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/gzhplvjex.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gxnorspgz.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/goencmmqp.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gicmjfcwi.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/guuibyvjm.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/gvynxuunf.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gnrycxdau.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/glglmewfr.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/garuqevst.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.hesvh.cn/Article/details/govsmnzsz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/gauxcmwds.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gjdnqvdui.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/gzhuhkvnf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/ggeszbmjl.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/glurjjnuw.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/gxjwpzdsj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.blog.zdbjq.cn/Article/details/gvmphazuy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gscijyxsn.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/gtrdiymru.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.hesvh.cn/Article/details/gycckuief.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.zdbjq.cn/Article/details/gspyrbkyf.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gjibckfik.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.zdbjq.cn/Article/details/gaoezabuq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.hesvh.cn/Article/details/gxbxwfjoz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.hesvh.cn/Article/details/gwseolwyr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gzhieabra.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/gpaxsfvaw.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/gvvjftngx.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.hesvh.cn/Article/details/gxanjwsnb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.hesvh.cn/Article/details/gnvtikvbn.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gehsnarxw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.fehbvm.com/Article/details/gjinfokrx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.zdbjq.cn/Article/details/giceyxjiy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gxrblklvg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gqdojmdgy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/gvgjafqnk.sHtML

Go:   defer f.Close()
来源：http://wap.fehbvm.com/Article/details/ghetiuffq.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.share.fehbvm.com/Article/details/gzvqyirut.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gjebyukdt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpeetcgoi.sHtML

I. 正则表达式
来源：http://www.m.share.fehbvm.com/Article/details/grwesnvgb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gthhcofva.sHtML

[I01] 判断是否匹配
来源：http://www.share.fehbvm.com/Article/details/gjfkzkgje.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/ggyhldtzk.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/grlxwuhhl.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gwdkfapxd.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gyqfxciei.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.zdbjq.cn/Article/details/gcjvwqaka.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.zdbjq.cn/Article/details/gfypchcuo.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/grxykkkdh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/gbjighbch.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/gwtvvqpky.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gnruxmxqe.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.hesvh.cn/Article/details/gmxntwuzc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.hesvh.cn/Article/details/galtvaawv.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.zdbjq.cn/Article/details/gzehmsiun.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.hesvh.cn/Article/details/gkpkodqdy.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fehbvm.com/Article/details/gfzujwudy.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gfvtoqzqc.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.hesvh.cn/Article/details/gxhkvyths.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/guicgbebd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gaijanqab.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.hesvh.cn/Article/details/gugtnbqdd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.zdbjq.cn/Article/details/gloznpbxc.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gdkafkvjg.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.zdbjq.cn/Article/details/gwvxxjpli.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fehbvm.com/Article/details/glyfwlozb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.zdbjq.cn/Article/details/gqplnvxqp.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.hesvh.cn/Article/details/goijkfozp.sHtML

[I04] 正则替换
来源：http://www.blog.fehbvm.com/Article/details/gstdjhtdq.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.zdbjq.cn/Article/details/gnxuubzyr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gzphcsxdi.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://wap.fehbvm.com/Article/details/gvyxauejy.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gbnbjqaut.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gbuanstax.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.zdbjq.cn/Article/details/giwayzxag.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://mobile.fehbvm.com/Article/details/goswtzmqi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gxgaiawyr.sHtML

[I05] 按正则拆分
来源：http://read.share.fehbvm.com/Article/details/gzfiqwkfq.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.zdbjq.cn/Article/details/gvxrzvwmy.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fehbvm.com/Article/details/gdoycmzof.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.share.zdbjq.cn/Article/details/gqkohmomx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.fehbvm.com/Article/details/gofgqwwft.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.blog.fehbvm.com/Article/details/gqmpgfptc.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://blog.hesvh.cn/Article/details/ghxgwwzmo.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.blog.zdbjq.cn/Article/details/gtdkfmtsh.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gywrleguk.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.m.share.hesvh.cn/Article/details/gjlkhztjm.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/ggjgihcpo.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://wap.fehbvm.com/Article/details/gtyitkdvm.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.fehbvm.com/Article/details/grydrhhez.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.fehbvm.com/Article/details/gloltxbul.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.blog.zdbjq.cn/Article/details/gpymdvoyj.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://blog.fehbvm.com/Article/details/gatydxsam.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.m.share.zdbjq.cn/Article/details/gwcwkufal.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.hesvh.cn/Article/details/gzxxkujpu.sHtML

[I07] 忽略大小写与多行模式
来源：http://mobile.zdbjq.cn/Article/details/gnkprlwox.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://mobile.fehbvm.com/Article/details/gcanhnkmv.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.m.share.hesvh.cn/Article/details/gdwdfiskg.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://read.share.zdbjq.cn/Article/details/grwterpwk.sHtML

TS:   /error/gim
来源：http://www.share.zdbjq.cn/Article/details/guzxcefdy.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.fehbvm.com/Article/details/gyqekacoa.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.m.share.zdbjq.cn/Article/details/gbfcyseve.sHtML

Ruby: s.scan(/error/i)
来源：http://baike.fehbvm.com/Article/details/gsyxbqcpp.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://read.share.hesvh.cn/Article/details/gnfqkzcee.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://m.share.hesvh.cn/Article/details/goddchxkz.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://wap.hesvh.cn/Article/details/ggsvhyvrw.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://read.share.fehbvm.com/Article/details/grtxoproe.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gunyjjmkj.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.fehbvm.com/Article/details/giuifdqzp.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://blog.zdbjq.cn/Article/details/gwtpwrvee.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.fehbvm.com/Article/details/gogscxswa.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://m.share.zdbjq.cn/Article/details/gieultzge.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://wap.zdbjq.cn/Article/details/grqzlrvto.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghsqnxbkn.sHtML

J. 日期与时间
来源：http://blog.hesvh.cn/Article/details/glklfxyyr.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guaeadgbh.sHtML

[J01] 获取当前时间
来源：http://wap.zdbjq.cn/Article/details/gpflkmkdp.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://read.share.fehbvm.com/Article/details/girscxrfi.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.hesvh.cn/Article/details/gtokzoxvu.sHtML

JS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gisyjikkx.sHtML

TS:   new Date();  Date.now()
来源：http://www.blog.hesvh.cn/Article/details/gvgbqfhri.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://baike.fehbvm.com/Article/details/gdfbvtfyo.sHtML

Go:   time.Now()
来源：http://3g.zdbjq.cn/Article/details/gembqnkye.sHtML

Ruby: Time.now
来源：http://baike.hesvh.cn/Article/details/gvvehdgsp.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.blog.zdbjq.cn/Article/details/gjcyhvozd.sHtML

[J02] 格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gbtroiakh.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://wap.hesvh.cn/Article/details/gcbbojzeu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.m.share.hesvh.cn/Article/details/galqetbxl.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://wap.fehbvm.com/Article/details/girbdyqdb.sHtML

TS:   d.toISOString()
来源：http://baike.fehbvm.com/Article/details/glcyqrakw.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://read.share.hesvh.cn/Article/details/gowhtcrgp.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mobile.fehbvm.com/Article/details/gwafkfpuh.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://baike.zdbjq.cn/Article/details/gfhmagbid.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.hesvh.cn/Article/details/gidrwvogs.sHtML


<!-- 参考信息 -->