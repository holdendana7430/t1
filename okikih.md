代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ywan-chungtsiang.top/gteakdkaal.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.chenjidiqi.icu/gtykqoptfh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.sweek.top/gtysrwkdsz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.52xcode.cn/gtmddjpblp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gaohongyu789.top/gtzcrkyrky.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hnxiangtu.top/gtiwvluyor.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.aizwys.cn/gteegkxblv.html

[H02] finally / ensure 收尾
来源：http://hz.zdqjudy.top/gtduqinkrn.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhongyouzk.top/gtnazdmumj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtwzgyvwpp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtptpbfygj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.bjfxy.top/gtcutokbjg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.316326.xyz/gtggklkbrf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jyoumei.cn/gtpxzaifru.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yueranfly.top/gttpgaczob.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cdnleiting.top/gtmrpocwsd.html

[H03] 主动抛出异常
来源：http://hz.yuanzhike.top/gtvblrvvfo.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhoulong.xyz/gthstlazbt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.birdmap.top/gtqinnwqhs.html

JS:   throw new Error("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtmcerpynh.html

TS:   throw new Error("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtzdgqsqoh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yuanzhike.top/gtgtsmrvid.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinqigfzy.top/gtxkyrndol.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hnqzz.top/gtbkvvrfib.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xziqi.cn/gtydphztsf.html

[H04] 自定义异常类型
来源：http://hz.yvedp.cn/gtivmvwqed.html

Py:   class MyError(Exception): pass
来源：http://hz.gotoacloud.top/gtdsxamlki.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.kuanghao11.cn/gtqzkaumpx.html

JS:   class MyError extends Error {}
来源：http://hz.c1oappe.top/gtlcqvfjie.html

TS:   class MyError extends Error {}
来源：http://hz.yanxiufei.cn/gtnsieugeb.html

Java: class MyException extends RuntimeException {}
来源：http://hz.smart0.xyz/gtpbjsgpzg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ydzc1.top/gtjobjqqxj.html

Ruby: class MyError < StandardError; end
来源：http://hz.c1oappe.top/gttcrdzmdm.html

C#:   class MyException : Exception {}
来源：http://hz.yj20258.top/gtdefmjzcz.html

[H05] 捕获特定类型
来源：http://hz.bjfxy.top/gtjtksyuuk.html

Py:   except ValueError as e:
来源：http://hz.hnxiangtu.top/gtlouyoqun.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cqqwz.cn/gtimbijilf.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tian-w.cn/gtxpbsimhx.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.dianchejie.cn/gtmmglnptb.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.birdmap.top/gtxvhtafcz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jlsjyb.cn/gtfznnbqbr.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhixingplan.top/gtuuzritpk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.dashuyun.cn/gtshopszis.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sufxvd.cn/gtifvvwite.html

Py:   value = d.get("k") or default
来源：http://hz.aibaodan.cn/gtujbdtuxw.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hongshengwenyu.top/gtpopqmwak.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jyoumei.cn/gtvmhulqgd.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.feifeiyinyue.top/gtieejbgmi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.meibo888.top/gteruptxki.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.xuetiantiany.cn/gtuqmwsehu.html

Ruby: d&.dig(:a, :b)
来源：http://hz.nwbrower.top/gtyhdgkflk.html

C#:   obj?.A?.B ?? default
来源：http://hz.smart0.xyz/gtbhqmzmvo.html

[H07] 断言
来源：http://hz.0kj1m.cn/gtfsjbxvoz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinqigfzy.top/gtalonkdzm.html

PHP:  assert($x > 0);
来源：http://hz.chenjidiqi.icu/gtrvdaavxy.html

JS:   console.assert(x > 0);
来源：http://hz.yongpay.top/gtpxzfuecl.html

TS:   console.assert(x > 0);
来源：http://hz.xuetiantiany.cn/gtipzrsmxo.html

Java: assert x > 0 : "必须为正";
来源：http://hz.fengsongda.top/gtkpsbxzga.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yuxming.cn/gtnforwxdo.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.dianchejie.cn/gtvvilbkqo.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hongshengwenyu.top/gtglincbgs.html

[H08] 获取错误信息与堆栈
来源：http://hz.yanxiufei.cn/gtzassvufg.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yuanzhike.top/gtcjypjncy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shzxlz.cn/gtobqkywbd.html

JS:   e.message;  e.stack
来源：http://hz.daxiang520.top/gtqrcabnip.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jqgufenzy.top/gtgypymiqh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hnqzz.top/gtcmhycbzi.html

Go:   err.Error()
来源：http://hz.jqgufenzy.top/gtypstwhkf.html

Ruby: e.message;  e.backtrace
来源：http://hz.gogol.net.cn/gtmlggrhve.html

C#:   e.Message;  e.StackTrace
来源：http://hz.hfpthk.cn/gtxzofqtur.html

[H09] 带错误码的异常
来源：http://hz.yuanzhike.top/gtflokfsal.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.wangdashe.top/gtokukunsf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.316326.xyz/gtsbolmzpf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yongpay.top/gtxcxlgvhf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.sysykeji.top/gtumlqojvp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.tanke756.top/gtvnelelgk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cqqwz.cn/gtxxkqwofp.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.tian-w.cn/gtilqdeghl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.redwolf501.top/gtsmtdyvvq.html

[H10] 资源自动释放
来源：http://hz.cheryme.top/gtaeshduwg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.dianchejie.cn/gtrtkcarrc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj20258.top/gtsvkccxzn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jianghu66.top/gtyjakzvri.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.meibo888.top/gtzlrfofuj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.tanke756.top/gtmkdloxhv.html

Go:   defer f.Close()
来源：http://hz.meibo888.top/gtcpagwnkb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.daria6918.cn/gtxpjghdna.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhengqikj.top/gtjoscglvs.html

================================================================================
来源：http://hz.yj20258888.top/gtredaxcic.html

I. 正则表达式
来源：http://hz.guowangkeji.top/gtyatfghut.html

================================================================================
来源：http://hz.yueranfly.top/gtoctyiugv.html

[I01] 判断是否匹配
来源：http://hz.52xcode.cn/gtgagzhjot.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.9152youxi.cn/gtvtibysgu.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gzhubu.top/gtqqsciizv.html

JS:   /\d+/.test(s)
来源：http://hz.ydzc1.top/gtvmdtipoo.html

TS:   /\d+/.test(s)
来源：http://hz.shanyushiyangtech.top/gtyrwfkfhl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.pycfn.com/gtmmdxwhpb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yonumen.top/gtrqzitovc.html

Ruby: s.match?(/\d+/)
来源：http://hz.haohaochexian.top/gtjvfifhew.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.quarkkingdee.top/gtldxakjch.html

[I02] 提取所有匹配
来源：http://hz.hfpthk.cn/gtizqfcdhy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.dashuyun.cn/gtohzhuypk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ehwqpu.com/gtjoahriwn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yj20258.top/gtzqszckpp.html

TS:   s.match(/\d+/g)
来源：http://hz.9152youxi.cn/gtdvpgyyxd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.nanxuanxn.top/gtlovolfzx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ybcxt.top/gtrdjlkkrv.html

Ruby: s.scan(/\d+/)
来源：http://hz.wangdashe.top/gtgomwspwi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.tian-w.cn/gtcsazzyif.html

[I03] 提取捕获分组
来源：http://hz.chenzaomai.com/gtjmpiykhz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.chenlongwang.top/gtjifxbatj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.chenlongwang.top/gtzmtpbvrn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.bjfxy.top/gtqxcemzan.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.andypj.xyz/gtuwfuncwo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.tian-w.cn/gtamfutyeu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj202588.top/gtcjgnxvix.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.chenzaomai.com/gtlesuxcmn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.pengpengdd.cyou/gtzviusugh.html

[I04] 正则替换
来源：http://hz.xuetiantiany.cn/gtdghdlfzn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zdqjudy.top/gtukcnfijm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cdnleiting.top/gtntvpqzsg.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jianghu66.top/gtdloaxbdw.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yueranfly.top/gthqgadasz.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.aibaodan.cn/gtuoccyskz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.tianlin.xyz/gtnzygkefr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nanxinkj.top/gtfqfmglju.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.tianlin.xyz/gtglbliijl.html

[I05] 按正则拆分
来源：http://hz.sysykeji.top/gtuquyvetz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.dianchejie.cn/gtlokjsgcw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ybcxt.top/gtqggqqniq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gtcsiiszfc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jqgufenzy.top/gtzkszfqbv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhiwuduotai.top/gtiukrgkej.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gzhubu.top/gtnnpemfwz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nanxuanxn.top/gtwxnsagwo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gaohongyu789.top/gtttuohqbj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jiagoushi.top/gtkcwjvjaq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.xylfe.cn/gtmsdrahsk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.kuanghao11.cn/gteqnwzdrr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.quarkkingdee.top/gtjhbuoicq.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhixingplan.top/gtekaptncm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.nanxinkj.top/gtwrwfkecx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.fzhhl.top/gtirhvxzcx.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ydzc1.top/gtnadfyqdr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yvedp.cn/gtakrrvnvg.html

[I07] 忽略大小写与多行模式
来源：http://hz.guowangkeji.top/gtumgapsst.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jlsjyb.cn/gttyevkkfa.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.andypj.xyz/gtmmsaisam.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ivvv.top/gtccwzhqwv.html

TS:   /error/gim
来源：http://hz.xuetiantiany.cn/gtuwltcibb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.guannengcc.top/gtwsyldyiz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shanyushiyangtech.top/gtadzobkzm.html

Ruby: s.scan(/error/i)
来源：http://hz.iojbl.cn/gtlaxamxzz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cashguo.top/gtwzjijtyh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gzhubu.top/gtvbvuzcbt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jinqigufen.top/gtxsxmbltc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cqqwz.cn/gtkjycwxai.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yongpay.top/gtaodmbsbi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ivvv.top/gtfqvzskmt.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.chenlongwang.top/gtxzejcuzi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shanyushiyangtech.top/gtcpftylfu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shzxlz.cn/gtwezqbviw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jqgfzy.top/gthzpjyfvu.html

================================================================================
来源：http://hz.redwolf501.top/gtwvdaykxg.html

J. 日期与时间
来源：http://hz.jianghu66.top/gtlgomaugs.html

================================================================================
来源：http://hz.cdnleiting.top/gtoccozcof.html

[J01] 获取当前时间
来源：http://hz.jinyuanbaomall.cn/gtiwfmonmc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinyuanbaomall.cn/gtdjlqsbso.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.gaohongyu789.top/gtincddjxb.html

JS:   new Date();  Date.now()
来源：http://hz.jyoumei.cn/gtufbbnnfg.html

TS:   new Date();  Date.now()
来源：http://hz.yj20258888.top/gtjqbaanwy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.wangdashe.top/gtiggxwqkc.html

Go:   time.Now()
来源：http://hz.sxryk.cn/gtlrxfksns.html

Ruby: Time.now
来源：http://hz.fzhhl.top/gtrwhszhbk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yj20258.top/gtbpobwcyb.html

[J02] 格式化输出
来源：http://hz.xinyue.icu/gtvfyrtxpi.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yongpay.top/gtixopfecl.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hongshengwenyu.top/gtohhagxrn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.fengsongda.top/gtwvzwduod.html

TS:   d.toISOString()
来源：http://hz.kuanghao11.cn/gtorimfaxk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.chenjidiqi.icu/gtfsmenkga.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hysaishi.cn/gtmbyzkbzf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ybcxt.top/gtwmzllopb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shanyushiyangkeji.top/gtiucwamfi.html

[J03] 字符串解析为日期
来源：http://hz.pengpengdd.cyou/gtlwwrjvyv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yj20258888.top/gtamuztunh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhijiandao.cn/gthnszpbdb.html

JS:   new Date("2024-01-02")
来源：http://hz.yj202588.top/gtsdzcbcwx.html

TS:   new Date("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtiblayoti.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hammf.cn/gtmfcbigri.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xinyue.icu/gtvsdgecpl.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtyffifnwo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cucudq.cn/gtjnvjddst.html

[J04] 时间戳与日期互转
来源：http://hz.tanke756.top/gtkmljakjj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhaomingkeji.xyz/gtmihuvruo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhiwuduotai.top/gtsfhiqbrk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xuetiantiany.cn/gtmexhwrmr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yanxiufei.cn/gtohxxcrps.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.havefunace.top/gtsalodhdm.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hnxiangtu.top/gtwoycbykk.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.pengpengdd.cyou/gtcomirsbs.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shanyushiyangtech.top/gtvmvlwakq.html

[J05] 时间加减（加 7 天）
来源：http://hz.guowangkeji.top/gtpcbxymbp.html

Py:   now + timedelta(days=7)
来源：http://hz.jianghu66.top/gtceejifzt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jinghuilouyu.cn/gtunfyimla.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gotoacloud.top/gtbpabgnwo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.52xcode.cn/gtechdsnim.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj20258.top/gtolwvqvpf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.daxiang520.top/gtrugueehr.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yuanzhike.top/gtwaifsmkc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.fzhhl.top/gtcvgetpcl.html

[J06] 计算两时间之差
来源：http://hz.chenzaomai.com/gtavnourkm.html

Py:   (end - start).total_seconds()
来源：http://hz.wangshuangyany.cn/gtymxsfaln.html

PHP:  $end->diff($start)->days;
来源：http://hz.dashuyun.cn/gtowwgqffg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jiagoushi.top/gtzpxofbwr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sysykeji.top/gtlhxhyvot.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.316326.xyz/gtmjczlbrd.html

Go:   end.Sub(start).Hours()
来源：http://hz.jiagoushi.top/gtqolizyoq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.316326.xyz/gtofgxrkdt.html

C#:   (end - start).TotalSeconds
来源：http://hz.redwolf501.top/gtydfhaccp.html

[J07] 比较两个日期
来源：http://hz.aizwys.cn/gtdyefrkff.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.gzhubu.top/gtvgihyplx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shuidangran.top/gtzultkdyn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gtkvresihy.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinqigfzy.top/gthnqlphel.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xingfuxueyuan.xyz/gtgnfjmjhv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.nanxinkj.top/gtazpitviu.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.quarkkingdee.top/gtamobindb.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.quarkkingdee.top/gtheynsknm.html

[J08] 提取年月日与星期
来源：http://hz.zhixingplan.top/gtbehwxqmw.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.gotoacloud.top/gtsllthsby.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.fengsongda.top/gtyzfclngm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.bjfxy.top/gtzjjanpqw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jqgfzy.top/gtshcapyxt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.guowangkeji.top/gtfattuidl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.52xcode.cn/gtfggwowwy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhoulong.xyz/gtjamtnftx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gzhubu.top/gtckubvxfz.html

[J09] 时区处理
来源：http://hz.ybcxt.top/gtbsutljxd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.jinyuanbaomall.cn/gtfrvqcjdp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.fengsongda.top/gtesxdqfpz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhixingplan.top/gttusxhztr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.fzhhl.top/gtcaegcdjg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.chenzaomai.com/gthuwvloox.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.tian-w.cn/gtvkfekwtr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cdnleiting.top/gtkibztrqo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shangyingyoupin.top/gtpwxkirod.html

[J10] 取今天 / 本月第一天
来源：http://hz.nanxinkj.top/gtozutseik.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.9152youxi.cn/gtkyrfkkfb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yangfankeji.com/gtjxhhkzfi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.daria6918.cn/gtiaadwtre.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhixingplan.top/gtcebxkdzg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ydjk.org.cn/gtglbhvzed.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cqqwz.cn/gtkrsluoqf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hnxiangtu.top/gtunsuxivi.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xuanzx.com/gtxftsbazn.html

================================================================================
来源：http://hz.cqqwz.cn/gtzhbknciz.html

K. JSON 与序列化
来源：http://hz.sysykeji.top/gthfcuouje.html

================================================================================
来源：http://hz.guowangkeji.top/gthibtbgyr.html

[K01] 对象转 JSON 字符串
来源：http://hz.xuanzx.com/gtdrwzonal.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.nanxuanxn.top/gtcibgycjj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhijiandao.cn/gtpudgsgmu.html

JS:   JSON.stringify(obj)
来源：http://hz.chenjidiqi.icu/gtoxlgyxuw.html

TS:   JSON.stringify(obj)
来源：http://hz.redwolf501.top/gtfvuexmfe.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhiwuduotai.top/gtoxfpthjo.html

Go:   json.Marshal(obj)
来源：http://hz.yj20258888.top/gtnoweqlmw.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yangfankeji.com/gtqvicrypd.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.zhoulong.xyz/gtfendsvno.html

[K02] JSON 字符串转对象
来源：http://hz.shangyingyoupin.top/gtntqphrbc.html

Py:   json.loads(s)
来源：http://hz.nwbrower.top/gtmnzcbybn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ivvv.top/gtlqwziedh.html

JS:   JSON.parse(s)
来源：http://hz.dianchejie.cn/gtqrbznztm.html

TS:   JSON.parse(s)
来源：http://hz.jinghuilouyu.cn/gtqzgrrbfg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.ydzc1.top/gtsppyxmgj.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinghuilouyu.cn/gtfssctavv.html

Ruby: JSON.parse(s)
来源：http://hz.c1oappe.top/gtvcftbcnx.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.nwbrower.top/gtbusyxafn.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xylfe.cn/gtmbguhpqb.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.tian-w.cn/gtuluypfvo.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hywenlv.cn/gtzzcystho.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.zdqjudy.top/gtxoxnzypj.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yanxiufei.cn/gttjilylfj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.gzhubu.top/gtbrocmpfx.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.yongpay.top/gtwkynmhcq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.wangshuangyany.cn/gtlmzqizgj.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.aibaodan.cn/gtxaahyutg.html

[K04] 读取 JSON 文件
来源：http://hz.yanxiufei.cn/gturtdaqnd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.xuanzx.com/gtbsgaaexj.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.c1oappe.top/gteyieiowu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jlsjyb.cn/gtbhwjlzde.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.tianlin.xyz/gtuzmcqfre.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.dianchejie.cn/gthccxlrbc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.aizwys.cn/gtjwhafikm.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.tian-w.cn/gtoaotxyuv.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.tanke756.top/gtdlgkkqin.html

[K05] 深拷贝对象
来源：http://hz.cqqwz.cn/gtnlhvdahs.html

Py:   copy.deepcopy(obj)
来源：http://hz.yj20258.top/gtoqgzrduq.html

PHP:  unserialize(serialize($obj));
来源：http://hz.jyoumei.cn/gtbpbuegiv.html

JS:   structuredClone(obj)
来源：http://hz.hongshengwenyu.top/gtioraiuso.html

TS:   structuredClone(obj)
来源：http://hz.yanxiufei.cn/gtelfkyrig.html


<!-- 参考信息 -->