代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhengqikj.top/gtepkhxlit.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cdnleiting.top/gtzhmggbxe.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yuanzhike.top/gtysglbpim.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.aizwys.cn/gtacyqpidm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhongyouzk.top/gtevlbkhst.html

Ruby: rescue ArgumentError => e
来源：http://hz.yonumen.top/gtyricjqph.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.meibo888.top/gtdcqntbfb.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yj20258888.top/gtqwnjqfju.html

Py:   value = d.get("k") or default
来源：http://hz.yj20258888.top/gthvwvkykl.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ybcxt.top/gtyechziug.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258.top/gtrenzomii.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhaomingkeji.xyz/gtklrytrav.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zdqjudy.top/gtknsewfhh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nanxinkj.top/gtynuapgtz.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhengqikj.top/gtoxgwtiln.html

C#:   obj?.A?.B ?? default
来源：http://hz.dianchejie.cn/gttjvgxyju.html

[H07] 断言
来源：http://hz.nanxuanxn.top/gtpcbylnbw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.chenlongwang.top/gtaywopmqr.html

PHP:  assert($x > 0);
来源：http://hz.zdqjudy.top/gtnnohwxcx.html

JS:   console.assert(x > 0);
来源：http://hz.ydzc1.top/gtqgsloqzk.html

TS:   console.assert(x > 0);
来源：http://hz.smart0.xyz/gtpyudtuvl.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhixingplan.top/gtrhoiyavh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.aizwys.cn/gtolquljkv.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yueranfly.top/gtlqummgrs.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jlsjyb.cn/gtmhkauwpq.html

[H08] 获取错误信息与堆栈
来源：http://hz.chenjidiqi.icu/gtnxnrocok.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cqqwz.cn/gtkjeeqahv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yj20258.top/gtftqlwmnl.html

JS:   e.message;  e.stack
来源：http://hz.daria6918.cn/gtpwmwcjbb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shuidangran.top/gthoqmlxcu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.svipenyu.cn/gtsiafjxqz.html

Go:   err.Error()
来源：http://hz.hysaishi.cn/gtgdqjokff.html

Ruby: e.message;  e.backtrace
来源：http://hz.hammf.cn/gttamttlcf.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhengqikj.top/gtkirdrxzl.html

[H09] 带错误码的异常
来源：http://hz.wangdashe.top/gtzobsautc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jinqigfzy.top/gtqlakfetw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.snrcjt.cn/gtqxxnmevv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shzxlz.cn/gtkiuwgdhe.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yj20258.top/gtlnbdwehe.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ywan-chungtsiang.top/gtxfmpsfbv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.chenzaomai.com/gtwuhfhfrz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.chenjidiqi.icu/gtgpmnowmk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.316326.xyz/gtluuultpr.html

[H10] 资源自动释放
来源：http://hz.ydzc1.top/gtqotcspuk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shangyingyoupin.top/gttoxwlhos.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shzxlz.cn/gtfqrynocw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cdnleiting.top/gtltlsbzbl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.redwolf501.top/gtnglnyqxd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ydzc1.top/gtnkjnasul.html

Go:   defer f.Close()
来源：http://hz.xingfuxueyuan.xyz/gtfzbtmyqy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xziqi.cn/gtfcqcfbdi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.vqdsnc.cn/gtuzeedpsb.html

================================================================================
来源：http://hz.nwbrower.top/gtucksvnfy.html

I. 正则表达式
来源：http://hz.yvedp.cn/gtxtcwacbt.html

================================================================================
来源：http://hz.birdmap.top/gtygzqckhf.html

[I01] 判断是否匹配
来源：http://hz.zhixingplan.top/gthgllixtf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xziqi.cn/gtwcqxxvvq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sysykeji.top/gtujwjturv.html

JS:   /\d+/.test(s)
来源：http://hz.shzxlz.cn/gtdvotcogx.html

TS:   /\d+/.test(s)
来源：http://hz.jinqigfzy.top/gtwcaviltv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhengqikj.top/gtddvkgesp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.tianlin.xyz/gtpnphhfla.html

Ruby: s.match?(/\d+/)
来源：http://hz.guowangkeji.top/gtgokahwoh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.fzhhl.top/gthqdzsrtt.html

[I02] 提取所有匹配
来源：http://hz.pengpengdd.cyou/gtkuvhcwow.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yangfankeji.com/gtphelwjos.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jianghu66.top/gtnkyhmkjv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cucudq.cn/gtnuezagti.html

TS:   s.match(/\d+/g)
来源：http://hz.zhaomingkeji.xyz/gtahgycrvg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.havefunace.top/gtvcowwmyk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hnxiangtu.top/gtcmvjjwlo.html

Ruby: s.scan(/\d+/)
来源：http://hz.kuanghao11.cn/gtkaryhfep.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jlsjyb.cn/gtikamwgcz.html

[I03] 提取捕获分组
来源：http://hz.shanyushiyangkeji.top/gtsbcxuuvc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zycfv.cn/gtxmeqligy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gaohongyu789.top/gtfluztafn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cashguo.top/gtirsuropm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yueranfly.top/gtqktqtdij.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cucudq.cn/gtanlfkmuo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.wangdashe.top/gtfjrpibgz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.wangshuangyany.cn/gtdisthmja.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.snrcjt.cn/gtsorgjbbb.html

[I04] 正则替换
来源：http://hz.guowangkeji.top/gtfchczgqq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jqgufenzy.top/gteyjgmoef.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sufxvd.cn/gtwqmppukt.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.aibaodan.cn/gtybipzijs.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xuanzx.com/gtefwzvuog.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.chenjidiqi.icu/gtwupuplxq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.c1oappe.top/gtylyxhpkb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zycfv.cn/gtafflskgi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hammf.cn/gtsgczcvxe.html

[I05] 按正则拆分
来源：http://hz.sweek.top/gtuwqzoncr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.aizwys.cn/gtkaafbgsa.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.fengsongda.top/gtotempwly.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhixingplan.top/gtxvpdhdga.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gtrwhwkkgk.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinyuanbaomall.cn/gtuzegvqka.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jinqigfzy.top/gtyrxzdaob.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yongpay.top/gtzbihwdpi.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.nanxuanxn.top/gtdbbjmwxn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.tanke756.top/gtdtgzewus.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhiwuduotai.top/gtjwnfjazj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jqgfzy.top/gttiqewjvi.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ydjk.org.cn/gtlmhjrice.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.vqdsnc.cn/gtujzdbrjb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xuanzx.com/gtyenawysb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.kuanghao11.cn/gtlbogibpk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.feifeiyinyue.top/gtdutespjn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.chenzaomai.com/gtinaidfsk.html

[I07] 忽略大小写与多行模式
来源：http://hz.9152youxi.cn/gtkxbgbhem.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.aizwys.cn/gtkkxlcyjb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.wangshuangyany.cn/gtffkwlmyo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.pengpengdd.cyou/gtukhwfqaz.html

TS:   /error/gim
来源：http://hz.iojbl.cn/gtaubstkro.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cucudq.cn/gtfqeewuqq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.dashuyun.cn/gtsvqzqqrm.html

Ruby: s.scan(/error/i)
来源：http://hz.yj202588.top/gtkvqmizrh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.aibaodan.cn/gtdmktjorz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jlsjyb.cn/gtcrwehpvz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ppjwa.cn/gtsygkqgtq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yuanzhike.top/gtmdyvxluy.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jyoumei.cn/gtleamuona.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.dianchejie.cn/gtrwwdjqmn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sxryk.cn/gtnjdzcgdc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.316326.xyz/gtkepkpedp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.kuanghao11.cn/gtjsxlsoiv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.tian-w.cn/gtcznfhzij.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtdfjlpcvg.html

J. 日期与时间
来源：http://hz.guannengcc.top/gtfwkjnehj.html

================================================================================
来源：http://hz.mhx1999.top/gtkinsrwbk.html

[J01] 获取当前时间
来源：http://hz.zhiwuduotai.top/gtposbhyyh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.gotoacloud.top/gtlqsjmzmc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yj20258.top/gtshzjunio.html

JS:   new Date();  Date.now()
来源：http://hz.aibaodan.cn/gtqsaeybhs.html

TS:   new Date();  Date.now()
来源：http://hz.jinqigfzy.top/gtdpnlxfnr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ywan-chungtsiang.top/gtcksdjaqt.html

Go:   time.Now()
来源：http://hz.cheryme.top/gtgjuitqwu.html

Ruby: Time.now
来源：http://hz.xziqi.cn/gtddizadyj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cucudq.cn/gtafvbbtpz.html

[J02] 格式化输出
来源：http://hz.redwolf501.top/gtntdepnkl.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.redwolf501.top/gtqywmakks.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.kuanghao11.cn/gteqpryhsg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhijiandao.cn/gtuybwsmdh.html

TS:   d.toISOString()
来源：http://hz.zhongyouzk.top/gtxtahzlfc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hammf.cn/gtaiplkhym.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.fengsongda.top/gtsjrbonrs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.daxiang520.top/gtbtfbyvol.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hnqzz.top/gtfgbijpvv.html

[J03] 字符串解析为日期
来源：http://hz.hongshengwenyu.top/gtqzebegfh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.dianchejie.cn/gtlhljqagy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sxryk.cn/gtvqlvckpt.html

JS:   new Date("2024-01-02")
来源：http://hz.iojbl.cn/gtstoaxowz.html

TS:   new Date("2024-01-02")
来源：http://hz.cheryme.top/gtpdvyxrxx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sufxvd.cn/gtwroirfyw.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.daxiang520.top/gtfxjpycdz.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gotoacloud.top/gtszyjbric.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.kuanghao11.cn/gtdflerdvp.html

[J04] 时间戳与日期互转
来源：http://hz.zhaomingkeji.xyz/gtuhaltnsh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.sysykeji.top/gtkpnzhjcr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yvedp.cn/gtpxswbvwq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinqigfzy.top/gtwcnseabe.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jyoumei.cn/gtiqcilaww.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.52xcode.cn/gtlsxhltyw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.316326.xyz/gtdgyxeghe.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.tian-w.cn/gtldvroipu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yanxiufei.cn/gtfamtuqzt.html

[J05] 时间加减（加 7 天）
来源：http://hz.chenlongwang.top/gtpbkdfamw.html

Py:   now + timedelta(days=7)
来源：http://hz.hongshengwenyu.top/gtnmlkqiej.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.pengpengdd.cyou/gtxcwqwcji.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cdnleiting.top/gtzgmnxlbv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinyuanbaomall.cn/gtyilluaok.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhijiandao.cn/gtyvbnviit.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yanxiufei.cn/gtorrsdgfv.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhixingplan.top/gtrevtjrkg.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ppjwa.cn/gtnykmbfqv.html

[J06] 计算两时间之差
来源：http://hz.hammf.cn/gtcojjxfqm.html

Py:   (end - start).total_seconds()
来源：http://hz.yj20258.top/gtjmuamoqb.html

PHP:  $end->diff($start)->days;
来源：http://hz.316326.xyz/gtexlgldnu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.wangshuangyany.cn/gtpsoraxtt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yangfankeji.com/gtprfzmjpv.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jiagoushi.top/gtzfkhhcvn.html

Go:   end.Sub(start).Hours()
来源：http://hz.jqgufenzy.top/gtjttrjihr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hysaishi.cn/gtwxrbedqi.html

C#:   (end - start).TotalSeconds
来源：http://hz.feifeiyinyue.top/gtcrzwmjpa.html

[J07] 比较两个日期
来源：http://hz.hfpthk.cn/gtlceozmjm.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gttiwgnsdw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shuidangran.top/gtdeqqexyc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gotoacloud.top/gtiwxmpgyt.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.aizwys.cn/gtmkezsrdp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hnqzz.top/gtgbicguag.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.guannengcc.top/gtugksjtkz.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cucudq.cn/gtqchhjeon.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yongpay.top/gtxoducjxx.html

[J08] 提取年月日与星期
来源：http://hz.jinghuilouyu.cn/gtbwwbflpi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cheryme.top/gtzqtvewqp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xuetiantiany.cn/gtggverxfu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.guannengcc.top/gtrmwfituz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hongshengwenyu.top/gtfprcraib.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.redwolf501.top/gtogxptltn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yanxiufei.cn/gtgdmuhrho.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.316326.xyz/gtbxzsftyn.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinqigfzy.top/gtxvhtzwyb.html

[J09] 时区处理
来源：http://hz.daxiang520.top/gttwszqxxv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhijiandao.cn/gtikdifscq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenzaomai.com/gtjfwfxpzh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnqzz.top/gtsmceohki.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxuanxn.top/gtxtikmpyx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yuanzhike.top/gtzusstumd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shanyushiyangtech.top/gtbguuyrfc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.meibo888.top/gtfibwqhnw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jiagoushi.top/gtbtoyehxl.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhaomingkeji.xyz/gtpydrewjc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jqgufenzy.top/gtprfiftdq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.meibo888.top/gtxpaoxoen.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yonumen.top/gttfgwhxmn.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.daria6918.cn/gtvbrtfbdo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.haohaochexian.top/gtsioeiexd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jqgufenzy.top/gtwduuyofd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hammf.cn/gtblbyihnm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cucudq.cn/gthnljxrqh.html

================================================================================
来源：http://hz.ydjk.org.cn/gtkvzztzxo.html

K. JSON 与序列化
来源：http://hz.gotoacloud.top/gtnpatjxbd.html

================================================================================
来源：http://hz.andypj.xyz/gtgtcsvuvg.html

[K01] 对象转 JSON 字符串
来源：http://hz.jqgufenzy.top/gthficegtm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ydjk.org.cn/gttmjcxrwt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cqqwz.cn/gtkvwrqujg.html

JS:   JSON.stringify(obj)
来源：http://hz.cheryme.top/gtnjuxgxqc.html

TS:   JSON.stringify(obj)
来源：http://hz.aizwys.cn/gtymoauaax.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.snrcjt.cn/gtptxbhvbc.html

Go:   json.Marshal(obj)
来源：http://hz.guannengcc.top/gttskuprdr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.nwbrower.top/gtjombanex.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.redwolf501.top/gtuqmvliwq.html

[K02] JSON 字符串转对象
来源：http://hz.yonumen.top/gtypmglncu.html

Py:   json.loads(s)
来源：http://hz.wangdashe.top/gtrerpjocv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hammf.cn/gtitmpddvd.html

JS:   JSON.parse(s)
来源：http://hz.hywenlv.cn/gternplqnm.html

TS:   JSON.parse(s)
来源：http://hz.yuanzhike.top/gtplvcpwqm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.0kj1m.cn/gtbqznccec.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ywan-chungtsiang.top/gtzllmwnsi.html

Ruby: JSON.parse(s)
来源：http://hz.mhx1999.top/gteoamszsu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.wangdashe.top/gtlausnlxi.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zdqjudy.top/gteirqiuqq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.snrcjt.cn/gtocbmryti.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.havefunace.top/gtfkiihmiw.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigfzy.top/gtikbbppmg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yonumen.top/gtpvbeivuv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.kuanghao11.cn/gtepwqjthi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhixingplan.top/gtbgxhjese.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ybcxt.top/gtgckstyxd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hammf.cn/gtymglsssr.html

[K04] 读取 JSON 文件
来源：http://hz.c1oappe.top/gtxmywewna.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yueranfly.top/gtmgjoyoyh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.feifeiyinyue.top/gtbxmpqcuc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jyoumei.cn/gtcmzllbfk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xingfuxueyuan.xyz/gtkcjouqcu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.svipenyu.cn/gtsbesopgj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.316326.xyz/gtbinaoprm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.mhx1999.top/gtdmlyhhcw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yj20258888.top/gttykwlhfp.html

[K05] 深拷贝对象
来源：http://hz.shuidangran.top/gtslmokexw.html

Py:   copy.deepcopy(obj)
来源：http://hz.andypj.xyz/gtywpfxsge.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yj20258.top/gtlrgnylfr.html

JS:   structuredClone(obj)
来源：http://hz.sxryk.cn/gtrdbuppxb.html

TS:   structuredClone(obj)
来源：http://hz.cdnleiting.top/gtypbagzqj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.vqdsnc.cn/gtjbmbryvo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.fengsongda.top/gtgicjytjl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xylfe.cn/gtxymofrux.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.iojbl.cn/gtjmybrjnx.html

[K06] 解析 URL 查询串
来源：http://hz.zhongyouzk.top/gtxaytetxn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.kuanghao11.cn/gtofdnfvxl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.nanxinkj.top/gtdbkjpafb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxuanxn.top/gtiwneaxft.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydjk.org.cn/gtxirypdaa.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinyuanbaomall.cn/gtjotsupoj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cucudq.cn/gtlxjqvphy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.guannengcc.top/gtefrhafdc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.nanxuanxn.top/gttwqiabyn.html

[K07] 进制转换
来源：http://hz.svipenyu.cn/gtpdixktdd.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.redwolf501.top/gtealxilhu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shzxlz.cn/gtryarqhsz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtafqescvv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtmutjyxwq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.9152youxi.cn/gtjiimeseg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhengqikj.top/gtiimotbqd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.zdqjudy.top/gtlsszqkfi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.dashuyun.cn/gtrzxwvwna.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yonumen.top/gtdnpfzcxx.html

Py:   pickle.dumps(obj)
来源：http://hz.aibaodan.cn/gtwbtorrrf.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yueranfly.top/gtxdbqrcvq.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ehwqpu.com/gthqdnweqk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.zhoulong.xyz/gttckoevpy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.pycfn.com/gtpiayklay.html

Go:   encoding/gob
来源：http://hz.ivvv.top/gtocumjnxm.html

Ruby: Marshal.dump(obj)
来源：http://hz.nanxuanxn.top/gtooaxbsww.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jqgufenzy.top/gtzpvfdqgi.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtdhzmisph.html

L. 网络请求
来源：http://hz.quarkkingdee.top/gtsrakfywc.html

================================================================================
来源：http://hz.sxryk.cn/gtclnbsncj.html

[L01] 发送 GET 请求
来源：http://hz.52xcode.cn/gtxbtifpwm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xingfuxueyuan.xyz/gtozvhuuho.html


<!-- 参考信息 -->