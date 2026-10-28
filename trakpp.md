代发 wailian999

C#:   public override string Greet() => "admin";
来源：http://hz.cheryme.top/gtldsgolec.html

[G07] 调用父类方法
来源：http://hz.jlsjyb.cn/gthfywovci.html

Py:   super().greet()
来源：http://hz.guowangkeji.top/gtbirqaezo.html

PHP:  parent::greet();
来源：http://hz.yuanzhike.top/gtsefzyvlu.html

JS:   super.greet();
来源：http://hz.meibo888.top/gtxrwpbtxc.html

TS:   super.greet();
来源：http://hz.xziqi.cn/gtkksjzlos.html

Java: super.greet();
来源：http://hz.cqqwz.cn/gtjsdsmrri.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.chenzaomai.com/gturxrqcwh.html

Ruby: super
来源：http://hz.shangyingyoupin.top/gtwwlsfvku.html

C#:   base.Greet();
来源：http://hz.andypj.xyz/gttblzawwg.html

[G08] 静态方法与属性
来源：http://hz.mhx1999.top/gtkbeguhyg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shanyushiyangkeji.top/gteqphebmp.html

PHP:  public static function f() {}
来源：http://hz.xuanzx.com/gtdiurbwep.html

JS:   static f() {}
来源：http://hz.zdqjudy.top/gtyipwupfn.html

TS:   static f(): void {}
来源：http://hz.guowangkeji.top/gtiviscemy.html

Java: static void f() {}
来源：http://hz.yonumen.top/gtaunrlslo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.wangshuangyany.cn/gtaeqckldh.html

Ruby: def self.f; end
来源：http://hz.cqqwz.cn/gtulxqdmij.html

C#:   public static void F() {}
来源：http://hz.xuetiantiany.cn/gtwgaowrqc.html

[G09] 接口 / 抽象类
来源：http://hz.bjfxy.top/gtykwfawhi.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hywenlv.cn/gtyhadbnnd.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yj20258.top/gtaoiufzig.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.guannengcc.top/gtyjrgrnph.html

TS:   interface Shape { area(): number; }
来源：http://hz.jqgufenzy.top/gtkclqreyk.html

Java: interface Shape { double area(); }
来源：http://hz.xingfuxueyuan.xyz/gtzokjulit.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.dianchejie.cn/gtrdipfves.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.nanxinkj.top/gtsacdhncd.html

C#:   interface IShape { double Area(); }
来源：http://hz.ppjwa.cn/gtkchvgavc.html

[G10] 访问控制
来源：http://hz.mhx1999.top/gtudlnmcsp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hnqzz.top/gthmaeckzx.html

PHP:  public / protected / private
来源：http://hz.birdmap.top/gttypjelkj.html

JS:   #private 字段；其余公开
来源：http://hz.tian-w.cn/gtlsbjovua.html

TS:   public / protected / private
来源：http://hz.shuidangran.top/gtgspijrbi.html

Java: public / protected / private / 默认包级
来源：http://hz.jinqigfzy.top/gtgvirfkte.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.nwbrower.top/gtmggsaafy.html

Ruby: public / protected / private
来源：http://hz.feifeiyinyue.top/gtcbgsuvqf.html

C#:   public / protected / private / internal
来源：http://hz.kuanghao11.cn/gtmojssixg.html

[G11] getter / setter
来源：http://hz.jinyuanbaomall.cn/gtryjsdjns.html

Py:   @property 与 @x.setter
来源：http://hz.hongshengwenyu.top/gtxfljmpfw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.tianlin.xyz/gtpdvdegov.html

JS:   get name() { return this._name; }
来源：http://hz.iojbl.cn/gtwvzfktru.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhoulong.xyz/gtyyrdihuk.html

Java: public String getName() { return name; }
来源：http://hz.pycfn.com/gtzdcynykm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.guowangkeji.top/gtmzwfqekr.html

Ruby: attr_accessor :name
来源：http://hz.yj202588.top/gttypxxamz.html

C#:   public string Name { get; set; }
来源：http://hz.tian-w.cn/gtvtaovjux.html

[G12] 对象转字符串
来源：http://hz.hongshengwenyu.top/gthtbnldhc.html

Py:   def __str__(self): return self.name
来源：http://hz.xuetiantiany.cn/gtcgtwokuz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gtxdomomar.html

JS:   toString() { return this.name; }
来源：http://hz.nwbrower.top/gteeeexlbh.html

TS:   toString(): string { return this.name; }
来源：http://hz.shanyushiyangtech.top/gteagophxm.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhiwuduotai.top/gtcnqmtxki.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yueranfly.top/gtlvjemdum.html

Ruby: def to_s; @name; end
来源：http://hz.ybcxt.top/gtzmnauxur.html

C#:   public override string ToString() => Name;
来源：http://hz.gotoacloud.top/gtcnungwdi.html

[G13] 判断对象类型
来源：http://hz.ivvv.top/gteohqeezr.html

Py:   isinstance(u, User)
来源：http://hz.jyoumei.cn/gtunlpflvj.html

PHP:  $u instanceof User
来源：http://hz.kuanghao11.cn/gtdapkagri.html

JS:   u instanceof User
来源：http://hz.fzhhl.top/gtymgbvacc.html

TS:   u instanceof User
来源：http://hz.zhiwuduotai.top/gthfsalkyc.html

Java: u instanceof User
来源：http://hz.hammf.cn/gtbhoevsdc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.aizwys.cn/gtwyzedlrd.html

Ruby: u.is_a?(User)
来源：http://hz.xinyue.icu/gtwsekabli.html

C#:   u is User
来源：http://hz.hysaishi.cn/gtwwotsqhi.html

[G14] 数据类 / record
来源：http://hz.sufxvd.cn/gttnxxxssi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yongpay.top/gtizjhgmav.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zhijiandao.cn/gtyibwvcsu.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.hongshengwenyu.top/gtumiiealx.html

TS:   type User = { name: string; age: number };
来源：http://hz.dashuyun.cn/gtsckjysgi.html

Java: record User(String name, int age) {}
来源：http://hz.andypj.xyz/gtkkkmomiz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cdnleiting.top/gtseqtsbvm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.pycfn.com/gtytdbboni.html

C#:   record User(string Name, int Age);
来源：http://hz.ivvv.top/gtvhkqdrlh.html

[G15] 枚举
来源：http://hz.sxryk.cn/gthaghdvtf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.dianchejie.cn/gtduuhtpro.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.svipenyu.cn/gtdfpirfyz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.dianchejie.cn/gtyjcmqcbh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ivvv.top/gtyluuqarc.html

Java: enum Color { RED, GREEN }
来源：http://hz.zdqjudy.top/gtckcvwzim.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.aizwys.cn/gtqcopcqpu.html

Ruby: Color = %i[red green].freeze
来源：http://hz.wangshuangyany.cn/gtxewkjhmi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cdnleiting.top/gtukidrdyf.html

[G16] 对象转数组 / 字典
来源：http://hz.tianlin.xyz/gtnksvgtte.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.redwolf501.top/gtflrxmies.html

PHP:  get_object_vars($obj);
来源：http://hz.zhiwuduotai.top/gtpijekxys.html

JS:   Object.entries(obj)
来源：http://hz.jyoumei.cn/gtfnyalstk.html

TS:   Object.entries(obj)
来源：http://hz.yj20258.top/gtthfobkeq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yuanzhike.top/gtvrdcfxtu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.tanke756.top/gtcovkqufu.html

Ruby: obj.instance_variables
来源：http://hz.andypj.xyz/gtgmtdyzxk.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.c1oappe.top/gtfrvyeiku.html

================================================================================
来源：http://hz.yongpay.top/gtrzuoxktw.html

H. 异常与错误处理
来源：http://hz.hfpthk.cn/gtwfrchdwa.html

================================================================================
来源：http://hz.haohaochexian.top/gtwzzosvhr.html

[H01] try / catch 基础
来源：http://hz.zhoulong.xyz/gthfaskrou.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jqgufenzy.top/gtgrqsioeq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhixingplan.top/gtxgbulvkx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gaohongyu789.top/gtlkkzeoyi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ybcxt.top/gtqeldtask.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhengqikj.top/gtimkjwqkd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ydzc1.top/gtcwkguqug.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yj20258.top/gtuljwfqyj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.tanke756.top/gtnjgkyzib.html

[H02] finally / ensure 收尾
来源：http://hz.feifeiyinyue.top/gtgyjsqvuz.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hongshengwenyu.top/gtbrjpxfte.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gtnlbdolgm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtgnkgcqyj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtligstsgi.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xziqi.cn/gtpjxzkuay.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yj20258.top/gtymevluit.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jlsjyb.cn/gtptjyzsgb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtkerdobsk.html

[H03] 主动抛出异常
来源：http://hz.nanxinkj.top/gtdkhhvaaf.html

Py:   raise ValueError("错误信息")
来源：http://hz.yangfankeji.com/gtnjcqxbrk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.daxiang520.top/gtnhglwowt.html

JS:   throw new Error("错误信息");
来源：http://hz.hnxiangtu.top/gtjiswtvkg.html

TS:   throw new Error("错误信息");
来源：http://hz.jqgfzy.top/gthnfreued.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.316326.xyz/gtitjhsbjj.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.mhx1999.top/gtxfpajqzz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cheryme.top/gtzzwrbsaj.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.tanke756.top/gttmayhvui.html

[H04] 自定义异常类型
来源：http://hz.zhongyouzk.top/gttbpindfa.html

Py:   class MyError(Exception): pass
来源：http://hz.chenzaomai.com/gtvgstfjur.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xylfe.cn/gtwivadvlt.html

JS:   class MyError extends Error {}
来源：http://hz.hywenlv.cn/gtybfofbpn.html

TS:   class MyError extends Error {}
来源：http://hz.svipenyu.cn/gtuednoczd.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ivvv.top/gtfwyfubhb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jiagoushi.top/gtwvshnikn.html

Ruby: class MyError < StandardError; end
来源：http://hz.bjfxy.top/gtcjylseie.html

C#:   class MyException : Exception {}
来源：http://hz.zhijiandao.cn/gtfntwccnq.html

[H05] 捕获特定类型
来源：http://hz.hammf.cn/gthmunioga.html

Py:   except ValueError as e:
来源：http://hz.zhiwuduotai.top/gtnrrtrret.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.andypj.xyz/gtwbwmystb.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.pengpengdd.cyou/gtrzmrnonv.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhoulong.xyz/gtzpgphagh.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shuidangran.top/gtojrqjhkj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hongshengwenyu.top/gtxzvypxmv.html

Ruby: rescue ArgumentError => e
来源：http://hz.redwolf501.top/gtmnvybags.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yangfankeji.com/gtdbhxlpjn.html

[H06] 可选值 / 空值安全访问
来源：http://hz.vqdsnc.cn/gttqmsgzuo.html

Py:   value = d.get("k") or default
来源：http://hz.cheryme.top/gtafygzzyy.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tian-w.cn/gtvlilaaoi.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.redwolf501.top/gtupawckcr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgufenzy.top/gtfzpgjwga.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhixingplan.top/gtqwhzbikx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.gogol.net.cn/gtdgraxmqw.html

Ruby: d&.dig(:a, :b)
来源：http://hz.nanxuanxn.top/gtlvdyqdup.html

C#:   obj?.A?.B ?? default
来源：http://hz.havefunace.top/gtrlfafiyg.html

[H07] 断言
来源：http://hz.chenzaomai.com/gtszgqfhzx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gaohongyu789.top/gtnjxgdkba.html

PHP:  assert($x > 0);
来源：http://hz.pycfn.com/gtrhnheknu.html

JS:   console.assert(x > 0);
来源：http://hz.kuanghao11.cn/gtvannqlrx.html

TS:   console.assert(x > 0);
来源：http://hz.shzxlz.cn/gtyaywcywr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.haohaochexian.top/gtrgntpsau.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jqgufenzy.top/gtnnvtfqvc.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.redwolf501.top/gtyucwszox.html

C#:   Debug.Assert(x > 0);
来源：http://hz.iojbl.cn/gtittctsrw.html

[H08] 获取错误信息与堆栈
来源：http://hz.bjfxy.top/gtrwkwmddr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xinyue.icu/gttfagggpr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gzhubu.top/gtxdhdzsbb.html

JS:   e.message;  e.stack
来源：http://hz.jqgufenzy.top/gtoxvccyda.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.tanke756.top/gtvquiumfh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yuanzhike.top/gtqcbotjqu.html

Go:   err.Error()
来源：http://hz.yuanzhike.top/gtkdcrnpuu.html

Ruby: e.message;  e.backtrace
来源：http://hz.daxiang520.top/gtllzstjtx.html

C#:   e.Message;  e.StackTrace
来源：http://hz.gogol.net.cn/gttqmzcqyb.html

[H09] 带错误码的异常
来源：http://hz.zhijiandao.cn/gtxwhijsej.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jyoumei.cn/gtqozetkjt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gaohongyu789.top/gthmumdbld.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.tianlin.xyz/gtzljexrlc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.haohaochexian.top/gthzloyqlz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.guannengcc.top/gtosxrkzrb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.gzhubu.top/gtafxaxhze.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yvedp.cn/gtoeozcxpm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yueranfly.top/gtwaollegc.html

[H10] 资源自动释放
来源：http://hz.dianchejie.cn/gtcvecivix.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.feifeiyinyue.top/gtxfbaduvr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jiagoushi.top/gtujevilwz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangtech.top/gtzdbhsaui.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aizwys.cn/gtscpdvvbp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zdqjudy.top/gtjthgjebu.html

Go:   defer f.Close()
来源：http://hz.aibaodan.cn/gtfkeasbta.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.feifeiyinyue.top/gtuukgclsk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jianghu66.top/gtnfuphrom.html

================================================================================
来源：http://hz.cqqwz.cn/gtxjjrzkum.html

I. 正则表达式
来源：http://hz.gaohongyu789.top/gtzpplnmqr.html

================================================================================
来源：http://hz.zhixingplan.top/gtbwthetms.html

[I01] 判断是否匹配
来源：http://hz.wangdashe.top/gtsbbeozuy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.meibo888.top/gtotkbdfnj.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ybcxt.top/gtazotvjyy.html

JS:   /\d+/.test(s)
来源：http://hz.bjfxy.top/gtmlgpmumm.html

TS:   /\d+/.test(s)
来源：http://hz.andypj.xyz/gtfmmgsemj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cdnleiting.top/gtunvbmsoq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yanxiufei.cn/gtqzpmgwij.html

Ruby: s.match?(/\d+/)
来源：http://hz.dashuyun.cn/gtawpbzkqe.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jiagoushi.top/gtawjcxdel.html

[I02] 提取所有匹配
来源：http://hz.wangdashe.top/gtuuxchqzr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.tian-w.cn/gtgxudtaat.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.dianchejie.cn/gtlwddmbkx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shzxlz.cn/gtqptxlfbg.html

TS:   s.match(/\d+/g)
来源：http://hz.hywenlv.cn/gtahhbsgiy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shuidangran.top/gtnezvlmdz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.chenlongwang.top/gtkavavyov.html

Ruby: s.scan(/\d+/)
来源：http://hz.dashuyun.cn/gttolcnjhm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.tanke756.top/gtuqygfguj.html

[I03] 提取捕获分组
来源：http://hz.daria6918.cn/gtkbeqpjrs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.aibaodan.cn/gtlwrlbvbr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jqgfzy.top/gtawgyekds.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj20258888.top/gtyssrvufo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jianghu66.top/gtgjucwndb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.meibo888.top/gtmglcgsfq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hnxiangtu.top/gtmqwckodw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ehwqpu.com/gtchachaui.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cashguo.top/gtgemlsaxl.html

[I04] 正则替换
来源：http://hz.9152youxi.cn/gtyjuvmzvk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xuanzx.com/gtprievjkv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj20258.top/gtjwvicjfw.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hnxiangtu.top/gtvztndgzr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.bjfxy.top/gtdivxjgdc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yj20258.top/gtdwkxqnhy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.fengsongda.top/gtucvurtsj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shanyushiyangtech.top/gthcprurjd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.tanke756.top/gtvluxosdg.html

[I05] 按正则拆分
来源：http://hz.yj20258888.top/gtmuvzlddo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hnxiangtu.top/gtqbeccrbb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gogol.net.cn/gticznyyah.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.vqdsnc.cn/gtbfalmwvl.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jyoumei.cn/gtvowppfkt.html

Java: s.split("\\s*,\\s*")
来源：http://hz.feifeiyinyue.top/gtimyqgysk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yuanzhike.top/gtlwfpeagn.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ydjk.org.cn/gtmvhppyht.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.quarkkingdee.top/gtyzsorxwh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.aibaodan.cn/gtelfdpfxi.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jyoumei.cn/gthlfunevl.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hongshengwenyu.top/gtyodytpze.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sxryk.cn/gttgieitdb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgufenzy.top/gtdjjttmfo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tian-w.cn/gtvkxdepps.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cheryme.top/gtvppcjown.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.daxiang520.top/gtucstyuqm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.dianchejie.cn/gtqyyvzwvh.html

[I07] 忽略大小写与多行模式
来源：http://hz.tianlin.xyz/gtdsaqxdpi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.haohaochexian.top/gtyogptpwg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.iojbl.cn/gtljbtavsn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cucudq.cn/gtkomelawu.html

TS:   /error/gim
来源：http://hz.cqqwz.cn/gtaskbvxht.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.aizwys.cn/gtzyeqhfec.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ehwqpu.com/gtggjenleu.html

Ruby: s.scan(/error/i)
来源：http://hz.mhx1999.top/gtkysmowec.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jqgfzy.top/gtxoixkpzf.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.nanxuanxn.top/gtphfkswgt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.guowangkeji.top/gtegtqoyig.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.snrcjt.cn/gtkzxaivjv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.birdmap.top/gtrwqpchfh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hongshengwenyu.top/gtubbgtrbq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yongpay.top/gtlzvwpfgv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yangfankeji.com/gtarvzmkzo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jyoumei.cn/gtlvyushad.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.dianchejie.cn/gtubjstrpt.html

================================================================================
来源：http://hz.shzxlz.cn/gtzrxxqusn.html

J. 日期与时间
来源：http://hz.yj20258888.top/gtyadspknn.html

================================================================================
来源：http://hz.zhoulong.xyz/gtnxdbmlok.html

[J01] 获取当前时间
来源：http://hz.jinyuanbaomall.cn/gtwepmdhvb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jqgfzy.top/gtkxkzzidi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.feifeiyinyue.top/gtjtthvldo.html

JS:   new Date();  Date.now()
来源：http://hz.jiagoushi.top/gtzaesrjva.html

TS:   new Date();  Date.now()
来源：http://hz.kuanghao11.cn/gtbaygzvbs.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hfpthk.cn/gtvewtqple.html

Go:   time.Now()
来源：http://hz.jinyuanbaomall.cn/gtfaidcybm.html

Ruby: Time.now
来源：http://hz.gzhubu.top/gtqmrfzuuk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hnqzz.top/gtlctihswv.html

[J02] 格式化输出
来源：http://hz.fengsongda.top/gtqwdmekjt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.redwolf501.top/gtsofvaiaq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ppjwa.cn/gtooxfdlsg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yj20258.top/gtaacgvxbl.html

TS:   d.toISOString()
来源：http://hz.jianghu66.top/gtudvxvrjv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hnxiangtu.top/gtrthpzhkl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.chenjidiqi.icu/gtzyrmhydf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj202588.top/gtxrklolbu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yangfankeji.com/gtynjtgecw.html

[J03] 字符串解析为日期
来源：http://hz.chenzaomai.com/gtpkadvcgc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jiagoushi.top/gttjiinaag.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gzhubu.top/gtmjuztzno.html

JS:   new Date("2024-01-02")
来源：http://hz.yuxming.cn/gtbobcaics.html

TS:   new Date("2024-01-02")
来源：http://hz.ybcxt.top/gtntehbuir.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.52xcode.cn/gtqywxmxax.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.smart0.xyz/gtewrfjasp.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.birdmap.top/gtflsspxay.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jqgfzy.top/gtkaghaibl.html

[J04] 时间戳与日期互转
来源：http://hz.zdqjudy.top/gtpxdaarfz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jiagoushi.top/gtxcqesaiv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.wangshuangyany.cn/gtifvzmani.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.bjfxy.top/gtkwrlodfk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.tianlin.xyz/gtjpcnkljm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.bjfxy.top/gtuvdovoew.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xuanzx.com/gtkyusllxf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhaomingkeji.xyz/gtmbneoqiy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yvedp.cn/gtwdkegzmk.html

[J05] 时间加减（加 7 天）
来源：http://hz.jinghuilouyu.cn/gtmxqlrnoo.html

Py:   now + timedelta(days=7)
来源：http://hz.vqdsnc.cn/gtplelczhe.html


<!-- 参考信息 -->