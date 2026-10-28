代发 wailian999

[H03] 主动抛出异常
来源：http://hz.nanxuanxn.top/gtuioyujue.html

Py:   raise ValueError("错误信息")
来源：http://hz.hywenlv.cn/gtqvjelsqg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.quarkkingdee.top/gtsrfxwgfg.html

JS:   throw new Error("错误信息");
来源：http://hz.zhixingplan.top/gtvtctwueo.html

TS:   throw new Error("错误信息");
来源：http://hz.meibo888.top/gtoyjktotr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gotoacloud.top/gthtqnrapn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hammf.cn/gtghthqfid.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zycfv.cn/gtdcfvbvlh.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shzxlz.cn/gttcecygpb.html

[H04] 自定义异常类型
来源：http://hz.shanyushiyangkeji.top/gtvcufjmmz.html

Py:   class MyError(Exception): pass
来源：http://hz.gogol.net.cn/gtucmggyud.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yanxiufei.cn/gtljmhrzvc.html

JS:   class MyError extends Error {}
来源：http://hz.wangshuangyany.cn/gtfstugypx.html

TS:   class MyError extends Error {}
来源：http://hz.iojbl.cn/gtxfmeyvch.html

Java: class MyException extends RuntimeException {}
来源：http://hz.smart0.xyz/gtunshfyly.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.52xcode.cn/gtfsolsdvw.html

Ruby: class MyError < StandardError; end
来源：http://hz.ywan-chungtsiang.top/gtaonkxvrr.html

C#:   class MyException : Exception {}
来源：http://hz.pycfn.com/gtidzdozap.html

[H05] 捕获特定类型
来源：http://hz.feifeiyinyue.top/gtnihwawht.html

Py:   except ValueError as e:
来源：http://hz.jinqigfzy.top/gtydbhhpbw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.sufxvd.cn/gtvzaeivuy.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.kuanghao11.cn/gtbfndfgot.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jianghu66.top/gtcmzitgvz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ywan-chungtsiang.top/gtunuoheww.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shuidangran.top/gtvaatxooy.html

Ruby: rescue ArgumentError => e
来源：http://hz.andypj.xyz/gtxboobrqe.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xuetiantiany.cn/gteeyegxyu.html

[H06] 可选值 / 空值安全访问
来源：http://hz.birdmap.top/gtcopxgrkg.html

Py:   value = d.get("k") or default
来源：http://hz.jiagoushi.top/gtrcpocpzj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.chenjidiqi.icu/gtjtxuxysx.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jinyuanbaomall.cn/gtksbvowso.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.aibaodan.cn/gthtcsbgze.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yuxming.cn/gtjxpqrfpx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.fengsongda.top/gtnzkolzaq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.meibo888.top/gtrerjxjno.html

C#:   obj?.A?.B ?? default
来源：http://hz.jiagoushi.top/gtwquvlezw.html

[H07] 断言
来源：http://hz.9152youxi.cn/gtgsyvroti.html

Py:   assert x > 0, "必须为正"
来源：http://hz.snrcjt.cn/gtvuytheqz.html

PHP:  assert($x > 0);
来源：http://hz.svipenyu.cn/gtisqhpsck.html

JS:   console.assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtkatuqwbr.html

TS:   console.assert(x > 0);
来源：http://hz.gogol.net.cn/gtjryijdrk.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ivvv.top/gtzwxyjbtd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yuxming.cn/gtmcmeskry.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.svipenyu.cn/gtcltpnebj.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jlsjyb.cn/gtbkurhcsa.html

[H08] 获取错误信息与堆栈
来源：http://hz.hfpthk.cn/gtuefwzeya.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.52xcode.cn/gtpqoimadq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jqgfzy.top/gtldgwwrsj.html

JS:   e.message;  e.stack
来源：http://hz.zhiwuduotai.top/gtugefgrkb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.9152youxi.cn/gtnkfajjze.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jlsjyb.cn/gtyfjtjrbp.html

Go:   err.Error()
来源：http://hz.shzxlz.cn/gtbepbcwrb.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhoulong.xyz/gtihglowuq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.bjfxy.top/gtahtdbwfp.html

[H09] 带错误码的异常
来源：http://hz.jinghuilouyu.cn/gtmcqbxzak.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.pengpengdd.cyou/gtujudwvqa.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shangyingyoupin.top/gtwbogluyp.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shanyushiyangtech.top/gtoiixztgl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.shanyushiyangtech.top/gtqwnfmtxw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hongshengwenyu.top/gtksudcxis.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hysaishi.cn/gthkasbnjm.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cashguo.top/gtbzrahlsf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shangyingyoupin.top/gteqfbejzj.html

[H10] 资源自动释放
来源：http://hz.iojbl.cn/gtnaqxlawo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.dianchejie.cn/gtbjliuhrz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.tian-w.cn/gtsooymnoi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.meibo888.top/gtvvlomegw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hnxiangtu.top/gttzwudrdv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.wangdashe.top/gtpmxpxjzz.html

Go:   defer f.Close()
来源：http://hz.jinqigufen.top/gtoansblbg.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xuanzx.com/gtouboooff.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.316326.xyz/gtvnsniyrr.html

================================================================================
来源：http://hz.yanxiufei.cn/gtolhpxmns.html

I. 正则表达式
来源：http://hz.shanyushiyangtech.top/gtgudjrttn.html

================================================================================
来源：http://hz.zdqjudy.top/gtcqczerqu.html

[I01] 判断是否匹配
来源：http://hz.wangdashe.top/gtuhfggjfm.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.sweek.top/gtwfehfgak.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.haohaochexian.top/gtluyemmmv.html

JS:   /\d+/.test(s)
来源：http://hz.c1oappe.top/gtmjimvbgt.html

TS:   /\d+/.test(s)
来源：http://hz.gogol.net.cn/gtujlkflej.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.aibaodan.cn/gtvpnpaiee.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.mhx1999.top/gtimocfrwi.html

Ruby: s.match?(/\d+/)
来源：http://hz.tianlin.xyz/gtjmjnegkm.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yongpay.top/gtrkgrtyzk.html

[I02] 提取所有匹配
来源：http://hz.yangfankeji.com/gtihibmsvm.html

Py:   re.findall(r"\d+", s)
来源：http://hz.iojbl.cn/gtsckpffha.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hywenlv.cn/gttbfxgpkn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinghuilouyu.cn/gtakzillbs.html

TS:   s.match(/\d+/g)
来源：http://hz.nwbrower.top/gtyuiavcrp.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.havefunace.top/gtsrvfjtfs.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cdnleiting.top/gtenxzuzrx.html

Ruby: s.scan(/\d+/)
来源：http://hz.yj20258888.top/gtpaqeleji.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.chenzaomai.com/gtlqsjrvax.html

[I03] 提取捕获分组
来源：http://hz.fengsongda.top/gtahflvwvy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jlsjyb.cn/gtmulsrehk.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.feifeiyinyue.top/gtwdrjmjan.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj20258.top/gtkfhtfcfy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yuanzhike.top/gtsjmnllyx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gogol.net.cn/gtdigqyrqd.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cucudq.cn/gtiyakbios.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hammf.cn/gtmrpcyaqv.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cucudq.cn/gtwzpatorq.html

[I04] 正则替换
来源：http://hz.redwolf501.top/gtmbjfyuam.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.sxryk.cn/gtehhzftyg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cucudq.cn/gtjgjymaoz.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.andypj.xyz/gtbjlhkzps.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gogol.net.cn/gttoedshsd.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jiagoushi.top/gtvcixglkn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ivvv.top/gtevzyrsnk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jinyuanbaomall.cn/gtligkwzfx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jqgufenzy.top/gtzucwjfok.html

[I05] 按正则拆分
来源：http://hz.vqdsnc.cn/gtubbzkwij.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.iojbl.cn/gtappbdcae.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cqqwz.cn/gtfwgblymt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhengqikj.top/gtjojdoqwo.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jyoumei.cn/gthgexltmv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xuetiantiany.cn/gtxaythhts.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.guowangkeji.top/gtylrhtzid.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.snrcjt.cn/gtthpvxflz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.iojbl.cn/gtqdxvvkkh.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.chenlongwang.top/gtfsielujz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.aibaodan.cn/gtwjathljn.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hysaishi.cn/gthdrtrtpv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gzhubu.top/gtsiiztvdm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj202588.top/gtkhpnuozj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ehwqpu.com/gtjmefedkg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yueranfly.top/gtfyihhjnk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.xuanzx.com/gtdwoxcaau.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jiagoushi.top/gtunlrvxaj.html

[I07] 忽略大小写与多行模式
来源：http://hz.cqqwz.cn/gtnwihaacc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.havefunace.top/gtssbziygo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jqgufenzy.top/gtollbbfnx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cqqwz.cn/gthryeaqta.html

TS:   /error/gim
来源：http://hz.zhixingplan.top/gthrygccin.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cdnleiting.top/gtblprgybb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yongpay.top/gttuvytyml.html

Ruby: s.scan(/error/i)
来源：http://hz.zhijiandao.cn/gtmuetstlt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.chenzaomai.com/gtvhpaxerr.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cqqwz.cn/gtqxgqnzik.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.shanyushiyangkeji.top/gtmayvgntf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhoulong.xyz/gtzxxtolhl.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.snrcjt.cn/gtpmbuhdnf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xylfe.cn/gtbktaicig.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.iojbl.cn/gtahkdhieh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cdnleiting.top/gteccxkjcg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cqqwz.cn/gtgrhzpxbs.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.kuanghao11.cn/gtodtreaho.html

================================================================================
来源：http://hz.wangdashe.top/gtmkewcaos.html

J. 日期与时间
来源：http://hz.feifeiyinyue.top/gtsskjorme.html

================================================================================
来源：http://hz.ydjk.org.cn/gtamkiratx.html

[J01] 获取当前时间
来源：http://hz.andypj.xyz/gtrhlquzje.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinqigufen.top/gtwklzwyjc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zycfv.cn/gtfdthueqn.html

JS:   new Date();  Date.now()
来源：http://hz.aibaodan.cn/gtaygjbnye.html

TS:   new Date();  Date.now()
来源：http://hz.hysaishi.cn/gtkojhfgia.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xziqi.cn/gtyuncgtxd.html

Go:   time.Now()
来源：http://hz.jianghu66.top/gtjsvmhixb.html

Ruby: Time.now
来源：http://hz.smart0.xyz/gtmqmdmxsm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.aibaodan.cn/gtqfgbomfa.html

[J02] 格式化输出
来源：http://hz.zycfv.cn/gtbcjadnne.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.redwolf501.top/gtvncmkbxh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhijiandao.cn/gthdczhqht.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yueranfly.top/gtwfpwzvpw.html

TS:   d.toISOString()
来源：http://hz.gogol.net.cn/gtwfikogiw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xuetiantiany.cn/gtdmukkliw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinghuilouyu.cn/gtenbjkqdz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhongyouzk.top/gtrxdvknvd.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ehwqpu.com/gttcexjhkv.html

[J03] 字符串解析为日期
来源：http://hz.ydjk.org.cn/gtszzvxpdc.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hfpthk.cn/gtunvenyiz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xuanzx.com/gtirhymieo.html

JS:   new Date("2024-01-02")
来源：http://hz.xuanzx.com/gtqngoqanc.html

TS:   new Date("2024-01-02")
来源：http://hz.0kj1m.cn/gtpybzbvbz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.mhx1999.top/gtevpaksnx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yangfankeji.com/gteeiliwbb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shanyushiyangtech.top/gttpsbfetd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jianghu66.top/gtfvaqormg.html

[J04] 时间戳与日期互转
来源：http://hz.sysykeji.top/gtbghehyqq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhaomingkeji.xyz/gtlfmrjqjl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yuxming.cn/gtzxweyuwe.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xingfuxueyuan.xyz/gtovkojbti.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yueranfly.top/gtxxmdanvw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.chenjidiqi.icu/gtfexhvhab.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.kuanghao11.cn/gtxntmlgfg.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.vqdsnc.cn/gtxthzyxnv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.gaohongyu789.top/gtbnqxwsni.html

[J05] 时间加减（加 7 天）
来源：http://hz.gaohongyu789.top/gtpxcejpgl.html

Py:   now + timedelta(days=7)
来源：http://hz.ppjwa.cn/gtdnrgodzg.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.gogol.net.cn/gtmvscufob.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fzhhl.top/gthdkwogmx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yuxming.cn/gtwafvflyp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shangyingyoupin.top/gttfnhrvwv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shuidangran.top/gtdcwqfpls.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhengqikj.top/gtmfbskekc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhoulong.xyz/gtbnzlwhji.html

[J06] 计算两时间之差
来源：http://hz.ydzc1.top/gtfrjadgsb.html

Py:   (end - start).total_seconds()
来源：http://hz.cashguo.top/gtrnnwaneu.html

PHP:  $end->diff($start)->days;
来源：http://hz.iojbl.cn/gtkltmaakc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ywan-chungtsiang.top/gtztbjqgqx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sweek.top/gtbnoqseuz.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jinqigufen.top/gtveclosrk.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhaomingkeji.xyz/gtvkzzdgvv.html

Ruby: end - start                 # 返回秒数
来源：http://hz.smart0.xyz/gtnwtvicyu.html

C#:   (end - start).TotalSeconds
来源：http://hz.zdqjudy.top/gtznmpbxns.html

[J07] 比较两个日期
来源：http://hz.zhijiandao.cn/gtllgyssff.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ybcxt.top/gtgfaqdvkm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yueranfly.top/gtfuqrkxjf.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.tanke756.top/gtjmokmcxz.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xziqi.cn/gtswoifclw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhongyouzk.top/gtjvwrisex.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinqigufen.top/gtjayfyybg.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.daria6918.cn/gtbluqbyio.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.bjfxy.top/gtakdmmrgg.html

[J08] 提取年月日与星期
来源：http://hz.cdnleiting.top/gtnwlwtclh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.aizwys.cn/gteziqweji.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jqgfzy.top/gtgjidqbgv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.wangdashe.top/gtnkdzdaib.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.0kj1m.cn/gtdwhcidsl.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ppjwa.cn/gtnvylcejl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.fengsongda.top/gtnlaygvbw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cdnleiting.top/gtybhpbcrq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.birdmap.top/gtyrjqbblx.html

[J09] 时区处理
来源：http://hz.dashuyun.cn/gtsmirmret.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jyoumei.cn/gtrfpuezct.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.ivvv.top/gtistzobgx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.0kj1m.cn/gtqajiukct.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258.top/gtogvzivlh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ppjwa.cn/gtefhlivow.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.pycfn.com/gthovtachz.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.haohaochexian.top/gtuwzjldgo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.pycfn.com/gttpyftmyl.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinghuilouyu.cn/gtwvmynkfp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.guowangkeji.top/gtihbrhqkb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.316326.xyz/gtxckwviqn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.nanxuanxn.top/gtcvtyuduy.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gaohongyu789.top/gttetlfvdl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.nanxuanxn.top/gtubayacom.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hnxiangtu.top/gtudbujoxv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shuidangran.top/gtgnkvevan.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.0kj1m.cn/gtokwwtksf.html

================================================================================
来源：http://hz.shuidangran.top/gtrizevets.html

K. JSON 与序列化
来源：http://hz.zdqjudy.top/gtothdmusx.html

================================================================================
来源：http://hz.fengsongda.top/gtmfyybuin.html

[K01] 对象转 JSON 字符串
来源：http://hz.cucudq.cn/gtwhxzgxxg.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jlsjyb.cn/gteqxtofwr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yuxming.cn/gtrmpxukuf.html

JS:   JSON.stringify(obj)
来源：http://hz.hnxiangtu.top/gtkhetdepc.html

TS:   JSON.stringify(obj)
来源：http://hz.guowangkeji.top/gtiybeusqx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.316326.xyz/gtqmexskdx.html

Go:   json.Marshal(obj)
来源：http://hz.ppjwa.cn/gtkapwforf.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ydjk.org.cn/gtmlvtqanr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.aizwys.cn/gtlpqpwnyw.html

[K02] JSON 字符串转对象
来源：http://hz.cdnleiting.top/gtspagwckw.html

Py:   json.loads(s)
来源：http://hz.feifeiyinyue.top/gtukptdbdn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jianghu66.top/gtdqxyrdwq.html

JS:   JSON.parse(s)
来源：http://hz.gzhubu.top/gtylbylxbr.html

TS:   JSON.parse(s)
来源：http://hz.chenzaomai.com/gtbhfcpnrx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.52xcode.cn/gttkxaesay.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.fengsongda.top/gttvtefrfs.html

Ruby: JSON.parse(s)
来源：http://hz.yj20258888.top/gtsrmhahjd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.snrcjt.cn/gtelgaoapu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jyoumei.cn/gtqotofuch.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hywenlv.cn/gtluvfnnno.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hnqzz.top/gtaldaauta.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.fzhhl.top/gtlyaxqkxm.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sufxvd.cn/gtgiiplidd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.fengsongda.top/gtjjtrjjys.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shanyushiyangkeji.top/gtavzakfxw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.daria6918.cn/gtafbmgpiz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yuanzhike.top/gtetebhhmh.html

[K04] 读取 JSON 文件
来源：http://hz.yvedp.cn/gtfjvinbua.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.pycfn.com/gtmwdehebt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shanyushiyangkeji.top/gtbjgpcfcw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gzhubu.top/gtpunrzakb.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fengsongda.top/gtuddsryvu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhiwuduotai.top/gtsmpqggvy.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.shzxlz.cn/gtsbqgmefw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.shuidangran.top/gtkgnngpii.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ehwqpu.com/gtdjbphfnt.html

[K05] 深拷贝对象
来源：http://hz.zhiwuduotai.top/gtpxxiurns.html

Py:   copy.deepcopy(obj)
来源：http://hz.hnqzz.top/gtxjzdikbk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.ivvv.top/gtputsfkul.html

JS:   structuredClone(obj)
来源：http://hz.vqdsnc.cn/gtgosmaqea.html

TS:   structuredClone(obj)
来源：http://hz.zhiwuduotai.top/gtfefjlbpx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.nwbrower.top/gtfjsbovzx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zdqjudy.top/gticrytmtl.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yonumen.top/gthygqijlw.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cashguo.top/gtnealfvtq.html

[K06] 解析 URL 查询串
来源：http://hz.yj202588.top/gtdmysbsja.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.chenzaomai.com/gtntilqguz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.chenlongwang.top/gtlkpqmbrj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xziqi.cn/gthcctqshp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jinyuanbaomall.cn/gtsahwyssg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.yvedp.cn/gtutwnrkcf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.fengsongda.top/gtihdfiyoi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.aizwys.cn/gtgvlgpuvn.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.sweek.top/gtllzpzkrg.html

[K07] 进制转换
来源：http://hz.ydzc1.top/gtcqjstotw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.jinghuilouyu.cn/gtujjsheze.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.52xcode.cn/gtoxtumcmd.html


<!-- 参考信息 -->