代发 wailian999

Java: class Admin extends User {}
来源：http://hz.zhiwuduotai.top/gtjaqevzxm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.iojbl.cn/gtgplwjrsl.html

Ruby: class Admin < User; end
来源：http://hz.nwbrower.top/gtvkpfmepq.html

C#:   class Admin : User {}
来源：http://hz.tianlin.xyz/gtscpucdro.html

[G06] 重写方法
来源：http://hz.jianghu66.top/gttgvrtdhd.html

Py:   def greet(self): return "admin"
来源：http://hz.gotoacloud.top/gtejecllmr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hongshengwenyu.top/gttmcmpgkj.html

JS:   greet() { return "admin"; }
来源：http://hz.0kj1m.cn/gtukhskxof.html

TS:   greet(): string { return "admin"; }
来源：http://hz.wangshuangyany.cn/gthavyrjts.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.chenzaomai.com/gtqvhjbfxv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hnxiangtu.top/gtcorwvcsq.html

Ruby: def greet; "admin"; end
来源：http://hz.xuetiantiany.cn/gtbbixaoas.html

C#:   public override string Greet() => "admin";
来源：http://hz.hywenlv.cn/gtdrmjjtuu.html

[G07] 调用父类方法
来源：http://hz.ywan-chungtsiang.top/gtuijxzomw.html

Py:   super().greet()
来源：http://hz.pengpengdd.cyou/gtwtaxcmdp.html

PHP:  parent::greet();
来源：http://hz.yvedp.cn/gtehlolaoh.html

JS:   super.greet();
来源：http://hz.sxryk.cn/gtdubfcndd.html

TS:   super.greet();
来源：http://hz.shuidangran.top/gtuxjuvvmw.html

Java: super.greet();
来源：http://hz.guannengcc.top/gtkdgmmxfq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.chenjidiqi.icu/gtkqzcaupx.html

Ruby: super
来源：http://hz.shanyushiyangtech.top/gtoooeryyq.html

C#:   base.Greet();
来源：http://hz.wangshuangyany.cn/gtgvkzenvp.html

[G08] 静态方法与属性
来源：http://hz.yj20258888.top/gtqloycdmk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shangyingyoupin.top/gtmpbfgqyw.html

PHP:  public static function f() {}
来源：http://hz.snrcjt.cn/gthzkhbdyo.html

JS:   static f() {}
来源：http://hz.fengsongda.top/gttdjbynlv.html

TS:   static f(): void {}
来源：http://hz.pengpengdd.cyou/gtndgqqzps.html

Java: static void f() {}
来源：http://hz.316326.xyz/gtaqdrenzx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhixingplan.top/gtfgtbhjoe.html

Ruby: def self.f; end
来源：http://hz.yangfankeji.com/gtlfcgegym.html

C#:   public static void F() {}
来源：http://hz.aibaodan.cn/gtclvvyiqc.html

[G09] 接口 / 抽象类
来源：http://hz.hywenlv.cn/gtlemyjrdt.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.fzhhl.top/gtondxksip.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.havefunace.top/gtzoprzmme.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.nanxuanxn.top/gtwpghfhcy.html

TS:   interface Shape { area(): number; }
来源：http://hz.cqqwz.cn/gtulmplcou.html

Java: interface Shape { double area(); }
来源：http://hz.316326.xyz/gtvfnlvnwk.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cashguo.top/gtgbutpiut.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yanxiufei.cn/gtalvyjkft.html

C#:   interface IShape { double Area(); }
来源：http://hz.yj20258.top/gtmibtibee.html

[G10] 访问控制
来源：http://hz.0kj1m.cn/gthftadrns.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.bjfxy.top/gtzoepxubr.html

PHP:  public / protected / private
来源：http://hz.shanyushiyangkeji.top/gttcfeizfo.html

JS:   #private 字段；其余公开
来源：http://hz.daxiang520.top/gtjkodavou.html

TS:   public / protected / private
来源：http://hz.xuanzx.com/gtrfkfexon.html

Java: public / protected / private / 默认包级
来源：http://hz.gaohongyu789.top/gtussoxipq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yuxming.cn/gtdbjcxipv.html

Ruby: public / protected / private
来源：http://hz.meibo888.top/gtzpbwubsj.html

C#:   public / protected / private / internal
来源：http://hz.tanke756.top/gtnqvyccmp.html

[G11] getter / setter
来源：http://hz.zycfv.cn/gtfpmvdpzr.html

Py:   @property 与 @x.setter
来源：http://hz.yanxiufei.cn/gtryftidaw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.pengpengdd.cyou/gtyurvbnfx.html

JS:   get name() { return this._name; }
来源：http://hz.gaohongyu789.top/gthixgisil.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj20258.top/gtkrekpkfw.html

Java: public String getName() { return name; }
来源：http://hz.aizwys.cn/gtmiktglbs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.chenlongwang.top/gtynzespah.html

Ruby: attr_accessor :name
来源：http://hz.hnxiangtu.top/gtkhdiaeht.html

C#:   public string Name { get; set; }
来源：http://hz.xingfuxueyuan.xyz/gtqpvxcyrt.html

[G12] 对象转字符串
来源：http://hz.tianlin.xyz/gttocrhrkn.html

Py:   def __str__(self): return self.name
来源：http://hz.hfpthk.cn/gtmuzkoccj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zdqjudy.top/gtxlwbmdti.html

JS:   toString() { return this.name; }
来源：http://hz.jyoumei.cn/gtnnuvvqjo.html

TS:   toString(): string { return this.name; }
来源：http://hz.xuetiantiany.cn/gtidkyebkk.html

Java: @Override public String toString() { return name; }
来源：http://hz.hongshengwenyu.top/gtkimcjmax.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.shanyushiyangtech.top/gtjoahgoph.html

Ruby: def to_s; @name; end
来源：http://hz.52xcode.cn/gtlupcqkcf.html

C#:   public override string ToString() => Name;
来源：http://hz.jinqigfzy.top/gtmrhnnjed.html

[G13] 判断对象类型
来源：http://hz.yuanzhike.top/gttyifpyvb.html

Py:   isinstance(u, User)
来源：http://hz.yj202588.top/gturzjojzl.html

PHP:  $u instanceof User
来源：http://hz.yueranfly.top/gtmcvwfunf.html

JS:   u instanceof User
来源：http://hz.9152youxi.cn/gtwemzwzcg.html

TS:   u instanceof User
来源：http://hz.9152youxi.cn/gtimiachsg.html

Java: u instanceof User
来源：http://hz.hongshengwenyu.top/gtybxshror.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xingfuxueyuan.xyz/gtwhaiabjd.html

Ruby: u.is_a?(User)
来源：http://hz.yj20258888.top/gtsnawicsl.html

C#:   u is User
来源：http://hz.sufxvd.cn/gtuiikwffp.html

[G14] 数据类 / record
来源：http://hz.ppjwa.cn/gtmsetuhvj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.svipenyu.cn/gtodepluvn.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.gzhubu.top/gtkckkuoen.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhengqikj.top/gtukeftozk.html

TS:   type User = { name: string; age: number };
来源：http://hz.cucudq.cn/gtxibkpqqh.html

Java: record User(String name, int age) {}
来源：http://hz.xingfuxueyuan.xyz/gteuyvfoqd.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jyoumei.cn/gthpybkrry.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.316326.xyz/gtwjtminoa.html

C#:   record User(string Name, int Age);
来源：http://hz.yonumen.top/gterszzmsa.html

[G15] 枚举
来源：http://hz.316326.xyz/gtlbujcdpq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.fengsongda.top/gtxhkinyik.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhixingplan.top/gtbolmuyng.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.c1oappe.top/gtczmfltfq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhaomingkeji.xyz/gtrzwyllcn.html

Java: enum Color { RED, GREEN }
来源：http://hz.meibo888.top/gtlgrbregz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yj20258.top/gtbdswwjbc.html

Ruby: Color = %i[red green].freeze
来源：http://hz.dashuyun.cn/gtzdnejnkv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgufenzy.top/gtfimuyhln.html

[G16] 对象转数组 / 字典
来源：http://hz.yj20258.top/gtjtusnlqs.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jqgfzy.top/gtgdbonrqo.html

PHP:  get_object_vars($obj);
来源：http://hz.wangdashe.top/gtcgujsxpt.html

JS:   Object.entries(obj)
来源：http://hz.gzhubu.top/gtnnutiatz.html

TS:   Object.entries(obj)
来源：http://hz.havefunace.top/gtpafwsyen.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhongyouzk.top/gtswtnezyz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yueranfly.top/gtaqtlvjfs.html

Ruby: obj.instance_variables
来源：http://hz.jyoumei.cn/gtsbrynkiy.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xinyue.icu/gtwnprohav.html

================================================================================
来源：http://hz.hnqzz.top/gtethpcift.html

H. 异常与错误处理
来源：http://hz.xingfuxueyuan.xyz/gtleorxgbj.html

================================================================================
来源：http://hz.jqgfzy.top/gtxrafteya.html

[H01] try / catch 基础
来源：http://hz.shanyushiyangtech.top/gtyunpooir.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ppjwa.cn/gtcjcnmkvb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ppjwa.cn/gtdilljprf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.fengsongda.top/gtyqxulxfb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jinghuilouyu.cn/gtnabrxmqq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ydzc1.top/gtuphuhccn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xuanzx.com/gtsdqworvo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ehwqpu.com/gtjqgdwspg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xuetiantiany.cn/gtvvfxxdoc.html

[H02] finally / ensure 收尾
来源：http://hz.chenlongwang.top/gtyxjrocet.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.iojbl.cn/gtofeshedj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtcfffvjxx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtfyvthlor.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtgeazgolp.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nwbrower.top/gtzzphixde.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.havefunace.top/gtxffwhowt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.kuanghao11.cn/gtdeylikpt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yueranfly.top/gtrinbylrw.html

[H03] 主动抛出异常
来源：http://hz.vqdsnc.cn/gtbrucauev.html

Py:   raise ValueError("错误信息")
来源：http://hz.hnxiangtu.top/gtdjfyqcwu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cheryme.top/gtwrndklqm.html

JS:   throw new Error("错误信息");
来源：http://hz.ydjk.org.cn/gtsdrcnjms.html

TS:   throw new Error("错误信息");
来源：http://hz.yj202588.top/gttgbyyxln.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gtwddddiqi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hysaishi.cn/gttozypljg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.bjfxy.top/gtfiqqwned.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hfpthk.cn/gtwbopfrhe.html

[H04] 自定义异常类型
来源：http://hz.yj202588.top/gtgdciorcu.html

Py:   class MyError(Exception): pass
来源：http://hz.cucudq.cn/gtfitztihv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.wangdashe.top/gtrufrcors.html

JS:   class MyError extends Error {}
来源：http://hz.chenzaomai.com/gtgivjkbdv.html

TS:   class MyError extends Error {}
来源：http://hz.tian-w.cn/gtvswvrcox.html

Java: class MyException extends RuntimeException {}
来源：http://hz.wangdashe.top/gthzpdzmdx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xuanzx.com/gteyrxunia.html

Ruby: class MyError < StandardError; end
来源：http://hz.ydzc1.top/gtgmhvwvjq.html

C#:   class MyException : Exception {}
来源：http://hz.guannengcc.top/gtwrwzrstl.html

[H05] 捕获特定类型
来源：http://hz.jqgfzy.top/gtetgaorqv.html

Py:   except ValueError as e:
来源：http://hz.hnxiangtu.top/gtosckcxcp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.snrcjt.cn/gtrgomruux.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xziqi.cn/gtnftkbxuq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yueranfly.top/gtqieuhtjp.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.kuanghao11.cn/gtpvwqxhlr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinqigfzy.top/gtrlwvzrkb.html

Ruby: rescue ArgumentError => e
来源：http://hz.jqgufenzy.top/gtotwjvmjj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jlsjyb.cn/gtvdcldpgl.html

[H06] 可选值 / 空值安全访问
来源：http://hz.chenjidiqi.icu/gtnjcboxqj.html

Py:   value = d.get("k") or default
来源：http://hz.shanyushiyangkeji.top/gtuqaepmdg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.quarkkingdee.top/gtkabitdok.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.fengsongda.top/gtbotfeogn.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.fengsongda.top/gtjnakpvzx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yangfankeji.com/gtivqeglhd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sufxvd.cn/gtuygeuvge.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jianghu66.top/gthrqvdtie.html

C#:   obj?.A?.B ?? default
来源：http://hz.jyoumei.cn/gtrjhjwpxt.html

[H07] 断言
来源：http://hz.chenzaomai.com/gtwlzxcesw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhengqikj.top/gtnhgjrdri.html

PHP:  assert($x > 0);
来源：http://hz.svipenyu.cn/gtmgkrigvb.html

JS:   console.assert(x > 0);
来源：http://hz.xingfuxueyuan.xyz/gttrueosvc.html

TS:   console.assert(x > 0);
来源：http://hz.shangyingyoupin.top/gtanoyuanv.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sysykeji.top/gtyqntykff.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shangyingyoupin.top/gtxrkskqdz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.mhx1999.top/gtzttreewh.html

C#:   Debug.Assert(x > 0);
来源：http://hz.9152youxi.cn/gtqfqncpgm.html

[H08] 获取错误信息与堆栈
来源：http://hz.gaohongyu789.top/gturifaxjc.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.guannengcc.top/gtjyjsqmhc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.0kj1m.cn/gttimearaj.html

JS:   e.message;  e.stack
来源：http://hz.shanyushiyangkeji.top/gtjovfghqg.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cqqwz.cn/gtbkczyiyv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yj20258.top/gtgghubojc.html

Go:   err.Error()
来源：http://hz.cheryme.top/gtjvftbwez.html

Ruby: e.message;  e.backtrace
来源：http://hz.yuxming.cn/gtaybowfyh.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xingfuxueyuan.xyz/gtwxvfdsue.html

[H09] 带错误码的异常
来源：http://hz.jyoumei.cn/gtzupnfaro.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hnqzz.top/gtfgqrfvnd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hnxiangtu.top/gtqpubiqng.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.nwbrower.top/gtgzngvdht.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jqgufenzy.top/gtvuudzbly.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hysaishi.cn/gtodrmviec.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.gaohongyu789.top/gtcvjjtqkq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.c1oappe.top/gtagpimhqz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.fengsongda.top/gtwiqlajrl.html

[H10] 资源自动释放
来源：http://hz.shzxlz.cn/gtizmbdnfm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yonumen.top/gtmrzulegb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yangfankeji.com/gtullibccr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigufen.top/gtigrokono.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dianchejie.cn/gtwdnfoscc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.shanyushiyangkeji.top/gtckfbawqi.html

Go:   defer f.Close()
来源：http://hz.hnxiangtu.top/gtwknrajky.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jyoumei.cn/gthrzscqqc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cucudq.cn/gtpqekarpc.html

================================================================================
来源：http://hz.gogol.net.cn/gtccwfdiyv.html

I. 正则表达式
来源：http://hz.yanxiufei.cn/gtxeokwuqo.html

================================================================================
来源：http://hz.xinyue.icu/gtzhafqove.html

[I01] 判断是否匹配
来源：http://hz.nwbrower.top/gtopuumrhr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jinyuanbaomall.cn/gtvahmpava.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.chenjidiqi.icu/gtzeyyhgwa.html

JS:   /\d+/.test(s)
来源：http://hz.pycfn.com/gtcjogbmcd.html

TS:   /\d+/.test(s)
来源：http://hz.hywenlv.cn/gtmrytsyvu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhaomingkeji.xyz/gtmsszhrti.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhaomingkeji.xyz/gtwdfwhuhe.html

Ruby: s.match?(/\d+/)
来源：http://hz.kuanghao11.cn/gtjhkpytxw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhaomingkeji.xyz/gtuuvkhphq.html

[I02] 提取所有匹配
来源：http://hz.wangdashe.top/gtoidonjlo.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hnxiangtu.top/gtoogkfghr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xuetiantiany.cn/gtccxhhjmv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zycfv.cn/gthkblxavc.html

TS:   s.match(/\d+/g)
来源：http://hz.kuanghao11.cn/gtfofpndvg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.aizwys.cn/gtguqfjpsa.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.nwbrower.top/gtgwecybfh.html

Ruby: s.scan(/\d+/)
来源：http://hz.jqgufenzy.top/gtghmwzvko.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.daria6918.cn/gtkcfjwoga.html

[I03] 提取捕获分组
来源：http://hz.c1oappe.top/gthdfcfkfd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sysykeji.top/gtezwyzqjl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.cdnleiting.top/gtimkbolfa.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj202588.top/gtyynadwyj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yanxiufei.cn/gtizcfuour.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jlsjyb.cn/gtorjjtcbe.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.gotoacloud.top/gtznlipbwx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.meibo888.top/gtnzniucmn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhixingplan.top/gtnvkvluqm.html

[I04] 正则替换
来源：http://hz.haohaochexian.top/gtdaxwzunw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shzxlz.cn/gtsromkzey.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.nanxinkj.top/gtzptcupaf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yj202588.top/gtlaiddcvs.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.chenzaomai.com/gtosxxyuhf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hongshengwenyu.top/gtwydwowim.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sufxvd.cn/gteqpvalzs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gotoacloud.top/gtnjnvmsnu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.chenjidiqi.icu/gtdjqtxfgv.html

[I05] 按正则拆分
来源：http://hz.hywenlv.cn/gtwparqzpo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhoulong.xyz/gtnbukkuiw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhoulong.xyz/gtvnthkuci.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yvedp.cn/gtralzjrlv.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shangyingyoupin.top/gtkkmveoof.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shzxlz.cn/gtaleskhwi.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.daxiang520.top/gtdzuirwpc.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shangyingyoupin.top/gtmsgfpcdo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.dashuyun.cn/gtzesgscwt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jinqigfzy.top/gtjegrfkuq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yj20258888.top/gtglcoxtkb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.pycfn.com/gtheezhiqm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ehwqpu.com/gtjoikpiup.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.haohaochexian.top/gteyctkpvx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xuanzx.com/gtsrekvkwz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cheryme.top/gtiqfhpbyx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hnxiangtu.top/gtijpengzw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ppjwa.cn/gthgaoyffl.html

[I07] 忽略大小写与多行模式
来源：http://hz.daxiang520.top/gtbwxuykwo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yongpay.top/gtrdmgsrtw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ehwqpu.com/gtfejkhhdi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yueranfly.top/gtxaaldjjm.html

TS:   /error/gim
来源：http://hz.ydjk.org.cn/gtngnwhdjw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.vqdsnc.cn/gtndrdobwm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.dashuyun.cn/gtuigokejp.html

Ruby: s.scan(/error/i)
来源：http://hz.ywan-chungtsiang.top/gtiogescir.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.pengpengdd.cyou/gttlplzluy.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yongpay.top/gtazvjvutc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yuanzhike.top/gttpciuzpo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhiwuduotai.top/gtzjdnjejt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nanxinkj.top/gtqcauyhpz.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.meibo888.top/gtarhclpyr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhengqikj.top/gtyhyiupsl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yanxiufei.cn/gtewgnpfcg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shangyingyoupin.top/gteaqlfdvs.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cqqwz.cn/gtmvfwrbbt.html

================================================================================
来源：http://hz.iojbl.cn/gtpljzxqxo.html

J. 日期与时间
来源：http://hz.yanxiufei.cn/gtnclsrnme.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtjcmetqzp.html

[J01] 获取当前时间
来源：http://hz.tianlin.xyz/gtynhikuni.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zycfv.cn/gtupjnkpdi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xingfuxueyuan.xyz/gtozpxkyco.html

JS:   new Date();  Date.now()
来源：http://hz.fengsongda.top/gtzuehlmch.html

TS:   new Date();  Date.now()
来源：http://hz.gaohongyu789.top/gthroowiii.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cdnleiting.top/gtzoubeywr.html

Go:   time.Now()
来源：http://hz.svipenyu.cn/gtdlyqoawq.html

Ruby: Time.now
来源：http://hz.xinyue.icu/gtuctderoh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.vqdsnc.cn/gtodxbpexb.html

[J02] 格式化输出
来源：http://hz.cucudq.cn/gtvshzztpr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.meibo888.top/gttdjsicfv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.guowangkeji.top/gtrthought.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gaohongyu789.top/gtujxaezme.html

TS:   d.toISOString()
来源：http://hz.hammf.cn/gtijadbvyb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.quarkkingdee.top/gtsdipjqdg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.52xcode.cn/gtgnvlnwwe.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258888.top/gttimfhjlh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yj202588.top/gtlpavxjga.html

[J03] 字符串解析为日期
来源：http://hz.yonumen.top/gtipfaixxo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinqigufen.top/gtajtujhix.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hysaishi.cn/gtjuuyztgb.html

JS:   new Date("2024-01-02")
来源：http://hz.daxiang520.top/gtertzikrk.html

TS:   new Date("2024-01-02")
来源：http://hz.dashuyun.cn/gttkxnwjan.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.c1oappe.top/gtvuggdpby.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.0kj1m.cn/gtyuchrkwd.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.guowangkeji.top/gtcbtwqtml.html


<!-- 参考信息 -->