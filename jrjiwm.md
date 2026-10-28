代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.birdmap.top/gtjpabpyhh.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj20258.top/gtbqmojtwu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.gaohongyu789.top/gtzgfdrrbv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.dashuyun.cn/gteubgxevb.html

Py:   value = d.get("k") or default
来源：http://hz.nanxuanxn.top/gtddefgkco.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.nanxuanxn.top/gthrdiqxvp.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.smart0.xyz/gtuusbwuhi.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.316326.xyz/gtuuaqtlnz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhaomingkeji.xyz/gtjsukhmjy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhixingplan.top/gtnhucqqjg.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jqgfzy.top/gtmisdgnkd.html

C#:   obj?.A?.B ?? default
来源：http://hz.chenzaomai.com/gtshcgoqdz.html

[H07] 断言
来源：http://hz.hammf.cn/gtzxyrosre.html

Py:   assert x > 0, "必须为正"
来源：http://hz.pycfn.com/gtvaxdlskd.html

PHP:  assert($x > 0);
来源：http://hz.ybcxt.top/gtdbuixpoo.html

JS:   console.assert(x > 0);
来源：http://hz.snrcjt.cn/gtfvxvkibb.html

TS:   console.assert(x > 0);
来源：http://hz.xingfuxueyuan.xyz/gthqwqoccx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.smart0.xyz/gthwrzpkds.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hnxiangtu.top/gtictilcyy.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.0kj1m.cn/gtashyqpgh.html

C#:   Debug.Assert(x > 0);
来源：http://hz.svipenyu.cn/gtynvpbkjq.html

[H08] 获取错误信息与堆栈
来源：http://hz.ivvv.top/gtzxvozeqv.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.chenjidiqi.icu/gtmidmntqy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yanxiufei.cn/gtzbeiwlaz.html

JS:   e.message;  e.stack
来源：http://hz.yueranfly.top/gtpposlmmn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jianghu66.top/gtblfklbrz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.dashuyun.cn/gtfndshgia.html

Go:   err.Error()
来源：http://hz.ybcxt.top/gtafrijleq.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhoulong.xyz/gtbeugsxzg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.dashuyun.cn/gtvjlbxiat.html

[H09] 带错误码的异常
来源：http://hz.vqdsnc.cn/gtdbsfgypl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.guowangkeji.top/gtupokdcuw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shuidangran.top/gtncnnhwcw.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.pengpengdd.cyou/gtrxiygnhm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shanyushiyangkeji.top/gtbuwvfarq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.chenjidiqi.icu/gtykzamlfz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.redwolf501.top/gtdfdqicgp.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hammf.cn/gtidqcjfrk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.mhx1999.top/gtdvhbxbsw.html

[H10] 资源自动释放
来源：http://hz.jinqigfzy.top/gtuvxlzsid.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yangfankeji.com/gtzewygimb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.bjfxy.top/gtyutbeoat.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.pycfn.com/gtlbszlcuu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuxming.cn/gtflccsrtq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yj202588.top/gtyvbemacd.html

Go:   defer f.Close()
来源：http://hz.hfpthk.cn/gthzwviphd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.nwbrower.top/gtncwqfrum.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ehwqpu.com/gtcjbwincy.html

================================================================================
来源：http://hz.yj202588.top/gtcrukivry.html

I. 正则表达式
来源：http://hz.9152youxi.cn/gtlogvulgy.html

================================================================================
来源：http://hz.9152youxi.cn/gtofiekhzi.html

[I01] 判断是否匹配
来源：http://hz.meibo888.top/gtxzgndsey.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jinqigfzy.top/gtpdjeiohk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cheryme.top/gtkehbjmfn.html

JS:   /\d+/.test(s)
来源：http://hz.jyoumei.cn/gtbqqvkrlk.html

TS:   /\d+/.test(s)
来源：http://hz.daria6918.cn/gtvsonbriq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.wangdashe.top/gtesbqddai.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhiwuduotai.top/gtkoxkduvo.html

Ruby: s.match?(/\d+/)
来源：http://hz.yuxming.cn/gtkkoscomt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.redwolf501.top/gtixdguhjn.html

[I02] 提取所有匹配
来源：http://hz.ybcxt.top/gtgyimjcso.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yj20258888.top/gtbfugtktz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.snrcjt.cn/gtdbvpmbrx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jyoumei.cn/gtqudybkyj.html

TS:   s.match(/\d+/g)
来源：http://hz.yj20258.top/gtoislievx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hnqzz.top/gtgrhydnlk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ivvv.top/gtrdbmiwmj.html

Ruby: s.scan(/\d+/)
来源：http://hz.snrcjt.cn/gtfgihzyae.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yuxming.cn/gtzhewyxxv.html

[I03] 提取捕获分组
来源：http://hz.hnxiangtu.top/gtvbcqftzg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shanyushiyangkeji.top/gtjctlfrtw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xuetiantiany.cn/gtfxvheyyl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jqgfzy.top/gtfkbhdyzt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cqqwz.cn/gtlnxprgeg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cucudq.cn/gtecgpzzlq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.dashuyun.cn/gtkzdudmgy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cqqwz.cn/gtlggbswqp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hongshengwenyu.top/gtvplfinov.html

[I04] 正则替换
来源：http://hz.yuxming.cn/gtowykjzfa.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zdqjudy.top/gtmxkxjqtj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.tian-w.cn/gtxwaplchx.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xuanzx.com/gtvhdlryvo.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.svipenyu.cn/gtfeynvvez.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.dashuyun.cn/gtgxijiqqv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.snrcjt.cn/gtgkduevch.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jianghu66.top/gtfohjhkjc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nanxinkj.top/gtmwedtxzc.html

[I05] 按正则拆分
来源：http://hz.hysaishi.cn/gtxaepaojs.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hammf.cn/gtygjrnchl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.wangshuangyany.cn/gtddwahhlu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cashguo.top/gtgriuzkce.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ywan-chungtsiang.top/gtfldunjga.html

Java: s.split("\\s*,\\s*")
来源：http://hz.gogol.net.cn/gtizdatixg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jyoumei.cn/gtrhzkjylz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ivvv.top/gtrgogjyfx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.birdmap.top/gtoegfatux.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jiagoushi.top/gtixrmykeq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sweek.top/gtcrumongb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shanyushiyangtech.top/gtvlyzedas.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.9152youxi.cn/gtgywjlroi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fengsongda.top/gtpcrpeylg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ehwqpu.com/gthvoevxzr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jianghu66.top/gtybhdpsbh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.sxryk.cn/gtnzaddgza.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.c1oappe.top/gtxvnzoduq.html

[I07] 忽略大小写与多行模式
来源：http://hz.ywan-chungtsiang.top/gtbnuawxcq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xuetiantiany.cn/gtawrsrndg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hywenlv.cn/gtiiqwoxqg.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinyuanbaomall.cn/gthswfaaxw.html

TS:   /error/gim
来源：http://hz.yangfankeji.com/gtyriwqbev.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sxryk.cn/gtucoxugiu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.chenjidiqi.icu/gtqhjknger.html

Ruby: s.scan(/error/i)
来源：http://hz.xylfe.cn/gtnaijuhrr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yongpay.top/gtfextfxhm.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.pycfn.com/gtevrkoaza.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ybcxt.top/gtuayivvhk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xuanzx.com/gtsntikoaf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenjidiqi.icu/gtwhdtpine.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuanzhike.top/gtvzmccnwh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jianghu66.top/gtliumqnjy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yuxming.cn/gtxwkncbdu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.nanxuanxn.top/gtkeonbelw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhengqikj.top/gttiihbzid.html

================================================================================
来源：http://hz.ivvv.top/gtjstakxjm.html

J. 日期与时间
来源：http://hz.dianchejie.cn/gthlafmqxc.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtfeseuebs.html

[J01] 获取当前时间
来源：http://hz.zhongyouzk.top/gtpczlcgub.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.birdmap.top/gtgbldsjiq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hnqzz.top/gttmbuoepw.html

JS:   new Date();  Date.now()
来源：http://hz.zhengqikj.top/gtzqgmksat.html

TS:   new Date();  Date.now()
来源：http://hz.yuxming.cn/gtgnvdzezg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.redwolf501.top/gtokkoafbw.html

Go:   time.Now()
来源：http://hz.guowangkeji.top/gtlozuckty.html

Ruby: Time.now
来源：http://hz.ydzc1.top/gthapazamh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jinqigufen.top/gtlpsduald.html

[J02] 格式化输出
来源：http://hz.cashguo.top/gtxpfhqrrk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cheryme.top/gtclshxpsr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.guannengcc.top/gtoulccvgz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.daxiang520.top/gtirisisqf.html

TS:   d.toISOString()
来源：http://hz.yueranfly.top/gtbluskhvm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yj202588.top/gtyhfautkh.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.52xcode.cn/gtpjobuiwu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jlsjyb.cn/gtbbovlhrc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.guannengcc.top/gtmfvyiocw.html

[J03] 字符串解析为日期
来源：http://hz.xuetiantiany.cn/gtrofebjkv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hammf.cn/gtgrhhdbds.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jiagoushi.top/gtnvzrgvcm.html

JS:   new Date("2024-01-02")
来源：http://hz.gotoacloud.top/gtiwqargja.html

TS:   new Date("2024-01-02")
来源：http://hz.ivvv.top/gtcjpslmxw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.pycfn.com/gtnnrftnqo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ivvv.top/gtkdwwegsx.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtyykqwskw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.9152youxi.cn/gtrxqwrvdv.html

[J04] 时间戳与日期互转
来源：http://hz.zhongyouzk.top/gtzmucikli.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.havefunace.top/gtwyeebbhw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xinyue.icu/gtrfbjxxnu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhiwuduotai.top/gtppknjefd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.fzhhl.top/gtpabfzyci.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.havefunace.top/gtycwxatuc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhongyouzk.top/gtvzvtcvmq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.tanke756.top/gthxtrcicd.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.sxryk.cn/gtqbxosgot.html

[J05] 时间加减（加 7 天）
来源：http://hz.andypj.xyz/gthtffvwcx.html

Py:   now + timedelta(days=7)
来源：http://hz.52xcode.cn/gtnentvjne.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.mhx1999.top/gtaabqfgwn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xingfuxueyuan.xyz/gtcnnjsfyd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jqgufenzy.top/gtulukelme.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.redwolf501.top/gtwjbnmrxq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.iojbl.cn/gtnvfouxww.html

Ruby: Time.now + 7 * 86400
来源：http://hz.chenlongwang.top/gtqflfrxwm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.feifeiyinyue.top/gtbhroahbj.html

[J06] 计算两时间之差
来源：http://hz.zhiwuduotai.top/gtvacbqiwf.html

Py:   (end - start).total_seconds()
来源：http://hz.sysykeji.top/gtxfodulwl.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhijiandao.cn/gtueqzlwgl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.tanke756.top/gtsjjcohsa.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.chenjidiqi.icu/gtflaelxvt.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xylfe.cn/gtdtdgfmip.html

Go:   end.Sub(start).Hours()
来源：http://hz.sufxvd.cn/gtynsiwyvr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jinqigfzy.top/gtxmvrvxhk.html

C#:   (end - start).TotalSeconds
来源：http://hz.jianghu66.top/gtwwwkcwcg.html

[J07] 比较两个日期
来源：http://hz.yj20258.top/gtmevcoprh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.iojbl.cn/gtneebspix.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cucudq.cn/gtuilrivez.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ywan-chungtsiang.top/gtfskbimcy.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.haohaochexian.top/gtbiuoagda.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.dianchejie.cn/gtqlebxeiy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shzxlz.cn/gtfsuzngqq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.daxiang520.top/gtpnntuhpd.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.fengsongda.top/gttscvtszw.html

[J08] 提取年月日与星期
来源：http://hz.shuidangran.top/gtkzumdrla.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.snrcjt.cn/gtbxgoemso.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.kuanghao11.cn/gtpznjegzb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.fzhhl.top/gtqhrvejux.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xylfe.cn/gtcwejdvbz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.guowangkeji.top/gtexwbqjpj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yuxming.cn/gtcrmopomq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.nanxinkj.top/gteaahuhaf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.birdmap.top/gtxddkjpih.html

[J09] 时区处理
来源：http://hz.sysykeji.top/gtsysyovly.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yj202588.top/gtsdpaorti.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yanxiufei.cn/gtwegrekvc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shuidangran.top/gtcvgrshjg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.pycfn.com/gtxmppsnlc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.sweek.top/gtpboowezy.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zycfv.cn/gtoqrgnsif.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yj202588.top/gtzbklajay.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.daxiang520.top/gtusibiaix.html

[J10] 取今天 / 本月第一天
来源：http://hz.c1oappe.top/gtrxclegof.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.daria6918.cn/gtrhahcbww.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sufxvd.cn/gtpvapdorq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.vqdsnc.cn/gtpywewxcd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cheryme.top/gtmuzgzaut.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ehwqpu.com/gtshytccmb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.sysykeji.top/gtgjlgsflb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.wangshuangyany.cn/gtwcstcmnc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.redwolf501.top/gtycgyxkyd.html

================================================================================
来源：http://hz.ydzc1.top/gtqykxezko.html

K. JSON 与序列化
来源：http://hz.chenzaomai.com/gtoozjlazi.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtospxgpkj.html

[K01] 对象转 JSON 字符串
来源：http://hz.dianchejie.cn/gtjxzqlnoh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.tian-w.cn/gtijizaqfq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.meibo888.top/gtgxfgyfda.html

JS:   JSON.stringify(obj)
来源：http://hz.xuetiantiany.cn/gtygfhldyl.html

TS:   JSON.stringify(obj)
来源：http://hz.zhengqikj.top/gtayxrturu.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shuidangran.top/gtqzvkgyfh.html

Go:   json.Marshal(obj)
来源：http://hz.9152youxi.cn/gtxzfmuydi.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.wangdashe.top/gtowvatwmy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jqgfzy.top/gtojqhyjkf.html

[K02] JSON 字符串转对象
来源：http://hz.guannengcc.top/gtagfdoral.html

Py:   json.loads(s)
来源：http://hz.vqdsnc.cn/gtmhhvsrlg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hywenlv.cn/gtxensyebi.html

JS:   JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtszwdjxxf.html

TS:   JSON.parse(s)
来源：http://hz.jinyuanbaomall.cn/gtxwmtyiya.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shanyushiyangtech.top/gtxuziiisq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yuanzhike.top/gtcthvjbxl.html

Ruby: JSON.parse(s)
来源：http://hz.jqgfzy.top/gtjrvnmcco.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.chenzaomai.com/gtgccjovmy.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ywan-chungtsiang.top/gtklyupenm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.nanxuanxn.top/gtwsshlmne.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yuanzhike.top/gtkufrfxmi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.birdmap.top/gtolwsdsfo.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.redwolf501.top/gtxtnnaaqt.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.c1oappe.top/gtonrpionx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.pycfn.com/gtdzoudtem.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.guannengcc.top/gtkklffmer.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.feifeiyinyue.top/gtgiudciod.html

[K04] 读取 JSON 文件
来源：http://hz.chenlongwang.top/gtqokterdf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cheryme.top/gtpxhupsfz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ivvv.top/gtmxvdualy.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dianchejie.cn/gtczlanzuo.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhijiandao.cn/gtpcmtyfvt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jqgufenzy.top/gtxyfqrkkc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.snrcjt.cn/gtpjgzeayf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jyoumei.cn/gtffcqpdhy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ivvv.top/gtrwjtldbn.html

[K05] 深拷贝对象
来源：http://hz.hysaishi.cn/gtjvrmoaiu.html

Py:   copy.deepcopy(obj)
来源：http://hz.havefunace.top/gtspwqague.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jiagoushi.top/gtasktxxtv.html

JS:   structuredClone(obj)
来源：http://hz.gotoacloud.top/gtfkcnbdyt.html

TS:   structuredClone(obj)
来源：http://hz.aizwys.cn/gtbhrxjnhz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xingfuxueyuan.xyz/gtficiewvn.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.fengsongda.top/gtimblccqh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.tian-w.cn/gtcyluvwju.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hammf.cn/gthphtatwj.html

[K06] 解析 URL 查询串
来源：http://hz.smart0.xyz/gtrzujpyvu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ehwqpu.com/gtzouqtbqh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.sxryk.cn/gtcntrhppd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jqgfzy.top/gtrpqnvpmg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.guannengcc.top/gtyucgxujq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.chenzaomai.com/gtybyverwm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.daxiang520.top/gtratgxsmi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yj202588.top/gtyiwvivfy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cdnleiting.top/gtqbxyvbux.html

[K07] 进制转换
来源：http://hz.cqqwz.cn/gtswwwfoxa.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtbepkccct.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.hammf.cn/gtrqkjjwjc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hnxiangtu.top/gttdnnhslr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zdqjudy.top/gtrmuipucr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.daria6918.cn/gtbywdppfi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.chenjidiqi.icu/gtopbsjuxk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sxryk.cn/gtibtfhmqw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yangfankeji.com/gtjwplagic.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zhijiandao.cn/gtszpkesja.html

Py:   pickle.dumps(obj)
来源：http://hz.havefunace.top/gtmkipakfo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.xingfuxueyuan.xyz/gttoyfcoki.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.fzhhl.top/gtlyeseqla.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.xziqi.cn/gtyurfgzoy.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.tianlin.xyz/gtpjlzxtgx.html

Go:   encoding/gob
来源：http://hz.hywenlv.cn/gtgzoqcuea.html

Ruby: Marshal.dump(obj)
来源：http://hz.svipenyu.cn/gtsdjttdnn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.haohaochexian.top/gtmajrgiya.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtevdtccvo.html

L. 网络请求
来源：http://hz.sweek.top/gtfwyqxwoc.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtbhjuakbl.html

[L01] 发送 GET 请求
来源：http://hz.jianghu66.top/gtyhlehyqe.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jinghuilouyu.cn/gtvnkfdhgj.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhongyouzk.top/gtsoubuxrx.html

JS:   await fetch(url)
来源：http://hz.shanyushiyangkeji.top/gtemuillrr.html

TS:   await fetch(url)
来源：http://hz.xuanzx.com/gttllrmckp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.shuidangran.top/gtjdhzfysf.html


<!-- 参考信息 -->