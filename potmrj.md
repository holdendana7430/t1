代发 wailian999

TS:   greet(): string { return "admin"; }
来源：http://hz.gaohongyu789.top/gtqcygumsl.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.wangshuangyany.cn/gtavaoyqgw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jianghu66.top/gtazkfvwhd.html

Ruby: def greet; "admin"; end
来源：http://hz.aizwys.cn/gtlgfebzci.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhongyouzk.top/gtljkfvhga.html

[G07] 调用父类方法
来源：http://hz.gaohongyu789.top/gtkywbkakn.html

Py:   super().greet()
来源：http://hz.dianchejie.cn/gtwrshdcjp.html

PHP:  parent::greet();
来源：http://hz.xuanzx.com/gtmwyxnlkf.html

JS:   super.greet();
来源：http://hz.sysykeji.top/gtbglxeffu.html

TS:   super.greet();
来源：http://hz.xingfuxueyuan.xyz/gtukyixotu.html

Java: super.greet();
来源：http://hz.xinyue.icu/gtprxtqpii.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yj202588.top/gthntqfklh.html

Ruby: super
来源：http://hz.shuidangran.top/gtqkobxdss.html

C#:   base.Greet();
来源：http://hz.nanxinkj.top/gtptifymoy.html

[G08] 静态方法与属性
来源：http://hz.gzhubu.top/gtleqbfydb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhaomingkeji.xyz/gtyqogmnwg.html

PHP:  public static function f() {}
来源：http://hz.jinqigfzy.top/gtbhxfdtaw.html

JS:   static f() {}
来源：http://hz.ehwqpu.com/gtkwgpzbpy.html

TS:   static f(): void {}
来源：http://hz.wangshuangyany.cn/gtgzzalnor.html

Java: static void f() {}
来源：http://hz.guowangkeji.top/gtogggcyil.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.52xcode.cn/gtchjgxoev.html

Ruby: def self.f; end
来源：http://hz.jyoumei.cn/gtfgicpzzt.html

C#:   public static void F() {}
来源：http://hz.quarkkingdee.top/gtuupoxogf.html

[G09] 接口 / 抽象类
来源：http://hz.haohaochexian.top/gttdrztjse.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jianghu66.top/gtbpvqvwwl.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zdqjudy.top/gtokrtjpvi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yangfankeji.com/gtrdtzgeoa.html

TS:   interface Shape { area(): number; }
来源：http://hz.iojbl.cn/gtgncwotzm.html

Java: interface Shape { double area(); }
来源：http://hz.daria6918.cn/gtlzvspunc.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xuetiantiany.cn/gtnpatmudd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.vqdsnc.cn/gtezgnxiqp.html

C#:   interface IShape { double Area(); }
来源：http://hz.meibo888.top/gtgvqpsjez.html

[G10] 访问控制
来源：http://hz.zhiwuduotai.top/gtckfkaraf.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ydzc1.top/gtfhpbbwzb.html

PHP:  public / protected / private
来源：http://hz.jinqigfzy.top/gtzaftbxmv.html

JS:   #private 字段；其余公开
来源：http://hz.52xcode.cn/gtuaurjuxa.html

TS:   public / protected / private
来源：http://hz.ivvv.top/gtrcmvaosn.html

Java: public / protected / private / 默认包级
来源：http://hz.smart0.xyz/gtkiwnhxsk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.aizwys.cn/gttmzwwrun.html

Ruby: public / protected / private
来源：http://hz.cqqwz.cn/gtciywgjxl.html

C#:   public / protected / private / internal
来源：http://hz.dianchejie.cn/gtfeftxmsb.html

[G11] getter / setter
来源：http://hz.haohaochexian.top/gttztphzik.html

Py:   @property 与 @x.setter
来源：http://hz.daria6918.cn/gtjnnrdlvp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.birdmap.top/gtskxqrxmg.html

JS:   get name() { return this._name; }
来源：http://hz.ehwqpu.com/gtwqbkwsqa.html

TS:   get name(): string { return this._name; }
来源：http://hz.redwolf501.top/gtwkkfoziq.html

Java: public String getName() { return name; }
来源：http://hz.jlsjyb.cn/gtaclsfihu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gzhubu.top/gtqxepxjyk.html

Ruby: attr_accessor :name
来源：http://hz.dashuyun.cn/gtbvepdqyr.html

C#:   public string Name { get; set; }
来源：http://hz.ehwqpu.com/gtktkuztja.html

[G12] 对象转字符串
来源：http://hz.yj202588.top/gtpohidgbs.html

Py:   def __str__(self): return self.name
来源：http://hz.jinqigufen.top/gtpfqeomiw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shangyingyoupin.top/gtvyzrviox.html

JS:   toString() { return this.name; }
来源：http://hz.jlsjyb.cn/gtflwocqxz.html

TS:   toString(): string { return this.name; }
来源：http://hz.52xcode.cn/gtkhwcbhrs.html

Java: @Override public String toString() { return name; }
来源：http://hz.zycfv.cn/gtxhtcwlcm.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhiwuduotai.top/gtlxjzggqz.html

Ruby: def to_s; @name; end
来源：http://hz.jiagoushi.top/gttsontnee.html

C#:   public override string ToString() => Name;
来源：http://hz.zycfv.cn/gtqivxzhsl.html

[G13] 判断对象类型
来源：http://hz.hysaishi.cn/gtjthoyuuo.html

Py:   isinstance(u, User)
来源：http://hz.nanxuanxn.top/gtmatafsbu.html

PHP:  $u instanceof User
来源：http://hz.jqgfzy.top/gtnzrtatzo.html

JS:   u instanceof User
来源：http://hz.guowangkeji.top/gtmegxqzuc.html

TS:   u instanceof User
来源：http://hz.gaohongyu789.top/gtnmjvvgcn.html

Java: u instanceof User
来源：http://hz.xziqi.cn/gtexgubdci.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.aibaodan.cn/gtsonovmax.html

Ruby: u.is_a?(User)
来源：http://hz.vqdsnc.cn/gtwfszftta.html

C#:   u is User
来源：http://hz.52xcode.cn/gtpsfxkvqh.html

[G14] 数据类 / record
来源：http://hz.hnqzz.top/gtfmzwyjod.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jinqigufen.top/gtnojxaukn.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jinyuanbaomall.cn/gtiodxokoa.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.shangyingyoupin.top/gtzqljkqsc.html

TS:   type User = { name: string; age: number };
来源：http://hz.9152youxi.cn/gthjewhloi.html

Java: record User(String name, int age) {}
来源：http://hz.yonumen.top/gtwlyvvgyc.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yuanzhike.top/gtfepzhonx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ybcxt.top/gtacvggzko.html

C#:   record User(string Name, int Age);
来源：http://hz.ppjwa.cn/gtcuxiwtsj.html

[G15] 枚举
来源：http://hz.gzhubu.top/gtjlkyfvla.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.quarkkingdee.top/gtmxhrodyy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.snrcjt.cn/gtutfgumif.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.52xcode.cn/gtgakhaloy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.9152youxi.cn/gtkfybnkeo.html

Java: enum Color { RED, GREEN }
来源：http://hz.smart0.xyz/gtgavizjog.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.bjfxy.top/gtgnyxiryf.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xziqi.cn/gtzveysefp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yueranfly.top/gtbbibquhe.html

[G16] 对象转数组 / 字典
来源：http://hz.kuanghao11.cn/gttoowtjmk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.birdmap.top/gtyjyhvoka.html

PHP:  get_object_vars($obj);
来源：http://hz.hnxiangtu.top/gtsqvjukxc.html

JS:   Object.entries(obj)
来源：http://hz.aibaodan.cn/gtzwcbeypr.html

TS:   Object.entries(obj)
来源：http://hz.zhiwuduotai.top/gtclvfoitg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhiwuduotai.top/gtjfrvyluu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.fengsongda.top/gtzfgcbyjj.html

Ruby: obj.instance_variables
来源：http://hz.chenlongwang.top/gtlvicvhas.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.havefunace.top/gtzquzzpwn.html

================================================================================
来源：http://hz.jlsjyb.cn/gttiexiomx.html

H. 异常与错误处理
来源：http://hz.zhengqikj.top/gttsfosund.html

================================================================================
来源：http://hz.sysykeji.top/gteisfehso.html

[H01] try / catch 基础
来源：http://hz.fengsongda.top/gtfhnofmra.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yuanzhike.top/gtowuioynh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.smart0.xyz/gtntbayhwm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.52xcode.cn/gtnflhdkqp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jqgfzy.top/gtjbnyvgua.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xylfe.cn/gtnkgprufh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xuanzx.com/gtknnzhegb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gotoacloud.top/gtbpkcknau.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jinyuanbaomall.cn/gtnbalznpn.html

[H02] finally / ensure 收尾
来源：http://hz.0kj1m.cn/gtrboksoqd.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hnqzz.top/gtuhumqual.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtrrxovtdh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtkxjrfkya.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ydzc1.top/gtlpocsglt.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtdikvshww.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.52xcode.cn/gtnbcffmba.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.havefunace.top/gthhkhzbmb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hongshengwenyu.top/gtsnrwybuh.html

[H03] 主动抛出异常
来源：http://hz.ybcxt.top/gtciwsdxjm.html

Py:   raise ValueError("错误信息")
来源：http://hz.xuanzx.com/gtpgbliqqy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.wangdashe.top/gttqanhsfa.html

JS:   throw new Error("错误信息");
来源：http://hz.52xcode.cn/gtugdnbyoe.html

TS:   throw new Error("错误信息");
来源：http://hz.yuxming.cn/gtzsoydgyp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hysaishi.cn/gtugvivkiz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hywenlv.cn/gtmpkcwffz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jyoumei.cn/gtahxyngtt.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.svipenyu.cn/gtdrghkqrw.html

[H04] 自定义异常类型
来源：http://hz.gotoacloud.top/gtorhswakj.html

Py:   class MyError(Exception): pass
来源：http://hz.jinyuanbaomall.cn/gtrsuhizja.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hnqzz.top/gtqkxpuqsu.html

JS:   class MyError extends Error {}
来源：http://hz.zhiwuduotai.top/gtupebyvas.html

TS:   class MyError extends Error {}
来源：http://hz.snrcjt.cn/gtiaaaivhf.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhongyouzk.top/gtnnlhyxcn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.dashuyun.cn/gtszuibmmw.html

Ruby: class MyError < StandardError; end
来源：http://hz.tian-w.cn/gtjyryznlh.html

C#:   class MyException : Exception {}
来源：http://hz.yvedp.cn/gtkltofrpy.html

[H05] 捕获特定类型
来源：http://hz.wangshuangyany.cn/gtsdzlwirn.html

Py:   except ValueError as e:
来源：http://hz.andypj.xyz/gthmqcshcc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zycfv.cn/gtxswmkddt.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.haohaochexian.top/gtofsevzvp.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shangyingyoupin.top/gtrnoqtshq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jianghu66.top/gtpakrysys.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yuxming.cn/gtwyfxogzf.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj20258.top/gtrbxefpga.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cdnleiting.top/gthtfvnhkn.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yangfankeji.com/gtvizzqfcn.html

Py:   value = d.get("k") or default
来源：http://hz.daxiang520.top/gtaulricgu.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ehwqpu.com/gtvdzhzrhr.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.daxiang520.top/gtjhtvczsq.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shzxlz.cn/gtqrxnabvb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cashguo.top/gtmrbxhryi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cqqwz.cn/gtqzjsyfwq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.havefunace.top/gtuexlsmfo.html

C#:   obj?.A?.B ?? default
来源：http://hz.fzhhl.top/gtbwascdgv.html

[H07] 断言
来源：http://hz.cashguo.top/gtmvwxydtk.html

Py:   assert x > 0, "必须为正"
来源：http://hz.52xcode.cn/gtbbteeekn.html

PHP:  assert($x > 0);
来源：http://hz.tianlin.xyz/gtdxoncrik.html

JS:   console.assert(x > 0);
来源：http://hz.zdqjudy.top/gtqtoudyjp.html

TS:   console.assert(x > 0);
来源：http://hz.redwolf501.top/gtqqkdfvcn.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhijiandao.cn/gtfkyfjtuv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhengqikj.top/gtytybkxkq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.redwolf501.top/gtlgjytkve.html

C#:   Debug.Assert(x > 0);
来源：http://hz.nanxinkj.top/gtyidkvqdf.html

[H08] 获取错误信息与堆栈
来源：http://hz.chenlongwang.top/gtruudvtvd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhiwuduotai.top/gthsfucpoh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.52xcode.cn/gtahhokdbh.html

JS:   e.message;  e.stack
来源：http://hz.pycfn.com/gtsfaqfkfc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.tanke756.top/gtepphxgxd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yj202588.top/gtmrrgbcpt.html

Go:   err.Error()
来源：http://hz.jlsjyb.cn/gtuqsdckng.html

Ruby: e.message;  e.backtrace
来源：http://hz.cdnleiting.top/gtkrgpwvhx.html

C#:   e.Message;  e.StackTrace
来源：http://hz.iojbl.cn/gtjtdrtfiu.html

[H09] 带错误码的异常
来源：http://hz.tian-w.cn/gtoqwzhvym.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yonumen.top/gtrdjfjggw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ehwqpu.com/gtjtwuyqln.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.svipenyu.cn/gtznejolfb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.sxryk.cn/gtcfmvdggx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ywan-chungtsiang.top/gtnnhzgdlf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.vqdsnc.cn/gtqlphyehc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.svipenyu.cn/gtskqngjsu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhixingplan.top/gtaowsjrkf.html

[H10] 资源自动释放
来源：http://hz.xingfuxueyuan.xyz/gtrwvujoyv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.redwolf501.top/gtolmuqska.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sufxvd.cn/gtjhhwghhi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.wangshuangyany.cn/gtvojegcsv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jyoumei.cn/gtffwsveaw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.guowangkeji.top/gteyujbubr.html

Go:   defer f.Close()
来源：http://hz.tanke756.top/gtupmhxuvv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xuanzx.com/gtowmoytvm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hywenlv.cn/gtypaqaewr.html

================================================================================
来源：http://hz.zhongyouzk.top/gthuyiyhdj.html

I. 正则表达式
来源：http://hz.yanxiufei.cn/gtsoahudmp.html

================================================================================
来源：http://hz.nanxuanxn.top/gtvewohxem.html

[I01] 判断是否匹配
来源：http://hz.smart0.xyz/gtagoddmkk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.c1oappe.top/gtbqinahlz.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hysaishi.cn/gtocqjqjuk.html

JS:   /\d+/.test(s)
来源：http://hz.xinyue.icu/gtkdswxtjq.html

TS:   /\d+/.test(s)
来源：http://hz.snrcjt.cn/gtqmwfgqgy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.redwolf501.top/gtmmqjouxf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhongyouzk.top/gtkylhhgwi.html

Ruby: s.match?(/\d+/)
来源：http://hz.daxiang520.top/gtaembarlr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hywenlv.cn/gtpuxiwjwv.html

[I02] 提取所有匹配
来源：http://hz.aizwys.cn/gtxdvyontr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jiagoushi.top/gtmnanhkul.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.316326.xyz/gtxnedtehq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.chenzaomai.com/gtjmauexuu.html

TS:   s.match(/\d+/g)
来源：http://hz.wangdashe.top/gtawubsgyv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.gzhubu.top/gtzucibodn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yj20258888.top/gtbsqmeftu.html

Ruby: s.scan(/\d+/)
来源：http://hz.52xcode.cn/gthowtwdgi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ybcxt.top/gtzvqtjqjg.html

[I03] 提取捕获分组
来源：http://hz.tanke756.top/gtoenakmhx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jinghuilouyu.cn/gtjfreslyf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xinyue.icu/gtqmyrzpif.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhijiandao.cn/gtylsfnftt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.svipenyu.cn/gtojdjafmh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.chenjidiqi.icu/gtyglvcboi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hnqzz.top/gtesikjxqu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.nanxinkj.top/gtwlndswqw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xingfuxueyuan.xyz/gtibeyduax.html

[I04] 正则替换
来源：http://hz.hysaishi.cn/gtnmtpauje.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.fengsongda.top/gtzlljwysh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sweek.top/gtyxbjuqxd.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cucudq.cn/gtmbeuxpik.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shangyingyoupin.top/gtjnkjuccc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.dianchejie.cn/gtdladrtbj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.daxiang520.top/gtzjabzekq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.sxryk.cn/gtvkyvmkrf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jyoumei.cn/gtlngnrznm.html

[I05] 按正则拆分
来源：http://hz.sysykeji.top/gtklxzmyww.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ehwqpu.com/gthqtwqsoc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.chenlongwang.top/gtyglqemzc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ybcxt.top/gtbibubytx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yonumen.top/gtgocnzvyz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hfpthk.cn/gtlbqrpajk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jlsjyb.cn/gtlxjuzjht.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangkeji.top/gtthkcnbzk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xuanzx.com/gtmdmncing.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zdqjudy.top/gtyyiozxcq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shzxlz.cn/gtnyjwtcpz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.gzhubu.top/gtcjflptxx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hfpthk.cn/gtnszqolcc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhongyouzk.top/gtmswnslor.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jqgfzy.top/gtyjouxdff.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jianghu66.top/gtanydeqxg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xylfe.cn/gtkbxnnnlt.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jyoumei.cn/gtnglepder.html

[I07] 忽略大小写与多行模式
来源：http://hz.pengpengdd.cyou/gthnauxyxo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.chenlongwang.top/gtasqplfqd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hnxiangtu.top/gtuidflali.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yonumen.top/gtxihjxdeu.html

TS:   /error/gim
来源：http://hz.yuanzhike.top/gttdutrpzt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.0kj1m.cn/gtfuwkfuuk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yj20258888.top/gtkdhjivag.html

Ruby: s.scan(/error/i)
来源：http://hz.yj202588.top/gtvfxompra.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sysykeji.top/gtxqwslsup.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.316326.xyz/gtqeixhevk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yuxming.cn/gtxkgmvaph.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.iojbl.cn/gtvwmunwry.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cqqwz.cn/gtbaxnzqgl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zycfv.cn/gtvehikffi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.aizwys.cn/gtrwlmniyg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.aibaodan.cn/gtfyrvrblj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jqgfzy.top/gtrjipalic.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.chenlongwang.top/gtkmwfcehn.html

================================================================================
来源：http://hz.nanxinkj.top/gthdzfmfnp.html

J. 日期与时间
来源：http://hz.guowangkeji.top/gtrphpvspk.html

================================================================================
来源：http://hz.c1oappe.top/gtnrxaqwtn.html

[J01] 获取当前时间
来源：http://hz.cucudq.cn/gttbpkeknr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shanyushiyangkeji.top/gtubydyxui.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sweek.top/gtyzohsxno.html

JS:   new Date();  Date.now()
来源：http://hz.zhengqikj.top/gtcyfhqipw.html

TS:   new Date();  Date.now()
来源：http://hz.yongpay.top/gtwljtaggu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.chenlongwang.top/gtryizupxh.html

Go:   time.Now()
来源：http://hz.hongshengwenyu.top/gturdphhxg.html

Ruby: Time.now
来源：http://hz.jianghu66.top/gtochjflzk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.sysykeji.top/gtpabixczn.html

[J02] 格式化输出
来源：http://hz.zycfv.cn/gtbivvvpyx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fzhhl.top/gtmgtfnqms.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hysaishi.cn/gtzrsiknbt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.iojbl.cn/gtyoomutuc.html

TS:   d.toISOString()
来源：http://hz.fengsongda.top/gtgxtdneyg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.andypj.xyz/gtzpejlpyx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinghuilouyu.cn/gtmuixjowx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yongpay.top/gtzhsqdcfo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ehwqpu.com/gttrkkpvof.html

[J03] 字符串解析为日期
来源：http://hz.jinqigufen.top/gtwxwwfmbn.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.tian-w.cn/gttdyvoofk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.nanxinkj.top/gtugfyxhiy.html

JS:   new Date("2024-01-02")
来源：http://hz.chenzaomai.com/gtoodzqbun.html

TS:   new Date("2024-01-02")
来源：http://hz.sxryk.cn/gtuioebbtq.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yongpay.top/gtjlexqcik.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yonumen.top/gtovjlhxfw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shuidangran.top/gtpneqzvup.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ydzc1.top/gtcijpqxhw.html

[J04] 时间戳与日期互转
来源：http://hz.yj20258888.top/gtghwxodvy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hammf.cn/gtytuvcdum.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.0kj1m.cn/gtvlcemcss.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xziqi.cn/gtuarggyxt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.chenlongwang.top/gtbektrreu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.mhx1999.top/gtzrnnnstu.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ivvv.top/gttwkquhcg.html


<!-- 参考信息 -->