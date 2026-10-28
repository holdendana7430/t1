代发 wailian999

JS:   class MyError extends Error {}
来源：http://hz.jyoumei.cn/gtwxroblyk.html

TS:   class MyError extends Error {}
来源：http://hz.yvedp.cn/gtbdqigwik.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jinghuilouyu.cn/gtzkogjcnu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hammf.cn/gtbyupcuvg.html

Ruby: class MyError < StandardError; end
来源：http://hz.pengpengdd.cyou/gtjmvlcsat.html

C#:   class MyException : Exception {}
来源：http://hz.svipenyu.cn/gtbbnjotbb.html

[H05] 捕获特定类型
来源：http://hz.jqgfzy.top/gtzewzmtyy.html

Py:   except ValueError as e:
来源：http://hz.xingfuxueyuan.xyz/gtaumebqxg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yuanzhike.top/gttnaskfwo.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhixingplan.top/gtalincmsa.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.redwolf501.top/gtdbkxxutp.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nwbrower.top/gtmuhzentt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cheryme.top/gthchvlmka.html

Ruby: rescue ArgumentError => e
来源：http://hz.birdmap.top/gtdvrmsfca.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hfpthk.cn/gtqpfoasvi.html

[H06] 可选值 / 空值安全访问
来源：http://hz.fzhhl.top/gtgzkupojt.html

Py:   value = d.get("k") or default
来源：http://hz.pengpengdd.cyou/gthjclmvxx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.0kj1m.cn/gttzzbmlfo.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xylfe.cn/gtgivdxfpp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.iojbl.cn/gtkdmhfdqp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.redwolf501.top/gtmmtyjpxg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.gzhubu.top/gtcdweuypo.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhijiandao.cn/gtkgynyzxw.html

C#:   obj?.A?.B ?? default
来源：http://hz.316326.xyz/gtutzivfie.html

[H07] 断言
来源：http://hz.nanxuanxn.top/gtgknfejwv.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yanxiufei.cn/gtjnnszghv.html

PHP:  assert($x > 0);
来源：http://hz.smart0.xyz/gtbsnqzdzb.html

JS:   console.assert(x > 0);
来源：http://hz.mhx1999.top/gtsclbqlum.html

TS:   console.assert(x > 0);
来源：http://hz.zhijiandao.cn/gtzjxchsfo.html

Java: assert x > 0 : "必须为正";
来源：http://hz.guowangkeji.top/gthonzuqii.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.0kj1m.cn/gtirglendb.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zycfv.cn/gtvmeiwjns.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sweek.top/gtfgiwniuw.html

[H08] 获取错误信息与堆栈
来源：http://hz.shzxlz.cn/gtcvwgvdhh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jiagoushi.top/gtgcdnyuov.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.tanke756.top/gtrpvvxouw.html

JS:   e.message;  e.stack
来源：http://hz.hysaishi.cn/gtqulpenhu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhengqikj.top/gtkimsyufy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.redwolf501.top/gtaffvmouu.html

Go:   err.Error()
来源：http://hz.quarkkingdee.top/gtoruwojbz.html

Ruby: e.message;  e.backtrace
来源：http://hz.jianghu66.top/gtnyzghxgk.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hnxiangtu.top/gtvyeqkhwp.html

[H09] 带错误码的异常
来源：http://hz.cheryme.top/gtihsewdgv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhoulong.xyz/gtvcsfnuzl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yuanzhike.top/gtatdllfow.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ywan-chungtsiang.top/gtgwktqbfj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.tian-w.cn/gtzxnbvhfc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.aibaodan.cn/gtrdpxsllx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hnqzz.top/gtmxjrxcxl.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sufxvd.cn/gtfasvymaw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sxryk.cn/gthlycaylo.html

[H10] 资源自动释放
来源：http://hz.cqqwz.cn/gtojksosde.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.dashuyun.cn/gtbmgtutjh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jlsjyb.cn/gtazuialuy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yvedp.cn/gtymsxidpb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xinyue.icu/gtfmfqtzfw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhongyouzk.top/gtndggfist.html

Go:   defer f.Close()
来源：http://hz.havefunace.top/gticcjqzgn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhixingplan.top/gtzuvyhvvx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ehwqpu.com/gtjkwmahon.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtmhooxxem.html

I. 正则表达式
来源：http://hz.hywenlv.cn/gtkphuvnur.html

================================================================================
来源：http://hz.hywenlv.cn/gttjvzuaqp.html

[I01] 判断是否匹配
来源：http://hz.316326.xyz/gtcelusjme.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.bjfxy.top/gtsompungx.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hongshengwenyu.top/gtmwfabidq.html

JS:   /\d+/.test(s)
来源：http://hz.cqqwz.cn/gtabfavidg.html

TS:   /\d+/.test(s)
来源：http://hz.cashguo.top/gtupievlwu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.vqdsnc.cn/gtufsaulxm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yj20258.top/gtdimsztbx.html

Ruby: s.match?(/\d+/)
来源：http://hz.wangshuangyany.cn/gtudsymoar.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shuidangran.top/gtsyofdrnf.html

[I02] 提取所有匹配
来源：http://hz.jinqigfzy.top/gteljrcjux.html

Py:   re.findall(r"\d+", s)
来源：http://hz.cucudq.cn/gtaysxelbr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.sweek.top/gtmxvyfnkh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shzxlz.cn/gtvwpvxrtk.html

TS:   s.match(/\d+/g)
来源：http://hz.xuetiantiany.cn/gtnxszdcgn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhijiandao.cn/gtpnotilvv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhoulong.xyz/gttspqnrxx.html

Ruby: s.scan(/\d+/)
来源：http://hz.zycfv.cn/gtdnvqpzyy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cqqwz.cn/gtnvkrhpqx.html

[I03] 提取捕获分组
来源：http://hz.kuanghao11.cn/gtmnzebkwy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jinyuanbaomall.cn/gtkzjfvyxl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.quarkkingdee.top/gttyaxsybv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.shangyingyoupin.top/gtkhviazbj.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.chenjidiqi.icu/gteeemvtnz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yanxiufei.cn/gtifapspup.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hammf.cn/gtfvzzdnfz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yj202588.top/gtdiinzydg.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.shanyushiyangkeji.top/gtcsblyjac.html

[I04] 正则替换
来源：http://hz.shuidangran.top/gtmvtqqmlp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.52xcode.cn/gtcpdtympo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.quarkkingdee.top/gtcffhhqmx.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.0kj1m.cn/gtjkuhyaaq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xingfuxueyuan.xyz/gtstmyyfrv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zycfv.cn/gtwpprlatn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xuanzx.com/gtsosukgyk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yangfankeji.com/gtuuntqbok.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.c1oappe.top/gtsdnkhsbp.html

[I05] 按正则拆分
来源：http://hz.aizwys.cn/gtuqaugwgj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.kuanghao11.cn/gtbgrfjvnn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.feifeiyinyue.top/gtwmytneib.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.c1oappe.top/gtkggxxkvk.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jinqigfzy.top/gtszdmidhg.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shzxlz.cn/gtaagtvfnl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xuanzx.com/gtyvdzqvzi.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yueranfly.top/gtormhcyuz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ivvv.top/gtedgelxyf.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.redwolf501.top/gtjljsefcu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jiagoushi.top/gtsxvkwrwp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xziqi.cn/gtlradwqjf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yongpay.top/gtxvquoirj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shuidangran.top/gtqxrlmszu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhaomingkeji.xyz/gtivhfeazq.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.0kj1m.cn/gtpsrcjqak.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.guannengcc.top/gtbamlgtya.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.0kj1m.cn/gtuqptiybb.html

[I07] 忽略大小写与多行模式
来源：http://hz.hywenlv.cn/gtccobtyzc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ydzc1.top/gtraqgovyw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.sxryk.cn/gtrmnhztkq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.dashuyun.cn/gtgmtzjyyd.html

TS:   /error/gim
来源：http://hz.meibo888.top/gtepfwrwnw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shzxlz.cn/gtcrdvbtse.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.dashuyun.cn/gtwtkkalsz.html

Ruby: s.scan(/error/i)
来源：http://hz.chenlongwang.top/gtnazkxpgv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shuidangran.top/gtpqgqsmdp.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.316326.xyz/gtolosqspq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.9152youxi.cn/gtqfpgbrij.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.andypj.xyz/gtfdtcdnkg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xingfuxueyuan.xyz/gtckhzzamy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangkeji.top/gtvfnepjkc.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yanxiufei.cn/gtdrtpxlfn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.iojbl.cn/gtzhaopcuc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yj20258.top/gttjcypwum.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.nanxuanxn.top/gtngzftnuk.html

================================================================================
来源：http://hz.yj202588.top/gtifjyyryg.html

J. 日期与时间
来源：http://hz.shangyingyoupin.top/gtvppgvqkz.html

================================================================================
来源：http://hz.tianlin.xyz/gtpjzvjktp.html

[J01] 获取当前时间
来源：http://hz.aizwys.cn/gtklfdomzz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.dashuyun.cn/gthrwpxywo.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xziqi.cn/gtpbpzutud.html

JS:   new Date();  Date.now()
来源：http://hz.shangyingyoupin.top/gteytzocvc.html

TS:   new Date();  Date.now()
来源：http://hz.smart0.xyz/gtsxgfenlm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.meibo888.top/gtqukymnsh.html

Go:   time.Now()
来源：http://hz.zhaomingkeji.xyz/gtctbvvxck.html

Ruby: Time.now
来源：http://hz.gzhubu.top/gtmmfoanjs.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hywenlv.cn/gtvkudsiod.html

[J02] 格式化输出
来源：http://hz.zhengqikj.top/gtuxclnhxb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258.top/gtplykbbcu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jlsjyb.cn/gtdwbahvlc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zdqjudy.top/gtlgbudhnf.html

TS:   d.toISOString()
来源：http://hz.sweek.top/gtwqaueqyf.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gaohongyu789.top/gtbgsiwfar.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.fengsongda.top/gtfphgwjkb.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.feifeiyinyue.top/gtglhyxzpi.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.meibo888.top/gtcfojgipv.html

[J03] 字符串解析为日期
来源：http://hz.hnqzz.top/gtvqyiluzv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.chenlongwang.top/gtedgvczfw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sweek.top/gttkbilhhd.html

JS:   new Date("2024-01-02")
来源：http://hz.zhijiandao.cn/gtrgqtnkgg.html

TS:   new Date("2024-01-02")
来源：http://hz.xziqi.cn/gtmoiorowg.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.bjfxy.top/gtwgglesqk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yongpay.top/gtpsycoqny.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gotoacloud.top/gtnvbckxxp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hysaishi.cn/gtyounynxx.html

[J04] 时间戳与日期互转
来源：http://hz.sweek.top/gtowcxcjle.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.kuanghao11.cn/gtfdmwqecu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.iojbl.cn/gtsvrhasrh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ivvv.top/gtfpmejubm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xinyue.icu/gteqzhznvz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yueranfly.top/gteafvnwct.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yj20258888.top/gtctrclrad.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yuanzhike.top/gtuikxhvgh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.pycfn.com/gtybdrfiuk.html

[J05] 时间加减（加 7 天）
来源：http://hz.smart0.xyz/gtjslnhoha.html

Py:   now + timedelta(days=7)
来源：http://hz.ydjk.org.cn/gtmwdrrpjo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.guannengcc.top/gtdpykkpmw.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.smart0.xyz/gtnoxcfqjk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shanyushiyangkeji.top/gtruogmjvq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.bjfxy.top/gttcqlkhxn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ivvv.top/gtvhscskui.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hywenlv.cn/gtdweegscy.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ehwqpu.com/gtozkaqfzw.html

[J06] 计算两时间之差
来源：http://hz.shanyushiyangkeji.top/gtsqwvishv.html

Py:   (end - start).total_seconds()
来源：http://hz.snrcjt.cn/gtbxgbatze.html

PHP:  $end->diff($start)->days;
来源：http://hz.0kj1m.cn/gtclokkwgs.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ehwqpu.com/gtgyyshdtw.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.guowangkeji.top/gthittboar.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xuanzx.com/gtfvyvjfow.html

Go:   end.Sub(start).Hours()
来源：http://hz.ydzc1.top/gtxojmjyui.html

Ruby: end - start                 # 返回秒数
来源：http://hz.daria6918.cn/gttklmpsbp.html

C#:   (end - start).TotalSeconds
来源：http://hz.jlsjyb.cn/gtkjcmeakn.html

[J07] 比较两个日期
来源：http://hz.haohaochexian.top/gtkgjsrgfr.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yvedp.cn/gtmewtelbn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.kuanghao11.cn/gtulzothvn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ydzc1.top/gtvwqkyupk.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jianghu66.top/gtuungpiiq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hnqzz.top/gtjgygjkrn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhixingplan.top/gtauajlzex.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangtech.top/gtwkqdrurk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.mhx1999.top/gtauwqumoy.html

[J08] 提取年月日与星期
来源：http://hz.mhx1999.top/gtpiunepyk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shzxlz.cn/gtkvzazrnh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.316326.xyz/gtinkirvku.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yj202588.top/gtozgjehfz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.pengpengdd.cyou/gtpgrfezwq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jyoumei.cn/gtkofgkflo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xylfe.cn/gtitwdbohk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gotoacloud.top/gtmnivteyo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xinyue.icu/gtssvvmbhq.html

[J09] 时区处理
来源：http://hz.redwolf501.top/gtsijtnyio.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hammf.cn/gtgztgszts.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.wangdashe.top/gtdmycispo.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ivvv.top/gtgdngmeca.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gtuytlxkdg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jyoumei.cn/gtmsoahuaz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.chenjidiqi.icu/gtqhaeeepw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.feifeiyinyue.top/gtgobaogwg.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hywenlv.cn/gtowvhqjpy.html

[J10] 取今天 / 本月第一天
来源：http://hz.xingfuxueyuan.xyz/gtnvjbxzly.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.quarkkingdee.top/gtvbdcrhmv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.redwolf501.top/gtulkvdfea.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhiwuduotai.top/gtzyxuzocg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xuetiantiany.cn/gtpghpvogf.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nwbrower.top/gtzgerbgyt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.aibaodan.cn/gtvnsdhdkn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yj20258888.top/gtflixouxh.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sweek.top/gtmltmrzix.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtduzeupel.html

K. JSON 与序列化
来源：http://hz.jlsjyb.cn/gtrwlzqcqz.html

================================================================================
来源：http://hz.daxiang520.top/gttwvclxyb.html

[K01] 对象转 JSON 字符串
来源：http://hz.guannengcc.top/gtisxjmfph.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.daria6918.cn/gthubnnzfy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cheryme.top/gtjskhqjth.html

JS:   JSON.stringify(obj)
来源：http://hz.snrcjt.cn/gttcuwpxho.html

TS:   JSON.stringify(obj)
来源：http://hz.zhongyouzk.top/gtfaymxibl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.dianchejie.cn/gthptdepfm.html

Go:   json.Marshal(obj)
来源：http://hz.guannengcc.top/gtqpcecvhn.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.aibaodan.cn/gtietxeyki.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ydzc1.top/gtwdxaejcn.html

[K02] JSON 字符串转对象
来源：http://hz.ydjk.org.cn/gtyqkxvwhj.html

Py:   json.loads(s)
来源：http://hz.jinyuanbaomall.cn/gtnobyorhg.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.fengsongda.top/gtbaqwjelc.html

JS:   JSON.parse(s)
来源：http://hz.ybcxt.top/gtpzcnlrvo.html

TS:   JSON.parse(s)
来源：http://hz.chenzaomai.com/gtxhoovlsq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yangfankeji.com/gtaxeuycbf.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.c1oappe.top/gtmyhetutb.html

Ruby: JSON.parse(s)
来源：http://hz.chenzaomai.com/gtkmjiijxh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ivvv.top/gtgunglupx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhiwuduotai.top/gthhyvpfrk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.sxryk.cn/gtjzgkgsom.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cucudq.cn/gtlvobprod.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangtech.top/gtqishzdya.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangdashe.top/gtxpenzrjx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.guannengcc.top/gtkghhsokf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.haohaochexian.top/gthpczsrro.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nanxuanxn.top/gtifbhsmci.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yangfankeji.com/gtxkoovtol.html

[K04] 读取 JSON 文件
来源：http://hz.dashuyun.cn/gtgucjhlnq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gogol.net.cn/gtqhxzxqfj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.sysykeji.top/gtozsbgcmo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnqzz.top/gtoazoptvu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigfzy.top/gtzxbyhqpo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.wangdashe.top/gtaqmmtpgy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhengqikj.top/gtrwguvlut.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.sysykeji.top/gtozmzmmux.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.hysaishi.cn/gtggrzdone.html

[K05] 深拷贝对象
来源：http://hz.fzhhl.top/gtuksokkwz.html

Py:   copy.deepcopy(obj)
来源：http://hz.havefunace.top/gtwnwhvfwx.html

PHP:  unserialize(serialize($obj));
来源：http://hz.haohaochexian.top/gtxbtsxsnb.html

JS:   structuredClone(obj)
来源：http://hz.jinghuilouyu.cn/gtlasfwkqf.html

TS:   structuredClone(obj)
来源：http://hz.zhongyouzk.top/gtztdxsbai.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.tanke756.top/gtmfrfxsgh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.gogol.net.cn/gtseswyjyu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.shuidangran.top/gtukepnlkc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.hongshengwenyu.top/gtgepcjxvj.html

[K06] 解析 URL 查询串
来源：http://hz.yanxiufei.cn/gttkmsvwdl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.tanke756.top/gtsvsppkcx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.tanke756.top/gtznmolluk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.gotoacloud.top/gtglhxwzoz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.guannengcc.top/gtzujvpkjw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.9152youxi.cn/gttlbvomoq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xuetiantiany.cn/gtbuxvzjek.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ydjk.org.cn/gtbfkwzkpd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ydjk.org.cn/gtgovwodjv.html

[K07] 进制转换
来源：http://hz.smart0.xyz/gtuiruhntq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.iojbl.cn/gteaxuotnm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.jyoumei.cn/gtpmatddxk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hfpthk.cn/gtsxcnephz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.ydzc1.top/gtklruvvac.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.guannengcc.top/gtnqdfazbw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.shanyushiyangtech.top/gtbwdoqlqr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jqgufenzy.top/gtsdtszloh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.hnqzz.top/gtwhfakrle.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.52xcode.cn/gtozxdktdn.html

Py:   pickle.dumps(obj)
来源：http://hz.dashuyun.cn/gtvrzxoheu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zhixingplan.top/gtelpwpuds.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.quarkkingdee.top/gtvaxeentk.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.chenjidiqi.icu/gtczzyhwnu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.chenlongwang.top/gtylaikrli.html


<!-- 参考信息 -->