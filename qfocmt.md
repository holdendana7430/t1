代发 wailian999

C#:   public User(string name) { Name = name; }
来源：http://hz.jyoumei.cn/gtkkhqewmq.html

[G03] 实例属性
来源：http://hz.pengpengdd.cyou/gtqdmzqafo.html

Py:   self.name = "x"
来源：http://hz.9152youxi.cn/gtepzbwmpn.html

PHP:  public string $name = "x";
来源：http://hz.hnqzz.top/gtlzxabnyu.html

JS:   this.name = "x";
来源：http://hz.ybcxt.top/gtwzknkokg.html

TS:   name: string = "x";
来源：http://hz.gotoacloud.top/gternxcsxt.html

Java: private String name;
来源：http://hz.52xcode.cn/gtdzqeymng.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shangyingyoupin.top/gtoauhyxft.html

Ruby: @name = "x"
来源：http://hz.feifeiyinyue.top/gtcxcussvv.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.316326.xyz/gtpogiztbx.html

[G04] 定义方法
来源：http://hz.tian-w.cn/gtbfqwgewj.html

Py:   def greet(self): return self.name
来源：http://hz.xziqi.cn/gttmwdtiyc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.pengpengdd.cyou/gttikrmmvo.html

JS:   greet() { return this.name; }
来源：http://hz.vqdsnc.cn/gtdejzarao.html

TS:   greet(): string { return this.name; }
来源：http://hz.cheryme.top/gtudarrjkv.html

Java: String greet() { return name; }
来源：http://hz.jqgufenzy.top/gtxklnrgyr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hnqzz.top/gtfvmwxwti.html

Ruby: def greet; @name; end
来源：http://hz.pycfn.com/gtkkmphmpc.html

C#:   public string Greet() => Name;
来源：http://hz.jqgufenzy.top/gtisexgecg.html

[G05] 继承
来源：http://hz.hywenlv.cn/gtgtiedkef.html

Py:   class Admin(User): pass
来源：http://hz.tian-w.cn/gtybazatyd.html

PHP:  class Admin extends User {}
来源：http://hz.52xcode.cn/gthnnfhtsa.html

JS:   class Admin extends User {}
来源：http://hz.zhongyouzk.top/gtffvqjoax.html

TS:   class Admin extends User {}
来源：http://hz.cucudq.cn/gtkpezrwjg.html

Java: class Admin extends User {}
来源：http://hz.ydzc1.top/gtmykpadri.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gaohongyu789.top/gtsodbpkzr.html

Ruby: class Admin < User; end
来源：http://hz.zycfv.cn/gtxihjasft.html

C#:   class Admin : User {}
来源：http://hz.yanxiufei.cn/gtjmjyotin.html

[G06] 重写方法
来源：http://hz.sufxvd.cn/gtyitegcsx.html

Py:   def greet(self): return "admin"
来源：http://hz.nanxinkj.top/gtpjrdwcak.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hongshengwenyu.top/gtfaoaewfh.html

JS:   greet() { return "admin"; }
来源：http://hz.hongshengwenyu.top/gtxhwrlpyi.html

TS:   greet(): string { return "admin"; }
来源：http://hz.dashuyun.cn/gtfsmsevse.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.wangdashe.top/gtatvldakx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sweek.top/gtaibuatgs.html

Ruby: def greet; "admin"; end
来源：http://hz.sysykeji.top/gtvoacbrmf.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhijiandao.cn/gtaunsgxou.html

[G07] 调用父类方法
来源：http://hz.jqgufenzy.top/gtwyvsqzym.html

Py:   super().greet()
来源：http://hz.ydzc1.top/gtwsatlven.html

PHP:  parent::greet();
来源：http://hz.jinqigfzy.top/gtetxauseb.html

JS:   super.greet();
来源：http://hz.yj20258.top/gtbfrhfylz.html

TS:   super.greet();
来源：http://hz.tianlin.xyz/gtpqdbxtqg.html

Java: super.greet();
来源：http://hz.mhx1999.top/gtpnkfnkrg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.havefunace.top/gtpjyllvlk.html

Ruby: super
来源：http://hz.yj20258888.top/gtduolethw.html

C#:   base.Greet();
来源：http://hz.andypj.xyz/gtumhrttvd.html

[G08] 静态方法与属性
来源：http://hz.hongshengwenyu.top/gtqhwgvgtj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.gotoacloud.top/gtpdhpyuen.html

PHP:  public static function f() {}
来源：http://hz.tanke756.top/gthuyffejo.html

JS:   static f() {}
来源：http://hz.hywenlv.cn/gtiypiucal.html

TS:   static f(): void {}
来源：http://hz.ydjk.org.cn/gtdvkyrnjq.html

Java: static void f() {}
来源：http://hz.cashguo.top/gthzerhaez.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jlsjyb.cn/gtntjvaczv.html

Ruby: def self.f; end
来源：http://hz.sysykeji.top/gtfmbiamfv.html

C#:   public static void F() {}
来源：http://hz.0kj1m.cn/gtsgyyddtl.html

[G09] 接口 / 抽象类
来源：http://hz.xingfuxueyuan.xyz/gtxbklemsp.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.feifeiyinyue.top/gtajrgdqdj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jinqigufen.top/gtdqiiewri.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.quarkkingdee.top/gtklnjwdwa.html

TS:   interface Shape { area(): number; }
来源：http://hz.dianchejie.cn/gtuwktwgki.html

Java: interface Shape { double area(); }
来源：http://hz.ydzc1.top/gtryclugft.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yuxming.cn/gtajgaxokw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ppjwa.cn/gtuxjeevad.html

C#:   interface IShape { double Area(); }
来源：http://hz.xuetiantiany.cn/gtyheypsgb.html

[G10] 访问控制
来源：http://hz.quarkkingdee.top/gthbmimflt.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.snrcjt.cn/gtrazamytq.html

PHP:  public / protected / private
来源：http://hz.dianchejie.cn/gtquurxxpi.html

JS:   #private 字段；其余公开
来源：http://hz.shanyushiyangkeji.top/gtbnkbzmdr.html

TS:   public / protected / private
来源：http://hz.wangdashe.top/gtcprvkijk.html

Java: public / protected / private / 默认包级
来源：http://hz.ywan-chungtsiang.top/gtjmxnchsz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ybcxt.top/gtchkodorm.html

Ruby: public / protected / private
来源：http://hz.guannengcc.top/gtcbhldwdz.html

C#:   public / protected / private / internal
来源：http://hz.ivvv.top/gtoxwyhyzt.html

[G11] getter / setter
来源：http://hz.shzxlz.cn/gtrzbiiqum.html

Py:   @property 与 @x.setter
来源：http://hz.kuanghao11.cn/gtlnytgqnx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.quarkkingdee.top/gtrradwdki.html

JS:   get name() { return this._name; }
来源：http://hz.yvedp.cn/gtqusyidrv.html

TS:   get name(): string { return this._name; }
来源：http://hz.haohaochexian.top/gtrmnddwrs.html

Java: public String getName() { return name; }
来源：http://hz.gzhubu.top/gtiatxrjqn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gzhubu.top/gtftpdcbyn.html

Ruby: attr_accessor :name
来源：http://hz.jinqigufen.top/gtubgxcina.html

C#:   public string Name { get; set; }
来源：http://hz.tanke756.top/gtadsedqwn.html

[G12] 对象转字符串
来源：http://hz.tian-w.cn/gtoefckueh.html

Py:   def __str__(self): return self.name
来源：http://hz.hysaishi.cn/gtcepepsxc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.316326.xyz/gtqerkhbbn.html

JS:   toString() { return this.name; }
来源：http://hz.jinqigufen.top/gtznkuctjd.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinyuanbaomall.cn/gtzqxtieuv.html

Java: @Override public String toString() { return name; }
来源：http://hz.shzxlz.cn/gthmqiiiji.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zdqjudy.top/gtxpsgupgr.html

Ruby: def to_s; @name; end
来源：http://hz.zhongyouzk.top/gtdpaqbrny.html

C#:   public override string ToString() => Name;
来源：http://hz.shanyushiyangkeji.top/gtnrcguiud.html

[G13] 判断对象类型
来源：http://hz.ydzc1.top/gtnvajrapj.html

Py:   isinstance(u, User)
来源：http://hz.wangdashe.top/gtjegamdbj.html

PHP:  $u instanceof User
来源：http://hz.shangyingyoupin.top/gtcvryaend.html

JS:   u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtsieqnytc.html

TS:   u instanceof User
来源：http://hz.yuxming.cn/gtlxvxwugt.html

Java: u instanceof User
来源：http://hz.yuxming.cn/gtnezijqxm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.xinyue.icu/gthudcvmmc.html

Ruby: u.is_a?(User)
来源：http://hz.yongpay.top/gttynoluav.html

C#:   u is User
来源：http://hz.svipenyu.cn/gtscaehczn.html

[G14] 数据类 / record
来源：http://hz.c1oappe.top/gtnnzkntlm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.svipenyu.cn/gtpjztolmq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhoulong.xyz/gtsmpjzjur.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hysaishi.cn/gtqxnxptkr.html

TS:   type User = { name: string; age: number };
来源：http://hz.0kj1m.cn/gteepmcuoz.html

Java: record User(String name, int age) {}
来源：http://hz.316326.xyz/gtpjwixbdt.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jiagoushi.top/gtppdwvgza.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cucudq.cn/gtuxwonplp.html

C#:   record User(string Name, int Age);
来源：http://hz.yuxming.cn/gtakermump.html

[G15] 枚举
来源：http://hz.c1oappe.top/gtmzwozsmw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.bjfxy.top/gthdjfqlpm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yonumen.top/gtmiupzkkw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.svipenyu.cn/gtdduwhgrr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.chenzaomai.com/gtwsdanawu.html

Java: enum Color { RED, GREEN }
来源：http://hz.ybcxt.top/gtdproplkz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.iojbl.cn/gtcmiqmqci.html

Ruby: Color = %i[red green].freeze
来源：http://hz.andypj.xyz/gtmcfrxdqd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.9152youxi.cn/gtvyqhaozk.html

[G16] 对象转数组 / 字典
来源：http://hz.quarkkingdee.top/gtyloakogp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.redwolf501.top/gtufhuvagz.html

PHP:  get_object_vars($obj);
来源：http://hz.meibo888.top/gtpibemwxc.html

JS:   Object.entries(obj)
来源：http://hz.meibo888.top/gtmqxcisze.html

TS:   Object.entries(obj)
来源：http://hz.jlsjyb.cn/gtcoalfjbk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.chenzaomai.com/gttbapfsxu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.aizwys.cn/gtqmrvblai.html

Ruby: obj.instance_variables
来源：http://hz.chenzaomai.com/gtldpsxdtx.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.gotoacloud.top/gtgpcbrhfx.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtseliqjog.html

H. 异常与错误处理
来源：http://hz.ywan-chungtsiang.top/gtyrahiaqw.html

================================================================================
来源：http://hz.zycfv.cn/gtekeenhzw.html

[H01] try / catch 基础
来源：http://hz.hongshengwenyu.top/gtggxngyfe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ydzc1.top/gteyihbiby.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.daxiang520.top/gtqatsosro.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.redwolf501.top/gttjpfudiu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shuidangran.top/gtzajrrebc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cqqwz.cn/gtyqoszvrp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gaohongyu789.top/gttkbhkvwz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hnxiangtu.top/gtywcerdyx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gotoacloud.top/gtfwzcnnmm.html

[H02] finally / ensure 收尾
来源：http://hz.gotoacloud.top/gttjkhbwwh.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hnxiangtu.top/gtmyjgvsyj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ydzc1.top/gtpkbptbeh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtlpbxhqyk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gtjygonktq.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.daxiang520.top/gtkohzexpo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yongpay.top/gtwqahhfuw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shanyushiyangkeji.top/gtuwjvibel.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtysbtjfbp.html

[H03] 主动抛出异常
来源：http://hz.yj202588.top/gtobbvbsgg.html

Py:   raise ValueError("错误信息")
来源：http://hz.jianghu66.top/gtixcewcpd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.haohaochexian.top/gtcqfcetro.html

JS:   throw new Error("错误信息");
来源：http://hz.tian-w.cn/gtnccvnefn.html

TS:   throw new Error("错误信息");
来源：http://hz.feifeiyinyue.top/gtetrskfes.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.fengsongda.top/gtnizienqi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.vqdsnc.cn/gtspsqifjv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nwbrower.top/gtcaophiax.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.daxiang520.top/gtycmlftlt.html

[H04] 自定义异常类型
来源：http://hz.zhengqikj.top/gtrcfzhxrn.html

Py:   class MyError(Exception): pass
来源：http://hz.gzhubu.top/gtwlivcvok.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shanyushiyangkeji.top/gttcdtxnro.html

JS:   class MyError extends Error {}
来源：http://hz.chenzaomai.com/gthegbdizj.html

TS:   class MyError extends Error {}
来源：http://hz.yangfankeji.com/gtptakhfal.html

Java: class MyException extends RuntimeException {}
来源：http://hz.9152youxi.cn/gtlxzlfvit.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ehwqpu.com/gtodjhobyx.html

Ruby: class MyError < StandardError; end
来源：http://hz.chenjidiqi.icu/gtftgrijdp.html

C#:   class MyException : Exception {}
来源：http://hz.zhaomingkeji.xyz/gtybazruug.html

[H05] 捕获特定类型
来源：http://hz.cheryme.top/gtrlvdbftb.html

Py:   except ValueError as e:
来源：http://hz.quarkkingdee.top/gtfriggefk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.andypj.xyz/gtybauzawc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cashguo.top/gtunwsiyro.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hywenlv.cn/gttmzxrbry.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shangyingyoupin.top/gtclixtqbf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jianghu66.top/gtmzjejjpz.html

Ruby: rescue ArgumentError => e
来源：http://hz.sweek.top/gttjuvocza.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.haohaochexian.top/gtiaxyysad.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zdqjudy.top/gtxrsnrrtb.html

Py:   value = d.get("k") or default
来源：http://hz.dashuyun.cn/gtmrorhjrx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhixingplan.top/gtwphqtitc.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sufxvd.cn/gtftgreosj.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.bjfxy.top/gthtfyjlzk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.0kj1m.cn/gtffsaeyvs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yonumen.top/gtjkngajhf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shanyushiyangtech.top/gtvlvpgbme.html

C#:   obj?.A?.B ?? default
来源：http://hz.dianchejie.cn/gtanhkurtt.html

[H07] 断言
来源：http://hz.wangshuangyany.cn/gtyzncogbs.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hammf.cn/gtxhmdsyxq.html

PHP:  assert($x > 0);
来源：http://hz.cdnleiting.top/gtdaitpnhf.html

JS:   console.assert(x > 0);
来源：http://hz.shuidangran.top/gtfndlqial.html

TS:   console.assert(x > 0);
来源：http://hz.yongpay.top/gtmtbusnek.html

Java: assert x > 0 : "必须为正";
来源：http://hz.gogol.net.cn/gtgnobuetr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ydzc1.top/gttkbzhsow.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.pycfn.com/gtnipzhjkw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.316326.xyz/gtvqgvhqia.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhongyouzk.top/gtsuwapkzc.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.wangshuangyany.cn/gtewbsiurg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xinyue.icu/gtpwgcfzcv.html

JS:   e.message;  e.stack
来源：http://hz.yj20258888.top/gtacsrxwfp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinyuanbaomall.cn/gtblabiuix.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yuanzhike.top/gtbnpvwehm.html

Go:   err.Error()
来源：http://hz.haohaochexian.top/gtwnqssuuy.html

Ruby: e.message;  e.backtrace
来源：http://hz.yj20258888.top/gtyuvxvhww.html

C#:   e.Message;  e.StackTrace
来源：http://hz.fengsongda.top/gtkbocksvr.html

[H09] 带错误码的异常
来源：http://hz.yj202588.top/gtwpwjyfle.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.316326.xyz/gtssukgmej.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.tianlin.xyz/gtfpapuvyu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.vqdsnc.cn/gtqobzohdq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.kuanghao11.cn/gtcveuhydj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.sweek.top/gtpfezrgly.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.gzhubu.top/gtonardeap.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xylfe.cn/gtledtfddx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jiagoushi.top/gtwugnndlp.html

[H10] 资源自动释放
来源：http://hz.xingfuxueyuan.xyz/gtgkckvlpq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhengqikj.top/gtkxaczhlq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yangfankeji.com/gtmneemjen.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.havefunace.top/gtbjihvcrz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.bjfxy.top/gtwwmwdvkd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hnqzz.top/gtlegodqqq.html

Go:   defer f.Close()
来源：http://hz.sxryk.cn/gthrmpmsge.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sweek.top/gthanxcmjb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ehwqpu.com/gtifmdqkld.html

================================================================================
来源：http://hz.cheryme.top/gtyhidhnje.html

I. 正则表达式
来源：http://hz.dashuyun.cn/gtrhxepxbc.html

================================================================================
来源：http://hz.9152youxi.cn/gtahbpyhxg.html

[I01] 判断是否匹配
来源：http://hz.havefunace.top/gtplaegrhm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.kuanghao11.cn/gtbtezppvi.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cucudq.cn/gtrwpdmopf.html

JS:   /\d+/.test(s)
来源：http://hz.ydzc1.top/gtaxuuxjmh.html

TS:   /\d+/.test(s)
来源：http://hz.chenjidiqi.icu/gtlcsqtuql.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cqqwz.cn/gtldzhgtwm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.svipenyu.cn/gtjicazvlk.html

Ruby: s.match?(/\d+/)
来源：http://hz.chenzaomai.com/gtwpkppkjo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.bjfxy.top/gtqqrqyjkn.html

[I02] 提取所有匹配
来源：http://hz.gaohongyu789.top/gthiidiikc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yongpay.top/gtggidcxtm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.sweek.top/gtdjbuyjar.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ydzc1.top/gtfxtclxii.html

TS:   s.match(/\d+/g)
来源：http://hz.xziqi.cn/gtmvvetfna.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.316326.xyz/gtyhpusjgm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.gogol.net.cn/gtytbcvyfq.html

Ruby: s.scan(/\d+/)
来源：http://hz.pengpengdd.cyou/gtnzobtdyn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.redwolf501.top/gtficqcpxg.html

[I03] 提取捕获分组
来源：http://hz.dianchejie.cn/gtuqgjapft.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.redwolf501.top/gtuqpgavzr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.cdnleiting.top/gtogqyqphf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cashguo.top/gtcscafhtg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.nanxinkj.top/gtrqidyjld.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.pycfn.com/gtbvylbmqs.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jqgfzy.top/gtvvfmgtar.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.daxiang520.top/gtmaonjvfh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ybcxt.top/gtlimahwoe.html

[I04] 正则替换
来源：http://hz.shzxlz.cn/gtyocenwui.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.fengsongda.top/gtniaetqqc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinqigfzy.top/gtljjgxssj.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.9152youxi.cn/gtalxgecwy.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.andypj.xyz/gtakjhbwyi.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.cdnleiting.top/gtplgqwurn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yj20258888.top/gtlzpqsfwt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ivvv.top/gteelywemg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.shzxlz.cn/gtvcoacffq.html

[I05] 按正则拆分
来源：http://hz.quarkkingdee.top/gtvviqeprb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jinqigufen.top/gtpeuwtyxz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cdnleiting.top/gtsakgzkta.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jyoumei.cn/gtsrldkggq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xinyue.icu/gtjrtszulu.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jianghu66.top/gttmikblqc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.daxiang520.top/gtzwdlotug.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.andypj.xyz/gtvfmzxlgu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yuxming.cn/gtecfemkhy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.0kj1m.cn/gtclrqezui.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhijiandao.cn/gtdhxpodkh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.pycfn.com/gtoxspehjy.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zycfv.cn/gtgaaflnnm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.havefunace.top/gtdhcjupmz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.fengsongda.top/gtbblbfxpm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zycfv.cn/gtysmtnhuz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.aizwys.cn/gttxsljepv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.svipenyu.cn/gtrsskaqii.html

[I07] 忽略大小写与多行模式
来源：http://hz.feifeiyinyue.top/gtyyuerqyq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhijiandao.cn/gthvviltor.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.pengpengdd.cyou/gtidelvsjq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.pycfn.com/gtoufzaibu.html

TS:   /error/gim
来源：http://hz.shangyingyoupin.top/gtllgeejsc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hfpthk.cn/gtyfjlihmv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jqgufenzy.top/gtntbwsoaj.html

Ruby: s.scan(/error/i)
来源：http://hz.gotoacloud.top/gtzkzeyecu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sweek.top/gtpxvhxkjk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cheryme.top/gtwkwtycbn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.wangshuangyany.cn/gtwdookqwc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.pycfn.com/gtlqiqvnpb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guowangkeji.top/gtfeczsapa.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.vqdsnc.cn/gtayezmspf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.gotoacloud.top/gttmycbisp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yonumen.top/gtsnagxzyo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jiagoushi.top/gtdrmcuspu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cucudq.cn/gtfqqdfucp.html

================================================================================
来源：http://hz.9152youxi.cn/gtandzqstf.html

J. 日期与时间
来源：http://hz.jiagoushi.top/gtuwhoircn.html

================================================================================
来源：http://hz.yuanzhike.top/gtdtjkdvbf.html

[J01] 获取当前时间
来源：http://hz.redwolf501.top/gtffnbthez.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ppjwa.cn/gtiotdzntb.html


<!-- 参考信息 -->