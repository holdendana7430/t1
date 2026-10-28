代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hammf.cn/gtdgjeykbo.html

Ruby: rescue ArgumentError => e
来源：http://hz.nanxinkj.top/gtejjuakah.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.kuanghao11.cn/gtxrekqtdx.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sxryk.cn/gtuaqhwsjh.html

Py:   value = d.get("k") or default
来源：http://hz.cashguo.top/gtqzzfxyod.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xylfe.cn/gteeyccygb.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.meibo888.top/gtqmahqbal.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.haohaochexian.top/gtbsahenxj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhengqikj.top/gtmntqborg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.haohaochexian.top/gtuhseooxf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.vqdsnc.cn/gtdomjxawv.html

C#:   obj?.A?.B ?? default
来源：http://hz.ppjwa.cn/gtxzehxwus.html

[H07] 断言
来源：http://hz.9152youxi.cn/gtvyyiummv.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhaomingkeji.xyz/gtjazmqcbq.html

PHP:  assert($x > 0);
来源：http://hz.bjfxy.top/gtwebcxklh.html

JS:   console.assert(x > 0);
来源：http://hz.wangdashe.top/gtvayszqbv.html

TS:   console.assert(x > 0);
来源：http://hz.tian-w.cn/gtwjckkzcz.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xziqi.cn/gtgqhjgpxr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.316326.xyz/gtlfaaeucp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.birdmap.top/gtlcnxhcdl.html

C#:   Debug.Assert(x > 0);
来源：http://hz.0kj1m.cn/gtrlrmtrvb.html

[H08] 获取错误信息与堆栈
来源：http://hz.hongshengwenyu.top/gtdsswotlb.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yvedp.cn/gtntrjnvhr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shzxlz.cn/gthpicqzha.html

JS:   e.message;  e.stack
来源：http://hz.ybcxt.top/gtoemvvwnw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yueranfly.top/gtdtuzdnwr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gotoacloud.top/gtevapqueb.html

Go:   err.Error()
来源：http://hz.9152youxi.cn/gtlkezxlmo.html

Ruby: e.message;  e.backtrace
来源：http://hz.cucudq.cn/gtxdvpimgf.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cqqwz.cn/gtltjgjzsp.html

[H09] 带错误码的异常
来源：http://hz.redwolf501.top/gtcqkesdow.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.daria6918.cn/gtlogqouts.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.daria6918.cn/gtvqvwauno.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jqgufenzy.top/gtwlgsujio.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xingfuxueyuan.xyz/gtvgvtzdtq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinqigfzy.top/gtqicnkjvr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yanxiufei.cn/gtasqnvrjk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhongyouzk.top/gtummunuul.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.chenzaomai.com/gtrbhxymcu.html

[H10] 资源自动释放
来源：http://hz.zhixingplan.top/gtytvdwekw.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gzhubu.top/gtlxieuonp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yueranfly.top/gtelrjkouy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cucudq.cn/gtuclvgobi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cqqwz.cn/gtuylnasbl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hongshengwenyu.top/gtuxnojeby.html

Go:   defer f.Close()
来源：http://hz.xingfuxueyuan.xyz/gtcwnqqlke.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.gotoacloud.top/gtdgwlpofp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cdnleiting.top/gttelibbey.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtxecpxlaq.html

I. 正则表达式
来源：http://hz.vqdsnc.cn/gtpbqclyof.html

================================================================================
来源：http://hz.redwolf501.top/gtzeavyvxs.html

[I01] 判断是否匹配
来源：http://hz.jqgufenzy.top/gthghfiggi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhoulong.xyz/gtpbuvgclo.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xuetiantiany.cn/gtckgveupj.html

JS:   /\d+/.test(s)
来源：http://hz.cucudq.cn/gtmlzcdmwl.html

TS:   /\d+/.test(s)
来源：http://hz.wangdashe.top/gtbjbhtlhi.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cqqwz.cn/gtdvqiidae.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhaomingkeji.xyz/gtftouzljk.html

Ruby: s.match?(/\d+/)
来源：http://hz.birdmap.top/gtamdizzum.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jianghu66.top/gtyzyludws.html

[I02] 提取所有匹配
来源：http://hz.birdmap.top/gtbcovaula.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhaomingkeji.xyz/gtowkowhrn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.52xcode.cn/gtspnwnxws.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ehwqpu.com/gtfdemrhsd.html

TS:   s.match(/\d+/g)
来源：http://hz.jinqigufen.top/gtrwwvjmgf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhiwuduotai.top/gtdxpvrvfq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.wangshuangyany.cn/gthoyiglfi.html

Ruby: s.scan(/\d+/)
来源：http://hz.dianchejie.cn/gtludmsaei.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yueranfly.top/gtdywhhazc.html

[I03] 提取捕获分组
来源：http://hz.havefunace.top/gtrvwhycqq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.kuanghao11.cn/gtqfigctkf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jyoumei.cn/gtgnucrjqj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yuxming.cn/gtxddtaeie.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.iojbl.cn/gtizxalrwr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xingfuxueyuan.xyz/gtowaxmjsk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.quarkkingdee.top/gtiljatpfs.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.feifeiyinyue.top/gtifnhqigh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.feifeiyinyue.top/gtgerdwarj.html

[I04] 正则替换
来源：http://hz.ehwqpu.com/gtbzxptqwn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinqigfzy.top/gtxyjigfpr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yueranfly.top/gtqprmyswo.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jianghu66.top/gtkofkmkfc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgufenzy.top/gtkuaaeixt.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhijiandao.cn/gtgizxnobn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.feifeiyinyue.top/gteihceteq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cheryme.top/gtvoowfnoo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.guannengcc.top/gtpvtnepye.html

[I05] 按正则拆分
来源：http://hz.hnqzz.top/gtpuwpcmkv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.mhx1999.top/gtsguoxwuv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yuanzhike.top/gtwupwzkuh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.vqdsnc.cn/gtwmuvxglz.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ydjk.org.cn/gtmisgjaeo.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xuanzx.com/gtnrbhazob.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shanyushiyangkeji.top/gtihopumie.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtremmseis.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xingfuxueyuan.xyz/gtdbauqakl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.aizwys.cn/gturoevlmc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shuidangran.top/gtedxqkbst.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yangfankeji.com/gtqkownoku.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hysaishi.cn/gtucuihout.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cashguo.top/gtjcjcfhgh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hysaishi.cn/gtiwilywpd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.316326.xyz/gtnwgasuky.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.nanxuanxn.top/gtkhvqdfwi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.guowangkeji.top/gtalgoiajo.html

[I07] 忽略大小写与多行模式
来源：http://hz.yangfankeji.com/gthhwgurvt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yongpay.top/gtgypsbuie.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.tanke756.top/gtjftoahln.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ydjk.org.cn/gtqtcbsobw.html

TS:   /error/gim
来源：http://hz.shangyingyoupin.top/gtcuwuvygb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cashguo.top/gtnpzmczrf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.haohaochexian.top/gtgtqzdked.html

Ruby: s.scan(/error/i)
来源：http://hz.sysykeji.top/gtcqybrbcn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhongyouzk.top/gtromwhjsh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shuidangran.top/gtpjqcplmw.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jianghu66.top/gtlmytrodc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hysaishi.cn/gtqjhvyzud.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dianchejie.cn/gtczqtnnsp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jyoumei.cn/gtyfonpbne.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hnqzz.top/gthsatqoii.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.birdmap.top/gtsbwpfnjq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.aizwys.cn/gtnufadhut.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhengqikj.top/gtcfabtwez.html

================================================================================
来源：http://hz.ydjk.org.cn/gtbaxpvxns.html

J. 日期与时间
来源：http://hz.xingfuxueyuan.xyz/gtszwokyrl.html

================================================================================
来源：http://hz.guowangkeji.top/gtgfuvywmr.html

[J01] 获取当前时间
来源：http://hz.andypj.xyz/gtfvumktph.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.dashuyun.cn/gtanqwxqsb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yueranfly.top/gthjvtkuco.html

JS:   new Date();  Date.now()
来源：http://hz.haohaochexian.top/gtrtddyngv.html

TS:   new Date();  Date.now()
来源：http://hz.jianghu66.top/gtcqofjvvg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhengqikj.top/gtaixsqaek.html

Go:   time.Now()
来源：http://hz.cheryme.top/gtyhjryyxr.html

Ruby: Time.now
来源：http://hz.yuxming.cn/gtiizyklms.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hnxiangtu.top/gtnywxbnuf.html

[J02] 格式化输出
来源：http://hz.nwbrower.top/gtbvhxhsye.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258.top/gtgfalxcwe.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhiwuduotai.top/gtacrilpjf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.havefunace.top/gtnnviyeub.html

TS:   d.toISOString()
来源：http://hz.kuanghao11.cn/gtfexjsemb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.tianlin.xyz/gtowuwitlq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.mhx1999.top/gtvjoltmth.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.pycfn.com/gtfdaawvmx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hnxiangtu.top/gtzuwjuhhw.html

[J03] 字符串解析为日期
来源：http://hz.shangyingyoupin.top/gtzwnizzgf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yvedp.cn/gtigeyjryb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.nwbrower.top/gtpsxaptcu.html

JS:   new Date("2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtjqxlbejg.html

TS:   new Date("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtjnlgckrb.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.guowangkeji.top/gtwtiblqbm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.wangdashe.top/gttsxjobuq.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hnqzz.top/gthddqdxtb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.chenzaomai.com/gtoukiuhrr.html

[J04] 时间戳与日期互转
来源：http://hz.xylfe.cn/gtpxtjopfi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.daxiang520.top/gtpditwhsv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zycfv.cn/gthdlgbnxh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sufxvd.cn/gthesodrof.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.wangdashe.top/gtzyerdhkk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.bjfxy.top/gtcgtlpklm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.vqdsnc.cn/gtsvlidprz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.pengpengdd.cyou/gtgsxompyu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.gzhubu.top/gtwbbrlijo.html

[J05] 时间加减（加 7 天）
来源：http://hz.cdnleiting.top/gtgotazzpc.html

Py:   now + timedelta(days=7)
来源：http://hz.ybcxt.top/gtghioskjl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yvedp.cn/gtzwcfhboe.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pycfn.com/gtxmazegoi.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.iojbl.cn/gtokmqyebq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.bjfxy.top/gtzbqueweg.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.vqdsnc.cn/gtpwpmupjc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.andypj.xyz/gtnaszufsl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cheryme.top/gtufkfufca.html

[J06] 计算两时间之差
来源：http://hz.zhijiandao.cn/gtrekbkyko.html

Py:   (end - start).total_seconds()
来源：http://hz.jianghu66.top/gtgqeyxnqn.html

PHP:  $end->diff($start)->days;
来源：http://hz.aibaodan.cn/gtmlhkbqtm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.kuanghao11.cn/gtorsgnwuo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ivvv.top/gtjynmahdt.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ehwqpu.com/gtcllkurvh.html

Go:   end.Sub(start).Hours()
来源：http://hz.sysykeji.top/gtklpcxder.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jinghuilouyu.cn/gttoyfgtpj.html

C#:   (end - start).TotalSeconds
来源：http://hz.chenlongwang.top/gtduoigqbc.html

[J07] 比较两个日期
来源：http://hz.ehwqpu.com/gtubolwuog.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.tian-w.cn/gtmadanpko.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.daxiang520.top/gtzhvwuiqa.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xylfe.cn/gtvgejvqzh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.nwbrower.top/gtqxwyfhxt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.guowangkeji.top/gtkyotrzks.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yuxming.cn/gtpyeylkju.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhiwuduotai.top/gtcavbjvza.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenlongwang.top/gtrscquylw.html

[J08] 提取年月日与星期
来源：http://hz.xylfe.cn/gtybbjascw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.pengpengdd.cyou/gtigskqnoz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ehwqpu.com/gtbxllvmyr.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.kuanghao11.cn/gtseyrhkxo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhixingplan.top/gtvggiglue.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ppjwa.cn/gtzotxlzsk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jinghuilouyu.cn/gtjblaoxur.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.wangdashe.top/gtywlratze.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jqgufenzy.top/gtgxwqcgxd.html

[J09] 时区处理
来源：http://hz.hongshengwenyu.top/gtkdyvcmsg.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zycfv.cn/gtvbjatbcx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zycfv.cn/gtdchgwqcy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ehwqpu.com/gtsmhzlzla.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sufxvd.cn/gtozmhasqa.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gaohongyu789.top/gtzswupcdf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.iojbl.cn/gtvvpnsymd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yuxming.cn/gtdphshxfs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ywan-chungtsiang.top/gteynnfwfb.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhijiandao.cn/gtvaswwqbn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhijiandao.cn/gttitrqykx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ehwqpu.com/gthwyjvrmu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cdnleiting.top/gtonzhxwbg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hammf.cn/gtsleslkvj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.aibaodan.cn/gtghjvitqc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhengqikj.top/gttrjzuefe.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yj20258888.top/gtqqpihclw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.0kj1m.cn/gtjbnbcobx.html

================================================================================
来源：http://hz.jyoumei.cn/gtwqlwybgl.html

K. JSON 与序列化
来源：http://hz.cdnleiting.top/gtuglgbaad.html

================================================================================
来源：http://hz.zdqjudy.top/gtbyckqvze.html

[K01] 对象转 JSON 字符串
来源：http://hz.hnqzz.top/gtypewvrfc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.gaohongyu789.top/gtydtuborq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.chenzaomai.com/gtweeywgdj.html

JS:   JSON.stringify(obj)
来源：http://hz.redwolf501.top/gttbaopjfs.html

TS:   JSON.stringify(obj)
来源：http://hz.yonumen.top/gtgfqdoyhp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ehwqpu.com/gtxtpqmyfd.html

Go:   json.Marshal(obj)
来源：http://hz.xziqi.cn/gtmeljzwjn.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhengqikj.top/gtcsccbjqw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hfpthk.cn/gtbgccqwpw.html

[K02] JSON 字符串转对象
来源：http://hz.shanyushiyangtech.top/gtkzpfnlvl.html

Py:   json.loads(s)
来源：http://hz.zhoulong.xyz/gtwzofmmuk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xziqi.cn/gteocfykhf.html

JS:   JSON.parse(s)
来源：http://hz.haohaochexian.top/gtwhzqjqah.html

TS:   JSON.parse(s)
来源：http://hz.sysykeji.top/gtaifbltdi.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhoulong.xyz/gtzrfdrvwv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinqigufen.top/gtsqhnexyx.html

Ruby: JSON.parse(s)
来源：http://hz.zhongyouzk.top/gtcffunjut.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hongshengwenyu.top/gtflzznxyj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zycfv.cn/gtpmwclkbr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hywenlv.cn/gtxcpxhsya.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.haohaochexian.top/gtizyhfjpm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shuidangran.top/gtgelgjzle.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangtech.top/gtgkqpjaru.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xziqi.cn/gtezvgzwsh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ehwqpu.com/gtgsmxximi.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.smart0.xyz/gtwfugnlyr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinghuilouyu.cn/gtaegytqwb.html

[K04] 读取 JSON 文件
来源：http://hz.jinqigufen.top/gtqwvmpovl.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinyuanbaomall.cn/gtwmipmlsn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.bjfxy.top/gtoibleqsv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xingfuxueyuan.xyz/gtspwrjcko.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ppjwa.cn/gtxteehfnw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinghuilouyu.cn/gttnznjmoq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.mhx1999.top/gtwkfmtyyx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zdqjudy.top/gttzglzagy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.nanxinkj.top/gtcfxnnkpw.html

[K05] 深拷贝对象
来源：http://hz.svipenyu.cn/gtyjjkcyru.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhaomingkeji.xyz/gtzptygshe.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ydzc1.top/gtywhzomdi.html

JS:   structuredClone(obj)
来源：http://hz.jinqigfzy.top/gtivihrhuv.html

TS:   structuredClone(obj)
来源：http://hz.svipenyu.cn/gthhpwzkgx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.yj20258888.top/gtwveuwhfp.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ppjwa.cn/gtocrcvnas.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.birdmap.top/gtcgvomqwi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.vqdsnc.cn/gtesjuzcmr.html

[K06] 解析 URL 查询串
来源：http://hz.nwbrower.top/gtbdxeaekv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ybcxt.top/gtgjogjkjf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhiwuduotai.top/gtmcclzygh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cqqwz.cn/gtejzvtwzd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.haohaochexian.top/gtkeklegkd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.gotoacloud.top/gtgicjdsvb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.wangshuangyany.cn/gtuyreunsh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.sysykeji.top/gtqhdrgogs.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jyoumei.cn/gtbyumnlsg.html

[K07] 进制转换
来源：http://hz.yuanzhike.top/gtgnbrggwo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.haohaochexian.top/gthkntcocy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hammf.cn/gtdnxotgcb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.nanxuanxn.top/gtctmwipvg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jiagoushi.top/gtryhsdvmj.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhongyouzk.top/gtmeiltpuu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.guannengcc.top/gtyrnvymrx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.chenlongwang.top/gtbjoypppi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.redwolf501.top/gtpgjuwzkb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.shanyushiyangtech.top/gtkuevtley.html

Py:   pickle.dumps(obj)
来源：http://hz.fzhhl.top/gtnlevqbxg.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.kuanghao11.cn/gtivsqicub.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.meibo888.top/gteqvowstd.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.sweek.top/gtwncqqmau.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.9152youxi.cn/gtgdzhnhll.html

Go:   encoding/gob
来源：http://hz.dashuyun.cn/gtavefdydv.html

Ruby: Marshal.dump(obj)
来源：http://hz.xuetiantiany.cn/gtuttsaplf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yj202588.top/gtuoagnazg.html

================================================================================
来源：http://hz.chenzaomai.com/gteeibkgag.html

L. 网络请求
来源：http://hz.hywenlv.cn/gtsgsiqrix.html

================================================================================
来源：http://hz.bjfxy.top/gtkjtbhcwq.html

[L01] 发送 GET 请求
来源：http://hz.hammf.cn/gtgcqwrhqe.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xingfuxueyuan.xyz/gtmzrhvnte.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.c1oappe.top/gtavrpenqu.html

JS:   await fetch(url)
来源：http://hz.yj20258888.top/gtrgbowfsc.html

TS:   await fetch(url)
来源：http://hz.aibaodan.cn/gtkttoltsk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.sweek.top/gtzmejlnkb.html


<!-- 参考信息 -->