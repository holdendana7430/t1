代发 wailian999

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenlongwang.top/gtvtpqesux.html

Ruby: def greet; @name; end
来源：http://hz.yj202588.top/gteevjedtx.html

C#:   public string Greet() => Name;
来源：http://hz.jinghuilouyu.cn/gtlitxwrge.html

[G05] 继承
来源：http://hz.wangdashe.top/gtjmbdbwqi.html

Py:   class Admin(User): pass
来源：http://hz.jiagoushi.top/gtwhpdhesq.html

PHP:  class Admin extends User {}
来源：http://hz.cqqwz.cn/gtbztunpik.html

JS:   class Admin extends User {}
来源：http://hz.chenzaomai.com/gtabcpnbzg.html

TS:   class Admin extends User {}
来源：http://hz.wangdashe.top/gtqssoavrf.html

Java: class Admin extends User {}
来源：http://hz.sxryk.cn/gtopevbmwr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.vqdsnc.cn/gtgfpfxkhn.html

Ruby: class Admin < User; end
来源：http://hz.shangyingyoupin.top/gtxidqsxpj.html

C#:   class Admin : User {}
来源：http://hz.sysykeji.top/gthmukfwxa.html

[G06] 重写方法
来源：http://hz.havefunace.top/gtctkidckl.html

Py:   def greet(self): return "admin"
来源：http://hz.andypj.xyz/gtdqjautrc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.pycfn.com/gtundqomkg.html

JS:   greet() { return "admin"; }
来源：http://hz.andypj.xyz/gtqhxzfluz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.tian-w.cn/gtfbbprkii.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ivvv.top/gtqnspezkw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shanyushiyangkeji.top/gtflldoxrb.html

Ruby: def greet; "admin"; end
来源：http://hz.mhx1999.top/gtorjwuwdc.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhixingplan.top/gtqfrgmquu.html

[G07] 调用父类方法
来源：http://hz.0kj1m.cn/gtpojlunjz.html

Py:   super().greet()
来源：http://hz.yuxming.cn/gtqsorbirp.html

PHP:  parent::greet();
来源：http://hz.bjfxy.top/gtymmwbdvt.html

JS:   super.greet();
来源：http://hz.0kj1m.cn/gthdzcwiio.html

TS:   super.greet();
来源：http://hz.jinyuanbaomall.cn/gtjgaayeea.html

Java: super.greet();
来源：http://hz.kuanghao11.cn/gtxyimjbwa.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinqigufen.top/gtvwhuqhgo.html

Ruby: super
来源：http://hz.jinqigufen.top/gtygwbimmc.html

C#:   base.Greet();
来源：http://hz.316326.xyz/gtdghuxfii.html

[G08] 静态方法与属性
来源：http://hz.jinghuilouyu.cn/gtvconoeya.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xingfuxueyuan.xyz/gtluoejavs.html

PHP:  public static function f() {}
来源：http://hz.jinyuanbaomall.cn/gtqqmjydzf.html

JS:   static f() {}
来源：http://hz.jinqigfzy.top/gtkvanbdog.html

TS:   static f(): void {}
来源：http://hz.shzxlz.cn/gtdowlbolr.html

Java: static void f() {}
来源：http://hz.shzxlz.cn/gtiohxunjw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.9152youxi.cn/gtpqggyjlx.html

Ruby: def self.f; end
来源：http://hz.hywenlv.cn/gtqcznnyik.html

C#:   public static void F() {}
来源：http://hz.shanyushiyangkeji.top/gtkbqyrfrf.html

[G09] 接口 / 抽象类
来源：http://hz.havefunace.top/gtawcdagqt.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhengqikj.top/gtihhtibqk.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zhongyouzk.top/gtqbxsjkts.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.iojbl.cn/gtwytveonj.html

TS:   interface Shape { area(): number; }
来源：http://hz.ybcxt.top/gtafmoizne.html

Java: interface Shape { double area(); }
来源：http://hz.sxryk.cn/gtdyfldrdo.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xingfuxueyuan.xyz/gtwduacnja.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yvedp.cn/gtnvqhjfep.html

C#:   interface IShape { double Area(); }
来源：http://hz.sufxvd.cn/gtrztuotmx.html

[G10] 访问控制
来源：http://hz.52xcode.cn/gtjgzdcfse.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hongshengwenyu.top/gtwxzkefcj.html

PHP:  public / protected / private
来源：http://hz.birdmap.top/gtpdvruisi.html

JS:   #private 字段；其余公开
来源：http://hz.daria6918.cn/gtejlpzqtx.html

TS:   public / protected / private
来源：http://hz.jinghuilouyu.cn/gtshqpzfoj.html

Java: public / protected / private / 默认包级
来源：http://hz.sufxvd.cn/gttpfyxald.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.chenlongwang.top/gteskixwpq.html

Ruby: public / protected / private
来源：http://hz.zhaomingkeji.xyz/gtbysowlwc.html

C#:   public / protected / private / internal
来源：http://hz.xinyue.icu/gtkahylocm.html

[G11] getter / setter
来源：http://hz.snrcjt.cn/gtmzbknlkl.html

Py:   @property 与 @x.setter
来源：http://hz.smart0.xyz/gtacuktjva.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtpugdmtey.html

JS:   get name() { return this._name; }
来源：http://hz.andypj.xyz/gttzecymzw.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhoulong.xyz/gtfwudbvju.html

Java: public String getName() { return name; }
来源：http://hz.yuanzhike.top/gtwlzwrjcl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yongpay.top/gtwjssvrge.html

Ruby: attr_accessor :name
来源：http://hz.pycfn.com/gtxhoruzfu.html

C#:   public string Name { get; set; }
来源：http://hz.shuidangran.top/gtlstsmumo.html

[G12] 对象转字符串
来源：http://hz.cucudq.cn/gtcybcmhao.html

Py:   def __str__(self): return self.name
来源：http://hz.shzxlz.cn/gtzrjwlxgh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jqgfzy.top/gtrvilrucb.html

JS:   toString() { return this.name; }
来源：http://hz.cqqwz.cn/gtilaaizyj.html

TS:   toString(): string { return this.name; }
来源：http://hz.shangyingyoupin.top/gtzndimlzo.html

Java: @Override public String toString() { return name; }
来源：http://hz.vqdsnc.cn/gtsfctabgm.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.chenjidiqi.icu/gtyqmgpdqn.html

Ruby: def to_s; @name; end
来源：http://hz.nwbrower.top/gtoaawvmpr.html

C#:   public override string ToString() => Name;
来源：http://hz.chenlongwang.top/gtrtfpswdc.html

[G13] 判断对象类型
来源：http://hz.ywan-chungtsiang.top/gtsxtlhkym.html

Py:   isinstance(u, User)
来源：http://hz.yongpay.top/gttsybjdvb.html

PHP:  $u instanceof User
来源：http://hz.chenzaomai.com/gtmcxvrhlt.html

JS:   u instanceof User
来源：http://hz.hysaishi.cn/gtdnzwneaw.html

TS:   u instanceof User
来源：http://hz.jianghu66.top/gtesiepwsf.html

Java: u instanceof User
来源：http://hz.hnxiangtu.top/gtnuyaolhd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhiwuduotai.top/gtqjdpoxyf.html

Ruby: u.is_a?(User)
来源：http://hz.bjfxy.top/gtgxwbwzts.html

C#:   u is User
来源：http://hz.ppjwa.cn/gtzkpjgvsg.html

[G14] 数据类 / record
来源：http://hz.chenzaomai.com/gtjuchcitd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.gotoacloud.top/gtonvddwri.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.pycfn.com/gtrbrylbtz.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yangfankeji.com/gttnpvkqzh.html

TS:   type User = { name: string; age: number };
来源：http://hz.zycfv.cn/gthrjsoaxz.html

Java: record User(String name, int age) {}
来源：http://hz.zhoulong.xyz/gtordajvsd.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yongpay.top/gtdrmtyxaj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.nwbrower.top/gtjggabpqk.html

C#:   record User(string Name, int Age);
来源：http://hz.shuidangran.top/gtyonqcqge.html

[G15] 枚举
来源：http://hz.jqgufenzy.top/gtodtjiqcw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.nwbrower.top/gtrdpshsnv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.aizwys.cn/gtrpvrdcnv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shanyushiyangtech.top/gtbdafeunm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xingfuxueyuan.xyz/gtjxtpcwpe.html

Java: enum Color { RED, GREEN }
来源：http://hz.haohaochexian.top/gtondevxjq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.9152youxi.cn/gtgmddpnac.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hysaishi.cn/gtoawheibn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daria6918.cn/gttmtbrltf.html

[G16] 对象转数组 / 字典
来源：http://hz.aizwys.cn/gtfqfchkdd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.tianlin.xyz/gtprahzykk.html

PHP:  get_object_vars($obj);
来源：http://hz.sufxvd.cn/gtntcjhrxq.html

JS:   Object.entries(obj)
来源：http://hz.zhixingplan.top/gtzgkyzxyu.html

TS:   Object.entries(obj)
来源：http://hz.xinyue.icu/gtvyvuxloq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ybcxt.top/gtvyiccnlw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jinghuilouyu.cn/gtdmzxqdbk.html

Ruby: obj.instance_variables
来源：http://hz.yj20258888.top/gtqcbhtxel.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.meibo888.top/gtahvuvwoj.html

================================================================================
来源：http://hz.cdnleiting.top/gtasunvfjf.html

H. 异常与错误处理
来源：http://hz.feifeiyinyue.top/gteqkkodtt.html

================================================================================
来源：http://hz.nwbrower.top/gtsxvalvus.html

[H01] try / catch 基础
来源：http://hz.zhoulong.xyz/gtdmljjtml.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yuanzhike.top/gtbejpnmud.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.smart0.xyz/gtzubpcjun.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.dianchejie.cn/gtatapumle.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hnqzz.top/gtsziukdkv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jqgfzy.top/gtigrrkntm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.sysykeji.top/gtbanttcey.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cdnleiting.top/gtfibxwcjd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.chenzaomai.com/gtjbbesgdx.html

[H02] finally / ensure 收尾
来源：http://hz.yj20258888.top/gtjiumiyvl.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ehwqpu.com/gtmsmcdspx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.52xcode.cn/gtcnoceqel.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtrchmttzo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gthmjurvik.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtfitpdsqi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.snrcjt.cn/gtadkdavpc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jiagoushi.top/gtnxtcuida.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.chenlongwang.top/gthloohtow.html

[H03] 主动抛出异常
来源：http://hz.chenjidiqi.icu/gttdoiuzjh.html

Py:   raise ValueError("错误信息")
来源：http://hz.yuanzhike.top/gtmarpmrwq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gtuyxmstib.html

JS:   throw new Error("错误信息");
来源：http://hz.tian-w.cn/gtjbmjsgwl.html

TS:   throw new Error("错误信息");
来源：http://hz.yj202588.top/gtnkicprqk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.fzhhl.top/gtfmgnbtyf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhoulong.xyz/gttqphulcr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hywenlv.cn/gtjjapodde.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cheryme.top/gtfgrxlwqh.html

[H04] 自定义异常类型
来源：http://hz.jiagoushi.top/gtgfhegslr.html

Py:   class MyError(Exception): pass
来源：http://hz.tanke756.top/gtuubhspws.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhengqikj.top/gthhxdsyek.html

JS:   class MyError extends Error {}
来源：http://hz.jqgufenzy.top/gtfobshabs.html

TS:   class MyError extends Error {}
来源：http://hz.kuanghao11.cn/gtgtkyuvrx.html

Java: class MyException extends RuntimeException {}
来源：http://hz.fzhhl.top/gtvrwiwmdd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hfpthk.cn/gtuojmtjow.html

Ruby: class MyError < StandardError; end
来源：http://hz.aibaodan.cn/gtvlgalmjl.html

C#:   class MyException : Exception {}
来源：http://hz.jianghu66.top/gtucheypev.html

[H05] 捕获特定类型
来源：http://hz.fengsongda.top/gtvwmdnxxg.html

Py:   except ValueError as e:
来源：http://hz.cheryme.top/gtiwkgkwkx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.dianchejie.cn/gtwfowcjoo.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jiagoushi.top/gtnljvzmxq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.birdmap.top/gtiwddmiyd.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ehwqpu.com/gtdxunchxo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ybcxt.top/gttcwbcdsb.html

Ruby: rescue ArgumentError => e
来源：http://hz.haohaochexian.top/gtaitfhopb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhijiandao.cn/gtudlhkhlj.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yj202588.top/gtryjtdign.html

Py:   value = d.get("k") or default
来源：http://hz.ydzc1.top/gtrthktpjv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jqgfzy.top/gtdvbpjyhf.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shanyushiyangtech.top/gtoxhodspq.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.gogol.net.cn/gtezlvjbpp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhiwuduotai.top/gtsdondvjl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.dashuyun.cn/gtezyhztal.html

Ruby: d&.dig(:a, :b)
来源：http://hz.sufxvd.cn/gtfuhskkij.html

C#:   obj?.A?.B ?? default
来源：http://hz.cucudq.cn/gtmooezdvj.html

[H07] 断言
来源：http://hz.gogol.net.cn/gtmdkbyppq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.316326.xyz/gtqxvlffkm.html

PHP:  assert($x > 0);
来源：http://hz.yj202588.top/gtkufcxqpa.html

JS:   console.assert(x > 0);
来源：http://hz.cashguo.top/gtmneisyfj.html

TS:   console.assert(x > 0);
来源：http://hz.sysykeji.top/gtrqcfdcze.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sweek.top/gtedokmdsv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yj202588.top/gtilequyjg.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.nanxuanxn.top/gtmxocgmpf.html

C#:   Debug.Assert(x > 0);
来源：http://hz.gogol.net.cn/gtypstrxlo.html

[H08] 获取错误信息与堆栈
来源：http://hz.gaohongyu789.top/gtiaxlhndz.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ehwqpu.com/gtkxtqxwmc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.guowangkeji.top/gtbwfcceyn.html

JS:   e.message;  e.stack
来源：http://hz.dianchejie.cn/gtgntscuwc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.redwolf501.top/gtdgwmswcu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.dianchejie.cn/gtbjyzuydp.html

Go:   err.Error()
来源：http://hz.nanxinkj.top/gtsbcwxdck.html

Ruby: e.message;  e.backtrace
来源：http://hz.ppjwa.cn/gtsjnzonfy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.aizwys.cn/gtzqanfufa.html

[H09] 带错误码的异常
来源：http://hz.jiagoushi.top/gtvuucnnlc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.0kj1m.cn/gtazirhdmk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.pengpengdd.cyou/gtvgdnsbip.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ppjwa.cn/gtxqvftvsj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cashguo.top/gtkeseojdv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yonumen.top/gtqpfybslc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.andypj.xyz/gtwsbrflys.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.wangshuangyany.cn/gteijbpnti.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhixingplan.top/gtucfxfqnk.html

[H10] 资源自动释放
来源：http://hz.jqgufenzy.top/gtjavylzld.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xinyue.icu/gtgtfeulok.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ppjwa.cn/gtirbrcyfo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinyuanbaomall.cn/gtabvmhzsz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangtech.top/gthoherqtf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ydjk.org.cn/gttxpktngd.html

Go:   defer f.Close()
来源：http://hz.gogol.net.cn/gtiqcqzbky.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hfpthk.cn/gtjoaiwoyj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtszartwve.html

================================================================================
来源：http://hz.316326.xyz/gtuuusjbvx.html

I. 正则表达式
来源：http://hz.xuetiantiany.cn/gtulbjpqvi.html

================================================================================
来源：http://hz.xziqi.cn/gtnxekvrgj.html

[I01] 判断是否匹配
来源：http://hz.hywenlv.cn/gtcllmxwuq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.daxiang520.top/gtgeafwkfy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hywenlv.cn/gttehrgcdv.html

JS:   /\d+/.test(s)
来源：http://hz.guannengcc.top/gtjkbauqlo.html

TS:   /\d+/.test(s)
来源：http://hz.yj20258.top/gtkkyevbxe.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jqgufenzy.top/gtjftdskld.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shuidangran.top/gtvqzqpbjb.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhaomingkeji.xyz/gtlcmsfjqa.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.redwolf501.top/gtbbustbpu.html

[I02] 提取所有匹配
来源：http://hz.vqdsnc.cn/gtaapohddc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.iojbl.cn/gtpamcrich.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhaomingkeji.xyz/gtzrzokhyv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hfpthk.cn/gtlczlsirh.html

TS:   s.match(/\d+/g)
来源：http://hz.jinghuilouyu.cn/gtwlcuzvza.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.wangshuangyany.cn/gtfgetldci.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xziqi.cn/gtnyujiozv.html

Ruby: s.scan(/\d+/)
来源：http://hz.chenlongwang.top/gtonzculpg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.daria6918.cn/gttemcynkx.html

[I03] 提取捕获分组
来源：http://hz.jiagoushi.top/gtxmxedzhg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yuxming.cn/gtatucnpyy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.guannengcc.top/gtejnifvno.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.nanxuanxn.top/gtsrvjdzct.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zycfv.cn/gtzfotfbtn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hammf.cn/gtjjaopquy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hysaishi.cn/gtjdrurxry.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.316326.xyz/gtugkjggmn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ywan-chungtsiang.top/gthxgbrrom.html

[I04] 正则替换
来源：http://hz.shangyingyoupin.top/gtrwebkyhd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.feifeiyinyue.top/gtzmibiuhm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.kuanghao11.cn/gtlnrgvtpy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhengqikj.top/gtuyujatei.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jiagoushi.top/gtbcezewkj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhaomingkeji.xyz/gtkymqqzfp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ywan-chungtsiang.top/gtvpkjphym.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hysaishi.cn/gtxwkaxptp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hysaishi.cn/gtdasnzkyr.html

[I05] 按正则拆分
来源：http://hz.feifeiyinyue.top/gtttezlowm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yvedp.cn/gtxopxiaez.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.meibo888.top/gtsslbypyp.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.quarkkingdee.top/gtmndyyomu.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhaomingkeji.xyz/gtozefchsd.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hnxiangtu.top/gtfqhhlgay.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yvedp.cn/gtjzwiwlgx.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jinqigfzy.top/gtpmknlkqt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhoulong.xyz/gtskfiwxas.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.havefunace.top/gtrteewjzw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.pycfn.com/gtvovoxnnk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yj202588.top/gtdbsdwnxz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hysaishi.cn/gtimaasvrt.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fzhhl.top/gtqmmmtwpz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.snrcjt.cn/gttodlzjlw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.0kj1m.cn/gteodszdzl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.pycfn.com/gtepuekeew.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.guannengcc.top/gthlvjtdpu.html

[I07] 忽略大小写与多行模式
来源：http://hz.daria6918.cn/gtmunnbhqu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.tianlin.xyz/gtrtyrwinp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.birdmap.top/gtryhdmltm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.fzhhl.top/gtdkpmjckn.html

TS:   /error/gim
来源：http://hz.haohaochexian.top/gtyjdfbeer.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.meibo888.top/gtqhysoxvd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.9152youxi.cn/gttkkotsry.html

Ruby: s.scan(/error/i)
来源：http://hz.quarkkingdee.top/gtilgjexgu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xziqi.cn/gtasxaxubs.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yvedp.cn/gtzqdonpnh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ywan-chungtsiang.top/gtrfdfylkl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jlsjyb.cn/gtnexlkshm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.pycfn.com/gtjeddtzon.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhengqikj.top/gtekncivmd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.aizwys.cn/gtokcjolal.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.havefunace.top/gtbiliahnm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shanyushiyangkeji.top/gtjmfionka.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jinyuanbaomall.cn/gtpkpsrprs.html

================================================================================
来源：http://hz.bjfxy.top/gtiynmebui.html

J. 日期与时间
来源：http://hz.nanxuanxn.top/gtpecsnnbp.html

================================================================================
来源：http://hz.aibaodan.cn/gtioguoqmv.html

[J01] 获取当前时间
来源：http://hz.chenlongwang.top/gtmgnywoqn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.gzhubu.top/gtxnodngfb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.bjfxy.top/gtkpsjcpti.html

JS:   new Date();  Date.now()
来源：http://hz.feifeiyinyue.top/gtrgztezmi.html

TS:   new Date();  Date.now()
来源：http://hz.aibaodan.cn/gtliouvyos.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ehwqpu.com/gtrhsjekyo.html

Go:   time.Now()
来源：http://hz.fzhhl.top/gtfhkemnrn.html

Ruby: Time.now
来源：http://hz.shzxlz.cn/gtfphpucvp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yj202588.top/gtauzfsfwj.html

[J02] 格式化输出
来源：http://hz.9152youxi.cn/gtluzfakkw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhaomingkeji.xyz/gtlillbcne.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.0kj1m.cn/gtkadqcfxw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.52xcode.cn/gtvxrdtjdl.html

TS:   d.toISOString()
来源：http://hz.wangdashe.top/gtrqwizyab.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xuanzx.com/gtnwkkkell.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xylfe.cn/gtuxnfpzoa.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.316326.xyz/gtsyfydnif.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cqqwz.cn/gtpvvxgchl.html


<!-- 参考信息 -->