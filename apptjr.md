代发 wailian999

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhijiandao.cn/gtfbxuxedg.html

[H04] 自定义异常类型
来源：http://hz.xinyue.icu/gtzppgjsuq.html

Py:   class MyError(Exception): pass
来源：http://hz.sysykeji.top/gtfpsvabgk.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zdqjudy.top/gtjwfwymap.html

JS:   class MyError extends Error {}
来源：http://hz.wangdashe.top/gtkdnsmeaj.html

TS:   class MyError extends Error {}
来源：http://hz.shangyingyoupin.top/gtdizjmkpa.html

Java: class MyException extends RuntimeException {}
来源：http://hz.svipenyu.cn/gtharvqhmj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.cheryme.top/gtuslzrdtr.html

Ruby: class MyError < StandardError; end
来源：http://hz.tanke756.top/gtmmlbbaoq.html

C#:   class MyException : Exception {}
来源：http://hz.xinyue.icu/gtngvvcalt.html

[H05] 捕获特定类型
来源：http://hz.sxryk.cn/gtuyzaykds.html

Py:   except ValueError as e:
来源：http://hz.cqqwz.cn/gtxygwpkod.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zycfv.cn/gtimgrmvac.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shuidangran.top/gtrniuvgsb.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xuetiantiany.cn/gtmoxgropz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.shzxlz.cn/gtwudgzoqf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.dashuyun.cn/gtqskehfyj.html

Ruby: rescue ArgumentError => e
来源：http://hz.yuanzhike.top/gtvaatcdmq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.mhx1999.top/gtdreerifl.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhaomingkeji.xyz/gtxwnvsbnl.html

Py:   value = d.get("k") or default
来源：http://hz.c1oappe.top/gtsvpqymve.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.svipenyu.cn/gtptkuksem.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.redwolf501.top/gtroxvcxby.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.aizwys.cn/gttrihoywv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yueranfly.top/gtdacwvtgy.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sufxvd.cn/gtzhjackhp.html

Ruby: d&.dig(:a, :b)
来源：http://hz.9152youxi.cn/gtvditzafu.html

C#:   obj?.A?.B ?? default
来源：http://hz.nanxuanxn.top/gtrbsuewip.html

[H07] 断言
来源：http://hz.dianchejie.cn/gtveigimbd.html

Py:   assert x > 0, "必须为正"
来源：http://hz.aizwys.cn/gtspakzrdg.html

PHP:  assert($x > 0);
来源：http://hz.hywenlv.cn/gtduvuachv.html

JS:   console.assert(x > 0);
来源：http://hz.daria6918.cn/gtzlbuumna.html

TS:   console.assert(x > 0);
来源：http://hz.shuidangran.top/gtzxpqgabk.html

Java: assert x > 0 : "必须为正";
来源：http://hz.hammf.cn/gtyicjhbti.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinghuilouyu.cn/gtrjvbkhxn.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinqigfzy.top/gtrpdqabju.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zycfv.cn/gtovehdflt.html

[H08] 获取错误信息与堆栈
来源：http://hz.gzhubu.top/gttfmkxpie.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.birdmap.top/gtxexvgyin.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cucudq.cn/gtgyiriubh.html

JS:   e.message;  e.stack
来源：http://hz.sufxvd.cn/gtwvgwivxc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hnqzz.top/gtxqwdfnss.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hfpthk.cn/gtoljxbwzp.html

Go:   err.Error()
来源：http://hz.daxiang520.top/gtgtnuapje.html

Ruby: e.message;  e.backtrace
来源：http://hz.cucudq.cn/gtlktdhrnu.html

C#:   e.Message;  e.StackTrace
来源：http://hz.nanxuanxn.top/gtkekerocv.html

[H09] 带错误码的异常
来源：http://hz.nanxinkj.top/gtkizdvvij.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.nanxuanxn.top/gtjbteclem.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.tian-w.cn/gthazycwfv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhengqikj.top/gtiohskxia.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.feifeiyinyue.top/gtoqawgnga.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ppjwa.cn/gtewymckoc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.gotoacloud.top/gttoiziijo.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cucudq.cn/gtbzfbjzup.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.xingfuxueyuan.xyz/gtsrtrztyf.html

[H10] 资源自动释放
来源：http://hz.yuanzhike.top/gtropmfhiu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.kuanghao11.cn/gtgtrrcckw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ydjk.org.cn/gtumbflpfm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sxryk.cn/gtksjmaooe.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangkeji.top/gtbuejnafb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yanxiufei.cn/gtlhoeifeo.html

Go:   defer f.Close()
来源：http://hz.vqdsnc.cn/gtrwmjdwhv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhengqikj.top/gtknzhevov.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jyoumei.cn/gtbunkueih.html

================================================================================
来源：http://hz.jinqigufen.top/gttcrooruz.html

I. 正则表达式
来源：http://hz.jqgfzy.top/gtlwbabhah.html

================================================================================
来源：http://hz.c1oappe.top/gtngnuruhc.html

[I01] 判断是否匹配
来源：http://hz.tianlin.xyz/gtqibpldwt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.svipenyu.cn/gtjwgzlrqi.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.bjfxy.top/gtfzmlkmfq.html

JS:   /\d+/.test(s)
来源：http://hz.sufxvd.cn/gtizkjtsaf.html

TS:   /\d+/.test(s)
来源：http://hz.xuanzx.com/gtcmrgnhvs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.tian-w.cn/gtyavzmdnl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yueranfly.top/gthfowmfai.html

Ruby: s.match?(/\d+/)
来源：http://hz.jianghu66.top/gtvrxrdman.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.kuanghao11.cn/gtdyvqxgnq.html

[I02] 提取所有匹配
来源：http://hz.9152youxi.cn/gtceoyzhaj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.nwbrower.top/gtzwvcwprz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhaomingkeji.xyz/gtxzevvvds.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.chenjidiqi.icu/gtlugcjzpg.html

TS:   s.match(/\d+/g)
来源：http://hz.gzhubu.top/gtmswbalqc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhengqikj.top/gtghndqgzk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.wangdashe.top/gtpmpiskwu.html

Ruby: s.scan(/\d+/)
来源：http://hz.gogol.net.cn/gtuisxgnnx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhijiandao.cn/gtmmgrunnv.html

[I03] 提取捕获分组
来源：http://hz.jiagoushi.top/gtwyofpiei.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hfpthk.cn/gttbsvfqzq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gzhubu.top/gtyjkhaubh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.daxiang520.top/gtojdklzob.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.birdmap.top/gtrwtieoca.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhengqikj.top/gttbrwofuj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.pycfn.com/gtwbqrwoai.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shangyingyoupin.top/gtzblzvdss.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.iojbl.cn/gtwyhcdlgx.html

[I04] 正则替换
来源：http://hz.jlsjyb.cn/gtzguvkfku.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xylfe.cn/gtxxrpivxg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.daxiang520.top/gtfqifdmcd.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxinkj.top/gtryucsmxm.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.iojbl.cn/gtwgiignhr.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jyoumei.cn/gtxgfvlcer.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shangyingyoupin.top/gtooomrfqw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hysaishi.cn/gtvepdklvh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.pycfn.com/gtwlcekaoy.html

[I05] 按正则拆分
来源：http://hz.guowangkeji.top/gttkmanufj.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yonumen.top/gtkwdfcepj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jlsjyb.cn/gtgdqejjzk.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.kuanghao11.cn/gtpxbusgwn.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tianlin.xyz/gtewokazsi.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenzaomai.com/gtqobwaamv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.dashuyun.cn/gtwjyidvzd.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yuxming.cn/gtopbdfuop.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.andypj.xyz/gtrvkhrrht.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.dashuyun.cn/gtrkyygdwq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.daria6918.cn/gtqiquejsw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.316326.xyz/gtjldyyimg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hfpthk.cn/gtfrjrakmh.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangtech.top/gtnnisjtqb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jinqigufen.top/gtshgubcrh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hysaishi.cn/gtxfmbkqvh.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jqgufenzy.top/gtonzhzztv.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hongshengwenyu.top/gtpebmhxrw.html

[I07] 忽略大小写与多行模式
来源：http://hz.ydzc1.top/gtcnsjpeej.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yj20258888.top/gtgpvkkwrq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.shanyushiyangkeji.top/gtzsznuggz.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.smart0.xyz/gtizkgiolx.html

TS:   /error/gim
来源：http://hz.jqgufenzy.top/gtcqkavxoe.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.pycfn.com/gtqmyikwed.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yj20258.top/gtnqlrepfb.html

Ruby: s.scan(/error/i)
来源：http://hz.jinghuilouyu.cn/gthoijbbti.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shzxlz.cn/gtlnnmpygm.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.fengsongda.top/gtpfxsaixk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jqgfzy.top/gtmyplxiaa.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.chenlongwang.top/gtczcozgjj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cheryme.top/gthwrekyrp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hysaishi.cn/gtqkxmteys.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.nanxinkj.top/gtpdcdiinn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zhiwuduotai.top/gtzcslisbu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yongpay.top/gteeylyzhs.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jqgfzy.top/gtgzieuwqa.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtufztpmje.html

J. 日期与时间
来源：http://hz.xinyue.icu/gtssqtmoox.html

================================================================================
来源：http://hz.cdnleiting.top/gtzzmarhxk.html

[J01] 获取当前时间
来源：http://hz.yanxiufei.cn/gtjsthgssp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jianghu66.top/gtlcrifeyu.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shzxlz.cn/gtjydhexwb.html

JS:   new Date();  Date.now()
来源：http://hz.chenzaomai.com/gtvwexmsau.html

TS:   new Date();  Date.now()
来源：http://hz.jlsjyb.cn/gtfbqhhgkz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.kuanghao11.cn/gttuaxczar.html

Go:   time.Now()
来源：http://hz.xuanzx.com/gtxrmjdcvq.html

Ruby: Time.now
来源：http://hz.jinqigufen.top/gtdjzoauid.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhoulong.xyz/gtgupuwhvy.html

[J02] 格式化输出
来源：http://hz.meibo888.top/gtxhstlgzc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fengsongda.top/gtzkbifonc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yueranfly.top/gtnglalggk.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.cashguo.top/gtgmhufjmx.html

TS:   d.toISOString()
来源：http://hz.ivvv.top/gtirhgghen.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.redwolf501.top/gtccdblwjd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cdnleiting.top/gtaidpppcj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yanxiufei.cn/gtjukxglfg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.chenlongwang.top/gtcxybhivg.html

[J03] 字符串解析为日期
来源：http://hz.bjfxy.top/gtngqhwzxu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hongshengwenyu.top/gtogovukge.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ywan-chungtsiang.top/gtdderched.html

JS:   new Date("2024-01-02")
来源：http://hz.yuxming.cn/gtigamibsp.html

TS:   new Date("2024-01-02")
来源：http://hz.pycfn.com/gtftmvtmjx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtdosyjmtz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yuanzhike.top/gtclclaegs.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yvedp.cn/gtzgzakhmv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj202588.top/gtexpjbyww.html

[J04] 时间戳与日期互转
来源：http://hz.zhaomingkeji.xyz/gtlkkikyzn.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.sufxvd.cn/gttistagct.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xingfuxueyuan.xyz/gthcgrfsbi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.fzhhl.top/gttzzhimqt.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.dashuyun.cn/gtnrsvtnsz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.tian-w.cn/gtxwpzvfzd.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jqgufenzy.top/gtmgaialpo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yj20258.top/gteavwpvaq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hnxiangtu.top/gtowsptrtp.html

[J05] 时间加减（加 7 天）
来源：http://hz.hysaishi.cn/gtehnnjklw.html

Py:   now + timedelta(days=7)
来源：http://hz.52xcode.cn/gtlooanzps.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xziqi.cn/gtyatonlua.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sxryk.cn/gtnaqterlu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.smart0.xyz/gtgtakkvrx.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.0kj1m.cn/gtiagvrsej.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ivvv.top/gtsunmkfjh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ywan-chungtsiang.top/gtieppfbzt.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yvedp.cn/gtveyxcntg.html

[J06] 计算两时间之差
来源：http://hz.havefunace.top/gtstwlfqtf.html

Py:   (end - start).total_seconds()
来源：http://hz.9152youxi.cn/gtjauigcmj.html

PHP:  $end->diff($start)->days;
来源：http://hz.havefunace.top/gtlblfdppk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hongshengwenyu.top/gtatkvnyjv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.dashuyun.cn/gthxhxkbwa.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xinyue.icu/gtafozvuli.html

Go:   end.Sub(start).Hours()
来源：http://hz.nanxinkj.top/gtdywulpdq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yangfankeji.com/gtobtlwrik.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhaomingkeji.xyz/gtpzbsbcuh.html

[J07] 比较两个日期
来源：http://hz.birdmap.top/gtimznzzmk.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.daxiang520.top/gtjhdjrsgu.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xinyue.icu/gtpholiitt.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhoulong.xyz/gtieibgwly.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhengqikj.top/gtubbmfdbx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.havefunace.top/gtwhuththr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhiwuduotai.top/gtaonimyyf.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.havefunace.top/gtfsdgvfte.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zdqjudy.top/gtxevbaugs.html

[J08] 提取年月日与星期
来源：http://hz.shanyushiyangtech.top/gttazzqxhn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.sufxvd.cn/gtftrpgajq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.haohaochexian.top/gthzvjsdrs.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhiwuduotai.top/gtubgnlbrt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yangfankeji.com/gtqgbgnhgr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.vqdsnc.cn/gtlxoconeg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yj20258.top/gtnvihogox.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jinqigufen.top/gtdmsofaeh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.nanxuanxn.top/gtnfwhlmbh.html

[J09] 时区处理
来源：http://hz.havefunace.top/gtlocxnpsk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jianghu66.top/gtgjjjfepn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhongyouzk.top/gtamzkbxjf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dianchejie.cn/gtxubjgzgm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.aizwys.cn/gtlsigqtoi.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.tianlin.xyz/gtkueyxlww.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.guowangkeji.top/gtacpzyaod.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ydjk.org.cn/gtmcwjslkb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.nwbrower.top/gtappqiqxu.html

[J10] 取今天 / 本月第一天
来源：http://hz.fengsongda.top/gtgvwrhtpe.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gaohongyu789.top/gthvianshv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shuidangran.top/gtsoxkaraw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.nanxinkj.top/gtciufqfxz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yuxming.cn/gtlimpuwnb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.feifeiyinyue.top/gtmkcyknbm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yongpay.top/gtsxkgbddk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.kuanghao11.cn/gtulrllizw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.iojbl.cn/gtbrfaoozy.html

================================================================================
来源：http://hz.smart0.xyz/gtvmbswrnd.html

K. JSON 与序列化
来源：http://hz.zhaomingkeji.xyz/gtpwppywbf.html

================================================================================
来源：http://hz.gogol.net.cn/gtlxcewmuw.html

[K01] 对象转 JSON 字符串
来源：http://hz.ivvv.top/gtusgsbjpe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.316326.xyz/gthooltrui.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xuanzx.com/gtkbhiirte.html

JS:   JSON.stringify(obj)
来源：http://hz.ppjwa.cn/gteemyvtzh.html

TS:   JSON.stringify(obj)
来源：http://hz.bjfxy.top/gtxcqsuqpg.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.316326.xyz/gticdzhayq.html

Go:   json.Marshal(obj)
来源：http://hz.haohaochexian.top/gtkfpfisjg.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cheryme.top/gtnsekztil.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hysaishi.cn/gtiydjlxiq.html

[K02] JSON 字符串转对象
来源：http://hz.sysykeji.top/gtskygkrzc.html

Py:   json.loads(s)
来源：http://hz.gogol.net.cn/gtbxeetvar.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.wangdashe.top/gtrkoafios.html

JS:   JSON.parse(s)
来源：http://hz.yj20258888.top/gtzhfwpoot.html

TS:   JSON.parse(s)
来源：http://hz.andypj.xyz/gtutijdayz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.fzhhl.top/gtyhcawidu.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhaomingkeji.xyz/gtswdxgkos.html

Ruby: JSON.parse(s)
来源：http://hz.zhongyouzk.top/gtxadietdq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.pycfn.com/gtcnyxnxjt.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.cashguo.top/gtsdszxozx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cqqwz.cn/gtshjcnukb.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.52xcode.cn/gtufxlscdz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.dianchejie.cn/gtforkvsbp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shanyushiyangkeji.top/gtstialxrl.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xingfuxueyuan.xyz/gtjfnrfqsx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.chenjidiqi.icu/gtpijuxikj.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.jqgufenzy.top/gtuepjnevt.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.snrcjt.cn/gtgvxcmyap.html

[K04] 读取 JSON 文件
来源：http://hz.xziqi.cn/gtgylhbyme.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.guowangkeji.top/gtvxevbxsn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.yanxiufei.cn/gtavwlmdom.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fengsongda.top/gtsbonzong.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zdqjudy.top/gtzswwxaxo.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.daria6918.cn/gtwfzogdlj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yj20258888.top/gtsclpofax.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zhoulong.xyz/gtolnafcuh.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhixingplan.top/gtnsctamju.html

[K05] 深拷贝对象
来源：http://hz.zhijiandao.cn/gtvwfvockc.html

Py:   copy.deepcopy(obj)
来源：http://hz.cdnleiting.top/gtfzdjqcqp.html

PHP:  unserialize(serialize($obj));
来源：http://hz.gotoacloud.top/gtjtksjqpo.html

JS:   structuredClone(obj)
来源：http://hz.jianghu66.top/gtqcavkzoy.html

TS:   structuredClone(obj)
来源：http://hz.dianchejie.cn/gtpozkxikt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xinyue.icu/gttnxanqcj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.smart0.xyz/gtkblwzaba.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.redwolf501.top/gtnexnnipr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xylfe.cn/gtuqllhwan.html

[K06] 解析 URL 查询串
来源：http://hz.haohaochexian.top/gtgahanxwl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.jinyuanbaomall.cn/gtwytfiqwx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.zhaomingkeji.xyz/gtdqzphmfd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhijiandao.cn/gthknmicnh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xingfuxueyuan.xyz/gtbzkqzqtt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jyoumei.cn/gttesrrtay.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xingfuxueyuan.xyz/gtuodiozow.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.shuidangran.top/gtmrbxyhhi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.mhx1999.top/gtuhtadgxz.html

[K07] 进制转换
来源：http://hz.haohaochexian.top/gttghnltrm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.mhx1999.top/gtxgemzauo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.chenzaomai.com/gtvlhfyouh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yanxiufei.cn/gtnrlfwgdw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sweek.top/gtbdkkkybs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.aibaodan.cn/gtaqbcwuim.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.xingfuxueyuan.xyz/gtccnudghu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.jqgfzy.top/gtyfesysxi.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.sweek.top/gtwhvcscwb.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.0kj1m.cn/gttjcmvcqv.html

Py:   pickle.dumps(obj)
来源：http://hz.birdmap.top/gtedsiqpxc.html


<!-- 参考信息 -->