代发 wailian999

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.guowangkeji.top/gtlwsfjrkh.html

Ruby: rescue ArgumentError => e
来源：http://hz.dashuyun.cn/gtirccqgjh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.andypj.xyz/gtebayllnb.html

[H06] 可选值 / 空值安全访问
来源：http://hz.mhx1999.top/gtliwaohad.html

Py:   value = d.get("k") or default
来源：http://hz.tanke756.top/gtodxpwnmj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ydzc1.top/gtsjjnbwcx.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.0kj1m.cn/gtlqbzsuxg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.birdmap.top/gtznptybak.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yvedp.cn/gtpvfmnseb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zycfv.cn/gtkhpysfnm.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cucudq.cn/gtlhkzojhh.html

C#:   obj?.A?.B ?? default
来源：http://hz.wangdashe.top/gtuhuifxmt.html

[H07] 断言
来源：http://hz.snrcjt.cn/gtoccgjbyq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.birdmap.top/gtspbtmoxq.html

PHP:  assert($x > 0);
来源：http://hz.nanxinkj.top/gtzimgmrch.html

JS:   console.assert(x > 0);
来源：http://hz.yanxiufei.cn/gtpakpepne.html

TS:   console.assert(x > 0);
来源：http://hz.hnxiangtu.top/gteqycjodb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.daria6918.cn/gtdwasyvlw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.wangdashe.top/gtlqcwhewz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.daria6918.cn/gthquclftl.html

C#:   Debug.Assert(x > 0);
来源：http://hz.feifeiyinyue.top/gtwbvqhgin.html

[H08] 获取错误信息与堆栈
来源：http://hz.feifeiyinyue.top/gtbcilfgtw.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yj20258.top/gtxcnzwpdj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinqigufen.top/gtqdruuzgt.html

JS:   e.message;  e.stack
来源：http://hz.yonumen.top/gtbajpxzwz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinqigufen.top/gtxvzzpown.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.daxiang520.top/gthrwkpacy.html

Go:   err.Error()
来源：http://hz.hammf.cn/gtltfdebhl.html

Ruby: e.message;  e.backtrace
来源：http://hz.0kj1m.cn/gtxlhndugv.html

C#:   e.Message;  e.StackTrace
来源：http://hz.nanxinkj.top/gtjrmmnkuj.html

[H09] 带错误码的异常
来源：http://hz.guowangkeji.top/gtsyzmrsij.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhiwuduotai.top/gtejzjocbo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zycfv.cn/gtteumdqwa.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cqqwz.cn/gtumomnhqc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xylfe.cn/gtqlfpgvfi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.mhx1999.top/gtsjsgowrf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yuanzhike.top/gttilgssam.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.svipenyu.cn/gttmyskipn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.chenjidiqi.icu/gtighnfghr.html

[H10] 资源自动释放
来源：http://hz.yuxming.cn/gtdcgbivcl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jianghu66.top/gtubdmpuhd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ehwqpu.com/gtctudlyhd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.c1oappe.top/gtxaizuekt.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yvedp.cn/gtpavjwlrx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xuanzx.com/gtnseofhbq.html

Go:   defer f.Close()
来源：http://hz.jyoumei.cn/gtjqskapnc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yangfankeji.com/gttfvceria.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhiwuduotai.top/gtgwwadvpi.html

================================================================================
来源：http://hz.yuxming.cn/gtfkxjudwf.html

I. 正则表达式
来源：http://hz.cashguo.top/gtmwmckboa.html

================================================================================
来源：http://hz.ydzc1.top/gtxaigftuy.html

[I01] 判断是否匹配
来源：http://hz.hnqzz.top/gtlxwrklsd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.bjfxy.top/gtmoiubqlf.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yvedp.cn/gtmjcpttwn.html

JS:   /\d+/.test(s)
来源：http://hz.yanxiufei.cn/gtyvshhobr.html

TS:   /\d+/.test(s)
来源：http://hz.yuxming.cn/gtlakwpouf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.wangdashe.top/gtpheddrrp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.gogol.net.cn/gtistzxhze.html

Ruby: s.match?(/\d+/)
来源：http://hz.jiagoushi.top/gtgiimxmsv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.smart0.xyz/gtuitdvklm.html

[I02] 提取所有匹配
来源：http://hz.haohaochexian.top/gtpovfycum.html

Py:   re.findall(r"\d+", s)
来源：http://hz.mhx1999.top/gtvxnznjgn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yonumen.top/gtpoaznrdn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hongshengwenyu.top/gtnopvaovi.html

TS:   s.match(/\d+/g)
来源：http://hz.hongshengwenyu.top/gtrkvlxgjm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.dianchejie.cn/gtcwkcbukw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.dianchejie.cn/gthtgfcnmy.html

Ruby: s.scan(/\d+/)
来源：http://hz.sweek.top/gtanzbkcbx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cqqwz.cn/gtofwvqoyg.html

[I03] 提取捕获分组
来源：http://hz.yangfankeji.com/gtmssqidwb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shuidangran.top/gtfmgcolef.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ppjwa.cn/gtyojmxytu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gaohongyu789.top/gtgscgygph.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.vqdsnc.cn/gtdibjrufq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhongyouzk.top/gtsoyyfcux.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj20258.top/gtyxodzsaw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.316326.xyz/gtyvaxpzfw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hnqzz.top/gtzbtkempc.html

[I04] 正则替换
来源：http://hz.vqdsnc.cn/gthgginamf.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhiwuduotai.top/gtwphpckvi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hfpthk.cn/gthftcxhqv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.pycfn.com/gtdyndjbxx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.snrcjt.cn/gtipbhctmp.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.snrcjt.cn/gtmhbtvfpe.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jiagoushi.top/gtyttmreyg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ehwqpu.com/gtwhaxlcfg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.iojbl.cn/gtivsjyghi.html

[I05] 按正则拆分
来源：http://hz.xuanzx.com/gtvbxklxcn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.sxryk.cn/gtqhaouuqm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hnxiangtu.top/gtfcyzmonc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cashguo.top/gtsvmeldtm.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gttcofclik.html

Java: s.split("\\s*,\\s*")
来源：http://hz.meibo888.top/gtkitbzirk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.haohaochexian.top/gtiqqdxfvk.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nanxinkj.top/gtjoopvdzu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xziqi.cn/gtpottgtee.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hammf.cn/gtdkmadlyg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yonumen.top/gtyasygrxv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.smart0.xyz/gtuccwsabq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhoulong.xyz/gtmuhfeoyc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.9152youxi.cn/gtijtlpxxu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.svipenyu.cn/gtjdnqslob.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hywenlv.cn/gttiuhbupt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.smart0.xyz/gtrdjujwth.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hfpthk.cn/gtqrqaohnc.html

[I07] 忽略大小写与多行模式
来源：http://hz.svipenyu.cn/gtfiypsvmu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ppjwa.cn/gtgsshtmpm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.9152youxi.cn/gtjaomrdos.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shangyingyoupin.top/gtqhztstli.html

TS:   /error/gim
来源：http://hz.shzxlz.cn/gtzzqdmzpq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.fengsongda.top/gtmachzkgj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yonumen.top/gttyejgaiv.html

Ruby: s.scan(/error/i)
来源：http://hz.tianlin.xyz/gtgilufxvr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.snrcjt.cn/gtbictmmfo.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sufxvd.cn/gtuzgmskff.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hfpthk.cn/gteeiucvcr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jqgufenzy.top/gtonxvquka.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.birdmap.top/gtushulduk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gzhubu.top/gtqidiijwy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cdnleiting.top/gtznobxvmk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.pycfn.com/gtzdlojths.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hongshengwenyu.top/gtbhlheyzv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.daxiang520.top/gttjoxtmuh.html

================================================================================
来源：http://hz.yuanzhike.top/gteafgdqzz.html

J. 日期与时间
来源：http://hz.0kj1m.cn/gtjfkthtgx.html

================================================================================
来源：http://hz.nanxinkj.top/gtcvgdewpb.html

[J01] 获取当前时间
来源：http://hz.cheryme.top/gtlxzepccy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhixingplan.top/gttdltnfpa.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.haohaochexian.top/gtvosuikjk.html

JS:   new Date();  Date.now()
来源：http://hz.ydjk.org.cn/gtpwivftod.html

TS:   new Date();  Date.now()
来源：http://hz.0kj1m.cn/gtwwtjpaec.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinghuilouyu.cn/gtmthxuerm.html

Go:   time.Now()
来源：http://hz.9152youxi.cn/gtqzwqadhr.html

Ruby: Time.now
来源：http://hz.xylfe.cn/gtfrzwohqf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jyoumei.cn/gteyghadkh.html

[J02] 格式化输出
来源：http://hz.snrcjt.cn/gtlnddyhuu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangshuangyany.cn/gtlbsjlrcs.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhoulong.xyz/gtrefhoxlu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xinyue.icu/gtyxlurjku.html

TS:   d.toISOString()
来源：http://hz.wangshuangyany.cn/gtwsziiaxz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yueranfly.top/gtyzwjzzne.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.sweek.top/gtvixhagnc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgfzy.top/gtmjfdxdzc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.sufxvd.cn/gtcrftobwg.html

[J03] 字符串解析为日期
来源：http://hz.sufxvd.cn/gtgibaiafd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hywenlv.cn/gtybpcimtn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cdnleiting.top/gtvhxdbems.html

JS:   new Date("2024-01-02")
来源：http://hz.kuanghao11.cn/gtamgsfobz.html

TS:   new Date("2024-01-02")
来源：http://hz.bjfxy.top/gtbfysyktm.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.c1oappe.top/gtesiedimp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.quarkkingdee.top/gtwfnhxzkd.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.snrcjt.cn/gtgxwjfpmg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ydjk.org.cn/gtzwbealij.html

[J04] 时间戳与日期互转
来源：http://hz.zhiwuduotai.top/gtzqoojino.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yuxming.cn/gttmhycstf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jianghu66.top/gtstozdiab.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jlsjyb.cn/gtfyuwzkzi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.chenjidiqi.icu/gtiayxpdcb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.guannengcc.top/gtoitqjisw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.wangdashe.top/gtttgvlbrf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hfpthk.cn/gtyzaukydh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.meibo888.top/gtqlfjqozu.html

[J05] 时间加减（加 7 天）
来源：http://hz.kuanghao11.cn/gtdewyxwgo.html

Py:   now + timedelta(days=7)
来源：http://hz.ywan-chungtsiang.top/gtpugwdzeq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shzxlz.cn/gtfmlhcwgw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.9152youxi.cn/gtbvdxfnat.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fengsongda.top/gtsqspfrir.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.52xcode.cn/gtkwwqhsmw.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.chenzaomai.com/gtnbejupkp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.c1oappe.top/gtplpqelue.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.sysykeji.top/gtesvktums.html

[J06] 计算两时间之差
来源：http://hz.jianghu66.top/gttllsvibd.html

Py:   (end - start).total_seconds()
来源：http://hz.yanxiufei.cn/gtxdvzofpn.html

PHP:  $end->diff($start)->days;
来源：http://hz.fzhhl.top/gtacnhnxki.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sxryk.cn/gtompsqpuc.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cashguo.top/gtgjakcztk.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.nanxinkj.top/gtddpkwbsv.html

Go:   end.Sub(start).Hours()
来源：http://hz.sysykeji.top/gtkltfumcw.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gzhubu.top/gthwzcaqzj.html

C#:   (end - start).TotalSeconds
来源：http://hz.xingfuxueyuan.xyz/gtoqcogmah.html

[J07] 比较两个日期
来源：http://hz.ybcxt.top/gtqilegtlr.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.fengsongda.top/gtzbyxsbcy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yongpay.top/gtmelagkrq.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shanyushiyangkeji.top/gtwoohdche.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jiagoushi.top/gtnswsbqqq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yanxiufei.cn/gtedyafspa.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.pycfn.com/gtdkpwblxg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gtoifblmom.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.redwolf501.top/gtzjpwahnf.html

[J08] 提取年月日与星期
来源：http://hz.pengpengdd.cyou/gtfbmxlnfk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinqigufen.top/gttcimzetp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhijiandao.cn/gtdcxczgeo.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.dashuyun.cn/gtsgxsddlv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.daria6918.cn/gtefhmiiee.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.0kj1m.cn/gtssovsrqx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jinqigufen.top/gtetwbrwvx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hammf.cn/gtlecmpfyo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.fengsongda.top/gtlhsluqzw.html

[J09] 时区处理
来源：http://hz.hnxiangtu.top/gtzcfqtvbx.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jiagoushi.top/gtjxydolzm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jinqigufen.top/gtoralenlm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.9152youxi.cn/gtuwnturuj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.iojbl.cn/gtveebsyxx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.meibo888.top/gttdzxetgh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.316326.xyz/gtleglzvgt.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenzaomai.com/gtkwdrstfs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cheryme.top/gtkqwixzpv.html

[J10] 取今天 / 本月第一天
来源：http://hz.yanxiufei.cn/gtewfkrzcf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.svipenyu.cn/gtxobzcvts.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hysaishi.cn/gtxjcnnhus.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.0kj1m.cn/gtbqirivpy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhiwuduotai.top/gtbzsbltjh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.jinghuilouyu.cn/gtukhcklai.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.andypj.xyz/gtuftjvlkv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.pengpengdd.cyou/gtjqmfkoql.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.snrcjt.cn/gtbskcjzgu.html

================================================================================
来源：http://hz.vqdsnc.cn/gtwlejjjok.html

K. JSON 与序列化
来源：http://hz.daria6918.cn/gtaehafdoc.html

================================================================================
来源：http://hz.xylfe.cn/gtthqjsgxc.html

[K01] 对象转 JSON 字符串
来源：http://hz.tian-w.cn/gtogwzjhpd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yanxiufei.cn/gtbmokbzpj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yangfankeji.com/gtzjqxtvvw.html

JS:   JSON.stringify(obj)
来源：http://hz.pengpengdd.cyou/gteofgfnnq.html

TS:   JSON.stringify(obj)
来源：http://hz.hongshengwenyu.top/gtwfvdyati.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tian-w.cn/gttytaeeck.html

Go:   json.Marshal(obj)
来源：http://hz.tanke756.top/gtdcjxqbgh.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.gzhubu.top/gtxbezjslo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shanyushiyangkeji.top/gtqjkubchn.html

[K02] JSON 字符串转对象
来源：http://hz.jyoumei.cn/gtjwjcvugu.html

Py:   json.loads(s)
来源：http://hz.xingfuxueyuan.xyz/gttmnxudli.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.fzhhl.top/gtcdlfgcsb.html

JS:   JSON.parse(s)
来源：http://hz.xinyue.icu/gtyrhaijtu.html

TS:   JSON.parse(s)
来源：http://hz.yueranfly.top/gtxpnuzunp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.aibaodan.cn/gtthmcodqu.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.daxiang520.top/gtqxeurmvn.html

Ruby: JSON.parse(s)
来源：http://hz.yangfankeji.com/gtufsriadb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hywenlv.cn/gtsxxgxtjb.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zdqjudy.top/gtwjtsqsdj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.c1oappe.top/gteawkhphh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.vqdsnc.cn/gtqimgkbsy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.guannengcc.top/gtikoybrot.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgfzy.top/gtbbdugkcq.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yj202588.top/gtzvhfgkte.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.nanxinkj.top/gtjfbarhjd.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cheryme.top/gtzszotmjv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zdqjudy.top/gtvhqsjyyn.html

[K04] 读取 JSON 文件
来源：http://hz.jinyuanbaomall.cn/gtpiuozxzd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.fzhhl.top/gtpeltkyya.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shangyingyoupin.top/gtwosuoqcb.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ybcxt.top/gtynuexncv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cheryme.top/gtiqxsahjv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yj20258.top/gtyjuavzso.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.cqqwz.cn/gtvnxrqzsr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hfpthk.cn/gtfzfsihkr.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.snrcjt.cn/gtkqwakwre.html

[K05] 深拷贝对象
来源：http://hz.yonumen.top/gttkycywvc.html

Py:   copy.deepcopy(obj)
来源：http://hz.xuanzx.com/gtwimcswyn.html

PHP:  unserialize(serialize($obj));
来源：http://hz.smart0.xyz/gteeolkena.html

JS:   structuredClone(obj)
来源：http://hz.zhoulong.xyz/gtjfhqinsg.html

TS:   structuredClone(obj)
来源：http://hz.yuanzhike.top/gtxkcrcuba.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.chenjidiqi.icu/gtbncfrbwx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ywan-chungtsiang.top/gtcgipxqrw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jqgfzy.top/gtemyqqofg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cashguo.top/gtcdtcsfqh.html

[K06] 解析 URL 查询串
来源：http://hz.gzhubu.top/gtllumjlls.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.gogol.net.cn/gtozaccadk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yuxming.cn/gtohwgzerl.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jiagoushi.top/gtrzjkvxlp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hywenlv.cn/gtayfzflur.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.haohaochexian.top/gtzisiweht.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.yongpay.top/gtwshpqkmn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.yuxming.cn/gtajjrolob.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.feifeiyinyue.top/gtshryvmdt.html

[K07] 进制转换
来源：http://hz.pengpengdd.cyou/gtqybkeyyo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtpnhopkyj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cucudq.cn/gtacftzreb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zycfv.cn/gtvabgiiow.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ppjwa.cn/gttpppyajq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.dashuyun.cn/gttajxuczo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.wangshuangyany.cn/gtehokledx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.xziqi.cn/gtlfawaqvz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.shanyushiyangkeji.top/gtfbqzypzz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.havefunace.top/gtpisgodrs.html

Py:   pickle.dumps(obj)
来源：http://hz.chenzaomai.com/gtosnwoyys.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.0kj1m.cn/gtvlkkyhew.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.mhx1999.top/gtmaitdmpt.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.redwolf501.top/gttnfmkwdl.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.daria6918.cn/gtrprynaya.html

Go:   encoding/gob
来源：http://hz.sysykeji.top/gtgdabljgb.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhengqikj.top/gtqwzqgtwd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xingfuxueyuan.xyz/gtfwsanwsx.html

================================================================================
来源：http://hz.smart0.xyz/gttxhgyrvr.html

L. 网络请求
来源：http://hz.zhaomingkeji.xyz/gtpqshmiqm.html

================================================================================
来源：http://hz.jlsjyb.cn/gtepjzveuk.html

[L01] 发送 GET 请求
来源：http://hz.yj20258888.top/gtlacfuwpe.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.cashguo.top/gtckwirvtn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hz.hywenlv.cn/gtxqcnxdcb.html

JS:   await fetch(url)
来源：http://hz.9152youxi.cn/gtrdkqyecs.html

TS:   await fetch(url)
来源：http://hz.jiagoushi.top/gtbopfsafa.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hz.wangshuangyany.cn/gtsllgbfcp.html


<!-- 参考信息 -->