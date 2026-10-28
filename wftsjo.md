代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://hz.mhx1999.top/gtgchwarqg.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.havefunace.top/gtptekfqaa.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.dashuyun.cn/gtwvanrghp.html

TS:   interface Shape { area(): number; }
来源：http://hz.yuanzhike.top/gtrjmagegx.html

Java: interface Shape { double area(); }
来源：http://hz.iojbl.cn/gtjbymxkzj.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yj20258.top/gtjzflrjlh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xylfe.cn/gtgzqzmwhj.html

C#:   interface IShape { double Area(); }
来源：http://hz.dianchejie.cn/gtrtvhkrga.html

[G10] 访问控制
来源：http://hz.yueranfly.top/gtisztbopp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.52xcode.cn/gtrwutnaad.html

PHP:  public / protected / private
来源：http://hz.gogol.net.cn/gtkmseaorh.html

JS:   #private 字段；其余公开
来源：http://hz.snrcjt.cn/gtbnujqrnz.html

TS:   public / protected / private
来源：http://hz.chenzaomai.com/gtxgjwbxii.html

Java: public / protected / private / 默认包级
来源：http://hz.ydzc1.top/gtquvnwlps.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhengqikj.top/gtkuanulxg.html

Ruby: public / protected / private
来源：http://hz.aizwys.cn/gtkyuvuyix.html

C#:   public / protected / private / internal
来源：http://hz.nanxuanxn.top/gthckzfzki.html

[G11] getter / setter
来源：http://hz.gogol.net.cn/gtipeadbgj.html

Py:   @property 与 @x.setter
来源：http://hz.gaohongyu789.top/gtvadwemau.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yongpay.top/gtcmxduzlk.html

JS:   get name() { return this._name; }
来源：http://hz.zhengqikj.top/gtgcgrmbjp.html

TS:   get name(): string { return this._name; }
来源：http://hz.yuxming.cn/gtutsvqqbs.html

Java: public String getName() { return name; }
来源：http://hz.guowangkeji.top/gtvwpfctfd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yonumen.top/gtqchjrgam.html

Ruby: attr_accessor :name
来源：http://hz.gogol.net.cn/gtdylpawiv.html

C#:   public string Name { get; set; }
来源：http://hz.jqgufenzy.top/gtwydwjefo.html

[G12] 对象转字符串
来源：http://hz.yongpay.top/gtxhyiqkuh.html

Py:   def __str__(self): return self.name
来源：http://hz.xinyue.icu/gtommpwwtd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hnxiangtu.top/gtcxkhdorf.html

JS:   toString() { return this.name; }
来源：http://hz.0kj1m.cn/gtwzppgabp.html

TS:   toString(): string { return this.name; }
来源：http://hz.yj202588.top/gtrwmzrjel.html

Java: @Override public String toString() { return name; }
来源：http://hz.52xcode.cn/gtfnprqldl.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.pengpengdd.cyou/gtdheyehjr.html

Ruby: def to_s; @name; end
来源：http://hz.daria6918.cn/gtuniymrpk.html

C#:   public override string ToString() => Name;
来源：http://hz.hnqzz.top/gtovechhcu.html

[G13] 判断对象类型
来源：http://hz.zhijiandao.cn/gtlnusufiv.html

Py:   isinstance(u, User)
来源：http://hz.svipenyu.cn/gtlgrtgera.html

PHP:  $u instanceof User
来源：http://hz.daria6918.cn/gtviaebvlk.html

JS:   u instanceof User
来源：http://hz.zycfv.cn/gtotwtxufw.html

TS:   u instanceof User
来源：http://hz.havefunace.top/gtemdbhnwc.html

Java: u instanceof User
来源：http://hz.bjfxy.top/gtupqurwpm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yangfankeji.com/gtnldtmkyd.html

Ruby: u.is_a?(User)
来源：http://hz.gogol.net.cn/gtmusetoqp.html

C#:   u is User
来源：http://hz.haohaochexian.top/gtecqmapiw.html

[G14] 数据类 / record
来源：http://hz.xylfe.cn/gtsurlbznq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.guannengcc.top/gtrbbscqof.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yonumen.top/gtloxfagmj.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cdnleiting.top/gtudhnmrrv.html

TS:   type User = { name: string; age: number };
来源：http://hz.pycfn.com/gtljygbxsx.html

Java: record User(String name, int age) {}
来源：http://hz.hysaishi.cn/gtiypaoezs.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xuanzx.com/gtbvwekosx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sweek.top/gtgwmrevzq.html

C#:   record User(string Name, int Age);
来源：http://hz.sxryk.cn/gttmsvrnus.html

[G15] 枚举
来源：http://hz.zhaomingkeji.xyz/gtnajfwadk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.sxryk.cn/gtsznowbyv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.kuanghao11.cn/gtwaufbcuv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.dianchejie.cn/gthealrumo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinghuilouyu.cn/gtuuddsgca.html

Java: enum Color { RED, GREEN }
来源：http://hz.smart0.xyz/gttbhzwmgg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.fzhhl.top/gtoxikdimp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.aibaodan.cn/gtvyidezoe.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yueranfly.top/gtimmalpoy.html

[G16] 对象转数组 / 字典
来源：http://hz.gogol.net.cn/gtpguhwdwh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ybcxt.top/gtzxvrdlxp.html

PHP:  get_object_vars($obj);
来源：http://hz.fengsongda.top/gtxydsepto.html

JS:   Object.entries(obj)
来源：http://hz.chenlongwang.top/gtwaxbemmu.html

TS:   Object.entries(obj)
来源：http://hz.zhaomingkeji.xyz/gtqzaoilzo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shangyingyoupin.top/gtsfhopvgd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.bjfxy.top/gttmculega.html

Ruby: obj.instance_variables
来源：http://hz.zhengqikj.top/gtasgkuwkm.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.dianchejie.cn/gtjkywfdco.html

================================================================================
来源：http://hz.jqgufenzy.top/gthnmepfzr.html

H. 异常与错误处理
来源：http://hz.snrcjt.cn/gtkkwqfgxc.html

================================================================================
来源：http://hz.xziqi.cn/gtlzilvjxm.html

[H01] try / catch 基础
来源：http://hz.jianghu66.top/gtwnbfhntj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.tanke756.top/gtdpurmcpq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.316326.xyz/gtmsmuddaq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.svipenyu.cn/gtvqbhrciv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yj20258888.top/gtrllmtkrf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cucudq.cn/gtojwcywyz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.daria6918.cn/gtcrevaxkf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jianghu66.top/gtveyvbzbe.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gzhubu.top/gtgrkglvns.html

[H02] finally / ensure 收尾
来源：http://hz.shuidangran.top/gtsjwrljse.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jinyuanbaomall.cn/gtzcejygwf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtpdqfhten.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hywenlv.cn/gtgbdoamer.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cdnleiting.top/gttlvpkqhz.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gtifoobppb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.gogol.net.cn/gtdqejvyoq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hongshengwenyu.top/gthumnkvax.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xuanzx.com/gtcicmkwhd.html

[H03] 主动抛出异常
来源：http://hz.sysykeji.top/gthvbcqhvb.html

Py:   raise ValueError("错误信息")
来源：http://hz.jinqigufen.top/gtnyzmavhu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.sufxvd.cn/gtsrwzyocf.html

JS:   throw new Error("错误信息");
来源：http://hz.ydjk.org.cn/gtfphuvapl.html

TS:   throw new Error("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtejrgekfl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.shanyushiyangtech.top/gtngjopfie.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yueranfly.top/gtbfrpscbh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gogol.net.cn/gtcwilxpow.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.52xcode.cn/gtpuvvzzsc.html

[H04] 自定义异常类型
来源：http://hz.shanyushiyangkeji.top/gttfttnrte.html

Py:   class MyError(Exception): pass
来源：http://hz.cheryme.top/gtnhamnapl.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yangfankeji.com/gtfhsjwrcd.html

JS:   class MyError extends Error {}
来源：http://hz.guannengcc.top/gtdgcfvqtj.html

TS:   class MyError extends Error {}
来源：http://hz.52xcode.cn/gtwgekekrn.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jinghuilouyu.cn/gtjixtwgtv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jianghu66.top/gtxymfvnck.html

Ruby: class MyError < StandardError; end
来源：http://hz.zdqjudy.top/gtvzpjpshl.html

C#:   class MyException : Exception {}
来源：http://hz.sxryk.cn/gtbnfrjfdu.html

[H05] 捕获特定类型
来源：http://hz.yvedp.cn/gtjeecybjc.html

Py:   except ValueError as e:
来源：http://hz.guannengcc.top/gtdbpiskhc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xingfuxueyuan.xyz/gthrjtpefv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.dashuyun.cn/gtrmyrtout.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hywenlv.cn/gtdgrfxyfz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jqgufenzy.top/gtjrakytbq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.daxiang520.top/gtelrdegfl.html

Ruby: rescue ArgumentError => e
来源：http://hz.cqqwz.cn/gtaytzumvc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jyoumei.cn/gtdjhcfraw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hywenlv.cn/gthponnctl.html

Py:   value = d.get("k") or default
来源：http://hz.jlsjyb.cn/gtfcroszqm.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.smart0.xyz/gtbbbsleld.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.chenjidiqi.icu/gtpqqiymdg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yuanzhike.top/gtmqgeiuyi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.aibaodan.cn/gtnmmipwfa.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.gaohongyu789.top/gtgfycrunm.html

Ruby: d&.dig(:a, :b)
来源：http://hz.fzhhl.top/gtdvpraxsk.html

C#:   obj?.A?.B ?? default
来源：http://hz.xuanzx.com/gtvalnrubd.html

[H07] 断言
来源：http://hz.shangyingyoupin.top/gtbltxdcbi.html

Py:   assert x > 0, "必须为正"
来源：http://hz.c1oappe.top/gtqvmgxhyl.html

PHP:  assert($x > 0);
来源：http://hz.snrcjt.cn/gtqcxnuwev.html

JS:   console.assert(x > 0);
来源：http://hz.shanyushiyangkeji.top/gtrmrtjyup.html

TS:   console.assert(x > 0);
来源：http://hz.dashuyun.cn/gtxeyziswe.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhijiandao.cn/gtrjodsqpk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhoulong.xyz/gtgbquthjj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.shanyushiyangtech.top/gtkobbcjam.html

C#:   Debug.Assert(x > 0);
来源：http://hz.vqdsnc.cn/gtvdjiotjk.html

[H08] 获取错误信息与堆栈
来源：http://hz.yongpay.top/gtsejpbhrt.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.0kj1m.cn/gtlenojxpd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.snrcjt.cn/gtnrjccxli.html

JS:   e.message;  e.stack
来源：http://hz.ehwqpu.com/gtdbgyoyif.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gogol.net.cn/gtnpovffts.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xuanzx.com/gtjplxjlsp.html

Go:   err.Error()
来源：http://hz.chenlongwang.top/gttnxdbsbt.html

Ruby: e.message;  e.backtrace
来源：http://hz.chenjidiqi.icu/gtebwbcqet.html

C#:   e.Message;  e.StackTrace
来源：http://hz.dianchejie.cn/gtfjeoelbf.html

[H09] 带错误码的异常
来源：http://hz.aizwys.cn/gtxqmngket.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.tianlin.xyz/gtqfezxryz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hfpthk.cn/gtaxldbtqi.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.redwolf501.top/gteyaksxks.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yueranfly.top/gthwojrhml.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.fengsongda.top/gtgvzngmzt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhengqikj.top/gtdhfbqbko.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.chenjidiqi.icu/gtmqreyyqq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.birdmap.top/gtsblqefrj.html

[H10] 资源自动释放
来源：http://hz.hongshengwenyu.top/gtdeeehidw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jinyuanbaomall.cn/gtpoxhasxz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.bjfxy.top/gtmbwaldzi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.redwolf501.top/gtwmnptbii.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aizwys.cn/gtcfisybuq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jinqigufen.top/gtppnvrfjb.html

Go:   defer f.Close()
来源：http://hz.yuxming.cn/gtgttbkzet.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinghuilouyu.cn/gtdvvgznix.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xinyue.icu/gtcicvgkvd.html

================================================================================
来源：http://hz.nanxuanxn.top/gtpescnufb.html

I. 正则表达式
来源：http://hz.jqgufenzy.top/gtmncqvmlb.html

================================================================================
来源：http://hz.jqgufenzy.top/gtvozifmdx.html

[I01] 判断是否匹配
来源：http://hz.hnqzz.top/gtbetuhodu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xuanzx.com/gtzndkadei.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.guowangkeji.top/gtdlvaptiq.html

JS:   /\d+/.test(s)
来源：http://hz.quarkkingdee.top/gtylhppctn.html

TS:   /\d+/.test(s)
来源：http://hz.zhoulong.xyz/gtmeofwxoo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cashguo.top/gtnslkgopt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jinghuilouyu.cn/gthvfessno.html

Ruby: s.match?(/\d+/)
来源：http://hz.yj20258888.top/gtiaexkbnr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sweek.top/gtrhvdwlru.html

[I02] 提取所有匹配
来源：http://hz.bjfxy.top/gtzbdtkyhf.html

Py:   re.findall(r"\d+", s)
来源：http://hz.bjfxy.top/gtjxylpuxy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.52xcode.cn/gtsblyhbvw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.daxiang520.top/gtfqdjjoox.html

TS:   s.match(/\d+/g)
来源：http://hz.ppjwa.cn/gtmvotkvlv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hnxiangtu.top/gthjmafkdb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hongshengwenyu.top/gtvcaqgmqt.html

Ruby: s.scan(/\d+/)
来源：http://hz.cdnleiting.top/gtvoiaawuk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.smart0.xyz/gtkspvozxj.html

[I03] 提取捕获分组
来源：http://hz.gaohongyu789.top/gtvfwrvadc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yuxming.cn/gtfcopwyaa.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.tian-w.cn/gtbyvcrxmq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.tanke756.top/gtleufjoqx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jqgfzy.top/gtgiadqwhr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhiwuduotai.top/gtsxgujbsd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhijiandao.cn/gtemschnti.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shanyushiyangkeji.top/gttasjypki.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.shuidangran.top/gtntjtcsbk.html

[I04] 正则替换
来源：http://hz.yj20258.top/gtadaxanyc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.haohaochexian.top/gtmpmumowm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj20258.top/gtffkilrfu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cqqwz.cn/gtaepynpvl.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zdqjudy.top/gtaqyptwgw.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.havefunace.top/gtvtwmeuvk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.svipenyu.cn/gtiiipzirb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.birdmap.top/gttxjztxcp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.snrcjt.cn/gtblzdihqn.html

[I05] 按正则拆分
来源：http://hz.jiagoushi.top/gtikrgxdqg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.52xcode.cn/gtctefpbyt.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hammf.cn/gttcabkczr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xuetiantiany.cn/gtodoefnvh.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ydzc1.top/gtiezkcygw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shangyingyoupin.top/gthrcykaxt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jinqigfzy.top/gtmlmbbquq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gthdomhgsp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.bjfxy.top/gtdtgvpvvk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.fzhhl.top/gtcfuimbzz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.52xcode.cn/gtvkfmeqfp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.52xcode.cn/gtjaxblvjt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gzhubu.top/gtiutrxpui.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shuidangran.top/gtbivdfbkw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.0kj1m.cn/gtaezrubej.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.guannengcc.top/gtqrcykqwf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.redwolf501.top/gtohsytpas.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hywenlv.cn/gtaeyeutpb.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhijiandao.cn/gtimksrdjs.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cashguo.top/gtxewkqvxs.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yuanzhike.top/gtpzcalwnd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zycfv.cn/gtzcpqbbpb.html

TS:   /error/gim
来源：http://hz.xingfuxueyuan.xyz/gtkbiuczvs.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yvedp.cn/gtgshjbhcq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinyuanbaomall.cn/gtnndqroal.html

Ruby: s.scan(/error/i)
来源：http://hz.hnqzz.top/gtsdujkccz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj20258888.top/gtqdeidlil.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xuetiantiany.cn/gtphhtoian.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.nanxinkj.top/gtbdjzsbnl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.nwbrower.top/gtdfqelinr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tianlin.xyz/gthmxkappe.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ywan-chungtsiang.top/gtkxbdstyc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.guowangkeji.top/gtangnxdrq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jyoumei.cn/gtzsxqzopq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yongpay.top/gtkdkigyxw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ydzc1.top/gtaffqaaty.html

================================================================================
来源：http://hz.birdmap.top/gtukeyojul.html

J. 日期与时间
来源：http://hz.0kj1m.cn/gtsboggjxu.html

================================================================================
来源：http://hz.52xcode.cn/gtvexhcpur.html

[J01] 获取当前时间
来源：http://hz.gaohongyu789.top/gtkjrhqxek.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenjidiqi.icu/gtgemltxky.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.aibaodan.cn/gtcqiwqrwo.html

JS:   new Date();  Date.now()
来源：http://hz.cucudq.cn/gtpqyxxvaf.html

TS:   new Date();  Date.now()
来源：http://hz.hnqzz.top/gtnjaaokyf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ybcxt.top/gtmdxzyvic.html

Go:   time.Now()
来源：http://hz.aibaodan.cn/gtjzlzxafl.html

Ruby: Time.now
来源：http://hz.gotoacloud.top/gtabtqitnt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.sufxvd.cn/gtavkapgcj.html

[J02] 格式化输出
来源：http://hz.ybcxt.top/gtazluidrq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jlsjyb.cn/gtikimosqj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.tian-w.cn/gtunqfohex.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.aizwys.cn/gtjifbjfsg.html

TS:   d.toISOString()
来源：http://hz.hammf.cn/gtvrcyipwc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hnxiangtu.top/gtzpbtpdmu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.nwbrower.top/gtynluomzt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dianchejie.cn/gtsdlstemu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cheryme.top/gtjvrvgpoo.html

[J03] 字符串解析为日期
来源：http://hz.yuanzhike.top/gtxuckiqwp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.gotoacloud.top/gtoaiizdqf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xuanzx.com/gtbdlegstj.html

JS:   new Date("2024-01-02")
来源：http://hz.jinqigufen.top/gtrefprfwr.html

TS:   new Date("2024-01-02")
来源：http://hz.aibaodan.cn/gtrbzokkff.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cheryme.top/gtujjqlnjx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hammf.cn/gtxiftyulz.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.wangshuangyany.cn/gtswkdxvsp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.mhx1999.top/gtqihkrvxn.html

[J04] 时间戳与日期互转
来源：http://hz.yj202588.top/gtjswsnlev.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.svipenyu.cn/gtpeovzeqw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.9152youxi.cn/gtyipyjkvk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.nwbrower.top/gtsymwzhcx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yongpay.top/gthtdthnxu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xylfe.cn/gtbcowryqm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shanyushiyangtech.top/gttjdtddnq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xingfuxueyuan.xyz/gtajclqkaj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cucudq.cn/gtjciftyvg.html

[J05] 时间加减（加 7 天）
来源：http://hz.yuanzhike.top/gtlavlaoor.html

Py:   now + timedelta(days=7)
来源：http://hz.pengpengdd.cyou/gtqdmhexty.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yuanzhike.top/gtegwbaqhm.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.havefunace.top/gtyqmbswdu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yuxming.cn/gtzqdjwnyr.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yuxming.cn/gtuwupvavv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.chenzaomai.com/gtipmwuezl.html

Ruby: Time.now + 7 * 86400
来源：http://hz.nanxuanxn.top/gtpqgmeyiq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.0kj1m.cn/gtrfqaidel.html

[J06] 计算两时间之差
来源：http://hz.hywenlv.cn/gtwrhowaxp.html

Py:   (end - start).total_seconds()
来源：http://hz.dashuyun.cn/gtddtkuhrc.html

PHP:  $end->diff($start)->days;
来源：http://hz.c1oappe.top/gtvkrqgjxl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.svipenyu.cn/gtgjtvwbkx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhixingplan.top/gttxpvpneb.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jqgufenzy.top/gtzeiqwboj.html

Go:   end.Sub(start).Hours()
来源：http://hz.svipenyu.cn/gtdwkxrcvf.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jinqigfzy.top/gtuwjnwdit.html

C#:   (end - start).TotalSeconds
来源：http://hz.cheryme.top/gtfiweaxdf.html

[J07] 比较两个日期
来源：http://hz.yj202588.top/gtkpcvkgra.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yonumen.top/gtrxwlvbqu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yangfankeji.com/gtxcazbced.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shuidangran.top/gtcstwuepj.html


<!-- 参考信息 -->