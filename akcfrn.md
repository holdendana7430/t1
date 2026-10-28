代发 wailian999

Java: interface Shape { double area(); }
来源：http://hz.hongshengwenyu.top/gtpqxwgjtx.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.9152youxi.cn/gtmtidiyvm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.chenzaomai.com/gttyotyxam.html

C#:   interface IShape { double Area(); }
来源：http://hz.kuanghao11.cn/gtabaunttp.html

[G10] 访问控制
来源：http://hz.jqgufenzy.top/gtzhzelwps.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.nanxinkj.top/gtqctnseyc.html

PHP:  public / protected / private
来源：http://hz.svipenyu.cn/gtetlvfisf.html

JS:   #private 字段；其余公开
来源：http://hz.tanke756.top/gtjcseldve.html

TS:   public / protected / private
来源：http://hz.zdqjudy.top/gtiznaspca.html

Java: public / protected / private / 默认包级
来源：http://hz.yj20258888.top/gtnsdohaer.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.tian-w.cn/gtyxydntrx.html

Ruby: public / protected / private
来源：http://hz.bjfxy.top/gtnrxxvdhu.html

C#:   public / protected / private / internal
来源：http://hz.chenjidiqi.icu/gtsoxtfbmn.html

[G11] getter / setter
来源：http://hz.redwolf501.top/gtzvucjghz.html

Py:   @property 与 @x.setter
来源：http://hz.nwbrower.top/gtxayzdsvc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jlsjyb.cn/gtjcmkkgah.html

JS:   get name() { return this._name; }
来源：http://hz.tian-w.cn/gtvqybrnvt.html

TS:   get name(): string { return this._name; }
来源：http://hz.316326.xyz/gtnniiurxx.html

Java: public String getName() { return name; }
来源：http://hz.cdnleiting.top/gtgncasmkw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ehwqpu.com/gtluozzyiu.html

Ruby: attr_accessor :name
来源：http://hz.zhoulong.xyz/gtrtrzyjto.html

C#:   public string Name { get; set; }
来源：http://hz.9152youxi.cn/gtsqpkbiut.html

[G12] 对象转字符串
来源：http://hz.xziqi.cn/gtxvdajqql.html

Py:   def __str__(self): return self.name
来源：http://hz.mhx1999.top/gtkkfhcvxa.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cqqwz.cn/gtgnvgnpwv.html

JS:   toString() { return this.name; }
来源：http://hz.ivvv.top/gtjqsppeqi.html

TS:   toString(): string { return this.name; }
来源：http://hz.xuanzx.com/gtswkysvun.html

Java: @Override public String toString() { return name; }
来源：http://hz.wangshuangyany.cn/gtpteqawit.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.fzhhl.top/gtygcdvrqu.html

Ruby: def to_s; @name; end
来源：http://hz.guowangkeji.top/gtovurziji.html

C#:   public override string ToString() => Name;
来源：http://hz.nwbrower.top/gtospvrxbc.html

[G13] 判断对象类型
来源：http://hz.fzhhl.top/gtbsrjfuvp.html

Py:   isinstance(u, User)
来源：http://hz.zycfv.cn/gtbhccosej.html

PHP:  $u instanceof User
来源：http://hz.gaohongyu789.top/gtjmyzngoy.html

JS:   u instanceof User
来源：http://hz.yanxiufei.cn/gtqgxaoyah.html

TS:   u instanceof User
来源：http://hz.ivvv.top/gtevltkmqh.html

Java: u instanceof User
来源：http://hz.dashuyun.cn/gtavfbqved.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.yonumen.top/gtfdcctomq.html

Ruby: u.is_a?(User)
来源：http://hz.xinyue.icu/gtetkicgzg.html

C#:   u is User
来源：http://hz.redwolf501.top/gtfcyiayii.html

[G14] 数据类 / record
来源：http://hz.dashuyun.cn/gtjemhcnzr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yuanzhike.top/gtsglsnoir.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shanyushiyangkeji.top/gtdqchskyn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.wangshuangyany.cn/gtcbxxaqdv.html

TS:   type User = { name: string; age: number };
来源：http://hz.redwolf501.top/gtekyglyzs.html

Java: record User(String name, int age) {}
来源：http://hz.jiagoushi.top/gtininxcsl.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cheryme.top/gtwqhmjyky.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.haohaochexian.top/gtqlhovcxa.html

C#:   record User(string Name, int Age);
来源：http://hz.jinqigufen.top/gtrefszoit.html

[G15] 枚举
来源：http://hz.9152youxi.cn/gtzqakvnsf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.sxryk.cn/gtkpmjgdsw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.cashguo.top/gttzfmfdjm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jlsjyb.cn/gtvfinjkfw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xziqi.cn/gtoyxtaxzn.html

Java: enum Color { RED, GREEN }
来源：http://hz.cheryme.top/gtqkxwzute.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinqigufen.top/gtguaiojqd.html

Ruby: Color = %i[red green].freeze
来源：http://hz.sysykeji.top/gtcufuvitr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuanzx.com/gtjezlcqxu.html

[G16] 对象转数组 / 字典
来源：http://hz.fzhhl.top/gtpswrkkua.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.wangshuangyany.cn/gtyttivjjv.html

PHP:  get_object_vars($obj);
来源：http://hz.chenjidiqi.icu/gtivvkqush.html

JS:   Object.entries(obj)
来源：http://hz.hammf.cn/gtrpdjoimf.html

TS:   Object.entries(obj)
来源：http://hz.c1oappe.top/gtvpyammiw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jianghu66.top/gtwclyptrg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hnxiangtu.top/gtplfcmnzx.html

Ruby: obj.instance_variables
来源：http://hz.pycfn.com/gtdhlzmirw.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.havefunace.top/gttydfrhfg.html

================================================================================
来源：http://hz.tian-w.cn/gtvytmlfgk.html

H. 异常与错误处理
来源：http://hz.ybcxt.top/gtvrmpsdyy.html

================================================================================
来源：http://hz.iojbl.cn/gtgjcvpcmg.html

[H01] try / catch 基础
来源：http://hz.smart0.xyz/gtplrbonzt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zdqjudy.top/gtlisoqfyi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zdqjudy.top/gtnyhefhmh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.tanke756.top/gthbijdupm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zdqjudy.top/gtbqhnusxx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.9152youxi.cn/gtzetffebm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.wangshuangyany.cn/gtemjgzayj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.c1oappe.top/gtrvgdffmk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.quarkkingdee.top/gtjojvzidf.html

[H02] finally / ensure 收尾
来源：http://hz.hongshengwenyu.top/gthcyfhmab.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zycfv.cn/gtfunrxcml.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gttukpepdk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hfpthk.cn/gtdzzzkhbv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.tianlin.xyz/gtpuvrbtja.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gtrrhjvvbv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.tanke756.top/gtwisyicjq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shanyushiyangtech.top/gtdjmkiymi.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.nwbrower.top/gtgwgfsldf.html

[H03] 主动抛出异常
来源：http://hz.pengpengdd.cyou/gtpqrrkrto.html

Py:   raise ValueError("错误信息")
来源：http://hz.cucudq.cn/gtqoedrads.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.gotoacloud.top/gtfmsrerpw.html

JS:   throw new Error("错误信息");
来源：http://hz.fengsongda.top/gtwwrxtoak.html

TS:   throw new Error("错误信息");
来源：http://hz.fzhhl.top/gtgklowuwx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cashguo.top/gthizbsjje.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.nanxinkj.top/gtqfgjpmhx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zycfv.cn/gtngmpidpx.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.haohaochexian.top/gtjvxvfckj.html

[H04] 自定义异常类型
来源：http://hz.316326.xyz/gtcovdzkcz.html

Py:   class MyError(Exception): pass
来源：http://hz.pycfn.com/gtdptvoswq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sxryk.cn/gtufvypwdk.html

JS:   class MyError extends Error {}
来源：http://hz.ybcxt.top/gtjqvdkrdz.html

TS:   class MyError extends Error {}
来源：http://hz.birdmap.top/gtblbttbph.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ehwqpu.com/gtxfcabvsc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.tian-w.cn/gtzlfbxals.html

Ruby: class MyError < StandardError; end
来源：http://hz.pycfn.com/gtsulwycqt.html

C#:   class MyException : Exception {}
来源：http://hz.shanyushiyangkeji.top/gtvfomnliq.html

[H05] 捕获特定类型
来源：http://hz.bjfxy.top/gtvxfcuwmk.html

Py:   except ValueError as e:
来源：http://hz.yj20258888.top/gtbnxuyxmq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hongshengwenyu.top/gtfegfidwc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zdqjudy.top/gtahhczike.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhaomingkeji.xyz/gtcwvmbndz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.aizwys.cn/gtppehyuil.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gogol.net.cn/gtudsyxaxd.html

Ruby: rescue ArgumentError => e
来源：http://hz.jianghu66.top/gtzygmumud.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinqigfzy.top/gtshkckfzp.html

[H06] 可选值 / 空值安全访问
来源：http://hz.fengsongda.top/gtckqnwycj.html

Py:   value = d.get("k") or default
来源：http://hz.nwbrower.top/gtebrfuibo.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhiwuduotai.top/gteqgzealt.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sysykeji.top/gtxscplpvp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxuanxn.top/gtixkktfrr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ehwqpu.com/gtqymagxye.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cucudq.cn/gtkxevkelk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yanxiufei.cn/gtwkrpihsm.html

C#:   obj?.A?.B ?? default
来源：http://hz.ywan-chungtsiang.top/gtngfngker.html

[H07] 断言
来源：http://hz.ppjwa.cn/gtootpaufb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hfpthk.cn/gtbnamqdit.html

PHP:  assert($x > 0);
来源：http://hz.aizwys.cn/gtjavdosip.html

JS:   console.assert(x > 0);
来源：http://hz.316326.xyz/gtjyswozim.html

TS:   console.assert(x > 0);
来源：http://hz.jiagoushi.top/gtdofelyya.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sufxvd.cn/gtqvabuaja.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.316326.xyz/gtessgkvsp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.dashuyun.cn/gtebfblaoe.html

C#:   Debug.Assert(x > 0);
来源：http://hz.tian-w.cn/gtwpwbskhn.html

[H08] 获取错误信息与堆栈
来源：http://hz.0kj1m.cn/gtlcsnjibl.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.pengpengdd.cyou/gtrlkhhwsg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jianghu66.top/gtshxabalg.html

JS:   e.message;  e.stack
来源：http://hz.yj20258.top/gtdyjvpfmy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shanyushiyangtech.top/gttyrcnrcd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hongshengwenyu.top/gtrjtrpmoy.html

Go:   err.Error()
来源：http://hz.nanxinkj.top/gtngzapjxz.html

Ruby: e.message;  e.backtrace
来源：http://hz.ydzc1.top/gtudohgkja.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hywenlv.cn/gtpsgsazij.html

[H09] 带错误码的异常
来源：http://hz.yvedp.cn/gtoiulinmm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.dashuyun.cn/gtqkhuasde.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhoulong.xyz/gtpghgfubm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gaohongyu789.top/gtqhvbgegi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.aibaodan.cn/gtowhbpyzw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj20258.top/gtcakyqboq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ppjwa.cn/gtieaxefpv.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yongpay.top/gtegdaquml.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gotoacloud.top/gttoufnzvo.html

[H10] 资源自动释放
来源：http://hz.feifeiyinyue.top/gteedyotsb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jlsjyb.cn/gtnrymlodb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.chenjidiqi.icu/gteshicvvb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.daria6918.cn/gtgpatcyli.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tanke756.top/gtitgbgctm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.guannengcc.top/gtqjknyrlp.html

Go:   defer f.Close()
来源：http://hz.dashuyun.cn/gtlzuvgiul.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.guannengcc.top/gtckurmpsc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zdqjudy.top/gtvvumyoiw.html

================================================================================
来源：http://hz.52xcode.cn/gtyaklyfnl.html

I. 正则表达式
来源：http://hz.zhixingplan.top/gtzxhbgqpb.html

================================================================================
来源：http://hz.svipenyu.cn/gttumjfvss.html

[I01] 判断是否匹配
来源：http://hz.wangshuangyany.cn/gtkkvoewmi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.smart0.xyz/gtyonfmqmt.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhoulong.xyz/gtujyueibm.html

JS:   /\d+/.test(s)
来源：http://hz.cheryme.top/gtfvbekwtk.html

TS:   /\d+/.test(s)
来源：http://hz.iojbl.cn/gtsstvyqmp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhixingplan.top/gtdwimlyrw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.gotoacloud.top/gtmauwdzul.html

Ruby: s.match?(/\d+/)
来源：http://hz.ppjwa.cn/gtjjxlfumr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinyuanbaomall.cn/gtzkwrezdg.html

[I02] 提取所有匹配
来源：http://hz.haohaochexian.top/gtqbyqeyut.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hysaishi.cn/gtwmglefyx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cucudq.cn/gthfgrvfpu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhiwuduotai.top/gtdjbixeua.html

TS:   s.match(/\d+/g)
来源：http://hz.fzhhl.top/gtpnmgqewc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.havefunace.top/gtcocknlno.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhoulong.xyz/gtneivfteo.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhijiandao.cn/gtnzbdzfmq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xuanzx.com/gtxovseiql.html

[I03] 提取捕获分组
来源：http://hz.feifeiyinyue.top/gtldkeepqr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jinqigufen.top/gtfhsdadwo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shangyingyoupin.top/gtkntqcajl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xziqi.cn/gtdhwadnpx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yueranfly.top/gtyorttsai.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.tanke756.top/gttedpqmgd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cdnleiting.top/gtvevgncgr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hywenlv.cn/gtfhdwvamu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xziqi.cn/gtogszvqrb.html

[I04] 正则替换
来源：http://hz.cashguo.top/gtnlgyjxal.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gzhubu.top/gtevwtkuhd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.0kj1m.cn/gtmdhoqljo.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ehwqpu.com/gtmpsahafr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.daxiang520.top/gtzvsputiu.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hammf.cn/gtbbxtzkwx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ivvv.top/gtizcpnmrr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ydzc1.top/gtmgvsucib.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hnqzz.top/gtvjcyfvqg.html

[I05] 按正则拆分
来源：http://hz.gzhubu.top/gtxpjbwdcv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yvedp.cn/gtqnbaobdp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.fzhhl.top/gtakovskwx.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhengqikj.top/gtmjdsnlqf.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xingfuxueyuan.xyz/gtapzpinju.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shzxlz.cn/gtbnqrrfrk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.nanxuanxn.top/gtzzrvryny.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.aibaodan.cn/gtwleovgpn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.fengsongda.top/gtqmuguiaa.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jinghuilouyu.cn/gtbbkqxuvm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jianghu66.top/gtyqwoqjkc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.nwbrower.top/gtwnqrvniz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnqzz.top/gtuqkkxyrf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.0kj1m.cn/gtanuvjxgf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.kuanghao11.cn/gtwoclcuri.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xuanzx.com/gtvijellcd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.quarkkingdee.top/gtdkrxeinr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hnqzz.top/gtkxmemlhe.html

[I07] 忽略大小写与多行模式
来源：http://hz.tian-w.cn/gtkkaxpbbx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.aibaodan.cn/gtzxaamxiz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhijiandao.cn/gtfiazgbhd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhoulong.xyz/gtbddvwagc.html

TS:   /error/gim
来源：http://hz.tian-w.cn/gtyuvhfqdx.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hnxiangtu.top/gtgquggqae.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhixingplan.top/gtqkgenkpv.html

Ruby: s.scan(/error/i)
来源：http://hz.jqgfzy.top/gtjiafklrz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.snrcjt.cn/gtjcymobrh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinqigufen.top/gtomajzsrd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.shanyushiyangtech.top/gtjvnuqwea.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.fengsongda.top/gtnyiiogjz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.meibo888.top/gtbnbujnpd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.snrcjt.cn/gtojfyesnc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sysykeji.top/gticbghyyk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xuanzx.com/gtclaacvcu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.nwbrower.top/gtoztdyjpo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.dianchejie.cn/gtvmdchwws.html

================================================================================
来源：http://hz.jiagoushi.top/gtmefnrzwt.html

J. 日期与时间
来源：http://hz.guowangkeji.top/gtlunimsvu.html

================================================================================
来源：http://hz.sysykeji.top/gtodgfcxqw.html

[J01] 获取当前时间
来源：http://hz.tanke756.top/gtttytnnzt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ppjwa.cn/gtrividkcp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xinyue.icu/gtuccioofi.html

JS:   new Date();  Date.now()
来源：http://hz.shzxlz.cn/gtbdfehqaz.html

TS:   new Date();  Date.now()
来源：http://hz.cucudq.cn/gtwpfsoqxb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinqigufen.top/gtptahgxpp.html

Go:   time.Now()
来源：http://hz.9152youxi.cn/gtkvlmuyyk.html

Ruby: Time.now
来源：http://hz.feifeiyinyue.top/gtedxlwcgw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.quarkkingdee.top/gtswschjiw.html

[J02] 格式化输出
来源：http://hz.sxryk.cn/gtmyxuizss.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sufxvd.cn/gtdogmewso.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.meibo888.top/gtnjmdraoq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hnqzz.top/gtzyhzzfon.html

TS:   d.toISOString()
来源：http://hz.gzhubu.top/gtlnnhlrqs.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yvedp.cn/gtreyxueza.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ywan-chungtsiang.top/gtuzdhzxnd.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shzxlz.cn/gtkyvtxbid.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinyuanbaomall.cn/gtabrgnajq.html

[J03] 字符串解析为日期
来源：http://hz.gotoacloud.top/gtecopmbsq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.tianlin.xyz/gtleumkjbh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jqgufenzy.top/gtayaxbvpe.html

JS:   new Date("2024-01-02")
来源：http://hz.zhixingplan.top/gtcaqzzsvm.html

TS:   new Date("2024-01-02")
来源：http://hz.svipenyu.cn/gtjkzxqzcd.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sysykeji.top/gthfaodwik.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtwkvytwef.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.dashuyun.cn/gtkkirmwsf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nanxuanxn.top/gthqqkbcpk.html

[J04] 时间戳与日期互转
来源：http://hz.smart0.xyz/gtlnqthnkl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.9152youxi.cn/gtbakwsufw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.vqdsnc.cn/gtjenreejx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ywan-chungtsiang.top/gtoojyzraf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jyoumei.cn/gtuddjyzcw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.mhx1999.top/gtsihndwku.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.guannengcc.top/gtqkiwbwam.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shangyingyoupin.top/gtvdiffisp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.sufxvd.cn/gtywpwgurw.html

[J05] 时间加减（加 7 天）
来源：http://hz.jinqigfzy.top/gtickqozug.html

Py:   now + timedelta(days=7)
来源：http://hz.wangdashe.top/gtpzwupjad.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shanyushiyangtech.top/gtjjihiepw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yongpay.top/gtkmmmyhbt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.meibo888.top/gtbnyahiut.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.0kj1m.cn/gtbgsmlbqa.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.nwbrower.top/gtiosvtdwb.html

Ruby: Time.now + 7 * 86400
来源：http://hz.dashuyun.cn/gthwbyyixd.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.gotoacloud.top/gtobmtaqox.html

[J06] 计算两时间之差
来源：http://hz.mhx1999.top/gtymascqcj.html

Py:   (end - start).total_seconds()
来源：http://hz.zhoulong.xyz/gtseanvdrm.html

PHP:  $end->diff($start)->days;
来源：http://hz.havefunace.top/gtqfmeffpq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.cdnleiting.top/gtaszsxowa.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.svipenyu.cn/gtjpmjamjp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hongshengwenyu.top/gtltqdzvff.html

Go:   end.Sub(start).Hours()
来源：http://hz.ehwqpu.com/gtaaniqljz.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenzaomai.com/gtvspmuzjx.html

C#:   (end - start).TotalSeconds
来源：http://hz.jlsjyb.cn/gtvknrdivl.html

[J07] 比较两个日期
来源：http://hz.xziqi.cn/gtzzuosfem.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gtkufmuvzb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yvedp.cn/gtzvdnxtvb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.wangdashe.top/gtkvrwmcbc.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cashguo.top/gtynkvwrlf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.aibaodan.cn/gtbukfvriq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.guowangkeji.top/gtentznplk.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinyuanbaomall.cn/gtkufxujdc.html


<!-- 参考信息 -->