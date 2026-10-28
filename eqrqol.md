代发 wailian999

Java: u instanceof User
来源：http://hz.zdqjudy.top/gtajsaqtkb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.nanxuanxn.top/gtsfxkngor.html

Ruby: u.is_a?(User)
来源：http://hz.aizwys.cn/gtqkvccmhr.html

C#:   u is User
来源：http://hz.daria6918.cn/gtybpsnxvt.html

[G14] 数据类 / record
来源：http://hz.pycfn.com/gtkxwdqatp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhiwuduotai.top/gtmdpzqrpo.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sxryk.cn/gtyevseaex.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.sysykeji.top/gthwocsnet.html

TS:   type User = { name: string; age: number };
来源：http://hz.hammf.cn/gtuvnhzavl.html

Java: record User(String name, int age) {}
来源：http://hz.52xcode.cn/gtswazwlli.html

Go:   type User struct { Name string; Age int }
来源：http://hz.xziqi.cn/gtpihblklb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yvedp.cn/gtqznfdwvf.html

C#:   record User(string Name, int Age);
来源：http://hz.cashguo.top/gtvpmxpzsw.html

[G15] 枚举
来源：http://hz.redwolf501.top/gtfyylcffv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.tianlin.xyz/gtkdyfsaxw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yuanzhike.top/gthhwrofjx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.birdmap.top/gthtteajsq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hongshengwenyu.top/gtmgezwcxw.html

Java: enum Color { RED, GREEN }
来源：http://hz.hongshengwenyu.top/gtkiowzrwo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.316326.xyz/gtyjvgbflr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.chenlongwang.top/gtdkagbqap.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.mhx1999.top/gthqkvuvvn.html

[G16] 对象转数组 / 字典
来源：http://hz.hysaishi.cn/gtubmyovhw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.316326.xyz/gtgqpfmwzi.html

PHP:  get_object_vars($obj);
来源：http://hz.yanxiufei.cn/gtfloejnwf.html

JS:   Object.entries(obj)
来源：http://hz.jqgufenzy.top/gtxdwdkakl.html

TS:   Object.entries(obj)
来源：http://hz.yj20258888.top/gtuegnspyl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.tanke756.top/gtijvtrhsb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cucudq.cn/gtcmhtpvjv.html

Ruby: obj.instance_variables
来源：http://hz.havefunace.top/gtnjfnrcsp.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhixingplan.top/gtpwdhygiv.html

================================================================================
来源：http://hz.sufxvd.cn/gtyxyuafhp.html

H. 异常与错误处理
来源：http://hz.zhengqikj.top/gtybuxxdft.html

================================================================================
来源：http://hz.mhx1999.top/gtbqmtgebn.html

[H01] try / catch 基础
来源：http://hz.wangdashe.top/gtgnlqujpk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.wangdashe.top/gtatldviup.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jyoumei.cn/gtexbldliu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cdnleiting.top/gtaiqruiam.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.nwbrower.top/gtdjoukmpg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xylfe.cn/gtbdgqblvc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.guannengcc.top/gtwaxdjgky.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.wangdashe.top/gtjlxliwou.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shuidangran.top/gtayewrtjs.html

[H02] finally / ensure 收尾
来源：http://hz.havefunace.top/gtrlqugvsx.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.smart0.xyz/gtcdguocgc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtwtsmzgua.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gtafqntsmy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sufxvd.cn/gtbdwqrjgh.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtqgkndswx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yuanzhike.top/gtjmtkshdv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.wangdashe.top/gtopdagiaq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.pycfn.com/gtwzxzumuj.html

[H03] 主动抛出异常
来源：http://hz.iojbl.cn/gtetmmtlpn.html

Py:   raise ValueError("错误信息")
来源：http://hz.gotoacloud.top/gtlglpwikq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.0kj1m.cn/gtfarbytox.html

JS:   throw new Error("错误信息");
来源：http://hz.sufxvd.cn/gtjjeidcda.html

TS:   throw new Error("错误信息");
来源：http://hz.ivvv.top/gtdqseykaz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.pycfn.com/gtdiqtllss.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.meibo888.top/gtdeiungrr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.52xcode.cn/gtrviqbkcr.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hammf.cn/gtlsrcowct.html

[H04] 自定义异常类型
来源：http://hz.fzhhl.top/gttixkpriw.html

Py:   class MyError(Exception): pass
来源：http://hz.jinghuilouyu.cn/gtffkkyvpm.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yanxiufei.cn/gtmnuiyccx.html

JS:   class MyError extends Error {}
来源：http://hz.ydzc1.top/gtlnyidxko.html

TS:   class MyError extends Error {}
来源：http://hz.haohaochexian.top/gtbohhrxxf.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jinqigufen.top/gtkdmoknhw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.meibo888.top/gttqvgvpni.html

Ruby: class MyError < StandardError; end
来源：http://hz.yvedp.cn/gtpbqozomp.html

C#:   class MyException : Exception {}
来源：http://hz.ehwqpu.com/gtuwqkrkay.html

[H05] 捕获特定类型
来源：http://hz.bjfxy.top/gtyniuoaej.html

Py:   except ValueError as e:
来源：http://hz.birdmap.top/gtezgwygll.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.redwolf501.top/gtbgvmfzfg.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jinyuanbaomall.cn/gttsvjdeqb.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.feifeiyinyue.top/gttnxsudoc.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhijiandao.cn/gtnqyrzfpg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.9152youxi.cn/gtldebagya.html

Ruby: rescue ArgumentError => e
来源：http://hz.vqdsnc.cn/gtdyyyqzhw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ehwqpu.com/gtrklhzbzr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.dianchejie.cn/gtmamsdmdb.html

Py:   value = d.get("k") or default
来源：http://hz.jinqigfzy.top/gtfbdnknww.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.wangdashe.top/gtpwiyoueo.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gaohongyu789.top/gtyxtqppff.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.tianlin.xyz/gtaslokrsi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yongpay.top/gtfaiprkah.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.gotoacloud.top/gtlyuqhvmh.html

Ruby: d&.dig(:a, :b)
来源：http://hz.sxryk.cn/gtlomyuwaw.html

C#:   obj?.A?.B ?? default
来源：http://hz.jyoumei.cn/gtqwfmqmwl.html

[H07] 断言
来源：http://hz.yanxiufei.cn/gtoghrrkji.html

Py:   assert x > 0, "必须为正"
来源：http://hz.birdmap.top/gtofwikimg.html

PHP:  assert($x > 0);
来源：http://hz.cashguo.top/gtcsecuxyk.html

JS:   console.assert(x > 0);
来源：http://hz.cucudq.cn/gtrhyxudct.html

TS:   console.assert(x > 0);
来源：http://hz.sxryk.cn/gtdtnucbon.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yuanzhike.top/gtomjkenqz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.nwbrower.top/gtxkfctuuw.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yuanzhike.top/gtkhibqqvo.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yvedp.cn/gtegxlocht.html

[H08] 获取错误信息与堆栈
来源：http://hz.316326.xyz/gtmqqxxajw.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.smart0.xyz/gtxmlwwmvw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shangyingyoupin.top/gtfhckjcvg.html

JS:   e.message;  e.stack
来源：http://hz.yongpay.top/gtogbaksre.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.aizwys.cn/gtmvtwpgna.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cheryme.top/gtoozqxnxb.html

Go:   err.Error()
来源：http://hz.jyoumei.cn/gtmutixrfd.html

Ruby: e.message;  e.backtrace
来源：http://hz.guannengcc.top/gtghhosmjx.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jlsjyb.cn/gttyvvlarh.html

[H09] 带错误码的异常
来源：http://hz.wangshuangyany.cn/gtifnldwnz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhixingplan.top/gtoxgqjhmb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shanyushiyangtech.top/gtycspclrs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.meibo888.top/gtwqeyjjqf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hongshengwenyu.top/gtqbfslqof.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.9152youxi.cn/gtbvzfemii.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hnqzz.top/gtjixdgdfl.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.dianchejie.cn/gtmwdbskhk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.0kj1m.cn/gtlqszyxyz.html

[H10] 资源自动释放
来源：http://hz.hongshengwenyu.top/gtymrlhjtr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.dianchejie.cn/gtnclwynqr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.svipenyu.cn/gtaoxfmmuy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ydjk.org.cn/gtpjupqeaq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangkeji.top/gtzowdanll.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.haohaochexian.top/gtzhxvhmhs.html

Go:   defer f.Close()
来源：http://hz.zdqjudy.top/gtejdlzqmh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yonumen.top/gtfqphbaub.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jiagoushi.top/gtuatxbsez.html

================================================================================
来源：http://hz.aibaodan.cn/gtzokfcdlg.html

I. 正则表达式
来源：http://hz.yanxiufei.cn/gtnitlbvba.html

================================================================================
来源：http://hz.yuanzhike.top/gtdsilaama.html

[I01] 判断是否匹配
来源：http://hz.svipenyu.cn/gtaflopjbu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shanyushiyangkeji.top/gtnvfvegmo.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.daria6918.cn/gtpoerkori.html

JS:   /\d+/.test(s)
来源：http://hz.yonumen.top/gtgancyoec.html

TS:   /\d+/.test(s)
来源：http://hz.hnqzz.top/gtmlvtlxme.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.wangshuangyany.cn/gtjzmmjdsw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shanyushiyangtech.top/gtsvjpolkn.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinqigfzy.top/gtlkvbqazp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xingfuxueyuan.xyz/gtumwporan.html

[I02] 提取所有匹配
来源：http://hz.yueranfly.top/gtmeospgdr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.mhx1999.top/gthzfyuwbj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yangfankeji.com/gtzgyqacux.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xziqi.cn/gtzqsjblva.html

TS:   s.match(/\d+/g)
来源：http://hz.aibaodan.cn/gtfbsjqjen.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinyuanbaomall.cn/gtpaqzwkso.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hysaishi.cn/gtzghmihrf.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhongyouzk.top/gtdplkhtlv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.wangdashe.top/gtnnikecyb.html

[I03] 提取捕获分组
来源：http://hz.yj20258888.top/gtknhsomka.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.meibo888.top/gtqtrabfjq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.mhx1999.top/gtjhpetrbp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yongpay.top/gtmqhwfsrh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ivvv.top/gtpqmgmwcv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.dashuyun.cn/gtrnkhcwhj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hywenlv.cn/gtfpelfqid.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinqigufen.top/gtzdmluxrv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.quarkkingdee.top/gtthahbnmp.html

[I04] 正则替换
来源：http://hz.shzxlz.cn/gtffjjsdgl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.nwbrower.top/gtqrolkdbk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.daxiang520.top/gtyondqgdt.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.fzhhl.top/gtsbffkqgs.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.dashuyun.cn/gtrnkedpmz.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.daxiang520.top/gtlrydzvaf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.sweek.top/gtjpcncwvj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.kuanghao11.cn/gtdynqlkye.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sweek.top/gtzcmzcqip.html

[I05] 按正则拆分
来源：http://hz.quarkkingdee.top/gtjtssduqc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hywenlv.cn/gtwxnilssg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.tanke756.top/gtoivdshsc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yj20258.top/gtnwbiwxcl.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.nanxuanxn.top/gtbjaphmiw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenlongwang.top/gtziabfqrw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.c1oappe.top/gtgjejfkrl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sysykeji.top/gtmyivcnei.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhaomingkeji.xyz/gtczgjqxvr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yuxming.cn/gtpjarxhbw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.vqdsnc.cn/gtcwcyviur.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ywan-chungtsiang.top/gtalviccxs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cucudq.cn/gtddrofzwf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yuanzhike.top/gtsoocbhgr.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xingfuxueyuan.xyz/gtijgxxzka.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hfpthk.cn/gtifmrqtqv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhixingplan.top/gtvlcydqaw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.chenjidiqi.icu/gtlyoiyhds.html

[I07] 忽略大小写与多行模式
来源：http://hz.haohaochexian.top/gtizybljir.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ydjk.org.cn/gtuewxecta.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.9152youxi.cn/gtxfpgvtne.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinyuanbaomall.cn/gtnscrcpgt.html

TS:   /error/gim
来源：http://hz.chenjidiqi.icu/gtodvgafns.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zdqjudy.top/gtrplyuckw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.daxiang520.top/gtzbavbjkk.html

Ruby: s.scan(/error/i)
来源：http://hz.iojbl.cn/gtgfxwhmwb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.havefunace.top/gtybbwkkqt.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.chenzaomai.com/gtcwiloiql.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.gogol.net.cn/gtgdavxkgz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.pengpengdd.cyou/gtmeddvmtu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sweek.top/gtwpvqwifa.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hysaishi.cn/gtzdovqdpr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.dianchejie.cn/gtlfuuwmcr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.daria6918.cn/gtikwkvksi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yanxiufei.cn/gtasejojke.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.haohaochexian.top/gtywvpumyk.html

================================================================================
来源：http://hz.bjfxy.top/gthreqnpad.html

J. 日期与时间
来源：http://hz.yanxiufei.cn/gtebmoieqy.html

================================================================================
来源：http://hz.9152youxi.cn/gtioyimoww.html

[J01] 获取当前时间
来源：http://hz.xinyue.icu/gtxwrwbosa.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhixingplan.top/gtiqhyolry.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.daria6918.cn/gtdhjplvvj.html

JS:   new Date();  Date.now()
来源：http://hz.yj20258888.top/gtesowshac.html

TS:   new Date();  Date.now()
来源：http://hz.kuanghao11.cn/gtgfngnfds.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.meibo888.top/gtupxdawad.html

Go:   time.Now()
来源：http://hz.ivvv.top/gtycrhzhzj.html

Ruby: Time.now
来源：http://hz.cdnleiting.top/gtzhksihxy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xylfe.cn/gtpssgrekc.html

[J02] 格式化输出
来源：http://hz.hongshengwenyu.top/gtjemrshkq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.bjfxy.top/gtkngpznak.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.svipenyu.cn/gtwaniksxc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jinyuanbaomall.cn/gtmkblaepm.html

TS:   d.toISOString()
来源：http://hz.feifeiyinyue.top/gtuwrdppxx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.mhx1999.top/gtpwtfmvhg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.fengsongda.top/gtdwyzrdqj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tanke756.top/gtxjildxdb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shangyingyoupin.top/gtwvdkshgu.html

[J03] 字符串解析为日期
来源：http://hz.zhixingplan.top/gtzompesan.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jqgufenzy.top/gtwlkmznbv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhixingplan.top/gtmlzcidhz.html

JS:   new Date("2024-01-02")
来源：http://hz.nanxinkj.top/gtcfflpomk.html

TS:   new Date("2024-01-02")
来源：http://hz.haohaochexian.top/gtbderxkii.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yonumen.top/gttgtvxzhq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtumbehmyn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ppjwa.cn/gtyowoqdvo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinqigfzy.top/gtejcqtrzi.html

[J04] 时间戳与日期互转
来源：http://hz.zhijiandao.cn/gtgourkoke.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.c1oappe.top/gtbkamykrq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.0kj1m.cn/gtqtslcljn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.guannengcc.top/gthdaziuwv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.mhx1999.top/gtbftkiqfu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hywenlv.cn/gtpwxsobin.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yonumen.top/gtmtogjiep.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.52xcode.cn/gtzrhuzwhw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhengqikj.top/gtawewsecv.html

[J05] 时间加减（加 7 天）
来源：http://hz.52xcode.cn/gtzecvcspx.html

Py:   now + timedelta(days=7)
来源：http://hz.pycfn.com/gtgtfwjxog.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hfpthk.cn/gttvkrammi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangshuangyany.cn/gtzacnclwo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenlongwang.top/gtsdfyfwvj.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.guannengcc.top/gtyjndenhj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.gzhubu.top/gtltchfgcc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hfpthk.cn/gtfwhatnst.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.haohaochexian.top/gtldcuztcs.html

[J06] 计算两时间之差
来源：http://hz.chenlongwang.top/gtcmosvdve.html

Py:   (end - start).total_seconds()
来源：http://hz.chenjidiqi.icu/gtesmcjkyb.html

PHP:  $end->diff($start)->days;
来源：http://hz.hnxiangtu.top/gtxsmhutll.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinqigfzy.top/gtbzasrbrh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.havefunace.top/gtnlhwtbgw.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.tianlin.xyz/gtlddwdhri.html

Go:   end.Sub(start).Hours()
来源：http://hz.sxryk.cn/gtkwfcrqry.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gotoacloud.top/gtajgyzeln.html

C#:   (end - start).TotalSeconds
来源：http://hz.shanyushiyangtech.top/gtrparyyna.html

[J07] 比较两个日期
来源：http://hz.xuanzx.com/gtdqaazjxw.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.daxiang520.top/gtawqpjqri.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shangyingyoupin.top/gtxkiaqusg.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258888.top/gtdqdfslsg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.svipenyu.cn/gtbcrmeqcw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cqqwz.cn/gtryengfkn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.svipenyu.cn/gtoillmnvk.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sweek.top/gtxzsfscpc.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.c1oappe.top/gtdjerdimp.html

[J08] 提取年月日与星期
来源：http://hz.smart0.xyz/gttxfxazgb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.meibo888.top/gtqxbgqmxr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jlsjyb.cn/gtqsyuymet.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sufxvd.cn/gttgqnfkuq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.pengpengdd.cyou/gtoshjgomk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.52xcode.cn/gtnyjcucps.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shzxlz.cn/gtekoaqtsq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yangfankeji.com/gtichubmdt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.c1oappe.top/gtnyowafpr.html

[J09] 时区处理
来源：http://hz.zhijiandao.cn/gtqlatoxpo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gaohongyu789.top/gtlkjyqrcz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jiagoushi.top/gtjxvusoxp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhongyouzk.top/gtkjwisrfw.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gaohongyu789.top/gtnfiqaufj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.tian-w.cn/gtcbyilawy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yvedp.cn/gtzoaykmfk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.daxiang520.top/gttdgixsos.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hnqzz.top/gtvkgrycvq.html

[J10] 取今天 / 本月第一天
来源：http://hz.9152youxi.cn/gtuvgthfsp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sysykeji.top/gtsyouchjf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.9152youxi.cn/gtslhjytbz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hnxiangtu.top/gtthsoafgc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yj202588.top/gtqdsasmpv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yj20258.top/gtclfyuyhw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.nanxuanxn.top/gtarxihozt.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.andypj.xyz/gtlvbpenad.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ywan-chungtsiang.top/gtonepnnat.html

================================================================================
来源：http://hz.yueranfly.top/gtjocxxdsk.html

K. JSON 与序列化
来源：http://hz.zhongyouzk.top/gtprcfbndx.html

================================================================================
来源：http://hz.jqgufenzy.top/gtwdytgfij.html

[K01] 对象转 JSON 字符串
来源：http://hz.hnqzz.top/gtrrtrkluk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yuanzhike.top/gtlagfjrwm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yueranfly.top/gtjhnzomun.html

JS:   JSON.stringify(obj)
来源：http://hz.yj202588.top/gtvahjmuwq.html

TS:   JSON.stringify(obj)
来源：http://hz.gotoacloud.top/gtzrisjbxg.html


<!-- 参考信息 -->