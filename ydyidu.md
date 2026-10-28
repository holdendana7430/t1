代发 wailian999

[H03] 主动抛出异常
来源：http://hz.sysykeji.top/gtiwamycjq.html

Py:   raise ValueError("错误信息")
来源：http://hz.ppjwa.cn/gttgnxufyn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.meibo888.top/gtimthzlom.html

JS:   throw new Error("错误信息");
来源：http://hz.c1oappe.top/gtmrwkoote.html

TS:   throw new Error("错误信息");
来源：http://hz.ybcxt.top/gtuqonhgsa.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.wangshuangyany.cn/gtukfminih.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.dianchejie.cn/gtfujpgduc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nwbrower.top/gtevbzaamq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ybcxt.top/gteoefiwtp.html

[H04] 自定义异常类型
来源：http://hz.guannengcc.top/gtdagrpbna.html

Py:   class MyError(Exception): pass
来源：http://hz.birdmap.top/gteohhyorf.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhongyouzk.top/gtwbyklpxw.html

JS:   class MyError extends Error {}
来源：http://hz.hysaishi.cn/gtghvasscv.html

TS:   class MyError extends Error {}
来源：http://hz.c1oappe.top/gtzlzunlgb.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhongyouzk.top/gtlhzyoxhf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xuetiantiany.cn/gtwmsbebel.html

Ruby: class MyError < StandardError; end
来源：http://hz.hysaishi.cn/gteucvyvon.html

C#:   class MyException : Exception {}
来源：http://hz.fengsongda.top/gtxmecxbbi.html

[H05] 捕获特定类型
来源：http://hz.hywenlv.cn/gtyxkjnozy.html

Py:   except ValueError as e:
来源：http://hz.wangshuangyany.cn/gtbmhzapts.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.fzhhl.top/gtcooocbzc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hongshengwenyu.top/gtlgvwpwij.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.dianchejie.cn/gtlebhzexl.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yj202588.top/gtidvnsdmg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jqgfzy.top/gttosxrvrl.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj202588.top/gtaeowinri.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xinyue.icu/gtgoghfyht.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xuanzx.com/gtnynagukc.html

Py:   value = d.get("k") or default
来源：http://hz.yangfankeji.com/gtnmldhmov.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.guowangkeji.top/gtxomotvfu.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.cqqwz.cn/gtjrbfzsno.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.chenzaomai.com/gthhmqbxyu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shangyingyoupin.top/gtqymjcpma.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.daxiang520.top/gtgiwtxlfx.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yuxming.cn/gtypvaoosd.html

C#:   obj?.A?.B ?? default
来源：http://hz.cdnleiting.top/gtxknbcagb.html

[H07] 断言
来源：http://hz.yvedp.cn/gtlaekynlk.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jyoumei.cn/gtedgxhgdv.html

PHP:  assert($x > 0);
来源：http://hz.havefunace.top/gtftvbdsng.html

JS:   console.assert(x > 0);
来源：http://hz.snrcjt.cn/gtxljuvmku.html

TS:   console.assert(x > 0);
来源：http://hz.pengpengdd.cyou/gtnmwedpvm.html

Java: assert x > 0 : "必须为正";
来源：http://hz.tian-w.cn/gtdmlnluqp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gotoacloud.top/gtussgpqdu.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.gotoacloud.top/gthvkvtnbn.html

C#:   Debug.Assert(x > 0);
来源：http://hz.daxiang520.top/gtgyguvaqp.html

[H08] 获取错误信息与堆栈
来源：http://hz.yongpay.top/gtjrxiqpwl.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tian-w.cn/gtnkglxmxy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jqgufenzy.top/gtlybrykcc.html

JS:   e.message;  e.stack
来源：http://hz.sweek.top/gtrovsgbtl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xuanzx.com/gtletqnfhv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.guowangkeji.top/gtqalmogfz.html

Go:   err.Error()
来源：http://hz.xuetiantiany.cn/gtifsxrttd.html

Ruby: e.message;  e.backtrace
来源：http://hz.fzhhl.top/gtagzejldg.html

C#:   e.Message;  e.StackTrace
来源：http://hz.meibo888.top/gtwrojzoaq.html

[H09] 带错误码的异常
来源：http://hz.smart0.xyz/gtvunusgnw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jinqigufen.top/gtmbssfwmy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.52xcode.cn/gtschziaxr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gogol.net.cn/gtvbbesrqi.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jqgfzy.top/gtbwijpmbs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jianghu66.top/gtdlkptwvr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.pengpengdd.cyou/gtaricikff.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.chenzaomai.com/gtshogxecu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xuetiantiany.cn/gtibvyover.html

[H10] 资源自动释放
来源：http://hz.tianlin.xyz/gtludhxlds.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shuidangran.top/gtvqpeeixv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yueranfly.top/gtkjruhrtn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.guannengcc.top/gtzanmicyx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ppjwa.cn/gtvvivdhfm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.52xcode.cn/gtwivixtwh.html

Go:   defer f.Close()
来源：http://hz.meibo888.top/gtldlbbbol.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xuanzx.com/gtkhuxqtna.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.mhx1999.top/gtybalfxvt.html

================================================================================
来源：http://hz.vqdsnc.cn/gtstvjigvm.html

I. 正则表达式
来源：http://hz.mhx1999.top/gtnjpkzrlp.html

================================================================================
来源：http://hz.daria6918.cn/gteohvrphf.html

[I01] 判断是否匹配
来源：http://hz.jinyuanbaomall.cn/gtvjktgxsi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ydzc1.top/gtxhoyydoi.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gzhubu.top/gtmyouwlst.html

JS:   /\d+/.test(s)
来源：http://hz.zycfv.cn/gtwdocwnvk.html

TS:   /\d+/.test(s)
来源：http://hz.chenlongwang.top/gthvzyeaxu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinyuanbaomall.cn/gtdpksqwbk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhongyouzk.top/gtpsalyvek.html

Ruby: s.match?(/\d+/)
来源：http://hz.yonumen.top/gtgmhlsyfg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.fzhhl.top/gtqmbjxmqx.html

[I02] 提取所有匹配
来源：http://hz.chenjidiqi.icu/gtnwquezfs.html

Py:   re.findall(r"\d+", s)
来源：http://hz.haohaochexian.top/gtxlvnwadr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.nanxuanxn.top/gtixfybzin.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shanyushiyangtech.top/gtpwrbwjyk.html

TS:   s.match(/\d+/g)
来源：http://hz.tian-w.cn/gtqhbffwco.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xingfuxueyuan.xyz/gtrftwdhcu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhijiandao.cn/gtkmqgamcw.html

Ruby: s.scan(/\d+/)
来源：http://hz.zdqjudy.top/gtviljoeun.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.meibo888.top/gtvyfwxzfl.html

[I03] 提取捕获分组
来源：http://hz.jinqigfzy.top/gthtbtoyvu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yanxiufei.cn/gthuhibbzt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yuxming.cn/gtpxhqbzkl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.quarkkingdee.top/gtrkzllwhl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhiwuduotai.top/gtwaqaziwd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhixingplan.top/gtspvgnjwg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jlsjyb.cn/gtlkymswwu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shzxlz.cn/gthksdjzwl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xinyue.icu/gttgmbvtlo.html

[I04] 正则替换
来源：http://hz.pycfn.com/gtxslywkwz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jlsjyb.cn/gtwqmbiaba.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhixingplan.top/gtxajjznqg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.quarkkingdee.top/gtpjpakvym.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yvedp.cn/gtbdbltjpl.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.pengpengdd.cyou/gtdsqfobir.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.cucudq.cn/gtfcaxtxqk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xinyue.icu/gtyybyawop.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.meibo888.top/gtvlvbvbeo.html

[I05] 按正则拆分
来源：http://hz.ydjk.org.cn/gtphsxnyou.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yanxiufei.cn/gtvxppjpln.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.iojbl.cn/gtmkhmlnrr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.svipenyu.cn/gtbmungzse.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sysykeji.top/gteegasslu.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenlongwang.top/gtfamzttee.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhijiandao.cn/gtvztpbklj.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jqgufenzy.top/gtgqvfukws.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.havefunace.top/gtflyvxowj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.aibaodan.cn/gtkeveqcqc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shzxlz.cn/gtbeddrmhh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.svipenyu.cn/gtfmjqwkkg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnqzz.top/gttdpmopmh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhaomingkeji.xyz/gtihmzjtfy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.shanyushiyangtech.top/gtvoafrmvn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.shangyingyoupin.top/gtobiaxwgx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ywan-chungtsiang.top/gtnzcwvrow.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jyoumei.cn/gtrnvrouex.html

[I07] 忽略大小写与多行模式
来源：http://hz.fzhhl.top/gtfmkkzwbo.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.vqdsnc.cn/gtbjkepzje.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.pycfn.com/gtsmsvxbwi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.tianlin.xyz/gtgqxszczx.html

TS:   /error/gim
来源：http://hz.ydzc1.top/gtbvxirqsr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.9152youxi.cn/gtfscadgbj.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.sweek.top/gtoobcaovf.html

Ruby: s.scan(/error/i)
来源：http://hz.316326.xyz/gttrtkguoa.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yanxiufei.cn/gtogmnbpnq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.pycfn.com/gtjdsichbd.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jqgfzy.top/gthxxyyjhq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.wangdashe.top/gtkmoclhcg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangkeji.top/gtzgjmxnuh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigfzy.top/gtcqgeeljo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ydzc1.top/gtcyaqmuqr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ydjk.org.cn/gtijdjqpqc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.aizwys.cn/gtshvcaujr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.meibo888.top/gtvvgrorvv.html

================================================================================
来源：http://hz.xuanzx.com/gtvngqnetm.html

J. 日期与时间
来源：http://hz.hnqzz.top/gtoewmlkfx.html

================================================================================
来源：http://hz.yueranfly.top/gthfjyeerq.html

[J01] 获取当前时间
来源：http://hz.cheryme.top/gtjpyshsrj.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.vqdsnc.cn/gtyeghvsud.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhengqikj.top/gtkmvrkabr.html

JS:   new Date();  Date.now()
来源：http://hz.birdmap.top/gtdyxgymkf.html

TS:   new Date();  Date.now()
来源：http://hz.aizwys.cn/gtehjblxtp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinqigfzy.top/gtwgisepjb.html

Go:   time.Now()
来源：http://hz.birdmap.top/gttnfmjiyk.html

Ruby: Time.now
来源：http://hz.shanyushiyangkeji.top/gtbdkyayjv.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yuanzhike.top/gtdblzppft.html

[J02] 格式化输出
来源：http://hz.jianghu66.top/gtrmvkjwhi.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hammf.cn/gtwseugsfe.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ydzc1.top/gtpqulrmyw.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhengqikj.top/gtxgskfnwl.html

TS:   d.toISOString()
来源：http://hz.mhx1999.top/gtffczdidp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.wangdashe.top/gtegtglvwn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yangfankeji.com/gtodyvhdbx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shanyushiyangkeji.top/gtouxkvapf.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jiagoushi.top/gtpjouyzkc.html

[J03] 字符串解析为日期
来源：http://hz.cheryme.top/gtuehbcfxd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shanyushiyangkeji.top/gtodyzygsx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zycfv.cn/gtuzlqidor.html

JS:   new Date("2024-01-02")
来源：http://hz.ehwqpu.com/gtbsqsulyf.html

TS:   new Date("2024-01-02")
来源：http://hz.yuanzhike.top/gtaazmwuem.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xuetiantiany.cn/gtldgppysa.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhoulong.xyz/gteitttmnx.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cdnleiting.top/gtwkgubdkl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.smart0.xyz/gtrtyqycjk.html

[J04] 时间戳与日期互转
来源：http://hz.316326.xyz/gtqqsjsfid.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xylfe.cn/gtdkjddqcz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.aibaodan.cn/gtkfygfibd.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gzhubu.top/gtzotcdvgc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yj20258.top/gtcstiegdj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xinyue.icu/gtpzwmwimt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.svipenyu.cn/gtfubscurr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhoulong.xyz/gttwfwustn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yuanzhike.top/gtxdjgdshf.html

[J05] 时间加减（加 7 天）
来源：http://hz.wangshuangyany.cn/gtwgfnotid.html

Py:   now + timedelta(days=7)
来源：http://hz.zhixingplan.top/gteyrnikaz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.vqdsnc.cn/gtgjocscmv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.c1oappe.top/gteemrbdrg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gogol.net.cn/gtaesqftws.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.dianchejie.cn/gtzweaqtnz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hywenlv.cn/gtuanodrhy.html

Ruby: Time.now + 7 * 86400
来源：http://hz.chenjidiqi.icu/gtwtuurwkf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yj20258888.top/gtxwtqtoeg.html

[J06] 计算两时间之差
来源：http://hz.jyoumei.cn/gtmmymsbpw.html

Py:   (end - start).total_seconds()
来源：http://hz.zhaomingkeji.xyz/gtzciumedv.html

PHP:  $end->diff($start)->days;
来源：http://hz.shanyushiyangkeji.top/gtkbkqdzzt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jianghu66.top/gtopwesrwl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.svipenyu.cn/gtiufuugod.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.fengsongda.top/gtswbqbekc.html

Go:   end.Sub(start).Hours()
来源：http://hz.tianlin.xyz/gtxengnjdg.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sxryk.cn/gtqxeibhnc.html

C#:   (end - start).TotalSeconds
来源：http://hz.xuetiantiany.cn/gtzhggrcsw.html

[J07] 比较两个日期
来源：http://hz.nwbrower.top/gtlwfhuolo.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.smart0.xyz/gtdfvipwro.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.wangdashe.top/gtwijxsqnh.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.aibaodan.cn/gtrdmqhgzv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.snrcjt.cn/gtlwdhbojf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hammf.cn/gtauqyedzn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.bjfxy.top/gtysfwpgnr.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ehwqpu.com/gtzakpkhgf.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jiagoushi.top/gtzwmnikqm.html

[J08] 提取年月日与星期
来源：http://hz.yvedp.cn/gtimjqgexb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhijiandao.cn/gtbihdzhnq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhiwuduotai.top/gtwwvfyfxx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.tian-w.cn/gthnhqahor.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.sxryk.cn/gtwathaiin.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xuanzx.com/gtcmjjvohx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xylfe.cn/gtimikrhkc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.daria6918.cn/gtmvrxcfjw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.kuanghao11.cn/gtcbobzddr.html

[J09] 时区处理
来源：http://hz.zycfv.cn/gtgfdskhdb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jlsjyb.cn/gttwzfgvgm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ydjk.org.cn/gtlhlisznc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhongyouzk.top/gtcbmkbrao.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangshuangyany.cn/gtkmvgszdg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gotoacloud.top/gtlzbacvjr.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.kuanghao11.cn/gtvuxgttpj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yangfankeji.com/gtnbdbrxmu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ydzc1.top/gtjuwniiuv.html

[J10] 取今天 / 本月第一天
来源：http://hz.ydzc1.top/gtqrznfeig.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hnqzz.top/gtnnntezfc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xuanzx.com/gtowozondn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhijiandao.cn/gtalwihgxl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.quarkkingdee.top/gtcgpckqhx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zycfv.cn/gtdoubgsmb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.316326.xyz/gtfvsfpljl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cheryme.top/gtbqtxucrf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yuxming.cn/gtkibgflno.html

================================================================================
来源：http://hz.cucudq.cn/gtovdggxet.html

K. JSON 与序列化
来源：http://hz.ppjwa.cn/gtkqerpovg.html

================================================================================
来源：http://hz.meibo888.top/gtncgfdzkk.html

[K01] 对象转 JSON 字符串
来源：http://hz.fengsongda.top/gtnpudgbtv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhixingplan.top/gtvfnapsap.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigufen.top/gtcgiwualy.html

JS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangkeji.top/gtkrpozhto.html

TS:   JSON.stringify(obj)
来源：http://hz.dashuyun.cn/gtlplzlgbb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.guannengcc.top/gtmpybjrqe.html

Go:   json.Marshal(obj)
来源：http://hz.jinyuanbaomall.cn/gtsiehegru.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.redwolf501.top/gtosgwpfny.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yongpay.top/gtieebwndh.html

[K02] JSON 字符串转对象
来源：http://hz.zhengqikj.top/gtkappmhfo.html

Py:   json.loads(s)
来源：http://hz.jinqigufen.top/gtkvaspyjw.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.wangshuangyany.cn/gtyncmfvtb.html

JS:   JSON.parse(s)
来源：http://hz.ywan-chungtsiang.top/gtspepbzpk.html

TS:   JSON.parse(s)
来源：http://hz.zhixingplan.top/gtseoilgkq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.fengsongda.top/gtpkzwifwu.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhongyouzk.top/gthldfwtfa.html

Ruby: JSON.parse(s)
来源：http://hz.jinqigfzy.top/gtntojxkot.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinghuilouyu.cn/gthhtphxfl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ybcxt.top/gttxsgqnmi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ybcxt.top/gtkglynqpp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yvedp.cn/gtojpfxivv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnqzz.top/gtasepuaee.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.iojbl.cn/gtawsdtkov.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.feifeiyinyue.top/gtayarjgvf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yonumen.top/gtppvjflmm.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jqgfzy.top/gthqfagxvd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tanke756.top/gtnjvebulb.html

[K04] 读取 JSON 文件
来源：http://hz.52xcode.cn/gtbgbqhaea.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yueranfly.top/gtvwygtnaj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shzxlz.cn/gtwkizedql.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yvedp.cn/gtmwdwhzmh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ivvv.top/gtartjktii.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhiwuduotai.top/gtiwhylwsh.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sufxvd.cn/gtriqqdgtf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.dashuyun.cn/gtfdnutght.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xuetiantiany.cn/gtreosaokt.html

[K05] 深拷贝对象
来源：http://hz.sysykeji.top/gtafhcbrzj.html

Py:   copy.deepcopy(obj)
来源：http://hz.bjfxy.top/gtraovqiri.html

PHP:  unserialize(serialize($obj));
来源：http://hz.vqdsnc.cn/gtnljpfbdr.html

JS:   structuredClone(obj)
来源：http://hz.yuxming.cn/gtnvflttnd.html

TS:   structuredClone(obj)
来源：http://hz.0kj1m.cn/gtkfbvukvd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.chenjidiqi.icu/gtmuicwcgx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.cqqwz.cn/gtmwqqttzf.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shangyingyoupin.top/gtfuoxhkkr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jiagoushi.top/gtjbcjdfxn.html

[K06] 解析 URL 查询串
来源：http://hz.hfpthk.cn/gtjnrjbxqn.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.wangshuangyany.cn/gtvkefzzzl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhoulong.xyz/gtakgnemur.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.c1oappe.top/gtbggtghgt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zdqjudy.top/gtgsuexctu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xingfuxueyuan.xyz/gtlcszgulx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sysykeji.top/gtjixmzweu.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.birdmap.top/gtetdhbdgt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cqqwz.cn/gtxbxawvkr.html

[K07] 进制转换
来源：http://hz.sysykeji.top/gtyckqtjyp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhoulong.xyz/gtqigkfjep.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.guowangkeji.top/gtlvptdjlx.html


<!-- 参考信息 -->