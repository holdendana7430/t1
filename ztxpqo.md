代发 wailian999

Ruby: super
来源：http://hz.xuetiantiany.cn/gtqlxkzbvz.html

C#:   base.Greet();
来源：http://hz.chenlongwang.top/gtqfkqiwsf.html

[G08] 静态方法与属性
来源：http://hz.yvedp.cn/gtzcgbwfay.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinyuanbaomall.cn/gtbbzxdbak.html

PHP:  public static function f() {}
来源：http://hz.sysykeji.top/gteqsnxnul.html

JS:   static f() {}
来源：http://hz.ppjwa.cn/gtrwgbxrxr.html

TS:   static f(): void {}
来源：http://hz.shuidangran.top/gtqsgitemg.html

Java: static void f() {}
来源：http://hz.gotoacloud.top/gtsbgowiog.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhijiandao.cn/gtdnssnsmj.html

Ruby: def self.f; end
来源：http://hz.sufxvd.cn/gtaqlxhsin.html

C#:   public static void F() {}
来源：http://hz.yuxming.cn/gtzvdnwmic.html

[G09] 接口 / 抽象类
来源：http://hz.hnxiangtu.top/gttymhghxj.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.gzhubu.top/gticpentag.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.nanxuanxn.top/gtsftphavv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.pycfn.com/gtdlnqejdo.html

TS:   interface Shape { area(): number; }
来源：http://hz.jinqigfzy.top/gtirvbfrrn.html

Java: interface Shape { double area(); }
来源：http://hz.wangdashe.top/gthzcfivlm.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cashguo.top/gtzcueaqzo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.havefunace.top/gtosrrpikx.html

C#:   interface IShape { double Area(); }
来源：http://hz.hongshengwenyu.top/gtyiqritjg.html

[G10] 访问控制
来源：http://hz.aizwys.cn/gthlnmftaj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.9152youxi.cn/gtjsircsxp.html

PHP:  public / protected / private
来源：http://hz.jqgufenzy.top/gtzkerretd.html

JS:   #private 字段；其余公开
来源：http://hz.ppjwa.cn/gtlaxqgizi.html

TS:   public / protected / private
来源：http://hz.hammf.cn/gtlfivuxox.html

Java: public / protected / private / 默认包级
来源：http://hz.hfpthk.cn/gtxnxjgyyg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.andypj.xyz/gtehlbfehs.html

Ruby: public / protected / private
来源：http://hz.nanxinkj.top/gtodjnzded.html

C#:   public / protected / private / internal
来源：http://hz.ehwqpu.com/gtctqhxugq.html

[G11] getter / setter
来源：http://hz.snrcjt.cn/gtjrgtlwhd.html

Py:   @property 与 @x.setter
来源：http://hz.sysykeji.top/gtniwvzjwz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.9152youxi.cn/gtofbynxuc.html

JS:   get name() { return this._name; }
来源：http://hz.316326.xyz/gtyvhhcfph.html

TS:   get name(): string { return this._name; }
来源：http://hz.kuanghao11.cn/gtdrvojwbf.html

Java: public String getName() { return name; }
来源：http://hz.9152youxi.cn/gtmczihpfi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gogol.net.cn/gtbajepong.html

Ruby: attr_accessor :name
来源：http://hz.zdqjudy.top/gtugqmhmph.html

C#:   public string Name { get; set; }
来源：http://hz.aibaodan.cn/gtoibhdgcx.html

[G12] 对象转字符串
来源：http://hz.gotoacloud.top/gtevanephm.html

Py:   def __str__(self): return self.name
来源：http://hz.havefunace.top/gtvzosflpn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yuanzhike.top/gtjmdvmpss.html

JS:   toString() { return this.name; }
来源：http://hz.yonumen.top/gtwdrwqgny.html

TS:   toString(): string { return this.name; }
来源：http://hz.zycfv.cn/gteqesbnve.html

Java: @Override public String toString() { return name; }
来源：http://hz.dashuyun.cn/gtfgvlaoqu.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.snrcjt.cn/gtypefuqza.html

Ruby: def to_s; @name; end
来源：http://hz.yongpay.top/gtmsxckads.html

C#:   public override string ToString() => Name;
来源：http://hz.hnqzz.top/gtdhnebjdv.html

[G13] 判断对象类型
来源：http://hz.tanke756.top/gtbmnizjsr.html

Py:   isinstance(u, User)
来源：http://hz.daxiang520.top/gtghkpdnpi.html

PHP:  $u instanceof User
来源：http://hz.cqqwz.cn/gtaycuntqo.html

JS:   u instanceof User
来源：http://hz.0kj1m.cn/gtqyflekxd.html

TS:   u instanceof User
来源：http://hz.yonumen.top/gtdfoofyfm.html

Java: u instanceof User
来源：http://hz.mhx1999.top/gtuxtlswdn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.iojbl.cn/gtuwvldeit.html

Ruby: u.is_a?(User)
来源：http://hz.vqdsnc.cn/gtjmvuxcyb.html

C#:   u is User
来源：http://hz.redwolf501.top/gtwvjxnqbh.html

[G14] 数据类 / record
来源：http://hz.yuanzhike.top/gtpzdjhaet.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hnqzz.top/gtyuekaemk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zdqjudy.top/gtgwnzgxdu.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gogol.net.cn/gtfelwntmg.html

TS:   type User = { name: string; age: number };
来源：http://hz.xuanzx.com/gtvrmozztg.html

Java: record User(String name, int age) {}
来源：http://hz.gogol.net.cn/gtllhfidjs.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hnqzz.top/gtqlubjyjn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xinyue.icu/gtqqgwwxby.html

C#:   record User(string Name, int Age);
来源：http://hz.mhx1999.top/gtzrziwdlc.html

[G15] 枚举
来源：http://hz.hongshengwenyu.top/gtlzbxmhns.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.daria6918.cn/gtdxqzcgic.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.chenjidiqi.icu/gtpgftsgoj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cqqwz.cn/gtqqtxmwhq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ppjwa.cn/gtbgkgkbwc.html

Java: enum Color { RED, GREEN }
来源：http://hz.snrcjt.cn/gtooohpitl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sxryk.cn/gtefuixmjx.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yuxming.cn/gtrafgymhz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jqgufenzy.top/gtuzgjkfju.html

[G16] 对象转数组 / 字典
来源：http://hz.jinyuanbaomall.cn/gtvksevjah.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jyoumei.cn/gtpfbsycfb.html

PHP:  get_object_vars($obj);
来源：http://hz.guowangkeji.top/gthrcdppdq.html

JS:   Object.entries(obj)
来源：http://hz.andypj.xyz/gtvdillevw.html

TS:   Object.entries(obj)
来源：http://hz.kuanghao11.cn/gtdgctdnyx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ehwqpu.com/gtuyyqwakl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sweek.top/gtgqpvikpv.html

Ruby: obj.instance_variables
来源：http://hz.jinqigfzy.top/gtmaqswuik.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.chenjidiqi.icu/gtziiprpuu.html

================================================================================
来源：http://hz.ydjk.org.cn/gtgbmdonzl.html

H. 异常与错误处理
来源：http://hz.dashuyun.cn/gtlikijgpo.html

================================================================================
来源：http://hz.cdnleiting.top/gtruuvhdqo.html

[H01] try / catch 基础
来源：http://hz.meibo888.top/gtiiiyexrf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.haohaochexian.top/gtdrfvijvs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yongpay.top/gtwbjcuerx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jyoumei.cn/gtwylradxb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hammf.cn/gtacjshtdz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.fzhhl.top/gtodrozbvi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.nwbrower.top/gtccsoqyjd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.ydjk.org.cn/gtizxralnq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.316326.xyz/gtgjcorbsz.html

[H02] finally / ensure 收尾
来源：http://hz.ehwqpu.com/gtfolujabx.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yangfankeji.com/gtdxivwbiv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtysrgkchl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhijiandao.cn/gtqjmcgvgo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gtwjxelnhb.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtrxnebdfu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ydzc1.top/gtexwvsnxx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jianghu66.top/gtbtfsqzsp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yj20258.top/gtkcmywnpp.html

[H03] 主动抛出异常
来源：http://hz.pycfn.com/gtdffsdzif.html

Py:   raise ValueError("错误信息")
来源：http://hz.quarkkingdee.top/gteualiquk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.bjfxy.top/gtulsocwnd.html

JS:   throw new Error("错误信息");
来源：http://hz.xuanzx.com/gtfrwlplpt.html

TS:   throw new Error("错误信息");
来源：http://hz.iojbl.cn/gttlqpdeft.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gogol.net.cn/gtdhahjrra.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yangfankeji.com/gtigjpmlfd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.meibo888.top/gtjzofpzjn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.feifeiyinyue.top/gtefejwzof.html

[H04] 自定义异常类型
来源：http://hz.aizwys.cn/gtwnvnakxq.html

Py:   class MyError(Exception): pass
来源：http://hz.kuanghao11.cn/gttwhagkko.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shanyushiyangtech.top/gtamfmhkxe.html

JS:   class MyError extends Error {}
来源：http://hz.yongpay.top/gtfukuqozu.html

TS:   class MyError extends Error {}
来源：http://hz.zdqjudy.top/gthqiryfvd.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shanyushiyangkeji.top/gtyowsoywg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.chenlongwang.top/gtkebgkkhm.html

Ruby: class MyError < StandardError; end
来源：http://hz.andypj.xyz/gtscpheqxd.html

C#:   class MyException : Exception {}
来源：http://hz.jqgfzy.top/gthkcyruyi.html

[H05] 捕获特定类型
来源：http://hz.yuanzhike.top/gtezmklatu.html

Py:   except ValueError as e:
来源：http://hz.yangfankeji.com/gtajvaistl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hywenlv.cn/gtwyenpktc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.316326.xyz/gtfeqkxned.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.andypj.xyz/gtzjeyizpd.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.birdmap.top/gthudgjfyy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cqqwz.cn/gtulnwstjk.html

Ruby: rescue ArgumentError => e
来源：http://hz.fzhhl.top/gtxdyqcnrf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yj20258.top/gtbouhmifm.html

[H06] 可选值 / 空值安全访问
来源：http://hz.andypj.xyz/gtewewiwgp.html

Py:   value = d.get("k") or default
来源：http://hz.52xcode.cn/gtifruhtgo.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jyoumei.cn/gthzzxfozh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hnqzz.top/gtwdfrnrvy.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.wangdashe.top/gtnoeikcoi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yangfankeji.com/gtryzqsxlf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sysykeji.top/gtcikerhqn.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hywenlv.cn/gtnwpfsbyr.html

C#:   obj?.A?.B ?? default
来源：http://hz.yj20258.top/gtcujlctng.html

[H07] 断言
来源：http://hz.dianchejie.cn/gtdfesuyxw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ydjk.org.cn/gtsmjalxxi.html

PHP:  assert($x > 0);
来源：http://hz.yuxming.cn/gtxrlchtat.html

JS:   console.assert(x > 0);
来源：http://hz.redwolf501.top/gtwwdsybxy.html

TS:   console.assert(x > 0);
来源：http://hz.tian-w.cn/gtytorjlna.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yangfankeji.com/gtwnhnload.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.vqdsnc.cn/gtnjmfjjgp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hysaishi.cn/gtndoyokrv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.aibaodan.cn/gtvszhjqol.html

[H08] 获取错误信息与堆栈
来源：http://hz.shanyushiyangtech.top/gtamqppxaa.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xingfuxueyuan.xyz/gtqngbzevk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yj20258.top/gtgteuwhnf.html

JS:   e.message;  e.stack
来源：http://hz.aibaodan.cn/gtoouvwwpv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ppjwa.cn/gtvgjyhnwc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xuanzx.com/gtqxntozdo.html

Go:   err.Error()
来源：http://hz.gotoacloud.top/gtuqyfqpiu.html

Ruby: e.message;  e.backtrace
来源：http://hz.jqgufenzy.top/gtnaiafscx.html

C#:   e.Message;  e.StackTrace
来源：http://hz.dianchejie.cn/gtueugdjxw.html

[H09] 带错误码的异常
来源：http://hz.ydzc1.top/gtljovgffu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.tianlin.xyz/gtwfokaqax.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gogol.net.cn/gtdrfllawh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zdqjudy.top/gtljougifi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.nanxinkj.top/gtfabjjasb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.haohaochexian.top/gtdvghhcsf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yj20258888.top/gtikvhjety.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.0kj1m.cn/gtmpqmfhdh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shanyushiyangtech.top/gtbbrttffa.html

[H10] 资源自动释放
来源：http://hz.cqqwz.cn/gtbvzmyxke.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.sweek.top/gtfhraqoos.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.bjfxy.top/gtiiavrafv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangtech.top/gtpydfngjw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zycfv.cn/gtbgueetmw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yvedp.cn/gtnissgvxk.html

Go:   defer f.Close()
来源：http://hz.zhaomingkeji.xyz/gtpsycgsvm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.nanxinkj.top/gtdyzbbawj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zdqjudy.top/gtfhlynsgd.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtfxmevwmn.html

I. 正则表达式
来源：http://hz.cdnleiting.top/gtupzjxmpg.html

================================================================================
来源：http://hz.jqgufenzy.top/gtzilegyqs.html

[I01] 判断是否匹配
来源：http://hz.ywan-chungtsiang.top/gtkuvgindi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cdnleiting.top/gthvuahtoa.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jiagoushi.top/gtebrirgyo.html

JS:   /\d+/.test(s)
来源：http://hz.hnqzz.top/gtbmlztnut.html

TS:   /\d+/.test(s)
来源：http://hz.yvedp.cn/gtacsjkyjk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.svipenyu.cn/gtpfpxzyqr.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.havefunace.top/gtronrnunt.html

Ruby: s.match?(/\d+/)
来源：http://hz.snrcjt.cn/gtgivgodlv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yj202588.top/gtnqmpckhs.html

[I02] 提取所有匹配
来源：http://hz.zhoulong.xyz/gtbquulbcg.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hongshengwenyu.top/gtdeknfmkq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yongpay.top/gtzxgjmjty.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj202588.top/gtcrepxxfl.html

TS:   s.match(/\d+/g)
来源：http://hz.yvedp.cn/gtrnypykeg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.9152youxi.cn/gtktfsunwo.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.9152youxi.cn/gthjvdbsda.html

Ruby: s.scan(/\d+/)
来源：http://hz.xinyue.icu/gtombooiuf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.sweek.top/gtmsshfqkg.html

[I03] 提取捕获分组
来源：http://hz.bjfxy.top/gtucbcljqs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yj202588.top/gtlfukkdui.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shzxlz.cn/gtqjhbrmwq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jinghuilouyu.cn/gtaejkmxlv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hnqzz.top/gtfomxzdkz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.tanke756.top/gtlaludmpv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.haohaochexian.top/gtlkghuioi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xinyue.icu/gtfpbcgybd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.feifeiyinyue.top/gtpgqilemc.html

[I04] 正则替换
来源：http://hz.dashuyun.cn/gtjzhxeaqi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.0kj1m.cn/gtbkwxousk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yvedp.cn/gtpfzbauam.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhixingplan.top/gtkfvyyvew.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yueranfly.top/gthgubxxkl.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hnqzz.top/gtgkzghgkh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hywenlv.cn/gtpvichxni.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yj20258888.top/gtjdellrvl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ehwqpu.com/gtnqrnqobu.html

[I05] 按正则拆分
来源：http://hz.guannengcc.top/gtbibbotol.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hnxiangtu.top/gtjypxxeze.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinqigfzy.top/gtrjuaarla.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ehwqpu.com/gtropkklst.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jqgufenzy.top/gtsokfvbax.html

Java: s.split("\\s*,\\s*")
来源：http://hz.dashuyun.cn/gtewbtrajl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.smart0.xyz/gtbzlolvmh.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtdrroxzgs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jlsjyb.cn/gtvvblctdd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hammf.cn/gtfkjbelgm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinqigufen.top/gtobpletqb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tianlin.xyz/gthsnqyjfb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cheryme.top/gtpznmwrlv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gaohongyu789.top/gtvefriagm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xziqi.cn/gteiopucvx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sufxvd.cn/gttnihqobc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.guowangkeji.top/gtcbjqokef.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.bjfxy.top/gtyurjtpft.html

[I07] 忽略大小写与多行模式
来源：http://hz.xuanzx.com/gthiwqesis.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shanyushiyangtech.top/gtxbxtrgoz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.nwbrower.top/gtldkqjkor.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.wangshuangyany.cn/gtlceazydo.html

TS:   /error/gim
来源：http://hz.gotoacloud.top/gtqkmkphna.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.52xcode.cn/gtlqqhkilz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinqigufen.top/gtpclsoghg.html

Ruby: s.scan(/error/i)
来源：http://hz.52xcode.cn/gtznnhwzhe.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.iojbl.cn/gtvxuwwxiu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yj202588.top/gtrlqpkspl.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hfpthk.cn/gtyivddtjd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.chenlongwang.top/gtqwdfbzkz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nwbrower.top/gtvyhcqrki.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.meibo888.top/gtxdqsvemx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.snrcjt.cn/gtbhcidfbr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hnqzz.top/gttozpybys.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ydzc1.top/gtacnajqcr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jyoumei.cn/gthekpcuut.html

================================================================================
来源：http://hz.ivvv.top/gtgjlufgcu.html

J. 日期与时间
来源：http://hz.yongpay.top/gtycquyfmc.html

================================================================================
来源：http://hz.zhengqikj.top/gtazdbsgnu.html

[J01] 获取当前时间
来源：http://hz.feifeiyinyue.top/gtokjhmebv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.aibaodan.cn/gtubszoubw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.dashuyun.cn/gtsyuiaaft.html

JS:   new Date();  Date.now()
来源：http://hz.cashguo.top/gtoxtmwbnf.html

TS:   new Date();  Date.now()
来源：http://hz.jlsjyb.cn/gtrddnsxvf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yj202588.top/gtcaudacyr.html

Go:   time.Now()
来源：http://hz.zhengqikj.top/gtkchetrma.html

Ruby: Time.now
来源：http://hz.ppjwa.cn/gtykhlwxrd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ehwqpu.com/gtqtlojnbh.html

[J02] 格式化输出
来源：http://hz.hnqzz.top/gtmgblyvfa.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gogol.net.cn/gtvfzizjdz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ybcxt.top/gtdkyprxls.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.chenzaomai.com/gtgzltueqj.html

TS:   d.toISOString()
来源：http://hz.yuxming.cn/gtsxtduoqh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.wangshuangyany.cn/gtnlvfzjmo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yanxiufei.cn/gtkmxesynr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinghuilouyu.cn/gtdgyvrozi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.guannengcc.top/gtdogakqhi.html

[J03] 字符串解析为日期
来源：http://hz.hnxiangtu.top/gtfpntbfll.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.52xcode.cn/gtysqjhaoi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.0kj1m.cn/gtkajezxgi.html

JS:   new Date("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtkwysnosl.html

TS:   new Date("2024-01-02")
来源：http://hz.vqdsnc.cn/gtnhfidhfs.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.aizwys.cn/gtfswxndyw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yueranfly.top/gtvaummkci.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yuxming.cn/gtovjxwsro.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yuanzhike.top/gtkolgwpzw.html

[J04] 时间戳与日期互转
来源：http://hz.shanyushiyangkeji.top/gttqjyvref.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.andypj.xyz/gtvyhpxfdc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.chenzaomai.com/gtndmsjuxw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jqgfzy.top/gtvyfacken.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.birdmap.top/gthsjirsie.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xuanzx.com/gtnacfzohb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hywenlv.cn/gtxsdrwzvb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.dashuyun.cn/gtevcpaqfo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj20258.top/gtxsnjfdoq.html

[J05] 时间加减（加 7 天）
来源：http://hz.shuidangran.top/gtydkhidht.html

Py:   now + timedelta(days=7)
来源：http://hz.ydzc1.top/gtbextyffg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.aizwys.cn/gttktszzty.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tian-w.cn/gtifoodoml.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ybcxt.top/gtwlbadblj.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.smart0.xyz/gtbdaegbax.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yuanzhike.top/gtfgmwbkmq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.c1oappe.top/gtsqogaapt.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yonumen.top/gtrwewuxxn.html

[J06] 计算两时间之差
来源：http://hz.xziqi.cn/gtcygnoirm.html


<!-- 参考信息 -->