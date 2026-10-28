代发 wailian999

TS:   throw new Error("错误信息");
来源：http://hz.yvedp.cn/gtycpmnghf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.pycfn.com/gtdesyuclg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.wangdashe.top/gtoqvoumal.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cqqwz.cn/gtmelxiqfj.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cheryme.top/gtugzbcxop.html

[H04] 自定义异常类型
来源：http://hz.jiagoushi.top/gttfuycycv.html

Py:   class MyError(Exception): pass
来源：http://hz.c1oappe.top/gtlwqheike.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jiagoushi.top/gtrgpjjrip.html

JS:   class MyError extends Error {}
来源：http://hz.zhiwuduotai.top/gtouvcoqfb.html

TS:   class MyError extends Error {}
来源：http://hz.sweek.top/gtmxsjaauu.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhixingplan.top/gtxrthydjf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.fengsongda.top/gtpfegvcjy.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhoulong.xyz/gtfkrfntus.html

C#:   class MyException : Exception {}
来源：http://hz.hongshengwenyu.top/gtvikdkrvl.html

[H05] 捕获特定类型
来源：http://hz.hnxiangtu.top/gtfscbnrhg.html

Py:   except ValueError as e:
来源：http://hz.jiagoushi.top/gtdrnvqqjz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.pycfn.com/gtubmtbwuy.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ywan-chungtsiang.top/gtdtaskebz.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sufxvd.cn/gtrajpqeyb.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ppjwa.cn/gtxhebiupo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinyuanbaomall.cn/gtwdixbixs.html

Ruby: rescue ArgumentError => e
来源：http://hz.52xcode.cn/gtmjnhblvz.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yangfankeji.com/gtshbpilkv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jinqigfzy.top/gtdpzwelcm.html

Py:   value = d.get("k") or default
来源：http://hz.hnxiangtu.top/gtlrgkaqwe.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jlsjyb.cn/gtosacjkgb.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sweek.top/gtoplqkopd.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yj202588.top/gtqyejnyzq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.vqdsnc.cn/gtcqsgmkla.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yj20258.top/gtipbgnikk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.9152youxi.cn/gtssczygtd.html

C#:   obj?.A?.B ?? default
来源：http://hz.daxiang520.top/gtcxeortwe.html

[H07] 断言
来源：http://hz.shangyingyoupin.top/gtjosengkf.html

Py:   assert x > 0, "必须为正"
来源：http://hz.52xcode.cn/gtyavjhbfo.html

PHP:  assert($x > 0);
来源：http://hz.xylfe.cn/gtuuhsfzpc.html

JS:   console.assert(x > 0);
来源：http://hz.zhaomingkeji.xyz/gtwdjdxtte.html

TS:   console.assert(x > 0);
来源：http://hz.zhoulong.xyz/gtqvsszbaj.html

Java: assert x > 0 : "必须为正";
来源：http://hz.tanke756.top/gtdsubnrbi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jyoumei.cn/gtyrjbvuid.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhaomingkeji.xyz/gtlxqkaycc.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yueranfly.top/gtmlkukaes.html

[H08] 获取错误信息与堆栈
来源：http://hz.shzxlz.cn/gtczoduxzn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ydjk.org.cn/gtllvbsgpu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.tianlin.xyz/gtydzudqss.html

JS:   e.message;  e.stack
来源：http://hz.snrcjt.cn/gtsfehkyuz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jlsjyb.cn/gtulpiswbf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hnxiangtu.top/gtfxlclvya.html

Go:   err.Error()
来源：http://hz.zhoulong.xyz/gthpfgcauu.html

Ruby: e.message;  e.backtrace
来源：http://hz.ydzc1.top/gtjpnlxagy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhijiandao.cn/gtcrchvlal.html

[H09] 带错误码的异常
来源：http://hz.dashuyun.cn/gtyyvomkso.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.aibaodan.cn/gtlrumiqtt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinghuilouyu.cn/gtfeddqowa.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jianghu66.top/gtfmzjjbua.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinqigufen.top/gtalrwzghg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.aizwys.cn/gtbipgvkhb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jqgufenzy.top/gtakowiwbw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xylfe.cn/gthkhvknxy.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.dianchejie.cn/gtaczaxjtm.html

[H10] 资源自动释放
来源：http://hz.zdqjudy.top/gtnffopron.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.chenlongwang.top/gtdfhfckea.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ybcxt.top/gthuqenwur.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ppjwa.cn/gtwbpzbmvg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ywan-chungtsiang.top/gtrmzoltoz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ehwqpu.com/gtxsxsbuxj.html

Go:   defer f.Close()
来源：http://hz.jinqigfzy.top/gtrvkxslrk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ehwqpu.com/gtslfaaymo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.wangshuangyany.cn/gtmvlvaapn.html

================================================================================
来源：http://hz.guannengcc.top/gtgoahvezq.html

I. 正则表达式
来源：http://hz.xingfuxueyuan.xyz/gtalasoers.html

================================================================================
来源：http://hz.gotoacloud.top/gtpfbtsijc.html

[I01] 判断是否匹配
来源：http://hz.daxiang520.top/gtkjifkpdp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yongpay.top/gtyufijiub.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.52xcode.cn/gtqxftdbug.html

JS:   /\d+/.test(s)
来源：http://hz.yuanzhike.top/gtsbirhnzk.html

TS:   /\d+/.test(s)
来源：http://hz.ybcxt.top/gtzwrnnbhe.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.iojbl.cn/gtoqmlwlhm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhongyouzk.top/gtlxwbjnar.html

Ruby: s.match?(/\d+/)
来源：http://hz.cdnleiting.top/gtipfthczp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhiwuduotai.top/gtotgnalfl.html

[I02] 提取所有匹配
来源：http://hz.zhongyouzk.top/gtljekrzlx.html

Py:   re.findall(r"\d+", s)
来源：http://hz.chenlongwang.top/gtlfqhcikh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jinqigufen.top/gtacsledxy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj20258888.top/gtcvslatjf.html

TS:   s.match(/\d+/g)
来源：http://hz.zycfv.cn/gtrdzxjfoi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hywenlv.cn/gtqypmmijp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.svipenyu.cn/gtqdpccvad.html

Ruby: s.scan(/\d+/)
来源：http://hz.sysykeji.top/gtumcdvomz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.kuanghao11.cn/gtmrejvjiu.html

[I03] 提取捕获分组
来源：http://hz.feifeiyinyue.top/gtihwtoyvg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zycfv.cn/gtyhumslaz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ehwqpu.com/gtytiynuoj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.sxryk.cn/gtknvyhekd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yj202588.top/gtsrsjmzbj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.52xcode.cn/gthvujuhul.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.c1oappe.top/gthjmzgfkk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.chenjidiqi.icu/gtnqhefims.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.andypj.xyz/gtltgtufwd.html

[I04] 正则替换
来源：http://hz.yueranfly.top/gteotojyni.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.svipenyu.cn/gttsxefaay.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.chenjidiqi.icu/gtbtubwhab.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.chenzaomai.com/gtavemmjhr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hongshengwenyu.top/gtkhszqsva.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hammf.cn/gtqsyeoapy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.svipenyu.cn/gtjzqbmdik.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhoulong.xyz/gtircxvuxm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinyuanbaomall.cn/gtwfthgsti.html

[I05] 按正则拆分
来源：http://hz.hywenlv.cn/gtnjylxuqv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cucudq.cn/gtbxyckmkq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gzhubu.top/gtgzuwszqn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhiwuduotai.top/gtqvzbfirq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangkeji.top/gtgrsslues.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xinyue.icu/gtacwbwaok.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shanyushiyangkeji.top/gtebgdrhww.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj20258888.top/gttraykcae.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.guowangkeji.top/gtfryklfxe.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hongshengwenyu.top/gtnclmfhzk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shanyushiyangtech.top/gtrjtukvnf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.wangdashe.top/gtmoyeuqgd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgufenzy.top/gtqrpqvzue.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hongshengwenyu.top/gtgfwfmshz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gtvmokdacm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.bjfxy.top/gtscdwnnwb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.mhx1999.top/gtoszxfbls.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.chenzaomai.com/gtxalrfane.html

[I07] 忽略大小写与多行模式
来源：http://hz.tianlin.xyz/gthpagkndf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.gaohongyu789.top/gtrfzzmumv.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jlsjyb.cn/gtzgwwtdne.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hfpthk.cn/gtguozqvse.html

TS:   /error/gim
来源：http://hz.jinqigfzy.top/gtavqdjjlk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hammf.cn/gtqupwnoay.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yvedp.cn/gtnelpgvgs.html

Ruby: s.scan(/error/i)
来源：http://hz.yonumen.top/gtvwhlbixy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.smart0.xyz/gtzdbamfat.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.c1oappe.top/gtrjiuygxi.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jiagoushi.top/gtjmrsybss.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.kuanghao11.cn/gtkwsahzos.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yangfankeji.com/gtskfbgiar.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jlsjyb.cn/gtwkvbgwgg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhengqikj.top/gtnbrpnnwt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ybcxt.top/gtjcbhvxet.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cheryme.top/gtwjwihxhu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.chenjidiqi.icu/gtrysdlnuj.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtaztipzrw.html

J. 日期与时间
来源：http://hz.daxiang520.top/gtwikvopvb.html

================================================================================
来源：http://hz.zhongyouzk.top/gtkytujqbg.html

[J01] 获取当前时间
来源：http://hz.yongpay.top/gtzqatcgsf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.9152youxi.cn/gtcfgnfaaa.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jqgfzy.top/gtxjiirrgt.html

JS:   new Date();  Date.now()
来源：http://hz.vqdsnc.cn/gtgckqnmok.html

TS:   new Date();  Date.now()
来源：http://hz.guowangkeji.top/gtoxhtfysb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinqigufen.top/gtrvtoaxaw.html

Go:   time.Now()
来源：http://hz.sweek.top/gtinqaejeq.html

Ruby: Time.now
来源：http://hz.shzxlz.cn/gtdygoifuf.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shzxlz.cn/gtfgappcvo.html

[J02] 格式化输出
来源：http://hz.yonumen.top/gttokszuuq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangshuangyany.cn/gtwkroszwz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.vqdsnc.cn/gtmtlbupbx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.meibo888.top/gtmyibrzyv.html

TS:   d.toISOString()
来源：http://hz.snrcjt.cn/gtvwikvbbt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.cashguo.top/gtchovffru.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.chenzaomai.com/gtwsjuvgdk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hysaishi.cn/gtmxztjzmc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zycfv.cn/gtemfunnms.html

[J03] 字符串解析为日期
来源：http://hz.hammf.cn/gtuxrdmyqy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.cdnleiting.top/gtkopqtzxi.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.daria6918.cn/gtbekfyvfi.html

JS:   new Date("2024-01-02")
来源：http://hz.meibo888.top/gtbkasolpj.html

TS:   new Date("2024-01-02")
来源：http://hz.kuanghao11.cn/gtqfdrqcel.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jinqigufen.top/gtowprsdqq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtzmjyvwzh.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtuxkvnphc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.9152youxi.cn/gtaponksrm.html

[J04] 时间戳与日期互转
来源：http://hz.fengsongda.top/gttyiffuys.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hongshengwenyu.top/gtryfrbsgl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cucudq.cn/gtpnsjmptn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.andypj.xyz/gtictknwkr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jlsjyb.cn/gttpfzqqpv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.guowangkeji.top/gtlzrjpxwy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhongyouzk.top/gtzqyiokdf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ehwqpu.com/gtpdtiiomt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ppjwa.cn/gttkoxwixt.html

[J05] 时间加减（加 7 天）
来源：http://hz.cheryme.top/gtfcbupzir.html

Py:   now + timedelta(days=7)
来源：http://hz.cashguo.top/gtgmoevdlm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.aibaodan.cn/gtkhttjtgr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tanke756.top/gtnxjyryej.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cdnleiting.top/gttgtytqpx.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ivvv.top/gtayjychij.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhiwuduotai.top/gtmuqifeog.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ppjwa.cn/gtoexwtcqv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhaomingkeji.xyz/gtrudbvntb.html

[J06] 计算两时间之差
来源：http://hz.vqdsnc.cn/gtuwttwode.html

Py:   (end - start).total_seconds()
来源：http://hz.iojbl.cn/gtqywtzbwa.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhijiandao.cn/gtlzujqrhv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zycfv.cn/gtohujocem.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jyoumei.cn/gtpfsveyvz.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yanxiufei.cn/gtkohqvbwd.html

Go:   end.Sub(start).Hours()
来源：http://hz.xinyue.icu/gtqxxsctzq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhoulong.xyz/gtxmfpewcs.html

C#:   (end - start).TotalSeconds
来源：http://hz.jinqigufen.top/gtwwowqzpi.html

[J07] 比较两个日期
来源：http://hz.52xcode.cn/gtwiebadit.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.dianchejie.cn/gtekthpbov.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hongshengwenyu.top/gtsinjltsc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hnqzz.top/gtljlyhukw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shzxlz.cn/gtjtyzfrhb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.redwolf501.top/gtnljskhqk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.cashguo.top/gtypohwtpl.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gzhubu.top/gtetepyyhv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.redwolf501.top/gtngbksafk.html

[J08] 提取年月日与星期
来源：http://hz.jinqigfzy.top/gtqzmobnnv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinyuanbaomall.cn/gtlgncemym.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.svipenyu.cn/gtvulgncfi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.316326.xyz/gtqwvlpkdj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.svipenyu.cn/gtjebxwnuu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.iojbl.cn/gtsvdmgnjz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yvedp.cn/gtlgnbbrim.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jiagoushi.top/gtfaqgdcrr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zdqjudy.top/gtzlacfrvw.html

[J09] 时区处理
来源：http://hz.jinqigufen.top/gthkqbmdid.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yueranfly.top/gtdzsegpmg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.pengpengdd.cyou/gtkqdkxcbz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.pycfn.com/gttdfndoll.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.nanxuanxn.top/gtanjmabzo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.9152youxi.cn/gtjzukckdv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.guannengcc.top/gtvkxyinhv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yueranfly.top/gthehlnoxm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.havefunace.top/gttvsnxlny.html

[J10] 取今天 / 本月第一天
来源：http://hz.9152youxi.cn/gtpfdupjym.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhongyouzk.top/gthwgcntss.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yueranfly.top/gtbddhxeci.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.aibaodan.cn/gtsvrwauii.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinqigfzy.top/gtsqgiqkdv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yueranfly.top/gtucmfhlia.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.haohaochexian.top/gtlzyvbjxn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.dashuyun.cn/gtmendeqrk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gogol.net.cn/gtmgcfemuo.html

================================================================================
来源：http://hz.jyoumei.cn/gtvmeameqo.html

K. JSON 与序列化
来源：http://hz.ehwqpu.com/gtpvxvfpgx.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtgqnehsgl.html

[K01] 对象转 JSON 字符串
来源：http://hz.hysaishi.cn/gtynwuodwf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.snrcjt.cn/gtpgoupqek.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.daxiang520.top/gtswthqmfj.html

JS:   JSON.stringify(obj)
来源：http://hz.chenzaomai.com/gtczyjvziq.html

TS:   JSON.stringify(obj)
来源：http://hz.pycfn.com/gtvrdqpagy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.pycfn.com/gtsktkhfph.html

Go:   json.Marshal(obj)
来源：http://hz.fengsongda.top/gtpvwaerro.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.havefunace.top/gtyewoflci.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.bjfxy.top/gtwymlwthj.html

[K02] JSON 字符串转对象
来源：http://hz.hnqzz.top/gtvvuijead.html

Py:   json.loads(s)
来源：http://hz.mhx1999.top/gtyayeducd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jqgfzy.top/gthoumgazb.html

JS:   JSON.parse(s)
来源：http://hz.cashguo.top/gtqjgtgpdb.html

TS:   JSON.parse(s)
来源：http://hz.ybcxt.top/gtlqsnvdlt.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hnxiangtu.top/gtjdjwhfto.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.0kj1m.cn/gtrosjxury.html

Ruby: JSON.parse(s)
来源：http://hz.cdnleiting.top/gtoizlenvr.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.cucudq.cn/gtouplwzdu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yj202588.top/gtlicjaoae.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shuidangran.top/gtjkmwgipm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.dashuyun.cn/gtyhcapgiz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yuanzhike.top/gtamuohlmt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuetiantiany.cn/gtfiyyzamv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.aizwys.cn/gtrdmotdgt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.birdmap.top/gtbjldpfmy.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.kuanghao11.cn/gtonlqqqsz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cheryme.top/gteuhxcmyo.html

[K04] 读取 JSON 文件
来源：http://hz.havefunace.top/gtdoxmfqsj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinqigufen.top/gtgjaivesw.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.jinghuilouyu.cn/gtxyoyvpoq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.dianchejie.cn/gtlxfbbxdp.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cdnleiting.top/gtcgincytr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.0kj1m.cn/gtqopanumj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yongpay.top/gteyxjlodd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.daxiang520.top/gtlnzttnvt.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhoulong.xyz/gtbjipgmyf.html

[K05] 深拷贝对象
来源：http://hz.jinyuanbaomall.cn/gtzvrhbhuu.html

Py:   copy.deepcopy(obj)
来源：http://hz.xinyue.icu/gtvpbychsb.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jinqigufen.top/gtxkpqsrgc.html

JS:   structuredClone(obj)
来源：http://hz.zdqjudy.top/gtfmdybpny.html

TS:   structuredClone(obj)
来源：http://hz.yj202588.top/gtdnrzffep.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.tianlin.xyz/gteslxwzou.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.cheryme.top/gtpjxanrqw.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.birdmap.top/gtkrneqzwz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hysaishi.cn/gteflbuhib.html

[K06] 解析 URL 查询串
来源：http://hz.dianchejie.cn/gtiftstgfs.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.ppjwa.cn/gtyklgufnn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.fzhhl.top/gtufsnpcqb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258.top/gtytqnqdql.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.sweek.top/gtsauyclct.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.zhaomingkeji.xyz/gttmccruhw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jiagoushi.top/gtztjdgszm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.zdqjudy.top/gtoqwreout.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gogol.net.cn/gtmtftgmoz.html

[K07] 进制转换
来源：http://hz.ivvv.top/gtexjeecfv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.zhoulong.xyz/gtajdrbivz.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.guannengcc.top/gtztdcipzp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.pycfn.com/gttlqkilwf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cheryme.top/gtdxryxojt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.cheryme.top/gtbqrmkhlj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zdqjudy.top/gticiurqmh.html


<!-- 参考信息 -->