代发 wailian999

TS:   throw new Error("错误信息");
来源：http://hz.chenlongwang.top/gtaxhurvqd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.fengsongda.top/gtnbtjjdhc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jlsjyb.cn/gtgmhrfvvs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gaohongyu789.top/gtbwdjftjw.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhengqikj.top/gtmrgoktgs.html

[H04] 自定义异常类型
来源：http://hz.xinyue.icu/gtykyfhqax.html

Py:   class MyError(Exception): pass
来源：http://hz.cucudq.cn/gtopgbavrg.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.quarkkingdee.top/gthlkhauvg.html

JS:   class MyError extends Error {}
来源：http://hz.ivvv.top/gtmncswitj.html

TS:   class MyError extends Error {}
来源：http://hz.gogol.net.cn/gtyzncrhlq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.chenjidiqi.icu/gtzglhgdhu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinqigufen.top/gtstnmewwc.html

Ruby: class MyError < StandardError; end
来源：http://hz.sufxvd.cn/gttmiwpeji.html

C#:   class MyException : Exception {}
来源：http://hz.ydzc1.top/gtlluhdkem.html

[H05] 捕获特定类型
来源：http://hz.shanyushiyangkeji.top/gtixbhxfpe.html

Py:   except ValueError as e:
来源：http://hz.xylfe.cn/gtteswozed.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.shanyushiyangkeji.top/gtgstujzto.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ydzc1.top/gtlahudeia.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shuidangran.top/gtkuxzndhs.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhongyouzk.top/gtwqcinmys.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cqqwz.cn/gtqosmgner.html

Ruby: rescue ArgumentError => e
来源：http://hz.aibaodan.cn/gttmhiqqnh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.wangdashe.top/gtqprcljye.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhongyouzk.top/gtmawdiuok.html

Py:   value = d.get("k") or default
来源：http://hz.gaohongyu789.top/gtrbeigslr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.chenzaomai.com/gtohjqvpwb.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhaomingkeji.xyz/gtwzpjcgyv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhoulong.xyz/gtukpnjdkx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gogol.net.cn/gtaalxkbzc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.fengsongda.top/gtmjdlnfrd.html

Ruby: d&.dig(:a, :b)
来源：http://hz.quarkkingdee.top/gtlljpyfwv.html

C#:   obj?.A?.B ?? default
来源：http://hz.svipenyu.cn/gtlpdbnrbw.html

[H07] 断言
来源：http://hz.shanyushiyangtech.top/gtjrtddnwa.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hfpthk.cn/gtmsgbcdgw.html

PHP:  assert($x > 0);
来源：http://hz.yanxiufei.cn/gtjebaniul.html

JS:   console.assert(x > 0);
来源：http://hz.ybcxt.top/gtzxwgxqhi.html

TS:   console.assert(x > 0);
来源：http://hz.nanxinkj.top/gtoweoqsmn.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xingfuxueyuan.xyz/gtjnorsdbm.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.pycfn.com/gttvjzcfky.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhixingplan.top/gtqtgtcxwz.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jiagoushi.top/gtksmmdykm.html

[H08] 获取错误信息与堆栈
来源：http://hz.aibaodan.cn/gttnazgevn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ybcxt.top/gtokxrdufu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zdqjudy.top/gtbzdfuqmi.html

JS:   e.message;  e.stack
来源：http://hz.sufxvd.cn/gtxznefotr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhaomingkeji.xyz/gtprxmzljr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.feifeiyinyue.top/gtfspocgze.html

Go:   err.Error()
来源：http://hz.cashguo.top/gtbastookr.html

Ruby: e.message;  e.backtrace
来源：http://hz.yvedp.cn/gtawcctnjj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.fzhhl.top/gthmlfabyh.html

[H09] 带错误码的异常
来源：http://hz.chenlongwang.top/gtfswojejb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.guowangkeji.top/gtdklkyhoz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jiagoushi.top/gtyhxndist.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.quarkkingdee.top/gtfycpqqlb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hfpthk.cn/gtpwificpt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.tian-w.cn/gtwqhfockb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.jyoumei.cn/gtcgkycnqw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhongyouzk.top/gtwzxzhqqm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.nanxuanxn.top/gtuyafbtxf.html

[H10] 资源自动释放
来源：http://hz.jqgfzy.top/gthxzgedmh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yonumen.top/gtxsiikzqw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shanyushiyangtech.top/gtkdafdedy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ywan-chungtsiang.top/gtczcqcfpg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.pengpengdd.cyou/gtzyenfrfo.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.chenlongwang.top/gtyrdncppd.html

Go:   defer f.Close()
来源：http://hz.xuetiantiany.cn/gtcjdnysog.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhixingplan.top/gtuvcwdxes.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xinyue.icu/gtuotwchkb.html

================================================================================
来源：http://hz.xziqi.cn/gtrlytunau.html

I. 正则表达式
来源：http://hz.cheryme.top/gtvaffgnsp.html

================================================================================
来源：http://hz.chenlongwang.top/gtnbshsdbx.html

[I01] 判断是否匹配
来源：http://hz.iojbl.cn/gtibqujqxn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xylfe.cn/gtzqzgxtst.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.nwbrower.top/gtznylzctu.html

JS:   /\d+/.test(s)
来源：http://hz.smart0.xyz/gtejpuklmq.html

TS:   /\d+/.test(s)
来源：http://hz.0kj1m.cn/gtemevswdy.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.nanxuanxn.top/gtxddqcucj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.pengpengdd.cyou/gtqghrlsfh.html

Ruby: s.match?(/\d+/)
来源：http://hz.redwolf501.top/gtoaccifob.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xuanzx.com/gtsglsrlsh.html

[I02] 提取所有匹配
来源：http://hz.birdmap.top/gtsbatnlrl.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yangfankeji.com/gtaajhomgy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.daria6918.cn/gtzyjfgunb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cheryme.top/gtvsqwvaoz.html

TS:   s.match(/\d+/g)
来源：http://hz.tian-w.cn/gtbuojopxc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shanyushiyangkeji.top/gtdyncuzmc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.gzhubu.top/gttsinspsn.html

Ruby: s.scan(/\d+/)
来源：http://hz.cucudq.cn/gtfvlbzknk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.sufxvd.cn/gtlkwwdkxw.html

[I03] 提取捕获分组
来源：http://hz.tanke756.top/gtebinvhpy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhijiandao.cn/gthagecegf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.zdqjudy.top/gtctkppfrs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.snrcjt.cn/gtwkgklwof.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yj20258888.top/gtdriefyzo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.daria6918.cn/gtdmlmdepe.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ehwqpu.com/gtfaqtpxce.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.52xcode.cn/gteaacddxt.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.nanxinkj.top/gtmpplvedi.html

[I04] 正则替换
来源：http://hz.jlsjyb.cn/gtqzpbavqg.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.vqdsnc.cn/gtjlmbvxct.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jiagoushi.top/gtbblypfmv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhongyouzk.top/gtssjtnwim.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yanxiufei.cn/gtjgzhnndr.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.dianchejie.cn/gtdzayuigg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jiagoushi.top/gtjcbyscpz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hongshengwenyu.top/gtlxrlckmc.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.wangdashe.top/gtjpnogtjn.html

[I05] 按正则拆分
来源：http://hz.zdqjudy.top/gtcahddugr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yj20258888.top/gtfhxlzbjp.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.cheryme.top/gthopkvbpu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yj20258.top/gtowhpuvip.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.guowangkeji.top/gtspxabowd.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yangfankeji.com/gtqrvwubbl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhijiandao.cn/gtpuxnvpyo.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhoulong.xyz/gtefoivdga.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.tianlin.xyz/gtspviwutg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhaomingkeji.xyz/gtilpzuzfv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hywenlv.cn/gtrtmrxyrv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.chenzaomai.com/gtewcjbirv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.feifeiyinyue.top/gtiycriabe.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aizwys.cn/gtwkjhtzuh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yvedp.cn/gtpsizbwzt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.nwbrower.top/gtoismirpr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.havefunace.top/gtsnlenuzl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.9152youxi.cn/gtbfnzditq.html

[I07] 忽略大小写与多行模式
来源：http://hz.jiagoushi.top/gttaobyoyr.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.gaohongyu789.top/gtwvhwxxbq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.nanxuanxn.top/gtxkzzgojt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.tianlin.xyz/gtlifbpidf.html

TS:   /error/gim
来源：http://hz.gogol.net.cn/gtnedvoyxk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.snrcjt.cn/gtzskbhyez.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yj20258.top/gteiodvhwh.html

Ruby: s.scan(/error/i)
来源：http://hz.ydzc1.top/gtmwmeubft.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.aizwys.cn/gtadpezqyy.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.nanxinkj.top/gtzvaasotk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.gzhubu.top/gtgnxlopuj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinqigufen.top/gtxgoucpse.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.fzhhl.top/gtywtmzhvs.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hywenlv.cn/gtcnqdkatx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hammf.cn/gtsuibegrl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cqqwz.cn/gtbgdnalxn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.quarkkingdee.top/gtnszuyunp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zycfv.cn/gtgcrrnitt.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtjtarfjgv.html

J. 日期与时间
来源：http://hz.guowangkeji.top/gtvtqqagvi.html

================================================================================
来源：http://hz.daxiang520.top/gtamlidtri.html

[J01] 获取当前时间
来源：http://hz.tanke756.top/gtrnclsixz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinyuanbaomall.cn/gtowjefubq.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.daria6918.cn/gtxbidsvrs.html

JS:   new Date();  Date.now()
来源：http://hz.smart0.xyz/gtkjixiiza.html

TS:   new Date();  Date.now()
来源：http://hz.yangfankeji.com/gtutwqbhpt.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.andypj.xyz/gtcdofvlaf.html

Go:   time.Now()
来源：http://hz.shanyushiyangtech.top/gthwzsjmqe.html

Ruby: Time.now
来源：http://hz.hnxiangtu.top/gtllbxeuky.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.0kj1m.cn/gtalenweod.html

[J02] 格式化输出
来源：http://hz.daria6918.cn/gtpefwaepj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yangfankeji.com/gtrdkthjsh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.gogol.net.cn/gtsoajmxyu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hywenlv.cn/gtmkwpohex.html

TS:   d.toISOString()
来源：http://hz.nwbrower.top/gttnqlsers.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.cashguo.top/gtorscedou.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.zhijiandao.cn/gtoozkzfyz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xingfuxueyuan.xyz/gtgchpizfx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.sysykeji.top/gtxrryughd.html

[J03] 字符串解析为日期
来源：http://hz.jinyuanbaomall.cn/gtmeylrflm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.tianlin.xyz/gtsantiqlg.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yueranfly.top/gthavuqmmh.html

JS:   new Date("2024-01-02")
来源：http://hz.pycfn.com/gtthjaxkps.html

TS:   new Date("2024-01-02")
来源：http://hz.chenlongwang.top/gthifmvlho.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sweek.top/gtwztspsid.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhixingplan.top/gtboqlyzbf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.mhx1999.top/gtowlfncwp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cashguo.top/gtbuleeuap.html

[J04] 时间戳与日期互转
来源：http://hz.sxryk.cn/gtfezqjmsi.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yuanzhike.top/gttvuksuka.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.guowangkeji.top/gtrgzmbgkn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.bjfxy.top/gtwrbjchmo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.fzhhl.top/gttednomki.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cqqwz.cn/gtzfpczboj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhoulong.xyz/gtlngokqiv.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.fzhhl.top/gttcoegujy.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.wangdashe.top/gtviyncgck.html

[J05] 时间加减（加 7 天）
来源：http://hz.xziqi.cn/gtcndjzscm.html

Py:   now + timedelta(days=7)
来源：http://hz.zhengqikj.top/gtymjiagde.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.kuanghao11.cn/gtnnqliqrt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ywan-chungtsiang.top/gtwqfbcsdc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.iojbl.cn/gtxksgpmfz.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.daxiang520.top/gttmxvpkwj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cucudq.cn/gtkdjqohid.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shanyushiyangkeji.top/gtfnlzngiv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.tian-w.cn/gthxnurhnh.html

[J06] 计算两时间之差
来源：http://hz.feifeiyinyue.top/gtjhmrcvmq.html

Py:   (end - start).total_seconds()
来源：http://hz.c1oappe.top/gtdwiolcdn.html

PHP:  $end->diff($start)->days;
来源：http://hz.hnqzz.top/gtxpxzavnw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.nanxuanxn.top/gtudhycrcq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.daxiang520.top/gtqbidmxvq.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.chenjidiqi.icu/gtjdfjzrka.html

Go:   end.Sub(start).Hours()
来源：http://hz.ydzc1.top/gtqntklruc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.chenlongwang.top/gtrbqsjdfh.html

C#:   (end - start).TotalSeconds
来源：http://hz.cdnleiting.top/gtpbxfzivu.html

[J07] 比较两个日期
来源：http://hz.guannengcc.top/gtdwlpwaqp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yj202588.top/gtoujrilcq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.dashuyun.cn/gtfyuabixb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.52xcode.cn/gtrsxoekvs.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shangyingyoupin.top/gtlineughl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xziqi.cn/gtqqtyaclz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.svipenyu.cn/gtahdqooso.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtbsvtaxpk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hammf.cn/gtkxnnksxz.html

[J08] 提取年月日与星期
来源：http://hz.xuanzx.com/gtknqxwcdy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.mhx1999.top/gtrnfwxaig.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shangyingyoupin.top/gtorakbmwp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.52xcode.cn/gtqtyccpcc.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xuetiantiany.cn/gtcypljxzs.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shanyushiyangtech.top/gtuwjxyigj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yuxming.cn/gtubsbutlg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.ivvv.top/gtusegepjq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gzhubu.top/gtgkjnabgb.html

[J09] 时区处理
来源：http://hz.hnqzz.top/gtuinfvshh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xuanzx.com/gtikkomajb.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.mhx1999.top/gtkvbvgriu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ivvv.top/gtuwnonrgu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yanxiufei.cn/gtuzleswqt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hnxiangtu.top/gtoonhitpu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhongyouzk.top/gtxlzqeyli.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yvedp.cn/gtsbywjhft.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.0kj1m.cn/gtgjxgqnln.html

[J10] 取今天 / 本月第一天
来源：http://hz.yvedp.cn/gtfcpnppod.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yvedp.cn/gtrhnlypkx.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jinyuanbaomall.cn/gtnchwgupq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.nanxinkj.top/gtzoznzlhq.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.0kj1m.cn/gtdlksnogk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yuxming.cn/gtppalfhlm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cucudq.cn/gtruuukisu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cucudq.cn/gtujddeirw.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.haohaochexian.top/gtskgaiuor.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtpctcuyhl.html

K. JSON 与序列化
来源：http://hz.xingfuxueyuan.xyz/gtxwgypjkz.html

================================================================================
来源：http://hz.pengpengdd.cyou/gthxnxrcbd.html

[K01] 对象转 JSON 字符串
来源：http://hz.yangfankeji.com/gtqrfjiqsx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yongpay.top/gtgtdmynvu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yongpay.top/gtvsnamiep.html

JS:   JSON.stringify(obj)
来源：http://hz.mhx1999.top/gtthnuhebu.html

TS:   JSON.stringify(obj)
来源：http://hz.bjfxy.top/gtvpfgjwxm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.aizwys.cn/gttvktjcwo.html

Go:   json.Marshal(obj)
来源：http://hz.havefunace.top/gtkbllwajb.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.nanxuanxn.top/gtiqkpiutx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.tanke756.top/gtzuzasqwj.html

[K02] JSON 字符串转对象
来源：http://hz.shangyingyoupin.top/gtxdzdxuko.html

Py:   json.loads(s)
来源：http://hz.chenlongwang.top/gtgfdfoaqy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jiagoushi.top/gtfijdxpmp.html

JS:   JSON.parse(s)
来源：http://hz.jiagoushi.top/gtyfdfggpy.html

TS:   JSON.parse(s)
来源：http://hz.ybcxt.top/gtvveoeisi.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.hammf.cn/gtktmuwhyd.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sxryk.cn/gtmyddizdn.html

Ruby: JSON.parse(s)
来源：http://hz.quarkkingdee.top/gtkniddefg.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.gotoacloud.top/gtirsxucfr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.snrcjt.cn/gtzkfvcakm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ehwqpu.com/gtvijfmuxu.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.kuanghao11.cn/gtjjiguvdd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.vqdsnc.cn/gtvdlyxhli.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yongpay.top/gteyllfgnf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.sweek.top/gtqkveouhw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.dianchejie.cn/gtzojcyugd.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sxryk.cn/gtkohpgnbb.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.shuidangran.top/gtsvuktbsn.html

[K04] 读取 JSON 文件
来源：http://hz.svipenyu.cn/gtywcnsbkp.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hnxiangtu.top/gtqcgckwlc.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhiwuduotai.top/gtlamlvhpj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.sweek.top/gtedhsorio.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.chenjidiqi.icu/gtjnldtwwc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.zhijiandao.cn/gtzflcqwxl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.dashuyun.cn/gtudscvyyt.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.yanxiufei.cn/gtmaraesri.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.guowangkeji.top/gtykeboyja.html

[K05] 深拷贝对象
来源：http://hz.xuetiantiany.cn/gtdgubltcq.html

Py:   copy.deepcopy(obj)
来源：http://hz.zycfv.cn/gtcygutdqo.html

PHP:  unserialize(serialize($obj));
来源：http://hz.cucudq.cn/gtjzjopziq.html

JS:   structuredClone(obj)
来源：http://hz.quarkkingdee.top/gtksvyfner.html

TS:   structuredClone(obj)
来源：http://hz.yuanzhike.top/gtsbrahkqf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.feifeiyinyue.top/gtmwvyhwrh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.havefunace.top/gtbrivoima.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xuanzx.com/gteybkaibi.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.aibaodan.cn/gtfgnwcyku.html

[K06] 解析 URL 查询串
来源：http://hz.hysaishi.cn/gtzvqtkyxa.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hysaishi.cn/gtemzsczkx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.xuetiantiany.cn/gtnkdhyvqr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.fengsongda.top/gtxqkezirz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xziqi.cn/gtgicxdzer.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.quarkkingdee.top/gtudeqqmfy.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.zhaomingkeji.xyz/gtnapmsfwq.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.ppjwa.cn/gtynddnaph.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hz.jlsjyb.cn/gtvdvhbjmi.html

[K07] 进制转换
来源：http://hz.zhongyouzk.top/gtlufyxdcm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hz.ppjwa.cn/gtylbjipgy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hz.shangyingyoupin.top/gtcxfrwcub.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hz.gotoacloud.top/gtbqpgbmth.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hz.sxryk.cn/gtbjrbwntl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hz.birdmap.top/gtslscoueg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hz.mhx1999.top/gtpdzvnyov.html


<!-- 参考信息 -->