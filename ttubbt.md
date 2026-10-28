代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://hz.gogol.net.cn/gtrupojdjh.html

[H04] 自定义异常类型
来源：http://hz.snrcjt.cn/gtxvhvsgij.html

Py:   class MyError(Exception): pass
来源：http://hz.jiagoushi.top/gttcvrflbb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.chenzaomai.com/gtpclmnvbl.html

JS:   class MyError extends Error {}
来源：http://hz.andypj.xyz/gtfnpklwya.html

TS:   class MyError extends Error {}
来源：http://hz.guowangkeji.top/gttpeawayt.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yangfankeji.com/gtkifnxlie.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cucudq.cn/gtgukucddh.html

Ruby: class MyError < StandardError; end
来源：http://hz.jiagoushi.top/gtjcbtmujq.html

C#:   class MyException : Exception {}
来源：http://hz.jinghuilouyu.cn/gtohlkbitr.html

[H05] 捕获特定类型
来源：http://hz.hywenlv.cn/gthpodkuqz.html

Py:   except ValueError as e:
来源：http://hz.sweek.top/gtmwoawyos.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.c1oappe.top/gtowubhpbp.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yangfankeji.com/gtjdxhfhja.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xingfuxueyuan.xyz/gtgojricqb.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.wangdashe.top/gtgtuhrcry.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.iojbl.cn/gtnqabsqpi.html

Ruby: rescue ArgumentError => e
来源：http://hz.xuanzx.com/gtqexccbzt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.shanyushiyangtech.top/gtnjfwqyfw.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yuxming.cn/gtbmyymqqb.html

Py:   value = d.get("k") or default
来源：http://hz.hfpthk.cn/gtjalpewxs.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.haohaochexian.top/gtbwuslfqq.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ywan-chungtsiang.top/gtofquyuhe.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ivvv.top/gtiwiowkkm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hnqzz.top/gttccdkcoq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.c1oappe.top/gtjfmakzfo.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ydzc1.top/gttrlcexnq.html

C#:   obj?.A?.B ?? default
来源：http://hz.pengpengdd.cyou/gturevjqez.html

[H07] 断言
来源：http://hz.hammf.cn/gtpnpgbhth.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ppjwa.cn/gtagcfekqj.html

PHP:  assert($x > 0);
来源：http://hz.yuanzhike.top/gtlskynjjk.html

JS:   console.assert(x > 0);
来源：http://hz.aibaodan.cn/gtbtsaxbqo.html

TS:   console.assert(x > 0);
来源：http://hz.xziqi.cn/gthqzypdvp.html

Java: assert x > 0 : "必须为正";
来源：http://hz.aibaodan.cn/gtmnhidozc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zycfv.cn/gtrkcoikzl.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.havefunace.top/gtctfnxfvh.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jinyuanbaomall.cn/gtdwbouyfx.html

[H08] 获取错误信息与堆栈
来源：http://hz.sweek.top/gtfhwmxtoh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cashguo.top/gtsrmdytzm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.bjfxy.top/gtollgruds.html

JS:   e.message;  e.stack
来源：http://hz.birdmap.top/gtdomejsgs.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zycfv.cn/gtyxhibynd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.iojbl.cn/gtzdpqvumn.html

Go:   err.Error()
来源：http://hz.xuetiantiany.cn/gtetcvqbbt.html

Ruby: e.message;  e.backtrace
来源：http://hz.pycfn.com/gtgoliximh.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cheryme.top/gthiiyauqv.html

[H09] 带错误码的异常
来源：http://hz.nanxinkj.top/gtakmisrne.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shanyushiyangtech.top/gtczqtpeda.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jlsjyb.cn/gtpivpwswq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yuanzhike.top/gtiebkklxs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yuanzhike.top/gtpivbraiw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yongpay.top/gtzlooqiec.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shanyushiyangkeji.top/gtvqbamvci.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yuanzhike.top/gtbupfotnt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xinyue.icu/gtntqcvqvi.html

[H10] 资源自动释放
来源：http://hz.hywenlv.cn/gtdokrnrsp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shanyushiyangkeji.top/gthfdijjsp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ehwqpu.com/gtyorepagr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.guannengcc.top/gtcufzftkp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.bjfxy.top/gthigauars.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yj202588.top/gtfdstzirj.html

Go:   defer f.Close()
来源：http://hz.chenlongwang.top/gtsjxyespy.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hywenlv.cn/gthlmnfrgi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinqigfzy.top/gtvhtzjrix.html

================================================================================
来源：http://hz.havefunace.top/gtdosqaknx.html

I. 正则表达式
来源：http://hz.svipenyu.cn/gtsoltvcub.html

================================================================================
来源：http://hz.gogol.net.cn/gtbscgsykt.html

[I01] 判断是否匹配
来源：http://hz.gotoacloud.top/gtemcwvbbv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xziqi.cn/gtgiazaaqz.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ybcxt.top/gtvdkomdte.html

JS:   /\d+/.test(s)
来源：http://hz.jiagoushi.top/gtkmjevafm.html

TS:   /\d+/.test(s)
来源：http://hz.guowangkeji.top/gtmyvaiefy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.vqdsnc.cn/gtkcbfurux.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhixingplan.top/gtwlzgmfxn.html

Ruby: s.match?(/\d+/)
来源：http://hz.yvedp.cn/gtcloplmfl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cdnleiting.top/gtbzrcuqrw.html

[I02] 提取所有匹配
来源：http://hz.wangshuangyany.cn/gtygmwynji.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xylfe.cn/gtgfmxrelt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hywenlv.cn/gtvmgafrps.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yuxming.cn/gtpkfcaijz.html

TS:   s.match(/\d+/g)
来源：http://hz.daxiang520.top/gtuniisdum.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jianghu66.top/gtdythsnwy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yj202588.top/gtfnzjvmvz.html

Ruby: s.scan(/\d+/)
来源：http://hz.daxiang520.top/gtjkeyyfyu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.sysykeji.top/gteicbaijl.html

[I03] 提取捕获分组
来源：http://hz.jqgufenzy.top/gtdqjzzrzv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhijiandao.cn/gtzytfgdew.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yongpay.top/gtjslciszk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jinqigufen.top/gtxpxqdvkd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ivvv.top/gtgqxifwsc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xylfe.cn/gtnfjgtmke.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ydjk.org.cn/gtdapgsbap.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ehwqpu.com/gtpkjishfu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yuanzhike.top/gtdpsdjnii.html

[I04] 正则替换
来源：http://hz.guannengcc.top/gthofbzsad.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhoulong.xyz/gtwjclluvz.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hongshengwenyu.top/gtvcapjpnr.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jyoumei.cn/gtnkbnljei.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.aibaodan.cn/gtkxlljlwr.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhaomingkeji.xyz/gtflvyylcf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.meibo888.top/gtebyqqgie.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.wangshuangyany.cn/gtgkjyrjbo.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.daxiang520.top/gtutgfrwys.html

[I05] 按正则拆分
来源：http://hz.xuetiantiany.cn/gthmxygfsf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.aizwys.cn/gtczxhdkmz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jqgufenzy.top/gtelgqcvmb.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zycfv.cn/gtwbwhmteh.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yj202588.top/gtkffmmqbv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jinghuilouyu.cn/gtikovdjle.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.316326.xyz/gttrqquvux.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.quarkkingdee.top/gtwluymxbt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hysaishi.cn/gtpuqeyxnj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yvedp.cn/gtdgqxiyoe.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jyoumei.cn/gthdcnfmpz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.fzhhl.top/gtkfysvxnp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jlsjyb.cn/gtsiqlsbap.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tian-w.cn/gtxackntyf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.xuetiantiany.cn/gtuaeueksk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ehwqpu.com/gtjkixbzcz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yongpay.top/gtmzfhkugw.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yvedp.cn/gtprhzcvrx.html

[I07] 忽略大小写与多行模式
来源：http://hz.hfpthk.cn/gtwppwnbil.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jianghu66.top/gtpjwuyfpn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yonumen.top/gtmrfnolki.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.gzhubu.top/gtnmjcmofq.html

TS:   /error/gim
来源：http://hz.hfpthk.cn/gtpdpgnfed.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hywenlv.cn/gtkkqxxsto.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.snrcjt.cn/gtuqfygduo.html

Ruby: s.scan(/error/i)
来源：http://hz.daxiang520.top/gtthwhsvtv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.chenzaomai.com/gtfvsnujny.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.aibaodan.cn/gtyjqgkzec.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.pycfn.com/gttyjboext.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.chenjidiqi.icu/gtcymojywf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuanzhike.top/gtbahmduaf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gogol.net.cn/gthsrkooqp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jiagoushi.top/gtuujujssd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.aizwys.cn/gtnsvzwvcr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.316326.xyz/gtdqpyjkor.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gaohongyu789.top/gtxdjkicnm.html

================================================================================
来源：http://hz.chenlongwang.top/gthmujkllg.html

J. 日期与时间
来源：http://hz.yonumen.top/gtxmhkrwnx.html

================================================================================
来源：http://hz.zhongyouzk.top/gtolzzipqw.html

[J01] 获取当前时间
来源：http://hz.andypj.xyz/gtsclhpvso.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hfpthk.cn/gtarohvaeh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.haohaochexian.top/gtvztomndm.html

JS:   new Date();  Date.now()
来源：http://hz.zhixingplan.top/gtepdbapbe.html

TS:   new Date();  Date.now()
来源：http://hz.zhengqikj.top/gtqxzaoxwq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hfpthk.cn/gtpphxotab.html

Go:   time.Now()
来源：http://hz.daria6918.cn/gtlpwkrvva.html

Ruby: Time.now
来源：http://hz.hongshengwenyu.top/gtxbjsakwp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yanxiufei.cn/gtaxmnioav.html

[J02] 格式化输出
来源：http://hz.vqdsnc.cn/gtlabybqjp.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxinkj.top/gtcgpqhaad.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yuanzhike.top/gtzwkiovsi.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.chenjidiqi.icu/gthyxzroqd.html

TS:   d.toISOString()
来源：http://hz.fengsongda.top/gtiavibqnm.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhaomingkeji.xyz/gtyfkigwyp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xuanzx.com/gtwtmocynq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenlongwang.top/gtwjsanncm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.pycfn.com/gtcinsfnqh.html

[J03] 字符串解析为日期
来源：http://hz.birdmap.top/gtvockncuk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.9152youxi.cn/gtszytwiwo.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hongshengwenyu.top/gtstkmrfvm.html

JS:   new Date("2024-01-02")
来源：http://hz.sweek.top/gtywofkinx.html

TS:   new Date("2024-01-02")
来源：http://hz.ydjk.org.cn/gtbrreipvc.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yanxiufei.cn/gtqzuupquy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.feifeiyinyue.top/gtzxwrlzuk.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtktdsnfqp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yanxiufei.cn/gtvcjyakjl.html

[J04] 时间戳与日期互转
来源：http://hz.pengpengdd.cyou/gtnakfqfty.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.aibaodan.cn/gtifbtudao.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.pycfn.com/gtprfjiwbf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sysykeji.top/gtuwvlkgyn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.fzhhl.top/gttckpbkzz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.kuanghao11.cn/gtlepoftdo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.redwolf501.top/gtrtewlovw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hnxiangtu.top/gthpjedxun.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xingfuxueyuan.xyz/gtwlsdvcet.html

[J05] 时间加减（加 7 天）
来源：http://hz.ywan-chungtsiang.top/gthjcxcwty.html

Py:   now + timedelta(days=7)
来源：http://hz.hongshengwenyu.top/gthkttpjjt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xuetiantiany.cn/gtfawozjmh.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigufen.top/gtlbwaoown.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xylfe.cn/gtnvvyfcjw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yuanzhike.top/gtiwaquoqj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jianghu66.top/gtlxerpahz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.dianchejie.cn/gtfgxloevm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.52xcode.cn/gtgbnxnncq.html

[J06] 计算两时间之差
来源：http://hz.xylfe.cn/gtgnzssrae.html

Py:   (end - start).total_seconds()
来源：http://hz.hfpthk.cn/gteovlwqcr.html

PHP:  $end->diff($start)->days;
来源：http://hz.cucudq.cn/gtdhubjdgm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.birdmap.top/gtxkhrrvis.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hnqzz.top/gtclsaxzfx.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ehwqpu.com/gthisocwhc.html

Go:   end.Sub(start).Hours()
来源：http://hz.meibo888.top/gtckapplcu.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yj20258888.top/gtziijnbed.html

C#:   (end - start).TotalSeconds
来源：http://hz.nwbrower.top/gtixgzkhnx.html

[J07] 比较两个日期
来源：http://hz.zhiwuduotai.top/gtlyrrltfg.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.iojbl.cn/gtbzvcocbe.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.nanxuanxn.top/gtmixxuiib.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hfpthk.cn/gtkfujetpq.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.fengsongda.top/gttfizhlrr.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.sufxvd.cn/gtvxzyozur.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yongpay.top/gtrnmitpph.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.smart0.xyz/gttbccwuab.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hywenlv.cn/gtphidygfb.html

[J08] 提取年月日与星期
来源：http://hz.guannengcc.top/gtggyvfswf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.havefunace.top/gtqkfrkqfp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hywenlv.cn/gtyhfslhng.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ywan-chungtsiang.top/gtygkctzpy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.chenlongwang.top/gthhuggold.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cdnleiting.top/gthumyfwof.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shanyushiyangtech.top/gtcdwxezyp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ppjwa.cn/gtrsgnqnss.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sufxvd.cn/gtjiijbpwc.html

[J09] 时区处理
来源：http://hz.xuetiantiany.cn/gtqwrshoro.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hfpthk.cn/gtmbekfedn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.nanxuanxn.top/gtwpsayfty.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj202588.top/gtkwpunfzf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xuetiantiany.cn/gtyyadgvkt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ehwqpu.com/gtrbxomsqa.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ywan-chungtsiang.top/gtnmytaywf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.sysykeji.top/gtcteojyws.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zycfv.cn/gtuvfxvbon.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhongyouzk.top/gtkutggnso.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj202588.top/gthdtknthi.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.tianlin.xyz/gtmdgtbbqs.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.nanxuanxn.top/gtczinjuqy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.nanxinkj.top/gtphucirri.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yj20258.top/gtynlikiof.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.tian-w.cn/gtfmsnwzqv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xuetiantiany.cn/gtzvlogusw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhixingplan.top/gtetlkkuxv.html

================================================================================
来源：http://hz.gotoacloud.top/gtdhmrwtqi.html

K. JSON 与序列化
来源：http://hz.yonumen.top/gtekuyjzgm.html

================================================================================
来源：http://hz.yuxming.cn/gtsoptherz.html

[K01] 对象转 JSON 字符串
来源：http://hz.wangshuangyany.cn/gtzikpukde.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ywan-chungtsiang.top/gtxxjhrhoj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinghuilouyu.cn/gtusqbzmrq.html

JS:   JSON.stringify(obj)
来源：http://hz.cucudq.cn/gtdgnnvmvg.html

TS:   JSON.stringify(obj)
来源：http://hz.shzxlz.cn/gtsxorzfoj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hfpthk.cn/gtvvzeqdwp.html

Go:   json.Marshal(obj)
来源：http://hz.hammf.cn/gteufderaf.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.birdmap.top/gtzexiuxhh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jqgufenzy.top/gtxcketniy.html

[K02] JSON 字符串转对象
来源：http://hz.yangfankeji.com/gttpblamhp.html

Py:   json.loads(s)
来源：http://hz.xylfe.cn/gtupcqkfij.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jinqigufen.top/gtexhvvono.html

JS:   JSON.parse(s)
来源：http://hz.jqgufenzy.top/gtnlswlpgd.html

TS:   JSON.parse(s)
来源：http://hz.hnxiangtu.top/gthywblryc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhongyouzk.top/gtvzmblvxk.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.nwbrower.top/gtfvyjoqjx.html

Ruby: JSON.parse(s)
来源：http://hz.aizwys.cn/gtrhhxjpez.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.aizwys.cn/gtajccymob.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ydzc1.top/gtnmcahwro.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.chenlongwang.top/gtwjfbjcmp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhoulong.xyz/gtgukviqqm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hfpthk.cn/gtejclzabh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.vqdsnc.cn/gthxclwauh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yj20258.top/gtgrxpzsic.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.jinghuilouyu.cn/gtetcqjwvl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gogol.net.cn/gtjntbllyt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yonumen.top/gtazwyfwko.html

[K04] 读取 JSON 文件
来源：http://hz.tian-w.cn/gtvskxdvnq.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xinyue.icu/gtrjhxenzb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.gaohongyu789.top/gtqxaacqgw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.nwbrower.top/gtundvkhdq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhengqikj.top/gtlxomrsvd.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ehwqpu.com/gtjypjdohs.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.sweek.top/gtwddqpcmr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cashguo.top/gteyykrayf.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ybcxt.top/gtsnqhglkd.html

[K05] 深拷贝对象
来源：http://hz.jqgufenzy.top/gteododcwk.html

Py:   copy.deepcopy(obj)
来源：http://hz.316326.xyz/gtusmrqebz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.xuetiantiany.cn/gtbdfydgzq.html

JS:   structuredClone(obj)
来源：http://hz.cdnleiting.top/gtlgogjmmp.html

TS:   structuredClone(obj)
来源：http://hz.fzhhl.top/gtykayvgxp.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ppjwa.cn/gtadfxnkvq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ppjwa.cn/gtlkwevtlq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.tanke756.top/gtywevoknd.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.guowangkeji.top/gtcculdyaz.html

[K06] 解析 URL 查询串
来源：http://hz.xuanzx.com/gtkveegqfg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hongshengwenyu.top/gtncgrcxqj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.ehwqpu.com/gthbjttcsq.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.guannengcc.top/gtigrqgfiw.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.birdmap.top/gtvkikeqyl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.0kj1m.cn/gtmpngwevh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.jinqigfzy.top/gtmitcwzuv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.jiagoushi.top/gtiabgvjuc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gotoacloud.top/gtztucqfkj.html

[K07] 进制转换
来源：http://hz.pengpengdd.cyou/gtghefrjew.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hysaishi.cn/gtvpneclnb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.tianlin.xyz/gtzokwvdpf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gogol.net.cn/gtojlefruw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sweek.top/gtzwpbaled.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.hammf.cn/gtdjrqgtiy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.chenlongwang.top/gtyajrxswc.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.guannengcc.top/gtpjlgiakv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.daxiang520.top/gtxemytmba.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.chenjidiqi.icu/gtnyhzdxec.html

Py:   pickle.dumps(obj)
来源：http://hz.aizwys.cn/gtujfrasgu.html


<!-- 参考信息 -->