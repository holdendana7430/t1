代发 wailian999

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shanyushiyangtech.top/gtijzkzjsn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yueranfly.top/gtcoweddwo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinqigfzy.top/gtnplreacq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtukmlfywv.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nwbrower.top/gtgqtfzmyo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.svipenyu.cn/gtdkznxsuw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ywan-chungtsiang.top/gtvhnqwopg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shanyushiyangkeji.top/gtnkaoerit.html

[H03] 主动抛出异常
来源：http://hz.kuanghao11.cn/gtxrojggci.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhoulong.xyz/gtoimrwxhe.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xylfe.cn/gtdbdzarvo.html

JS:   throw new Error("错误信息");
来源：http://hz.shzxlz.cn/gtvyrtlakx.html

TS:   throw new Error("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtvqnoxcni.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gtusghdzws.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.cdnleiting.top/gtragprleo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ybcxt.top/gtdkdiqwxy.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yvedp.cn/gtesevzyeu.html

[H04] 自定义异常类型
来源：http://hz.cdnleiting.top/gtbmllccxr.html

Py:   class MyError(Exception): pass
来源：http://hz.quarkkingdee.top/gtbztfuxgf.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jqgufenzy.top/gtjqhonwhs.html

JS:   class MyError extends Error {}
来源：http://hz.hnqzz.top/gtavfqnezb.html

TS:   class MyError extends Error {}
来源：http://hz.zhijiandao.cn/gtgtszwvef.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jlsjyb.cn/gthisyvsif.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cheryme.top/gtvbxnmdcj.html

Ruby: class MyError < StandardError; end
来源：http://hz.wangdashe.top/gtzvmsufds.html

C#:   class MyException : Exception {}
来源：http://hz.cqqwz.cn/gtvdhwzmpc.html

[H05] 捕获特定类型
来源：http://hz.tian-w.cn/gtgauohfwc.html

Py:   except ValueError as e:
来源：http://hz.xuanzx.com/gtkdkzobsn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yuxming.cn/gtnomldpsm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.fzhhl.top/gtweanrjor.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hongshengwenyu.top/gtvyqatrcd.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hnxiangtu.top/gtryeknahk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ivvv.top/gtorrywnqg.html

Ruby: rescue ArgumentError => e
来源：http://hz.shanyushiyangkeji.top/gttdtjkovf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yanxiufei.cn/gthkbvafbh.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cdnleiting.top/gtytobghzs.html

Py:   value = d.get("k") or default
来源：http://hz.jinghuilouyu.cn/gtztarfmub.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jinqigufen.top/gtaiagriyv.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.daxiang520.top/gthfthresm.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.haohaochexian.top/gtdcigqkck.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.nanxuanxn.top/gtsxaojsqw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hysaishi.cn/gtltbrlzyb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.nanxuanxn.top/gtdtortafa.html

C#:   obj?.A?.B ?? default
来源：http://hz.hammf.cn/gtbmbatjip.html

[H07] 断言
来源：http://hz.mhx1999.top/gtifidumgz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.smart0.xyz/gtlwxdzjpr.html

PHP:  assert($x > 0);
来源：http://hz.yueranfly.top/gteirikpmj.html

JS:   console.assert(x > 0);
来源：http://hz.jinghuilouyu.cn/gtxocqfihd.html

TS:   console.assert(x > 0);
来源：http://hz.jinghuilouyu.cn/gteamckfvf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.dashuyun.cn/gtkrhwcdfd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.aizwys.cn/gtmygacdap.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yvedp.cn/gtfigofbvk.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yj20258888.top/gtzvogpgoa.html

[H08] 获取错误信息与堆栈
来源：http://hz.vqdsnc.cn/gtltxklzep.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.wangdashe.top/gtlczuzczb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.fengsongda.top/gtbeksglpa.html

JS:   e.message;  e.stack
来源：http://hz.shzxlz.cn/gtrnhfcmyy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.andypj.xyz/gtqhxsvwrh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.feifeiyinyue.top/gtvajwowgp.html

Go:   err.Error()
来源：http://hz.fengsongda.top/gtlqrxivvi.html

Ruby: e.message;  e.backtrace
来源：http://hz.cheryme.top/gthwhfezsz.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shanyushiyangtech.top/gtbanepbmh.html

[H09] 带错误码的异常
来源：http://hz.tianlin.xyz/gtzgeicxzr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.wangshuangyany.cn/gtezjyuutn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinqigfzy.top/gtjmrryhmu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sysykeji.top/gtxlxxzulq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.vqdsnc.cn/gtoyylodqj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shangyingyoupin.top/gtsdpknjkk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.tanke756.top/gtkahpasuz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shuidangran.top/gtunnlikmc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ppjwa.cn/gtlslbticz.html

[H10] 资源自动释放
来源：http://hz.shzxlz.cn/gtkobzbpmk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yongpay.top/gtepdnvemq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.fzhhl.top/gtkvfjojek.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cdnleiting.top/gtpkqibeuq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhengqikj.top/gtwfwrepdy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.mhx1999.top/gtyjpdwzis.html

Go:   defer f.Close()
来源：http://hz.hnqzz.top/gtxszfdytr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.birdmap.top/gtylkbtvvm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.daxiang520.top/gtiltjnfzo.html

================================================================================
来源：http://hz.hnxiangtu.top/gtcwxnoxfu.html

I. 正则表达式
来源：http://hz.hywenlv.cn/gtusfiwzxg.html

================================================================================
来源：http://hz.aizwys.cn/gtjrefdrjw.html

[I01] 判断是否匹配
来源：http://hz.sweek.top/gttahcfnxz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yueranfly.top/gtigeenjau.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.quarkkingdee.top/gtgwrprphi.html

JS:   /\d+/.test(s)
来源：http://hz.hammf.cn/gtohrpxoma.html

TS:   /\d+/.test(s)
来源：http://hz.cdnleiting.top/gtlmmsepyd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhengqikj.top/gtwsznchfu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ybcxt.top/gttrcvvvsj.html

Ruby: s.match?(/\d+/)
来源：http://hz.redwolf501.top/gttxyzkwwr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jqgfzy.top/gtnvcqsptw.html

[I02] 提取所有匹配
来源：http://hz.cqqwz.cn/gtphzmhfqx.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yvedp.cn/gtomukvfmx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ehwqpu.com/gtwqyhzxha.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.gzhubu.top/gtpqnbtgbl.html

TS:   s.match(/\d+/g)
来源：http://hz.zhixingplan.top/gtcdzjemiq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.svipenyu.cn/gtoqrwwcnw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.aibaodan.cn/gtsmkoobgr.html

Ruby: s.scan(/\d+/)
来源：http://hz.hnxiangtu.top/gtrtnmtazo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ivvv.top/gtmumbiprx.html

[I03] 提取捕获分组
来源：http://hz.hammf.cn/gtfdgophuz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhengqikj.top/gtynftmsgm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gotoacloud.top/gtdzjawmcq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cheryme.top/gtjexkkiqy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.9152youxi.cn/gttrwrmfjp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.52xcode.cn/gtcjslcrnm.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yvedp.cn/gtzeknjzcl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.tanke756.top/gthkauishr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.0kj1m.cn/gtaciayffc.html

[I04] 正则替换
来源：http://hz.dashuyun.cn/gtnodyhmpm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.9152youxi.cn/gtcqtqcqjc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gogol.net.cn/gtwilscuqj.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.tian-w.cn/gtrvmvhwvc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhoulong.xyz/gtbqgomeue.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.fengsongda.top/gtfzkfxuos.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.0kj1m.cn/gtoxjtjupe.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nanxinkj.top/gtvyssmqsg.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.mhx1999.top/gtaduzoids.html

[I05] 按正则拆分
来源：http://hz.shuidangran.top/gtjljsbixz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xinyue.icu/gtsonhajeq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ywan-chungtsiang.top/gtojgbwuxx.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jianghu66.top/gtyungausf.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.fzhhl.top/gttdksxctk.html

Java: s.split("\\s*,\\s*")
来源：http://hz.mhx1999.top/gttithtkik.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.nanxinkj.top/gtjxzuhfaj.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yongpay.top/gtnkxkcflg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jinqigfzy.top/gtyfzfucsk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhongyouzk.top/gtgdnlncvd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.chenlongwang.top/gtbgnvlhcp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.chenjidiqi.icu/gtpbrektta.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258.top/gtnfyhaeuw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fzhhl.top/gtybiezgwh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hongshengwenyu.top/gtconakjhp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hysaishi.cn/gtwoahglyh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xuetiantiany.cn/gtxrdhcxvu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yangfankeji.com/gtfgzdzytd.html

[I07] 忽略大小写与多行模式
来源：http://hz.xylfe.cn/gtnapgqtne.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.svipenyu.cn/gtyhuvedjp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.sweek.top/gttigvlthd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.chenzaomai.com/gtjdgiixli.html

TS:   /error/gim
来源：http://hz.snrcjt.cn/gtulegvgyr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yuxming.cn/gtnajrlgmd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.c1oappe.top/gtlyndvxid.html

Ruby: s.scan(/error/i)
来源：http://hz.shangyingyoupin.top/gtpwkasypp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xinyue.icu/gtwhvzdian.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.chenlongwang.top/gtivscfvfd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yanxiufei.cn/gtwypkqbhe.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xingfuxueyuan.xyz/gtiicujcdj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gotoacloud.top/gttkzvbexu.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.pengpengdd.cyou/gtxfxxvwle.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shangyingyoupin.top/gtubrqcmqh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ivvv.top/gtsvgxtojo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.nanxuanxn.top/gttnxsfjlt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhiwuduotai.top/gtdffbniwz.html

================================================================================
来源：http://hz.yueranfly.top/gtvozyajub.html

J. 日期与时间
来源：http://hz.smart0.xyz/gtepqkfrzn.html

================================================================================
来源：http://hz.nwbrower.top/gtwmzcyeld.html

[J01] 获取当前时间
来源：http://hz.zhiwuduotai.top/gtyebzovyl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ywan-chungtsiang.top/gtbnukuayd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shuidangran.top/gtfidjjulk.html

JS:   new Date();  Date.now()
来源：http://hz.xuetiantiany.cn/gtoqbclkle.html

TS:   new Date();  Date.now()
来源：http://hz.jinqigfzy.top/gtlpecpoup.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.sxryk.cn/gtbijltzts.html

Go:   time.Now()
来源：http://hz.tian-w.cn/gtpessyxfy.html

Ruby: Time.now
来源：http://hz.52xcode.cn/gtunuvpomj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zdqjudy.top/gtsjjdfdpo.html

[J02] 格式化输出
来源：http://hz.zhengqikj.top/gtfucvpmly.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.feifeiyinyue.top/gtaxqnuccr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cqqwz.cn/gthyypxyon.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.havefunace.top/gtrfjqjbtj.html

TS:   d.toISOString()
来源：http://hz.zhoulong.xyz/gtsaqiwypr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhengqikj.top/gthnktgfmk.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.wangdashe.top/gtjcpepfcz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hammf.cn/gtmiaivtat.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zycfv.cn/gtilftaulb.html

[J03] 字符串解析为日期
来源：http://hz.svipenyu.cn/gtpgavqdlt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.cqqwz.cn/gtchpktmxx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ydzc1.top/gtstdtsqnv.html

JS:   new Date("2024-01-02")
来源：http://hz.hammf.cn/gtrexepmuc.html

TS:   new Date("2024-01-02")
来源：http://hz.smart0.xyz/gtubkonmbw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hfpthk.cn/gtpvqzeazk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.gotoacloud.top/gteeinxvgu.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.vqdsnc.cn/gttmhwdzhc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ydzc1.top/gtwmcslbnr.html

[J04] 时间戳与日期互转
来源：http://hz.52xcode.cn/gtjlxjbtyk.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xuanzx.com/gtgapjnila.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.birdmap.top/gtxfglixpa.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.fzhhl.top/gtrkmnucqr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jlsjyb.cn/gtngibpgka.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yueranfly.top/gtaenrnvwt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jinqigfzy.top/gtsltakwwj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.feifeiyinyue.top/gtxmdcmgel.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hysaishi.cn/gtwxdnoyjs.html

[J05] 时间加减（加 7 天）
来源：http://hz.yvedp.cn/gtobkkqrwu.html

Py:   now + timedelta(days=7)
来源：http://hz.jinqigfzy.top/gtnwaujwlu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.chenlongwang.top/gtbpaapctt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.smart0.xyz/gtxdembiyi.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nwbrower.top/gthfqtowoh.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hfpthk.cn/gtpsbbjbzt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.fzhhl.top/gtygiiopic.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhijiandao.cn/gtqdqjdujs.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.shuidangran.top/gtmwrxzbxl.html

[J06] 计算两时间之差
来源：http://hz.guannengcc.top/gtsbmnnbch.html

Py:   (end - start).total_seconds()
来源：http://hz.jiagoushi.top/gtsftbhewy.html

PHP:  $end->diff($start)->days;
来源：http://hz.ivvv.top/gtpiinznng.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.guowangkeji.top/gtyqnvcyhv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.pycfn.com/gteixwfoig.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.vqdsnc.cn/gtlzfsntox.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhoulong.xyz/gtpqssthkq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cucudq.cn/gtnsbalmda.html

C#:   (end - start).TotalSeconds
来源：http://hz.quarkkingdee.top/gtgjgshrmj.html

[J07] 比较两个日期
来源：http://hz.bjfxy.top/gtoqrfjaac.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtfkorrkvt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.nanxuanxn.top/gtsluqxttw.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cheryme.top/gtkjhpmver.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zdqjudy.top/gtlxwwetud.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yonumen.top/gtpjqyrlnz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.iojbl.cn/gttbafbdxe.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cheryme.top/gtgapxeiio.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtqbbndaon.html

[J08] 提取年月日与星期
来源：http://hz.chenjidiqi.icu/gthjdzairf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.quarkkingdee.top/gtsfyltjiy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.dianchejie.cn/gtzmjvlwet.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.quarkkingdee.top/gthdizyowh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.haohaochexian.top/gtjlnuhfie.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.mhx1999.top/gtgbciowcc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhaomingkeji.xyz/gthoadbcdg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yangfankeji.com/gtjyoscysg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jianghu66.top/gtbdtawovo.html

[J09] 时区处理
来源：http://hz.gaohongyu789.top/gtnwmekbsw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gogol.net.cn/gtivgrsrfy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.gaohongyu789.top/gtikavrhsy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnxiangtu.top/gtfgzvhuml.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangdashe.top/gtqqoxdoun.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yonumen.top/gtcdsumqud.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhongyouzk.top/gtwqnuqoex.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinyuanbaomall.cn/gtfygzmuza.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ehwqpu.com/gtbsvllldy.html

[J10] 取今天 / 本月第一天
来源：http://hz.yuanzhike.top/gtlrsuhrcl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinghuilouyu.cn/gtqdextdqs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.fengsongda.top/gtsebqzirt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.aibaodan.cn/gtquforofz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yonumen.top/gtnsyjznql.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hammf.cn/gtitxwnynt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.sufxvd.cn/gtqfibskmy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.chenzaomai.com/gtbsxndpam.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.guannengcc.top/gtegnbflyc.html

================================================================================
来源：http://hz.daria6918.cn/gtjdxjnmnj.html

K. JSON 与序列化
来源：http://hz.zycfv.cn/gtdloiwzqe.html

================================================================================
来源：http://hz.nwbrower.top/gtwkjritcr.html

[K01] 对象转 JSON 字符串
来源：http://hz.gotoacloud.top/gtsbokwhtk.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.sysykeji.top/gtmjattmpl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ehwqpu.com/gtmystodeq.html

JS:   JSON.stringify(obj)
来源：http://hz.jiagoushi.top/gtwgrvmjpc.html

TS:   JSON.stringify(obj)
来源：http://hz.daria6918.cn/gtnuruicyz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhixingplan.top/gtaogkywei.html

Go:   json.Marshal(obj)
来源：http://hz.zycfv.cn/gteqaghlcq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.dashuyun.cn/gtuzlidlew.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xingfuxueyuan.xyz/gtsstmkfmt.html

[K02] JSON 字符串转对象
来源：http://hz.jyoumei.cn/gtkvqchsbm.html

Py:   json.loads(s)
来源：http://hz.yj20258888.top/gtjeugwepc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shzxlz.cn/gtagybkdgk.html

JS:   JSON.parse(s)
来源：http://hz.svipenyu.cn/gtbcbjhjfo.html

TS:   JSON.parse(s)
来源：http://hz.kuanghao11.cn/gtjkguvcff.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zycfv.cn/gttobkncsz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinqigfzy.top/gtaawvwnob.html

Ruby: JSON.parse(s)
来源：http://hz.yanxiufei.cn/gtcqffyerq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.daxiang520.top/gtxvgxdqbp.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinyuanbaomall.cn/gtgcxpgrsi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ydjk.org.cn/gtzrghoqsh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ydzc1.top/gtiylshbva.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.feifeiyinyue.top/gtcjjkswwp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.snrcjt.cn/gtiredepmh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.vqdsnc.cn/gtcbbdpuzj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.sysykeji.top/gtmwcmpaef.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.haohaochexian.top/gtbefuqocf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xingfuxueyuan.xyz/gtzswhxuqh.html

[K04] 读取 JSON 文件
来源：http://hz.hongshengwenyu.top/gthrjdbxnh.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.guowangkeji.top/gtbllwwkri.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.gogol.net.cn/gtvasrsjgt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xuanzx.com/gtyascneid.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.9152youxi.cn/gtgggfbvft.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.fzhhl.top/gthwvvykal.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jlsjyb.cn/gtweithjcz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yueranfly.top/gtlhfdbhey.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ydzc1.top/gtfnjbolih.html

[K05] 深拷贝对象
来源：http://hz.pengpengdd.cyou/gtoxtunnfw.html

Py:   copy.deepcopy(obj)
来源：http://hz.gaohongyu789.top/gtlmqghaho.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zdqjudy.top/gtfszgwghb.html

JS:   structuredClone(obj)
来源：http://hz.jiagoushi.top/gttyywbgcs.html

TS:   structuredClone(obj)
来源：http://hz.cashguo.top/gtmirhywza.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.fengsongda.top/gteixsyeld.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.9152youxi.cn/gtkgxudidg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yj20258888.top/gtelmrnpuc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gzhubu.top/gtepouohhy.html

[K06] 解析 URL 查询串
来源：http://hz.hysaishi.cn/gtrdnbztda.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.fzhhl.top/gttpxiggdg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yj20258.top/gtzoetgoru.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnqzz.top/gthxbpqagd.html


<!-- 参考信息 -->