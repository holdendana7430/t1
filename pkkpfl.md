代发 wailian999

PHP:  get_object_vars($obj);
来源：http://hz.havefunace.top/gtesjspbnq.html

JS:   Object.entries(obj)
来源：http://hz.andypj.xyz/gtopwvfzsq.html

TS:   Object.entries(obj)
来源：http://hz.fengsongda.top/gtwkpaekba.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hongshengwenyu.top/gtstsgfiuq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.guannengcc.top/gtvptmrvxd.html

Ruby: obj.instance_variables
来源：http://hz.shuidangran.top/gtfpnznnvg.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cucudq.cn/gtzrqolzib.html

================================================================================
来源：http://hz.zhixingplan.top/gtbpmbiflo.html

H. 异常与错误处理
来源：http://hz.ydzc1.top/gtdssndxax.html

================================================================================
来源：http://hz.sxryk.cn/gtzfsqspze.html

[H01] try / catch 基础
来源：http://hz.andypj.xyz/gtjqqoqfog.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yonumen.top/gtkfercqlf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jiagoushi.top/gtinwshvdy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.daxiang520.top/gtsyzektjn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.fengsongda.top/gtvnpyhovk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.sysykeji.top/gtfredkhip.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.cdnleiting.top/gtvzdezgyi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.xinyue.icu/gtvxhaiqho.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.9152youxi.cn/gtrsydbdyt.html

[H02] finally / ensure 收尾
来源：http://hz.yj20258888.top/gtroqpbwsw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jinqigfzy.top/gtjzpwovsn.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gtuhpfurmk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gtzyqauocu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sxryk.cn/gtdlodgpwb.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtjjlipzdi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.haohaochexian.top/gtghhkvcze.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hammf.cn/gtedzjwrsz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cheryme.top/gtpdsdlech.html

[H03] 主动抛出异常
来源：http://hz.tian-w.cn/gtnsnngfvf.html

Py:   raise ValueError("错误信息")
来源：http://hz.birdmap.top/gtlrybrxbl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.aibaodan.cn/gthlforkpx.html

JS:   throw new Error("错误信息");
来源：http://hz.aizwys.cn/gtrohnzkkp.html

TS:   throw new Error("错误信息");
来源：http://hz.yongpay.top/gtjflcvubx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jlsjyb.cn/gtszlyazpf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hnqzz.top/gteyojxrqy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cashguo.top/gtrhcwyyko.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhiwuduotai.top/gtvwaeiagj.html

[H04] 自定义异常类型
来源：http://hz.xingfuxueyuan.xyz/gthjllrkyz.html

Py:   class MyError(Exception): pass
来源：http://hz.svipenyu.cn/gtvvhafgbs.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhoulong.xyz/gtdrqgrkjj.html

JS:   class MyError extends Error {}
来源：http://hz.zhengqikj.top/gthbrkmdod.html

TS:   class MyError extends Error {}
来源：http://hz.c1oappe.top/gtzfcxltby.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xinyue.icu/gtoiygvmis.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.feifeiyinyue.top/gthlddoyyz.html

Ruby: class MyError < StandardError; end
来源：http://hz.daxiang520.top/gtmwurlhfo.html

C#:   class MyException : Exception {}
来源：http://hz.haohaochexian.top/gtzudeuhrp.html

[H05] 捕获特定类型
来源：http://hz.tianlin.xyz/gtdwooesqs.html

Py:   except ValueError as e:
来源：http://hz.jlsjyb.cn/gtowyzisjy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cqqwz.cn/gtwhngvbkr.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.gaohongyu789.top/gtxtikkzvs.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhaomingkeji.xyz/gtsaofaush.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.xingfuxueyuan.xyz/gtnvurmqep.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jianghu66.top/gtmsqropgm.html

Ruby: rescue ArgumentError => e
来源：http://hz.dianchejie.cn/gtgbnneuiu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.chenjidiqi.icu/gthpftargy.html

[H06] 可选值 / 空值安全访问
来源：http://hz.snrcjt.cn/gtuhrvkyow.html

Py:   value = d.get("k") or default
来源：http://hz.9152youxi.cn/gttqgcytvj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jinqigfzy.top/gtlkpfehaa.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yanxiufei.cn/gtknfzsfvt.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shzxlz.cn/gtpgvwnptc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.aibaodan.cn/gtslbgpfat.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.andypj.xyz/gtspwpjyrq.html

Ruby: d&.dig(:a, :b)
来源：http://hz.xuanzx.com/gtkgxzmcjf.html

C#:   obj?.A?.B ?? default
来源：http://hz.dianchejie.cn/gtkalhbbmf.html

[H07] 断言
来源：http://hz.sufxvd.cn/gtqwslfbnk.html

Py:   assert x > 0, "必须为正"
来源：http://hz.nanxuanxn.top/gtbqarrsrs.html

PHP:  assert($x > 0);
来源：http://hz.guowangkeji.top/gtanjhaatl.html

JS:   console.assert(x > 0);
来源：http://hz.xingfuxueyuan.xyz/gtkwzrgqiy.html

TS:   console.assert(x > 0);
来源：http://hz.kuanghao11.cn/gtjshbhjqr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jinqigfzy.top/gtdcihukku.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ivvv.top/gtbpplcjvi.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ppjwa.cn/gtaiglgsss.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yonumen.top/gtehenoimi.html

[H08] 获取错误信息与堆栈
来源：http://hz.yuxming.cn/gtouzttzgy.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jianghu66.top/gttoosfdfz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.0kj1m.cn/gttecqugsv.html

JS:   e.message;  e.stack
来源：http://hz.shangyingyoupin.top/gtjririzgd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shanyushiyangtech.top/gttdfoflnd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.aizwys.cn/gtlsfbavge.html

Go:   err.Error()
来源：http://hz.hfpthk.cn/gtayldlkeb.html

Ruby: e.message;  e.backtrace
来源：http://hz.xuetiantiany.cn/gtpwgaaniq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jinghuilouyu.cn/gtwtqtmhgr.html

[H09] 带错误码的异常
来源：http://hz.zycfv.cn/gtlywwktnn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.chenlongwang.top/gtrjsyxltb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sweek.top/gtqujdvlki.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhongyouzk.top/gtxeiqejqw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.daria6918.cn/gtqneaugzi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xingfuxueyuan.xyz/gtzzejzxzh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.snrcjt.cn/gtaqpjumco.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.haohaochexian.top/gtlbdthntd.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yj20258.top/gtrhfozbst.html

[H10] 资源自动释放
来源：http://hz.mhx1999.top/gtcnnepbgp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xinyue.icu/gtbwshpvbz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jianghu66.top/gtvbkawvcs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuanzx.com/gtgkmymxgv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.pycfn.com/gtxxnwymsv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.havefunace.top/gtuqolicrf.html

Go:   defer f.Close()
来源：http://hz.zhaomingkeji.xyz/gtasuothgw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yongpay.top/gtgbujvdhl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ybcxt.top/gttjdwmmfk.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtkoigvynm.html

I. 正则表达式
来源：http://hz.iojbl.cn/gthuwqrftu.html

================================================================================
来源：http://hz.jlsjyb.cn/gthjvzucbd.html

[I01] 判断是否匹配
来源：http://hz.andypj.xyz/gteqhwszjz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yueranfly.top/gtbfepmchk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yuanzhike.top/gtfhgpjafk.html

JS:   /\d+/.test(s)
来源：http://hz.ehwqpu.com/gtvobmgajx.html

TS:   /\d+/.test(s)
来源：http://hz.chenjidiqi.icu/gtpzguacfz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zdqjudy.top/gtnzadaunm.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jiagoushi.top/gtheotejav.html

Ruby: s.match?(/\d+/)
来源：http://hz.havefunace.top/gtcfrrfvtg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hongshengwenyu.top/gtvgawjwcq.html

[I02] 提取所有匹配
来源：http://hz.yueranfly.top/gtkikqiydb.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ydjk.org.cn/gtwfujypgj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jinghuilouyu.cn/gtidnsrxbx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.nanxuanxn.top/gtqjoboozp.html

TS:   s.match(/\d+/g)
来源：http://hz.zhaomingkeji.xyz/gtrjusupqj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.vqdsnc.cn/gtpyizhkjj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zycfv.cn/gtmhixntfe.html

Ruby: s.scan(/\d+/)
来源：http://hz.nanxinkj.top/gtgxlttnzc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ydjk.org.cn/gtzstgkdrs.html

[I03] 提取捕获分组
来源：http://hz.pengpengdd.cyou/gturtketco.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhixingplan.top/gtxcmqskon.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.pengpengdd.cyou/gtzxncscml.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.daxiang520.top/gtyxzzsjbn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.fzhhl.top/gtyxnnptaq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gzhubu.top/gtdweesifi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhaomingkeji.xyz/gtvxzmzhvu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yj202588.top/gtmakqqdnh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.pengpengdd.cyou/gtqvnerfnn.html

[I04] 正则替换
来源：http://hz.0kj1m.cn/gttlqqnuzw.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.pengpengdd.cyou/gtndntxsbm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.aizwys.cn/gtznpvyjxe.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.feifeiyinyue.top/gtzookcvwe.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xinyue.icu/gtzcfymdxf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yonumen.top/gtyftwyvvl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jqgfzy.top/gthttewyor.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hnqzz.top/gtjobgixtv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.gaohongyu789.top/gtuahdkylz.html

[I05] 按正则拆分
来源：http://hz.dashuyun.cn/gtzzsrbwtm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xylfe.cn/gtbdsqjuoq.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ybcxt.top/gtyzncytpr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.nanxinkj.top/gtjoxfyvqn.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gogol.net.cn/gtztuwbrtv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.gogol.net.cn/gthwyhtayw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yueranfly.top/gtuyobroen.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gtcnfabqzd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.svipenyu.cn/gtpbskzegy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shangyingyoupin.top/gtvklzgjyc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinqigfzy.top/gtetifobuq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.meibo888.top/gteuoxcwqx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangdashe.top/gthzxfwxfv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tian-w.cn/gtbbykntcc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hammf.cn/gttvwqobik.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.birdmap.top/gtaxkrglet.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.chenzaomai.com/gteledqfgb.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhoulong.xyz/gteeasjdgl.html

[I07] 忽略大小写与多行模式
来源：http://hz.nanxinkj.top/gtieszydpb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.andypj.xyz/gtjznylvik.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhaomingkeji.xyz/gtqylkaynr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jqgfzy.top/gteoilzetv.html

TS:   /error/gim
来源：http://hz.hysaishi.cn/gtqkochtck.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.wangshuangyany.cn/gtxkxosica.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.haohaochexian.top/gtrplgatub.html

Ruby: s.scan(/error/i)
来源：http://hz.c1oappe.top/gtogvtvvzi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.pycfn.com/gtsbdpppmk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.xingfuxueyuan.xyz/gtcywzstry.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.wangshuangyany.cn/gtweniwscv.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yanxiufei.cn/gttcsmfxgu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.fengsongda.top/gtzxwznfvo.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenlongwang.top/gtnbjvwfzl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.haohaochexian.top/gtcsfgeivh.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yuanzhike.top/gtrpwcchpi.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.kuanghao11.cn/gtqinqvslz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhijiandao.cn/gtrtxbbaud.html

================================================================================
来源：http://hz.dianchejie.cn/gtvobcfvqa.html

J. 日期与时间
来源：http://hz.wangshuangyany.cn/gtrlsolkpf.html

================================================================================
来源：http://hz.fengsongda.top/gtvqzdvmtn.html

[J01] 获取当前时间
来源：http://hz.gogol.net.cn/gtthbbzldn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.9152youxi.cn/gtoqojskum.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yanxiufei.cn/gtdphtjizg.html

JS:   new Date();  Date.now()
来源：http://hz.yuxming.cn/gtpthniuhc.html

TS:   new Date();  Date.now()
来源：http://hz.tanke756.top/gtdfldvkhy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shangyingyoupin.top/gtvvoemwgf.html

Go:   time.Now()
来源：http://hz.cucudq.cn/gtjgvudejw.html

Ruby: Time.now
来源：http://hz.vqdsnc.cn/gtmqmazyse.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xingfuxueyuan.xyz/gtxpkvypxc.html

[J02] 格式化输出
来源：http://hz.yanxiufei.cn/gtwfouorve.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zdqjudy.top/gtbkfxqgdy.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jianghu66.top/gtpjoeyapd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shanyushiyangkeji.top/gtsuechtaz.html

TS:   d.toISOString()
来源：http://hz.cheryme.top/gtxggfouch.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zdqjudy.top/gtavhxtdro.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.bjfxy.top/gtkrddrbfc.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.guannengcc.top/gtlxkotzsq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.mhx1999.top/gtdkwwdytj.html

[J03] 字符串解析为日期
来源：http://hz.52xcode.cn/gtrjbtcpfj.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.daxiang520.top/gtwsbckhdb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.pycfn.com/gtrfblljim.html

JS:   new Date("2024-01-02")
来源：http://hz.zhijiandao.cn/gtwytdifwa.html

TS:   new Date("2024-01-02")
来源：http://hz.dianchejie.cn/gtydjpjzxu.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.vqdsnc.cn/gtsqwbemtm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.cdnleiting.top/gtwkpqbxyz.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shzxlz.cn/gtjmnzhlan.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yanxiufei.cn/gtadpjtimx.html

[J04] 时间戳与日期互转
来源：http://hz.bjfxy.top/gtormbcwdy.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.fzhhl.top/gtvxznpcoq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhiwuduotai.top/gtmczclcrr.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.52xcode.cn/gtjveinjhh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zycfv.cn/gtioavbdhu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.kuanghao11.cn/gtpsdfjxzz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhaomingkeji.xyz/gtsnziyjzs.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hongshengwenyu.top/gtsvaulhdw.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hongshengwenyu.top/gtvfnyuvsd.html

[J05] 时间加减（加 7 天）
来源：http://hz.jinyuanbaomall.cn/gtjlqfmccn.html

Py:   now + timedelta(days=7)
来源：http://hz.sysykeji.top/gttjtbzbeu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.pycfn.com/gtsuhtfsli.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shangyingyoupin.top/gtfhgczjci.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.52xcode.cn/gtotsqlapw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj20258.top/gtcmwsauie.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yonumen.top/gtwgngnndd.html

Ruby: Time.now + 7 * 86400
来源：http://hz.fzhhl.top/gtkuhwpltz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.52xcode.cn/gtgywlefoc.html

[J06] 计算两时间之差
来源：http://hz.guowangkeji.top/gtwgdzcriz.html

Py:   (end - start).total_seconds()
来源：http://hz.yueranfly.top/gtdyopvtgr.html

PHP:  $end->diff($start)->days;
来源：http://hz.sxryk.cn/gtfmazjoxf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.tanke756.top/gtqzustsav.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.316326.xyz/gttaixyawc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.dianchejie.cn/gtjnlkkepr.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhongyouzk.top/gtjlcxblps.html

Ruby: end - start                 # 返回秒数
来源：http://hz.feifeiyinyue.top/gtbhxafzjt.html

C#:   (end - start).TotalSeconds
来源：http://hz.yuxming.cn/gtlvkhyokq.html

[J07] 比较两个日期
来源：http://hz.quarkkingdee.top/gtpwygpxxa.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.meibo888.top/gtrvawqcqi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.haohaochexian.top/gtkiraamdr.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xuanzx.com/gtmrzvahde.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jiagoushi.top/gtmstijvmb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.gotoacloud.top/gtyzqqqdtj.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinghuilouyu.cn/gtidvynxun.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.mhx1999.top/gtzvuhfnax.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jqgufenzy.top/gtycvheesb.html

[J08] 提取年月日与星期
来源：http://hz.yanxiufei.cn/gtegsqqequ.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ehwqpu.com/gtlioucchm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.gotoacloud.top/gtfvievqrb.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sxryk.cn/gtcfxcaqgz.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.tian-w.cn/gtcnjzqqsr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cheryme.top/gtcocqcvvv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.dianchejie.cn/gtoblqcnko.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.aibaodan.cn/gtkzpamygz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.mhx1999.top/gtceaddgae.html

[J09] 时区处理
来源：http://hz.zhaomingkeji.xyz/gtoduvasau.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xingfuxueyuan.xyz/gtppaeqbxw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shanyushiyangkeji.top/gtdnnagqtn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.birdmap.top/gthcrhydnu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuxming.cn/gtqkmzxjnz.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.52xcode.cn/gtlamvpkqv.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sxryk.cn/gtmkbtzych.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xziqi.cn/gtlaaviseo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.redwolf501.top/gthhaboobh.html

[J10] 取今天 / 本月第一天
来源：http://hz.xylfe.cn/gtzywnorhg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jlsjyb.cn/gtwawoempq.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xinyue.icu/gtxmvcpzqz.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jqgfzy.top/gtgikjoefu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhongyouzk.top/gtkucwmiiy.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xuetiantiany.cn/gtloyereps.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hywenlv.cn/gtmjbpiiow.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.fengsongda.top/gtcgtauunk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yvedp.cn/gtxprafzsz.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtvpnwccpf.html

K. JSON 与序列化
来源：http://hz.aibaodan.cn/gtuarxwbmn.html

================================================================================
来源：http://hz.guowangkeji.top/gtlexqubul.html

[K01] 对象转 JSON 字符串
来源：http://hz.sufxvd.cn/gtfyqjilli.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.cashguo.top/gthevtrawq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.aizwys.cn/gtthgznmzn.html

JS:   JSON.stringify(obj)
来源：http://hz.dashuyun.cn/gtfyfumirh.html

TS:   JSON.stringify(obj)
来源：http://hz.cqqwz.cn/gtezksgcwm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yongpay.top/gtuvnrdxnm.html

Go:   json.Marshal(obj)
来源：http://hz.yonumen.top/gtlzqjvyse.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhongyouzk.top/gthvvrntuy.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.birdmap.top/gtunrcclxo.html

[K02] JSON 字符串转对象
来源：http://hz.gogol.net.cn/gtxowazxws.html

Py:   json.loads(s)
来源：http://hz.shuidangran.top/gtfzeqppli.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.nanxinkj.top/gtjsbdksgy.html

JS:   JSON.parse(s)
来源：http://hz.mhx1999.top/gtukjocbsm.html

TS:   JSON.parse(s)
来源：http://hz.chenjidiqi.icu/gtjhjqqnfs.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xylfe.cn/gtywcmvswq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.cdnleiting.top/gtzxbnwure.html

Ruby: JSON.parse(s)
来源：http://hz.sxryk.cn/gtelwkjtlu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ydzc1.top/gtygdkusxw.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yongpay.top/gtoietgwdp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shzxlz.cn/gtlbnpylpf.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yj20258888.top/gtmewweftg.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yuxming.cn/gtzddmzsxb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cdnleiting.top/gtovqgonju.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.zycfv.cn/gtavpfhybz.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.pycfn.com/gtdsncqpfq.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.sxryk.cn/gtzslzngof.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.xingfuxueyuan.xyz/gtgisykxpr.html

[K04] 读取 JSON 文件
来源：http://hz.guowangkeji.top/gtmevcdnbu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.wangdashe.top/gtmzzncvkm.html


<!-- 参考信息 -->