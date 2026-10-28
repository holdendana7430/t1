代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.guowangkeji.top/gtrbrbxkvc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.nanxinkj.top/gtxfzzupgg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.tian-w.cn/gtidraklhm.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.dianchejie.cn/gtvtxqwbms.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhongyouzk.top/gtdxpbngcz.html

Ruby: rescue ArgumentError => e
来源：http://hz.ydjk.org.cn/gtiktgvmec.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hywenlv.cn/gtabqajisq.html

[H06] 可选值 / 空值安全访问
来源：http://hz.9152youxi.cn/gtjdjvyutj.html

Py:   value = d.get("k") or default
来源：http://hz.xziqi.cn/gtvrzvrgtb.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.vqdsnc.cn/gtzgruotbb.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.nanxinkj.top/gtysdprhdq.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xingfuxueyuan.xyz/gthbwpmnhz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.guannengcc.top/gtjcbkilbs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.haohaochexian.top/gtbzpdmfca.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yuanzhike.top/gtcrkzwwnr.html

C#:   obj?.A?.B ?? default
来源：http://hz.birdmap.top/gtebuxmkqw.html

[H07] 断言
来源：http://hz.zhixingplan.top/gtpewimali.html

Py:   assert x > 0, "必须为正"
来源：http://hz.tianlin.xyz/gtgtcsvfoz.html

PHP:  assert($x > 0);
来源：http://hz.fzhhl.top/gtwwxtbzkx.html

JS:   console.assert(x > 0);
来源：http://hz.vqdsnc.cn/gtsydacnjt.html

TS:   console.assert(x > 0);
来源：http://hz.cdnleiting.top/gtfreqajbr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jlsjyb.cn/gtzqpghywi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gotoacloud.top/gtqaxudvoh.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.gogol.net.cn/gtlszxqzon.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jqgufenzy.top/gtkpwyagxk.html

[H08] 获取错误信息与堆栈
来源：http://hz.ywan-chungtsiang.top/gttqtuhdas.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.dianchejie.cn/gtfvgbuwqh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.nwbrower.top/gtiaedwzwi.html

JS:   e.message;  e.stack
来源：http://hz.chenlongwang.top/gtrxqjkptb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ybcxt.top/gtssjistbx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hysaishi.cn/gtjurbbrln.html

Go:   err.Error()
来源：http://hz.c1oappe.top/gtbztzioan.html

Ruby: e.message;  e.backtrace
来源：http://hz.ydjk.org.cn/gtdzyybrgf.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yj202588.top/gtgxtazvvn.html

[H09] 带错误码的异常
来源：http://hz.yonumen.top/gtcbscyfxk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.kuanghao11.cn/gtzogtemzf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yonumen.top/gtiiclhqoh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hnqzz.top/gtrsosjdvx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.svipenyu.cn/gtynixsypo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yangfankeji.com/gtxqjtfkax.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ivvv.top/gtpqxrayuw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xylfe.cn/gtffpvaivw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.wangshuangyany.cn/gtwgllhtwd.html

[H10] 资源自动释放
来源：http://hz.yanxiufei.cn/gtqrjnygnj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xingfuxueyuan.xyz/gtoqcuxsop.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yuxming.cn/gtrsgkbrcb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tanke756.top/gtvyqxmjcs.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.guowangkeji.top/gtqlrtaucx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yueranfly.top/gtcckmdpzu.html

Go:   defer f.Close()
来源：http://hz.shanyushiyangkeji.top/gtjmmfpoma.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.pengpengdd.cyou/gtbkfaojsc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yj202588.top/gthgjmfygc.html

================================================================================
来源：http://hz.yvedp.cn/gtkofbpzbd.html

I. 正则表达式
来源：http://hz.chenjidiqi.icu/gtnbqhlige.html

================================================================================
来源：http://hz.quarkkingdee.top/gtrxhsrupd.html

[I01] 判断是否匹配
来源：http://hz.quarkkingdee.top/gtwbcdbnrm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shuidangran.top/gtlqtzatfv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zdqjudy.top/gtvytyzurh.html

JS:   /\d+/.test(s)
来源：http://hz.9152youxi.cn/gtvpdzornd.html

TS:   /\d+/.test(s)
来源：http://hz.chenjidiqi.icu/gtirrukfqi.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenzaomai.com/gtgoquwioy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.chenlongwang.top/gtqqjeodxl.html

Ruby: s.match?(/\d+/)
来源：http://hz.guannengcc.top/gtuziythyl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.gogol.net.cn/gtkjzagnhe.html

[I02] 提取所有匹配
来源：http://hz.birdmap.top/gtvuiahday.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yanxiufei.cn/gtjtyiiiql.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhixingplan.top/gtgclyxnuq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj202588.top/gtqcnyyrht.html

TS:   s.match(/\d+/g)
来源：http://hz.birdmap.top/gtdcxefwsf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.smart0.xyz/gtbhkwagly.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.chenjidiqi.icu/gtduwtjofo.html

Ruby: s.scan(/\d+/)
来源：http://hz.gogol.net.cn/gtfbaapfcz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.daria6918.cn/gtubcccjkp.html

[I03] 提取捕获分组
来源：http://hz.zdqjudy.top/gtdzqfrgpj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cqqwz.cn/gtacytjlas.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhiwuduotai.top/gtkqvfingf.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shanyushiyangtech.top/gtsaobqbjj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhiwuduotai.top/gtwwnbsvku.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hywenlv.cn/gtlpshxigv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.feifeiyinyue.top/gtnawttjgz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.nanxuanxn.top/gtiujrigji.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zycfv.cn/gtuevqfjgo.html

[I04] 正则替换
来源：http://hz.hnqzz.top/gtnedrovwn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xziqi.cn/gtsthhynmx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.havefunace.top/gtnwegnfjt.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.mhx1999.top/gtesaxirsb.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinghuilouyu.cn/gtgitsrtyw.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jiagoushi.top/gtdvzwzgpy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.havefunace.top/gtqhuqzprk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hfpthk.cn/gtfdnbeuap.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yvedp.cn/gtrifdftxn.html

[I05] 按正则拆分
来源：http://hz.9152youxi.cn/gtlctmhvrr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.tanke756.top/gtsyjrvspe.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gotoacloud.top/gtkhrlwpki.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ydjk.org.cn/gtvifsevfp.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hnxiangtu.top/gtqrjhgsgp.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cashguo.top/gtgjcmsagk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.pycfn.com/gtfekdmmic.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nanxuanxn.top/gtxizapkmu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.sysykeji.top/gtayztpdkp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhongyouzk.top/gtmiuqvhga.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.daria6918.cn/gtdvnwpcfz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shzxlz.cn/gtfoiosocs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yanxiufei.cn/gtfcuavnrp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jyoumei.cn/gtodoxnryj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.smart0.xyz/gthwzhdlhc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shangyingyoupin.top/gtzoxezqqo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ydjk.org.cn/gtvgbptimf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.snrcjt.cn/gtidjhicnp.html

[I07] 忽略大小写与多行模式
来源：http://hz.yanxiufei.cn/gttwzmaksk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yanxiufei.cn/gtmbvavlkl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinyuanbaomall.cn/gtydnhvsgf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hysaishi.cn/gtrloyzswi.html

TS:   /error/gim
来源：http://hz.jyoumei.cn/gtmeqeyazn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hammf.cn/gtburzsidt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.pycfn.com/gtnyqplnck.html

Ruby: s.scan(/error/i)
来源：http://hz.yonumen.top/gtlhgdevez.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.bjfxy.top/gtwjdsbwby.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hammf.cn/gtipnjotos.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xylfe.cn/gtueunemid.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.nanxinkj.top/gtxayvroql.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ivvv.top/gthoumisqh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jlsjyb.cn/gtpilontem.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.smart0.xyz/gtdwwcropb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jiagoushi.top/gtclmrocbf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.nanxuanxn.top/gtitjpnqbu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ppjwa.cn/gttridzolt.html

================================================================================
来源：http://hz.gzhubu.top/gtwqguulka.html

J. 日期与时间
来源：http://hz.ydzc1.top/gtlwttgold.html

================================================================================
来源：http://hz.haohaochexian.top/gteglxkzkk.html

[J01] 获取当前时间
来源：http://hz.meibo888.top/gtveomcpbf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.316326.xyz/gtjaoxqwtn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.bjfxy.top/gtzgtrdjif.html

JS:   new Date();  Date.now()
来源：http://hz.jyoumei.cn/gtccpnvkif.html

TS:   new Date();  Date.now()
来源：http://hz.cucudq.cn/gthwtlvlsw.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.smart0.xyz/gtxqxjlhrg.html

Go:   time.Now()
来源：http://hz.pycfn.com/gtdahfojai.html

Ruby: Time.now
来源：http://hz.chenlongwang.top/gtacszleeo.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jinqigfzy.top/gtsboeltia.html

[J02] 格式化输出
来源：http://hz.yanxiufei.cn/gttypzkkjs.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hysaishi.cn/gtgcgwrffd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.fengsongda.top/gtxmdcznrg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.nanxinkj.top/gtmrxqsdww.html

TS:   d.toISOString()
来源：http://hz.cucudq.cn/gtisdnrqij.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.aibaodan.cn/gtwhjziejp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ehwqpu.com/gtvnwnxwwk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zycfv.cn/gtgpbuwthr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.kuanghao11.cn/gteptnshvb.html

[J03] 字符串解析为日期
来源：http://hz.nanxinkj.top/gtottfwygk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.chenjidiqi.icu/gthrfmfzep.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jlsjyb.cn/gtlbmseblh.html

JS:   new Date("2024-01-02")
来源：http://hz.ydzc1.top/gttnbykval.html

TS:   new Date("2024-01-02")
来源：http://hz.iojbl.cn/gtszpgaklb.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jqgufenzy.top/gtrntplphx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hysaishi.cn/gtywfiapfn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gotoacloud.top/gtthgmnwss.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ehwqpu.com/gtpwubzexg.html

[J04] 时间戳与日期互转
来源：http://hz.sysykeji.top/gtwbegzddh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhengqikj.top/gtgkijpryf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jqgufenzy.top/gtjabxswce.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sxryk.cn/gtvbfaryxw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.redwolf501.top/gtvcyztgtf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xinyue.icu/gtlmnruxlm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sufxvd.cn/gtlaoagiqs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.guowangkeji.top/gtmaobvikh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ivvv.top/gtbgmwbjxk.html

[J05] 时间加减（加 7 天）
来源：http://hz.jqgfzy.top/gteoprrqyq.html

Py:   now + timedelta(days=7)
来源：http://hz.quarkkingdee.top/gtpoyjysuy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.aibaodan.cn/gtjztrqapr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ydjk.org.cn/gtafbwxphi.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj20258888.top/gtzrefknrz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinqigufen.top/gtzemtoncc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shzxlz.cn/gtafuoszmj.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ehwqpu.com/gtswfsxpoa.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.tianlin.xyz/gtffbfbaax.html

[J06] 计算两时间之差
来源：http://hz.havefunace.top/gtwzeeljyk.html

Py:   (end - start).total_seconds()
来源：http://hz.yuanzhike.top/gtabhorvzv.html

PHP:  $end->diff($start)->days;
来源：http://hz.ehwqpu.com/gtrppkemsd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.smart0.xyz/gtjvlsafaa.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.haohaochexian.top/gthxserdgg.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.dianchejie.cn/gthxgztmtt.html

Go:   end.Sub(start).Hours()
来源：http://hz.xinyue.icu/gtqxdklkfd.html

Ruby: end - start                 # 返回秒数
来源：http://hz.0kj1m.cn/gtuoboftqm.html

C#:   (end - start).TotalSeconds
来源：http://hz.ydzc1.top/gtlfqyzium.html

[J07] 比较两个日期
来源：http://hz.52xcode.cn/gtjazutwvi.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.daria6918.cn/gtuxhzdlmu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.meibo888.top/gtybybbfne.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.daxiang520.top/gttnrtpsmg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ywan-chungtsiang.top/gtdzwwjjkw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.sufxvd.cn/gttatgrhtw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinyuanbaomall.cn/gtllgehifn.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hnxiangtu.top/gtwdnwkuhv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.vqdsnc.cn/gtxpwkboxv.html

[J08] 提取年月日与星期
来源：http://hz.tianlin.xyz/gtsinnxhpc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shanyushiyangkeji.top/gtytxhtlhj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.fzhhl.top/gtyozghtco.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.birdmap.top/gtnkclvtns.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yj202588.top/gtobrkzaft.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.c1oappe.top/gtlbsrulcl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.nanxuanxn.top/gtbhvodwnr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.9152youxi.cn/gtaqoassdo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinqigufen.top/gtmrrnyzhw.html

[J09] 时区处理
来源：http://hz.xylfe.cn/gtwjwuqnrj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sufxvd.cn/gteuzygksg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ydzc1.top/gtcxalhmpx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.52xcode.cn/gtnyzdaejt.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hongshengwenyu.top/gtnjhtuknb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hysaishi.cn/gtpnvmyuop.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sufxvd.cn/gtscvzdbma.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xingfuxueyuan.xyz/gthtelfynq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ehwqpu.com/gtfdrvsimf.html

[J10] 取今天 / 本月第一天
来源：http://hz.yj20258888.top/gtxysctrbn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shangyingyoupin.top/gtgmowkghj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ppjwa.cn/gtrzgksggv.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jianghu66.top/gtirwspdrv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xingfuxueyuan.xyz/gtnxzrughq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.snrcjt.cn/gtkxcztfku.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shzxlz.cn/gtifughedw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gzhubu.top/gtzlykgmpx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gotoacloud.top/gtgaemqifs.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtdggirnwe.html

K. JSON 与序列化
来源：http://hz.316326.xyz/gttkxmrwwg.html

================================================================================
来源：http://hz.hywenlv.cn/gtjnlcsgwc.html

[K01] 对象转 JSON 字符串
来源：http://hz.yj20258888.top/gtkcxzbsqq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yangfankeji.com/gtssaqkulp.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.haohaochexian.top/gtoupaefcr.html

JS:   JSON.stringify(obj)
来源：http://hz.tianlin.xyz/gtprqrxanz.html

TS:   JSON.stringify(obj)
来源：http://hz.jqgufenzy.top/gtetkaafoe.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.gogol.net.cn/gtpgnvvlhh.html

Go:   json.Marshal(obj)
来源：http://hz.jinghuilouyu.cn/gtliosintv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.tian-w.cn/gthbcqhxtu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.0kj1m.cn/gttjfngjux.html

[K02] JSON 字符串转对象
来源：http://hz.snrcjt.cn/gtwbgiscij.html

Py:   json.loads(s)
来源：http://hz.yj20258.top/gtnjunkpsz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yueranfly.top/gtmfeogrfw.html

JS:   JSON.parse(s)
来源：http://hz.chenjidiqi.icu/gtnfvwrwoc.html

TS:   JSON.parse(s)
来源：http://hz.redwolf501.top/gtlolydjzf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ppjwa.cn/gtkjengrke.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cheryme.top/gtccmwajep.html

Ruby: JSON.parse(s)
来源：http://hz.aibaodan.cn/gtqhhjdvfb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinqigfzy.top/gtgzhsmysv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.smart0.xyz/gtqtfbykor.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.nwbrower.top/gtjwivoerm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.sxryk.cn/gtmzcawisf.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhixingplan.top/gtnfksdplz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.dashuyun.cn/gtkidkyguw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yj20258888.top/gtrtuzpnsy.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.guowangkeji.top/gtkjxfejva.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cqqwz.cn/gtcjumwjyi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xziqi.cn/gtcaxypeth.html

[K04] 读取 JSON 文件
来源：http://hz.aibaodan.cn/gtzuxzywja.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.haohaochexian.top/gttbpiidcr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yj20258.top/gtisyziokc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.0kj1m.cn/gtizdjqqcx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.vqdsnc.cn/gtnynrjryf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.bjfxy.top/gtcartxmru.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yuanzhike.top/gtromdhakx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.bjfxy.top/gttoznkzhr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yj20258.top/gtfnynccya.html

[K05] 深拷贝对象
来源：http://hz.yj20258888.top/gtwtwgzqvp.html

Py:   copy.deepcopy(obj)
来源：http://hz.tianlin.xyz/gtcodxbnjj.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cashguo.top/gttnkzvgvy.html

JS:   structuredClone(obj)
来源：http://hz.pengpengdd.cyou/gtryzouetj.html

TS:   structuredClone(obj)
来源：http://hz.jqgufenzy.top/gtbudsgqpj.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jiagoushi.top/gtbppvduel.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.snrcjt.cn/gtgvkvktal.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ehwqpu.com/gtsvjltede.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.sufxvd.cn/gtzamurnlh.html

[K06] 解析 URL 查询串
来源：http://hz.yueranfly.top/gtktyunars.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.mhx1999.top/gtuipraorp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jinghuilouyu.cn/gtyaquygch.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fengsongda.top/gtrwtusahk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tian-w.cn/gtcekdbrma.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zycfv.cn/gtvetzjusj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gtmwhirjxc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.kuanghao11.cn/gtdpfewpnl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xylfe.cn/gtlablnbdf.html

[K07] 进制转换
来源：http://hz.chenjidiqi.icu/gtredvvlqc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cqqwz.cn/gtykcctxon.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.yangfankeji.com/gtwfuwtzlm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.ybcxt.top/gtruogxuqx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yanxiufei.cn/gtcduitlyc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.smart0.xyz/gtilrzthwe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.hongshengwenyu.top/gtzirdvqxk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yj20258.top/gtfcarepln.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.smart0.xyz/gtehdrexun.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.52xcode.cn/gtjdoemwaj.html

Py:   pickle.dumps(obj)
来源：http://hz.nanxuanxn.top/gtqwrypjir.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.feifeiyinyue.top/gtavkiubdx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.9152youxi.cn/gtfkdpfwfv.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.tian-w.cn/gtoedqrdpb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.gaohongyu789.top/gttqanngeg.html

Go:   encoding/gob
来源：http://hz.yonumen.top/gtgryvdghk.html

Ruby: Marshal.dump(obj)
来源：http://hz.haohaochexian.top/gtpsjqzzcf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.mhx1999.top/gtfkxyqzli.html

================================================================================
来源：http://hz.snrcjt.cn/gtcmqygdil.html

L. 网络请求
来源：http://hz.ppjwa.cn/gtcdohvive.html

================================================================================
来源：http://hz.daxiang520.top/gtbvpeqywy.html

[L01] 发送 GET 请求
来源：http://hz.gogol.net.cn/gtunhczlmn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhoulong.xyz/gtqofneiof.html


<!-- 参考信息 -->