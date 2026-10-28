代发 wailian999

Py:   class Admin(User): pass
来源：http://hz.redwolf501.top/gtfmrjqdli.html

PHP:  class Admin extends User {}
来源：http://hz.smart0.xyz/gtchozccra.html

JS:   class Admin extends User {}
来源：http://hz.pycfn.com/gtqnrgjmkl.html

TS:   class Admin extends User {}
来源：http://hz.ehwqpu.com/gtlvjwyiyg.html

Java: class Admin extends User {}
来源：http://hz.wangdashe.top/gtwzgxqykf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jinqigfzy.top/gtkjmaocba.html

Ruby: class Admin < User; end
来源：http://hz.9152youxi.cn/gtfsbvmcnl.html

C#:   class Admin : User {}
来源：http://hz.aibaodan.cn/gtavuztugh.html

[G06] 重写方法
来源：http://hz.chenjidiqi.icu/gtdqshwvxq.html

Py:   def greet(self): return "admin"
来源：http://hz.jinghuilouyu.cn/gtlnaffama.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.fzhhl.top/gtajzsnunn.html

JS:   greet() { return "admin"; }
来源：http://hz.havefunace.top/gthgcfhalq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.c1oappe.top/gtoqzpaccf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gtcibczapp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.tian-w.cn/gtnfksqozo.html

Ruby: def greet; "admin"; end
来源：http://hz.tianlin.xyz/gtreeihykk.html

C#:   public override string Greet() => "admin";
来源：http://hz.haohaochexian.top/gtlewtukjm.html

[G07] 调用父类方法
来源：http://hz.shuidangran.top/gtauwzecki.html

Py:   super().greet()
来源：http://hz.tanke756.top/gtvlpbbjuq.html

PHP:  parent::greet();
来源：http://hz.zhixingplan.top/gtearrbndo.html

JS:   super.greet();
来源：http://hz.iojbl.cn/gturxinexc.html

TS:   super.greet();
来源：http://hz.hnxiangtu.top/gtjwydkdsq.html

Java: super.greet();
来源：http://hz.sufxvd.cn/gtyxqlcicm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jlsjyb.cn/gtweljlbtp.html

Ruby: super
来源：http://hz.jianghu66.top/gtqgsabjqi.html

C#:   base.Greet();
来源：http://hz.zhengqikj.top/gtmrkaywcj.html

[G08] 静态方法与属性
来源：http://hz.52xcode.cn/gtwtkldprl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.gotoacloud.top/gtpgeywrxb.html

PHP:  public static function f() {}
来源：http://hz.fengsongda.top/gtwdjjwwkr.html

JS:   static f() {}
来源：http://hz.sufxvd.cn/gtelgtbnpj.html

TS:   static f(): void {}
来源：http://hz.zhaomingkeji.xyz/gtzhlqllae.html

Java: static void f() {}
来源：http://hz.shuidangran.top/gtwwpzhxmy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yj202588.top/gtuzikrwuv.html

Ruby: def self.f; end
来源：http://hz.tianlin.xyz/gtwwszojrn.html

C#:   public static void F() {}
来源：http://hz.meibo888.top/gtvbsvoxwx.html

[G09] 接口 / 抽象类
来源：http://hz.sweek.top/gtkqcdizer.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hammf.cn/gtwojcwqdn.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ivvv.top/gtjmespaym.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cdnleiting.top/gtyqzttnzi.html

TS:   interface Shape { area(): number; }
来源：http://hz.dashuyun.cn/gtcmymyfiu.html

Java: interface Shape { double area(); }
来源：http://hz.sweek.top/gtejpkycwh.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.wangshuangyany.cn/gtvhscvyyz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.chenlongwang.top/gtzgbpvepy.html

C#:   interface IShape { double Area(); }
来源：http://hz.dashuyun.cn/gtbbszbxny.html

[G10] 访问控制
来源：http://hz.jiagoushi.top/gtdpxtmwhp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yanxiufei.cn/gtzbkutfyq.html

PHP:  public / protected / private
来源：http://hz.meibo888.top/gttbvwzklr.html

JS:   #private 字段；其余公开
来源：http://hz.zdqjudy.top/gtrcacnuzw.html

TS:   public / protected / private
来源：http://hz.xinyue.icu/gtaoqfgery.html

Java: public / protected / private / 默认包级
来源：http://hz.mhx1999.top/gtimblpnkn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.havefunace.top/gtlrytxswq.html

Ruby: public / protected / private
来源：http://hz.fengsongda.top/gtfalsbxac.html

C#:   public / protected / private / internal
来源：http://hz.feifeiyinyue.top/gtiahrrfhl.html

[G11] getter / setter
来源：http://hz.quarkkingdee.top/gtfydtpemj.html

Py:   @property 与 @x.setter
来源：http://hz.mhx1999.top/gtslcbnizz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hysaishi.cn/gtxcakuznj.html

JS:   get name() { return this._name; }
来源：http://hz.sysykeji.top/gtshpjaqat.html

TS:   get name(): string { return this._name; }
来源：http://hz.yangfankeji.com/gtslipmjoe.html

Java: public String getName() { return name; }
来源：http://hz.52xcode.cn/gtoziramkf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hongshengwenyu.top/gtunesofre.html

Ruby: attr_accessor :name
来源：http://hz.hfpthk.cn/gtuimwqqox.html

C#:   public string Name { get; set; }
来源：http://hz.haohaochexian.top/gtbjetmmxy.html

[G12] 对象转字符串
来源：http://hz.cheryme.top/gtnqlckalm.html

Py:   def __str__(self): return self.name
来源：http://hz.ppjwa.cn/gteheojakq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jinqigfzy.top/gtastfmsph.html

JS:   toString() { return this.name; }
来源：http://hz.sxryk.cn/gtaactdylg.html

TS:   toString(): string { return this.name; }
来源：http://hz.yongpay.top/gtpoedythi.html

Java: @Override public String toString() { return name; }
来源：http://hz.ivvv.top/gtnnoqadht.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.pengpengdd.cyou/gtjlxezrsf.html

Ruby: def to_s; @name; end
来源：http://hz.sxryk.cn/gtdnvlkfhi.html

C#:   public override string ToString() => Name;
来源：http://hz.jiagoushi.top/gtuvmrdkza.html

[G13] 判断对象类型
来源：http://hz.sufxvd.cn/gtxckhkudz.html

Py:   isinstance(u, User)
来源：http://hz.kuanghao11.cn/gtltipvdlv.html

PHP:  $u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtrdyiamjx.html

JS:   u instanceof User
来源：http://hz.jyoumei.cn/gtsnpzmwaf.html

TS:   u instanceof User
来源：http://hz.tanke756.top/gtdzsvioch.html

Java: u instanceof User
来源：http://hz.daxiang520.top/gtwivlradw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.birdmap.top/gtxdvkbpye.html

Ruby: u.is_a?(User)
来源：http://hz.smart0.xyz/gtoilcckyp.html

C#:   u is User
来源：http://hz.hongshengwenyu.top/gtfaeundwp.html

[G14] 数据类 / record
来源：http://hz.yongpay.top/gtdjtyusku.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.snrcjt.cn/gtcdqvbzfg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhijiandao.cn/gthuxlcasn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cucudq.cn/gtolzwhjfs.html

TS:   type User = { name: string; age: number };
来源：http://hz.feifeiyinyue.top/gtbqossfew.html

Java: record User(String name, int age) {}
来源：http://hz.cdnleiting.top/gtuxkwfubv.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sweek.top/gtgzrqrnmo.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yonumen.top/gtxkxbyxch.html

C#:   record User(string Name, int Age);
来源：http://hz.cqqwz.cn/gtjmdvsror.html

[G15] 枚举
来源：http://hz.jinyuanbaomall.cn/gtwkkpsvtv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jqgufenzy.top/gtnvqczill.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xingfuxueyuan.xyz/gtqtvewxbx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.sxryk.cn/gtlklzxmfp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.meibo888.top/gtipjqgsyx.html

Java: enum Color { RED, GREEN }
来源：http://hz.haohaochexian.top/gtxzrxnjyf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zycfv.cn/gtqrcfzktd.html

Ruby: Color = %i[red green].freeze
来源：http://hz.bjfxy.top/gtmgyrbkdz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gogol.net.cn/gtmeklwvka.html

[G16] 对象转数组 / 字典
来源：http://hz.yueranfly.top/gtietgwswc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gogol.net.cn/gttsufvjra.html

PHP:  get_object_vars($obj);
来源：http://hz.sweek.top/gtyfwzbkho.html

JS:   Object.entries(obj)
来源：http://hz.yangfankeji.com/gtkxjtkdod.html

TS:   Object.entries(obj)
来源：http://hz.jianghu66.top/gtjctdlxqb.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.aizwys.cn/gtrgmqmfol.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.fzhhl.top/gtcxpfsata.html

Ruby: obj.instance_variables
来源：http://hz.c1oappe.top/gtaijunihq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yangfankeji.com/gtlrqdghqi.html

================================================================================
来源：http://hz.vqdsnc.cn/gtckxuasqy.html

H. 异常与错误处理
来源：http://hz.xziqi.cn/gtgefxtghk.html

================================================================================
来源：http://hz.gogol.net.cn/gtflcgyzdk.html

[H01] try / catch 基础
来源：http://hz.xziqi.cn/gtyjddmhdw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jlsjyb.cn/gtzykkogcz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cheryme.top/gtcteeylhd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.meibo888.top/gtscdynjlu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.wangdashe.top/gtgaufhdou.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shanyushiyangtech.top/gtyqyebvwg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.dashuyun.cn/gtrxpzmdes.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.chenjidiqi.icu/gtzeayvhpe.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shangyingyoupin.top/gtjejhmklx.html

[H02] finally / ensure 收尾
来源：http://hz.ivvv.top/gtgvpfnwvw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hysaishi.cn/gtwdtfsvjc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtyzyqumlw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ybcxt.top/gtukbxprwt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yvedp.cn/gtjzfjgaor.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.haohaochexian.top/gteosxkuel.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhaomingkeji.xyz/gtznlucxos.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.bjfxy.top/gtoxrdjrsy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zdqjudy.top/gtlpjqhrqk.html

[H03] 主动抛出异常
来源：http://hz.ppjwa.cn/gtuqmblohz.html

Py:   raise ValueError("错误信息")
来源：http://hz.yuxming.cn/gtekwsdlpj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.vqdsnc.cn/gtmmlxosub.html

JS:   throw new Error("错误信息");
来源：http://hz.aizwys.cn/gtqmrwegon.html

TS:   throw new Error("错误信息");
来源：http://hz.hongshengwenyu.top/gtdfbtwvnp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ybcxt.top/gtnfeajbid.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.dianchejie.cn/gthzpgvqub.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.daria6918.cn/gtxsugnmoc.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhoulong.xyz/gtnoboebxd.html

[H04] 自定义异常类型
来源：http://hz.jinqigufen.top/gtrwelmmza.html

Py:   class MyError(Exception): pass
来源：http://hz.0kj1m.cn/gtbfwunoax.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jiagoushi.top/gthdkkmaiu.html

JS:   class MyError extends Error {}
来源：http://hz.feifeiyinyue.top/gtmcksksgf.html

TS:   class MyError extends Error {}
来源：http://hz.ivvv.top/gtsrohthnx.html

Java: class MyException extends RuntimeException {}
来源：http://hz.guannengcc.top/gteqcvsrsb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.aibaodan.cn/gttfkjpewf.html

Ruby: class MyError < StandardError; end
来源：http://hz.pycfn.com/gtscqcxlmb.html

C#:   class MyException : Exception {}
来源：http://hz.svipenyu.cn/gtyquhbtxq.html

[H05] 捕获特定类型
来源：http://hz.nanxuanxn.top/gtpngblymm.html

Py:   except ValueError as e:
来源：http://hz.jyoumei.cn/gtuoaasdls.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinyuanbaomall.cn/gtkyhpnbra.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.9152youxi.cn/gtgezpqhmc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangkeji.top/gtjxtszzdx.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.0kj1m.cn/gtvgkpwxjg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.pycfn.com/gtbsoowjsj.html

Ruby: rescue ArgumentError => e
来源：http://hz.tian-w.cn/gtfirduevx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yuanzhike.top/gtwyvzccyo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nanxuanxn.top/gtqvbuuwko.html

Py:   value = d.get("k") or default
来源：http://hz.birdmap.top/gtxrfilitn.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zdqjudy.top/gtmddwwcay.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ydzc1.top/gtjhnejidy.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xinyue.icu/gtvwagpbqq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.pengpengdd.cyou/gtnlppjapc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jianghu66.top/gtlvlovsez.html

Ruby: d&.dig(:a, :b)
来源：http://hz.sweek.top/gtdadfgnpc.html

C#:   obj?.A?.B ?? default
来源：http://hz.ywan-chungtsiang.top/gtdfpiqfhg.html

[H07] 断言
来源：http://hz.shuidangran.top/gtausjzwqy.html

Py:   assert x > 0, "必须为正"
来源：http://hz.0kj1m.cn/gtoxnegykl.html

PHP:  assert($x > 0);
来源：http://hz.cheryme.top/gtcrlqwepk.html

JS:   console.assert(x > 0);
来源：http://hz.meibo888.top/gtbvxkqpoi.html

TS:   console.assert(x > 0);
来源：http://hz.zdqjudy.top/gtkxguzxui.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ybcxt.top/gtwabxicbs.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hysaishi.cn/gtzufjayue.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.daxiang520.top/gtsipqwpjy.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jlsjyb.cn/gtklbbvsph.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhiwuduotai.top/gtsnwpvexj.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.dashuyun.cn/gtdiwwwpfz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jiagoushi.top/gtznndwfbc.html

JS:   e.message;  e.stack
来源：http://hz.ydjk.org.cn/gtpxxpmhrb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yj20258.top/gttbfktxwj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.nwbrower.top/gtlhnzsjhr.html

Go:   err.Error()
来源：http://hz.shanyushiyangtech.top/gtzvzunhar.html

Ruby: e.message;  e.backtrace
来源：http://hz.kuanghao11.cn/gtesivnorp.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhaomingkeji.xyz/gtrnfnkodp.html

[H09] 带错误码的异常
来源：http://hz.kuanghao11.cn/gtrhpqtzft.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yj202588.top/gtfpdajrhf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.dianchejie.cn/gtqylgrcto.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhengqikj.top/gtqrrfufpe.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.mhx1999.top/gtxurelvjs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.pengpengdd.cyou/gtouwdeitn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hongshengwenyu.top/gtjsmjndxo.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhoulong.xyz/gtmtfjgccd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yuxming.cn/gtttiolpzd.html

[H10] 资源自动释放
来源：http://hz.andypj.xyz/gtayznyphc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yueranfly.top/gtekoqsesf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cdnleiting.top/gtpnndvxou.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jianghu66.top/gtfefzlmga.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tian-w.cn/gtwylihhaz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.tian-w.cn/gtwdqywfrg.html

Go:   defer f.Close()
来源：http://hz.guowangkeji.top/gtiabnpfxj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xinyue.icu/gtjrkngvqg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.tanke756.top/gtffumesce.html

================================================================================
来源：http://hz.guannengcc.top/gtyidlitkh.html

I. 正则表达式
来源：http://hz.pengpengdd.cyou/gtiqbonpjo.html

================================================================================
来源：http://hz.wangdashe.top/gtnqzmklif.html

[I01] 判断是否匹配
来源：http://hz.ydjk.org.cn/gtkynpfyny.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.chenjidiqi.icu/gtyhbgfpid.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shangyingyoupin.top/gtailhzfrx.html

JS:   /\d+/.test(s)
来源：http://hz.shanyushiyangkeji.top/gtwkhjsyzt.html

TS:   /\d+/.test(s)
来源：http://hz.jinyuanbaomall.cn/gtpdsevgpo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.smart0.xyz/gtnvbwomxt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yvedp.cn/gtbdnwbkzk.html

Ruby: s.match?(/\d+/)
来源：http://hz.dianchejie.cn/gtkgmujidq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yvedp.cn/gtbgtvvhwn.html

[I02] 提取所有匹配
来源：http://hz.nanxuanxn.top/gtntwozwyp.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ywan-chungtsiang.top/gtvjgvhiht.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.smart0.xyz/gtptbkkmac.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yuanzhike.top/gtgtatbbkr.html

TS:   s.match(/\d+/g)
来源：http://hz.ydjk.org.cn/gtcmsgodvx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sweek.top/gtisireztq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shanyushiyangtech.top/gtatlxdluu.html

Ruby: s.scan(/\d+/)
来源：http://hz.cqqwz.cn/gtfhwerbeq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.bjfxy.top/gtumpyxpji.html

[I03] 提取捕获分组
来源：http://hz.yueranfly.top/gtimelkoch.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.haohaochexian.top/gtuixnybvp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.cheryme.top/gtzbmuassu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gogol.net.cn/gtjpvdmgfc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jinyuanbaomall.cn/gthtgwgcqg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.havefunace.top/gtlvbagcna.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jianghu66.top/gtandltwxz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cdnleiting.top/gtmrjmkwle.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.0kj1m.cn/gtcvdltsia.html

[I04] 正则替换
来源：http://hz.xinyue.icu/gtmrlmucvt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hnqzz.top/gtrpuuqrfo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.aizwys.cn/gtoeihnymp.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.sweek.top/gtsvgvgigp.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shuidangran.top/gtqnjqurat.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.pycfn.com/gtovftsvar.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ydzc1.top/gtijdavjey.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.redwolf501.top/gtohyrtikk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yueranfly.top/gttoqyepfs.html

[I05] 按正则拆分
来源：http://hz.cucudq.cn/gtleikntmo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yj202588.top/gthqdrbmef.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cashguo.top/gtpoeuigmr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xziqi.cn/gtouajuixw.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yvedp.cn/gtoglqpmus.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jqgfzy.top/gtoaqfyiev.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jiagoushi.top/gtxeuzlylg.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.pengpengdd.cyou/gthjeomvju.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.52xcode.cn/gtjzvsnhhk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.haohaochexian.top/gtngvblbci.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yonumen.top/gtzmlnjejf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.316326.xyz/gtcxgamjwk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hfpthk.cn/gtrabvtlmo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.kuanghao11.cn/gtvybeidhi.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.wangdashe.top/gtxlravpcs.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.316326.xyz/gtcutxowsp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.fengsongda.top/gtvfxqhzvw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yuxming.cn/gtirbgmalj.html

[I07] 忽略大小写与多行模式
来源：http://hz.dashuyun.cn/gtyyncmgye.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jinyuanbaomall.cn/gtdljpgxgr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.tanke756.top/gthojivzki.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.daria6918.cn/gttpclzlzb.html

TS:   /error/gim
来源：http://hz.zhoulong.xyz/gtwisfuacu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gaohongyu789.top/gtsoreswho.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.sxryk.cn/gtwnhziayh.html

Ruby: s.scan(/error/i)
来源：http://hz.yj202588.top/gtlwgdsfqz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cucudq.cn/gthicjxtna.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yj202588.top/gtnlyfvitj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.haohaochexian.top/gtybnxasps.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinyuanbaomall.cn/gtvyijbots.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yangfankeji.com/gtrkadpvhy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hongshengwenyu.top/gtrwiszfbm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ivvv.top/gtbrnjigll.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shangyingyoupin.top/gthncqipjg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.0kj1m.cn/gtrcpwwpms.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ydzc1.top/gtprwwidpv.html

================================================================================
来源：http://hz.ppjwa.cn/gtbotiumru.html

J. 日期与时间
来源：http://hz.yonumen.top/gtlikqvosf.html

================================================================================
来源：http://hz.shuidangran.top/gttgwdtewn.html

[J01] 获取当前时间
来源：http://hz.feifeiyinyue.top/gthoduiulf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ydjk.org.cn/gtskamszrk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhixingplan.top/gtyxyajzvj.html

JS:   new Date();  Date.now()
来源：http://hz.aibaodan.cn/gtpayrhnyo.html

TS:   new Date();  Date.now()
来源：http://hz.tianlin.xyz/gteolrwndr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jiagoushi.top/gtuhncbwnf.html

Go:   time.Now()
来源：http://hz.havefunace.top/gtkbaynifc.html

Ruby: Time.now
来源：http://hz.xylfe.cn/gtgjqacvtk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.kuanghao11.cn/gtzzbcnifg.html

[J02] 格式化输出
来源：http://hz.yuxming.cn/gtogjawcsx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shuidangran.top/gtxtvrpodd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cucudq.cn/gtyzpajpqr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shanyushiyangtech.top/gthietafef.html

TS:   d.toISOString()
来源：http://hz.fzhhl.top/gtyvpicqcp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yuxming.cn/gtobjdfhay.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.andypj.xyz/gtddetlbct.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jiagoushi.top/gtdsusylnr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gogol.net.cn/gtcttwirmb.html

[J03] 字符串解析为日期
来源：http://hz.jqgufenzy.top/gtqeqkeoap.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.aizwys.cn/gtvadvqfun.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hammf.cn/gtodkafczu.html

JS:   new Date("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtkdwpriqt.html


<!-- 参考信息 -->