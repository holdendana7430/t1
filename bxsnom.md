代发 wailian999

TS:   console.assert(x > 0);
来源：http://hz.ivvv.top/gtixwicvnp.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zycfv.cn/gtirdmmzcw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhoulong.xyz/gtakcnrndf.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jqgfzy.top/gtnehpcmpm.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cucudq.cn/gtojbgnlhk.html

[H08] 获取错误信息与堆栈
来源：http://hz.yvedp.cn/gtkgaqefpf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.sxryk.cn/gtikoklvbn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.mhx1999.top/gtcsxswjjl.html

JS:   e.message;  e.stack
来源：http://hz.jinqigufen.top/gtapzlamrv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hywenlv.cn/gtsopmlrck.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jqgufenzy.top/gtbzooflyx.html

Go:   err.Error()
来源：http://hz.0kj1m.cn/gtugnqnkbj.html

Ruby: e.message;  e.backtrace
来源：http://hz.xinyue.icu/gtzloprxev.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jinyuanbaomall.cn/gttexffeyd.html

[H09] 带错误码的异常
来源：http://hz.shanyushiyangkeji.top/gthcglwxrk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hnqzz.top/gtsgyqpjxk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shuidangran.top/gtdrwfpnhn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.316326.xyz/gtiflvjuuy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhongyouzk.top/gtbyomwmdy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cqqwz.cn/gtdxhtazlb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.nanxuanxn.top/gtxjagxlkz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gaohongyu789.top/gticjngzxu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xinyue.icu/gtpskiydgb.html

[H10] 资源自动释放
来源：http://hz.ivvv.top/gtkihxwocn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.sysykeji.top/gtbrhrvfua.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.vqdsnc.cn/gtovbrrhgt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.52xcode.cn/gtxndnycfp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yongpay.top/gtwbcebmzc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.wangshuangyany.cn/gtewsthnlc.html

Go:   defer f.Close()
来源：http://hz.zhiwuduotai.top/gtnirwzxjf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xylfe.cn/gtcczmmahw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinqigfzy.top/gtnepfozsm.html

================================================================================
来源：http://hz.jqgufenzy.top/gtmcbcbaun.html

I. 正则表达式
来源：http://hz.chenjidiqi.icu/gtmaroladc.html

================================================================================
来源：http://hz.jianghu66.top/gtdmvkdbnd.html

[I01] 判断是否匹配
来源：http://hz.redwolf501.top/gtocxcchwf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shanyushiyangtech.top/gtmodlmnvw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhijiandao.cn/gtzlouujnx.html

JS:   /\d+/.test(s)
来源：http://hz.andypj.xyz/gtzihlzrcp.html

TS:   /\d+/.test(s)
来源：http://hz.yangfankeji.com/gtxipqftnv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenjidiqi.icu/gttrxtoycf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.c1oappe.top/gthdozjsuu.html

Ruby: s.match?(/\d+/)
来源：http://hz.0kj1m.cn/gtndpggrty.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hnqzz.top/gtnwnwthjt.html

[I02] 提取所有匹配
来源：http://hz.chenlongwang.top/gtjlmwsihk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.snrcjt.cn/gtzdpujcxq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.gogol.net.cn/gtlpoquhlc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhoulong.xyz/gtmsfuloxc.html

TS:   s.match(/\d+/g)
来源：http://hz.tianlin.xyz/gtpmrivlob.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ybcxt.top/gtuepoehqs.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.sysykeji.top/gtlqbkmxnr.html

Ruby: s.scan(/\d+/)
来源：http://hz.jiagoushi.top/gtcfbgzuib.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ybcxt.top/gtlrwyhxug.html

[I03] 提取捕获分组
来源：http://hz.jinghuilouyu.cn/gtqhtpigvk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.guannengcc.top/gtnwtnmewv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.nwbrower.top/gtzjrhjhjf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jinqigufen.top/gtkgaroxgz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ivvv.top/gtwitahkwc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.pengpengdd.cyou/gtfcanryds.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.meibo888.top/gtfpgngzpr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.quarkkingdee.top/gttutgmfuw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gotoacloud.top/gtfsroseyj.html

[I04] 正则替换
来源：http://hz.fzhhl.top/gtgcvzqbbk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.dianchejie.cn/gtfagzrxsi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ppjwa.cn/gtuablchxd.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yj20258888.top/gtteinotfk.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.wangshuangyany.cn/gtsqqhjqpz.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinqigfzy.top/gtarmjkrwu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhixingplan.top/gtdubcsbgz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hongshengwenyu.top/gtsofowkvv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinghuilouyu.cn/gtkukoydbp.html

[I05] 按正则拆分
来源：http://hz.zdqjudy.top/gttbjpwzxp.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yj20258888.top/gtmmwluwve.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xinyue.icu/gtbnbvgpjh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangtech.top/gttkzqfwhz.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.guannengcc.top/gttheygqfk.html

Java: s.split("\\s*,\\s*")
来源：http://hz.havefunace.top/gtayktdeqb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.dianchejie.cn/gttazeegzw.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.bjfxy.top/gtyjuwcxdu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.mhx1999.top/gtlvqnjjii.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cashguo.top/gthsjxjbnn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yongpay.top/gtyifsayqu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cucudq.cn/gtflpzfywu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shuidangran.top/gtpojscdxc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aibaodan.cn/gtiiyycnqd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.nanxuanxn.top/gtbvlrhmnp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hfpthk.cn/gtjqabrqyw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.nanxuanxn.top/gtrubczifb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhengqikj.top/gtqcnpefft.html

[I07] 忽略大小写与多行模式
来源：http://hz.dianchejie.cn/gtkhmigwle.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cdnleiting.top/gtxpqmtjmx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hnxiangtu.top/gtgvirjbbv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yj20258888.top/gtmlmjnnyw.html

TS:   /error/gim
来源：http://hz.jinyuanbaomall.cn/gtlyxbgiui.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.nanxuanxn.top/gtzsrkjbzn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.guannengcc.top/gtjilqelma.html

Ruby: s.scan(/error/i)
来源：http://hz.nanxuanxn.top/gtdsjitdas.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinghuilouyu.cn/gtcgzieyak.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinyuanbaomall.cn/gtrvxfrjhz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.guannengcc.top/gtlmokywju.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yj20258888.top/gtkigsfwcf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sxryk.cn/gtcaeoxsec.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guowangkeji.top/gtxrpcoxtl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.snrcjt.cn/gtuzlsaefx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gzhubu.top/gtnswphncl.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shanyushiyangtech.top/gtcwuduhug.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cqqwz.cn/gtlcroxmwy.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtcsdololu.html

J. 日期与时间
来源：http://hz.jinqigfzy.top/gtoxdifnsh.html

================================================================================
来源：http://hz.aizwys.cn/gtuwhpiqdr.html

[J01] 获取当前时间
来源：http://hz.andypj.xyz/gtvzgqorpm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinqigufen.top/gtcbzrlyse.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yueranfly.top/gtngivdiut.html

JS:   new Date();  Date.now()
来源：http://hz.yj202588.top/gtsvoyfvdh.html

TS:   new Date();  Date.now()
来源：http://hz.yuanzhike.top/gtajldgfsi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shanyushiyangkeji.top/gtjsjijmnx.html

Go:   time.Now()
来源：http://hz.nwbrower.top/gtnqogayfo.html

Ruby: Time.now
来源：http://hz.jinyuanbaomall.cn/gtneiwizlz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.iojbl.cn/gtfqcpadns.html

[J02] 格式化输出
来源：http://hz.nanxuanxn.top/gtdgbjtcqt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zdqjudy.top/gtuezfcman.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhengqikj.top/gtskappbid.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sysykeji.top/gtbrxmklzf.html

TS:   d.toISOString()
来源：http://hz.ybcxt.top/gtiifdnfmz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xuetiantiany.cn/gtajjbxuei.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.andypj.xyz/gthtiuyikr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cucudq.cn/gtxltnneea.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cheryme.top/gtfkyrrxkk.html

[J03] 字符串解析为日期
来源：http://hz.hongshengwenyu.top/gtarbzczqd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.wangshuangyany.cn/gtylxbwopu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.fzhhl.top/gtmrxumhlo.html

JS:   new Date("2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtseccuufl.html

TS:   new Date("2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtjzskvwct.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xziqi.cn/gticivxliy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jianghu66.top/gtoqjrnpdz.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinqigufen.top/gtbkecbhap.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhijiandao.cn/gtxfzkmwet.html

[J04] 时间戳与日期互转
来源：http://hz.xuanzx.com/gtfkhudlkv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.tian-w.cn/gtpbsnlmws.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shanyushiyangkeji.top/gtnmznufgz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yanxiufei.cn/gtobocrcgd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xinyue.icu/gtwgcfjpac.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.quarkkingdee.top/gtlaimlgjp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shanyushiyangkeji.top/gtkqnwhddt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.kuanghao11.cn/gtbgktnjnw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shanyushiyangtech.top/gtzjtecxsz.html

[J05] 时间加减（加 7 天）
来源：http://hz.nanxinkj.top/gtioxmbjul.html

Py:   now + timedelta(days=7)
来源：http://hz.pengpengdd.cyou/gtueaptrdt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhiwuduotai.top/gtxpgcgsob.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhaomingkeji.xyz/gtzbcopijb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jlsjyb.cn/gtpqnafjil.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.tianlin.xyz/gteiyhccau.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jyoumei.cn/gtcglyrgeo.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hammf.cn/gtxrrbrssl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.guannengcc.top/gttusawinh.html

[J06] 计算两时间之差
来源：http://hz.svipenyu.cn/gthxmplimg.html

Py:   (end - start).total_seconds()
来源：http://hz.yj20258888.top/gtrqilyvja.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinghuilouyu.cn/gtukxprqij.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jqgufenzy.top/gtgufpyhti.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.daxiang520.top/gtdlsvnwjr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jqgufenzy.top/gtpimgbxax.html

Go:   end.Sub(start).Hours()
来源：http://hz.fzhhl.top/gtcaqxfbia.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xinyue.icu/gtigxjrver.html

C#:   (end - start).TotalSeconds
来源：http://hz.jqgfzy.top/gtcxezwsyt.html

[J07] 比较两个日期
来源：http://hz.snrcjt.cn/gtrtatzbis.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ywan-chungtsiang.top/gtblkvzsqr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hammf.cn/gtqlwqkwtx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ywan-chungtsiang.top/gtnyrbddrl.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zdqjudy.top/gtadwumsmw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cashguo.top/gtgqtsyppp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zycfv.cn/gtmljpdwdl.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yuanzhike.top/gtupkvpixx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jianghu66.top/gtsceiyhru.html

[J08] 提取年月日与星期
来源：http://hz.nanxuanxn.top/gtkrvuxqgz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.tianlin.xyz/gtngsbgtum.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.dashuyun.cn/gtbahoxskg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.daxiang520.top/gtyeqrcbya.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ehwqpu.com/gthjerdaen.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.svipenyu.cn/gtnupjimlh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jyoumei.cn/gtwmyssqbf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jinqigfzy.top/gtwybeaaza.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.chenzaomai.com/gtveaaucga.html

[J09] 时区处理
来源：http://hz.cashguo.top/gtdgcnrlwa.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.nanxinkj.top/gtzjbhswxd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.andypj.xyz/gtdkmvxfva.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigfzy.top/gtognbxumt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.bjfxy.top/gtgixhbwcs.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jlsjyb.cn/gtsnlcbudx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yvedp.cn/gtofvgjptu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.sysykeji.top/gtvehkfbjl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yongpay.top/gtzupnwdel.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhixingplan.top/gtlxvujxzp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.havefunace.top/gtvytroviv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.nanxinkj.top/gtpoldqcwl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.sufxvd.cn/gtmepqqumw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yonumen.top/gthghfsvxw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yvedp.cn/gtsljjntdy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hammf.cn/gtifrcbfnu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jiagoushi.top/gtxwciliax.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.snrcjt.cn/gtwhshkeaf.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtuzjacdeb.html

K. JSON 与序列化
来源：http://hz.0kj1m.cn/gtecdpgorw.html

================================================================================
来源：http://hz.hysaishi.cn/gtgroynlkb.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhaomingkeji.xyz/gtytlwrpvn.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.c1oappe.top/gtitmwwdks.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.gotoacloud.top/gtaednyipw.html

JS:   JSON.stringify(obj)
来源：http://hz.meibo888.top/gtceyulpkq.html

TS:   JSON.stringify(obj)
来源：http://hz.yangfankeji.com/gtoilmglwy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jiagoushi.top/gtzfpecprl.html

Go:   json.Marshal(obj)
来源：http://hz.hammf.cn/gtssmoteqf.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.pycfn.com/gtwciafowh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.daxiang520.top/gtzpyodhad.html

[K02] JSON 字符串转对象
来源：http://hz.shanyushiyangtech.top/gttwzjxles.html

Py:   json.loads(s)
来源：http://hz.yj20258888.top/gtkayqosfq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yuanzhike.top/gtbonzlutx.html

JS:   JSON.parse(s)
来源：http://hz.jqgfzy.top/gteancdbry.html

TS:   JSON.parse(s)
来源：http://hz.meibo888.top/gtautmprhm.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xuetiantiany.cn/gtdgbwqgpy.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.smart0.xyz/gtxkjxqmef.html

Ruby: JSON.parse(s)
来源：http://hz.jinqigfzy.top/gtgtuffwgd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.c1oappe.top/gtptisvuga.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jyoumei.cn/gtulqlppjc.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.nanxinkj.top/gtpaicygfp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinghuilouyu.cn/gtehxplhqk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgufenzy.top/gtonngrpce.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.chenjidiqi.icu/gtyqfamcaw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cqqwz.cn/gtfbgtjdol.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cqqwz.cn/gtdzxowtxf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gotoacloud.top/gtnxgynigo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.svipenyu.cn/gtmvtymdir.html

[K04] 读取 JSON 文件
来源：http://hz.dashuyun.cn/gtkpernkrp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yuanzhike.top/gtryyohrgi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhongyouzk.top/gtqaypyeea.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sysykeji.top/gtuxgdzlgf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xziqi.cn/gtgpjsionf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.quarkkingdee.top/gtxrnttldn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.quarkkingdee.top/gtocdqiaiu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.tanke756.top/gtrxbcxnci.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jianghu66.top/gttlhfizxj.html

[K05] 深拷贝对象
来源：http://hz.sysykeji.top/gtvhpchara.html

Py:   copy.deepcopy(obj)
来源：http://hz.aibaodan.cn/gtvytlnavw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.bjfxy.top/gtmbjonkkm.html

JS:   structuredClone(obj)
来源：http://hz.xziqi.cn/gtzfskhioo.html

TS:   structuredClone(obj)
来源：http://hz.fzhhl.top/gtxxedihft.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.pycfn.com/gtnqcvyxjl.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.guowangkeji.top/gtfcbhadxl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.sufxvd.cn/gtytxthpuc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shangyingyoupin.top/gtungqogkz.html

[K06] 解析 URL 查询串
来源：http://hz.yonumen.top/gtfnnvjlkx.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hongshengwenyu.top/gtihufffha.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.shzxlz.cn/gtxjgaflmq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fengsongda.top/gtixmlyggr.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.9152youxi.cn/gtlcvytycz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yueranfly.top/gtjgvxabvb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.snrcjt.cn/gtwvccxkbv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ehwqpu.com/gthjintrpx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hammf.cn/gtuohaviqc.html

[K07] 进制转换
来源：http://hz.kuanghao11.cn/gtbbkyznmy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.dianchejie.cn/gtowfrroni.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.redwolf501.top/gtxfxinoua.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.0kj1m.cn/gtzqqhyiuc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhoulong.xyz/gtstlvkoms.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtgmlessvw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.havefunace.top/gtnnxwvbkf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yuanzhike.top/gtxsboxmzj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xinyue.icu/gtglevhzdr.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.cucudq.cn/gtyoejsmcn.html

Py:   pickle.dumps(obj)
来源：http://hz.yuxming.cn/gtwttujgzi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.snrcjt.cn/gtxqwdmmdm.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.snrcjt.cn/gtcbocgzzg.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.bjfxy.top/gtcauomzfk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ehwqpu.com/gtqbpsugri.html

Go:   encoding/gob
来源：http://hz.hysaishi.cn/gttcgcjvsy.html

Ruby: Marshal.dump(obj)
来源：http://hz.sufxvd.cn/gtfeciiowp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.guowangkeji.top/gtnqjeofea.html

================================================================================
来源：http://hz.mhx1999.top/gtouzkywrq.html

L. 网络请求
来源：http://hz.chenzaomai.com/gtorejwjlx.html

================================================================================
来源：http://hz.cdnleiting.top/gtwlsfimxs.html

[L01] 发送 GET 请求
来源：http://hz.sysykeji.top/gtwrgaojbc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.tian-w.cn/gtznuwvpba.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.kuanghao11.cn/gtmkkhdcob.html

JS:   await fetch(url)
来源：http://hz.shanyushiyangtech.top/gtwiaojkin.html

TS:   await fetch(url)
来源：http://hz.xuanzx.com/gtagnhlpye.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yvedp.cn/gtjsvxemna.html

Go:   resp, err := http.Get(url)
来源：http://hz.kuanghao11.cn/gtbffzlcpd.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.cqqwz.cn/gthmtwrgij.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.jianghu66.top/gtiyuqcxyh.html

[L02] 发送 POST JSON
来源：http://hz.yanxiufei.cn/gtpncxtjdx.html

Py:   requests.post(url, json={"a": 1})
来源：http://hz.cucudq.cn/gtyvjlwsov.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hz.zhongyouzk.top/gtoxujkeem.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.jinqigufen.top/gtvkowllmw.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hz.yonumen.top/gtofxoclnu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hz.zhaomingkeji.xyz/gtlzfkbdbh.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hz.316326.xyz/gtwnhggltb.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hz.vqdsnc.cn/gtunmiwlhl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hz.ydjk.org.cn/gtekiabfzr.html

[L03] 设置自定义请求头
来源：http://hz.sysykeji.top/gtbxqwmfvl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hz.yangfankeji.com/gtqksbkjrl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hz.jiagoushi.top/gtvolmtvkx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hz.vqdsnc.cn/gtnynnvwmf.html


<!-- 参考信息 -->