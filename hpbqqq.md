代发 wailian999

[H03] 主动抛出异常
来源：http://hz.sxryk.cn/gtrngzffxn.html

Py:   raise ValueError("错误信息")
来源：http://hz.hnxiangtu.top/gtdsghtpln.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cucudq.cn/gtdzioqwdu.html

JS:   throw new Error("错误信息");
来源：http://hz.zhoulong.xyz/gtkwarfidd.html

TS:   throw new Error("错误信息");
来源：http://hz.gaohongyu789.top/gtlcaejrxr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtqtemyosx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.feifeiyinyue.top/gtmisismrx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.birdmap.top/gtfeygccdr.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gtbagnewco.html

[H04] 自定义异常类型
来源：http://hz.hammf.cn/gtptamymhl.html

Py:   class MyError(Exception): pass
来源：http://hz.zhiwuduotai.top/gtrtbhnnao.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.0kj1m.cn/gtssbztwji.html

JS:   class MyError extends Error {}
来源：http://hz.ivvv.top/gtaqshnzdr.html

TS:   class MyError extends Error {}
来源：http://hz.smart0.xyz/gtxlmznjxm.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hfpthk.cn/gtvghkgysc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yuxming.cn/gtwspigydu.html

Ruby: class MyError < StandardError; end
来源：http://hz.0kj1m.cn/gtursmshlk.html

C#:   class MyException : Exception {}
来源：http://hz.guowangkeji.top/gtahisuoco.html

[H05] 捕获特定类型
来源：http://hz.snrcjt.cn/gtpaburspy.html

Py:   except ValueError as e:
来源：http://hz.cqqwz.cn/gtyyumhusj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ydzc1.top/gteiyzmubg.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.chenjidiqi.icu/gtihrufphf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.sweek.top/gteouraijv.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.birdmap.top/gtkaedrega.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jianghu66.top/gtislqjmtl.html

Ruby: rescue ArgumentError => e
来源：http://hz.jinqigufen.top/gtcpuwzots.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yj20258.top/gtnjllarkq.html

[H06] 可选值 / 空值安全访问
来源：http://hz.pengpengdd.cyou/gtwkqxlbxv.html

Py:   value = d.get("k") or default
来源：http://hz.snrcjt.cn/gtqenucess.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.shangyingyoupin.top/gtmleuomwp.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yj202588.top/gtmskbjstz.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shanyushiyangtech.top/gtkzrkrols.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.aizwys.cn/gtrvwovyue.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ydjk.org.cn/gtgnocdiqg.html

Ruby: d&.dig(:a, :b)
来源：http://hz.chenzaomai.com/gtxpucbvsa.html

C#:   obj?.A?.B ?? default
来源：http://hz.nanxuanxn.top/gttcavdwwd.html

[H07] 断言
来源：http://hz.meibo888.top/gtxjfpynjs.html

Py:   assert x > 0, "必须为正"
来源：http://hz.9152youxi.cn/gtwxdvudsi.html

PHP:  assert($x > 0);
来源：http://hz.aibaodan.cn/gtilkahjej.html

JS:   console.assert(x > 0);
来源：http://hz.fengsongda.top/gtyhdfvrwc.html

TS:   console.assert(x > 0);
来源：http://hz.havefunace.top/gtgitmtbgu.html

Java: assert x > 0 : "必须为正";
来源：http://hz.havefunace.top/gtjkfxqsbm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yueranfly.top/gtqvdstuuw.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinqigfzy.top/gtfbujdtks.html

C#:   Debug.Assert(x > 0);
来源：http://hz.fzhhl.top/gtjdnczehe.html

[H08] 获取错误信息与堆栈
来源：http://hz.zdqjudy.top/gtvgsojsnt.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yueranfly.top/gttecycwst.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenjidiqi.icu/gtiawaqrzn.html

JS:   e.message;  e.stack
来源：http://hz.ybcxt.top/gtlshmrqll.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.nwbrower.top/gtlqrkromn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.shanyushiyangkeji.top/gteqhrmgjs.html

Go:   err.Error()
来源：http://hz.xylfe.cn/gtifidyxuf.html

Ruby: e.message;  e.backtrace
来源：http://hz.wangdashe.top/gtajfjsjsc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.quarkkingdee.top/gtqbcxfteh.html

[H09] 带错误码的异常
来源：http://hz.vqdsnc.cn/gtqstlikml.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ybcxt.top/gtetpelimd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.xingfuxueyuan.xyz/gtalfgxsbn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yangfankeji.com/gtblcpuanx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jianghu66.top/gtljmdgtbc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ybcxt.top/gttujeifxe.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xinyue.icu/gtiswvrety.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.chenzaomai.com/gtuibhnbja.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.9152youxi.cn/gtgpinieyq.html

[H10] 资源自动释放
来源：http://hz.ydjk.org.cn/gtgpwhiyku.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.kuanghao11.cn/gttogdfuia.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ydjk.org.cn/gtumexsrux.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hysaishi.cn/gtjdegbsks.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yonumen.top/gtsvnnsoxd.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.shuidangran.top/gtupnzthxq.html

Go:   defer f.Close()
来源：http://hz.yongpay.top/gtpcusinkv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.mhx1999.top/gtozjeypzg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.meibo888.top/gtkpdkgsfh.html

================================================================================
来源：http://hz.9152youxi.cn/gttcibdonj.html

I. 正则表达式
来源：http://hz.hnqzz.top/gtfkxnozgi.html

================================================================================
来源：http://hz.iojbl.cn/gthtzweduy.html

[I01] 判断是否匹配
来源：http://hz.tian-w.cn/gtfwtrcdjg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.vqdsnc.cn/gtvywekkyj.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.aizwys.cn/gtcbiicmel.html

JS:   /\d+/.test(s)
来源：http://hz.zhongyouzk.top/gtbyuqdfjf.html

TS:   /\d+/.test(s)
来源：http://hz.zhijiandao.cn/gtvrswpurl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zycfv.cn/gtsrcfmtjb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.iojbl.cn/gtygxrytfj.html

Ruby: s.match?(/\d+/)
来源：http://hz.chenlongwang.top/gtjogfhocf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sxryk.cn/gtlhhcknlz.html

[I02] 提取所有匹配
来源：http://hz.zhongyouzk.top/gtigbesgmg.html

Py:   re.findall(r"\d+", s)
来源：http://hz.shanyushiyangtech.top/gtzsbdxvtd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.9152youxi.cn/gtrreeollu.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.52xcode.cn/gtxmtunynr.html

TS:   s.match(/\d+/g)
来源：http://hz.redwolf501.top/gtpmdoqylc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.chenzaomai.com/gtgdlisket.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ydzc1.top/gtwiwcmnvm.html

Ruby: s.scan(/\d+/)
来源：http://hz.hfpthk.cn/gtcqmydlty.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.daria6918.cn/gthypybkne.html

[I03] 提取捕获分组
来源：http://hz.jiagoushi.top/gtdnjzzwtg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.gzhubu.top/gtolwtudap.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ydzc1.top/gtkmvizgwp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yuanzhike.top/gtbwmszoqe.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yuanzhike.top/gtdvbvviad.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cqqwz.cn/gtosiqdegl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cdnleiting.top/gtrkeenzcp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.guannengcc.top/gtrundcmjs.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cucudq.cn/gtvwefjvzb.html

[I04] 正则替换
来源：http://hz.c1oappe.top/gttfrwotda.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yj20258888.top/gtzxbiqsoe.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yanxiufei.cn/gtkhepbape.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.bjfxy.top/gtbputssyb.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.dianchejie.cn/gtzoeecgbj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.nanxinkj.top/gtxahmjhml.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yuxming.cn/gtddeauwbe.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cucudq.cn/gtxxrqcfvd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ppjwa.cn/gtgtktorrt.html

[I05] 按正则拆分
来源：http://hz.tanke756.top/gtnebjgynd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.pengpengdd.cyou/gtbixqrhwr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.iojbl.cn/gtijvuyttt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gtkeglhkek.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sufxvd.cn/gtoyzrwjxx.html

Java: s.split("\\s*,\\s*")
来源：http://hz.dashuyun.cn/gtwnhiciup.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gogol.net.cn/gtnqcucsos.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jinyuanbaomall.cn/gtmtkqeisv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.bjfxy.top/gtmqnzxeso.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xinyue.icu/gtnexyrrfn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ydjk.org.cn/gtzflvyxuc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.gzhubu.top/gtdgcvoerq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ydzc1.top/gtrnvccngv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zdqjudy.top/gtyztiyugt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhixingplan.top/gtkgadfuxn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.daria6918.cn/gtwqxbbfro.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.chenjidiqi.icu/gtmnlwowig.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.andypj.xyz/gtqeygotfl.html

[I07] 忽略大小写与多行模式
来源：http://hz.zycfv.cn/gtbzjbraiy.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.redwolf501.top/gtjvbiaofk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jqgufenzy.top/gtkgkjowpf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zycfv.cn/gtmrlmlfjk.html

TS:   /error/gim
来源：http://hz.meibo888.top/gthwsiiwzn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yanxiufei.cn/gtuktguyhf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jyoumei.cn/gtfwbtktrn.html

Ruby: s.scan(/error/i)
来源：http://hz.vqdsnc.cn/gtdqzhlbmp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.chenzaomai.com/gtftseewro.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xinyue.icu/gtejfwogyc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hysaishi.cn/gtkorinlhh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhiwuduotai.top/gtoqwniath.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tian-w.cn/gtojjgqjmx.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinyuanbaomall.cn/gtjlzozllq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shanyushiyangtech.top/gteetsgmnv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.nanxuanxn.top/gtdlsbspwh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shangyingyoupin.top/gtrknrdbmc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jianghu66.top/gtxxinqlxq.html

================================================================================
来源：http://hz.redwolf501.top/gtefbltldo.html

J. 日期与时间
来源：http://hz.zycfv.cn/gtpaewhrdi.html

================================================================================
来源：http://hz.cqqwz.cn/gtoppafgnj.html

[J01] 获取当前时间
来源：http://hz.yangfankeji.com/gtijccaxgm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhengqikj.top/gtcnhsaqkg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cqqwz.cn/gthszpmbwi.html

JS:   new Date();  Date.now()
来源：http://hz.tian-w.cn/gtxhforonp.html

TS:   new Date();  Date.now()
来源：http://hz.fengsongda.top/gtybfdfkzg.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cqqwz.cn/gtezpcjehj.html

Go:   time.Now()
来源：http://hz.hfpthk.cn/gtniabcaqe.html

Ruby: Time.now
来源：http://hz.redwolf501.top/gtmdiglllp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.chenjidiqi.icu/gtilwmjxgi.html

[J02] 格式化输出
来源：http://hz.316326.xyz/gtsrizenrt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dianchejie.cn/gtvwiezvdb.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.snrcjt.cn/gtuzkpgplj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zycfv.cn/gthktmhdhd.html

TS:   d.toISOString()
来源：http://hz.zycfv.cn/gthepjrbia.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.pengpengdd.cyou/gtprmzpxkn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.bjfxy.top/gtgzflxove.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nwbrower.top/gtasqecnfd.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.cqqwz.cn/gtsbntjyiu.html

[J03] 字符串解析为日期
来源：http://hz.ywan-chungtsiang.top/gtrwdgmspl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinghuilouyu.cn/gtswkugmhm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sxryk.cn/gtfnvovrht.html

JS:   new Date("2024-01-02")
来源：http://hz.meibo888.top/gtszrzrjka.html

TS:   new Date("2024-01-02")
来源：http://hz.wangshuangyany.cn/gtxartnjov.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yj20258888.top/gtcxqjyiai.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.svipenyu.cn/gtamkfabbb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhijiandao.cn/gtxxqsrdxm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.kuanghao11.cn/gtlfsqhxkm.html

[J04] 时间戳与日期互转
来源：http://hz.sweek.top/gtvxrkunmv.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yvedp.cn/gtfwyztjjo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.feifeiyinyue.top/gtpsibijct.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.cqqwz.cn/gtwzxhyxoe.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.smart0.xyz/gtyyavfchj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xuanzx.com/gtkuqpquvz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xinyue.icu/gtvymtaqld.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.daxiang520.top/gtyzxmieyk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.gotoacloud.top/gtbflsflbh.html

[J05] 时间加减（加 7 天）
来源：http://hz.hfpthk.cn/gtwljczqny.html

Py:   now + timedelta(days=7)
来源：http://hz.zhiwuduotai.top/gtbnvrjvff.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgfzy.top/gtwqpekype.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigfzy.top/gtcodljxco.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yangfankeji.com/gtrloyeeoq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.9152youxi.cn/gtvcmxqpus.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hfpthk.cn/gtlzvnvkkm.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ywan-chungtsiang.top/gtwbddemgr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yanxiufei.cn/gtluzhhqeb.html

[J06] 计算两时间之差
来源：http://hz.yueranfly.top/gtcibzpmif.html

Py:   (end - start).total_seconds()
来源：http://hz.gogol.net.cn/gtgunhzzau.html

PHP:  $end->diff($start)->days;
来源：http://hz.nwbrower.top/gtosjhfwfq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xylfe.cn/gtmqedtebk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cdnleiting.top/gtbblfpwap.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.tianlin.xyz/gtvmihsbht.html

Go:   end.Sub(start).Hours()
来源：http://hz.ydzc1.top/gtreccesfc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.aizwys.cn/gtlcosvxzv.html

C#:   (end - start).TotalSeconds
来源：http://hz.sweek.top/gtuwxavvfk.html

[J07] 比较两个日期
来源：http://hz.vqdsnc.cn/gtlcjpqizf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yj20258888.top/gthiepouly.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.chenlongwang.top/gttapqzmew.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.kuanghao11.cn/gtycltktfe.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.bjfxy.top/gtwwilgdse.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xuetiantiany.cn/gtgfukisgb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hfpthk.cn/gtcijykgmo.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zhixingplan.top/gttplvyryb.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangtech.top/gtvuuoiozt.html

[J08] 提取年月日与星期
来源：http://hz.cashguo.top/gtohwrvmik.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yangfankeji.com/gtvcwvcmdp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sweek.top/gtdjmuvoxq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xziqi.cn/gtugyalbrp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jianghu66.top/gtujoxgxjg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.svipenyu.cn/gtibitrzzv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yonumen.top/gtjvbwodad.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenjidiqi.icu/gtvxtzyvqv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xylfe.cn/gtubtoycft.html

[J09] 时区处理
来源：http://hz.zhixingplan.top/gtiuzfyall.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jlsjyb.cn/gtotxobtaa.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yueranfly.top/gtilrjfkmx.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tian-w.cn/gtwispddvg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.daxiang520.top/gtgcyfslha.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.316326.xyz/gthvrlvuvx.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hysaishi.cn/gtagwqpuet.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.havefunace.top/gtyyzpcuri.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ywan-chungtsiang.top/gtzfhxzidi.html

[J10] 取今天 / 本月第一天
来源：http://hz.chenlongwang.top/gtwgnrrucb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cucudq.cn/gtdbwlnchb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhiwuduotai.top/gtsgyxtpqc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gaohongyu789.top/gttyxuztfa.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ydzc1.top/gtvnbegfmg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sufxvd.cn/gtjideegkk.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.ppjwa.cn/gtpnfyltct.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shanyushiyangtech.top/gthclyxzky.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhaomingkeji.xyz/gtvgdhbjif.html

================================================================================
来源：http://hz.vqdsnc.cn/gtowzbnqzd.html

K. JSON 与序列化
来源：http://hz.jiagoushi.top/gtyldrhcdr.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtryznqnel.html

[K01] 对象转 JSON 字符串
来源：http://hz.birdmap.top/gtknzjainz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinqigufen.top/gttodcjtuf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zycfv.cn/gtpxcyxivq.html

JS:   JSON.stringify(obj)
来源：http://hz.ppjwa.cn/gtrnoerbpf.html

TS:   JSON.stringify(obj)
来源：http://hz.jqgfzy.top/gtguprbfos.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinghuilouyu.cn/gtulcyyoup.html

Go:   json.Marshal(obj)
来源：http://hz.ppjwa.cn/gtehoyxuga.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.vqdsnc.cn/gtdnppzsxu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhaomingkeji.xyz/gtbbozwhdq.html

[K02] JSON 字符串转对象
来源：http://hz.cqqwz.cn/gtkenifouy.html

Py:   json.loads(s)
来源：http://hz.jqgfzy.top/gtbvjmrdml.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.aizwys.cn/gteuptanyk.html

JS:   JSON.parse(s)
来源：http://hz.nanxinkj.top/gttdodsxdv.html

TS:   JSON.parse(s)
来源：http://hz.ydjk.org.cn/gtpkswgatb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.chenjidiqi.icu/gtfrlizmel.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.andypj.xyz/gtgwkdhpkr.html

Ruby: JSON.parse(s)
来源：http://hz.fzhhl.top/gthqzmzjin.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.tanke756.top/gtgkdrbcfo.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.mhx1999.top/gtfdpohiki.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jiagoushi.top/gtwtcihajx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.fengsongda.top/gtacrhtjae.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhengqikj.top/gtzmwwolnn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.guowangkeji.top/gtadjyygck.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ydzc1.top/gtuzotofqw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.ydjk.org.cn/gtnegmuxks.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.shzxlz.cn/gtfdrimyhq.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.svipenyu.cn/gttoiuydee.html

[K04] 读取 JSON 文件
来源：http://hz.hammf.cn/gtlplffrvf.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.gzhubu.top/gtrzhelohu.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ydzc1.top/gtdhzvejee.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yj20258888.top/gtkqjlnmpr.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhaomingkeji.xyz/gtesuqvhka.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yuxming.cn/gtvqnqrace.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.jlsjyb.cn/gtkmkwthje.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.meibo888.top/gtyijnjoix.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.jiagoushi.top/gtunfhaove.html

[K05] 深拷贝对象
来源：http://hz.zycfv.cn/gttnvoaeaa.html

Py:   copy.deepcopy(obj)
来源：http://hz.ydzc1.top/gtnbkddcus.html

PHP:  unserialize(serialize($obj));
来源：http://hz.shuidangran.top/gtzleufeet.html

JS:   structuredClone(obj)
来源：http://hz.mhx1999.top/gtthgftqvx.html

TS:   structuredClone(obj)
来源：http://hz.yangfankeji.com/gtcfyyfvwu.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.zhiwuduotai.top/gthicjroet.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yueranfly.top/gthxnekzcx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.pengpengdd.cyou/gtstkugxxx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.sxryk.cn/gtvsjrhmcf.html

[K06] 解析 URL 查询串
来源：http://hz.hnxiangtu.top/gtmyqjbkal.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.zhongyouzk.top/gtcfhhffuy.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.hnxiangtu.top/gtfyvwtnxk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.cashguo.top/gtvvpfmxkz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.shanyushiyangkeji.top/gtqgygafxa.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.cdnleiting.top/gtlbsokrrw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.sxryk.cn/gtpkcuecme.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ydjk.org.cn/gtrzxolaka.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.chenjidiqi.icu/gtvsvcwfqb.html

[K07] 进制转换
来源：http://hz.quarkkingdee.top/gtfoqnsssm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.cheryme.top/gttgwitnmi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.aizwys.cn/gtpmapauit.html


<!-- 参考信息 -->