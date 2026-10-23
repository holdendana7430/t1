代发 wailian999

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mjezkequ.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wsjymkai.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3hxudrune.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ayxgpkxk.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3oekxybok.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3jmfofylo.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3kfhexvhm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3zvbsanaj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlujrnlx.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pfdcddoy.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tdymgjxm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibblemvs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gjqghfsz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3oscvjfzf.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3fxsirves.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3dbcxeccc.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3aqwdxsxd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3daxehoqj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gbbjkwqq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zggpqckv.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oownzftm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3cxneyfie.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3iymsrzpa.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3jggtkbrf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3feedifkr.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3xbyicyeg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpbrvuof.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bubzahjt.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3evtyvglf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mokuylba.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3vgxkdgbk.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3uyfigojv.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ffctagfw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3abkgpglm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3zxlvrrjm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3qykuaorw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pafqtdkt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nlibjzqb.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pgxzhjla.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3dtbejpmq.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3hwiyivzm.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3pyfodprc.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3fykclujd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3xdvfaeez.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mvowyvwr.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vtkqunjj.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3jeblsjiv.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3pnnfgknl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ueacdnpb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3zazynymz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwplysao.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3jtvmmfnd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3jalgdbuz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3awuubzre.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ulzujvot.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlbfyonp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ccjxenxg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3rwhivwpk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3sffwdvpi.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3exejctpu.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3eezrsjdl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3relbrooj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3gcpveshr.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3kwgjqhsv.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3urwiskfv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3wngvlikc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3xbaghtte.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wxjipvdc.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3dxsrtmjc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3yexodqkq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3sibsgtxu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uhbpwjgf.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3cnkiadle.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ffngzajy.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jlgqejds.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3iwbwwpko.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3hmxatmyx.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3qzsvyxfp.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ayviszdh.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3shnzyafb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjkeyibq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mntenqbu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjcztwhj.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmsvsqsi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zxhuahfk.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hirgrmri.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ixjjhkuq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ffkapzid.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ankrncme.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3beimfrcu.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dfcffcel.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ixtrhwbb.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3txdlxrhd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3wuhfekwy.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3enpdxnih.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3osvxzeta.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3gyehkunj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3dfrdcflg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3afgcrcua.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3mootoslx.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3kihkkpbl.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3sxzxedum.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3clmjyjwd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3jodlitlx.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3zvrgsgue.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3kzyhdxlv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3iplrrltc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3fnxlzgtr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3jhqknsub.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3nljepmxs.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ramzcshn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3eoiykctn.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3cylceltw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3fkzruger.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3mzcvgmcs.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3dvdfkjsz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3pgyusdoj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dsdlfnmw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3bommxyla.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3auvkofbz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3zxnfikvj.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3lhzyzchp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3colilsxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3omsizhyt.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vhfsqgcw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jsxhuijf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3yukqfpdp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3sfftqvwm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nmhcjaof.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3zrjedock.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hvnpbvpc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3rcyyesdv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3qvnpsmwt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ropgwzxv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3cooaachm.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3rzcntgua.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3uqkovhbl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ppiunmig.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hzqduenn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbzyqqvu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgrnlwlb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3mhdvsray.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3xqsqqryi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cgixoybw.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ckarlweo.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3fgdeupio.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rhuhwcmq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3bpvxqizt.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lupgizfb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wtshdjkz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3paabhgbl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3advqicnv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cqipnvnk.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3hdnxcylf.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3rsmmvpno.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3lnizkjkj.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3qcegzdvf.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3rxspwhtq.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3yiosqist.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3oqwxqgss.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3uenmaqld.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3voimyqnv.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3lgbqjpnj.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3visnbzlp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3tbzbkuns.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3fxpzaqow.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3uxqhrbfw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hdzkyxkr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3icpolska.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3hzrmcytn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cblkiwmr.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3gywprlqj.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3rxgqxkru.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3zfiweqcv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3jjmfgswi.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3miujfxfz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3jzitvrqd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3qkgyoqyc.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3zcuvkmwz.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3mfgiuybj.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3xvuhvptc.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3rkzcmgbe.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dppkvegl.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3egzhrajr.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3jhjqthhd.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3vkukrwwv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3kawvivqi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3qzaqdxpo.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3walnyabq.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3puiwkcvv.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3xywfbfyb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3fqitavdu.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3niukkwfv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3tptpweqx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3prkajric.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3syzpewtp.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3fkhgptvh.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3ghwouitr.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3ywhlrbbn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3mxaazovk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3qfswukdz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3wbxfonco.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3bsxadqmm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3tipdfecb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3xxyviwzd.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3mgkwfycx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3mjdslnzr.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3drbibifo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3zjashqzr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3qiwhcncq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3jqhyovkt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3yfvynuvp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3pujunacv.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3kzkvnrij.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3tmzzlcov.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ijkfegjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ovcfolyl.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3jadaguje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eamlabye.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3icruguhv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3fylxiplf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3eifaikff.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3pxpvkert.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rnqvboct.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3nbbtsutn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wclppixi.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3pcqznaue.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3iddpinle.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hqsimvzy.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3repqgtdi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3ygtbbzja.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3gysfknof.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3chmnahmk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3geprbrnk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3gdzyscke.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3utbhmgka.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yabronsn.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3rskknnid.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cmvbmfqy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3iyyivvht.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3disxdjss.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3aymmltoj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3czsnxbfn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3fwyokidp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3hhtesnbt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3udzbkahh.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3jhejlrbm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fskmycsd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zphnlnpv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gchaemvi.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3uzbrdcdw.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3vaajnkfx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3zcqkybjp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3bwyyxlvr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3hjnbdwrj.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ddvktqqh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3yscgvqac.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gcwswbsx.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3bblfofwx.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3edhspkwm.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3rzsrzmqq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3fzmjvbdq.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3xxldcjdv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3nlqlenip.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.52xcode.cn/Article/details/gt3eicmfibb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3gochgiuk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.52xcode.cn/Article/details/gt3fckemhmo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.ydjk.org.cn/Article/details/gt3kaqbwlxq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt3qvhsitzl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3eqwvozzz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.52xcode.cn/Article/details/gt3ogirufso.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.ydjk.org.cn/Article/details/gt3xhlaoxfx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt3qhpzmpdw.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt3tsshrbjv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt3heckqcac.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3nejpvgdu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.52xcode.cn/Article/details/gt3dsqpxvtn.html

TS:   /error/gim
来源：http://www.ydjk.org.cn/Article/details/gt3ocqzexje.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt3drytnpgv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt3crdqslax.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt3hofqjzpq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.52xcode.cn/Article/details/gt3mwekreyz.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt3wezoojvv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.ydjk.org.cn/Article/details/gt3snmudbvk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt3pivibhna.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt3olqlayup.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.52xcode.cn/Article/details/gt3kplssrmc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.52xcode.cn/Article/details/gt3lyonvbde.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.52xcode.cn/Article/details/gt3dmstoddx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt3koqziasm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt3hwykgwaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uxzunlys.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt3zzrbvgam.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3acrlfqsq.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt3jguknrhg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt3itzukzbj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.52xcode.cn/Article/details/gt3ifwodnzy.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt3kedivyhd.html

TS:   new Date();  Date.now()
来源：http://www.ydjk.org.cn/Article/details/gt3bnotxwdq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt3jdeqrjri.html


<!-- 参考信息 -->