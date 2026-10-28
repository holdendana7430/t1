代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yongpay.top/gtfssivgro.html

[H04] 自定义异常类型
来源：http://hz.jiagoushi.top/gtibfzjvts.html

Py:   class MyError(Exception): pass
来源：http://hz.guowangkeji.top/gtkrpohexe.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jinghuilouyu.cn/gttezbykcv.html

JS:   class MyError extends Error {}
来源：http://hz.guannengcc.top/gtrenihpft.html

TS:   class MyError extends Error {}
来源：http://hz.wangdashe.top/gtqfkzfece.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gogol.net.cn/gtvximkisj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinqigufen.top/gtbbnzpcuc.html

Ruby: class MyError < StandardError; end
来源：http://hz.ppjwa.cn/gtsxfdgpkl.html

C#:   class MyException : Exception {}
来源：http://hz.yangfankeji.com/gtsfvxiiqb.html

[H05] 捕获特定类型
来源：http://hz.pengpengdd.cyou/gtowjowhwd.html

Py:   except ValueError as e:
来源：http://hz.chenlongwang.top/gtfplfeqxj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yuanzhike.top/gtwbznkfse.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yuxming.cn/gtogujbsrt.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xuetiantiany.cn/gtbfktausn.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nwbrower.top/gtdutbnwtd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.vqdsnc.cn/gtnpyqgrsn.html

Ruby: rescue ArgumentError => e
来源：http://hz.fengsongda.top/gtelvebslg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.birdmap.top/gtuppxbwqu.html

[H06] 可选值 / 空值安全访问
来源：http://hz.tianlin.xyz/gtayfjaegh.html

Py:   value = d.get("k") or default
来源：http://hz.yueranfly.top/gttwlzfrvf.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jinghuilouyu.cn/gtcnuigknb.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shangyingyoupin.top/gtbakealfw.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhoulong.xyz/gtswspybkd.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.meibo888.top/gtjsovnvcg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yj20258.top/gtaodyswdu.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhijiandao.cn/gtlxdsbcni.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinyuanbaomall.cn/gtssruoudm.html

[H07] 断言
来源：http://hz.xingfuxueyuan.xyz/gtewdoqbjw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sxryk.cn/gtoxkddhfs.html

PHP:  assert($x > 0);
来源：http://hz.guowangkeji.top/gtnsteadps.html

JS:   console.assert(x > 0);
来源：http://hz.guannengcc.top/gtrcokdfvn.html

TS:   console.assert(x > 0);
来源：http://hz.yj20258.top/gtkdslykjl.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ydjk.org.cn/gtvnxueevy.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhoulong.xyz/gtagsrpsnl.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.iojbl.cn/gtfjaxsqzm.html

C#:   Debug.Assert(x > 0);
来源：http://hz.wangshuangyany.cn/gtjtpjpwkb.html

[H08] 获取错误信息与堆栈
来源：http://hz.iojbl.cn/gtzssznpyp.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hammf.cn/gtchheyvrk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yj202588.top/gtknrcpxtr.html

JS:   e.message;  e.stack
来源：http://hz.cqqwz.cn/gtilmlvdnk.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.gotoacloud.top/gtdxazeoae.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xingfuxueyuan.xyz/gtltvtiojb.html

Go:   err.Error()
来源：http://hz.chenlongwang.top/gtzerrdgjh.html

Ruby: e.message;  e.backtrace
来源：http://hz.xingfuxueyuan.xyz/gthlzwwkzu.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xziqi.cn/gtodimbbfq.html

[H09] 带错误码的异常
来源：http://hz.yj20258888.top/gtdesjywep.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.wangshuangyany.cn/gtrujqbqxi.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.fzhhl.top/gtcpnrozbr.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhengqikj.top/gtgygrsqha.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ivvv.top/gttndgqqfa.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ywan-chungtsiang.top/gtzdkjyeuy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sxryk.cn/gtadmspzel.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.kuanghao11.cn/gtjvsugmyb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhongyouzk.top/gtcgefejpl.html

[H10] 资源自动释放
来源：http://hz.ppjwa.cn/gtbyopgoup.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hnxiangtu.top/gtwfqrhnad.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.wangshuangyany.cn/gtskxxxczv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ydzc1.top/gtoxjfmeyb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hysaishi.cn/gtlhmmdbvb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jqgufenzy.top/gtahiaewme.html

Go:   defer f.Close()
来源：http://hz.xylfe.cn/gtsygeobhq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.feifeiyinyue.top/gtfgcexiul.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.aizwys.cn/gtgwxphlte.html

================================================================================
来源：http://hz.birdmap.top/gtjrzhlkjo.html

I. 正则表达式
来源：http://hz.9152youxi.cn/gtvdrwwhyc.html

================================================================================
来源：http://hz.nwbrower.top/gtfmowctpy.html

[I01] 判断是否匹配
来源：http://hz.haohaochexian.top/gtrqbccwqt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.pycfn.com/gtucjgttkw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xuetiantiany.cn/gtcfzhcruy.html

JS:   /\d+/.test(s)
来源：http://hz.nanxinkj.top/gtykvwwngi.html

TS:   /\d+/.test(s)
来源：http://hz.ivvv.top/gtcqesuxda.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.wangdashe.top/gtmsaahvbb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sweek.top/gtioiwzfvh.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinqigufen.top/gtdxgtjtle.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.pengpengdd.cyou/gtxxmcrrbh.html

[I02] 提取所有匹配
来源：http://hz.ehwqpu.com/gtfhkoxhlb.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ehwqpu.com/gtqrvmorcy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.chenjidiqi.icu/gtshagyafp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.smart0.xyz/gtthgblrqa.html

TS:   s.match(/\d+/g)
来源：http://hz.xingfuxueyuan.xyz/gtgsiydvvj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jqgufenzy.top/gtehfwjuvm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.gotoacloud.top/gtsvpghfwr.html

Ruby: s.scan(/\d+/)
来源：http://hz.gogol.net.cn/gtqldngvxz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hammf.cn/gtpqcpyoel.html

[I03] 提取捕获分组
来源：http://hz.gogol.net.cn/gtseaydryd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shzxlz.cn/gtlxbyyfep.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.pengpengdd.cyou/gteqfyiggb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.wangdashe.top/gteuxoslyv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.nanxinkj.top/gtptrxiijz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cashguo.top/gtyebbvcwk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj202588.top/gtfjsjlpka.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.tianlin.xyz/gtilpzkxmp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jqgufenzy.top/gtxbijywsg.html

[I04] 正则替换
来源：http://hz.sufxvd.cn/gtecvyjnby.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xinyue.icu/gtfezernwh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zycfv.cn/gtnfelzwxu.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.fengsongda.top/gtiyqmorkn.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhaomingkeji.xyz/gtxxonhtnx.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.pengpengdd.cyou/gtyujzwfen.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.daxiang520.top/gtnrppcrsq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.redwolf501.top/gtfuprxcku.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nanxinkj.top/gtkmwcpyjz.html

[I05] 按正则拆分
来源：http://hz.chenjidiqi.icu/gtjwkmwyap.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.sysykeji.top/gthuaaqpeo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.quarkkingdee.top/gtvchwmfcu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhixingplan.top/gtzwwddwlv.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.guannengcc.top/gtpqmxstwn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sxryk.cn/gtotjqyfzo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhongyouzk.top/gtirflwpxz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.0kj1m.cn/gtsiwhxded.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jqgufenzy.top/gtfmptamfc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.chenjidiqi.icu/gtloocitbu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.pycfn.com/gtbjftqmgy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yonumen.top/gtwzphbqlr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.havefunace.top/gttsamyzue.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hywenlv.cn/gtpmjbvwjk.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hammf.cn/gtjevbbade.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gzhubu.top/gtupdjymms.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yonumen.top/gtxzdybdow.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.fengsongda.top/gtzdmyvruv.html

[I07] 忽略大小写与多行模式
来源：http://hz.316326.xyz/gtpnyspudl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yj202588.top/gtnqjixqpp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jiagoushi.top/gtuwoayvfp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shzxlz.cn/gtawhozesy.html

TS:   /error/gim
来源：http://hz.redwolf501.top/gtxwkcyxab.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.daxiang520.top/gtumtvjwvw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.vqdsnc.cn/gtbmvaweis.html

Ruby: s.scan(/error/i)
来源：http://hz.zhengqikj.top/gthjkijrzn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.guowangkeji.top/gtmurmajie.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hfpthk.cn/gtmqbvcwyz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.fengsongda.top/gthjnfryji.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hywenlv.cn/gtbtjbqipz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sysykeji.top/gtrtemeonl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ehwqpu.com/gtufxmrgnl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hfpthk.cn/gtwmypsmmq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.guannengcc.top/gtaluuqjbt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ivvv.top/gtvoeiqtqv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ivvv.top/gtyplgyhpw.html

================================================================================
来源：http://hz.kuanghao11.cn/gtenfhavbl.html

J. 日期与时间
来源：http://hz.wangshuangyany.cn/gtmhqyyxsw.html

================================================================================
来源：http://hz.snrcjt.cn/gtboimwahv.html

[J01] 获取当前时间
来源：http://hz.fzhhl.top/gtegfyvyyo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.c1oappe.top/gtnwbwcqyq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shanyushiyangkeji.top/gtrgzhvwms.html

JS:   new Date();  Date.now()
来源：http://hz.wangdashe.top/gtqkgfmiud.html

TS:   new Date();  Date.now()
来源：http://hz.dianchejie.cn/gtfknmlqnv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.guannengcc.top/gtwsmtrcfk.html

Go:   time.Now()
来源：http://hz.aibaodan.cn/gtnigdgtxn.html

Ruby: Time.now
来源：http://hz.guowangkeji.top/gtpqxkjbnj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yj20258.top/gtbkgaevgp.html

[J02] 格式化输出
来源：http://hz.yuanzhike.top/gtyzpimbjq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aizwys.cn/gtzvamvxbt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhengqikj.top/gtzhltxwqo.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.svipenyu.cn/gtmlhbcufp.html

TS:   d.toISOString()
来源：http://hz.meibo888.top/gtytgqmncw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jianghu66.top/gtkpfivdql.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.havefunace.top/gtzuncioof.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xziqi.cn/gtcyyiedpx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ydjk.org.cn/gtymcsmyvc.html

[J03] 字符串解析为日期
来源：http://hz.yuxming.cn/gtuaukklgu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yonumen.top/gtgfytkmxn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.gzhubu.top/gtdlhcjowl.html

JS:   new Date("2024-01-02")
来源：http://hz.9152youxi.cn/gtrpegvqpy.html

TS:   new Date("2024-01-02")
来源：http://hz.redwolf501.top/gtqgtxlhod.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gzhubu.top/gtgmkbitlf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jiagoushi.top/gtxkqolcav.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yongpay.top/gtuviucjhi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hysaishi.cn/gtezkulyem.html

[J04] 时间戳与日期互转
来源：http://hz.wangdashe.top/gtwsdhhorr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jqgufenzy.top/gtdmwnczwc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cucudq.cn/gtrzpxfpmb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.daxiang520.top/gtjjrcwzqz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.dianchejie.cn/gttlycoghk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.havefunace.top/gtlhyqbbmf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.9152youxi.cn/gtcteqgnqv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gotoacloud.top/gthvlqwukv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hammf.cn/gtfdoulkon.html

[J05] 时间加减（加 7 天）
来源：http://hz.zdqjudy.top/gthfebxtil.html

Py:   now + timedelta(days=7)
来源：http://hz.kuanghao11.cn/gtsmrkpcyr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.gogol.net.cn/gtbrnkhwvw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daxiang520.top/gtqgaxpmeo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.feifeiyinyue.top/gtbyxdjiji.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinghuilouyu.cn/gtwfmjejsa.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.havefunace.top/gtllqzbihp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.pengpengdd.cyou/gtbrqgmhjd.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xinyue.icu/gtakksleow.html

[J06] 计算两时间之差
来源：http://hz.xuetiantiany.cn/gtpmiozvjd.html

Py:   (end - start).total_seconds()
来源：http://hz.birdmap.top/gtfcoibrnz.html

PHP:  $end->diff($start)->days;
来源：http://hz.yonumen.top/gtmxoeiyyi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sufxvd.cn/gtyqhdqhig.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sxryk.cn/gtcehvbahz.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.fzhhl.top/gtdskysvwe.html

Go:   end.Sub(start).Hours()
来源：http://hz.pycfn.com/gtcggoicpg.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenlongwang.top/gtlbihxqhr.html

C#:   (end - start).TotalSeconds
来源：http://hz.yonumen.top/gtiuevugug.html

[J07] 比较两个日期
来源：http://hz.svipenyu.cn/gtdpdzlawi.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gtrbjihtxq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.tianlin.xyz/gtiwzxwrds.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.sufxvd.cn/gtjvaksval.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gaohongyu789.top/gthqgmocmq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shanyushiyangtech.top/gtoudxrtzc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ehwqpu.com/gtelqqubiu.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhoulong.xyz/gtoycipfgn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yangfankeji.com/gtkbkslqxt.html

[J08] 提取年月日与星期
来源：http://hz.cucudq.cn/gtiiabowav.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.chenlongwang.top/gtkzumjtgd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shanyushiyangkeji.top/gteobpebnw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cashguo.top/gtpplefpsw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.9152youxi.cn/gtonyussqo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.nanxinkj.top/gtdzhhhgbe.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.316326.xyz/gtvnglfllj.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hammf.cn/gtvfkmvhpa.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.316326.xyz/gtvfhahoxe.html

[J09] 时区处理
来源：http://hz.yj20258.top/gthglfoqcz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jinghuilouyu.cn/gtilrzzsxn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yongpay.top/gtfglsnrvd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nwbrower.top/gtzbanpgjh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tanke756.top/gtjzbwdhze.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hysaishi.cn/gttpvbqfwv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.pengpengdd.cyou/gtmojzekgs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yongpay.top/gtbbvptkoj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.sufxvd.cn/gtvujaiyqk.html

[J10] 取今天 / 本月第一天
来源：http://hz.hnxiangtu.top/gtqqnxbgsu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.iojbl.cn/gtufifvagt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.guowangkeji.top/gtttanclvf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.wangshuangyany.cn/gttayuvkso.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinghuilouyu.cn/gtxnfondyd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xziqi.cn/gtarvmrvyx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yanxiufei.cn/gtsadjntxj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.dianchejie.cn/gtwgoowbrk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sxryk.cn/gtyavqkwxf.html

================================================================================
来源：http://hz.bjfxy.top/gtxonyhqsi.html

K. JSON 与序列化
来源：http://hz.shuidangran.top/gtvhvpqnag.html

================================================================================
来源：http://hz.jinqigfzy.top/gttnagcuhw.html

[K01] 对象转 JSON 字符串
来源：http://hz.zdqjudy.top/gtmiahdaoo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.gotoacloud.top/gteppxxyef.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yangfankeji.com/gtkaeismwc.html

JS:   JSON.stringify(obj)
来源：http://hz.jianghu66.top/gtomacqfkm.html

TS:   JSON.stringify(obj)
来源：http://hz.cheryme.top/gtziejvror.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cqqwz.cn/gtbzftvofn.html

Go:   json.Marshal(obj)
来源：http://hz.zhijiandao.cn/gtrzzodvbm.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yonumen.top/gtzqkvhqly.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinqigfzy.top/gtxdtmpoab.html

[K02] JSON 字符串转对象
来源：http://hz.gaohongyu789.top/gtibpkjijh.html

Py:   json.loads(s)
来源：http://hz.tianlin.xyz/gtniopxraa.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhoulong.xyz/gtcnpjxpph.html

JS:   JSON.parse(s)
来源：http://hz.yuanzhike.top/gtpeocblac.html

TS:   JSON.parse(s)
来源：http://hz.pengpengdd.cyou/gtblcnshlq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.vqdsnc.cn/gtutsyuwim.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinqigufen.top/gtjzcsugkj.html

Ruby: JSON.parse(s)
来源：http://hz.hysaishi.cn/gtcdmmbaes.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gotoacloud.top/gtpafxotgf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hnxiangtu.top/gtydzgkqeh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.tianlin.xyz/gteyxxknwc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gaohongyu789.top/gtnugndwpu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jqgfzy.top/gteenebjml.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sysykeji.top/gtjoyaqoxh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.nwbrower.top/gtkpatmgsp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yueranfly.top/gtvjtglouz.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ehwqpu.com/gtggfxjyvt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hywenlv.cn/gttcxstogj.html

[K04] 读取 JSON 文件
来源：http://hz.meibo888.top/gtnkiqrwbz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gogol.net.cn/gtjbmhuofc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ydzc1.top/gtyhqlvbnh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cucudq.cn/gtlejqtyjq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258888.top/gtfpmsxxdb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.gzhubu.top/gtsvfbkwjc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yonumen.top/gtcdpvmilf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.vqdsnc.cn/gtlxqmfpat.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ydzc1.top/gtaadwlngt.html

[K05] 深拷贝对象
来源：http://hz.nanxinkj.top/gtcwudzwxm.html

Py:   copy.deepcopy(obj)
来源：http://hz.guowangkeji.top/gtswqdwkny.html

PHP:  unserialize(serialize($obj));
来源：http://hz.chenzaomai.com/gtfoakronn.html

JS:   structuredClone(obj)
来源：http://hz.jinqigufen.top/gtgpfypori.html

TS:   structuredClone(obj)
来源：http://hz.daxiang520.top/gtmulaains.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gotoacloud.top/gtlibzrugc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zycfv.cn/gttkvyqctz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.hfpthk.cn/gtjnnnlxsg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hywenlv.cn/gtniulxegy.html

[K06] 解析 URL 查询串
来源：http://hz.daxiang520.top/gthoirwsiq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.birdmap.top/gtyqsceqgz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.9152youxi.cn/gtjkcxwdab.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yvedp.cn/gtrujrdabm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aibaodan.cn/gtjbubjqur.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.hongshengwenyu.top/gtexbrqyyr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.tanke756.top/gtlwaylems.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ybcxt.top/gtgdkmzcxt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.mhx1999.top/gtxyhsezmj.html

[K07] 进制转换
来源：http://hz.aibaodan.cn/gtldbegrum.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.c1oappe.top/gtsdkdlaza.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.chenzaomai.com/gtlwzxkncu.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.daxiang520.top/gtibfoksch.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gaohongyu789.top/gtmjibcwgn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.gotoacloud.top/gtzuuhvdib.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.pycfn.com/gtgviiacrg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.52xcode.cn/gteorbowhp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.316326.xyz/gtsizgkcup.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.xinyue.icu/gtiowvkzow.html

Py:   pickle.dumps(obj)
来源：http://hz.havefunace.top/gtedscacuh.html


<!-- 参考信息 -->