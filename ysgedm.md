代发 wailian999

[H07] 断言
来源：http://hz.yangfankeji.com/gttvwaoxrp.html

Py:   assert x > 0, "必须为正"
来源：http://hz.chenzaomai.com/gtqbhgygxk.html

PHP:  assert($x > 0);
来源：http://hz.hnxiangtu.top/gtkwbcqymo.html

JS:   console.assert(x > 0);
来源：http://hz.hammf.cn/gtvwifmhot.html

TS:   console.assert(x > 0);
来源：http://hz.wangdashe.top/gtjdozpmcq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jinghuilouyu.cn/gthxdeetnf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yueranfly.top/gtshrzpwdf.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.0kj1m.cn/gtexsslkgq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.daxiang520.top/gtmtrudfub.html

[H08] 获取错误信息与堆栈
来源：http://hz.bjfxy.top/gtmuzswwtk.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.dashuyun.cn/gttaqsywax.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ywan-chungtsiang.top/gtmvlqpoaj.html

JS:   e.message;  e.stack
来源：http://hz.jinqigfzy.top/gtwahnwxro.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hongshengwenyu.top/gtsnlzskpd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cdnleiting.top/gtubttzdyd.html

Go:   err.Error()
来源：http://hz.jiagoushi.top/gtxksitees.html

Ruby: e.message;  e.backtrace
来源：http://hz.yj202588.top/gtdtxiahro.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ybcxt.top/gtvkuiivrv.html

[H09] 带错误码的异常
来源：http://hz.yonumen.top/gtzzntixdk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yuanzhike.top/gtbyckclta.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.wangdashe.top/gtduifyozq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jyoumei.cn/gtazypixfn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gogol.net.cn/gtfenfcehk.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yvedp.cn/gtsptuomcn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhoulong.xyz/gtudvmoudl.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.daria6918.cn/gttzpsnodv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ehwqpu.com/gtwirbyeqd.html

[H10] 资源自动释放
来源：http://hz.jyoumei.cn/gtizqgbdtw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.smart0.xyz/gtftpqugcj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xziqi.cn/gtpwmrfxmp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gtuounguny.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dashuyun.cn/gtipabowxa.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ivvv.top/gtzqmxmqan.html

Go:   defer f.Close()
来源：http://hz.tanke756.top/gtsimpbpuy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cucudq.cn/gtgeovnpwv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yongpay.top/gtrzaofbdi.html

================================================================================
来源：http://hz.xziqi.cn/gtvatcagrq.html

I. 正则表达式
来源：http://hz.ybcxt.top/gtufcvqafj.html

================================================================================
来源：http://hz.nwbrower.top/gtsfgxrhys.html

[I01] 判断是否匹配
来源：http://hz.shzxlz.cn/gtpliiwaid.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shanyushiyangtech.top/gtoxgjvgfr.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xziqi.cn/gtvqxfzdvb.html

JS:   /\d+/.test(s)
来源：http://hz.ydzc1.top/gtorjwsquc.html

TS:   /\d+/.test(s)
来源：http://hz.haohaochexian.top/gtzaceozse.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhixingplan.top/gthixdpbpd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cheryme.top/gtnercupxq.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhiwuduotai.top/gtmyjhzbez.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.feifeiyinyue.top/gtktjpsifr.html

[I02] 提取所有匹配
来源：http://hz.haohaochexian.top/gtanffpbng.html

Py:   re.findall(r"\d+", s)
来源：http://hz.guowangkeji.top/gthivprdgi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.0kj1m.cn/gtdlgtsnre.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jlsjyb.cn/gtwptsyvxo.html

TS:   s.match(/\d+/g)
来源：http://hz.yj20258.top/gtjdjmjjqs.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jlsjyb.cn/gtabrcoifh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xziqi.cn/gtjggulmpa.html

Ruby: s.scan(/\d+/)
来源：http://hz.c1oappe.top/gtqicyivnh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhixingplan.top/gtkubmnagb.html

[I03] 提取捕获分组
来源：http://hz.c1oappe.top/gtmtxjdcmp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zdqjudy.top/gtpenjmuww.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gaohongyu789.top/gtffrtlpiq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhijiandao.cn/gtkljbxajb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tanke756.top/gtdaixyqux.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jqgufenzy.top/gtlpbybsmv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.fzhhl.top/gtluzgpwgu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.9152youxi.cn/gtorownvsf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.sysykeji.top/gthwiqqdtx.html

[I04] 正则替换
来源：http://hz.nwbrower.top/gtpofrbvzo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.andypj.xyz/gtldfbtxdm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jiagoushi.top/gtfnggnzzm.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.quarkkingdee.top/gtyksjunlg.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cdnleiting.top/gtufpxzahs.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yuanzhike.top/gtkizzveff.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.nanxinkj.top/gtzntdkcam.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.tianlin.xyz/gtaooielao.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nanxuanxn.top/gtgxsmknrz.html

[I05] 按正则拆分
来源：http://hz.shanyushiyangkeji.top/gtjqtggxti.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cqqwz.cn/gtnjhmdgfb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.birdmap.top/gtyxfhnurd.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.aizwys.cn/gteukqnvqj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xingfuxueyuan.xyz/gtndtxmdut.html

Java: s.split("\\s*,\\s*")
来源：http://hz.gotoacloud.top/gtdnzbvhbc.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.sxryk.cn/gtugckdxgq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.aizwys.cn/gtqrynffsi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.daria6918.cn/gtdzelhtfq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.snrcjt.cn/gtrycsnmsm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinqigfzy.top/gttzzytwkj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jinyuanbaomall.cn/gtpxtraauq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhixingplan.top/gtamyemiqf.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhiwuduotai.top/gthhgidxgw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.daxiang520.top/gtzreiiuan.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.redwolf501.top/gtdoyfrzgi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.snrcjt.cn/gtglbvaefa.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhaomingkeji.xyz/gtvbzetiry.html

[I07] 忽略大小写与多行模式
来源：http://hz.snrcjt.cn/gttwveoamp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jinyuanbaomall.cn/gtdacmwohw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.birdmap.top/gtwzgsgjxp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.iojbl.cn/gtjwayjyhy.html

TS:   /error/gim
来源：http://hz.jinghuilouyu.cn/gtnooinymo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.pengpengdd.cyou/gtqnhnporq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hywenlv.cn/gtdgkvajji.html

Ruby: s.scan(/error/i)
来源：http://hz.pycfn.com/gtunliclga.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xuetiantiany.cn/gtktklsafu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shangyingyoupin.top/gtqfpaxhcp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.nwbrower.top/gtijgjrsyk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hywenlv.cn/gtpejecpoq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.svipenyu.cn/gtglradlnv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.52xcode.cn/gtmkfewmic.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.guowangkeji.top/gtieoxipoh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.dianchejie.cn/gtijrkczoa.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yonumen.top/gtbldygztx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yj20258888.top/gtyrrayfta.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtwwevtcfo.html

J. 日期与时间
来源：http://hz.ydzc1.top/gtuernzqjz.html

================================================================================
来源：http://hz.0kj1m.cn/gtohqmsjop.html

[J01] 获取当前时间
来源：http://hz.smart0.xyz/gtdoyiwovy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xuanzx.com/gtxvjhoriq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.gogol.net.cn/gtqbdglacz.html

JS:   new Date();  Date.now()
来源：http://hz.shangyingyoupin.top/gtetgzwhrb.html

TS:   new Date();  Date.now()
来源：http://hz.vqdsnc.cn/gtezgzylyl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gogol.net.cn/gtfegturfn.html

Go:   time.Now()
来源：http://hz.shanyushiyangkeji.top/gtdpeguurf.html

Ruby: Time.now
来源：http://hz.iojbl.cn/gtlxjntxbt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.gaohongyu789.top/gtwlqszgvi.html

[J02] 格式化输出
来源：http://hz.wangdashe.top/gtcvigzway.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.vqdsnc.cn/gtjpgavfcv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhengqikj.top/gtwvyqedbp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hnxiangtu.top/gtbggcxqch.html

TS:   d.toISOString()
来源：http://hz.quarkkingdee.top/gtzfdbylgi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.iojbl.cn/gtmsiphkwu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.sysykeji.top/gtuiwtlxhr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.redwolf501.top/gthavylnus.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.daria6918.cn/gtggqxvgic.html

[J03] 字符串解析为日期
来源：http://hz.cqqwz.cn/gtmypyhrax.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sxryk.cn/gtrvyqxwmu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.guowangkeji.top/gtptcfmnsg.html

JS:   new Date("2024-01-02")
来源：http://hz.jqgufenzy.top/gtamjmfsfi.html

TS:   new Date("2024-01-02")
来源：http://hz.jianghu66.top/gtqntgunzy.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sufxvd.cn/gttycvxucq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tanke756.top/gtttlmiqqa.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhengqikj.top/gtouxdlvsk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cashguo.top/gttqnudezk.html

[J04] 时间戳与日期互转
来源：http://hz.pycfn.com/gtqkhyptit.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.0kj1m.cn/gtjfbgeiys.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.fengsongda.top/gtwgcaahin.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.chenzaomai.com/gtnylvmswh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jianghu66.top/gttgiqfrhn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhongyouzk.top/gtuxlzaqdk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jinqigufen.top/gtogtgybbb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.aibaodan.cn/gtfscnrjsg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hywenlv.cn/gtmpdihrjw.html

[J05] 时间加减（加 7 天）
来源：http://hz.sysykeji.top/gtzbeomueo.html

Py:   now + timedelta(days=7)
来源：http://hz.yj202588.top/gtyoqsqjro.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.chenlongwang.top/gtwechdvmh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnqzz.top/gtawskiblr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nwbrower.top/gtmelncibi.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.vqdsnc.cn/gtsqfzzmmc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cucudq.cn/gtakhtyqfm.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jiagoushi.top/gtbkcbbcoo.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.tian-w.cn/gtxxufotao.html

[J06] 计算两时间之差
来源：http://hz.chenlongwang.top/gtsrlfjzuj.html

Py:   (end - start).total_seconds()
来源：http://hz.wangshuangyany.cn/gtrspfhlko.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhixingplan.top/gtktoottbq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.cashguo.top/gtwszkdhmx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yueranfly.top/gtvpcimzfd.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cucudq.cn/gtgonvuitp.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhengqikj.top/gtmkrsyzfv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.andypj.xyz/gthhmvfnmz.html

C#:   (end - start).TotalSeconds
来源：http://hz.nanxuanxn.top/gtgeydbtuj.html

[J07] 比较两个日期
来源：http://hz.meibo888.top/gtbrhuqbfm.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.c1oappe.top/gtjdhxetvo.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ydzc1.top/gtzkyeomun.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj202588.top/gttfrjphtu.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xuanzx.com/gttlgsrwds.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jlsjyb.cn/gtcxeitziq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hammf.cn/gtnoycpiyt.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ywan-chungtsiang.top/gtkiylozbf.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.kuanghao11.cn/gtihiatshv.html

[J08] 提取年月日与星期
来源：http://hz.cqqwz.cn/gtgebvvqmu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhongyouzk.top/gtqnajcrfm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.gaohongyu789.top/gtcfzipzdo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hnxiangtu.top/gtldpuknrd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.pycfn.com/gtatbzssds.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yueranfly.top/gtuxsrndik.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.guowangkeji.top/gtbgeipeja.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xuetiantiany.cn/gtphjqcwwg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zdqjudy.top/gtygmjzabd.html

[J09] 时区处理
来源：http://hz.yuxming.cn/gtllzeshgr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xuanzx.com/gtwvwquazn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.andypj.xyz/gtequgimpo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangshuangyany.cn/gtrekkwqaa.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgfzy.top/gtntgxdrbw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gzhubu.top/gtebcubflz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.kuanghao11.cn/gtbmwgbido.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.nanxinkj.top/gtijtfoftw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yj20258888.top/gtayvoufiv.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhijiandao.cn/gtllrcsuhl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj20258888.top/gtnlhelvuc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shanyushiyangtech.top/gtgilorhef.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yj20258888.top/gtuikufqxl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hammf.cn/gthhdmyhcw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.andypj.xyz/gtnlntrlxn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ehwqpu.com/gtrtrmyadg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.snrcjt.cn/gtzdnicefl.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xuanzx.com/gtwyqqixaz.html

================================================================================
来源：http://hz.gzhubu.top/gtoqeobmed.html

K. JSON 与序列化
来源：http://hz.shangyingyoupin.top/gtktwbroox.html

================================================================================
来源：http://hz.cheryme.top/gtvbbwifwu.html

[K01] 对象转 JSON 字符串
来源：http://hz.zycfv.cn/gtqguhstxv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yj20258.top/gtvflxyiqj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yanxiufei.cn/gtxurgnvrn.html

JS:   JSON.stringify(obj)
来源：http://hz.jianghu66.top/gthpuppaxq.html

TS:   JSON.stringify(obj)
来源：http://hz.iojbl.cn/gtzefylyxc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cdnleiting.top/gtfujwuiif.html

Go:   json.Marshal(obj)
来源：http://hz.birdmap.top/gtpzswklkg.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cqqwz.cn/gtgtqtgwxc.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shangyingyoupin.top/gtbpxsnido.html

[K02] JSON 字符串转对象
来源：http://hz.quarkkingdee.top/gtvcovadax.html

Py:   json.loads(s)
来源：http://hz.yonumen.top/gtzkgopqwz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.chenjidiqi.icu/gtpgjzimlj.html

JS:   JSON.parse(s)
来源：http://hz.feifeiyinyue.top/gtmedvohel.html

TS:   JSON.parse(s)
来源：http://hz.gogol.net.cn/gtzsgaczki.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.nanxinkj.top/gtxgljmyzu.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hongshengwenyu.top/gtawgsjqhf.html

Ruby: JSON.parse(s)
来源：http://hz.gogol.net.cn/gtvhmnymjo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinqigfzy.top/gtdhqtjvxr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinqigufen.top/gtorxbhnzm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.guowangkeji.top/gthnmdbmgp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.sxryk.cn/gtapnbucmd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hongshengwenyu.top/gttqmyddok.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.smart0.xyz/gthwolrhow.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hammf.cn/gtzdgljzsk.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhiwuduotai.top/gtfzotussr.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhaomingkeji.xyz/gtrlkpwdao.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yuxming.cn/gttrtpkgpe.html

[K04] 读取 JSON 文件
来源：http://hz.gotoacloud.top/gtstygzuwp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.smart0.xyz/gtkosiiryj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ppjwa.cn/gtdqmevlpz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gtitkismyj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hysaishi.cn/gtaagulsew.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.wangdashe.top/gtwpmwuydc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xingfuxueyuan.xyz/gtizajlgzb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yuanzhike.top/gtjbsonclq.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinqigufen.top/gtdajiaexp.html

[K05] 深拷贝对象
来源：http://hz.sxryk.cn/gtjhkzrnyk.html

Py:   copy.deepcopy(obj)
来源：http://hz.chenjidiqi.icu/gtbnkqydiq.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhoulong.xyz/gtkftqrekm.html

JS:   structuredClone(obj)
来源：http://hz.quarkkingdee.top/gtwlgzvrhh.html

TS:   structuredClone(obj)
来源：http://hz.mhx1999.top/gtzzzmvuky.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gotoacloud.top/gttvqpkvpz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.shzxlz.cn/gtmheuwyxx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shuidangran.top/gtohgvcgwi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zhoulong.xyz/gtljiosbki.html

[K06] 解析 URL 查询串
来源：http://hz.hammf.cn/gtsmmrnakf.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.52xcode.cn/gtbysylilz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.dashuyun.cn/gtmrzfklby.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xuanzx.com/gtvmzwwnvo.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydzc1.top/gtcbdofvgn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xuetiantiany.cn/gtnijzavem.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.birdmap.top/gtchnhumzp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.guowangkeji.top/gtatnoudqs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhaomingkeji.xyz/gtexuosnun.html

[K07] 进制转换
来源：http://hz.ywan-chungtsiang.top/gtcfxhmnqn.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shangyingyoupin.top/gtethoktbz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ydjk.org.cn/gtsnqkhyuj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.dianchejie.cn/gtgatfahbe.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.fzhhl.top/gtwwqinfnh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hywenlv.cn/gtlpwczrzq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.chenzaomai.com/gtjiqigrzo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.pycfn.com/gtodddlxxn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ivvv.top/gtnwfggimc.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhixingplan.top/gtznxraovk.html

Py:   pickle.dumps(obj)
来源：http://hz.dashuyun.cn/gtndobdfcz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ehwqpu.com/gttzlgfido.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.xingfuxueyuan.xyz/gtimymdaef.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.daxiang520.top/gtveapbhdz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.feifeiyinyue.top/gtkosgrcxw.html

Go:   encoding/gob
来源：http://hz.ppjwa.cn/gtundwmatp.html

Ruby: Marshal.dump(obj)
来源：http://hz.haohaochexian.top/gtjvbiueth.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yuxming.cn/gtgprkkada.html

================================================================================
来源：http://hz.xuanzx.com/gtptkakzuv.html

L. 网络请求
来源：http://hz.yj20258888.top/gtdrxhgptn.html

================================================================================
来源：http://hz.gzhubu.top/gtcjcqxzlr.html

[L01] 发送 GET 请求
来源：http://hz.jinghuilouyu.cn/gtmffyqdgt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.chenzaomai.com/gtujkyezvn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.52xcode.cn/gtxmcgfkgu.html

JS:   await fetch(url)
来源：http://hz.hysaishi.cn/gtxpvxtbaj.html

TS:   await fetch(url)
来源：http://hz.zhaomingkeji.xyz/gtczboqozw.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.ivvv.top/gtplwxtmjd.html

Go:   resp, err := http.Get(url)
来源：http://hz.snrcjt.cn/gtchfuvrvt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.dianchejie.cn/gtthtnlfvj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xingfuxueyuan.xyz/gtehghhedr.html

[L02] 发送 POST JSON
来源：http://hz.zhaomingkeji.xyz/gtiyrqfcqp.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.xuanzx.com/gtcyfamipe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.xylfe.cn/gtxybriotd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.nanxinkj.top/gtfzufsbpt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.wangshuangyany.cn/gtofflvdkt.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.xuanzx.com/gtlpcfqkbm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.hongshengwenyu.top/gtqxjlbbtm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.xingfuxueyuan.xyz/gtzmerjgxz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.hfpthk.cn/gtpqqztqhb.html


<!-- 参考信息 -->