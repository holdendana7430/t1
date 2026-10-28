代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.iojbl.cn/gtbvxswrbv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.dianchejie.cn/gtozdyipod.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hongshengwenyu.top/gthdxtdggj.html

[H02] finally / ensure 收尾
来源：http://hz.fengsongda.top/gtrrwggvug.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.daxiang520.top/gtccnjcwbh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtfefiyqrj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gtoibuuwxk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jinghuilouyu.cn/gtewufpvay.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtmmfupfdm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhijiandao.cn/gtykaajjey.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhijiandao.cn/gtncnytgvt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.dianchejie.cn/gtiqtnpmcw.html

[H03] 主动抛出异常
来源：http://hz.havefunace.top/gtspdovxzp.html

Py:   raise ValueError("错误信息")
来源：http://hz.daria6918.cn/gtubhbhnlk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yvedp.cn/gtuvvzagmw.html

JS:   throw new Error("错误信息");
来源：http://hz.0kj1m.cn/gtsbypmhif.html

TS:   throw new Error("错误信息");
来源：http://hz.zhongyouzk.top/gtasuafrnd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sxryk.cn/gtflagyrag.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.pengpengdd.cyou/gtorrhghvy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.mhx1999.top/gtxrrgsrqy.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ydjk.org.cn/gtvpkbanyy.html

[H04] 自定义异常类型
来源：http://hz.yueranfly.top/gtdfkvbpsk.html

Py:   class MyError(Exception): pass
来源：http://hz.zhiwuduotai.top/gthqiewxtl.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.cqqwz.cn/gticrgavaf.html

JS:   class MyError extends Error {}
来源：http://hz.vqdsnc.cn/gtletgbpxe.html

TS:   class MyError extends Error {}
来源：http://hz.zhengqikj.top/gtwciodqyl.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hongshengwenyu.top/gtkqeyvyfi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.guowangkeji.top/gtkydmauvz.html

Ruby: class MyError < StandardError; end
来源：http://hz.yj202588.top/gtkmmgawon.html

C#:   class MyException : Exception {}
来源：http://hz.bjfxy.top/gtvuvbhzhi.html

[H05] 捕获特定类型
来源：http://hz.zhixingplan.top/gtwfjefuzq.html

Py:   except ValueError as e:
来源：http://hz.jyoumei.cn/gtexykyzgy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ehwqpu.com/gtopvrfpaa.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hfpthk.cn/gtguvzmvwh.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shzxlz.cn/gtsfthgltr.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.dianchejie.cn/gtyjivpdrt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.fengsongda.top/gtubpyjsul.html

Ruby: rescue ArgumentError => e
来源：http://hz.xuetiantiany.cn/gteylxkagv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.daria6918.cn/gtuwqfmsrl.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sxryk.cn/gtcabyqmoq.html

Py:   value = d.get("k") or default
来源：http://hz.tian-w.cn/gtpxssesye.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yj202588.top/gtqvyntcou.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhongyouzk.top/gtzswinnax.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.0kj1m.cn/gtajfvvurw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.nwbrower.top/gtxrbrjotg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.snrcjt.cn/gteuhqazpi.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yongpay.top/gtciwjnmra.html

C#:   obj?.A?.B ?? default
来源：http://hz.andypj.xyz/gtlelpuoxf.html

[H07] 断言
来源：http://hz.cashguo.top/gtegcshkdd.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinghuilouyu.cn/gtvxmrasgh.html

PHP:  assert($x > 0);
来源：http://hz.yangfankeji.com/gtuwsislot.html

JS:   console.assert(x > 0);
来源：http://hz.jianghu66.top/gtcvirhcau.html

TS:   console.assert(x > 0);
来源：http://hz.xuanzx.com/gtzbthbmvi.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cucudq.cn/gtolukwlig.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinyuanbaomall.cn/gtiqqiyytl.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sweek.top/gtbfddmrax.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yuxming.cn/gtgvngcpfe.html

[H08] 获取错误信息与堆栈
来源：http://hz.yj20258.top/gtgwiifffl.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.wangdashe.top/gtrmyijqdp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.kuanghao11.cn/gtyyvsvlmk.html

JS:   e.message;  e.stack
来源：http://hz.gogol.net.cn/gtkdhxprxc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinqigufen.top/gtttnqmvgn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yonumen.top/gtejcyllpn.html

Go:   err.Error()
来源：http://hz.xingfuxueyuan.xyz/gtovkkdjup.html

Ruby: e.message;  e.backtrace
来源：http://hz.yonumen.top/gtuwnylpnb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhengqikj.top/gtnymvvxfy.html

[H09] 带错误码的异常
来源：http://hz.9152youxi.cn/gtqbwjjtcq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.svipenyu.cn/gtkvdfsbij.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.andypj.xyz/gtagkqggeo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.gaohongyu789.top/gtenipbuim.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yvedp.cn/gtjyxpznac.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cqqwz.cn/gtklpcihuc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.nanxuanxn.top/gtcocrielk.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hnxiangtu.top/gtoabpkquv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinyuanbaomall.cn/gtzcymcnqf.html

[H10] 资源自动释放
来源：http://hz.hywenlv.cn/gtltgpttjl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jinghuilouyu.cn/gtfbybtido.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj20258.top/gtxsxlclkv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jlsjyb.cn/gtaggaqcav.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuxming.cn/gtzyvtpoxc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.gogol.net.cn/gtjgcuvicc.html

Go:   defer f.Close()
来源：http://hz.kuanghao11.cn/gtbtwpzstb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xylfe.cn/gtqmjzbocv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ehwqpu.com/gtdefrqizf.html

================================================================================
来源：http://hz.mhx1999.top/gtgnwejash.html

I. 正则表达式
来源：http://hz.fengsongda.top/gtfqxestjz.html

================================================================================
来源：http://hz.yanxiufei.cn/gtqpmutjou.html

[I01] 判断是否匹配
来源：http://hz.nanxuanxn.top/gtffjbmmgm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jianghu66.top/gttkfcgwhi.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhixingplan.top/gtbexjhwmv.html

JS:   /\d+/.test(s)
来源：http://hz.redwolf501.top/gteyymmqmm.html

TS:   /\d+/.test(s)
来源：http://hz.dianchejie.cn/gtpnwqyvoo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hnqzz.top/gttkhqduup.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hnxiangtu.top/gtldbcifkg.html

Ruby: s.match?(/\d+/)
来源：http://hz.xinyue.icu/gtzufjutpr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yj20258888.top/gtkoubdbhw.html

[I02] 提取所有匹配
来源：http://hz.52xcode.cn/gtatblitrj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.sweek.top/gtxdpoiehq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jinqigfzy.top/gteaesmaxq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.birdmap.top/gtagcplvlz.html

TS:   s.match(/\d+/g)
来源：http://hz.jinghuilouyu.cn/gtxmkwcbpb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xylfe.cn/gtnpueyjmn.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cucudq.cn/gtwqsarytt.html

Ruby: s.scan(/\d+/)
来源：http://hz.cashguo.top/gtpsjzyusq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gaohongyu789.top/gtztpmdzyw.html

[I03] 提取捕获分组
来源：http://hz.hywenlv.cn/gtiqqlpuyt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jinqigufen.top/gtuwsjcqmx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.meibo888.top/gtznzenbwr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.dianchejie.cn/gthyyvyzph.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cucudq.cn/gtkmhbbbrt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gaohongyu789.top/gtenqozrfx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.chenjidiqi.icu/gtecuuxdqt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hnqzz.top/gtwhqztvpq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.birdmap.top/gttmwawvxw.html

[I04] 正则替换
来源：http://hz.chenlongwang.top/gtjyvqgjwc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.sxryk.cn/gtmiaevuam.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.chenjidiqi.icu/gtmvscqcyq.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ydjk.org.cn/gtoquejjdn.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.guannengcc.top/gtioavkxbj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jiagoushi.top/gtfuusugjv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.nanxinkj.top/gtdhgcwmop.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ywan-chungtsiang.top/gtqxgldnab.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hfpthk.cn/gtogzpours.html

[I05] 按正则拆分
来源：http://hz.zhixingplan.top/gtmffhukqb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xinyue.icu/gtbvipzhdg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.wangshuangyany.cn/gttknglnjt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.fzhhl.top/gtwklxmoum.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jinqigufen.top/gtcvcmihgs.html

Java: s.split("\\s*,\\s*")
来源：http://hz.mhx1999.top/gtmzvybmvp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.nanxinkj.top/gthqqlsvrk.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.fzhhl.top/gtmctllvsa.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yj202588.top/gtltreqtyq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.andypj.xyz/gtjfnrjuxl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.0kj1m.cn/gtroqmfaii.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.svipenyu.cn/gtbafqlljj.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ehwqpu.com/gtvtthvbzg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gzhubu.top/gtwlfcaaxb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gtcfknqavn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.cashguo.top/gtlgqodzgm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.bjfxy.top/gtjvrejivz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yuanzhike.top/gtszmgzyxe.html

[I07] 忽略大小写与多行模式
来源：http://hz.sxryk.cn/gtnnuumhwe.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.gotoacloud.top/gtgbgyjafd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.daria6918.cn/gtmibtkgvj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zdqjudy.top/gtvcpbnqje.html

TS:   /error/gim
来源：http://hz.iojbl.cn/gtvcdspukj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xingfuxueyuan.xyz/gtcznkwqgq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.kuanghao11.cn/gtczprdtdp.html

Ruby: s.scan(/error/i)
来源：http://hz.guannengcc.top/gttldkofkd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhoulong.xyz/gtpapgcnba.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.wangshuangyany.cn/gtsfhblent.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.pycfn.com/gtdauekvpb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.tanke756.top/gtzerfggny.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenjidiqi.icu/gthilktxsf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ivvv.top/gtcwynsrce.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.daria6918.cn/gtqjgdwhrn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.kuanghao11.cn/gtydovxkvf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jiagoushi.top/gthfevpont.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.bjfxy.top/gtapcegeiv.html

================================================================================
来源：http://hz.yuanzhike.top/gtgmzkapzv.html

J. 日期与时间
来源：http://hz.shangyingyoupin.top/gtzhyioeye.html

================================================================================
来源：http://hz.daxiang520.top/gtrwmtqxtx.html

[J01] 获取当前时间
来源：http://hz.birdmap.top/gtefuyhnmh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.daria6918.cn/gtadmiqcer.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhaomingkeji.xyz/gtxnzleity.html

JS:   new Date();  Date.now()
来源：http://hz.hfpthk.cn/gtiifyplxg.html

TS:   new Date();  Date.now()
来源：http://hz.zycfv.cn/gtvqudkets.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jqgufenzy.top/gtohsiortv.html

Go:   time.Now()
来源：http://hz.aizwys.cn/gtxouodwyo.html

Ruby: Time.now
来源：http://hz.52xcode.cn/gtzyxfeyug.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hysaishi.cn/gtwgrvltfa.html

[J02] 格式化输出
来源：http://hz.sufxvd.cn/gtarlqjnru.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cheryme.top/gtfkzbzisv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ivvv.top/gtphvdbijd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yj20258.top/gtdemkbrmk.html

TS:   d.toISOString()
来源：http://hz.jlsjyb.cn/gtpwxkbsvu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jianghu66.top/gtginkxriu.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zycfv.cn/gtrqqecdyf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.9152youxi.cn/gtbbuzpxsv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xuetiantiany.cn/gtpbdcxesl.html

[J03] 字符串解析为日期
来源：http://hz.sysykeji.top/gtvpmxaucp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.snrcjt.cn/gtbrzgtzez.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xingfuxueyuan.xyz/gtmdvlqgtn.html

JS:   new Date("2024-01-02")
来源：http://hz.zhoulong.xyz/gtjliqohyi.html

TS:   new Date("2024-01-02")
来源：http://hz.dashuyun.cn/gtrglmhrxw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.havefunace.top/gtoltylcdk.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tianlin.xyz/gtizdicdfb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cashguo.top/gtqamnwidl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.52xcode.cn/gtmmppgjlq.html

[J04] 时间戳与日期互转
来源：http://hz.aizwys.cn/gtxyprubba.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yj20258.top/gtmvjarfqh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.chenzaomai.com/gteiwyvkam.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hnxiangtu.top/gtqeghxcze.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.0kj1m.cn/gtrylokhds.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shanyushiyangtech.top/gtpvezsxhg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nanxuanxn.top/gtecgbspmb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ybcxt.top/gtnkwyyimo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.bjfxy.top/gtswsympdk.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhiwuduotai.top/gtllhiwebl.html

Py:   now + timedelta(days=7)
来源：http://hz.hammf.cn/gtkfhcfwdf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhiwuduotai.top/gthakujicz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yueranfly.top/gtbwajdkbi.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuetiantiany.cn/gtrzdhmtbv.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj20258.top/gtgxovwcuv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cashguo.top/gtwzizpmcu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ywan-chungtsiang.top/gtifyszwsb.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.daria6918.cn/gthvhzyxhx.html

[J06] 计算两时间之差
来源：http://hz.jinghuilouyu.cn/gtehwdvayk.html

Py:   (end - start).total_seconds()
来源：http://hz.cashguo.top/gtevbuhebt.html

PHP:  $end->diff($start)->days;
来源：http://hz.ybcxt.top/gtrrylmghx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sysykeji.top/gtkksojwqj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ydzc1.top/gtzoolrwwc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jlsjyb.cn/gtemoomnta.html

Go:   end.Sub(start).Hours()
来源：http://hz.hnqzz.top/gtidsheqwc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.cashguo.top/gtlmlqjzcf.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhongyouzk.top/gtidizmteq.html

[J07] 比较两个日期
来源：http://hz.9152youxi.cn/gtppkiwkws.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cashguo.top/gtgqqgjhsw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cqqwz.cn/gtippwaekg.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ybcxt.top/gtuptjmudj.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xylfe.cn/gtvkpnihhm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jianghu66.top/gtydxbofhu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinqigufen.top/gttuwhkvfm.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhaomingkeji.xyz/gtxwcazgru.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yuanzhike.top/gtwoqdufex.html

[J08] 提取年月日与星期
来源：http://hz.haohaochexian.top/gtaardipjl.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yvedp.cn/gtbvxjxsmy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhongyouzk.top/gtuazivxuh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cheryme.top/gtgarpswsz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.nwbrower.top/gtojtqdxpb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.iojbl.cn/gttbiywrje.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.andypj.xyz/gtqykhwoqc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ywan-chungtsiang.top/gtefprhjyl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.9152youxi.cn/gtsrfpfzye.html

[J09] 时区处理
来源：http://hz.cucudq.cn/gtabsfsusu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.tianlin.xyz/gtggnhsxnd.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.snrcjt.cn/gthnonhosi.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhaomingkeji.xyz/gtebhjvgus.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangkeji.top/gtmabldwcl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.shzxlz.cn/gtlhdwotku.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.tianlin.xyz/gtxkxrqosp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhengqikj.top/gtkoxtfidf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yuanzhike.top/gtapfpuonj.html

[J10] 取今天 / 本月第一天
来源：http://hz.chenjidiqi.icu/gtclaieljj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cashguo.top/gtjigzqqkg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hfpthk.cn/gtgarmlxkt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xuanzx.com/gtkkjzfuzp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hongshengwenyu.top/gtdztgvfeh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yonumen.top/gtbilgagov.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gzhubu.top/gtgazaxjzn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.tianlin.xyz/gtprylqbru.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.svipenyu.cn/gtxquvavpk.html

================================================================================
来源：http://hz.hnxiangtu.top/gtqnzgqlpm.html

K. JSON 与序列化
来源：http://hz.dianchejie.cn/gtenusjecp.html

================================================================================
来源：http://hz.sxryk.cn/gtcoizzsck.html

[K01] 对象转 JSON 字符串
来源：http://hz.fengsongda.top/gthdyhxfwl.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.havefunace.top/gtyhrwtcnk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xylfe.cn/gtxqrzvzhp.html

JS:   JSON.stringify(obj)
来源：http://hz.snrcjt.cn/gtdfhwpgpj.html

TS:   JSON.stringify(obj)
来源：http://hz.nanxuanxn.top/gtrgwjztpt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yuanzhike.top/gtqwjokviw.html

Go:   json.Marshal(obj)
来源：http://hz.ydjk.org.cn/gteqnhaqdy.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.dashuyun.cn/gtbttjojna.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sysykeji.top/gtdsmdqymv.html

[K02] JSON 字符串转对象
来源：http://hz.yonumen.top/gtlxwlnyad.html

Py:   json.loads(s)
来源：http://hz.shuidangran.top/gtbbgyehkx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shanyushiyangtech.top/gtbmrylleg.html

JS:   JSON.parse(s)
来源：http://hz.xingfuxueyuan.xyz/gtatmenjth.html

TS:   JSON.parse(s)
来源：http://hz.guannengcc.top/gthstnrare.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hongshengwenyu.top/gtbmlnlcfx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hnqzz.top/gtsuymcrbr.html

Ruby: JSON.parse(s)
来源：http://hz.daxiang520.top/gtoeahkmlf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ybcxt.top/gtpaetstmf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.sweek.top/gtpfhqnyct.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jqgufenzy.top/gtysxwfrsk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.meibo888.top/gtalsxbioq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.bjfxy.top/gtidoeteng.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinqigufen.top/gtekaqulod.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinyuanbaomall.cn/gthkaaeuyi.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ydzc1.top/gtshfajlpk.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.yj20258.top/gtvnzmxksh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xuanzx.com/gtunoykkyd.html

[K04] 读取 JSON 文件
来源：http://hz.jqgfzy.top/gtadkfanbk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cdnleiting.top/gtvteglvri.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.redwolf501.top/gtlzxdvjyq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.wangdashe.top/gtxhtgkzky.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.aibaodan.cn/gttktkhfhv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.jinqigfzy.top/gtngygssqp.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yongpay.top/gtaqwabzxu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.chenjidiqi.icu/gtsfwtffxv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shanyushiyangkeji.top/gttvjmenra.html

[K05] 深拷贝对象
来源：http://hz.yj20258.top/gtckdcewgv.html

Py:   copy.deepcopy(obj)
来源：http://hz.guowangkeji.top/gtqhhblqdy.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yuanzhike.top/gtwukvibav.html

JS:   structuredClone(obj)
来源：http://hz.jinqigufen.top/gtlmgwhqlj.html

TS:   structuredClone(obj)
来源：http://hz.yvedp.cn/gtaghiirtb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.nanxinkj.top/gtbseaepux.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.fzhhl.top/gtxkusioad.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.52xcode.cn/gtumkvdxvq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.havefunace.top/gtsbltvhmv.html


<!-- 参考信息 -->