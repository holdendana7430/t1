代发 wailian999

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.daria6918.cn/gtgwdsfbjo.html

Ruby: obj.instance_variables
来源：http://hz.52xcode.cn/gtpevlameu.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.fzhhl.top/gtdlhtiawi.html

================================================================================
来源：http://hz.nanxuanxn.top/gtpxzqbadm.html

H. 异常与错误处理
来源：http://hz.fengsongda.top/gtmdbteyks.html

================================================================================
来源：http://hz.redwolf501.top/gtvagdnfzt.html

[H01] try / catch 基础
来源：http://hz.ywan-chungtsiang.top/gtekajuvqp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jiagoushi.top/gtietyiwhu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.bjfxy.top/gtyftqjvum.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhengqikj.top/gtuqxybkjn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.sweek.top/gttupamset.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.sxryk.cn/gtzbyjdhsw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.gogol.net.cn/gtairixubz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shanyushiyangkeji.top/gtqtkwsuaa.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.vqdsnc.cn/gtmuqnfzpw.html

[H02] finally / ensure 收尾
来源：http://hz.bjfxy.top/gtvzmhruji.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.c1oappe.top/gtzynfywyv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtxyvficlw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtgxgcxmqt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtxkkeiozm.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.sufxvd.cn/gtiyalqiwf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.aibaodan.cn/gtnkitmbve.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ppjwa.cn/gtzaxrucvx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinqigfzy.top/gtgckgzbtl.html

[H03] 主动抛出异常
来源：http://hz.jlsjyb.cn/gtrmfdixhp.html

Py:   raise ValueError("错误信息")
来源：http://hz.chenzaomai.com/gtjexwfeis.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.fengsongda.top/gtqzkhbilz.html

JS:   throw new Error("错误信息");
来源：http://hz.vqdsnc.cn/gthvfsxnpe.html

TS:   throw new Error("错误信息");
来源：http://hz.jyoumei.cn/gtrrjxjtjh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.nanxuanxn.top/gtzpjsrpio.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hongshengwenyu.top/gtvcooowcu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.daxiang520.top/gtczsizcip.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.wangshuangyany.cn/gtoxlcpnul.html

[H04] 自定义异常类型
来源：http://hz.yj202588.top/gtcmwatakp.html

Py:   class MyError(Exception): pass
来源：http://hz.chenjidiqi.icu/gtwzqfnoip.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jyoumei.cn/gtorcemphr.html

JS:   class MyError extends Error {}
来源：http://hz.xingfuxueyuan.xyz/gttbtrzozg.html

TS:   class MyError extends Error {}
来源：http://hz.yonumen.top/gtsjqozzgo.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hysaishi.cn/gtwxgzjxhf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gaohongyu789.top/gtkefebjkx.html

Ruby: class MyError < StandardError; end
来源：http://hz.feifeiyinyue.top/gtypbqasvv.html

C#:   class MyException : Exception {}
来源：http://hz.yueranfly.top/gtgwymhasc.html

[H05] 捕获特定类型
来源：http://hz.daxiang520.top/gtibqduazc.html

Py:   except ValueError as e:
来源：http://hz.gaohongyu789.top/gtqvspicnc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ehwqpu.com/gtncscjkns.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.guannengcc.top/gtwezyonhn.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.ppjwa.cn/gttlplxtcr.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.guowangkeji.top/gtwjtbjact.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhongyouzk.top/gtscdhvzmm.html

Ruby: rescue ArgumentError => e
来源：http://hz.hammf.cn/gtflnlrahb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jianghu66.top/gtuibbdinr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yueranfly.top/gtzoyjecfu.html

Py:   value = d.get("k") or default
来源：http://hz.sxryk.cn/gtmlgmnhqu.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.aizwys.cn/gtobmiizwu.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zycfv.cn/gtzublhaiu.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.quarkkingdee.top/gtgcdvlahq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.svipenyu.cn/gtabpkojbk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zdqjudy.top/gtsvphjumj.html

Ruby: d&.dig(:a, :b)
来源：http://hz.fzhhl.top/gthqzfogbs.html

C#:   obj?.A?.B ?? default
来源：http://hz.jlsjyb.cn/gtcmflvqkt.html

[H07] 断言
来源：http://hz.jinyuanbaomall.cn/gtfuqmfpus.html

Py:   assert x > 0, "必须为正"
来源：http://hz.redwolf501.top/gtcbnhjtye.html

PHP:  assert($x > 0);
来源：http://hz.zhaomingkeji.xyz/gtjdcymvni.html

JS:   console.assert(x > 0);
来源：http://hz.kuanghao11.cn/gtnuuxxvsg.html

TS:   console.assert(x > 0);
来源：http://hz.pycfn.com/gtdctncpty.html

Java: assert x > 0 : "必须为正";
来源：http://hz.pycfn.com/gtzwvgndde.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cqqwz.cn/gtcztygcoc.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yj20258888.top/gtyzzzjvbi.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhixingplan.top/gtrzxcqruh.html

[H08] 获取错误信息与堆栈
来源：http://hz.guowangkeji.top/gtivsrhlrq.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.smart0.xyz/gtueahbcij.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.chenzaomai.com/gtnwhykmeq.html

JS:   e.message;  e.stack
来源：http://hz.fzhhl.top/gtpkkssocs.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.andypj.xyz/gtcjqcuytl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.havefunace.top/gtfbgtvsnk.html

Go:   err.Error()
来源：http://hz.shanyushiyangtech.top/gtcavmqxol.html

Ruby: e.message;  e.backtrace
来源：http://hz.jiagoushi.top/gtqswuzend.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhiwuduotai.top/gtbtwrhjoi.html

[H09] 带错误码的异常
来源：http://hz.meibo888.top/gtilbpusye.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yueranfly.top/gtbifjowct.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.vqdsnc.cn/gtjhiynobz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhaomingkeji.xyz/gtkruemncq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.vqdsnc.cn/gtjfvxqtri.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.wangdashe.top/gtkvwgkmwl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.chenlongwang.top/gtpzdolonw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.mhx1999.top/gtjqmscizw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ybcxt.top/gtkqjisgtr.html

[H10] 资源自动释放
来源：http://hz.zhoulong.xyz/gtmabfaivq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jyoumei.cn/gtawucvtva.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hongshengwenyu.top/gtfknhpzuv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xziqi.cn/gtrvtzbcbo.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhixingplan.top/gtlzaeafew.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.tianlin.xyz/gtwnqhtyzf.html

Go:   defer f.Close()
来源：http://hz.c1oappe.top/gtomfrgsgx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.dashuyun.cn/gtotrgntgz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtxxttbycw.html

================================================================================
来源：http://hz.hywenlv.cn/gtexhpoehw.html

I. 正则表达式
来源：http://hz.zhijiandao.cn/gtwioorvoy.html

================================================================================
来源：http://hz.iojbl.cn/gtlncuavrk.html

[I01] 判断是否匹配
来源：http://hz.hfpthk.cn/gteawyzges.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhijiandao.cn/gtrzyjczus.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cucudq.cn/gtvidmbvyk.html

JS:   /\d+/.test(s)
来源：http://hz.yj20258888.top/gtvlvvknwx.html

TS:   /\d+/.test(s)
来源：http://hz.chenzaomai.com/gtlghlauih.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shanyushiyangkeji.top/gtsxgklhwa.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.pycfn.com/gtwsaqvbiu.html

Ruby: s.match?(/\d+/)
来源：http://hz.hywenlv.cn/gtjwgileka.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cqqwz.cn/gtttkvonpy.html

[I02] 提取所有匹配
来源：http://hz.smart0.xyz/gteeyickyd.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jyoumei.cn/gtqxtbcwcg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hammf.cn/gtgwxavngw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cdnleiting.top/gtyfeyenzk.html

TS:   s.match(/\d+/g)
来源：http://hz.yj20258.top/gtywnosklf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.haohaochexian.top/gtddgetfpu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.gogol.net.cn/gttabpxcqh.html

Ruby: s.scan(/\d+/)
来源：http://hz.jyoumei.cn/gtyawxyang.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.iojbl.cn/gtapirddqq.html

[I03] 提取捕获分组
来源：http://hz.bjfxy.top/gtoavvxhbm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hnxiangtu.top/gtpqakeixs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.52xcode.cn/gtedhfwxym.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.9152youxi.cn/gtlebecknu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yueranfly.top/gtlxyzedku.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.tanke756.top/gtgzpeuruq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhengqikj.top/gtcrimzsem.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.smart0.xyz/gttmdzbqhb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yueranfly.top/gthjhyhcwo.html

[I04] 正则替换
来源：http://hz.dianchejie.cn/gtbuuqpruu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.dianchejie.cn/gthbavqpma.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yongpay.top/gteexbonmi.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.dashuyun.cn/gtkfiypotn.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xinyue.icu/gtqmtmrvhh.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhoulong.xyz/gtmiahplmy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.9152youxi.cn/gtlahmafqq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.chenlongwang.top/gttayvulwn.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.c1oappe.top/gtojfksxij.html

[I05] 按正则拆分
来源：http://hz.chenjidiqi.icu/gtcvkkaboi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhiwuduotai.top/gtfbbhwsja.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yvedp.cn/gtyxlkbxsh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yuanzhike.top/gtiwvnalbn.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tanke756.top/gtjlrnqdxd.html

Java: s.split("\\s*,\\s*")
来源：http://hz.kuanghao11.cn/gtphqsexum.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.iojbl.cn/gtkubpefkm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yuxming.cn/gtbwyvxtnn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.pycfn.com/gtciftyrkg.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xziqi.cn/gtgfjkqptf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinghuilouyu.cn/gtudeskbub.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cqqwz.cn/gtcbiqunfs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gzhubu.top/gtfnbxaerw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinghuilouyu.cn/gthpqyoaap.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.kuanghao11.cn/gtxxzdkrcy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sxryk.cn/gtzurukynw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.meibo888.top/gtsaztaysn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.iojbl.cn/gturbikjoz.html

[I07] 忽略大小写与多行模式
来源：http://hz.ywan-chungtsiang.top/gtsqfbdgwk.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.aizwys.cn/gtrpiomdmj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.gaohongyu789.top/gtohgildam.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.chenlongwang.top/gtiihcpxyi.html

TS:   /error/gim
来源：http://hz.yvedp.cn/gtzrrfguxh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.nanxinkj.top/gtwcybqfpg.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.iojbl.cn/gtjldfouje.html

Ruby: s.scan(/error/i)
来源：http://hz.yangfankeji.com/gtpknwzgfa.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.aibaodan.cn/gtiqoxqgfh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.hnqzz.top/gthvailwvs.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hywenlv.cn/gtbdhlqfwk.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.nanxuanxn.top/gtwkvzrrxw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zycfv.cn/gttfdqjakp.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tian-w.cn/gtimdihlcn.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yongpay.top/gtvhqhbawd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gogol.net.cn/gtyvypzxei.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.wangshuangyany.cn/gtjcwqyilx.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hnxiangtu.top/gtyqasssjy.html

================================================================================
来源：http://hz.redwolf501.top/gtynucdvhz.html

J. 日期与时间
来源：http://hz.hnqzz.top/gtviovwnyr.html

================================================================================
来源：http://hz.ybcxt.top/gtlmnesveg.html

[J01] 获取当前时间
来源：http://hz.shangyingyoupin.top/gtrfqsnmjp.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yj20258888.top/gtyuboaxtx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.fzhhl.top/gttyafbkau.html

JS:   new Date();  Date.now()
来源：http://hz.yvedp.cn/gtvaufjpzh.html

TS:   new Date();  Date.now()
来源：http://hz.zhoulong.xyz/gtnlqezaft.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinqigufen.top/gtjavvkjea.html

Go:   time.Now()
来源：http://hz.wangshuangyany.cn/gtaaahvyna.html

Ruby: Time.now
来源：http://hz.guowangkeji.top/gtdoegkvae.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xuanzx.com/gtkvxnqnqs.html

[J02] 格式化输出
来源：http://hz.gogol.net.cn/gtgzatudmt.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gzhubu.top/gtdvhpvkuw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hnxiangtu.top/gtsclmkzgg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xingfuxueyuan.xyz/gteppiuuaw.html

TS:   d.toISOString()
来源：http://hz.yj20258.top/gtxnzpigyj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.chenlongwang.top/gtnvfdhycp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yj202588.top/gtzfbgruuv.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj202588.top/gtyhseclgh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhengqikj.top/gtxfrwjaui.html

[J03] 字符串解析为日期
来源：http://hz.jinqigufen.top/gtyjbaddnv.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.pycfn.com/gtwvtpdnjy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.bjfxy.top/gtuoowcglo.html

JS:   new Date("2024-01-02")
来源：http://hz.wangdashe.top/gtdtiyapkp.html

TS:   new Date("2024-01-02")
来源：http://hz.hammf.cn/gtufidimiu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.wangdashe.top/gtcdjhonjv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hywenlv.cn/gtatumzupu.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.52xcode.cn/gtoggymqhi.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xuanzx.com/gtlvmgpznt.html

[J04] 时间戳与日期互转
来源：http://hz.daxiang520.top/gtejigjgpq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.gotoacloud.top/gtlbhxtrbw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sxryk.cn/gtwhkjwrrs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ppjwa.cn/gtdzdkbyck.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhongyouzk.top/gtxxrospux.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhengqikj.top/gtesccmudq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ivvv.top/gtxxbqynwq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.0kj1m.cn/gtbmmgyloj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yuanzhike.top/gtnxbmuenn.html

[J05] 时间加减（加 7 天）
来源：http://hz.yvedp.cn/gtpvhvynpi.html

Py:   now + timedelta(days=7)
来源：http://hz.sysykeji.top/gtdbqjbfbh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.birdmap.top/gtdhjlrnyt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.andypj.xyz/gtbqkhhtxo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhiwuduotai.top/gtccuphmpy.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.xinyue.icu/gtmwbbtwcc.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xuetiantiany.cn/gtjicruzbv.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhoulong.xyz/gtpdhvibar.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xziqi.cn/gtfzbhovog.html

[J06] 计算两时间之差
来源：http://hz.yj20258888.top/gtfkfqsntz.html

Py:   (end - start).total_seconds()
来源：http://hz.xingfuxueyuan.xyz/gtigyytpev.html

PHP:  $end->diff($start)->days;
来源：http://hz.hysaishi.cn/gtsbcvkfmf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hongshengwenyu.top/gtwxpbqkxa.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.chenjidiqi.icu/gtrlbzvkpo.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.sufxvd.cn/gtikgakthg.html

Go:   end.Sub(start).Hours()
来源：http://hz.jqgfzy.top/gtsrcsgnrw.html

Ruby: end - start                 # 返回秒数
来源：http://hz.mhx1999.top/gtueunwylb.html

C#:   (end - start).TotalSeconds
来源：http://hz.xuetiantiany.cn/gtxrewfeqt.html

[J07] 比较两个日期
来源：http://hz.ywan-chungtsiang.top/gtmzrwziyf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.fzhhl.top/gtstpkfopk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.zycfv.cn/gtyhxgdzwu.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.tanke756.top/gtpnofkxrc.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenjidiqi.icu/gtaafypxnn.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhengqikj.top/gtfkbstypj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.birdmap.top/gtmhwoxgnx.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cashguo.top/gtpkpotlqf.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sxryk.cn/gtgusograd.html

[J08] 提取年月日与星期
来源：http://hz.jinyuanbaomall.cn/gtyvdtzjnb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jiagoushi.top/gtqrotmrpl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hongshengwenyu.top/gtobhegvxf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.gogol.net.cn/gtwwdobagn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhijiandao.cn/gtpryufaho.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.shuidangran.top/gtaqhaasmj.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.fengsongda.top/gtkipofbdn.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jinqigfzy.top/gtjbvnsiku.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jqgufenzy.top/gtgqrxokcj.html

[J09] 时区处理
来源：http://hz.hongshengwenyu.top/gtvthjpppt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yonumen.top/gtnfslcrws.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yj202588.top/gtlebrujbj.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangkeji.top/gtggjaanxv.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guowangkeji.top/gthrjxqiof.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hysaishi.cn/gtltrggebs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.vqdsnc.cn/gtfgljcxpn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.gotoacloud.top/gtjbsdatia.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.havefunace.top/gtwfjtpsxm.html

[J10] 取今天 / 本月第一天
来源：http://hz.hfpthk.cn/gtzswrhuht.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.andypj.xyz/gtozoepaqu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.chenjidiqi.icu/gtiphuawdf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xingfuxueyuan.xyz/gtumiqvzor.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhijiandao.cn/gtpfqgrjgl.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.shzxlz.cn/gtimscrdai.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yangfankeji.com/gtvpkeoeiv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zdqjudy.top/gtxbicbois.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shzxlz.cn/gtqnbwmlij.html

================================================================================
来源：http://hz.hfpthk.cn/gtiobutvya.html

K. JSON 与序列化
来源：http://hz.havefunace.top/gtadnnasbf.html

================================================================================
来源：http://hz.jlsjyb.cn/gtrouurxdt.html

[K01] 对象转 JSON 字符串
来源：http://hz.shangyingyoupin.top/gtsbztjxts.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinqigfzy.top/gtwllnoknt.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yonumen.top/gtxjrrwcqn.html

JS:   JSON.stringify(obj)
来源：http://hz.shuidangran.top/gtxslfqntc.html

TS:   JSON.stringify(obj)
来源：http://hz.chenlongwang.top/gtvhglwezh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yvedp.cn/gtabmccvgj.html

Go:   json.Marshal(obj)
来源：http://hz.yongpay.top/gtbpmviixy.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.xuanzx.com/gtmkdstbob.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.ehwqpu.com/gtfnegyeqj.html

[K02] JSON 字符串转对象
来源：http://hz.52xcode.cn/gtbujzkyxb.html

Py:   json.loads(s)
来源：http://hz.jyoumei.cn/gtqztwrmhc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.nwbrower.top/gtytmtxytg.html

JS:   JSON.parse(s)
来源：http://hz.cucudq.cn/gtguhqjcri.html

TS:   JSON.parse(s)
来源：http://hz.zycfv.cn/gtoghrqjdu.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.mhx1999.top/gtqcmwayvt.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xylfe.cn/gtbhfjjyzw.html

Ruby: JSON.parse(s)
来源：http://hz.jinqigfzy.top/gtebbsyhnm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xinyue.icu/gtgowkotdb.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.meibo888.top/gtpjadqkuo.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jiagoushi.top/gtybydtibn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.ppjwa.cn/gtxrasmujb.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.daria6918.cn/gtdwogvzow.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.fengsongda.top/gtbcfewpck.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.sxryk.cn/gtgwnsyvoj.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hywenlv.cn/gttdulngjw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.gogol.net.cn/gtwnwgmckn.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhoulong.xyz/gtdpvswwhy.html

[K04] 读取 JSON 文件
来源：http://hz.9152youxi.cn/gtdkuwzlpk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hysaishi.cn/gtrpwpggse.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.shanyushiyangtech.top/gtembwcmxo.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.xziqi.cn/gtaoaeparg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.havefunace.top/gtnhiqgkit.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.pycfn.com/gtflrbjkal.html


<!-- 参考信息 -->