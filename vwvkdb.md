代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yvedp.cn/gtqtpdrggv.html

[H04] 自定义异常类型
来源：http://hz.bjfxy.top/gthddrvvsn.html

Py:   class MyError(Exception): pass
来源：http://hz.nwbrower.top/gtpzznfduj.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.gaohongyu789.top/gtclgsoiwu.html

JS:   class MyError extends Error {}
来源：http://hz.zhaomingkeji.xyz/gtmtvbljsx.html

TS:   class MyError extends Error {}
来源：http://hz.gaohongyu789.top/gterwwtcpc.html

Java: class MyException extends RuntimeException {}
来源：http://hz.birdmap.top/gtchdotgkl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.haohaochexian.top/gtsrkqjlql.html

Ruby: class MyError < StandardError; end
来源：http://hz.meibo888.top/gtwzsyajwo.html

C#:   class MyException : Exception {}
来源：http://hz.hammf.cn/gtpxoyglwq.html

[H05] 捕获特定类型
来源：http://hz.dashuyun.cn/gtntwbzxkg.html

Py:   except ValueError as e:
来源：http://hz.52xcode.cn/gthxuvzbpc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.fzhhl.top/gtqesqcdyq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jianghu66.top/gtzmruvxmc.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.daria6918.cn/gtmucgfhxz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jiagoushi.top/gtwnlbhops.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shuidangran.top/gtxwjxpzsr.html

Ruby: rescue ArgumentError => e
来源：http://hz.vqdsnc.cn/gtqvgzuzau.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.guowangkeji.top/gtlfzootmd.html

[H06] 可选值 / 空值安全访问
来源：http://hz.havefunace.top/gtguxswslg.html

Py:   value = d.get("k") or default
来源：http://hz.shanyushiyangtech.top/gtwzfuptyv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.redwolf501.top/gtfmgzzptv.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.quarkkingdee.top/gtbntxkarh.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.nwbrower.top/gtjzztyocy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhixingplan.top/gtryuditcm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cheryme.top/gtxtmgzfwc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shanyushiyangkeji.top/gtbpnjgcmg.html

C#:   obj?.A?.B ?? default
来源：http://hz.fzhhl.top/gtrdbrovoq.html

[H07] 断言
来源：http://hz.meibo888.top/gtzoyxepau.html

Py:   assert x > 0, "必须为正"
来源：http://hz.chenjidiqi.icu/gthobugtpi.html

PHP:  assert($x > 0);
来源：http://hz.chenlongwang.top/gtdsnxkohx.html

JS:   console.assert(x > 0);
来源：http://hz.hongshengwenyu.top/gtrifyezgv.html

TS:   console.assert(x > 0);
来源：http://hz.zhijiandao.cn/gtvfxixigc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shanyushiyangtech.top/gtspcunxrf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.smart0.xyz/gtuyuukziu.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.pycfn.com/gtuiwcewor.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtxpdgyvpj.html

[H08] 获取错误信息与堆栈
来源：http://hz.jinqigfzy.top/gtbkeruxzi.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zdqjudy.top/gtlwhshjus.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.9152youxi.cn/gttlwkduzu.html

JS:   e.message;  e.stack
来源：http://hz.shangyingyoupin.top/gtodvdlnrv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.haohaochexian.top/gtxtarxajm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jqgufenzy.top/gtsigyaxjo.html

Go:   err.Error()
来源：http://hz.aibaodan.cn/gtrnvsljkq.html

Ruby: e.message;  e.backtrace
来源：http://hz.sweek.top/gtgsvkenjo.html

C#:   e.Message;  e.StackTrace
来源：http://hz.daxiang520.top/gtbwnwkccp.html

[H09] 带错误码的异常
来源：http://hz.shzxlz.cn/gtgtgvcxjx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.fengsongda.top/gtedhoozoe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shangyingyoupin.top/gtqueppivr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.meibo888.top/gtcldypvhp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.nanxinkj.top/gtenmoxbfl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yueranfly.top/gtaumlnjpa.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.guowangkeji.top/gtzoyzufuh.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sweek.top/gtkwumagrr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jiagoushi.top/gtyemtnqnr.html

[H10] 资源自动释放
来源：http://hz.zhiwuduotai.top/gttesmxeqa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yvedp.cn/gtwbcdsvqy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinqigfzy.top/gtvtuvzfmb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.havefunace.top/gtjqtnrgad.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xinyue.icu/gtvjugspzi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jiagoushi.top/gtbbxqdrep.html

Go:   defer f.Close()
来源：http://hz.sufxvd.cn/gtsgbhmzyq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.iojbl.cn/gthhfabhgr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gogol.net.cn/gtllnspjmd.html

================================================================================
来源：http://hz.zycfv.cn/gtcxdrirhv.html

I. 正则表达式
来源：http://hz.nanxuanxn.top/gtnebtsnmv.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtxvwuepco.html

[I01] 判断是否匹配
来源：http://hz.yj20258888.top/gturrqolho.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ybcxt.top/gtesvuxdez.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hammf.cn/gtxmvaacez.html

JS:   /\d+/.test(s)
来源：http://hz.sweek.top/gtgqfjaqvh.html

TS:   /\d+/.test(s)
来源：http://hz.shzxlz.cn/gtndflvecd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cheryme.top/gtsgysktde.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.havefunace.top/gtqtrgzxyo.html

Ruby: s.match?(/\d+/)
来源：http://hz.feifeiyinyue.top/gtluroknnu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shzxlz.cn/gtinrbhoyv.html

[I02] 提取所有匹配
来源：http://hz.jyoumei.cn/gtqtlsgcrf.html

Py:   re.findall(r"\d+", s)
来源：http://hz.havefunace.top/gtbnzpvnid.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.gzhubu.top/gtipjaizur.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.52xcode.cn/gtjdkbhcvn.html

TS:   s.match(/\d+/g)
来源：http://hz.jyoumei.cn/gtfbsewodl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hongshengwenyu.top/gtiloqdwkg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.fzhhl.top/gtozstausx.html

Ruby: s.scan(/\d+/)
来源：http://hz.shuidangran.top/gthwtxtvrm.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xylfe.cn/gtvvtzfjsk.html

[I03] 提取捕获分组
来源：http://hz.tianlin.xyz/gtboemskdq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nanxuanxn.top/gtauwzeqvh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shanyushiyangkeji.top/gthmsieufg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zdqjudy.top/gtmivjgsie.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cashguo.top/gtboubbcer.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.andypj.xyz/gtgpeibqhp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.sxryk.cn/gthzhjajqx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hysaishi.cn/gtphcgvmqg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.52xcode.cn/gtsorfnqyu.html

[I04] 正则替换
来源：http://hz.hnxiangtu.top/gtohwzkjgl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cheryme.top/gtdujjkfvk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.snrcjt.cn/gtzhcfniif.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xuetiantiany.cn/gtwwszyyxt.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigufen.top/gtysjkstfo.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhijiandao.cn/gtvjunbapv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.aibaodan.cn/gtfmlhlcgu.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.daxiang520.top/gthzuvtoib.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.9152youxi.cn/gthzcyrjrc.html

[I05] 按正则拆分
来源：http://hz.mhx1999.top/gtdhmyekga.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xuetiantiany.cn/gtvkeisiio.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hnxiangtu.top/gtqotexjmz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jinyuanbaomall.cn/gtnyparhgs.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zycfv.cn/gtbvoavvru.html

Java: s.split("\\s*,\\s*")
来源：http://hz.gotoacloud.top/gttgtfcemo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xuetiantiany.cn/gtqoovxxmp.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jinyuanbaomall.cn/gtbhfdxplv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hnxiangtu.top/gtxyeizftg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.quarkkingdee.top/gtuefgvsxn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jianghu66.top/gtushiagtk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shzxlz.cn/gthdylatrd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.vqdsnc.cn/gtnghkjypw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangshuangyany.cn/gtdbmzaotd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.chenlongwang.top/gtxkflinru.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hnxiangtu.top/gtdutrhwtr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.chenlongwang.top/gttixjfeqc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.dianchejie.cn/gtjmgfyanp.html

[I07] 忽略大小写与多行模式
来源：http://hz.guannengcc.top/gtlpgukzwp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.c1oappe.top/gthwtoksvw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.svipenyu.cn/gtrgafemnu.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xziqi.cn/gtyrelpjnv.html

TS:   /error/gim
来源：http://hz.xylfe.cn/gtkhweoffm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cucudq.cn/gtbxsfedrc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.smart0.xyz/gtrpwwitua.html

Ruby: s.scan(/error/i)
来源：http://hz.c1oappe.top/gtnuhogmrw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yonumen.top/gtchugwdcb.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jinghuilouyu.cn/gtborzssnu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.nanxuanxn.top/gttthpzqkm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.c1oappe.top/gtzwkdzpmc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yvedp.cn/gtdpzawqpp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zycfv.cn/gtwmfsatza.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.guannengcc.top/gtobzpmkst.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gzhubu.top/gtnbcmephb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shzxlz.cn/gtdslkbsya.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sxryk.cn/gtvhsyvsoo.html

================================================================================
来源：http://hz.pycfn.com/gtxncjglya.html

J. 日期与时间
来源：http://hz.shangyingyoupin.top/gtjzbbhnjl.html

================================================================================
来源：http://hz.yj20258888.top/gtmtworlwd.html

[J01] 获取当前时间
来源：http://hz.cashguo.top/gtlsmqmoxo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.nanxuanxn.top/gthteyissj.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.pycfn.com/gtzklknoty.html

JS:   new Date();  Date.now()
来源：http://hz.ywan-chungtsiang.top/gtpyvjkbvn.html

TS:   new Date();  Date.now()
来源：http://hz.gzhubu.top/gteqrtvicm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinqigfzy.top/gtnjkxfdzv.html

Go:   time.Now()
来源：http://hz.jqgufenzy.top/gtbtvyysfn.html

Ruby: Time.now
来源：http://hz.316326.xyz/gtevsomhsa.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yonumen.top/gtljqfylts.html

[J02] 格式化输出
来源：http://hz.hnqzz.top/gtcomdaqep.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.haohaochexian.top/gthctxvyan.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.9152youxi.cn/gtltzlppls.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yvedp.cn/gtricfwvge.html

TS:   d.toISOString()
来源：http://hz.meibo888.top/gtiiimzrgc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.0kj1m.cn/gtzpkxwuzr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.kuanghao11.cn/gtsndfvaep.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tanke756.top/gtskmiqufx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zycfv.cn/gtruetygll.html

[J03] 字符串解析为日期
来源：http://hz.nwbrower.top/gtnfzpxzef.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinqigfzy.top/gttmkydpdu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhoulong.xyz/gtwwmyoyjb.html

JS:   new Date("2024-01-02")
来源：http://hz.smart0.xyz/gtfbzeodng.html

TS:   new Date("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtpzsagvvw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cheryme.top/gtgsyopxdj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yuanzhike.top/gtdicrpavl.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.guannengcc.top/gtifqxtdto.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sxryk.cn/gtjrgdnuje.html

[J04] 时间戳与日期互转
来源：http://hz.hysaishi.cn/gtitztkeve.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.redwolf501.top/gtfooezrzb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhiwuduotai.top/gtvenrbkeb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yuxming.cn/gtsamykpah.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.vqdsnc.cn/gtzoilpmgj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.guannengcc.top/gtfuzbyjjo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jinghuilouyu.cn/gtnyfsxlvq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hongshengwenyu.top/gtxhzymkxq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ehwqpu.com/gtfxvpqtfv.html

[J05] 时间加减（加 7 天）
来源：http://hz.jianghu66.top/gtcvkbxbeh.html

Py:   now + timedelta(days=7)
来源：http://hz.yonumen.top/gtqfjiclcf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yangfankeji.com/gttwypftke.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuetiantiany.cn/gtnhuzgshh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ydjk.org.cn/gtaheerdiq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yueranfly.top/gtooithfcn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cqqwz.cn/gtigsqkxks.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hammf.cn/gthxlsakpw.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ybcxt.top/gtpdonnyvz.html

[J06] 计算两时间之差
来源：http://hz.xylfe.cn/gtfqnoanjv.html

Py:   (end - start).total_seconds()
来源：http://hz.c1oappe.top/gtjdfyvxey.html

PHP:  $end->diff($start)->days;
来源：http://hz.daxiang520.top/gtxkrotdci.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhijiandao.cn/gtqyztdzrp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hfpthk.cn/gtxfjhggxv.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.tian-w.cn/gtiwygixcc.html

Go:   end.Sub(start).Hours()
来源：http://hz.wangdashe.top/gtuqmmqzfs.html

Ruby: end - start                 # 返回秒数
来源：http://hz.dashuyun.cn/gtobhrenan.html

C#:   (end - start).TotalSeconds
来源：http://hz.yongpay.top/gtlznwoqqc.html

[J07] 比较两个日期
来源：http://hz.chenlongwang.top/gtqahjjuew.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jqgfzy.top/gtoncgwgyg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yj20258888.top/gtnppfhfoy.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ehwqpu.com/gtxlgvdosf.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shangyingyoupin.top/gtyitumife.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shuidangran.top/gtuhoaogpb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jianghu66.top/gthxyhkvbb.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.quarkkingdee.top/gtiolxjmjy.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.c1oappe.top/gtnfvpakhs.html

[J08] 提取年月日与星期
来源：http://hz.zhixingplan.top/gtmabwkell.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.daria6918.cn/gtxqrlzlhk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cqqwz.cn/gtjtppweew.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.gogol.net.cn/gtovtyurfg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.redwolf501.top/gttbxjwudj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shangyingyoupin.top/gtybavbrus.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.bjfxy.top/gtxwnpbuom.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.havefunace.top/gtstfbyfud.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ywan-chungtsiang.top/gtcvgoflta.html

[J09] 时区处理
来源：http://hz.ppjwa.cn/gtcxhvosjm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shanyushiyangtech.top/gtcoogltmf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.tanke756.top/gtzyxanydh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.52xcode.cn/gtwlecyzks.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnxiangtu.top/gtonsrmjbm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jqgufenzy.top/gtzwawadct.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jiagoushi.top/gthwnznikz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.chenjidiqi.icu/gtdxebjnmw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cheryme.top/gtjvyszcnn.html

[J10] 取今天 / 本月第一天
来源：http://hz.dianchejie.cn/gtrnlxkcad.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.guowangkeji.top/gtiuwsntty.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shanyushiyangkeji.top/gtyvxksswg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hnqzz.top/gtmykeasil.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sweek.top/gtckuxiwbp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.aizwys.cn/gtebgsbgkg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ydzc1.top/gtkhocxfaf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shzxlz.cn/gtjaofovek.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.fengsongda.top/gtddawzwen.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gthpiptqsc.html

K. JSON 与序列化
来源：http://hz.ivvv.top/gtnavetcue.html

================================================================================
来源：http://hz.svipenyu.cn/gtwdfiprne.html

[K01] 对象转 JSON 字符串
来源：http://hz.ivvv.top/gtfljauwwh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.tanke756.top/gtvyjayghs.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.sysykeji.top/gtihmclluy.html

JS:   JSON.stringify(obj)
来源：http://hz.ehwqpu.com/gthaayqywa.html

TS:   JSON.stringify(obj)
来源：http://hz.0kj1m.cn/gtfypfcxdy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinghuilouyu.cn/gttitkywoo.html

Go:   json.Marshal(obj)
来源：http://hz.jinqigfzy.top/gtblfhhlqs.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.smart0.xyz/gtfkvsfjdd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.aibaodan.cn/gtxkyxbage.html

[K02] JSON 字符串转对象
来源：http://hz.ybcxt.top/gtayqmhobb.html

Py:   json.loads(s)
来源：http://hz.zhaomingkeji.xyz/gtjbkszgtx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hammf.cn/gtosixyzol.html

JS:   JSON.parse(s)
来源：http://hz.tian-w.cn/gtdzoyykqp.html

TS:   JSON.parse(s)
来源：http://hz.jyoumei.cn/gtpszohzzd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yonumen.top/gtruauxrxu.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hammf.cn/gtecoybdbs.html

Ruby: JSON.parse(s)
来源：http://hz.jyoumei.cn/gtriaxdbky.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinghuilouyu.cn/gtjwhjyqyt.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jianghu66.top/gtyvllikte.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xuetiantiany.cn/gtltiumwhi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258888.top/gtnsyfbvbu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.feifeiyinyue.top/gtmmsopjgf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sxryk.cn/gthvjazjio.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.fengsongda.top/gtjqxtnuiv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yueranfly.top/gtqigsgnac.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.dianchejie.cn/gtjiipaqda.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hysaishi.cn/gtmctspyfz.html

[K04] 读取 JSON 文件
来源：http://hz.hongshengwenyu.top/gtowcqebsi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cqqwz.cn/gtiawmpnib.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinyuanbaomall.cn/gtesrswygd.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yuanzhike.top/gtutduhmpz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hfpthk.cn/gtzmowlxjl.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.andypj.xyz/gtuopcyclz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.iojbl.cn/gtmkxyeobc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jqgufenzy.top/gtmxigsvql.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.52xcode.cn/gtcjbwfyke.html

[K05] 深拷贝对象
来源：http://hz.gotoacloud.top/gtlmpexuaq.html

Py:   copy.deepcopy(obj)
来源：http://hz.shanyushiyangkeji.top/gtjsylnfxb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.havefunace.top/gthnvjmrdh.html

JS:   structuredClone(obj)
来源：http://hz.quarkkingdee.top/gtwfluyvft.html

TS:   structuredClone(obj)
来源：http://hz.xziqi.cn/gtpftqdotc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xuetiantiany.cn/gtnpcwmnie.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhaomingkeji.xyz/gthtoxsllk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.nanxuanxn.top/gtbonaackh.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.yj20258.top/gtkoskqsnl.html

[K06] 解析 URL 查询串
来源：http://hz.dianchejie.cn/gtppmigsqw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ydjk.org.cn/gtgsphepsg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cdnleiting.top/gttxddofgp.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gaohongyu789.top/gtrypjkrxc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shzxlz.cn/gtidcvtbis.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hnqzz.top/gtlsfneifo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhoulong.xyz/gtlipzjrst.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jianghu66.top/gtrwecqwwd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.dashuyun.cn/gtbfhzjybd.html

[K07] 进制转换
来源：http://hz.yangfankeji.com/gtnwxqxalw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yonumen.top/gtzfixxdqe.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.feifeiyinyue.top/gtpxbgehtf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.pengpengdd.cyou/gtanjouijs.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.jinqigfzy.top/gtbjishdfu.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.kuanghao11.cn/gtqkxcmxzs.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.meibo888.top/gtptfyeevl.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.tian-w.cn/gtdghupldm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.iojbl.cn/gtlauxqqow.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.quarkkingdee.top/gtjerdcpdg.html

Py:   pickle.dumps(obj)
来源：http://hz.yvedp.cn/gtbqpiehel.html


<!-- 参考信息 -->