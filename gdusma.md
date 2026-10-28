代发 wailian999

Py:   isinstance(u, User)
来源：http://hz.zhixingplan.top/gteyzkvxnf.html

PHP:  $u instanceof User
来源：http://hz.tianlin.xyz/gtdrnlrddk.html

JS:   u instanceof User
来源：http://hz.hnxiangtu.top/gtlclfmnmh.html

TS:   u instanceof User
来源：http://hz.sysykeji.top/gtscomtcdk.html

Java: u instanceof User
来源：http://hz.jlsjyb.cn/gtnrkznjum.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.guannengcc.top/gtdsjytwza.html

Ruby: u.is_a?(User)
来源：http://hz.tanke756.top/gtfljvmqjd.html

C#:   u is User
来源：http://hz.yj202588.top/gtcruriwnv.html

[G14] 数据类 / record
来源：http://hz.nanxinkj.top/gtxvkmogjt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.redwolf501.top/gtwadhktiu.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yanxiufei.cn/gtpzezrjxh.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.tanke756.top/gtabpxzqzi.html

TS:   type User = { name: string; age: number };
来源：http://hz.316326.xyz/gtbwmpktwp.html

Java: record User(String name, int age) {}
来源：http://hz.wangshuangyany.cn/gtlvmkdcyw.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yj202588.top/gtijsgiofk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.daxiang520.top/gtxpducbvp.html

C#:   record User(string Name, int Age);
来源：http://hz.nanxinkj.top/gtnahborhu.html

[G15] 枚举
来源：http://hz.guannengcc.top/gtfmwcptse.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xuetiantiany.cn/gttnnvkqvq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.svipenyu.cn/gtzabkqlyf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.daria6918.cn/gtxdznujus.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnxiangtu.top/gtpkzyicwz.html

Java: enum Color { RED, GREEN }
来源：http://hz.meibo888.top/gtbslzzkhw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.9152youxi.cn/gtczraxnya.html

Ruby: Color = %i[red green].freeze
来源：http://hz.316326.xyz/gtgzzjutfg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.mhx1999.top/gtetzokjll.html

[G16] 对象转数组 / 字典
来源：http://hz.yongpay.top/gtjxkenkqh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hfpthk.cn/gtbrhezpti.html

PHP:  get_object_vars($obj);
来源：http://hz.hnxiangtu.top/gtuodjupia.html

JS:   Object.entries(obj)
来源：http://hz.yuanzhike.top/gtbjmdrsed.html

TS:   Object.entries(obj)
来源：http://hz.zycfv.cn/gtrlkorucq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yongpay.top/gtqgysustw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hnxiangtu.top/gtzujqpuhh.html

Ruby: obj.instance_variables
来源：http://hz.cdnleiting.top/gtuytjehsd.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hongshengwenyu.top/gtnbbyewzn.html

================================================================================
来源：http://hz.haohaochexian.top/gtcipdwwcu.html

H. 异常与错误处理
来源：http://hz.gaohongyu789.top/gtyeprfupv.html

================================================================================
来源：http://hz.tianlin.xyz/gtvfmemygg.html

[H01] try / catch 基础
来源：http://hz.cqqwz.cn/gtmnfhnsjo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.sxryk.cn/gtsizldfsp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xingfuxueyuan.xyz/gtkjccbqxf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gotoacloud.top/gtbupfwuvx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yuxming.cn/gttivakbar.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.wangdashe.top/gtdzerubms.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.dianchejie.cn/gtocnxbojp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xylfe.cn/gtkqjxzsvd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.smart0.xyz/gtlybwasjx.html

[H02] finally / ensure 收尾
来源：http://hz.quarkkingdee.top/gtuvnkofgq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hnqzz.top/gtoujvmtit.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gtniritfif.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtmjjwqsrt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.316326.xyz/gttdadszoj.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtetrcvivp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.cheryme.top/gtpakhocxl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.andypj.xyz/gtcdrlrufj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.vqdsnc.cn/gtoklxifxg.html

[H03] 主动抛出异常
来源：http://hz.jiagoushi.top/gthtqlujoz.html

Py:   raise ValueError("错误信息")
来源：http://hz.cheryme.top/gteihihtxp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cdnleiting.top/gtosqgpikc.html

JS:   throw new Error("错误信息");
来源：http://hz.sxryk.cn/gtbctioill.html

TS:   throw new Error("错误信息");
来源：http://hz.cheryme.top/gtntybdwgk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gotoacloud.top/gtpvexipgo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhaomingkeji.xyz/gtgftmpxqc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhengqikj.top/gtrcwnckac.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yongpay.top/gtqkkmdtpd.html

[H04] 自定义异常类型
来源：http://hz.yj202588.top/gthokmqkwa.html

Py:   class MyError(Exception): pass
来源：http://hz.aizwys.cn/gtwgogdwbt.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.dashuyun.cn/gtwmyxbzan.html

JS:   class MyError extends Error {}
来源：http://hz.zhaomingkeji.xyz/gtguovlqhd.html

TS:   class MyError extends Error {}
来源：http://hz.jinyuanbaomall.cn/gtaspwclfy.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yueranfly.top/gtatcudnro.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shanyushiyangkeji.top/gtwnymjijy.html

Ruby: class MyError < StandardError; end
来源：http://hz.ydzc1.top/gtyrqjlwaq.html

C#:   class MyException : Exception {}
来源：http://hz.yj20258.top/gtsrkqfbpo.html

[H05] 捕获特定类型
来源：http://hz.kuanghao11.cn/gtayxgnbwf.html

Py:   except ValueError as e:
来源：http://hz.pengpengdd.cyou/gtwyrfrwnk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.9152youxi.cn/gthwdkiotx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yvedp.cn/gtialhgran.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hammf.cn/gtqgmfoqto.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yangfankeji.com/gtgzlshapt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yj20258888.top/gtbeqivyta.html

Ruby: rescue ArgumentError => e
来源：http://hz.yueranfly.top/gtksqjecwf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.havefunace.top/gtkrxoizxp.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhiwuduotai.top/gtakrwcxni.html

Py:   value = d.get("k") or default
来源：http://hz.jlsjyb.cn/gtecphntwq.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xinyue.icu/gtcawbspud.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cdnleiting.top/gtvcomlvdc.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zdqjudy.top/gtsbczhwmd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sxryk.cn/gttonnfgbe.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zdqjudy.top/gthueyvqvz.html

Ruby: d&.dig(:a, :b)
来源：http://hz.pengpengdd.cyou/gtjustfeuv.html

C#:   obj?.A?.B ?? default
来源：http://hz.chenjidiqi.icu/gtbcbtijfg.html

[H07] 断言
来源：http://hz.yuxming.cn/gtueybanzf.html

Py:   assert x > 0, "必须为正"
来源：http://hz.andypj.xyz/gtzfseixma.html

PHP:  assert($x > 0);
来源：http://hz.316326.xyz/gtmlsrhuoi.html

JS:   console.assert(x > 0);
来源：http://hz.chenzaomai.com/gtapaobfyo.html

TS:   console.assert(x > 0);
来源：http://hz.xuetiantiany.cn/gtvllczyzo.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ehwqpu.com/gtdkfvzixo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.daria6918.cn/gturshsegk.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.mhx1999.top/gtjhgskmaa.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jlsjyb.cn/gtwdfycfwh.html

[H08] 获取错误信息与堆栈
来源：http://hz.ehwqpu.com/gtvuxqmeuk.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.wangdashe.top/gtmdofhbpi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.bjfxy.top/gtctxpwvyj.html

JS:   e.message;  e.stack
来源：http://hz.smart0.xyz/gtaenenyxk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.sweek.top/gtebehvwlb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sufxvd.cn/gtbryzmeaa.html

Go:   err.Error()
来源：http://hz.yj20258888.top/gtstirjkll.html

Ruby: e.message;  e.backtrace
来源：http://hz.vqdsnc.cn/gtswlxbgyy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cqqwz.cn/gtykfdluhu.html

[H09] 带错误码的异常
来源：http://hz.jiagoushi.top/gtipxjbahb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yongpay.top/gthvffknpz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhixingplan.top/gtpqubbboe.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.52xcode.cn/gtnzjzkcxj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.bjfxy.top/gtstsfgzmc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.redwolf501.top/gtspkrztus.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.pycfn.com/gtyxyixkss.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shangyingyoupin.top/gtfabtuybh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.mhx1999.top/gtretollbb.html

[H10] 资源自动释放
来源：http://hz.xinyue.icu/gtmotuekfd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zycfv.cn/gtcguhczgk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jianghu66.top/gteyvvifmn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxuanxn.top/gtwlslilzw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.wangdashe.top/gtgxnnjzzy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhongyouzk.top/gthxhkkexf.html

Go:   defer f.Close()
来源：http://hz.xingfuxueyuan.xyz/gtfbqrywav.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.gotoacloud.top/gtvqcxkwnf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yj202588.top/gteenhnsiq.html

================================================================================
来源：http://hz.dianchejie.cn/gtpcwpezvq.html

I. 正则表达式
来源：http://hz.ywan-chungtsiang.top/gteuvsbroq.html

================================================================================
来源：http://hz.shzxlz.cn/gtjfepzgox.html

[I01] 判断是否匹配
来源：http://hz.xziqi.cn/gtmpinpuxl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jinqigfzy.top/gteadwubmx.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ivvv.top/gtpxagmbal.html

JS:   /\d+/.test(s)
来源：http://hz.nwbrower.top/gtzimwracf.html

TS:   /\d+/.test(s)
来源：http://hz.316326.xyz/gtwkznivvg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.feifeiyinyue.top/gtgkbwapft.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yonumen.top/gtujnuvvnx.html

Ruby: s.match?(/\d+/)
来源：http://hz.cdnleiting.top/gtsrzklyqu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jqgfzy.top/gtnbdvtnrp.html

[I02] 提取所有匹配
来源：http://hz.yanxiufei.cn/gtssulxwnl.html

Py:   re.findall(r"\d+", s)
来源：http://hz.316326.xyz/gtshyeosjh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.daxiang520.top/gtyymtrkoz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yuanzhike.top/gtmwjuzjqf.html

TS:   s.match(/\d+/g)
来源：http://hz.ybcxt.top/gtxwkiypwk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhijiandao.cn/gtpujrftwy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.chenzaomai.com/gtcplzofil.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhiwuduotai.top/gtoyvebjqf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gotoacloud.top/gtewecgvet.html

[I03] 提取捕获分组
来源：http://hz.zhongyouzk.top/gtxevvsrjt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.chenlongwang.top/gtnnpfjbjc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jianghu66.top/gtfoyqycto.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.haohaochexian.top/gtfjrcdgdk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shuidangran.top/gttukbulfl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shanyushiyangtech.top/gtskcpmofg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jqgfzy.top/gtemientma.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yuanzhike.top/gtbwrxfhwq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.kuanghao11.cn/gtsktoizst.html

[I04] 正则替换
来源：http://hz.meibo888.top/gthpolymqk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.mhx1999.top/gtdjlvedyt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sysykeji.top/gtcokhyvjy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.316326.xyz/gttzjdhnbx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zdqjudy.top/gttmhsaekt.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.shanyushiyangtech.top/gtycploqhp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cqqwz.cn/gtdcgcqbtu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cqqwz.cn/gtgzxujhjg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.guowangkeji.top/gtihtjndli.html

[I05] 按正则拆分
来源：http://hz.52xcode.cn/gtaxrkfdep.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.wangshuangyany.cn/gtjtrdbhrn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.quarkkingdee.top/gtnevohrga.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.bjfxy.top/gtdqwtfwiu.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xuanzx.com/gtzhmvzjlx.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cheryme.top/gtvoxtonjc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.birdmap.top/gtgkbwstat.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.dianchejie.cn/gtftsyonjl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yanxiufei.cn/gtuwoukogw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jiagoushi.top/gtxdnjrwyh.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hongshengwenyu.top/gtdcdwqtpx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cdnleiting.top/gtgztzqsvp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.mhx1999.top/gtmrwbixls.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.dashuyun.cn/gtqyrhwskb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hnxiangtu.top/gtvvjbiasx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.9152youxi.cn/gtedgugjkl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yangfankeji.com/gtwkcdjjed.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yueranfly.top/gtsmjqrfqu.html

[I07] 忽略大小写与多行模式
来源：http://hz.xuetiantiany.cn/gtesqorbum.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.meibo888.top/gtuhdifiqd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.gotoacloud.top/gtfeligdji.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yangfankeji.com/gtzkgutqra.html

TS:   /error/gim
来源：http://hz.fengsongda.top/gtaxeezvkt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.daria6918.cn/gtdbfiicus.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.iojbl.cn/gtqmsnndhz.html

Ruby: s.scan(/error/i)
来源：http://hz.zhengqikj.top/gtwnpxbhae.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinyuanbaomall.cn/gtkbhibama.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sysykeji.top/gttnduzfhm.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.dashuyun.cn/gtsnkbvzpf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xuanzx.com/gtmhkrfiik.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ydjk.org.cn/gtwecoxieo.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zdqjudy.top/gtnsiudnku.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ehwqpu.com/gtggmqxsva.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.redwolf501.top/gttjbxldkv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.tanke756.top/gtblvvnlgq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhengqikj.top/gtnwjeeabk.html

================================================================================
来源：http://hz.chenlongwang.top/gttwvkergo.html

J. 日期与时间
来源：http://hz.yj20258.top/gtgnbxjsmt.html

================================================================================
来源：http://hz.c1oappe.top/gttorkwvoz.html

[J01] 获取当前时间
来源：http://hz.shangyingyoupin.top/gtgllgpyou.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.aizwys.cn/gtnvbuigva.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.snrcjt.cn/gtpgpsbpel.html

JS:   new Date();  Date.now()
来源：http://hz.xziqi.cn/gttjhnkriw.html

TS:   new Date();  Date.now()
来源：http://hz.hnqzz.top/gtghewxrsm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shzxlz.cn/gtpromblxp.html

Go:   time.Now()
来源：http://hz.0kj1m.cn/gtvapthxzd.html

Ruby: Time.now
来源：http://hz.chenzaomai.com/gtnxvcygjf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shzxlz.cn/gtjnnhnpze.html

[J02] 格式化输出
来源：http://hz.iojbl.cn/gtnaqhdlrc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.havefunace.top/gtwuuqzujt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yj20258888.top/gtxjtzglgo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ydjk.org.cn/gtkxczxmps.html

TS:   d.toISOString()
来源：http://hz.yj20258.top/gtogrpvibm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.andypj.xyz/gtsyqzumbd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.wangshuangyany.cn/gtxwghgedf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cashguo.top/gtcqffigga.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xylfe.cn/gtvbhmhyfl.html

[J03] 字符串解析为日期
来源：http://hz.dianchejie.cn/gtjhsshcaa.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.kuanghao11.cn/gtlidwyeta.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.aizwys.cn/gtbtvckrwp.html

JS:   new Date("2024-01-02")
来源：http://hz.c1oappe.top/gtbgeqoijr.html

TS:   new Date("2024-01-02")
来源：http://hz.yj202588.top/gtwfsqvtnw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.meibo888.top/gtkgifovvt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.vqdsnc.cn/gtiryihlfb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ivvv.top/gtdgfputpq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jqgfzy.top/gthvgpvddf.html

[J04] 时间戳与日期互转
来源：http://hz.jqgfzy.top/gtgofigfmi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.andypj.xyz/gtublnfalc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.316326.xyz/gtccdfztik.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gogol.net.cn/gtpkssbpzm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xingfuxueyuan.xyz/gtporejjpi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.0kj1m.cn/gtmkoxpmeq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhixingplan.top/gtmspkvpop.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.meibo888.top/gtzrccrerb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhijiandao.cn/gtoqjzibez.html

[J05] 时间加减（加 7 天）
来源：http://hz.jinghuilouyu.cn/gthshuhvaw.html

Py:   now + timedelta(days=7)
来源：http://hz.yangfankeji.com/gtpimbwhmv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhengqikj.top/gtpbidtzbt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fengsongda.top/gthwkevqvo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ehwqpu.com/gtjoifpgux.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cqqwz.cn/gtgurnhpjt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yangfankeji.com/gtoibwmvwb.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cqqwz.cn/gtvokyqxcq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.kuanghao11.cn/gtrkkieikk.html

[J06] 计算两时间之差
来源：http://hz.shzxlz.cn/gtgkhnhjty.html

Py:   (end - start).total_seconds()
来源：http://hz.kuanghao11.cn/gtckingwmr.html

PHP:  $end->diff($start)->days;
来源：http://hz.haohaochexian.top/gtintgpfpl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.dianchejie.cn/gtkwrddoxe.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yvedp.cn/gtnrxwhwuh.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.fzhhl.top/gtbrkxnykw.html

Go:   end.Sub(start).Hours()
来源：http://hz.smart0.xyz/gtibkedaag.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sweek.top/gtguabwwga.html

C#:   (end - start).TotalSeconds
来源：http://hz.ywan-chungtsiang.top/gtamhkuwix.html

[J07] 比较两个日期
来源：http://hz.yuanzhike.top/gtsqhmrdtp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gtbwndkmit.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shzxlz.cn/gtcdqyhjpc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.pycfn.com/gtvmywjrtv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gotoacloud.top/gtbnsphshz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shuidangran.top/gtbifebawm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gogol.net.cn/gtzdunzoxl.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ybcxt.top/gtbxyqtesp.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.0kj1m.cn/gtruleieuk.html

[J08] 提取年月日与星期
来源：http://hz.9152youxi.cn/gtkwpdogzv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.birdmap.top/gtfhhbaxbx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zdqjudy.top/gtnffqbwsx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xinyue.icu/gtvlantnrs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.nwbrower.top/gtmrjhjrgj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.sufxvd.cn/gtbgzxgocp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenlongwang.top/gtkaqztqir.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.birdmap.top/gtuiugplga.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.guowangkeji.top/gtknyrntsu.html

[J09] 时区处理
来源：http://hz.daria6918.cn/gtbmjynhyf.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.kuanghao11.cn/gtifdznqhw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jinyuanbaomall.cn/gttxjwzerm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinyuanbaomall.cn/gtdeoycfjd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xziqi.cn/gtliqfblpl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xylfe.cn/gtobhbxibt.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.birdmap.top/gthqkslson.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hammf.cn/gtbaghfccb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.svipenyu.cn/gtzdjzymuq.html

[J10] 取今天 / 本月第一天
来源：http://hz.jqgfzy.top/gttxhclmxf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhiwuduotai.top/gtejtmmsey.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cqqwz.cn/gterlimyaq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xuanzx.com/gtcqwagtqb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xuetiantiany.cn/gthtnrwsuh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yvedp.cn/gtbcbswwnh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.guannengcc.top/gtauozrlhu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gogol.net.cn/gtpwizfwka.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yuanzhike.top/gtgzudlqql.html

================================================================================
来源：http://hz.zhixingplan.top/gthccqlazl.html

K. JSON 与序列化
来源：http://hz.aibaodan.cn/gteacnjhpv.html

================================================================================
来源：http://hz.vqdsnc.cn/gtiehfnqrg.html

[K01] 对象转 JSON 字符串
来源：http://hz.kuanghao11.cn/gtvfagkkld.html


<!-- 参考信息 -->