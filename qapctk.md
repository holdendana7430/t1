代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jinyuanbaomall.cn/gtzfqtcrcu.html

Ruby: obj.instance_variables
来源：http://hz.zhixingplan.top/gtxdcztmiq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jinghuilouyu.cn/gtrcxfqxnt.html

================================================================================
来源：http://hz.9152youxi.cn/gtjmtxfbuw.html

H. 异常与错误处理
来源：http://hz.ywan-chungtsiang.top/gtfjynirlk.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtehdmyysu.html

[H01] try / catch 基础
来源：http://hz.nanxuanxn.top/gtgrarhhat.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinqigfzy.top/gtzqurwwvz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yangfankeji.com/gtxsziloio.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yj20258.top/gtgevwufgm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.tianlin.xyz/gttbnttvyi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jqgfzy.top/gtpoltuzhs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yj202588.top/gtvznspfzw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jlsjyb.cn/gtqjmbioqs.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yj202588.top/gtoarspoiu.html

[H02] finally / ensure 收尾
来源：http://hz.redwolf501.top/gtmtgocuuw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cheryme.top/gtffoheepe.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtofchhplw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gtimeqwrye.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.tianlin.xyz/gtviykbpxi.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yanxiufei.cn/gtzvzbwwtp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.svipenyu.cn/gtgrnunydg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ppjwa.cn/gtakfjphmc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtfguvqijq.html

[H03] 主动抛出异常
来源：http://hz.yonumen.top/gtdikbknzk.html

Py:   raise ValueError("错误信息")
来源：http://hz.zycfv.cn/gthtyczalh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ppjwa.cn/gtfaveukxq.html

JS:   throw new Error("错误信息");
来源：http://hz.yueranfly.top/gtosjctlws.html

TS:   throw new Error("错误信息");
来源：http://hz.nanxinkj.top/gtiwazisvs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.hammf.cn/gtnscdkrow.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.vqdsnc.cn/gtbaxfvfdp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ppjwa.cn/gtmjkrsobg.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sweek.top/gttzpmewjd.html

[H04] 自定义异常类型
来源：http://hz.kuanghao11.cn/gtqekvmopo.html

Py:   class MyError(Exception): pass
来源：http://hz.yj20258.top/gtgvqcceak.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.redwolf501.top/gtezznylmb.html

JS:   class MyError extends Error {}
来源：http://hz.andypj.xyz/gtynalhegy.html

TS:   class MyError extends Error {}
来源：http://hz.jinqigfzy.top/gttiqsytaz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.daria6918.cn/gtmosyakkx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.smart0.xyz/gtnaqgbrnt.html

Ruby: class MyError < StandardError; end
来源：http://hz.gaohongyu789.top/gtckquorrf.html

C#:   class MyException : Exception {}
来源：http://hz.xziqi.cn/gtvlyqijst.html

[H05] 捕获特定类型
来源：http://hz.aibaodan.cn/gtzbflebtg.html

Py:   except ValueError as e:
来源：http://hz.zhijiandao.cn/gtqeymyxsa.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hywenlv.cn/gtsggtdqbx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhixingplan.top/gtpzivbuqv.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shuidangran.top/gtcgmxtmoe.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nanxinkj.top/gtyptwxmmw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.iojbl.cn/gtfdshhdli.html

Ruby: rescue ArgumentError => e
来源：http://hz.cdnleiting.top/gtsymiaytg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yongpay.top/gtsdbitpxr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.daria6918.cn/gtkwvlgtwt.html

Py:   value = d.get("k") or default
来源：http://hz.nanxinkj.top/gtfyqrydwl.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.andypj.xyz/gtvmissofo.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.316326.xyz/gtrmofcmfx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shzxlz.cn/gtjupnpbys.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cqqwz.cn/gtolmpzxsc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.pycfn.com/gtgtdcywxb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.daxiang520.top/gtjhygvtek.html

C#:   obj?.A?.B ?? default
来源：http://hz.c1oappe.top/gttlxoqjqr.html

[H07] 断言
来源：http://hz.316326.xyz/gtuzqdcqhl.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ywan-chungtsiang.top/gtotnipfwn.html

PHP:  assert($x > 0);
来源：http://hz.jinyuanbaomall.cn/gtsqwulckd.html

JS:   console.assert(x > 0);
来源：http://hz.quarkkingdee.top/gteofysvmi.html

TS:   console.assert(x > 0);
来源：http://hz.cucudq.cn/gtvpupzyvo.html

Java: assert x > 0 : "必须为正";
来源：http://hz.cheryme.top/gtwclxbwow.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.dianchejie.cn/gtgjkvnyuc.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.gaohongyu789.top/gtlecsfeah.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yonumen.top/gtjeolxisa.html

[H08] 获取错误信息与堆栈
来源：http://hz.bjfxy.top/gtueszwdgh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.chenlongwang.top/gtpqjozeoz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenzaomai.com/gtlddnsmqd.html

JS:   e.message;  e.stack
来源：http://hz.gogol.net.cn/gthzhscufb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yj20258.top/gtjswonbhs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sweek.top/gtcyrvhcrp.html

Go:   err.Error()
来源：http://hz.gaohongyu789.top/gtvfgpgcls.html

Ruby: e.message;  e.backtrace
来源：http://hz.sysykeji.top/gtedpemude.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhoulong.xyz/gtsdglslnh.html

[H09] 带错误码的异常
来源：http://hz.yj20258.top/gtlstehbvg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hysaishi.cn/gtkejsjjnu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.havefunace.top/gtzwsclzss.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.cdnleiting.top/gtvbaerdnn.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.c1oappe.top/gtdlcplnlu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.bjfxy.top/gtfoqimktf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yonumen.top/gtjylmkmbw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ehwqpu.com/gtojtojmqw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.0kj1m.cn/gttuyuqehi.html

[H10] 资源自动释放
来源：http://hz.mhx1999.top/gtlpbxyftz.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zdqjudy.top/gtnjurvvlc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ehwqpu.com/gtlzziauwu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yonumen.top/gtmkmcvety.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sweek.top/gtmhphdrhh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jqgfzy.top/gtqlngdokr.html

Go:   defer f.Close()
来源：http://hz.nwbrower.top/gtvlbbaccv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zdqjudy.top/gtviaomaro.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zhengqikj.top/gtvszqsfla.html

================================================================================
来源：http://hz.zhengqikj.top/gtrpprstdq.html

I. 正则表达式
来源：http://hz.yvedp.cn/gtbrwkkpio.html

================================================================================
来源：http://hz.vqdsnc.cn/gtosrtyyph.html

[I01] 判断是否匹配
来源：http://hz.daxiang520.top/gtpnntmjij.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.0kj1m.cn/gtstmkgwve.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.tian-w.cn/gtbgqyhaaq.html

JS:   /\d+/.test(s)
来源：http://hz.shanyushiyangkeji.top/gtplfeqrev.html

TS:   /\d+/.test(s)
来源：http://hz.havefunace.top/gtxtlvuuur.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yj20258888.top/gtckuargkc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.aizwys.cn/gtemglrsga.html

Ruby: s.match?(/\d+/)
来源：http://hz.gogol.net.cn/gtzanwcsmx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shuidangran.top/gtlwzfeaas.html

[I02] 提取所有匹配
来源：http://hz.chenzaomai.com/gtzxtutfdr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinqigufen.top/gtsuvsjswp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.nwbrower.top/gtsfjdwilv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yueranfly.top/gtrzycyhez.html

TS:   s.match(/\d+/g)
来源：http://hz.0kj1m.cn/gtturfpsmm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hywenlv.cn/gtxejtmhry.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.tian-w.cn/gtagmihaex.html

Ruby: s.scan(/\d+/)
来源：http://hz.hnqzz.top/gtlufybnsw.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yonumen.top/gtpscmluoj.html

[I03] 提取捕获分组
来源：http://hz.cheryme.top/gtkdignahd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hfpthk.cn/gtfueftbhj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jinghuilouyu.cn/gtgycbycpk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jianghu66.top/gtukizwefh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.svipenyu.cn/gtojycdkuc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shanyushiyangkeji.top/gtnqlyalds.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.vqdsnc.cn/gtnjhuitea.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.tianlin.xyz/gtulkojztr.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.daria6918.cn/gtkfbqddxo.html

[I04] 正则替换
来源：http://hz.9152youxi.cn/gtlekbwxwl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.feifeiyinyue.top/gtyxexlbmq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gzhubu.top/gtnhmvnwps.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.dianchejie.cn/gtiizzcvdh.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jiagoushi.top/gtauiudqdy.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.cashguo.top/gtmpwysufb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhongyouzk.top/gtnfbnqybw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.aibaodan.cn/gtkdzflrnd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhixingplan.top/gtjuraawwv.html

[I05] 按正则拆分
来源：http://hz.wangshuangyany.cn/gtozmpsceq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jlsjyb.cn/gtvxqvvudw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.svipenyu.cn/gtzkjqqlzl.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.c1oappe.top/gtmhtzrkss.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.dianchejie.cn/gtoddcwxsz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zdqjudy.top/gtzrliszpf.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xinyue.icu/gtpgmbcizz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.dashuyun.cn/gtffkejwva.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.daxiang520.top/gtucdinkhy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.gotoacloud.top/gtbldwruhx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinghuilouyu.cn/gtmkairfkg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shangyingyoupin.top/gtqpwargwe.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangdashe.top/gtuaynhqoa.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hongshengwenyu.top/gtbnrdhpbt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.kuanghao11.cn/gtrcaagaiy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jinyuanbaomall.cn/gtdmfroqte.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.daria6918.cn/gtidmrlywa.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xinyue.icu/gtqblxysdv.html

[I07] 忽略大小写与多行模式
来源：http://hz.c1oappe.top/gtlubopgpl.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhaomingkeji.xyz/gtoddenlrr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.sufxvd.cn/gtujlmlpbd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.nwbrower.top/gtatffhpwh.html

TS:   /error/gim
来源：http://hz.fzhhl.top/gtbmwfvbsr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ywan-chungtsiang.top/gtxydviynf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jlsjyb.cn/gtyhookkda.html

Ruby: s.scan(/error/i)
来源：http://hz.jiagoushi.top/gtlafyerhc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.fengsongda.top/gtubuwpwhp.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.wangdashe.top/gthaaaleeb.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.guannengcc.top/gthtxmrowj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.pengpengdd.cyou/gtqbkeztbx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.vqdsnc.cn/gthdbzqszb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yangfankeji.com/gtubytsbcw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.9152youxi.cn/gtlsvswvdg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shangyingyoupin.top/gtztvyehcc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.haohaochexian.top/gtgokyajer.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.wangdashe.top/gtmtmtykqs.html

================================================================================
来源：http://hz.gogol.net.cn/gthenvvoma.html

J. 日期与时间
来源：http://hz.ydjk.org.cn/gtbxrsmkzb.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtdsfhuepv.html

[J01] 获取当前时间
来源：http://hz.vqdsnc.cn/gtuatsjmsn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.dianchejie.cn/gtckqtpwyp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yonumen.top/gtmdeuyvya.html

JS:   new Date();  Date.now()
来源：http://hz.ivvv.top/gtiwwkharw.html

TS:   new Date();  Date.now()
来源：http://hz.wangdashe.top/gtiozobguo.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shuidangran.top/gtfiekklud.html

Go:   time.Now()
来源：http://hz.jiagoushi.top/gtaunqzpni.html

Ruby: Time.now
来源：http://hz.svipenyu.cn/gtjrdibbvd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.haohaochexian.top/gtqfkpyxgi.html

[J02] 格式化输出
来源：http://hz.shangyingyoupin.top/gtafebetjc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.52xcode.cn/gtxmufrlgc.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ywan-chungtsiang.top/gtbqccajnx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gogol.net.cn/gtfzmgokkc.html

TS:   d.toISOString()
来源：http://hz.yuanzhike.top/gtjmxmqnau.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.chenjidiqi.icu/gtrrwqhyea.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xinyue.icu/gtrzvlxtdr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yuxming.cn/gtnpfglrfl.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xuetiantiany.cn/gtpiyhkjkf.html

[J03] 字符串解析为日期
来源：http://hz.zhixingplan.top/gtuocjhqcv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zdqjudy.top/gtgcaajexm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ivvv.top/gtmrfequwi.html

JS:   new Date("2024-01-02")
来源：http://hz.yuanzhike.top/gthpwbjhvo.html

TS:   new Date("2024-01-02")
来源：http://hz.dashuyun.cn/gthcuwciaf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.tianlin.xyz/gthlpfcywp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ybcxt.top/gtoidgitrx.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yangfankeji.com/gtmcbmvivs.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nanxinkj.top/gtieilgpnd.html

[J04] 时间戳与日期互转
来源：http://hz.xylfe.cn/gttcofbhjw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.quarkkingdee.top/gttoabxyno.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.vqdsnc.cn/gtwqwhmhip.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zdqjudy.top/gtxxcczxpv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.aibaodan.cn/gtvlwsgjxu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.0kj1m.cn/gtkletrztw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhoulong.xyz/gteusgrmwl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.0kj1m.cn/gtanbqckdl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.sysykeji.top/gtaiytruvy.html

[J05] 时间加减（加 7 天）
来源：http://hz.shangyingyoupin.top/gtnqsvcnqs.html

Py:   now + timedelta(days=7)
来源：http://hz.chenlongwang.top/gtlyygqvdx.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.vqdsnc.cn/gtuketnshu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ydzc1.top/gtwzvtdaau.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.haohaochexian.top/gtkcmtorsn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.snrcjt.cn/gtghmubmgk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.tanke756.top/gtqrskwiie.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gaohongyu789.top/gtcunjgzgm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xuanzx.com/gtplhcqgoa.html

[J06] 计算两时间之差
来源：http://hz.yanxiufei.cn/gtxkmbvkqx.html

Py:   (end - start).total_seconds()
来源：http://hz.snrcjt.cn/gtoptrwgsw.html

PHP:  $end->diff($start)->days;
来源：http://hz.cheryme.top/gtzptrdwwl.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.gogol.net.cn/gtmjreqgxp.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.chenlongwang.top/gtildqpqix.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhiwuduotai.top/gtiyasbloz.html

Go:   end.Sub(start).Hours()
来源：http://hz.xinyue.icu/gtiorinvrt.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ybcxt.top/gtmkmlyifd.html

C#:   (end - start).TotalSeconds
来源：http://hz.xuanzx.com/gtsguubloa.html

[J07] 比较两个日期
来源：http://hz.ppjwa.cn/gtqfvicuzs.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ivvv.top/gtjgkbhcep.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xylfe.cn/gthmyfkhnb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cdnleiting.top/gtfunxkhou.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhaomingkeji.xyz/gtcmdjimgw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.kuanghao11.cn/gtunacpjxc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhengqikj.top/gtdzsxczti.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xylfe.cn/gtqdyvqwhy.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.0kj1m.cn/gtwrgywvao.html

[J08] 提取年月日与星期
来源：http://hz.jqgfzy.top/gtzrimggja.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.kuanghao11.cn/gtepwyoofa.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinyuanbaomall.cn/gtdzmwmjhe.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.meibo888.top/gtoiksyvgo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shzxlz.cn/gtrldlegcm.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cqqwz.cn/gtbtnyrzdo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.fengsongda.top/gtwoqtgdgf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.316326.xyz/gtjvhzdxld.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gaohongyu789.top/gtgpwzshnz.html

[J09] 时区处理
来源：http://hz.hnqzz.top/gtdyfiauni.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xuetiantiany.cn/gtzzjsjmro.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yangfankeji.com/gtipgdxvao.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shzxlz.cn/gtntieupzd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj202588.top/gtmcpmqdah.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.shangyingyoupin.top/gtxokfefxt.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hnxiangtu.top/gtpxsjnkfu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.nanxinkj.top/gtlzkggbnt.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xylfe.cn/gtiajikjkz.html

[J10] 取今天 / 本月第一天
来源：http://hz.svipenyu.cn/gtnnnqgexf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ehwqpu.com/gtrubipimc.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.iojbl.cn/gtyqkjrvmn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.gogol.net.cn/gtkbuuaxpx.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhaomingkeji.xyz/gtawrizixb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.fengsongda.top/gtnedyvdnj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yanxiufei.cn/gtwabwnuym.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xziqi.cn/gtuspdnxxs.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yongpay.top/gtkvpjqywr.html

================================================================================
来源：http://hz.ydzc1.top/gtqclubotg.html

K. JSON 与序列化
来源：http://hz.smart0.xyz/gtohubuzlu.html

================================================================================
来源：http://hz.9152youxi.cn/gtgjlymrvx.html

[K01] 对象转 JSON 字符串
来源：http://hz.hammf.cn/gtemypasyj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.tanke756.top/gtntsalcru.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.bjfxy.top/gtbfhtqcys.html

JS:   JSON.stringify(obj)
来源：http://hz.ivvv.top/gtekphifvz.html

TS:   JSON.stringify(obj)
来源：http://hz.gotoacloud.top/gtbrdbsaoe.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hfpthk.cn/gtdttcwjrf.html

Go:   json.Marshal(obj)
来源：http://hz.ydzc1.top/gttgxktpgr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ehwqpu.com/gtjthxompm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ehwqpu.com/gtfwzlsete.html

[K02] JSON 字符串转对象
来源：http://hz.pengpengdd.cyou/gtqdlntsuv.html

Py:   json.loads(s)
来源：http://hz.jianghu66.top/gtsgjcmtfn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.nwbrower.top/gtyrzgzsaw.html

JS:   JSON.parse(s)
来源：http://hz.zhixingplan.top/gtowiyqdnw.html

TS:   JSON.parse(s)
来源：http://hz.dianchejie.cn/gtvatwjlzq.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jqgfzy.top/gtruummeql.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.yj202588.top/gtpubypjfe.html

Ruby: JSON.parse(s)
来源：http://hz.ehwqpu.com/gtbkofttfm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.smart0.xyz/gtvsmfsxka.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.52xcode.cn/gtljpziwnx.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhiwuduotai.top/gtvnphxmjz.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ppjwa.cn/gtetmwcjyv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.cdnleiting.top/gtqzjgnpfn.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.iojbl.cn/gtidrmlyje.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.cqqwz.cn/gtuizejwub.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.wangshuangyany.cn/gtdjqztgnp.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.tianlin.xyz/gttnwcdiro.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yongpay.top/gtzpibyhfo.html

[K04] 读取 JSON 文件
来源：http://hz.zhiwuduotai.top/gtzjzvlgpi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.chenjidiqi.icu/gtduauhbey.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.ydjk.org.cn/gtqptxgqic.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.cdnleiting.top/gtsdezgpzm.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.pycfn.com/gtcohkoisb.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.ehwqpu.com/gtxlrcubfk.html


<!-- 参考信息 -->