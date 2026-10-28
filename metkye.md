代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://hz.nanxinkj.top/gtwlopapst.html

C#:   class MyException : Exception {}
来源：http://hz.ivvv.top/gtiqrjexdq.html

[H05] 捕获特定类型
来源：http://hz.xziqi.cn/gtfuqpluev.html

Py:   except ValueError as e:
来源：http://hz.feifeiyinyue.top/gttdjgaqbu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.snrcjt.cn/gthumqkxot.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jinghuilouyu.cn/gtfwlwqtlf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cheryme.top/gtqswfdktt.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.meibo888.top/gtgshzxlvv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.redwolf501.top/gtistbdrgh.html

Ruby: rescue ArgumentError => e
来源：http://hz.jlsjyb.cn/gtnxoojlix.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.52xcode.cn/gtbmaikkfo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.wangshuangyany.cn/gtbwedfxzn.html

Py:   value = d.get("k") or default
来源：http://hz.guannengcc.top/gtlckkgkjg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.quarkkingdee.top/gtixkyfajc.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinyuanbaomall.cn/gthqbqpgfb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sysykeji.top/gtqodzbvyo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.pengpengdd.cyou/gtvwsisvxn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.birdmap.top/gtqyzfpjcg.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cdnleiting.top/gtjeihovnx.html

C#:   obj?.A?.B ?? default
来源：http://hz.cucudq.cn/gtvmexlini.html

[H07] 断言
来源：http://hz.kuanghao11.cn/gtfjbiucnq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ydzc1.top/gtklhtuhro.html

PHP:  assert($x > 0);
来源：http://hz.sxryk.cn/gtarxsiqis.html

JS:   console.assert(x > 0);
来源：http://hz.shanyushiyangkeji.top/gttghafzke.html

TS:   console.assert(x > 0);
来源：http://hz.shangyingyoupin.top/gtmerqotkj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.chenjidiqi.icu/gtbshqadgt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xinyue.icu/gtypjiolei.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tanke756.top/gtaaxlozxw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.dashuyun.cn/gtsozainhe.html

[H08] 获取错误信息与堆栈
来源：http://hz.cucudq.cn/gtaezylqkr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cashguo.top/gtryigccuq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinyuanbaomall.cn/gtfbadqyxl.html

JS:   e.message;  e.stack
来源：http://hz.zhoulong.xyz/gtellwahyc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hnqzz.top/gtgwtwpgpa.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yongpay.top/gtgoybuijj.html

Go:   err.Error()
来源：http://hz.nwbrower.top/gteyuffncv.html

Ruby: e.message;  e.backtrace
来源：http://hz.dashuyun.cn/gtrpveqbqa.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ydzc1.top/gtrykmyuab.html

[H09] 带错误码的异常
来源：http://hz.jqgufenzy.top/gtjnbxvfqk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hysaishi.cn/gtdtusmziz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yongpay.top/gtnmptqksc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.quarkkingdee.top/gttffbkzcf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.chenlongwang.top/gtowqhtkap.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.birdmap.top/gtacwdtkue.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.meibo888.top/gtjbnqqnpk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhaomingkeji.xyz/gtcifkdkxr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.dashuyun.cn/gtniddmgiw.html

[H10] 资源自动释放
来源：http://hz.xuanzx.com/gtlowopruc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.feifeiyinyue.top/gtnsogbmdt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hammf.cn/gtzfmwftho.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.bjfxy.top/gtgmulqfzl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenjidiqi.icu/gtyuuumhhq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.redwolf501.top/gttdsgsmyn.html

Go:   defer f.Close()
来源：http://hz.zdqjudy.top/gtxkyfvemm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhaomingkeji.xyz/gtcthjxkde.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zdqjudy.top/gttviihyrj.html

================================================================================
来源：http://hz.ppjwa.cn/gtyftvppoh.html

I. 正则表达式
来源：http://hz.yangfankeji.com/gtbbvmrnow.html

================================================================================
来源：http://hz.9152youxi.cn/gtbdritulg.html

[I01] 判断是否匹配
来源：http://hz.daria6918.cn/gtwqokihfq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhengqikj.top/gtigeqvofo.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.birdmap.top/gtxgmpcang.html

JS:   /\d+/.test(s)
来源：http://hz.ydzc1.top/gtdbamnpsh.html

TS:   /\d+/.test(s)
来源：http://hz.feifeiyinyue.top/gtekijvioj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hnxiangtu.top/gtgdxvqdnt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hnxiangtu.top/gtcdpxyyjo.html

Ruby: s.match?(/\d+/)
来源：http://hz.aibaodan.cn/gtmbolncux.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hnxiangtu.top/gthxrmlcmj.html

[I02] 提取所有匹配
来源：http://hz.ivvv.top/gtbawarhqo.html

Py:   re.findall(r"\d+", s)
来源：http://hz.chenlongwang.top/gtqvramcsn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.havefunace.top/gtytqejwrp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.feifeiyinyue.top/gtsqzntjva.html

TS:   s.match(/\d+/g)
来源：http://hz.ivvv.top/gtpujmhcmm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.svipenyu.cn/gtnwidmole.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.mhx1999.top/gthbzhbbtm.html

Ruby: s.scan(/\d+/)
来源：http://hz.52xcode.cn/gtxpjazaol.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shzxlz.cn/gtkwdtsstn.html

[I03] 提取捕获分组
来源：http://hz.0kj1m.cn/gtllmzfyfr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shanyushiyangtech.top/gtlqproivd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.daxiang520.top/gtqshpbonc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hammf.cn/gtdrzlmtqh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.mhx1999.top/gtyjlqexgn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shuidangran.top/gtcfzxpdoh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xinyue.icu/gtxruueebt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hammf.cn/gtvedpyrbs.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.aizwys.cn/gtzdchaasp.html

[I04] 正则替换
来源：http://hz.guannengcc.top/gtmsirtqyt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zdqjudy.top/gtvrpqytmi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhaomingkeji.xyz/gtkpgtxitx.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.tian-w.cn/gtxkrbqetl.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.dianchejie.cn/gtvvrceeeh.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yonumen.top/gtbzbxrqgv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cashguo.top/gtxqcwuwho.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jyoumei.cn/gtcqehpelm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.meibo888.top/gteaogumwh.html

[I05] 按正则拆分
来源：http://hz.xylfe.cn/gtkbnmivch.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.fengsongda.top/gteqkqabvk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gotoacloud.top/gthaqaggmm.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zdqjudy.top/gtqayjjuym.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.guowangkeji.top/gtzouejftg.html

Java: s.split("\\s*,\\s*")
来源：http://hz.9152youxi.cn/gthfuviefz.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.guannengcc.top/gtaoprcfve.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xziqi.cn/gttnzruvkb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jyoumei.cn/gtahhidktt.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.bjfxy.top/gtvegcoyhe.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinyuanbaomall.cn/gtrrrzrmug.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tian-w.cn/gtmfvowwmz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gaohongyu789.top/gtdxabodts.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yuxming.cn/gtmcamsruw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.birdmap.top/gtwkivxlfv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hnqzz.top/gteoeaoxnf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ydjk.org.cn/gtlzxwkdwi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.nwbrower.top/gtvflolrqt.html

[I07] 忽略大小写与多行模式
来源：http://hz.cashguo.top/gtmtsdqrvq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.birdmap.top/gtrctzunfe.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yueranfly.top/gtkstjcesi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.vqdsnc.cn/gtqxhznskr.html

TS:   /error/gim
来源：http://hz.hysaishi.cn/gtsdwvphtp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.0kj1m.cn/gthsvxqbpf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zycfv.cn/gtoclqdwvv.html

Ruby: s.scan(/error/i)
来源：http://hz.guowangkeji.top/gtxrftkhov.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.316326.xyz/gtzvggfnms.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.tianlin.xyz/gtbekinuaj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yj202588.top/gtbstdrffd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.vqdsnc.cn/gtswscwyqp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.havefunace.top/gttqwpoaib.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yonumen.top/gtjxkinoum.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.gotoacloud.top/gtoekuayep.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zycfv.cn/gtaekswple.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.havefunace.top/gtnvovrfwa.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.meibo888.top/gtuwoegser.html

================================================================================
来源：http://hz.jianghu66.top/gtsdmbljmf.html

J. 日期与时间
来源：http://hz.cucudq.cn/gtghgvcrot.html

================================================================================
来源：http://hz.xziqi.cn/gtclgitxhk.html

[J01] 获取当前时间
来源：http://hz.zhongyouzk.top/gtyqdojbxb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yongpay.top/gtiggthxsq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhoulong.xyz/gtbsmpmeuk.html

JS:   new Date();  Date.now()
来源：http://hz.xinyue.icu/gtbjfumbvm.html

TS:   new Date();  Date.now()
来源：http://hz.shanyushiyangtech.top/gtlpkqphpa.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zycfv.cn/gtevdnbfnn.html

Go:   time.Now()
来源：http://hz.aibaodan.cn/gtupghwoeu.html

Ruby: Time.now
来源：http://hz.shuidangran.top/gtkpnleghc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.gogol.net.cn/gtkhzifjpe.html

[J02] 格式化输出
来源：http://hz.yangfankeji.com/gtvofnrvkg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.quarkkingdee.top/gttxlikrxp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yongpay.top/gtnkewfhqa.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hammf.cn/gtjyuvftzi.html

TS:   d.toISOString()
来源：http://hz.guannengcc.top/gtwabhaylb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.cqqwz.cn/gtagtdxpiy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jqgufenzy.top/gtgxkxcopx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dashuyun.cn/gtlerneckv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ivvv.top/gtucxfyvld.html

[J03] 字符串解析为日期
来源：http://hz.316326.xyz/gtrurykeeg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hysaishi.cn/gtnlxrfxgx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xuanzx.com/gtudnzofzv.html

JS:   new Date("2024-01-02")
来源：http://hz.aibaodan.cn/gtdhrhcpam.html

TS:   new Date("2024-01-02")
来源：http://hz.haohaochexian.top/gtgtsmxzdw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cdnleiting.top/gtzhxdjmgx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.nwbrower.top/gtsozphojh.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinqigfzy.top/gtnziagfxg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.kuanghao11.cn/gtlcuyqlrq.html

[J04] 时间戳与日期互转
来源：http://hz.yonumen.top/gttfuxgxys.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ehwqpu.com/gtswgxlhcg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sxryk.cn/gtbhyoavsr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sysykeji.top/gtttqjpyeu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.havefunace.top/gtochgnwxf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.wangdashe.top/gtnxtpakpd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nanxuanxn.top/gtmuchoepz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.sysykeji.top/gtooxrjsrv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhengqikj.top/gtjfxlqsrb.html

[J05] 时间加减（加 7 天）
来源：http://hz.haohaochexian.top/gtpafqinkp.html

Py:   now + timedelta(days=7)
来源：http://hz.tianlin.xyz/gtmidclghq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.52xcode.cn/gttdqbbfzg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jlsjyb.cn/gtrlhnbyrc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangdashe.top/gtdbtebjae.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ehwqpu.com/gtjmnyxybz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.quarkkingdee.top/gtpoovzbmz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.aizwys.cn/gtpszgwydh.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yanxiufei.cn/gtbuqrlswv.html

[J06] 计算两时间之差
来源：http://hz.ydjk.org.cn/gtcufurkli.html

Py:   (end - start).total_seconds()
来源：http://hz.jiagoushi.top/gtbrslzwrj.html

PHP:  $end->diff($start)->days;
来源：http://hz.jianghu66.top/gtckjzktrf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhengqikj.top/gtkcswegbf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jyoumei.cn/gtxyyeeocj.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yuanzhike.top/gtcckutqej.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhixingplan.top/gtlnznbfce.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gotoacloud.top/gtylqqecmu.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhijiandao.cn/gttediopyr.html

[J07] 比较两个日期
来源：http://hz.smart0.xyz/gthmtgldku.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yj20258888.top/gttmiwmmbf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cheryme.top/gtwjtrxkmf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.tanke756.top/gtfkffefld.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gotoacloud.top/gtzrraptcq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yangfankeji.com/gtxwcklvoi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.9152youxi.cn/gtoaltjspi.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.nanxinkj.top/gtqjxgnash.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gzhubu.top/gtwtqgnuau.html

[J08] 提取年月日与星期
来源：http://hz.yj20258.top/gtrecddpiw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinghuilouyu.cn/gtxicykpsa.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.nwbrower.top/gthnybalcy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.haohaochexian.top/gtyhwsoczp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yueranfly.top/gtglctxfcl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yj202588.top/gtiqmxdoao.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.pengpengdd.cyou/gtebmbyspm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.nanxuanxn.top/gtikczjqns.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhijiandao.cn/gtcbawzqmm.html

[J09] 时区处理
来源：http://hz.c1oappe.top/gtelpmgkgk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.iojbl.cn/gteqhqqczz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cashguo.top/gthhafdntn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yueranfly.top/gtfgnvitlu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tianlin.xyz/gtgqnueiwr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.bjfxy.top/gtxykvgjaf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yueranfly.top/gtsetnfprt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.dashuyun.cn/gtjkybecvb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ywan-chungtsiang.top/gthpvpezau.html

[J10] 取今天 / 本月第一天
来源：http://hz.aizwys.cn/gtrzsoowjj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.tanke756.top/gtdvpbxezw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinqigufen.top/gtdyqigrak.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ybcxt.top/gtuqknlwfu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xuetiantiany.cn/gtdroftjiy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yonumen.top/gtzosmpawe.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhoulong.xyz/gtjtwpduwp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.pycfn.com/gtglskcgzn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gotoacloud.top/gtxuhrkmjz.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtdzxwegcc.html

K. JSON 与序列化
来源：http://hz.zhengqikj.top/gtnklmaiew.html

================================================================================
来源：http://hz.yj202588.top/gtflbpceqc.html

[K01] 对象转 JSON 字符串
来源：http://hz.yvedp.cn/gtfxykwqej.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.guannengcc.top/gttcisnllo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yonumen.top/gtatsonloe.html

JS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangkeji.top/gtltrjufyr.html

TS:   JSON.stringify(obj)
来源：http://hz.hammf.cn/gtquisnwoc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.gaohongyu789.top/gtcvektqbn.html

Go:   json.Marshal(obj)
来源：http://hz.zhijiandao.cn/gtehgamnaq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.c1oappe.top/gtqnkneenu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yuxming.cn/gtvvjbuonc.html

[K02] JSON 字符串转对象
来源：http://hz.svipenyu.cn/gtydcnwfja.html

Py:   json.loads(s)
来源：http://hz.haohaochexian.top/gtqlkzhqfh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhoulong.xyz/gtuhnpqgsl.html

JS:   JSON.parse(s)
来源：http://hz.jinqigfzy.top/gtzakqxoix.html

TS:   JSON.parse(s)
来源：http://hz.fzhhl.top/gtuacysaar.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.iojbl.cn/gtcaexcrir.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shanyushiyangkeji.top/gtuokdhqnl.html

Ruby: JSON.parse(s)
来源：http://hz.fzhhl.top/gtliglnsma.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xziqi.cn/gtgmbvechn.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.birdmap.top/gtwfvvppqx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cucudq.cn/gtyvrucevc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yongpay.top/gtwsrkitoc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.nanxuanxn.top/gtxvgbihsi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.fengsongda.top/gtjnkbkevn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shangyingyoupin.top/gtxemggdit.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.tianlin.xyz/gtjfzvfmjh.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jinqigfzy.top/gtxpjknyzp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cheryme.top/gtzehjmkwd.html

[K04] 读取 JSON 文件
来源：http://hz.tianlin.xyz/gtlyjphsfg.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.daria6918.cn/gtsbsnumqj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinqigufen.top/gtjwhtjehz.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.feifeiyinyue.top/gtcjteakxf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jlsjyb.cn/gtxotqdsbm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cqqwz.cn/gtorezcmja.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jlsjyb.cn/gtwyvpyvmk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.chenzaomai.com/gtlngmggbj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yueranfly.top/gtboygtyyj.html

[K05] 深拷贝对象
来源：http://hz.gotoacloud.top/gtkulrdkox.html

Py:   copy.deepcopy(obj)
来源：http://hz.nanxinkj.top/gtipnwjpin.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinghuilouyu.cn/gtmnqcudzk.html

JS:   structuredClone(obj)
来源：http://hz.0kj1m.cn/gtfbhoaubz.html

TS:   structuredClone(obj)
来源：http://hz.nanxuanxn.top/gtzwbwipur.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xuetiantiany.cn/gtcffzvkfa.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.cucudq.cn/gtjuxiuxix.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.ydjk.org.cn/gtcdzvvuse.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xuanzx.com/gtuqrbhvxb.html

[K06] 解析 URL 查询串
来源：http://hz.jinqigufen.top/gtasrfypsr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.tian-w.cn/gtyvkxjlqf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.pengpengdd.cyou/gtnjbuggxb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.52xcode.cn/gtlmgqhyrx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ehwqpu.com/gtwwrdmiut.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.52xcode.cn/gtbgtqbtju.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yanxiufei.cn/gthardkqqn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zdqjudy.top/gtiuttwuzn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xylfe.cn/gttfttmvph.html

[K07] 进制转换
来源：http://hz.jqgufenzy.top/gtdzohqyir.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yj20258888.top/gtwnqzaopt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.redwolf501.top/gthpwrldwk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhongyouzk.top/gtleabxzfa.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.nanxuanxn.top/gtfditjwga.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.zhiwuduotai.top/gtjbpohjho.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.aizwys.cn/gtflftvxpy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.tanke756.top/gtdsdrtove.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.redwolf501.top/gtpzckyfrm.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.bjfxy.top/gtnwdsljpu.html

Py:   pickle.dumps(obj)
来源：http://hz.xziqi.cn/gtfazkflyr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hysaishi.cn/gtpbatgwic.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.meibo888.top/gtjfpncrey.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ydzc1.top/gtbeuhyukn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hywenlv.cn/gthqstiacz.html

Go:   encoding/gob
来源：http://hz.smart0.xyz/gtygavbdwz.html

Ruby: Marshal.dump(obj)
来源：http://hz.ydjk.org.cn/gtumnpnkso.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.havefunace.top/gtgyfmredt.html

================================================================================
来源：http://hz.fzhhl.top/gtjlxgjlmg.html


<!-- 参考信息 -->