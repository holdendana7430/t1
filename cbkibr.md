代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtlpudauzt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhiwuduotai.top/gtkgqpunwo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.feifeiyinyue.top/gtfbtkisss.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtjeoeibqy.html

[H03] 主动抛出异常
来源：http://hz.shuidangran.top/gtvaztdtca.html

Py:   raise ValueError("错误信息")
来源：http://hz.guowangkeji.top/gtetuefteo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shzxlz.cn/gtuhocawrw.html

JS:   throw new Error("错误信息");
来源：http://hz.pycfn.com/gtoctytlkb.html

TS:   throw new Error("错误信息");
来源：http://hz.jianghu66.top/gtvykznfeq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cashguo.top/gtxhhqndgk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hysaishi.cn/gtdljnjwxk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xziqi.cn/gttdviglmj.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jinghuilouyu.cn/gtxzneejdc.html

[H04] 自定义异常类型
来源：http://hz.yj20258888.top/gtjkvhrcjg.html

Py:   class MyError(Exception): pass
来源：http://hz.yj20258888.top/gtrxcyrani.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ybcxt.top/gtditsituu.html

JS:   class MyError extends Error {}
来源：http://hz.xylfe.cn/gtbxqghwpm.html

TS:   class MyError extends Error {}
来源：http://hz.zhiwuduotai.top/gtrfekfqjr.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gaohongyu789.top/gtnegutbii.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.chenlongwang.top/gtoaupmoeu.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhiwuduotai.top/gtawftoysr.html

C#:   class MyException : Exception {}
来源：http://hz.andypj.xyz/gtxaodpnia.html

[H05] 捕获特定类型
来源：http://hz.havefunace.top/gtkfgidfva.html

Py:   except ValueError as e:
来源：http://hz.nanxuanxn.top/gthbfhamlh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ehwqpu.com/gtmmzonvdx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yuanzhike.top/gtloqttrlh.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.andypj.xyz/gtwqmiejsz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhiwuduotai.top/gtrafzlqhc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yj20258.top/gtvmkmjonf.html

Ruby: rescue ArgumentError => e
来源：http://hz.zycfv.cn/gttdcurgvt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinqigufen.top/gtliwznhza.html

[H06] 可选值 / 空值安全访问
来源：http://hz.andypj.xyz/gtsnpdxjli.html

Py:   value = d.get("k") or default
来源：http://hz.zhoulong.xyz/gtrmyuxhau.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.redwolf501.top/gtxcpfggpn.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yuxming.cn/gtkffiurft.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinyuanbaomall.cn/gtukiosyia.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.9152youxi.cn/gtllbvwyhs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nanxuanxn.top/gtgiukwnmn.html

Ruby: d&.dig(:a, :b)
来源：http://hz.andypj.xyz/gtmtoayxzp.html

C#:   obj?.A?.B ?? default
来源：http://hz.andypj.xyz/gtmlxqlquk.html

[H07] 断言
来源：http://hz.iojbl.cn/gtcdildpjl.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shzxlz.cn/gtffyvkutc.html

PHP:  assert($x > 0);
来源：http://hz.hysaishi.cn/gtlksspawj.html

JS:   console.assert(x > 0);
来源：http://hz.yj20258888.top/gtwhgvtbsu.html

TS:   console.assert(x > 0);
来源：http://hz.gaohongyu789.top/gtecjbwlbt.html

Java: assert x > 0 : "必须为正";
来源：http://hz.aizwys.cn/gtfssxalen.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xinyue.icu/gtszrvfwkm.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ppjwa.cn/gttavcjqwr.html

C#:   Debug.Assert(x > 0);
来源：http://hz.meibo888.top/gtjqyvctqd.html

[H08] 获取错误信息与堆栈
来源：http://hz.birdmap.top/gtyzcrqyvi.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.smart0.xyz/gtirqyhyms.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cdnleiting.top/gtygqrkiut.html

JS:   e.message;  e.stack
来源：http://hz.fzhhl.top/gtgoycbbna.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.havefunace.top/gtaccmskdd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yongpay.top/gtymkijmtf.html

Go:   err.Error()
来源：http://hz.yj202588.top/gtuhwcygdv.html

Ruby: e.message;  e.backtrace
来源：http://hz.ybcxt.top/gthzmvsxic.html

C#:   e.Message;  e.StackTrace
来源：http://hz.guowangkeji.top/gtzyhdpvgh.html

[H09] 带错误码的异常
来源：http://hz.xingfuxueyuan.xyz/gtlkmnkwhk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xylfe.cn/gtpjnvugvv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sufxvd.cn/gtfrivjlmx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.svipenyu.cn/gtwueorste.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hysaishi.cn/gtohrwgnxt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ppjwa.cn/gtepmzwdaz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xuanzx.com/gtomzpmqae.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sysykeji.top/gtiofluzdv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.iojbl.cn/gtbskcyzee.html

[H10] 资源自动释放
来源：http://hz.sweek.top/gtcvdegzge.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.dianchejie.cn/gthcbbtjpd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinqigfzy.top/gtowqnfbsu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.kuanghao11.cn/gtyvanznzl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hammf.cn/gtewesmcod.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ivvv.top/gtmkzziwtm.html

Go:   defer f.Close()
来源：http://hz.fzhhl.top/gtbcheddeu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.fengsongda.top/gtmceneqjp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yueranfly.top/gtjswibwkf.html

================================================================================
来源：http://hz.birdmap.top/gtsyznvbdl.html

I. 正则表达式
来源：http://hz.shanyushiyangtech.top/gtxukttonu.html

================================================================================
来源：http://hz.gaohongyu789.top/gtqgtetwsz.html

[I01] 判断是否匹配
来源：http://hz.tianlin.xyz/gtewtqlknl.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.feifeiyinyue.top/gtkffduihh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xylfe.cn/gtrerfegiy.html

JS:   /\d+/.test(s)
来源：http://hz.gotoacloud.top/gtrctndqzw.html

TS:   /\d+/.test(s)
来源：http://hz.havefunace.top/gtxrsattns.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.0kj1m.cn/gtyoyjlkhf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ivvv.top/gthzgoffhf.html

Ruby: s.match?(/\d+/)
来源：http://hz.yj20258888.top/gtjnduvumd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hywenlv.cn/gtjlszafjl.html

[I02] 提取所有匹配
来源：http://hz.xziqi.cn/gttosagcqu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zdqjudy.top/gtygcxysbg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yangfankeji.com/gtlqiwgjvx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.fengsongda.top/gtbsirnipo.html

TS:   s.match(/\d+/g)
来源：http://hz.fzhhl.top/gtaavopacg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.birdmap.top/gtmkndmwgm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.redwolf501.top/gtpzorgmgk.html

Ruby: s.scan(/\d+/)
来源：http://hz.cheryme.top/gtnbukgfgr.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.svipenyu.cn/gtsnaekfqt.html

[I03] 提取捕获分组
来源：http://hz.ivvv.top/gtccnqdsha.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yvedp.cn/gtwbfolpxz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yvedp.cn/gtadwfnnio.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yuxming.cn/gtnsozgsws.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.iojbl.cn/gtbqkdtkst.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yongpay.top/gtkfloshhe.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nwbrower.top/gtqqqmsusx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hammf.cn/gtgcjcgoxu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.quarkkingdee.top/gtidetvtum.html

[I04] 正则替换
来源：http://hz.kuanghao11.cn/gtxctigzjd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hysaishi.cn/gtipcbriec.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ydzc1.top/gtjnjkealu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cucudq.cn/gtubdifzha.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shuidangran.top/gtesmanfgi.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.wangdashe.top/gtphzxngop.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.svipenyu.cn/gtvhjbicqn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nwbrower.top/gtjrztqvfr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.kuanghao11.cn/gthdhmixcy.html

[I05] 按正则拆分
来源：http://hz.sxryk.cn/gtfudfwvpk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jinqigufen.top/gtfpkyctxm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.daxiang520.top/gtxpqysgmq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jyoumei.cn/gtqtagwgoa.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gtgxkozgnw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhaomingkeji.xyz/gtheemqzuh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yangfankeji.com/gtnrxxpcff.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.cashguo.top/gtbfahzyuf.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hysaishi.cn/gtywnhydfd.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.aizwys.cn/gtkjuuwtml.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.wangdashe.top/gtvmnqlkqf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yuxming.cn/gtkfizlmvb.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.guannengcc.top/gtjazeejll.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hongshengwenyu.top/gtxmiiyeta.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.wangshuangyany.cn/gtuetkohdn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhiwuduotai.top/gtsoljhaba.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.pengpengdd.cyou/gtpgqbdxsu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jinyuanbaomall.cn/gtzmfsmsym.html

[I07] 忽略大小写与多行模式
来源：http://hz.feifeiyinyue.top/gtnkwywouw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhoulong.xyz/gtojfbtbdk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.quarkkingdee.top/gtsjaijyid.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.fengsongda.top/gtwxanqgix.html

TS:   /error/gim
来源：http://hz.ivvv.top/gtxgmlaizr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.svipenyu.cn/gtaydetsbz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhiwuduotai.top/gtmkouzazo.html

Ruby: s.scan(/error/i)
来源：http://hz.meibo888.top/gtelgjwimo.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.svipenyu.cn/gthswqjryg.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.smart0.xyz/gtucedgfmz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yongpay.top/gtsbctcpjv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xylfe.cn/gtryubptdm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuetiantiany.cn/gtzvzpqwye.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jyoumei.cn/gtmwreyniu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhijiandao.cn/gtnphrjvqt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.dianchejie.cn/gtxffrtpit.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ehwqpu.com/gthdxpzokg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gaohongyu789.top/gtsbeppnzw.html

================================================================================
来源：http://hz.kuanghao11.cn/gtailqjpyb.html

J. 日期与时间
来源：http://hz.316326.xyz/gtotoguqvm.html

================================================================================
来源：http://hz.guowangkeji.top/gtmnywoamn.html

[J01] 获取当前时间
来源：http://hz.iojbl.cn/gtwpcvrlar.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.snrcjt.cn/gthwtdipcn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hfpthk.cn/gtifrgzems.html

JS:   new Date();  Date.now()
来源：http://hz.gaohongyu789.top/gteslpfwkz.html

TS:   new Date();  Date.now()
来源：http://hz.9152youxi.cn/gtxbfpacdo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hnxiangtu.top/gtqmskkvbd.html

Go:   time.Now()
来源：http://hz.zycfv.cn/gtgqflzkwo.html

Ruby: Time.now
来源：http://hz.shanyushiyangtech.top/gtdeywindn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.mhx1999.top/gtxpgpgnjb.html

[J02] 格式化输出
来源：http://hz.aibaodan.cn/gtpacpecdp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.daxiang520.top/gtdkcwjqew.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.52xcode.cn/gtnorkltcg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jqgfzy.top/gtnuzueluj.html

TS:   d.toISOString()
来源：http://hz.shzxlz.cn/gtahvxerau.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hnxiangtu.top/gtmhsekcjs.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhijiandao.cn/gtbtlrukcf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenzaomai.com/gtpisrphot.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinqigfzy.top/gtlpwwaxwb.html

[J03] 字符串解析为日期
来源：http://hz.jiagoushi.top/gtqyigziba.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.nanxinkj.top/gtaxafchum.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cucudq.cn/gtnppxmqbr.html

JS:   new Date("2024-01-02")
来源：http://hz.shzxlz.cn/gtzjayilag.html

TS:   new Date("2024-01-02")
来源：http://hz.gogol.net.cn/gtgjdpbsvd.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hnqzz.top/gtazzlsjnv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtndvcxycv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhiwuduotai.top/gteaallfby.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cashguo.top/gtvjtnszsu.html

[J04] 时间戳与日期互转
来源：http://hz.sxryk.cn/gtjnelmxlv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hongshengwenyu.top/gtlymwzcwi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jinqigufen.top/gtpdljedyn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinghuilouyu.cn/gtnafwohjt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cashguo.top/gtedqwaxjr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.kuanghao11.cn/gtmhtkohsn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.52xcode.cn/gttmwrougr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinqigufen.top/gtcsngqdvx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.c1oappe.top/gttimvhcvu.html

[J05] 时间加减（加 7 天）
来源：http://hz.snrcjt.cn/gtudtlvxvg.html

Py:   now + timedelta(days=7)
来源：http://hz.ywan-chungtsiang.top/gtraejocbj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgufenzy.top/gtjjjsuxih.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuetiantiany.cn/gtomzpfvwz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jqgufenzy.top/gttvqmjcyw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.kuanghao11.cn/gtdsjzgyhp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.redwolf501.top/gtmylkcmua.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shzxlz.cn/gtyogebvhr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.chenlongwang.top/gtzbsdlgad.html

[J06] 计算两时间之差
来源：http://hz.cashguo.top/gtzcayxbkk.html

Py:   (end - start).total_seconds()
来源：http://hz.c1oappe.top/gthvygbjqz.html

PHP:  $end->diff($start)->days;
来源：http://hz.cqqwz.cn/gtiztdksan.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hnqzz.top/gtgvyvwcbx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hfpthk.cn/gtbwdinpwa.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.dashuyun.cn/gtpbkrquoa.html

Go:   end.Sub(start).Hours()
来源：http://hz.mhx1999.top/gtvbirycan.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jqgufenzy.top/gtngsrktuv.html

C#:   (end - start).TotalSeconds
来源：http://hz.jinqigfzy.top/gtydarkijw.html

[J07] 比较两个日期
来源：http://hz.zhoulong.xyz/gtellmbsce.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jinqigfzy.top/gtsffabafo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.316326.xyz/gtfabpzwjs.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.wangdashe.top/gttgmbxzni.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.havefunace.top/gtehsmzxrc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.sweek.top/gtddfnlbvh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhengqikj.top/gttteavwdx.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinghuilouyu.cn/gtbxfkzyia.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.0kj1m.cn/gttzahvuer.html

[J08] 提取年月日与星期
来源：http://hz.gaohongyu789.top/gtdiqerbiw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hnxiangtu.top/gtwnqfyggx.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.wangshuangyany.cn/gtdtopgxsv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.havefunace.top/gtqgdlvcos.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.meibo888.top/gthjjfyvig.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jlsjyb.cn/gttoyhulnl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yj20258.top/gtluthoebd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yvedp.cn/gtzakswpjb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.iojbl.cn/gtirpyagny.html

[J09] 时区处理
来源：http://hz.gogol.net.cn/gthevewvfz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shangyingyoupin.top/gtlgjddzsh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.quarkkingdee.top/gtwjneordk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.pengpengdd.cyou/gtoliiedbz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgufenzy.top/gtaqbcwsrd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yangfankeji.com/gtewxweoao.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hysaishi.cn/gtofkdylsj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.aibaodan.cn/gtfzryijkn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shanyushiyangtech.top/gtuynxiysv.html

[J10] 取今天 / 本月第一天
来源：http://hz.xingfuxueyuan.xyz/gtdudpbtcy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cheryme.top/gtiieqmdjr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hongshengwenyu.top/gtlownvvat.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yuanzhike.top/gtrirznpol.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.havefunace.top/gtpttahblz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sysykeji.top/gtjeovdduk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.quarkkingdee.top/gtzmrrdqcl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cashguo.top/gtunjfhinf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xylfe.cn/gtlkximqrw.html

================================================================================
来源：http://hz.xziqi.cn/gtudzmilsh.html

K. JSON 与序列化
来源：http://hz.yj20258.top/gtifuotgzj.html

================================================================================
来源：http://hz.zhijiandao.cn/gtedqgbgua.html

[K01] 对象转 JSON 字符串
来源：http://hz.hammf.cn/gtxarkqfts.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhixingplan.top/gtfqdrlokc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.andypj.xyz/gtnftzambj.html

JS:   JSON.stringify(obj)
来源：http://hz.redwolf501.top/gtwxlfjocz.html

TS:   JSON.stringify(obj)
来源：http://hz.hysaishi.cn/gtwfmrozcm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shzxlz.cn/gtmxpiiqkb.html

Go:   json.Marshal(obj)
来源：http://hz.yonumen.top/gtkmnvvcsq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.wangdashe.top/gthgiazjgs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.wangdashe.top/gtjgfpspba.html

[K02] JSON 字符串转对象
来源：http://hz.cashguo.top/gtmroxaocb.html

Py:   json.loads(s)
来源：http://hz.jinqigufen.top/gtfglpgbip.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cucudq.cn/gtchnhkxyc.html

JS:   JSON.parse(s)
来源：http://hz.ybcxt.top/gtrstnmjyk.html

TS:   JSON.parse(s)
来源：http://hz.fzhhl.top/gtmyghruuj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gzhubu.top/gthtrtjgop.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xylfe.cn/gtltlxvfjz.html

Ruby: JSON.parse(s)
来源：http://hz.hysaishi.cn/gtlmydmqdg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.daria6918.cn/gtneompxqd.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.mhx1999.top/gtdcxslbhv.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xuanzx.com/gtbqximjpg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.sxryk.cn/gtiacthucv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.0kj1m.cn/gtnrueerzc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.tanke756.top/gtnwhqmrzb.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.aizwys.cn/gtsnrhbzqq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.c1oappe.top/gtaxqrnaho.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yonumen.top/gtwcaaasjq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xylfe.cn/gtdgendlby.html

[K04] 读取 JSON 文件
来源：http://hz.9152youxi.cn/gtpwpulpqw.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.nanxuanxn.top/gtyvrclvlm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sweek.top/gtzegfbncg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ehwqpu.com/gtafnxsfpa.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ppjwa.cn/gtcoofgkre.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ydjk.org.cn/gtqgigjnhi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hammf.cn/gtpwtljjhj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhengqikj.top/gtkuzjvtvn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yongpay.top/gtdpbstsqr.html

[K05] 深拷贝对象
来源：http://hz.zdqjudy.top/gtbqtvthws.html

Py:   copy.deepcopy(obj)
来源：http://hz.hysaishi.cn/gtkcfjjokz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jqgufenzy.top/gtnbbwdldt.html

JS:   structuredClone(obj)
来源：http://hz.jyoumei.cn/gtvgxfylhg.html

TS:   structuredClone(obj)
来源：http://hz.jiagoushi.top/gttzhlnnzy.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.fengsongda.top/gtnayjewuw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yvedp.cn/gtnnbptdqy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jqgufenzy.top/gtlumlptha.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jinqigfzy.top/gtyjefhnjd.html

[K06] 解析 URL 查询串
来源：http://hz.shanyushiyangkeji.top/gtnolyagsw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.aizwys.cn/gtuigviqhz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.dashuyun.cn/gtewaukylj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ywan-chungtsiang.top/gtrbmwhigc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jqgufenzy.top/gtnkxieqgl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj20258.top/gtpgjqvdrh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.daxiang520.top/gtutuscvak.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.fengsongda.top/gtaewahqez.html


<!-- 参考信息 -->