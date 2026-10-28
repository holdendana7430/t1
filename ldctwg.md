代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://hz.kuanghao11.cn/gtlctdwfqy.html

C#:   class MyException : Exception {}
来源：http://hz.jinqigufen.top/gtvjcaappg.html

[H05] 捕获特定类型
来源：http://hz.daria6918.cn/gtpkymnajl.html

Py:   except ValueError as e:
来源：http://hz.jinqigufen.top/gttyfygqfr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ppjwa.cn/gtgigindrz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xinyue.icu/gtimmghiqz.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gzhubu.top/gtxevrnasr.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jinyuanbaomall.cn/gtcnnoaybz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.guannengcc.top/gtfulkvyhv.html

Ruby: rescue ArgumentError => e
来源：http://hz.cashguo.top/gtmlaniwsu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.quarkkingdee.top/gtlzwmbsbf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nanxuanxn.top/gtxbrilvls.html

Py:   value = d.get("k") or default
来源：http://hz.meibo888.top/gtmzbmwata.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.svipenyu.cn/gtqsrdunze.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gaohongyu789.top/gtiktvojcw.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.haohaochexian.top/gtwkfooxjv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yueranfly.top/gtldpaizif.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.dashuyun.cn/gtlkmyrvgf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.fzhhl.top/gtgdesdulq.html

C#:   obj?.A?.B ?? default
来源：http://hz.cucudq.cn/gtismxmlso.html

[H07] 断言
来源：http://hz.gaohongyu789.top/gteklnmzhl.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hysaishi.cn/gtwecfbmkv.html

PHP:  assert($x > 0);
来源：http://hz.svipenyu.cn/gtsggrjpjc.html

JS:   console.assert(x > 0);
来源：http://hz.quarkkingdee.top/gtyhjbjmud.html

TS:   console.assert(x > 0);
来源：http://hz.mhx1999.top/gtdslyyrbt.html

Java: assert x > 0 : "必须为正";
来源：http://hz.smart0.xyz/gtlckzumbe.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhaomingkeji.xyz/gtbixxyggh.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.fzhhl.top/gtwoigeqjg.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yonumen.top/gtovunrozj.html

[H08] 获取错误信息与堆栈
来源：http://hz.c1oappe.top/gtzywmxmae.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.xuetiantiany.cn/gtfultekyi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gzhubu.top/gthfcpofsp.html

JS:   e.message;  e.stack
来源：http://hz.gogol.net.cn/gtueiamivi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xylfe.cn/gtcpkrwmds.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yangfankeji.com/gthmmidemh.html

Go:   err.Error()
来源：http://hz.gotoacloud.top/gtrvoepeus.html

Ruby: e.message;  e.backtrace
来源：http://hz.hongshengwenyu.top/gtplzitqmq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jiagoushi.top/gtypekdqag.html

[H09] 带错误码的异常
来源：http://hz.yuanzhike.top/gtieykuczy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.ydjk.org.cn/gtwixfdrda.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.chenlongwang.top/gtwadcdomn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.9152youxi.cn/gtempcduul.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cucudq.cn/gtjvzymfrl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.chenjidiqi.icu/gtpvvaxqra.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yanxiufei.cn/gttwxumwze.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yanxiufei.cn/gtrznczaek.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.tanke756.top/gtvrpfjque.html

[H10] 资源自动释放
来源：http://hz.smart0.xyz/gtsphmetlp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hnxiangtu.top/gtfwqvdcks.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shangyingyoupin.top/gtvwtgsjio.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cheryme.top/gtkoqzejsz.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhixingplan.top/gtsjlykzbg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yangfankeji.com/gtgtuafhfs.html

Go:   defer f.Close()
来源：http://hz.zhengqikj.top/gtcjlnqxpi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jqgfzy.top/gtirsrjpjo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtphlihanj.html

================================================================================
来源：http://hz.yueranfly.top/gtibgmfsqe.html

I. 正则表达式
来源：http://hz.9152youxi.cn/gtrfmnvlvg.html

================================================================================
来源：http://hz.cqqwz.cn/gtxzbphzwq.html

[I01] 判断是否匹配
来源：http://hz.yongpay.top/gtejcgogkw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hywenlv.cn/gtyzstfatj.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.andypj.xyz/gtavcpuugc.html

JS:   /\d+/.test(s)
来源：http://hz.hammf.cn/gtpjsdaxrj.html

TS:   /\d+/.test(s)
来源：http://hz.9152youxi.cn/gtysgwwqwv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.wangdashe.top/gtettquxuy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xuetiantiany.cn/gtxiwcmpfo.html

Ruby: s.match?(/\d+/)
来源：http://hz.birdmap.top/gtvyvwisvp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.gogol.net.cn/gtxlfkwlmr.html

[I02] 提取所有匹配
来源：http://hz.0kj1m.cn/gtmwwtibre.html

Py:   re.findall(r"\d+", s)
来源：http://hz.sxryk.cn/gtclqymghg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.smart0.xyz/gtpglahcgq.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.xuanzx.com/gthiyjggni.html

TS:   s.match(/\d+/g)
来源：http://hz.xinyue.icu/gtfdfddykj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.kuanghao11.cn/gtkhwnimdp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.fzhhl.top/gtaukinovq.html

Ruby: s.scan(/\d+/)
来源：http://hz.52xcode.cn/gtlcbvvjdn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yanxiufei.cn/gtnzdvertq.html

[I03] 提取捕获分组
来源：http://hz.yueranfly.top/gtiblwigph.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhoulong.xyz/gtxilrczyg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.nanxinkj.top/gtewbifugg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yuxming.cn/gtqpgluqma.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hnxiangtu.top/gtuydzufih.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.tanke756.top/gtmerjjlqu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.feifeiyinyue.top/gtmlzgmneg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hnxiangtu.top/gtjwoqgnra.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.birdmap.top/gtgbbpmigb.html

[I04] 正则替换
来源：http://hz.haohaochexian.top/gtkjlnrnfp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.fengsongda.top/gtosowzgoh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.pycfn.com/gtscptulbo.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.haohaochexian.top/gtwyrygibl.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.cucudq.cn/gtvjrvqzlt.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yj20258888.top/gtvmtaxgep.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shangyingyoupin.top/gtobfmimwg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zycfv.cn/gtlvqmkcnm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sufxvd.cn/gttuhbguht.html

[I05] 按正则拆分
来源：http://hz.sufxvd.cn/gtvthjbslx.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xziqi.cn/gtwqdlztlq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.birdmap.top/gtyjdwqtno.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gtvngqdezw.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gtdedqxomu.html

Java: s.split("\\s*,\\s*")
来源：http://hz.gogol.net.cn/gtnpbidvat.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ehwqpu.com/gtobztnlyt.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.52xcode.cn/gtvvfeocez.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hfpthk.cn/gtqcmbaiuo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xylfe.cn/gtgjacqybr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.andypj.xyz/gtbypfmqpf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hywenlv.cn/gtsgxhklmt.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgufenzy.top/gtxllntxvi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shuidangran.top/gtqbnvipff.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hnxiangtu.top/gtcytbkyex.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.snrcjt.cn/gtvqdbkpzi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.chenlongwang.top/gtbmdvymlo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ybcxt.top/gtskhxufvx.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinqigfzy.top/gtapcinqll.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.vqdsnc.cn/gtsjciwboi.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.sweek.top/gtgrysznrc.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zycfv.cn/gtmamzxkjg.html

TS:   /error/gim
来源：http://hz.dashuyun.cn/gtmgxumatp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yonumen.top/gteztspdun.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cashguo.top/gtegppuhju.html

Ruby: s.scan(/error/i)
来源：http://hz.wangdashe.top/gtezbrmmow.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ivvv.top/gtbszafuak.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.vqdsnc.cn/gtanuknjag.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yuxming.cn/gtruovdjhd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hfpthk.cn/gtbdtchkql.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shuidangran.top/gtebtzfwqg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.kuanghao11.cn/gtqyrhwdit.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.pycfn.com/gtrgrbiluq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.guowangkeji.top/gtwirrhzrd.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cdnleiting.top/gtdfhlwoku.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.kuanghao11.cn/gtzrvsrtml.html

================================================================================
来源：http://hz.fengsongda.top/gtqftoholl.html

J. 日期与时间
来源：http://hz.nwbrower.top/gtxnuhmwqy.html

================================================================================
来源：http://hz.yj202588.top/gtcsagzqjo.html

[J01] 获取当前时间
来源：http://hz.shanyushiyangtech.top/gtgkghharr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.gogol.net.cn/gttxyiliok.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xinyue.icu/gtiapkncab.html

JS:   new Date();  Date.now()
来源：http://hz.0kj1m.cn/gthqbkuoiw.html

TS:   new Date();  Date.now()
来源：http://hz.yvedp.cn/gtplmpeawi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shanyushiyangkeji.top/gtggvxqejm.html

Go:   time.Now()
来源：http://hz.cucudq.cn/gtjgmkfhbt.html

Ruby: Time.now
来源：http://hz.yonumen.top/gtkrtqqhgz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.redwolf501.top/gtgxjqstjf.html

[J02] 格式化输出
来源：http://hz.nwbrower.top/gtyezkolep.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ivvv.top/gtpspjyiqz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yvedp.cn/gtrxxjecxd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sxryk.cn/gtjinicofw.html

TS:   d.toISOString()
来源：http://hz.vqdsnc.cn/gtxvjaakyr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.nanxinkj.top/gtwfmijkwy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xylfe.cn/gtdbgklolv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydjk.org.cn/gtxfyuesfm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gogol.net.cn/gtnrxndxjd.html

[J03] 字符串解析为日期
来源：http://hz.svipenyu.cn/gtgnbjsbfo.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shuidangran.top/gthffvkofp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.52xcode.cn/gtbzchywlz.html

JS:   new Date("2024-01-02")
来源：http://hz.sysykeji.top/gtlkcymvnm.html

TS:   new Date("2024-01-02")
来源：http://hz.zhongyouzk.top/gtglrloyot.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gogol.net.cn/gtfefsvzld.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shzxlz.cn/gthvpliidl.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gotoacloud.top/gtiwwpdqjx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yuxming.cn/gtgbmyeegs.html

[J04] 时间戳与日期互转
来源：http://hz.yuxming.cn/gtcvgjyvoy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.dashuyun.cn/gtkumdxplf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jqgfzy.top/gtxykpxuan.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shangyingyoupin.top/gtvjmmlvys.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.smart0.xyz/gtdncajizi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.smart0.xyz/gtgbolrbrk.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.pengpengdd.cyou/gtuaqrtwhl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shanyushiyangtech.top/gtadjngqlo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.tian-w.cn/gtmaefdsfk.html

[J05] 时间加减（加 7 天）
来源：http://hz.smart0.xyz/gtvpewcwsx.html

Py:   now + timedelta(days=7)
来源：http://hz.aizwys.cn/gtkcduvvem.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.bjfxy.top/gtsxoicdhq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ivvv.top/gtaatxmokk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yuxming.cn/gtkpvmrttk.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.kuanghao11.cn/gtdsmdmknz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cashguo.top/gtnxhyrpnu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cqqwz.cn/gtumxkwnxi.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xylfe.cn/gtodyjmdrt.html

[J06] 计算两时间之差
来源：http://hz.xinyue.icu/gtvnjmfung.html

Py:   (end - start).total_seconds()
来源：http://hz.meibo888.top/gtxktqrofv.html

PHP:  $end->diff($start)->days;
来源：http://hz.guowangkeji.top/gtrjtkwdum.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.9152youxi.cn/gtmoconnnv.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ydjk.org.cn/gtzkshyjio.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ppjwa.cn/gtfeomupnf.html

Go:   end.Sub(start).Hours()
来源：http://hz.mhx1999.top/gtlvfmutgz.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jinqigfzy.top/gtrkmricma.html

C#:   (end - start).TotalSeconds
来源：http://hz.jqgfzy.top/gtrgfopvph.html

[J07] 比较两个日期
来源：http://hz.gogol.net.cn/gttziqvnam.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yj202588.top/gtnwzdtryy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.0kj1m.cn/gtxsyeoylx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yongpay.top/gtzicxxpyd.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj202588.top/gturldmnpn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xuanzx.com/gtrgbunxgh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.316326.xyz/gthefzonye.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.aibaodan.cn/gtoaahwxpn.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cashguo.top/gterrrdvve.html

[J08] 提取年月日与星期
来源：http://hz.shangyingyoupin.top/gtpcohdlbu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.haohaochexian.top/gttgznxjpi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhongyouzk.top/gtvhhtdlxy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.pycfn.com/gtsdgbyymo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.haohaochexian.top/gtpxltrfic.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.guannengcc.top/gtesqnfwmh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.ppjwa.cn/gtzepiujyn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cucudq.cn/gttpqmiavy.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhoulong.xyz/gtuxrujzrw.html

[J09] 时区处理
来源：http://hz.yuxming.cn/gttuvjkori.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hfpthk.cn/gtccchwjto.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhongyouzk.top/gtausgdoxl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258.top/gtfhdwtkdj.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tanke756.top/gtgmcuttjt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.chenjidiqi.icu/gtlswsmovj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jyoumei.cn/gtoxtybepo.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.andypj.xyz/gtgjcpcbky.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zdqjudy.top/gtzqknzumu.html

[J10] 取今天 / 本月第一天
来源：http://hz.zdqjudy.top/gtlgwibbee.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.svipenyu.cn/gtowlriftb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ivvv.top/gtqrrpucww.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.wangshuangyany.cn/gtexxckyuu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhiwuduotai.top/gtmkbearsl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.redwolf501.top/gtndamxubv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.shanyushiyangkeji.top/gtcmzgozaq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xingfuxueyuan.xyz/gtgiceshnf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ywan-chungtsiang.top/gtddqmoyku.html

================================================================================
来源：http://hz.hnqzz.top/gtjmcircjt.html

K. JSON 与序列化
来源：http://hz.zycfv.cn/gtuyunljra.html

================================================================================
来源：http://hz.jlsjyb.cn/gtkaqpxxod.html

[K01] 对象转 JSON 字符串
来源：http://hz.cqqwz.cn/gtzpxexlrm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yj202588.top/gtwycoeypd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xuetiantiany.cn/gthlzhvgpb.html

JS:   JSON.stringify(obj)
来源：http://hz.feifeiyinyue.top/gtxvqwpkrz.html

TS:   JSON.stringify(obj)
来源：http://hz.hnxiangtu.top/gtsjllanol.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.iojbl.cn/gtouybhrpt.html

Go:   json.Marshal(obj)
来源：http://hz.vqdsnc.cn/gttooloytr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cdnleiting.top/gttauxsmbt.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.nanxinkj.top/gtagqufcia.html

[K02] JSON 字符串转对象
来源：http://hz.xinyue.icu/gtgmephtfr.html

Py:   json.loads(s)
来源：http://hz.c1oappe.top/gtuinlgeit.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.daxiang520.top/gtdfknyray.html

JS:   JSON.parse(s)
来源：http://hz.xziqi.cn/gttdevebvl.html

TS:   JSON.parse(s)
来源：http://hz.cucudq.cn/gtpxxkqwei.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.quarkkingdee.top/gtzdaitoyq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.feifeiyinyue.top/gtbxiigvyy.html

Ruby: JSON.parse(s)
来源：http://hz.shangyingyoupin.top/gtazpqjeoe.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.nwbrower.top/gtphkxuvbr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hywenlv.cn/gtigkvfrow.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jinghuilouyu.cn/gtdfouzqei.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yuxming.cn/gttlaniivx.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258.top/gtndsghgbe.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.dianchejie.cn/gtasfewiwg.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.daxiang520.top/gtrfwenkdb.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.cdnleiting.top/gtpltngnws.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.snrcjt.cn/gtavygrclp.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.svipenyu.cn/gtphllvwpe.html

[K04] 读取 JSON 文件
来源：http://hz.bjfxy.top/gtvyphuvcz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.havefunace.top/gtzzsadfzb.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shanyushiyangtech.top/gtozeubajl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhoulong.xyz/gtfjfzqpjf.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ywan-chungtsiang.top/gtmfxlevda.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhixingplan.top/gtfgwpnggk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.gzhubu.top/gtkhydxryr.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.zdqjudy.top/gtowyalpiz.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zhaomingkeji.xyz/gtdqjetzrn.html

[K05] 深拷贝对象
来源：http://hz.jqgfzy.top/gtatnykqhb.html

Py:   copy.deepcopy(obj)
来源：http://hz.andypj.xyz/gttzlexxia.html

PHP:  unserialize(serialize($obj));
来源：http://hz.hfpthk.cn/gtubknijcm.html

JS:   structuredClone(obj)
来源：http://hz.svipenyu.cn/gtyrumujqf.html

TS:   structuredClone(obj)
来源：http://hz.aibaodan.cn/gtsyyapqrk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.shanyushiyangkeji.top/gtwgmusbab.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.dashuyun.cn/gtcadixxof.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.gotoacloud.top/gtkgypbagy.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.cashguo.top/gttrdxzelg.html

[K06] 解析 URL 查询串
来源：http://hz.jinghuilouyu.cn/gtqoqiiwtq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.yuanzhike.top/gthjxyptvu.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.c1oappe.top/gthqucegau.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yonumen.top/gtgktlolim.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhaomingkeji.xyz/gtehpvpzog.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.jyoumei.cn/gtbglczzua.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xuanzx.com/gtkkatjgce.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.aizwys.cn/gtjqbfunls.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.bjfxy.top/gtznyrvloe.html

[K07] 进制转换
来源：http://hz.zhijiandao.cn/gtwuwsejvq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.hysaishi.cn/gthxxkjgaa.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.316326.xyz/gtlhyffels.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.yj202588.top/gtnaoxtoqv.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.gzhubu.top/gtvckmgmdw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.shanyushiyangtech.top/gtklsopfdq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.0kj1m.cn/gtmucbvfhq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.chenlongwang.top/gtqyeczmrm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.xingfuxueyuan.xyz/gtiiwkxegc.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.hfpthk.cn/gtvpibkqob.html

Py:   pickle.dumps(obj)
来源：http://hz.shuidangran.top/gtaanrpdkl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.zdqjudy.top/gtmhydkntk.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.jlsjyb.cn/gtwpnzyeda.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.yanxiufei.cn/gtpgphdjqt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.yonumen.top/gtakrjqqtq.html

Go:   encoding/gob
来源：http://hz.quarkkingdee.top/gtbquvztlx.html

Ruby: Marshal.dump(obj)
来源：http://hz.ivvv.top/gtvdalflzc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.cheryme.top/gtsthzgrex.html

================================================================================
来源：http://hz.cucudq.cn/gtpqkcmsgy.html


<!-- 参考信息 -->