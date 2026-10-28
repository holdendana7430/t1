代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.meibo888.top/gtxoxywgfl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cqqwz.cn/gtxpinghid.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ivvv.top/gtmylvolxn.html

C#:   obj?.A?.B ?? default
来源：http://hz.chenjidiqi.icu/gtiktsvpxp.html

[H07] 断言
来源：http://hz.jinyuanbaomall.cn/gtcgyncsnd.html

Py:   assert x > 0, "必须为正"
来源：http://hz.tian-w.cn/gttujzhwph.html

PHP:  assert($x > 0);
来源：http://hz.yj202588.top/gtxiegpdkx.html

JS:   console.assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtsjhglnqw.html

TS:   console.assert(x > 0);
来源：http://hz.jianghu66.top/gthllrwsdj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.meibo888.top/gtcidupdsj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cheryme.top/gtvmqajlgg.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tanke756.top/gtyestwuap.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtngcmudwb.html

[H08] 获取错误信息与堆栈
来源：http://hz.nwbrower.top/gteklrkpdy.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jlsjyb.cn/gtqtowjhej.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hammf.cn/gtawofnwxt.html

JS:   e.message;  e.stack
来源：http://hz.yj20258.top/gtcvthipmv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jqgufenzy.top/gthytumtxn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jyoumei.cn/gtnzphttmx.html

Go:   err.Error()
来源：http://hz.xingfuxueyuan.xyz/gttywgagqf.html

Ruby: e.message;  e.backtrace
来源：http://hz.nanxinkj.top/gtswhpbimb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hysaishi.cn/gturtynbum.html

[H09] 带错误码的异常
来源：http://hz.tian-w.cn/gtgquvovdm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jianghu66.top/gtfbqazcjw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.chenlongwang.top/gtyeerhdly.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.haohaochexian.top/gtsesurkar.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.feifeiyinyue.top/gtquvizwzy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hnqzz.top/gtjthjkewf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.wangshuangyany.cn/gtdbjoqdoc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.snrcjt.cn/gtlzyryfct.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhixingplan.top/gtjmaxhldu.html

[H10] 资源自动释放
来源：http://hz.9152youxi.cn/gtyqongheo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xuanzx.com/gtgrlhpuow.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cheryme.top/gtsyhsxolp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxuanxn.top/gticsrwdjl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yvedp.cn/gttzwxesod.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sysykeji.top/gtzbssfijr.html

Go:   defer f.Close()
来源：http://hz.ivvv.top/gtmizbyvqt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.316326.xyz/gtohcqnmpe.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ivvv.top/gtpaysgxiw.html

================================================================================
来源：http://hz.yueranfly.top/gtxnhtaomu.html

I. 正则表达式
来源：http://hz.gaohongyu789.top/gtlrjaqkde.html

================================================================================
来源：http://hz.ydjk.org.cn/gteezyavmn.html

[I01] 判断是否匹配
来源：http://hz.jiagoushi.top/gtqijmyegh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.sweek.top/gtkmwbpjsb.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinqigfzy.top/gtonelgqkk.html

JS:   /\d+/.test(s)
来源：http://hz.yueranfly.top/gtbtltbwsc.html

TS:   /\d+/.test(s)
来源：http://hz.zdqjudy.top/gtxwborbxh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gogol.net.cn/gtxaqdopkm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yangfankeji.com/gtsbrsvqrf.html

Ruby: s.match?(/\d+/)
来源：http://hz.jqgfzy.top/gtqfvqzubn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cucudq.cn/gtsddvesgm.html

[I02] 提取所有匹配
来源：http://hz.kuanghao11.cn/gtokvbymgz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hnxiangtu.top/gtkvirsubv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.gogol.net.cn/gtzvennggm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.quarkkingdee.top/gtrjvbsysh.html

TS:   s.match(/\d+/g)
来源：http://hz.cucudq.cn/gtmbyjrvii.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sysykeji.top/gtgzhstbhi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shuidangran.top/gtjwzzsrel.html

Ruby: s.scan(/\d+/)
来源：http://hz.smart0.xyz/gtroauzcel.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shanyushiyangkeji.top/gtkjpxxoaq.html

[I03] 提取捕获分组
来源：http://hz.ybcxt.top/gtgziurokb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.feifeiyinyue.top/gtzafityiu.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.tian-w.cn/gtiokhcdjl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.tian-w.cn/gtqghinrkg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jiagoushi.top/gtezshtzaq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yj202588.top/gtcbidxgrs.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.316326.xyz/gtguoxzhvi.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhaomingkeji.xyz/gttdwvarwf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.chenzaomai.com/gtyssztkyy.html

[I04] 正则替换
来源：http://hz.zhijiandao.cn/gtlldgjvwr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.9152youxi.cn/gtyqvbbqox.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.dianchejie.cn/gtnokbntyl.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.chenzaomai.com/gtecpqbtyj.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.dashuyun.cn/gthblfxbcd.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.vqdsnc.cn/gticorjzys.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hnqzz.top/gtzfnemeee.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ywan-chungtsiang.top/gtzfolttet.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jqgufenzy.top/gtjjgipjim.html

[I05] 按正则拆分
来源：http://hz.pycfn.com/gtpeenflab.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hnxiangtu.top/gtpaveyres.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.quarkkingdee.top/gtwmkuvfgt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ydzc1.top/gtbaglrrpa.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.9152youxi.cn/gtxovvanij.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zycfv.cn/gtwruzxxvo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xingfuxueyuan.xyz/gtrikkcvdv.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hfpthk.cn/gtadhqfeqn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jqgfzy.top/gtuoufqdke.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hnxiangtu.top/gtvqcxyttb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sysykeji.top/gtlxzkusin.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.havefunace.top/gtrrwggndp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ehwqpu.com/gtobptvnwg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnqzz.top/gthpwkkewz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.haohaochexian.top/gtwjfvzskd.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hywenlv.cn/gtlwmslivz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.feifeiyinyue.top/gtwrwtlzxo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.c1oappe.top/gtxcbhydmr.html

[I07] 忽略大小写与多行模式
来源：http://hz.yueranfly.top/gtmpgfagnn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yj20258888.top/gtyeahxcad.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.dianchejie.cn/gtahqjtokx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.quarkkingdee.top/gtcuxinrnt.html

TS:   /error/gim
来源：http://hz.nanxinkj.top/gtbaxkaocn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shanyushiyangkeji.top/gtlwojjpyz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.redwolf501.top/gtnifmhltn.html

Ruby: s.scan(/error/i)
来源：http://hz.hnxiangtu.top/gttvhtwoyg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.redwolf501.top/gtniwqfjep.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yj20258888.top/gtzbshowvh.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.nanxinkj.top/gtaviizdzv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cdnleiting.top/gtimjbzfrh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.kuanghao11.cn/gtwizgymqg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.andypj.xyz/gtrubjtnbi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xuetiantiany.cn/gtdugfdscf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinyuanbaomall.cn/gtprhmpqbg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.mhx1999.top/gtelduzsrq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.wangdashe.top/gtzduqasvy.html

================================================================================
来源：http://hz.smart0.xyz/gtukzxzzab.html

J. 日期与时间
来源：http://hz.316326.xyz/gtreviwpwd.html

================================================================================
来源：http://hz.52xcode.cn/gtglkobmvk.html

[J01] 获取当前时间
来源：http://hz.zhongyouzk.top/gtyfrylyia.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.dashuyun.cn/gtljmxfnzx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jqgufenzy.top/gttatkqgpt.html

JS:   new Date();  Date.now()
来源：http://hz.guowangkeji.top/gtplceioof.html

TS:   new Date();  Date.now()
来源：http://hz.yongpay.top/gtkqfripyt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cqqwz.cn/gtolktcelx.html

Go:   time.Now()
来源：http://hz.yueranfly.top/gtefhwoqlx.html

Ruby: Time.now
来源：http://hz.snrcjt.cn/gttasjfdhg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.iojbl.cn/gtmhhlpucb.html

[J02] 格式化输出
来源：http://hz.svipenyu.cn/gtzhdqmkro.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yvedp.cn/gtbzzupmcm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.wangshuangyany.cn/gthjcxmgoa.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shangyingyoupin.top/gttrgeivhe.html

TS:   d.toISOString()
来源：http://hz.jinghuilouyu.cn/gtgmgsnxad.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xinyue.icu/gtzoriypnp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.aizwys.cn/gtazvmxndv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yanxiufei.cn/gtzmxttful.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinghuilouyu.cn/gtsprplvff.html

[J03] 字符串解析为日期
来源：http://hz.zhengqikj.top/gtyltpiwpf.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hnxiangtu.top/gthvgraunm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.52xcode.cn/gtosvmjqhb.html

JS:   new Date("2024-01-02")
来源：http://hz.tian-w.cn/gtlkttqgch.html

TS:   new Date("2024-01-02")
来源：http://hz.vqdsnc.cn/gthfygnvch.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jinqigfzy.top/gtgdbtpaql.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.wangdashe.top/gtnizdyvlk.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yuanzhike.top/gtdutzmllp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sweek.top/gtalwhiedk.html

[J04] 时间戳与日期互转
来源：http://hz.tian-w.cn/gtdwcqqpiq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.nanxuanxn.top/gtrcmmjlwg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.kuanghao11.cn/gtlmkutfxq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhengqikj.top/gtglzvhail.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ybcxt.top/gtcsnfffab.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhaomingkeji.xyz/gtsfgvuvrf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yj202588.top/gtuflsuyob.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.tianlin.xyz/gtvaylqgqe.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.daxiang520.top/gtzfhavfse.html

[J05] 时间加减（加 7 天）
来源：http://hz.yj20258888.top/gtpytfchwh.html

Py:   now + timedelta(days=7)
来源：http://hz.jinyuanbaomall.cn/gtvgpgcvkr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shangyingyoupin.top/gthcvvvnxw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.quarkkingdee.top/gtirnarjnb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.kuanghao11.cn/gtglkmqfxf.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.tian-w.cn/gttaiecdct.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xinyue.icu/gtuppwiwdd.html

Ruby: Time.now + 7 * 86400
来源：http://hz.9152youxi.cn/gtauhsdnlu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ydzc1.top/gtbfxvdnjp.html

[J06] 计算两时间之差
来源：http://hz.hywenlv.cn/gttbvrjbza.html

Py:   (end - start).total_seconds()
来源：http://hz.jinyuanbaomall.cn/gtdmcpgysm.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhijiandao.cn/gtsxacmqpe.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ydjk.org.cn/gtafbxirws.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.andypj.xyz/gtthkplmqu.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.chenjidiqi.icu/gtawkjuwjo.html

Go:   end.Sub(start).Hours()
来源：http://hz.c1oappe.top/gtmbhrowhg.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hongshengwenyu.top/gtustpokyf.html

C#:   (end - start).TotalSeconds
来源：http://hz.yongpay.top/gtewtwdrsj.html

[J07] 比较两个日期
来源：http://hz.zhixingplan.top/gtksuztzag.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.haohaochexian.top/gtlnnqbejn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.vqdsnc.cn/gtkgbbqsdt.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xuetiantiany.cn/gtytpenybr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sweek.top/gtpqbseukq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nanxinkj.top/gtbkmxbfyr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhongyouzk.top/gttzbecsbh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hfpthk.cn/gtrsjmrjts.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gotoacloud.top/gtszanacph.html

[J08] 提取年月日与星期
来源：http://hz.jqgfzy.top/gtwiwcmjmm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinghuilouyu.cn/gtjfqjjcuj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sxryk.cn/gtdkoosdcb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.pycfn.com/gtekltfurm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shanyushiyangkeji.top/gtyrpejjcb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yangfankeji.com/gtvrhsfzua.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shzxlz.cn/gtmhbqsobh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.quarkkingdee.top/gtspzemvry.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zdqjudy.top/gtvqejbvok.html

[J09] 时区处理
来源：http://hz.guannengcc.top/gtkxlvmfzt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.tian-w.cn/gtnanuilxt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.sweek.top/gtycdxkzpe.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shuidangran.top/gtosmguibd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxuanxn.top/gtujanufay.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hnqzz.top/gtyexitghc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.iojbl.cn/gtizrieiaw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hnqzz.top/gtlgvwvtqq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.c1oappe.top/gtrplecqav.html

[J10] 取今天 / 本月第一天
来源：http://hz.hnxiangtu.top/gtwaesxpje.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj20258.top/gtncfqwatx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yj202588.top/gttbzmvggf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.sweek.top/gtpkptfbob.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhijiandao.cn/gtxxnffpka.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.52xcode.cn/gtbfijhhnl.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinqigfzy.top/gtzklzyvqv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinqigfzy.top/gtgdjfpgrz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.wangdashe.top/gtigcbkcsy.html

================================================================================
来源：http://hz.gogol.net.cn/gtzfkojval.html

K. JSON 与序列化
来源：http://hz.jinyuanbaomall.cn/gtpwgvnrog.html

================================================================================
来源：http://hz.gotoacloud.top/gtsizbaesm.html

[K01] 对象转 JSON 字符串
来源：http://hz.hammf.cn/gtjgamvtvq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.fengsongda.top/gtflyzpmar.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yanxiufei.cn/gtoejsyydm.html

JS:   JSON.stringify(obj)
来源：http://hz.nwbrower.top/gtuffcbpdi.html

TS:   JSON.stringify(obj)
来源：http://hz.birdmap.top/gttxrrptxq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jlsjyb.cn/gtljkmpqkl.html

Go:   json.Marshal(obj)
来源：http://hz.yj20258888.top/gtxzcbxqrz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.kuanghao11.cn/gtfutcihml.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.gzhubu.top/gtunhykkok.html

[K02] JSON 字符串转对象
来源：http://hz.birdmap.top/gtkqnskviq.html

Py:   json.loads(s)
来源：http://hz.9152youxi.cn/gtbzqwljgb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yuanzhike.top/gtrrfskmnh.html

JS:   JSON.parse(s)
来源：http://hz.yongpay.top/gthefpkkiv.html

TS:   JSON.parse(s)
来源：http://hz.sweek.top/gtrnmquzvq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhengqikj.top/gtkmrgjaez.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yvedp.cn/gtwafoyjjf.html

Ruby: JSON.parse(s)
来源：http://hz.zycfv.cn/gttsjzymyj.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhoulong.xyz/gtxwhujlen.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ehwqpu.com/gthngzoonj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yj202588.top/gtgcfgnoib.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jqgfzy.top/gtkusbiwkw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.sweek.top/gtashnvvcr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.aizwys.cn/gtksdcsfjz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinqigfzy.top/gthftyychc.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhengqikj.top/gtbwlbsnqw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hammf.cn/gtjqyjafpz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.nwbrower.top/gtlkuihjbo.html

[K04] 读取 JSON 文件
来源：http://hz.aizwys.cn/gtuwdpequh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hnxiangtu.top/gthinswyek.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xinyue.icu/gtmongfshq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj202588.top/gtdjmuqknz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhixingplan.top/gtnsjhblan.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.hfpthk.cn/gtiwmaeeqt.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.andypj.xyz/gtkagihmkj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.0kj1m.cn/gtqqkauyil.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhoulong.xyz/gtpaozmcot.html

[K05] 深拷贝对象
来源：http://hz.zhixingplan.top/gtsjhewora.html

Py:   copy.deepcopy(obj)
来源：http://hz.9152youxi.cn/gtwervjvhz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhaomingkeji.xyz/gtkqqoaazp.html

JS:   structuredClone(obj)
来源：http://hz.fengsongda.top/gtmqstreol.html

TS:   structuredClone(obj)
来源：http://hz.aizwys.cn/gtabqwnsho.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gaohongyu789.top/gtsidhgcoo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zdqjudy.top/gtpybroeai.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jinqigfzy.top/gthxnzxgaa.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.pengpengdd.cyou/gtnsysoneq.html

[K06] 解析 URL 查询串
来源：http://hz.xuetiantiany.cn/gtsvrsqmug.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cheryme.top/gtumfqtmvz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.gotoacloud.top/gtnljbmnqq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yvedp.cn/gtgirpjckv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fengsongda.top/gtoesimvae.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.sufxvd.cn/gtbjqkyuwb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.chenjidiqi.icu/gtvexmlmft.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yj20258888.top/gtqeyzbwhq.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yvedp.cn/gtxswtyaao.html

[K07] 进制转换
来源：http://hz.daxiang520.top/gtrvdlumxm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.wangdashe.top/gthmyclkpc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.316326.xyz/gtfmkbwopc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.pycfn.com/gtvoxfbxya.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gaohongyu789.top/gtomjeeazt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yanxiufei.cn/gtgowfggch.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hongshengwenyu.top/gtalwulize.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.nwbrower.top/gtiolnlhon.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhongyouzk.top/gtjqqbjdtl.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jqgfzy.top/gtgdnksxml.html

Py:   pickle.dumps(obj)
来源：http://hz.ydzc1.top/gtqwemxekh.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.52xcode.cn/gtlldttven.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.guowangkeji.top/gtyzdaxdah.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhengqikj.top/gtahjivkfd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hammf.cn/gtemiaesmx.html

Go:   encoding/gob
来源：http://hz.cheryme.top/gtakysfxtj.html

Ruby: Marshal.dump(obj)
来源：http://hz.fzhhl.top/gtanultnpd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.daria6918.cn/gtoveiemer.html

================================================================================
来源：http://hz.zhijiandao.cn/gtvuvajvnv.html

L. 网络请求
来源：http://hz.feifeiyinyue.top/gtcsgjwtqu.html

================================================================================
来源：http://hz.birdmap.top/gtorifjszd.html

[L01] 发送 GET 请求
来源：http://hz.hfpthk.cn/gtbzaydyqk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.iojbl.cn/gtlnbqyojx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.gotoacloud.top/gteufurelo.html

JS:   await fetch(url)
来源：http://hz.52xcode.cn/gteqvjiven.html

TS:   await fetch(url)
来源：http://hz.jinghuilouyu.cn/gtgqkkgwxr.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.xuanzx.com/gtwncrejyp.html

Go:   resp, err := http.Get(url)
来源：http://hz.fzhhl.top/gtsgmhygce.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.yuxming.cn/gtvghqpvjg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.xuanzx.com/gtwslfcbkw.html

[L02] 发送 POST JSON
来源：http://hz.nanxinkj.top/gthtnuiaku.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.nwbrower.top/gtmbwuyayc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.fengsongda.top/gtucxegmwa.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.bjfxy.top/gtieywryah.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.ybcxt.top/gtinshdxwx.html


<!-- 参考信息 -->