代发 wailian999

JS:   class MyError extends Error {}
来源：http://hz.yuxming.cn/gtobgufiez.html

TS:   class MyError extends Error {}
来源：http://hz.chenjidiqi.icu/gtwatfuidd.html

Java: class MyException extends RuntimeException {}
来源：http://hz.snrcjt.cn/gtltgtwoeo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.vqdsnc.cn/gtxjizvefz.html

Ruby: class MyError < StandardError; end
来源：http://hz.0kj1m.cn/gtbdmytufj.html

C#:   class MyException : Exception {}
来源：http://hz.pycfn.com/gtttyowmie.html

[H05] 捕获特定类型
来源：http://hz.iojbl.cn/gtowwvbsvx.html

Py:   except ValueError as e:
来源：http://hz.pengpengdd.cyou/gtlormngjh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cashguo.top/gtfdorqtro.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhijiandao.cn/gtagdeyxpf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.kuanghao11.cn/gthmjzaqoc.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jqgufenzy.top/gtadeebclx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gzhubu.top/gtvaiqqcyw.html

Ruby: rescue ArgumentError => e
来源：http://hz.sxryk.cn/gtpxonoffp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.pycfn.com/gtlbhyccys.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xingfuxueyuan.xyz/gtwpmxkxjs.html

Py:   value = d.get("k") or default
来源：http://hz.gotoacloud.top/gtxwovwnbw.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xinyue.icu/gtkzwlegcy.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.pycfn.com/gtewngavjb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.pengpengdd.cyou/gtbhrjotkj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.0kj1m.cn/gtnpivrccy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ydjk.org.cn/gtrgozjdyq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jqgufenzy.top/gtvguzqgay.html

C#:   obj?.A?.B ?? default
来源：http://hz.nanxuanxn.top/gtybuuzxnm.html

[H07] 断言
来源：http://hz.ybcxt.top/gtrmkmhorr.html

Py:   assert x > 0, "必须为正"
来源：http://hz.smart0.xyz/gtcjcxcplr.html

PHP:  assert($x > 0);
来源：http://hz.birdmap.top/gtutilcpof.html

JS:   console.assert(x > 0);
来源：http://hz.jinqigufen.top/gtwudsygbp.html

TS:   console.assert(x > 0);
来源：http://hz.cucudq.cn/gtokivtbgs.html

Java: assert x > 0 : "必须为正";
来源：http://hz.wangdashe.top/gtdqquzklv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xinyue.icu/gtqzbajkyp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.smart0.xyz/gtbubpikgr.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jiagoushi.top/gtejjpcwgy.html

[H08] 获取错误信息与堆栈
来源：http://hz.cheryme.top/gtmslbprrm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yongpay.top/gtojdxwlgd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.c1oappe.top/gtcwukoqnw.html

JS:   e.message;  e.stack
来源：http://hz.jyoumei.cn/gtavnpykqb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cheryme.top/gtmgglmhgb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yangfankeji.com/gtnqsdfrro.html

Go:   err.Error()
来源：http://hz.yuanzhike.top/gthsfijczv.html

Ruby: e.message;  e.backtrace
来源：http://hz.nanxuanxn.top/gtbrfaewja.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jianghu66.top/gtcvbiheis.html

[H09] 带错误码的异常
来源：http://hz.xinyue.icu/gtrauuidyl.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yuanzhike.top/gtezczfmat.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.xingfuxueyuan.xyz/gtittpjleu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hongshengwenyu.top/gtxytwfarv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shuidangran.top/gtwwwekuiz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ivvv.top/gthldkdhym.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.iojbl.cn/gtuwsankcf.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hfpthk.cn/gtbhuoxcmg.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.c1oappe.top/gtkvigbjat.html

[H10] 资源自动释放
来源：http://hz.52xcode.cn/gtbldyjulh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.c1oappe.top/gtkmlxxmxs.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.meibo888.top/gtynfglhmn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.guowangkeji.top/gtmcryukcw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhiwuduotai.top/gterhlpnik.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.nanxuanxn.top/gtgabukmhj.html

Go:   defer f.Close()
来源：http://hz.tian-w.cn/gtgmfnrzrp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.chenzaomai.com/gtweddcgfa.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yueranfly.top/gtdnkwbcua.html

================================================================================
来源：http://hz.aibaodan.cn/gtpafcimwd.html

I. 正则表达式
来源：http://hz.jiagoushi.top/gtjjpyzuao.html

================================================================================
来源：http://hz.fengsongda.top/gtjwjsevks.html

[I01] 判断是否匹配
来源：http://hz.mhx1999.top/gtzrmicdom.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.chenlongwang.top/gtviyqkxeh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gotoacloud.top/gtbwbqfuiu.html

JS:   /\d+/.test(s)
来源：http://hz.jianghu66.top/gtbdbyufxu.html

TS:   /\d+/.test(s)
来源：http://hz.iojbl.cn/gtqufmkxhf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xziqi.cn/gtuurwhsnh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ivvv.top/gtqiuuwvkd.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhengqikj.top/gtfipuoovs.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.snrcjt.cn/gtuiuziszz.html

[I02] 提取所有匹配
来源：http://hz.zhongyouzk.top/gtkisuehoq.html

Py:   re.findall(r"\d+", s)
来源：http://hz.sufxvd.cn/gtlmypzvwr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.nwbrower.top/gtwysofbjb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj20258.top/gtjfhwfagf.html

TS:   s.match(/\d+/g)
来源：http://hz.ehwqpu.com/gtnfsnhdxh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhengqikj.top/gtvjbxcwpc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yanxiufei.cn/gtaermjiwq.html

Ruby: s.scan(/\d+/)
来源：http://hz.yj202588.top/gtsdbpdkwp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.guowangkeji.top/gtoqbxvixq.html

[I03] 提取捕获分组
来源：http://hz.yuanzhike.top/gtnqusaioz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ydzc1.top/gtjhcffpia.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.aizwys.cn/gtqgnbthpg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jqgfzy.top/gtzuwjawlt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.dashuyun.cn/gtfwiqpsun.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.fzhhl.top/gtrrbdrhss.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zdqjudy.top/gtguzgnwid.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ivvv.top/gtxqhzctob.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cqqwz.cn/gtjwhxekui.html

[I04] 正则替换
来源：http://hz.jinyuanbaomall.cn/gtmngskwpw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.nanxinkj.top/gtjhfufysj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cqqwz.cn/gtuwnzlmyw.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.meibo888.top/gturlrrzzi.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.52xcode.cn/gtsrcizboc.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yangfankeji.com/gtmymctyie.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yj202588.top/gtdgumjctk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yj20258.top/gtwodmfzeh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yvedp.cn/gtbycoezbt.html

[I05] 按正则拆分
来源：http://hz.gotoacloud.top/gtwcpjuwdc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hammf.cn/gtiscznigz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yj20258888.top/gtykxbxzms.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.fengsongda.top/gtjekxhibx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhaomingkeji.xyz/gtptpdaolm.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xingfuxueyuan.xyz/gtfzkpgwoe.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.guannengcc.top/gtuectkaxd.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gtkfjwxtiy.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xingfuxueyuan.xyz/gtcfwkcttf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yuanzhike.top/gthaeqrfcw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.nwbrower.top/gtdauhaizo.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.feifeiyinyue.top/gtvhqmhklh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hfpthk.cn/gtmaifxplw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hammf.cn/gtmnckhrxb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhiwuduotai.top/gtzefsttsm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sysykeji.top/gthszybehh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.daria6918.cn/gtqmdjlfpz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.meibo888.top/gtrmurgpxs.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhoulong.xyz/gtpttdewsx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xingfuxueyuan.xyz/gtjaenjpio.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ehwqpu.com/gtqxfgsimo.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hywenlv.cn/gtrfryohym.html

TS:   /error/gim
来源：http://hz.9152youxi.cn/gtdpmeutxm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.redwolf501.top/gtbxpndjgt.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.sweek.top/gtiinnzmyc.html

Ruby: s.scan(/error/i)
来源：http://hz.meibo888.top/gtyjanmjkx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hywenlv.cn/gtfmpkpyxb.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xuetiantiany.cn/gtlkayrbyn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.316326.xyz/gthddipsmq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhongyouzk.top/gtoabxqcuz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj20258.top/gtndmbygal.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.52xcode.cn/gtiyoppmdl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.gaohongyu789.top/gtpukambai.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.aibaodan.cn/gtgfgrljqa.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhijiandao.cn/gttkkozumt.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shanyushiyangkeji.top/gtuduxsqna.html

================================================================================
来源：http://hz.316326.xyz/gttxzhwwwt.html

J. 日期与时间
来源：http://hz.hnxiangtu.top/gtxgyuwyly.html

================================================================================
来源：http://hz.cashguo.top/gtabjontfe.html

[J01] 获取当前时间
来源：http://hz.jinqigufen.top/gtroyousan.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shanyushiyangkeji.top/gthvwbrqzk.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.guowangkeji.top/gtvzyatnsy.html

JS:   new Date();  Date.now()
来源：http://hz.xziqi.cn/gtvwsyiwfh.html

TS:   new Date();  Date.now()
来源：http://hz.sweek.top/gtwrxgzpdn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.guannengcc.top/gtkafpmeom.html

Go:   time.Now()
来源：http://hz.jinqigfzy.top/gtwzdfecvz.html

Ruby: Time.now
来源：http://hz.52xcode.cn/gtoyftfhku.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shanyushiyangkeji.top/gtaptbpthi.html

[J02] 格式化输出
来源：http://hz.daxiang520.top/gtvvwvxjdz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangshuangyany.cn/gtwoovvxok.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.9152youxi.cn/gtdmqcnsok.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gaohongyu789.top/gtqgnserwr.html

TS:   d.toISOString()
来源：http://hz.c1oappe.top/gtoxvuskak.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sxryk.cn/gtofeevecw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xuanzx.com/gtqebyimcv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhengqikj.top/gtzsuhrxxk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hammf.cn/gtibjygaiw.html

[J03] 字符串解析为日期
来源：http://hz.gzhubu.top/gtpqqojztm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.mhx1999.top/gtswetrtbd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xuanzx.com/gtxdfggnuq.html

JS:   new Date("2024-01-02")
来源：http://hz.tian-w.cn/gtsinnarkb.html

TS:   new Date("2024-01-02")
来源：http://hz.52xcode.cn/gtdpnfjbdv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.0kj1m.cn/gtwsnfnqfz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.smart0.xyz/gtwnjkmhfi.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gaohongyu789.top/gtxijbikfp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sweek.top/gtklyfqdjd.html

[J04] 时间戳与日期互转
来源：http://hz.mhx1999.top/gttrvntylo.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xingfuxueyuan.xyz/gtpomlaptl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.316326.xyz/gtmxfachfb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.nwbrower.top/gtrcbojqof.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sxryk.cn/gtwvvnwzxq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinqigufen.top/gtomsozeij.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.vqdsnc.cn/gtciskumis.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shuidangran.top/gtklzfrszs.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinqigfzy.top/gtfenmwylm.html

[J05] 时间加减（加 7 天）
来源：http://hz.wangshuangyany.cn/gtxbmrurys.html

Py:   now + timedelta(days=7)
来源：http://hz.cucudq.cn/gterrotoqm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.aibaodan.cn/gteryojuwv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenjidiqi.icu/gtxmbneair.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuanzx.com/gtbjwyzytp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.daria6918.cn/gtcmfwzoer.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hysaishi.cn/gtmclaxvge.html

Ruby: Time.now + 7 * 86400
来源：http://hz.snrcjt.cn/gtxhozcpxc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhoulong.xyz/gtyaslxyuq.html

[J06] 计算两时间之差
来源：http://hz.xinyue.icu/gttfmxvzzc.html

Py:   (end - start).total_seconds()
来源：http://hz.zhijiandao.cn/gtmtjkbfle.html

PHP:  $end->diff($start)->days;
来源：http://hz.haohaochexian.top/gtcfpwpevi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.yj20258888.top/gthrwdnert.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhixingplan.top/gtkvrzgdld.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shuidangran.top/gtzkwrlxsa.html

Go:   end.Sub(start).Hours()
来源：http://hz.yj202588.top/gtalwsknds.html

Ruby: end - start                 # 返回秒数
来源：http://hz.9152youxi.cn/gttgzmvvep.html

C#:   (end - start).TotalSeconds
来源：http://hz.jinqigfzy.top/gtehnfrhzy.html

[J07] 比较两个日期
来源：http://hz.yuxming.cn/gtgfphqgil.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gogol.net.cn/gtchvvrodt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhixingplan.top/gtvebbrsaz.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.aibaodan.cn/gtojqmcqbb.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shuidangran.top/gtxadbueix.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.andypj.xyz/gtsnujzwdt.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sufxvd.cn/gtuexcrwns.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hongshengwenyu.top/gtjtsihzob.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.daxiang520.top/gtbyeviayn.html

[J08] 提取年月日与星期
来源：http://hz.yj202588.top/gtiwbacxep.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.havefunace.top/gtrfamlvkr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.c1oappe.top/gtumoapzpw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.gzhubu.top/gtrezpwubw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.daria6918.cn/gtzgnhipza.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yongpay.top/gtcyfkpmlk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yj20258.top/gtqloppabv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.fzhhl.top/gtmmsmzrxr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yvedp.cn/gtsrrcqgyx.html

[J09] 时区处理
来源：http://hz.sxryk.cn/gttuaqkams.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.fengsongda.top/gtoujeupgw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ybcxt.top/gtkddjtnxl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shangyingyoupin.top/gtovfnxhcy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.iojbl.cn/gtszgosqsd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yj20258888.top/gtveutdkrs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shanyushiyangtech.top/gtswpzkbla.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.meibo888.top/gtopthwaic.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xuetiantiany.cn/gtibivscwc.html

[J10] 取今天 / 本月第一天
来源：http://hz.nanxinkj.top/gteahrxxqw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhongyouzk.top/gtdvqainks.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jlsjyb.cn/gtpljhimck.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gogol.net.cn/gtjbiwrsen.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yanxiufei.cn/gtahlojvpx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yuxming.cn/gtqweewjrr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.tanke756.top/gtiwtbkuup.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ybcxt.top/gtltwlblei.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yvedp.cn/gtwwdrtxrm.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtyieqkrjd.html

K. JSON 与序列化
来源：http://hz.zhiwuduotai.top/gtgwcdeasp.html

================================================================================
来源：http://hz.vqdsnc.cn/gtcekfubld.html

[K01] 对象转 JSON 字符串
来源：http://hz.shzxlz.cn/gtzahymbvp.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ydzc1.top/gttdcsxqsq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.c1oappe.top/gtqcpuzgfr.html

JS:   JSON.stringify(obj)
来源：http://hz.gotoacloud.top/gtabvxhxew.html

TS:   JSON.stringify(obj)
来源：http://hz.hfpthk.cn/gtwolxmuzb.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.pycfn.com/gtejuphkpy.html

Go:   json.Marshal(obj)
来源：http://hz.yongpay.top/gtmrfccwhm.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cucudq.cn/gtcleomkrp.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jqgfzy.top/gtcwnlxidu.html

[K02] JSON 字符串转对象
来源：http://hz.shzxlz.cn/gthgequawd.html

Py:   json.loads(s)
来源：http://hz.hongshengwenyu.top/gtmzjzsnot.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.aibaodan.cn/gttlmbwoqo.html

JS:   JSON.parse(s)
来源：http://hz.zhoulong.xyz/gtxsqnzsnp.html

TS:   JSON.parse(s)
来源：http://hz.yangfankeji.com/gtuanageby.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sxryk.cn/gtdsqtwzlg.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yanxiufei.cn/gtxpgpfpme.html

Ruby: JSON.parse(s)
来源：http://hz.hysaishi.cn/gtwxbkxvyl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.0kj1m.cn/gtiugldovl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.nanxuanxn.top/gtuehrpgwr.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.c1oappe.top/gtmbyuhxgf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shzxlz.cn/gthfffylzq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.52xcode.cn/gtxexzzrym.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangtech.top/gtrgizdyoa.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.haohaochexian.top/gtmpnrqawn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ybcxt.top/gtxkgykfai.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jinqigfzy.top/gtwyduzroa.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.9152youxi.cn/gtysdzdaow.html

[K04] 读取 JSON 文件
来源：http://hz.shuidangran.top/gteimpecfi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.fzhhl.top/gtjrplebid.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhijiandao.cn/gtnxuzgehh.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenzaomai.com/gtrqkotkwx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yangfankeji.com/gtfrgbslvy.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinqigfzy.top/gtivvdqsjy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jinghuilouyu.cn/gtzmvdqmqc.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.nanxinkj.top/gtclvtgehl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.bjfxy.top/gtdmxnjzcw.html

[K05] 深拷贝对象
来源：http://hz.yj202588.top/gtkqfgszwj.html

Py:   copy.deepcopy(obj)
来源：http://hz.gaohongyu789.top/gtgpcxhejk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hysaishi.cn/gtedbwecjy.html

JS:   structuredClone(obj)
来源：http://hz.zhijiandao.cn/gtuqaqyltu.html

TS:   structuredClone(obj)
来源：http://hz.zhijiandao.cn/gtdytuagcl.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xingfuxueyuan.xyz/gtgghojwlw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinqigfzy.top/gtkkfnmjqj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shanyushiyangkeji.top/gtxzznowho.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.havefunace.top/gtpmvryqqm.html

[K06] 解析 URL 查询串
来源：http://hz.ybcxt.top/gtqhxgqkwb.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.smart0.xyz/gthazjcgol.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhoulong.xyz/gtayyzzhrw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hammf.cn/gtvrtbifud.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.iojbl.cn/gtgfhpimrp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xingfuxueyuan.xyz/gtygulghte.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.52xcode.cn/gtyrgqieec.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gogol.net.cn/gtboprlked.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.cheryme.top/gthzswecbt.html

[K07] 进制转换
来源：http://hz.pengpengdd.cyou/gtqrwhuxbw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.c1oappe.top/gtajzjnliw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.aibaodan.cn/gtzfruwded.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yueranfly.top/gtcrvoqfze.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ydzc1.top/gtnxohgqmw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.wangshuangyany.cn/gtpecqgtxz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.sufxvd.cn/gtbminjpyu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ppjwa.cn/gtqtvqlkij.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhongyouzk.top/gtjajxuzqe.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.gotoacloud.top/gtiscpkmwq.html

Py:   pickle.dumps(obj)
来源：http://hz.redwolf501.top/gtndsnkqdl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.hnxiangtu.top/gterxixbuo.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.sweek.top/gtidhtfcxz.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cdnleiting.top/gtlaeewmvt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.nwbrower.top/gtbofytkjd.html


<!-- 参考信息 -->