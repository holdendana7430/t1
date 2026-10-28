代发 wailian999

JS:   class MyError extends Error {}
来源：http://hz.havefunace.top/gtiiepfgiz.html

TS:   class MyError extends Error {}
来源：http://hz.daxiang520.top/gtqbgkulvh.html

Java: class MyException extends RuntimeException {}
来源：http://hz.tian-w.cn/gtylvemuuy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gaohongyu789.top/gtmhqnjlcj.html

Ruby: class MyError < StandardError; end
来源：http://hz.yj202588.top/gtcfhezrce.html

C#:   class MyException : Exception {}
来源：http://hz.hfpthk.cn/gtayxyqdmg.html

[H05] 捕获特定类型
来源：http://hz.hywenlv.cn/gttmdfonev.html

Py:   except ValueError as e:
来源：http://hz.wangshuangyany.cn/gtyzwrksqr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.fzhhl.top/gtbrsuqxfn.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.vqdsnc.cn/gtgutpygpm.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.redwolf501.top/gtlznbpjpt.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yongpay.top/gtdbfdkwis.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ybcxt.top/gtbledmyzf.html

Ruby: rescue ArgumentError => e
来源：http://hz.nanxuanxn.top/gtqlhabpwq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yvedp.cn/gtqncgvnjf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.guowangkeji.top/gtscocvgyg.html

Py:   value = d.get("k") or default
来源：http://hz.cdnleiting.top/gtnbirhqsw.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sufxvd.cn/gtvvalzszo.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.wangdashe.top/gtgjhpbdvw.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shzxlz.cn/gtpmfgxyij.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.nwbrower.top/gtlibzeows.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.dianchejie.cn/gtodnzatnb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gaohongyu789.top/gtfpgrbtyt.html

C#:   obj?.A?.B ?? default
来源：http://hz.meibo888.top/gthcxrllft.html

[H07] 断言
来源：http://hz.redwolf501.top/gtbgjdxdow.html

Py:   assert x > 0, "必须为正"
来源：http://hz.chenzaomai.com/gtjdfoiijl.html

PHP:  assert($x > 0);
来源：http://hz.52xcode.cn/gtydkwtrle.html

JS:   console.assert(x > 0);
来源：http://hz.yuxming.cn/gtgykilrak.html

TS:   console.assert(x > 0);
来源：http://hz.yj20258.top/gtxtssepfg.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hnqzz.top/gtwapzouap.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hysaishi.cn/gtbqktzjtn.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yonumen.top/gtpnbhrglj.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ydzc1.top/gtyclvzajb.html

[H08] 获取错误信息与堆栈
来源：http://hz.xingfuxueyuan.xyz/gtijwybwwx.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.dianchejie.cn/gtytgcnden.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhoulong.xyz/gtbsfviaej.html

JS:   e.message;  e.stack
来源：http://hz.snrcjt.cn/gtofxcgktw.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yueranfly.top/gtmiikgpzv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ivvv.top/gtrlndkout.html

Go:   err.Error()
来源：http://hz.jiagoushi.top/gtmtbomftl.html

Ruby: e.message;  e.backtrace
来源：http://hz.yuanzhike.top/gtmvzvykkm.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shangyingyoupin.top/gtyutvavmb.html

[H09] 带错误码的异常
来源：http://hz.jinqigufen.top/gttlwyybyq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.daria6918.cn/gtsqrffbzq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cheryme.top/gtohflwtfy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhaomingkeji.xyz/gtonosxdsy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.9152youxi.cn/gtkeadqxwl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zdqjudy.top/gtknwhabgw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.vqdsnc.cn/gtkgyldbnq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yonumen.top/gtpxlswqje.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.meibo888.top/gtregpuccx.html

[H10] 资源自动释放
来源：http://hz.tianlin.xyz/gtbfmguqcn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.aizwys.cn/gtivjxwtzn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.nanxuanxn.top/gtjwoqcgez.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.pycfn.com/gttciehhji.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.daria6918.cn/gterwwnxgp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yvedp.cn/gtlzvggrnw.html

Go:   defer f.Close()
来源：http://hz.c1oappe.top/gtijowrtaw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.c1oappe.top/gtagahisnx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.52xcode.cn/gtyhkncstc.html

================================================================================
来源：http://hz.cqqwz.cn/gtdmktfovz.html

I. 正则表达式
来源：http://hz.jqgfzy.top/gtxuhqyaed.html

================================================================================
来源：http://hz.guannengcc.top/gtjkjmuphm.html

[I01] 判断是否匹配
来源：http://hz.guannengcc.top/gtezsdddmy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.pengpengdd.cyou/gtztllqszq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ywan-chungtsiang.top/gttgcxplzx.html

JS:   /\d+/.test(s)
来源：http://hz.tian-w.cn/gtzmtehecn.html

TS:   /\d+/.test(s)
来源：http://hz.xingfuxueyuan.xyz/gtzynoehnc.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ydzc1.top/gtufbdtdnk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.c1oappe.top/gtjarijarb.html

Ruby: s.match?(/\d+/)
来源：http://hz.shanyushiyangtech.top/gtasgcgijr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shzxlz.cn/gtkbckqrme.html

[I02] 提取所有匹配
来源：http://hz.svipenyu.cn/gtzyhoxnmr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ydjk.org.cn/gtumcktitt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.gaohongyu789.top/gtgvbypsza.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.gzhubu.top/gtahvctfzi.html

TS:   s.match(/\d+/g)
来源：http://hz.zhoulong.xyz/gtqdrjajnd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zdqjudy.top/gtixpisapq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zycfv.cn/gtoqirrkpt.html

Ruby: s.scan(/\d+/)
来源：http://hz.jiagoushi.top/gtzxboownn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.pengpengdd.cyou/gthvyvksmj.html

[I03] 提取捕获分组
来源：http://hz.yonumen.top/gtoatodtva.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.nanxuanxn.top/gtlwjvnnrp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.aibaodan.cn/gtaqkxfxjs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.sweek.top/gtgxbmwztc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.nwbrower.top/gtwkfinpin.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yueranfly.top/gtsuubqibh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhengqikj.top/gtbfthkmgq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.haohaochexian.top/gtziriqrdq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gotoacloud.top/gtbqzvgzuw.html

[I04] 正则替换
来源：http://hz.ppjwa.cn/gtxkesoerp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yuxming.cn/gtkgczhamc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.svipenyu.cn/gtbrwrebpj.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xuanzx.com/gtfbswwphu.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hongshengwenyu.top/gtxvutzrjd.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.haohaochexian.top/gtibyqlvch.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhixingplan.top/gtlduocjyr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shzxlz.cn/gtfppradoj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sysykeji.top/gteoteyodq.html

[I05] 按正则拆分
来源：http://hz.52xcode.cn/gtowhpwsby.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jinqigfzy.top/gtctcgmddn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cashguo.top/gtypyhrohk.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhoulong.xyz/gtceifmbbb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jqgufenzy.top/gtrgqpwklm.html

Java: s.split("\\s*,\\s*")
来源：http://hz.snrcjt.cn/gtscrgytkr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.shanyushiyangtech.top/gtglpmjokl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.quarkkingdee.top/gtsrsvpepd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.chenzaomai.com/gtdahydhbf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.nanxinkj.top/gtqjreyuaw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yuanzhike.top/gtdladzbal.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.gzhubu.top/gtlmlhfufv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nwbrower.top/gtcxumwvfo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.9152youxi.cn/gttzecqkyg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yuxming.cn/gtxwtsckrk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.feifeiyinyue.top/gtgdnwshfd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.snrcjt.cn/gtcpvepfbe.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.meibo888.top/gtcxjpkrae.html

[I07] 忽略大小写与多行模式
来源：http://hz.hongshengwenyu.top/gtfghbeokv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhengqikj.top/gtujqhulyd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.nanxuanxn.top/gtckxcbcvz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhixingplan.top/gtucaaqtdp.html

TS:   /error/gim
来源：http://hz.wangdashe.top/gtvfqedxka.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.0kj1m.cn/gtihmuhbgn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinqigufen.top/gtrjadkeif.html

Ruby: s.scan(/error/i)
来源：http://hz.yuanzhike.top/gtdhvyeyxc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xingfuxueyuan.xyz/gtgdeknbad.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sxryk.cn/gtufkqndqu.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.pycfn.com/gtdjskfrmt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhixingplan.top/gtqfkzaqof.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.bjfxy.top/gtosfludru.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.kuanghao11.cn/gtwcvyqoid.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sysykeji.top/gtvogiyoii.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.daria6918.cn/gtgrzhfnbh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.birdmap.top/gthanmmjen.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jyoumei.cn/gtcbxczljn.html

================================================================================
来源：http://hz.cucudq.cn/gttlkgazkg.html

J. 日期与时间
来源：http://hz.dashuyun.cn/gtzyceehre.html

================================================================================
来源：http://hz.yuanzhike.top/gtmileumkm.html

[J01] 获取当前时间
来源：http://hz.nwbrower.top/gtoxzoiite.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhixingplan.top/gtkurvhytn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.pycfn.com/gtmnghwvkw.html

JS:   new Date();  Date.now()
来源：http://hz.ppjwa.cn/gtlmfzwcli.html

TS:   new Date();  Date.now()
来源：http://hz.c1oappe.top/gtkdkzhqke.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.dashuyun.cn/gtnyzklydw.html

Go:   time.Now()
来源：http://hz.xinyue.icu/gtmkswomfl.html

Ruby: Time.now
来源：http://hz.cashguo.top/gtmumotpwr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.aibaodan.cn/gtrevcjewc.html

[J02] 格式化输出
来源：http://hz.tian-w.cn/gtypxytgzf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nwbrower.top/gtxazabols.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.nanxuanxn.top/gtumflhptq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jinqigfzy.top/gtdauckbkh.html

TS:   d.toISOString()
来源：http://hz.52xcode.cn/gtgyasffrm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yuxming.cn/gtmzulkmhw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jqgufenzy.top/gtxuvuxdbm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jlsjyb.cn/gtnutwprsr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shzxlz.cn/gtcghvvaak.html

[J03] 字符串解析为日期
来源：http://hz.hongshengwenyu.top/gtquwbvcyd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yuxming.cn/gtfxbwzegf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jqgufenzy.top/gtadbgzxpj.html

JS:   new Date("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtrshmbatj.html

TS:   new Date("2024-01-02")
来源：http://hz.jinqigufen.top/gtzsejkmjs.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.daxiang520.top/gtfodmxxzl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yangfankeji.com/gtdxomaxnx.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.quarkkingdee.top/gtazbdqxol.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.chenzaomai.com/gtslkqafdx.html

[J04] 时间戳与日期互转
来源：http://hz.xinyue.icu/gtesgvsqjw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ybcxt.top/gtrhijczxr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ydjk.org.cn/gtqdhzqmgj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.chenjidiqi.icu/gtruxjqwht.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yuanzhike.top/gtotqgggqe.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yj20258888.top/gtzywpeagn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hnxiangtu.top/gtgtafxfpn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zycfv.cn/gtidzfuuoi.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.52xcode.cn/gtlzfvreed.html

[J05] 时间加减（加 7 天）
来源：http://hz.shuidangran.top/gtiemrruac.html

Py:   now + timedelta(days=7)
来源：http://hz.yuanzhike.top/gtshrlnsyv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.guowangkeji.top/gtjgsasgep.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cheryme.top/gtlbcyiptk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tian-w.cn/gtktcqolyy.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.chenlongwang.top/gtroomkcmh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.gotoacloud.top/gtdjufyjkn.html

Ruby: Time.now + 7 * 86400
来源：http://hz.chenjidiqi.icu/gttrmnirhe.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.nanxuanxn.top/gtkbgicpub.html

[J06] 计算两时间之差
来源：http://hz.ybcxt.top/gtevmzfwiu.html

Py:   (end - start).total_seconds()
来源：http://hz.tianlin.xyz/gtdxiisuht.html

PHP:  $end->diff($start)->days;
来源：http://hz.shuidangran.top/gtdhqfbvqc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.quarkkingdee.top/gtgkxbvyxl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yvedp.cn/gteaqxggvd.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hnqzz.top/gtdlgowrzt.html

Go:   end.Sub(start).Hours()
来源：http://hz.yonumen.top/gtoololhft.html

Ruby: end - start                 # 返回秒数
来源：http://hz.wangshuangyany.cn/gtkwkdmzim.html

C#:   (end - start).TotalSeconds
来源：http://hz.dianchejie.cn/gtiyytdxpq.html

[J07] 比较两个日期
来源：http://hz.kuanghao11.cn/gtftxrhvat.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.sysykeji.top/gtaqlwomli.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.iojbl.cn/gtmshvdeei.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.aibaodan.cn/gtquwpqmcu.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yuxming.cn/gtlufiwcyl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xingfuxueyuan.xyz/gtineznyyk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.snrcjt.cn/gtkqlvktwk.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hnxiangtu.top/gtzaxkrynj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhixingplan.top/gttyqdzwvz.html

[J08] 提取年月日与星期
来源：http://hz.zhijiandao.cn/gtqllnaldp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xingfuxueyuan.xyz/gtokxpmfjk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhijiandao.cn/gtjpnxvuuw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.9152youxi.cn/gtjmjxgaif.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.guowangkeji.top/gtpefslqud.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yj202588.top/gtehyyuzzz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.9152youxi.cn/gtofftrasb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhengqikj.top/gtfwdvhhqx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sweek.top/gtyjrelyem.html

[J09] 时区处理
来源：http://hz.ydjk.org.cn/gteyxplsmp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cucudq.cn/gtdltusssp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.tanke756.top/gtsydwkpfk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hnxiangtu.top/gtlyunybvd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhaomingkeji.xyz/gtjrdmbrdm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.dianchejie.cn/gtbhjlwbnl.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.tianlin.xyz/gtqltzcani.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.sxryk.cn/gtgdwbilty.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.mhx1999.top/gtkwmqjikg.html

[J10] 取今天 / 本月第一天
来源：http://hz.shzxlz.cn/gtqysxhlvl.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.wangdashe.top/gtzzyjpszs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.birdmap.top/gtlgcuqktw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.vqdsnc.cn/gtxsukdxwm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.guannengcc.top/gtpctiydkc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xylfe.cn/gthtpgzsnd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shanyushiyangkeji.top/gtwghopqlg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.nwbrower.top/gtuagojcad.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.meibo888.top/gtpvcvwlxz.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtyyuawaiv.html

K. JSON 与序列化
来源：http://hz.gaohongyu789.top/gtvaabciew.html

================================================================================
来源：http://hz.vqdsnc.cn/gtxhjsbszr.html

[K01] 对象转 JSON 字符串
来源：http://hz.gogol.net.cn/gtqzxkjypq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cashguo.top/gtbjpdndht.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.0kj1m.cn/gtcbdeasst.html

JS:   JSON.stringify(obj)
来源：http://hz.andypj.xyz/gtwlpkpkrz.html

TS:   JSON.stringify(obj)
来源：http://hz.hammf.cn/gtgqwrfqes.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.fzhhl.top/gtngvcrzpv.html

Go:   json.Marshal(obj)
来源：http://hz.hnqzz.top/gtwtjcwrko.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yonumen.top/gtpetcvune.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ehwqpu.com/gtpwdrjlsp.html

[K02] JSON 字符串转对象
来源：http://hz.ivvv.top/gtjqkoeaba.html

Py:   json.loads(s)
来源：http://hz.ivvv.top/gtnjitbaaz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.snrcjt.cn/gtxdthdjkv.html

JS:   JSON.parse(s)
来源：http://hz.xinyue.icu/gtzlkgorgy.html

TS:   JSON.parse(s)
来源：http://hz.zdqjudy.top/gthpkoqxkj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.fengsongda.top/gtyljxpmon.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cucudq.cn/gtlhwibfgj.html

Ruby: JSON.parse(s)
来源：http://hz.birdmap.top/gtlcfnkgxt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xuanzx.com/gtvupqkulh.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.shzxlz.cn/gtbluqkytz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shanyushiyangtech.top/gteezvebrj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shangyingyoupin.top/gtsynkbrqy.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.kuanghao11.cn/gtdsskchvi.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yanxiufei.cn/gtpkmylazd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cashguo.top/gtgtavezzt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.havefunace.top/gtojxwboip.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ybcxt.top/gtriamlpgl.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hnxiangtu.top/gtwgojkvnn.html

[K04] 读取 JSON 文件
来源：http://hz.gaohongyu789.top/gtmukvaxqb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jyoumei.cn/gtlhvotull.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.316326.xyz/gtyjupjfig.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yonumen.top/gtekddtllq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gaohongyu789.top/gtkncymtjk.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.bjfxy.top/gtpznbrdjg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yj20258.top/gtniatsjqj.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yj20258.top/gtkxicubsg.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shuidangran.top/gtuiwlvfni.html

[K05] 深拷贝对象
来源：http://hz.cqqwz.cn/gtaqinksbt.html

Py:   copy.deepcopy(obj)
来源：http://hz.sufxvd.cn/gtoutkvatc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.gzhubu.top/gtrrhovpzv.html

JS:   structuredClone(obj)
来源：http://hz.ppjwa.cn/gtctuwpkxx.html

TS:   structuredClone(obj)
来源：http://hz.zhijiandao.cn/gtmpefmbpm.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.hfpthk.cn/gtgsvuebgh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.jinghuilouyu.cn/gtytxrltro.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.zhiwuduotai.top/gtrzbliiua.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.feifeiyinyue.top/gtfgchilra.html

[K06] 解析 URL 查询串
来源：http://hz.meibo888.top/gthxrfrgsm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.mhx1999.top/gtltepcntl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.sysykeji.top/gtuazthuuc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ywan-chungtsiang.top/gtdvwvjdjq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.c1oappe.top/gtezskahtu.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.smart0.xyz/gtsiusevgc.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gotoacloud.top/gtokfllzxk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.dianchejie.cn/gtawgqrffn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.meibo888.top/gtxvdzyifq.html

[K07] 进制转换
来源：http://hz.ybcxt.top/gtmiqoiwxu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.guannengcc.top/gtvkxrprry.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tanke756.top/gtlmrrfvtw.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yuanzhike.top/gtuvytusyc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.zhixingplan.top/gtixdmuogc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.fengsongda.top/gtlfrivpop.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.gaohongyu789.top/gtoctinesf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.ybcxt.top/gtdqajncul.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.316326.xyz/gtzloirube.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.ywan-chungtsiang.top/gthfbeqqqt.html

Py:   pickle.dumps(obj)
来源：http://hz.c1oappe.top/gtydpmaafb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.kuanghao11.cn/gtfdzlrpei.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.feifeiyinyue.top/gtkiapjhbl.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.feifeiyinyue.top/gtcccjvljx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenjidiqi.icu/gthjvixuhb.html


<!-- 参考信息 -->