代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.feifeiyinyue.top/gtqylykbdx.html

Ruby: obj.instance_variables
来源：http://hz.kuanghao11.cn/gtqejcohrs.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.fengsongda.top/gtbrunsnge.html

================================================================================
来源：http://hz.shzxlz.cn/gtlrhmowtw.html

H. 异常与错误处理
来源：http://hz.zhoulong.xyz/gtmifdvwkl.html

================================================================================
来源：http://hz.iojbl.cn/gtavdpzgqv.html

[H01] try / catch 基础
来源：http://hz.yuanzhike.top/gtdlfrdabj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.cheryme.top/gtehizzhyd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xylfe.cn/gtxlxpadal.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yj20258.top/gtmdsnmrbz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xylfe.cn/gtfmmgyxij.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cdnleiting.top/gttsvdoobz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.shangyingyoupin.top/gtylfzlhaq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yuxming.cn/gtusxkbufz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.svipenyu.cn/gtgaitanju.html

[H02] finally / ensure 收尾
来源：http://hz.tanke756.top/gtwbbxwvch.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.chenlongwang.top/gtlahonzpa.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtjyklzkll.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shzxlz.cn/gttpuyrpdr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtvmtrnhrr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.0kj1m.cn/gtbhncdydl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.svipenyu.cn/gtvolsqyyt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zycfv.cn/gtkvnepeeg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.aizwys.cn/gttwxbwcyy.html

[H03] 主动抛出异常
来源：http://hz.gotoacloud.top/gtiwprannj.html

Py:   raise ValueError("错误信息")
来源：http://hz.xingfuxueyuan.xyz/gtanmotkwo.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xinyue.icu/gtddjcdczl.html

JS:   throw new Error("错误信息");
来源：http://hz.gotoacloud.top/gtqstwqfpe.html

TS:   throw new Error("错误信息");
来源：http://hz.yj20258888.top/gtmadcubgm.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yuxming.cn/gtlileacfb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jiagoushi.top/gtpyrxqmpm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.gogol.net.cn/gtdlkdwoeu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.hnxiangtu.top/gtoapnitbj.html

[H04] 自定义异常类型
来源：http://hz.jinqigfzy.top/gttlijqufm.html

Py:   class MyError(Exception): pass
来源：http://hz.ybcxt.top/gtapxnjrpj.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.52xcode.cn/gtcqgcakrj.html

JS:   class MyError extends Error {}
来源：http://hz.gotoacloud.top/gtnscrunqx.html

TS:   class MyError extends Error {}
来源：http://hz.zhiwuduotai.top/gthegwthbm.html

Java: class MyException extends RuntimeException {}
来源：http://hz.tian-w.cn/gtphewcpap.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zhongyouzk.top/gtypyupalg.html

Ruby: class MyError < StandardError; end
来源：http://hz.nanxuanxn.top/gtzwqtsbfe.html

C#:   class MyException : Exception {}
来源：http://hz.kuanghao11.cn/gtzwrscftc.html

[H05] 捕获特定类型
来源：http://hz.sweek.top/gtdtejgpli.html

Py:   except ValueError as e:
来源：http://hz.xziqi.cn/gtrqfcbmji.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ybcxt.top/gtwqktnknz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yj20258888.top/gtamjzqjjp.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.guannengcc.top/gtzxsuwadk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yj20258.top/gttxlsbkfb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.aibaodan.cn/gtgxcomysb.html

Ruby: rescue ArgumentError => e
来源：http://hz.guowangkeji.top/gtmqtxevks.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jqgfzy.top/gtnskcreqr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.daxiang520.top/gttacwzuvd.html

Py:   value = d.get("k") or default
来源：http://hz.yuanzhike.top/gttbhsikce.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.fengsongda.top/gtfaxnkjap.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.c1oappe.top/gtlygqptkx.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.aizwys.cn/gtxmlgsawg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.daria6918.cn/gtdgltfhsu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jinghuilouyu.cn/gtteuzirqu.html

Ruby: d&.dig(:a, :b)
来源：http://hz.chenjidiqi.icu/gtlpehecza.html

C#:   obj?.A?.B ?? default
来源：http://hz.xuetiantiany.cn/gtdedqidem.html

[H07] 断言
来源：http://hz.xuetiantiany.cn/gteeauwote.html

Py:   assert x > 0, "必须为正"
来源：http://hz.bjfxy.top/gthpruyslh.html

PHP:  assert($x > 0);
来源：http://hz.yj20258.top/gtuoxnyrmn.html

JS:   console.assert(x > 0);
来源：http://hz.vqdsnc.cn/gtgjetkttv.html

TS:   console.assert(x > 0);
来源：http://hz.daxiang520.top/gtkqozmxwd.html

Java: assert x > 0 : "必须为正";
来源：http://hz.gaohongyu789.top/gtkgcngkuo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yueranfly.top/gtadgljafz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.cucudq.cn/gtxodeyrmh.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hongshengwenyu.top/gtsrvyzqqw.html

[H08] 获取错误信息与堆栈
来源：http://hz.snrcjt.cn/gtxhggpuaz.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.andypj.xyz/gtlcyqcxtz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gotoacloud.top/gthrbxqsno.html

JS:   e.message;  e.stack
来源：http://hz.cqqwz.cn/gtkaqhircj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinqigfzy.top/gtvnbykdsl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.dashuyun.cn/gtrqkxtxyh.html

Go:   err.Error()
来源：http://hz.daxiang520.top/gtfwabzveq.html

Ruby: e.message;  e.backtrace
来源：http://hz.tian-w.cn/gtuzbcjqdv.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tian-w.cn/gtmofdkpgq.html

[H09] 带错误码的异常
来源：http://hz.aizwys.cn/gtdnmincgm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.9152youxi.cn/gtcmztcjhe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shanyushiyangtech.top/gtmltecxzd.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.quarkkingdee.top/gtkepswlla.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.svipenyu.cn/gttvbiqrkf.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.shanyushiyangkeji.top/gthygyimji.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.aizwys.cn/gtmfspcnxz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.guowangkeji.top/gtmzobksut.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.snrcjt.cn/gtmwarfzbt.html

[H10] 资源自动释放
来源：http://hz.andypj.xyz/gtmbubfhwt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.chenzaomai.com/gtqtjstmdl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ybcxt.top/gtceyojxly.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jiagoushi.top/gtebcrqwka.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ybcxt.top/gtvglryyix.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.iojbl.cn/gtaojtzavk.html

Go:   defer f.Close()
来源：http://hz.zhiwuduotai.top/gthmypzlij.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yongpay.top/gtuqgegywj.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.pengpengdd.cyou/gtgoopdahl.html

================================================================================
来源：http://hz.0kj1m.cn/gtlfpclokk.html

I. 正则表达式
来源：http://hz.shanyushiyangtech.top/gtcuuurkud.html

================================================================================
来源：http://hz.gzhubu.top/gtehzgejvz.html

[I01] 判断是否匹配
来源：http://hz.ywan-chungtsiang.top/gtwvuszumj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yvedp.cn/gtszigyxou.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ppjwa.cn/gtpvdatgkt.html

JS:   /\d+/.test(s)
来源：http://hz.guowangkeji.top/gtsykknlby.html

TS:   /\d+/.test(s)
来源：http://hz.nwbrower.top/gtzikwwenp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.chenlongwang.top/gtkvscjsci.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.nanxinkj.top/gtcbmjwhtd.html

Ruby: s.match?(/\d+/)
来源：http://hz.yongpay.top/gtloxyzmgk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.aibaodan.cn/gtrwvtpsni.html

[I02] 提取所有匹配
来源：http://hz.yuxming.cn/gtaczwyabc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.cqqwz.cn/gtcmffyhdi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jqgfzy.top/gtdqgsnknr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zycfv.cn/gtditzefsn.html

TS:   s.match(/\d+/g)
来源：http://hz.dashuyun.cn/gtccipxtie.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yangfankeji.com/gtbpyulmpd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.dashuyun.cn/gtqrdmnlzm.html

Ruby: s.scan(/\d+/)
来源：http://hz.nanxinkj.top/gtpdrzcjdg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ehwqpu.com/gtcnasxnzb.html

[I03] 提取捕获分组
来源：http://hz.yj202588.top/gtzuscpnso.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yuanzhike.top/gtdpddfrbs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.quarkkingdee.top/gtlnpywuiq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gogol.net.cn/gtcaxxflpp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.tanke756.top/gtqfsbsdmx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhijiandao.cn/gtasglucha.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj20258.top/gtkamodzne.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.9152youxi.cn/gtioikpgvn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jiagoushi.top/gtjhfughtj.html

[I04] 正则替换
来源：http://hz.meibo888.top/gtzokwvsqu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.0kj1m.cn/gtgfgkwffr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.hfpthk.cn/gtqgktznti.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.sweek.top/gtbodaxhjo.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hnxiangtu.top/gtruznuaxk.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.shanyushiyangtech.top/gtnhgxjkrk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shzxlz.cn/gtcshihetk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shzxlz.cn/gtjmscatty.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.kuanghao11.cn/gtglpnxkmk.html

[I05] 按正则拆分
来源：http://hz.xziqi.cn/gtwfobvdjd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yuanzhike.top/gtuybazobz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shanyushiyangtech.top/gtafaulvac.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cheryme.top/gtzaspzwvc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gttpltxqgd.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cdnleiting.top/gteyvxqkuj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.dianchejie.cn/gtabtykspq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj20258.top/gtgvfpmjrc.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.guowangkeji.top/gtdvisksow.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ppjwa.cn/gtlnlakjvv.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hammf.cn/gtsobwrwhj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jinqigfzy.top/gtfcnwbumr.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fengsongda.top/gtyrgmcptd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258.top/gtywfsuhvl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ivvv.top/gtwtgoljqr.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.wangshuangyany.cn/gtslbcjolz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.sysykeji.top/gtusrzoyqo.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhongyouzk.top/gtgnxlogtj.html

[I07] 忽略大小写与多行模式
来源：http://hz.c1oappe.top/gtfejqvgvv.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.kuanghao11.cn/gtgycogdbm.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ivvv.top/gtxzloqytt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.aizwys.cn/gtcljtyimd.html

TS:   /error/gim
来源：http://hz.nwbrower.top/gtdhalyach.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yonumen.top/gtvqqgqreo.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cqqwz.cn/gtofgjowdi.html

Ruby: s.scan(/error/i)
来源：http://hz.quarkkingdee.top/gtjicfryxl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.chenlongwang.top/gtphxtassz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.vqdsnc.cn/gtiuwdkvzx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.fzhhl.top/gtvbyzsodc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yanxiufei.cn/gtlavhbtxu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.gogol.net.cn/gtpmtowtop.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xingfuxueyuan.xyz/gtibagbppb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.pengpengdd.cyou/gtwwoynzcm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hfpthk.cn/gtuctzmnpa.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yj20258.top/gtylkfcnjm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shzxlz.cn/gtvjaqoxck.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtxvjltvdr.html

J. 日期与时间
来源：http://hz.xziqi.cn/gtcdczujcv.html

================================================================================
来源：http://hz.ivvv.top/gtemmpsbmz.html

[J01] 获取当前时间
来源：http://hz.zhongyouzk.top/gtnmlbdhxa.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.wangdashe.top/gtaanedvzn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sufxvd.cn/gtrqzgytdz.html

JS:   new Date();  Date.now()
来源：http://hz.hammf.cn/gtbvolcnuy.html

TS:   new Date();  Date.now()
来源：http://hz.tianlin.xyz/gtjknxkuzu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gogol.net.cn/gtqiqzpzeq.html

Go:   time.Now()
来源：http://hz.ppjwa.cn/gtoumpdgse.html

Ruby: Time.now
来源：http://hz.yangfankeji.com/gttswufkhm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jqgufenzy.top/gttbxtkwnc.html

[J02] 格式化输出
来源：http://hz.zhixingplan.top/gtzrvylgox.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxuanxn.top/gtxarbwukp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.birdmap.top/gtsyqvhezr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.bjfxy.top/gtoztjqmrh.html

TS:   d.toISOString()
来源：http://hz.dashuyun.cn/gtczuisbox.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.aibaodan.cn/gtsjejdnpy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.redwolf501.top/gtjhlermqv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangdashe.top/gtbtqgplyj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.wangdashe.top/gtfmtshpgj.html

[J03] 字符串解析为日期
来源：http://hz.zhixingplan.top/gtmvmyqfgm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sysykeji.top/gtmrwuynwq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.birdmap.top/gtnjynxqxd.html

JS:   new Date("2024-01-02")
来源：http://hz.wangdashe.top/gtigkhetni.html

TS:   new Date("2024-01-02")
来源：http://hz.jianghu66.top/gtjvwziodn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zdqjudy.top/gtglprrvjf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jlsjyb.cn/gtnetcfuav.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhixingplan.top/gtuwcsdksl.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xylfe.cn/gtqcbynnsq.html

[J04] 时间戳与日期互转
来源：http://hz.zhixingplan.top/gtivzatnnl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yj20258.top/gtfiovxykc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xingfuxueyuan.xyz/gtfzqbvfvu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hfpthk.cn/gtpskxphqf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jlsjyb.cn/gtzfexutti.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zycfv.cn/gtsvwivcte.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sweek.top/gtjvuvhpcw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.sweek.top/gttuglejmn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.meibo888.top/gtgmhllmvs.html

[J05] 时间加减（加 7 天）
来源：http://hz.yongpay.top/gtxviudnol.html

Py:   now + timedelta(days=7)
来源：http://hz.bjfxy.top/gtrcsqvdzs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shzxlz.cn/gtisetcspo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.52xcode.cn/gtiyldcnhc.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.guowangkeji.top/gtcqamlwdd.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xylfe.cn/gtlodwqkai.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.redwolf501.top/gtwnvsrqvh.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gogol.net.cn/gtcutiobba.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.shanyushiyangtech.top/gtapbsemfz.html

[J06] 计算两时间之差
来源：http://hz.ppjwa.cn/gtyunqmdqz.html

Py:   (end - start).total_seconds()
来源：http://hz.tian-w.cn/gtkstvvwch.html

PHP:  $end->diff($start)->days;
来源：http://hz.meibo888.top/gtcvjyfgpk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sweek.top/gtncezuwah.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yj202588.top/gtatzctdel.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.redwolf501.top/gteeesdslh.html

Go:   end.Sub(start).Hours()
来源：http://hz.mhx1999.top/gtgvrsaobp.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhixingplan.top/gthptoflxz.html

C#:   (end - start).TotalSeconds
来源：http://hz.hysaishi.cn/gthfntzpqh.html

[J07] 比较两个日期
来源：http://hz.yj20258888.top/gthjvlcdop.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.mhx1999.top/gtjtsaggen.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ivvv.top/gtfufudzhc.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hywenlv.cn/gtmzlaaelr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yanxiufei.cn/gttkvbkcew.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cdnleiting.top/gtsamhywxa.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.daxiang520.top/gtatptqfpj.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sweek.top/gthueyjcgi.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.guannengcc.top/gtxmhfuimi.html

[J08] 提取年月日与星期
来源：http://hz.svipenyu.cn/gtyckyonrr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hywenlv.cn/gtisljkdsc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ywan-chungtsiang.top/gtmjeefiqe.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinqigfzy.top/gtztzaenpz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ydzc1.top/gtynlgfugw.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yuanzhike.top/gtznmkjhqy.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shzxlz.cn/gtljivyuio.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xingfuxueyuan.xyz/gthcwjizwe.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.svipenyu.cn/gteuvkyzue.html

[J09] 时区处理
来源：http://hz.xziqi.cn/gtxcuvjqzi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.gzhubu.top/gtcjnkngsp.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.hysaishi.cn/gtecvglytc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.smart0.xyz/gtjcuuqtnr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.svipenyu.cn/gtlrwnwkuf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.smart0.xyz/gtpkdwtkvk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sweek.top/gtzjlfbdmj.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.9152youxi.cn/gtfprtztzf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ydzc1.top/gtyikusxkp.html

[J10] 取今天 / 本月第一天
来源：http://hz.cdnleiting.top/gtzitlinay.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gzhubu.top/gtceawpwnw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ybcxt.top/gtoqtdoduw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xuanzx.com/gtjhhwhmrm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gaohongyu789.top/gtmljkspvq.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.dashuyun.cn/gtxwuebtvj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yonumen.top/gtfpvqgfql.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yvedp.cn/gtnygvjduz.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.52xcode.cn/gtwqcthisp.html

================================================================================
来源：http://hz.jinqigfzy.top/gtzqjniqhh.html

K. JSON 与序列化
来源：http://hz.jinqigfzy.top/gtjrhuzoxa.html

================================================================================
来源：http://hz.ydjk.org.cn/gtoasefsct.html

[K01] 对象转 JSON 字符串
来源：http://hz.sweek.top/gtejmihzva.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shzxlz.cn/gtslhlymqg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.kuanghao11.cn/gtbtsitkzi.html

JS:   JSON.stringify(obj)
来源：http://hz.andypj.xyz/gtvsbxkral.html

TS:   JSON.stringify(obj)
来源：http://hz.fengsongda.top/gthgbdkbiz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.tanke756.top/gtqvfqebtn.html

Go:   json.Marshal(obj)
来源：http://hz.gaohongyu789.top/gtgnmwpdxr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shuidangran.top/gtblvqyers.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ivvv.top/gtuhkixqdi.html

[K02] JSON 字符串转对象
来源：http://hz.ppjwa.cn/gtruirgyjc.html

Py:   json.loads(s)
来源：http://hz.meibo888.top/gtzwqyitoo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.gzhubu.top/gtgnlhrvaw.html

JS:   JSON.parse(s)
来源：http://hz.shzxlz.cn/gtmiwynuvn.html

TS:   JSON.parse(s)
来源：http://hz.chenlongwang.top/gtfqabacpd.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.shangyingyoupin.top/gtxynlczdg.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.gaohongyu789.top/gtplrjeeee.html

Ruby: JSON.parse(s)
来源：http://hz.zhijiandao.cn/gtrzqkgtmp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.mhx1999.top/gtvddylavs.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yuanzhike.top/gtuhhlztdl.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.andypj.xyz/gtvqkpertd.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hfpthk.cn/gtayiafavm.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.tian-w.cn/gtqcztrwdc.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258.top/gthblfbucy.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hysaishi.cn/gtqvgnubzv.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhiwuduotai.top/gtoaxmelxm.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.cqqwz.cn/gtsimupdwz.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yonumen.top/gtcyjqphia.html

[K04] 读取 JSON 文件
来源：http://hz.snrcjt.cn/gtgornjelx.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.fzhhl.top/gtamxuqoex.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xziqi.cn/gtbkdwxzvl.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.shzxlz.cn/gtpznxhkje.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ybcxt.top/gtgixuatys.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.sysykeji.top/gtmcgabavp.html


<!-- 参考信息 -->