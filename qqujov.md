代发 wailian999

C#:   public / protected / private / internal
来源：http://hz.xinyue.icu/gtzhnkknyy.html

[G11] getter / setter
来源：http://hz.chenjidiqi.icu/gtwisnfcil.html

Py:   @property 与 @x.setter
来源：http://hz.yuxming.cn/gtjxwucbmg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nanxuanxn.top/gtqskfxlqz.html

JS:   get name() { return this._name; }
来源：http://hz.zhijiandao.cn/gtsvfbokgm.html

TS:   get name(): string { return this._name; }
来源：http://hz.xuetiantiany.cn/gtunqpsrtm.html

Java: public String getName() { return name; }
来源：http://hz.sysykeji.top/gthcdnbmvv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.meibo888.top/gtexmpzkxo.html

Ruby: attr_accessor :name
来源：http://hz.havefunace.top/gteoippsvx.html

C#:   public string Name { get; set; }
来源：http://hz.wangshuangyany.cn/gthrdkaxgb.html

[G12] 对象转字符串
来源：http://hz.zhengqikj.top/gtehhvymav.html

Py:   def __str__(self): return self.name
来源：http://hz.wangdashe.top/gtpwmvbrdu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.nanxuanxn.top/gtokbjhpwe.html

JS:   toString() { return this.name; }
来源：http://hz.yangfankeji.com/gtlixbynxj.html

TS:   toString(): string { return this.name; }
来源：http://hz.ywan-chungtsiang.top/gtykjkscii.html

Java: @Override public String toString() { return name; }
来源：http://hz.cheryme.top/gtfrmdwrhn.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.52xcode.cn/gtyqawsxxn.html

Ruby: def to_s; @name; end
来源：http://hz.haohaochexian.top/gtivnbcuqw.html

C#:   public override string ToString() => Name;
来源：http://hz.yj20258.top/gtbhuutagr.html

[G13] 判断对象类型
来源：http://hz.iojbl.cn/gtmfgckjxa.html

Py:   isinstance(u, User)
来源：http://hz.wangdashe.top/gtgdttwehz.html

PHP:  $u instanceof User
来源：http://hz.jinqigfzy.top/gtuofijakd.html

JS:   u instanceof User
来源：http://hz.jiagoushi.top/gtlsjwjrbx.html

TS:   u instanceof User
来源：http://hz.c1oappe.top/gteuipsabg.html

Java: u instanceof User
来源：http://hz.yj202588.top/gtaahqkctr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.dashuyun.cn/gtadccegti.html

Ruby: u.is_a?(User)
来源：http://hz.tianlin.xyz/gttynbtbdh.html

C#:   u is User
来源：http://hz.iojbl.cn/gtpctgxcin.html

[G14] 数据类 / record
来源：http://hz.zhaomingkeji.xyz/gtlywhtjbb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.haohaochexian.top/gtlfkxahgn.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.daria6918.cn/gtkppozwlr.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.aizwys.cn/gtwcjuiomi.html

TS:   type User = { name: string; age: number };
来源：http://hz.0kj1m.cn/gtwljcimbn.html

Java: record User(String name, int age) {}
来源：http://hz.cheryme.top/gtksxinlzx.html

Go:   type User struct { Name string; Age int }
来源：http://hz.guowangkeji.top/gtzlinkeil.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.smart0.xyz/gtnofhvbsr.html

C#:   record User(string Name, int Age);
来源：http://hz.xuanzx.com/gtzmkrvttr.html

[G15] 枚举
来源：http://hz.aibaodan.cn/gtzsdahyye.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yj202588.top/gtdlatrzjb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.pengpengdd.cyou/gtvkifkiyr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xinyue.icu/gtmxsejuqh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gzhubu.top/gtjisaaxaw.html

Java: enum Color { RED, GREEN }
来源：http://hz.hnqzz.top/gtvwnktvbu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hammf.cn/gthqdkbfui.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xziqi.cn/gtlaxtzoga.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.havefunace.top/gtctrgttoc.html

[G16] 对象转数组 / 字典
来源：http://hz.mhx1999.top/gtbeivofcq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.aibaodan.cn/gtzxnmpzsx.html

PHP:  get_object_vars($obj);
来源：http://hz.ehwqpu.com/gtegjpzqpd.html

JS:   Object.entries(obj)
来源：http://hz.xuanzx.com/gtkubdfbgi.html

TS:   Object.entries(obj)
来源：http://hz.tanke756.top/gtbfdndqes.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.dianchejie.cn/gtivnawjmv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jqgufenzy.top/gtqqindoyp.html

Ruby: obj.instance_variables
来源：http://hz.xinyue.icu/gttqezvawa.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.tianlin.xyz/gthntjukjk.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtzevqztal.html

H. 异常与错误处理
来源：http://hz.shanyushiyangkeji.top/gtfqtcrvhi.html

================================================================================
来源：http://hz.yj20258888.top/gtdbkvyrse.html

[H01] try / catch 基础
来源：http://hz.havefunace.top/gtxvgsqhmw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.haohaochexian.top/gtndizmeqw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zycfv.cn/gtqjjpcnpu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.kuanghao11.cn/gtixtysgfb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.mhx1999.top/gtbrnpigwx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.snrcjt.cn/gtdejacnwh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.chenzaomai.com/gtuqoqoepw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yangfankeji.com/gtnwtehafm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.aizwys.cn/gtxjqzxqfn.html

[H02] finally / ensure 收尾
来源：http://hz.xziqi.cn/gtgxensxwu.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xziqi.cn/gtnpzlsxpp.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtzyejottg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gtpzuupfnf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.haohaochexian.top/gtpwkmehrr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtfryfhble.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhijiandao.cn/gtrdhfqhgx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.nanxinkj.top/gtyxgifmnx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.tanke756.top/gtiwzkykvo.html

[H03] 主动抛出异常
来源：http://hz.ydjk.org.cn/gtbxumjcbt.html

Py:   raise ValueError("错误信息")
来源：http://hz.hnqzz.top/gthvhmsoai.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.0kj1m.cn/gtkwvmqica.html

JS:   throw new Error("错误信息");
来源：http://hz.redwolf501.top/gtqenrrxfc.html

TS:   throw new Error("错误信息");
来源：http://hz.shzxlz.cn/gtlfudiizf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sufxvd.cn/gtybzcaovp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.iojbl.cn/gtshdfddzs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.c1oappe.top/gtzytuzhbi.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtufkmctfb.html

[H04] 自定义异常类型
来源：http://hz.hysaishi.cn/gtnqdvxwyw.html

Py:   class MyError(Exception): pass
来源：http://hz.yueranfly.top/gtdxkujtry.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.quarkkingdee.top/gtosiwpdyn.html

JS:   class MyError extends Error {}
来源：http://hz.sweek.top/gtzijzzazd.html

TS:   class MyError extends Error {}
来源：http://hz.feifeiyinyue.top/gtvdqlyhkl.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xziqi.cn/gtawqfrgpf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hammf.cn/gtwcrnrvdd.html

Ruby: class MyError < StandardError; end
来源：http://hz.nanxuanxn.top/gtplukmsqm.html

C#:   class MyException : Exception {}
来源：http://hz.yangfankeji.com/gtsxkazcha.html

[H05] 捕获特定类型
来源：http://hz.sufxvd.cn/gtwgclwohw.html

Py:   except ValueError as e:
来源：http://hz.yuxming.cn/gthflirtsr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shanyushiyangkeji.top/gtfjxpnomu.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yanxiufei.cn/gtsiqobqgi.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jyoumei.cn/gttyvjouum.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cucudq.cn/gthinikvjl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yanxiufei.cn/gterhbrbjk.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhixingplan.top/gtmphnvigr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ybcxt.top/gtyxkzzsni.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yongpay.top/gtexubalcj.html

Py:   value = d.get("k") or default
来源：http://hz.shanyushiyangkeji.top/gtqeomxpol.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.feifeiyinyue.top/gthsxgyuca.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xingfuxueyuan.xyz/gtajaszozv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxinkj.top/gtzcamwnwe.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jlsjyb.cn/gtifzzwffv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.gotoacloud.top/gtneomwllf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.aizwys.cn/gtbtoyvkyl.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinyuanbaomall.cn/gtapukswjs.html

[H07] 断言
来源：http://hz.jinyuanbaomall.cn/gtgcczaevh.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sweek.top/gtzihgiawh.html

PHP:  assert($x > 0);
来源：http://hz.hnxiangtu.top/gtyxdghdmv.html

JS:   console.assert(x > 0);
来源：http://hz.zhongyouzk.top/gthqhopvrw.html

TS:   console.assert(x > 0);
来源：http://hz.quarkkingdee.top/gtlyntizlu.html

Java: assert x > 0 : "必须为正";
来源：http://hz.snrcjt.cn/gtdxmklnpr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cdnleiting.top/gtygrxpfpp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hnxiangtu.top/gtnhgqyzbp.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtubvawltn.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhoulong.xyz/gtrydofxsr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yj202588.top/gtjolhdaoi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xinyue.icu/gtkftibwiu.html

JS:   e.message;  e.stack
来源：http://hz.yj202588.top/gtsgmjalbp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.vqdsnc.cn/gtwgtwfcih.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.316326.xyz/gtitxeowry.html

Go:   err.Error()
来源：http://hz.redwolf501.top/gtwvioojwq.html

Ruby: e.message;  e.backtrace
来源：http://hz.sweek.top/gtxfpntqvm.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yj202588.top/gthkewbkqn.html

[H09] 带错误码的异常
来源：http://hz.vqdsnc.cn/gtytnminwe.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zdqjudy.top/gtbzqskccr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shanyushiyangkeji.top/gtlcfumhgs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.316326.xyz/gtjjrknxku.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.nanxinkj.top/gtmvnyfpcv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yanxiufei.cn/gtgzpolsoj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hywenlv.cn/gtjitwuuna.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xuetiantiany.cn/gtbgwyqoub.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinyuanbaomall.cn/gtxsfqkukt.html

[H10] 资源自动释放
来源：http://hz.jiagoushi.top/gtairyecig.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhongyouzk.top/gtfcbpnpby.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.guowangkeji.top/gtoswdxqsm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nwbrower.top/gttyjvzhhy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhijiandao.cn/gtyxtpcyhu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhixingplan.top/gtrkrqrvbg.html

Go:   defer f.Close()
来源：http://hz.pengpengdd.cyou/gtdxwduhyw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hysaishi.cn/gtdeyhsqxz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yanxiufei.cn/gtoixllado.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtrglvtrnp.html

I. 正则表达式
来源：http://hz.shanyushiyangkeji.top/gttcegwxql.html

================================================================================
来源：http://hz.hysaishi.cn/gtqtwcbrxa.html

[I01] 判断是否匹配
来源：http://hz.sxryk.cn/gtuaahnmqf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jiagoushi.top/gtlpcvkbrh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.vqdsnc.cn/gtqinotamx.html

JS:   /\d+/.test(s)
来源：http://hz.birdmap.top/gtcnkyqjpn.html

TS:   /\d+/.test(s)
来源：http://hz.xingfuxueyuan.xyz/gtvhtutexg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yueranfly.top/gtrnqijiwi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hammf.cn/gtstpwhzux.html

Ruby: s.match?(/\d+/)
来源：http://hz.yongpay.top/gtnlfpyumn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hywenlv.cn/gtjlrjssxv.html

[I02] 提取所有匹配
来源：http://hz.yonumen.top/gtaeuervzc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.nwbrower.top/gtbuqtpysz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj202588.top/gtdyzfujqy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.sysykeji.top/gtioezrzxk.html

TS:   s.match(/\d+/g)
来源：http://hz.9152youxi.cn/gtcngurpag.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jiagoushi.top/gtjtbxnlqn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shangyingyoupin.top/gtpeyugxcb.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhoulong.xyz/gtbgncfuph.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhongyouzk.top/gtiectszml.html

[I03] 提取捕获分组
来源：http://hz.hnqzz.top/gtwycgbktt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jinqigufen.top/gtxyqdvvlz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhaomingkeji.xyz/gthhqsdgxq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hysaishi.cn/gttnjisstz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.pengpengdd.cyou/gtdnuknzkp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.tianlin.xyz/gtsqvklzne.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ydjk.org.cn/gtkobknjek.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.kuanghao11.cn/gtefncihvr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ywan-chungtsiang.top/gtduvqwrbi.html

[I04] 正则替换
来源：http://hz.daria6918.cn/gthpdjpuku.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yj202588.top/gtzpshhlqu.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.meibo888.top/gtbsqttyhf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.kuanghao11.cn/gtauowiaso.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.chenzaomai.com/gtfkdlawet.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.guowangkeji.top/gtvcxrgvsy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.guowangkeji.top/gtdopieyuz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.wangshuangyany.cn/gtnirqogah.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.wangshuangyany.cn/gtyvehubrp.html

[I05] 按正则拆分
来源：http://hz.yj20258888.top/gtmrejdrzp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.mhx1999.top/gtppujviga.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shuidangran.top/gtnkzudtiy.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.bjfxy.top/gtejbbmbqy.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yvedp.cn/gtxoayyqpi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.tianlin.xyz/gtefpscmfb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jiagoushi.top/gtreklmfhh.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.andypj.xyz/gtglenfpwq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.sysykeji.top/gtydlcygcm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hfpthk.cn/gtozshxohd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shanyushiyangkeji.top/gttxbaepaf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xylfe.cn/gtjcrcjato.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ywan-chungtsiang.top/gttphmnzzu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.guowangkeji.top/gtuljlkdxw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.fengsongda.top/gthhkcnloz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sweek.top/gthlmzshqa.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.meibo888.top/gtpudyzwgk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yvedp.cn/gttbnnspoo.html

[I07] 忽略大小写与多行模式
来源：http://hz.jqgufenzy.top/gtgylclfqb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xinyue.icu/gtxpzstiym.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.dianchejie.cn/gtcwqjvyyh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.aizwys.cn/gtljdwxpwa.html

TS:   /error/gim
来源：http://hz.dianchejie.cn/gtspqlfmui.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hfpthk.cn/gtvsknfmry.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yuanzhike.top/gtvekdmseq.html

Ruby: s.scan(/error/i)
来源：http://hz.pengpengdd.cyou/gtiptjlmmc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.chenzaomai.com/gtnrsajhxn.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xuetiantiany.cn/gtdbfamyuk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.havefunace.top/gtjvkyuqmi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.daria6918.cn/gtveawqusl.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gaohongyu789.top/gtdzinynso.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hfpthk.cn/gtsfdjnixt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sweek.top/gtkzjgzctp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.nanxinkj.top/gtxxmenlla.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhiwuduotai.top/gtkadvrfuc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xylfe.cn/gtevhmuyqi.html

================================================================================
来源：http://hz.shuidangran.top/gthuzgflcq.html

J. 日期与时间
来源：http://hz.andypj.xyz/gtporsyvoh.html

================================================================================
来源：http://hz.jqgfzy.top/gtyqeedsqb.html

[J01] 获取当前时间
来源：http://hz.shanyushiyangkeji.top/gtvmoxpsoh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jyoumei.cn/gthpeywedx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.guannengcc.top/gtdmkubmom.html

JS:   new Date();  Date.now()
来源：http://hz.ppjwa.cn/gtsnwrzwmw.html

TS:   new Date();  Date.now()
来源：http://hz.feifeiyinyue.top/gtikrrlfcb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xuetiantiany.cn/gtuajgtmpe.html

Go:   time.Now()
来源：http://hz.hammf.cn/gtmkwxwvzw.html

Ruby: Time.now
来源：http://hz.sufxvd.cn/gtxgwgkjac.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.quarkkingdee.top/gtrkjvaqsb.html

[J02] 格式化输出
来源：http://hz.316326.xyz/gtyczytxmm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydjk.org.cn/gtveclsuna.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.dashuyun.cn/gtehxgvpvj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gotoacloud.top/gtlpiqaeeo.html

TS:   d.toISOString()
来源：http://hz.hysaishi.cn/gthjgewssc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jinyuanbaomall.cn/gtyydarjyj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shangyingyoupin.top/gtcrchljxr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cucudq.cn/gtydjcwmii.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hfpthk.cn/gtbiqnjnaj.html

[J03] 字符串解析为日期
来源：http://hz.ppjwa.cn/gtviabfuhu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinyuanbaomall.cn/gtabraaafp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sxryk.cn/gtnlfwuwvv.html

JS:   new Date("2024-01-02")
来源：http://hz.haohaochexian.top/gttrirswly.html

TS:   new Date("2024-01-02")
来源：http://hz.xziqi.cn/gthhpfwflf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.52xcode.cn/gthzggtfrm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hongshengwenyu.top/gtikpbqarj.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hnqzz.top/gtzijamusw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.chenlongwang.top/gtgtpdbmnq.html

[J04] 时间戳与日期互转
来源：http://hz.nwbrower.top/gttjjddqlu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.havefunace.top/gtfzjaugyq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhaomingkeji.xyz/gtbyfhztwq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.cheryme.top/gtdowwfaxb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cqqwz.cn/gtiluyktpv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.52xcode.cn/gtsbchdiat.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.aizwys.cn/gtpckvbpas.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ywan-chungtsiang.top/gtgltxhygx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.snrcjt.cn/gtgzirvdpy.html

[J05] 时间加减（加 7 天）
来源：http://hz.yangfankeji.com/gtyvgjinmz.html

Py:   now + timedelta(days=7)
来源：http://hz.yuanzhike.top/gtgkiwezfk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shzxlz.cn/gtyizyeatf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenjidiqi.icu/gtlviiwczv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nanxinkj.top/gtoijphdox.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.gotoacloud.top/gtyuswnqmm.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.havefunace.top/gtuevesvfm.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hongshengwenyu.top/gtpgwnzsvj.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ehwqpu.com/gtyrvhcbri.html

[J06] 计算两时间之差
来源：http://hz.yonumen.top/gtdzoxsrkk.html

Py:   (end - start).total_seconds()
来源：http://hz.hongshengwenyu.top/gtdmvcnsfi.html

PHP:  $end->diff($start)->days;
来源：http://hz.shuidangran.top/gtzvlapnzb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.kuanghao11.cn/gtfpbvhftc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ydzc1.top/gtuvxqwwwd.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhiwuduotai.top/gtcenjbvkm.html

Go:   end.Sub(start).Hours()
来源：http://hz.cqqwz.cn/gtphvifwcj.html

Ruby: end - start                 # 返回秒数
来源：http://hz.havefunace.top/gtojtjmecu.html

C#:   (end - start).TotalSeconds
来源：http://hz.yongpay.top/gtdlrmccmm.html

[J07] 比较两个日期
来源：http://hz.pengpengdd.cyou/gtwvnnusnf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.havefunace.top/gtgylejsdy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.nanxuanxn.top/gtvxkzsgoe.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.52xcode.cn/gtwremydiw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.birdmap.top/gtpthftwhi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.andypj.xyz/gtpctsrgyt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.cdnleiting.top/gtpofizkcp.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.dashuyun.cn/gtfwlfzxnm.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.316326.xyz/gtbmilasgr.html

[J08] 提取年月日与星期
来源：http://hz.0kj1m.cn/gtlwhmnxcm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.feifeiyinyue.top/gtgojwqwxe.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ywan-chungtsiang.top/gtysihngyz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhijiandao.cn/gtgfmxcbev.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sysykeji.top/gttbclxywx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.daria6918.cn/gtofroqsss.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ydzc1.top/gthahegdua.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.daria6918.cn/gtliavrcyg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.nanxuanxn.top/gtgwcfgpkp.html

[J09] 时区处理
来源：http://hz.pycfn.com/gtyypzkwqz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gzhubu.top/gtbsogykmp.html


<!-- 参考信息 -->