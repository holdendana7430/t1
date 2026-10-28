代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yueranfly.top/gtvzpeiahy.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.svipenyu.cn/gtfyjoviof.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhiwuduotai.top/gtjivdbcfg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xinyue.icu/gthtmndwff.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jinghuilouyu.cn/gteprwjsij.html

Ruby: rescue ArgumentError => e
来源：http://hz.cheryme.top/gtwrojpuor.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.shanyushiyangtech.top/gtysqztwui.html

[H06] 可选值 / 空值安全访问
来源：http://hz.chenlongwang.top/gtusoicxtv.html

Py:   value = d.get("k") or default
来源：http://hz.dashuyun.cn/gtrpcubpoi.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhiwuduotai.top/gtlpafauan.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yangfankeji.com/gtiijlmpii.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.feifeiyinyue.top/gtndgvcsjx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.nwbrower.top/gtcyrbqwio.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhijiandao.cn/gtvfwanota.html

Ruby: d&.dig(:a, :b)
来源：http://hz.316326.xyz/gtdzlsnrhg.html

C#:   obj?.A?.B ?? default
来源：http://hz.sysykeji.top/gtovsdzoij.html

[H07] 断言
来源：http://hz.shanyushiyangkeji.top/gtnkgcimzr.html

Py:   assert x > 0, "必须为正"
来源：http://hz.nwbrower.top/gtzacriezc.html

PHP:  assert($x > 0);
来源：http://hz.shanyushiyangkeji.top/gtfvtxggqq.html

JS:   console.assert(x > 0);
来源：http://hz.zycfv.cn/gtfhbngozg.html

TS:   console.assert(x > 0);
来源：http://hz.hfpthk.cn/gtkwmhwtvo.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hywenlv.cn/gtycajqbjl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.fengsongda.top/gtoqtalisa.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hammf.cn/gttxgoxsvy.html

C#:   Debug.Assert(x > 0);
来源：http://hz.tianlin.xyz/gtbxkxpoby.html

[H08] 获取错误信息与堆栈
来源：http://hz.xylfe.cn/gtyaxtrftc.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cashguo.top/gtajxdigfj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xingfuxueyuan.xyz/gttlknhlai.html

JS:   e.message;  e.stack
来源：http://hz.cashguo.top/gtixkjrmfr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.kuanghao11.cn/gtxfkjyqyg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gaohongyu789.top/gtshhbjljl.html

Go:   err.Error()
来源：http://hz.sxryk.cn/gtfstkrpro.html

Ruby: e.message;  e.backtrace
来源：http://hz.gotoacloud.top/gtztvdabeb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhoulong.xyz/gtuiamuaco.html

[H09] 带错误码的异常
来源：http://hz.yueranfly.top/gtetdfkykf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xingfuxueyuan.xyz/gtcenuurjw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.pycfn.com/gtguwmsmkq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.aizwys.cn/gttvgtzfib.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinyuanbaomall.cn/gtjqlbjvmf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.smart0.xyz/gtfgqeeffo.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sxryk.cn/gtsozkuypj.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.0kj1m.cn/gtusbdlncz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zdqjudy.top/gtonmxveos.html

[H10] 资源自动释放
来源：http://hz.mhx1999.top/gtdbfwuvor.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.iojbl.cn/gtqmshfeot.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ydzc1.top/gtdodlkwnw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hnxiangtu.top/gtyrwdqnsj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.daria6918.cn/gtoeeaxccn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.chenjidiqi.icu/gtkqksplka.html

Go:   defer f.Close()
来源：http://hz.yuxming.cn/gtkkxwifoh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ydjk.org.cn/gtmvsyfzaz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hnxiangtu.top/gtzglvdfor.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtyebznuxb.html

I. 正则表达式
来源：http://hz.pycfn.com/gtacolgzod.html

================================================================================
来源：http://hz.andypj.xyz/gtqhfmkkib.html

[I01] 判断是否匹配
来源：http://hz.zhixingplan.top/gttyqqkjox.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.nanxinkj.top/gtroldpcbh.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinyuanbaomall.cn/gtjnhofsxj.html

JS:   /\d+/.test(s)
来源：http://hz.xingfuxueyuan.xyz/gtnukfmyhg.html

TS:   /\d+/.test(s)
来源：http://hz.gzhubu.top/gtyhzuyeee.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhaomingkeji.xyz/gthfdvahrc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.haohaochexian.top/gtabejewkt.html

Ruby: s.match?(/\d+/)
来源：http://hz.hnxiangtu.top/gtdyikdcsz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xziqi.cn/gtuchfyttb.html

[I02] 提取所有匹配
来源：http://hz.birdmap.top/gtypkgitfp.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yangfankeji.com/gtpjtpbpva.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhixingplan.top/gtrhmnltqr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.tanke756.top/gtagkwaawl.html

TS:   s.match(/\d+/g)
来源：http://hz.zhongyouzk.top/gtrddqzalo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xylfe.cn/gtcdjxnscd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.chenlongwang.top/gtianydcts.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhongyouzk.top/gteejsyqfc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yangfankeji.com/gtxdurzvwg.html

[I03] 提取捕获分组
来源：http://hz.xziqi.cn/gtefsrqsqx.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ybcxt.top/gthwvxdmbl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jinqigfzy.top/gtcuchygrl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jqgufenzy.top/gtdlpzfzrk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.pengpengdd.cyou/gtnrjxxljk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jinqigfzy.top/gtczhmcslu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhoulong.xyz/gtovhosrya.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.nanxuanxn.top/gtdclrodfs.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yvedp.cn/gtzhxbmwga.html

[I04] 正则替换
来源：http://hz.jlsjyb.cn/gtdlxtiwye.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.sysykeji.top/gtojqcdinf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jianghu66.top/gtusafeejt.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gotoacloud.top/gtqmjuejfi.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.haohaochexian.top/gtjxdrifia.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.guowangkeji.top/gtgaaahjmn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.dianchejie.cn/gtafjkfqro.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.quarkkingdee.top/gtuvytsczu.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.0kj1m.cn/gtjcehxlqu.html

[I05] 按正则拆分
来源：http://hz.gzhubu.top/gtbfypgqsl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shanyushiyangkeji.top/gtpvdxexxo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yuxming.cn/gtmcyjpwme.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ywan-chungtsiang.top/gttreeazao.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.havefunace.top/gtoxmvsswn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.guowangkeji.top/gtufltevkh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.nanxinkj.top/gtgvdsvvdx.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jianghu66.top/gtoshdbozb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.aibaodan.cn/gtxgacbccx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jianghu66.top/gtchitmtpe.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yj202588.top/gtcpbdglnx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.feifeiyinyue.top/gtknnjyufu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgufenzy.top/gtnpmbilas.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgufenzy.top/gtftkxtkko.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ivvv.top/gtjmchocsl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yj20258888.top/gttqkcpikt.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.iojbl.cn/gtmwsiwuij.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.pycfn.com/gtumtkichk.html

[I07] 忽略大小写与多行模式
来源：http://hz.sysykeji.top/gtxvbfyrtc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yj202588.top/gtgresnlaf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.aizwys.cn/gtqdtvbtrv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ybcxt.top/gtrwncjyed.html

TS:   /error/gim
来源：http://hz.bjfxy.top/gtbxxgruqn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sufxvd.cn/gtuycvafxh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cqqwz.cn/gthssrlhss.html

Ruby: s.scan(/error/i)
来源：http://hz.xuetiantiany.cn/gtmixwcpzd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.nanxinkj.top/gtdljwbfcd.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cashguo.top/gtshhdbvdz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.andypj.xyz/gtyjqwhxph.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.sysykeji.top/gtpiynevsa.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nwbrower.top/gtriquldxb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hfpthk.cn/gtqylgrdez.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.daxiang520.top/gtqgzzzxxk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shanyushiyangkeji.top/gtoghfpevi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jinghuilouyu.cn/gtzftzvpuv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zdqjudy.top/gtwtavmzxl.html

================================================================================
来源：http://hz.chenzaomai.com/gtuukfrxzk.html

J. 日期与时间
来源：http://hz.haohaochexian.top/gtkzmefjey.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtunubyvbq.html

[J01] 获取当前时间
来源：http://hz.shangyingyoupin.top/gtbvmtpnjq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.fzhhl.top/gtvvyooibv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ywan-chungtsiang.top/gtwpbtehgx.html

JS:   new Date();  Date.now()
来源：http://hz.wangdashe.top/gtknokfgda.html

TS:   new Date();  Date.now()
来源：http://hz.svipenyu.cn/gthrltnuvg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yuxming.cn/gtuspuhbvx.html

Go:   time.Now()
来源：http://hz.jiagoushi.top/gtblzkhabx.html

Ruby: Time.now
来源：http://hz.kuanghao11.cn/gtxvagcglb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.fengsongda.top/gtmpibefnp.html

[J02] 格式化输出
来源：http://hz.0kj1m.cn/gtxwinlyrj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangdashe.top/gtlugnrfvd.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.nwbrower.top/gtbcasvtsn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.52xcode.cn/gtwhjkllwe.html

TS:   d.toISOString()
来源：http://hz.smart0.xyz/gtajyvphns.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.nwbrower.top/gtqvuexcxi.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.nwbrower.top/gtcolwddff.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ivvv.top/gtmidhrbns.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.tanke756.top/gtljzzyjrz.html

[J03] 字符串解析为日期
来源：http://hz.zhongyouzk.top/gtyhpwjbhz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jqgfzy.top/gtddwcxvbr.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ybcxt.top/gtvpjqagjx.html

JS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtqwsgdjjv.html

TS:   new Date("2024-01-02")
来源：http://hz.52xcode.cn/gtgxxjtmnk.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yvedp.cn/gtpzcejiex.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yanxiufei.cn/gtceiftbim.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtyeksnyoo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.gogol.net.cn/gtlfdxqnmv.html

[J04] 时间戳与日期互转
来源：http://hz.guannengcc.top/gtsrieilrw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinghuilouyu.cn/gtljwzxcia.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhixingplan.top/gtpzwzqgsw.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.c1oappe.top/gtdgzaqdvf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.havefunace.top/gtudcqzqgl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ydjk.org.cn/gtggapwcyl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xingfuxueyuan.xyz/gtjdwpszmp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.kuanghao11.cn/gtypmroleb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.tianlin.xyz/gtilhjpzgg.html

[J05] 时间加减（加 7 天）
来源：http://hz.yanxiufei.cn/gtfinwccwk.html

Py:   now + timedelta(days=7)
来源：http://hz.yj20258888.top/gtdzggkrho.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.chenlongwang.top/gtugucndgi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.birdmap.top/gtvxzbxyzx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sufxvd.cn/gtcyegrups.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yongpay.top/gtbzoeteli.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.vqdsnc.cn/gtljmpqoeo.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hammf.cn/gtostsidku.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jqgufenzy.top/gtxjzvqyii.html

[J06] 计算两时间之差
来源：http://hz.jianghu66.top/gtxhfgopxh.html

Py:   (end - start).total_seconds()
来源：http://hz.yonumen.top/gtyajtsnpp.html

PHP:  $end->diff($start)->days;
来源：http://hz.daria6918.cn/gtfepwgzbj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhiwuduotai.top/gtdoflzust.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.chenjidiqi.icu/gtpepjbxpm.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hywenlv.cn/gtapveqkry.html

Go:   end.Sub(start).Hours()
来源：http://hz.birdmap.top/gtliuqjyof.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shuidangran.top/gtxwyzbnup.html

C#:   (end - start).TotalSeconds
来源：http://hz.316326.xyz/gtpfjorvlx.html

[J07] 比较两个日期
来源：http://hz.xziqi.cn/gtdbvjciql.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.dianchejie.cn/gtrdyracwz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.bjfxy.top/gtzbtcmewe.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.svipenyu.cn/gtyxazbkbl.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gotoacloud.top/gteombwdcl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.sxryk.cn/gthidtfrzw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jqgfzy.top/gtbnxchrmh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.fzhhl.top/gthxflwtza.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gtpkjkxvcw.html

[J08] 提取年月日与星期
来源：http://hz.hywenlv.cn/gtrfeuxpvq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.chenzaomai.com/gthbtahwgh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.chenlongwang.top/gtqennqimv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jlsjyb.cn/gtgmifwaff.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ydzc1.top/gtkjvxvclx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.birdmap.top/gtztojbslh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hysaishi.cn/gtrdaklguv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cdnleiting.top/gtbwnncvdu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.bjfxy.top/gtkcamaeix.html

[J09] 时区处理
来源：http://hz.yj202588.top/gtdpedjynr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yvedp.cn/gthmqahvon.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhiwuduotai.top/gtcfdyhirc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ehwqpu.com/gtfepvfjch.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.fzhhl.top/gtilqptpmm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.svipenyu.cn/gtszjqjttp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.daria6918.cn/gtmtseyasy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.dianchejie.cn/gtwixbtmvx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.gaohongyu789.top/gtzzmpnzcq.html

[J10] 取今天 / 本月第一天
来源：http://hz.316326.xyz/gtounfliew.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shzxlz.cn/gtludgvuhe.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.316326.xyz/gtwnqywqpp.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.redwolf501.top/gtdgflfzhl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yj20258.top/gtzbjyvwye.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hnxiangtu.top/gtfletjftk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.pengpengdd.cyou/gtpxluwerl.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.iojbl.cn/gtfunqdkhw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.iojbl.cn/gtdulgeqfn.html

================================================================================
来源：http://hz.zdqjudy.top/gtpawlgmmh.html

K. JSON 与序列化
来源：http://hz.mhx1999.top/gtywfqqcgy.html

================================================================================
来源：http://hz.daxiang520.top/gtykllptmd.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhengqikj.top/gtlgychckv.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xingfuxueyuan.xyz/gtowzyedzk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jianghu66.top/gtvamwudce.html

JS:   JSON.stringify(obj)
来源：http://hz.cashguo.top/gtxyrslhbr.html

TS:   JSON.stringify(obj)
来源：http://hz.tian-w.cn/gtfpqmirsg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yanxiufei.cn/gtdapijvsf.html

Go:   json.Marshal(obj)
来源：http://hz.jinyuanbaomall.cn/gtcapkbtkq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.redwolf501.top/gtphduqvwr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hammf.cn/gtxiekwfwz.html

[K02] JSON 字符串转对象
来源：http://hz.52xcode.cn/gtduwmcwpp.html

Py:   json.loads(s)
来源：http://hz.0kj1m.cn/gtpgxcbmxd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hysaishi.cn/gtdqujyfiq.html

JS:   JSON.parse(s)
来源：http://hz.vqdsnc.cn/gtdkuobfpo.html

TS:   JSON.parse(s)
来源：http://hz.jlsjyb.cn/gtsulyunbd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yongpay.top/gtwmcjkuni.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yangfankeji.com/gtwutriirq.html

Ruby: JSON.parse(s)
来源：http://hz.nanxinkj.top/gtdenzylkb.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.tian-w.cn/gteaxvcxhn.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.nanxuanxn.top/gtcvailxel.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hfpthk.cn/gtomnzkcfg.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gzhubu.top/gtcifabmsi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.aizwys.cn/gtkidznske.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangshuangyany.cn/gtuarnsaix.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hnqzz.top/gtscauvnuu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yuanzhike.top/gtvlczoudt.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sufxvd.cn/gttiwpvijh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.guowangkeji.top/gtkidfnypa.html

[K04] 读取 JSON 文件
来源：http://hz.ywan-chungtsiang.top/gtmckxdjmk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yongpay.top/gtuznbkvgn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ybcxt.top/gtqogoyttp.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.bjfxy.top/gtkjydnzpu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gzhubu.top/gtmymgquzs.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ppjwa.cn/gtmzigctwb.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.52xcode.cn/gtxfqkcitf.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.feifeiyinyue.top/gtjjvcljuo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sysykeji.top/gtjpbjwqfd.html

[K05] 深拷贝对象
来源：http://hz.aibaodan.cn/gtijmsfrwm.html

Py:   copy.deepcopy(obj)
来源：http://hz.zhongyouzk.top/gtukxwnmmy.html

PHP:  unserialize(serialize($obj));
来源：http://hz.zhengqikj.top/gttghllycm.html

JS:   structuredClone(obj)
来源：http://hz.gaohongyu789.top/gtqtzuzsjz.html

TS:   structuredClone(obj)
来源：http://hz.ybcxt.top/gtxmkgkezk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.redwolf501.top/gtsqfiqmiu.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hysaishi.cn/gtflasjfne.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.c1oappe.top/gtogjoweaj.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.gogol.net.cn/gtqwcrlqpz.html

[K06] 解析 URL 查询串
来源：http://hz.yuanzhike.top/gtgemvcund.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.redwolf501.top/gtimphsyrz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yj202588.top/gtqjxzychi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jyoumei.cn/gtfjyfkqev.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhongyouzk.top/gtizizskuh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yj202588.top/gthtbgqowu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.feifeiyinyue.top/gtshqpearz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.nwbrower.top/gtvhzzfzcy.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.nanxinkj.top/gtnrjpzrqx.html

[K07] 进制转换
来源：http://hz.zhixingplan.top/gtqnvhtrbm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xuetiantiany.cn/gtreaeqbpt.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.0kj1m.cn/gtdejfpwyd.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.zhaomingkeji.xyz/gtkuytygvl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.cheryme.top/gtgqbcjiez.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.birdmap.top/gtkirlbdlk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.zhoulong.xyz/gtdutehetw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.tanke756.top/gtagveqnue.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hywenlv.cn/gtdjponvia.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.cdnleiting.top/gtghdpttdf.html

Py:   pickle.dumps(obj)
来源：http://hz.yj20258.top/gtzfqsyivq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yj20258888.top/gtdrpipbzx.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.zhongyouzk.top/gtzbcpgchm.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.tianlin.xyz/gtwjlvpcsx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.dashuyun.cn/gtwinlktyw.html

Go:   encoding/gob
来源：http://hz.hfpthk.cn/gthjiplqss.html

Ruby: Marshal.dump(obj)
来源：http://hz.yuxming.cn/gtxzioypua.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.xziqi.cn/gtcxxehjwy.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtnurvqluq.html

L. 网络请求
来源：http://hz.chenlongwang.top/gtvgithvak.html

================================================================================
来源：http://hz.xziqi.cn/gtoghkjwgc.html

[L01] 发送 GET 请求
来源：http://hz.shangyingyoupin.top/gtrgsujqqj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.zhiwuduotai.top/gtlggkhsxz.html


<!-- 参考信息 -->