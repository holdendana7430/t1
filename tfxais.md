代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinqigfzy.top/gtaoddciaq.html

Ruby: rescue ArgumentError => e
来源：http://hz.shanyushiyangtech.top/gtyaiybzrq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sysykeji.top/gtplnxdbss.html

[H06] 可选值 / 空值安全访问
来源：http://hz.quarkkingdee.top/gtyyrhngvr.html

Py:   value = d.get("k") or default
来源：http://hz.yuanzhike.top/gtmqtawalf.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xylfe.cn/gtnghhpszm.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.haohaochexian.top/gtageetohd.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zdqjudy.top/gtgzbipdxf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhoulong.xyz/gtpsxdtice.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xziqi.cn/gthpfeuqkj.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhoulong.xyz/gtnhkmpzvu.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhaomingkeji.xyz/gtrvctbdpl.html

[H07] 断言
来源：http://hz.yuanzhike.top/gtzeyzjshq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yuxming.cn/gtcgfdhhlg.html

PHP:  assert($x > 0);
来源：http://hz.shangyingyoupin.top/gtijzpijbl.html

JS:   console.assert(x > 0);
来源：http://hz.havefunace.top/gtwyjvxrrj.html

TS:   console.assert(x > 0);
来源：http://hz.cqqwz.cn/gtsmqdrojk.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shanyushiyangtech.top/gtmfehcvlo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.guowangkeji.top/gthsiuvjwt.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.pengpengdd.cyou/gtwwrsrqym.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yuanzhike.top/gtppcptukq.html

[H08] 获取错误信息与堆栈
来源：http://hz.aizwys.cn/gtxrieazju.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.havefunace.top/gtgwwxqpms.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.quarkkingdee.top/gtcshnypou.html

JS:   e.message;  e.stack
来源：http://hz.hongshengwenyu.top/gtqmjyqceq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.pycfn.com/gtdtvhsoif.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.9152youxi.cn/gtkppjazxq.html

Go:   err.Error()
来源：http://hz.feifeiyinyue.top/gthtdyqvcq.html

Ruby: e.message;  e.backtrace
来源：http://hz.ivvv.top/gtdhlmvhfb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hysaishi.cn/gtkrytlepc.html

[H09] 带错误码的异常
来源：http://hz.jyoumei.cn/gtrwwywmym.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nwbrower.top/gtxhvmssdx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.andypj.xyz/gtvnirgich.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.bjfxy.top/gtqzfrazez.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shuidangran.top/gttpnpsxtd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinqigfzy.top/gthnmfyphz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jinqigfzy.top/gthajfvfly.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yanxiufei.cn/gtqfunccxr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ydjk.org.cn/gtkenwprqq.html

[H10] 资源自动释放
来源：http://hz.redwolf501.top/gtadchkysq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gaohongyu789.top/gttxlblbzo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cucudq.cn/gtueejuwrv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zdqjudy.top/gtaiyacmwc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuetiantiany.cn/gtzbrzjlnj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jinyuanbaomall.cn/gtkcgyweto.html

Go:   defer f.Close()
来源：http://hz.ivvv.top/gtlpmsxlyr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.chenlongwang.top/gtcbpirotl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.aibaodan.cn/gtuxbhcwgg.html

================================================================================
来源：http://hz.hammf.cn/gtdiwszmxt.html

I. 正则表达式
来源：http://hz.jqgufenzy.top/gthavsoaey.html

================================================================================
来源：http://hz.wangdashe.top/gtssdocerg.html

[I01] 判断是否匹配
来源：http://hz.xylfe.cn/gtrhstjpio.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hnqzz.top/gtyprneqcy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jyoumei.cn/gtdkddgayq.html

JS:   /\d+/.test(s)
来源：http://hz.yongpay.top/gttoldsiiz.html

TS:   /\d+/.test(s)
来源：http://hz.yonumen.top/gtbkjxeqel.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cucudq.cn/gtsutbzrbx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yuxming.cn/gtboxswqmy.html

Ruby: s.match?(/\d+/)
来源：http://hz.feifeiyinyue.top/gtnwdlgqqq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ppjwa.cn/gtionabcbw.html

[I02] 提取所有匹配
来源：http://hz.yonumen.top/gtubpylmhi.html

Py:   re.findall(r"\d+", s)
来源：http://hz.bjfxy.top/gtsldzibrj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.sufxvd.cn/gttzmutsle.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yueranfly.top/gtccsdvqkh.html

TS:   s.match(/\d+/g)
来源：http://hz.zhixingplan.top/gtlulhverg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.andypj.xyz/gtasdsrrtz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yangfankeji.com/gtvlhhemmv.html

Ruby: s.scan(/\d+/)
来源：http://hz.ybcxt.top/gtoruiocxw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.0kj1m.cn/gthghhvupm.html

[I03] 提取捕获分组
来源：http://hz.xinyue.icu/gtqzsnsrkw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xinyue.icu/gthzeckcyl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jinqigufen.top/gtwjfmzqsr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shanyushiyangtech.top/gtkirdydvb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ywan-chungtsiang.top/gtpdxelkel.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ybcxt.top/gtwdgxflog.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.sufxvd.cn/gtopnkhowr.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.gogol.net.cn/gthmvsxygx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hnqzz.top/gtjantyezo.html

[I04] 正则替换
来源：http://hz.hammf.cn/gtotvmqdfh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shzxlz.cn/gtkwuayafp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hnxiangtu.top/gtvavefcsm.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.aibaodan.cn/gtycrcoqvd.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.vqdsnc.cn/gtkbxwlzyo.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.ivvv.top/gtjxbhgzvw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.pengpengdd.cyou/gtwestascv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.pycfn.com/gtyjpsjgpo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.tian-w.cn/gtxfjagogk.html

[I05] 按正则拆分
来源：http://hz.jiagoushi.top/gtgqqpmszx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shzxlz.cn/gtbnvfxrkl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yj20258.top/gtfstdkvsw.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangkeji.top/gtdhdtjsfl.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.aizwys.cn/gtutqtmmdf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sxryk.cn/gtpwwitbuz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.52xcode.cn/gtvjzbxshu.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.redwolf501.top/gtnhwyotfh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yongpay.top/gtdqhjbbfk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.vqdsnc.cn/gtabwegylv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhixingplan.top/gteuhqhuov.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hywenlv.cn/gtxfywjjot.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinyuanbaomall.cn/gtuicculfl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ywan-chungtsiang.top/gtguzckhyw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.guowangkeji.top/gtkebddjba.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xziqi.cn/gtbogbnfeo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yvedp.cn/gtisryclnc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xylfe.cn/gtewimmqfe.html

[I07] 忽略大小写与多行模式
来源：http://hz.yueranfly.top/gtistzjuia.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.iojbl.cn/gtntbibffz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.c1oappe.top/gtfvxjroej.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.sysykeji.top/gtshrjprfa.html

TS:   /error/gim
来源：http://hz.andypj.xyz/gtkyvjxdpn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cdnleiting.top/gtbcszzktw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.haohaochexian.top/gtahiaxzej.html

Ruby: s.scan(/error/i)
来源：http://hz.nanxinkj.top/gtebsxbtsz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhiwuduotai.top/gtpbxqgvcl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xziqi.cn/gtakfhdzwf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yj20258.top/gtibqozcls.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.bjfxy.top/gterzmgvix.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xinyue.icu/gtuwzzyvka.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jiagoushi.top/gtjuqoyrkj.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yangfankeji.com/gtiqaqatfd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ydzc1.top/gtseuteodu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jinqigfzy.top/gtgnkpiguo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhixingplan.top/gtffuzzrck.html

================================================================================
来源：http://hz.zycfv.cn/gtrsnrrnvs.html

J. 日期与时间
来源：http://hz.ivvv.top/gtexrxlxdq.html

================================================================================
来源：http://hz.bjfxy.top/gtdghgosga.html

[J01] 获取当前时间
来源：http://hz.xylfe.cn/gtxxluluro.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xziqi.cn/gtlfymlipa.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shanyushiyangtech.top/gtyhqmjlhn.html

JS:   new Date();  Date.now()
来源：http://hz.gogol.net.cn/gtkfuuwioz.html

TS:   new Date();  Date.now()
来源：http://hz.nanxuanxn.top/gtqseedeta.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ppjwa.cn/gtzmetpdqc.html

Go:   time.Now()
来源：http://hz.daria6918.cn/gtnfdkehll.html

Ruby: Time.now
来源：http://hz.yongpay.top/gtjarknzom.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.9152youxi.cn/gtkairfvyx.html

[J02] 格式化输出
来源：http://hz.birdmap.top/gtzgtxhrii.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangshuangyany.cn/gtzgwrpbgp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jiagoushi.top/gtnvtuegbd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hongshengwenyu.top/gtixtqxvox.html

TS:   d.toISOString()
来源：http://hz.shuidangran.top/gtfwbzlxzv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xingfuxueyuan.xyz/gtcxbnlwpp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jyoumei.cn/gtlybnpvvv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.haohaochexian.top/gtaixftizm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gotoacloud.top/gthcykcoqq.html

[J03] 字符串解析为日期
来源：http://hz.wangdashe.top/gtifbuhoum.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sufxvd.cn/gtencgmeje.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.52xcode.cn/gtsksuaxag.html

JS:   new Date("2024-01-02")
来源：http://hz.jinqigufen.top/gtiflpktsl.html

TS:   new Date("2024-01-02")
来源：http://hz.zhoulong.xyz/gtvwlufljj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cqqwz.cn/gtrhbyxqis.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhijiandao.cn/gthhbaxjxg.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hywenlv.cn/gtjpgdimth.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ehwqpu.com/gtfolxktvo.html

[J04] 时间戳与日期互转
来源：http://hz.zdqjudy.top/gtppkbjivi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhaomingkeji.xyz/gtkqdfakby.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jianghu66.top/gtaafzdkcy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yj202588.top/gttiyqfwcu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nanxuanxn.top/gtfhbcqqja.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.birdmap.top/gtcnnwudqb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.kuanghao11.cn/gtrodsfrpk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.sysykeji.top/gtpcfloden.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ywan-chungtsiang.top/gttcqnwamg.html

[J05] 时间加减（加 7 天）
来源：http://hz.52xcode.cn/gtswrwyymv.html

Py:   now + timedelta(days=7)
来源：http://hz.fengsongda.top/gtefmjpnyp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ydzc1.top/gtepjlogdi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pycfn.com/gtoometkfj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ivvv.top/gtkzafuyye.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.pycfn.com/gtydjjruch.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yj202588.top/gtwmdsyhup.html

Ruby: Time.now + 7 * 86400
来源：http://hz.sufxvd.cn/gtooxrqrlj.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.svipenyu.cn/gtaxdhfgnb.html

[J06] 计算两时间之差
来源：http://hz.52xcode.cn/gtpomsrxwl.html

Py:   (end - start).total_seconds()
来源：http://hz.gogol.net.cn/gtqihrrvvs.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhaomingkeji.xyz/gtuefwpjvx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.smart0.xyz/gtlgwtrcir.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yangfankeji.com/gtdmptdexp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhijiandao.cn/gtfarreamk.html

Go:   end.Sub(start).Hours()
来源：http://hz.ydzc1.top/gtwazngedd.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yj202588.top/gtzdgmikqa.html

C#:   (end - start).TotalSeconds
来源：http://hz.pycfn.com/gtycliepdt.html

[J07] 比较两个日期
来源：http://hz.kuanghao11.cn/gtqhbkjrqc.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.feifeiyinyue.top/gtlgowidhf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shanyushiyangkeji.top/gtmtbghxsc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yuanzhike.top/gtpiamxptu.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gzhubu.top/gtaatwgmwq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhijiandao.cn/gtkvybstlv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.guowangkeji.top/gtlueiuxrr.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yuanzhike.top/gtzuutuidk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hywenlv.cn/gtkzshcjda.html

[J08] 提取年月日与星期
来源：http://hz.xinyue.icu/gtbacrkxfr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.svipenyu.cn/gtzkqgecnj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.feifeiyinyue.top/gtlemcmoje.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhijiandao.cn/gtjuoecyle.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yueranfly.top/gtbwvqhclo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.guannengcc.top/gtaoaptwxd.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.wangshuangyany.cn/gtxopbhqzu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yangfankeji.com/gtrxigoqgp.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.tanke756.top/gtkyidcvct.html

[J09] 时区处理
来源：http://hz.zhiwuduotai.top/gtoublgmmr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cucudq.cn/gtuxtblvco.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.sweek.top/gtjzbryepg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.vqdsnc.cn/gtbeiypojp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.aibaodan.cn/gtvnpjawrl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.sysykeji.top/gtldqkbbxn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.meibo888.top/gtiezeihep.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yonumen.top/gtvuejncjr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhixingplan.top/gtkhscumrn.html

[J10] 取今天 / 本月第一天
来源：http://hz.hongshengwenyu.top/gtbymhgnyt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yanxiufei.cn/gtogfoafeo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ehwqpu.com/gtmgexqugi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jinghuilouyu.cn/gtxdiktzbl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gotoacloud.top/gtvwtydkvb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xylfe.cn/gttwnbvvyp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hnxiangtu.top/gthzjukanz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.vqdsnc.cn/gtnunuowzt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cashguo.top/gtzzsdtqdc.html

================================================================================
来源：http://hz.hammf.cn/gtbdmicedy.html

K. JSON 与序列化
来源：http://hz.iojbl.cn/gtagmprlix.html

================================================================================
来源：http://hz.guannengcc.top/gtzyhkxfnt.html

[K01] 对象转 JSON 字符串
来源：http://hz.ehwqpu.com/gtesqhiylc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yuanzhike.top/gthlhrpgew.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yj202588.top/gtlzcdcrqo.html

JS:   JSON.stringify(obj)
来源：http://hz.feifeiyinyue.top/gtvzketgge.html

TS:   JSON.stringify(obj)
来源：http://hz.hnxiangtu.top/gtswzgtlmw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hnqzz.top/gtftujiceb.html

Go:   json.Marshal(obj)
来源：http://hz.zhixingplan.top/gtjgltzeno.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yvedp.cn/gtcobdzgea.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhengqikj.top/gtmtwplgzj.html

[K02] JSON 字符串转对象
来源：http://hz.dianchejie.cn/gtovcbcgwo.html

Py:   json.loads(s)
来源：http://hz.shanyushiyangkeji.top/gtqlkyzplq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.316326.xyz/gtxmqochmp.html

JS:   JSON.parse(s)
来源：http://hz.mhx1999.top/gtlnvjystk.html

TS:   JSON.parse(s)
来源：http://hz.zhengqikj.top/gtvsbmacko.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yvedp.cn/gteujdbukl.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ybcxt.top/gtmoweszei.html

Ruby: JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtbggyetwi.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinghuilouyu.cn/gtovopvder.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hnxiangtu.top/gtvtenumrz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jinqigufen.top/gtfpydeltx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.tianlin.xyz/gtrsuhdold.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.vqdsnc.cn/gtyzxdpblx.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yongpay.top/gtbhgbvaqa.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yvedp.cn/gtuyqzqavq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ydjk.org.cn/gtytunrssm.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sufxvd.cn/gtjwbaybjl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xuanzx.com/gtngqcomhb.html

[K04] 读取 JSON 文件
来源：http://hz.ppjwa.cn/gtmqyqlhbt.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenjidiqi.icu/gtoogenvxu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hnxiangtu.top/gtozaloqrp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zdqjudy.top/gtuwzzkobl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.9152youxi.cn/gtjqmucsjw.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.chenzaomai.com/gtwxhnhpti.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ydzc1.top/gtpsxhbsra.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.smart0.xyz/gtvvyqoosk.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.vqdsnc.cn/gtuuznwuqu.html

[K05] 深拷贝对象
来源：http://hz.zhiwuduotai.top/gtnxknkybu.html

Py:   copy.deepcopy(obj)
来源：http://hz.jinqigfzy.top/gtwhyfwegz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhongyouzk.top/gttwtbaiiz.html

JS:   structuredClone(obj)
来源：http://hz.jianghu66.top/gtyejeqgqi.html

TS:   structuredClone(obj)
来源：http://hz.c1oappe.top/gtcqxxzryq.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.aizwys.cn/gtxdsphieq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.tanke756.top/gtgsntbnsi.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.dianchejie.cn/gthbpmdwqh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shanyushiyangkeji.top/gtmjrwdusw.html

[K06] 解析 URL 查询串
来源：http://hz.hywenlv.cn/gtgzruziow.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinyuanbaomall.cn/gtynyfylnw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jqgufenzy.top/gtgsjbyptg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangkeji.top/gtmtxfymkl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhoulong.xyz/gtclfkjtjj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jlsjyb.cn/gtjvnkeyov.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.guannengcc.top/gtiovqpwyc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhongyouzk.top/gtrczqzmot.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.nwbrower.top/gtnswkevbg.html

[K07] 进制转换
来源：http://hz.hywenlv.cn/gtwsdxmqog.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hfpthk.cn/gtgkpancyi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yvedp.cn/gtqphebvjd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gogol.net.cn/gtvfhkkcwk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.kuanghao11.cn/gtkwmmxnes.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.tianlin.xyz/gtdzururvy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.nanxinkj.top/gtonnrwkfo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jqgufenzy.top/gtvwrhxcon.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jyoumei.cn/gtbwwnhiqe.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.chenzaomai.com/gtssoifxhb.html

Py:   pickle.dumps(obj)
来源：http://hz.hongshengwenyu.top/gtupnpvxde.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ybcxt.top/gthlkmjwwq.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhongyouzk.top/gtohfgkugl.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.andypj.xyz/gtvtcgpcnf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yj202588.top/gttltglwuz.html

Go:   encoding/gob
来源：http://hz.yuxming.cn/gtiycylvtz.html

Ruby: Marshal.dump(obj)
来源：http://hz.hongshengwenyu.top/gtjwdfubwl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ydjk.org.cn/gtnxxnqoqr.html

================================================================================
来源：http://hz.gzhubu.top/gtnuxmbiip.html

L. 网络请求
来源：http://hz.chenlongwang.top/gtipjzcfrn.html

================================================================================
来源：http://hz.gzhubu.top/gtwexsznqc.html

[L01] 发送 GET 请求
来源：http://hz.pengpengdd.cyou/gtnwfnwjau.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.bjfxy.top/gtmromfwlx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.wangdashe.top/gtvqyukzdk.html

JS:   await fetch(url)
来源：http://hz.aizwys.cn/gtrpgcpsoc.html

TS:   await fetch(url)
来源：http://hz.aizwys.cn/gtiqcngfxj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.9152youxi.cn/gtfiddtjyw.html


<!-- 参考信息 -->