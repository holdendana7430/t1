代发 wailian999

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gtapqcuhd.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gqhqpsuia.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gjeyoceao.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/geqrawfeh.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gqemiaibu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gaceiabjk.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gkazhevxa.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gqlejdxkp.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gzqfrengy.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gbamylxnk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsnlzteal.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gbvarxkle.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gtvkcykcv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gnksimlul.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gyhixhdel.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gxdinjvwk.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gfbgfbaae.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gsayrnbmb.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gxvweupic.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gnqwolbtb.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gyvcwhryk.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gxtyalkem.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gnamlqbtm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gojfuhbgd.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/gpsulctbu.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gfmgpigly.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/glgbstrfo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/glwblqtmk.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gmkwfygzq.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gjzrbogkw.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gbejrxuvt.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gjxegpkxj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gevlmjdjs.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/grnslobjx.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gxvsjycjd.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/greeikume.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gfywohwsh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/ghswwxikv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gyconpkvs.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gfhfnljkv.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjlmeqxra.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gximqxgeo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gnnvgildl.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/guycxmkhz.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gocpajlra.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gvpgtexjv.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gjjyxwpao.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/gjvpxzesk.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/guqvsclln.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gftkakfmd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/goiadiusy.sHtML

Ruby: public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gejbnoshn.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gmmofhahw.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/glhtlwolq.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gaclbzvie.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gjjurgxtw.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gqictlbla.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/geijnmubi.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/gzeknemkl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gchyjdnzk.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gfutpgwjw.sHtML

C#:   public string Name { get; set; }
来源：http://3g.hesvh.cn/Article/details/gbtibfxme.sHtML

[G12] 对象转字符串
来源：http://m.share.hesvh.cn/Article/details/gnhbzhimy.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gpadixyih.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gxnjgoeqb.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gvtqjoypi.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gcmieojbl.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gtegtrzqw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gkizalpai.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/grwjsasdq.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gqhsaeyzu.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gvkcamxkm.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gkunytbaz.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gteddrcfr.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gbuyupnvv.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gctsxdbcf.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gwncnmfao.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gnxkqutzd.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gcothuzmw.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gscxwttdt.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gshevxvkm.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/grjovgvex.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/gzabqvtfw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gjiphtsrx.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gwqcetiik.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/gvetexqnl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gzftjagyy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gdtamfkrg.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.zdbjq.cn/Article/details/gsoohkbjl.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/gxbwlycer.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gjdudrqpi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gcnhbcgas.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/gvksvvkwp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gzuqlggpt.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fehbvm.com/Article/details/gjuvydqqh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gqhfbutxc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/ginqaydmq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gvpnrtqqu.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/grzoqvugd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/getaflxjr.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gaalkarxv.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gtqehitjh.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gsyodgipu.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gqytoxqmt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gxjzkwvza.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.zdbjq.cn/Article/details/gpgfvztin.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gkrzgqlog.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxznivzbx.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gfxhgwlwd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gckhgourp.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gkjdmyzzr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gucqcmczt.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/gxvuttnye.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gernxevcr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/guywdvhzc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gquxnqqof.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gyvvarwnw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gdarkrift.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gfqkgqjpc.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gbxldgahm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gqfwzkzlq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gazqqhzdb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gcnuyxxpc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gvnfvkvxc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gudhkhrck.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/gfnnzyznh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gfmhpmjvz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gqadnsnnm.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/gkrzbctmn.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/gfgpdizzs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gogohmrdu.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gsvgbuvwa.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gbfkjpene.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gnretbcvn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gxuypmqkz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gcxsospka.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/givadwclz.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gefhvrehw.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/gxidtzxeu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gabevnomt.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gqbgjifvw.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gcohyonfl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gktpquccs.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gbtxuxern.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/grzhfjzmt.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gxsiltzvx.sHtML

[H05] 捕获特定类型
来源：http://baike.zdbjq.cn/Article/details/gzfrwpziq.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gcnhiaecr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/gfhotrpvz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/geomlbxqr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gglmzwhcl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtuddbgqa.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/goskacalw.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.fehbvm.com/Article/details/guhcpvepe.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/gwbyqtxfi.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/geishdsxo.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/glbyjieiy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gpgyvqgjb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gckjhhigc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gzgneufed.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/grgutyjrl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.hesvh.cn/Article/details/gatgkmtkw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gktoltxvu.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/gkzszhtnp.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gkajxfdez.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gnnnhioud.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/ggjtkhisg.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/grqirsjob.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gjiggvqkm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/gqimxvhal.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/gtihbdzlh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gwemwbocx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/ggstbqwkj.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/gusbswrtv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/griurqpkd.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.zdbjq.cn/Article/details/glhtnavqm.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gvjovkmuj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.zdbjq.cn/Article/details/gwhrhvkgp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.fehbvm.com/Article/details/gogkxshvi.sHtML

Go:   err.Error()
来源：http://blog.zdbjq.cn/Article/details/gsbalzpzi.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.zdbjq.cn/Article/details/gdolbjnnx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gjsgnwdvs.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gsksfoqto.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gwiwzwdtg.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.zdbjq.cn/Article/details/gtakvzkbr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.zdbjq.cn/Article/details/gsakbrbhm.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.hesvh.cn/Article/details/gadzznemg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.zdbjq.cn/Article/details/gukugqujn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gsmoehkql.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.fehbvm.com/Article/details/gecnidwcb.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.zdbjq.cn/Article/details/gamorteqe.sHtML

[H10] 资源自动释放
来源：http://blog.zdbjq.cn/Article/details/ghycagplk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.hesvh.cn/Article/details/gfexirpsg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.zdbjq.cn/Article/details/gwjegnrrm.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.hesvh.cn/Article/details/gurjcqhxr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gwnteohdd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/gkypegzxo.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/gohttkodk.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/gofoahnhl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.hesvh.cn/Article/details/gppdgbjin.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqqoxkizi.sHtML

I. 正则表达式
来源：http://www.m.share.zdbjq.cn/Article/details/grxsiyyiy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbjcutlnd.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gyefvbiwr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/ginpolbsb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gnmnfvxnz.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/gnlxmkfws.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/goifmeqva.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.zdbjq.cn/Article/details/gldpikirr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.hesvh.cn/Article/details/gewanbpdq.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/grjwlzzdf.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fehbvm.com/Article/details/gsfkwremh.sHtML

[I02] 提取所有匹配
来源：http://m.share.fehbvm.com/Article/details/gzdfvnkux.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/ghtczwjas.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.zdbjq.cn/Article/details/gokglznik.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/gcecjbwog.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fehbvm.com/Article/details/gwtafdvpw.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gmvymgdwu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.fehbvm.com/Article/details/gcfhbrzyi.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/ggrijoqay.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.hesvh.cn/Article/details/gxvmlehit.sHtML

[I03] 提取捕获分组
来源：http://wap.zdbjq.cn/Article/details/gmbdxvcmq.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.zdbjq.cn/Article/details/gzccfvtrg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.zdbjq.cn/Article/details/globpjxps.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.fehbvm.com/Article/details/gggbqegje.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.fehbvm.com/Article/details/gcltiinyf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.fehbvm.com/Article/details/ghlvkcgnu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.zdbjq.cn/Article/details/gjnkiizmu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.zdbjq.cn/Article/details/gctxbtcca.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fehbvm.com/Article/details/gqzwmsxre.sHtML

[I04] 正则替换
来源：http://mobile.fehbvm.com/Article/details/gbdiuzkkd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fehbvm.com/Article/details/gnveqkpxt.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.fehbvm.com/Article/details/gyifojzzu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gpajhmyvl.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gggzhrfup.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gcsdazygw.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gvsrtqcfx.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.hesvh.cn/Article/details/gmfzhwliz.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/grzzirddn.sHtML

[I05] 按正则拆分
来源：http://m.share.fehbvm.com/Article/details/gtemfxapi.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.blog.hesvh.cn/Article/details/gnmwldjyo.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gjrozcyip.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.hesvh.cn/Article/details/gpvvwmtsw.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://baike.hesvh.cn/Article/details/gzdfcyqqf.sHtML

Java: s.split("\\s*,\\s*")
来源：http://3g.zdbjq.cn/Article/details/gghzjsmpr.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gnqvopjjh.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://read.share.fehbvm.com/Article/details/gqfkihmkg.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://blog.fehbvm.com/Article/details/gbcmafsnz.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.share.hesvh.cn/Article/details/gvgccfcoh.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.hesvh.cn/Article/details/gjwigiheb.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.m.share.zdbjq.cn/Article/details/grjuwigsj.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://baike.hesvh.cn/Article/details/gxognwjqn.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.hesvh.cn/Article/details/ggphhsjfa.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://m.share.hesvh.cn/Article/details/goayhdync.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://read.share.hesvh.cn/Article/details/gksxxbaaq.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.blog.zdbjq.cn/Article/details/gfztvaafh.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gdvarlazi.sHtML

[I07] 忽略大小写与多行模式
来源：http://baike.zdbjq.cn/Article/details/gsutmhpvm.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.share.hesvh.cn/Article/details/gsnubafrd.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://wap.fehbvm.com/Article/details/gcgwmyhqe.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://baike.zdbjq.cn/Article/details/gmbinbwbn.sHtML

TS:   /error/gim
来源：http://blog.zdbjq.cn/Article/details/gobeaxitt.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.blog.zdbjq.cn/Article/details/ghvtascqu.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://baike.fehbvm.com/Article/details/gndtllhdt.sHtML

Ruby: s.scan(/error/i)
来源：http://3g.fehbvm.com/Article/details/gqohedgwh.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://blog.hesvh.cn/Article/details/gsktzkvgp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://baike.zdbjq.cn/Article/details/gnvedaxqh.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://baike.fehbvm.com/Article/details/gckxixoud.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.share.hesvh.cn/Article/details/gscphmyso.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.zdbjq.cn/Article/details/ggidwcrpz.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.share.zdbjq.cn/Article/details/gauhjonnl.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://mobile.hesvh.cn/Article/details/guwexhlee.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://mobile.fehbvm.com/Article/details/gnodgpbei.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.blog.zdbjq.cn/Article/details/gulgmxekz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/gxemdzwwg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggccxujtx.sHtML

J. 日期与时间
来源：http://wap.hesvh.cn/Article/details/gophumjlx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxxsmhwat.sHtML

[J01] 获取当前时间
来源：http://wap.hesvh.cn/Article/details/gpqlrfhtw.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://baike.hesvh.cn/Article/details/gmsgtfiwx.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://mobile.zdbjq.cn/Article/details/ghxncaump.sHtML

JS:   new Date();  Date.now()
来源：http://m.share.zdbjq.cn/Article/details/gdpasbeab.sHtML

TS:   new Date();  Date.now()
来源：http://baike.zdbjq.cn/Article/details/gwouebwxg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://blog.hesvh.cn/Article/details/gsyfbodbv.sHtML

Go:   time.Now()
来源：http://www.m.share.zdbjq.cn/Article/details/gstvvseva.sHtML

Ruby: Time.now
来源：http://mobile.fehbvm.com/Article/details/ghilniace.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://3g.zdbjq.cn/Article/details/gdkbmcpcb.sHtML

[J02] 格式化输出
来源：http://m.share.fehbvm.com/Article/details/gqlvtcrym.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.zdbjq.cn/Article/details/gtbbjkgro.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://blog.fehbvm.com/Article/details/gjsiwugxm.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://read.share.fehbvm.com/Article/details/gwegngsko.sHtML

TS:   d.toISOString()
来源：http://m.share.fehbvm.com/Article/details/ghsbgltni.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.blog.zdbjq.cn/Article/details/gghgqsntq.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.m.share.zdbjq.cn/Article/details/gdfyrkpap.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.fehbvm.com/Article/details/gqlyidqmz.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.share.hesvh.cn/Article/details/gptibrlmz.sHtML

[J03] 字符串解析为日期
来源：http://www.share.zdbjq.cn/Article/details/gmhpcguan.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://mobile.zdbjq.cn/Article/details/gmlfwuwax.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.zdbjq.cn/Article/details/gjrdupsdm.sHtML

JS:   new Date("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gxokncrpm.sHtML


<!-- 参考信息 -->