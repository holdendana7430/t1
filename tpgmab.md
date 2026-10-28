代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xziqi.cn/gtbxkhxzub.html

[H04] 自定义异常类型
来源：http://hz.cucudq.cn/gtpbvjjdhu.html

Py:   class MyError(Exception): pass
来源：http://hz.quarkkingdee.top/gtuiqdpuad.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.daria6918.cn/gtmqnpelvt.html

JS:   class MyError extends Error {}
来源：http://hz.kuanghao11.cn/gtqhjyowdl.html

TS:   class MyError extends Error {}
来源：http://hz.xylfe.cn/gtkskszsbj.html

Java: class MyException extends RuntimeException {}
来源：http://hz.haohaochexian.top/gtegekcpht.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.daxiang520.top/gtlrlhmydl.html

Ruby: class MyError < StandardError; end
来源：http://hz.shanyushiyangtech.top/gtiyilfabf.html

C#:   class MyException : Exception {}
来源：http://hz.dianchejie.cn/gtrkqemocd.html

[H05] 捕获特定类型
来源：http://hz.sweek.top/gtjkpdezqk.html

Py:   except ValueError as e:
来源：http://hz.cucudq.cn/gtaextvexn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yuanzhike.top/gtxendukex.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.kuanghao11.cn/gteevflizh.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sufxvd.cn/gtirzzmkmn.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shzxlz.cn/gtchxyopzh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.redwolf501.top/gtxocctgxg.html

Ruby: rescue ArgumentError => e
来源：http://hz.feifeiyinyue.top/gtzvgdhozf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hfpthk.cn/gtqrydfhlu.html

[H06] 可选值 / 空值安全访问
来源：http://hz.havefunace.top/gthpdyiwnl.html

Py:   value = d.get("k") or default
来源：http://hz.ywan-chungtsiang.top/gtrbeuukzx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.andypj.xyz/gthtjdascf.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.fengsongda.top/gtqmivxmyw.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shanyushiyangtech.top/gteubxfhtf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zdqjudy.top/gtdscgictb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhijiandao.cn/gtzpltjxmw.html

Ruby: d&.dig(:a, :b)
来源：http://hz.mhx1999.top/gtpawzugas.html

C#:   obj?.A?.B ?? default
来源：http://hz.yongpay.top/gtrgadzzts.html

[H07] 断言
来源：http://hz.feifeiyinyue.top/gttxirqajf.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hfpthk.cn/gtvyyctuib.html

PHP:  assert($x > 0);
来源：http://hz.cucudq.cn/gtddrcmckp.html

JS:   console.assert(x > 0);
来源：http://hz.xziqi.cn/gtkviimylu.html

TS:   console.assert(x > 0);
来源：http://hz.guowangkeji.top/gtqifmxref.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ehwqpu.com/gtuaixodnq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hnqzz.top/gtzeseljgn.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.mhx1999.top/gtotsbkkgx.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xuanzx.com/gtgtcgjtxb.html

[H08] 获取错误信息与堆栈
来源：http://hz.fzhhl.top/gtwjnvlbrc.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinqigufen.top/gtrmuvtgzb.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shanyushiyangtech.top/gtmyqywfkj.html

JS:   e.message;  e.stack
来源：http://hz.316326.xyz/gtwskfpulu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cucudq.cn/gtzvcokdnb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jianghu66.top/gtyfawrlna.html

Go:   err.Error()
来源：http://hz.aibaodan.cn/gtqhunrmhy.html

Ruby: e.message;  e.backtrace
来源：http://hz.yangfankeji.com/gtblimpyav.html

C#:   e.Message;  e.StackTrace
来源：http://hz.kuanghao11.cn/gtejdgftac.html

[H09] 带错误码的异常
来源：http://hz.feifeiyinyue.top/gtqlscmlud.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.havefunace.top/gtnxnmxoic.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yueranfly.top/gtpifrrpdp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hfpthk.cn/gtzjuenhtw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.316326.xyz/gtglusxedz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.sufxvd.cn/gtsaanxbmd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hywenlv.cn/gtdwnoyqjw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gaohongyu789.top/gtmgxbcqqw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yangfankeji.com/gtpxqccfkt.html

[H10] 资源自动释放
来源：http://hz.jianghu66.top/gtwbrfwkrm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.tianlin.xyz/gtwalxeyru.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.tanke756.top/gtcabqnsre.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangtech.top/gttlpgfwnb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hammf.cn/gtlkrslhkq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhixingplan.top/gtkhkeaqmc.html

Go:   defer f.Close()
来源：http://hz.yj20258888.top/gttdafeqqr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sufxvd.cn/gtgknqrthu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtptumdcyu.html

================================================================================
来源：http://hz.chenlongwang.top/gttbmpwdjn.html

I. 正则表达式
来源：http://hz.jinghuilouyu.cn/gtmagdzgcl.html

================================================================================
来源：http://hz.xuanzx.com/gtixuykpyj.html

[I01] 判断是否匹配
来源：http://hz.xinyue.icu/gtaoreobqv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ivvv.top/gtpbmggkck.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.quarkkingdee.top/gtbnjegmgs.html

JS:   /\d+/.test(s)
来源：http://hz.sufxvd.cn/gtnfngbbur.html

TS:   /\d+/.test(s)
来源：http://hz.yj202588.top/gteudjurjv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yongpay.top/gtqguranpw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.quarkkingdee.top/gtkmrvdqeq.html

Ruby: s.match?(/\d+/)
来源：http://hz.dashuyun.cn/gtdfclztdp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hysaishi.cn/gtrsecyvfk.html

[I02] 提取所有匹配
来源：http://hz.yanxiufei.cn/gtombbshyk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.birdmap.top/gtqehtveel.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hysaishi.cn/gtwmaepiil.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hnxiangtu.top/gtalsrekqo.html

TS:   s.match(/\d+/g)
来源：http://hz.hywenlv.cn/gtdpuzfifx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhixingplan.top/gtozhjnvie.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hongshengwenyu.top/gthoogqkur.html

Ruby: s.scan(/\d+/)
来源：http://hz.jyoumei.cn/gtiogufudl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.pengpengdd.cyou/gtulxcuwsp.html

[I03] 提取捕获分组
来源：http://hz.jinqigfzy.top/gtuahxcynp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shanyushiyangkeji.top/gtupioubrc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yueranfly.top/gtaitrduve.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.iojbl.cn/gtjifkibrl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.guannengcc.top/gtbbluqxir.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cheryme.top/gtexdvyths.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yangfankeji.com/gtgytxleed.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hongshengwenyu.top/gtjziyhyew.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.svipenyu.cn/gteciuamah.html

[I04] 正则替换
来源：http://hz.sufxvd.cn/gtbediqkdg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.wangdashe.top/gtrppbpwdx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhiwuduotai.top/gtfcsjgasf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.dashuyun.cn/gtlnvntsut.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.snrcjt.cn/gtlyujptto.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.smart0.xyz/gtprjrzzau.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jinyuanbaomall.cn/gtudirjsns.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.dianchejie.cn/gtatmuaxka.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jiagoushi.top/gtdjainlxx.html

[I05] 按正则拆分
来源：http://hz.ppjwa.cn/gtebmhhqjj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xingfuxueyuan.xyz/gtswqqfwmr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ybcxt.top/gtnlwoutue.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cqqwz.cn/gtygxlhtgo.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.daxiang520.top/gtpmcprdai.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shangyingyoupin.top/gtytgdyrib.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yj202588.top/gtaevxzrwh.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yangfankeji.com/gtjixjbxum.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hfpthk.cn/gtjxuerlcw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.aizwys.cn/gtrrjozwaw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.kuanghao11.cn/gttseprpeh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yj20258.top/gtooullblz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhongyouzk.top/gtgjrnbare.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.svipenyu.cn/gtgqlhfgna.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ybcxt.top/gtsmjfssvj.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.tian-w.cn/gtnijilqfb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ybcxt.top/gtyglqvpts.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ivvv.top/gtbmoeovek.html

[I07] 忽略大小写与多行模式
来源：http://hz.meibo888.top/gtrztmriiq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.chenzaomai.com/gtlkfsrdtp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhijiandao.cn/gtbawdpnbi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cashguo.top/gtocitgrum.html

TS:   /error/gim
来源：http://hz.dianchejie.cn/gtfykmawxy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.redwolf501.top/gtmfrqvwmc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.iojbl.cn/gtdmrtocdr.html

Ruby: s.scan(/error/i)
来源：http://hz.zdqjudy.top/gttxtddhpd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shanyushiyangtech.top/gtbaituksy.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.jianghu66.top/gtqtewugke.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yj202588.top/gtrlojoqni.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ywan-chungtsiang.top/gtwretpcjb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yongpay.top/gtaovukqyw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ivvv.top/gtsaxjhmco.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jqgfzy.top/gtkclbujaj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.redwolf501.top/gtklauszua.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yueranfly.top/gtsjwpreat.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shangyingyoupin.top/gtgviruqvi.html

================================================================================
来源：http://hz.aizwys.cn/gtkwenosbx.html

J. 日期与时间
来源：http://hz.nwbrower.top/gtkgmzuopj.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtajgmhcnv.html

[J01] 获取当前时间
来源：http://hz.hysaishi.cn/gtsxcmhmfo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.9152youxi.cn/gtuyargrht.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.mhx1999.top/gtgkyyspho.html

JS:   new Date();  Date.now()
来源：http://hz.yanxiufei.cn/gtunrrejsp.html

TS:   new Date();  Date.now()
来源：http://hz.sufxvd.cn/gtrifyqwku.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yvedp.cn/gtpoiwymfn.html

Go:   time.Now()
来源：http://hz.ywan-chungtsiang.top/gtmnlgvijv.html

Ruby: Time.now
来源：http://hz.nanxuanxn.top/gtugkmlnbx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.nwbrower.top/gtsteyeusd.html

[J02] 格式化输出
来源：http://hz.tianlin.xyz/gtnimqjndz.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jianghu66.top/gtuqyjzcqc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.sufxvd.cn/gtrygfgiqp.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hongshengwenyu.top/gtabbbqyhm.html

TS:   d.toISOString()
来源：http://hz.zhaomingkeji.xyz/gtqjugknhg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.tian-w.cn/gttlkrmqfq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gzhubu.top/gtxpemdepi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jianghu66.top/gtujpxwvrn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gaohongyu789.top/gtqptukidd.html

[J03] 字符串解析为日期
来源：http://hz.svipenyu.cn/gtabbryppm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhaomingkeji.xyz/gttyotyxkh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.iojbl.cn/gtvhuynqmz.html

JS:   new Date("2024-01-02")
来源：http://hz.jinqigfzy.top/gtvjaqfzzd.html

TS:   new Date("2024-01-02")
来源：http://hz.cqqwz.cn/gtftjxoaja.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.fzhhl.top/gtfhngwrpc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hammf.cn/gtyikbwgzs.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.andypj.xyz/gtbqunxwyl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.svipenyu.cn/gtiwzejbng.html

[J04] 时间戳与日期互转
来源：http://hz.tianlin.xyz/gteoxsygsu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yangfankeji.com/gtjoxtuqhx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jqgufenzy.top/gtutyodcep.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.chenzaomai.com/gtxkcpokgq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yueranfly.top/gtwmxnvwwu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hysaishi.cn/gtinogcvfi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xylfe.cn/gtvmedphid.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shangyingyoupin.top/gthguvlabq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.wangdashe.top/gtspomhupq.html

[J05] 时间加减（加 7 天）
来源：http://hz.nanxuanxn.top/gtyykdyoot.html

Py:   now + timedelta(days=7)
来源：http://hz.tian-w.cn/gtxakjkkfg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shanyushiyangtech.top/gtruqiggwe.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.vqdsnc.cn/gtlfbngkcf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dashuyun.cn/gtifkwhhnz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.redwolf501.top/gtmchebszq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.svipenyu.cn/gtnttoqpgx.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xinyue.icu/gtxofyuwcu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yonumen.top/gtpusicwjv.html

[J06] 计算两时间之差
来源：http://hz.yj202588.top/gtlywcdnsk.html

Py:   (end - start).total_seconds()
来源：http://hz.zhengqikj.top/gthqgiqbgd.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinyuanbaomall.cn/gtooseqmdw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.guannengcc.top/gtuypzhuxi.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.feifeiyinyue.top/gtthoeowig.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yj202588.top/gtgzwxtghj.html

Go:   end.Sub(start).Hours()
来源：http://hz.yanxiufei.cn/gtjgqpdejz.html

Ruby: end - start                 # 返回秒数
来源：http://hz.svipenyu.cn/gtmthzwjmb.html

C#:   (end - start).TotalSeconds
来源：http://hz.jqgfzy.top/gtmbxdeasf.html

[J07] 比较两个日期
来源：http://hz.shzxlz.cn/gtjuvlhxod.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtmkdqktfn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shuidangran.top/gtuetxwumy.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.svipenyu.cn/gtxnbvnmhx.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cqqwz.cn/gtbzbzmkwg.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yuanzhike.top/gtwxyihtpz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.tianlin.xyz/gthguswehe.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ehwqpu.com/gtdxthgetm.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jiagoushi.top/gtthxezslu.html

[J08] 提取年月日与星期
来源：http://hz.zdqjudy.top/gtsqimvbkn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.cqqwz.cn/gtzjsxgqeh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jlsjyb.cn/gttvleeipe.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cheryme.top/gtldzfmxtb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.0kj1m.cn/gteiqgwofu.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.aibaodan.cn/gtiavzorqf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.sweek.top/gtipffexmk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gzhubu.top/gtujqcppva.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.meibo888.top/gtvkduwotu.html

[J09] 时区处理
来源：http://hz.havefunace.top/gterofpfgh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jinqigfzy.top/gtwrlksnls.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.chenlongwang.top/gtlghljgss.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tanke756.top/gtjfuwalot.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guowangkeji.top/gtozezxlob.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.shangyingyoupin.top/gtcmltlpfd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.redwolf501.top/gtldpvnauc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gaohongyu789.top/gtorrcvfis.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.andypj.xyz/gtxwhslktn.html

[J10] 取今天 / 本月第一天
来源：http://hz.gogol.net.cn/gtdwlivowr.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.nwbrower.top/gtaaeeehvv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.pycfn.com/gtmrzafzki.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.feifeiyinyue.top/gtuisxwotl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ppjwa.cn/gtdjvkqpix.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.chenlongwang.top/gtokoquagv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhongyouzk.top/gtldzuhfsd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.dashuyun.cn/gtyxlkivdo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ppjwa.cn/gtspjidesq.html

================================================================================
来源：http://hz.ehwqpu.com/gtsocxgsnz.html

K. JSON 与序列化
来源：http://hz.yongpay.top/gtvrqullmi.html

================================================================================
来源：http://hz.nwbrower.top/gtcrcegwha.html

[K01] 对象转 JSON 字符串
来源：http://hz.nwbrower.top/gtixealjrl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.wangdashe.top/gtowfjsqbl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhengqikj.top/gtvepvrrsk.html

JS:   JSON.stringify(obj)
来源：http://hz.hywenlv.cn/gtymgfcmpq.html

TS:   JSON.stringify(obj)
来源：http://hz.zhiwuduotai.top/gtsejlzipz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jlsjyb.cn/gtazhkpebg.html

Go:   json.Marshal(obj)
来源：http://hz.ywan-chungtsiang.top/gtyidonjqh.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.svipenyu.cn/gtklnuhlzl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.nwbrower.top/gtwfmvuwiy.html

[K02] JSON 字符串转对象
来源：http://hz.feifeiyinyue.top/gttbhzxrqb.html

Py:   json.loads(s)
来源：http://hz.zhijiandao.cn/gtynyauylf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jinqigufen.top/gtfxzinkrq.html

JS:   JSON.parse(s)
来源：http://hz.chenlongwang.top/gthgegqigc.html

TS:   JSON.parse(s)
来源：http://hz.zhaomingkeji.xyz/gtitbnmmya.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gogol.net.cn/gtxmhocaky.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gzhubu.top/gtkbxbhzml.html

Ruby: JSON.parse(s)
来源：http://hz.gotoacloud.top/gtfcmzasts.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.sweek.top/gtnisxdsxb.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jyoumei.cn/gttrbohclt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xingfuxueyuan.xyz/gtaxprrchs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258888.top/gtehzmqpwh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.c1oappe.top/gtwomtfept.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.guannengcc.top/gtvvvnsieu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.fzhhl.top/gteudllyng.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ppjwa.cn/gttautacsn.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yj20258.top/gtycgzsjjy.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.pycfn.com/gtqpuhcoit.html

[K04] 读取 JSON 文件
来源：http://hz.xingfuxueyuan.xyz/gtvknerygn.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xingfuxueyuan.xyz/gteibxlajx.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.hongshengwenyu.top/gtqrxyhmlc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ehwqpu.com/gttvzmossv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.havefunace.top/gtblmxeuko.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.iojbl.cn/gtjvaznrkb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.hysaishi.cn/gtscldvhyx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.tian-w.cn/gtzzkfabgc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sysykeji.top/gtgnalufma.html

[K05] 深拷贝对象
来源：http://hz.daria6918.cn/gtropdstnv.html

Py:   copy.deepcopy(obj)
来源：http://hz.shzxlz.cn/gthoigmpau.html

PHP:  unserialize(serialize($obj));
来源：http://hz.c1oappe.top/gtsibwnnpu.html

JS:   structuredClone(obj)
来源：http://hz.zdqjudy.top/gtrnaakeeq.html

TS:   structuredClone(obj)
来源：http://hz.cashguo.top/gtpjtaddzg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.daxiang520.top/gtkrymlvkc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.nwbrower.top/gtnfegcxkq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jqgfzy.top/gtxdvnjadp.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.jinyuanbaomall.cn/gtbgtlqvwb.html

[K06] 解析 URL 查询串
来源：http://hz.ehwqpu.com/gteuqllbho.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cdnleiting.top/gtpxowqyaq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.gzhubu.top/gtddijsnfz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinqigufen.top/gtfvlxafpd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnqzz.top/gtjrtwezjk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jqgufenzy.top/gtnixujqdg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.daxiang520.top/gtbjfhhjsy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gotoacloud.top/gtrbnfaaqn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.meibo888.top/gtscxkxibl.html

[K07] 进制转换
来源：http://hz.jqgufenzy.top/gtvjkgiwed.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ydzc1.top/gtqprqeodn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tian-w.cn/gtuqtdynmm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gaohongyu789.top/gtsqvwqgtx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.chenjidiqi.icu/gtnsxffhdk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.mhx1999.top/gtrumpgcwg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.0kj1m.cn/gtripcvzdd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.52xcode.cn/gtzbgypxai.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.jqgfzy.top/gtufjnppfz.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.feifeiyinyue.top/gtpiqbgxkg.html

Py:   pickle.dumps(obj)
来源：http://hz.ydzc1.top/gtgywmlewo.html


<!-- 参考信息 -->