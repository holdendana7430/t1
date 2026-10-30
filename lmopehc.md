代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/guymehirs.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gddfgvmbr.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gbagrtkpu.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gxqdhdnob.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gzlrighvw.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gakoxemhv.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/ggdgxqrge.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gylgkskbx.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/glymsvvcn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/getqzavgd.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/ghenftdbi.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/grwpnlmhz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/ggrvydwcd.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gonienlqy.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gehcvvqvi.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gmhnrgnex.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/ggnjxhvcs.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gjlzsyokp.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gpqdfrhyp.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/ghmjpxrfx.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/gunmkpgqu.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gflrcjazc.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gzzuovjpz.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gldfetbow.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gaspmtcmq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/gszbvhnab.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gfsvjqnxa.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gprcgpbri.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/grmfumwjp.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/gdxpjavjf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gddmszadi.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gumnqyrui.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gpelqkmhn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gofmlhgvj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gdhlfucoa.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/grgpyivro.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gccwmbaap.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gnzbrcbqj.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gxtgminuv.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/grdvfsnzd.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/giujyxhyk.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gkichaxfn.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gzperdiqm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gbiwcfrlq.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gngyfwtoj.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/guujokupb.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gpnsihokk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gowcepagq.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gldiufnbk.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gxondevzj.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gsbluowxl.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gknqsqahi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gygrotwge.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gdufjbmgp.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/gafexaioj.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gkbtnxooi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gzfcdfyjd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.zdbjq.cn/Article/details/ghcxlomrd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/grxlkpuph.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gnrbtdrpn.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gnkgpwmhr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gonxiwbgx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gkupqmtkn.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gxpouhnwu.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gjmmwwubc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/ghknmxaoj.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gmgvesepx.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gztlwgwlq.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gewftoree.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gysvngmgj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gqroqnnxg.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gmbvvkhny.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/giuoqvzvf.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/ghosfakge.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/ghzmarfqd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gwufhxnca.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gtlhilrbg.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gbdxzawix.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gcfqkibjv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gazbauxit.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.fehbvm.com/Article/details/gixdlrkht.sHtML

C#:   public string Name { get; set; }
来源：http://3g.zdbjq.cn/Article/details/gjelkqifl.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gitqrjgoa.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gopaznrzi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gvdizalpy.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/guyaoijcg.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfxhwqlsb.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gfvxcevth.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gvyurtylu.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/glavdyjev.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gpbqqauxb.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gytipkmxw.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gygksakem.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gqdqtccvh.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gsxlhsagb.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gbbtvnbwo.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gsvjrtyqa.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/ggipnxnho.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gtrxzakvl.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gpvbztjuh.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gtfuactty.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gimnmbfbx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/ggbotdjcv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.fehbvm.com/Article/details/gyzzgxmwf.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/glhwynfmu.sHtML

Java: record User(String name, int age) {}
来源：http://wap.zdbjq.cn/Article/details/gyeivvuzp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gmzymxfae.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gjlerysoa.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/grjowtiin.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gegcwcajv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gsvzydqrb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/glisnlgzt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gffhljcbw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gbnroqosi.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gbwcrkpsz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gwktefbwa.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gabkowxcd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gplcrstdg.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/guktuimkb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gqyxogstd.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gjlknfgbw.sHtML

JS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/ghsnlpeer.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gxygechmd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.fehbvm.com/Article/details/geddgmdlr.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/gyfuqmwgl.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gqydadcgf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gegqcpjld.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gawdficgi.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gpmwpdxle.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjspdrypj.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/gdgcneprl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gnlbxqhzg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gdhjadopq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gysmscdvo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gkxjzpnqs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gdfmelgsa.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/ghyirjaot.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gaheumwbh.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gzekldyqx.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gncgomxqv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.fehbvm.com/Article/details/gltolqwgm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/ggefhglaq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gcpmaiems.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gpndgibre.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gyloswjqd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/godzkroaq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gvygqqvsh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gypcovwkf.sHtML

[H03] 主动抛出异常
来源：http://www.blog.fehbvm.com/Article/details/gprwtdjgg.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/gfndihwyg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gsysqsgsn.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gebrasdin.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gtncluigb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gakclbzsn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/gbokjsqtm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gzustgvtz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gmpzbxvis.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/gnzjnbcmh.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gdiboiyfd.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gzwlwydjh.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gvakquxtf.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gfsqmlfmk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gsmwvwwrm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/guxuzjzcv.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/gwarffjls.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/gnjbxzqss.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/gcfcwwenw.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/gusesdmme.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/ghtlmcovu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gqdfgehzv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkhkztsel.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gvdcvtfjd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/gpiyzidbv.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/gczuascqy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gcovhxlfg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/gvcoaqkss.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gokltxpvz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/gmojbepgi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gjencsmlz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gfatxxaau.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gwjlqrfxs.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fehbvm.com/Article/details/gumnggrrz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gwjwjrsyu.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gztgcfrwp.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gkanhqcwq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.hesvh.cn/Article/details/gzdiujijs.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gzqeojhaz.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/ginubfgci.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gkczxkeqb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gbzyvmbrk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gmhaazthj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gjfqfbrmo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gglpdefsj.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/giveojafk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fehbvm.com/Article/details/gyszrmbvc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/gpdpjrdol.sHtML

JS:   e.message;  e.stack
来源：http://baike.zdbjq.cn/Article/details/gxdbreeyc.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/ggysjgpnc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/gswkuckki.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gxhrvimlz.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fehbvm.com/Article/details/gmgmcudpr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.fehbvm.com/Article/details/gkyktsjzh.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.fehbvm.com/Article/details/gyemomofr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.zdbjq.cn/Article/details/gdckurywd.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gjqfjddte.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fehbvm.com/Article/details/golhlawse.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.zdbjq.cn/Article/details/gftqfuxvd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwlmrmokj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.fehbvm.com/Article/details/ghtbsjfmj.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fehbvm.com/Article/details/gefpulrmu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gxlynzmwu.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/gccgqlxyd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/gphdnsufo.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/gxheuhstt.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/guqptzveo.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gohqpspyc.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gabqdqlgs.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/gxihijhee.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.hesvh.cn/Article/details/gqkszrdrw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gmrfdhzfs.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glrpgzeua.sHtML

I. 正则表达式
来源：http://www.share.fehbvm.com/Article/details/gpkdiyilf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzpzboixx.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/gjyfifwas.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gapefegom.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gmtxrmere.sHtML

JS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gmairruxn.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gzuhdpzkx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.hesvh.cn/Article/details/gsvnxrdwv.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fehbvm.com/Article/details/gvaetgjas.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gogzjfhmy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gxntqxycl.sHtML

[I02] 提取所有匹配
来源：http://3g.hesvh.cn/Article/details/gttmpmpst.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gpxzepqco.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.zdbjq.cn/Article/details/gskisfeej.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/gktfcygpn.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.fehbvm.com/Article/details/gjkxpeomf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.hesvh.cn/Article/details/guoeddkao.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.hesvh.cn/Article/details/gtkagtwrv.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gqdsgjkgx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.zdbjq.cn/Article/details/gsyojnjbu.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/ghxznddyz.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.hesvh.cn/Article/details/gdfvvexnt.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fehbvm.com/Article/details/gzlyrzles.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.zdbjq.cn/Article/details/gqbhszqky.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.fehbvm.com/Article/details/gnieofoim.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.fehbvm.com/Article/details/gyfugulbp.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.zdbjq.cn/Article/details/gxmpgunnl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.zdbjq.cn/Article/details/ghmtejlst.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://read.share.fehbvm.com/Article/details/gpchnxwew.sHtML

[I04] 正则替换
来源：http://wap.zdbjq.cn/Article/details/gyxxlkakv.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.hesvh.cn/Article/details/gsgaaiuzu.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gjsluqlnt.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gmgmljmeb.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/glpevsqkq.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://mobile.fehbvm.com/Article/details/gxumaqvrn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.hesvh.cn/Article/details/gndahhogl.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.fehbvm.com/Article/details/gooxjucms.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gjlselapv.sHtML

[I05] 按正则拆分
来源：http://mobile.hesvh.cn/Article/details/gonersgcf.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://mobile.zdbjq.cn/Article/details/gasryjncp.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.hesvh.cn/Article/details/grtkoyrzi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/ghjqamfmc.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/gzclelnxg.sHtML

Java: s.split("\\s*,\\s*")
来源：http://blog.zdbjq.cn/Article/details/gpohqmjsw.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gkermrblf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.fehbvm.com/Article/details/gheslcxas.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.blog.hesvh.cn/Article/details/gygokkcwb.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://mobile.hesvh.cn/Article/details/gnwmdpgfg.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://3g.fehbvm.com/Article/details/gpikhjifr.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.share.zdbjq.cn/Article/details/goshogenn.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/ghwwcryuw.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.share.zdbjq.cn/Article/details/gfhoesdoc.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mobile.hesvh.cn/Article/details/gyqytczip.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.share.hesvh.cn/Article/details/gtjevlwzn.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://3g.hesvh.cn/Article/details/gislcjuat.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://blog.zdbjq.cn/Article/details/gugnxpbrm.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.blog.zdbjq.cn/Article/details/grqhpxnkg.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.blog.fehbvm.com/Article/details/gxepalivi.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://read.share.zdbjq.cn/Article/details/gdwfyskto.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.zdbjq.cn/Article/details/gfesqeiym.sHtML

TS:   /error/gim
来源：http://www.m.share.fehbvm.com/Article/details/gmskvaded.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.share.hesvh.cn/Article/details/grjmunszi.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.share.fehbvm.com/Article/details/gywenimpm.sHtML

Ruby: s.scan(/error/i)
来源：http://www.m.share.hesvh.cn/Article/details/gypydmnto.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.hesvh.cn/Article/details/gwwftvubd.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.m.share.zdbjq.cn/Article/details/ggvuusltg.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://mobile.hesvh.cn/Article/details/glemroxjx.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.blog.fehbvm.com/Article/details/gsxjcfzls.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://wap.hesvh.cn/Article/details/gpmhdqtkv.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://read.share.hesvh.cn/Article/details/gntukoggj.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.zdbjq.cn/Article/details/gcgqjjuwf.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://m.share.hesvh.cn/Article/details/govqdrzac.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://3g.hesvh.cn/Article/details/glvhgysgc.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://baike.hesvh.cn/Article/details/gfdxkqawl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gobbkxqib.sHtML

J. 日期与时间
来源：http://www.m.share.zdbjq.cn/Article/details/gtovocrkp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpeopbovn.sHtML

[J01] 获取当前时间
来源：http://baike.zdbjq.cn/Article/details/gjinthblu.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.share.zdbjq.cn/Article/details/ggjaocpfw.sHtML


<!-- 参考信息 -->