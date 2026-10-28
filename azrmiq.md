代发 wailian999

TS:   throw new Error("错误信息");
来源：http://hz.dianchejie.cn/gtcswpxnfz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yuxming.cn/gttfnswcxd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yj20258888.top/gtmsyugujk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.mhx1999.top/gtfuzxsnyu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.vqdsnc.cn/gtmwfpnlqg.html

[H04] 自定义异常类型
来源：http://hz.yongpay.top/gtlfzuemyz.html

Py:   class MyError(Exception): pass
来源：http://hz.jinyuanbaomall.cn/gtaoimpmaj.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.birdmap.top/gtexzraodo.html

JS:   class MyError extends Error {}
来源：http://hz.kuanghao11.cn/gtarndashx.html

TS:   class MyError extends Error {}
来源：http://hz.smart0.xyz/gtyxxunkbm.html

Java: class MyException extends RuntimeException {}
来源：http://hz.havefunace.top/gtgfsechem.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.meibo888.top/gtrwfkfnxu.html

Ruby: class MyError < StandardError; end
来源：http://hz.kuanghao11.cn/gtlwvabltr.html

C#:   class MyException : Exception {}
来源：http://hz.9152youxi.cn/gtjnwekdeb.html

[H05] 捕获特定类型
来源：http://hz.chenlongwang.top/gtvsjywsnf.html

Py:   except ValueError as e:
来源：http://hz.jinyuanbaomall.cn/gtgljapdab.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ydjk.org.cn/gtnaqdhvej.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.snrcjt.cn/gtmipjnbuq.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangkeji.top/gtjudcigid.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.tian-w.cn/gtgobrbyan.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hnqzz.top/gtpvyakonn.html

Ruby: rescue ArgumentError => e
来源：http://hz.aizwys.cn/gtskiqwbgr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xinyue.icu/gtbuhquriz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jinghuilouyu.cn/gtipueewjw.html

Py:   value = d.get("k") or default
来源：http://hz.chenlongwang.top/gtypgdsbvp.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cashguo.top/gttncxxyyp.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sxryk.cn/gtprdcrjum.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sxryk.cn/gtavjikloa.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xuanzx.com/gttaanarmv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.smart0.xyz/gtrbmdrsrj.html

Ruby: d&.dig(:a, :b)
来源：http://hz.316326.xyz/gtojmilvcr.html

C#:   obj?.A?.B ?? default
来源：http://hz.jlsjyb.cn/gtyvbwkuri.html

[H07] 断言
来源：http://hz.cheryme.top/gtvjsmsgmq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hysaishi.cn/gtiworwzem.html

PHP:  assert($x > 0);
来源：http://hz.cheryme.top/gtbiqynlxf.html

JS:   console.assert(x > 0);
来源：http://hz.cdnleiting.top/gtcspvknvu.html

TS:   console.assert(x > 0);
来源：http://hz.ehwqpu.com/gtytkvmmip.html

Java: assert x > 0 : "必须为正";
来源：http://hz.svipenyu.cn/gteyjigxvh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhaomingkeji.xyz/gtelevmehy.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sysykeji.top/gtkkayfecz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shzxlz.cn/gtwxibubxk.html

[H08] 获取错误信息与堆栈
来源：http://hz.chenlongwang.top/gtgqqwhwys.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yj20258888.top/gtrfpjjjbh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gogol.net.cn/gtfprllqzy.html

JS:   e.message;  e.stack
来源：http://hz.pycfn.com/gtpnmyvsbf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shuidangran.top/gtjzlhhezt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.wangdashe.top/gtiunwjmmg.html

Go:   err.Error()
来源：http://hz.fengsongda.top/gtwyvvhaph.html

Ruby: e.message;  e.backtrace
来源：http://hz.c1oappe.top/gtbzhxsjtj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.0kj1m.cn/gtzgdyjpel.html

[H09] 带错误码的异常
来源：http://hz.tian-w.cn/gtovzlfoyo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yj202588.top/gtwakcfeho.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.daxiang520.top/gtxuetkaob.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xingfuxueyuan.xyz/gtopmllqgg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.9152youxi.cn/gtekcfxmyp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.snrcjt.cn/gtxaotzfbz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jlsjyb.cn/gtiltvczja.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.pycfn.com/gtymrtaxut.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shanyushiyangkeji.top/gtvqyliali.html

[H10] 资源自动释放
来源：http://hz.hywenlv.cn/gtxntbwyoh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.tianlin.xyz/gtwhtkhqjk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.pengpengdd.cyou/gtkyettvje.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ywan-chungtsiang.top/gtewgochqf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigfzy.top/gtyagdxmcb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yongpay.top/gtvdwyzaoz.html

Go:   defer f.Close()
来源：http://hz.yuanzhike.top/gthjlkkexx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yuanzhike.top/gtogqoskak.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ivvv.top/gtvttwmkrk.html

================================================================================
来源：http://hz.ybcxt.top/gtlhfgmpvu.html

I. 正则表达式
来源：http://hz.hongshengwenyu.top/gtcymtxeit.html

================================================================================
来源：http://hz.pycfn.com/gtuqlvqmkw.html

[I01] 判断是否匹配
来源：http://hz.zhengqikj.top/gtxnwjbxqj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yj202588.top/gterhfpxuz.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.shzxlz.cn/gtqwlypqsy.html

JS:   /\d+/.test(s)
来源：http://hz.yueranfly.top/gthqrcvdhn.html

TS:   /\d+/.test(s)
来源：http://hz.jyoumei.cn/gtgevyftlu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.nwbrower.top/gtqqynrtcc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jlsjyb.cn/gtmrqxvecs.html

Ruby: s.match?(/\d+/)
来源：http://hz.ivvv.top/gthplcehil.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cheryme.top/gtythccnbq.html

[I02] 提取所有匹配
来源：http://hz.vqdsnc.cn/gtnidcicov.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yj20258.top/gtjkfwswjn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhijiandao.cn/gtctdfihwk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.smart0.xyz/gtovpnqlhr.html

TS:   s.match(/\d+/g)
来源：http://hz.shanyushiyangkeji.top/gtriumyipq.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jqgfzy.top/gtfkynuoqa.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.svipenyu.cn/gtfwqdvjvs.html

Ruby: s.scan(/\d+/)
来源：http://hz.zycfv.cn/gtbovwfalo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cucudq.cn/gtflvllkgl.html

[I03] 提取捕获分组
来源：http://hz.ybcxt.top/gtamefxodw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.haohaochexian.top/gtrkpkdprf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.tian-w.cn/gtsivmmhrn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.meibo888.top/gtsbphkpfu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.fzhhl.top/gtltnglseb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.snrcjt.cn/gtizlzcyix.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nwbrower.top/gtmunsvcoy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shanyushiyangkeji.top/gtfylavcfn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zycfv.cn/gthtcsoumh.html

[I04] 正则替换
来源：http://hz.9152youxi.cn/gtyoxsthnn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.svipenyu.cn/gtfhukanhs.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhoulong.xyz/gtdxpuacha.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yonumen.top/gthxtajepj.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shzxlz.cn/gtoagahhlq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jqgfzy.top/gtvccudvqp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.gaohongyu789.top/gtktvtwpew.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.sweek.top/gtocxijxlr.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.chenjidiqi.icu/gtcuwypmrs.html

[I05] 按正则拆分
来源：http://hz.wangshuangyany.cn/gtfosikwot.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.chenlongwang.top/gtjcktloem.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhijiandao.cn/gtvxvegyjt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yuxming.cn/gthsmfnpdd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jqgufenzy.top/gtqxobwobe.html

Java: s.split("\\s*,\\s*")
来源：http://hz.smart0.xyz/gtwnmptzau.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.vqdsnc.cn/gtefwglrzl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj20258888.top/gtdrtnoycp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cdnleiting.top/gtdufnfgpy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.bjfxy.top/gtjvhrdpyc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ydjk.org.cn/gttyettymk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sxryk.cn/gtfqfrtyej.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.svipenyu.cn/gtxxnyejea.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.feifeiyinyue.top/gtxdikjafq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yangfankeji.com/gtokvtythf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yj202588.top/gtzdnmxhmw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.smart0.xyz/gtkrxiknmy.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.daxiang520.top/gtuspqnoad.html

[I07] 忽略大小写与多行模式
来源：http://hz.hnxiangtu.top/gtunsbodse.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.aizwys.cn/gtfqwqptyu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yangfankeji.com/gtobytaxge.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.aizwys.cn/gtjqjyhtdb.html

TS:   /error/gim
来源：http://hz.gzhubu.top/gtkhqzuzmd.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shanyushiyangkeji.top/gtcsgffpxx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gzhubu.top/gtqvwblmud.html

Ruby: s.scan(/error/i)
来源：http://hz.c1oappe.top/gtarrxlcxy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gaohongyu789.top/gtfbdorqqb.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.chenlongwang.top/gtpyrlpcbx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.guowangkeji.top/gthcjfffxq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinqigufen.top/gtzktjjstf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aibaodan.cn/gtaxacszyn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nanxinkj.top/gtqijdlbmm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xuetiantiany.cn/gtlwpiwdbz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hysaishi.cn/gtyscxasrq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shzxlz.cn/gtmrrozrfe.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhengqikj.top/gtytbczrmo.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtljlqggra.html

J. 日期与时间
来源：http://hz.ydzc1.top/gtilkevcua.html

================================================================================
来源：http://hz.zycfv.cn/gtmryxgiqt.html

[J01] 获取当前时间
来源：http://hz.yvedp.cn/gtpfbxrvnx.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xingfuxueyuan.xyz/gtonxwswqi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jinqigufen.top/gtkhcbhanf.html

JS:   new Date();  Date.now()
来源：http://hz.guannengcc.top/gtnpetfhlm.html

TS:   new Date();  Date.now()
来源：http://hz.jiagoushi.top/gtdpsudhtl.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jiagoushi.top/gtluojyurx.html

Go:   time.Now()
来源：http://hz.jianghu66.top/gtqjhvynfl.html

Ruby: Time.now
来源：http://hz.yj202588.top/gtkvehhrkc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yanxiufei.cn/gtsnupwbsu.html

[J02] 格式化输出
来源：http://hz.gogol.net.cn/gtfpovmnir.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yuanzhike.top/gthfjwbflp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.aizwys.cn/gtuyasljmg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jqgfzy.top/gtvyuhxrbh.html

TS:   d.toISOString()
来源：http://hz.snrcjt.cn/gtnncbhwfx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zdqjudy.top/gtfxbitkmm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cucudq.cn/gtvcktpcuf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinqigfzy.top/gtsutynela.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jqgufenzy.top/gtzehwkpps.html

[J03] 字符串解析为日期
来源：http://hz.sufxvd.cn/gtoqeutebu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.52xcode.cn/gtfpaxmwrw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.tianlin.xyz/gthoyorcov.html

JS:   new Date("2024-01-02")
来源：http://hz.cucudq.cn/gtdqjlfuux.html

TS:   new Date("2024-01-02")
来源：http://hz.316326.xyz/gtzxfazklx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zhengqikj.top/gtfsgqjyej.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.316326.xyz/gtkmbkxnkz.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.meibo888.top/gtenkmpeuc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hfpthk.cn/gtgprzdqfr.html

[J04] 时间戳与日期互转
来源：http://hz.iojbl.cn/gtcjxniicg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jqgfzy.top/gtvasefsuq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.aibaodan.cn/gtmfsdzugi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.nanxinkj.top/gtknqafcxk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ydzc1.top/gtcdjpehzl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.pycfn.com/gtfusvgajr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.daria6918.cn/gtbrqtechc.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jqgufenzy.top/gtcdurqhee.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yj202588.top/gtnswsknbe.html

[J05] 时间加减（加 7 天）
来源：http://hz.jqgufenzy.top/gtrdtzyfik.html

Py:   now + timedelta(days=7)
来源：http://hz.yvedp.cn/gtasftnsdf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.feifeiyinyue.top/gtsjfdkupo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.svipenyu.cn/gtjoannqdv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnxiangtu.top/gtxxtftzkq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.havefunace.top/gtawyxpgje.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hfpthk.cn/gtbygnaepx.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinqigufen.top/gtvuuwhtrl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.svipenyu.cn/gtdiryoyde.html

[J06] 计算两时间之差
来源：http://hz.bjfxy.top/gthipoqhbi.html

Py:   (end - start).total_seconds()
来源：http://hz.hywenlv.cn/gtuwwhzsdt.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhijiandao.cn/gtepadprzb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.aizwys.cn/gtrnvopnnz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hywenlv.cn/gtfclttqjs.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ivvv.top/gtociopbii.html

Go:   end.Sub(start).Hours()
来源：http://hz.andypj.xyz/gtnoicgajk.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gogol.net.cn/gtoemvozaa.html

C#:   (end - start).TotalSeconds
来源：http://hz.jinqigufen.top/gtmfqpdyuj.html

[J07] 比较两个日期
来源：http://hz.xingfuxueyuan.xyz/gtwgjpzpdd.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangkeji.top/gtckehnzsw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.redwolf501.top/gtnlsxhrrp.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shuidangran.top/gtzkxoymgw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ydzc1.top/gtnbipqvdv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.wangshuangyany.cn/gtzfdogapg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.bjfxy.top/gtscorythm.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhengqikj.top/gtpboqladc.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhaomingkeji.xyz/gtijkianyr.html

[J08] 提取年月日与星期
来源：http://hz.aizwys.cn/gtwtkeycch.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.fzhhl.top/gtrmyvjbms.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xinyue.icu/gtlcafazxm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hfpthk.cn/gtgekpziln.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.aizwys.cn/gtignwupou.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.daria6918.cn/gtzbbxcjht.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shanyushiyangkeji.top/gtgzomcxcw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.wangshuangyany.cn/gtrauqsbky.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinqigfzy.top/gtirabddit.html

[J09] 时区处理
来源：http://hz.sxryk.cn/gtczbxhkhd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ybcxt.top/gtdajsvzsi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.aibaodan.cn/gthfuhogpv.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tian-w.cn/gtpkqdatxb.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ybcxt.top/gtydoeijfy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hywenlv.cn/gtznzwoplq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ehwqpu.com/gtgromyolp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.redwolf501.top/gtxzepxdns.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jianghu66.top/gtyjerbska.html

[J10] 取今天 / 本月第一天
来源：http://hz.iojbl.cn/gtdxyceffu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sufxvd.cn/gthgekmymm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jianghu66.top/gtxabncnbc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.chenjidiqi.icu/gtcrryrogg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinghuilouyu.cn/gtxgnffmkg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.dashuyun.cn/gtcfexpcjd.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shangyingyoupin.top/gtdcslivzr.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jqgufenzy.top/gtvaqmvclz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jiagoushi.top/gtcmrxtgtd.html

================================================================================
来源：http://hz.gzhubu.top/gtxuvvzwlv.html

K. JSON 与序列化
来源：http://hz.mhx1999.top/gtdsfdkvvm.html

================================================================================
来源：http://hz.cashguo.top/gtwenlhenj.html

[K01] 对象转 JSON 字符串
来源：http://hz.shanyushiyangkeji.top/gtqulpcuuz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ehwqpu.com/gtkokpyxsy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.redwolf501.top/gtemqruqfl.html

JS:   JSON.stringify(obj)
来源：http://hz.tian-w.cn/gtcumwfbnk.html

TS:   JSON.stringify(obj)
来源：http://hz.bjfxy.top/gtbpilthqp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.aizwys.cn/gtfistkmam.html

Go:   json.Marshal(obj)
来源：http://hz.ivvv.top/gtfnmgehfl.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shangyingyoupin.top/gtajnqfxek.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cucudq.cn/gtfbdezfrf.html

[K02] JSON 字符串转对象
来源：http://hz.xuetiantiany.cn/gtxgjudwfr.html

Py:   json.loads(s)
来源：http://hz.ivvv.top/gtttfbeudh.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.fengsongda.top/gtipeiyfcf.html

JS:   JSON.parse(s)
来源：http://hz.jiagoushi.top/gtivsobfhr.html

TS:   JSON.parse(s)
来源：http://hz.chenlongwang.top/gtzdmaxnwr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yonumen.top/gttbclqfhj.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cdnleiting.top/gtgmyhizhe.html

Ruby: JSON.parse(s)
来源：http://hz.wangdashe.top/gtkbmjjhex.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.tian-w.cn/gtslrlyhwb.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ydzc1.top/gtbynrwagg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.xuanzx.com/gtphczswrx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jyoumei.cn/gtwjihkyvz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.nanxinkj.top/gtvfusokwd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.daxiang520.top/gtgifpciht.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hnqzz.top/gtqhfjsexf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.wangdashe.top/gtsqshmnay.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xingfuxueyuan.xyz/gtkfiuxefb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xinyue.icu/gtlafwebtj.html

[K04] 读取 JSON 文件
来源：http://hz.kuanghao11.cn/gtlzjvzafm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.cashguo.top/gtypujamij.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yongpay.top/gtnslfheya.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.0kj1m.cn/gtkjgdesov.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnxiangtu.top/gtmbubohhd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.fzhhl.top/gtqxnssiyn.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.snrcjt.cn/gtewvmtndv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shzxlz.cn/gtjaicsphm.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jinqigufen.top/gtjzmmhnxw.html

[K05] 深拷贝对象
来源：http://hz.gogol.net.cn/gtglfoxkwi.html

Py:   copy.deepcopy(obj)
来源：http://hz.shuidangran.top/gtwpozjpgq.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hnqzz.top/gtkkxaipug.html

JS:   structuredClone(obj)
来源：http://hz.xylfe.cn/gtoocleuuq.html

TS:   structuredClone(obj)
来源：http://hz.tanke756.top/gtghwzjhwb.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.redwolf501.top/gthzxltpph.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.haohaochexian.top/gtvjcxthwu.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yvedp.cn/gtatyjwrsz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.snrcjt.cn/gtsmhxggys.html

[K06] 解析 URL 查询串
来源：http://hz.tanke756.top/gtqesijnjr.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cashguo.top/gteldfdylp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hysaishi.cn/gttarlixxk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhiwuduotai.top/gtdtxpbjft.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuxming.cn/gtbamdoxib.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.daria6918.cn/gtfpmidjsd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.dashuyun.cn/gtoqtqynis.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ehwqpu.com/gtxzumsofk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.hywenlv.cn/gtwcoikoyq.html

[K07] 进制转换
来源：http://hz.hnxiangtu.top/gtycgzsloo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.havefunace.top/gtornyuwdf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shanyushiyangkeji.top/gttnwvladb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yonumen.top/gthqkwfndy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.iojbl.cn/gtvjpeshvq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hysaishi.cn/gtawigheqj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xingfuxueyuan.xyz/gtlthdrbcl.html


<!-- 参考信息 -->