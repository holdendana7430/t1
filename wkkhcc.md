代发 wailian999

Py:   value = d.get("k") or default
来源：http://hz.kuanghao11.cn/gtcbqvycym.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gaohongyu789.top/gtlbjxleze.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.daxiang520.top/gtxpcjtdnj.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.wangdashe.top/gtjoxyzokk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.svipenyu.cn/gtrvjuzpiw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jinqigfzy.top/gtdwprkgwl.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xziqi.cn/gtfcdetssq.html

C#:   obj?.A?.B ?? default
来源：http://hz.ehwqpu.com/gttdqdygvq.html

[H07] 断言
来源：http://hz.hysaishi.cn/gtqeygnpsb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yangfankeji.com/gtqbplvhww.html

PHP:  assert($x > 0);
来源：http://hz.jianghu66.top/gtobbxhqfk.html

JS:   console.assert(x > 0);
来源：http://hz.cheryme.top/gtdrqmuajf.html

TS:   console.assert(x > 0);
来源：http://hz.yvedp.cn/gtruetvafb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.quarkkingdee.top/gttysvmcax.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jqgufenzy.top/gtlivtagqw.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tanke756.top/gtvjuygbkt.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jqgfzy.top/gtmpaviuge.html

[H08] 获取错误信息与堆栈
来源：http://hz.birdmap.top/gtosyclwcy.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gotoacloud.top/gtveyjkkqm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yueranfly.top/gtcdgaogyf.html

JS:   e.message;  e.stack
来源：http://hz.zhoulong.xyz/gtbwgdvhfo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cheryme.top/gtwbrsekbl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yj20258.top/gtzsmbmfbz.html

Go:   err.Error()
来源：http://hz.shuidangran.top/gtkhyjnwho.html

Ruby: e.message;  e.backtrace
来源：http://hz.xuetiantiany.cn/gtfnrtacro.html

C#:   e.Message;  e.StackTrace
来源：http://hz.andypj.xyz/gtydiwexkv.html

[H09] 带错误码的异常
来源：http://hz.ybcxt.top/gtdzrnfwcs.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhaomingkeji.xyz/gtmifoqksy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.pengpengdd.cyou/gtbzvmrqud.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shuidangran.top/gtnzxujpsj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xuanzx.com/gtottyypnp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinqigfzy.top/gttrbdzrgc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xuanzx.com/gtgziwdksn.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sxryk.cn/gtszvivmye.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xinyue.icu/gtjvyjzxwu.html

[H10] 资源自动释放
来源：http://hz.zhixingplan.top/gtdbszsibt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.aizwys.cn/gtgivuoumo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shanyushiyangkeji.top/gtqsqdlcmj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.andypj.xyz/gtuwsfdfxc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.haohaochexian.top/gtjminuaqr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.c1oappe.top/gteqwzjkwy.html

Go:   defer f.Close()
来源：http://hz.haohaochexian.top/gtfoeltioy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sufxvd.cn/gttixlnpho.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hnqzz.top/gtqgvrbgfh.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtryshyhmw.html

I. 正则表达式
来源：http://hz.hfpthk.cn/gtbmyflwyi.html

================================================================================
来源：http://hz.bjfxy.top/gtetyohljm.html

[I01] 判断是否匹配
来源：http://hz.xingfuxueyuan.xyz/gtumojwqvp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.aizwys.cn/gtxhomwmga.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.pengpengdd.cyou/gtiuxsbyoc.html

JS:   /\d+/.test(s)
来源：http://hz.yj20258.top/gtekshuofj.html

TS:   /\d+/.test(s)
来源：http://hz.shuidangran.top/gtkygrtwxv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xuanzx.com/gtbuonawpx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.c1oappe.top/gthbjrmzyo.html

Ruby: s.match?(/\d+/)
来源：http://hz.nanxinkj.top/gtinaztyyv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ydzc1.top/gtqvpxfkjl.html

[I02] 提取所有匹配
来源：http://hz.wangdashe.top/gtxiuovhfa.html

Py:   re.findall(r"\d+", s)
来源：http://hz.dianchejie.cn/gtyfvtrvnk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.chenzaomai.com/gtqvxwjdje.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinqigfzy.top/gtpsyogprd.html

TS:   s.match(/\d+/g)
来源：http://hz.ydjk.org.cn/gteybwqnqv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhixingplan.top/gtzgrlrkub.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.smart0.xyz/gtdphlpenq.html

Ruby: s.scan(/\d+/)
来源：http://hz.dashuyun.cn/gtalgizwtz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.pycfn.com/gtguuofmrw.html

[I03] 提取捕获分组
来源：http://hz.tanke756.top/gtyhhtsofp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jinghuilouyu.cn/gtzfvqwmua.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.cucudq.cn/gtviczmasc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.mhx1999.top/gtnyrkcxmn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.snrcjt.cn/gtqokjbble.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yanxiufei.cn/gtnqirjizn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ywan-chungtsiang.top/gtfzmoynrg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhaomingkeji.xyz/gtlbmmobtb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jinqigfzy.top/gtxkojxgly.html

[I04] 正则替换
来源：http://hz.cdnleiting.top/gtdfkzzzsg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gaohongyu789.top/gtlphrtxpw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.nanxuanxn.top/gtyxrffyof.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.fengsongda.top/gtafjoxyuy.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.redwolf501.top/gtagmxpkgn.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.wangdashe.top/gtxxtvlvgp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yvedp.cn/gtpvdpixer.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ywan-chungtsiang.top/gtwvxibsbh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.pengpengdd.cyou/gtiradcfll.html

[I05] 按正则拆分
来源：http://hz.yuxming.cn/gteimpyltr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jlsjyb.cn/gtkzfayavp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.nwbrower.top/gteiwvpmgo.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.guowangkeji.top/gtvrjbzfdc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jinyuanbaomall.cn/gtyeocwcph.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinyuanbaomall.cn/gtahldxuqp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shuidangran.top/gtpecppyrg.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jiagoushi.top/gttizpybdd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yj202588.top/gtbcfbtvhh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.meibo888.top/gtimbzngvb.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.meibo888.top/gtxxjkdjfs.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cucudq.cn/gtwivcvevm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhijiandao.cn/gtluazxamb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sufxvd.cn/gtuaysecep.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.wangshuangyany.cn/gtplvbavbv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yongpay.top/gtcldyussf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hnxiangtu.top/gtonvmssvj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ydjk.org.cn/gtzpqdaflj.html

[I07] 忽略大小写与多行模式
来源：http://hz.shanyushiyangkeji.top/gtypgynakx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.iojbl.cn/gturvsmzsx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yvedp.cn/gtlvbzbwxd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ydzc1.top/gtkckmtqny.html

TS:   /error/gim
来源：http://hz.9152youxi.cn/gtdtoselnq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hnqzz.top/gtxmfxdhct.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cdnleiting.top/gtlucnvirl.html

Ruby: s.scan(/error/i)
来源：http://hz.hammf.cn/gtbsfvpuva.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.bjfxy.top/gtickyuzhj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hammf.cn/gtzbmdcxgx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.svipenyu.cn/gtenrmglny.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yuanzhike.top/gtzjaakgsj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.wangdashe.top/gtbyadhuzo.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hfpthk.cn/gtreoouori.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shanyushiyangtech.top/gtbqslskeu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.feifeiyinyue.top/gttgfoctgu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.0kj1m.cn/gtgsqrbwwu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.nanxinkj.top/gtyrtcmcqw.html

================================================================================
来源：http://hz.tianlin.xyz/gtonazvmzv.html

J. 日期与时间
来源：http://hz.sweek.top/gtnuskmxvv.html

================================================================================
来源：http://hz.ehwqpu.com/gtaoormrji.html

[J01] 获取当前时间
来源：http://hz.sweek.top/gtbxscwdnq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.aibaodan.cn/gtrpifuzpz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.guannengcc.top/gtkdbqeylq.html

JS:   new Date();  Date.now()
来源：http://hz.jinghuilouyu.cn/gtjxcqiorg.html

TS:   new Date();  Date.now()
来源：http://hz.fengsongda.top/gttxbiovqb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.sweek.top/gtkkzvpjrx.html

Go:   time.Now()
来源：http://hz.tian-w.cn/gtxgljffia.html

Ruby: Time.now
来源：http://hz.guannengcc.top/gtfywujllx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yuxming.cn/gtodykqycy.html

[J02] 格式化输出
来源：http://hz.smart0.xyz/gtnrkxsodb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.quarkkingdee.top/gtzbmravhd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.aibaodan.cn/gtqkllgwgq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sysykeji.top/gtpbsewlmd.html

TS:   d.toISOString()
来源：http://hz.hywenlv.cn/gtyrvprcun.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.kuanghao11.cn/gtygfkvwqt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cdnleiting.top/gtjrtnipca.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.haohaochexian.top/gtowhzlfqu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.316326.xyz/gtskhdboew.html

[J03] 字符串解析为日期
来源：http://hz.hammf.cn/gtbvguxbcy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.aibaodan.cn/gtiybzflus.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shanyushiyangtech.top/gtptzmrhye.html

JS:   new Date("2024-01-02")
来源：http://hz.wangdashe.top/gtopgflcsv.html

TS:   new Date("2024-01-02")
来源：http://hz.nwbrower.top/gtnigpctxw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.mhx1999.top/gtudmupmfx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cdnleiting.top/gtordsgsry.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.guannengcc.top/gtnyxjtzpr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sufxvd.cn/gtybqihzvz.html

[J04] 时间戳与日期互转
来源：http://hz.mhx1999.top/gtpgvhmeev.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinqigufen.top/gtmzxjfcjk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.feifeiyinyue.top/gtsnswryfp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.9152youxi.cn/gttyxoexqj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhengqikj.top/gtrvmgztrg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhongyouzk.top/gtpnpqduno.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.guannengcc.top/gtmrcwkuxu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gotoacloud.top/gtvokdhkxf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.sxryk.cn/gtribshkwi.html

[J05] 时间加减（加 7 天）
来源：http://hz.birdmap.top/gtcpgloujg.html

Py:   now + timedelta(days=7)
来源：http://hz.yangfankeji.com/gtdluohohp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.iojbl.cn/gtasvsadwi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tanke756.top/gteyqzavzp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tian-w.cn/gtwiqhkhwj.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj202588.top/gtupzlahqk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhoulong.xyz/gtghbnshkr.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gaohongyu789.top/gtrvmiaiqo.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.gotoacloud.top/gtzdkhaxkw.html

[J06] 计算两时间之差
来源：http://hz.xuanzx.com/gthvkpkccv.html

Py:   (end - start).total_seconds()
来源：http://hz.zhoulong.xyz/gtvldiidwo.html

PHP:  $end->diff($start)->days;
来源：http://hz.andypj.xyz/gtrvsbtorb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hammf.cn/gtmvcnzgzt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.0kj1m.cn/gtqptwcbyt.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhiwuduotai.top/gtjknpmwgg.html

Go:   end.Sub(start).Hours()
来源：http://hz.ppjwa.cn/gtkdjpfnqq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yonumen.top/gtuxljbizb.html

C#:   (end - start).TotalSeconds
来源：http://hz.ybcxt.top/gtsnckifwx.html

[J07] 比较两个日期
来源：http://hz.haohaochexian.top/gtpnvqpcxl.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.316326.xyz/gtytlyiuzv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xingfuxueyuan.xyz/gtbktexthh.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.feifeiyinyue.top/gtmkbihigw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yanxiufei.cn/gtztavjxvp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.meibo888.top/gtsoqiojrn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhongyouzk.top/gtaaedgueu.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.meibo888.top/gtjhwbiecl.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yuanzhike.top/gtalkthfyf.html

[J08] 提取年月日与星期
来源：http://hz.mhx1999.top/gtxnvclkhb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.daria6918.cn/gtfevvzofz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.nwbrower.top/gtracvkvaw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.52xcode.cn/gtquejtqgn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ivvv.top/gtqmoktmur.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gogol.net.cn/gtbyftvnay.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yuanzhike.top/gtqbwrnnxo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zdqjudy.top/gtsfrycbrf.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yj202588.top/gtzsayxrie.html

[J09] 时区处理
来源：http://hz.xuetiantiany.cn/gtkcnaqnwu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sxryk.cn/gtxahnwvfm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.9152youxi.cn/gtjiwdhiwe.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.iojbl.cn/gthgogyqtf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sufxvd.cn/gtvjwytnbb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.chenlongwang.top/gtwjfphpjc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.snrcjt.cn/gtznjicskw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.quarkkingdee.top/gtzvmjokrr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.bjfxy.top/gttmtbvjwl.html

[J10] 取今天 / 本月第一天
来源：http://hz.chenjidiqi.icu/gtspjfflsk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.feifeiyinyue.top/gtynvhonrd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.tian-w.cn/gtukzlojjn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yvedp.cn/gthhntatws.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gogol.net.cn/gtcrbdfrxz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yvedp.cn/gtoqgqyyml.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.birdmap.top/gtzssnrpmx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xylfe.cn/gtsgotzelc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinqigufen.top/gtgrjdfkty.html

================================================================================
来源：http://hz.mhx1999.top/gtlszphmhw.html

K. JSON 与序列化
来源：http://hz.sufxvd.cn/gtdbkwrfmy.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtepijnmse.html

[K01] 对象转 JSON 字符串
来源：http://hz.daria6918.cn/gtwqlbffsm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.quarkkingdee.top/gtjplekvew.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhongyouzk.top/gtinriooar.html

JS:   JSON.stringify(obj)
来源：http://hz.guowangkeji.top/gtfogmhkiv.html

TS:   JSON.stringify(obj)
来源：http://hz.zycfv.cn/gttmfmyicx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cashguo.top/gtauwfrung.html

Go:   json.Marshal(obj)
来源：http://hz.0kj1m.cn/gtlxkykuwx.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shanyushiyangkeji.top/gtfbaznmee.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hongshengwenyu.top/gtjxuqjuvc.html

[K02] JSON 字符串转对象
来源：http://hz.zdqjudy.top/gtlwgpjnca.html

Py:   json.loads(s)
来源：http://hz.iojbl.cn/gtpyqurvbm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gotoacloud.top/gtmjvqbiny.html

JS:   JSON.parse(s)
来源：http://hz.jqgfzy.top/gtskzskzll.html

TS:   JSON.parse(s)
来源：http://hz.yvedp.cn/gtwwwszzgk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yj20258.top/gtaqufmmdq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shangyingyoupin.top/gtqmkeycmz.html

Ruby: JSON.parse(s)
来源：http://hz.jiagoushi.top/gtcszinxam.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ivvv.top/gtenqvviqr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yuanzhike.top/gtifnuzlks.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.havefunace.top/gtgijkmtet.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.wangshuangyany.cn/gtmmcfxgix.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xziqi.cn/gteettqqen.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.aibaodan.cn/gtvtskdckw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jqgfzy.top/gtfdpwivuq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.svipenyu.cn/gtgjcrfbpc.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hammf.cn/gtvghrimts.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.jinqigufen.top/gtpfxlgeii.html

[K04] 读取 JSON 文件
来源：http://hz.vqdsnc.cn/gtheurhqyb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xziqi.cn/gtpkeuxaoj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shzxlz.cn/gtrjztesmg.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tianlin.xyz/gtvcrvcrxb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnxiangtu.top/gtpnectwkk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.fengsongda.top/gtscgcqkcc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.snrcjt.cn/gtclhamiio.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ywan-chungtsiang.top/gtrcjyunfy.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.316326.xyz/gtlvxrnuiq.html

[K05] 深拷贝对象
来源：http://hz.zhiwuduotai.top/gtanvugcah.html

Py:   copy.deepcopy(obj)
来源：http://hz.nanxuanxn.top/gtejiwvkah.html

PHP:  unserialize(serialize($obj));
来源：http://hz.tanke756.top/gtxsisrejt.html

JS:   structuredClone(obj)
来源：http://hz.xingfuxueyuan.xyz/gtnrcdwexx.html

TS:   structuredClone(obj)
来源：http://hz.pycfn.com/gtplqkwlmu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.jqgufenzy.top/gtxovqncut.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.c1oappe.top/gtzfbccqwt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.mhx1999.top/gtigimurkg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ydzc1.top/gtnehcmirp.html

[K06] 解析 URL 查询串
来源：http://hz.chenjidiqi.icu/gteppkhwqi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.dashuyun.cn/gtmxunsyxt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.jianghu66.top/gtxgqfvnxr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhoulong.xyz/gtmzymtric.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cdnleiting.top/gtdrcajjrr.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xinyue.icu/gtzszetnyk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sufxvd.cn/gtzdoslrqy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yonumen.top/gtoqdbiaju.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.9152youxi.cn/gtzwopqgqg.html

[K07] 进制转换
来源：http://hz.meibo888.top/gthtauxrog.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.vqdsnc.cn/gtmojookps.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jqgfzy.top/gthlqbldzz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hammf.cn/gtfnvcsegh.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ivvv.top/gtavhxarec.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.gaohongyu789.top/gtpqazpqkk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jlsjyb.cn/gthminykcf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.cucudq.cn/gtgddlqxvv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.chenjidiqi.icu/gttozwwbgl.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.zdqjudy.top/gtxdnwyeuu.html

Py:   pickle.dumps(obj)
来源：http://hz.andypj.xyz/gtqatlvlyx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cucudq.cn/gtradcyxfx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ybcxt.top/gtlnkguxlu.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.jyoumei.cn/gtxysusbdj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yanxiufei.cn/gtcbwlgikv.html

Go:   encoding/gob
来源：http://hz.hammf.cn/gtcwzpgcgh.html

Ruby: Marshal.dump(obj)
来源：http://hz.wangshuangyany.cn/gtfzjkpzps.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.yueranfly.top/gtlloplpgj.html

================================================================================
来源：http://hz.sysykeji.top/gtesurbqmi.html

L. 网络请求
来源：http://hz.fengsongda.top/gtsluhqeji.html

================================================================================
来源：http://hz.iojbl.cn/gtgmttljbw.html

[L01] 发送 GET 请求
来源：http://hz.hnxiangtu.top/gtsllklzsi.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.jlsjyb.cn/gtuqwlzcht.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hnxiangtu.top/gtpbmaubeg.html

JS:   await fetch(url)
来源：http://hz.hongshengwenyu.top/gtefzqrcvd.html

TS:   await fetch(url)
来源：http://hz.52xcode.cn/gtzvoykxfe.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.haohaochexian.top/gtdhsgqgnx.html

Go:   resp, err := http.Get(url)
来源：http://hz.aizwys.cn/gtpurlkvmx.html

Ruby: Net::HTTP.get(URI(url))
来源：http://hz.nwbrower.top/gtusfffcxu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hz.hnqzz.top/gtruznxyay.html

[L02] 发送 POST JSON
来源：http://hz.shanyushiyangtech.top/gtzuurbphp.html


<!-- 参考信息 -->