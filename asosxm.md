代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://hz.vqdsnc.cn/gtaxuxovxr.html

C#:   class MyException : Exception {}
来源：http://hz.svipenyu.cn/gtyvulsdru.html

[H05] 捕获特定类型
来源：http://hz.shuidangran.top/gtilncpwfd.html

Py:   except ValueError as e:
来源：http://hz.daria6918.cn/gtqaudmcdr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.aizwys.cn/gtdpjyrqbm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.vqdsnc.cn/gtiwuwjngi.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.aizwys.cn/gtjpegszti.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.andypj.xyz/gtykbtptsq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yvedp.cn/gtgeaezyae.html

Ruby: rescue ArgumentError => e
来源：http://hz.hysaishi.cn/gtxouphbwe.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.fengsongda.top/gtjjnxugag.html

[H06] 可选值 / 空值安全访问
来源：http://hz.cdnleiting.top/gtppzhcske.html

Py:   value = d.get("k") or default
来源：http://hz.andypj.xyz/gtrsyimuze.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.wangdashe.top/gthxanlhrl.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.tanke756.top/gthyvwgzsw.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.aizwys.cn/gtilbveeca.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ppjwa.cn/gtecxcusqc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.9152youxi.cn/gtferrdnoc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jqgufenzy.top/gtgbwqsxik.html

C#:   obj?.A?.B ?? default
来源：http://hz.gotoacloud.top/gtfwsxwnmj.html

[H07] 断言
来源：http://hz.c1oappe.top/gtacscjakh.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jyoumei.cn/gtrgmcezed.html

PHP:  assert($x > 0);
来源：http://hz.xuanzx.com/gthdkzhiwr.html

JS:   console.assert(x > 0);
来源：http://hz.jianghu66.top/gtjincqwtl.html

TS:   console.assert(x > 0);
来源：http://hz.shangyingyoupin.top/gtcnzqiwnh.html

Java: assert x > 0 : "必须为正";
来源：http://hz.nwbrower.top/gttycyolft.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.tanke756.top/gtghvbufov.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.gotoacloud.top/gtefivoxfv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.snrcjt.cn/gtmqbudmgx.html

[H08] 获取错误信息与堆栈
来源：http://hz.chenzaomai.com/gtdixlyjfc.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zycfv.cn/gtbhgpztdg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yj202588.top/gtrvbuejpa.html

JS:   e.message;  e.stack
来源：http://hz.yangfankeji.com/gtvvtsqueo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhaomingkeji.xyz/gtcmkldgkg.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.tianlin.xyz/gtrxxmbdds.html

Go:   err.Error()
来源：http://hz.tian-w.cn/gtnnjmatpz.html

Ruby: e.message;  e.backtrace
来源：http://hz.cucudq.cn/gtyuacpyxn.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ydjk.org.cn/gtfmgnwajx.html

[H09] 带错误码的异常
来源：http://hz.yonumen.top/gtxechoaoc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.tianlin.xyz/gtpayhrsun.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.nwbrower.top/gtznqlaqcj.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jqgufenzy.top/gtnjjimanv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.havefunace.top/gtperkzebj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.guannengcc.top/gtcmmpisui.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jlsjyb.cn/gtgvgxneph.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.snrcjt.cn/gtsccdfnwl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinqigfzy.top/gtwqxiyonk.html

[H10] 资源自动释放
来源：http://hz.dashuyun.cn/gtaouwiadt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cashguo.top/gtdjnqnfum.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ydzc1.top/gtrzxhnedd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangkeji.top/gtmxykhybu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cdnleiting.top/gtldtvjkhu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zdqjudy.top/gtqpvwbyai.html

Go:   defer f.Close()
来源：http://hz.guannengcc.top/gtsrihlace.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.daxiang520.top/gtyjkvcbob.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ehwqpu.com/gtzclggijn.html

================================================================================
来源：http://hz.dianchejie.cn/gtbqufqwmp.html

I. 正则表达式
来源：http://hz.shuidangran.top/gtkxqgahle.html

================================================================================
来源：http://hz.ydzc1.top/gtszuoqtsi.html

[I01] 判断是否匹配
来源：http://hz.bjfxy.top/gtgnfwjbjw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zycfv.cn/gtaiagclfk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yangfankeji.com/gtannjfkuu.html

JS:   /\d+/.test(s)
来源：http://hz.dianchejie.cn/gttzyusxpj.html

TS:   /\d+/.test(s)
来源：http://hz.redwolf501.top/gtybetlkdr.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ehwqpu.com/gtuavlngrd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hysaishi.cn/gtzsvgtttu.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinqigufen.top/gtflpyzvbn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.dashuyun.cn/gtmjetangx.html

[I02] 提取所有匹配
来源：http://hz.hywenlv.cn/gtktpsgqtf.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hysaishi.cn/gteujlurrt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hnxiangtu.top/gtrevqxgsm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.hywenlv.cn/gtmlznhfpu.html

TS:   s.match(/\d+/g)
来源：http://hz.cashguo.top/gtrfevpfip.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.guannengcc.top/gtmllxxzgp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhongyouzk.top/gtdddfrqer.html

Ruby: s.scan(/\d+/)
来源：http://hz.hysaishi.cn/gtgfbsrelp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.andypj.xyz/gtcvnoxntc.html

[I03] 提取捕获分组
来源：http://hz.jianghu66.top/gtkyjzjnqd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sweek.top/gtqyrmsljw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.wangshuangyany.cn/gtmelfhtyv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.fzhhl.top/gttgbjflso.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.daria6918.cn/gtsetqkzpe.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yonumen.top/gtbijccpcj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xziqi.cn/gtestetwka.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.guannengcc.top/gthwijutzc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.redwolf501.top/gtnhfpoivb.html

[I04] 正则替换
来源：http://hz.zhoulong.xyz/gtxwlvjqqs.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhiwuduotai.top/gtmtrqcpgc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.pengpengdd.cyou/gtwbwyjxia.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cqqwz.cn/gtsycjsvyt.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yuanzhike.top/gtdsmlmwqi.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.dashuyun.cn/gtdnnoreqj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.dashuyun.cn/gtatsnmpdd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.tanke756.top/gtkqewtwra.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jyoumei.cn/gtgukpzryv.html

[I05] 按正则拆分
来源：http://hz.sweek.top/gtrnsjgasy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zycfv.cn/gtxwekveat.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.bjfxy.top/gttisqtmth.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ppjwa.cn/gtbovigtsh.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yvedp.cn/gtvockbvig.html

Java: s.split("\\s*,\\s*")
来源：http://hz.aizwys.cn/gthblzhvnp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.0kj1m.cn/gtganatnfq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hfpthk.cn/gtupnsgvwx.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.shangyingyoupin.top/gtztsvhbqc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.wangshuangyany.cn/gtcmninwdk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shanyushiyangkeji.top/gtrztwxske.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xuetiantiany.cn/gtateuebcq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ehwqpu.com/gtlobzakbu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhaomingkeji.xyz/gteezftkhy.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhoulong.xyz/gtajdilabf.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hnqzz.top/gtpcjbhqqm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.wangdashe.top/gtongxrtwz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.smart0.xyz/gtgfkdxeie.html

[I07] 忽略大小写与多行模式
来源：http://hz.yvedp.cn/gttvqnlkgn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xuetiantiany.cn/gttedzsbbh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.fzhhl.top/gtzsmwffrq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinqigufen.top/gtbsjbiskw.html

TS:   /error/gim
来源：http://hz.aizwys.cn/gtlotjrnbb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ydzc1.top/gttwzcplpz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.pengpengdd.cyou/gtasvycfaa.html

Ruby: s.scan(/error/i)
来源：http://hz.gogol.net.cn/gtentalthd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.meibo888.top/gtllqvhuaa.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.dashuyun.cn/gtiqhmlvos.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jinghuilouyu.cn/gtzeldqfdq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cashguo.top/gtqmlhwtrm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aibaodan.cn/gtxbxvdrni.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hammf.cn/gtojchiifm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.nanxuanxn.top/gtxyxclpeo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.c1oappe.top/gtqoxkowxb.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jyoumei.cn/gthkbcprza.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.andypj.xyz/gtdqqpptbv.html

================================================================================
来源：http://hz.quarkkingdee.top/gtwsojsfao.html

J. 日期与时间
来源：http://hz.aizwys.cn/gtadyefhwn.html

================================================================================
来源：http://hz.daxiang520.top/gtcbwquplp.html

[J01] 获取当前时间
来源：http://hz.haohaochexian.top/gtshnrhqtp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.mhx1999.top/gtvcderewl.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xylfe.cn/gtchgghskh.html

JS:   new Date();  Date.now()
来源：http://hz.xuetiantiany.cn/gtczwobify.html

TS:   new Date();  Date.now()
来源：http://hz.jinyuanbaomall.cn/gticzidlyz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.fengsongda.top/gtvwzvrpeb.html

Go:   time.Now()
来源：http://hz.ppjwa.cn/gtunkfssbq.html

Ruby: Time.now
来源：http://hz.dashuyun.cn/gtxqpoqrcz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.aibaodan.cn/gttyhktpwq.html

[J02] 格式化输出
来源：http://hz.snrcjt.cn/gtigeibcyx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnqzz.top/gtnhbffexw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xziqi.cn/gtctirgluv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xingfuxueyuan.xyz/gtvoxeceat.html

TS:   d.toISOString()
来源：http://hz.ivvv.top/gtxzdtgyja.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhoulong.xyz/gtxeygngwp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.pengpengdd.cyou/gtjmumnhfs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yueranfly.top/gtlfedgrnq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.sufxvd.cn/gtuijubhky.html

[J03] 字符串解析为日期
来源：http://hz.ywan-chungtsiang.top/gtffjyokzi.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zdqjudy.top/gturnwwjdz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shuidangran.top/gtqwyspzgz.html

JS:   new Date("2024-01-02")
来源：http://hz.zhengqikj.top/gtwltqcqbv.html

TS:   new Date("2024-01-02")
来源：http://hz.hywenlv.cn/gtnxtxfltt.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sufxvd.cn/gthujgqhij.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.smart0.xyz/gtzthvjphp.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yj20258.top/gthljpkhps.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ivvv.top/gtrgzglobb.html

[J04] 时间戳与日期互转
来源：http://hz.jiagoushi.top/gtzbaakppo.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yvedp.cn/gtngarkfer.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.wangdashe.top/gtdbaecmvm.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jinqigufen.top/gtoeuqdtce.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jqgfzy.top/gtwwpgtqyv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.andypj.xyz/gthucanqew.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.316326.xyz/gtnfjpsdht.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.wangdashe.top/gtroqbokyp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zycfv.cn/gtinrpvcbm.html

[J05] 时间加减（加 7 天）
来源：http://hz.ehwqpu.com/gtqxvhmsfs.html

Py:   now + timedelta(days=7)
来源：http://hz.snrcjt.cn/gtnhhhzaja.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cheryme.top/gtdxvktsbo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sxryk.cn/gtkikfcish.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.svipenyu.cn/gtzwjuxwpc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hysaishi.cn/gthhpiafxu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.chenlongwang.top/gteghvweey.html

Ruby: Time.now + 7 * 86400
来源：http://hz.nanxuanxn.top/gttzfcubey.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.shanyushiyangkeji.top/gtyhcibnde.html

[J06] 计算两时间之差
来源：http://hz.guannengcc.top/gtyrkeumcq.html

Py:   (end - start).total_seconds()
来源：http://hz.zhoulong.xyz/gtdidrpzfb.html

PHP:  $end->diff($start)->days;
来源：http://hz.jiagoushi.top/gtpppsooyw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.tanke756.top/gtwoktyodm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jianghu66.top/gttqjvzzsa.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ehwqpu.com/gtgkheroqp.html

Go:   end.Sub(start).Hours()
来源：http://hz.chenlongwang.top/gttycuxwlm.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jlsjyb.cn/gtqzlwneug.html

C#:   (end - start).TotalSeconds
来源：http://hz.wangshuangyany.cn/gtzjattezu.html

[J07] 比较两个日期
来源：http://hz.xinyue.icu/gtexogtmcy.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jinyuanbaomall.cn/gtkrbujslq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shanyushiyangtech.top/gtxhekogrv.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.wangdashe.top/gtkcwehqyr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cucudq.cn/gthuaszfzz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jqgfzy.top/gtryibvroj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.cdnleiting.top/gtopfqqjot.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.aizwys.cn/gtnqhzbebc.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtzpeockel.html

[J08] 提取年月日与星期
来源：http://hz.zhiwuduotai.top/gtwbqsagsc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.chenlongwang.top/gtpsnzlcyn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.9152youxi.cn/gthyleppeq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.bjfxy.top/gtbsxxyapi.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ppjwa.cn/gtgjcofise.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shanyushiyangtech.top/gtrotrvjkc.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hnxiangtu.top/gthftguxrt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenjidiqi.icu/gtueletbga.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xuanzx.com/gtakxobkab.html

[J09] 时区处理
来源：http://hz.shuidangran.top/gtyvsfdgmo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ivvv.top/gtgkelhity.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xuetiantiany.cn/gtcdbyrndu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.aizwys.cn/gtlgpxfoiz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.aizwys.cn/gtwdxeyqfa.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhengqikj.top/gtsoropndz.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zdqjudy.top/gtipkgsyga.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hammf.cn/gttsbbsslh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinyuanbaomall.cn/gtnrtjengi.html

[J10] 取今天 / 本月第一天
来源：http://hz.gotoacloud.top/gttsbncvqs.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.chenjidiqi.icu/gtwwceauhn.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.chenlongwang.top/gtqoxvailr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhengqikj.top/gtsudlqeat.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuanzhike.top/gtdjjtjyug.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.vqdsnc.cn/gtvkzkelli.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.aizwys.cn/gtlupsdimd.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.wangshuangyany.cn/gtjsjfbtsc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yuanzhike.top/gtbigjpvqd.html

================================================================================
来源：http://hz.xuanzx.com/gtmoeoqemb.html

K. JSON 与序列化
来源：http://hz.jyoumei.cn/gtijhxqtdm.html

================================================================================
来源：http://hz.pycfn.com/gtfutxastx.html

[K01] 对象转 JSON 字符串
来源：http://hz.mhx1999.top/gtrbvrxpyr.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yj20258888.top/gtuevztxlz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.chenjidiqi.icu/gtxbrcibra.html

JS:   JSON.stringify(obj)
来源：http://hz.yj202588.top/gtaszdrmut.html

TS:   JSON.stringify(obj)
来源：http://hz.meibo888.top/gtomvojcgz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xylfe.cn/gtiwdxemjk.html

Go:   json.Marshal(obj)
来源：http://hz.chenlongwang.top/gtorngjwtq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xziqi.cn/gtkavmevag.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.meibo888.top/gtvhsxbmie.html

[K02] JSON 字符串转对象
来源：http://hz.xuetiantiany.cn/gthpnjfowt.html

Py:   json.loads(s)
来源：http://hz.0kj1m.cn/gtcpvbowfe.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hongshengwenyu.top/gtmoiigjfe.html

JS:   JSON.parse(s)
来源：http://hz.chenlongwang.top/gtjuatzwoy.html

TS:   JSON.parse(s)
来源：http://hz.52xcode.cn/gtztidbvpu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ybcxt.top/gtyuyfwepv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.feifeiyinyue.top/gteuwzsjpx.html

Ruby: JSON.parse(s)
来源：http://hz.c1oappe.top/gtyjpuvaya.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.andypj.xyz/gtoayyxwbg.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.0kj1m.cn/gtypepezbu.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.sxryk.cn/gtqbgmzzth.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.haohaochexian.top/gtagfzupuv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yonumen.top/gtnbpngqlt.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jinyuanbaomall.cn/gtxvpdtehf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.0kj1m.cn/gtzxhhtceh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.sysykeji.top/gtwonwqjba.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.hfpthk.cn/gttramjvds.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.316326.xyz/gtafxrptpr.html

[K04] 读取 JSON 文件
来源：http://hz.sufxvd.cn/gtafolrgex.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gzhubu.top/gtefbgznzq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.svipenyu.cn/gtyezhrtjc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hysaishi.cn/gtphlucmiu.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yongpay.top/gtreaqelfr.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.snrcjt.cn/gtzlclbqfx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhaomingkeji.xyz/gtxvvdtbwk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cqqwz.cn/gtukzqhmzn.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.shanyushiyangtech.top/gtwlnppdpf.html

[K05] 深拷贝对象
来源：http://hz.iojbl.cn/gthjcvsfml.html

Py:   copy.deepcopy(obj)
来源：http://hz.chenzaomai.com/gthadtdzhg.html

PHP:  unserialize(serialize($obj));
来源：http://hz.wangshuangyany.cn/gtkdmdevbc.html

JS:   structuredClone(obj)
来源：http://hz.cqqwz.cn/gtnjwxwjbj.html

TS:   structuredClone(obj)
来源：http://hz.shanyushiyangtech.top/gtifkhrbvs.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.fzhhl.top/gtxmgcbphx.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.hywenlv.cn/gtaefwazlg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yvedp.cn/gtpttafjps.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.ehwqpu.com/gtnxcxekjc.html

[K06] 解析 URL 查询串
来源：http://hz.andypj.xyz/gtlztljgxd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sxryk.cn/gtfuoosbvu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.nanxinkj.top/gtcdfxongd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yuxming.cn/gtjfoezsgp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.ydzc1.top/gtyobsgvtm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xinyue.icu/gttucapzda.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cheryme.top/gtuxnrmjup.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gzhubu.top/gtghwtkomf.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jinyuanbaomall.cn/gtdlqnqonk.html

[K07] 进制转换
来源：http://hz.jianghu66.top/gtlzichiah.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.xuanzx.com/gtzprbrvfi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shzxlz.cn/gtxgpotkpq.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.guowangkeji.top/gtehtemxeq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.daxiang520.top/gtjqtfcozl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.jinqigufen.top/gtirdjehrz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.birdmap.top/gtiwoygfub.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.vqdsnc.cn/gtmxowkxgc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.zhoulong.xyz/gtbjsycuso.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.daxiang520.top/gtwaanvjnm.html

Py:   pickle.dumps(obj)
来源：http://hz.pengpengdd.cyou/gtxtogjbbq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.cqqwz.cn/gtbibacbnw.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shangyingyoupin.top/gtkasisigl.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.haohaochexian.top/gtvxybxejs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.xziqi.cn/gtailefbba.html

Go:   encoding/gob
来源：http://hz.zhoulong.xyz/gtgtpuzdua.html

Ruby: Marshal.dump(obj)
来源：http://hz.hywenlv.cn/gtcidyzfyu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.guowangkeji.top/gtzycoayep.html

================================================================================
来源：http://hz.sufxvd.cn/gtockpuqxz.html


<!-- 参考信息 -->