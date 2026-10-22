代发 wailian999

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2bbcvdxsg.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2jfslyubv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2aichmxis.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wggwghfo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2xqjlcjfi.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2mmyueaze.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ipaczzhw.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2cvmktmop.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ijlduwdo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2zuuhkkwn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2wumeizjb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftmyqoan.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtutvirx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2rixlrcpl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2zdnkbfyo.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tcioojkj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2yzbuwnpd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2oznmbnfv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tbhlaugv.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2pglqqcik.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wclpudos.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2tknszwnp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2njnzbgqz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2aujeoajo.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2khobywfn.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2podosvwi.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2nwunbnid.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxwdzaoz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2vrejgjuk.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2hasfufsl.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqsisnvg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qsgfbkqe.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2bpawnphg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqgniurj.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2fiyjicty.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vlwtgmcz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfyvckda.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2testgevg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uzwwyvua.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2whdzlhto.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2pbyxzonu.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2adcuobcb.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ozngerod.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2otdstasp.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2pmtcrble.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2npybvxeb.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2zbmzdnrc.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ncsyatwl.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pvruqtof.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2mcjdniln.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2vflmshxy.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2twffjcai.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2cbsqfxse.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2sxxhapjj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2hdkxwxmh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2kbfzhewn.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2dqmfxbse.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zaygzqpn.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2xtlouqak.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2boiukjcm.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2kkkgkdjg.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2aqezoywe.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2kjsafcdk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ulwzplww.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2vbaubkeh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2caaafafl.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2tyothqyl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2iwpnvbsz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2wngpdefb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ypdamhkh.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2gnbshinw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2mxumwvgs.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2vcrfusbx.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2uruvfdqe.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2qkiyjzna.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2dhquzuja.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2diitpgcc.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2lyabzxmu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2uvzoydvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mfskgeot.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2lfufkaya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yamjcopp.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2bsbautpg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2yaqksytq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2ayqxlvxf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2iexzulnl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2rjuynlvg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2cpenmsev.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2igimqehp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2uwycuatc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2bzcavanh.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2uvaqiukk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ypgwzxms.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ogndmqgj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xcuqqrqm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2peocfnvu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hodthzgf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2avwlyguq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2xhhxzvmu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xdgfbzoz.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2mqoncxcl.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ljydmimt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wgolorxl.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2nhxssblo.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bpjlyixi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zkdqyvef.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2ilwoeywi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2sadgnxrg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qqwzkqrr.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2vtujkbvl.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2yxbhkbva.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2gkbjzaxu.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2kfbefdmz.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2zlzeytcn.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2kionxvxw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2cltwjzpp.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2nwammgxu.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2juubouvq.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2akpfxpbt.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2symuogld.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2dowdeflr.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ffeuyhkr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2addxdpgz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vderzqqm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2kfmjlzjd.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2sjngctgl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqfphjrh.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2mctxryuv.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2wvbtppzt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2bowdhtmz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ysmrbrhf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2socwrtix.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2kzrzgfrt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2zfouvocg.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2eujvbhpp.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2taezyrne.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2zzhhhoir.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2amowtxky.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ypnrgoxw.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dvbfgiks.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vnurwame.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2fwfnzgqg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2dpuieymi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2ocsvgggk.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bxmggkqy.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2lrzfgbmc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2ciggidfg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2wzbgyqaj.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2eckemmcg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2lfximjml.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2sdzzziyq.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2bcdtgbjv.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2kboxnyks.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2shhnzpgd.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2mgoguree.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2mjsarzjj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2rnzsdjpy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2msacbbll.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2qylatyhf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2uvvhkysd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2qjzieygu.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2vrtavtde.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2hzuupdvq.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2zjbpmfhn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2acaolvtf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2wepulufy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2onkwtyuo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2dkqmkzpe.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2dbasitzb.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2kiuajtbc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2cnfrixjd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jhynzzog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dnxdindt.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wbqvlsys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzhxwkvm.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2jbmpebfk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2npzpeyjz.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zddewgix.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yqjnalvj.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2bwgrgckl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2cdpscphm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tghzkafk.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2pcqmgyxi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2yqxwtbds.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2vbmnyidt.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2bvylheng.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2yninrjgz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2zcjajiie.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2fkmlsims.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2obnkldke.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2sunfwxes.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2zuzpauua.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jiygjfqm.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2fekfvnyf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hkcvulfq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2vlaabajo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2fnoenpuc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt2kjaxmacn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2ozobxeaw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2rusjrrbm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2hnhntwat.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2qhepynye.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2jbkxhepm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2nzhrizjf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2wppecvvq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2bfajyfhv.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2thizbkmq.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2afigqtbt.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt2ffywlyrt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt2lkhktjxz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2thfuzcqs.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hlngtkwx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt2ftjtpavu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.52xcode.cn/Article/details/gt2trgsztdl.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2symjrkyo.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt2ccuzfeei.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt2iekkjtbj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2vwqkqoku.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt2kxqnrgon.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt2szzodtio.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://www.ydjk.org.cn/Article/details/gt2zrrojmzz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2obejrdxw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://www.ydjk.org.cn/Article/details/gt2tsjukgzd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2zkzkxnfz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://www.52xcode.cn/Article/details/gt2bxzfhvzw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://www.52xcode.cn/Article/details/gt2gacuhlni.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.ydjk.org.cn/Article/details/gt2ujgnubcf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://www.52xcode.cn/Article/details/gt2impruubi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.ydjk.org.cn/Article/details/gt2bkreirwa.html

[I07] 忽略大小写与多行模式
来源：http://www.52xcode.cn/Article/details/gt2jvxukqxe.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://www.ydjk.org.cn/Article/details/gt2iowohino.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2sbdlscrp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://www.ydjk.org.cn/Article/details/gt2xgcqtjai.html

TS:   /error/gim
来源：http://www.52xcode.cn/Article/details/gt2mwnfxlgb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://www.ydjk.org.cn/Article/details/gt2pqdzjewm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://www.52xcode.cn/Article/details/gt2dndfsrti.html

Ruby: s.scan(/error/i)
来源：http://www.52xcode.cn/Article/details/gt2bqtboyds.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.ydjk.org.cn/Article/details/gt2ylkbgmee.html

[I08] 贪婪与非贪婪匹配
来源：http://www.52xcode.cn/Article/details/gt2whnvefeq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://www.52xcode.cn/Article/details/gt2novefzdx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://www.52xcode.cn/Article/details/gt2oplbyooo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2tkfxsnbt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.ydjk.org.cn/Article/details/gt2etmlaqrv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2xzikbclm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://www.ydjk.org.cn/Article/details/gt2ensyzyun.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://www.ydjk.org.cn/Article/details/gt2ubzuvwot.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://www.ydjk.org.cn/Article/details/gt2iptkjbyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qwdjaavp.html

J. 日期与时间
来源：http://www.ydjk.org.cn/Article/details/gt2urcuhtog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rqrvyqkz.html

[J01] 获取当前时间
来源：http://www.52xcode.cn/Article/details/gt2dwofkjwd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://www.52xcode.cn/Article/details/gt2ruylhtca.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2ktjbcija.html

JS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2yutpxzfw.html

TS:   new Date();  Date.now()
来源：http://www.52xcode.cn/Article/details/gt2wtmvegrc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://www.52xcode.cn/Article/details/gt2shydxghq.html

Go:   time.Now()
来源：http://www.ydjk.org.cn/Article/details/gt2lkiiqevq.html

Ruby: Time.now
来源：http://www.ydjk.org.cn/Article/details/gt2cfotmcbj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.ydjk.org.cn/Article/details/gt2cjamhgrg.html

[J02] 格式化输出
来源：http://www.52xcode.cn/Article/details/gt2mpdxjiec.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2zttvdeeo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.ydjk.org.cn/Article/details/gt2lkgwefxz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://www.ydjk.org.cn/Article/details/gt2gximcbew.html

TS:   d.toISOString()
来源：http://www.ydjk.org.cn/Article/details/gt2jthhxinl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://www.ydjk.org.cn/Article/details/gt2ahoqvajj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://www.ydjk.org.cn/Article/details/gt2rqlobgbi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://www.ydjk.org.cn/Article/details/gt2bdiznjhl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://www.52xcode.cn/Article/details/gt2gijpvtzv.html

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2tfhdheby.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt2ahygplby.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2wfniuros.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2kyamkacd.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2fgcsdtly.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2exdxdtgh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ndnyayfy.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2tzluikkq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt2coignnbk.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2byjuwskt.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2pbqwduco.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2dgmgddur.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2ynmdrnql.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2fljzaebu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt2jowhjfnc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2rlhunsap.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2qbthtprd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt2fooqesdg.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt2zseqbipk.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2ptugnlfp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2vubwkwrl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2rcrqthnv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2jystgefb.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2gapzcmkc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mmcskayp.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2oehswvbh.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2oaucyqpf.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt2orbcugrq.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt2kovbvfsi.html

PHP:  $end->diff($start)->days;
来源：http://www.ydjk.org.cn/Article/details/gt2avyroohc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2jzghpmky.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2xruqeykn.html


<!-- 参考信息 -->