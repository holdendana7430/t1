代发 wailian999

Ruby: class MyError < StandardError; end
来源：http://hz.shuidangran.top/gtthqvgxhs.html

C#:   class MyException : Exception {}
来源：http://hz.jiagoushi.top/gtrotvzpum.html

[H05] 捕获特定类型
来源：http://hz.dashuyun.cn/gtftwlrohu.html

Py:   except ValueError as e:
来源：http://hz.ybcxt.top/gtoksjkwtz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yj20258888.top/gthuqxbvcl.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ehwqpu.com/gthhruxjis.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.chenlongwang.top/gtiuabpmep.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhijiandao.cn/gtfqglrteg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yj20258.top/gtsoxxblme.html

Ruby: rescue ArgumentError => e
来源：http://hz.vqdsnc.cn/gtwdnyodid.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhixingplan.top/gtnvzfdjgc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jianghu66.top/gtwquyahlf.html

Py:   value = d.get("k") or default
来源：http://hz.ydzc1.top/gtgbzncxrl.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhengqikj.top/gtoeghgjlf.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.c1oappe.top/gtzlkuzphi.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ehwqpu.com/gtfdyhyoih.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.chenjidiqi.icu/gtuouwgvcx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yvedp.cn/gtdzeqkoqd.html

Ruby: d&.dig(:a, :b)
来源：http://hz.nanxinkj.top/gtwzcvluaq.html

C#:   obj?.A?.B ?? default
来源：http://hz.jyoumei.cn/gtinhpjjtp.html

[H07] 断言
来源：http://hz.316326.xyz/gtyrbwvvza.html

Py:   assert x > 0, "必须为正"
来源：http://hz.iojbl.cn/gtrcxggucd.html

PHP:  assert($x > 0);
来源：http://hz.yvedp.cn/gtfpumqiuk.html

JS:   console.assert(x > 0);
来源：http://hz.zhiwuduotai.top/gtjhgiqrtb.html

TS:   console.assert(x > 0);
来源：http://hz.yongpay.top/gtyxwcpwgc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.dianchejie.cn/gtatjowcpn.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hfpthk.cn/gtrtgfbqwe.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sweek.top/gtgvyyfmas.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xuanzx.com/gtjtnyrtgf.html

[H08] 获取错误信息与堆栈
来源：http://hz.pycfn.com/gtyuvabwua.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.tanke756.top/gtidlvliox.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.0kj1m.cn/gtxrvibqaf.html

JS:   e.message;  e.stack
来源：http://hz.yj202588.top/gtwyflmgzq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhijiandao.cn/gtvqagkntr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.0kj1m.cn/gtlfaeqrnl.html

Go:   err.Error()
来源：http://hz.nanxinkj.top/gtnwlsxtdj.html

Ruby: e.message;  e.backtrace
来源：http://hz.tian-w.cn/gtbgxzshtp.html

C#:   e.Message;  e.StackTrace
来源：http://hz.guowangkeji.top/gtjzdrayvi.html

[H09] 带错误码的异常
来源：http://hz.meibo888.top/gtccufavsg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zhixingplan.top/gtksuajsvw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.tian-w.cn/gtsaetmecz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.wangshuangyany.cn/gtnvxqdbvz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.52xcode.cn/gtqrfnxogp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhoulong.xyz/gtkqalderw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhiwuduotai.top/gtraccncxy.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.fengsongda.top/gtakyfrevq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.52xcode.cn/gttlmfsieq.html

[H10] 资源自动释放
来源：http://hz.yueranfly.top/gtgxkixuoj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yj20258.top/gteotfrspr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ivvv.top/gtdtsksduh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj202588.top/gthrkqxdva.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.fzhhl.top/gttputaxjw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.wangshuangyany.cn/gtvbohuvdl.html

Go:   defer f.Close()
来源：http://hz.yj20258.top/gtkltnlthk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ybcxt.top/gtvpphmyek.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.sufxvd.cn/gtoqnbyuoj.html

================================================================================
来源：http://hz.meibo888.top/gtzmxvvoef.html

I. 正则表达式
来源：http://hz.ydzc1.top/gtebfwmqmj.html

================================================================================
来源：http://hz.nwbrower.top/gtmiympvxr.html

[I01] 判断是否匹配
来源：http://hz.yuxming.cn/gtjvzoparc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yangfankeji.com/gtwsdnqnao.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yangfankeji.com/gtaqxoadyy.html

JS:   /\d+/.test(s)
来源：http://hz.zhongyouzk.top/gtxvcpztxb.html

TS:   /\d+/.test(s)
来源：http://hz.shzxlz.cn/gtwkcvwhbe.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.redwolf501.top/gtqbfqicka.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yangfankeji.com/gtybvlrxdl.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinqigufen.top/gtajzuywqv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sufxvd.cn/gtgrxsgggj.html

[I02] 提取所有匹配
来源：http://hz.xingfuxueyuan.xyz/gtuelqnvpc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.pycfn.com/gtrugpskbn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yangfankeji.com/gtycnbrunx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.daria6918.cn/gtpyikeoih.html

TS:   s.match(/\d+/g)
来源：http://hz.zhiwuduotai.top/gtqgfkfutj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zdqjudy.top/gtkhxepetj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.guannengcc.top/gtkakswwpu.html

Ruby: s.scan(/\d+/)
来源：http://hz.hammf.cn/gttnumtscz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ywan-chungtsiang.top/gtfmvfcdyu.html

[I03] 提取捕获分组
来源：http://hz.daria6918.cn/gtidzxlgni.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ivvv.top/gtypugwqon.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gogol.net.cn/gtlckribdl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jiagoushi.top/gtxwjxaepq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jianghu66.top/gthvantswk.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.dashuyun.cn/gtceeqbumg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.meibo888.top/gtxvmekgfb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.wangshuangyany.cn/gtpngeyddq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zycfv.cn/gtnckjrqfh.html

[I04] 正则替换
来源：http://hz.daria6918.cn/gtnmysigxq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cdnleiting.top/gthjpwgvyd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jinghuilouyu.cn/gthiahnmja.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ppjwa.cn/gtcoqypych.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xingfuxueyuan.xyz/gtqulimmii.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.nwbrower.top/gtwqqsxbwr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.0kj1m.cn/gtrsaztyzm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hammf.cn/gtdxcrfbxx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.birdmap.top/gtskbkdjqd.html

[I05] 按正则拆分
来源：http://hz.dashuyun.cn/gtwbvjrifv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shzxlz.cn/gtizooswfr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hammf.cn/gthtlugdqa.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gtjorlwnlt.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ywan-chungtsiang.top/gtpfxvqrwa.html

Java: s.split("\\s*,\\s*")
来源：http://hz.smart0.xyz/gttgpkvggf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yueranfly.top/gtwynrhiup.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xziqi.cn/gtrsmnbkqr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.birdmap.top/gtpgxumcor.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jinqigfzy.top/gtbtgbhlvl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yonumen.top/gttnzinezh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.wangdashe.top/gtxkpulfsf.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hammf.cn/gtvqvzekus.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhaomingkeji.xyz/gtxqpcjtoz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.pycfn.com/gtfzbfxmev.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sufxvd.cn/gtukzilcof.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.tian-w.cn/gtosupnmci.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.sweek.top/gtegzfbcpm.html

[I07] 忽略大小写与多行模式
来源：http://hz.316326.xyz/gtalwlbozv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jqgufenzy.top/gtlrirdpkg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.gzhubu.top/gtlddejhrm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yj20258888.top/gtqwzqsbkb.html

TS:   /error/gim
来源：http://hz.shanyushiyangtech.top/gtidwnwqnh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.chenzaomai.com/gtwptbzavv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.sysykeji.top/gtkdkbuvrf.html

Ruby: s.scan(/error/i)
来源：http://hz.fengsongda.top/gtxdamuaye.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.aizwys.cn/gthtnqkyok.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.nanxuanxn.top/gtkwxdxvuv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yongpay.top/gtoqdxfugn.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.smart0.xyz/gtersaabig.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj20258888.top/gtxmqhiytw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nanxinkj.top/gtaschijtf.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.chenjidiqi.icu/gtlkzkitny.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.sxryk.cn/gtpdkmtusz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.chenlongwang.top/gtdgkluyhz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yongpay.top/gtdimhabks.html

================================================================================
来源：http://hz.daria6918.cn/gtccczuguv.html

J. 日期与时间
来源：http://hz.hammf.cn/gtqxvmtruc.html

================================================================================
来源：http://hz.wangdashe.top/gtpldhiymt.html

[J01] 获取当前时间
来源：http://hz.pycfn.com/gtrrdsgjza.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenlongwang.top/gtireyvdar.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.chenzaomai.com/gtxnlmyria.html

JS:   new Date();  Date.now()
来源：http://hz.hnqzz.top/gtbxapfqjg.html

TS:   new Date();  Date.now()
来源：http://hz.jianghu66.top/gtyqmmrecp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xinyue.icu/gtrfjdrwbh.html

Go:   time.Now()
来源：http://hz.hnxiangtu.top/gtuoegybty.html

Ruby: Time.now
来源：http://hz.ybcxt.top/gtdzfkzcuh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yueranfly.top/gtndtivdaf.html

[J02] 格式化输出
来源：http://hz.haohaochexian.top/gtdxfyvzie.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gotoacloud.top/gtupuuwqgk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.gaohongyu789.top/gtpezfsbvf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.chenjidiqi.icu/gtdmzmgcye.html

TS:   d.toISOString()
来源：http://hz.jqgufenzy.top/gtnkiazsun.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shuidangran.top/gtgsvabhvq.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cqqwz.cn/gtrqkqdbsk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.iojbl.cn/gtuzklgoud.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gzhubu.top/gtcvqffpdf.html

[J03] 字符串解析为日期
来源：http://hz.shanyushiyangtech.top/gtruvcljpj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.aizwys.cn/gtbmuqrkwp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jqgufenzy.top/gtnheseyts.html

JS:   new Date("2024-01-02")
来源：http://hz.yj202588.top/gtutxizvuq.html

TS:   new Date("2024-01-02")
来源：http://hz.sxryk.cn/gteliuyppr.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.birdmap.top/gtkflnucfn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.dashuyun.cn/gtxcignvtk.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtnycqczux.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ywan-chungtsiang.top/gtisyrrihy.html

[J04] 时间戳与日期互转
来源：http://hz.guowangkeji.top/gtwakbcwme.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yuanzhike.top/gtqafyfasf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.fzhhl.top/gtbnjxoqiu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.mhx1999.top/gtmwasbdfv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yvedp.cn/gtdenexosj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jlsjyb.cn/gterorzktv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jqgufenzy.top/gtkhzwjwyu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhixingplan.top/gtnyeimrzt.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.tanke756.top/gtwodldscj.html

[J05] 时间加减（加 7 天）
来源：http://hz.jlsjyb.cn/gthizyhpwk.html

Py:   now + timedelta(days=7)
来源：http://hz.dianchejie.cn/gtelsmlukr.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.aibaodan.cn/gttsvrnaxr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ydjk.org.cn/gtcmhqsibk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangdashe.top/gtqtgpcwbh.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ivvv.top/gtrxudboaf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.gogol.net.cn/gtgzcqmduu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cdnleiting.top/gtsrtheyeg.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jlsjyb.cn/gttcyitzao.html

[J06] 计算两时间之差
来源：http://hz.shanyushiyangkeji.top/gtvoddhcip.html

Py:   (end - start).total_seconds()
来源：http://hz.sysykeji.top/gtbtkbaeou.html

PHP:  $end->diff($start)->days;
来源：http://hz.chenlongwang.top/gtpnxnwoie.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.mhx1999.top/gtxlnlkkse.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xinyue.icu/gtksxefoix.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.feifeiyinyue.top/gttlhvzlvx.html

Go:   end.Sub(start).Hours()
来源：http://hz.hysaishi.cn/gtvwnauewx.html

Ruby: end - start                 # 返回秒数
来源：http://hz.vqdsnc.cn/gtojalibsi.html

C#:   (end - start).TotalSeconds
来源：http://hz.feifeiyinyue.top/gtdxvndhhq.html

[J07] 比较两个日期
来源：http://hz.yonumen.top/gtdhdxfrtd.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.fzhhl.top/gtfudbcuex.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zhiwuduotai.top/gtmufwjkdw.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.daxiang520.top/gtpmtwgwbm.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yonumen.top/gtcxkjcbva.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jiagoushi.top/gtpgngsfpv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.nwbrower.top/gtcworxxwo.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.smart0.xyz/gtnqdomdqz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gtrtjbuwnr.html

[J08] 提取年月日与星期
来源：http://hz.guannengcc.top/gthkluorer.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinqigufen.top/gtjsgcsurf.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.svipenyu.cn/gtgnegqcbu.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhijiandao.cn/gtlhbjvupw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hammf.cn/gtrabezsus.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jianghu66.top/gtggdlokdj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.quarkkingdee.top/gtapvcihwh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hnqzz.top/gtwiejeopt.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhaomingkeji.xyz/gtxheafsbx.html

[J09] 时区处理
来源：http://hz.yj202588.top/gtmhuobpmk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.feifeiyinyue.top/gttnmlhskj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.gogol.net.cn/gtkwbqrnkw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.fengsongda.top/gtoepnuuev.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zycfv.cn/gtmvekeiim.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yongpay.top/gtbrfhvnbo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.nanxinkj.top/gtmsmjllhj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shzxlz.cn/gtjmgayxup.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.52xcode.cn/gtgeyzpngu.html

[J10] 取今天 / 本月第一天
来源：http://hz.52xcode.cn/gtydecemrn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.tanke756.top/gtzweegqty.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jianghu66.top/gtsbtizzon.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yuanzhike.top/gtssxjgfxg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yvedp.cn/gtpbuyeans.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yj20258.top/gteoeyfhyz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.tian-w.cn/gtqqoftybo.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shzxlz.cn/gtbynjpkxp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.kuanghao11.cn/gtwxkrpgcq.html

================================================================================
来源：http://hz.yj20258888.top/gtxeugspet.html

K. JSON 与序列化
来源：http://hz.wangdashe.top/gtoflbvsdh.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtaktwukfu.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhengqikj.top/gtumbsgnij.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.chenjidiqi.icu/gtzoxgckoy.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.meibo888.top/gtoyzjzuon.html

JS:   JSON.stringify(obj)
来源：http://hz.nwbrower.top/gtaesabqco.html

TS:   JSON.stringify(obj)
来源：http://hz.yvedp.cn/gtbjbxpvwv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yj202588.top/gtegohcrmk.html

Go:   json.Marshal(obj)
来源：http://hz.gogol.net.cn/gtkymhzwxj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.yj20258888.top/gtigiezjgr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hongshengwenyu.top/gtmjtxpvco.html

[K02] JSON 字符串转对象
来源：http://hz.hammf.cn/gtptgarwrw.html

Py:   json.loads(s)
来源：http://hz.pengpengdd.cyou/gtzjjdoodp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xuanzx.com/gtrinnpvuz.html

JS:   JSON.parse(s)
来源：http://hz.jinqigufen.top/gtyqloooil.html

TS:   JSON.parse(s)
来源：http://hz.zhoulong.xyz/gtuvfkmtaq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hammf.cn/gtoazwkhcl.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhijiandao.cn/gtotzpjbwc.html

Ruby: JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtbnyxlwev.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yj202588.top/gtjepeppqf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jyoumei.cn/gtxdfmznza.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cheryme.top/gtfsgxsjza.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.52xcode.cn/gtmjuhkjym.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.dianchejie.cn/gtbvkgyydd.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhixingplan.top/gtbbousrru.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ydjk.org.cn/gtnnhjqjyf.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.tianlin.xyz/gtlnmtbdtf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.xuanzx.com/gtflrutnjr.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.sweek.top/gtcexrogvg.html

[K04] 读取 JSON 文件
来源：http://hz.daxiang520.top/gtzbvixixm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.tianlin.xyz/gtroehxiwp.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cucudq.cn/gttbqrwwxc.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.fzhhl.top/gtmlqdmfju.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cdnleiting.top/gtlhygzdea.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.wangdashe.top/gtnzvzuxpc.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.haohaochexian.top/gtkiyawtaw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.hongshengwenyu.top/gtynhniwdd.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.pycfn.com/gtqdyzkseo.html

[K05] 深拷贝对象
来源：http://hz.jiagoushi.top/gtczazasiu.html

Py:   copy.deepcopy(obj)
来源：http://hz.shanyushiyangkeji.top/gtjcplqgdi.html

PHP:  unserialize(serialize($obj));
来源：http://hz.dianchejie.cn/gtwxzidrci.html

JS:   structuredClone(obj)
来源：http://hz.iojbl.cn/gtnbrsrnpl.html

TS:   structuredClone(obj)
来源：http://hz.tianlin.xyz/gtiauskzjg.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.xuanzx.com/gtrgnosskz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.xziqi.cn/gtmntbfbdy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.wangshuangyany.cn/gtfhocntcu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.xuetiantiany.cn/gtjovupzne.html

[K06] 解析 URL 查询串
来源：http://hz.pengpengdd.cyou/gtxxgnwhll.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.haohaochexian.top/gtzppgrocw.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.wangdashe.top/gtmlsqmbgk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.nanxuanxn.top/gtcpfgegkb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.jyoumei.cn/gtzouoeeqo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.gzhubu.top/gtyhrgrjfz.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.hfpthk.cn/gtizirpmub.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.tianlin.xyz/gtztbkfyxe.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.ywan-chungtsiang.top/gtyrerytdi.html

[K07] 进制转换
来源：http://hz.shanyushiyangkeji.top/gtermfitfi.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.c1oappe.top/gtvxitczzf.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.bjfxy.top/gtactvtrpb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.hnxiangtu.top/gtxgdltpmd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.kuanghao11.cn/gtspixliuf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.yj20258.top/gtzufbsmou.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.havefunace.top/gtknejhlkn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hz.hammf.cn/gtdcgzmrme.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://hz.gzhubu.top/gtmzwxzbjf.html

[K08] 二进制序列化（非 JSON）
来源：http://hz.jlsjyb.cn/gtypbxjrkd.html

Py:   pickle.dumps(obj)
来源：http://hz.jinyuanbaomall.cn/gtdnnifdor.html

PHP:  serialize($obj);  unserialize($s);
来源：http://hz.316326.xyz/gtvrvhpayw.html

JS:   v8.serialize(obj)        // Node
来源：http://hz.ppjwa.cn/gtzitpaaba.html

TS:   v8.serialize(obj)        // Node
来源：http://hz.cashguo.top/gthtrwqimr.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hz.cucudq.cn/gtqkgkvagl.html

Go:   encoding/gob
来源：http://hz.meibo888.top/gtpfsdvowj.html

Ruby: Marshal.dump(obj)
来源：http://hz.ehwqpu.com/gtmmpsqyuc.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://hz.jinqigufen.top/gtorevvsnh.html

================================================================================
来源：http://hz.jinqigufen.top/gtowwyqmgd.html


<!-- 参考信息 -->