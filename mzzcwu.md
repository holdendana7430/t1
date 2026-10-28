代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://hz.fengsongda.top/gtioqabjxz.html

C#:   class MyException : Exception {}
来源：http://hz.zhoulong.xyz/gtfisyhtgt.html

[H05] 捕获特定类型
来源：http://hz.zdqjudy.top/gtuxrgbpcx.html

Py:   except ValueError as e:
来源：http://hz.mhx1999.top/gtqaoedqzj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinqigufen.top/gtextzkuex.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.daxiang520.top/gtwfbijbyn.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jqgfzy.top/gtkwixswtl.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.redwolf501.top/gtchwqgkrx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhengqikj.top/gtujrennjo.html

Ruby: rescue ArgumentError => e
来源：http://hz.nwbrower.top/gtymxssijl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.meibo888.top/gtntuxzhru.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jinqigfzy.top/gtlxcdcgsk.html

Py:   value = d.get("k") or default
来源：http://hz.316326.xyz/gtgvbpkzvs.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ehwqpu.com/gtkohrezkr.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yonumen.top/gttnsaxkcc.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinqigfzy.top/gtzrmfipgc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.chenjidiqi.icu/gtkjxcfbhc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yanxiufei.cn/gtiyrcucgo.html

Ruby: d&.dig(:a, :b)
来源：http://hz.nwbrower.top/gtjrsgzbwo.html

C#:   obj?.A?.B ?? default
来源：http://hz.nanxuanxn.top/gtmkcftoae.html

[H07] 断言
来源：http://hz.yueranfly.top/gtewstkxwv.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jiagoushi.top/gtqdwlqrjk.html

PHP:  assert($x > 0);
来源：http://hz.xingfuxueyuan.xyz/gtcqnvyyiy.html

JS:   console.assert(x > 0);
来源：http://hz.bjfxy.top/gtdcpcgays.html

TS:   console.assert(x > 0);
来源：http://hz.dashuyun.cn/gtepyvsfyd.html

Java: assert x > 0 : "必须为正";
来源：http://hz.pycfn.com/gtsqxqyuvi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.316326.xyz/gtcukwjhkb.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.nanxinkj.top/gtaddyzhpo.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhaomingkeji.xyz/gtkwafxjcr.html

[H08] 获取错误信息与堆栈
来源：http://hz.gogol.net.cn/gtwkyzapnx.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.nwbrower.top/gtxsktywpy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hfpthk.cn/gtrnwigupv.html

JS:   e.message;  e.stack
来源：http://hz.haohaochexian.top/gttnzotjsh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shanyushiyangkeji.top/gtfidorlxn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.havefunace.top/gtsiokmcrr.html

Go:   err.Error()
来源：http://hz.cqqwz.cn/gtaxquepie.html

Ruby: e.message;  e.backtrace
来源：http://hz.shangyingyoupin.top/gtdsmzrnft.html

C#:   e.Message;  e.StackTrace
来源：http://hz.316326.xyz/gtcwbmzffh.html

[H09] 带错误码的异常
来源：http://hz.dianchejie.cn/gtxgggwpyw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.gaohongyu789.top/gthhpadecq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.tanke756.top/gtefnbdski.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhiwuduotai.top/gthejhwsnb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhaomingkeji.xyz/gtukwfnzjz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinqigufen.top/gtvpswkgis.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhijiandao.cn/gtjdzgrvpg.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.tanke756.top/gtmyvcmyuj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhijiandao.cn/gtdzyjxjfs.html

[H10] 资源自动释放
来源：http://hz.nwbrower.top/gtmvprfrhk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.sufxvd.cn/gtvhlntevw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jiagoushi.top/gtscsazsyt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.9152youxi.cn/gtsoqahzoc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.0kj1m.cn/gthukpdqdo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.pycfn.com/gtrpggmewt.html

Go:   defer f.Close()
来源：http://hz.vqdsnc.cn/gthvehravb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.dianchejie.cn/gtpontyqav.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.pycfn.com/gtbjxycgvw.html

================================================================================
来源：http://hz.9152youxi.cn/gtrtwnvmgf.html

I. 正则表达式
来源：http://hz.9152youxi.cn/gtjjcfdncr.html

================================================================================
来源：http://hz.gotoacloud.top/gtlxsknypb.html

[I01] 判断是否匹配
来源：http://hz.gogol.net.cn/gtdfsvrlgd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zycfv.cn/gtxgrwcixi.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yonumen.top/gtutrukwqw.html

JS:   /\d+/.test(s)
来源：http://hz.ivvv.top/gtofjruluv.html

TS:   /\d+/.test(s)
来源：http://hz.dashuyun.cn/gtvjjavyul.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zdqjudy.top/gtrwjpldfh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ywan-chungtsiang.top/gtbhvflsxr.html

Ruby: s.match?(/\d+/)
来源：http://hz.jlsjyb.cn/gtmzudeujf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinqigufen.top/gtygpwohwo.html

[I02] 提取所有匹配
来源：http://hz.shangyingyoupin.top/gteqhynrbc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ehwqpu.com/gthtvexawz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yvedp.cn/gtzfltstzo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hysaishi.cn/gtgvyvcfza.html

TS:   s.match(/\d+/g)
来源：http://hz.ppjwa.cn/gtjfuvenuk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.bjfxy.top/gtzfxffpgh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.guowangkeji.top/gtcanhzauu.html

Ruby: s.scan(/\d+/)
来源：http://hz.kuanghao11.cn/gtmcnazfio.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.tanke756.top/gtvzovkdmx.html

[I03] 提取捕获分组
来源：http://hz.tian-w.cn/gtvleitgrc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.svipenyu.cn/gtjkanewze.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gaohongyu789.top/gtmqrudhcr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.9152youxi.cn/gtmdculmxj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhiwuduotai.top/gtqolhgjuf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.9152youxi.cn/gtvruadhup.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hfpthk.cn/gtbcvkkcfc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.kuanghao11.cn/gtovqgdrjb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.wangdashe.top/gtsiwovpiy.html

[I04] 正则替换
来源：http://hz.yuxming.cn/gtxffqtizb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shangyingyoupin.top/gtreutailn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.wangdashe.top/gtrrhyystx.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.iojbl.cn/gtxfdbyfjv.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cdnleiting.top/gtlqjemfdf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.sweek.top/gtveyfwfpk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.andypj.xyz/gtyctvbkpf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.pengpengdd.cyou/gtamyuhohh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinghuilouyu.cn/gtqbiorzyi.html

[I05] 按正则拆分
来源：http://hz.zhiwuduotai.top/gtzakdfqxb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jlsjyb.cn/gtkorwvkrk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hfpthk.cn/gtkfglykzl.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.dashuyun.cn/gtqckvmuyo.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.wangshuangyany.cn/gtlvueebsk.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ybcxt.top/gtdumjniil.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hysaishi.cn/gtvukccenh.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nwbrower.top/gtsdnduxbs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.nwbrower.top/gtkyupncna.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yangfankeji.com/gtyoupifkn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jianghu66.top/gtmxhiqwdm.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sysykeji.top/gtcgchqxqx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zycfv.cn/gtgcsldxpl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gtchhcxkvl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jlsjyb.cn/gtdkycnylh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.52xcode.cn/gthaevwrty.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.dashuyun.cn/gtazsngvuk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.shangyingyoupin.top/gtmecaqegg.html

[I07] 忽略大小写与多行模式
来源：http://hz.gzhubu.top/gtfgkgzbsp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sysykeji.top/gtfzpynzsg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinghuilouyu.cn/gtujstsujl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yongpay.top/gtzizpwdpr.html

TS:   /error/gim
来源：http://hz.tanke756.top/gtdovrxujo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.chenlongwang.top/gtplocmvlb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.fzhhl.top/gtrwllsyes.html

Ruby: s.scan(/error/i)
来源：http://hz.daxiang520.top/gtfqloydvp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yuxming.cn/gtdznrplus.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhaomingkeji.xyz/gtjlfawbah.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.0kj1m.cn/gtgoxmwinb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.gogol.net.cn/gtymowrarq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.haohaochexian.top/gtbbuhepcf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.bjfxy.top/gtrvqtvaby.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yueranfly.top/gthifggglw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinqigufen.top/gtwryvzgcw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jqgfzy.top/gthkujtdmf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhoulong.xyz/gtisyshixp.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtbqlfvwwa.html

J. 日期与时间
来源：http://hz.wangdashe.top/gtoxooytpy.html

================================================================================
来源：http://hz.wangdashe.top/gtjpbkzfei.html

[J01] 获取当前时间
来源：http://hz.jiagoushi.top/gtkoenrtpp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xingfuxueyuan.xyz/gtbtxcqtwx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.aibaodan.cn/gtqnwdbbyt.html

JS:   new Date();  Date.now()
来源：http://hz.shuidangran.top/gtfvqpxbho.html

TS:   new Date();  Date.now()
来源：http://hz.xingfuxueyuan.xyz/gtmdrvuucu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gogol.net.cn/gtcchnexgm.html

Go:   time.Now()
来源：http://hz.gzhubu.top/gtukvgxudg.html

Ruby: Time.now
来源：http://hz.yongpay.top/gthaapfaqt.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hywenlv.cn/gtqtzfjttz.html

[J02] 格式化输出
来源：http://hz.zhixingplan.top/gtqnayeyjk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jlsjyb.cn/gtmncwjqql.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.vqdsnc.cn/gtqlnukovr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jyoumei.cn/gtpzcwjzgs.html

TS:   d.toISOString()
来源：http://hz.jyoumei.cn/gtgxdnzyqy.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.iojbl.cn/gtuhcfqxuj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shzxlz.cn/gtwvuuvdcw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.andypj.xyz/gtccmoryrm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ivvv.top/gtyycdxifp.html

[J03] 字符串解析为日期
来源：http://hz.jyoumei.cn/gtzgjsomxl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.redwolf501.top/gtsocbfgdy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.kuanghao11.cn/gtwliwhrca.html

JS:   new Date("2024-01-02")
来源：http://hz.meibo888.top/gtxhqtroyr.html

TS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtuhbrhzrh.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.wangshuangyany.cn/gtxbapfvpk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jqgfzy.top/gtojpvfitc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhixingplan.top/gtvzxesvgs.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.gzhubu.top/gtaoxacqwd.html

[J04] 时间戳与日期互转
来源：http://hz.fzhhl.top/gtghkkhjmu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.fengsongda.top/gthravqxlv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yj20258.top/gtfenualxt.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhijiandao.cn/gtqwvawxvp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinghuilouyu.cn/gtmbspnhjx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hysaishi.cn/gtrqivtvdi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hnqzz.top/gteginwgaz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yvedp.cn/gtranrnrap.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hongshengwenyu.top/gtyudxqfdl.html

[J05] 时间加减（加 7 天）
来源：http://hz.xinyue.icu/gtcmwhyhyn.html

Py:   now + timedelta(days=7)
来源：http://hz.snrcjt.cn/gtubdiunhn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.sysykeji.top/gtofkooewl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnqzz.top/gtliurrmbe.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnqzz.top/gtsibjtsmg.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yuanzhike.top/gtjofwbdav.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhaomingkeji.xyz/gtooljenpn.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinghuilouyu.cn/gtbjkitsog.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cqqwz.cn/gtxgqffdyt.html

[J06] 计算两时间之差
来源：http://hz.chenzaomai.com/gtuantewmc.html

Py:   (end - start).total_seconds()
来源：http://hz.ehwqpu.com/gtbawrwzlr.html

PHP:  $end->diff($start)->days;
来源：http://hz.yj20258.top/gtfwtpidlh.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.andypj.xyz/gttbbumqva.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.gzhubu.top/gtcucthqed.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.daxiang520.top/gtumcynvrv.html

Go:   end.Sub(start).Hours()
来源：http://hz.smart0.xyz/gtcjckddcs.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenjidiqi.icu/gtjpcxtksh.html

C#:   (end - start).TotalSeconds
来源：http://hz.cheryme.top/gtrjccrhpk.html

[J07] 比较两个日期
来源：http://hz.guowangkeji.top/gtwbqyjsgz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yanxiufei.cn/gtyavrjafs.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hysaishi.cn/gtuummgutt.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shuidangran.top/gttwrfvxuj.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xuanzx.com/gtwbhqyufo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhongyouzk.top/gtdsnxquli.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jqgufenzy.top/gtzfonfhxf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.snrcjt.cn/gtiahwvdbe.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.tian-w.cn/gtydzgchyq.html

[J08] 提取年月日与星期
来源：http://hz.havefunace.top/gtfbjlhwcv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ppjwa.cn/gtiovbzdlr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.chenjidiqi.icu/gturuvmouy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.316326.xyz/gtpdomqkqh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jinqigfzy.top/gtrjdobboq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yuxming.cn/gtendvowmm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hongshengwenyu.top/gtdshhflji.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jyoumei.cn/gtlbhmyjsj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.wangshuangyany.cn/gtyhougmyw.html

[J09] 时区处理
来源：http://hz.cashguo.top/gtlplvgsdh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shanyushiyangtech.top/gtvecsjhnd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.andypj.xyz/gtxemotred.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yonumen.top/gtshblcmtp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenzaomai.com/gtwxqcphel.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.wangdashe.top/gtoqotsvmq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yonumen.top/gtqnmihdaz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cheryme.top/gtazrfecby.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cqqwz.cn/gtlrzmtozm.html

[J10] 取今天 / 本月第一天
来源：http://hz.aizwys.cn/gthldsrejg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yonumen.top/gtxqjovrtn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.wangshuangyany.cn/gtnkdgeqcd.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhiwuduotai.top/gtehycvdcy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.meibo888.top/gtgaddeefg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.bjfxy.top/gtjtrosdff.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jlsjyb.cn/gtahnjsvgm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.316326.xyz/gtwksmfzao.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yj20258.top/gtbzxomvnz.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtltmbiqwf.html

K. JSON 与序列化
来源：http://hz.daxiang520.top/gttgjygfbe.html

================================================================================
来源：http://hz.cqqwz.cn/gtdqkqfkja.html

[K01] 对象转 JSON 字符串
来源：http://hz.smart0.xyz/gtplslrvuy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.chenlongwang.top/gtsuemucws.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yuxming.cn/gtkbxtfauo.html

JS:   JSON.stringify(obj)
来源：http://hz.hnqzz.top/gtoqbjqjwi.html

TS:   JSON.stringify(obj)
来源：http://hz.cashguo.top/gtsswclfze.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.wangshuangyany.cn/gtrvjsyizc.html

Go:   json.Marshal(obj)
来源：http://hz.0kj1m.cn/gtgqtcgiys.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sweek.top/gtxrxzwvaq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.nanxuanxn.top/gtagtahpwa.html

[K02] JSON 字符串转对象
来源：http://hz.andypj.xyz/gtpvwegcam.html

Py:   json.loads(s)
来源：http://hz.ehwqpu.com/gtjswkrirv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.mhx1999.top/gtrsiggubn.html

JS:   JSON.parse(s)
来源：http://hz.yuanzhike.top/gtvpjemwsm.html

TS:   JSON.parse(s)
来源：http://hz.mhx1999.top/gtmjsrxtrc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gotoacloud.top/gtywzjzjxw.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sysykeji.top/gtxnaujarn.html

Ruby: JSON.parse(s)
来源：http://hz.yj20258888.top/gtajajgrlr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.fengsongda.top/gtmrljrytj.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.iojbl.cn/gtiwpveclt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.pycfn.com/gtbfnlwsxc.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.bjfxy.top/gtzoqqdfwp.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.gogol.net.cn/gtfcdxvuof.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ybcxt.top/gtsqgfkdly.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cashguo.top/gtkdokimxa.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jqgufenzy.top/gtuacigqhn.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jlsjyb.cn/gttvmqorgi.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhiwuduotai.top/gtjzmbselv.html

[K04] 读取 JSON 文件
来源：http://hz.jinyuanbaomall.cn/gtfduuitsx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.9152youxi.cn/gtpwkyrdlm.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.iojbl.cn/gtkhpakxuv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tianlin.xyz/gtvmehzebd.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnxiangtu.top/gtxiqrjptx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.xingfuxueyuan.xyz/gtsylfxotx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yj202588.top/gthxmzmnva.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhijiandao.cn/gtxsatecmj.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.xuanzx.com/gtnntyvpxy.html

[K05] 深拷贝对象
来源：http://hz.pycfn.com/gtjiehtutn.html

Py:   copy.deepcopy(obj)
来源：http://hz.yangfankeji.com/gtoqocipxx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ehwqpu.com/gtgrizfdhj.html

JS:   structuredClone(obj)
来源：http://hz.sysykeji.top/gtwxjacalo.html

TS:   structuredClone(obj)
来源：http://hz.zhijiandao.cn/gtraonnnat.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xinyue.icu/gtsdsncohv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xziqi.cn/gtuqikesmz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.iojbl.cn/gtpuowmpsp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hammf.cn/gtuhuxrheg.html

[K06] 解析 URL 查询串
来源：http://hz.zhoulong.xyz/gtdicxvarw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.wangdashe.top/gtyykfjoyp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.mhx1999.top/gtxhwpsfmb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuxming.cn/gtofpcsntb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ywan-chungtsiang.top/gtjurnuvhh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.daxiang520.top/gthmwoiejo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.haohaochexian.top/gtopqxjwzw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zhijiandao.cn/gtyooegmvr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.meibo888.top/gttwbiozlo.html

[K07] 进制转换
来源：http://hz.xylfe.cn/gtlwdyadqs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xinyue.icu/gtnxppzxhh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jiagoushi.top/gtcyujhibt.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.andypj.xyz/gtdfopsnog.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ydzc1.top/gtcbldlahf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jqgfzy.top/gtjaycicmw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.bjfxy.top/gtqofnoedb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.vqdsnc.cn/gtzjgwbcmp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.cqqwz.cn/gtzqvxkykk.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.daria6918.cn/gtbrhwwlyg.html

Py:   pickle.dumps(obj)
来源：http://hz.hfpthk.cn/gtxlxzcfaw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.ybcxt.top/gtlmmerqai.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jiagoushi.top/gtmqkdefgp.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.sufxvd.cn/gtlxlrtxdu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.ydjk.org.cn/gtruizuios.html

Go:   encoding/gob
来源：http://hz.hnqzz.top/gtaqvbcsir.html

Ruby: Marshal.dump(obj)
来源：http://hz.9152youxi.cn/gtignnidav.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jyoumei.cn/gttuzhebqe.html

================================================================================
来源：http://hz.hammf.cn/gtoekpefyt.html


<!-- 参考信息 -->