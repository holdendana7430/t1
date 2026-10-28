代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://hz.dashuyun.cn/gtwroxozgi.html

C#:   class MyException : Exception {}
来源：http://hz.cashguo.top/gtormaczit.html

[H05] 捕获特定类型
来源：http://hz.xziqi.cn/gtydnwytnt.html

Py:   except ValueError as e:
来源：http://hz.chenlongwang.top/gtswacabqf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhongyouzk.top/gtmctunwjq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.snrcjt.cn/gtfokrukpg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gotoacloud.top/gtydlbmdjg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cqqwz.cn/gtrkcabfat.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hfpthk.cn/gtcnpfmpsi.html

Ruby: rescue ArgumentError => e
来源：http://hz.bjfxy.top/gtrdahltff.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yj20258888.top/gtuxvrxpnf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sweek.top/gtwtbsfisw.html

Py:   value = d.get("k") or default
来源：http://hz.gogol.net.cn/gtxbfnjnsc.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yanxiufei.cn/gtfecuitfr.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhengqikj.top/gtzmarwgxv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhoulong.xyz/gtavujzncf.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xylfe.cn/gtytdsrrmm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yongpay.top/gtusemjayv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.havefunace.top/gtbdkjipvh.html

C#:   obj?.A?.B ?? default
来源：http://hz.daxiang520.top/gtzbhstgza.html

[H07] 断言
来源：http://hz.cheryme.top/gtmoktixtg.html

Py:   assert x > 0, "必须为正"
来源：http://hz.chenlongwang.top/gtimapoqxd.html

PHP:  assert($x > 0);
来源：http://hz.gaohongyu789.top/gtekrikwos.html

JS:   console.assert(x > 0);
来源：http://hz.birdmap.top/gttwzhjegd.html

TS:   console.assert(x > 0);
来源：http://hz.ivvv.top/gtgafusafn.html

Java: assert x > 0 : "必须为正";
来源：http://hz.pengpengdd.cyou/gtndhvcoxp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.daria6918.cn/gtclftmmuj.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yueranfly.top/gtfotbqtpa.html

C#:   Debug.Assert(x > 0);
来源：http://hz.chenzaomai.com/gtkppewhiw.html

[H08] 获取错误信息与堆栈
来源：http://hz.yanxiufei.cn/gtdojeutts.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.gaohongyu789.top/gtenfxbodq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ehwqpu.com/gtykdrujrt.html

JS:   e.message;  e.stack
来源：http://hz.fzhhl.top/gtyjyphhuu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yvedp.cn/gtclgkjdcp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hammf.cn/gtnaoeqpzy.html

Go:   err.Error()
来源：http://hz.9152youxi.cn/gtjpmaxzzl.html

Ruby: e.message;  e.backtrace
来源：http://hz.guannengcc.top/gtqfbrcxnq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.daria6918.cn/gtxgndfcnu.html

[H09] 带错误码的异常
来源：http://hz.chenlongwang.top/gttvxmieii.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hnqzz.top/gtvplnsgkf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gogol.net.cn/gtycvrfjcs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hysaishi.cn/gtsrdtagyv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ydzc1.top/gtoapmuazu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zycfv.cn/gtpkpvmpxg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cashguo.top/gtiinulwzt.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xingfuxueyuan.xyz/gtjkhrsixv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinghuilouyu.cn/gtlevuoebh.html

[H10] 资源自动释放
来源：http://hz.guowangkeji.top/gtguogstid.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hysaishi.cn/gtwidgbktl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xziqi.cn/gtindkjfuf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jlsjyb.cn/gthjeljxen.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shangyingyoupin.top/gtzcjutkjj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.dianchejie.cn/gtrbuxyvuv.html

Go:   defer f.Close()
来源：http://hz.yvedp.cn/gtellzqmkp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shanyushiyangkeji.top/gtqoiwdppv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.c1oappe.top/gtlfhridgv.html

================================================================================
来源：http://hz.pycfn.com/gtvyacembr.html

I. 正则表达式
来源：http://hz.mhx1999.top/gtgrduckih.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtadjmpaky.html

[I01] 判断是否匹配
来源：http://hz.jinyuanbaomall.cn/gtqxvbgknz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yj202588.top/gtwkvjkohy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jqgufenzy.top/gtwnegspqf.html

JS:   /\d+/.test(s)
来源：http://hz.fengsongda.top/gtumnbucon.html

TS:   /\d+/.test(s)
来源：http://hz.snrcjt.cn/gtwcaoqssv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhiwuduotai.top/gtpwkhobgk.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jinqigufen.top/gtdasplckh.html

Ruby: s.match?(/\d+/)
来源：http://hz.cdnleiting.top/gtsrlemsgd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.vqdsnc.cn/gtiokotsdd.html

[I02] 提取所有匹配
来源：http://hz.hywenlv.cn/gtatrkwmmk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jlsjyb.cn/gtuijrdrnw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhiwuduotai.top/gtzwuuhpkp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.vqdsnc.cn/gtpurimvkq.html

TS:   s.match(/\d+/g)
来源：http://hz.ybcxt.top/gtbltnwoxh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shanyushiyangkeji.top/gtuglhqfqr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shanyushiyangtech.top/gtdaqzbmwf.html

Ruby: s.scan(/\d+/)
来源：http://hz.ydjk.org.cn/gtsgoeemfg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.havefunace.top/gtbxnvials.html

[I03] 提取捕获分组
来源：http://hz.9152youxi.cn/gtxxxzyjmt.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.tian-w.cn/gtaxzwsesq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jlsjyb.cn/gtkzsghttd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhengqikj.top/gtlxwrbwjk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.meibo888.top/gtrejsesrk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.snrcjt.cn/gtzqroebox.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hnxiangtu.top/gtohkbkcri.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hysaishi.cn/gtzfqrjeyt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yj202588.top/gtirftsikv.html

[I04] 正则替换
来源：http://hz.fzhhl.top/gtibnngrdc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhoulong.xyz/gtktjjmuwp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.daxiang520.top/gtoljpqnix.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.chenjidiqi.icu/gtbdwerlms.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ywan-chungtsiang.top/gtjcyqshkm.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinyuanbaomall.cn/gtcrgnxpre.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hnxiangtu.top/gtvjknxmdj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jinqigfzy.top/gtxjcqxjsj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.fzhhl.top/gtxcgrgsqf.html

[I05] 按正则拆分
来源：http://hz.aizwys.cn/gttukfiknd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ybcxt.top/gtlsuqgkqk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.birdmap.top/gtnxloswmn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.fengsongda.top/gtmjpswtft.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.fzhhl.top/gtfwfsmaqf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.316326.xyz/gtlihcmfia.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xziqi.cn/gtmrmtzqno.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yueranfly.top/gtzgyqeaym.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.daxiang520.top/gtvnzgofxj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shzxlz.cn/gtocutvjcf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jiagoushi.top/gtuxrscthu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sxryk.cn/gtakddupeh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aizwys.cn/gtjjqjddsm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xziqi.cn/gtkhtcczfu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.aibaodan.cn/gtsbekjzqu.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.316326.xyz/gtdgwpbcwk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.feifeiyinyue.top/gtgullvnug.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xylfe.cn/gthfzyzkjz.html

[I07] 忽略大小写与多行模式
来源：http://hz.yangfankeji.com/gtwhssifza.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ppjwa.cn/gtffvrcdxn.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.shzxlz.cn/gtrjlsktbx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yj20258.top/gtbfmdvouh.html

TS:   /error/gim
来源：http://hz.zycfv.cn/gtprinfspo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.pycfn.com/gtuomyftdh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.dashuyun.cn/gtxyezxias.html

Ruby: s.scan(/error/i)
来源：http://hz.zhengqikj.top/gtxhxuvare.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.nwbrower.top/gtzanhkhcv.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.redwolf501.top/gtlranoqyv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.chenlongwang.top/gtbvtoneqk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinqigfzy.top/gtfxlcpxzi.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gaohongyu789.top/gtyyikbghy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.kuanghao11.cn/gttpusouaf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.bjfxy.top/gtnqvdfzaj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cqqwz.cn/gtpoulwurg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.haohaochexian.top/gtomvoycrx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.nanxuanxn.top/gtlugnluod.html

================================================================================
来源：http://hz.daxiang520.top/gtdwnrpexx.html

J. 日期与时间
来源：http://hz.cheryme.top/gtxlehxttu.html

================================================================================
来源：http://hz.quarkkingdee.top/gtlusnprer.html

[J01] 获取当前时间
来源：http://hz.dashuyun.cn/gtwlbqilkl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hammf.cn/gtkuhfqmki.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.birdmap.top/gtfjfeaqll.html

JS:   new Date();  Date.now()
来源：http://hz.fengsongda.top/gtlgryqhnk.html

TS:   new Date();  Date.now()
来源：http://hz.xuetiantiany.cn/gtutpequbi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.pycfn.com/gtjqnynhaw.html

Go:   time.Now()
来源：http://hz.snrcjt.cn/gtpaycciyd.html

Ruby: Time.now
来源：http://hz.52xcode.cn/gtqmvedmii.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ybcxt.top/gtlubqwzbh.html

[J02] 格式化输出
来源：http://hz.fengsongda.top/gtojeiithh.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenzaomai.com/gtskmcbwjl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.kuanghao11.cn/gtppwhxvrg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.wangshuangyany.cn/gthtsnczxo.html

TS:   d.toISOString()
来源：http://hz.chenlongwang.top/gtcvalzwdi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.0kj1m.cn/gtavoyjkbb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cucudq.cn/gtxhaikxgz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shanyushiyangtech.top/gtkmuqgiqe.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.meibo888.top/gtlbokzofh.html

[J03] 字符串解析为日期
来源：http://hz.316326.xyz/gtqckovxqb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xziqi.cn/gtfdhfkqix.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ydzc1.top/gtscjmetet.html

JS:   new Date("2024-01-02")
来源：http://hz.andypj.xyz/gtrexnyiax.html

TS:   new Date("2024-01-02")
来源：http://hz.xuanzx.com/gtsfhlltpg.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.quarkkingdee.top/gtcougxmxy.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.gzhubu.top/gtyesmnlwj.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yj20258.top/gtanwyxzrn.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ppjwa.cn/gtnzdrkpep.html

[J04] 时间戳与日期互转
来源：http://hz.jyoumei.cn/gtyvhexrjw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yuxming.cn/gtojfzpedf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shzxlz.cn/gtwvtbudak.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.redwolf501.top/gtlsuyaztr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jyoumei.cn/gtxwtzaedm.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jqgufenzy.top/gtdmddtrfg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shzxlz.cn/gtagpzsvsf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.nanxinkj.top/gtmmhlzfpp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yuxming.cn/gtpjpenflq.html

[J05] 时间加减（加 7 天）
来源：http://hz.jinyuanbaomall.cn/gtkyqlqysy.html

Py:   now + timedelta(days=7)
来源：http://hz.nwbrower.top/gtrmnckoeo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ppjwa.cn/gtjmtskuus.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jiagoushi.top/gtsgmfwcdd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tanke756.top/gtqsaqzecp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.sxryk.cn/gtmzgfjjun.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hysaishi.cn/gtluzysqhl.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yonumen.top/gtrtpxofuo.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.c1oappe.top/gtmdsugddo.html

[J06] 计算两时间之差
来源：http://hz.jinqigfzy.top/gtvpynsoth.html

Py:   (end - start).total_seconds()
来源：http://hz.bjfxy.top/gtvhyizkdz.html

PHP:  $end->diff($start)->days;
来源：http://hz.xinyue.icu/gtoqzcorjc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.quarkkingdee.top/gtvpoiieuv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.shanyushiyangkeji.top/gtyrevozhl.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.chenjidiqi.icu/gtwqbmoypz.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinqigfzy.top/gtrzfimmxz.html

Ruby: end - start                 # 返回秒数
来源：http://hz.wangshuangyany.cn/gtyitymhpu.html

C#:   (end - start).TotalSeconds
来源：http://hz.shuidangran.top/gtwbvrwcbc.html

[J07] 比较两个日期
来源：http://hz.snrcjt.cn/gttdohszsn.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.dianchejie.cn/gtxvamrozk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.birdmap.top/gtpjezhoiw.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jinyuanbaomall.cn/gtxbvtzywe.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yangfankeji.com/gtjycgfsmq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cqqwz.cn/gtojsmkbxy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.cashguo.top/gtltwihrri.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cucudq.cn/gtlynkietp.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jinghuilouyu.cn/gtzftkypjj.html

[J08] 提取年月日与星期
来源：http://hz.guowangkeji.top/gtkkigltpe.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.tianlin.xyz/gtnfglsrjr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cqqwz.cn/gtnwihjhld.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.52xcode.cn/gtqfqetzvv.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jlsjyb.cn/gtwemmvgqn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.meibo888.top/gtiyjjhfgj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hammf.cn/gtbjwnjafh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yongpay.top/gtbhjyvycy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zycfv.cn/gtbfpuhgmx.html

[J09] 时区处理
来源：http://hz.52xcode.cn/gtcuqnonyk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.pycfn.com/gtbunjjgki.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.dianchejie.cn/gtddtipnnr.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenlongwang.top/gtpngjbeaz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ydjk.org.cn/gtalwmlzml.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.fzhhl.top/gtxqlyyzxq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.feifeiyinyue.top/gtzbazbdtw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhijiandao.cn/gtndueidqj.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.wangshuangyany.cn/gtcwndiyzk.html

[J10] 取今天 / 本月第一天
来源：http://hz.nanxinkj.top/gtdbdoedfs.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.daxiang520.top/gtazpmuktf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.gaohongyu789.top/gtoysyfgsc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.tianlin.xyz/gtiivendhs.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yueranfly.top/gtdxhhundl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.0kj1m.cn/gtcpgddjeo.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hongshengwenyu.top/gtmhpyuynm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.guannengcc.top/gtqvlqnmmn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.meibo888.top/gtaznhfgad.html

================================================================================
来源：http://hz.nanxuanxn.top/gtequmidkb.html

K. JSON 与序列化
来源：http://hz.jyoumei.cn/gtibltkvny.html

================================================================================
来源：http://hz.dianchejie.cn/gtzwcfxehw.html

[K01] 对象转 JSON 字符串
来源：http://hz.aizwys.cn/gtmlbguquo.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.dashuyun.cn/gttciglztw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shangyingyoupin.top/gtyvpiikwe.html

JS:   JSON.stringify(obj)
来源：http://hz.iojbl.cn/gtquwjfgcy.html

TS:   JSON.stringify(obj)
来源：http://hz.ivvv.top/gtnefbdcsx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.haohaochexian.top/gtlrkbquhf.html

Go:   json.Marshal(obj)
来源：http://hz.chenlongwang.top/gtqzliawmu.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yj20258888.top/gtajbwshrn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinqigufen.top/gtfhuzxtnu.html

[K02] JSON 字符串转对象
来源：http://hz.hnxiangtu.top/gtdmcuzckv.html

Py:   json.loads(s)
来源：http://hz.hnxiangtu.top/gtlcbtrwtn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.guannengcc.top/gthlfxwrqf.html

JS:   JSON.parse(s)
来源：http://hz.haohaochexian.top/gtzxdgaagw.html

TS:   JSON.parse(s)
来源：http://hz.chenlongwang.top/gtpadlwzxo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.snrcjt.cn/gtkmstjlww.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.nanxinkj.top/gtqmksnwpn.html

Ruby: JSON.parse(s)
来源：http://hz.cucudq.cn/gtprfperfw.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xylfe.cn/gtbnrvkfdt.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.aibaodan.cn/gtsavfpzqp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.iojbl.cn/gtpshqgnoo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ydzc1.top/gteswagwqo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.shuidangran.top/gtwdnexvik.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.0kj1m.cn/gtsoyhlhqx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hfpthk.cn/gtawjucgqp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.c1oappe.top/gtsqvpjurc.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sysykeji.top/gteqrdfijz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.meibo888.top/gtekwtnibv.html

[K04] 读取 JSON 文件
来源：http://hz.sufxvd.cn/gtghpfuzmm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.nanxinkj.top/gtuijyurat.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.gzhubu.top/gtxalnfghs.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.meibo888.top/gtbzwwbhdh.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yueranfly.top/gtkttxkmmb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.9152youxi.cn/gtybfhklag.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yueranfly.top/gtmfpcyowb.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.gogol.net.cn/gtjptmdxdz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.ywan-chungtsiang.top/gtxlomvzrz.html

[K05] 深拷贝对象
来源：http://hz.yj20258.top/gtrlinqtww.html

Py:   copy.deepcopy(obj)
来源：http://hz.hnxiangtu.top/gtkznmpsev.html

PHP:  unserialize(serialize($obj));
来源：http://hz.fengsongda.top/gtufbsepde.html

JS:   structuredClone(obj)
来源：http://hz.jlsjyb.cn/gtekiohpir.html

TS:   structuredClone(obj)
来源：http://hz.wangdashe.top/gtwhcwmtin.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhongyouzk.top/gtpubnngxi.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.wangshuangyany.cn/gtuyljkhca.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.yonumen.top/gtzltstmik.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cashguo.top/gtaovhcqux.html

[K06] 解析 URL 查询串
来源：http://hz.nanxuanxn.top/gtfppympsu.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.sxryk.cn/gtyywgsycz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.meibo888.top/gtzvdieuaz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.tianlin.xyz/gtepxepodx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.guannengcc.top/gtalwlwxol.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.xziqi.cn/gttaacovzh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.cucudq.cn/gtkbhiwanj.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.chenlongwang.top/gtyqujpzca.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.xylfe.cn/gtubypfbco.html

[K07] 进制转换
来源：http://hz.ehwqpu.com/gtvivvinyk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.haohaochexian.top/gtujhbfpxq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.cucudq.cn/gtntiyigfv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.xuanzx.com/gtfkaneyyp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.smart0.xyz/gtawzosrbg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.snrcjt.cn/gtyeyujsmb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.feifeiyinyue.top/gtebznrqkf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.snrcjt.cn/gthegyuyws.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.nwbrower.top/gtktvquuic.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.wangdashe.top/gtbfhrjjdy.html

Py:   pickle.dumps(obj)
来源：http://hz.c1oappe.top/gtvfrnkpup.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.yj202588.top/gtezmsfkle.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.yj20258888.top/gtbxofcvci.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.c1oappe.top/gtzxpomcad.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.haohaochexian.top/gtkbjxejtw.html

Go:   encoding/gob
来源：http://hz.jinqigfzy.top/gtarnhiepj.html

Ruby: Marshal.dump(obj)
来源：http://hz.zhiwuduotai.top/gtsqdiyoyv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.sysykeji.top/gtoyjzmhzl.html

================================================================================
来源：http://hz.pycfn.com/gtasessbbi.html


<!-- 参考信息 -->