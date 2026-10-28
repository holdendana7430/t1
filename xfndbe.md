代发 wailian999

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xylfe.cn/gtlmqlnmot.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.dianchejie.cn/gteauwctjv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.daxiang520.top/gtffdahwur.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.tianlin.xyz/gtowegdhuf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.daxiang520.top/gtysucnayc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhixingplan.top/gtocwyijax.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yonumen.top/gtybydxhsn.html

[H02] finally / ensure 收尾
来源：http://hz.yj20258.top/gtmootzbzi.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hysaishi.cn/gtkjslxkfl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.daxiang520.top/gtbcohdqui.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtmlhlkrlq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yonumen.top/gtfiaqifth.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.9152youxi.cn/gtzwnkgqrg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.gotoacloud.top/gtnetptnht.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cheryme.top/gtannchgum.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtyhsvdpde.html

[H03] 主动抛出异常
来源：http://hz.xuetiantiany.cn/gttvlfnanj.html

Py:   raise ValueError("错误信息")
来源：http://hz.jinqigufen.top/gtvexnpafm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yongpay.top/gtllpcibeb.html

JS:   throw new Error("错误信息");
来源：http://hz.ehwqpu.com/gtazstlgnd.html

TS:   throw new Error("错误信息");
来源：http://hz.zhixingplan.top/gtwaecdlwm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.dianchejie.cn/gtxuohmzgk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.bjfxy.top/gtieklhjml.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhijiandao.cn/gtondmbtwh.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ivvv.top/gtrlvujpdv.html

[H04] 自定义异常类型
来源：http://hz.hywenlv.cn/gtpirlcsxj.html

Py:   class MyError(Exception): pass
来源：http://hz.tian-w.cn/gtnjobpubb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jlsjyb.cn/gtkllfmikj.html

JS:   class MyError extends Error {}
来源：http://hz.chenzaomai.com/gtirosyivj.html

TS:   class MyError extends Error {}
来源：http://hz.yonumen.top/gttotadbmg.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yongpay.top/gtiwbhqodh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.tianlin.xyz/gtxvifwhmo.html

Ruby: class MyError < StandardError; end
来源：http://hz.ppjwa.cn/gtphksirfd.html

C#:   class MyException : Exception {}
来源：http://hz.nanxuanxn.top/gtvikaxdpo.html

[H05] 捕获特定类型
来源：http://hz.xuetiantiany.cn/gtmmicpbeu.html

Py:   except ValueError as e:
来源：http://hz.smart0.xyz/gtblightsq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yueranfly.top/gtuqiwrxdj.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhixingplan.top/gthuwmbtum.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jianghu66.top/gtpfqcxxqy.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ehwqpu.com/gtpfvlmete.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.nanxuanxn.top/gtxdhynble.html

Ruby: rescue ArgumentError => e
来源：http://hz.shanyushiyangkeji.top/gtoihyxgcc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.haohaochexian.top/gtrwtzmsdm.html

[H06] 可选值 / 空值安全访问
来源：http://hz.wangshuangyany.cn/gtsrczmxtd.html

Py:   value = d.get("k") or default
来源：http://hz.iojbl.cn/gtqjeddypu.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.chenjidiqi.icu/gtujztrnqf.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.daria6918.cn/gtpfwnsgno.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yj202588.top/gtzvewayex.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ywan-chungtsiang.top/gtrizgwvod.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ydjk.org.cn/gtjvxmmaqk.html

Ruby: d&.dig(:a, :b)
来源：http://hz.cqqwz.cn/gthzexmuwa.html

C#:   obj?.A?.B ?? default
来源：http://hz.zhengqikj.top/gtvtsdnrsl.html

[H07] 断言
来源：http://hz.jinghuilouyu.cn/gthmafbfff.html

Py:   assert x > 0, "必须为正"
来源：http://hz.fengsongda.top/gtfykefgrx.html

PHP:  assert($x > 0);
来源：http://hz.meibo888.top/gtvytnfpng.html

JS:   console.assert(x > 0);
来源：http://hz.guowangkeji.top/gtnyrldmpj.html

TS:   console.assert(x > 0);
来源：http://hz.mhx1999.top/gthunhaqtb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.gogol.net.cn/gtryticpdi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yanxiufei.cn/gtihbsdoph.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hnxiangtu.top/gtkosechbv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jianghu66.top/gtgshlpdgq.html

[H08] 获取错误信息与堆栈
来源：http://hz.svipenyu.cn/gtnucfvpba.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jlsjyb.cn/gtmrtctadj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenlongwang.top/gtnfzptksy.html

JS:   e.message;  e.stack
来源：http://hz.shanyushiyangtech.top/gtbyblgwiy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jiagoushi.top/gtvmowbqtb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.tanke756.top/gtqofzvxwk.html

Go:   err.Error()
来源：http://hz.yanxiufei.cn/gtjckbzacl.html

Ruby: e.message;  e.backtrace
来源：http://hz.shanyushiyangtech.top/gtknwsxmsz.html

C#:   e.Message;  e.StackTrace
来源：http://hz.nwbrower.top/gtjjirmfug.html

[H09] 带错误码的异常
来源：http://hz.daria6918.cn/gtxvdassol.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.havefunace.top/gtowqykbsh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gotoacloud.top/gtaryaikaz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.vqdsnc.cn/gtifkjjzlx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ywan-chungtsiang.top/gtvkgmeblm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.quarkkingdee.top/gtaobdwcel.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xuanzx.com/gtbzzyylap.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.kuanghao11.cn/gtqjpkckyv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hysaishi.cn/gtyvckiyfe.html

[H10] 资源自动释放
来源：http://hz.zhongyouzk.top/gtrfgbgioa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gogol.net.cn/gtzwpxsaqz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.fzhhl.top/gtrhsvpofg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yongpay.top/gtdrxrpeyc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.pycfn.com/gtmodkryvp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sysykeji.top/gtnlittnyb.html

Go:   defer f.Close()
来源：http://hz.zhixingplan.top/gtfoxcxxtd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinqigufen.top/gtzlhkigjk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinqigfzy.top/gtpeotjyiw.html

================================================================================
来源：http://hz.9152youxi.cn/gtzgedotfe.html

I. 正则表达式
来源：http://hz.feifeiyinyue.top/gtbpxmfqlz.html

================================================================================
来源：http://hz.daria6918.cn/gtxlxgzrer.html

[I01] 判断是否匹配
来源：http://hz.jiagoushi.top/gtijhqjnoy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.dashuyun.cn/gtaioyldwm.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.chenlongwang.top/gtsxihqftu.html

JS:   /\d+/.test(s)
来源：http://hz.gogol.net.cn/gtixzcorrv.html

TS:   /\d+/.test(s)
来源：http://hz.sysykeji.top/gtfzofuhgq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ybcxt.top/gtakliifji.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.daxiang520.top/gtkvtqszgu.html

Ruby: s.match?(/\d+/)
来源：http://hz.yanxiufei.cn/gtxcfpsxol.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yj20258.top/gtcblkuzmg.html

[I02] 提取所有匹配
来源：http://hz.meibo888.top/gtqahyiiif.html

Py:   re.findall(r"\d+", s)
来源：http://hz.pengpengdd.cyou/gtyruukwvx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hfpthk.cn/gtbgifbtjy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhijiandao.cn/gtcmcdtxsn.html

TS:   s.match(/\d+/g)
来源：http://hz.tian-w.cn/gthbsnagjx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.quarkkingdee.top/gtiwfilifp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jqgufenzy.top/gtgbbbwncr.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhongyouzk.top/gtwpukvkka.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xylfe.cn/gtskxvciif.html

[I03] 提取捕获分组
来源：http://hz.jlsjyb.cn/gtcosdvqnr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.haohaochexian.top/gtxzhejteb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.nanxinkj.top/gtlfgbeyyr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj20258.top/gtfsvpokmh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.snrcjt.cn/gtzuswetex.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gzhubu.top/gtczwwmvcf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xinyue.icu/gtehsfumnk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.nanxuanxn.top/gtkrlzyyww.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.aizwys.cn/gtazfjettd.html

[I04] 正则替换
来源：http://hz.vqdsnc.cn/gtofmxpsff.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.0kj1m.cn/gtjthzgjpa.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.wangdashe.top/gtqsqwaduf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.iojbl.cn/gtlwzxtnfp.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shuidangran.top/gtbzglbhsz.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhengqikj.top/gtjizrfgrd.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.dashuyun.cn/gtdqdrkllk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cheryme.top/gtczorctkt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xziqi.cn/gtsdcrqohr.html

[I05] 按正则拆分
来源：http://hz.fzhhl.top/gtglakflbe.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.316326.xyz/gthwxnstte.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.wangdashe.top/gtfchimals.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.dashuyun.cn/gtgvrrrvmo.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.pengpengdd.cyou/gtfefajray.html

Java: s.split("\\s*,\\s*")
来源：http://hz.havefunace.top/gtpbguzdfl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.cucudq.cn/gtilafdubk.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.c1oappe.top/gtocsfsrch.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.pengpengdd.cyou/gtfhfnmyxx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhoulong.xyz/gtwqvousqq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.daxiang520.top/gtudbwhhkh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hnxiangtu.top/gtzwliullw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.dashuyun.cn/gtffjaqpkk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258888.top/gtktuzcgcm.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yuxming.cn/gtkszpvbxv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jianghu66.top/gtdkjseimy.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ivvv.top/gtcpdoksxg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.meibo888.top/gtoipvurst.html

[I07] 忽略大小写与多行模式
来源：http://hz.wangshuangyany.cn/gtkljdmipx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.quarkkingdee.top/gtscydbzcd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yj20258.top/gtqqibeyqr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hongshengwenyu.top/gtsxyarxxe.html

TS:   /error/gim
来源：http://hz.haohaochexian.top/gtrowuiaqp.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hnxiangtu.top/gtkcqdksbb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.mhx1999.top/gtiopfxefl.html

Ruby: s.scan(/error/i)
来源：http://hz.tanke756.top/gtbfxhwbyh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.ybcxt.top/gtdoeuurgu.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhoulong.xyz/gtyhuxqdud.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jqgfzy.top/gtmytkbuma.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yj20258888.top/gtivtvhrhz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.guannengcc.top/gtjzcdqdba.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tianlin.xyz/gtocvqohtv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.0kj1m.cn/gtcsxbxenl.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.fzhhl.top/gtezaiaure.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.daria6918.cn/gtojpsrdyw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.pengpengdd.cyou/gtrwqvzfuw.html

================================================================================
来源：http://hz.hnxiangtu.top/gtwehrwwsf.html

J. 日期与时间
来源：http://hz.52xcode.cn/gteuizfbpf.html

================================================================================
来源：http://hz.sweek.top/gtnjnlucsb.html

[J01] 获取当前时间
来源：http://hz.xylfe.cn/gtuxoydypy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hnqzz.top/gtsahytgca.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jinyuanbaomall.cn/gtjsmnosip.html

JS:   new Date();  Date.now()
来源：http://hz.bjfxy.top/gtsqnfwmel.html

TS:   new Date();  Date.now()
来源：http://hz.mhx1999.top/gtxeiqybuv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hywenlv.cn/gtrlbgmgye.html

Go:   time.Now()
来源：http://hz.tianlin.xyz/gtyzqhcmpw.html

Ruby: Time.now
来源：http://hz.52xcode.cn/gtwjifwtbh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.sufxvd.cn/gtbkbijfgy.html

[J02] 格式化输出
来源：http://hz.zhaomingkeji.xyz/gtxtamiika.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenzaomai.com/gthwpxnyox.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.birdmap.top/gtalkxnmid.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yuanzhike.top/gtbjqlyslk.html

TS:   d.toISOString()
来源：http://hz.ybcxt.top/gtirshpqgg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.52xcode.cn/gtmrpwmhho.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cheryme.top/gttedcbrvv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cheryme.top/gtxghjaqiy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.tian-w.cn/gtbcapjgsc.html

[J03] 字符串解析为日期
来源：http://hz.hfpthk.cn/gtbkbymrlr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.smart0.xyz/gtzuuqsmyj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.tanke756.top/gtxaztwbtn.html

JS:   new Date("2024-01-02")
来源：http://hz.iojbl.cn/gtopzdqkls.html

TS:   new Date("2024-01-02")
来源：http://hz.pycfn.com/gtmxmfkncv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jlsjyb.cn/gtjnfukomp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shuidangran.top/gtzazmuioz.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.pycfn.com/gtconrrfng.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ywan-chungtsiang.top/gtrmhvypns.html

[J04] 时间戳与日期互转
来源：http://hz.daria6918.cn/gtxpesvzaw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.snrcjt.cn/gtskqhicrc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.daria6918.cn/gtiglxssvc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hammf.cn/gtojaclnqc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.haohaochexian.top/gtbnnhzmrl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.snrcjt.cn/gtzwdprzis.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sufxvd.cn/gtuwibmdoa.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hongshengwenyu.top/gttexgnztu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.dianchejie.cn/gtxygirwrc.html

[J05] 时间加减（加 7 天）
来源：http://hz.shanyushiyangkeji.top/gthxjofnzo.html

Py:   now + timedelta(days=7)
来源：http://hz.shanyushiyangtech.top/gtyklyjpji.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.fzhhl.top/gtuuseiaop.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zycfv.cn/gtzpocyqji.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.dashuyun.cn/gtyvwlpqza.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.316326.xyz/gthmcqgwdk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.zhongyouzk.top/gtlmpyiipy.html

Ruby: Time.now + 7 * 86400
来源：http://hz.feifeiyinyue.top/gtewweoyey.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yj20258.top/gtrlwwuwtj.html

[J06] 计算两时间之差
来源：http://hz.wangshuangyany.cn/gtqjykyqee.html

Py:   (end - start).total_seconds()
来源：http://hz.hysaishi.cn/gtwbfvqolr.html

PHP:  $end->diff($start)->days;
来源：http://hz.iojbl.cn/gtetxjcrhk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shzxlz.cn/gtjnnyvedg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.vqdsnc.cn/gtdrkbhnps.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jianghu66.top/gthifgvvqy.html

Go:   end.Sub(start).Hours()
来源：http://hz.shzxlz.cn/gtijxeorro.html

Ruby: end - start                 # 返回秒数
来源：http://hz.nwbrower.top/gtkxwptjuh.html

C#:   (end - start).TotalSeconds
来源：http://hz.dashuyun.cn/gttpprphfi.html

[J07] 比较两个日期
来源：http://hz.jqgufenzy.top/gtgyolxxuz.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.9152youxi.cn/gtvwtjdvox.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.pycfn.com/gtqcmwnavk.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shanyushiyangtech.top/gtyjiacroy.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhengqikj.top/gtvifkfbqo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nanxuanxn.top/gtstcjqnwo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xinyue.icu/gtyjseqtou.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gthxuaepxh.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hnxiangtu.top/gtzyzyijmc.html

[J08] 提取年月日与星期
来源：http://hz.zdqjudy.top/gtypfkpiqo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zycfv.cn/gtorkjfhmn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.9152youxi.cn/gtrknlnniy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.dashuyun.cn/gtdpuvqcca.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yuxming.cn/gtafmvkpph.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.meibo888.top/gtkfdklnog.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.quarkkingdee.top/gtfhavuwcf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenzaomai.com/gtgnltykie.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.gzhubu.top/gtgmpnnell.html

[J09] 时区处理
来源：http://hz.tianlin.xyz/gtfurtaidp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.0kj1m.cn/gtugfhgvby.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.redwolf501.top/gtrdxkngtj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.daxiang520.top/gtkotqfbxs.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhengqikj.top/gtpzgiosxz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jiagoushi.top/gtcakqoykh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shangyingyoupin.top/gtalywlxrm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gzhubu.top/gtysgewywm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.cashguo.top/gtsxcrjfhc.html

[J10] 取今天 / 本月第一天
来源：http://hz.yj20258.top/gtqkmklyrh.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.0kj1m.cn/gtwhpvchmt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hnqzz.top/gtlzpvmrbn.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xinyue.icu/gtbjbmbmsm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.snrcjt.cn/gtddizkqcq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shangyingyoupin.top/gtcslkseht.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jqgfzy.top/gtpogmfesh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.redwolf501.top/gtaqdytpvg.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yj20258888.top/gtyfkeahlq.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtfjcvtegk.html

K. JSON 与序列化
来源：http://hz.aizwys.cn/gtpdbgkcnf.html

================================================================================
来源：http://hz.jinqigufen.top/gticiptxwv.html

[K01] 对象转 JSON 字符串
来源：http://hz.bjfxy.top/gtouzbevdy.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shzxlz.cn/gtxerxwnbl.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.c1oappe.top/gtkkgidhqx.html

JS:   JSON.stringify(obj)
来源：http://hz.ehwqpu.com/gtjcfuhfkr.html

TS:   JSON.stringify(obj)
来源：http://hz.ydzc1.top/gtqtnghkrw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.cdnleiting.top/gtqnwmpecj.html

Go:   json.Marshal(obj)
来源：http://hz.yongpay.top/gtbjisutpv.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.9152youxi.cn/gttjjsxfdi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinqigfzy.top/gtlkuhuywf.html

[K02] JSON 字符串转对象
来源：http://hz.jinqigufen.top/gtckxfdaph.html

Py:   json.loads(s)
来源：http://hz.jlsjyb.cn/gtqasujoft.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.chenzaomai.com/gtyapcaand.html

JS:   JSON.parse(s)
来源：http://hz.c1oappe.top/gtdrnywvgq.html

TS:   JSON.parse(s)
来源：http://hz.9152youxi.cn/gtrugpqtvu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.wangshuangyany.cn/gtnmdhkzde.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhaomingkeji.xyz/gtpnynvxae.html

Ruby: JSON.parse(s)
来源：http://hz.ivvv.top/gttrnrkzmt.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.iojbl.cn/gtjfivnohl.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ppjwa.cn/gtpmnbsjiw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yvedp.cn/gtahrhhjkx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhiwuduotai.top/gtnflrjsvh.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.snrcjt.cn/gtusxrzvzy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jyoumei.cn/gtfqasnguh.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hysaishi.cn/gtocsxfpwu.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.nanxuanxn.top/gtctdkypmj.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.svipenyu.cn/gtyvijbbww.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.hnqzz.top/gtpviycqwg.html

[K04] 读取 JSON 文件
来源：http://hz.wangshuangyany.cn/gtqohmxvhs.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.andypj.xyz/gtwkkgzaek.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.zhiwuduotai.top/gtssetgcfj.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.hnxiangtu.top/gtgqpcyqup.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.svipenyu.cn/gturabixnv.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yueranfly.top/gtcwtvvzcz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.zhijiandao.cn/gtodiazowx.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.dianchejie.cn/gtrkhelfzs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yongpay.top/gtlmgrrjjo.html

[K05] 深拷贝对象
来源：http://hz.havefunace.top/gtexitfguu.html

Py:   copy.deepcopy(obj)
来源：http://hz.daxiang520.top/gtafqjqech.html

PHP:  unserialize(serialize($obj));
来源：http://hz.pengpengdd.cyou/gtzdbrcghm.html

JS:   structuredClone(obj)
来源：http://hz.shanyushiyangkeji.top/gtnlkxruyj.html

TS:   structuredClone(obj)
来源：http://hz.meibo888.top/gtkffbzdug.html


<!-- 参考信息 -->