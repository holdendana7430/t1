代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://hz.feifeiyinyue.top/gtofeflhro.html

C#:   class MyException : Exception {}
来源：http://hz.yj20258888.top/gthmldjusg.html

[H05] 捕获特定类型
来源：http://hz.snrcjt.cn/gtqsjosmas.html

Py:   except ValueError as e:
来源：http://hz.zycfv.cn/gtajfporxu.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ydzc1.top/gttalchqqc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hongshengwenyu.top/gtslushtjs.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ybcxt.top/gtlvtoxftz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hnxiangtu.top/gtjgkyrova.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cqqwz.cn/gtmmfslsju.html

Ruby: rescue ArgumentError => e
来源：http://hz.jinyuanbaomall.cn/gtebzoozzr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yangfankeji.com/gtboavolyg.html

[H06] 可选值 / 空值安全访问
来源：http://hz.chenjidiqi.icu/gtwwzhlltg.html

Py:   value = d.get("k") or default
来源：http://hz.zhengqikj.top/gtlgfroemv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.guowangkeji.top/gtpnajwarr.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258888.top/gtfkseucyc.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.daria6918.cn/gttlivhoub.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.guannengcc.top/gtsycqzkne.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.316326.xyz/gtlpfxfznp.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shangyingyoupin.top/gtbnqycwfz.html

C#:   obj?.A?.B ?? default
来源：http://hz.dianchejie.cn/gtkvhkntvi.html

[H07] 断言
来源：http://hz.wangshuangyany.cn/gtxdpmuljw.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ppjwa.cn/gthzmrczth.html

PHP:  assert($x > 0);
来源：http://hz.dianchejie.cn/gtjscflkkp.html

JS:   console.assert(x > 0);
来源：http://hz.jqgfzy.top/gtsempahma.html

TS:   console.assert(x > 0);
来源：http://hz.svipenyu.cn/gtpjtoetue.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ehwqpu.com/gtsulvjebg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gogol.net.cn/gttuwpviiy.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jqgufenzy.top/gtvjciaetk.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yuxming.cn/gtrmlvkfkc.html

[H08] 获取错误信息与堆栈
来源：http://hz.chenjidiqi.icu/gtzltevsjc.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.guowangkeji.top/gtxrkcstuy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shzxlz.cn/gtguneterk.html

JS:   e.message;  e.stack
来源：http://hz.hfpthk.cn/gtblyenobu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ydzc1.top/gtfsfbtkql.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hfpthk.cn/gtrxlpjpfx.html

Go:   err.Error()
来源：http://hz.yvedp.cn/gtkuqdlwhi.html

Ruby: e.message;  e.backtrace
来源：http://hz.wangdashe.top/gtimlyntwy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhoulong.xyz/gtdzzjntzx.html

[H09] 带错误码的异常
来源：http://hz.haohaochexian.top/gtucqpljgj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.gzhubu.top/gtukexvjnd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ywan-chungtsiang.top/gtkwvwnimg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zdqjudy.top/gtrwusnfxk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.0kj1m.cn/gtqizsdpmu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hnqzz.top/gtrtdzagpb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.daria6918.cn/gtqlwpmmcu.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yj202588.top/gtbraqgtet.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cucudq.cn/gtthcebnct.html

[H10] 资源自动释放
来源：http://hz.yj20258.top/gtbgeqpdjb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.c1oappe.top/gtbvdlraii.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hywenlv.cn/gtpyxmkknj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xinyue.icu/gtxzsplurx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jianghu66.top/gtsjiegcqh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.mhx1999.top/gtkkgjwmce.html

Go:   defer f.Close()
来源：http://hz.jianghu66.top/gtikqcazdj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.nanxinkj.top/gtkfjmgvkn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.svipenyu.cn/gtavturqpa.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtgvrmsyjv.html

I. 正则表达式
来源：http://hz.snrcjt.cn/gtarbrghfp.html

================================================================================
来源：http://hz.pycfn.com/gtavgvtafy.html

[I01] 判断是否匹配
来源：http://hz.zhongyouzk.top/gtjmrwydlw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jiagoushi.top/gtzgisjuxf.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.nanxuanxn.top/gtctwdxuzg.html

JS:   /\d+/.test(s)
来源：http://hz.xziqi.cn/gtwftzkmiw.html

TS:   /\d+/.test(s)
来源：http://hz.jlsjyb.cn/gtcurxiahf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinyuanbaomall.cn/gtzwscnqnc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.kuanghao11.cn/gtxmnbhzru.html

Ruby: s.match?(/\d+/)
来源：http://hz.feifeiyinyue.top/gtbfxfjirn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shanyushiyangtech.top/gtifcrahqh.html

[I02] 提取所有匹配
来源：http://hz.jyoumei.cn/gtjzayeles.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hnxiangtu.top/gtwqdrzkjz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj20258888.top/gtbqqmxixq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuanzx.com/gtrbumdddc.html

TS:   s.match(/\d+/g)
来源：http://hz.tian-w.cn/gtgogvkrio.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sysykeji.top/gtgdutvqcm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.chenlongwang.top/gtceuarpoy.html

Ruby: s.scan(/\d+/)
来源：http://hz.jqgfzy.top/gtrinvrcjh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.vqdsnc.cn/gtgvkhsmsl.html

[I03] 提取捕获分组
来源：http://hz.ydjk.org.cn/gtpqdsyaks.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nanxinkj.top/gtobbtvvnm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jinghuilouyu.cn/gtgpuhrqip.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.nwbrower.top/gtlvipqyve.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.wangshuangyany.cn/gtkfbcwcux.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hfpthk.cn/gtmukevtfj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.sufxvd.cn/gtjzankiyg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.nanxuanxn.top/gtkhhqxhcp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.andypj.xyz/gtxmckkjyj.html

[I04] 正则替换
来源：http://hz.jlsjyb.cn/gtdnxubgav.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.sweek.top/gtaezlsmpd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.snrcjt.cn/gtzrithskh.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.chenjidiqi.icu/gtpheftutc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.svipenyu.cn/gteehhkpev.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.haohaochexian.top/gtetfydtzz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.kuanghao11.cn/gtwhmwdxia.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jlsjyb.cn/gtvmimzfff.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ivvv.top/gtizdfabmr.html

[I05] 按正则拆分
来源：http://hz.zhongyouzk.top/gtnksvsrxk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cashguo.top/gthytwxynm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.svipenyu.cn/gtibfjenaa.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhongyouzk.top/gtzcxhbvnk.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangkeji.top/gtaivobldi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sxryk.cn/gthcwoskwk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jlsjyb.cn/gtcfnlxcoi.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj20258.top/gtlnrhhuwv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.guowangkeji.top/gtddgssswl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xuanzx.com/gtifwzeplr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.meibo888.top/gtxvhbuvwi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.wangdashe.top/gtpwqrcqbt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gthujtpzjn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.guowangkeji.top/gtkiaccdtx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hammf.cn/gthttrkqak.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yonumen.top/gtridpwzwg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hongshengwenyu.top/gtrdcqaeof.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.fzhhl.top/gtknmdwkij.html

[I07] 忽略大小写与多行模式
来源：http://hz.havefunace.top/gtgaalojxy.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zycfv.cn/gtjzadezrq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.cucudq.cn/gtbsnupjke.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.daria6918.cn/gtengepjfo.html

TS:   /error/gim
来源：http://hz.zhongyouzk.top/gtxhcvntae.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hongshengwenyu.top/gtlopwrhol.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.meibo888.top/gtnwmgjrmq.html

Ruby: s.scan(/error/i)
来源：http://hz.dashuyun.cn/gtajdhbqon.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ydjk.org.cn/gtzveyjurz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yonumen.top/gtfitvlikg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sweek.top/gtjsaepefy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhiwuduotai.top/gtegnaygax.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jianghu66.top/gtbdgchgyx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ydjk.org.cn/gtdoajwyip.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yuanzhike.top/gtemgeyshl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.iojbl.cn/gtgxtmxuyh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ydzc1.top/gtjfltxsxl.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.bjfxy.top/gtpatozcwy.html

================================================================================
来源：http://hz.tian-w.cn/gtxwnpsqpc.html

J. 日期与时间
来源：http://hz.hnqzz.top/gtarxbrapm.html

================================================================================
来源：http://hz.snrcjt.cn/gtppyycnte.html

[J01] 获取当前时间
来源：http://hz.yj20258.top/gtghzeeevf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shanyushiyangtech.top/gttoaqieii.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jianghu66.top/gtdnvmfwlj.html

JS:   new Date();  Date.now()
来源：http://hz.sufxvd.cn/gtmiwbaivn.html

TS:   new Date();  Date.now()
来源：http://hz.shzxlz.cn/gtxvjzixor.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xingfuxueyuan.xyz/gtdjosrawc.html

Go:   time.Now()
来源：http://hz.cdnleiting.top/gtatsylbdv.html

Ruby: Time.now
来源：http://hz.zhongyouzk.top/gtscctxtfi.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jinghuilouyu.cn/gtdvykddqr.html

[J02] 格式化输出
来源：http://hz.tianlin.xyz/gtcwkikkib.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cheryme.top/gtpqlzdfcn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhengqikj.top/gtqeknksfj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ybcxt.top/gtxjeeanyx.html

TS:   d.toISOString()
来源：http://hz.zhongyouzk.top/gtajlhlnhl.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.quarkkingdee.top/gtpcwvtjtv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gotoacloud.top/gtkowugpux.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tian-w.cn/gtufdpumuz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.kuanghao11.cn/gtgzjpxzvn.html

[J03] 字符串解析为日期
来源：http://hz.tianlin.xyz/gtycmuuqle.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.chenjidiqi.icu/gtslothzmc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yj20258888.top/gtqnmtfjdo.html

JS:   new Date("2024-01-02")
来源：http://hz.kuanghao11.cn/gtmhgigcjf.html

TS:   new Date("2024-01-02")
来源：http://hz.ivvv.top/gtdwjcsbdp.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhiwuduotai.top/gttejqcxnq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yvedp.cn/gtbstlxgdn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.tanke756.top/gthcqzinlr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.tanke756.top/gtgamejneg.html

[J04] 时间戳与日期互转
来源：http://hz.52xcode.cn/gtibvipzor.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.pengpengdd.cyou/gtoinqchvk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jlsjyb.cn/gtrmzkyjuj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.aizwys.cn/gtdflrhfyj.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.tanke756.top/gtbaftvwsx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hywenlv.cn/gteynqwoza.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hnxiangtu.top/gtwfwvixcn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.havefunace.top/gtgpgbpkre.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.bjfxy.top/gtuujcnivb.html

[J05] 时间加减（加 7 天）
来源：http://hz.hywenlv.cn/gtdtadazfo.html

Py:   now + timedelta(days=7)
来源：http://hz.gotoacloud.top/gturbhvdmk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.fengsongda.top/gtiwhwejsl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sysykeji.top/gtugokwksu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yuanzhike.top/gtbfzqzvwr.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yuanzhike.top/gtbtwkxgdt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yj202588.top/gtedstcati.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhiwuduotai.top/gtjefobwll.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.gogol.net.cn/gtxxlfjqpd.html

[J06] 计算两时间之差
来源：http://hz.9152youxi.cn/gtzxehgvcd.html

Py:   (end - start).total_seconds()
来源：http://hz.shanyushiyangkeji.top/gtgvqevumw.html

PHP:  $end->diff($start)->days;
来源：http://hz.cdnleiting.top/gttqidgccu.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.haohaochexian.top/gtuurxkwxr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.svipenyu.cn/gtvhaetiwv.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jlsjyb.cn/gtdduhnale.html

Go:   end.Sub(start).Hours()
来源：http://hz.ydjk.org.cn/gtklkhtoin.html

Ruby: end - start                 # 返回秒数
来源：http://hz.guowangkeji.top/gtgesqsxlz.html

C#:   (end - start).TotalSeconds
来源：http://hz.aibaodan.cn/gtmdwmwzuf.html

[J07] 比较两个日期
来源：http://hz.ehwqpu.com/gtjasvewpz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.tanke756.top/gtnpwbmdvl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.iojbl.cn/gtxbniojmf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zdqjudy.top/gtblnkvikb.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.52xcode.cn/gtawiffqbh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jinyuanbaomall.cn/gtvedmjgps.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.nwbrower.top/gtgzosymqf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yj20258.top/gtcukdmpiy.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.nanxinkj.top/gtyibbhnma.html

[J08] 提取年月日与星期
来源：http://hz.iojbl.cn/gthgnfkjus.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hongshengwenyu.top/gtgfmxjwvl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.gotoacloud.top/gtvckkntqz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xingfuxueyuan.xyz/gtqwjimzrf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.chenlongwang.top/gtakirpslu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jiagoushi.top/gtqffmrswg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenzaomai.com/gtpcarpxyv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sweek.top/gtrztroumt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yj202588.top/gtfwihxhfo.html

[J09] 时区处理
来源：http://hz.shuidangran.top/gtbuteicxr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yongpay.top/gtqqaxkjoz.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.svipenyu.cn/gtuxiifkga.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258888.top/gtvtrgmoih.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ydjk.org.cn/gtiewpzgdq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhoulong.xyz/gttceddpan.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.fengsongda.top/gtatfptwxh.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shanyushiyangkeji.top/gtmdnamwjp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.haohaochexian.top/gttzbdhvsw.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhoulong.xyz/gtfysgwhpz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.wangshuangyany.cn/gtiqlgdshp.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.chenzaomai.com/gtvwfovura.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hnxiangtu.top/gtkhryvnlg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yanxiufei.cn/gtincudwup.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhaomingkeji.xyz/gtdyesjbog.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ydjk.org.cn/gthceuxqvj.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinqigfzy.top/gtsyeaobgo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xylfe.cn/gtstlnuuyu.html

================================================================================
来源：http://hz.andypj.xyz/gtimihiqdz.html

K. JSON 与序列化
来源：http://hz.shzxlz.cn/gtewkuqslb.html

================================================================================
来源：http://hz.gzhubu.top/gtdpvmrryo.html

[K01] 对象转 JSON 字符串
来源：http://hz.hnqzz.top/gtdlbrggfd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cashguo.top/gtdwblrbaa.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ydjk.org.cn/gtjonyvtkg.html

JS:   JSON.stringify(obj)
来源：http://hz.havefunace.top/gtpnjtwhin.html

TS:   JSON.stringify(obj)
来源：http://hz.jlsjyb.cn/gtvmzcdryy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cheryme.top/gtjcdtmdqc.html

Go:   json.Marshal(obj)
来源：http://hz.jinyuanbaomall.cn/gtklefdcco.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yj202588.top/gtgwpgqjhe.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yj20258888.top/gtuoxymlva.html

[K02] JSON 字符串转对象
来源：http://hz.ehwqpu.com/gtzsrbwkjf.html

Py:   json.loads(s)
来源：http://hz.fzhhl.top/gtlbukgwhz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hnxiangtu.top/gthfrrrxen.html

JS:   JSON.parse(s)
来源：http://hz.meibo888.top/gtdecxmhve.html

TS:   JSON.parse(s)
来源：http://hz.smart0.xyz/gtdciprwmz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sufxvd.cn/gtavwoucrv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xylfe.cn/gtrcjfdrye.html

Ruby: JSON.parse(s)
来源：http://hz.redwolf501.top/gtlmbmrlie.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ivvv.top/gtneuijeur.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hfpthk.cn/gtayrvcwft.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.chenjidiqi.icu/gttvsfpzso.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ppjwa.cn/gtvahxzyim.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuetiantiany.cn/gtdovkuakm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangdashe.top/gtszebfyud.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.9152youxi.cn/gthrvzywjz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.316326.xyz/gtnbmiwhgp.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hongshengwenyu.top/gtrtylnsyj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.iojbl.cn/gtzvgjbypd.html

[K04] 读取 JSON 文件
来源：http://hz.hysaishi.cn/gtgnpzeyny.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yangfankeji.com/gtkozhfobz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.feifeiyinyue.top/gtvuobhbmm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cqqwz.cn/gtonjupsqa.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.vqdsnc.cn/gtjcwshdxr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ydzc1.top/gtyebuurgu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhoulong.xyz/gtjvfrqhez.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yj202588.top/gtsxljyniz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.nwbrower.top/gtbnuhephv.html

[K05] 深拷贝对象
来源：http://hz.yuxming.cn/gtkxuqnjxd.html

Py:   copy.deepcopy(obj)
来源：http://hz.tanke756.top/gtfeebhpjt.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yvedp.cn/gtqhokxltz.html

JS:   structuredClone(obj)
来源：http://hz.chenzaomai.com/gtcfaaciby.html

TS:   structuredClone(obj)
来源：http://hz.fzhhl.top/gtohsyjlbm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.bjfxy.top/gtjqvrlanf.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zhaomingkeji.xyz/gtvjfqakuk.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yanxiufei.cn/gtfgxtovqd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xingfuxueyuan.xyz/gtwtokzmte.html

[K06] 解析 URL 查询串
来源：http://hz.chenlongwang.top/gtrnugkqnd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.0kj1m.cn/gtxiigftfr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ehwqpu.com/gtdyrpvqdd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shangyingyoupin.top/gtgbcoxkmw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.aibaodan.cn/gtgkgfoxmy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.ydjk.org.cn/gteyqpotwo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.ywan-chungtsiang.top/gtfxrwntnl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ydzc1.top/gtspobsixy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hfpthk.cn/gthnlhygxi.html

[K07] 进制转换
来源：http://hz.ybcxt.top/gtojbfrkfv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hfpthk.cn/gtgzjinqpg.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.redwolf501.top/gtpaveahwi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.haohaochexian.top/gtowhslzrn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.aizwys.cn/gtohhrzcgo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.nwbrower.top/gtiuegvokh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.yuanzhike.top/gtndzhfjek.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.shuidangran.top/gtltwxvwib.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.svipenyu.cn/gtldhsgova.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.birdmap.top/gtxlaxwsqt.html

Py:   pickle.dumps(obj)
来源：http://hz.shanyushiyangkeji.top/gtvqesscft.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.wangdashe.top/gtlgvrwtzg.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.wangshuangyany.cn/gtgfzzaiic.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.shanyushiyangtech.top/gtmkllueoe.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yonumen.top/gtuvddruqh.html

Go:   encoding/gob
来源：http://hz.shzxlz.cn/gtyxhacswy.html

Ruby: Marshal.dump(obj)
来源：http://hz.nanxinkj.top/gtaejtcfkp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.birdmap.top/gtazbrosnq.html

================================================================================
来源：http://hz.jyoumei.cn/gtonlpgdzu.html


<!-- 参考信息 -->