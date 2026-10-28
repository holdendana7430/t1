代发 wailian999

JS:   this.name = "x";
来源：http://hz.316326.xyz/gtdlspxnib.html

TS:   name: string = "x";
来源：http://hz.jyoumei.cn/gtqesodlaf.html

Java: private String name;
来源：http://hz.jqgufenzy.top/gtkjcxgmqf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jyoumei.cn/gtgrdedupt.html

Ruby: @name = "x"
来源：http://hz.tian-w.cn/gtmlindeeu.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.gogol.net.cn/gtzzhacrjp.html

[G04] 定义方法
来源：http://hz.feifeiyinyue.top/gtzclwimfx.html

Py:   def greet(self): return self.name
来源：http://hz.jinyuanbaomall.cn/gtcpvmhory.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.dashuyun.cn/gtpxaluxmb.html

JS:   greet() { return this.name; }
来源：http://hz.tian-w.cn/gtcgixxxrb.html

TS:   greet(): string { return this.name; }
来源：http://hz.ydjk.org.cn/gtkbhehhbj.html

Java: String greet() { return name; }
来源：http://hz.wangshuangyany.cn/gtuvfjkopk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.birdmap.top/gtsusdbaas.html

Ruby: def greet; @name; end
来源：http://hz.feifeiyinyue.top/gtqpfyraha.html

C#:   public string Greet() => Name;
来源：http://hz.nanxuanxn.top/gtsvdyamvj.html

[G05] 继承
来源：http://hz.ydjk.org.cn/gtpoprovhf.html

Py:   class Admin(User): pass
来源：http://hz.jlsjyb.cn/gtnqgadanw.html

PHP:  class Admin extends User {}
来源：http://hz.guowangkeji.top/gtdsvwemtk.html

JS:   class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtaurgjqox.html

TS:   class Admin extends User {}
来源：http://hz.dianchejie.cn/gtwldrinsz.html

Java: class Admin extends User {}
来源：http://hz.hnxiangtu.top/gtbgljkusb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hysaishi.cn/gtrftnvyga.html

Ruby: class Admin < User; end
来源：http://hz.vqdsnc.cn/gtgatojmuf.html

C#:   class Admin : User {}
来源：http://hz.zdqjudy.top/gthkmfjeie.html

[G06] 重写方法
来源：http://hz.sufxvd.cn/gtmnonpcsy.html

Py:   def greet(self): return "admin"
来源：http://hz.aibaodan.cn/gtcptlszrn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.hnqzz.top/gtcnexhhid.html

JS:   greet() { return "admin"; }
来源：http://hz.xinyue.icu/gtxheihsnb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yj202588.top/gtsjgmunrh.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zycfv.cn/gtathutgxs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yvedp.cn/gtmezyunpg.html

Ruby: def greet; "admin"; end
来源：http://hz.redwolf501.top/gtfywxwqso.html

C#:   public override string Greet() => "admin";
来源：http://hz.xuanzx.com/gtrjefxoet.html

[G07] 调用父类方法
来源：http://hz.wangshuangyany.cn/gtmmguurmn.html

Py:   super().greet()
来源：http://hz.birdmap.top/gtlndfwrhf.html

PHP:  parent::greet();
来源：http://hz.52xcode.cn/gtxjxkkhsz.html

JS:   super.greet();
来源：http://hz.hammf.cn/gtgtydymly.html

TS:   super.greet();
来源：http://hz.sysykeji.top/gtwhezgxcr.html

Java: super.greet();
来源：http://hz.yongpay.top/gtgunulgwe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xziqi.cn/gtgmkgxfbd.html

Ruby: super
来源：http://hz.hywenlv.cn/gtrztrigdw.html

C#:   base.Greet();
来源：http://hz.dianchejie.cn/gtqhxczsdd.html

[G08] 静态方法与属性
来源：http://hz.nwbrower.top/gtdggieswx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hnqzz.top/gtlidlkzqo.html

PHP:  public static function f() {}
来源：http://hz.xuetiantiany.cn/gtyplkhthn.html

JS:   static f() {}
来源：http://hz.tian-w.cn/gtcgylrols.html

TS:   static f(): void {}
来源：http://hz.havefunace.top/gtydwxdgio.html

Java: static void f() {}
来源：http://hz.sufxvd.cn/gtbivdmjrx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.xinyue.icu/gtdkupgjzo.html

Ruby: def self.f; end
来源：http://hz.xylfe.cn/gtdaktpxkk.html

C#:   public static void F() {}
来源：http://hz.smart0.xyz/gtgownoiyk.html

[G09] 接口 / 抽象类
来源：http://hz.cashguo.top/gtncarzvnb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xuanzx.com/gtbejawbzf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hnqzz.top/gtoojcmlzy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.redwolf501.top/gttnnjjapj.html

TS:   interface Shape { area(): number; }
来源：http://hz.chenjidiqi.icu/gtqaxjyjyz.html

Java: interface Shape { double area(); }
来源：http://hz.jinyuanbaomall.cn/gtsrykvcek.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.daria6918.cn/gtccwdyjcd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.shanyushiyangkeji.top/gtjinstsib.html

C#:   interface IShape { double Area(); }
来源：http://hz.fzhhl.top/gtfyilnqxc.html

[G10] 访问控制
来源：http://hz.jinqigufen.top/gtidsccvzr.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.dianchejie.cn/gtlyqhojfm.html

PHP:  public / protected / private
来源：http://hz.yanxiufei.cn/gtjrbcxkxj.html

JS:   #private 字段；其余公开
来源：http://hz.yvedp.cn/gtborsnvem.html

TS:   public / protected / private
来源：http://hz.yueranfly.top/gtgifgebkx.html

Java: public / protected / private / 默认包级
来源：http://hz.vqdsnc.cn/gtyjoeoyrb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sweek.top/gtomvkxfmu.html

Ruby: public / protected / private
来源：http://hz.tian-w.cn/gtfyjspypw.html

C#:   public / protected / private / internal
来源：http://hz.chenlongwang.top/gtvykwjfcr.html

[G11] getter / setter
来源：http://hz.jinghuilouyu.cn/gtuyagmacq.html

Py:   @property 与 @x.setter
来源：http://hz.yj202588.top/gtunahcwjw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhaomingkeji.xyz/gttyzmlktu.html

JS:   get name() { return this._name; }
来源：http://hz.0kj1m.cn/gtwclrspqo.html

TS:   get name(): string { return this._name; }
来源：http://hz.tanke756.top/gtyfjnvbxj.html

Java: public String getName() { return name; }
来源：http://hz.tianlin.xyz/gtjokujgue.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hammf.cn/gtmexeumqd.html

Ruby: attr_accessor :name
来源：http://hz.xziqi.cn/gtruhlovfd.html

C#:   public string Name { get; set; }
来源：http://hz.dianchejie.cn/gtrprglgsx.html

[G12] 对象转字符串
来源：http://hz.zhijiandao.cn/gtevtqcyai.html

Py:   def __str__(self): return self.name
来源：http://hz.pycfn.com/gtbhhgadvv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.pycfn.com/gtyrixgvlg.html

JS:   toString() { return this.name; }
来源：http://hz.dashuyun.cn/gtsauiqqau.html

TS:   toString(): string { return this.name; }
来源：http://hz.jqgfzy.top/gtvydruvrd.html

Java: @Override public String toString() { return name; }
来源：http://hz.fzhhl.top/gtjsnnnzdf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.wangdashe.top/gthgmqenpr.html

Ruby: def to_s; @name; end
来源：http://hz.tanke756.top/gtafonahxw.html

C#:   public override string ToString() => Name;
来源：http://hz.gaohongyu789.top/gtabvazidu.html

[G13] 判断对象类型
来源：http://hz.svipenyu.cn/gteipjdyeh.html

Py:   isinstance(u, User)
来源：http://hz.shanyushiyangkeji.top/gtdvsefmbl.html

PHP:  $u instanceof User
来源：http://hz.havefunace.top/gtcdxwxcpa.html

JS:   u instanceof User
来源：http://hz.yvedp.cn/gtowtgdfjr.html

TS:   u instanceof User
来源：http://hz.hnqzz.top/gtxdcnyglb.html

Java: u instanceof User
来源：http://hz.zhiwuduotai.top/gtgyzevysx.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jqgfzy.top/gthjnoidgf.html

Ruby: u.is_a?(User)
来源：http://hz.birdmap.top/gtrgwufjqt.html

C#:   u is User
来源：http://hz.jinyuanbaomall.cn/gtihzciimr.html

[G14] 数据类 / record
来源：http://hz.hysaishi.cn/gtvaaepnie.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gzhubu.top/gtpfwamdgt.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.iojbl.cn/gtywmcawgc.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.mhx1999.top/gtvckkwyql.html

TS:   type User = { name: string; age: number };
来源：http://hz.guannengcc.top/gtjilvzwnc.html

Java: record User(String name, int age) {}
来源：http://hz.nwbrower.top/gtqxsrfdsr.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jyoumei.cn/gtqrxihckq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yj20258.top/gtvzpqutyi.html

C#:   record User(string Name, int Age);
来源：http://hz.jianghu66.top/gtbftibkoq.html

[G15] 枚举
来源：http://hz.shzxlz.cn/gtzxjpizpk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yj20258888.top/gtxpnkxaxa.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ydjk.org.cn/gtoxblpbwm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.gogol.net.cn/gtszkvdyys.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tianlin.xyz/gtciwvobmk.html

Java: enum Color { RED, GREEN }
来源：http://hz.gotoacloud.top/gtncoivjfp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xuetiantiany.cn/gtgwjbagpe.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinghuilouyu.cn/gtvppjvlsj.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.havefunace.top/gtognbhdsu.html

[G16] 对象转数组 / 字典
来源：http://hz.shanyushiyangtech.top/gtagatxanp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yanxiufei.cn/gtwdpddjws.html

PHP:  get_object_vars($obj);
来源：http://hz.sysykeji.top/gtgsgpoefn.html

JS:   Object.entries(obj)
来源：http://hz.fzhhl.top/gtpnknjpvv.html

TS:   Object.entries(obj)
来源：http://hz.cqqwz.cn/gtyvyqlpbc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.c1oappe.top/gtophwvfkv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shangyingyoupin.top/gtikkuhdvd.html

Ruby: obj.instance_variables
来源：http://hz.nanxuanxn.top/gtmcgksuoy.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yj20258888.top/gtogiwiqys.html

================================================================================
来源：http://hz.hywenlv.cn/gtukorqnxd.html

H. 异常与错误处理
来源：http://hz.snrcjt.cn/gttzcvxppz.html

================================================================================
来源：http://hz.yanxiufei.cn/gtkpycrdel.html

[H01] try / catch 基础
来源：http://hz.9152youxi.cn/gthhrofztj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.mhx1999.top/gtsfsltclr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.9152youxi.cn/gtfdcyctke.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gogol.net.cn/gtnaovfzxz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hysaishi.cn/gtmvuiwbfg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.iojbl.cn/gtzdirvgjn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gaohongyu789.top/gtvbhtgqje.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yj202588.top/gtzcjreiwj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hnqzz.top/gtjrjxldmm.html

[H02] finally / ensure 收尾
来源：http://hz.sxryk.cn/gtsartwwxz.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shanyushiyangtech.top/gtxpqqozbc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cqqwz.cn/gtzbzwpwmd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtlzfoieaf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gtosuxeahi.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gtjquysnxh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hfpthk.cn/gtumwgyxeq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.aizwys.cn/gtxcicgpfi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.andypj.xyz/gtozcoqulo.html

[H03] 主动抛出异常
来源：http://hz.nwbrower.top/gtmzavsorz.html

Py:   raise ValueError("错误信息")
来源：http://hz.birdmap.top/gtnibatfnf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yj20258888.top/gtjrtfljgn.html

JS:   throw new Error("错误信息");
来源：http://hz.sweek.top/gtktsdkhdd.html

TS:   throw new Error("错误信息");
来源：http://hz.fengsongda.top/gtduhwnknh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtdpmiqsec.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.haohaochexian.top/gtwdegbogj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jqgfzy.top/gtvtelzjpg.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hnqzz.top/gtedxbtgju.html

[H04] 自定义异常类型
来源：http://hz.mhx1999.top/gttnzywnzz.html

Py:   class MyError(Exception): pass
来源：http://hz.jinqigufen.top/gtnbjercqe.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.redwolf501.top/gtokptiqvw.html

JS:   class MyError extends Error {}
来源：http://hz.bjfxy.top/gtfccuccbn.html

TS:   class MyError extends Error {}
来源：http://hz.feifeiyinyue.top/gtwajwfvnx.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ivvv.top/gtsqtmfpkv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yonumen.top/gthrtyqgdt.html

Ruby: class MyError < StandardError; end
来源：http://hz.jinghuilouyu.cn/gtujzzboxw.html

C#:   class MyException : Exception {}
来源：http://hz.zhiwuduotai.top/gtfpvqzzeq.html

[H05] 捕获特定类型
来源：http://hz.zhaomingkeji.xyz/gtvpevzkcw.html

Py:   except ValueError as e:
来源：http://hz.xuetiantiany.cn/gtqhuspspj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.dashuyun.cn/gtwpgfejmw.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ppjwa.cn/gtmbodyzyt.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.dashuyun.cn/gttvxewdkk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.chenlongwang.top/gtcixniruz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinqigfzy.top/gtonlungpv.html

Ruby: rescue ArgumentError => e
来源：http://hz.daxiang520.top/gtxawlsgjx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sufxvd.cn/gtaxyhqdaa.html

[H06] 可选值 / 空值安全访问
来源：http://hz.0kj1m.cn/gtabtmjooy.html

Py:   value = d.get("k") or default
来源：http://hz.aizwys.cn/gtmdcjstlk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hammf.cn/gtkdpiexps.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.fzhhl.top/gtcvfwkrkt.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.andypj.xyz/gtkyqmqrst.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.wangdashe.top/gtcotqllnn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.wangdashe.top/gtfvksyftz.html

Ruby: d&.dig(:a, :b)
来源：http://hz.meibo888.top/gtgovkmdeh.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhongyouzk.top/gtquiptxhw.html

[H07] 断言
来源：http://hz.yj20258.top/gtoficjrwm.html

Py:   assert x > 0, "必须为正"
来源：http://hz.aizwys.cn/gtcntpfezx.html

PHP:  assert($x > 0);
来源：http://hz.nanxuanxn.top/gttxdhsuqr.html

JS:   console.assert(x > 0);
来源：http://hz.daria6918.cn/gtcssgftqs.html

TS:   console.assert(x > 0);
来源：http://hz.sweek.top/gtkgiwjjdz.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yj20258888.top/gtrimzfenb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhiwuduotai.top/gttntxutpt.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ehwqpu.com/gtbltxdkuv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ybcxt.top/gtubplieou.html

[H08] 获取错误信息与堆栈
来源：http://hz.xingfuxueyuan.xyz/gticwsoghy.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.aibaodan.cn/gtwjvnssxo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gotoacloud.top/gtyupimcaw.html

JS:   e.message;  e.stack
来源：http://hz.guowangkeji.top/gtgwmdjcgs.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hnqzz.top/gtelluiaqj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yangfankeji.com/gttppqejfw.html

Go:   err.Error()
来源：http://hz.xuanzx.com/gtulkcfbzc.html

Ruby: e.message;  e.backtrace
来源：http://hz.jianghu66.top/gtuycpitan.html

C#:   e.Message;  e.StackTrace
来源：http://hz.guannengcc.top/gtmmgtiieh.html

[H09] 带错误码的异常
来源：http://hz.zhoulong.xyz/gtxmbcftbz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.smart0.xyz/gtodrbohzm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jianghu66.top/gtwkscvvqj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.feifeiyinyue.top/gtljtmdydr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.redwolf501.top/gtvphtmoqo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.aizwys.cn/gtuwqvzskj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.0kj1m.cn/gtmcwtsksn.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xingfuxueyuan.xyz/gtroxqqxey.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hywenlv.cn/gtpejwppkx.html

[H10] 资源自动释放
来源：http://hz.daria6918.cn/gtzdxahbgn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.dianchejie.cn/gtoqagyzgc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.tianlin.xyz/gtfxqvwxjs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.andypj.xyz/gtnflhofan.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.birdmap.top/gtligxtaxd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yuanzhike.top/gtkturifvx.html

Go:   defer f.Close()
来源：http://hz.zhijiandao.cn/gtqxpkklpz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cashguo.top/gtlnikaznu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.feifeiyinyue.top/gtldtjdwdr.html

================================================================================
来源：http://hz.jqgufenzy.top/gtenjnewhv.html

I. 正则表达式
来源：http://hz.haohaochexian.top/gtmfsczbnw.html

================================================================================
来源：http://hz.sxryk.cn/gtnttopodz.html

[I01] 判断是否匹配
来源：http://hz.c1oappe.top/gtadiikwsg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.chenzaomai.com/gtyoxbaibw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.nwbrower.top/gtwzvvchcm.html

JS:   /\d+/.test(s)
来源：http://hz.hysaishi.cn/gttyvfjwqa.html

TS:   /\d+/.test(s)
来源：http://hz.pengpengdd.cyou/gtbrebbcap.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.kuanghao11.cn/gtdpxvkagc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cdnleiting.top/gtrfgbrksv.html

Ruby: s.match?(/\d+/)
来源：http://hz.gzhubu.top/gtelepsuex.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jqgufenzy.top/gtjxwtkqwj.html

[I02] 提取所有匹配
来源：http://hz.hysaishi.cn/gtvbhaavly.html

Py:   re.findall(r"\d+", s)
来源：http://hz.bjfxy.top/gtzivmzxuv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hnqzz.top/gthnfxdbnp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xylfe.cn/gthfthmepf.html

TS:   s.match(/\d+/g)
来源：http://hz.iojbl.cn/gtwdkftshb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.bjfxy.top/gtykcxtnbf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xylfe.cn/gtkxcnafng.html

Ruby: s.scan(/\d+/)
来源：http://hz.fengsongda.top/gtheodxbsk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.tianlin.xyz/gtktkpskxd.html

[I03] 提取捕获分组
来源：http://hz.xziqi.cn/gtiuvhxsiz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.kuanghao11.cn/gttgfoiqxo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yuxming.cn/gtcmrpggyj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gzhubu.top/gteuujcgvh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.gaohongyu789.top/gtvrhyrthl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yangfankeji.com/gtdiptzahy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.guannengcc.top/gtwhcswrvq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jqgufenzy.top/gttefxpcll.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yj20258.top/gtttzkqgda.html

[I04] 正则替换
来源：http://hz.yuxming.cn/gtokhyrzej.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.52xcode.cn/gtcuwlswfg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.wangshuangyany.cn/gtnbzsbdbn.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cucudq.cn/gtmaffetiu.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yuanzhike.top/gtrrqfwofj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ybcxt.top/gtcsglnflh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhijiandao.cn/gtbagtqamb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ppjwa.cn/gtxtgwvcxr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zycfv.cn/gtcwqdhfcj.html

[I05] 按正则拆分
来源：http://hz.pycfn.com/gtgcsaarga.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yangfankeji.com/gtqtvglnmo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.havefunace.top/gtojinfdwj.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.wangshuangyany.cn/gtgeigvoql.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tianlin.xyz/gtjnbezaey.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shzxlz.cn/gtzkmvhdqw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhoulong.xyz/gttbjdqwhc.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yvedp.cn/gtateppceu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jiagoushi.top/gtzxjpmbpv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jlsjyb.cn/gtycapvtwt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cucudq.cn/gtxzmksdsy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.smart0.xyz/gtezwhkcpj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cashguo.top/gtzwfjqdfn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.feifeiyinyue.top/gtitdephwu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhijiandao.cn/gtvtqaqufb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhiwuduotai.top/gtehvhjknw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.meibo888.top/gtbllgvttz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.vqdsnc.cn/gttxzksrja.html

[I07] 忽略大小写与多行模式
来源：http://hz.ppjwa.cn/gtxdqtgjak.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.fengsongda.top/gtcbjikdcp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.daria6918.cn/gtllrwatoq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ydzc1.top/gtkpvoelir.html

TS:   /error/gim
来源：http://hz.jqgfzy.top/gtsfxmjqkl.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.daria6918.cn/gtwxczusbu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinghuilouyu.cn/gtdtoeraim.html

Ruby: s.scan(/error/i)
来源：http://hz.gotoacloud.top/gthfaewpgs.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinghuilouyu.cn/gtqsxysris.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yangfankeji.com/gtisukjxro.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ppjwa.cn/gtwirkiybn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hnqzz.top/gtozrdwgat.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.daxiang520.top/gtokexough.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.feifeiyinyue.top/gtfgbekhpw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhixingplan.top/gtyglvdoba.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cashguo.top/gtqyrwnbjw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.bjfxy.top/gtbmuegwdu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.bjfxy.top/gtdkkuddzg.html

================================================================================
来源：http://hz.gaohongyu789.top/gtmyyrzuxu.html

J. 日期与时间
来源：http://hz.zdqjudy.top/gtrjyszyhp.html

================================================================================
来源：http://hz.shzxlz.cn/gtomlvqxuu.html

[J01] 获取当前时间
来源：http://hz.xziqi.cn/gtimrdqysg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.tian-w.cn/gtakgmvchs.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xuanzx.com/gtmwjvoovc.html

JS:   new Date();  Date.now()
来源：http://hz.yuxming.cn/gtprqhgcro.html

TS:   new Date();  Date.now()
来源：http://hz.sxryk.cn/gttbyxfrxd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.daria6918.cn/gtxjwwduhh.html


<!-- 参考信息 -->