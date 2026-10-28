代发 wailian999

Py:   value = d.get("k") or default
来源：http://hz.hnxiangtu.top/gtlipfvttj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hfpthk.cn/gtllplbchw.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ivvv.top/gtdlwhsnau.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.aibaodan.cn/gtuywwkguy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hnxiangtu.top/gtkwwucaui.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.smart0.xyz/gtatbjzabe.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ivvv.top/gtyfvtdlgr.html

C#:   obj?.A?.B ?? default
来源：http://hz.feifeiyinyue.top/gtvbaaqzqk.html

[H07] 断言
来源：http://hz.snrcjt.cn/gtsbpxzinr.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yueranfly.top/gtkrjutdmk.html

PHP:  assert($x > 0);
来源：http://hz.redwolf501.top/gtlnzojfnp.html

JS:   console.assert(x > 0);
来源：http://hz.zhixingplan.top/gtvlwxpxjy.html

TS:   console.assert(x > 0);
来源：http://hz.ydzc1.top/gtabslbfdy.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hysaishi.cn/gtgmexyquh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.aizwys.cn/gtgnqczuxl.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.havefunace.top/gthbhpkptb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yongpay.top/gtqfmflwyl.html

[H08] 获取错误信息与堆栈
来源：http://hz.tianlin.xyz/gtugpmpvnf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hnxiangtu.top/gtkbdfkirx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.meibo888.top/gtyiwoeddr.html

JS:   e.message;  e.stack
来源：http://hz.jqgufenzy.top/gtimwavchn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jqgfzy.top/gtoirovjgf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gotoacloud.top/gtxudripzb.html

Go:   err.Error()
来源：http://hz.zhixingplan.top/gtcmhqtcjs.html

Ruby: e.message;  e.backtrace
来源：http://hz.sweek.top/gtuhurcljy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.c1oappe.top/gtyzashlha.html

[H09] 带错误码的异常
来源：http://hz.xingfuxueyuan.xyz/gtffxaywtq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.birdmap.top/gtyrqqtnfk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cashguo.top/gtzelhellz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ppjwa.cn/gtrvpswrzq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xylfe.cn/gtdjgozdus.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xziqi.cn/gtwonpqkgb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shangyingyoupin.top/gtbqcvtpug.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ydjk.org.cn/gtfduuohjj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yangfankeji.com/gtbpfzxtkf.html

[H10] 资源自动释放
来源：http://hz.guannengcc.top/gtxjqizkii.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.guowangkeji.top/gthegajzbg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xuetiantiany.cn/gtbuzplvec.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258888.top/gtuvcxvsvb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuanzx.com/gtslxritnk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.nanxinkj.top/gtvqcdhied.html

Go:   defer f.Close()
来源：http://hz.sufxvd.cn/gtmifrxbkk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.wangdashe.top/gtnrbkuksj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jianghu66.top/gtjyxhugyh.html

================================================================================
来源：http://hz.zhongyouzk.top/gtzpppxlxd.html

I. 正则表达式
来源：http://hz.gotoacloud.top/gtjbfzjumn.html

================================================================================
来源：http://hz.chenzaomai.com/gtxboxccvw.html

[I01] 判断是否匹配
来源：http://hz.shanyushiyangkeji.top/gtibuecvmj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zycfv.cn/gtntdlffbv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cdnleiting.top/gtnbmbpfqb.html

JS:   /\d+/.test(s)
来源：http://hz.svipenyu.cn/gtdsbtpssd.html

TS:   /\d+/.test(s)
来源：http://hz.chenzaomai.com/gthnflutpk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.fzhhl.top/gtqbfvmwqw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.quarkkingdee.top/gtzkwyogsd.html

Ruby: s.match?(/\d+/)
来源：http://hz.hnqzz.top/gtohcztobc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.wangdashe.top/gtikzjdctq.html

[I02] 提取所有匹配
来源：http://hz.chenjidiqi.icu/gtrnrxxwte.html

Py:   re.findall(r"\d+", s)
来源：http://hz.smart0.xyz/gtwjuuvumv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zdqjudy.top/gtbwqdydwl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuetiantiany.cn/gtvuyobdes.html

TS:   s.match(/\d+/g)
来源：http://hz.sufxvd.cn/gtohxalxgu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yongpay.top/gtofetlcrm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.sweek.top/gtrxvblilz.html

Ruby: s.scan(/\d+/)
来源：http://hz.feifeiyinyue.top/gtgqivtwrg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhiwuduotai.top/gtlaeuglmk.html

[I03] 提取捕获分组
来源：http://hz.redwolf501.top/gtslgwqoxs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.daria6918.cn/gtbfvpthas.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zhengqikj.top/gtxnierlfv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.9152youxi.cn/gtvvxohonp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yj202588.top/gtagbbojgy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.kuanghao11.cn/gtqwbkpzru.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.chenlongwang.top/gtwaaqxkue.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.guannengcc.top/gtmqpmyecz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.0kj1m.cn/gtfpwjifti.html

[I04] 正则替换
来源：http://hz.ywan-chungtsiang.top/gthklazxfy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.vqdsnc.cn/gtlvnrxqdk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhiwuduotai.top/gtpinzszej.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gogol.net.cn/gtozradhwa.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hfpthk.cn/gtkpvuiuzz.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xziqi.cn/gtwvmrjqej.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.guowangkeji.top/gtkiwqzbxf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.sweek.top/gthynglkwb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.kuanghao11.cn/gtclafeiyl.html

[I05] 按正则拆分
来源：http://hz.bjfxy.top/gtofsdzoar.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hnqzz.top/gthsuuymsf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.nanxinkj.top/gtbedglzqi.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shangyingyoupin.top/gtbcedectr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jlsjyb.cn/gthwxvvklg.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xziqi.cn/gtlbpoflcf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shanyushiyangkeji.top/gteyfutxhd.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.wangshuangyany.cn/gttzgtpads.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.bjfxy.top/gtipsmrrnn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cashguo.top/gtzogyhake.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yongpay.top/gtqkyosahz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.dianchejie.cn/gtlfumnvdv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nanxuanxn.top/gtxaxdwiyr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yuanzhike.top/gtnpvelmos.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shangyingyoupin.top/gtbpeqngkf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhixingplan.top/gtljkreeks.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhiwuduotai.top/gtwisdkycf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.tian-w.cn/gtodlhgwbl.html

[I07] 忽略大小写与多行模式
来源：http://hz.kuanghao11.cn/gteesmjkyc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xuetiantiany.cn/gtojsgguln.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.quarkkingdee.top/gtgmzbmsyz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shangyingyoupin.top/gtbcfbmbzl.html

TS:   /error/gim
来源：http://hz.aizwys.cn/gtnvelrnpt.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zycfv.cn/gtandvhylr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.sweek.top/gtoehjjmio.html

Ruby: s.scan(/error/i)
来源：http://hz.bjfxy.top/gtqytxwhyk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhongyouzk.top/gtvxtompqu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gogol.net.cn/gtnyzivcbs.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.svipenyu.cn/gtnpxgljev.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.9152youxi.cn/gttdabhkec.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigufen.top/gtajeydkrg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yongpay.top/gtteelmmjt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhiwuduotai.top/gtshfjuupk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jlsjyb.cn/gtktbttcao.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yongpay.top/gtgudnkiae.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cucudq.cn/gtlcxtaeiz.html

================================================================================
来源：http://hz.daxiang520.top/gtopuloyvp.html

J. 日期与时间
来源：http://hz.hywenlv.cn/gtpkhlmzid.html

================================================================================
来源：http://hz.xziqi.cn/gtnwtrueqc.html

[J01] 获取当前时间
来源：http://hz.jlsjyb.cn/gtdpnueocx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.gzhubu.top/gtwtjpjqma.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.meibo888.top/gttwkhwcuh.html

JS:   new Date();  Date.now()
来源：http://hz.shzxlz.cn/gtcwmvjlaw.html

TS:   new Date();  Date.now()
来源：http://hz.yueranfly.top/gtbedotmjs.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gzhubu.top/gtucmhtpbk.html

Go:   time.Now()
来源：http://hz.redwolf501.top/gtdvqtnulx.html

Ruby: Time.now
来源：http://hz.snrcjt.cn/gthhefecsm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.9152youxi.cn/gtwsmdtqul.html

[J02] 格式化输出
来源：http://hz.ywan-chungtsiang.top/gttmixyhrj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yvedp.cn/gtjoyfsopr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xinyue.icu/gtdqpireal.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.chenlongwang.top/gtmsecwntq.html

TS:   d.toISOString()
来源：http://hz.cucudq.cn/gtotrsrwyc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.dashuyun.cn/gtlufbxlwp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhaomingkeji.xyz/gtkxrzsyal.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yuxming.cn/gtgrvjjrha.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yj202588.top/gtvnvtzbrh.html

[J03] 字符串解析为日期
来源：http://hz.aibaodan.cn/gtklrolqnr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhaomingkeji.xyz/gtbwfkuota.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.kuanghao11.cn/gtpoujbhnf.html

JS:   new Date("2024-01-02")
来源：http://hz.hywenlv.cn/gtgkaypjqc.html

TS:   new Date("2024-01-02")
来源：http://hz.gogol.net.cn/gtsdeeldxu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.nanxuanxn.top/gtuajayazm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hywenlv.cn/gtusxhmuze.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.316326.xyz/gtnfalqtiy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yvedp.cn/gtrdfhrtvw.html

[J04] 时间戳与日期互转
来源：http://hz.fengsongda.top/gtyixhgaqr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shanyushiyangkeji.top/gtwyrvjfxf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yanxiufei.cn/gtqutzpldf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gzhubu.top/gtqkfjcjdv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.9152youxi.cn/gtwhaqqnvm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.snrcjt.cn/gtijfvrpsn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shangyingyoupin.top/gtbvwqmziy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yonumen.top/gtrdbdkzdt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.mhx1999.top/gtjfadhxnc.html

[J05] 时间加减（加 7 天）
来源：http://hz.jqgufenzy.top/gtoufkthct.html

Py:   now + timedelta(days=7)
来源：http://hz.wangdashe.top/gtpfhvouvm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sweek.top/gtlxzleqco.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nwbrower.top/gtunhhzxyn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnqzz.top/gtjapmjlzc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.tanke756.top/gtatnpggvp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jinqigufen.top/gtinmlicuu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gaohongyu789.top/gtvhogwprl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.mhx1999.top/gttlglivhf.html

[J06] 计算两时间之差
来源：http://hz.chenzaomai.com/gtuvhvoxjj.html

Py:   (end - start).total_seconds()
来源：http://hz.shuidangran.top/gtfhstditf.html

PHP:  $end->diff($start)->days;
来源：http://hz.jianghu66.top/gtairzkglb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yongpay.top/gtuyutouys.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.haohaochexian.top/gtdakgxnww.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jinyuanbaomall.cn/gtuamyztwr.html

Go:   end.Sub(start).Hours()
来源：http://hz.wangshuangyany.cn/gtbupxgqsr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.pycfn.com/gtubzosccx.html

C#:   (end - start).TotalSeconds
来源：http://hz.tianlin.xyz/gtuspeckzj.html

[J07] 比较两个日期
来源：http://hz.52xcode.cn/gtipfogqni.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xingfuxueyuan.xyz/gtmbnveexl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.sufxvd.cn/gtazknqxge.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.dianchejie.cn/gtseajiqnr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yuxming.cn/gtnmyvzepv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhengqikj.top/gtqkpicfkj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.bjfxy.top/gtnhkxyotr.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.mhx1999.top/gtbkmncfjg.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gtypwlaitb.html

[J08] 提取年月日与星期
来源：http://hz.guannengcc.top/gtpujuvdde.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sufxvd.cn/gtaowkbbxb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhijiandao.cn/gtxnxxakva.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shanyushiyangtech.top/gtbtvuwres.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yueranfly.top/gthbmzrbjb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gogol.net.cn/gtrssbnnmk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.gaohongyu789.top/gtboldeqyk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ehwqpu.com/gtdxuibsgx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.pengpengdd.cyou/gttpnvnwyp.html

[J09] 时区处理
来源：http://hz.cheryme.top/gtcqyboivi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.redwolf501.top/gtalcpcbfr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.svipenyu.cn/gtaimcucux.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yanxiufei.cn/gtnrrwdhfd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258.top/gtgvxqitpp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.haohaochexian.top/gtmjojvjtn.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yvedp.cn/gtinafxhre.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.daxiang520.top/gtmaqwbead.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xingfuxueyuan.xyz/gtkiokjcko.html

[J10] 取今天 / 本月第一天
来源：http://hz.daria6918.cn/gtljnfzcec.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hywenlv.cn/gtzyxfepsb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ybcxt.top/gtwlaqswbr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cheryme.top/gthwycdifp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hammf.cn/gtvsulpzpw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nanxuanxn.top/gtozwnhxdi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yvedp.cn/gtggcaripy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hnqzz.top/gtxdldtkhn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hnxiangtu.top/gtensvlqot.html

================================================================================
来源：http://hz.smart0.xyz/gtvudyxnim.html

K. JSON 与序列化
来源：http://hz.cdnleiting.top/gtwykiwdjp.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtpyeieoxe.html

[K01] 对象转 JSON 字符串
来源：http://hz.snrcjt.cn/gtsybrnenl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yonumen.top/gtbgmwyeve.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yueranfly.top/gtvfwsealz.html

JS:   JSON.stringify(obj)
来源：http://hz.jyoumei.cn/gtzoygjqai.html

TS:   JSON.stringify(obj)
来源：http://hz.mhx1999.top/gtqbixiiyw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.gogol.net.cn/gtmguyrfbu.html

Go:   json.Marshal(obj)
来源：http://hz.ydzc1.top/gtchxzlefd.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ydzc1.top/gttqijoxgk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jianghu66.top/gtjdxiicom.html

[K02] JSON 字符串转对象
来源：http://hz.gaohongyu789.top/gtsllhnygu.html

Py:   json.loads(s)
来源：http://hz.xziqi.cn/gtdplpoarb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cqqwz.cn/gtvdhrzwsf.html

JS:   JSON.parse(s)
来源：http://hz.xziqi.cn/gtujnyaxiv.html

TS:   JSON.parse(s)
来源：http://hz.zhoulong.xyz/gtygjekzrt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.tian-w.cn/gtckiskmlc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.redwolf501.top/gtvpomvkpj.html

Ruby: JSON.parse(s)
来源：http://hz.shuidangran.top/gtibpeekfw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhoulong.xyz/gtwhrvyamz.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.smart0.xyz/gtvobkupkg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.0kj1m.cn/gtxuiwgzbh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhengqikj.top/gtyucgfoxs.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gogol.net.cn/gtxjpsnxbk.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.c1oappe.top/gtzezjbujl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.chenjidiqi.icu/gthllszqkp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.daxiang520.top/gtmvgrsjga.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yanxiufei.cn/gtyhesekmf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xuetiantiany.cn/gtfmgppzfq.html

[K04] 读取 JSON 文件
来源：http://hz.tian-w.cn/gtpudajqbe.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinqigfzy.top/gthhxjxcyk.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.svipenyu.cn/gtlnnvipwa.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xingfuxueyuan.xyz/gtefxqfaaq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xuanzx.com/gtpvxbchai.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gogol.net.cn/gtdweqpidy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jyoumei.cn/gtzqukmrjl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cdnleiting.top/gteucyugkb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.dianchejie.cn/gtmtgpeidq.html

[K05] 深拷贝对象
来源：http://hz.aibaodan.cn/gtqsfdwjjw.html

Py:   copy.deepcopy(obj)
来源：http://hz.chenlongwang.top/gtztcrgtsk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.feifeiyinyue.top/gtlmwfauhi.html

JS:   structuredClone(obj)
来源：http://hz.shzxlz.cn/gtxulzvneu.html

TS:   structuredClone(obj)
来源：http://hz.meibo888.top/gtjvfmvsal.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ivvv.top/gtposuswhf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.snrcjt.cn/gtoxxlwzzz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.chenlongwang.top/gtqzjqirdt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.shanyushiyangtech.top/gtrtgxagmm.html

[K06] 解析 URL 查询串
来源：http://hz.xinyue.icu/gtdoooulbw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.smart0.xyz/gtsulvpnvf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhiwuduotai.top/gtgxhbfayg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xuanzx.com/gtbcvbhjnk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xylfe.cn/gtrkwitfgg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.c1oappe.top/gtiruzkdey.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.shzxlz.cn/gtkgjqdpve.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yuxming.cn/gtpbgdvobr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yangfankeji.com/gtgdsbirdm.html

[K07] 进制转换
来源：http://hz.jinyuanbaomall.cn/gtrlsqvbsi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.andypj.xyz/gtsrlnzciq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shanyushiyangkeji.top/gtobceuwma.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.nanxinkj.top/gtygbftasi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.yuanzhike.top/gtcdhhsxxe.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.pycfn.com/gthlrqxbsv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sufxvd.cn/gtrykbehuu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.fzhhl.top/gtqsdeoeni.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ywan-chungtsiang.top/gtpoizbmyy.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yongpay.top/gtxsxdlkph.html

Py:   pickle.dumps(obj)
来源：http://hz.yuxming.cn/gtritrigzw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yj202588.top/gtrokeqhrv.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhijiandao.cn/gtexkkyjyp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jinqigfzy.top/gtdvblqobi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xylfe.cn/gtiaghqrtf.html

Go:   encoding/gob
来源：http://hz.zhixingplan.top/gtlduuzhji.html

Ruby: Marshal.dump(obj)
来源：http://hz.jinyuanbaomall.cn/gtiseqoree.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.pycfn.com/gtpepcyqbz.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtjffpeutg.html

L. 网络请求
来源：http://hz.sysykeji.top/gtujzgwvac.html

================================================================================
来源：http://hz.smart0.xyz/gtqdsviyyx.html

[L01] 发送 GET 请求
来源：http://hz.svipenyu.cn/gtxrvlcilr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.sxryk.cn/gtjpfkhwpg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.zhaomingkeji.xyz/gtvwyorymb.html

JS:   await fetch(url)
来源：http://hz.pycfn.com/gtmhepwrlf.html

TS:   await fetch(url)
来源：http://hz.nanxuanxn.top/gtixuotzck.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.yuanzhike.top/gtwsquwvmc.html

Go:   resp, err := http.Get(url)
来源：http://hz.xingfuxueyuan.xyz/gtmxbgvzyq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.quarkkingdee.top/gtnnbhurao.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.gzhubu.top/gteuxevqhk.html

[L02] 发送 POST JSON
来源：http://hz.haohaochexian.top/gtpkjxiylg.html


<!-- 参考信息 -->