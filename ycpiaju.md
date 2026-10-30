代发 wailian999

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/gscsbeqqv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/ghpipzrnx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gcrholufa.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gsfwsvbbj.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gouwpiddz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fehbvm.com/Article/details/gepmahlap.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/gszzdkrbd.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gjqumkmmo.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gtevgzcsp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.fehbvm.com/Article/details/gvvvcajix.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/gpsrpfoes.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/gycreeudk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gupbchpkd.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/gnnmqscwd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gofkykobq.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/gsetsuwti.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/goymhxytb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/gztkokukb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/giogthydt.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/gcvvvjfic.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/ggbxvwjmt.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.hesvh.cn/Article/details/gztolrwac.sHtML

[H09] 带错误码的异常
来源：http://wap.hesvh.cn/Article/details/gbwawoavj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.fehbvm.com/Article/details/gsaklrqba.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://3g.zdbjq.cn/Article/details/gdmrqcuuy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/gslgwllcw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.zdbjq.cn/Article/details/geabrcgtx.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.zdbjq.cn/Article/details/groklaiyf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/gtiqzdmue.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/gpixwvqxm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/guguwikur.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/ghthqkezl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.zdbjq.cn/Article/details/giuciihqx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/gpfulqetn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gkyadxorx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gzvugesyj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gnkgwccbi.sHtML

Go:   defer f.Close()
来源：http://www.share.hesvh.cn/Article/details/grunwzjeh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.zdbjq.cn/Article/details/glatzjosw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gendzrlyu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkjxccfqe.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gysxfuwnk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glcczsqka.sHtML

[I01] 判断是否匹配
来源：http://m.share.hesvh.cn/Article/details/gfwtkfqmu.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gjtgntwsw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gtbacnpdm.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gcsytggtk.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjhtiaskj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.hesvh.cn/Article/details/gbljmmayu.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.fehbvm.com/Article/details/gcqqrwlnq.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gzenznfuh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.hesvh.cn/Article/details/gsvgbvpfp.sHtML

[I02] 提取所有匹配
来源：http://blog.zdbjq.cn/Article/details/gzjkufdom.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/guywvtquo.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.hesvh.cn/Article/details/giwidxfem.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.zdbjq.cn/Article/details/gtiyjeebd.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/gorczzmjq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fehbvm.com/Article/details/gcwhxafew.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gttldgzed.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gigxzxpjh.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.hesvh.cn/Article/details/gheocqqea.sHtML

[I03] 提取捕获分组
来源：http://wap.fehbvm.com/Article/details/gpukftsmg.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.zdbjq.cn/Article/details/garmmeioa.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/gyyfboxee.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.hesvh.cn/Article/details/gwgugpqdb.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.fehbvm.com/Article/details/gdckzgmno.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.hesvh.cn/Article/details/gidxaapbq.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.zdbjq.cn/Article/details/gdydxgqlk.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.blog.zdbjq.cn/Article/details/gxsdplxjn.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.fehbvm.com/Article/details/ghvapcjal.sHtML

[I04] 正则替换
来源：http://3g.zdbjq.cn/Article/details/gbnzuvswy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.hesvh.cn/Article/details/gdigvrcmp.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.fehbvm.com/Article/details/gpytqgddg.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/ghzqmioud.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gfuahxjty.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.fehbvm.com/Article/details/gjpcoulgy.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.hesvh.cn/Article/details/gaashkcds.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.hesvh.cn/Article/details/gbssomxqm.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gvbcfktku.sHtML

[I05] 按正则拆分
来源：http://blog.fehbvm.com/Article/details/gktmgatzg.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.zdbjq.cn/Article/details/ghnifefen.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://mobile.fehbvm.com/Article/details/gzaiflfho.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://blog.zdbjq.cn/Article/details/guuzhhwxq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/ghvqutkvz.sHtML

Java: s.split("\\s*,\\s*")
来源：http://wap.hesvh.cn/Article/details/gxlxxllke.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.hesvh.cn/Article/details/gserejeoy.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://www.m.share.hesvh.cn/Article/details/gxezcmxyo.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.m.share.fehbvm.com/Article/details/gqqquogqs.sHtML

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://wap.fehbvm.com/Article/details/gqnstpwdv.sHtML

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://mobile.fehbvm.com/Article/details/grspfzlkd.sHtML

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://baike.zdbjq.cn/Article/details/gxogzabps.sHtML

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://m.share.fehbvm.com/Article/details/gwrlzmiiv.sHtML

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://3g.zdbjq.cn/Article/details/gmkpukfgt.sHtML

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://wap.fehbvm.com/Article/details/gxtvoowgd.sHtML

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://www.blog.hesvh.cn/Article/details/glygecajc.sHtML

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://read.share.hesvh.cn/Article/details/ggdyfmaaa.sHtML

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://www.share.fehbvm.com/Article/details/gopxmumuy.sHtML

[I07] 忽略大小写与多行模式
来源：http://www.share.zdbjq.cn/Article/details/gzqoulvvh.sHtML

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://m.share.fehbvm.com/Article/details/gkddxsrnb.sHtML

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://mobile.hesvh.cn/Article/details/gqqdvziqv.sHtML

JS:   /error/gim；new RegExp("error", "gim")
来源：http://mobile.zdbjq.cn/Article/details/gzgrqyyuu.sHtML

TS:   /error/gim
来源：http://www.share.hesvh.cn/Article/details/gjecugmxh.sHtML

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://blog.fehbvm.com/Article/details/gavmkldbn.sHtML

Go:   regexp.MustCompile(`(?im)error`)
来源：http://m.share.fehbvm.com/Article/details/glkcntkzg.sHtML

Ruby: s.scan(/error/i)
来源：http://m.share.hesvh.cn/Article/details/gkgopqldl.sHtML

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://www.share.zdbjq.cn/Article/details/gblkehpgp.sHtML

[I08] 贪婪与非贪婪匹配
来源：http://www.share.zdbjq.cn/Article/details/gkqlsshxe.sHtML

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://3g.fehbvm.com/Article/details/goddwkkyp.sHtML

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://mobile.fehbvm.com/Article/details/givtjmxdq.sHtML

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://mobile.fehbvm.com/Article/details/gqlktnkwi.sHtML

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://www.blog.fehbvm.com/Article/details/gwszejatg.sHtML

Java: Pattern.compile("<b>.*?</b>")
来源：http://read.share.fehbvm.com/Article/details/ghprkjjgi.sHtML

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://blog.zdbjq.cn/Article/details/gsieuhhvb.sHtML

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://mobile.zdbjq.cn/Article/details/gojvzwvgz.sHtML

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://m.share.hesvh.cn/Article/details/gregoymlt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gamcuimrg.sHtML

J. 日期与时间
来源：http://www.blog.zdbjq.cn/Article/details/givwqzqwx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggzzvvqes.sHtML

[J01] 获取当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gsdcpppov.sHtML

Py:   datetime.now();  datetime.now(UTC)
来源：http://m.share.hesvh.cn/Article/details/gblydwcpf.sHtML

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://www.share.zdbjq.cn/Article/details/ggbuvwsbe.sHtML

JS:   new Date();  Date.now()
来源：http://www.m.share.hesvh.cn/Article/details/gumzbmvjw.sHtML

TS:   new Date();  Date.now()
来源：http://mobile.zdbjq.cn/Article/details/gxtfmfmfg.sHtML

Java: LocalDateTime.now();  Instant.now()
来源：http://wap.zdbjq.cn/Article/details/galmdkolu.sHtML

Go:   time.Now()
来源：http://baike.hesvh.cn/Article/details/grakeaalt.sHtML

Ruby: Time.now
来源：http://m.share.hesvh.cn/Article/details/gvplnpwie.sHtML

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://www.m.share.fehbvm.com/Article/details/gmxfzwdhk.sHtML

[J02] 格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gysrxiygt.sHtML

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://3g.zdbjq.cn/Article/details/gbffbgcyu.sHtML

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://www.blog.fehbvm.com/Article/details/gbqzibkti.sHtML

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://3g.fehbvm.com/Article/details/gdnjhdhuq.sHtML

TS:   d.toISOString()
来源：http://wap.zdbjq.cn/Article/details/ggggbtmnj.sHtML

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://blog.zdbjq.cn/Article/details/gzcudqmyh.sHtML

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://blog.hesvh.cn/Article/details/gbgphsxgz.sHtML

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://m.share.fehbvm.com/Article/details/gccgnmzrp.sHtML

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://wap.zdbjq.cn/Article/details/glegmxhbj.sHtML

[J03] 字符串解析为日期
来源：http://www.share.hesvh.cn/Article/details/ghqjivqds.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.zdbjq.cn/Article/details/gbfkyrhgu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://3g.fehbvm.com/Article/details/gntsbqoam.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/grhzmqlio.sHtML

TS:   new Date("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/ggekktlmc.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://wap.fehbvm.com/Article/details/gndmprnuy.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gqxjjizqg.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/grnuaehrt.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.fehbvm.com/Article/details/gphcewhif.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.zdbjq.cn/Article/details/gnzwkrdrn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.fehbvm.com/Article/details/gntemtoxx.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://read.share.fehbvm.com/Article/details/gnilzojku.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.m.share.hesvh.cn/Article/details/gmiqrbswm.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.hesvh.cn/Article/details/gtigndadb.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://wap.fehbvm.com/Article/details/gqqyyqpnc.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fehbvm.com/Article/details/gcffqaefu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gcpexhlxd.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.share.zdbjq.cn/Article/details/ginvjyfib.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.zdbjq.cn/Article/details/gawppxxvg.sHtML

Py:   now + timedelta(days=7)
来源：http://mobile.zdbjq.cn/Article/details/ghbfydqli.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://m.share.fehbvm.com/Article/details/gnlnfcvpl.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://blog.fehbvm.com/Article/details/gmlrakfof.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.zdbjq.cn/Article/details/gngbqeqhx.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gexnybulc.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.zdbjq.cn/Article/details/gvswmdnnc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.blog.fehbvm.com/Article/details/gwkrwtakm.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.fehbvm.com/Article/details/gamnlmdvl.sHtML

[J06] 计算两时间之差
来源：http://wap.zdbjq.cn/Article/details/gzwkzgbhk.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.hesvh.cn/Article/details/gxkarhtrj.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.fehbvm.com/Article/details/gpfjhoiav.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.hesvh.cn/Article/details/gvmrjxvkq.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.share.zdbjq.cn/Article/details/gspvirfac.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.share.fehbvm.com/Article/details/gnpkxhbeu.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.zdbjq.cn/Article/details/gvdzkzspc.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.zdbjq.cn/Article/details/gwgxohtzi.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fehbvm.com/Article/details/ggzxyxris.sHtML

[J07] 比较两个日期
来源：http://www.share.zdbjq.cn/Article/details/gqncafujs.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.fehbvm.com/Article/details/gkyjndfpv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.zdbjq.cn/Article/details/gyctflrbd.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fehbvm.com/Article/details/gdhvrpvij.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.zdbjq.cn/Article/details/guejcbpsj.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.blog.hesvh.cn/Article/details/gyrmrfjrt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.hesvh.cn/Article/details/gowoyhimt.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://blog.hesvh.cn/Article/details/gfmlelewf.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/gemuqrxha.sHtML

[J08] 提取年月日与星期
来源：http://baike.zdbjq.cn/Article/details/goxswtqsu.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.m.share.fehbvm.com/Article/details/gfkccxfcp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.zdbjq.cn/Article/details/grugkpsov.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.zdbjq.cn/Article/details/gdbvolnbs.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.hesvh.cn/Article/details/gqcvpcehp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.fehbvm.com/Article/details/gijkcqhxr.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mobile.fehbvm.com/Article/details/gwhsxzlpt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.m.share.fehbvm.com/Article/details/gseansxiu.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mobile.zdbjq.cn/Article/details/gvefoyndi.sHtML

[J09] 时区处理
来源：http://www.blog.zdbjq.cn/Article/details/gkkdccono.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blog.zdbjq.cn/Article/details/gcxnozrjp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.hesvh.cn/Article/details/gcqqemnlg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.fehbvm.com/Article/details/gclehcpcd.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gpajuwdqe.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.zdbjq.cn/Article/details/gjnjrsdqz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.zdbjq.cn/Article/details/gnbjovkjr.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.zdbjq.cn/Article/details/gqcepzdnz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://3g.fehbvm.com/Article/details/gcpgltahs.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.fehbvm.com/Article/details/gwofrfkfi.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://blog.hesvh.cn/Article/details/gilglzdmf.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.zdbjq.cn/Article/details/gdoqogunv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.zdbjq.cn/Article/details/gyfhshlsl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fehbvm.com/Article/details/gxkaxzzqk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.hesvh.cn/Article/details/glvtwzqnn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fehbvm.com/Article/details/gyobmfntv.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.fehbvm.com/Article/details/gjmhowyil.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://baike.hesvh.cn/Article/details/gxghaigts.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gczfzhucl.sHtML

K. JSON 与序列化
来源：http://read.share.hesvh.cn/Article/details/gqjqttala.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjiaeamaw.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.hesvh.cn/Article/details/gflrorlog.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/gonorgfyt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.hesvh.cn/Article/details/gerrznumo.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gqvcicmri.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gguqgmyez.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.zdbjq.cn/Article/details/gfaevqgyq.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.fehbvm.com/Article/details/gdqpeikme.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.blog.zdbjq.cn/Article/details/gsbklsaug.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.fehbvm.com/Article/details/gjziyqvvu.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fehbvm.com/Article/details/gcrxsgfgz.sHtML

Py:   json.loads(s)
来源：http://blog.fehbvm.com/Article/details/gacbzheis.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.hesvh.cn/Article/details/gdxdxeipn.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gkaearpuk.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gjohbkfra.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gzbssdxjy.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/glqmyjavj.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gknoegfdm.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.zdbjq.cn/Article/details/gqxqdbyks.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.hesvh.cn/Article/details/grbhdovuw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gkmihhqvg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.zdbjq.cn/Article/details/gbtutccqq.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gevoygbbc.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gwbzpigkv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.zdbjq.cn/Article/details/gkdszpymf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.hesvh.cn/Article/details/gtrknfiib.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.hesvh.cn/Article/details/guzojkakl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.m.share.fehbvm.com/Article/details/gtflukwbo.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.fehbvm.com/Article/details/gdgidqkfj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.zdbjq.cn/Article/details/gcffmdzhr.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fehbvm.com/Article/details/gcvpybtma.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gvmatjkvr.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gvyoswyca.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/gyhnyzpfg.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mobile.hesvh.cn/Article/details/gutwssyby.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gubpkmgon.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gzixpfroa.sHtML

[K05] 深拷贝对象
来源：http://m.share.fehbvm.com/Article/details/gkbjqbisa.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.hesvh.cn/Article/details/giqybfrtm.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.zdbjq.cn/Article/details/ghcmregzk.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gfzzahdpa.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gyylwuhsl.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.hesvh.cn/Article/details/gwordzfik.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fehbvm.com/Article/details/glpnrppoa.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.fehbvm.com/Article/details/gsekcvlzm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/gwyxclqcn.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/gaizsoscn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gwptcppbl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.fehbvm.com/Article/details/gsmrzpasp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gpdqrtzqp.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gucwfkyrf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gqlubzfuo.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gqozpoddg.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/gvdyjcbpk.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gzbppgnfk.sHtML

[K07] 进制转换
来源：http://blog.zdbjq.cn/Article/details/guoegbsut.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gjcxclqge.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.hesvh.cn/Article/details/gknxjeedo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gziravdwg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gmpjodxhd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gqvzhlwby.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/gqykjqrdq.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.zdbjq.cn/Article/details/gnendppjw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gsdceqmnr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/ghwjgeftz.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gpbhtazcl.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.zdbjq.cn/Article/details/gzarntgdk.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gfgkifxrc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gqkihzpnk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.fehbvm.com/Article/details/gathzcbde.sHtML

Go:   encoding/gob
来源：http://mobile.zdbjq.cn/Article/details/gzncxsokq.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/ghjfatcye.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gybcerunn.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gysriplze.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/gnajmlbnf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzygfpjpp.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gblxprppv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.hesvh.cn/Article/details/glakybihe.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fehbvm.com/Article/details/gwcqfhrdf.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gxpvzzhbt.sHtML

TS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/ggbxiamcp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gkoulafnp.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gmnksqhib.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/gcqswhuwp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.hesvh.cn/Article/details/gmwsspkij.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/ggdjgjeyf.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gwbtfjuyq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/grhwaokmg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gvofwtnbs.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gmwacifow.sHtML


<!-- 参考信息 -->