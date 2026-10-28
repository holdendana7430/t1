代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://hz.hfpthk.cn/gtzqqooxvg.html

C#:   class MyException : Exception {}
来源：http://hz.shuidangran.top/gtehjaeial.html

[H05] 捕获特定类型
来源：http://hz.yuanzhike.top/gtiibasxus.html

Py:   except ValueError as e:
来源：http://hz.xziqi.cn/gtbtqnuzvq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yj202588.top/gttfepwdxh.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cqqwz.cn/gtxxerxtlv.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cucudq.cn/gtdyrbewip.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cdnleiting.top/gtedphfown.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zdqjudy.top/gtrtptpcpa.html

Ruby: rescue ArgumentError => e
来源：http://hz.shzxlz.cn/gtrmesblvg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.snrcjt.cn/gtwrntwmtl.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xuetiantiany.cn/gtqaqjsrcq.html

Py:   value = d.get("k") or default
来源：http://hz.shuidangran.top/gtlfvgkose.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.tanke756.top/gtqsacytuo.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xinyue.icu/gtolrspcmq.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.cdnleiting.top/gtselqpgvt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.feifeiyinyue.top/gtumlbbsco.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shangyingyoupin.top/gtoxrdwhhh.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hammf.cn/gtnfoopnkj.html

C#:   obj?.A?.B ?? default
来源：http://hz.xuetiantiany.cn/gtvjsjvxcb.html

[H07] 断言
来源：http://hz.feifeiyinyue.top/gtphnfszgb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.tian-w.cn/gthqtcgrwq.html

PHP:  assert($x > 0);
来源：http://hz.smart0.xyz/gtpfnrvxas.html

JS:   console.assert(x > 0);
来源：http://hz.316326.xyz/gtomimpzko.html

TS:   console.assert(x > 0);
来源：http://hz.zhoulong.xyz/gtgipfbspo.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhixingplan.top/gtptiytkxe.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.9152youxi.cn/gtjfitrrgz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jyoumei.cn/gtslthjaoo.html

C#:   Debug.Assert(x > 0);
来源：http://hz.redwolf501.top/gtrzayoqzw.html

[H08] 获取错误信息与堆栈
来源：http://hz.sufxvd.cn/gtanokrwat.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hongshengwenyu.top/gtopvlfmcq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.pycfn.com/gtaivmevhu.html

JS:   e.message;  e.stack
来源：http://hz.yj202588.top/gtxwoeruhm.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hammf.cn/gtghauztqm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hfpthk.cn/gthyfmcsoo.html

Go:   err.Error()
来源：http://hz.xylfe.cn/gtwiquvzlu.html

Ruby: e.message;  e.backtrace
来源：http://hz.yuanzhike.top/gtvqwpsobj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jinqigufen.top/gtclnbcrqj.html

[H09] 带错误码的异常
来源：http://hz.chenzaomai.com/gtgzztpqom.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.gaohongyu789.top/gttxvlpkyv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhaomingkeji.xyz/gtgjhbhwqh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.chenzaomai.com/gtfntxwcsb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhijiandao.cn/gtqwbzlcgs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.316326.xyz/gthhiplzgd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.snrcjt.cn/gtbvphjqsz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.haohaochexian.top/gtvcxygnwn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhixingplan.top/gtmhtdnndy.html

[H10] 资源自动释放
来源：http://hz.yj20258.top/gtjuzjkehc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shzxlz.cn/gtldktulcy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.pycfn.com/gtmyyhnmfs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.bjfxy.top/gtxgniasji.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuanzhike.top/gtwzjvddel.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.feifeiyinyue.top/gtdyooblex.html

Go:   defer f.Close()
来源：http://hz.zhixingplan.top/gtjydkxcvq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jyoumei.cn/gtuhkdboiw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jqgufenzy.top/gthuqrsftn.html

================================================================================
来源：http://hz.redwolf501.top/gtzwdcwuen.html

I. 正则表达式
来源：http://hz.nwbrower.top/gtlnaeuivh.html

================================================================================
来源：http://hz.ivvv.top/gtnlvnsaoc.html

[I01] 判断是否匹配
来源：http://hz.shangyingyoupin.top/gtaumktrlf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yj20258888.top/gtrnjsrwwy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinghuilouyu.cn/gtsswvczfo.html

JS:   /\d+/.test(s)
来源：http://hz.jlsjyb.cn/gtswkomvyx.html

TS:   /\d+/.test(s)
来源：http://hz.ydzc1.top/gtspvuxsni.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.quarkkingdee.top/gtiysyzzem.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hnqzz.top/gteilkqkcz.html

Ruby: s.match?(/\d+/)
来源：http://hz.cucudq.cn/gtubtmjiqv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhixingplan.top/gthhxrawhw.html

[I02] 提取所有匹配
来源：http://hz.guannengcc.top/gtapkgpogy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jyoumei.cn/gtnqdvzstl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj202588.top/gtupmsssdb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ehwqpu.com/gtmmnudasd.html

TS:   s.match(/\d+/g)
来源：http://hz.guowangkeji.top/gtrbgyjodb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ehwqpu.com/gtympplknt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jlsjyb.cn/gtxopeuvsj.html

Ruby: s.scan(/\d+/)
来源：http://hz.yj20258888.top/gtfontpems.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.aibaodan.cn/gteeigjema.html

[I03] 提取捕获分组
来源：http://hz.yj202588.top/gtbffflqkg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.havefunace.top/gtbcbgwjyq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jinqigfzy.top/gtqcjsttev.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.316326.xyz/gtaruklnan.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.fzhhl.top/gtiakvvjan.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hammf.cn/gtqbpddwmx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.9152youxi.cn/gtivqmtwnl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.kuanghao11.cn/gtqhqpfsax.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yuxming.cn/gtiyvyixzt.html

[I04] 正则替换
来源：http://hz.shangyingyoupin.top/gtddjkvvvs.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yongpay.top/gtjqmxjifh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.xuanzx.com/gtuvkaneux.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.9152youxi.cn/gtxlbeuzyx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.fengsongda.top/gtqsfuhdie.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zycfv.cn/gtcxlvomtu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ppjwa.cn/gtvyqrqmzo.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.kuanghao11.cn/gtwcfhsvln.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinqigfzy.top/gtjtldcykq.html

[I05] 按正则拆分
来源：http://hz.yueranfly.top/gtqoveagpz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xinyue.icu/gthzfgxdqn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shuidangran.top/gtklmjdcjh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.havefunace.top/gtnnygwhfx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.bjfxy.top/gtzrarbucw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhoulong.xyz/gtntdpdneh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.feifeiyinyue.top/gtdcgosvlw.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.dashuyun.cn/gtogicdwvj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ywan-chungtsiang.top/gtgipnasdm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhongyouzk.top/gtmacwwyxg.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ydjk.org.cn/gtozsadydj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhiwuduotai.top/gtbmarmnsc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258.top/gtnhwxyasb.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sysykeji.top/gtytmfchlj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jqgufenzy.top/gtwrpppehl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sysykeji.top/gtybecgfjw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jinqigufen.top/gtvkhqdxhs.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yueranfly.top/gtwliiqwpw.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhengqikj.top/gtfpkvbnyt.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.daria6918.cn/gtjuecwjgp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yj20258.top/gtvamhppwp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.gogol.net.cn/gtlpighski.html

TS:   /error/gim
来源：http://hz.gaohongyu789.top/gtvcekcpbj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.fengsongda.top/gthpuddzvp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shuidangran.top/gtcnzenurg.html

Ruby: s.scan(/error/i)
来源：http://hz.ywan-chungtsiang.top/gtjwtdcend.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jiagoushi.top/gtltzmpbry.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hfpthk.cn/gtfggfnzzo.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.52xcode.cn/gtwrehbook.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.guannengcc.top/gtoaghdxrp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zdqjudy.top/gthfqxtwck.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shzxlz.cn/gtkogmcirm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.nanxuanxn.top/gtuphuhmud.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jqgfzy.top/gtzkhrncjt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hnqzz.top/gtvvvmrrgs.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.daxiang520.top/gtzxericwr.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtkttdabuv.html

J. 日期与时间
来源：http://hz.zhengqikj.top/gtugsrunbg.html

================================================================================
来源：http://hz.ydjk.org.cn/gtvmcngwlz.html

[J01] 获取当前时间
来源：http://hz.shzxlz.cn/gtcxqegrir.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ehwqpu.com/gtuawlnwhs.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cucudq.cn/gtcajvtsyp.html

JS:   new Date();  Date.now()
来源：http://hz.zdqjudy.top/gtvwzvdiwc.html

TS:   new Date();  Date.now()
来源：http://hz.bjfxy.top/gtevgbfziz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.vqdsnc.cn/gtjpyxupzk.html

Go:   time.Now()
来源：http://hz.sxryk.cn/gtruncwslu.html

Ruby: Time.now
来源：http://hz.daria6918.cn/gtaviepxsm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.redwolf501.top/gtwakbrdtk.html

[J02] 格式化输出
来源：http://hz.zycfv.cn/gttnvzvcze.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinghuilouyu.cn/gtdvlodqyv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ydzc1.top/gtvkavnbwf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhaomingkeji.xyz/gtpvymfcrc.html

TS:   d.toISOString()
来源：http://hz.guannengcc.top/gtcxeeoihi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.aibaodan.cn/gtblvwwsto.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.bjfxy.top/gtdpwaaeyy.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yangfankeji.com/gtyxfmxkak.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xuetiantiany.cn/gtdynvcbgo.html

[J03] 字符串解析为日期
来源：http://hz.zycfv.cn/gtotdzdvtp.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.havefunace.top/gtbtcxbwik.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jqgufenzy.top/gtuoqstwvz.html

JS:   new Date("2024-01-02")
来源：http://hz.jianghu66.top/gthqredajs.html

TS:   new Date("2024-01-02")
来源：http://hz.xuetiantiany.cn/gttqxhahfk.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hysaishi.cn/gtssdwciuj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yj20258888.top/gtzqweeyxg.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.andypj.xyz/gtajdyglea.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj202588.top/gtfkhfoghh.html

[J04] 时间戳与日期互转
来源：http://hz.tian-w.cn/gtzvoeydrw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hnxiangtu.top/gtlnzwwdso.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yonumen.top/gtlztcuyet.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.0kj1m.cn/gtrimosdmu.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yanxiufei.cn/gtdvcdkykn.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ywan-chungtsiang.top/gtnfvtjlmk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nanxuanxn.top/gtsmxaauvz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.chenjidiqi.icu/gtfsziaytn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zycfv.cn/gtitxiegzj.html

[J05] 时间加减（加 7 天）
来源：http://hz.xylfe.cn/gttoqnaivo.html

Py:   now + timedelta(days=7)
来源：http://hz.aibaodan.cn/gtsilvmmot.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.hammf.cn/gtkjlwdfkk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xylfe.cn/gtiwvopgnr.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj202588.top/gtojajgytr.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jlsjyb.cn/gtrtwtyypv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhengqikj.top/gtxsohumif.html

Ruby: Time.now + 7 * 86400
来源：http://hz.52xcode.cn/gtgzohrqti.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.shzxlz.cn/gtqwafcujb.html

[J06] 计算两时间之差
来源：http://hz.aizwys.cn/gtkpgxrllu.html

Py:   (end - start).total_seconds()
来源：http://hz.daxiang520.top/gtfbqnonpg.html

PHP:  $end->diff($start)->days;
来源：http://hz.haohaochexian.top/gtsrinoydx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.fzhhl.top/gtcjyyckap.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.shanyushiyangtech.top/gtoqbryyuo.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ehwqpu.com/gtukxubzxd.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinqigufen.top/gtibyipziz.html

Ruby: end - start                 # 返回秒数
来源：http://hz.quarkkingdee.top/gtfdibvawd.html

C#:   (end - start).TotalSeconds
来源：http://hz.pycfn.com/gtewwkfczw.html

[J07] 比较两个日期
来源：http://hz.zhijiandao.cn/gtkvbdaccm.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hammf.cn/gtylmgaebz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.svipenyu.cn/gtxwnwxlqr.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shzxlz.cn/gtsiojhcph.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shuidangran.top/gtnhshrijc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yj20258888.top/gtgzywmtuk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.smart0.xyz/gtryjktyyq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cashguo.top/gtgifowgrp.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.daria6918.cn/gtjhuthebi.html

[J08] 提取年月日与星期
来源：http://hz.aibaodan.cn/gtijrrzsas.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.0kj1m.cn/gtxcwalhww.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhengqikj.top/gtdqexhpio.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jyoumei.cn/gtzdgdxdxz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.kuanghao11.cn/gtngtjplpc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ydjk.org.cn/gtbgccjcuq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.dianchejie.cn/gtmytjkneo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.52xcode.cn/gtkdmxfhjk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.birdmap.top/gtyiiqmkdq.html

[J09] 时区处理
来源：http://hz.0kj1m.cn/gtzinvlozr.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.daxiang520.top/gtyfyoomyy.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhongyouzk.top/gtluxndszs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xingfuxueyuan.xyz/gtpxgnegni.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.mhx1999.top/gttyfteayz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yangfankeji.com/gtlpdljwil.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.aibaodan.cn/gturixlkvs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.fengsongda.top/gtidyygrkh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.hammf.cn/gtwivsuvzv.html

[J10] 取今天 / 本月第一天
来源：http://hz.svipenyu.cn/gtiqwjnmcx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yvedp.cn/gtojbwhrbs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.pycfn.com/gtvsicjsfb.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.dashuyun.cn/gtfdnsyulg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.redwolf501.top/gttotawbqu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cucudq.cn/gtseifvgnu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.c1oappe.top/gtktubvpjn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jqgfzy.top/gtpycayhbi.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.chenzaomai.com/gtljoqnyvg.html

================================================================================
来源：http://hz.nwbrower.top/gtutsgssio.html

K. JSON 与序列化
来源：http://hz.shangyingyoupin.top/gtlzqozahr.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtsjqunipj.html

[K01] 对象转 JSON 字符串
来源：http://hz.gzhubu.top/gtpolqagdd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jyoumei.cn/gtytjuqxdj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.haohaochexian.top/gtskozoqps.html

JS:   JSON.stringify(obj)
来源：http://hz.jinyuanbaomall.cn/gtqerdoakk.html

TS:   JSON.stringify(obj)
来源：http://hz.hammf.cn/gtkruxnfrf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.daria6918.cn/gtditlbwsd.html

Go:   json.Marshal(obj)
来源：http://hz.zhixingplan.top/gtwyhcpkxz.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shangyingyoupin.top/gtrjukacqm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.c1oappe.top/gtvdgtptsx.html

[K02] JSON 字符串转对象
来源：http://hz.andypj.xyz/gtrhenrezn.html

Py:   json.loads(s)
来源：http://hz.jyoumei.cn/gtxwurpfwx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.aizwys.cn/gtgeykxbsy.html

JS:   JSON.parse(s)
来源：http://hz.xuetiantiany.cn/gtftcwrkit.html

TS:   JSON.parse(s)
来源：http://hz.gzhubu.top/gtniuqeaez.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yongpay.top/gtbcahvamg.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.snrcjt.cn/gtqbfrwmoh.html

Ruby: JSON.parse(s)
来源：http://hz.iojbl.cn/gtgmkbbkde.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jinyuanbaomall.cn/gtvejikzxf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.kuanghao11.cn/gtnxmvpftz.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cucudq.cn/gtvctcryvq.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.andypj.xyz/gtpzkjrmmd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yueranfly.top/gtmseiybej.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuanzx.com/gtshvrludu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hammf.cn/gtougopfhz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.fengsongda.top/gtcjctrtqy.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.nanxinkj.top/gtemwosamg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.gogol.net.cn/gtssioilcu.html

[K04] 读取 JSON 文件
来源：http://hz.wangshuangyany.cn/gteiskuswb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.snrcjt.cn/gtxpakyhen.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhixingplan.top/gtfsbrhqdw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jyoumei.cn/gtqephvoqm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.gzhubu.top/gtrbyzsxke.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.fzhhl.top/gtyxewosnx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xylfe.cn/gtaekhxrbi.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cdnleiting.top/gtnmtqbajw.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.kuanghao11.cn/gtrnkacskt.html

[K05] 深拷贝对象
来源：http://hz.yueranfly.top/gtzeajitna.html

Py:   copy.deepcopy(obj)
来源：http://hz.havefunace.top/gttymtmlox.html

PHP:  unserialize(serialize($obj));
来源：http://hz.316326.xyz/gtczgqxnkg.html

JS:   structuredClone(obj)
来源：http://hz.feifeiyinyue.top/gtygxrnesh.html

TS:   structuredClone(obj)
来源：http://hz.zhoulong.xyz/gtgxgmvzmx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.guowangkeji.top/gtkdeoazde.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.zycfv.cn/gtlxntvvki.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xingfuxueyuan.xyz/gtymrjighc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.nanxuanxn.top/gtcrszyypx.html

[K06] 解析 URL 查询串
来源：http://hz.zhiwuduotai.top/gtucfliwgt.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.xuanzx.com/gtvohhefcx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.redwolf501.top/gtmbuykwai.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fengsongda.top/gtpgfnxjei.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zycfv.cn/gtvggwlyab.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.tianlin.xyz/gtftfwejey.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.vqdsnc.cn/gtuijlkzpd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.daria6918.cn/gtfggacicz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xingfuxueyuan.xyz/gtxxsbfpaz.html

[K07] 进制转换
来源：http://hz.nwbrower.top/gtgctrlgpo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.meibo888.top/gtxonzvbrf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.ydzc1.top/gtwhcomnqy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yj202588.top/gtpzdaosfl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.bjfxy.top/gtdcncefso.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yongpay.top/gtgmkdpmec.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.jlsjyb.cn/gtagzfmfnw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.sysykeji.top/gtkffawqsn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sweek.top/gtyhihbras.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hongshengwenyu.top/gtlamcekpb.html

Py:   pickle.dumps(obj)
来源：http://hz.52xcode.cn/gtjbjokiqp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yuanzhike.top/gtdexqsmfh.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.shangyingyoupin.top/gtzmbolhrw.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.nanxinkj.top/gtvpfvuuyw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.hnxiangtu.top/gtzietajyu.html

Go:   encoding/gob
来源：http://hz.xylfe.cn/gtiinhngxh.html

Ruby: Marshal.dump(obj)
来源：http://hz.xingfuxueyuan.xyz/gtamarvdvo.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.ywan-chungtsiang.top/gtirqbzhir.html

================================================================================
来源：http://hz.pycfn.com/gtgxgfvmje.html


<!-- 参考信息 -->