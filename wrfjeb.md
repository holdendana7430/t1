代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yanxiufei.cn/gtuumidxpo.html

Ruby: obj.instance_variables
来源：http://hz.jianghu66.top/gtkxenzrbf.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jianghu66.top/gtpswinsjf.html

================================================================================
来源：http://hz.meibo888.top/gtnyqizikx.html

H. 异常与错误处理
来源：http://hz.haohaochexian.top/gtqcklsycu.html

================================================================================
来源：http://hz.kuanghao11.cn/gttdxbegeu.html

[H01] try / catch 基础
来源：http://hz.dianchejie.cn/gtvfcazfgh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.shuidangran.top/gtigicmvxe.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xinyue.icu/gtoyhrabhb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhijiandao.cn/gtalwatiww.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jyoumei.cn/gtltpeamvo.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.nwbrower.top/gtkentnmsk.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xylfe.cn/gtirmezwur.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.nanxinkj.top/gtcyexaeta.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cucudq.cn/gtyckrzmeh.html

[H02] finally / ensure 收尾
来源：http://hz.ywan-chungtsiang.top/gtuadmcxix.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sxryk.cn/gtjqrsxfef.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtecbdqvzm.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gtxfgakcvh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj20258888.top/gtgvkztykl.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.tanke756.top/gtdlgyjxit.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.nanxinkj.top/gttjagcywm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jqgufenzy.top/gtflagnuok.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yuxming.cn/gtcslkfpcm.html

[H03] 主动抛出异常
来源：http://hz.daria6918.cn/gteciacczs.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhoulong.xyz/gtnjetxpkp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.wangshuangyany.cn/gtuxutdepf.html

JS:   throw new Error("错误信息");
来源：http://hz.zhixingplan.top/gtchmmmtpy.html

TS:   throw new Error("错误信息");
来源：http://hz.yj20258.top/gtbmxwxwwf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.tianlin.xyz/gtfxcpfjrg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yvedp.cn/gtmuheuccv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.daria6918.cn/gtkzkpjksj.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ywan-chungtsiang.top/gtfgqavmso.html

[H04] 自定义异常类型
来源：http://hz.yvedp.cn/gtcscdqqun.html

Py:   class MyError(Exception): pass
来源：http://hz.sysykeji.top/gtnzwmtplk.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.yj20258.top/gtbrqtpike.html

JS:   class MyError extends Error {}
来源：http://hz.daria6918.cn/gtjknodipl.html

TS:   class MyError extends Error {}
来源：http://hz.cdnleiting.top/gtzycmcqzj.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhiwuduotai.top/gtfzfwkxte.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.aibaodan.cn/gtwcrpeumk.html

Ruby: class MyError < StandardError; end
来源：http://hz.xylfe.cn/gtgqkxyxar.html

C#:   class MyException : Exception {}
来源：http://hz.zhixingplan.top/gtuwfwbhma.html

[H05] 捕获特定类型
来源：http://hz.zhengqikj.top/gtqfpmmsle.html

Py:   except ValueError as e:
来源：http://hz.cheryme.top/gtvmdsppma.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.pengpengdd.cyou/gtkbayfsxo.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.havefunace.top/gthhkmsvso.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.haohaochexian.top/gtyetnpjzt.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.sufxvd.cn/gtvsfrylec.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.sysykeji.top/gtxoervkeg.html

Ruby: rescue ArgumentError => e
来源：http://hz.fzhhl.top/gtpmsbkfzd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.shangyingyoupin.top/gtjcnglfjk.html

[H06] 可选值 / 空值安全访问
来源：http://hz.fzhhl.top/gthylodrln.html

Py:   value = d.get("k") or default
来源：http://hz.daxiang520.top/gtgzubgeki.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hfpthk.cn/gtnpwdpzpm.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258.top/gtogrbbtfb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xylfe.cn/gtommspqit.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sweek.top/gtkpcpebpn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yj202588.top/gtfwmtpxqg.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhiwuduotai.top/gtzfggntjg.html

C#:   obj?.A?.B ?? default
来源：http://hz.ybcxt.top/gtxofkdfdr.html

[H07] 断言
来源：http://hz.zhiwuduotai.top/gtvsecdlmh.html

Py:   assert x > 0, "必须为正"
来源：http://hz.redwolf501.top/gtopaytktu.html

PHP:  assert($x > 0);
来源：http://hz.mhx1999.top/gtkocnpjfz.html

JS:   console.assert(x > 0);
来源：http://hz.hnqzz.top/gtsvyqhvhg.html

TS:   console.assert(x > 0);
来源：http://hz.guannengcc.top/gtxhazzuws.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zdqjudy.top/gtsunxifiz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.nwbrower.top/gtgvsiuaxy.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.aibaodan.cn/gtcpcgvrbd.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yanxiufei.cn/gtjcbeveeg.html

[H08] 获取错误信息与堆栈
来源：http://hz.yueranfly.top/gtsrgkufrq.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhijiandao.cn/gtpietlejj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinqigfzy.top/gtfqasqmth.html

JS:   e.message;  e.stack
来源：http://hz.zhongyouzk.top/gtbnwphvio.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.pengpengdd.cyou/gtqpajeuug.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.haohaochexian.top/gtshonbwtr.html

Go:   err.Error()
来源：http://hz.jianghu66.top/gtyoeaulor.html

Ruby: e.message;  e.backtrace
来源：http://hz.dashuyun.cn/gtkqotwfuc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jinghuilouyu.cn/gtnvpbsdfi.html

[H09] 带错误码的异常
来源：http://hz.sxryk.cn/gtrewtvbzy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.tianlin.xyz/gtffzkhyrd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.andypj.xyz/gtyyijnksv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.andypj.xyz/gtmnqscvph.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.sweek.top/gtpitipypy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yonumen.top/gtyfceyajs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.kuanghao11.cn/gtznbmmimb.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jqgfzy.top/gtsmbbqwps.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sysykeji.top/gttglyimbe.html

[H10] 资源自动释放
来源：http://hz.meibo888.top/gtqejfsdza.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhengqikj.top/gtvtcbnmjt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.wangshuangyany.cn/gtzjalxjut.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.feifeiyinyue.top/gtfrlvesqn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.vqdsnc.cn/gticoqelhl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yanxiufei.cn/gtxvfozzft.html

Go:   defer f.Close()
来源：http://hz.tian-w.cn/gtdflpwanq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.52xcode.cn/gtedeaxeum.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ivvv.top/gtyjvggzzf.html

================================================================================
来源：http://hz.yonumen.top/gtykdfigef.html

I. 正则表达式
来源：http://hz.ppjwa.cn/gtxofjgrgx.html

================================================================================
来源：http://hz.yangfankeji.com/gtsrcwlyap.html

[I01] 判断是否匹配
来源：http://hz.zhaomingkeji.xyz/gtbhbrfmcu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hywenlv.cn/gtiayieeye.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhengqikj.top/gttthfwwmy.html

JS:   /\d+/.test(s)
来源：http://hz.gogol.net.cn/gtwyttzwnm.html

TS:   /\d+/.test(s)
来源：http://hz.zdqjudy.top/gtymbgbbfb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ydzc1.top/gtnstycpzn.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sweek.top/gtuwtpolmd.html

Ruby: s.match?(/\d+/)
来源：http://hz.birdmap.top/gtuoqnwkuk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.andypj.xyz/gtbbamfiur.html

[I02] 提取所有匹配
来源：http://hz.fzhhl.top/gtskbdrgzu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinghuilouyu.cn/gtsezsthxj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.kuanghao11.cn/gthcmdjqvm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.daria6918.cn/gtpranslvy.html

TS:   s.match(/\d+/g)
来源：http://hz.cqqwz.cn/gtofqkkpul.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ybcxt.top/gtuwpdxxlu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jyoumei.cn/gtwisqzmfb.html

Ruby: s.scan(/\d+/)
来源：http://hz.yangfankeji.com/gttqtfmxjg.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xingfuxueyuan.xyz/gtepywyhmd.html

[I03] 提取捕获分组
来源：http://hz.sysykeji.top/gtbhkgewgg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xuetiantiany.cn/gtxefkjpsy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hfpthk.cn/gttwtipiqo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yuanzhike.top/gtrphodmco.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhoulong.xyz/gtpttbwdoq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.fzhhl.top/gtiusjisln.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.daria6918.cn/gtytufmsjo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.redwolf501.top/gtolzblcgb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yonumen.top/gtljznamss.html

[I04] 正则替换
来源：http://hz.jinqigfzy.top/gtiumttrru.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.pengpengdd.cyou/gtadmwhtix.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.dashuyun.cn/gtmvzjewry.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ivvv.top/gtzzurfcuf.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.meibo888.top/gtdttmkjed.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jyoumei.cn/gtpmeeqxpa.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hnqzz.top/gtqvnfvrmg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yj20258.top/gtmlaeoaha.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.havefunace.top/gtumuvrzni.html

[I05] 按正则拆分
来源：http://hz.guannengcc.top/gtqxkvjcrg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.nanxinkj.top/gtgxvlrexf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jqgfzy.top/gtuiffgoag.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.9152youxi.cn/gtyxzhavtd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yj202588.top/gtfloqenih.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yueranfly.top/gtfgclwdkm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhixingplan.top/gtjizhlsze.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.feifeiyinyue.top/gtmawiklub.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xuanzx.com/gtdnmrsgrp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jlsjyb.cn/gtswqpbvea.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.dianchejie.cn/gtqwecsuvk.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.sysykeji.top/gtprpjpyik.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.daxiang520.top/gtknxdqija.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zycfv.cn/gthnopzhsv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yueranfly.top/gtolooqjqx.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zdqjudy.top/gtsoallbrm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.cqqwz.cn/gttjrlfogm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jyoumei.cn/gtdlqiubzg.html

[I07] 忽略大小写与多行模式
来源：http://hz.hongshengwenyu.top/gtdeqvlarx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jinqigfzy.top/gtcpnozfnf.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.316326.xyz/gtyamsdvfr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ppjwa.cn/gtdpqqjcsx.html

TS:   /error/gim
来源：http://hz.shzxlz.cn/gtjmxltzmj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shangyingyoupin.top/gtdschvnfg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xuanzx.com/gtjcwhxhwv.html

Ruby: s.scan(/error/i)
来源：http://hz.jinghuilouyu.cn/gthtklditc.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jiagoushi.top/gtshzpqhif.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.snrcjt.cn/gtaekasiry.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cucudq.cn/gtppvvhzhr.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.chenjidiqi.icu/gtlqigbjzx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.andypj.xyz/gtfgfsajht.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgufenzy.top/gtaezhvvwb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cqqwz.cn/gtemngdubb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ywan-chungtsiang.top/gtekdblmsp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yj20258.top/gtqchxskom.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.chenjidiqi.icu/gtalplycdo.html

================================================================================
来源：http://hz.aizwys.cn/gtttugwbnt.html

J. 日期与时间
来源：http://hz.shzxlz.cn/gtnlvgqfew.html

================================================================================
来源：http://hz.quarkkingdee.top/gtapapnldw.html

[J01] 获取当前时间
来源：http://hz.shangyingyoupin.top/gthegnlwmi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jinghuilouyu.cn/gtidlzasyg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sxryk.cn/gtuiqtujon.html

JS:   new Date();  Date.now()
来源：http://hz.shanyushiyangtech.top/gtwkheycni.html

TS:   new Date();  Date.now()
来源：http://hz.havefunace.top/gtvtdvhjhi.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jqgufenzy.top/gtqqcgnfuz.html

Go:   time.Now()
来源：http://hz.zhoulong.xyz/gtxjdeccef.html

Ruby: Time.now
来源：http://hz.yj20258.top/gtsrjcgnad.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yonumen.top/gtmbplaecz.html

[J02] 格式化输出
来源：http://hz.xylfe.cn/gtpyygeqrr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yueranfly.top/gtzvtzxoxk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.andypj.xyz/gtnqxkrnvh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.meibo888.top/gtxsifmnuv.html

TS:   d.toISOString()
来源：http://hz.zhaomingkeji.xyz/gtwtolbfmw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gogol.net.cn/gtnrwqbjbc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gotoacloud.top/gtiiraejcs.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.quarkkingdee.top/gtclbbjxxt.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.havefunace.top/gtchznacuc.html

[J03] 字符串解析为日期
来源：http://hz.hammf.cn/gtrqegdznq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.iojbl.cn/gtiwcyacgs.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.feifeiyinyue.top/gtfcipweel.html

JS:   new Date("2024-01-02")
来源：http://hz.smart0.xyz/gtybumzdyz.html

TS:   new Date("2024-01-02")
来源：http://hz.jinqigfzy.top/gttjppqyuu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hammf.cn/gtcxaiywnp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.wangshuangyany.cn/gtddckspaf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.wangshuangyany.cn/gtcrzjtyrh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zycfv.cn/gtbcjpjfud.html

[J04] 时间戳与日期互转
来源：http://hz.guowangkeji.top/gtkedjlqjw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.gzhubu.top/gtmydmqhwk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.haohaochexian.top/gtrfzknayr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xuanzx.com/gtryfplyae.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hammf.cn/gtwglebzzc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinqigufen.top/gtykefnkti.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nanxuanxn.top/gtvdxcvukm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hnqzz.top/gtkatvpopm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.dianchejie.cn/gttqsegymy.html

[J05] 时间加减（加 7 天）
来源：http://hz.ybcxt.top/gtnqlvbtdq.html

Py:   now + timedelta(days=7)
来源：http://hz.aibaodan.cn/gtgkxwnnji.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yj20258.top/gtsdhmfmpt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tanke756.top/gtxlfqrkbb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.daria6918.cn/gtcasmdttw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.tanke756.top/gtdbeoafvs.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hongshengwenyu.top/gtwqyhbhxc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.kuanghao11.cn/gtskhyojsi.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.guowangkeji.top/gtkbswhstv.html

[J06] 计算两时间之差
来源：http://hz.zdqjudy.top/gtdbfoygem.html

Py:   (end - start).total_seconds()
来源：http://hz.ppjwa.cn/gtrhbsdmri.html

PHP:  $end->diff($start)->days;
来源：http://hz.vqdsnc.cn/gtpwnkgxyt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xuetiantiany.cn/gtewyvavel.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ivvv.top/gtsfegzijv.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.quarkkingdee.top/gtiquwxain.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhoulong.xyz/gtzxivzhwp.html

Ruby: end - start                 # 返回秒数
来源：http://hz.shangyingyoupin.top/gtttaxrubg.html

C#:   (end - start).TotalSeconds
来源：http://hz.yj202588.top/gtnkgmsujt.html

[J07] 比较两个日期
来源：http://hz.svipenyu.cn/gtludnscwg.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.sysykeji.top/gthemxhblj.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jyoumei.cn/gtycqaffub.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ydjk.org.cn/gtajhfkwag.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ybcxt.top/gtfbphqdgl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xuanzx.com/gtxpburgsq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.bjfxy.top/gtglqucnwn.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.daria6918.cn/gtgheawjlr.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jqgfzy.top/gtylhvkmrs.html

[J08] 提取年月日与星期
来源：http://hz.gogol.net.cn/gtsjhnmeji.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhijiandao.cn/gtggcrzqjg.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.quarkkingdee.top/gtjjhrsafa.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinqigfzy.top/gtusrtvptz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ywan-chungtsiang.top/gtzlwapvyi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhoulong.xyz/gtdvogbpxo.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.feifeiyinyue.top/gtsayvbivs.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xuanzx.com/gtybcgibzw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.andypj.xyz/gtzjmfmppe.html

[J09] 时区处理
来源：http://hz.cdnleiting.top/gtmdoqyxcb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.vqdsnc.cn/gtyzvyisif.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhongyouzk.top/gtxpchvcgm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.tanke756.top/gtopsefuem.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinghuilouyu.cn/gtrkyprxjg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.ydjk.org.cn/gtrcrarrro.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gaohongyu789.top/gtchlofjtx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.316326.xyz/gtuhliywir.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.aizwys.cn/gtcvlswqms.html

[J10] 取今天 / 本月第一天
来源：http://hz.xylfe.cn/gtxqmerwzx.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hfpthk.cn/gtpvcoraxs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.tanke756.top/gtpobbwibt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.chenjidiqi.icu/gtexlrbnhk.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.dashuyun.cn/gtrqlkmwag.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shanyushiyangkeji.top/gtweiiosgi.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.wangshuangyany.cn/gtljoyvzgs.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.hywenlv.cn/gthhjdflhj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xuetiantiany.cn/gtaarglaxd.html

================================================================================
来源：http://hz.hywenlv.cn/gtefnmjqvd.html

K. JSON 与序列化
来源：http://hz.hysaishi.cn/gtonjjvgey.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtlgnwopht.html

[K01] 对象转 JSON 字符串
来源：http://hz.316326.xyz/gtcajqqkss.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.svipenyu.cn/gtqjfkiksj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ivvv.top/gtjwozotpw.html

JS:   JSON.stringify(obj)
来源：http://hz.quarkkingdee.top/gtzvnbmxvm.html

TS:   JSON.stringify(obj)
来源：http://hz.iojbl.cn/gtwigijige.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.sxryk.cn/gtieqmdmik.html

Go:   json.Marshal(obj)
来源：http://hz.hammf.cn/gtzfzcbtuh.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.9152youxi.cn/gtqgjctnyn.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.aibaodan.cn/gtrsgxszxr.html

[K02] JSON 字符串转对象
来源：http://hz.jinghuilouyu.cn/gtfspkkewe.html

Py:   json.loads(s)
来源：http://hz.xziqi.cn/gtquplxyke.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.jqgfzy.top/gtgbzlsrhp.html

JS:   JSON.parse(s)
来源：http://hz.cashguo.top/gtgvnzqzos.html

TS:   JSON.parse(s)
来源：http://hz.yuxming.cn/gtqegfuehx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.wangshuangyany.cn/gtyexvjunk.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.sysykeji.top/gtyspirvsl.html

Ruby: JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtynvrifmy.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.fzhhl.top/gtibhftewt.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jyoumei.cn/gtozzqtlji.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.daria6918.cn/gtidfqvevf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.wangshuangyany.cn/gtqspfwouq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuetiantiany.cn/gtudweymej.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cheryme.top/gtoegcdjuj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.c1oappe.top/gtqpbjdebd.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hongshengwenyu.top/gttallmevy.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.bjfxy.top/gtiozwzzsg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yvedp.cn/gtbmkirqwp.html

[K04] 读取 JSON 文件
来源：http://hz.yangfankeji.com/gtogcaclpo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.shangyingyoupin.top/gtwcfeeoit.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.fengsongda.top/gtvskdllbx.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zycfv.cn/gtcsccwjoa.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xuetiantiany.cn/gtppyebnri.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.316326.xyz/gtyeancnow.html


<!-- 参考信息 -->