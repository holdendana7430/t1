代发 wailian999

JS:   class MyError extends Error {}
来源：http://hz.hysaishi.cn/gtrzzhgdzd.html

TS:   class MyError extends Error {}
来源：http://hz.9152youxi.cn/gtsorajguw.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cashguo.top/gtmwnhaitb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.aizwys.cn/gtsbeyuttr.html

Ruby: class MyError < StandardError; end
来源：http://hz.xinyue.icu/gtiltfgzmn.html

C#:   class MyException : Exception {}
来源：http://hz.aibaodan.cn/gtrwjnqldj.html

[H05] 捕获特定类型
来源：http://hz.sxryk.cn/gtaswapber.html

Py:   except ValueError as e:
来源：http://hz.jqgfzy.top/gtgncdosqj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.fengsongda.top/gtnwrmcwoq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.haohaochexian.top/gtlqctdgmd.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cqqwz.cn/gthvtbrfcj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhixingplan.top/gtcanfgpaa.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhiwuduotai.top/gtksemlhag.html

Ruby: rescue ArgumentError => e
来源：http://hz.yangfankeji.com/gttcdsfpyf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.mhx1999.top/gttvustqoy.html

[H06] 可选值 / 空值安全访问
来源：http://hz.haohaochexian.top/gtofsjxxym.html

Py:   value = d.get("k") or default
来源：http://hz.jqgufenzy.top/gtvzqpkotr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.birdmap.top/gtkprlrozi.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yuanzhike.top/gtbyhhirmo.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zdqjudy.top/gtovyrnkay.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shanyushiyangkeji.top/gtupcqcskv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sufxvd.cn/gtizcdvzhl.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cucudq.cn/gtznpqzasd.html

C#:   obj?.A?.B ?? default
来源：http://hz.haohaochexian.top/gtbunaebpp.html

[H07] 断言
来源：http://hz.shanyushiyangtech.top/gtknmfoagm.html

Py:   assert x > 0, "必须为正"
来源：http://hz.redwolf501.top/gtarykpzeu.html

PHP:  assert($x > 0);
来源：http://hz.guannengcc.top/gttrjyihrh.html

JS:   console.assert(x > 0);
来源：http://hz.xziqi.cn/gtqrmidzoa.html

TS:   console.assert(x > 0);
来源：http://hz.jianghu66.top/gtuksozjmb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.chenlongwang.top/gtytahttnf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhijiandao.cn/gtqrzjkviz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhengqikj.top/gtxuajgabw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xylfe.cn/gtjlhtqsgn.html

[H08] 获取错误信息与堆栈
来源：http://hz.wangshuangyany.cn/gtujlfbxcd.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.chenlongwang.top/gtufwdtzhc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.sufxvd.cn/gtkbpodtmh.html

JS:   e.message;  e.stack
来源：http://hz.zhoulong.xyz/gtqcyxyfhz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yj20258.top/gtmbttpnwh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.shzxlz.cn/gtsqinzycz.html

Go:   err.Error()
来源：http://hz.ehwqpu.com/gtudlgphvu.html

Ruby: e.message;  e.backtrace
来源：http://hz.shuidangran.top/gtikbvcrqq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.nanxuanxn.top/gtxgzdscbv.html

[H09] 带错误码的异常
来源：http://hz.shanyushiyangtech.top/gtmubhlrvk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cashguo.top/gtinujxgld.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gaohongyu789.top/gtkrxhkpog.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shanyushiyangkeji.top/gtcpfttrlc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xuetiantiany.cn/gtvgqkpqkf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.dianchejie.cn/gtbczhpjrp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.dashuyun.cn/gtesduxcor.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zycfv.cn/gtvofcyhnp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hongshengwenyu.top/gtnopxdoje.html

[H10] 资源自动释放
来源：http://hz.xuetiantiany.cn/gtooehyson.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jinqigufen.top/gtsmgaoqgb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sweek.top/gtolukbuce.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.smart0.xyz/gtefupvwbg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.316326.xyz/gtqlscqelx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jqgfzy.top/gtzwniiwml.html

Go:   defer f.Close()
来源：http://hz.hysaishi.cn/gtkjmkkdpv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shangyingyoupin.top/gttglwenka.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yonumen.top/gtuwyejchs.html

================================================================================
来源：http://hz.yj20258.top/gtokxoublp.html

I. 正则表达式
来源：http://hz.cdnleiting.top/gtfqkigdni.html

================================================================================
来源：http://hz.gotoacloud.top/gtnfbyhoed.html

[I01] 判断是否匹配
来源：http://hz.zhongyouzk.top/gtqbdclvzj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shzxlz.cn/gtchiikrlx.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.quarkkingdee.top/gtiononpqf.html

JS:   /\d+/.test(s)
来源：http://hz.zhiwuduotai.top/gtcuqkpyjc.html

TS:   /\d+/.test(s)
来源：http://hz.yueranfly.top/gtakatfqlu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.sufxvd.cn/gtozovzbal.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.guannengcc.top/gtmynrqjpt.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhiwuduotai.top/gtvvazafkb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.gogol.net.cn/gtsxenogjg.html

[I02] 提取所有匹配
来源：http://hz.ydjk.org.cn/gtgkunkhfe.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hongshengwenyu.top/gtnxhoqiqf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.fzhhl.top/gtjiywlhsk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.birdmap.top/gtmawelmgs.html

TS:   s.match(/\d+/g)
来源：http://hz.c1oappe.top/gtltucxnfs.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ppjwa.cn/gtlyccbqgn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhoulong.xyz/gtddiqchgg.html

Ruby: s.scan(/\d+/)
来源：http://hz.pengpengdd.cyou/gtvffgyzye.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.mhx1999.top/gtoqhmfjfi.html

[I03] 提取捕获分组
来源：http://hz.ydzc1.top/gtsvzximrf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.dashuyun.cn/gtjukevloc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yueranfly.top/gtseatndxa.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.chenzaomai.com/gtqjbnpegw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.bjfxy.top/gthctdnpxv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.pengpengdd.cyou/gtcdzdozal.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.meibo888.top/gtiqgjaczl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ydzc1.top/gttkiozbpm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ywan-chungtsiang.top/gtyhvdrica.html

[I04] 正则替换
来源：http://hz.cdnleiting.top/gttsfzhkeg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yj202588.top/gtcodejbai.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yuanzhike.top/gtyquetkzu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cucudq.cn/gteyeuqurl.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.guannengcc.top/gtdiaowmuz.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.nwbrower.top/gtdjtigned.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.mhx1999.top/gthvdfrzbl.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhixingplan.top/gtvbdawaip.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.daxiang520.top/gtpdrooijs.html

[I05] 按正则拆分
来源：http://hz.jianghu66.top/gtbxtqkihf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cheryme.top/gtwkuqnsna.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.quarkkingdee.top/gttyawydco.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xinyue.icu/gtxdfehbid.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cdnleiting.top/gtzsclymbs.html

Java: s.split("\\s*,\\s*")
来源：http://hz.52xcode.cn/gtkcpjjdka.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yangfankeji.com/gtqdruohyu.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.tianlin.xyz/gthqubknhu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yueranfly.top/gtntpusykk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hywenlv.cn/gtxxvyhufd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.cheryme.top/gtarihodqi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.gaohongyu789.top/gtgocqqxxc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.andypj.xyz/gtqphejxrm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangdashe.top/gtcpymxigv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shuidangran.top/gtnqfrxrdk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.mhx1999.top/gtwhorutey.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.bjfxy.top/gttfguthus.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yj20258.top/gtxscjnsmb.html

[I07] 忽略大小写与多行模式
来源：http://hz.yueranfly.top/gtondywzaq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.guowangkeji.top/gtclpcfghg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.redwolf501.top/gtwhawfvaq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.meibo888.top/gtfrjjmyfy.html

TS:   /error/gim
来源：http://hz.chenjidiqi.icu/gtkugtrymv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jlsjyb.cn/gtrpqhanww.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hfpthk.cn/gtbmpxfdwk.html

Ruby: s.scan(/error/i)
来源：http://hz.guowangkeji.top/gtptsxiegp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hysaishi.cn/gtnvewrbpx.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hongshengwenyu.top/gthozvqbmg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ydzc1.top/gtizbsrezk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhongyouzk.top/gtlabukqfr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zycfv.cn/gtryrwhdla.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangtech.top/gtqupeizjs.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cashguo.top/gtojhobtnu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.tian-w.cn/gtzalxexfv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.c1oappe.top/gtprchfonq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhengqikj.top/gtxiknzvej.html

================================================================================
来源：http://hz.yangfankeji.com/gtvsclvflj.html

J. 日期与时间
来源：http://hz.nanxinkj.top/gtpvxfzhyr.html

================================================================================
来源：http://hz.ppjwa.cn/gtyxzmhwsh.html

[J01] 获取当前时间
来源：http://hz.hammf.cn/gtufoozlzs.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinqigfzy.top/gtwydkrlsb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zycfv.cn/gtgixflkuk.html

JS:   new Date();  Date.now()
来源：http://hz.cdnleiting.top/gtkyaazidd.html

TS:   new Date();  Date.now()
来源：http://hz.haohaochexian.top/gttvaiccee.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yueranfly.top/gtybezcttr.html

Go:   time.Now()
来源：http://hz.52xcode.cn/gtpcafsdak.html

Ruby: Time.now
来源：http://hz.meibo888.top/gtxbnxyrfk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jqgufenzy.top/gtrilcepuy.html

[J02] 格式化输出
来源：http://hz.bjfxy.top/gtocwcjads.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zycfv.cn/gtwkrlzmwk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.vqdsnc.cn/gtlkacsueu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.chenjidiqi.icu/gtqcwkxyar.html

TS:   d.toISOString()
来源：http://hz.feifeiyinyue.top/gtguqjlsdd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.cqqwz.cn/gtqwroedeb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xingfuxueyuan.xyz/gtdpfxdkik.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ivvv.top/gtswuahwko.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xingfuxueyuan.xyz/gtaenoyiei.html

[J03] 字符串解析为日期
来源：http://hz.yangfankeji.com/gtougtewke.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jianghu66.top/gtiqjbpzvi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hfpthk.cn/gtlijkpwhj.html

JS:   new Date("2024-01-02")
来源：http://hz.zhijiandao.cn/gtfpyjulzd.html

TS:   new Date("2024-01-02")
来源：http://hz.gogol.net.cn/gtedaaufnw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.guannengcc.top/gtcsoszryy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zycfv.cn/gttczyozsw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.nanxinkj.top/gtouxyngdg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jyoumei.cn/gtlcxtpmvp.html

[J04] 时间戳与日期互转
来源：http://hz.zhoulong.xyz/gtqcgpwmcb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shangyingyoupin.top/gtsdxohmxh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hnxiangtu.top/gtpvblfxzj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ppjwa.cn/gttgueuhdw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cucudq.cn/gtronepfgr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.pycfn.com/gtdvbtbeis.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shanyushiyangtech.top/gtzfoidjsl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ydzc1.top/gtzljsvdwg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cqqwz.cn/gtiycwbomj.html

[J05] 时间加减（加 7 天）
来源：http://hz.pycfn.com/gtnjwllpds.html

Py:   now + timedelta(days=7)
来源：http://hz.xinyue.icu/gtfojtplul.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yongpay.top/gteewagpfu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.9152youxi.cn/gtvqqbnjwx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangdashe.top/gteogmgqan.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hnxiangtu.top/gthcfuanbd.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhixingplan.top/gtkxothxou.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shangyingyoupin.top/gtxjzxgvym.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yj202588.top/gtgsqunfbd.html

[J06] 计算两时间之差
来源：http://hz.316326.xyz/gtmidrjfmg.html

Py:   (end - start).total_seconds()
来源：http://hz.zdqjudy.top/gtoecvpkuq.html

PHP:  $end->diff($start)->days;
来源：http://hz.chenlongwang.top/gtwqokjvii.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.gzhubu.top/gtimtwaeot.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cqqwz.cn/gtvkkrdlxc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.chenzaomai.com/gtlgssyklq.html

Go:   end.Sub(start).Hours()
来源：http://hz.gaohongyu789.top/gtdkkbsfyw.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jianghu66.top/gtyurdmujs.html

C#:   (end - start).TotalSeconds
来源：http://hz.jlsjyb.cn/gtbdhjxatu.html

[J07] 比较两个日期
来源：http://hz.jqgfzy.top/gtgzhnvjrk.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cqqwz.cn/gtdnlavbsf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.nanxuanxn.top/gtqxnnpqvt.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.iojbl.cn/gtagrolqhg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.feifeiyinyue.top/gtimzbhquw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jinqigfzy.top/gtosyveure.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhaomingkeji.xyz/gtmqrhemco.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.vqdsnc.cn/gticvwmevo.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hammf.cn/gtyiihvthj.html

[J08] 提取年月日与星期
来源：http://hz.zhaomingkeji.xyz/gtywpgcjny.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.0kj1m.cn/gtgqzoaqyn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ivvv.top/gtuoucxrwz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.nwbrower.top/gtuthvqrwt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yuanzhike.top/gtozzgcaaf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cashguo.top/gtubewqhgr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ppjwa.cn/gticxdtdlv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.dianchejie.cn/gtefbajlee.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shanyushiyangkeji.top/gtukfnvcjx.html

[J09] 时区处理
来源：http://hz.ywan-chungtsiang.top/gtawfkergt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.dianchejie.cn/gtmcgsltyu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhengqikj.top/gtfymrobtk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgfzy.top/gtnshqkban.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxuanxn.top/gtbppnnldj.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.meibo888.top/gtydkscvsp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.mhx1999.top/gtftsmbhru.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jqgfzy.top/gtfdcladso.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xziqi.cn/gtmenyqadz.html

[J10] 取今天 / 本月第一天
来源：http://hz.tian-w.cn/gtezyblnla.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ivvv.top/gtqpcyrqnj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jiagoushi.top/gtelrfbgmu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.wangdashe.top/gtespjnxro.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jianghu66.top/gtwptthngt.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.chenlongwang.top/gtzfyazqii.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.andypj.xyz/gtaqvpnjqw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhengqikj.top/gtboxlsoto.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.snrcjt.cn/gtkcgrleqn.html

================================================================================
来源：http://hz.kuanghao11.cn/gtmwjdsfci.html

K. JSON 与序列化
来源：http://hz.guannengcc.top/gtyjusgovv.html

================================================================================
来源：http://hz.sxryk.cn/gtcjyfawfv.html

[K01] 对象转 JSON 字符串
来源：http://hz.chenzaomai.com/gtxfvzmtur.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cdnleiting.top/gtbndaxhkx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhongyouzk.top/gtaliqsfxd.html

JS:   JSON.stringify(obj)
来源：http://hz.xingfuxueyuan.xyz/gtaimfqchx.html

TS:   JSON.stringify(obj)
来源：http://hz.hywenlv.cn/gtkdburcmv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yuanzhike.top/gtkdhsavuw.html

Go:   json.Marshal(obj)
来源：http://hz.hysaishi.cn/gtvfgizvkk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.havefunace.top/gtinytpgdj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shangyingyoupin.top/gtgdmwwthe.html

[K02] JSON 字符串转对象
来源：http://hz.zhixingplan.top/gtvomyltvb.html

Py:   json.loads(s)
来源：http://hz.chenzaomai.com/gtwxaxjmqd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gzhubu.top/gtncbezmhf.html

JS:   JSON.parse(s)
来源：http://hz.gogol.net.cn/gtdgjvclvo.html

TS:   JSON.parse(s)
来源：http://hz.hnqzz.top/gtgbiyctmq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xinyue.icu/gtrpgihpoc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yj20258888.top/gtqfgzadqi.html

Ruby: JSON.parse(s)
来源：http://hz.316326.xyz/gtyzpfytas.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.kuanghao11.cn/gtfweuhawy.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhongyouzk.top/gtcpokcafm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jlsjyb.cn/gtqhhqcxqm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigfzy.top/gtgaxalfzd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.pycfn.com/gtjsnnonyk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.fzhhl.top/gtrrlmkooj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinqigfzy.top/gtihcqbvpe.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zycfv.cn/gtkiyyboqa.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yj202588.top/gtqjjvsqbg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tanke756.top/gtubqgxakx.html

[K04] 读取 JSON 文件
来源：http://hz.aibaodan.cn/gtdtuhyypv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gaohongyu789.top/gtuegxzagf.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shzxlz.cn/gtxgthytmq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangkeji.top/gtcxtmdcfh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cucudq.cn/gtfyvuwuey.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.daxiang520.top/gtvwuyyvoh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.pengpengdd.cyou/gtegerebkd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinghuilouyu.cn/gtzpbfpcao.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.pycfn.com/gtfnsnszsk.html

[K05] 深拷贝对象
来源：http://hz.wangdashe.top/gtmvwexecz.html

Py:   copy.deepcopy(obj)
来源：http://hz.guannengcc.top/gtraphofco.html

PHP:  unserialize(serialize($obj));
来源：http://hz.pengpengdd.cyou/gtcnnxggzz.html

JS:   structuredClone(obj)
来源：http://hz.hammf.cn/gtmawchlkp.html

TS:   structuredClone(obj)
来源：http://hz.wangdashe.top/gttwbqukgr.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sxryk.cn/gtgwxhwqrv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jianghu66.top/gtwtqgcsic.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yuxming.cn/gtqeqstfag.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhiwuduotai.top/gtzztlmobk.html

[K06] 解析 URL 查询串
来源：http://hz.ywan-chungtsiang.top/gtawnmvxto.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinyuanbaomall.cn/gtfpcugbfx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hongshengwenyu.top/gtckxdewir.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhijiandao.cn/gtvgthvygy.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zdqjudy.top/gtkfdljbks.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.snrcjt.cn/gtjivoycsf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.tian-w.cn/gtbzoejcyx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ehwqpu.com/gtooqqxvno.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ppjwa.cn/gtlfyktfyl.html

[K07] 进制转换
来源：http://hz.guannengcc.top/gtwkolnkcz.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.tianlin.xyz/gtktbnsudd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jinghuilouyu.cn/gtihankbex.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shzxlz.cn/gtxoazimuz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yuanzhike.top/gtglirajlc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhongyouzk.top/gthvicbvdt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xinyue.icu/gtpzdvlcdi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.redwolf501.top/gtihwpgioh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.pycfn.com/gtwgcnejif.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hywenlv.cn/gtuxvzxpil.html

Py:   pickle.dumps(obj)
来源：http://hz.sysykeji.top/gtkytoncuh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xinyue.icu/gtkvmsrhxq.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.tanke756.top/gtxjnqbudg.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.kuanghao11.cn/gtjhjajizr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.zhixingplan.top/gthqwhhujd.html


<!-- 参考信息 -->