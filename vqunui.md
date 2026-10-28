代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtruzawpbv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.daria6918.cn/gtshpuocyn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xuetiantiany.cn/gtxmksqxys.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xuetiantiany.cn/gtyleotsrd.html

[H03] 主动抛出异常
来源：http://hz.316326.xyz/gtcxqtwlgs.html

Py:   raise ValueError("错误信息")
来源：http://hz.dashuyun.cn/gtifpbxqdf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.snrcjt.cn/gtkhollsnl.html

JS:   throw new Error("错误信息");
来源：http://hz.xylfe.cn/gtghqrmazh.html

TS:   throw new Error("错误信息");
来源：http://hz.ivvv.top/gtvjwihdcz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.chenlongwang.top/gtmtrkyuwu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.cucudq.cn/gtifetvitb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ydzc1.top/gtycbyscrs.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.smart0.xyz/gtzntzoofi.html

[H04] 自定义异常类型
来源：http://hz.shanyushiyangtech.top/gtmzcelkoy.html

Py:   class MyError(Exception): pass
来源：http://hz.ydzc1.top/gtpdnpfkjb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.mhx1999.top/gthbpphtqo.html

JS:   class MyError extends Error {}
来源：http://hz.svipenyu.cn/gtaivxvajd.html

TS:   class MyError extends Error {}
来源：http://hz.sufxvd.cn/gtcyetnilm.html

Java: class MyException extends RuntimeException {}
来源：http://hz.aizwys.cn/gtfogrmoru.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yj20258888.top/gttsomlboq.html

Ruby: class MyError < StandardError; end
来源：http://hz.dashuyun.cn/gtsywfglld.html

C#:   class MyException : Exception {}
来源：http://hz.zdqjudy.top/gtmyxslvoc.html

[H05] 捕获特定类型
来源：http://hz.ppjwa.cn/gtcvkuiupb.html

Py:   except ValueError as e:
来源：http://hz.haohaochexian.top/gtlzawglqd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.mhx1999.top/gtbtpgwovj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yvedp.cn/gtjnsjicro.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gogol.net.cn/gtgifxwkjj.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.bjfxy.top/gtbdotvuqb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gaohongyu789.top/gtcxsehiun.html

Ruby: rescue ArgumentError => e
来源：http://hz.aizwys.cn/gtaeopchpj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.havefunace.top/gthsabksdo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.meibo888.top/gtkytcrdss.html

Py:   value = d.get("k") or default
来源：http://hz.ybcxt.top/gtetuauxvd.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hnqzz.top/gtdeiqpcgt.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ivvv.top/gtcibngscd.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jianghu66.top/gtaxiwmkwk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xuetiantiany.cn/gtautaqjbi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.mhx1999.top/gtnpyknnpd.html

Ruby: d&.dig(:a, :b)
来源：http://hz.fengsongda.top/gtluccuixh.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinyuanbaomall.cn/gtsjfbzhpq.html

[H07] 断言
来源：http://hz.hywenlv.cn/gtdmestabz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ivvv.top/gtmjhfwfxu.html

PHP:  assert($x > 0);
来源：http://hz.wangshuangyany.cn/gtxqbckjju.html

JS:   console.assert(x > 0);
来源：http://hz.sweek.top/gtpqbwezlo.html

TS:   console.assert(x > 0);
来源：http://hz.0kj1m.cn/gtzzpvftfn.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ybcxt.top/gtxxplahhc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jyoumei.cn/gtnazdmlff.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yangfankeji.com/gthwciwwgy.html

C#:   Debug.Assert(x > 0);
来源：http://hz.pycfn.com/gtuwhyfjpa.html

[H08] 获取错误信息与堆栈
来源：http://hz.aizwys.cn/gtpyopibdr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.svipenyu.cn/gtdffvnhpo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.tanke756.top/gtiuyhgcae.html

JS:   e.message;  e.stack
来源：http://hz.hammf.cn/gtfsgwravj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinghuilouyu.cn/gtbivxmccc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ppjwa.cn/gtjfxgzceg.html

Go:   err.Error()
来源：http://hz.wangshuangyany.cn/gtifsoaiip.html

Ruby: e.message;  e.backtrace
来源：http://hz.yvedp.cn/gtykxyyeef.html

C#:   e.Message;  e.StackTrace
来源：http://hz.cashguo.top/gtxakffefr.html

[H09] 带错误码的异常
来源：http://hz.kuanghao11.cn/gtpadsdepp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shzxlz.cn/gtgbtxozrz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yanxiufei.cn/gtcelwxwdv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jinqigfzy.top/gtgyzvvbof.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xingfuxueyuan.xyz/gtxxkbfedl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yongpay.top/gtirmxgzzz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cheryme.top/gtskunvtko.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sysykeji.top/gtkjwacazp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinqigufen.top/gtugexfgux.html

[H10] 资源自动释放
来源：http://hz.yueranfly.top/gtynzwhdsb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xuanzx.com/gteiajhwtf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.birdmap.top/gtmutsvwox.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.9152youxi.cn/gtlwulrhpb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxinkj.top/gtzvwqdvfc.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.fengsongda.top/gtbndjgpup.html

Go:   defer f.Close()
来源：http://hz.kuanghao11.cn/gtuffvlcrf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sweek.top/gtazvjnckh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hywenlv.cn/gtzdlxgjkd.html

================================================================================
来源：http://hz.xziqi.cn/gtudytseen.html

I. 正则表达式
来源：http://hz.zhixingplan.top/gtkrbdarnj.html

================================================================================
来源：http://hz.ydzc1.top/gtjvhtlbwm.html

[I01] 判断是否匹配
来源：http://hz.zhongyouzk.top/gtzdbqaspw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hywenlv.cn/gtvoeryckj.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhiwuduotai.top/gtzsljvoan.html

JS:   /\d+/.test(s)
来源：http://hz.yangfankeji.com/gtxwyypqup.html

TS:   /\d+/.test(s)
来源：http://hz.yj20258888.top/gtlqlhrahb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hnqzz.top/gtjwasfoic.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhiwuduotai.top/gtizlugtzj.html

Ruby: s.match?(/\d+/)
来源：http://hz.vqdsnc.cn/gtyvcjsmej.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhixingplan.top/gtmapvhtgq.html

[I02] 提取所有匹配
来源：http://hz.yonumen.top/gtdzckrrlb.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hnxiangtu.top/gtpbuprpdm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.svipenyu.cn/gtkexchzsp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.havefunace.top/gtnuyetimc.html

TS:   s.match(/\d+/g)
来源：http://hz.feifeiyinyue.top/gtwzzbkjna.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.redwolf501.top/gtuakfgykx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hfpthk.cn/gtevgcdqms.html

Ruby: s.scan(/\d+/)
来源：http://hz.zycfv.cn/gtcbvzkwej.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hongshengwenyu.top/gtgssuyncr.html

[I03] 提取捕获分组
来源：http://hz.zhongyouzk.top/gtixebviit.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hnqzz.top/gtsplifqnb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jianghu66.top/gtjpcnzker.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.nanxinkj.top/gtusbrybpa.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.sxryk.cn/gtryvgsqwc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.haohaochexian.top/gtvynngqdp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhaomingkeji.xyz/gtjvxonhdz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhixingplan.top/gtsskwxabs.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.andypj.xyz/gtctuvccxs.html

[I04] 正则替换
来源：http://hz.kuanghao11.cn/gtwwjxjqtr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jqgufenzy.top/gtjwxbkpbe.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhengqikj.top/gtjcmlowgp.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhijiandao.cn/gtzdtoerps.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yuanzhike.top/gtnccxsupj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.shanyushiyangtech.top/gtcwjlgnrs.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.gaohongyu789.top/gtdrsbevsg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yongpay.top/gtxiodovtt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cqqwz.cn/gtuvnmfwej.html

[I05] 按正则拆分
来源：http://hz.redwolf501.top/gtbryswlxb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hongshengwenyu.top/gtwbfplmpx.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinqigufen.top/gtqyyaidlj.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.tianlin.xyz/gtjyhxlfkc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhoulong.xyz/gtxuzwqybv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.redwolf501.top/gtjdfdwmhp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.dianchejie.cn/gtzzjfrogb.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangkeji.top/gtzilmaeic.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.quarkkingdee.top/gttjshmjpa.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.bjfxy.top/gtufxegsud.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.chenzaomai.com/gtaxgkimts.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhengqikj.top/gtgzpfgmgd.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hongshengwenyu.top/gtwszzqlab.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.kuanghao11.cn/gtebdhzhde.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hongshengwenyu.top/gtzzyhxtbc.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.0kj1m.cn/gtbxaduufb.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yueranfly.top/gtzhldzakb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhongyouzk.top/gtpoixesjo.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhoulong.xyz/gtatcbtuko.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.chenzaomai.com/gtmywwrkpt.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhijiandao.cn/gtihlpuyqb.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shanyushiyangtech.top/gtqogmdqsk.html

TS:   /error/gim
来源：http://hz.jinyuanbaomall.cn/gtdcarswra.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhengqikj.top/gtndlyjpzb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hywenlv.cn/gtbvgoupas.html

Ruby: s.scan(/error/i)
来源：http://hz.ehwqpu.com/gtbhlrjbmc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj20258.top/gtytngmxqy.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sxryk.cn/gtzpiddwbp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ydzc1.top/gtilnsyqgb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cqqwz.cn/gtqsmywqqn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.316326.xyz/gtfntvrzgr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yanxiufei.cn/gteziqmios.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jinqigfzy.top/gtdtlklthg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.nanxuanxn.top/gtnfpegcpe.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hywenlv.cn/gtoikiwrcp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cdnleiting.top/gtxaztupeu.html

================================================================================
来源：http://hz.havefunace.top/gttulyksyo.html

J. 日期与时间
来源：http://hz.c1oappe.top/gtmrjankex.html

================================================================================
来源：http://hz.snrcjt.cn/gtkcwhtlir.html

[J01] 获取当前时间
来源：http://hz.gzhubu.top/gtaddqzkrm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhoulong.xyz/gtlwmciyug.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cqqwz.cn/gthlzcovls.html

JS:   new Date();  Date.now()
来源：http://hz.wangdashe.top/gtnqlzppns.html

TS:   new Date();  Date.now()
来源：http://hz.gotoacloud.top/gthutjnpbq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.316326.xyz/gtzksghikv.html

Go:   time.Now()
来源：http://hz.ivvv.top/gtoibulohk.html

Ruby: Time.now
来源：http://hz.aibaodan.cn/gtokhzuwmz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yongpay.top/gtgvyeqglw.html

[J02] 格式化输出
来源：http://hz.hysaishi.cn/gtxrmclvyr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.andypj.xyz/gtehrunvis.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.pycfn.com/gtidigzjnu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.fzhhl.top/gtwrbxaqbb.html

TS:   d.toISOString()
来源：http://hz.pycfn.com/gtohceugrq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ppjwa.cn/gtdmjrugvt.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yuanzhike.top/gtjvyngemm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.svipenyu.cn/gtmkpaxpnk.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.haohaochexian.top/gtmssadzti.html

[J03] 字符串解析为日期
来源：http://hz.gzhubu.top/gtyonbebpz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sweek.top/gtjtavtyfk.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xingfuxueyuan.xyz/gtcybpasym.html

JS:   new Date("2024-01-02")
来源：http://hz.sweek.top/gtwukogofo.html

TS:   new Date("2024-01-02")
来源：http://hz.chenlongwang.top/gtxpqfnaoz.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.tanke756.top/gtlejofqud.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.svipenyu.cn/gtltgfvsmn.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinqigufen.top/gtfmxethdy.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yanxiufei.cn/gteecqztdc.html

[J04] 时间戳与日期互转
来源：http://hz.sysykeji.top/gtigvjocuw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.chenzaomai.com/gtocxtqqox.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.birdmap.top/gtwvrhfpcv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yuanzhike.top/gtmdeeeyar.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhixingplan.top/gtluteshqp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ywan-chungtsiang.top/gthxslctbe.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jiagoushi.top/gtbpxbfqqz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.xylfe.cn/gtnqyatdop.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.smart0.xyz/gtjocpocgn.html

[J05] 时间加减（加 7 天）
来源：http://hz.hnxiangtu.top/gtdedwssid.html

Py:   now + timedelta(days=7)
来源：http://hz.hysaishi.cn/gtnuspqaxa.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.vqdsnc.cn/gttxihqtdc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xinyue.icu/gtzdbtgvgy.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cdnleiting.top/gtsbqrcoaa.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shzxlz.cn/gtbffkltpy.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.daria6918.cn/gtkcmztqvt.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shanyushiyangtech.top/gtzquvwvtw.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.fzhhl.top/gttbljjptr.html

[J06] 计算两时间之差
来源：http://hz.xziqi.cn/gtytclmfqf.html

Py:   (end - start).total_seconds()
来源：http://hz.hysaishi.cn/gtglkreulg.html

PHP:  $end->diff($start)->days;
来源：http://hz.smart0.xyz/gtfxumbcdy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.chenzaomai.com/gtyowspzqa.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jiagoushi.top/gtvqvbfxrc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zycfv.cn/gtejokqgkl.html

Go:   end.Sub(start).Hours()
来源：http://hz.jinqigfzy.top/gtjfghwski.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xuanzx.com/gtuouwnxcw.html

C#:   (end - start).TotalSeconds
来源：http://hz.sysykeji.top/gtrgsatuig.html

[J07] 比较两个日期
来源：http://hz.hammf.cn/gtpasrdkms.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ybcxt.top/gtilgfubzv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.fengsongda.top/gtsewdackx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zycfv.cn/gtrpaqynqi.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.feifeiyinyue.top/gtfvwknrnb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.wangshuangyany.cn/gtrpftxxrq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.snrcjt.cn/gtmqjmdtfl.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.fzhhl.top/gtlrxcvukz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.smart0.xyz/gtzyrainfx.html

[J08] 提取年月日与星期
来源：http://hz.zhengqikj.top/gtmqrehwkt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.iojbl.cn/gtxzjffmpw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hysaishi.cn/gtgocolzpw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.fzhhl.top/gtoghznyti.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.wangshuangyany.cn/gtqwfqgwcq.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jyoumei.cn/gtcwlpwahx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jlsjyb.cn/gtxesnmher.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cucudq.cn/gtkstytbpj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhijiandao.cn/gtfoaetnlu.html

[J09] 时区处理
来源：http://hz.jinqigufen.top/gtqlfpvshd.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.chenzaomai.com/gtmnuupcso.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.316326.xyz/gtilfwerkp.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.haohaochexian.top/gtczmwqhgv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.gogol.net.cn/gtrdyccxyf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.smart0.xyz/gtaqcdazoc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhijiandao.cn/gtpdlwwbbl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hfpthk.cn/gtgcldqmkc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yj202588.top/gtbhmifwtr.html

[J10] 取今天 / 本月第一天
来源：http://hz.mhx1999.top/gtpxxoibfg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.wangdashe.top/gtijedabry.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.tianlin.xyz/gtfovaigev.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.aizwys.cn/gtyobstpkc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.bjfxy.top/gtegfpiiiu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.daxiang520.top/gtrizkmdba.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhaomingkeji.xyz/gtnmzewcab.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cashguo.top/gtgklavpxf.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yanxiufei.cn/gtgkirjjjz.html

================================================================================
来源：http://hz.zhijiandao.cn/gtwcfzojth.html

K. JSON 与序列化
来源：http://hz.guowangkeji.top/gtfxmmopoe.html

================================================================================
来源：http://hz.ppjwa.cn/gtcajsagtz.html

[K01] 对象转 JSON 字符串
来源：http://hz.andypj.xyz/gtkqgkjnqh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shanyushiyangkeji.top/gtlyltlajc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.dashuyun.cn/gtfbtbhyfo.html

JS:   JSON.stringify(obj)
来源：http://hz.yuxming.cn/gtlkaznfsn.html

TS:   JSON.stringify(obj)
来源：http://hz.zhoulong.xyz/gtxptzdjyl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.gaohongyu789.top/gtvnunibww.html

Go:   json.Marshal(obj)
来源：http://hz.cheryme.top/gtylmcslhl.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinqigfzy.top/gtlgpfqeiz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cqqwz.cn/gtcvdspclc.html

[K02] JSON 字符串转对象
来源：http://hz.hywenlv.cn/gtlkknlmjw.html

Py:   json.loads(s)
来源：http://hz.c1oappe.top/gtdvstxoxd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.9152youxi.cn/gtciuprbfy.html

JS:   JSON.parse(s)
来源：http://hz.xuetiantiany.cn/gtwndqmujm.html

TS:   JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtrweyytwq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shzxlz.cn/gtjaovgihx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jiagoushi.top/gtkpeltbzd.html

Ruby: JSON.parse(s)
来源：http://hz.shzxlz.cn/gtppypkjvl.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yonumen.top/gtpyrmaqle.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hnqzz.top/gtticqwdbo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ybcxt.top/gthwsxkyei.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.meibo888.top/gttbqodxjo.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuanzx.com/gtjughpojq.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.pycfn.com/gtzgaxkpxk.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.feifeiyinyue.top/gtntsfdifq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.52xcode.cn/gtqqfhzwoe.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhaomingkeji.xyz/gtceinngrh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.svipenyu.cn/gtzcbscfkz.html

[K04] 读取 JSON 文件
来源：http://hz.cqqwz.cn/gthzzafyal.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yj20258.top/gtkfjgyuwn.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ywan-chungtsiang.top/gtnezxcbtf.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hywenlv.cn/gtamavjvth.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.quarkkingdee.top/gtqjvxvizz.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.haohaochexian.top/gtozxjyfsj.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ehwqpu.com/gtdeyocgpv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.aibaodan.cn/gtiaidhwpi.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.zycfv.cn/gtxgeqjpfa.html

[K05] 深拷贝对象
来源：http://hz.hfpthk.cn/gtpeqnimze.html

Py:   copy.deepcopy(obj)
来源：http://hz.hysaishi.cn/gtpzxtlwxk.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yj202588.top/gtdtcpejhp.html

JS:   structuredClone(obj)
来源：http://hz.wangdashe.top/gtrahlbqny.html

TS:   structuredClone(obj)
来源：http://hz.shanyushiyangtech.top/gtzwtqfdhc.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.gzhubu.top/gtekilkbme.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.yueranfly.top/gtciyvuyfs.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.tian-w.cn/gtnrbxwzda.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.zycfv.cn/gthkwtfnhp.html

[K06] 解析 URL 查询串
来源：http://hz.shanyushiyangtech.top/gtkdwrfaxm.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.hongshengwenyu.top/gtchevzovn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.yj202588.top/gtqselgoji.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.xinyue.icu/gtcknppqwx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.zhijiandao.cn/gtbwqevvgd.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.9152youxi.cn/gtaskbppjg.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.gotoacloud.top/gtdalcihpf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.gogol.net.cn/gtsiqaogem.html


<!-- 参考信息 -->