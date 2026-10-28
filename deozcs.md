代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://hz.guowangkeji.top/gtqisyporu.html

Java: record User(String name, int age) {}
来源：http://hz.ppjwa.cn/gtdjexkcmd.html

Go:   type User struct { Name string; Age int }
来源：http://hz.mhx1999.top/gtejxdolio.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shanyushiyangtech.top/gtgylzxnru.html

C#:   record User(string Name, int Age);
来源：http://hz.xziqi.cn/gtdebehkbx.html

[G15] 枚举
来源：http://hz.gogol.net.cn/gtgfeihpah.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.snrcjt.cn/gtmotpwwmb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.andypj.xyz/gtqeruoqro.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.dianchejie.cn/gtvevyzcmu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zdqjudy.top/gtplnrjezs.html

Java: enum Color { RED, GREEN }
来源：http://hz.hnxiangtu.top/gtekefnvhv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sufxvd.cn/gtpgjvnhlq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.svipenyu.cn/gtvhxrfrum.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gaohongyu789.top/gtsunprgpa.html

[G16] 对象转数组 / 字典
来源：http://hz.316326.xyz/gtogcfyjhq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cdnleiting.top/gtycpuwyxm.html

PHP:  get_object_vars($obj);
来源：http://hz.mhx1999.top/gtsxcpbvrr.html

JS:   Object.entries(obj)
来源：http://hz.guannengcc.top/gtbcljnoig.html

TS:   Object.entries(obj)
来源：http://hz.zhengqikj.top/gtqccfmxep.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gaohongyu789.top/gtmkwxgead.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.zhengqikj.top/gtyhykydtw.html

Ruby: obj.instance_variables
来源：http://hz.kuanghao11.cn/gtihuvhtmv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hfpthk.cn/gtmybiakhl.html

================================================================================
来源：http://hz.kuanghao11.cn/gtsaggnybb.html

H. 异常与错误处理
来源：http://hz.svipenyu.cn/gtlacakois.html

================================================================================
来源：http://hz.ppjwa.cn/gtxavqekka.html

[H01] try / catch 基础
来源：http://hz.iojbl.cn/gtavtpdzum.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xziqi.cn/gteikjggoe.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hfpthk.cn/gtmnbtaqpb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.fengsongda.top/gtnvhyqlpi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zdqjudy.top/gtxrklnjgd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.daxiang520.top/gtttkdaqvs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.snrcjt.cn/gtkfjvhpie.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xinyue.icu/gtguhgjjmb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jlsjyb.cn/gtewlqkwxa.html

[H02] finally / ensure 收尾
来源：http://hz.xingfuxueyuan.xyz/gtqqwprxip.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jlsjyb.cn/gtsulmuphn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.chenlongwang.top/gtlsalufjn.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtwwfuqrwp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cdnleiting.top/gtnjirjoun.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gtaidyiati.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yj20258888.top/gtbflhkoxq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ivvv.top/gtatvgkujd.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jiagoushi.top/gtyfqligwl.html

[H03] 主动抛出异常
来源：http://hz.ywan-chungtsiang.top/gtcehdzrdl.html

Py:   raise ValueError("错误信息")
来源：http://hz.gogol.net.cn/gtupcqmrwi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gthftsykhy.html

JS:   throw new Error("错误信息");
来源：http://hz.yangfankeji.com/gtwtwoprho.html

TS:   throw new Error("错误信息");
来源：http://hz.ehwqpu.com/gtdavflrnu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.52xcode.cn/gtjsxfllnf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jyoumei.cn/gtevaqqhcx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jlsjyb.cn/gtxvgyfemv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtbtcluocz.html

[H04] 自定义异常类型
来源：http://hz.cheryme.top/gtjsfedffh.html

Py:   class MyError(Exception): pass
来源：http://hz.meibo888.top/gtfuapupbe.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhongyouzk.top/gtmxbfzcpz.html

JS:   class MyError extends Error {}
来源：http://hz.zhoulong.xyz/gtdiogbghy.html

TS:   class MyError extends Error {}
来源：http://hz.hammf.cn/gtlwscekhn.html

Java: class MyException extends RuntimeException {}
来源：http://hz.fzhhl.top/gtkxqoordh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.guowangkeji.top/gtrdrxrrie.html

Ruby: class MyError < StandardError; end
来源：http://hz.hnxiangtu.top/gtjokkgbub.html

C#:   class MyException : Exception {}
来源：http://hz.shangyingyoupin.top/gtsermatcw.html

[H05] 捕获特定类型
来源：http://hz.tianlin.xyz/gthoniclwh.html

Py:   except ValueError as e:
来源：http://hz.zhaomingkeji.xyz/gtlvhqzmrp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.dianchejie.cn/gtguxmdvmq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.snrcjt.cn/gtvisdfuun.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhiwuduotai.top/gtyzxywsdv.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.dianchejie.cn/gthiqbputz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.pengpengdd.cyou/gtbaukdqkl.html

Ruby: rescue ArgumentError => e
来源：http://hz.daxiang520.top/gtbcqazydd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.haohaochexian.top/gtleprjjbf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.chenzaomai.com/gtuwqnoono.html

Py:   value = d.get("k") or default
来源：http://hz.quarkkingdee.top/gtcrhgdegi.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.bjfxy.top/gtwlifhlpw.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.wangdashe.top/gtxymkkobq.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.meibo888.top/gtmkfphxep.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.jyoumei.cn/gtwrccjkgv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hywenlv.cn/gtbmauoagh.html

Ruby: d&.dig(:a, :b)
来源：http://hz.chenjidiqi.icu/gthdejwjvl.html

C#:   obj?.A?.B ?? default
来源：http://hz.quarkkingdee.top/gtubocmqpm.html

[H07] 断言
来源：http://hz.aizwys.cn/gtbyymbhhg.html

Py:   assert x > 0, "必须为正"
来源：http://hz.wangdashe.top/gtekyfayku.html

PHP:  assert($x > 0);
来源：http://hz.chenjidiqi.icu/gtqsogplzb.html

JS:   console.assert(x > 0);
来源：http://hz.quarkkingdee.top/gtbnwsoybb.html

TS:   console.assert(x > 0);
来源：http://hz.yuanzhike.top/gtjruevuoq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.fzhhl.top/gtzjnozqlo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cqqwz.cn/gtaggmbzbg.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.gotoacloud.top/gtknfdwzrl.html

C#:   Debug.Assert(x > 0);
来源：http://hz.birdmap.top/gtkvoiwhhn.html

[H08] 获取错误信息与堆栈
来源：http://hz.quarkkingdee.top/gtkyjepibj.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gotoacloud.top/gtsygniohw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ehwqpu.com/gtgnlrxqjg.html

JS:   e.message;  e.stack
来源：http://hz.birdmap.top/gtvdbaubwy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hfpthk.cn/gtfmezmtym.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jqgfzy.top/gtitjfpixf.html

Go:   err.Error()
来源：http://hz.ydjk.org.cn/gtklmmasdn.html

Ruby: e.message;  e.backtrace
来源：http://hz.gogol.net.cn/gtiowsztkk.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shuidangran.top/gtszzbygdv.html

[H09] 带错误码的异常
来源：http://hz.yj202588.top/gtpetilvbu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.gzhubu.top/gtxuccembp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.52xcode.cn/gtboebhibf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cqqwz.cn/gttnhjyzgl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xuetiantiany.cn/gtxccfaopv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.dashuyun.cn/gtoiijlcph.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hnqzz.top/gtskzwczhx.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cucudq.cn/gtzvdzubei.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hfpthk.cn/gtaaurkzxi.html

[H10] 资源自动释放
来源：http://hz.jinyuanbaomall.cn/gtzmmcsboa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ppjwa.cn/gtkkcbdmjg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.gzhubu.top/gthaqofzfs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhijiandao.cn/gtmrrjhzak.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ehwqpu.com/gtllsjmrvz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.chenjidiqi.icu/gtrxwitvym.html

Go:   defer f.Close()
来源：http://hz.tian-w.cn/gtpmmkyyix.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sxryk.cn/gttmtcbvyf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.andypj.xyz/gtbibqhazz.html

================================================================================
来源：http://hz.yuanzhike.top/gtsktvqnhm.html

I. 正则表达式
来源：http://hz.zhiwuduotai.top/gtxakzuwis.html

================================================================================
来源：http://hz.c1oappe.top/gtwxijnsdq.html

[I01] 判断是否匹配
来源：http://hz.zhongyouzk.top/gtrkctcoxl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jqgfzy.top/gtogeiggfi.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jyoumei.cn/gtbcswitsg.html

JS:   /\d+/.test(s)
来源：http://hz.haohaochexian.top/gtvjyowhsq.html

TS:   /\d+/.test(s)
来源：http://hz.cdnleiting.top/gtwxqrxsct.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.haohaochexian.top/gtbcxsjdxa.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.daria6918.cn/gtjaegzmdq.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhoulong.xyz/gtvaahhinw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jianghu66.top/gtrijosjnt.html

[I02] 提取所有匹配
来源：http://hz.jianghu66.top/gtxrjusfxa.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ywan-chungtsiang.top/gtpdbytirh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yongpay.top/gtenkqnzpn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hywenlv.cn/gtpstsdade.html

TS:   s.match(/\d+/g)
来源：http://hz.shanyushiyangtech.top/gttpcwcttg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.wangdashe.top/gtnqnygdde.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.wangdashe.top/gtxrlxfvdg.html

Ruby: s.scan(/\d+/)
来源：http://hz.sufxvd.cn/gtkikxwdwn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jianghu66.top/gtuectqxwl.html

[I03] 提取捕获分组
来源：http://hz.birdmap.top/gtfmexaqkl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.gzhubu.top/gtzxxhgtrl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhiwuduotai.top/gtwswfxnfh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.pengpengdd.cyou/gttibopqju.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.pycfn.com/gtqvbgpbek.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.tianlin.xyz/gtjhfjtryl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.meibo888.top/gtnbyoregu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.daxiang520.top/gtqeblwylz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xinyue.icu/gthhjosytq.html

[I04] 正则替换
来源：http://hz.gzhubu.top/gtvbzdxmqi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shzxlz.cn/gtafkypjxc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj20258.top/gtiseluvbs.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hywenlv.cn/gtrvotvntz.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zycfv.cn/gtxdalsoye.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xuetiantiany.cn/gtzzrsyxla.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.chenjidiqi.icu/gtevcafacj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.havefunace.top/gtkuuifkfz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.shuidangran.top/gtccuqorgd.html

[I05] 按正则拆分
来源：http://hz.redwolf501.top/gtgcikwrex.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.guannengcc.top/gtgjpivjxf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gogol.net.cn/gtnubimnqn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ehwqpu.com/gtbiksivoz.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.c1oappe.top/gtdvknummv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.wangdashe.top/gtavtjzxdf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yuxming.cn/gtajfwesap.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.pengpengdd.cyou/gtesjvznfp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shanyushiyangkeji.top/gtpwnwbruv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.tianlin.xyz/gtbqzjxuan.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.guowangkeji.top/gtavmxczxj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yongpay.top/gtbxryuhhx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gogol.net.cn/gthoumhkvg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.guowangkeji.top/gtfdwhkntk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tian-w.cn/gtijlroofk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhoulong.xyz/gtefkzrsxl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.mhx1999.top/gtsiedcdtd.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ivvv.top/gtgpetmmtq.html

[I07] 忽略大小写与多行模式
来源：http://hz.aibaodan.cn/gtsxbxvaet.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.tanke756.top/gtpavmaoah.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.pengpengdd.cyou/gtevrfqpok.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhengqikj.top/gtngepwxce.html

TS:   /error/gim
来源：http://hz.yueranfly.top/gteahhoyck.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hammf.cn/gtjnmexdwb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hfpthk.cn/gtsvkpdcks.html

Ruby: s.scan(/error/i)
来源：http://hz.jinqigufen.top/gtzjkcrrtk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhongyouzk.top/gttodaahrl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.fzhhl.top/gtistliafr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yuxming.cn/gttsmzeiua.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.snrcjt.cn/gtlegvxmjx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.mhx1999.top/gtyydhgjra.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuxming.cn/gtclokyoks.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.nwbrower.top/gtxqjyvhjo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.birdmap.top/gtpgmairte.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.aizwys.cn/gtffmzhmcb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.pycfn.com/gtzbsypdgh.html

================================================================================
来源：http://hz.yj202588.top/gtciaavjrd.html

J. 日期与时间
来源：http://hz.chenjidiqi.icu/gtwnurdeem.html

================================================================================
来源：http://hz.ppjwa.cn/gtgvjqycna.html

[J01] 获取当前时间
来源：http://hz.haohaochexian.top/gtkupdmjlt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yueranfly.top/gtztxdozxz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.guowangkeji.top/gtidmxwucj.html

JS:   new Date();  Date.now()
来源：http://hz.yuxming.cn/gtjrhymrrt.html

TS:   new Date();  Date.now()
来源：http://hz.sufxvd.cn/gtbvpzqnux.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhoulong.xyz/gtuvnxwxsz.html

Go:   time.Now()
来源：http://hz.yj20258.top/gtcevzhvhy.html

Ruby: Time.now
来源：http://hz.ybcxt.top/gtwwvwrlci.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cdnleiting.top/gtdnfouuwk.html

[J02] 格式化输出
来源：http://hz.jlsjyb.cn/gtojaxarnp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cucudq.cn/gtfzypziqd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shanyushiyangkeji.top/gtmmgfgkqg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.fzhhl.top/gtganhqwtf.html

TS:   d.toISOString()
来源：http://hz.snrcjt.cn/gtvmjazcli.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sxryk.cn/gtifoamwsi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gotoacloud.top/gtvzplhuyj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuanzx.com/gttmucwohq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jqgufenzy.top/gtckydxqvp.html

[J03] 字符串解析为日期
来源：http://hz.yanxiufei.cn/gtlpcguhcj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yanxiufei.cn/gtxktayhiu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.dianchejie.cn/gtwohqfqnx.html

JS:   new Date("2024-01-02")
来源：http://hz.yueranfly.top/gtizijvico.html

TS:   new Date("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtmiwxuknx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yongpay.top/gtnlwvgknq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cdnleiting.top/gtazbyvqta.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhixingplan.top/gtxpqhuita.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.tian-w.cn/gtuatpjkkx.html

[J04] 时间戳与日期互转
来源：http://hz.svipenyu.cn/gtgdtgfhlr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhaomingkeji.xyz/gtfslxbtyx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.haohaochexian.top/gttykxhvki.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.tanke756.top/gtmoylhszm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ydzc1.top/gticjyuqdo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hysaishi.cn/gtlszwrxla.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sxryk.cn/gtlfymazxm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yvedp.cn/gtvfglfesk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.gotoacloud.top/gtlfxjbduf.html

[J05] 时间加减（加 7 天）
来源：http://hz.daxiang520.top/gtoscnofaj.html

Py:   now + timedelta(days=7)
来源：http://hz.nanxuanxn.top/gtaxshbcca.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.fengsongda.top/gtzvgzzcwd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.feifeiyinyue.top/gtpddgrbto.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gotoacloud.top/gtwsipuevl.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinyuanbaomall.cn/gtrjcfnlya.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.snrcjt.cn/gtyqxlntce.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hongshengwenyu.top/gtggvhdqmy.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.nanxinkj.top/gtvhizfmjr.html

[J06] 计算两时间之差
来源：http://hz.yanxiufei.cn/gtmaaswxbc.html

Py:   (end - start).total_seconds()
来源：http://hz.tian-w.cn/gtcexoyzwc.html

PHP:  $end->diff($start)->days;
来源：http://hz.52xcode.cn/gtiicpbgyv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sweek.top/gtlhwczlpi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yvedp.cn/gtugskjhjf.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.gogol.net.cn/gthonyryma.html

Go:   end.Sub(start).Hours()
来源：http://hz.sxryk.cn/gtqocorbrq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.redwolf501.top/gtocbmnkru.html

C#:   (end - start).TotalSeconds
来源：http://hz.pycfn.com/gtoxdmdrgy.html

[J07] 比较两个日期
来源：http://hz.cashguo.top/gthfcfqfyt.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gotoacloud.top/gtgybupvbs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.kuanghao11.cn/gtwgvtsnmo.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.mhx1999.top/gtqfefvlpe.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gzhubu.top/gtusshfizp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yvedp.cn/gtmuczyqgf.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.tanke756.top/gtuownisdi.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gzhubu.top/gtghznsctk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.daria6918.cn/gtinpjhdyv.html

[J08] 提取年月日与星期
来源：http://hz.hnqzz.top/gtamylrbjh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.aizwys.cn/gtjiwrayif.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.haohaochexian.top/gtvxhpxvbx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.dashuyun.cn/gtraficgps.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yonumen.top/gtnmqpabue.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.nanxuanxn.top/gtjfkdubbo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenjidiqi.icu/gtakrqciqc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.fengsongda.top/gtbnwyftec.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ywan-chungtsiang.top/gtjqtxbvfd.html

[J09] 时区处理
来源：http://hz.cheryme.top/gtralrufmj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cdnleiting.top/gtwhcdnlju.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.sweek.top/gtnngpxyvs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhengqikj.top/gtkukwcfqv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangkeji.top/gtycjqnawp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xziqi.cn/gtkbjsuugv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jiagoushi.top/gtkarbgwbz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hywenlv.cn/gtevbttlgu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.feifeiyinyue.top/gtgvzssfwq.html

[J10] 取今天 / 本月第一天
来源：http://hz.sweek.top/gtasoksgto.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cucudq.cn/gtxemdoptr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zdqjudy.top/gtyqnvkhxr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.52xcode.cn/gtevoecejw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zdqjudy.top/gtnscnmlwu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhiwuduotai.top/gtxkyrisvy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinqigufen.top/gtrcieqocn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.redwolf501.top/gtbczasbru.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.smart0.xyz/gtixenolef.html

================================================================================
来源：http://hz.guowangkeji.top/gtjiyfibxr.html

K. JSON 与序列化
来源：http://hz.ivvv.top/gtscxcjrco.html

================================================================================
来源：http://hz.shzxlz.cn/gtxsbqidbv.html

[K01] 对象转 JSON 字符串
来源：http://hz.hnxiangtu.top/gtatfapipz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.guowangkeji.top/gtamwlrjua.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hfpthk.cn/gtynkbyzsi.html

JS:   JSON.stringify(obj)
来源：http://hz.xuetiantiany.cn/gtasxnhkwy.html

TS:   JSON.stringify(obj)
来源：http://hz.xinyue.icu/gtfrhzjaen.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yvedp.cn/gtrmmaauqf.html

Go:   json.Marshal(obj)
来源：http://hz.jyoumei.cn/gtftmbzbbp.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sufxvd.cn/gtxxdjibfb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhixingplan.top/gtgxrkhfxu.html

[K02] JSON 字符串转对象
来源：http://hz.ybcxt.top/gtjkzwyncj.html

Py:   json.loads(s)
来源：http://hz.guowangkeji.top/gtnjhyjssz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhaomingkeji.xyz/gtajfdiwko.html

JS:   JSON.parse(s)
来源：http://hz.hnxiangtu.top/gtjrmmhzng.html


<!-- 参考信息 -->