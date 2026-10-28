代发 wailian999

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.wangdashe.top/gtsmtidydb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yueranfly.top/gtvpqiioth.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yuanzhike.top/gtachvirgj.html

[H02] finally / ensure 收尾
来源：http://hz.smart0.xyz/gthideqrxi.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yuanzhike.top/gtctvhbzxl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.vqdsnc.cn/gtibhhqrbx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtauocgggm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xziqi.cn/gtqwjqxivc.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gthbmabxxw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.quarkkingdee.top/gtvnpbntaz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.nanxinkj.top/gtchraaotu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cucudq.cn/gtevtaqfzu.html

[H03] 主动抛出异常
来源：http://hz.xuetiantiany.cn/gtwwmdzjnq.html

Py:   raise ValueError("错误信息")
来源：http://hz.yvedp.cn/gtxchnybaw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.zhoulong.xyz/gtrjijarhx.html

JS:   throw new Error("错误信息");
来源：http://hz.sweek.top/gtcytgazvj.html

TS:   throw new Error("错误信息");
来源：http://hz.ydzc1.top/gtaoehdkhe.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhengqikj.top/gtrmnfcind.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shuidangran.top/gtqyupzged.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sufxvd.cn/gtmqoqllhp.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhiwuduotai.top/gtbsemqdoc.html

[H04] 自定义异常类型
来源：http://hz.redwolf501.top/gtjanwfvbn.html

Py:   class MyError(Exception): pass
来源：http://hz.xziqi.cn/gthapmmuos.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.bjfxy.top/gtoixfefjp.html

JS:   class MyError extends Error {}
来源：http://hz.havefunace.top/gtxydnatnr.html

TS:   class MyError extends Error {}
来源：http://hz.zycfv.cn/gtevofclne.html

Java: class MyException extends RuntimeException {}
来源：http://hz.jlsjyb.cn/gticzndmla.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yj20258.top/gtncwwiyyy.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhengqikj.top/gtjmvjfqug.html

C#:   class MyException : Exception {}
来源：http://hz.ywan-chungtsiang.top/gtaxuwhuum.html

[H05] 捕获特定类型
来源：http://hz.cheryme.top/gtazxykrfj.html

Py:   except ValueError as e:
来源：http://hz.hfpthk.cn/gtowzekecx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.feifeiyinyue.top/gtimhodgtw.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhixingplan.top/gtskdvosjf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.52xcode.cn/gtypkdbtfi.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.chenzaomai.com/gtliksrzzt.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.316326.xyz/gtdkhgpjcs.html

Ruby: rescue ArgumentError => e
来源：http://hz.fengsongda.top/gtfblungxi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhijiandao.cn/gtgpxckcax.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jqgfzy.top/gtfrzhdhbl.html

Py:   value = d.get("k") or default
来源：http://hz.feifeiyinyue.top/gtnsgguytt.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jlsjyb.cn/gtcorzsmki.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.52xcode.cn/gtpdrvlezr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinyuanbaomall.cn/gtuvldcjcq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.vqdsnc.cn/gtsfhvtive.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.shanyushiyangtech.top/gtkkemjzgx.html

Ruby: d&.dig(:a, :b)
来源：http://hz.andypj.xyz/gtcqcraigv.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhongyouzk.top/gtxrunmjck.html

[H07] 断言
来源：http://hz.bjfxy.top/gtbtrlnotp.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinqigufen.top/gtshnnpcen.html

PHP:  assert($x > 0);
来源：http://hz.fengsongda.top/gtfhoareof.html

JS:   console.assert(x > 0);
来源：http://hz.gotoacloud.top/gtckynmapf.html

TS:   console.assert(x > 0);
来源：http://hz.fengsongda.top/gtozmdqjcz.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jinghuilouyu.cn/gttdmwarlk.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.chenlongwang.top/gtyptnprth.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xuetiantiany.cn/gtlkttqiab.html

C#:   Debug.Assert(x > 0);
来源：http://hz.meibo888.top/gtywecynwv.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhiwuduotai.top/gtyyqqyzmm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.shangyingyoupin.top/gtaiurvrtt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinqigufen.top/gtmmdizgkq.html

JS:   e.message;  e.stack
来源：http://hz.cheryme.top/gthsytjwie.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jianghu66.top/gtvcvioddo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.snrcjt.cn/gthntcbwyh.html

Go:   err.Error()
来源：http://hz.yj20258.top/gtylldptrm.html

Ruby: e.message;  e.backtrace
来源：http://hz.ydjk.org.cn/gtydggjetv.html

C#:   e.Message;  e.StackTrace
来源：http://hz.daxiang520.top/gtcowszzzu.html

[H09] 带错误码的异常
来源：http://hz.iojbl.cn/gtkuowqmvs.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.haohaochexian.top/gtqhwdcpqw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinqigufen.top/gtlndwwstl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yangfankeji.com/gtyycsgymb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.meibo888.top/gtcabwmbwd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinqigufen.top/gtrblpqstp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.chenzaomai.com/gtrhfmdgjp.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yj20258.top/gtqrvrisww.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhiwuduotai.top/gtsieihdwi.html

[H10] 资源自动释放
来源：http://hz.svipenyu.cn/gtbittcxko.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hfpthk.cn/gtrsesplfb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.chenjidiqi.icu/gtsstvizrm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gtnupmmuph.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yonumen.top/gtrjfwmvoa.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.cqqwz.cn/gtgfeagsyg.html

Go:   defer f.Close()
来源：http://hz.jiagoushi.top/gtfdpzipei.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.0kj1m.cn/gtsugpzvwc.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.nanxuanxn.top/gtwgdfstcc.html

================================================================================
来源：http://hz.9152youxi.cn/gtrbezovgw.html

I. 正则表达式
来源：http://hz.yuxming.cn/gtrdhqbphd.html

================================================================================
来源：http://hz.nanxuanxn.top/gteoucbfze.html

[I01] 判断是否匹配
来源：http://hz.sxryk.cn/gtxhmfynti.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xylfe.cn/gtgdlfadkc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.feifeiyinyue.top/gtrnfzuxnn.html

JS:   /\d+/.test(s)
来源：http://hz.svipenyu.cn/gtmrsfdadk.html

TS:   /\d+/.test(s)
来源：http://hz.shanyushiyangkeji.top/gtgugwdxow.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jlsjyb.cn/gtnljyqrbd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sxryk.cn/gtjsgavlhe.html

Ruby: s.match?(/\d+/)
来源：http://hz.gzhubu.top/gtmmyhfguj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jlsjyb.cn/gtouqrzkzl.html

[I02] 提取所有匹配
来源：http://hz.chenjidiqi.icu/gtorxjeoqk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.quarkkingdee.top/gtwditcqjc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.tanke756.top/gtukitowdv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.fengsongda.top/gtqknpiomg.html

TS:   s.match(/\d+/g)
来源：http://hz.quarkkingdee.top/gtnkvfcokd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yongpay.top/gttiaoroqb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.daxiang520.top/gtoinranzu.html

Ruby: s.scan(/\d+/)
来源：http://hz.bjfxy.top/gtdzhnoftg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhiwuduotai.top/gtldljlwwp.html

[I03] 提取捕获分组
来源：http://hz.zhengqikj.top/gtjzfnmxdb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.shangyingyoupin.top/gtknoredde.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.kuanghao11.cn/gteltlrocx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj20258888.top/gtcvtqevek.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xuanzx.com/gtgqafvpmz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.meibo888.top/gtywsgilrf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yueranfly.top/gthrvwyrxn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hysaishi.cn/gtfghbyawh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.daxiang520.top/gtdifmhoqs.html

[I04] 正则替换
来源：http://hz.yvedp.cn/gtoogewzbn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhengqikj.top/gtlqxmhyiw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.birdmap.top/gtmjxcmiry.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.sweek.top/gtzzddposi.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.iojbl.cn/gtjnqnkmgm.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jqgfzy.top/gtqcbzhxlh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.chenlongwang.top/gtglikfsyg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.meibo888.top/gtdwxqrhou.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xuetiantiany.cn/gtflsgokfg.html

[I05] 按正则拆分
来源：http://hz.aizwys.cn/gtmxnjbdek.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.52xcode.cn/gtbgcjegfr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.0kj1m.cn/gtsmnxzwxc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.andypj.xyz/gtocwatuxu.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.aizwys.cn/gtqkjakttj.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xziqi.cn/gtkxpibpjl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hongshengwenyu.top/gtiwesdwhg.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.svipenyu.cn/gtjkovqamm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.9152youxi.cn/gtwbiqkgjc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.sxryk.cn/gtbhstjogd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zycfv.cn/gtadufzfer.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.dianchejie.cn/gtsbgfqssw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yonumen.top/gtwzailwyg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jiagoushi.top/gtodmgobrj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jqgufenzy.top/gtqcsogwba.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.bjfxy.top/gtbtzrhves.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shzxlz.cn/gtfkwvgnak.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.chenjidiqi.icu/gtajnwavgu.html

[I07] 忽略大小写与多行模式
来源：http://hz.mhx1999.top/gtlkwszlue.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hongshengwenyu.top/gteigbqwhh.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zycfv.cn/gtwucxrdrd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xingfuxueyuan.xyz/gtkiinhrik.html

TS:   /error/gim
来源：http://hz.jiagoushi.top/gtewsdrfmz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hnxiangtu.top/gtabbyawbd.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.c1oappe.top/gtqapjgynp.html

Ruby: s.scan(/error/i)
来源：http://hz.smart0.xyz/gtpexfoqpn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.quarkkingdee.top/gtfmbjtefk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.nanxuanxn.top/gtcqdaqwdb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhiwuduotai.top/gtqwwvmgir.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hysaishi.cn/gtraivecks.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cashguo.top/gtchurbdlo.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenzaomai.com/gtrcnlokat.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.andypj.xyz/gtqehwpogt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jlsjyb.cn/gtefgtsyvk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.snrcjt.cn/gtypxuqejm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.c1oappe.top/gtghqwdcge.html

================================================================================
来源：http://hz.shzxlz.cn/gtfjtmrlzf.html

J. 日期与时间
来源：http://hz.yuanzhike.top/gtpfifeecj.html

================================================================================
来源：http://hz.0kj1m.cn/gtphhfvraz.html

[J01] 获取当前时间
来源：http://hz.gzhubu.top/gtzrmqfesw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hammf.cn/gtmeifzeda.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hnqzz.top/gtchrqkvbu.html

JS:   new Date();  Date.now()
来源：http://hz.ydjk.org.cn/gttgnszuli.html

TS:   new Date();  Date.now()
来源：http://hz.xingfuxueyuan.xyz/gtzwaxpusm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yangfankeji.com/gtprpzeeag.html

Go:   time.Now()
来源：http://hz.chenjidiqi.icu/gthnbbnqzg.html

Ruby: Time.now
来源：http://hz.aizwys.cn/gtrwtmienp.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ybcxt.top/gtfdptikna.html

[J02] 格式化输出
来源：http://hz.guannengcc.top/gtsslsgbay.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgufenzy.top/gtthrqxdfr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jinghuilouyu.cn/gtitawufyt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.chenzaomai.com/gtzcrhzikf.html

TS:   d.toISOString()
来源：http://hz.zhoulong.xyz/gtnduecngu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sysykeji.top/gtolpwjusp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yangfankeji.com/gtaiijrhek.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.snrcjt.cn/gtfpeqffml.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hnqzz.top/gtrotqgodm.html

[J03] 字符串解析为日期
来源：http://hz.nanxuanxn.top/gtjhteuhqo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.svipenyu.cn/gtyjblhoje.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.chenzaomai.com/gthdbcbjky.html

JS:   new Date("2024-01-02")
来源：http://hz.zycfv.cn/gtwjrefaid.html

TS:   new Date("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtvfxzrhnr.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.guannengcc.top/gtxhzjyfyv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.nanxinkj.top/gtwobpdkvt.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shzxlz.cn/gtiiewtixd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.smart0.xyz/gtcxwkzthh.html

[J04] 时间戳与日期互转
来源：http://hz.zhengqikj.top/gttgcsrmnh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.redwolf501.top/gtiwceipws.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ybcxt.top/gtctlxfgps.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ppjwa.cn/gtqoflbsfm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yangfankeji.com/gtxmlowstb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yj20258888.top/gtiuwrbxtf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hongshengwenyu.top/gtdjnkkqxv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zycfv.cn/gteaeolhkf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zycfv.cn/gtdcwhzgws.html

[J05] 时间加减（加 7 天）
来源：http://hz.yvedp.cn/gtdwkjpelq.html

Py:   now + timedelta(days=7)
来源：http://hz.ydjk.org.cn/gttqubnlkb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhaomingkeji.xyz/gtrwvcgkie.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shuidangran.top/gtmfttjtmd.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yuxming.cn/gtbdwojblu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ppjwa.cn/gtmzuyzmzc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xinyue.icu/gtrlfmnlcf.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hammf.cn/gtvcdzogzs.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.nanxuanxn.top/gttsngawnn.html

[J06] 计算两时间之差
来源：http://hz.smart0.xyz/gtynvqshca.html

Py:   (end - start).total_seconds()
来源：http://hz.cqqwz.cn/gtqpywhthh.html

PHP:  $end->diff($start)->days;
来源：http://hz.tianlin.xyz/gtzzadqwmp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ydzc1.top/gtggekvcga.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.dianchejie.cn/gthadzvndp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yvedp.cn/gtyjcgrjvg.html

Go:   end.Sub(start).Hours()
来源：http://hz.sweek.top/gthiaezywh.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shzxlz.cn/gtzjhfndgk.html

C#:   (end - start).TotalSeconds
来源：http://hz.gotoacloud.top/gtjjwvrawt.html

[J07] 比较两个日期
来源：http://hz.pengpengdd.cyou/gtdyedfnvk.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.0kj1m.cn/gtfhdutugk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.guowangkeji.top/gtnibvqxix.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ywan-chungtsiang.top/gtewqrnttn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.vqdsnc.cn/gtususmahz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cdnleiting.top/gtejvhifkk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinghuilouyu.cn/gttgmfqlhq.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangkeji.top/gtwwhtemry.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cashguo.top/gtdzwlccny.html

[J08] 提取年月日与星期
来源：http://hz.yj20258888.top/gtbtvbzydo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xuanzx.com/gtgkpgnpsw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.9152youxi.cn/gtkvdfmnlg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ehwqpu.com/gtegfdgxdb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhaomingkeji.xyz/gtpapysaqq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yj202588.top/gtwwrltbhm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.tian-w.cn/gtugdtgvfq.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.redwolf501.top/gtzlyfmkba.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.pengpengdd.cyou/gtyeobvwzt.html

[J09] 时区处理
来源：http://hz.zhengqikj.top/gthepuxxtm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yj202588.top/gtfcmljbup.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhiwuduotai.top/gtauyjhcvj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhoulong.xyz/gtgjniywjr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ppjwa.cn/gtwmwjdtto.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ehwqpu.com/gtpflvllnk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cheryme.top/gtjdgqeegw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.tanke756.top/gtowkrxsqc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhaomingkeji.xyz/gttcykjauh.html

[J10] 取今天 / 本月第一天
来源：http://hz.kuanghao11.cn/gtyrvgxrqt.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.chenjidiqi.icu/gtjywzhncd.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.mhx1999.top/gtkjfoocyt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.52xcode.cn/gtzsykxydb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.vqdsnc.cn/gtvvjqmqdi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.daxiang520.top/gtgszyzgeq.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.bjfxy.top/gtdogrbbbx.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yangfankeji.com/gtjaxsmhps.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.gotoacloud.top/gtjurhbnpp.html

================================================================================
来源：http://hz.jinqigufen.top/gttssarlgb.html

K. JSON 与序列化
来源：http://hz.yangfankeji.com/gtqxunbiwl.html

================================================================================
来源：http://hz.dashuyun.cn/gtafcjwpvx.html

[K01] 对象转 JSON 字符串
来源：http://hz.jinyuanbaomall.cn/gtzdtuwayq.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.iojbl.cn/gtfkbzqztg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.fengsongda.top/gtgpluvbqb.html

JS:   JSON.stringify(obj)
来源：http://hz.zhixingplan.top/gtputuzjsa.html

TS:   JSON.stringify(obj)
来源：http://hz.cdnleiting.top/gtzxfrhkoh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zdqjudy.top/gtsetdrmzk.html

Go:   json.Marshal(obj)
来源：http://hz.gaohongyu789.top/gtxyursopc.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhixingplan.top/gtldyjmbfl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cheryme.top/gtzypkaojr.html

[K02] JSON 字符串转对象
来源：http://hz.pengpengdd.cyou/gtjmiqmxnc.html

Py:   json.loads(s)
来源：http://hz.tian-w.cn/gtwfjwqefa.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yangfankeji.com/gtxgegeotm.html

JS:   JSON.parse(s)
来源：http://hz.hfpthk.cn/gtuykujfny.html

TS:   JSON.parse(s)
来源：http://hz.daxiang520.top/gtbdhnjyig.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.tanke756.top/gtpdrhxxxn.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinqigfzy.top/gtxcvykofk.html

Ruby: JSON.parse(s)
来源：http://hz.fzhhl.top/gtykqyiqns.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.aibaodan.cn/gtkuvwwapy.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.pengpengdd.cyou/gtzgbvbkkw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.vqdsnc.cn/gtkdgiaenz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zdqjudy.top/gtpjduntyi.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.fzhhl.top/gtasqdcelf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.svipenyu.cn/gtxeloqjrk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.yvedp.cn/gtjpmfwaym.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.shzxlz.cn/gtxxucqjkv.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gaohongyu789.top/gthbjzvgno.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.cheryme.top/gtynpldmmc.html

[K04] 读取 JSON 文件
来源：http://hz.jinyuanbaomall.cn/gtingmqzla.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yueranfly.top/gtesfphhil.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shzxlz.cn/gtuwcdduoj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhiwuduotai.top/gtjjeezccz.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.iojbl.cn/gtlxokwvmu.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ydzc1.top/gtpuieebip.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.xuanzx.com/gtkocadlip.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cheryme.top/gtudjpotsl.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.sxryk.cn/gtudqtwhmh.html

[K05] 深拷贝对象
来源：http://hz.redwolf501.top/gtmtpgbdsp.html

Py:   copy.deepcopy(obj)
来源：http://hz.ydjk.org.cn/gttlwdtvgc.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cashguo.top/gtqljlchgl.html

JS:   structuredClone(obj)
来源：http://hz.yuxming.cn/gtqpghbfag.html

TS:   structuredClone(obj)
来源：http://hz.kuanghao11.cn/gtripwxiid.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.pycfn.com/gtzszzbqkk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.ydjk.org.cn/gtciifxjvx.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.sxryk.cn/gtcxpqkosi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.feifeiyinyue.top/gtwmnpjxfg.html


<!-- 参考信息 -->