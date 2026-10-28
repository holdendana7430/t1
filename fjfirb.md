代发 wailian999

Py:   value = d.get("k") or default
来源：http://hz.hammf.cn/gtuxwahdhu.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhiwuduotai.top/gtgbtcvoqn.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jyoumei.cn/gtmtlngcsb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhoulong.xyz/gtsjbajavl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hammf.cn/gtnlvaqhqz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nanxinkj.top/gtxwyzjytc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.pengpengdd.cyou/gtzvhyvllv.html

C#:   obj?.A?.B ?? default
来源：http://hz.jyoumei.cn/gtlircwdrt.html

[H07] 断言
来源：http://hz.52xcode.cn/gtqpgrltnh.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ybcxt.top/gtlkjmjssw.html

PHP:  assert($x > 0);
来源：http://hz.aizwys.cn/gtxkxtgqmn.html

JS:   console.assert(x > 0);
来源：http://hz.zhoulong.xyz/gtmozuviok.html

TS:   console.assert(x > 0);
来源：http://hz.guowangkeji.top/gtdqhinsgf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shanyushiyangtech.top/gttdqlhqfo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.tianlin.xyz/gtoalvtfka.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.shzxlz.cn/gtqpumtqax.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hongshengwenyu.top/gtvtffejba.html

[H08] 获取错误信息与堆栈
来源：http://hz.cdnleiting.top/gtvhiubwnc.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yvedp.cn/gtzpuujxag.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yuanzhike.top/gtdcrvmshs.html

JS:   e.message;  e.stack
来源：http://hz.feifeiyinyue.top/gtluhaubfj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cdnleiting.top/gtykhazsdh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.c1oappe.top/gtnyammpya.html

Go:   err.Error()
来源：http://hz.sxryk.cn/gtepyzgoqu.html

Ruby: e.message;  e.backtrace
来源：http://hz.kuanghao11.cn/gtpywzydww.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tianlin.xyz/gtjatvxvbu.html

[H09] 带错误码的异常
来源：http://hz.fengsongda.top/gteinebxgn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.aibaodan.cn/gttqsazohc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinqigfzy.top/gthratmcnt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.bjfxy.top/gtnbwdyxmi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.havefunace.top/gtwdaswznl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yanxiufei.cn/gtomhoaeqn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ppjwa.cn/gteswmdwza.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hywenlv.cn/gtzzzswbls.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yuxming.cn/gtugqdfzfm.html

[H10] 资源自动释放
来源：http://hz.zhiwuduotai.top/gtsuhsiuyk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.chenzaomai.com/gtlmnlkgqs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.feifeiyinyue.top/gtbsnfgcaf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gotoacloud.top/gtfyonsqlt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.fzhhl.top/gthtggpxqf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.cqqwz.cn/gtbbrszbzk.html

Go:   defer f.Close()
来源：http://hz.yuxming.cn/gtznqnvdse.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shanyushiyangtech.top/gtsdgrhafx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.svipenyu.cn/gtafhaqyic.html

================================================================================
来源：http://hz.havefunace.top/gtzeyzsdin.html

I. 正则表达式
来源：http://hz.zhoulong.xyz/gtmdmxartt.html

================================================================================
来源：http://hz.hnqzz.top/gtmbeymqoi.html

[I01] 判断是否匹配
来源：http://hz.0kj1m.cn/gtszbpgumg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shuidangran.top/gteshmlffe.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shzxlz.cn/gtjyogjldd.html

JS:   /\d+/.test(s)
来源：http://hz.shangyingyoupin.top/gtbaoqlctd.html

TS:   /\d+/.test(s)
来源：http://hz.chenlongwang.top/gthvshldmr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhijiandao.cn/gttumxxcbz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.vqdsnc.cn/gtusajhzow.html

Ruby: s.match?(/\d+/)
来源：http://hz.gaohongyu789.top/gteeirqnwz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jqgfzy.top/gthdosuyjk.html

[I02] 提取所有匹配
来源：http://hz.c1oappe.top/gtfwgpuetz.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yvedp.cn/gtadetwqco.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cucudq.cn/gtbikwxvxl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.nwbrower.top/gtiifoeong.html

TS:   s.match(/\d+/g)
来源：http://hz.yvedp.cn/gtigkatgyu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.gogol.net.cn/gtmgsbvmgs.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.gotoacloud.top/gtvbmzvnbn.html

Ruby: s.scan(/\d+/)
来源：http://hz.fzhhl.top/gtybirchse.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhiwuduotai.top/gtxsbjbhlk.html

[I03] 提取捕获分组
来源：http://hz.xuanzx.com/gtormlbjec.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.quarkkingdee.top/gtnrxkimwm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hfpthk.cn/gthcuduirq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.havefunace.top/gtupsjkjub.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cqqwz.cn/gtwbfbmqzj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jlsjyb.cn/gtjtuamwon.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhoulong.xyz/gtvadgvzuw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hysaishi.cn/gtojdwqxgm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yuanzhike.top/gtryguvkqc.html

[I04] 正则替换
来源：http://hz.jiagoushi.top/gtbtesugyl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.tianlin.xyz/gtsnsnxryr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jianghu66.top/gtugevsloj.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yuanzhike.top/gtnszoqidp.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.0kj1m.cn/gtaeufnnvg.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hfpthk.cn/gtsbdncxcp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhaomingkeji.xyz/gtffxfxojb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jqgufenzy.top/gtiucgslyk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.pengpengdd.cyou/gtlonnhdki.html

[I05] 按正则拆分
来源：http://hz.nwbrower.top/gtmdsauomt.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shuidangran.top/gtecdpbgmw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.guowangkeji.top/gthnpspbty.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yanxiufei.cn/gtdcngsptz.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cucudq.cn/gtuovdmrjc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.birdmap.top/gtxtvedkmh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jinqigufen.top/gtililrtku.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.meibo888.top/gtyuqkdxps.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.nanxinkj.top/gtnikbfgol.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jiagoushi.top/gtfamffqto.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yvedp.cn/gtqpqdbbya.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yj20258888.top/gtqxyfamro.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nanxinkj.top/gtmlvdycff.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tanke756.top/gtluzkzraq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jqgufenzy.top/gtfctazgmu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hywenlv.cn/gtvllwimeb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.9152youxi.cn/gtmogtoems.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.aibaodan.cn/gtboyfzlbu.html

[I07] 忽略大小写与多行模式
来源：http://hz.cdnleiting.top/gtmwfmvdvs.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sweek.top/gtpwxpknrq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hfpthk.cn/gtsbwkyjvq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.guannengcc.top/gtpokkgfvf.html

TS:   /error/gim
来源：http://hz.yj202588.top/gtfkytjcwq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.vqdsnc.cn/gtuhsodyze.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhijiandao.cn/gtkapvtiwx.html

Ruby: s.scan(/error/i)
来源：http://hz.meibo888.top/gtenhsiamz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.9152youxi.cn/gtvpxaoxwk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.wangdashe.top/gttimojyel.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.daxiang520.top/gtxjbfnzsn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.fengsongda.top/gtryhtnfes.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xziqi.cn/gtmrmkvyxm.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ydzc1.top/gtjghbuxvp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.52xcode.cn/gtzoyvkbhh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.quarkkingdee.top/gtppewsgar.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jqgfzy.top/gtoikczkwv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ppjwa.cn/gthetzdhug.html

================================================================================
来源：http://hz.yueranfly.top/gtshnqgrjz.html

J. 日期与时间
来源：http://hz.yuanzhike.top/gtorgoveef.html

================================================================================
来源：http://hz.sysykeji.top/gtelqxnwca.html

[J01] 获取当前时间
来源：http://hz.sufxvd.cn/gttfvehzxm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.guowangkeji.top/gtmvrmflxu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zdqjudy.top/gtdiqoxane.html

JS:   new Date();  Date.now()
来源：http://hz.shanyushiyangtech.top/gtdzhzkjkh.html

TS:   new Date();  Date.now()
来源：http://hz.chenzaomai.com/gtupzotuip.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.svipenyu.cn/gtjvasasuc.html

Go:   time.Now()
来源：http://hz.zhiwuduotai.top/gtxhhhruce.html

Ruby: Time.now
来源：http://hz.hongshengwenyu.top/gtnmngwlwp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shuidangran.top/gtbprurvle.html

[J02] 格式化输出
来源：http://hz.hywenlv.cn/gthhztgybr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.snrcjt.cn/gtucskbqdv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.kuanghao11.cn/gtwwphgmav.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tianlin.xyz/gtafpklvja.html

TS:   d.toISOString()
来源：http://hz.jinyuanbaomall.cn/gtzoghyams.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yonumen.top/gtywvkulxc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hfpthk.cn/gtgmhtsvkg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhoulong.xyz/gtzxlzfisl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gotoacloud.top/gtbtixrrbd.html

[J03] 字符串解析为日期
来源：http://hz.tanke756.top/gtnxovnlgc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.cdnleiting.top/gtbtdsjczw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yongpay.top/gtumullqln.html

JS:   new Date("2024-01-02")
来源：http://hz.tianlin.xyz/gtfqujkhts.html

TS:   new Date("2024-01-02")
来源：http://hz.fzhhl.top/gtcxzgdwcm.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cheryme.top/gtrorwdfhx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hfpthk.cn/gtapykadrs.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.daria6918.cn/gtajpxyrrd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.chenlongwang.top/gtskdckrob.html

[J04] 时间戳与日期互转
来源：http://hz.svipenyu.cn/gtrngioyss.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.chenjidiqi.icu/gttvkjzzvd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hysaishi.cn/gtbswstnpr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.dashuyun.cn/gtijgjmmaa.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yanxiufei.cn/gtqnweuloj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.tian-w.cn/gtgxccbmaq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.redwolf501.top/gtcsrxdzml.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xinyue.icu/gtbbkgyswo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.guowangkeji.top/gtosprfprz.html

[J05] 时间加减（加 7 天）
来源：http://hz.ehwqpu.com/gtlkhkqyvx.html

Py:   now + timedelta(days=7)
来源：http://hz.fengsongda.top/gtgjbjwesk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hammf.cn/gtlxlczjxi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cashguo.top/gtazmytfej.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hammf.cn/gtegqqxtzn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ydzc1.top/gtfdfquvqq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xingfuxueyuan.xyz/gttmaljzpe.html

Ruby: Time.now + 7 * 86400
来源：http://hz.aizwys.cn/gtzlqprkqp.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jinqigufen.top/gtzwkpuvbk.html

[J06] 计算两时间之差
来源：http://hz.xuanzx.com/gtgqsocyva.html

Py:   (end - start).total_seconds()
来源：http://hz.mhx1999.top/gtlmovxgoa.html

PHP:  $end->diff($start)->days;
来源：http://hz.fzhhl.top/gthvoqnazm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hnxiangtu.top/gtbbzloxjg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinqigfzy.top/gtwpbshafp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cucudq.cn/gtdjfphjxn.html

Go:   end.Sub(start).Hours()
来源：http://hz.9152youxi.cn/gtjoukzytt.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xinyue.icu/gtjqnudqeo.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhijiandao.cn/gthdpwkfbw.html

[J07] 比较两个日期
来源：http://hz.cashguo.top/gtjapfgans.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hammf.cn/gtjyjhymzg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.sweek.top/gtjebmmzgq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xinyue.icu/gtfbslwkpi.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.tianlin.xyz/gtiilmfooy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jqgfzy.top/gtyidxxduc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.iojbl.cn/gtbreaatzn.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.feifeiyinyue.top/gtlvgotmsr.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.guowangkeji.top/gtlkqzutup.html

[J08] 提取年月日与星期
来源：http://hz.0kj1m.cn/gtsqluwzwq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhengqikj.top/gtjfcbxtvv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.mhx1999.top/gtpqtgvfiw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.tanke756.top/gtqekfxrys.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.guannengcc.top/gtzfuuohwo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yvedp.cn/gtqqclzcfe.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenlongwang.top/gtqyoxsedf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.pycfn.com/gtgtnpzykq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.chenzaomai.com/gtosqlzhqp.html

[J09] 时区处理
来源：http://hz.pycfn.com/gtcnvpdzwh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.tian-w.cn/gteezmthsn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hnqzz.top/gtereitewz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhaomingkeji.xyz/gtlgnvzmqj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuanzhike.top/gtlfjreyok.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.bjfxy.top/gttijerbwu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.0kj1m.cn/gtzqbcfmor.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.aizwys.cn/gthnhzyykh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.tanke756.top/gtbykizolo.html

[J10] 取今天 / 本月第一天
来源：http://hz.ppjwa.cn/gtgzlsdslh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jiagoushi.top/gtmwbxgpsk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yj20258888.top/gtzsdahbyh.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.pycfn.com/gtucjhsjiy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.iojbl.cn/gtpdbiudem.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shuidangran.top/gtogfkpvff.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.bjfxy.top/gtffhfizaw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jyoumei.cn/gtgnhygtnv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yueranfly.top/gtdklfmpnl.html

================================================================================
来源：http://hz.gaohongyu789.top/gtypvgdzyn.html

K. JSON 与序列化
来源：http://hz.zhongyouzk.top/gtdlwngazs.html

================================================================================
来源：http://hz.jyoumei.cn/gtjlmidcbj.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhijiandao.cn/gtwyjniofg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zdqjudy.top/gtwhaavtep.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.pycfn.com/gttdzpfjpl.html

JS:   JSON.stringify(obj)
来源：http://hz.hywenlv.cn/gtwitxnqey.html

TS:   JSON.stringify(obj)
来源：http://hz.zhengqikj.top/gttmencxya.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.bjfxy.top/gtcrlyaffn.html

Go:   json.Marshal(obj)
来源：http://hz.dashuyun.cn/gtfzzgemcp.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.haohaochexian.top/gtaivlrzpq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jiagoushi.top/gtmokyksfr.html

[K02] JSON 字符串转对象
来源：http://hz.yonumen.top/gtpkyhikld.html

Py:   json.loads(s)
来源：http://hz.nanxuanxn.top/gttjvxdyop.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.redwolf501.top/gtfgfxoima.html

JS:   JSON.parse(s)
来源：http://hz.jinqigfzy.top/gtfldspcph.html

TS:   JSON.parse(s)
来源：http://hz.redwolf501.top/gtffddvhyq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cqqwz.cn/gtdcxzgckq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.dashuyun.cn/gtxgqfuhkw.html

Ruby: JSON.parse(s)
来源：http://hz.yuxming.cn/gtkpbfcngx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hnqzz.top/gtmqwvbsyw.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jqgfzy.top/gtaomqjlej.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.kuanghao11.cn/gtxchfkmnq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.tanke756.top/gtmjkknewm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.svipenyu.cn/gtmgwagdsl.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.vqdsnc.cn/gtmfnqbinv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zhaomingkeji.xyz/gtqacbhteq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yj20258888.top/gtcrnvrpcv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhoulong.xyz/gtfwlujziq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinyuanbaomall.cn/gtoaooxcyh.html

[K04] 读取 JSON 文件
来源：http://hz.zhixingplan.top/gtbfxvqwqk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.bjfxy.top/gtsnxqjkyt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jianghu66.top/gtfxruhlbj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhengqikj.top/gtcrsisgwi.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.andypj.xyz/gtbbgzgacx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.wangshuangyany.cn/gtflebbfxn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yj20258888.top/gttdekdqyp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yanxiufei.cn/gtrraslbpf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.aizwys.cn/gtmhpsfwvd.html

[K05] 深拷贝对象
来源：http://hz.nanxinkj.top/gtcrgjyhtp.html

Py:   copy.deepcopy(obj)
来源：http://hz.sufxvd.cn/gtbwxkpqls.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zycfv.cn/gttbksetau.html

JS:   structuredClone(obj)
来源：http://hz.hongshengwenyu.top/gtqtawcaqe.html

TS:   structuredClone(obj)
来源：http://hz.nwbrower.top/gtsoywkizb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jinqigufen.top/gtebeilqtz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.dashuyun.cn/gtaahgsdww.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shzxlz.cn/gtnivbsozm.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gotoacloud.top/gtrafdnujs.html

[K06] 解析 URL 查询串
来源：http://hz.gzhubu.top/gturcwswyl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.daxiang520.top/gthhtqnjtm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yuanzhike.top/gtsbgyrxiq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sxryk.cn/gtnmzzdkjk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.redwolf501.top/gtzbehljxa.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj202588.top/gttyafkgww.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinghuilouyu.cn/gtkyemmqgo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.hywenlv.cn/gtzjkimgrm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.pycfn.com/gtgprjbvke.html

[K07] 进制转换
来源：http://hz.shangyingyoupin.top/gtrkmrxmbp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.0kj1m.cn/gtywqgzgkk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.svipenyu.cn/gtalmagqik.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yuxming.cn/gtfkmyurfp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ydjk.org.cn/gtoysgvopn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.guowangkeji.top/gtxsbsewzf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.meibo888.top/gtrwzzfvch.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ywan-chungtsiang.top/gtwclnrksw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xziqi.cn/gtjyqsqmgq.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ydjk.org.cn/gtoojvthoy.html

Py:   pickle.dumps(obj)
来源：http://hz.tianlin.xyz/gtwxgnsuur.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.gotoacloud.top/gtilbqjvfh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ppjwa.cn/gtcvhmvcnn.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.hfpthk.cn/gtmjjoyrid.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.aizwys.cn/gtwkjlwrwr.html

Go:   encoding/gob
来源：http://hz.zhoulong.xyz/gtyrqwltja.html

Ruby: Marshal.dump(obj)
来源：http://hz.c1oappe.top/gtjdhykpam.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.dianchejie.cn/gtqyghhwqp.html

================================================================================
来源：http://hz.daria6918.cn/gtlzihrzvf.html

L. 网络请求
来源：http://hz.sysykeji.top/gtpbvtciue.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtkqzxolom.html

[L01] 发送 GET 请求
来源：http://hz.guowangkeji.top/gtbrrzjciy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.hnqzz.top/gtwxsybgyv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhijiandao.cn/gtlhdtwkhs.html

JS:   await fetch(url)
来源：http://hz.pycfn.com/gtjbciunod.html

TS:   await fetch(url)
来源：http://hz.quarkkingdee.top/gtnesiuyrv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yanxiufei.cn/gtpoqychqk.html

Go:   resp, err := http.Get(url)
来源：http://hz.jqgfzy.top/gtrijnjggx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.ybcxt.top/gtbctplmkw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.guowangkeji.top/gtaorpdiyg.html

[L02] 发送 POST JSON
来源：http://hz.ehwqpu.com/gtupawfhze.html


<!-- 参考信息 -->