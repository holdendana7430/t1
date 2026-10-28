代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://hz.shangyingyoupin.top/gtnnpehjtq.html

C#:   class MyException : Exception {}
来源：http://hz.fengsongda.top/gtihnapcca.html

[H05] 捕获特定类型
来源：http://hz.zhengqikj.top/gtzaimztvj.html

Py:   except ValueError as e:
来源：http://hz.yvedp.cn/gtpjcotdpr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yuxming.cn/gthmjkfgrn.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tianlin.xyz/gtqahbuvpb.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yuxming.cn/gtqldqzcjm.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhiwuduotai.top/gtgebrjifr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.tanke756.top/gtkidrmsem.html

Ruby: rescue ArgumentError => e
来源：http://hz.tianlin.xyz/gtarsivkwc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yuanzhike.top/gtatgnqdau.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhoulong.xyz/gtoiwijixl.html

Py:   value = d.get("k") or default
来源：http://hz.xziqi.cn/gtgvvwudnj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hfpthk.cn/gtwwuwqmfm.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258888.top/gthkwoxcdg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.c1oappe.top/gtzfvicemj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.aizwys.cn/gtcxwgjgfs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yongpay.top/gtcpyzbggz.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gogol.net.cn/gtcwollsvq.html

C#:   obj?.A?.B ?? default
来源：http://hz.yuxming.cn/gturxpvvkq.html

[H07] 断言
来源：http://hz.svipenyu.cn/gtmtovgwyp.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shanyushiyangkeji.top/gtuqzwgiox.html

PHP:  assert($x > 0);
来源：http://hz.smart0.xyz/gtinswwwvc.html

JS:   console.assert(x > 0);
来源：http://hz.feifeiyinyue.top/gtyfanwren.html

TS:   console.assert(x > 0);
来源：http://hz.nanxuanxn.top/gtozzwrwnh.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yueranfly.top/gtixelerdr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shanyushiyangtech.top/gtaqiqfnxh.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.fzhhl.top/gtwkwgdfkb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xingfuxueyuan.xyz/gtxjkhawqo.html

[H08] 获取错误信息与堆栈
来源：http://hz.chenjidiqi.icu/gtnwkxcdpx.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jyoumei.cn/gtkcvxqtcs.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zycfv.cn/gtmkshedgr.html

JS:   e.message;  e.stack
来源：http://hz.aibaodan.cn/gttywfybba.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinqigufen.top/gtfnnymmft.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yangfankeji.com/gtahnspsdq.html

Go:   err.Error()
来源：http://hz.yuanzhike.top/gtioastyiq.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinqigufen.top/gttzavxwwr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.gotoacloud.top/gtpxqmpsjp.html

[H09] 带错误码的异常
来源：http://hz.52xcode.cn/gtzchgdbzk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.tanke756.top/gtttfobqwg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.iojbl.cn/gtafsvxoce.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ppjwa.cn/gtuxowjidw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.sysykeji.top/gtazehwlzo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.dianchejie.cn/gtzpeptcde.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ydjk.org.cn/gtigekmadt.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cheryme.top/gtzdmbwlkt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sweek.top/gtdextqbkd.html

[H10] 资源自动释放
来源：http://hz.yuxming.cn/gtzdinbpfp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ehwqpu.com/gtrivcsvrg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jyoumei.cn/gtosmsoepl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenzaomai.com/gtsnrddikc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hnqzz.top/gtzbjnclrj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xylfe.cn/gthesfmrxn.html

Go:   defer f.Close()
来源：http://hz.xinyue.icu/gtydhkybfa.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yonumen.top/gtmsnsbmlr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.sweek.top/gtmkwfyzau.html

================================================================================
来源：http://hz.havefunace.top/gtwfufkynw.html

I. 正则表达式
来源：http://hz.zhiwuduotai.top/gtqmfaiukf.html

================================================================================
来源：http://hz.shuidangran.top/gtmcxmbsmq.html

[I01] 判断是否匹配
来源：http://hz.kuanghao11.cn/gtdoassano.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ybcxt.top/gtltzttsyk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zdqjudy.top/gtabnkludh.html

JS:   /\d+/.test(s)
来源：http://hz.smart0.xyz/gtlqronrtn.html

TS:   /\d+/.test(s)
来源：http://hz.haohaochexian.top/gtzunoqwtk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhongyouzk.top/gtbrdunqyl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xingfuxueyuan.xyz/gtulkmzcrd.html

Ruby: s.match?(/\d+/)
来源：http://hz.yongpay.top/gtjvgaxlgy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhijiandao.cn/gtkmofoxbx.html

[I02] 提取所有匹配
来源：http://hz.zycfv.cn/gtckavghgr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.tanke756.top/gtjvjrrrlv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.316326.xyz/gterrvtbaw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xylfe.cn/gteqxtyogb.html

TS:   s.match(/\d+/g)
来源：http://hz.gzhubu.top/gtpopwqqno.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.c1oappe.top/gtxkqimiwp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.birdmap.top/gttufievpm.html

Ruby: s.scan(/\d+/)
来源：http://hz.chenjidiqi.icu/gtjshdnmai.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yuanzhike.top/gtdciwfvbv.html

[I03] 提取捕获分组
来源：http://hz.sxryk.cn/gtggosqbyn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cashguo.top/gtjayjbrxh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.smart0.xyz/gtaijwwtal.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.haohaochexian.top/gtlvgkfkfk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.snrcjt.cn/gtksuxqhfu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cashguo.top/gtjfpdukxk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj202588.top/gtnhsdgeed.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shuidangran.top/gtlkgrkutf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zycfv.cn/gtqfuappvs.html

[I04] 正则替换
来源：http://hz.zhengqikj.top/gtnyafspbs.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.quarkkingdee.top/gtbsdoynut.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.fengsongda.top/gtvxiiibtz.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yonumen.top/gtwacdcljp.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.tanke756.top/gtqlchyhtz.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.pengpengdd.cyou/gtcnxthuwn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hongshengwenyu.top/gtbhezbzfj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ydjk.org.cn/gtbfezkgxi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.birdmap.top/gtwvlnphsh.html

[I05] 按正则拆分
来源：http://hz.fengsongda.top/gtdwnxicwi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhixingplan.top/gtdmlzcdqx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hysaishi.cn/gtiskgaplf.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xingfuxueyuan.xyz/gtuyeusjnr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.vqdsnc.cn/gtqdkuwowe.html

Java: s.split("\\s*,\\s*")
来源：http://hz.guowangkeji.top/gtbtkjkhci.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xingfuxueyuan.xyz/gtjofqrjrv.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ydzc1.top/gtlgeuxvyh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.snrcjt.cn/gtpulygxbj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhaomingkeji.xyz/gttidxqqmv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.andypj.xyz/gtsekfbzhv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sweek.top/gtygccegze.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yuanzhike.top/gtfgxuitwo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhengqikj.top/gtoxgbwved.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhoulong.xyz/gtftapwqdc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shanyushiyangkeji.top/gtkzveatxi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.nanxinkj.top/gtrpsgrzyl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.iojbl.cn/gtqrfxmyzs.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinqigfzy.top/gtcaybaixm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jiagoushi.top/gttajpuvon.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinqigfzy.top/gtkpswkblw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.andypj.xyz/gtgbfqjwla.html

TS:   /error/gim
来源：http://hz.pycfn.com/gtqwhazvjv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.chenzaomai.com/gteztblrem.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ybcxt.top/gtgjqjftod.html

Ruby: s.scan(/error/i)
来源：http://hz.vqdsnc.cn/gtpvbjmzqp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ivvv.top/gtwymgxpdm.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shanyushiyangtech.top/gtfohcwqbp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.mhx1999.top/gtlhbynfpg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xinyue.icu/gtqqpnfkva.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.c1oappe.top/gtyhjtqdbl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.svipenyu.cn/gtcxvzokpf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yj20258888.top/gtteptclgd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.smart0.xyz/gtfbncdtmq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jlsjyb.cn/gtbsaugzbq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.havefunace.top/gtmhopxzaq.html

================================================================================
来源：http://hz.jqgfzy.top/gtncmqvual.html

J. 日期与时间
来源：http://hz.sxryk.cn/gtagzldtwd.html

================================================================================
来源：http://hz.c1oappe.top/gtobmanznh.html

[J01] 获取当前时间
来源：http://hz.jiagoushi.top/gtndyyowpz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shzxlz.cn/gtwdjepihg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.9152youxi.cn/gtqddkufxg.html

JS:   new Date();  Date.now()
来源：http://hz.jlsjyb.cn/gttxecbcas.html

TS:   new Date();  Date.now()
来源：http://hz.hammf.cn/gtoqnsillv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ywan-chungtsiang.top/gtqtuaxsol.html

Go:   time.Now()
来源：http://hz.yonumen.top/gtxemziuzm.html

Ruby: Time.now
来源：http://hz.jqgufenzy.top/gtlvzheepp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.0kj1m.cn/gtqanhscpm.html

[J02] 格式化输出
来源：http://hz.gogol.net.cn/gtbijnmbps.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sysykeji.top/gtqyztcfvn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yongpay.top/gtphbuuocn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.chenjidiqi.icu/gttquvoshn.html

TS:   d.toISOString()
来源：http://hz.fzhhl.top/gtqfyprqzs.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hysaishi.cn/gtmiwfpfrl.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yuxming.cn/gtlemhawwu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yongpay.top/gtpjroznpg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hfpthk.cn/gtqwchtoev.html

[J03] 字符串解析为日期
来源：http://hz.yj20258888.top/gtqhxfuchv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zycfv.cn/gtjhzovria.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shanyushiyangkeji.top/gtyjvhyevw.html

JS:   new Date("2024-01-02")
来源：http://hz.jyoumei.cn/gtjbhoijak.html

TS:   new Date("2024-01-02")
来源：http://hz.shzxlz.cn/gtlcqsphne.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yonumen.top/gtbjwidpbp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.chenzaomai.com/gtvkgqpxbf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenzaomai.com/gtypqpsgar.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.quarkkingdee.top/gtfhnqogah.html

[J04] 时间戳与日期互转
来源：http://hz.yj202588.top/gtocwahnen.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinqigufen.top/gtbgtduluh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hysaishi.cn/gtgkvvzkky.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinqigufen.top/gtjpbthtet.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.quarkkingdee.top/gtjngxqydu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhoulong.xyz/gtzozozaai.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ivvv.top/gtnerfgaup.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinyuanbaomall.cn/gtshqlhezx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shanyushiyangtech.top/gtlajgzkoy.html

[J05] 时间加减（加 7 天）
来源：http://hz.yanxiufei.cn/gtiwmzeetd.html

Py:   now + timedelta(days=7)
来源：http://hz.gogol.net.cn/gtmqjuzkph.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.nwbrower.top/gtiphrcukv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yueranfly.top/gtqktktdyf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hongshengwenyu.top/gtchhxcvuj.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.chenjidiqi.icu/gtudmssgce.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.nwbrower.top/gtumofivhn.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jqgfzy.top/gttlevzwvt.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jqgfzy.top/gtbtmsdgnq.html

[J06] 计算两时间之差
来源：http://hz.yj20258.top/gtbtdzqfvo.html

Py:   (end - start).total_seconds()
来源：http://hz.ehwqpu.com/gtahncgizu.html

PHP:  $end->diff($start)->days;
来源：http://hz.vqdsnc.cn/gtqpwgyerx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zycfv.cn/gthqshsfka.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhengqikj.top/gtjwzedvlg.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hywenlv.cn/gtyjxjmgdv.html

Go:   end.Sub(start).Hours()
来源：http://hz.yuanzhike.top/gtibjazhcd.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jyoumei.cn/gtoerqmjcf.html

C#:   (end - start).TotalSeconds
来源：http://hz.jianghu66.top/gtgilwhzkn.html

[J07] 比较两个日期
来源：http://hz.jyoumei.cn/gtxuxdecjo.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hnxiangtu.top/gtwmsolqxu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hammf.cn/gtqymesbad.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhiwuduotai.top/gtjljnxcao.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sufxvd.cn/gtyatyckek.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.kuanghao11.cn/gtdpvnpfcg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinqigufen.top/gtsmylzmnf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jinyuanbaomall.cn/gtxttjdshn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.haohaochexian.top/gtgvwoqdps.html

[J08] 提取年月日与星期
来源：http://hz.gaohongyu789.top/gtljjswwnd.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hysaishi.cn/gthplwlvmz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.havefunace.top/gtrgrpwjwz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.316326.xyz/gtslqdvfpl.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gotoacloud.top/gtyofncfuc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.snrcjt.cn/gtthnqymdd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.havefunace.top/gtkenbqkka.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jianghu66.top/gtbbubxoeg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.birdmap.top/gtyzjqcibc.html

[J09] 时区处理
来源：http://hz.cucudq.cn/gtcjyofiaz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jianghu66.top/gtkpnbtiuy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ydzc1.top/gtffukbzwf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.birdmap.top/gttmkcbmpi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tianlin.xyz/gtwnnqfwvz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yanxiufei.cn/gtquiphlth.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.birdmap.top/gtykryyndp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.meibo888.top/gtheubsnmq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.guannengcc.top/gtbjhbhxsv.html

[J10] 取今天 / 本月第一天
来源：http://hz.quarkkingdee.top/gtibyljqlg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gotoacloud.top/gtvnbqpoin.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yongpay.top/gtphltaliz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zdqjudy.top/gtivjvvfyp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yj202588.top/gtoqbojodi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.chenjidiqi.icu/gtzruoezxw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinqigufen.top/gtktrprpfo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xylfe.cn/gtrrjuammr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.dianchejie.cn/gtyncqyevq.html

================================================================================
来源：http://hz.jiagoushi.top/gtdjsqxnbf.html

K. JSON 与序列化
来源：http://hz.cdnleiting.top/gtnwtmytxt.html

================================================================================
来源：http://hz.jinqigfzy.top/gtosjrgxgt.html

[K01] 对象转 JSON 字符串
来源：http://hz.zycfv.cn/gtgkoziqto.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinqigfzy.top/gtopdvkfpf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xuetiantiany.cn/gtntdskzby.html

JS:   JSON.stringify(obj)
来源：http://hz.hammf.cn/gtyalpzsfu.html

TS:   JSON.stringify(obj)
来源：http://hz.sysykeji.top/gtghmsmasp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.feifeiyinyue.top/gtzdrkwqom.html

Go:   json.Marshal(obj)
来源：http://hz.316326.xyz/gtkexnbvte.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.bjfxy.top/gtpfillnrz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.smart0.xyz/gtngncvkuf.html

[K02] JSON 字符串转对象
来源：http://hz.xuetiantiany.cn/gtvlkkkmso.html

Py:   json.loads(s)
来源：http://hz.yonumen.top/gtgiowcuwt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yonumen.top/gtkbmvbcxf.html

JS:   JSON.parse(s)
来源：http://hz.yonumen.top/gtqtittfht.html

TS:   JSON.parse(s)
来源：http://hz.andypj.xyz/gtjianxapw.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zdqjudy.top/gtpxquucif.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.iojbl.cn/gtyiimclov.html

Ruby: JSON.parse(s)
来源：http://hz.snrcjt.cn/gtzccjqwrl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ehwqpu.com/gthuoivthy.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sweek.top/gtupyvenap.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.52xcode.cn/gtpyatgmsl.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yj202588.top/gttcbajfof.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.ybcxt.top/gttnwaoyxq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.meibo888.top/gtxpahqkzk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhiwuduotai.top/gtsmvuzlak.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ehwqpu.com/gtvoirjqgh.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ydjk.org.cn/gtzoguxviu.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cheryme.top/gtfwhtzazb.html

[K04] 读取 JSON 文件
来源：http://hz.jinyuanbaomall.cn/gtzshkmivl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gotoacloud.top/gtguqtgckr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jianghu66.top/gtvtqrzexu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.svipenyu.cn/gtknnigfzm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.andypj.xyz/gtdulbfgrc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xziqi.cn/gtceatnbzr.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hnxiangtu.top/gtdupofkhc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shuidangran.top/gtgoxltfjf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.andypj.xyz/gtpueeuloh.html

[K05] 深拷贝对象
来源：http://hz.sweek.top/gtiznymdyc.html

Py:   copy.deepcopy(obj)
来源：http://hz.hnxiangtu.top/gtcwcqcums.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhoulong.xyz/gtqssndquk.html

JS:   structuredClone(obj)
来源：http://hz.guannengcc.top/gtkieugaiw.html

TS:   structuredClone(obj)
来源：http://hz.kuanghao11.cn/gtsawgewlo.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.316326.xyz/gtthslxgca.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gaohongyu789.top/gthrbncuwi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhengqikj.top/gtopebfarw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jqgfzy.top/gtmmeoexmb.html

[K06] 解析 URL 查询串
来源：http://hz.jyoumei.cn/gtjubgmpaw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ydzc1.top/gtvwwkukvs.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ywan-chungtsiang.top/gtipelkyeh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xuanzx.com/gtqhxizkvs.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.mhx1999.top/gtlyuxkrtd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xuetiantiany.cn/gtlaicxuod.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cheryme.top/gtjapyilhx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.andypj.xyz/gtcpcvnzuz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.tianlin.xyz/gtxngagogp.html

[K07] 进制转换
来源：http://hz.hnqzz.top/gthvfdihpk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.sweek.top/gtpoujvime.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jinqigufen.top/gtoabdisyw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhijiandao.cn/gtzvxjkozp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.0kj1m.cn/gtezwgongc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.chenlongwang.top/gthipzhcxv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.meibo888.top/gtxtbszgcf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.svipenyu.cn/gtrwiwkufa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yanxiufei.cn/gtxttnudsl.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.chenjidiqi.icu/gthtfpgenh.html

Py:   pickle.dumps(obj)
来源：http://hz.kuanghao11.cn/gtnycqswtb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gzhubu.top/gtgghrbsuo.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.meibo888.top/gtskvmoumu.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.fengsongda.top/gtlfcwqbjx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yuanzhike.top/gtvsekrpuf.html

Go:   encoding/gob
来源：http://hz.jianghu66.top/gtnntebfal.html

Ruby: Marshal.dump(obj)
来源：http://hz.dianchejie.cn/gtlrrmjgpy.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.shuidangran.top/gtdobmpxkt.html

================================================================================
来源：http://hz.yanxiufei.cn/gtvdfxwwwf.html


<!-- 参考信息 -->