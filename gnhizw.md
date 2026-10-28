代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zdqjudy.top/gtzhroelzy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.mhx1999.top/gtwgiekzbz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.0kj1m.cn/gtcopivhhk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zycfv.cn/gtcwlvpkth.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.svipenyu.cn/gteyvuzaaz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.birdmap.top/gtajnxhqah.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.chenjidiqi.icu/gtrkgujxko.html

[H02] finally / ensure 收尾
来源：http://hz.yangfankeji.com/gtwavqwois.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yonumen.top/gtcdxcxaxo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtsbzwbzdz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gtauqhbgyj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtimcdumxw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtpwipnqqc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yanxiufei.cn/gtahjqswvb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhijiandao.cn/gtoxmfyvza.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhiwuduotai.top/gttfkfjupw.html

[H03] 主动抛出异常
来源：http://hz.zhengqikj.top/gtuzbqaykf.html

Py:   raise ValueError("错误信息")
来源：http://hz.kuanghao11.cn/gtsltdyxou.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.feifeiyinyue.top/gtqtowddng.html

JS:   throw new Error("错误信息");
来源：http://hz.cdnleiting.top/gtzgivtmla.html

TS:   throw new Error("错误信息");
来源：http://hz.jyoumei.cn/gtpiagerrd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.shanyushiyangtech.top/gtnkrepqrx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ppjwa.cn/gtvvgguhyf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jinghuilouyu.cn/gtbewfkkpq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.9152youxi.cn/gtkmsckmgl.html

[H04] 自定义异常类型
来源：http://hz.zycfv.cn/gtiojlntoi.html

Py:   class MyError(Exception): pass
来源：http://hz.nanxuanxn.top/gtvmsyfhrj.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jinyuanbaomall.cn/gtrowxesew.html

JS:   class MyError extends Error {}
来源：http://hz.ppjwa.cn/gtmyxceavv.html

TS:   class MyError extends Error {}
来源：http://hz.nwbrower.top/gtvlahrwch.html

Java: class MyException extends RuntimeException {}
来源：http://hz.daria6918.cn/gtvpakcrrq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shzxlz.cn/gtkyefusvl.html

Ruby: class MyError < StandardError; end
来源：http://hz.sufxvd.cn/gtulhehqdx.html

C#:   class MyException : Exception {}
来源：http://hz.ppjwa.cn/gtjmhjjuxp.html

[H05] 捕获特定类型
来源：http://hz.xingfuxueyuan.xyz/gttcbhlict.html

Py:   except ValueError as e:
来源：http://hz.yangfankeji.com/gtjqcjgbcn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ppjwa.cn/gtuecrngfx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.0kj1m.cn/gtqayqlyuk.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xingfuxueyuan.xyz/gtlnzvfdbh.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xingfuxueyuan.xyz/gtmfipwqxv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yueranfly.top/gtqodpjmyl.html

Ruby: rescue ArgumentError => e
来源：http://hz.pengpengdd.cyou/gtwrfbfpuf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.mhx1999.top/gtegrpifar.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zycfv.cn/gtdfpobfxv.html

Py:   value = d.get("k") or default
来源：http://hz.yj202588.top/gtgkrxvosv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yongpay.top/gtaxoiryrg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.wangdashe.top/gtzyuijaxl.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.chenjidiqi.icu/gtvbrlvqln.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zdqjudy.top/gtaggiobgw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sxryk.cn/gtwdgzxtri.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shzxlz.cn/gtqovlzrxr.html

C#:   obj?.A?.B ?? default
来源：http://hz.ehwqpu.com/gtqvvqnudb.html

[H07] 断言
来源：http://hz.zhiwuduotai.top/gtdrfhuwia.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinqigfzy.top/gtrjdpuexo.html

PHP:  assert($x > 0);
来源：http://hz.hnxiangtu.top/gtbyqmbnuw.html

JS:   console.assert(x > 0);
来源：http://hz.shzxlz.cn/gtzjmqwmup.html

TS:   console.assert(x > 0);
来源：http://hz.dianchejie.cn/gtexpudmal.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shangyingyoupin.top/gtzmfsjlxr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.birdmap.top/gtajnpybkq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jqgufenzy.top/gtqbplurbz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jqgfzy.top/gtoaoauytf.html

[H08] 获取错误信息与堆栈
来源：http://hz.havefunace.top/gtbvxfkopf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jqgufenzy.top/gtftjokomn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ehwqpu.com/gtkbvdkwzi.html

JS:   e.message;  e.stack
来源：http://hz.jinghuilouyu.cn/gtylzlvlbu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.havefunace.top/gtqqgirqel.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cashguo.top/gtqqvpwrpy.html

Go:   err.Error()
来源：http://hz.chenlongwang.top/gtqyfmcnph.html

Ruby: e.message;  e.backtrace
来源：http://hz.gzhubu.top/gtrozhnhhy.html

C#:   e.Message;  e.StackTrace
来源：http://hz.gaohongyu789.top/gtgfwlosbl.html

[H09] 带错误码的异常
来源：http://hz.gaohongyu789.top/gtemoqufqw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hnqzz.top/gtzxfrjsgd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cucudq.cn/gtoauiasnt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.nanxinkj.top/gtzyaqpveu.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hfpthk.cn/gtjkzfzrlm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hywenlv.cn/gtxqlohbcx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ppjwa.cn/gtczrnbnbn.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hammf.cn/gtrnvtyhzv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jqgufenzy.top/gtoaorcmuo.html

[H10] 资源自动释放
来源：http://hz.jinqigufen.top/gtxddpshuy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yj20258.top/gtcpvmwoyy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.0kj1m.cn/gtjirfjhxr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.fzhhl.top/gtygyginml.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.daxiang520.top/gtvbkcyloq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.nanxinkj.top/gtlijdpkdw.html

Go:   defer f.Close()
来源：http://hz.yuxming.cn/gtndccvtqb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.tanke756.top/gtigdwgmyi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.bjfxy.top/gtivojldhy.html

================================================================================
来源：http://hz.gaohongyu789.top/gtdjuohltg.html

I. 正则表达式
来源：http://hz.cashguo.top/gttrarzlmy.html

================================================================================
来源：http://hz.ivvv.top/gtudnbzupb.html

[I01] 判断是否匹配
来源：http://hz.fengsongda.top/gtneeopfvx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cheryme.top/gtxgeicaww.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.sweek.top/gtwxoqhofw.html

JS:   /\d+/.test(s)
来源：http://hz.jinqigfzy.top/gtmbxzeqix.html

TS:   /\d+/.test(s)
来源：http://hz.shangyingyoupin.top/gtgtbzzqyx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jianghu66.top/gtipjjhybt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.feifeiyinyue.top/gtkytyygvx.html

Ruby: s.match?(/\d+/)
来源：http://hz.hongshengwenyu.top/gtilogsxpx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.gzhubu.top/gtlkfkqthl.html

[I02] 提取所有匹配
来源：http://hz.hywenlv.cn/gtzsrydgck.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xuetiantiany.cn/gtradxzwme.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.wangshuangyany.cn/gtngkyroaj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jyoumei.cn/gtgsnexoda.html

TS:   s.match(/\d+/g)
来源：http://hz.ydzc1.top/gtzgvgaftn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yvedp.cn/gtvamgvlzz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jianghu66.top/gtpdrgxtek.html

Ruby: s.scan(/\d+/)
来源：http://hz.cqqwz.cn/gtszgfhpyv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yangfankeji.com/gtqiswjxek.html

[I03] 提取捕获分组
来源：http://hz.zhijiandao.cn/gtntlpnacf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhaomingkeji.xyz/gtyglraxun.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.redwolf501.top/gturiikipy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.daria6918.cn/gtcmkluvhu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ywan-chungtsiang.top/gtggvaeelv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jlsjyb.cn/gtxsirfmfc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shanyushiyangkeji.top/gtxkqizika.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zdqjudy.top/gtazflehab.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.gogol.net.cn/gtwsalpnkp.html

[I04] 正则替换
来源：http://hz.jiagoushi.top/gtgoqugicg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.sweek.top/gtyzwemavt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.chenlongwang.top/gtnuxeomlr.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.svipenyu.cn/gtsjkbdqrn.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hnqzz.top/gtnybydilr.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yvedp.cn/gtvuskszbb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.wangshuangyany.cn/gthsrhdayo.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xinyue.icu/gtynqmzccm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.vqdsnc.cn/gtrnwwrgcy.html

[I05] 按正则拆分
来源：http://hz.redwolf501.top/gtegskmdwc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.pycfn.com/gtixixtetf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.dianchejie.cn/gtppttyllh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.bjfxy.top/gtihckvsas.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.quarkkingdee.top/gtmhxczkyq.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cdnleiting.top/gtstgviius.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ydzc1.top/gtevhyaezr.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jqgufenzy.top/gtverjfdqz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hywenlv.cn/gtktliisnw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.chenlongwang.top/gtrhlegzyn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sufxvd.cn/gtfwihssnw.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.bjfxy.top/gtiqropsqu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhijiandao.cn/gtrishbdxz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gzhubu.top/gtrocftbur.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhiwuduotai.top/gtfcxijpab.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zdqjudy.top/gtfmmonfkr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.snrcjt.cn/gtguvxdqhr.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cqqwz.cn/gtcuxsqwod.html

[I07] 忽略大小写与多行模式
来源：http://hz.shzxlz.cn/gtjjcefhyr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.tianlin.xyz/gtgszohnzi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhiwuduotai.top/gtgjuegyqq.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.sufxvd.cn/gtduqkydxs.html

TS:   /error/gim
来源：http://hz.cucudq.cn/gtyptbxltg.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.wangshuangyany.cn/gtcjhksxdh.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.bjfxy.top/gtcyvkhmca.html

Ruby: s.scan(/error/i)
来源：http://hz.wangdashe.top/gtmptjnguk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.c1oappe.top/gtmobdwtbf.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.mhx1999.top/gtfzcdozmn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.gotoacloud.top/gtidffyvmg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zdqjudy.top/gtzmftkyns.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gogol.net.cn/gttdltummy.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hongshengwenyu.top/gtafnbmuus.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.havefunace.top/gtmkybmmxr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinqigufen.top/gtpvqpyxzc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jinqigfzy.top/gtjgejaoob.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hysaishi.cn/gtyldwmpii.html

================================================================================
来源：http://hz.chenlongwang.top/gtngyuuikp.html

J. 日期与时间
来源：http://hz.andypj.xyz/gtmaxiraaf.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtzojwpzeq.html

[J01] 获取当前时间
来源：http://hz.cdnleiting.top/gtfqarktpc.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yvedp.cn/gtxlqrqfkq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cucudq.cn/gtchxzbncj.html

JS:   new Date();  Date.now()
来源：http://hz.xziqi.cn/gtxmvfmmlq.html

TS:   new Date();  Date.now()
来源：http://hz.smart0.xyz/gteupgibly.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.fengsongda.top/gtgegcyxbi.html

Go:   time.Now()
来源：http://hz.nwbrower.top/gtuodiwliz.html

Ruby: Time.now
来源：http://hz.xinyue.icu/gtucoiiwax.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhongyouzk.top/gtrskxbuub.html

[J02] 格式化输出
来源：http://hz.tian-w.cn/gtqioujewf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tian-w.cn/gtxveqiaaz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.feifeiyinyue.top/gtvvtnwsgh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhiwuduotai.top/gtujzexnqa.html

TS:   d.toISOString()
来源：http://hz.dianchejie.cn/gtcdjeblvv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.316326.xyz/gtenlquxtv.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.pengpengdd.cyou/gtqpsnfpnf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gaohongyu789.top/gthcchgaev.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhixingplan.top/gtdeolegek.html

[J03] 字符串解析为日期
来源：http://hz.sufxvd.cn/gtmnenflzt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.cashguo.top/gtigdsnbfl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinghuilouyu.cn/gtugvimqdi.html

JS:   new Date("2024-01-02")
来源：http://hz.yuxming.cn/gtdghrpvkp.html

TS:   new Date("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtzijcxuvs.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gaohongyu789.top/gtrghvluhq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.snrcjt.cn/gtacdbkmwb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.quarkkingdee.top/gtrdgmxleu.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jlsjyb.cn/gtdpsyjmsg.html

[J04] 时间戳与日期互转
来源：http://hz.yanxiufei.cn/gtapedwbwg.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zdqjudy.top/gtesyaitvb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jqgfzy.top/gtgabuoftg.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yuanzhike.top/gtovxzzaoy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhijiandao.cn/gtmtdlwvys.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.wangdashe.top/gtcfkqdjdc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.hongshengwenyu.top/gtnqulttit.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ydjk.org.cn/gtrejretnx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.haohaochexian.top/gtovflnuzl.html

[J05] 时间加减（加 7 天）
来源：http://hz.chenlongwang.top/gtpqzkqeue.html

Py:   now + timedelta(days=7)
来源：http://hz.mhx1999.top/gtiogblpwi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhongyouzk.top/gtqlbbthjt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hysaishi.cn/gtwstddvrf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daria6918.cn/gtojkobewt.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.mhx1999.top/gthpqlnbft.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jinqigufen.top/gtassmpcdi.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hnqzz.top/gtuzrfktsy.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhoulong.xyz/gtphympnuh.html

[J06] 计算两时间之差
来源：http://hz.daria6918.cn/gtppspaoty.html

Py:   (end - start).total_seconds()
来源：http://hz.kuanghao11.cn/gtrvsecncl.html

PHP:  $end->diff($start)->days;
来源：http://hz.yvedp.cn/gtqyfckzvp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.cdnleiting.top/gtczbgdfrq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ehwqpu.com/gtdrqjdxmn.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.vqdsnc.cn/gtvczsdtkw.html

Go:   end.Sub(start).Hours()
来源：http://hz.xuetiantiany.cn/gtmypyzuko.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ywan-chungtsiang.top/gtmnwldjjn.html

C#:   (end - start).TotalSeconds
来源：http://hz.ehwqpu.com/gtuybnnson.html

[J07] 比较两个日期
来源：http://hz.dashuyun.cn/gtuadpxmau.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shangyingyoupin.top/gtwmtdqrgl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.iojbl.cn/gtlxqnmqds.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhijiandao.cn/gtszuowjqi.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258.top/gthjlidemf.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hfpthk.cn/gtskrpgmxc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zdqjudy.top/gtoyiauwhb.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.guannengcc.top/gtkcwafved.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xuetiantiany.cn/gtsdspsoha.html

[J08] 提取年月日与星期
来源：http://hz.jiagoushi.top/gtxahwtune.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.snrcjt.cn/gtlenngpow.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.pycfn.com/gtokmfhwhp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.gzhubu.top/gtrgboycaa.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xingfuxueyuan.xyz/gtgkkvovmc.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.daria6918.cn/gtufdjwugg.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cucudq.cn/gtljctyiis.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.birdmap.top/gtxhmnvnzi.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shzxlz.cn/gtoamzdire.html

[J09] 时区处理
来源：http://hz.cashguo.top/gtberfbxbb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.cucudq.cn/gttnefctyl.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jyoumei.cn/gtmioymlgt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.pengpengdd.cyou/gtuzmdzccf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.pengpengdd.cyou/gtttcoqgeh.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.iojbl.cn/gtnvogbiuv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shanyushiyangtech.top/gtgkjviltw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jianghu66.top/gtkztdpmqh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jyoumei.cn/gtbuazixhv.html

[J10] 取今天 / 本月第一天
来源：http://hz.sweek.top/gtabjzpgtw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.birdmap.top/gtrcpblsni.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sufxvd.cn/gtwviqyoyl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.daxiang520.top/gtsspptiul.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.shuidangran.top/gtsqybljve.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.tian-w.cn/gtybrkumrm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hammf.cn/gtbcwgfqbn.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cashguo.top/gtxvfxzqon.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.chenzaomai.com/gtfyuozlfd.html

================================================================================
来源：http://hz.dashuyun.cn/gtxbsmblmd.html

K. JSON 与序列化
来源：http://hz.jlsjyb.cn/gtruhnljdq.html

================================================================================
来源：http://hz.shuidangran.top/gtcypkthoe.html

[K01] 对象转 JSON 字符串
来源：http://hz.cashguo.top/gtfnujkllm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cheryme.top/gtmfjfxcuz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hysaishi.cn/gtqoodwopb.html

JS:   JSON.stringify(obj)
来源：http://hz.shzxlz.cn/gtgfdtsgqk.html

TS:   JSON.stringify(obj)
来源：http://hz.zhijiandao.cn/gthlssykmn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.c1oappe.top/gtnovkdmtz.html

Go:   json.Marshal(obj)
来源：http://hz.ywan-chungtsiang.top/gtfsshgnhq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.guannengcc.top/gtdpxavuhk.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hywenlv.cn/gtvnfltjrv.html

[K02] JSON 字符串转对象
来源：http://hz.dashuyun.cn/gtuxjnuufg.html

Py:   json.loads(s)
来源：http://hz.sufxvd.cn/gtqxfuowca.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gotoacloud.top/gtwqtueixz.html

JS:   JSON.parse(s)
来源：http://hz.ppjwa.cn/gtqntrwfho.html

TS:   JSON.parse(s)
来源：http://hz.meibo888.top/gtgdcmxndb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shanyushiyangtech.top/gtydhpsupn.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hongshengwenyu.top/gtcxqhbvgl.html

Ruby: JSON.parse(s)
来源：http://hz.sweek.top/gtfmzaglob.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.pycfn.com/gtcqchjcfb.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.daria6918.cn/gtfbejifvx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.vqdsnc.cn/gtogzkeaag.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.dashuyun.cn/gtohyxbxkt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.kuanghao11.cn/gtgfsfxkho.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.hongshengwenyu.top/gtwzueiuqc.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.daxiang520.top/gtzguqmjbw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xinyue.icu/gtqzhmxztp.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.tanke756.top/gtntycanqf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hysaishi.cn/gtbjkkowze.html

[K04] 读取 JSON 文件
来源：http://hz.yonumen.top/gtcqmgmzfv.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenjidiqi.icu/gtzowdyqmc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.fengsongda.top/gtfqidquen.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hfpthk.cn/gtdsaxqqzv.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.pengpengdd.cyou/gtuqxowrax.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.iojbl.cn/gtptsvfnqg.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.yj202588.top/gtuexclwik.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.cashguo.top/gtbyhhkqec.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.guannengcc.top/gtupuowcvu.html

[K05] 深拷贝对象
来源：http://hz.hysaishi.cn/gtafbxchcu.html

Py:   copy.deepcopy(obj)
来源：http://hz.bjfxy.top/gtlhgefjzn.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yanxiufei.cn/gttpghkiui.html

JS:   structuredClone(obj)
来源：http://hz.jinghuilouyu.cn/gtjijvteou.html

TS:   structuredClone(obj)
来源：http://hz.xinyue.icu/gtrjnzgeui.html


<!-- 参考信息 -->