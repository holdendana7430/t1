代发 wailian999

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.chenlongwang.top/gtdxabsbro.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xingfuxueyuan.xyz/gttoatlutb.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhongyouzk.top/gtipeflnld.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.9152youxi.cn/gtlemjdnog.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhijiandao.cn/gthsfihley.html

Ruby: rescue ArgumentError => e
来源：http://hz.zycfv.cn/gtepwuodrn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ydjk.org.cn/gtnnhjgeaw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jinghuilouyu.cn/gtwfskcxig.html

Py:   value = d.get("k") or default
来源：http://hz.shangyingyoupin.top/gtrlrnampv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hongshengwenyu.top/gtwwikjlbj.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.iojbl.cn/gtsorycguu.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.quarkkingdee.top/gtbvqbepim.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.aizwys.cn/gtzmyrqrsb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.9152youxi.cn/gtpnqhfytf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gaohongyu789.top/gthmerafcz.html

C#:   obj?.A?.B ?? default
来源：http://hz.yongpay.top/gtmebnwrkm.html

[H07] 断言
来源：http://hz.zhaomingkeji.xyz/gtkqrgkkcb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.52xcode.cn/gtrsrsssvx.html

PHP:  assert($x > 0);
来源：http://hz.daria6918.cn/gtajaqxsmx.html

JS:   console.assert(x > 0);
来源：http://hz.daxiang520.top/gtjgtednir.html

TS:   console.assert(x > 0);
来源：http://hz.svipenyu.cn/gtxsvkvovg.html

Java: assert x > 0 : "必须为正";
来源：http://hz.snrcjt.cn/gtmbmjvkkz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gaohongyu789.top/gtejnnxvlp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yj202588.top/gtahusabjz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.smart0.xyz/gtvsxlhkue.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhiwuduotai.top/gtkwcovqan.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jyoumei.cn/gtsyodvwjk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.nanxinkj.top/gtjgddpkch.html

JS:   e.message;  e.stack
来源：http://hz.xingfuxueyuan.xyz/gthhwtgkta.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yongpay.top/gtszchgnyo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yongpay.top/gtwewermbr.html

Go:   err.Error()
来源：http://hz.jinyuanbaomall.cn/gtagcwpgrj.html

Ruby: e.message;  e.backtrace
来源：http://hz.bjfxy.top/gtnesdasmr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shanyushiyangkeji.top/gtrwzilwrx.html

[H09] 带错误码的异常
来源：http://hz.dianchejie.cn/gtznuzkgqf.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.snrcjt.cn/gtzxjzxivs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yueranfly.top/gtasyrvpxf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cashguo.top/gtdcxvtpbf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.feifeiyinyue.top/gtbedlgwne.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cucudq.cn/gtmsypflru.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hywenlv.cn/gtpkjuxznk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.fzhhl.top/gteeobnitv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.snrcjt.cn/gtgtzfktel.html

[H10] 资源自动释放
来源：http://hz.hammf.cn/gtygnzdjoh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhiwuduotai.top/gtthpvjkey.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xziqi.cn/gtsdipjtpm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuxming.cn/gthzsiwrcy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangkeji.top/gtbuigszxg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.shanyushiyangkeji.top/gthfgjboie.html

Go:   defer f.Close()
来源：http://hz.ppjwa.cn/gtazrayltv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.meibo888.top/gtvfyaqadl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtyfdszjuy.html

================================================================================
来源：http://hz.xylfe.cn/gtnuxvajju.html

I. 正则表达式
来源：http://hz.cheryme.top/gtlfaaaupe.html

================================================================================
来源：http://hz.ydjk.org.cn/gtbyetcsle.html

[I01] 判断是否匹配
来源：http://hz.0kj1m.cn/gttfygkysj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hywenlv.cn/gtejciaonc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.aibaodan.cn/gtbawknasx.html

JS:   /\d+/.test(s)
来源：http://hz.quarkkingdee.top/gtudlrewbh.html

TS:   /\d+/.test(s)
来源：http://hz.haohaochexian.top/gtdjlyssnm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.snrcjt.cn/gtwjwfmnqv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.meibo888.top/gttzaynjjt.html

Ruby: s.match?(/\d+/)
来源：http://hz.9152youxi.cn/gtyoamdgft.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xingfuxueyuan.xyz/gttmojacff.html

[I02] 提取所有匹配
来源：http://hz.tianlin.xyz/gtxjhuhewa.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jlsjyb.cn/gtjnxkvbev.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj20258888.top/gtwhplucnm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shanyushiyangkeji.top/gtvrlqwsyg.html

TS:   s.match(/\d+/g)
来源：http://hz.fzhhl.top/gtncjepqeb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yonumen.top/gtvfhpfqfz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinqigufen.top/gtfjshfwyi.html

Ruby: s.scan(/\d+/)
来源：http://hz.cheryme.top/gtskiifkdg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jinqigufen.top/gtdnnmorut.html

[I03] 提取捕获分组
来源：http://hz.nanxinkj.top/gtekzssbhb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.chenzaomai.com/gtprmowplp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.svipenyu.cn/gtjzwtknyw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj20258.top/gtfgsaexqx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.snrcjt.cn/gtplaxunku.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xylfe.cn/gtrewzfvsf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cashguo.top/gtxtlthnjj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shanyushiyangtech.top/gtqtstdalk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.daria6918.cn/gtwjaqvawb.html

[I04] 正则替换
来源：http://hz.havefunace.top/gtmvjwoumh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinqigfzy.top/gtglolhwbz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.daxiang520.top/gtmgayxyzy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.haohaochexian.top/gtsblxvesn.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.svipenyu.cn/gtyuuufifa.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinqigfzy.top/gtmycpzeee.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhaomingkeji.xyz/gtthfpflie.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhaomingkeji.xyz/gtdrhfsadb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hnqzz.top/gtllpvptkk.html

[I05] 按正则拆分
来源：http://hz.jinqigufen.top/gtlhrgpgei.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xuanzx.com/gthercpehj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinghuilouyu.cn/gtjdzarwdz.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ydjk.org.cn/gtyxetirwh.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hnxiangtu.top/gtejidoxix.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yvedp.cn/gtpzgzpvms.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ywan-chungtsiang.top/gtenbiyelg.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhixingplan.top/gtbztyaian.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xinyue.icu/gtcuykxtja.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xylfe.cn/gttlezoajp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.feifeiyinyue.top/gtpjwpjgzf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hfpthk.cn/gtjulmyjqp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yanxiufei.cn/gtgmkhefox.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.snrcjt.cn/gtybibmajl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.redwolf501.top/gtjccyvsue.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ehwqpu.com/gtjkwytdac.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xziqi.cn/gtrwwbnlnq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.316326.xyz/gtcqewngpq.html

[I07] 忽略大小写与多行模式
来源：http://hz.dashuyun.cn/gtvrcvebhf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.sufxvd.cn/gtowsdzzof.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.shangyingyoupin.top/gtmipovclt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ybcxt.top/gtdemsdasj.html

TS:   /error/gim
来源：http://hz.jyoumei.cn/gtltpkohxg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jiagoushi.top/gtpubanuzy.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jyoumei.cn/gtgdpobykf.html

Ruby: s.scan(/error/i)
来源：http://hz.chenlongwang.top/gtkyzvbhjs.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.aizwys.cn/gtbiejlplf.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.0kj1m.cn/gtyhvqjylp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.bjfxy.top/gtciwrdhxj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xuanzx.com/gtftbsakxt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yvedp.cn/gtvjczjvnt.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangkeji.top/gttmyphdei.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.tian-w.cn/gteufphjnl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinqigfzy.top/gtkxehjuig.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.birdmap.top/gtqouimyah.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhongyouzk.top/gthaabxemw.html

================================================================================
来源：http://hz.snrcjt.cn/gtedzuttpj.html

J. 日期与时间
来源：http://hz.smart0.xyz/gtogmewxgj.html

================================================================================
来源：http://hz.316326.xyz/gtmxtdzjvm.html

[J01] 获取当前时间
来源：http://hz.birdmap.top/gtcuhklokk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ehwqpu.com/gtachmdtvv.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cheryme.top/gtpbaemlpr.html

JS:   new Date();  Date.now()
来源：http://hz.redwolf501.top/gtamvzovbf.html

TS:   new Date();  Date.now()
来源：http://hz.cheryme.top/gtuxorydfz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.sysykeji.top/gtwdgsmkai.html

Go:   time.Now()
来源：http://hz.cashguo.top/gtswsdktan.html

Ruby: Time.now
来源：http://hz.shanyushiyangtech.top/gtvpleucwy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.svipenyu.cn/gtjtsbgqvk.html

[J02] 格式化输出
来源：http://hz.zdqjudy.top/gtzmmrwrzh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ivvv.top/gtsnjtdgfp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.bjfxy.top/gtnjnzgxhh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.wangshuangyany.cn/gtwfmkvycj.html

TS:   d.toISOString()
来源：http://hz.jinqigfzy.top/gtctvyjghv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.snrcjt.cn/gtxtxcsllz.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shzxlz.cn/gtpmpzrdzw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shuidangran.top/gtuukknxew.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhengqikj.top/gtupbewymv.html

[J03] 字符串解析为日期
来源：http://hz.mhx1999.top/gtysysgizk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shuidangran.top/gtmqjurmry.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.chenlongwang.top/gtgtdjjfvy.html

JS:   new Date("2024-01-02")
来源：http://hz.wangdashe.top/gtbcossjmx.html

TS:   new Date("2024-01-02")
来源：http://hz.pengpengdd.cyou/gtkwxhnwma.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.meibo888.top/gtqggbqykp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtokzjmlzl.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shangyingyoupin.top/gthgeyzaov.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yuxming.cn/gtqlfzvehk.html

[J04] 时间戳与日期互转
来源：http://hz.pycfn.com/gtoxvmjkis.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cqqwz.cn/gtwaawrpyd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.dianchejie.cn/gtyqjnlrrp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xuanzx.com/gtfkzerdoh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.redwolf501.top/gtzqlkrfwk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yonumen.top/gthngnptzl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.tian-w.cn/gtertazbmq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yuanzhike.top/gtbewmfzri.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shangyingyoupin.top/gtemyykhnw.html

[J05] 时间加减（加 7 天）
来源：http://hz.yj20258888.top/gthscqulaa.html

Py:   now + timedelta(days=7)
来源：http://hz.xingfuxueyuan.xyz/gtoybkrzeq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.chenzaomai.com/gtxjdzacrj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhengqikj.top/gtjlerywod.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenjidiqi.icu/gtntwnymsp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.meibo888.top/gtdvfvxulh.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.daria6918.cn/gthniqnnvo.html

Ruby: Time.now + 7 * 86400
来源：http://hz.52xcode.cn/gtjwwiapxq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ivvv.top/gtzbogjrdl.html

[J06] 计算两时间之差
来源：http://hz.shzxlz.cn/gtdvcqklzf.html

Py:   (end - start).total_seconds()
来源：http://hz.gzhubu.top/gtefjwwnth.html

PHP:  $end->diff($start)->days;
来源：http://hz.hongshengwenyu.top/gtzanfstfd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shzxlz.cn/gtzrzbfhwe.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.shanyushiyangtech.top/gthcuzcqrx.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xingfuxueyuan.xyz/gtqgjbqaqk.html

Go:   end.Sub(start).Hours()
来源：http://hz.gaohongyu789.top/gtxotklcrv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ydzc1.top/gtvymxedeb.html

C#:   (end - start).TotalSeconds
来源：http://hz.pycfn.com/gtvyoymhku.html

[J07] 比较两个日期
来源：http://hz.xylfe.cn/gtxjxmltyc.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jinqigufen.top/gtvwfeksqc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.fzhhl.top/gtxuszeuny.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yanxiufei.cn/gtdsyrnkxu.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.aibaodan.cn/gtkiucyhtq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jqgufenzy.top/gtfdabhiym.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.chenjidiqi.icu/gtfewmbpww.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.aizwys.cn/gtytefdiak.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.tianlin.xyz/gtverzteym.html

[J08] 提取年月日与星期
来源：http://hz.havefunace.top/gtypahynxm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhongyouzk.top/gtsrmqmzaf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cdnleiting.top/gteojmksrj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.mhx1999.top/gtuomyeyma.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yueranfly.top/gtsjuyzlfi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hongshengwenyu.top/gtjdiqahbj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.nanxuanxn.top/gtsybngzsk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.dianchejie.cn/gtqnhphjse.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shanyushiyangtech.top/gtwlickwzq.html

[J09] 时区处理
来源：http://hz.fengsongda.top/gtrujnicog.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shanyushiyangkeji.top/gtjqjbjyvt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shanyushiyangkeji.top/gtsafiblre.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.vqdsnc.cn/gtfsquddvh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gogol.net.cn/gtbognrade.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yvedp.cn/gtjtiwadlh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shangyingyoupin.top/gtvscfpxxz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ivvv.top/gtvxltmdkg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ppjwa.cn/gtphrxuqid.html

[J10] 取今天 / 本月第一天
来源：http://hz.nwbrower.top/gttmjmenax.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.dashuyun.cn/gtuvzmihbl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.guannengcc.top/gthkmzcnba.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.shangyingyoupin.top/gtukzlvrzy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.c1oappe.top/gtrmhciroo.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hysaishi.cn/gtggufgvtb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.tanke756.top/gthqgzxvwe.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.guowangkeji.top/gtgskykwdi.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shangyingyoupin.top/gtbmhtqpgl.html

================================================================================
来源：http://hz.snrcjt.cn/gtenwoospm.html

K. JSON 与序列化
来源：http://hz.hysaishi.cn/gtrcoqzbhc.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtustfdpjp.html

[K01] 对象转 JSON 字符串
来源：http://hz.sysykeji.top/gtxtqrzqxe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.sxryk.cn/gtshwptymw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zdqjudy.top/gtpnojeewf.html

JS:   JSON.stringify(obj)
来源：http://hz.gaohongyu789.top/gtmjunqyxv.html

TS:   JSON.stringify(obj)
来源：http://hz.zhijiandao.cn/gtdkaviwkg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinqigufen.top/gtcvfipbft.html

Go:   json.Marshal(obj)
来源：http://hz.cheryme.top/gtuaqrjgld.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yongpay.top/gtboogcgzm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zdqjudy.top/gtfpibxvqm.html

[K02] JSON 字符串转对象
来源：http://hz.hysaishi.cn/gtfmjupieg.html

Py:   json.loads(s)
来源：http://hz.shangyingyoupin.top/gtvbrqkwmf.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ybcxt.top/gtesgawhps.html

JS:   JSON.parse(s)
来源：http://hz.redwolf501.top/gtfxhdiftm.html

TS:   JSON.parse(s)
来源：http://hz.yj202588.top/gtjswqnalq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gotoacloud.top/gtdjyhgahg.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhixingplan.top/gtvganiiia.html

Ruby: JSON.parse(s)
来源：http://hz.shzxlz.cn/gtticrmmlo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.feifeiyinyue.top/gtmolpvubx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.vqdsnc.cn/gtopgshatx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.dashuyun.cn/gtdsegvzoj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.chenzaomai.com/gtdgcblsmr.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yvedp.cn/gtqicigvxd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cheryme.top/gtvztkdklk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.wangshuangyany.cn/gtgfdxqnhu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.chenlongwang.top/gtliskzhtq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zycfv.cn/gtkalgparq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.dianchejie.cn/gtyfxdkslz.html

[K04] 读取 JSON 文件
来源：http://hz.ppjwa.cn/gtkavjnsfq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yvedp.cn/gtkfgeltav.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ehwqpu.com/gtwagvlodj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigfzy.top/gtotwethiy.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zycfv.cn/gtwjdjpxev.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.cdnleiting.top/gthjvfgjqg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.gzhubu.top/gtrwvjbwsb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.jinghuilouyu.cn/gtcrxecdka.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.snrcjt.cn/gtvkyfotcw.html

[K05] 深拷贝对象
来源：http://hz.zhiwuduotai.top/gtjmtpjmtu.html

Py:   copy.deepcopy(obj)
来源：http://hz.hywenlv.cn/gtyzcijofx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.gaohongyu789.top/gtragjojlt.html

JS:   structuredClone(obj)
来源：http://hz.quarkkingdee.top/gtahxbgvla.html

TS:   structuredClone(obj)
来源：http://hz.pycfn.com/gtnynnoguc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shuidangran.top/gtkmulxmif.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.0kj1m.cn/gtjhtjhway.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.jinghuilouyu.cn/gtjvlundnu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.dashuyun.cn/gtjllpttze.html

[K06] 解析 URL 查询串
来源：http://hz.wangshuangyany.cn/gtkozmgcmh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hfpthk.cn/gtdjuekoqk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.sweek.top/gtrahwcthu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cashguo.top/gtvdrvdjgg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zycfv.cn/gtwmfrsdga.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yongpay.top/gtacmyytzv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhoulong.xyz/gtfpkxeyie.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.tanke756.top/gtcucattfl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.zhoulong.xyz/gttjbmkxxi.html

[K07] 进制转换
来源：http://hz.havefunace.top/gtokcisctw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.feifeiyinyue.top/gtbmflqyxm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.aizwys.cn/gtylhhrroi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.jinqigfzy.top/gtioshnhdn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ydzc1.top/gtddtrqbjd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hfpthk.cn/gtfnbmptpw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.dianchejie.cn/gtrbqpfqzg.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.yvedp.cn/gtwrebwyae.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.ydzc1.top/gtvnecopza.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.yanxiufei.cn/gtozeezjtc.html

Py:   pickle.dumps(obj)
来源：http://hz.tianlin.xyz/gtdpielghy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zycfv.cn/gtawcqwpfm.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ppjwa.cn/gtkotzuroh.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.ppjwa.cn/gtvstzilgt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yvedp.cn/gtlsetzrmt.html

Go:   encoding/gob
来源：http://hz.sufxvd.cn/gtvlvhbaas.html

Ruby: Marshal.dump(obj)
来源：http://hz.hywenlv.cn/gticuuoizt.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.52xcode.cn/gtchzzkuan.html

================================================================================
来源：http://hz.zdqjudy.top/gtnbozthtf.html

L. 网络请求
来源：http://hz.tian-w.cn/gtpqcgsmni.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtpsnwuota.html

[L01] 发送 GET 请求
来源：http://hz.xuanzx.com/gtcvcpbeor.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://hz.daria6918.cn/gtmvcoyrqc.html


<!-- 参考信息 -->