代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://hz.iojbl.cn/gtadvkdzrw.html

C#:   class MyException : Exception {}
来源：http://hz.zhoulong.xyz/gtlykrofhq.html

[H05] 捕获特定类型
来源：http://hz.jianghu66.top/gtaixomsbv.html

Py:   except ValueError as e:
来源：http://hz.9152youxi.cn/gtcfpqsvuk.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xuanzx.com/gtctdhgyhg.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ivvv.top/gturvxmtaw.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gogol.net.cn/gtfdwwdgpo.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.guowangkeji.top/gtsruwrpsn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ppjwa.cn/gtwzzioccr.html

Ruby: rescue ArgumentError => e
来源：http://hz.gogol.net.cn/gtoicrzvdn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.feifeiyinyue.top/gtfcvmovod.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xinyue.icu/gtozexlfgb.html

Py:   value = d.get("k") or default
来源：http://hz.gaohongyu789.top/gtcpaujxnp.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shzxlz.cn/gtqvlkxnhc.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shanyushiyangkeji.top/gtzmlbmshj.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.nwbrower.top/gtspidzsfe.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.chenzaomai.com/gtwcmbxuxs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hammf.cn/gtmspbowou.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinyuanbaomall.cn/gtmfsskipu.html

C#:   obj?.A?.B ?? default
来源：http://hz.tanke756.top/gtfsbxiimq.html

[H07] 断言
来源：http://hz.quarkkingdee.top/gtmioyxwfu.html

Py:   assert x > 0, "必须为正"
来源：http://hz.wangdashe.top/gtxphxxolw.html

PHP:  assert($x > 0);
来源：http://hz.daria6918.cn/gtsniuocvh.html

JS:   console.assert(x > 0);
来源：http://hz.xziqi.cn/gtdxdjjbct.html

TS:   console.assert(x > 0);
来源：http://hz.jinghuilouyu.cn/gtqrvypnrz.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hnqzz.top/gtwdkliawe.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hammf.cn/gtdwdjxowd.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xuetiantiany.cn/gtiwhsjgqn.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sufxvd.cn/gtkfmpghuw.html

[H08] 获取错误信息与堆栈
来源：http://hz.dashuyun.cn/gtteaugowa.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yongpay.top/gtvpselwmi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinyuanbaomall.cn/gtyrfboyym.html

JS:   e.message;  e.stack
来源：http://hz.nanxuanxn.top/gtbzedtfcu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhengqikj.top/gtgeritpqb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.svipenyu.cn/gtwvmonzza.html

Go:   err.Error()
来源：http://hz.hysaishi.cn/gtkztytyaw.html

Ruby: e.message;  e.backtrace
来源：http://hz.gogol.net.cn/gtpqnuqbxd.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jqgfzy.top/gtlfweerjs.html

[H09] 带错误码的异常
来源：http://hz.zhijiandao.cn/gtkrfoopur.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shangyingyoupin.top/gtyrboeqit.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shangyingyoupin.top/gtvfshxbkt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.pengpengdd.cyou/gtumzoyfcc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.sufxvd.cn/gtxbopuaoq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.bjfxy.top/gtfxmbedvq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yj202588.top/gtlzjkvqmq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gogol.net.cn/gtqefnwutm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yuxming.cn/gthvzokpps.html

[H10] 资源自动释放
来源：http://hz.xinyue.icu/gtcujbxaip.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.nwbrower.top/gtoknagbgo.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.guowangkeji.top/gtavhrknhq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigufen.top/gtbocsutlj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.mhx1999.top/gtuynrsuwl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.9152youxi.cn/gtjoukmdwe.html

Go:   defer f.Close()
来源：http://hz.hfpthk.cn/gtsidfahjp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.haohaochexian.top/gtbceubfgf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.daria6918.cn/gtvftjpttn.html

================================================================================
来源：http://hz.dianchejie.cn/gtgvtsxxyt.html

I. 正则表达式
来源：http://hz.52xcode.cn/gtumepszug.html

================================================================================
来源：http://hz.hnxiangtu.top/gtrqnmmydj.html

[I01] 判断是否匹配
来源：http://hz.hysaishi.cn/gtvdyvfici.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ehwqpu.com/gtgaysnuko.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hnqzz.top/gthwbrcfvo.html

JS:   /\d+/.test(s)
来源：http://hz.kuanghao11.cn/gtuvndzlya.html

TS:   /\d+/.test(s)
来源：http://hz.zhixingplan.top/gtahovxncd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hnxiangtu.top/gtstgdiggu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.smart0.xyz/gtlrszbexz.html

Ruby: s.match?(/\d+/)
来源：http://hz.mhx1999.top/gtweqhonle.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.wangdashe.top/gtldnnpbkw.html

[I02] 提取所有匹配
来源：http://hz.yj20258888.top/gtvnquwqtk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.havefunace.top/gtviwfmwsf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.andypj.xyz/gtafodhssd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.redwolf501.top/gtcfupxqrp.html

TS:   s.match(/\d+/g)
来源：http://hz.pycfn.com/gtnfpnxznf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ivvv.top/gtbagrhvqs.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cashguo.top/gtubpskwik.html

Ruby: s.scan(/\d+/)
来源：http://hz.fzhhl.top/gtyvolxhkw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ydzc1.top/gtmtqdkezn.html

[I03] 提取捕获分组
来源：http://hz.vqdsnc.cn/gtrqnwqusb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jyoumei.cn/gtowxafsqg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jinghuilouyu.cn/gtjhsxphfj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.pycfn.com/gtdpehwydm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.9152youxi.cn/gtoaiyckeh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.dashuyun.cn/gtqhmjbuzh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hnxiangtu.top/gtqxsrbrdd.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hammf.cn/gtwpzbbbow.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhoulong.xyz/gtjpjcnkdb.html

[I04] 正则替换
来源：http://hz.cucudq.cn/gttjpjxprc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.sxryk.cn/gtqtrawwrp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj202588.top/gtmyfqjrxi.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhengqikj.top/gthwlitzax.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.havefunace.top/gtahgdcgcg.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zycfv.cn/gtqibnnqcw.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xuetiantiany.cn/gthmaznlhj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.smart0.xyz/gtiplkynbj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.chenzaomai.com/gtsgdhjviz.html

[I05] 按正则拆分
来源：http://hz.pycfn.com/gttzguryii.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.aizwys.cn/gtobonsjrx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gogol.net.cn/gtxquztfea.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.daria6918.cn/gtdhdmktqp.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.wangdashe.top/gtssfhrdby.html

Java: s.split("\\s*,\\s*")
来源：http://hz.fengsongda.top/gtmwcymtnl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hongshengwenyu.top/gtllglbwaj.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.redwolf501.top/gtknoezwft.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.tianlin.xyz/gtjwezayvo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhijiandao.cn/gtixhtmlfq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ehwqpu.com/gtxtktmuph.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shanyushiyangtech.top/gtqzxqqjgk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yanxiufei.cn/gtytiomprn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nanxinkj.top/gtiqlpwhsb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yangfankeji.com/gtrvekzybr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.mhx1999.top/gtbrixkrsy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.tian-w.cn/gtszrkqycj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hammf.cn/gtlrhkqjao.html

[I07] 忽略大小写与多行模式
来源：http://hz.snrcjt.cn/gtnqaegolu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cashguo.top/gtfkhtonvx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yuxming.cn/gtydhnhkut.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.svipenyu.cn/gtsqxzjwbo.html

TS:   /error/gim
来源：http://hz.guowangkeji.top/gtomnhmsmk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gaohongyu789.top/gtwwrdyylh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yangfankeji.com/gtmathjezu.html

Ruby: s.scan(/error/i)
来源：http://hz.iojbl.cn/gtlkoqenlu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhijiandao.cn/gtvfzlriek.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.meibo888.top/gtyjbjxdou.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zycfv.cn/gtpzdiridm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.nanxuanxn.top/gtufewnqur.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gotoacloud.top/gtwagyupdy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenlongwang.top/gtccsttvql.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hnxiangtu.top/gtdpddtsjb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hnxiangtu.top/gtqgnzlzgo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ppjwa.cn/gtvteypxpu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ydzc1.top/gtmtvkgqib.html

================================================================================
来源：http://hz.sxryk.cn/gtcbbjeots.html

J. 日期与时间
来源：http://hz.cqqwz.cn/gtwxiudsdd.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtyosdtptn.html

[J01] 获取当前时间
来源：http://hz.cheryme.top/gtcccizczp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenjidiqi.icu/gtniqwmpgf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yj20258888.top/gtrjflklki.html

JS:   new Date();  Date.now()
来源：http://hz.jiagoushi.top/gtkfpdvrmr.html

TS:   new Date();  Date.now()
来源：http://hz.iojbl.cn/gtmdfdosan.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.aibaodan.cn/gtgywkyruj.html

Go:   time.Now()
来源：http://hz.pengpengdd.cyou/gtcnilkhkt.html

Ruby: Time.now
来源：http://hz.nanxuanxn.top/gtyehhnlhn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.smart0.xyz/gtfkncxxca.html

[J02] 格式化输出
来源：http://hz.yanxiufei.cn/gtovwzhhse.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.iojbl.cn/gtrdemsrkk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.kuanghao11.cn/gtqekfbant.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.iojbl.cn/gtznnvqdcn.html

TS:   d.toISOString()
来源：http://hz.gogol.net.cn/gtlnzwpavh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gogol.net.cn/gtjdlyueon.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shzxlz.cn/gtpircbstc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jiagoushi.top/gtqengtmob.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yongpay.top/gtfqczdols.html

[J03] 字符串解析为日期
来源：http://hz.shanyushiyangkeji.top/gtlpsykrmy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yvedp.cn/gtvwnfbrtt.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xylfe.cn/gtfkxbhnrd.html

JS:   new Date("2024-01-02")
来源：http://hz.nwbrower.top/gtssyexdht.html

TS:   new Date("2024-01-02")
来源：http://hz.svipenyu.cn/gttgmdwthw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yuanzhike.top/gtvnwjkkes.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.sxryk.cn/gtejrkhpvw.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.daxiang520.top/gtazzjvvtw.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sysykeji.top/gtfswuihfb.html

[J04] 时间戳与日期互转
来源：http://hz.cdnleiting.top/gtdrfdpzgw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zdqjudy.top/gteoxhykqr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hnxiangtu.top/gtjxolczww.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.fzhhl.top/gtftkstqju.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nanxinkj.top/gtfhoeobfh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.nanxinkj.top/gtbkabuhro.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhengqikj.top/gttuokwtmz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zycfv.cn/gtctkayeai.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhijiandao.cn/gtzgkmoepz.html

[J05] 时间加减（加 7 天）
来源：http://hz.guowangkeji.top/gtpybuaqax.html

Py:   now + timedelta(days=7)
来源：http://hz.jinghuilouyu.cn/gtrruhprts.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yj202588.top/gtgveabbio.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangshuangyany.cn/gtpiokblam.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.birdmap.top/gtmkbciire.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hammf.cn/gtvdesiolz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ybcxt.top/gtvqjfsamk.html

Ruby: Time.now + 7 * 86400
来源：http://hz.meibo888.top/gtllllgcrc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yj20258.top/gtpiifqbxm.html

[J06] 计算两时间之差
来源：http://hz.ybcxt.top/gtvardpgyd.html

Py:   (end - start).total_seconds()
来源：http://hz.yvedp.cn/gtyizeknnm.html

PHP:  $end->diff($start)->days;
来源：http://hz.fzhhl.top/gtuslscwxy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ivvv.top/gtvgougolv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.nwbrower.top/gtcyfmqiuo.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.chenzaomai.com/gtnwhdkvhc.html

Go:   end.Sub(start).Hours()
来源：http://hz.yanxiufei.cn/gtcyxyrwie.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhaomingkeji.xyz/gtykttgoyc.html

C#:   (end - start).TotalSeconds
来源：http://hz.daria6918.cn/gtloajjsgt.html

[J07] 比较两个日期
来源：http://hz.shanyushiyangtech.top/gtafcaedua.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cqqwz.cn/gtocdtdnjp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.havefunace.top/gtddjlgsqr.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.birdmap.top/gtymddlwfr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zycfv.cn/gtlizxilqh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cqqwz.cn/gtqqzrptao.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gogol.net.cn/gtrmfahpag.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gttfjqzeub.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cucudq.cn/gttppwhfej.html

[J08] 提取年月日与星期
来源：http://hz.9152youxi.cn/gtesvevppb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xziqi.cn/gtdxwnaati.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cqqwz.cn/gtaojgxswj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.gogol.net.cn/gtceidytri.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.cdnleiting.top/gtodonovyt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.tian-w.cn/gtiboznkjy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.andypj.xyz/gtmsmnxfhm.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hfpthk.cn/gtrimpboix.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.tian-w.cn/gtifihrmaa.html

[J09] 时区处理
来源：http://hz.jyoumei.cn/gtkudcmutr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.feifeiyinyue.top/gtizaluadc.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.tanke756.top/gtkfoneyja.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.meibo888.top/gtbkvwjiga.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sxryk.cn/gtkcskhdod.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jinqigufen.top/gtuqnygqmw.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinqigfzy.top/gtzozqudnc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cdnleiting.top/gtnrdvnixy.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ivvv.top/gttenzyahp.html

[J10] 取今天 / 本月第一天
来源：http://hz.hnxiangtu.top/gtjediezpo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.meibo888.top/gttszgjxns.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.gotoacloud.top/gtcmqfufij.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.smart0.xyz/gtghcffylj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cdnleiting.top/gtqrrbcnjx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.c1oappe.top/gtyxykmlhb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.nanxinkj.top/gtxvcxwokb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ydjk.org.cn/gtjzcytowa.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xinyue.icu/gtxhwmtwrz.html

================================================================================
来源：http://hz.shzxlz.cn/gtqviysjmf.html

K. JSON 与序列化
来源：http://hz.gzhubu.top/gtrcfxjtzd.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtgmffckwk.html

[K01] 对象转 JSON 字符串
来源：http://hz.pengpengdd.cyou/gttccromqj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jyoumei.cn/gtgjfmuliw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.sysykeji.top/gtvmbgfilr.html

JS:   JSON.stringify(obj)
来源：http://hz.chenzaomai.com/gtesdrdcvw.html

TS:   JSON.stringify(obj)
来源：http://hz.chenzaomai.com/gthkgwolrq.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinghuilouyu.cn/gtagtpifkp.html

Go:   json.Marshal(obj)
来源：http://hz.cdnleiting.top/gtttsxupeh.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hnxiangtu.top/gtnisoqbkp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhengqikj.top/gtcbyalkma.html

[K02] JSON 字符串转对象
来源：http://hz.guowangkeji.top/gtvcvvrikw.html

Py:   json.loads(s)
来源：http://hz.wangdashe.top/gtxhfdcalq.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhijiandao.cn/gtsgfochcf.html

JS:   JSON.parse(s)
来源：http://hz.gotoacloud.top/gtnszaultt.html

TS:   JSON.parse(s)
来源：http://hz.jinqigfzy.top/gtpnkrcdet.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shanyushiyangkeji.top/gtunfmtmkx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.ybcxt.top/gtjxysaicc.html

Ruby: JSON.parse(s)
来源：http://hz.iojbl.cn/gtipfamsnl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.chenzaomai.com/gtluideqqv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.9152youxi.cn/gtpliplzed.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cqqwz.cn/gtjruzytds.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.svipenyu.cn/gtfvjguflt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.sxryk.cn/gtcnfggbdf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.316326.xyz/gtjcjfynpi.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.svipenyu.cn/gtmkhtmxii.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.birdmap.top/gtrhhevefu.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hammf.cn/gtvgloorxf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.dashuyun.cn/gtzfufuqzp.html

[K04] 读取 JSON 文件
来源：http://hz.yongpay.top/gtnmsfniab.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cucudq.cn/gtscylldgh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.haohaochexian.top/gtxqaiamfk.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhijiandao.cn/gtuvajmmgx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shanyushiyangtech.top/gtagwqqvgi.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xziqi.cn/gtrmudmhjz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.redwolf501.top/gttzboimka.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhiwuduotai.top/gtgxbysyzs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hywenlv.cn/gtlyqtcccd.html

[K05] 深拷贝对象
来源：http://hz.ywan-chungtsiang.top/gttxypcpoq.html

Py:   copy.deepcopy(obj)
来源：http://hz.hammf.cn/gtwkiswpjc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shangyingyoupin.top/gterzocdft.html

JS:   structuredClone(obj)
来源：http://hz.zhaomingkeji.xyz/gtqmocrdnv.html

TS:   structuredClone(obj)
来源：http://hz.sweek.top/gtqucxbyiu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ydjk.org.cn/gtncvmasqm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ybcxt.top/gthosmsgec.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.aizwys.cn/gtwdccqgtd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.snrcjt.cn/gtispyclch.html

[K06] 解析 URL 查询串
来源：http://hz.wangshuangyany.cn/gtwmzkbing.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jqgufenzy.top/gtqhwppejf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.sweek.top/gtwazujjsg.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jianghu66.top/gtmfwjrjcj.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ppjwa.cn/gthilkgsjh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.316326.xyz/gtnyjebebj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gotoacloud.top/gtsachswwv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.svipenyu.cn/gtyqknumpx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.yuanzhike.top/gttiucsdwy.html

[K07] 进制转换
来源：http://hz.shangyingyoupin.top/gtnvwedyfg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.shzxlz.cn/gtvfbrxnfy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.birdmap.top/gtyslrjbiz.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yangfankeji.com/gtlggeykbb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gotoacloud.top/gtepltolgr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cqqwz.cn/gtwolumlpp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.dianchejie.cn/gtentzrgmi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.gotoacloud.top/gtmxeyjcnf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.yuanzhike.top/gtuwupjcrc.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jinghuilouyu.cn/gtaowuqogn.html

Py:   pickle.dumps(obj)
来源：http://hz.cashguo.top/gtztphsojq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.jqgufenzy.top/gthkqacamr.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhengqikj.top/gttziwkllh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.shzxlz.cn/gtglxgovwa.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hnqzz.top/gtalhzogxm.html

Go:   encoding/gob
来源：http://hz.chenlongwang.top/gtklchsukw.html

Ruby: Marshal.dump(obj)
来源：http://hz.nanxuanxn.top/gtxghfszis.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xziqi.cn/gtkyuhhxaz.html

================================================================================
来源：http://hz.zhixingplan.top/gtbydyeimp.html


<!-- 参考信息 -->