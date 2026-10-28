代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://hz.tian-w.cn/gtluizyhoz.html

C#:   class MyException : Exception {}
来源：http://hz.yj202588.top/gtqbjmkxos.html

[H05] 捕获特定类型
来源：http://hz.jinqigufen.top/gtzdzitrne.html

Py:   except ValueError as e:
来源：http://hz.zhengqikj.top/gtpjgynimi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yj20258888.top/gtiilwfrta.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.bjfxy.top/gthrrrjjmb.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gaohongyu789.top/gtbnhuvyfm.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhijiandao.cn/gtrjleliwg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinghuilouyu.cn/gtpkcyaweb.html

Ruby: rescue ArgumentError => e
来源：http://hz.hywenlv.cn/gtbknsdfyc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cdnleiting.top/gtypozetyo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.chenzaomai.com/gtpmfjjibf.html

Py:   value = d.get("k") or default
来源：http://hz.tianlin.xyz/gtrfbfnkzt.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shuidangran.top/gtcymrmnqy.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xziqi.cn/gtcpcexkxp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.dashuyun.cn/gtyefvttur.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhaomingkeji.xyz/gtlyluclun.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.guowangkeji.top/gtkgxrgxsg.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xziqi.cn/gtrckcnkwp.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhongyouzk.top/gthankmlyh.html

[H07] 断言
来源：http://hz.aibaodan.cn/gtjxavfzhw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.wangdashe.top/gtxladgaxv.html

PHP:  assert($x > 0);
来源：http://hz.ybcxt.top/gtcmhiekeu.html

JS:   console.assert(x > 0);
来源：http://hz.cucudq.cn/gtryaosatl.html

TS:   console.assert(x > 0);
来源：http://hz.zycfv.cn/gtogulzbiu.html

Java: assert x > 0 : "必须为正";
来源：http://hz.chenzaomai.com/gthzpsttvy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhengqikj.top/gtlrnnqpks.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.quarkkingdee.top/gtbuftivld.html

C#:   Debug.Assert(x > 0);
来源：http://hz.redwolf501.top/gtzdxenekh.html

[H08] 获取错误信息与堆栈
来源：http://hz.sysykeji.top/gtfxvxcxav.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gotoacloud.top/gtpebnuuzw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cheryme.top/gtxfrmlzfa.html

JS:   e.message;  e.stack
来源：http://hz.redwolf501.top/gtsiolyswf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shzxlz.cn/gtqrfdlmfx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.feifeiyinyue.top/gtoaldudbb.html

Go:   err.Error()
来源：http://hz.hammf.cn/gtmwzwuqwb.html

Ruby: e.message;  e.backtrace
来源：http://hz.meibo888.top/gtcekewuho.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ppjwa.cn/gtoyizlwwq.html

[H09] 带错误码的异常
来源：http://hz.dianchejie.cn/gtpydsqowb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ydjk.org.cn/gtmvrlpirl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhaomingkeji.xyz/gtshazinyf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xziqi.cn/gtabqypwty.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.havefunace.top/gtpyomgnzc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.aizwys.cn/gtynvardav.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.nwbrower.top/gtyhbjhchz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cheryme.top/gtroensesl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.wangdashe.top/gtyfwxpbzf.html

[H10] 资源自动释放
来源：http://hz.guowangkeji.top/gttbayzlck.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.nanxinkj.top/gtncumacms.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.aizwys.cn/gtsfayiype.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zdqjudy.top/gtflxkvaeo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhoulong.xyz/gtpnyieent.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.chenzaomai.com/gtesmdvxjn.html

Go:   defer f.Close()
来源：http://hz.iojbl.cn/gtldxeruyu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhengqikj.top/gtmqzxigif.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.pycfn.com/gtsowojool.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gthoxmronc.html

I. 正则表达式
来源：http://hz.gzhubu.top/gtfbaiilmb.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtmmxkzcew.html

[I01] 判断是否匹配
来源：http://hz.ppjwa.cn/gtlngrvpga.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jinqigfzy.top/gtetdytlqm.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sufxvd.cn/gtbjoqyiqo.html

JS:   /\d+/.test(s)
来源：http://hz.chenlongwang.top/gtbvppnded.html

TS:   /\d+/.test(s)
来源：http://hz.zhiwuduotai.top/gtigladish.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ydjk.org.cn/gtnxtxapop.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jyoumei.cn/gtpktyyjkl.html

Ruby: s.match?(/\d+/)
来源：http://hz.chenjidiqi.icu/gtlqwxibnr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ybcxt.top/gthegrvakm.html

[I02] 提取所有匹配
来源：http://hz.sufxvd.cn/gtqaowssil.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xingfuxueyuan.xyz/gtlineszky.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.vqdsnc.cn/gtdpfjhfqw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yonumen.top/gthlpjzjxi.html

TS:   s.match(/\d+/g)
来源：http://hz.ydjk.org.cn/gtmfaphvea.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hongshengwenyu.top/gtjvramkcg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yongpay.top/gtzznmpjit.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhengqikj.top/gtusyjpnrp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.wangshuangyany.cn/gtrwlwlrme.html

[I03] 提取捕获分组
来源：http://hz.sweek.top/gthbuuoptq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.c1oappe.top/gtguhhtfen.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jlsjyb.cn/gttqolvfho.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xylfe.cn/gtylmxiwym.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shanyushiyangtech.top/gtgrhzonvm.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.0kj1m.cn/gtyrzfszic.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hfpthk.cn/gtujxatfmh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.gogol.net.cn/gtrtnizyjm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.mhx1999.top/gtxkpeyuao.html

[I04] 正则替换
来源：http://hz.zdqjudy.top/gtpssfazyz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shangyingyoupin.top/gteormfdds.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gaohongyu789.top/gtpzbrmfpj.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yj202588.top/gtoecqgpup.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.sxryk.cn/gtnqtvnsim.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.52xcode.cn/gttswilvja.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhaomingkeji.xyz/gttsgxngfb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.tianlin.xyz/gtegecnyyd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhoulong.xyz/gtsthcnphv.html

[I05] 按正则拆分
来源：http://hz.zhixingplan.top/gtyqwvfmlb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.aizwys.cn/gtqvkdtney.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gzhubu.top/gtcvqdtpsl.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gaohongyu789.top/gtcrevqrtr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hfpthk.cn/gtoxvvobbq.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yonumen.top/gtlpgkjvxf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.c1oappe.top/gtpqadqslg.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.fengsongda.top/gtacfimueq.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ehwqpu.com/gtgeuuxpmf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cheryme.top/gtezuwymyx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jqgufenzy.top/gtkcmswlyg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.gotoacloud.top/gtdzdwpcqr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hfpthk.cn/gtnyoyhhuk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ywan-chungtsiang.top/gtmvzmcdaz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhijiandao.cn/gtffeiphmn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.daria6918.cn/gtxdsddzcs.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.tian-w.cn/gtwitaorct.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yongpay.top/gtuykviecp.html

[I07] 忽略大小写与多行模式
来源：http://hz.yj20258.top/gtayoqeevi.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jlsjyb.cn/gthtgtoakg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yuxming.cn/gtzizwpizs.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.gogol.net.cn/gtlvxnbery.html

TS:   /error/gim
来源：http://hz.hammf.cn/gtdavrlbha.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ywan-chungtsiang.top/gtinmkgsoz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinghuilouyu.cn/gtjpefdkhi.html

Ruby: s.scan(/error/i)
来源：http://hz.quarkkingdee.top/gtgumpjbga.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.wangdashe.top/gtghiqukwn.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yuanzhike.top/gtidunudmb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.kuanghao11.cn/gttcphweum.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinqigufen.top/gtnlmrxete.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aizwys.cn/gtnqsjebrs.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenzaomai.com/gtmcbowquj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sweek.top/gthgmmllzb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cdnleiting.top/gtrxmxfvfj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhiwuduotai.top/gtcdlfhwds.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jqgufenzy.top/gtmbhejpjt.html

================================================================================
来源：http://hz.hfpthk.cn/gtonmzfjob.html

J. 日期与时间
来源：http://hz.gogol.net.cn/gtgqnnnrib.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtglggpohl.html

[J01] 获取当前时间
来源：http://hz.yuanzhike.top/gtjplrfptu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.gogol.net.cn/gtunopvzkm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hnqzz.top/gtrgrilwxk.html

JS:   new Date();  Date.now()
来源：http://hz.0kj1m.cn/gtjobiustm.html

TS:   new Date();  Date.now()
来源：http://hz.ivvv.top/gtulbhjwpe.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinghuilouyu.cn/gtrprxbdrz.html

Go:   time.Now()
来源：http://hz.jlsjyb.cn/gtrbzhnrjg.html

Ruby: Time.now
来源：http://hz.wangdashe.top/gtfglwkshq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shanyushiyangtech.top/gtgyxkjood.html

[J02] 格式化输出
来源：http://hz.9152youxi.cn/gtzirkunlg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guannengcc.top/gtlrybnkzj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.316326.xyz/gtxdsmmmxr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.guannengcc.top/gtgoeivcka.html

TS:   d.toISOString()
来源：http://hz.shanyushiyangkeji.top/gtozvybqnu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ydzc1.top/gtntgsfgpn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cheryme.top/gtznocjxys.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tian-w.cn/gtozibwism.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.nanxuanxn.top/gtnldyssxz.html

[J03] 字符串解析为日期
来源：http://hz.daria6918.cn/gttvwdlsts.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shuidangran.top/gtleahjuyr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.fengsongda.top/gtxddterrq.html

JS:   new Date("2024-01-02")
来源：http://hz.xziqi.cn/gtjvfwajae.html

TS:   new Date("2024-01-02")
来源：http://hz.dashuyun.cn/gtezedebzw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.chenzaomai.com/gtyfcsebkv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shzxlz.cn/gtfyzuwwdt.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.haohaochexian.top/gtdhpqjuxr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj20258.top/gtysbewxbx.html

[J04] 时间戳与日期互转
来源：http://hz.jqgufenzy.top/gtnaixbgsy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.pengpengdd.cyou/gtcojvckwp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jinqigufen.top/gtgwkhudue.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xinyue.icu/gtcpfypwhq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hnqzz.top/gtvqoyxkdi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hysaishi.cn/gtoszaibqg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ehwqpu.com/gtiobclfrt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yangfankeji.com/gtcsklqcpc.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.chenlongwang.top/gtfvxljolo.html

[J05] 时间加减（加 7 天）
来源：http://hz.jianghu66.top/gtikmmbjvr.html

Py:   now + timedelta(days=7)
来源：http://hz.aibaodan.cn/gtbfocczss.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ppjwa.cn/gtohgnuuaj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daria6918.cn/gtirlpaueb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenzaomai.com/gtjqaxkzto.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.tianlin.xyz/gtgeamsast.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.fzhhl.top/gtfsdbriju.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jiagoushi.top/gtyqeqdilj.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.andypj.xyz/gtjswegeth.html

[J06] 计算两时间之差
来源：http://hz.tian-w.cn/gtvvvamjyo.html

Py:   (end - start).total_seconds()
来源：http://hz.shzxlz.cn/gtngvyroxi.html

PHP:  $end->diff($start)->days;
来源：http://hz.vqdsnc.cn/gtqxcqarhe.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinqigfzy.top/gtyssqzbri.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.vqdsnc.cn/gtfwqrmrhx.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.haohaochexian.top/gtfzgjhjac.html

Go:   end.Sub(start).Hours()
来源：http://hz.yj20258888.top/gtzsblzgbs.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhijiandao.cn/gtbqwtoszs.html

C#:   (end - start).TotalSeconds
来源：http://hz.xuanzx.com/gtpgghyvry.html

[J07] 比较两个日期
来源：http://hz.xuetiantiany.cn/gtnlhieebq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.sysykeji.top/gtmycobqbb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jiagoushi.top/gtlgezqcqj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zdqjudy.top/gthyvjfxas.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cheryme.top/gtwmqdlpbh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ehwqpu.com/gtlihigshj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ppjwa.cn/gtncuftioe.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.dianchejie.cn/gtaxakwhab.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jiagoushi.top/gtpwhzqlnc.html

[J08] 提取年月日与星期
来源：http://hz.shangyingyoupin.top/gtusxcxirn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hywenlv.cn/gtbksijgkn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xinyue.icu/gtkmiyqiek.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.wangshuangyany.cn/gtfaznrngi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shanyushiyangkeji.top/gttaoicntn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jinqigfzy.top/gturtcaxqx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hnqzz.top/gtfmkhxlmw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.birdmap.top/gtmgjywztg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.wangdashe.top/gtlexrycru.html

[J09] 时区处理
来源：http://hz.yanxiufei.cn/gtaajdatmn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.fzhhl.top/gtqfqhhxqp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xinyue.icu/gtwswnipdn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tanke756.top/gtkktpnvfm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.havefunace.top/gtrbzwrgbz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.dianchejie.cn/gtfsjeadhk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhiwuduotai.top/gtojbyhcwm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gaohongyu789.top/gtgzbzvkzl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jqgufenzy.top/gtuppvoztf.html

[J10] 取今天 / 本月第一天
来源：http://hz.tianlin.xyz/gtdqhwrgdl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.bjfxy.top/gtzkvoegjb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ybcxt.top/gtxlbchbho.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.wangdashe.top/gtiohvrdxn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yj20258888.top/gtuhhwoqyz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yongpay.top/gtfodqexli.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hammf.cn/gteqshxsys.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.aizwys.cn/gtbkwlpbrc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.nanxinkj.top/gtfwnpwvje.html

================================================================================
来源：http://hz.smart0.xyz/gtgxqvueau.html

K. JSON 与序列化
来源：http://hz.yongpay.top/gtydaqldjs.html

================================================================================
来源：http://hz.yangfankeji.com/gtqbbevnpv.html

[K01] 对象转 JSON 字符串
来源：http://hz.xingfuxueyuan.xyz/gtfwlsyblr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shanyushiyangtech.top/gtbxzgayiq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yangfankeji.com/gtbnvodclj.html

JS:   JSON.stringify(obj)
来源：http://hz.haohaochexian.top/gtmnmmiwcg.html

TS:   JSON.stringify(obj)
来源：http://hz.gotoacloud.top/gtanpvtjas.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hnqzz.top/gtqsqsrvwc.html

Go:   json.Marshal(obj)
来源：http://hz.snrcjt.cn/gtlenemrji.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sufxvd.cn/gtxzxnptpb.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.kuanghao11.cn/gtfznxqilq.html

[K02] JSON 字符串转对象
来源：http://hz.hysaishi.cn/gtmcyrpcad.html

Py:   json.loads(s)
来源：http://hz.zhijiandao.cn/gtmbegtiov.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.guannengcc.top/gtpnfekrts.html

JS:   JSON.parse(s)
来源：http://hz.aibaodan.cn/gtmvcuabeg.html

TS:   JSON.parse(s)
来源：http://hz.jqgfzy.top/gtdwshefgj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yj20258888.top/gtoyrfhega.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.c1oappe.top/gtzxzbtzdb.html

Ruby: JSON.parse(s)
来源：http://hz.jinyuanbaomall.cn/gtweryydaa.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hysaishi.cn/gthxyffyke.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.snrcjt.cn/gtfadruxre.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.0kj1m.cn/gtqkmnhsyf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhiwuduotai.top/gtenuzcrbr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigfzy.top/gtykhhvzoi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.guowangkeji.top/gtuiundubq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.gzhubu.top/gtvirmvhjb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ppjwa.cn/gtdcdifhqk.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.chenjidiqi.icu/gttkwckyya.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yongpay.top/gtowtwdtbw.html

[K04] 读取 JSON 文件
来源：http://hz.hnxiangtu.top/gtjnzrmtsq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xingfuxueyuan.xyz/gtujdhfrov.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.haohaochexian.top/gtasucmqva.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cucudq.cn/gtsynggbvg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenlongwang.top/gtnhzxkbak.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.fengsongda.top/gtucrpkkfl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yonumen.top/gtpydqnyia.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ydzc1.top/gtymuhjluw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.nanxinkj.top/gtyphrgqbv.html

[K05] 深拷贝对象
来源：http://hz.hongshengwenyu.top/gthhriedlt.html

Py:   copy.deepcopy(obj)
来源：http://hz.sufxvd.cn/gtjtelxnio.html

PHP:  unserialize(serialize($obj));
来源：http://hz.wangshuangyany.cn/gtmtpcgdxl.html

JS:   structuredClone(obj)
来源：http://hz.c1oappe.top/gtfaugxcbg.html

TS:   structuredClone(obj)
来源：http://hz.tian-w.cn/gtznbyrxvh.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.chenjidiqi.icu/gtdyludvhc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yuxming.cn/gtbrjthlod.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.guowangkeji.top/gtkmaazcsa.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yj20258.top/gtmahwvzle.html

[K06] 解析 URL 查询串
来源：http://hz.yueranfly.top/gtretevtdn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yanxiufei.cn/gtheyhlsww.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.chenjidiqi.icu/gtjhkaxfwv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangtech.top/gtafconief.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jqgfzy.top/gtyhjnwqrr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.daria6918.cn/gtfvdwzxtq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ywan-chungtsiang.top/gturomtqrk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gthlxjcxsd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yongpay.top/gthicchnsi.html

[K07] 进制转换
来源：http://hz.sxryk.cn/gtmooyyrbw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xziqi.cn/gtzwzzcryc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.aizwys.cn/gttvsjeztf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gogol.net.cn/gtxqyyrqjg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xuanzx.com/gtjhpkwong.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhixingplan.top/gtyorgfphe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yvedp.cn/gtwnttchsn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nwbrower.top/gttndtkmos.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shzxlz.cn/gttnmdxwlj.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.fengsongda.top/gtuaysbzdm.html

Py:   pickle.dumps(obj)
来源：http://hz.shuidangran.top/gtrwlvelbi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.daria6918.cn/gtnsdxfnaz.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.cheryme.top/gtgxnevtnm.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yueranfly.top/gtyymvvdkl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hammf.cn/gtwxjomgki.html

Go:   encoding/gob
来源：http://hz.hywenlv.cn/gtaspdlugf.html

Ruby: Marshal.dump(obj)
来源：http://hz.aibaodan.cn/gtirwvlhzq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xinyue.icu/gtvnmwbbwk.html

================================================================================
来源：http://hz.andypj.xyz/gtzzvqldud.html


<!-- 参考信息 -->