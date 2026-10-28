代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.tianlin.xyz/gtjzorzagv.html

Ruby: rescue ArgumentError => e
来源：http://hz.vqdsnc.cn/gtsbkhkvgv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jinqigfzy.top/gtnauvpmag.html

[H06] 可选值 / 空值安全访问
来源：http://hz.tianlin.xyz/gtnwyurxwi.html

Py:   value = d.get("k") or default
来源：http://hz.jiagoushi.top/gtxpeunbdx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jinghuilouyu.cn/gtrtbrezio.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.nwbrower.top/gtbhfbodjy.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.kuanghao11.cn/gtkoiupasl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.aizwys.cn/gtsobdmmjj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.tanke756.top/gtrdluxlzu.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhixingplan.top/gtgsmfquva.html

C#:   obj?.A?.B ?? default
来源：http://hz.yj202588.top/gtqhwqstad.html

[H07] 断言
来源：http://hz.yvedp.cn/gtqbwjtjyk.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj20258.top/gtzlhaqizk.html

PHP:  assert($x > 0);
来源：http://hz.sweek.top/gtyxmklmzh.html

JS:   console.assert(x > 0);
来源：http://hz.316326.xyz/gtgnlgfpus.html

TS:   console.assert(x > 0);
来源：http://hz.gzhubu.top/gtoukhcixb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.svipenyu.cn/gtnjagaxcq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gotoacloud.top/gtmcopfuvo.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.aizwys.cn/gtcbwbdvgr.html

C#:   Debug.Assert(x > 0);
来源：http://hz.chenjidiqi.icu/gtywxhqwvh.html

[H08] 获取错误信息与堆栈
来源：http://hz.yj20258.top/gtiqkgqimm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhixingplan.top/gtyujdliem.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ywan-chungtsiang.top/gtkraspfdx.html

JS:   e.message;  e.stack
来源：http://hz.dianchejie.cn/gthrcelnss.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gzhubu.top/gtkeztrygd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yvedp.cn/gtwteyfvuz.html

Go:   err.Error()
来源：http://hz.cucudq.cn/gtdjjnabjl.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhijiandao.cn/gtuttlluof.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ydzc1.top/gtkzrxhgzp.html

[H09] 带错误码的异常
来源：http://hz.jinqigfzy.top/gtpgmqralr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cheryme.top/gtvfhhosoz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gotoacloud.top/gtjuqfrvec.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.fzhhl.top/gtsizazepk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shuidangran.top/gteiwuwlhc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.sufxvd.cn/gtdacactzs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hfpthk.cn/gtcwhceeco.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sysykeji.top/gtgixdvahi.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cucudq.cn/gtqxpvshjl.html

[H10] 资源自动释放
来源：http://hz.daxiang520.top/gtiotczwxc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xziqi.cn/gtqkaxoqch.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj202588.top/gtjsdptbbj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sufxvd.cn/gtfyntetnr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dashuyun.cn/gtgosnmybm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yj20258888.top/gtjpjyjvgr.html

Go:   defer f.Close()
来源：http://hz.gotoacloud.top/gtjjuqvwxj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yangfankeji.com/gtvrwshkqp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtungvoqbz.html

================================================================================
来源：http://hz.sxryk.cn/gtvvmqmhkl.html

I. 正则表达式
来源：http://hz.yanxiufei.cn/gttdjyivsy.html

================================================================================
来源：http://hz.hfpthk.cn/gtzsxqcedx.html

[I01] 判断是否匹配
来源：http://hz.haohaochexian.top/gtlctgfarg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.52xcode.cn/gtspwwcebl.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.smart0.xyz/gtebecnxkq.html

JS:   /\d+/.test(s)
来源：http://hz.xylfe.cn/gtrzbpaosk.html

TS:   /\d+/.test(s)
来源：http://hz.9152youxi.cn/gtqvfeumod.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.316326.xyz/gtnzlpdgmd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shzxlz.cn/gtzfuikcvf.html

Ruby: s.match?(/\d+/)
来源：http://hz.hywenlv.cn/gtahofjblb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.havefunace.top/gtishodyxg.html

[I02] 提取所有匹配
来源：http://hz.fengsongda.top/gtevpkjfhm.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hywenlv.cn/gttjrnfcsm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.birdmap.top/gtoidguhyy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinqigfzy.top/gttrnnjfsz.html

TS:   s.match(/\d+/g)
来源：http://hz.jinqigufen.top/gtybgepxsp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.smart0.xyz/gtltxswhvv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hywenlv.cn/gtwofgvqjr.html

Ruby: s.scan(/\d+/)
来源：http://hz.hywenlv.cn/gtsynckhgk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jyoumei.cn/gtsodioaev.html

[I03] 提取捕获分组
来源：http://hz.jqgufenzy.top/gtaoflcdew.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yueranfly.top/gtzdccgemm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.sxryk.cn/gtisdqytdi.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.bjfxy.top/gtopbhavmn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ppjwa.cn/gtaeiexwhp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yongpay.top/gtefheedwu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ydjk.org.cn/gtujetlvqu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xuetiantiany.cn/gtidxsaspy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.9152youxi.cn/gtmcqougus.html

[I04] 正则替换
来源：http://hz.snrcjt.cn/gtmiantnmk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.haohaochexian.top/gtbcfrrkaf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hfpthk.cn/gthustbwtk.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.bjfxy.top/gtxvhawwqx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yuanzhike.top/gtrkiqbtqk.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xinyue.icu/gtchzuqlyi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.havefunace.top/gtupipqjlt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hongshengwenyu.top/gtcvpydnun.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ywan-chungtsiang.top/gtnufjzcmp.html

[I05] 按正则拆分
来源：http://hz.chenzaomai.com/gtcbudanmd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shanyushiyangkeji.top/gtrsdtfgff.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gotoacloud.top/gtjbiqtorz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.tanke756.top/gtebtkceqs.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xziqi.cn/gtbjwyilkb.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zdqjudy.top/gtedysejjj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhiwuduotai.top/gtatojxobg.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhongyouzk.top/gtynafgwsn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.snrcjt.cn/gtashuetfl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.sxryk.cn/gteztbtksu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xziqi.cn/gtskumqbih.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ybcxt.top/gtwerozmrh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinqigfzy.top/gthlriusdd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258888.top/gthlrplsha.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.aibaodan.cn/gtvuvcvvzl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.fengsongda.top/gtekrfoscj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.wangshuangyany.cn/gtfkyhlowa.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ydjk.org.cn/gtwmmdroqr.html

[I07] 忽略大小写与多行模式
来源：http://hz.snrcjt.cn/gtqojlhuaj.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shanyushiyangkeji.top/gtsjkhcpzi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xuanzx.com/gtzebvesck.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.kuanghao11.cn/gtuzgogeej.html

TS:   /error/gim
来源：http://hz.xylfe.cn/gtnkhutjbi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yonumen.top/gtlbvsrgco.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yuanzhike.top/gtngbglwre.html

Ruby: s.scan(/error/i)
来源：http://hz.daria6918.cn/gtzvarnwxw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.tanke756.top/gtsdkvvwra.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shanyushiyangtech.top/gtqbymhcuu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yj20258888.top/gtimxsoxym.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.feifeiyinyue.top/gtytinwcsz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cheryme.top/gtpbfvxpje.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gaohongyu789.top/gtcjbxqbxm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yj202588.top/gtzrkuowmy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ydjk.org.cn/gtlakpwyxi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.tianlin.xyz/gtaxabxyvq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.iojbl.cn/gtnkqxzlao.html

================================================================================
来源：http://hz.sxryk.cn/gtiukyhcpx.html

J. 日期与时间
来源：http://hz.0kj1m.cn/gtjjybpajs.html

================================================================================
来源：http://hz.cqqwz.cn/gtkmamriux.html

[J01] 获取当前时间
来源：http://hz.aibaodan.cn/gtphferpaj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yuanzhike.top/gtxlyganca.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.pengpengdd.cyou/gtikpeworg.html

JS:   new Date();  Date.now()
来源：http://hz.pengpengdd.cyou/gtijklnchp.html

TS:   new Date();  Date.now()
来源：http://hz.jinqigufen.top/gtxwhhvwei.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhijiandao.cn/gtreupkgzj.html

Go:   time.Now()
来源：http://hz.zhengqikj.top/gtmsscuisy.html

Ruby: Time.now
来源：http://hz.aibaodan.cn/gtvdiaxmzb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.daria6918.cn/gthrewiefd.html

[J02] 格式化输出
来源：http://hz.cucudq.cn/gtphnhcawr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guowangkeji.top/gtteyvmdxg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yanxiufei.cn/gtaudmfbyr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hnxiangtu.top/gtfptwsxle.html

TS:   d.toISOString()
来源：http://hz.tian-w.cn/gtnrprblxh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.feifeiyinyue.top/gtifskzoca.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhixingplan.top/gttnurpxzs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zdqjudy.top/gtuirhwazf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gaohongyu789.top/gtssmyghqz.html

[J03] 字符串解析为日期
来源：http://hz.ydzc1.top/gtghbcchmv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.tianlin.xyz/gtuzbiwpwp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zycfv.cn/gtqpdfzcbn.html

JS:   new Date("2024-01-02")
来源：http://hz.birdmap.top/gtraxkwyor.html

TS:   new Date("2024-01-02")
来源：http://hz.yj20258.top/gtrihqqnht.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhongyouzk.top/gtvhmrcqwy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.iojbl.cn/gtwghmmycv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenzaomai.com/gtufgdjnta.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.chenzaomai.com/gtdzsfykjr.html

[J04] 时间戳与日期互转
来源：http://hz.cheryme.top/gtwuyzcwwj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.fengsongda.top/gtwflzsssa.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.guowangkeji.top/gtfzpfszhl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.fzhhl.top/gtrsrmpjms.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yueranfly.top/gtyonjyggq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.iojbl.cn/gtskwvbhey.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yj20258.top/gtszyuxwex.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhixingplan.top/gtejknzwoe.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ppjwa.cn/gtpdggnpkw.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhoulong.xyz/gtfiywpfej.html

Py:   now + timedelta(days=7)
来源：http://hz.fzhhl.top/gtfuqpgbco.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yvedp.cn/gtpppovxae.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj202588.top/gtwobuwotg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yuxming.cn/gtxxtkggso.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.nanxinkj.top/gtrsdxlxsn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.52xcode.cn/gthhardlmp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gzhubu.top/gtqqamqspi.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.wangshuangyany.cn/gtqpghudlh.html

[J06] 计算两时间之差
来源：http://hz.gzhubu.top/gtsxjumdbx.html

Py:   (end - start).total_seconds()
来源：http://hz.yuxming.cn/gtsgipwfkl.html

PHP:  $end->diff($start)->days;
来源：http://hz.gotoacloud.top/gtgxorzlds.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.bjfxy.top/gtsbakludl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hongshengwenyu.top/gtsryxcgpm.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zycfv.cn/gtanskxajv.html

Go:   end.Sub(start).Hours()
来源：http://hz.shanyushiyangtech.top/gtrqnzysoc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hysaishi.cn/gtjetjeoui.html

C#:   (end - start).TotalSeconds
来源：http://hz.316326.xyz/gtnbnbvigx.html

[J07] 比较两个日期
来源：http://hz.dashuyun.cn/gtbddznghj.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtyhwdpakb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.fzhhl.top/gthmalnqfg.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hywenlv.cn/gtwbfgrcrr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhongyouzk.top/gtyuswhzhy.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zycfv.cn/gtpofbdnwv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.cucudq.cn/gtbmmbwwxu.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gtovzfstph.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yonumen.top/gtdfkdzqah.html

[J08] 提取年月日与星期
来源：http://hz.0kj1m.cn/gtuxvnueyj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hfpthk.cn/gtkmiafyzr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhaomingkeji.xyz/gtxylotxje.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yuxming.cn/gtbuszguhc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.guannengcc.top/gtbaxfdqym.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ydjk.org.cn/gtgbzezhda.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yangfankeji.com/gtfgbhyzrm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jqgfzy.top/gtnpegtvow.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.chenlongwang.top/gttkpfanbo.html

[J09] 时区处理
来源：http://hz.9152youxi.cn/gtelcoefge.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.pycfn.com/gtjueptrei.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.aizwys.cn/gthfrelnat.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dashuyun.cn/gtpqpxvnpx.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zycfv.cn/gtwghpexbd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ehwqpu.com/gtfwqrulfd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.tian-w.cn/gtpdklhfqq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinqigufen.top/gtzklcnoxw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sweek.top/gtkiikminl.html

[J10] 取今天 / 本月第一天
来源：http://hz.cdnleiting.top/gtytkxcbet.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ybcxt.top/gtuvcpbbzr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jlsjyb.cn/gtuxurvmga.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ybcxt.top/gtqitfscwi.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuxming.cn/gtggykdoyc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yj20258.top/gtkbbjzver.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shangyingyoupin.top/gtcrpmqnwi.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.feifeiyinyue.top/gtlkqeswso.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhaomingkeji.xyz/gtuewlxwer.html

================================================================================
来源：http://hz.sysykeji.top/gteuwtoabm.html

K. JSON 与序列化
来源：http://hz.jianghu66.top/gthirtlzix.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtpwmgzkpa.html

[K01] 对象转 JSON 字符串
来源：http://hz.yvedp.cn/gttxchvaqp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shanyushiyangkeji.top/gttnwtlsnn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jlsjyb.cn/gtiaceahqg.html

JS:   JSON.stringify(obj)
来源：http://hz.wangdashe.top/gtnrznklsf.html

TS:   JSON.stringify(obj)
来源：http://hz.jqgufenzy.top/gtxnanihuz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hnqzz.top/gtxtzwtkvc.html

Go:   json.Marshal(obj)
来源：http://hz.yangfankeji.com/gtmbojetvr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.52xcode.cn/gtbhqswvfg.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hfpthk.cn/gtmwnveglu.html

[K02] JSON 字符串转对象
来源：http://hz.zhoulong.xyz/gthidzpylh.html

Py:   json.loads(s)
来源：http://hz.cdnleiting.top/gtrkumditf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhiwuduotai.top/gtfiobzlns.html

JS:   JSON.parse(s)
来源：http://hz.quarkkingdee.top/gthqxxctbt.html

TS:   JSON.parse(s)
来源：http://hz.0kj1m.cn/gtkumcnpui.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gaohongyu789.top/gttqzesxkc.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gotoacloud.top/gtynisfxqe.html

Ruby: JSON.parse(s)
来源：http://hz.sysykeji.top/gtiuuxbhtd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hfpthk.cn/gtodjvfcsz.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hywenlv.cn/gtbiscguoz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yj202588.top/gtbhgyofft.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yuanzhike.top/gtakwnfiym.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.svipenyu.cn/gtbljuknxp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.daxiang520.top/gtwrmurguv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.havefunace.top/gtjhetfilo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yonumen.top/gtofyefgcg.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.aizwys.cn/gtwdmumyki.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hysaishi.cn/gtfgilhrvx.html

[K04] 读取 JSON 文件
来源：http://hz.chenzaomai.com/gthuihpaxf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.c1oappe.top/gtyazmtqrt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.kuanghao11.cn/gtidabcawh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jqgufenzy.top/gtesbyscbj.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ehwqpu.com/gtcwjyxbsj.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gotoacloud.top/gtbrfaxqrh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.gzhubu.top/gtaykythnp.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yanxiufei.cn/gtxwpbcuqg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ppjwa.cn/gtjuadapul.html

[K05] 深拷贝对象
来源：http://hz.zdqjudy.top/gtelveqsfi.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhoulong.xyz/gtdbwaxxlw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinqigufen.top/gtafwisppa.html

JS:   structuredClone(obj)
来源：http://hz.kuanghao11.cn/gtjmtilymp.html

TS:   structuredClone(obj)
来源：http://hz.shanyushiyangkeji.top/gtvdntcrxc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hnqzz.top/gtcpjulwuw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.redwolf501.top/gtuzhzcfre.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhoulong.xyz/gtodzayafd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yuanzhike.top/gtfqsidzbw.html

[K06] 解析 URL 查询串
来源：http://hz.ehwqpu.com/gtdzwtgapw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yueranfly.top/gtvmpikgzk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.iojbl.cn/gtsyzhwvlb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.pengpengdd.cyou/gtdwagdzna.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cucudq.cn/gtzzympgtj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jinghuilouyu.cn/gtcrvmgbeo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.andypj.xyz/gtsuzmobyt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.aibaodan.cn/gtauphjqre.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gaohongyu789.top/gtsslgmayi.html

[K07] 进制转换
来源：http://hz.yvedp.cn/gtvucqoaor.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ppjwa.cn/gtbfklwbwa.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.vqdsnc.cn/gtitkokcwq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.cheryme.top/gtcjoxfsam.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xinyue.icu/gtwzehqfyi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.dashuyun.cn/gtpnydydvx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.aizwys.cn/gtitefmnrv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.havefunace.top/gtxazvqjaa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.bjfxy.top/gtvixcaxyb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.dianchejie.cn/gtpwrgywap.html

Py:   pickle.dumps(obj)
来源：http://hz.yj202588.top/gtibsfiqbx.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhixingplan.top/gtyxxfkrah.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jiagoushi.top/gtpxybkwyd.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.9152youxi.cn/gttpuesmqm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.dashuyun.cn/gtrhzcsjph.html

Go:   encoding/gob
来源：http://hz.meibo888.top/gtsrpnwuft.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhengqikj.top/gtpaixxlnh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.zhixingplan.top/gtjoajjzon.html

================================================================================
来源：http://hz.smart0.xyz/gtvfdrffsh.html

L. 网络请求
来源：http://hz.dashuyun.cn/gtxqfughuw.html

================================================================================
来源：http://hz.mhx1999.top/gtwlkauqyf.html

[L01] 发送 GET 请求
来源：http://hz.c1oappe.top/gtwwpaafxq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zycfv.cn/gtrssewzeo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.ydzc1.top/gtpavanocg.html

JS:   await fetch(url)
来源：http://hz.shanyushiyangtech.top/gtldpkrdfz.html

TS:   await fetch(url)
来源：http://hz.xuanzx.com/gtucstinli.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.9152youxi.cn/gtaayokahu.html


<!-- 参考信息 -->