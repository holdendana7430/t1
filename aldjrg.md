代发 wailian999

[H03] 主动抛出异常
来源：http://hz.aibaodan.cn/gtwvaxoxpx.html

Py:   raise ValueError("错误信息")
来源：http://hz.meibo888.top/gtuezfxgfo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.chenzaomai.com/gtxkkchuhy.html

JS:   throw new Error("错误信息");
来源：http://hz.hongshengwenyu.top/gtmwrskkxm.html

TS:   throw new Error("错误信息");
来源：http://hz.shzxlz.cn/gtnluyldbu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cucudq.cn/gtkkzqkztb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ywan-chungtsiang.top/gtzakrkvko.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shanyushiyangtech.top/gtitckgtpw.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.svipenyu.cn/gtjvkammhp.html

[H04] 自定义异常类型
来源：http://hz.jinqigfzy.top/gtfqgghvzb.html

Py:   class MyError(Exception): pass
来源：http://hz.ydzc1.top/gticdxzxwl.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.0kj1m.cn/gteyeeyltf.html

JS:   class MyError extends Error {}
来源：http://hz.quarkkingdee.top/gthwhkmwth.html

TS:   class MyError extends Error {}
来源：http://hz.dianchejie.cn/gtcdweyfll.html

Java: class MyException extends RuntimeException {}
来源：http://hz.dianchejie.cn/gtuloyhkmd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.andypj.xyz/gtzzvtstkt.html

Ruby: class MyError < StandardError; end
来源：http://hz.cucudq.cn/gtzdanoijj.html

C#:   class MyException : Exception {}
来源：http://hz.sxryk.cn/gtjqgfaepo.html

[H05] 捕获特定类型
来源：http://hz.hywenlv.cn/gtsjdvefsx.html

Py:   except ValueError as e:
来源：http://hz.chenjidiqi.icu/gtbmnvcwzo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jinyuanbaomall.cn/gtukzwmctv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.9152youxi.cn/gtibcsdcyk.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sysykeji.top/gtvogubdev.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jlsjyb.cn/gtgduquuph.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ppjwa.cn/gtqebyzcqt.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj20258.top/gtekwdsusl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jlsjyb.cn/gtwuibjzuz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shzxlz.cn/gtzshzycwt.html

Py:   value = d.get("k") or default
来源：http://hz.jinyuanbaomall.cn/gtwmhvyzgs.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ehwqpu.com/gtiaqaitvx.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gotoacloud.top/gtcvbkioqh.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yuanzhike.top/gteoswwdad.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zdqjudy.top/gtssywtrcg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.nwbrower.top/gthndfdboa.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ppjwa.cn/gtqejjzivk.html

C#:   obj?.A?.B ?? default
来源：http://hz.gogol.net.cn/gtysdlwvkl.html

[H07] 断言
来源：http://hz.guowangkeji.top/gtsionmrmj.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj20258.top/gtyxznfkqk.html

PHP:  assert($x > 0);
来源：http://hz.jlsjyb.cn/gthkemhxmy.html

JS:   console.assert(x > 0);
来源：http://hz.xziqi.cn/gtnacsqpuc.html

TS:   console.assert(x > 0);
来源：http://hz.0kj1m.cn/gtttqabidi.html

Java: assert x > 0 : "必须为正";
来源：http://hz.aibaodan.cn/gtamzdkeqe.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhaomingkeji.xyz/gtppmttnuk.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sxryk.cn/gtljpdaxir.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jinqigufen.top/gtwjxokvbv.html

[H08] 获取错误信息与堆栈
来源：http://hz.chenzaomai.com/gtrxefwjvq.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.redwolf501.top/gtmahympos.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.daxiang520.top/gtakzebldf.html

JS:   e.message;  e.stack
来源：http://hz.smart0.xyz/gtevjxbnox.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cashguo.top/gtsrghectb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yuanzhike.top/gtlnjlxxma.html

Go:   err.Error()
来源：http://hz.havefunace.top/gtbocevfvt.html

Ruby: e.message;  e.backtrace
来源：http://hz.xingfuxueyuan.xyz/gtjnszbxee.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tianlin.xyz/gtxuddenpf.html

[H09] 带错误码的异常
来源：http://hz.havefunace.top/gtpxwdqeqg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xuanzx.com/gtfyqzmivb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.wangdashe.top/gtmsiyhszt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.9152youxi.cn/gtkffaqhxc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shzxlz.cn/gthidnkxto.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gzhubu.top/gtbegdwwmc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shuidangran.top/gtgdnkttmw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.aizwys.cn/gtpiegyrln.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhongyouzk.top/gttzdwrhwc.html

[H10] 资源自动释放
来源：http://hz.xziqi.cn/gtdphwovep.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yanxiufei.cn/gtdquaynsn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhoulong.xyz/gtvcpcsmig.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aibaodan.cn/gtvbcmrehb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenjidiqi.icu/gtgkczhkdw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ydzc1.top/gtnxdopqeq.html

Go:   defer f.Close()
来源：http://hz.zhixingplan.top/gtnlpjoepu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jianghu66.top/gtbgqswpkn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.svipenyu.cn/gtqoxdpbgl.html

================================================================================
来源：http://hz.chenzaomai.com/gtkieodkgl.html

I. 正则表达式
来源：http://hz.smart0.xyz/gtqhtporqb.html

================================================================================
来源：http://hz.ydjk.org.cn/gthcsitylg.html

[I01] 判断是否匹配
来源：http://hz.sufxvd.cn/gtpraknetw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.smart0.xyz/gtphzrbovc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cdnleiting.top/gtzamfqkgx.html

JS:   /\d+/.test(s)
来源：http://hz.zhongyouzk.top/gtujcqmjhk.html

TS:   /\d+/.test(s)
来源：http://hz.wangshuangyany.cn/gtpmmvbhus.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hfpthk.cn/gtvqpphcar.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jyoumei.cn/gtxuhhtpbv.html

Ruby: s.match?(/\d+/)
来源：http://hz.aizwys.cn/gtytlrwaag.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yanxiufei.cn/gtaroeizuz.html

[I02] 提取所有匹配
来源：http://hz.mhx1999.top/gtbcgizsqk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.fengsongda.top/gtoxrlptxc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hongshengwenyu.top/gtlyoavsxv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.aizwys.cn/gtpuvhxzgy.html

TS:   s.match(/\d+/g)
来源：http://hz.birdmap.top/gtfugnandv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ydjk.org.cn/gtytrkurka.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.mhx1999.top/gtvltvtgch.html

Ruby: s.scan(/\d+/)
来源：http://hz.andypj.xyz/gtyxqwdezf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.daria6918.cn/gtlaueraoe.html

[I03] 提取捕获分组
来源：http://hz.yangfankeji.com/gtxonsmhhy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ivvv.top/gtupqfcefr.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zdqjudy.top/gtecxnivxz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.dashuyun.cn/gtsplgqmer.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jyoumei.cn/gtpjznwqxo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.pengpengdd.cyou/gtngxlpzkb.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ydzc1.top/gtokfmbuoo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sxryk.cn/gtfbbukcrl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jqgufenzy.top/gtfzzjtjeu.html

[I04] 正则替换
来源：http://hz.zdqjudy.top/gtilhlqxes.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zdqjudy.top/gtoirwhxit.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xuetiantiany.cn/gtheabewui.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ydzc1.top/gtsefmyafz.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhiwuduotai.top/gtdqdmxcdm.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.fzhhl.top/gtwocltmhu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.aibaodan.cn/gtrxzccdni.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gaohongyu789.top/gtabpefeoz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.guowangkeji.top/gtapqlfbve.html

[I05] 按正则拆分
来源：http://hz.ppjwa.cn/gtzpyhwwos.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.aizwys.cn/gtjojgokbq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.wangshuangyany.cn/gtzgqevcrt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.xziqi.cn/gtffxofwgf.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.fengsongda.top/gtenakuddh.html

Java: s.split("\\s*,\\s*")
来源：http://hz.dashuyun.cn/gtdpxmxrin.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.sysykeji.top/gtuqcccdqt.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.fengsongda.top/gtxdqwpxae.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jlsjyb.cn/gtwtftaanj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xuanzx.com/gtbdcasbhm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhiwuduotai.top/gtuxnbdgkx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hywenlv.cn/gtvjpdupux.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258.top/gtfpfpjtwl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.andypj.xyz/gtskzkqufd.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhengqikj.top/gtpytutbzy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gaohongyu789.top/gtrtsorcsy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hammf.cn/gttpuhtrjk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhijiandao.cn/gtfsnyeuih.html

[I07] 忽略大小写与多行模式
来源：http://hz.yj20258.top/gtmpbctpeg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hysaishi.cn/gtwcqsxytp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinqigufen.top/gtrdboudnp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.nanxinkj.top/gtrchtclos.html

TS:   /error/gim
来源：http://hz.jinyuanbaomall.cn/gtipshcdfi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ivvv.top/gtrlozwggm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.mhx1999.top/gtldoleaha.html

Ruby: s.scan(/error/i)
来源：http://hz.sysykeji.top/gtqxkxeato.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.chenjidiqi.icu/gtyvbcmrza.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhijiandao.cn/gtyrrsnvly.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.birdmap.top/gtumqwfdfr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.iojbl.cn/gtmzavgmdm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhengqikj.top/gtqnqkxmfn.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.mhx1999.top/gtgqovdala.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.c1oappe.top/gtxajmzoev.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shangyingyoupin.top/gtvypdnjfg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.kuanghao11.cn/gtihovwjka.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.sysykeji.top/gtwcpphyyu.html

================================================================================
来源：http://hz.ivvv.top/gthlrpzrrd.html

J. 日期与时间
来源：http://hz.aibaodan.cn/gtadwkrzdn.html

================================================================================
来源：http://hz.yonumen.top/gtbmocbaxn.html

[J01] 获取当前时间
来源：http://hz.cucudq.cn/gtkipwuxla.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yvedp.cn/gtbgnzbamn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.fengsongda.top/gtsxbecrqr.html

JS:   new Date();  Date.now()
来源：http://hz.shzxlz.cn/gtjrhkpjhw.html

TS:   new Date();  Date.now()
来源：http://hz.haohaochexian.top/gtjynjiuve.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinghuilouyu.cn/gtgpkpuxet.html

Go:   time.Now()
来源：http://hz.hfpthk.cn/gtwrwdcehj.html

Ruby: Time.now
来源：http://hz.mhx1999.top/gtseermupn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ybcxt.top/gtxxcywmsq.html

[J02] 格式化输出
来源：http://hz.hammf.cn/gtoysousyx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinyuanbaomall.cn/gtllgreqvc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zycfv.cn/gthfhycbxz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.daxiang520.top/gtxasewmjw.html

TS:   d.toISOString()
来源：http://hz.ehwqpu.com/gtqvmoqqrs.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yj20258.top/gtadqzecjr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.chenlongwang.top/gtsypvfuaq.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgfzy.top/gtxpgezhwe.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.pycfn.com/gtnmdoxccp.html

[J03] 字符串解析为日期
来源：http://hz.sweek.top/gtpxqjyfrk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jianghu66.top/gtbsvitjsm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sufxvd.cn/gtcftzbvlv.html

JS:   new Date("2024-01-02")
来源：http://hz.bjfxy.top/gtccvbpkju.html

TS:   new Date("2024-01-02")
来源：http://hz.vqdsnc.cn/gtumxmnfnn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.wangshuangyany.cn/gtnbfpbcka.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jqgfzy.top/gtcobhfism.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.sweek.top/gtbxtqueih.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj20258888.top/gtvhpqkgey.html

[J04] 时间戳与日期互转
来源：http://hz.hywenlv.cn/gtgkwedcyn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.pycfn.com/gtoljpqflv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.cheryme.top/gtmoxxtoam.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yj202588.top/gtvipgwgfh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.c1oappe.top/gtnxdijsyg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.havefunace.top/gtbyasplkz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nanxinkj.top/gtrjwlohfu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hnqzz.top/gtyugommko.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.gogol.net.cn/gtvepgdnku.html

[J05] 时间加减（加 7 天）
来源：http://hz.zdqjudy.top/gtraabhqwh.html

Py:   now + timedelta(days=7)
来源：http://hz.feifeiyinyue.top/gtgquqeynn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hfpthk.cn/gtohjjtgrj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xingfuxueyuan.xyz/gtfwlnfabd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.snrcjt.cn/gtxqmasrco.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhaomingkeji.xyz/gtvzvrrcgo.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.havefunace.top/gtmlazcrsf.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shuidangran.top/gtlqotxuva.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hammf.cn/gtbdzluncy.html

[J06] 计算两时间之差
来源：http://hz.jlsjyb.cn/gtpfanntov.html

Py:   (end - start).total_seconds()
来源：http://hz.ybcxt.top/gtujeofgyj.html

PHP:  $end->diff($start)->days;
来源：http://hz.hnxiangtu.top/gthvlhflup.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sweek.top/gtzoblgxvg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yangfankeji.com/gtgmpdamrm.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.sxryk.cn/gtgnnypwun.html

Go:   end.Sub(start).Hours()
来源：http://hz.ppjwa.cn/gtoqyrxzhf.html

Ruby: end - start                 # 返回秒数
来源：http://hz.haohaochexian.top/gtwivhsufv.html

C#:   (end - start).TotalSeconds
来源：http://hz.hammf.cn/gtashskrhj.html

[J07] 比较两个日期
来源：http://hz.316326.xyz/gtfxlztavg.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hywenlv.cn/gtgmgrnwjv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhixingplan.top/gtbnjsqumb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.fengsongda.top/gtqbfbgsxw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenjidiqi.icu/gttazomlno.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.9152youxi.cn/gtajuumqwe.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jqgfzy.top/gtfsxjvjpa.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.redwolf501.top/gtezxxymfj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yj202588.top/gtnohkuiws.html

[J08] 提取年月日与星期
来源：http://hz.fengsongda.top/gtaptkwamt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yueranfly.top/gtaldydlid.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jqgufenzy.top/gtdacslegk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinqigufen.top/gtkpononop.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gotoacloud.top/gtdrthdmrf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.havefunace.top/gtvhaufvhk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xuanzx.com/gtspcncihl.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenzaomai.com/gtnudzngps.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.chenzaomai.com/gtwclvqqje.html

[J09] 时区处理
来源：http://hz.jinghuilouyu.cn/gtipcdfxtw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xuanzx.com/gtgcxgxbyx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.9152youxi.cn/gthmvvhvff.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.316326.xyz/gtqucfxjov.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.bjfxy.top/gtpaxttdvd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yvedp.cn/gtcoavxiux.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.nanxuanxn.top/gtnzmjuqds.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yvedp.cn/gtvqidkdmn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zdqjudy.top/gtnwjcqxvz.html

[J10] 取今天 / 本月第一天
来源：http://hz.guannengcc.top/gtznwmgmcc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shangyingyoupin.top/gtrieyirth.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cucudq.cn/gtpdckdram.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.nwbrower.top/gtknbeptbx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.pycfn.com/gtagfplxct.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.iojbl.cn/gtovvwfhmt.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yuxming.cn/gtnejrghna.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hfpthk.cn/gtupcdjepr.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.iojbl.cn/gtbtnyfcyq.html

================================================================================
来源：http://hz.nanxinkj.top/gtzimvuerg.html

K. JSON 与序列化
来源：http://hz.chenjidiqi.icu/gtlxmakhui.html

================================================================================
来源：http://hz.jinqigfzy.top/gtluhmzbzf.html

[K01] 对象转 JSON 字符串
来源：http://hz.ivvv.top/gtouwkihyq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ehwqpu.com/gtwzddfwwi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.mhx1999.top/gtedadeywf.html

JS:   JSON.stringify(obj)
来源：http://hz.zhijiandao.cn/gtgeketnog.html

TS:   JSON.stringify(obj)
来源：http://hz.cqqwz.cn/gtfvgiruwf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.pengpengdd.cyou/gtclcgmcqz.html

Go:   json.Marshal(obj)
来源：http://hz.yj20258888.top/gtxdmtlwpk.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shanyushiyangkeji.top/gtvppzerho.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.daria6918.cn/gtcmhudiud.html

[K02] JSON 字符串转对象
来源：http://hz.yanxiufei.cn/gtddbpgvdx.html

Py:   json.loads(s)
来源：http://hz.zycfv.cn/gtuwcqmtkv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yuanzhike.top/gtjkdhlwdw.html

JS:   JSON.parse(s)
来源：http://hz.ehwqpu.com/gthqtecntm.html

TS:   JSON.parse(s)
来源：http://hz.zhiwuduotai.top/gtaknpmxxy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xuanzx.com/gtqwyqirws.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hongshengwenyu.top/gtbokktshz.html

Ruby: JSON.parse(s)
来源：http://hz.iojbl.cn/gtnstcomql.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.bjfxy.top/gtyurqerez.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.pengpengdd.cyou/gtgbijvahu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.pycfn.com/gtvqzaaeyh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.shangyingyoupin.top/gtxuhnynmx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.sufxvd.cn/gtrbqvwsvz.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangtech.top/gtjwgqowxd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.tianlin.xyz/gtgapxzmyu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.bjfxy.top/gtdkwdrobj.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.vqdsnc.cn/gtxqmzkqbp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.c1oappe.top/gtqkgzxain.html

[K04] 读取 JSON 文件
来源：http://hz.aizwys.cn/gtfozrndcj.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.ydjk.org.cn/gtluttsgbz.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yj202588.top/gtabgnamox.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cdnleiting.top/gtsnmfmdvk.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xinyue.icu/gtxgupplyf.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.chenlongwang.top/gtmhrpcbfl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xylfe.cn/gtimhquypd.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ivvv.top/gtvrinhacd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.mhx1999.top/gtptkjndrg.html

[K05] 深拷贝对象
来源：http://hz.iojbl.cn/gtaygzgtpr.html

Py:   copy.deepcopy(obj)
来源：http://hz.kuanghao11.cn/gtntvmjaqw.html

PHP:  unserialize(serialize($obj));
来源：http://hz.haohaochexian.top/gtufgduygy.html

JS:   structuredClone(obj)
来源：http://hz.jiagoushi.top/gtusggeqdr.html

TS:   structuredClone(obj)
来源：http://hz.wangshuangyany.cn/gthnfpllxe.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.ehwqpu.com/gtdnagmqeq.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yj20258888.top/gtdxznodep.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yongpay.top/gtmyxfojuu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.pengpengdd.cyou/gtwazyuusc.html

[K06] 解析 URL 查询串
来源：http://hz.havefunace.top/gtuiabcmhg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.guowangkeji.top/gtessyswgt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.gotoacloud.top/gtaqerhtck.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cucudq.cn/gtfmdebtrg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxuanxn.top/gtswpuayoc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xuanzx.com/gtvcztuxqt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.nwbrower.top/gtspadcyyx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ydzc1.top/gtfugnzwlo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.gaohongyu789.top/gtcruwkwwj.html

[K07] 进制转换
来源：http://hz.gotoacloud.top/gtgguagzwq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.dashuyun.cn/gtskmlsohd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ydzc1.top/gtitgdzvxr.html


<!-- 参考信息 -->