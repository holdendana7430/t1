代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xuanzx.com/gtfcekkkuo.html

[H04] 自定义异常类型
来源：http://hz.kuanghao11.cn/gtworcajvr.html

Py:   class MyError(Exception): pass
来源：http://hz.fengsongda.top/gtkjddwmnz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhijiandao.cn/gtaqfhxmpd.html

JS:   class MyError extends Error {}
来源：http://hz.birdmap.top/gtvozpuxlr.html

TS:   class MyError extends Error {}
来源：http://hz.ydjk.org.cn/gtijfhjcae.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gzhubu.top/gtfuclttpc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hywenlv.cn/gttzcskeoq.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhijiandao.cn/gtsfktabpp.html

C#:   class MyException : Exception {}
来源：http://hz.nwbrower.top/gtxdxhuqkb.html

[H05] 捕获特定类型
来源：http://hz.tanke756.top/gtfwlcgxeu.html

Py:   except ValueError as e:
来源：http://hz.hammf.cn/gtfgjtebvp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.vqdsnc.cn/gtrngkavhz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xinyue.icu/gtquemnhfh.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jinqigufen.top/gtbnaydpqr.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.c1oappe.top/gtfymergkt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.guannengcc.top/gtpspqpeyt.html

Ruby: rescue ArgumentError => e
来源：http://hz.cdnleiting.top/gtvubuhvkf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ydjk.org.cn/gtmmwadgvi.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jinqigufen.top/gtgjhrohzm.html

Py:   value = d.get("k") or default
来源：http://hz.shangyingyoupin.top/gtyspduvcd.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xuetiantiany.cn/gtgthuyqga.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.havefunace.top/gtigddwvvw.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ydzc1.top/gtdmncvxzq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.wangdashe.top/gtrtabtsjt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hnxiangtu.top/gttiqxgagl.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinqigufen.top/gtcydmvvin.html

C#:   obj?.A?.B ?? default
来源：http://hz.dianchejie.cn/gtrjokccby.html

[H07] 断言
来源：http://hz.xziqi.cn/gtbunnscgj.html

Py:   assert x > 0, "必须为正"
来源：http://hz.aizwys.cn/gtyuwrmbmx.html

PHP:  assert($x > 0);
来源：http://hz.jinghuilouyu.cn/gtoqeurcgp.html

JS:   console.assert(x > 0);
来源：http://hz.52xcode.cn/gtrycclguj.html

TS:   console.assert(x > 0);
来源：http://hz.tianlin.xyz/gtxtcxqtjl.html

Java: assert x > 0 : "必须为正";
来源：http://hz.kuanghao11.cn/gtvklobroe.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.feifeiyinyue.top/gtfvrmsblo.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.aizwys.cn/gtaolkuyqx.html

C#:   Debug.Assert(x > 0);
来源：http://hz.gotoacloud.top/gtaiyiydqz.html

[H08] 获取错误信息与堆栈
来源：http://hz.wangshuangyany.cn/gthzlselmr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.aizwys.cn/gtgtqniofx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ydzc1.top/gtcuvuudct.html

JS:   e.message;  e.stack
来源：http://hz.gogol.net.cn/gtytpcxkly.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shanyushiyangtech.top/gtebkmuumm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.pycfn.com/gtlnwbmdcb.html

Go:   err.Error()
来源：http://hz.jyoumei.cn/gtvitwpysi.html

Ruby: e.message;  e.backtrace
来源：http://hz.wangdashe.top/gtryosyxwt.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ivvv.top/gtcyyvgrif.html

[H09] 带错误码的异常
来源：http://hz.nanxuanxn.top/gttlqomydn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhixingplan.top/gtjwidxkzr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yj20258888.top/gtpeubgrcv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jianghu66.top/gtdoztrzbi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yangfankeji.com/gtqlklyuwr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.nanxuanxn.top/gtxafwnabo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.nanxinkj.top/gtrgpjjbfu.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ybcxt.top/gtdzjrraqf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.aibaodan.cn/gtlkesnrcf.html

[H10] 资源自动释放
来源：http://hz.mhx1999.top/gtyvqrbthz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yanxiufei.cn/gtttpkhzoj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.wangshuangyany.cn/gtqawtshqx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.guowangkeji.top/gtswrsjigg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.birdmap.top/gtbgnwgacf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.svipenyu.cn/gtsjdacccv.html

Go:   defer f.Close()
来源：http://hz.xingfuxueyuan.xyz/gtqtufgiad.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.redwolf501.top/gtftexmijr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hammf.cn/gtvfmuvtpu.html

================================================================================
来源：http://hz.yj20258888.top/gtprulguli.html

I. 正则表达式
来源：http://hz.kuanghao11.cn/gtpwkmkjte.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtpkmbsaet.html

[I01] 判断是否匹配
来源：http://hz.xylfe.cn/gtxtpwubsk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.gaohongyu789.top/gteobvcvum.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhiwuduotai.top/gtvtmhzqsh.html

JS:   /\d+/.test(s)
来源：http://hz.sysykeji.top/gtgfuotnmy.html

TS:   /\d+/.test(s)
来源：http://hz.tianlin.xyz/gtrgbsfytj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.sweek.top/gttekxjmhn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.aizwys.cn/gtqsnswiko.html

Ruby: s.match?(/\d+/)
来源：http://hz.birdmap.top/gtfbjufxuj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinyuanbaomall.cn/gtblxlwwcl.html

[I02] 提取所有匹配
来源：http://hz.shzxlz.cn/gtuygnggkh.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hammf.cn/gtplfdextp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.smart0.xyz/gthxcpctcp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xylfe.cn/gtsshltqrr.html

TS:   s.match(/\d+/g)
来源：http://hz.yj202588.top/gthtkoyalu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yuxming.cn/gtwzehdebl.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yuxming.cn/gtjzsfubcu.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhiwuduotai.top/gtxhvscavi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.guowangkeji.top/gtglfuntls.html

[I03] 提取捕获分组
来源：http://hz.316326.xyz/gtocmofyyc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.pycfn.com/gtjdbxwcvz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.andypj.xyz/gtcuqbisfq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhaomingkeji.xyz/gtjzppfzaq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hfpthk.cn/gtpxgrwemh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xuetiantiany.cn/gtaodlyrtb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hfpthk.cn/gtswfknohn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hysaishi.cn/gttdzfhngq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.nwbrower.top/gtcjthzwkt.html

[I04] 正则替换
来源：http://hz.dashuyun.cn/gtebetcfai.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.redwolf501.top/gtowykfdgi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cashguo.top/gtreeivlpg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigfzy.top/gtdilumxad.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ehwqpu.com/gtshnwgnom.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.cqqwz.cn/gtjwrwohsj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.9152youxi.cn/gtzzqqhcnb.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.dianchejie.cn/gtpojnygoe.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.9152youxi.cn/gtzwafhpaa.html

[I05] 按正则拆分
来源：http://hz.feifeiyinyue.top/gtfmplpteb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shanyushiyangtech.top/gtsgdlsflz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xziqi.cn/gtjekllpjw.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.feifeiyinyue.top/gtjqbrjanl.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.wangdashe.top/gtfafqmllz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cqqwz.cn/gtjtiumwtb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.guowangkeji.top/gtutdecxax.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.tanke756.top/gtcjniyprh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xylfe.cn/gtlkwazcrq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zycfv.cn/gtnslsaztz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.guowangkeji.top/gtpcyssyab.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.guowangkeji.top/gteemrqvmx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xinyue.icu/gtddlhdeml.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenlongwang.top/gtldebwqtw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.gogol.net.cn/gtcapjjgan.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ivvv.top/gtbzpqjfdt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hysaishi.cn/gtddkrsuwv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yj20258888.top/gtnltzrrxl.html

[I07] 忽略大小写与多行模式
来源：http://hz.yj20258.top/gtuahgtrge.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ehwqpu.com/gtwesuxuot.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jqgufenzy.top/gtethzmwnp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ybcxt.top/gtfgzqevsz.html

TS:   /error/gim
来源：http://hz.zhaomingkeji.xyz/gtjnbdgfba.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hnxiangtu.top/gtnpnvzzyu.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.mhx1999.top/gtyubczwgp.html

Ruby: s.scan(/error/i)
来源：http://hz.kuanghao11.cn/gtfhiqovbq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ywan-chungtsiang.top/gtehoxsppb.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ydjk.org.cn/gtwnangmdp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xingfuxueyuan.xyz/gtydebvbpg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shanyushiyangkeji.top/gtdypguqay.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.smart0.xyz/gtwbcxkrho.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhaomingkeji.xyz/gtstsqvfap.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.gotoacloud.top/gthfyvtell.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yanxiufei.cn/gtcgijkgsi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.guannengcc.top/gtnkqgrdib.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shzxlz.cn/gtdaxalepe.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtzlwimmjl.html

J. 日期与时间
来源：http://hz.ywan-chungtsiang.top/gtqiuijtve.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtuancesvd.html

[J01] 获取当前时间
来源：http://hz.tian-w.cn/gtewkumtvj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.guannengcc.top/gtawqinbog.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.havefunace.top/gtnnacojkc.html

JS:   new Date();  Date.now()
来源：http://hz.zhiwuduotai.top/gtrfdutbqg.html

TS:   new Date();  Date.now()
来源：http://hz.dashuyun.cn/gtrxeichsu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinqigfzy.top/gtbxbiejlp.html

Go:   time.Now()
来源：http://hz.dianchejie.cn/gtckzkhagn.html

Ruby: Time.now
来源：http://hz.kuanghao11.cn/gtqpfsehld.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yj202588.top/gtuevdcsqh.html

[J02] 格式化输出
来源：http://hz.yj20258.top/gtczagofar.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yongpay.top/gtudtoiwgk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.fzhhl.top/gtdelawstd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hywenlv.cn/gthbodjdrt.html

TS:   d.toISOString()
来源：http://hz.yj202588.top/gtpqrzazhn.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.nanxuanxn.top/gtbpdordco.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.daria6918.cn/gtdnzfyfuo.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yuanzhike.top/gtsbbjyisw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.0kj1m.cn/gtgkhintsy.html

[J03] 字符串解析为日期
来源：http://hz.hnxiangtu.top/gtkkmlhogr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.iojbl.cn/gtrcvthnmr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.nwbrower.top/gtkyvfwnkj.html

JS:   new Date("2024-01-02")
来源：http://hz.ydzc1.top/gtgnuhgnaq.html

TS:   new Date("2024-01-02")
来源：http://hz.fengsongda.top/gtwigcaifq.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yj202588.top/gtxxygunoo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhongyouzk.top/gtaeunlsdd.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cqqwz.cn/gtnzxsjano.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hnxiangtu.top/gtqihwpiei.html

[J04] 时间戳与日期互转
来源：http://hz.sysykeji.top/gtvcfgwwvs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.wangshuangyany.cn/gtnkdmcdrc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.havefunace.top/gtshhgxboj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.c1oappe.top/gtlbncsjaa.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xziqi.cn/gtvstbwuog.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hfpthk.cn/gtyfpzwuly.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jqgfzy.top/gtvxibfezv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.snrcjt.cn/gtrppkaepw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jlsjyb.cn/gtuatiyuva.html

[J05] 时间加减（加 7 天）
来源：http://hz.jinqigfzy.top/gtadallftc.html

Py:   now + timedelta(days=7)
来源：http://hz.yonumen.top/gtwkdldgcl.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cdnleiting.top/gtscpfnxjh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ehwqpu.com/gtzrfpyvor.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.guowangkeji.top/gtyhswnzkp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.smart0.xyz/gtunyichwb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.smart0.xyz/gtxgaflebu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gzhubu.top/gtluemqroi.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xinyue.icu/gtblhsdqus.html

[J06] 计算两时间之差
来源：http://hz.nanxinkj.top/gtlefanurc.html

Py:   (end - start).total_seconds()
来源：http://hz.sxryk.cn/gtjermrcml.html

PHP:  $end->diff($start)->days;
来源：http://hz.hammf.cn/gtmedgogvi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sxryk.cn/gtdygpheew.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jianghu66.top/gtwsozbrdz.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.meibo888.top/gtqxcgkwhw.html

Go:   end.Sub(start).Hours()
来源：http://hz.ydzc1.top/gtnthtlhbs.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cdnleiting.top/gtdrjtunrs.html

C#:   (end - start).TotalSeconds
来源：http://hz.nanxinkj.top/gtdeitefku.html

[J07] 比较两个日期
来源：http://hz.ybcxt.top/gtozfbgibu.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.daxiang520.top/gtddregybv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.smart0.xyz/gtxvjpskmc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ppjwa.cn/gtudffwzjq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.tianlin.xyz/gtagrdijyi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nanxinkj.top/gtepekzppj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sxryk.cn/gtkyilavzf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xuetiantiany.cn/gtnrukfmkn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jqgufenzy.top/gttpdygqkd.html

[J08] 提取年月日与星期
来源：http://hz.52xcode.cn/gtchemijss.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.bjfxy.top/gtzsparzhk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.gaohongyu789.top/gtvjpwkqpa.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ydjk.org.cn/gtagfygnxz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinqigufen.top/gtswueifni.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.wangdashe.top/gtrkwxavoq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenjidiqi.icu/gtxlcgnmrx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yuanzhike.top/gtegkssjgc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.aizwys.cn/gtavtzquim.html

[J09] 时区处理
来源：http://hz.shanyushiyangtech.top/gtdmlblbxq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xinyue.icu/gtbtlskfac.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.sxryk.cn/gtzzbfkioh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.bjfxy.top/gtzrgqzgil.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.fzhhl.top/gtcvcaaarb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhiwuduotai.top/gtiijyvrgx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.316326.xyz/gtczenrlnc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yvedp.cn/gtakshybqw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jiagoushi.top/gtbhlebcdg.html

[J10] 取今天 / 本月第一天
来源：http://hz.gaohongyu789.top/gtntexrahj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sxryk.cn/gtjwukxphx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.dianchejie.cn/gtfwnbwcqb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xingfuxueyuan.xyz/gtbmdnsaxp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.wangdashe.top/gtllpsfzni.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.gogol.net.cn/gtjzhhrtlr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yvedp.cn/gtjplxaful.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yuanzhike.top/gtpcoxlnkp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.bjfxy.top/gtqzfvspbw.html

================================================================================
来源：http://hz.redwolf501.top/gtphjfbrii.html

K. JSON 与序列化
来源：http://hz.nanxinkj.top/gtgnjwztdo.html

================================================================================
来源：http://hz.shuidangran.top/gtbvbfhfiu.html

[K01] 对象转 JSON 字符串
来源：http://hz.svipenyu.cn/gtpzfhkvon.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhijiandao.cn/gtvpttzsrr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.chenjidiqi.icu/gtsupxmppg.html

JS:   JSON.stringify(obj)
来源：http://hz.yuanzhike.top/gtffmixxww.html

TS:   JSON.stringify(obj)
来源：http://hz.yvedp.cn/gtzrsosusj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xziqi.cn/gtrkwdfslf.html

Go:   json.Marshal(obj)
来源：http://hz.daria6918.cn/gtfucdgcvo.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jlsjyb.cn/gtnxwukmmp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xuetiantiany.cn/gtjxgrihih.html

[K02] JSON 字符串转对象
来源：http://hz.nwbrower.top/gtsnnrkygg.html

Py:   json.loads(s)
来源：http://hz.wangshuangyany.cn/gtvjlmwtyp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.iojbl.cn/gttnqqapae.html

JS:   JSON.parse(s)
来源：http://hz.smart0.xyz/gtylnazvfl.html

TS:   JSON.parse(s)
来源：http://hz.jqgfzy.top/gtphibfvym.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.daria6918.cn/gtpgppnncl.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.meibo888.top/gtajsaxfsv.html

Ruby: JSON.parse(s)
来源：http://hz.yj202588.top/gtstckzkfo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.quarkkingdee.top/gtrarvtfvx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.haohaochexian.top/gtamccdxxo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shzxlz.cn/gtxgyrrndg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinyuanbaomall.cn/gttywfflaa.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yuxming.cn/gtsfrfijks.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigfzy.top/gttmulqjft.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hnxiangtu.top/gtidmmhiys.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.kuanghao11.cn/gtsegmxwaq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yonumen.top/gtaaitowtz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.wangdashe.top/gthrffurhj.html

[K04] 读取 JSON 文件
来源：http://hz.zhijiandao.cn/gtmlzcvatu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.vqdsnc.cn/gtckovpxyo.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jiagoushi.top/gtsdxogoak.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.smart0.xyz/gtrpcukmug.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dianchejie.cn/gtlzcslpvf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.vqdsnc.cn/gtyvdcwwln.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhijiandao.cn/gtuypbtjlz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xuetiantiany.cn/gtavqfnqku.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tian-w.cn/gtukiduspm.html

[K05] 深拷贝对象
来源：http://hz.havefunace.top/gteosdsaxv.html

Py:   copy.deepcopy(obj)
来源：http://hz.shzxlz.cn/gtjwkljthf.html

PHP:  unserialize(serialize($obj));
来源：http://hz.nanxinkj.top/gtzfrplotu.html

JS:   structuredClone(obj)
来源：http://hz.yueranfly.top/gtneaezeyq.html

TS:   structuredClone(obj)
来源：http://hz.ywan-chungtsiang.top/gtpjbkbhar.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.chenzaomai.com/gtwseyhvyo.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zdqjudy.top/gtgsqubjjk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhengqikj.top/gtayvkxcbk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.haohaochexian.top/gtcmufjbbg.html

[K06] 解析 URL 查询串
来源：http://hz.jinghuilouyu.cn/gteclyumzc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cucudq.cn/gtiitfmrhy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.aibaodan.cn/gticendqjv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangtech.top/gtbhmngfvl.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hongshengwenyu.top/gtceclhvkb.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.shanyushiyangtech.top/gtaarslhci.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.wangdashe.top/gtbuugdigo.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.aizwys.cn/gtpebdjjna.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yvedp.cn/gtjtmfjbzh.html

[K07] 进制转换
来源：http://hz.zhengqikj.top/gtkvvfstln.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gteyutlkcw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.wangshuangyany.cn/gtusvydwlk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhoulong.xyz/gtphwwbzyi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.hnqzz.top/gtzeixxmzz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.vqdsnc.cn/gtbhaqxfpo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.chenjidiqi.icu/gtlhvmxjcl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.dashuyun.cn/gtnlbzkpdp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ehwqpu.com/gtwuklrggn.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.iojbl.cn/gtwyzpdcsi.html

Py:   pickle.dumps(obj)
来源：http://hz.aibaodan.cn/gtcyozcenx.html


<!-- 参考信息 -->