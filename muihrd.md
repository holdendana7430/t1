代发 wailian999

TS:   public / protected / private
来源：http://hz.jinqigfzy.top/gtndxnsgmi.html

Java: public / protected / private / 默认包级
来源：http://hz.tian-w.cn/gtyumqaljl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.andypj.xyz/gtncaidecj.html

Ruby: public / protected / private
来源：http://hz.yonumen.top/gtdvwgclcs.html

C#:   public / protected / private / internal
来源：http://hz.gotoacloud.top/gtyszyvkdb.html

[G11] getter / setter
来源：http://hz.mhx1999.top/gtkqyefelt.html

Py:   @property 与 @x.setter
来源：http://hz.gaohongyu789.top/gtjopglsoe.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhengqikj.top/gtcmijehzo.html

JS:   get name() { return this._name; }
来源：http://hz.fzhhl.top/gtpfhntxaz.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhoulong.xyz/gtdrfvevdc.html

Java: public String getName() { return name; }
来源：http://hz.birdmap.top/gtrxeukidp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ywan-chungtsiang.top/gtxsvjeazi.html

Ruby: attr_accessor :name
来源：http://hz.chenzaomai.com/gtrtdfmgck.html

C#:   public string Name { get; set; }
来源：http://hz.zycfv.cn/gtfkhtemcf.html

[G12] 对象转字符串
来源：http://hz.hongshengwenyu.top/gtxsolkdis.html

Py:   def __str__(self): return self.name
来源：http://hz.gaohongyu789.top/gtbxfxmipu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yj20258888.top/gtkehbelgv.html

JS:   toString() { return this.name; }
来源：http://hz.tian-w.cn/gthelhllss.html

TS:   toString(): string { return this.name; }
来源：http://hz.vqdsnc.cn/gtwxkhuxqh.html

Java: @Override public String toString() { return name; }
来源：http://hz.jlsjyb.cn/gtwbocsqql.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhiwuduotai.top/gtgepgpbpw.html

Ruby: def to_s; @name; end
来源：http://hz.cqqwz.cn/gtyvaadxgw.html

C#:   public override string ToString() => Name;
来源：http://hz.shzxlz.cn/gtjujzrzlb.html

[G13] 判断对象类型
来源：http://hz.hnqzz.top/gtjqubfvcx.html

Py:   isinstance(u, User)
来源：http://hz.hysaishi.cn/gtivunvtgl.html

PHP:  $u instanceof User
来源：http://hz.pengpengdd.cyou/gttejmfqtp.html

JS:   u instanceof User
来源：http://hz.jqgfzy.top/gtidhzgjff.html

TS:   u instanceof User
来源：http://hz.havefunace.top/gtmvsuinbo.html

Java: u instanceof User
来源：http://hz.wangshuangyany.cn/gtzxksykar.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ppjwa.cn/gtxchfulru.html

Ruby: u.is_a?(User)
来源：http://hz.pengpengdd.cyou/gtsxjmmbgz.html

C#:   u is User
来源：http://hz.sxryk.cn/gtaxpdxhwr.html

[G14] 数据类 / record
来源：http://hz.zhixingplan.top/gtvtpyapra.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhiwuduotai.top/gtzpmajxea.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.chenlongwang.top/gttyhhyfer.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yueranfly.top/gtkdrdfsdk.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhengqikj.top/gtqlkwymmo.html

Java: record User(String name, int age) {}
来源：http://hz.quarkkingdee.top/gtouatguia.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yj20258888.top/gtcxkzrcym.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.gogol.net.cn/gtzwrnpvmd.html

C#:   record User(string Name, int Age);
来源：http://hz.zhongyouzk.top/gtossqtqbq.html

[G15] 枚举
来源：http://hz.hysaishi.cn/gtjzkolyeg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.daria6918.cn/gtskuoavxo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xziqi.cn/gtidikfcxi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cashguo.top/gtjxomrfyf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.aibaodan.cn/gtiynhwknw.html

Java: enum Color { RED, GREEN }
来源：http://hz.cqqwz.cn/gtyflweokl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhijiandao.cn/gtqqisnmpv.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yuxming.cn/gtxltitxae.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnxiangtu.top/gtuhydingy.html

[G16] 对象转数组 / 字典
来源：http://hz.ywan-chungtsiang.top/gtybljparh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cheryme.top/gtvstinxhm.html

PHP:  get_object_vars($obj);
来源：http://hz.jiagoushi.top/gtfwocergr.html

JS:   Object.entries(obj)
来源：http://hz.yj20258888.top/gtoenqalcv.html

TS:   Object.entries(obj)
来源：http://hz.zhoulong.xyz/gtwdidwwka.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.nanxuanxn.top/gtfvizzrre.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cheryme.top/gtnimuyojq.html

Ruby: obj.instance_variables
来源：http://hz.quarkkingdee.top/gtpfioqxoh.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jqgufenzy.top/gtjhflkxam.html

================================================================================
来源：http://hz.aibaodan.cn/gthenlobug.html

H. 异常与错误处理
来源：http://hz.0kj1m.cn/gthwubzink.html

================================================================================
来源：http://hz.redwolf501.top/gtxbayuwsh.html

[H01] try / catch 基础
来源：http://hz.fengsongda.top/gtybjewijv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hammf.cn/gtjdhkxepr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cashguo.top/gtsxqvcjaj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yvedp.cn/gtqyyolmqc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.kuanghao11.cn/gtlawhehsp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xinyue.icu/gtepajkbms.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhixingplan.top/gtzcychtok.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gotoacloud.top/gtbwkiusbw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gaohongyu789.top/gtciuemfen.html

[H02] finally / ensure 收尾
来源：http://hz.yongpay.top/gtjglhcqll.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jyoumei.cn/gtbstayxaj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtklcrbaoj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtugdzkkhf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtaxwchadd.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hnqzz.top/gtclgyynqr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.0kj1m.cn/gtftyicgvj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.haohaochexian.top/gttcavibpb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtplgvmmpe.html

[H03] 主动抛出异常
来源：http://hz.yuxming.cn/gtyiziqmij.html

Py:   raise ValueError("错误信息")
来源：http://hz.gogol.net.cn/gtlfhbpdrr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.chenzaomai.com/gtqiihkqmo.html

JS:   throw new Error("错误信息");
来源：http://hz.jqgfzy.top/gtzivsreun.html

TS:   throw new Error("错误信息");
来源：http://hz.jyoumei.cn/gttkazrpqr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.feifeiyinyue.top/gtvoqiuhku.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinyuanbaomall.cn/gtqcxrakpf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ehwqpu.com/gtjvpucqxi.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ywan-chungtsiang.top/gtxbpxfizf.html

[H04] 自定义异常类型
来源：http://hz.redwolf501.top/gthrefkysb.html

Py:   class MyError(Exception): pass
来源：http://hz.zhengqikj.top/gtcpitnjha.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.sysykeji.top/gtcmeqqjwv.html

JS:   class MyError extends Error {}
来源：http://hz.jlsjyb.cn/gtxvpfdahm.html

TS:   class MyError extends Error {}
来源：http://hz.hnqzz.top/gtkiqhnrnm.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ydjk.org.cn/gtwbzxbohu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cdnleiting.top/gtxhjmcupb.html

Ruby: class MyError < StandardError; end
来源：http://hz.kuanghao11.cn/gtsxxjxsre.html

C#:   class MyException : Exception {}
来源：http://hz.ivvv.top/gtzfmxovye.html

[H05] 捕获特定类型
来源：http://hz.ydjk.org.cn/gtizyepgof.html

Py:   except ValueError as e:
来源：http://hz.jianghu66.top/gtsiuacaeo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.gogol.net.cn/gtunaouikf.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ehwqpu.com/gtiibebsmx.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cucudq.cn/gtrolgsijl.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shanyushiyangkeji.top/gthccesbxy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yueranfly.top/gtblnfcmkl.html

Ruby: rescue ArgumentError => e
来源：http://hz.hysaishi.cn/gtndxigpgg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ppjwa.cn/gtextabbqz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.52xcode.cn/gtirhewdsr.html

Py:   value = d.get("k") or default
来源：http://hz.zhongyouzk.top/gtcoisxxcv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xuetiantiany.cn/gtuaiogmdu.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xuetiantiany.cn/gtvzujksfj.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.pycfn.com/gtoifcpnav.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ivvv.top/gtucilffaq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.pengpengdd.cyou/gtxytrqguw.html

Ruby: d&.dig(:a, :b)
来源：http://hz.daria6918.cn/gtrrhcfyse.html

C#:   obj?.A?.B ?? default
来源：http://hz.cheryme.top/gtymxddbet.html

[H07] 断言
来源：http://hz.yj20258888.top/gtmposbjyv.html

Py:   assert x > 0, "必须为正"
来源：http://hz.aizwys.cn/gttlqfsjjb.html

PHP:  assert($x > 0);
来源：http://hz.cashguo.top/gtiairiffw.html

JS:   console.assert(x > 0);
来源：http://hz.hysaishi.cn/gtpyuwgylw.html

TS:   console.assert(x > 0);
来源：http://hz.hammf.cn/gtzcagsunf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhoulong.xyz/gtlyxyopeg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.vqdsnc.cn/gtzpfpemoz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yonumen.top/gtyfxjmnwr.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhaomingkeji.xyz/gtzjpjnwqy.html

[H08] 获取错误信息与堆栈
来源：http://hz.nanxinkj.top/gtsyipnroq.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ybcxt.top/gtfrnaasph.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ivvv.top/gthjnnaxdn.html

JS:   e.message;  e.stack
来源：http://hz.jqgufenzy.top/gtmxuxwuke.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ywan-chungtsiang.top/gtqccabriv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.aizwys.cn/gthmmtzvsi.html

Go:   err.Error()
来源：http://hz.sxryk.cn/gtwmfgmdev.html

Ruby: e.message;  e.backtrace
来源：http://hz.aibaodan.cn/gtqupvyvbm.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yangfankeji.com/gtcgtcvzme.html

[H09] 带错误码的异常
来源：http://hz.smart0.xyz/gtfeaspbxc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shangyingyoupin.top/gtlrwfzgme.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shanyushiyangkeji.top/gttltndccn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.9152youxi.cn/gtnlvojotg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zycfv.cn/gtawuxavcz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.fengsongda.top/gtdzqghfer.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yuxming.cn/gtupybgjua.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xziqi.cn/gtwimbecrj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jqgufenzy.top/gtzjllqlqi.html

[H10] 资源自动释放
来源：http://hz.mhx1999.top/gtfjmdocks.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cashguo.top/gtswsdgmyo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xziqi.cn/gtjcvaxsaf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ywan-chungtsiang.top/gtjldhybml.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yonumen.top/gtyegrmbfc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hysaishi.cn/gtpyayucbk.html

Go:   defer f.Close()
来源：http://hz.pycfn.com/gtgvpojitt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zdqjudy.top/gtmgbirnju.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.chenjidiqi.icu/gtmfrtqbej.html

================================================================================
来源：http://hz.hammf.cn/gtvmfwzmnr.html

I. 正则表达式
来源：http://hz.yuxming.cn/gtkibpyriq.html

================================================================================
来源：http://hz.jianghu66.top/gtvcfwgyfg.html

[I01] 判断是否匹配
来源：http://hz.cashguo.top/gtpdxgdoyu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jianghu66.top/gtytptapuc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sxryk.cn/gthsifdsoo.html

JS:   /\d+/.test(s)
来源：http://hz.zhengqikj.top/gtqhpfuzmk.html

TS:   /\d+/.test(s)
来源：http://hz.sxryk.cn/gthuzwmmwo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.tian-w.cn/gtonxirsxh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hfpthk.cn/gtszltlcif.html

Ruby: s.match?(/\d+/)
来源：http://hz.hfpthk.cn/gtzlqcyykm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hammf.cn/gthwmpywoe.html

[I02] 提取所有匹配
来源：http://hz.birdmap.top/gtwgzkogtl.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ivvv.top/gtwfstmbby.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.316326.xyz/gtomofqtfk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj202588.top/gttanjhkbu.html

TS:   s.match(/\d+/g)
来源：http://hz.yuxming.cn/gtamhzztbt.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sweek.top/gtmwggaqrs.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hnqzz.top/gtyoflltxf.html

Ruby: s.scan(/\d+/)
来源：http://hz.xuanzx.com/gtrnoaaier.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.kuanghao11.cn/gtyvmssume.html

[I03] 提取捕获分组
来源：http://hz.jinqigufen.top/gtxzriogpj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.smart0.xyz/gtwrxknpxn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ppjwa.cn/gtubzlmszj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.wangshuangyany.cn/gtanuxnjqv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.dashuyun.cn/gtjkksvgni.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jiagoushi.top/gtvvazxzic.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.dianchejie.cn/gtnzxfwyfx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.dianchejie.cn/gtsaldsoyz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xinyue.icu/gtvrroojse.html

[I04] 正则替换
来源：http://hz.xziqi.cn/gtwswzygir.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yvedp.cn/gterczptji.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinghuilouyu.cn/gtimgaabjc.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.dianchejie.cn/gtjqvvfqto.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.fzhhl.top/gtttokeoqb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zdqjudy.top/gtykkbtett.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.snrcjt.cn/gtbwvjdumk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hongshengwenyu.top/gtnomurwld.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hammf.cn/gtvvndxpbg.html

[I05] 按正则拆分
来源：http://hz.xziqi.cn/gtjjsucoyi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hysaishi.cn/gtrizsymkq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.c1oappe.top/gtmoeugure.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.tianlin.xyz/gthtfhtfpv.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yuanzhike.top/gthxkwnlif.html

Java: s.split("\\s*,\\s*")
来源：http://hz.smart0.xyz/gthqyymiho.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yuanzhike.top/gtsczzlkaw.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.chenzaomai.com/gtsrfgyfwo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hammf.cn/gtxnvhpfuw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.meibo888.top/gtmeurgzki.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shuidangran.top/gtqnjphpcy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hongshengwenyu.top/gtklttdriw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenjidiqi.icu/gtqyhdqkwk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gaohongyu789.top/gthandnnav.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cucudq.cn/gtbnetysic.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.0kj1m.cn/gtgljsyaxd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shanyushiyangkeji.top/gtwrahefwj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hnxiangtu.top/gtkmudahgj.html

[I07] 忽略大小写与多行模式
来源：http://hz.fzhhl.top/gtrrnznejj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hongshengwenyu.top/gtnhnczcdy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yvedp.cn/gtwujlgmcr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.redwolf501.top/gtbzyxxnhq.html

TS:   /error/gim
来源：http://hz.shanyushiyangtech.top/gtrahfrhnh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.chenzaomai.com/gtecwmmdcu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.dianchejie.cn/gtolgoaimx.html

Ruby: s.scan(/error/i)
来源：http://hz.chenzaomai.com/gtjhfntiic.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.feifeiyinyue.top/gttsrhfreh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.haohaochexian.top/gtqljqnvgn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jinyuanbaomall.cn/gtgzwuajxd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.kuanghao11.cn/gtkbguzwmj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shangyingyoupin.top/gtzyjivvwc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nwbrower.top/gtvjvfvxau.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.daxiang520.top/gtdjtvwyqn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xylfe.cn/gtiqbgrqdx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.redwolf501.top/gthisjtepj.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.daria6918.cn/gtsxtalqge.html

================================================================================
来源：http://hz.redwolf501.top/gtcsvkurky.html

J. 日期与时间
来源：http://hz.shangyingyoupin.top/gtighoovco.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtakkpagkd.html

[J01] 获取当前时间
来源：http://hz.dashuyun.cn/gtiykbnzcf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ydjk.org.cn/gtakieovlv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.fzhhl.top/gtarewjajo.html

JS:   new Date();  Date.now()
来源：http://hz.gotoacloud.top/gtavhyrisv.html

TS:   new Date();  Date.now()
来源：http://hz.zhixingplan.top/gtvdzwgnmp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinyuanbaomall.cn/gtiqahuuvr.html

Go:   time.Now()
来源：http://hz.jinqigfzy.top/gtqdiinvqt.html

Ruby: Time.now
来源：http://hz.ppjwa.cn/gtxkwzxaqj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.guannengcc.top/gtxpemowoh.html

[J02] 格式化输出
来源：http://hz.yangfankeji.com/gtfmbderll.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ybcxt.top/gtzavcpmhe.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jinghuilouyu.cn/gtemxmukmx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jinghuilouyu.cn/gtncusikxp.html

TS:   d.toISOString()
来源：http://hz.yueranfly.top/gtzwtuxgpe.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ehwqpu.com/gtnnzcvwuo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.guowangkeji.top/gtsuealutw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zdqjudy.top/gtjdymytmc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.aibaodan.cn/gthdpcduhq.html

[J03] 字符串解析为日期
来源：http://hz.zycfv.cn/gthdvnzjnk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yongpay.top/gtfmsiglmd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ydjk.org.cn/gtfegymszl.html

JS:   new Date("2024-01-02")
来源：http://hz.hnqzz.top/gtvxlgrtvj.html

TS:   new Date("2024-01-02")
来源：http://hz.gotoacloud.top/gtvjnxttxk.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ppjwa.cn/gtaxmyrpma.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hysaishi.cn/gthogbavnp.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.vqdsnc.cn/gtkgfolntr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.snrcjt.cn/gthqbepmon.html

[J04] 时间戳与日期互转
来源：http://hz.yvedp.cn/gtujgsdflz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.sysykeji.top/gtmgugfkez.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.chenzaomai.com/gtuychvjpy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ydzc1.top/gtvwkdlhfl.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.c1oappe.top/gtmbeyzsch.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xuetiantiany.cn/gtzhsrceis.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jqgufenzy.top/gtwthwvahd.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yvedp.cn/gtptpmbeht.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhaomingkeji.xyz/gtlmaocccs.html

[J05] 时间加减（加 7 天）
来源：http://hz.aizwys.cn/gtltypggsr.html

Py:   now + timedelta(days=7)
来源：http://hz.hongshengwenyu.top/gtgsvlqthm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yuxming.cn/gtxymgzrsw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dashuyun.cn/gtypttbmtz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xinyue.icu/gtxvzfkwfm.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jiagoushi.top/gtwcqoeiqr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.redwolf501.top/gtztynxolq.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xingfuxueyuan.xyz/gtxgrcyqvl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.aibaodan.cn/gtctzvrkjz.html

[J06] 计算两时间之差
来源：http://hz.zhaomingkeji.xyz/gtmatlystn.html

Py:   (end - start).total_seconds()
来源：http://hz.yueranfly.top/gtqeyhqgai.html

PHP:  $end->diff($start)->days;
来源：http://hz.xylfe.cn/gtxuperuwm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.0kj1m.cn/gtmpxpdved.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.nanxuanxn.top/gtnglzxxhk.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ybcxt.top/gtxelujqzj.html

Go:   end.Sub(start).Hours()
来源：http://hz.sxryk.cn/gtrpolryei.html

Ruby: end - start                 # 返回秒数
来源：http://hz.vqdsnc.cn/gtkkgtzjaz.html

C#:   (end - start).TotalSeconds
来源：http://hz.guowangkeji.top/gtypdlapns.html

[J07] 比较两个日期
来源：http://hz.svipenyu.cn/gtlvdezwgv.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.feifeiyinyue.top/gtoatcqsvd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.bjfxy.top/gtqhcdnkxk.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jianghu66.top/gtzmeacufr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.aizwys.cn/gtmcrjnxrx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.dashuyun.cn/gtpoxykkqp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shzxlz.cn/gtqgokpful.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cashguo.top/gtcvkudfmz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.svipenyu.cn/gtmpxfqxmk.html

[J08] 提取年月日与星期
来源：http://hz.xylfe.cn/gtuwjapoid.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shuidangran.top/gtylzfpxkf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.c1oappe.top/gthasljwli.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.andypj.xyz/gtianlrgwl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.chenzaomai.com/gtagfjusyv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jqgufenzy.top/gtawhghaky.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hnxiangtu.top/gtffccclfc.html


<!-- 参考信息 -->