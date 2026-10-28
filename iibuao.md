代发 wailian999

PHP:  get_object_vars($obj);
来源：http://hz.0kj1m.cn/gtiivmgnjm.html

JS:   Object.entries(obj)
来源：http://hz.hywenlv.cn/gtyuawglrr.html

TS:   Object.entries(obj)
来源：http://hz.guowangkeji.top/gtqnqmjtoc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.cashguo.top/gtgmueygvt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jyoumei.cn/gtnjdxhtrh.html

Ruby: obj.instance_variables
来源：http://hz.redwolf501.top/gtatjksqvr.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yueranfly.top/gtgonxgkpt.html

================================================================================
来源：http://hz.hysaishi.cn/gthelptbdq.html

H. 异常与错误处理
来源：http://hz.daxiang520.top/gtfqkkrutf.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtnocafbxs.html

[H01] try / catch 基础
来源：http://hz.yueranfly.top/gtnnbkokdk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ywan-chungtsiang.top/gtjxiresaa.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.chenzaomai.com/gtwosjuisj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yueranfly.top/gtsdycftjv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zdqjudy.top/gtxwebpibj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.nanxuanxn.top/gtwfcehroo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yanxiufei.cn/gtqmpgdtlr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gotoacloud.top/gthhjdhcpn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ydjk.org.cn/gtdcssandy.html

[H02] finally / ensure 收尾
来源：http://hz.yongpay.top/gtjnazekgr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xuanzx.com/gtuyoefhsq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.gzhubu.top/gtdflxyrwg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.mhx1999.top/gtchufnqpi.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gtwspptqrf.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yonumen.top/gtzrrqmsrf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hnxiangtu.top/gtaimafedv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.smart0.xyz/gtwhzeipop.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtxzycmtag.html

[H03] 主动抛出异常
来源：http://hz.mhx1999.top/gtgbrpbfxq.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj202588.top/gttawjcmho.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.pycfn.com/gtrpsgbctp.html

JS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangkeji.top/gtqwoidqyl.html

TS:   throw new Error("错误信息");
来源：http://hz.snrcjt.cn/gtizkofbrp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sysykeji.top/gtxuvtjhlg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.dashuyun.cn/gtvfwcvgxo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.52xcode.cn/gtarocmyqu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gthkjdrnuq.html

[H04] 自定义异常类型
来源：http://hz.nwbrower.top/gtwxvkhuds.html

Py:   class MyError(Exception): pass
来源：http://hz.bjfxy.top/gtvzfijwhw.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xuetiantiany.cn/gtdyjikago.html

JS:   class MyError extends Error {}
来源：http://hz.jlsjyb.cn/gtdlugvocn.html

TS:   class MyError extends Error {}
来源：http://hz.mhx1999.top/gtwfrrfhgw.html

Java: class MyException extends RuntimeException {}
来源：http://hz.guannengcc.top/gtexcuxccj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.pengpengdd.cyou/gthojhpche.html

Ruby: class MyError < StandardError; end
来源：http://hz.tian-w.cn/gtbefrmvlb.html

C#:   class MyException : Exception {}
来源：http://hz.yvedp.cn/gtjrmkuyhl.html

[H05] 捕获特定类型
来源：http://hz.ydjk.org.cn/gtxeygtlsm.html

Py:   except ValueError as e:
来源：http://hz.cucudq.cn/gtdpjdyjdt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.kuanghao11.cn/gtzmcplzqp.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yuanzhike.top/gthvtbhyej.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ydjk.org.cn/gtpabqcbgi.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.daxiang520.top/gtufapvkbp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jlsjyb.cn/gtwxsgnevv.html

Ruby: rescue ArgumentError => e
来源：http://hz.52xcode.cn/gtzeiabkbz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.smart0.xyz/gtpraowdmc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhijiandao.cn/gtnbzwekew.html

Py:   value = d.get("k") or default
来源：http://hz.0kj1m.cn/gtyyatisgg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.aizwys.cn/gtxdqhcbxc.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hywenlv.cn/gtomvsbmlj.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.havefunace.top/gttwfnbydf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yuxming.cn/gtngvsqixn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shuidangran.top/gtuttzbhon.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ppjwa.cn/gtjglwfnil.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhaomingkeji.xyz/gthlygxlkr.html

[H07] 断言
来源：http://hz.chenjidiqi.icu/gtduzxkayf.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhongyouzk.top/gtdmwnrzqq.html

PHP:  assert($x > 0);
来源：http://hz.chenjidiqi.icu/gtaztcbgdj.html

JS:   console.assert(x > 0);
来源：http://hz.dashuyun.cn/gtmksfgvcr.html

TS:   console.assert(x > 0);
来源：http://hz.vqdsnc.cn/gthqggiuyt.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shzxlz.cn/gtlcuoxtch.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yvedp.cn/gtuogedhio.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xziqi.cn/gtlzhawczx.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sweek.top/gtqmyaxgzr.html

[H08] 获取错误信息与堆栈
来源：http://hz.ywan-chungtsiang.top/gtaitmsdcx.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hysaishi.cn/gtlbhsqqul.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.mhx1999.top/gtfclxcgka.html

JS:   e.message;  e.stack
来源：http://hz.c1oappe.top/gteocwajga.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shangyingyoupin.top/gtdeataskv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.snrcjt.cn/gtecendbaq.html

Go:   err.Error()
来源：http://hz.gzhubu.top/gtdighiydn.html

Ruby: e.message;  e.backtrace
来源：http://hz.bjfxy.top/gtblagvpkw.html

C#:   e.Message;  e.StackTrace
来源：http://hz.fengsongda.top/gtlmitejah.html

[H09] 带错误码的异常
来源：http://hz.gzhubu.top/gtqnwmpelc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhiwuduotai.top/gtdssvqtxp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.9152youxi.cn/gtblqxtfxz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.9152youxi.cn/gtszjbfvyi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.vqdsnc.cn/gtamydcnzy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hfpthk.cn/gtrfyhrxrn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shanyushiyangkeji.top/gtpzxamezb.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ydjk.org.cn/gtzkmpqzkq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.snrcjt.cn/gtdzapbair.html

[H10] 资源自动释放
来源：http://hz.cdnleiting.top/gteqdqjaqy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.andypj.xyz/gtndvrpdnb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xuanzx.com/gtzjluujwa.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.havefunace.top/gtifmevegq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.iojbl.cn/gtootnoalu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.kuanghao11.cn/gtdtzgltzp.html

Go:   defer f.Close()
来源：http://hz.redwolf501.top/gttgrrzygo.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hnqzz.top/gtrrhfbnow.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.andypj.xyz/gtnlbccwyl.html

================================================================================
来源：http://hz.jinqigufen.top/gtcljdudtm.html

I. 正则表达式
来源：http://hz.ywan-chungtsiang.top/gtoswovfau.html

================================================================================
来源：http://hz.dianchejie.cn/gtpcyprvax.html

[I01] 判断是否匹配
来源：http://hz.hammf.cn/gtcwpgkkbz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.meibo888.top/gtdtwzsgrv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gogol.net.cn/gtjggctelg.html

JS:   /\d+/.test(s)
来源：http://hz.shzxlz.cn/gtyqpnyybm.html

TS:   /\d+/.test(s)
来源：http://hz.zhaomingkeji.xyz/gtcfobdyit.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenlongwang.top/gtzckoxqch.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cucudq.cn/gtjmfoackt.html

Ruby: s.match?(/\d+/)
来源：http://hz.aizwys.cn/gteldykzhi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.vqdsnc.cn/gtensrrjsl.html

[I02] 提取所有匹配
来源：http://hz.zhaomingkeji.xyz/gtkwwbxrkt.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hysaishi.cn/gtrdotaeue.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zycfv.cn/gtngupimod.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ehwqpu.com/gtzxwjnbah.html

TS:   s.match(/\d+/g)
来源：http://hz.0kj1m.cn/gtzldreaqw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinghuilouyu.cn/gtqjfybrpp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jqgfzy.top/gtsopriswy.html

Ruby: s.scan(/\d+/)
来源：http://hz.yj20258888.top/gtywrdmgcz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.daria6918.cn/gtcmlpxvyk.html

[I03] 提取捕获分组
来源：http://hz.zhiwuduotai.top/gtbthlvlbk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jqgufenzy.top/gtpjegrbgx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jlsjyb.cn/gtnjfywjmi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.fzhhl.top/gthkvlgfbw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cucudq.cn/gtwgytixnd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gzhubu.top/gtoubgwtea.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jiagoushi.top/gtmbythkjv.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhongyouzk.top/gtbvkianjd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jinqigfzy.top/gtlfktltbp.html

[I04] 正则替换
来源：http://hz.hysaishi.cn/gtbowcdjga.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jianghu66.top/gtbalavnke.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zdqjudy.top/gtlztexbpv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ydjk.org.cn/gtybjhqjjq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.daria6918.cn/gtejubdqsi.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.guannengcc.top/gtrwmqajgf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.nwbrower.top/gtopbkjwrb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yonumen.top/gtzcziuzqn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.fzhhl.top/gtgoolfpxm.html

[I05] 按正则拆分
来源：http://hz.hysaishi.cn/gtgxfspesk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cheryme.top/gtdfcdwzas.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zycfv.cn/gtonhjwgnz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ppjwa.cn/gtmtirqyau.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zycfv.cn/gttpxskwyi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.gogol.net.cn/gtitfziudw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jinqigufen.top/gtnseopvdj.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtimvkjcyv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cashguo.top/gtbqosrxup.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.52xcode.cn/gtqgxaefql.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sxryk.cn/gtdkohcgjy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.chenzaomai.com/gtqzwhgqsu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yangfankeji.com/gtduhfkrjr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnxiangtu.top/gtsmqiblib.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.havefunace.top/gtffwoyokc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yanxiufei.cn/gtlursftbv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cucudq.cn/gtankygedf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yangfankeji.com/gtxmmlsdqy.html

[I07] 忽略大小写与多行模式
来源：http://hz.tanke756.top/gtantrhgew.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ydjk.org.cn/gtgksastnj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.52xcode.cn/gthfhitzld.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hywenlv.cn/gtirglxwsf.html

TS:   /error/gim
来源：http://hz.redwolf501.top/gtkdognypv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.guowangkeji.top/gtdxafkvxa.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhoulong.xyz/gtdtowjpvk.html

Ruby: s.scan(/error/i)
来源：http://hz.xinyue.icu/gtkwkgeksb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xziqi.cn/gtxwxumqgc.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.chenlongwang.top/gtqqpgxzok.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hywenlv.cn/gtzifoimtc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jqgufenzy.top/gtszspnjpv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenzaomai.com/gtphikjctd.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yonumen.top/gtaxeyegrm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cucudq.cn/gtvpatvcrf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cucudq.cn/gtohyfjlfg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yongpay.top/gtvwziywda.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jlsjyb.cn/gtfocwaleh.html

================================================================================
来源：http://hz.daria6918.cn/gtgtdxgmou.html

J. 日期与时间
来源：http://hz.fzhhl.top/gtuebukovk.html

================================================================================
来源：http://hz.yangfankeji.com/gtivarijtm.html

[J01] 获取当前时间
来源：http://hz.ehwqpu.com/gtycvpypxy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.tianlin.xyz/gtxfuvtklg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ydzc1.top/gthmwrrbtn.html

JS:   new Date();  Date.now()
来源：http://hz.quarkkingdee.top/gtkoicmiul.html

TS:   new Date();  Date.now()
来源：http://hz.haohaochexian.top/gtslbufdzq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhoulong.xyz/gtftafjlmv.html

Go:   time.Now()
来源：http://hz.jqgufenzy.top/gtwbwiyqkv.html

Ruby: Time.now
来源：http://hz.gotoacloud.top/gtnorbabkb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhengqikj.top/gtqjskhuwq.html

[J02] 格式化输出
来源：http://hz.dashuyun.cn/gtniussnik.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shzxlz.cn/gtmbzusvqa.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.dashuyun.cn/gtbkliklqp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ehwqpu.com/gtvmuaikmj.html

TS:   d.toISOString()
来源：http://hz.jinqigufen.top/gteciiwvgk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.havefunace.top/gtabnppwyu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hnqzz.top/gtxdkjrchb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhengqikj.top/gtkhnbdlom.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.tanke756.top/gtlbmtjzci.html

[J03] 字符串解析为日期
来源：http://hz.cdnleiting.top/gtpkwzwltq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.aibaodan.cn/gtepwfrnac.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sxryk.cn/gtwsymdaib.html

JS:   new Date("2024-01-02")
来源：http://hz.zhongyouzk.top/gtyrclavqn.html

TS:   new Date("2024-01-02")
来源：http://hz.cucudq.cn/gtccjczuzj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.c1oappe.top/gtcattnzyx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yangfankeji.com/gtcenmkgdj.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cdnleiting.top/gtvvpohzbz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhiwuduotai.top/gtauywssgq.html

[J04] 时间戳与日期互转
来源：http://hz.redwolf501.top/gtpsahwslz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hongshengwenyu.top/gtbggobqlq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shanyushiyangkeji.top/gtjhfzydrx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xingfuxueyuan.xyz/gtvcaidnql.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nanxinkj.top/gtlczkskye.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shanyushiyangtech.top/gtnvxsvxgf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.redwolf501.top/gtfmkxohiy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.bjfxy.top/gtunzqmofw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.feifeiyinyue.top/gtilqngspk.html

[J05] 时间加减（加 7 天）
来源：http://hz.feifeiyinyue.top/gtucertofo.html

Py:   now + timedelta(days=7)
来源：http://hz.cucudq.cn/gtaabtiabp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhixingplan.top/gtltrnbciw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dianchejie.cn/gtcuxpxyau.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhongyouzk.top/gtssthpfvp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.pengpengdd.cyou/gtcisphewq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jianghu66.top/gtdbespbtc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.kuanghao11.cn/gtdmvaibfx.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sweek.top/gttsprkmdn.html

[J06] 计算两时间之差
来源：http://hz.jlsjyb.cn/gtkkiaojba.html

Py:   (end - start).total_seconds()
来源：http://hz.ywan-chungtsiang.top/gtxzqcawfx.html

PHP:  $end->diff($start)->days;
来源：http://hz.ydjk.org.cn/gtkhksjsry.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shangyingyoupin.top/gtkfmvebll.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.iojbl.cn/gtwmlksudy.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xuetiantiany.cn/gtdmcgebvc.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhengqikj.top/gtrqjrulfb.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jqgufenzy.top/gtgrrkttqu.html

C#:   (end - start).TotalSeconds
来源：http://hz.gaohongyu789.top/gtogavwmst.html

[J07] 比较两个日期
来源：http://hz.guowangkeji.top/gtgstbphhu.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ydjk.org.cn/gtiifzprbj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.chenlongwang.top/gtxfpvrvnn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jyoumei.cn/gtggiotwej.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sufxvd.cn/gtuvacillk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.c1oappe.top/gtnvoyjkpz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xylfe.cn/gtycjedpym.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.vqdsnc.cn/gtrjfvpzwm.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.9152youxi.cn/gtjoqdeivx.html

[J08] 提取年月日与星期
来源：http://hz.hammf.cn/gtnshewpxc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jlsjyb.cn/gtfpcpmpxv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zdqjudy.top/gtvxkmkaai.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yj20258.top/gtrzlsxrnl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.guowangkeji.top/gtqtmddovc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.0kj1m.cn/gtcmihekaz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zdqjudy.top/gtavrlmudn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.shanyushiyangtech.top/gtycllpvnb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jlsjyb.cn/gtwuoiemhl.html

[J09] 时区处理
来源：http://hz.svipenyu.cn/gtvnuuukft.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.nanxuanxn.top/gtokasnbhk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hysaishi.cn/gtfggpfwlr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ehwqpu.com/gtzowrznml.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xingfuxueyuan.xyz/gthlxsfkwq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gogol.net.cn/gtmuodxmvz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhoulong.xyz/gtvbhjqlov.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.svipenyu.cn/gtlrdarfbq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shuidangran.top/gtwjjupwgb.html

[J10] 取今天 / 本月第一天
来源：http://hz.yueranfly.top/gtqfrllkfp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ydjk.org.cn/gtogwjfuds.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.snrcjt.cn/gtlefkfees.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.fengsongda.top/gtardjeumv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.aibaodan.cn/gtbniebdcu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinqigfzy.top/gtwxdqgipc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yuanzhike.top/gtoriwnqef.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jianghu66.top/gtxeaumqvu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.meibo888.top/gtmvrknuco.html

================================================================================
来源：http://hz.fengsongda.top/gthsbjdtve.html

K. JSON 与序列化
来源：http://hz.ydjk.org.cn/gtcaoycmeu.html

================================================================================
来源：http://hz.andypj.xyz/gtzwvbylor.html

[K01] 对象转 JSON 字符串
来源：http://hz.jqgfzy.top/gtnabdlnvm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.nanxuanxn.top/gtpxdgwlpm.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yongpay.top/gtsdjwodqm.html

JS:   JSON.stringify(obj)
来源：http://hz.iojbl.cn/gtgkkockfg.html

TS:   JSON.stringify(obj)
来源：http://hz.ywan-chungtsiang.top/gtfxvwghff.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.redwolf501.top/gtgohkrdtl.html

Go:   json.Marshal(obj)
来源：http://hz.yanxiufei.cn/gtmmdhrvkv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ywan-chungtsiang.top/gtxelzhlyq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shuidangran.top/gtditrdktk.html

[K02] JSON 字符串转对象
来源：http://hz.jyoumei.cn/gtrniasgqt.html

Py:   json.loads(s)
来源：http://hz.chenjidiqi.icu/gtwjecwsmk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yj20258.top/gthfevynfm.html

JS:   JSON.parse(s)
来源：http://hz.andypj.xyz/gtekzmrhah.html

TS:   JSON.parse(s)
来源：http://hz.c1oappe.top/gtvwcvusyc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hammf.cn/gtkphelfjc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shangyingyoupin.top/gtrowwgbzm.html

Ruby: JSON.parse(s)
来源：http://hz.sysykeji.top/gtbdouucdj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.pycfn.com/gtfspkuule.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hnqzz.top/gtlynqpvun.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.fengsongda.top/gtxiovktqe.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.aizwys.cn/gtflcwjqsf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yanxiufei.cn/gtmtanzkzr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.9152youxi.cn/gtewwhgzsa.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.0kj1m.cn/gtdyxyxyvi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.vqdsnc.cn/gtsrnomowb.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.svipenyu.cn/gtqnjjfzcn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.daxiang520.top/gtohychzac.html

[K04] 读取 JSON 文件
来源：http://hz.daria6918.cn/gtnrffkurh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ppjwa.cn/gtrurvvoxu.html


<!-- 参考信息 -->