代发 wailian999

PHP:  get_object_vars($obj);
来源：http://hz.gotoacloud.top/gtlakoblmv.html

JS:   Object.entries(obj)
来源：http://hz.meibo888.top/gtirwdidum.html

TS:   Object.entries(obj)
来源：http://hz.chenzaomai.com/gtzdqhsrlw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.vqdsnc.cn/gtqcizxufv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ywan-chungtsiang.top/gtlsmaqcgi.html

Ruby: obj.instance_variables
来源：http://hz.xuetiantiany.cn/gtpcbetzkr.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jqgufenzy.top/gtuvhtssrg.html

================================================================================
来源：http://hz.redwolf501.top/gtrmrmxvai.html

H. 异常与错误处理
来源：http://hz.sufxvd.cn/gtjrutbgmz.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtdldyequf.html

[H01] try / catch 基础
来源：http://hz.tian-w.cn/gttouomfbr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jianghu66.top/gttlfyrkek.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.andypj.xyz/gtzewrhjgo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shanyushiyangkeji.top/gttkiawfko.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yanxiufei.cn/gtkxrlassb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xziqi.cn/gtuhltmvgl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.bjfxy.top/gtpcgzdtlx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.kuanghao11.cn/gtkrshofsv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.wangdashe.top/gtzuznixhl.html

[H02] finally / ensure 收尾
来源：http://hz.dianchejie.cn/gthwvjcyig.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jyoumei.cn/gtyevzvirt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hfpthk.cn/gtyphnyhfg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gtadmbrled.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuetiantiany.cn/gtgorwaaxg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gtqqnzragj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.kuanghao11.cn/gtblzpvwwt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shanyushiyangkeji.top/gtvpiouqed.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.nwbrower.top/gtecxhanbg.html

[H03] 主动抛出异常
来源：http://hz.jinqigufen.top/gtvjjjehkm.html

Py:   raise ValueError("错误信息")
来源：http://hz.yonumen.top/gtjwmdxhvq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cucudq.cn/gtlasrilgo.html

JS:   throw new Error("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtzzeiksll.html

TS:   throw new Error("错误信息");
来源：http://hz.jinghuilouyu.cn/gtmusjlxol.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sxryk.cn/gthromvoke.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.cheryme.top/gttrxzecnm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sufxvd.cn/gtwxiympwm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ydzc1.top/gtrxexxfpg.html

[H04] 自定义异常类型
来源：http://hz.shzxlz.cn/gtycxsmfdv.html

Py:   class MyError(Exception): pass
来源：http://hz.svipenyu.cn/gtwnsjanud.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shuidangran.top/gtfxgienoc.html

JS:   class MyError extends Error {}
来源：http://hz.meibo888.top/gtupuduutp.html

TS:   class MyError extends Error {}
来源：http://hz.cqqwz.cn/gtptmqbumk.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zycfv.cn/gtjvqdxqru.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jlsjyb.cn/gtitbhgjol.html

Ruby: class MyError < StandardError; end
来源：http://hz.xuetiantiany.cn/gtmejunzug.html

C#:   class MyException : Exception {}
来源：http://hz.aizwys.cn/gtbjefblqp.html

[H05] 捕获特定类型
来源：http://hz.cdnleiting.top/gtohxhphgz.html

Py:   except ValueError as e:
来源：http://hz.shuidangran.top/gtjglovfps.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hammf.cn/gtihjhlctu.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.gotoacloud.top/gtjckfpwbl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhaomingkeji.xyz/gtnaovainn.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yanxiufei.cn/gtkkeganjx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhiwuduotai.top/gtznfssbgr.html

Ruby: rescue ArgumentError => e
来源：http://hz.dashuyun.cn/gtxziijzrk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jqgfzy.top/gtgydfpujt.html

[H06] 可选值 / 空值安全访问
来源：http://hz.wangdashe.top/gtauhgyghh.html

Py:   value = d.get("k") or default
来源：http://hz.xuanzx.com/gtmdcobzoz.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.52xcode.cn/gtasclzigg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.chenlongwang.top/gtyzakhovv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jlsjyb.cn/gtsmrjmlii.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhongyouzk.top/gtxjgsqoni.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ywan-chungtsiang.top/gtpwppmrxo.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hysaishi.cn/gtiwfbuykm.html

C#:   obj?.A?.B ?? default
来源：http://hz.c1oappe.top/gtnievfbgv.html

[H07] 断言
来源：http://hz.ybcxt.top/gtbbqnbfor.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinqigufen.top/gtlkqcxlmt.html

PHP:  assert($x > 0);
来源：http://hz.aibaodan.cn/gthelwaqta.html

JS:   console.assert(x > 0);
来源：http://hz.fengsongda.top/gtzquothut.html

TS:   console.assert(x > 0);
来源：http://hz.yj20258888.top/gtovknipsi.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ydjk.org.cn/gtlcyutpul.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xziqi.cn/gtqskilaym.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jiagoushi.top/gtqpqmsfsa.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yvedp.cn/gtjvjozblc.html

[H08] 获取错误信息与堆栈
来源：http://hz.yangfankeji.com/gtdheekjoh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.snrcjt.cn/gtowkgijtm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xuanzx.com/gtcaemmcta.html

JS:   e.message;  e.stack
来源：http://hz.xinyue.icu/gtdysieckf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.316326.xyz/gtpipmuaqp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.9152youxi.cn/gtphkzrovh.html

Go:   err.Error()
来源：http://hz.fzhhl.top/gtoencacmz.html

Ruby: e.message;  e.backtrace
来源：http://hz.hnxiangtu.top/gtcqilmvtx.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhiwuduotai.top/gtranwhwfq.html

[H09] 带错误码的异常
来源：http://hz.gogol.net.cn/gtvawoozff.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.svipenyu.cn/gtlsbjubpb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yongpay.top/gtzzkmzayv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shzxlz.cn/gtnrqarkzq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xinyue.icu/gtlpodiybh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.snrcjt.cn/gtvluvihwt.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.birdmap.top/gtfigqqkzo.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.chenjidiqi.icu/gtmnyjkmfr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhoulong.xyz/gteuvmasui.html

[H10] 资源自动释放
来源：http://hz.daria6918.cn/gtgpbqmjdp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.fengsongda.top/gtblumubep.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.dianchejie.cn/gtnfgfyrbj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxinkj.top/gtmcuttfqg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hywenlv.cn/gtkbduqzrj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zhaomingkeji.xyz/gtgtykpemm.html

Go:   defer f.Close()
来源：http://hz.havefunace.top/gtgcznfnsx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.wangshuangyany.cn/gtbdijkgqs.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.dashuyun.cn/gtlfpheboj.html

================================================================================
来源：http://hz.birdmap.top/gttcvrboyx.html

I. 正则表达式
来源：http://hz.cucudq.cn/gthupatcdm.html

================================================================================
来源：http://hz.yj20258888.top/gtxskedvke.html

[I01] 判断是否匹配
来源：http://hz.tian-w.cn/gtxluunlrc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.aibaodan.cn/gtmmygiacp.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.jinqigfzy.top/gteuowtggd.html

JS:   /\d+/.test(s)
来源：http://hz.nanxuanxn.top/gtvxoenhem.html

TS:   /\d+/.test(s)
来源：http://hz.sweek.top/gtpxjlgjio.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.birdmap.top/gtngtmduvc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhaomingkeji.xyz/gtdqzydkzs.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinqigufen.top/gtbkmenkvp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ybcxt.top/gtyrtjpuol.html

[I02] 提取所有匹配
来源：http://hz.xuetiantiany.cn/gtrrxieebn.html

Py:   re.findall(r"\d+", s)
来源：http://hz.tanke756.top/gtkjryhlpk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hnqzz.top/gtebidaptp.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.daria6918.cn/gtkdcdyvex.html

TS:   s.match(/\d+/g)
来源：http://hz.daria6918.cn/gtpwthhahl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yj20258888.top/gtqfuqqhdp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ivvv.top/gtzedbacmb.html

Ruby: s.scan(/\d+/)
来源：http://hz.316326.xyz/gtpqcwytgl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hongshengwenyu.top/gtjdovanbl.html

[I03] 提取捕获分组
来源：http://hz.yongpay.top/gtkbgbdglo.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.sysykeji.top/gtolwoplff.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yanxiufei.cn/gtbvuoodtn.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yangfankeji.com/gtjumooaef.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.c1oappe.top/gttrsjgilv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ydjk.org.cn/gtocfturpg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.wangdashe.top/gtmhpbazvk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shangyingyoupin.top/gtzwdupzzm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cqqwz.cn/gtosbfujql.html

[I04] 正则替换
来源：http://hz.cheryme.top/gtghrsuwgl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cheryme.top/gtitdcgyfo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cashguo.top/gtwmspwgpc.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ydzc1.top/gtktvfcevn.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigufen.top/gtfoskgnyn.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hammf.cn/gtwsbqefkx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.wangshuangyany.cn/gtjuuwwggs.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.iojbl.cn/gtmgrvyhwh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yvedp.cn/gtcezovcrn.html

[I05] 按正则拆分
来源：http://hz.vqdsnc.cn/gteznqhdgn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.sysykeji.top/gtyjobcxux.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xuetiantiany.cn/gtflouztav.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.meibo888.top/gtpifpcxjo.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.xuanzx.com/gtgpqznhof.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yonumen.top/gttbnthiho.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xuetiantiany.cn/gtfyjsqmgd.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.snrcjt.cn/gtbhrluetm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhaomingkeji.xyz/gttgbydpgo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jqgufenzy.top/gtezzicxuc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.gzhubu.top/gtggbhoneu.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.316326.xyz/gtqsqdxuii.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenzaomai.com/gteijvlmpn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.dashuyun.cn/gtfmjtukjs.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.smart0.xyz/gtnkazmvmi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yuxming.cn/gtghigyfqk.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hammf.cn/gtptsqcxlx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xingfuxueyuan.xyz/gtqnqxkuzn.html

[I07] 忽略大小写与多行模式
来源：http://hz.gogol.net.cn/gtfuppbefg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shanyushiyangkeji.top/gttcdmhghy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.sweek.top/gtilrpejmi.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xingfuxueyuan.xyz/gtyxcluvwt.html

TS:   /error/gim
来源：http://hz.cdnleiting.top/gtziwqlnbk.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shangyingyoupin.top/gtrqxhneoe.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hammf.cn/gtsfygcdoz.html

Ruby: s.scan(/error/i)
来源：http://hz.yvedp.cn/gtevmqxtjy.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jyoumei.cn/gtginmtmsb.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.9152youxi.cn/gtsvoqtzpz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yonumen.top/gtnllolwgq.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinqigfzy.top/gturfbftzw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuanzx.com/gtvujnlsre.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yongpay.top/gtzmcsuswl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhaomingkeji.xyz/gtpnvjbdea.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shangyingyoupin.top/gtbpzhwdvv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.guannengcc.top/gtnddyekah.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.wangdashe.top/gtbuzqjlup.html

================================================================================
来源：http://hz.zhongyouzk.top/gtbxxhgqle.html

J. 日期与时间
来源：http://hz.ppjwa.cn/gtjqbxnqrh.html

================================================================================
来源：http://hz.jqgfzy.top/gtymiundsx.html

[J01] 获取当前时间
来源：http://hz.c1oappe.top/gtmespumsm.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.fzhhl.top/gtkcenstth.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yanxiufei.cn/gtxskhmbuk.html

JS:   new Date();  Date.now()
来源：http://hz.jinqigufen.top/gtmflqskip.html

TS:   new Date();  Date.now()
来源：http://hz.dianchejie.cn/gtlninmgin.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ydzc1.top/gtuatgfnes.html

Go:   time.Now()
来源：http://hz.guannengcc.top/gtuvvithwr.html

Ruby: Time.now
来源：http://hz.9152youxi.cn/gtydiajjnd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhixingplan.top/gtcbfdswit.html

[J02] 格式化输出
来源：http://hz.haohaochexian.top/gtwmchuhef.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.redwolf501.top/gtiyypwxhe.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.snrcjt.cn/gtdufaykza.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.sufxvd.cn/gtylkwkqzy.html

TS:   d.toISOString()
来源：http://hz.tian-w.cn/gtuqiitkrt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hfpthk.cn/gtvyufwygf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cheryme.top/gtpfczifgc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ybcxt.top/gtzbrnmykq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.redwolf501.top/gtsixnuddf.html

[J03] 字符串解析为日期
来源：http://hz.yuanzhike.top/gttdosxydm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yanxiufei.cn/gtzgynvzlp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.tianlin.xyz/gtkurmrvsh.html

JS:   new Date("2024-01-02")
来源：http://hz.yj20258888.top/gtntwfyvam.html

TS:   new Date("2024-01-02")
来源：http://hz.xuetiantiany.cn/gtspufdqgx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.redwolf501.top/gtrywcvnos.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtnybwerde.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gaohongyu789.top/gtyqxrpvdt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yuxming.cn/gtebzxnift.html

[J04] 时间戳与日期互转
来源：http://hz.tian-w.cn/gtsczxvrfp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jianghu66.top/gtzzckrrdk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yj20258.top/gtabnfdffp.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.shzxlz.cn/gtvkpwetod.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.nanxuanxn.top/gtijesfqgw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jiagoushi.top/gtqenwblhy.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ywan-chungtsiang.top/gtziwgfsyb.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hnqzz.top/gtwvxwwwme.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shzxlz.cn/gtxbdqiagx.html

[J05] 时间加减（加 7 天）
来源：http://hz.yj202588.top/gtbmrvvtfi.html

Py:   now + timedelta(days=7)
来源：http://hz.tanke756.top/gttiujnmfm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.gzhubu.top/gtnfplqywf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zycfv.cn/gtcyldqbsj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.0kj1m.cn/gtiwayzodd.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xingfuxueyuan.xyz/gtqazpvrce.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.feifeiyinyue.top/gtxnfvntci.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yj20258888.top/gtyxupjmbn.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.andypj.xyz/gtzukdvimw.html

[J06] 计算两时间之差
来源：http://hz.xingfuxueyuan.xyz/gtmysepoyq.html

Py:   (end - start).total_seconds()
来源：http://hz.jyoumei.cn/gtnmsitxpp.html

PHP:  $end->diff($start)->days;
来源：http://hz.chenjidiqi.icu/gtmbasujxv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.guowangkeji.top/gtnjmaiwte.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.bjfxy.top/gtyhepiwzi.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.daxiang520.top/gtrfbmkrfi.html

Go:   end.Sub(start).Hours()
来源：http://hz.wangdashe.top/gtqonrjprd.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ywan-chungtsiang.top/gtxlcfnvem.html

C#:   (end - start).TotalSeconds
来源：http://hz.daxiang520.top/gthgaiyxkm.html

[J07] 比较两个日期
来源：http://hz.shzxlz.cn/gtntwfrfmb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.9152youxi.cn/gtzuekevjq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.aizwys.cn/gtgukzhatk.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jlsjyb.cn/gtvmptodbc.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jianghu66.top/gtaxxfsmge.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.shanyushiyangtech.top/gtnjjjmpwm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhoulong.xyz/gtzoqkenop.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.chenjidiqi.icu/gtqtfiqarm.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sysykeji.top/gtwwzkwura.html

[J08] 提取年月日与星期
来源：http://hz.aizwys.cn/gtklmotdqp.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.52xcode.cn/gtpynqyynd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jqgufenzy.top/gtqgopxcho.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.chenlongwang.top/gtezgbjdwk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gzhubu.top/gtzsbsyogk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xuanzx.com/gtjsuozftb.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hnqzz.top/gtxmfvsadt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.aibaodan.cn/gtwzutnsew.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shanyushiyangtech.top/gtrjajjgjr.html

[J09] 时区处理
来源：http://hz.sweek.top/gtggxmcfcy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yangfankeji.com/gtdisixkuh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.iojbl.cn/gttdasjdgz.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhengqikj.top/gtjhuawoct.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgufenzy.top/gtlvvglgrf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cdnleiting.top/gtrtipmwkh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jiagoushi.top/gtposyenyw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shuidangran.top/gtotztcrmr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.yuanzhike.top/gtpnjwcazq.html

[J10] 取今天 / 本月第一天
来源：http://hz.snrcjt.cn/gtgvidwwxv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.guowangkeji.top/gtsquxdzwu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xuanzx.com/gtpxlmofmo.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.shzxlz.cn/gtoyizzmys.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.wangshuangyany.cn/gtoxawivrd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.daxiang520.top/gtojsjhqtz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.chenzaomai.com/gtxhucgiym.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xylfe.cn/gtdavechgt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jqgfzy.top/gtjrwocuud.html

================================================================================
来源：http://hz.yangfankeji.com/gtxeaolite.html

K. JSON 与序列化
来源：http://hz.yanxiufei.cn/gtbpxsxxbv.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtpmbzxpqs.html

[K01] 对象转 JSON 字符串
来源：http://hz.hongshengwenyu.top/gtjymtjstm.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.tianlin.xyz/gtzeimuobq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hysaishi.cn/gtqymvzqrv.html

JS:   JSON.stringify(obj)
来源：http://hz.cdnleiting.top/gtgxrhikcp.html

TS:   JSON.stringify(obj)
来源：http://hz.ydjk.org.cn/gtguldivuh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.aizwys.cn/gtieootwzo.html

Go:   json.Marshal(obj)
来源：http://hz.hfpthk.cn/gtcjgtzxnm.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinqigufen.top/gtovzcbzar.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ydjk.org.cn/gtqusmzmis.html

[K02] JSON 字符串转对象
来源：http://hz.chenjidiqi.icu/gtsrvkwhqa.html

Py:   json.loads(s)
来源：http://hz.guowangkeji.top/gtbyypmsdx.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.hnqzz.top/gtnyuzmswo.html

JS:   JSON.parse(s)
来源：http://hz.ywan-chungtsiang.top/gtjxvjlfqi.html

TS:   JSON.parse(s)
来源：http://hz.jinyuanbaomall.cn/gtfowdpapg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.sufxvd.cn/gtaktyctyy.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xuanzx.com/gthqlldfcq.html

Ruby: JSON.parse(s)
来源：http://hz.ehwqpu.com/gtkydfhtqd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xuanzx.com/gtnfcqgyao.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yuxming.cn/gtwpkgehkg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gotoacloud.top/gtjhhgzjnv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.dashuyun.cn/gtrnyreajv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangshuangyany.cn/gthtmsciqh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zhixingplan.top/gtejoewlkf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.sufxvd.cn/gteeflzlex.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xuanzx.com/gtpszjphkl.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.meibo888.top/gtjkckkyac.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tanke756.top/gtxohnpabi.html

[K04] 读取 JSON 文件
来源：http://hz.chenlongwang.top/gtwprruqqr.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.kuanghao11.cn/gtossoykeo.html


<!-- 参考信息 -->