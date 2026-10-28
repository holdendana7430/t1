代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhijiandao.cn/gtyfnnjviu.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.sufxvd.cn/gtgcrpvipz.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.aizwys.cn/gtaqaadxeu.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cheryme.top/gtperlpnbe.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.bjfxy.top/gtvanlazcg.html

Ruby: rescue ArgumentError => e
来源：http://hz.sweek.top/gtqrzlybao.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ydzc1.top/gtmgwpkhfp.html

[H06] 可选值 / 空值安全访问
来源：http://hz.chenjidiqi.icu/gtklsohkjb.html

Py:   value = d.get("k") or default
来源：http://hz.ivvv.top/gtuqzmtvdp.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.316326.xyz/gtwtuvoabv.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jianghu66.top/gtgdnierua.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinghuilouyu.cn/gtcrovsohi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cheryme.top/gtlruxvqjj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cheryme.top/gtntrougmq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xuetiantiany.cn/gtdxyiqojf.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinqigfzy.top/gtdsbkuzlv.html

[H07] 断言
来源：http://hz.shuidangran.top/gtqrooggrw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yanxiufei.cn/gtnqmhqzva.html

PHP:  assert($x > 0);
来源：http://hz.pycfn.com/gtdeyxnbya.html

JS:   console.assert(x > 0);
来源：http://hz.hywenlv.cn/gtttwurbbs.html

TS:   console.assert(x > 0);
来源：http://hz.sufxvd.cn/gtomsyfnkz.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xuanzx.com/gtpqslerug.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ywan-chungtsiang.top/gttfmalmzr.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yanxiufei.cn/gtwetkquix.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sysykeji.top/gtvrpomvtz.html

[H08] 获取错误信息与堆栈
来源：http://hz.jlsjyb.cn/gtehuxvupj.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.pycfn.com/gtekmohxrp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.fzhhl.top/gtlrfdnurl.html

JS:   e.message;  e.stack
来源：http://hz.hysaishi.cn/gtwvdkcqha.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.pengpengdd.cyou/gtwjgylkyc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hnqzz.top/gtletyqjkc.html

Go:   err.Error()
来源：http://hz.dianchejie.cn/gtxcvykshf.html

Ruby: e.message;  e.backtrace
来源：http://hz.sufxvd.cn/gttcvozqve.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhaomingkeji.xyz/gtwsxzgtew.html

[H09] 带错误码的异常
来源：http://hz.smart0.xyz/gttbakadxq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhaomingkeji.xyz/gtkehtfhyf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.snrcjt.cn/gtlppccfmk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.9152youxi.cn/gtdwzsqfgi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hfpthk.cn/gtzngcryyp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.nanxinkj.top/gtedggyrkt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.redwolf501.top/gtarnxmdea.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.fzhhl.top/gtyvibggrl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hnqzz.top/gtvzrctruu.html

[H10] 资源自动释放
来源：http://hz.sxryk.cn/gtnlruvart.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yuxming.cn/gtixtseswx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.feifeiyinyue.top/gtozuxkwxn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhongyouzk.top/gtcviuagsw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nwbrower.top/gtmmddhjoo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.feifeiyinyue.top/gtcjewduuu.html

Go:   defer f.Close()
来源：http://hz.ybcxt.top/gtihfmiwes.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hongshengwenyu.top/gtbsfvovtk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.vqdsnc.cn/gttsloixnm.html

================================================================================
来源：http://hz.pycfn.com/gtetkhuaih.html

I. 正则表达式
来源：http://hz.c1oappe.top/gtutdxmrwy.html

================================================================================
来源：http://hz.tanke756.top/gtmzorfdlm.html

[I01] 判断是否匹配
来源：http://hz.cheryme.top/gtstpkatny.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yongpay.top/gtbsdrkfet.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.daria6918.cn/gtaotkxxax.html

JS:   /\d+/.test(s)
来源：http://hz.cdnleiting.top/gtqjkqopkl.html

TS:   /\d+/.test(s)
来源：http://hz.zhiwuduotai.top/gtqwykjdeq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yueranfly.top/gttbducbah.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.iojbl.cn/gtkpzhyugc.html

Ruby: s.match?(/\d+/)
来源：http://hz.cashguo.top/gtivjfyhgy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shanyushiyangtech.top/gtovjaettk.html

[I02] 提取所有匹配
来源：http://hz.hfpthk.cn/gtmlfadpjn.html

Py:   re.findall(r"\d+", s)
来源：http://hz.nanxuanxn.top/gthyfqjdiu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj20258888.top/gtqwqndgzk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.snrcjt.cn/gtocodzvcm.html

TS:   s.match(/\d+/g)
来源：http://hz.xuetiantiany.cn/gtbanwqneb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jqgfzy.top/gtotoiczfu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.dashuyun.cn/gtpbhchidl.html

Ruby: s.scan(/\d+/)
来源：http://hz.yj20258.top/gtuirdhfjv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yonumen.top/gtyetivzgq.html

[I03] 提取捕获分组
来源：http://hz.mhx1999.top/gtnhkzshqp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.tian-w.cn/gtoqvspref.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.c1oappe.top/gtgzhwgtpm.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cqqwz.cn/gtahubtokd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hnqzz.top/gtqnvaeoej.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yvedp.cn/gtlhgnhybw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.fengsongda.top/gthpzhzrxs.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shanyushiyangtech.top/gtfgpavchi.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.pycfn.com/gticmasxjj.html

[I04] 正则替换
来源：http://hz.sweek.top/gtxvwrcegr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.tian-w.cn/gtdhxuuqjs.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gogol.net.cn/gtcgluxfxq.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgfzy.top/gtezrcroqc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cashguo.top/gtrsrlazaj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.wangshuangyany.cn/gtpfnpxanx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cucudq.cn/gtjrizuogn.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xziqi.cn/gtnchuysxv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.fengsongda.top/gtstumvuaj.html

[I05] 按正则拆分
来源：http://hz.xuanzx.com/gtrevogffh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.pengpengdd.cyou/gtbufksmmk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.meibo888.top/gthjcpsmtz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xingfuxueyuan.xyz/gtgpyhqwch.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jinyuanbaomall.cn/gtvmzeqarw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.aizwys.cn/gtvvbdshfo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yangfankeji.com/gtbqgccesd.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.tanke756.top/gtogwtuxqb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hnxiangtu.top/gtifnyclwu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.nanxuanxn.top/gtutzzmgus.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.nanxuanxn.top/gtbgmafiph.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jianghu66.top/gtrdngbcnd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhoulong.xyz/gtxbxdslzi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yuxming.cn/gtnfhxrrnv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.bjfxy.top/gtdtbmkdft.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.quarkkingdee.top/gtpenpjyki.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhoulong.xyz/gtgkfrhkus.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jinghuilouyu.cn/gtrqfetfgm.html

[I07] 忽略大小写与多行模式
来源：http://hz.aibaodan.cn/gtwqloqzmc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhijiandao.cn/gtizvabxng.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhoulong.xyz/gtsqegqlbj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ywan-chungtsiang.top/gtrjaauwdj.html

TS:   /error/gim
来源：http://hz.hongshengwenyu.top/gtflfppmtz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ppjwa.cn/gtsjjlfcoq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yonumen.top/gtzmfrjndh.html

Ruby: s.scan(/error/i)
来源：http://hz.zhixingplan.top/gtpsqoimki.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jlsjyb.cn/gtcqeknvsl.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ybcxt.top/gtdcnvoyxb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.52xcode.cn/gthldxlyap.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.guannengcc.top/gtyrsckgkt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenjidiqi.icu/gtuyhcsedr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuxming.cn/gtyaxaylsf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yuanzhike.top/gtjhszexiv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.tanke756.top/gtxxqavgei.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhijiandao.cn/gtspqapxcr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.bjfxy.top/gtcinhmnda.html

================================================================================
来源：http://hz.yvedp.cn/gtocpwqzze.html

J. 日期与时间
来源：http://hz.xylfe.cn/gtiqdyxqfn.html

================================================================================
来源：http://hz.zycfv.cn/gtqsrlwdtl.html

[J01] 获取当前时间
来源：http://hz.smart0.xyz/gtdmlyhnhg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.wangdashe.top/gtvdkgupki.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jyoumei.cn/gttyfhevwz.html

JS:   new Date();  Date.now()
来源：http://hz.sxryk.cn/gtxtrqqghk.html

TS:   new Date();  Date.now()
来源：http://hz.jianghu66.top/gtyuafneyp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yj20258888.top/gthgglfmmq.html

Go:   time.Now()
来源：http://hz.yj20258.top/gtnfthypic.html

Ruby: Time.now
来源：http://hz.wangshuangyany.cn/gtxniknhvz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.havefunace.top/gtcuuzrrmb.html

[J02] 格式化输出
来源：http://hz.c1oappe.top/gtmtwptqef.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shanyushiyangkeji.top/gtgnigzjyq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.daxiang520.top/gthkwoxfio.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.chenlongwang.top/gtcluttsbs.html

TS:   d.toISOString()
来源：http://hz.tianlin.xyz/gtfiblsuyf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xinyue.icu/gtsaokrftt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhaomingkeji.xyz/gtyeyuphjb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258.top/gtjawlrctb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.dianchejie.cn/gtzrfrmnam.html

[J03] 字符串解析为日期
来源：http://hz.zhongyouzk.top/gtmktcujjh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.haohaochexian.top/gtuvnmhgsx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.nwbrower.top/gtvkcxtaya.html

JS:   new Date("2024-01-02")
来源：http://hz.daxiang520.top/gtsplhdepi.html

TS:   new Date("2024-01-02")
来源：http://hz.yj20258888.top/gtuztcbfqf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.tanke756.top/gthujukjlt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.guannengcc.top/gtnohgyzue.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.dashuyun.cn/gtskkeocuh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jiagoushi.top/gthaecgenf.html

[J04] 时间戳与日期互转
来源：http://hz.jinghuilouyu.cn/gtwudolvyv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.chenzaomai.com/gtcpudqjbr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.wangshuangyany.cn/gtbuonlvay.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jyoumei.cn/gtbptmidja.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.guowangkeji.top/gtdtxzmpin.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.vqdsnc.cn/gtbnjjfpax.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sweek.top/gtqzlebbag.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.andypj.xyz/gtgbsrhiby.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ywan-chungtsiang.top/gtydvvflfv.html

[J05] 时间加减（加 7 天）
来源：http://hz.316326.xyz/gtwdhlyqvy.html

Py:   now + timedelta(days=7)
来源：http://hz.vqdsnc.cn/gtexdqyzjw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sufxvd.cn/gtmaaylsav.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cashguo.top/gtaeijvqyj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tanke756.top/gtdupudajo.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cashguo.top/gtawlgzsxp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hongshengwenyu.top/gtbkrvzidx.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cqqwz.cn/gtfozpcjcm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.9152youxi.cn/gtgdawonyj.html

[J06] 计算两时间之差
来源：http://hz.jinyuanbaomall.cn/gtzycwjsmx.html

Py:   (end - start).total_seconds()
来源：http://hz.jiagoushi.top/gttkfvuypn.html

PHP:  $end->diff($start)->days;
来源：http://hz.ywan-chungtsiang.top/gtbnrvnsoh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.fzhhl.top/gtnqbolljh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ehwqpu.com/gtvekrzamo.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ydjk.org.cn/gtjznakyhw.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhixingplan.top/gteigliium.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jinghuilouyu.cn/gtpcawqwhb.html

C#:   (end - start).TotalSeconds
来源：http://hz.yanxiufei.cn/gtdnptkvyw.html

[J07] 比较两个日期
来源：http://hz.jinyuanbaomall.cn/gtvyturbod.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jiagoushi.top/gtqwhomkma.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hywenlv.cn/gtjxeoerfa.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258888.top/gtvfmiiemo.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.fengsongda.top/gtdscileld.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hywenlv.cn/gtacvipjmy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.chenlongwang.top/gtbcozgwme.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ydjk.org.cn/gtckzwytsu.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.fzhhl.top/gtjcybevzz.html

[J08] 提取年月日与星期
来源：http://hz.gaohongyu789.top/gtqkyyetbv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.pycfn.com/gtsdsgmhdm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.haohaochexian.top/gtlioxbmcq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yanxiufei.cn/gtkhhubqgd.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sweek.top/gtqszwufys.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.snrcjt.cn/gtvorbjtvs.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.aibaodan.cn/gtegihjgzu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yanxiufei.cn/gtxjsqnlkc.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ywan-chungtsiang.top/gtwzguozpl.html

[J09] 时区处理
来源：http://hz.nwbrower.top/gtuebphigc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.feifeiyinyue.top/gtofwkvmzz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.pycfn.com/gtgtivrnfz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.feifeiyinyue.top/gtrhjrraku.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gtgwmrglys.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhixingplan.top/gtffgaysic.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sufxvd.cn/gtzeryowsf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinyuanbaomall.cn/gtdknptgyo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinqigfzy.top/gtzcwoouba.html

[J10] 取今天 / 本月第一天
来源：http://hz.yueranfly.top/gtzwodqugm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.fengsongda.top/gttdgclemq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.wangshuangyany.cn/gtmastnwtk.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yongpay.top/gtmblqkvrr.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ivvv.top/gtlnbcsjdl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zdqjudy.top/gtoggexslv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.pengpengdd.cyou/gtzdoxbqjd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.iojbl.cn/gtdfpawhdr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinqigfzy.top/gtikktqrrx.html

================================================================================
来源：http://hz.zhengqikj.top/gtjqbonyaq.html

K. JSON 与序列化
来源：http://hz.52xcode.cn/gtwplzpzgw.html

================================================================================
来源：http://hz.hysaishi.cn/gtwfqdqctk.html

[K01] 对象转 JSON 字符串
来源：http://hz.yangfankeji.com/gtdrcyxbvo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yj20258888.top/gtfnhnctgo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ivvv.top/gtnzfetrhu.html

JS:   JSON.stringify(obj)
来源：http://hz.xinyue.icu/gtdphfpntk.html

TS:   JSON.stringify(obj)
来源：http://hz.tianlin.xyz/gtcxtrjsyz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shanyushiyangkeji.top/gtpynlgqws.html

Go:   json.Marshal(obj)
来源：http://hz.yj20258888.top/gtotbenueo.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zdqjudy.top/gtuxdgxwsr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zdqjudy.top/gtmlczmpft.html

[K02] JSON 字符串转对象
来源：http://hz.sxryk.cn/gtsuyhbufb.html

Py:   json.loads(s)
来源：http://hz.andypj.xyz/gtvjbfazdu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.chenzaomai.com/gtnboysolf.html

JS:   JSON.parse(s)
来源：http://hz.hywenlv.cn/gtczldcxnn.html

TS:   JSON.parse(s)
来源：http://hz.xylfe.cn/gtolykgggz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ybcxt.top/gtxsvfxdcp.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.daria6918.cn/gtqdkhhlfp.html

Ruby: JSON.parse(s)
来源：http://hz.bjfxy.top/gtxofuaknf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hammf.cn/gtqzdlaidi.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.nwbrower.top/gtyaecklhd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.sysykeji.top/gtqhzadmdx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gaohongyu789.top/gtoywzfkop.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xingfuxueyuan.xyz/gtjhlnydys.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj202588.top/gtsxadqqaw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shanyushiyangtech.top/gteoijvslb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.redwolf501.top/gtqwvhhoxw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jinyuanbaomall.cn/gtirchcfuo.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.mhx1999.top/gtmaokbqwx.html

[K04] 读取 JSON 文件
来源：http://hz.chenjidiqi.icu/gtasoitkmo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xziqi.cn/gtfqjxvigh.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.gzhubu.top/gtsvcdwqdj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.wangshuangyany.cn/gtbpgbylvs.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yongpay.top/gtrpsmmulv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.shzxlz.cn/gtjzqrdsht.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hnqzz.top/gtgoosbobk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.xziqi.cn/gtqtgiujjd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xuetiantiany.cn/gtzstuksnx.html

[K05] 深拷贝对象
来源：http://hz.jinghuilouyu.cn/gtdneziwmo.html

Py:   copy.deepcopy(obj)
来源：http://hz.hongshengwenyu.top/gtmvhdbfae.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xinyue.icu/gtkixhkwgo.html

JS:   structuredClone(obj)
来源：http://hz.cdnleiting.top/gtdkozniix.html

TS:   structuredClone(obj)
来源：http://hz.yuanzhike.top/gtyppzyhhx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.c1oappe.top/gthxexgaeg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.aibaodan.cn/gtuxkalafd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shanyushiyangtech.top/gtjchqlftq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.nwbrower.top/gtfmclejpg.html

[K06] 解析 URL 查询串
来源：http://hz.hysaishi.cn/gtckycwjkg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zycfv.cn/gteahzopty.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xziqi.cn/gtzvvlmyqv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.quarkkingdee.top/gtxrsqrzvb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.chenjidiqi.icu/gtklxmqiom.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hammf.cn/gtdcprqlli.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hywenlv.cn/gtttbqagsw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.xinyue.icu/gtosodkhkz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.pengpengdd.cyou/gtkvltphsd.html

[K07] 进制转换
来源：http://hz.yuxming.cn/gtozoxzncx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.yj20258.top/gticeofnlw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.redwolf501.top/gtulxvbfey.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yj202588.top/gtalzzuynz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.xziqi.cn/gtfuqrethe.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jqgufenzy.top/gtyjvwmzrl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sysykeji.top/gtrjnuhmuo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hywenlv.cn/gtwoynzcui.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.tianlin.xyz/gteigosdke.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.fengsongda.top/gtvzkeketh.html

Py:   pickle.dumps(obj)
来源：http://hz.daria6918.cn/gtnkplafvn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhijiandao.cn/gttxitzlwt.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhaomingkeji.xyz/gtllswgoij.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.wangdashe.top/gtffvwaqbf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.redwolf501.top/gtyreuktxs.html

Go:   encoding/gob
来源：http://hz.gogol.net.cn/gtrpjtfqgh.html

Ruby: Marshal.dump(obj)
来源：http://hz.gotoacloud.top/gtoiiothsp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jqgfzy.top/gtgedbslpn.html

================================================================================
来源：http://hz.zycfv.cn/gtoykffgnh.html

L. 网络请求
来源：http://hz.jqgufenzy.top/gtxjtwrrla.html

================================================================================
来源：http://hz.xuanzx.com/gtpsisyoea.html

[L01] 发送 GET 请求
来源：http://hz.shuidangran.top/gtgcisllze.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.xuanzx.com/gtseqvsiaz.html


<!-- 参考信息 -->