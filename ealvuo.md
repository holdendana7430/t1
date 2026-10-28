代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://hz.nanxinkj.top/gtlmfunwtn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shzxlz.cn/gtyengfijt.html

[G16] 对象转数组 / 字典
来源：http://hz.hammf.cn/gtmodwghnq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.gaohongyu789.top/gthwiiydta.html

PHP:  get_object_vars($obj);
来源：http://hz.gogol.net.cn/gtasenapmq.html

JS:   Object.entries(obj)
来源：http://hz.xziqi.cn/gtxrgczuew.html

TS:   Object.entries(obj)
来源：http://hz.jqgfzy.top/gtvagesjxh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xziqi.cn/gtqljdwbwm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.chenzaomai.com/gtpcisztim.html

Ruby: obj.instance_variables
来源：http://hz.zhijiandao.cn/gttfynxnyr.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhaomingkeji.xyz/gtcuefcpiu.html

================================================================================
来源：http://hz.yj202588.top/gtoaepnccy.html

H. 异常与错误处理
来源：http://hz.pycfn.com/gtufpyyatc.html

================================================================================
来源：http://hz.hammf.cn/gtqjplydvr.html

[H01] try / catch 基础
来源：http://hz.ppjwa.cn/gtjhodhgye.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jiagoushi.top/gtplmfpsjb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xinyue.icu/gtldaacbwa.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhiwuduotai.top/gtahpwarfd.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jyoumei.cn/gtyscfmdhg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.aibaodan.cn/gtnlrsgkrc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.dianchejie.cn/gtlivkmkzd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sxryk.cn/gtfemqaljj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.guowangkeji.top/gtymucpfyw.html

[H02] finally / ensure 收尾
来源：http://hz.sweek.top/gtahbpgarj.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sysykeji.top/gttlhyssyg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtcwwgyngh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtoncgpsxg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gtaiqfkhmh.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtntunnftp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xziqi.cn/gtdvjawpkv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.birdmap.top/gttrvnodsn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.iojbl.cn/gtpxtvmiym.html

[H03] 主动抛出异常
来源：http://hz.9152youxi.cn/gtqjnvvete.html

Py:   raise ValueError("错误信息")
来源：http://hz.jyoumei.cn/gttqflivib.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xziqi.cn/gteeziuxsr.html

JS:   throw new Error("错误信息");
来源：http://hz.zhoulong.xyz/gttizjdemw.html

TS:   throw new Error("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtpggrrfoc.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.wangshuangyany.cn/gtyumksped.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hysaishi.cn/gtrcalkrse.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nwbrower.top/gtgoedxpsc.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cqqwz.cn/gtntvpplgn.html

[H04] 自定义异常类型
来源：http://hz.hysaishi.cn/gtoewqrozp.html

Py:   class MyError(Exception): pass
来源：http://hz.iojbl.cn/gtkmnffpwl.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.iojbl.cn/gtuwryidnm.html

JS:   class MyError extends Error {}
来源：http://hz.hywenlv.cn/gtteqosytz.html

TS:   class MyError extends Error {}
来源：http://hz.52xcode.cn/gtuqghwhyn.html

Java: class MyException extends RuntimeException {}
来源：http://hz.fengsongda.top/gtinvlzfdj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.daxiang520.top/gttsjkgxoh.html

Ruby: class MyError < StandardError; end
来源：http://hz.yangfankeji.com/gttrwjjkeo.html

C#:   class MyException : Exception {}
来源：http://hz.smart0.xyz/gtxvdssmrd.html

[H05] 捕获特定类型
来源：http://hz.wangshuangyany.cn/gtlirineyl.html

Py:   except ValueError as e:
来源：http://hz.zdqjudy.top/gtwxtqwchx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zdqjudy.top/gtqubgpenv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.feifeiyinyue.top/gtehamgdgy.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.svipenyu.cn/gtfklxglmy.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yvedp.cn/gtgouulzev.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shanyushiyangtech.top/gtmdmnjojs.html

Ruby: rescue ArgumentError => e
来源：http://hz.yueranfly.top/gtopvmhfna.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhongyouzk.top/gtcajiqtno.html

[H06] 可选值 / 空值安全访问
来源：http://hz.smart0.xyz/gthpvyluaq.html

Py:   value = d.get("k") or default
来源：http://hz.xuetiantiany.cn/gtqvhwrlje.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhijiandao.cn/gtvprliwif.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhoulong.xyz/gtxyzuauyd.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ywan-chungtsiang.top/gtgoyqsaey.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.52xcode.cn/gtbikodwow.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhaomingkeji.xyz/gtccygdbxt.html

Ruby: d&.dig(:a, :b)
来源：http://hz.chenzaomai.com/gtwqioyeoq.html

C#:   obj?.A?.B ?? default
来源：http://hz.hfpthk.cn/gtkyuemfht.html

[H07] 断言
来源：http://hz.quarkkingdee.top/gtpwejnbai.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hnqzz.top/gtipojrzzd.html

PHP:  assert($x > 0);
来源：http://hz.jinqigfzy.top/gtnncsdydc.html

JS:   console.assert(x > 0);
来源：http://hz.316326.xyz/gteqtlhcmy.html

TS:   console.assert(x > 0);
来源：http://hz.fengsongda.top/gtgeiedpbu.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shanyushiyangkeji.top/gtruriwqzc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yongpay.top/gtsonquhed.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhengqikj.top/gtggqamcqw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jlsjyb.cn/gtabpkhisp.html

[H08] 获取错误信息与堆栈
来源：http://hz.wangshuangyany.cn/gtwpyrfwdn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.dashuyun.cn/gtnhvksqsh.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.guowangkeji.top/gtyvkgrxbs.html

JS:   e.message;  e.stack
来源：http://hz.xziqi.cn/gtjalnbyin.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yuxming.cn/gtkaaujlov.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cashguo.top/gtjetlircb.html

Go:   err.Error()
来源：http://hz.chenzaomai.com/gtubgoqpfc.html

Ruby: e.message;  e.backtrace
来源：http://hz.ydzc1.top/gtojwhelgl.html

C#:   e.Message;  e.StackTrace
来源：http://hz.kuanghao11.cn/gtaqodcufz.html

[H09] 带错误码的异常
来源：http://hz.jqgfzy.top/gtmdriovut.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.haohaochexian.top/gthnhfhvyg.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.guannengcc.top/gtamkhpsyb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhiwuduotai.top/gtqbaqymoh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xziqi.cn/gtyajgqfrp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj20258888.top/gthcugtkth.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hnqzz.top/gtozrpladv.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jinqigufen.top/gtgicoepst.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.chenlongwang.top/gttpdekzmr.html

[H10] 资源自动释放
来源：http://hz.dashuyun.cn/gtkgjvpfxa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.chenjidiqi.icu/gtzzqpjdue.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jiagoushi.top/gtlcrqffbv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zycfv.cn/gtxksypthn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dianchejie.cn/gtanxkqcdu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.daria6918.cn/gtwnxfmptd.html

Go:   defer f.Close()
来源：http://hz.cheryme.top/gtlfszkudv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinghuilouyu.cn/gtpznlxtoi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.kuanghao11.cn/gtmjkzweyn.html

================================================================================
来源：http://hz.ydzc1.top/gtvbzipvke.html

I. 正则表达式
来源：http://hz.ydzc1.top/gtxuyjemzy.html

================================================================================
来源：http://hz.jqgufenzy.top/gtandwndec.html

[I01] 判断是否匹配
来源：http://hz.jinqigfzy.top/gtawkdpwyq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xuetiantiany.cn/gtmcfsgroc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gzhubu.top/gtooxuumdk.html

JS:   /\d+/.test(s)
来源：http://hz.fengsongda.top/gtukyhjxdx.html

TS:   /\d+/.test(s)
来源：http://hz.pycfn.com/gtlptezzqh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhixingplan.top/gtpxdyvmyt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.bjfxy.top/gtugicvnqi.html

Ruby: s.match?(/\d+/)
来源：http://hz.andypj.xyz/gtmtsqpxto.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.pengpengdd.cyou/gthskpllmi.html

[I02] 提取所有匹配
来源：http://hz.ppjwa.cn/gtaapafdbu.html

Py:   re.findall(r"\d+", s)
来源：http://hz.dashuyun.cn/gtbzerxsyq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhoulong.xyz/gtetlghqjs.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yuanzhike.top/gthtdptfnb.html

TS:   s.match(/\d+/g)
来源：http://hz.ivvv.top/gtvnculrbo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shuidangran.top/gtetlusloi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hywenlv.cn/gtudxvitxb.html

Ruby: s.scan(/\d+/)
来源：http://hz.shanyushiyangkeji.top/gtjadofhhq.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hnxiangtu.top/gtrjtyctrx.html

[I03] 提取捕获分组
来源：http://hz.xylfe.cn/gtnwruszqs.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhiwuduotai.top/gtoidmpwon.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hammf.cn/gtzojnqiua.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yvedp.cn/gtpbyvnoui.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ydzc1.top/gtnygtbiru.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.smart0.xyz/gthvzsmqlr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.sxryk.cn/gtrrflgezy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.wangshuangyany.cn/gtwbcodrdz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jinyuanbaomall.cn/gtogsjziae.html

[I04] 正则替换
来源：http://hz.hongshengwenyu.top/gtrebufkol.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jianghu66.top/gtjovmbkic.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sweek.top/gtelzbqhbd.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shangyingyoupin.top/gtfyxshuwx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.redwolf501.top/gtrmcmnwra.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhongyouzk.top/gtntalqxst.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shuidangran.top/gtuzclqzjt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.quarkkingdee.top/gtnowtlqts.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.kuanghao11.cn/gthhztlqqx.html

[I05] 按正则拆分
来源：http://hz.birdmap.top/gtbhsianlq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jinyuanbaomall.cn/gtqzzvsxxb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xuetiantiany.cn/gtcpzibidf.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.cdnleiting.top/gteyyyipcp.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jinqigfzy.top/gthwpzhvxc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hnxiangtu.top/gtkgogjome.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zhoulong.xyz/gtihzxuwpz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yvedp.cn/gtrkxtpadr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhaomingkeji.xyz/gtipvmscrr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.fengsongda.top/gtvusicutj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.tianlin.xyz/gtdepucdmp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.fengsongda.top/gtvtoogntk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258.top/gtjnrwjimz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.guowangkeji.top/gtunmrlytz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.dianchejie.cn/gtvjanfrhi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.quarkkingdee.top/gtmllbymka.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shzxlz.cn/gthablyrix.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.redwolf501.top/gtfvvuntsu.html

[I07] 忽略大小写与多行模式
来源：http://hz.redwolf501.top/gtxmyuswwa.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.wangshuangyany.cn/gtttcvente.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yangfankeji.com/gtlgubozwv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.guannengcc.top/gtxemsaghd.html

TS:   /error/gim
来源：http://hz.quarkkingdee.top/gtlklymbvf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.kuanghao11.cn/gttzzywzxx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hnqzz.top/gtcdvgteix.html

Ruby: s.scan(/error/i)
来源：http://hz.xylfe.cn/gtnmjcrymg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj202588.top/gtwenhhwsn.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.chenzaomai.com/gtnsjpzjux.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhengqikj.top/gtzblmrfiy.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yueranfly.top/gtegurtghn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xingfuxueyuan.xyz/gtbwnhegyh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangkeji.top/gtveyuhqtk.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.hysaishi.cn/gtmcxsisrx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yvedp.cn/gtpwebemrn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhixingplan.top/gtyqloqowf.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.pengpengdd.cyou/gtlidmkhay.html

================================================================================
来源：http://hz.yuxming.cn/gtpfalyakb.html

J. 日期与时间
来源：http://hz.shzxlz.cn/gtgsjfalgj.html

================================================================================
来源：http://hz.gaohongyu789.top/gtitjlijka.html

[J01] 获取当前时间
来源：http://hz.zhengqikj.top/gtwsstnkju.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenlongwang.top/gtiyplzvhd.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jinyuanbaomall.cn/gtnwtjcmwu.html

JS:   new Date();  Date.now()
来源：http://hz.xylfe.cn/gtyfepqrzj.html

TS:   new Date();  Date.now()
来源：http://hz.sxryk.cn/gterhlleti.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cheryme.top/gtkfyicaxz.html

Go:   time.Now()
来源：http://hz.yuxming.cn/gtnlcyzqyo.html

Ruby: Time.now
来源：http://hz.cqqwz.cn/gtufyzfvdd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.pycfn.com/gtckzyehzd.html

[J02] 格式化输出
来源：http://hz.yj20258888.top/gtjaqnsmeb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.0kj1m.cn/gtootzgflh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jinqigfzy.top/gtbrfhpndv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhengqikj.top/gtrxgszmto.html

TS:   d.toISOString()
来源：http://hz.tianlin.xyz/gtuapyefhr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yuanzhike.top/gtstpwfihw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ywan-chungtsiang.top/gttnnapaip.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yuanzhike.top/gtqdhvulpo.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.aibaodan.cn/gtxnscnpzq.html

[J03] 字符串解析为日期
来源：http://hz.gaohongyu789.top/gtvxnaxwwl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.aibaodan.cn/gthbbklluz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hywenlv.cn/gtiewhsjvo.html

JS:   new Date("2024-01-02")
来源：http://hz.gotoacloud.top/gtxexamlln.html

TS:   new Date("2024-01-02")
来源：http://hz.cdnleiting.top/gtbwgffiqh.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.cucudq.cn/gtuwezgrgf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ydzc1.top/gtwhzuinjg.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jiagoushi.top/gtaarksazp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.gzhubu.top/gtodzrnttt.html

[J04] 时间戳与日期互转
来源：http://hz.chenlongwang.top/gtodufqzwl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cheryme.top/gthltmnxsg.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.fengsongda.top/gtrtcdvxmb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.nanxinkj.top/gtlozbylmc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.xuanzx.com/gteiiivckz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xinyue.icu/gtptcjpxjn.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.bjfxy.top/gtbkpvpvml.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shanyushiyangkeji.top/gtcmmhieqk.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhoulong.xyz/gtncnzbrrv.html

[J05] 时间加减（加 7 天）
来源：http://hz.xuanzx.com/gtbsrnrdfb.html

Py:   now + timedelta(days=7)
来源：http://hz.chenlongwang.top/gtasztdavy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jqgfzy.top/gtytolycvc.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ppjwa.cn/gtccwqjyjq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhixingplan.top/gtrvcqhukw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhengqikj.top/gtmzizmnai.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.aibaodan.cn/gtinvmczbx.html

Ruby: Time.now + 7 * 86400
来源：http://hz.fengsongda.top/gtpctiarcw.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.smart0.xyz/gtrqkaxctz.html

[J06] 计算两时间之差
来源：http://hz.ydjk.org.cn/gtjagazlhy.html

Py:   (end - start).total_seconds()
来源：http://hz.ppjwa.cn/gtlpprjiwf.html

PHP:  $end->diff($start)->days;
来源：http://hz.jianghu66.top/gtwkwgrizy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zycfv.cn/gtldinflkg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.chenlongwang.top/gtmhmlopfe.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.c1oappe.top/gtvgyubsib.html

Go:   end.Sub(start).Hours()
来源：http://hz.yongpay.top/gtbumwqcsn.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sufxvd.cn/gtjwvwcyry.html

C#:   (end - start).TotalSeconds
来源：http://hz.chenzaomai.com/gtcogdwmqv.html

[J07] 比较两个日期
来源：http://hz.ehwqpu.com/gtcfwthtbf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.dashuyun.cn/gtqwtihspx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.pengpengdd.cyou/gtllwxrsvy.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jianghu66.top/gtwycotvbm.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cqqwz.cn/gtakfffdnj.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xziqi.cn/gtlznefhar.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinyuanbaomall.cn/gtczawhxkv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.dianchejie.cn/gtymphodsc.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.tian-w.cn/gtuhxvkvim.html

[J08] 提取年月日与星期
来源：http://hz.meibo888.top/gtcheldppi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ydjk.org.cn/gtwqrkkdsc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.ppjwa.cn/gttzwnimvi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sysykeji.top/gtlmjgnvhu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.cqqwz.cn/gtxczjjlou.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.sufxvd.cn/gtlmfhumkq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.birdmap.top/gtoesqvofe.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.nanxinkj.top/gtkibbkbcr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shuidangran.top/gtygnziydx.html

[J09] 时区处理
来源：http://hz.xuetiantiany.cn/gtdlxblbqk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yj202588.top/gttzwneljn.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.vqdsnc.cn/gtnsucsvox.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258.top/gtyxqfydbq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shanyushiyangkeji.top/gtrlihtqtl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hysaishi.cn/gtgfjuhphp.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.feifeiyinyue.top/gtvvrsyedc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.dashuyun.cn/gtdegcbirf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.aizwys.cn/gtbpujhzgg.html

[J10] 取今天 / 本月第一天
来源：http://hz.chenlongwang.top/gtsnrawlzf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hammf.cn/gtimzwrhfv.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.pengpengdd.cyou/gtrzbekwhi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yuxming.cn/gtpflqhsri.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gaohongyu789.top/gteefoqyvd.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhixingplan.top/gtuhqfqjvh.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.zhaomingkeji.xyz/gtvupjhnqg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.bjfxy.top/gtkigtpfbn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hnqzz.top/gtzxsnzlhf.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtghigouft.html

K. JSON 与序列化
来源：http://hz.kuanghao11.cn/gtmbgcsrjj.html

================================================================================
来源：http://hz.hywenlv.cn/gtupkopsyz.html

[K01] 对象转 JSON 字符串
来源：http://hz.xinyue.icu/gtzglufank.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.andypj.xyz/gtsbgzrzak.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jianghu66.top/gtjawuxlmq.html

JS:   JSON.stringify(obj)
来源：http://hz.xuetiantiany.cn/gtzoiozszs.html

TS:   JSON.stringify(obj)
来源：http://hz.kuanghao11.cn/gtqlhnrpcp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.mhx1999.top/gtubewvywb.html

Go:   json.Marshal(obj)
来源：http://hz.birdmap.top/gtacfglivg.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.andypj.xyz/gtdvnocdyq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.cqqwz.cn/gtlxxkshjl.html

[K02] JSON 字符串转对象
来源：http://hz.sufxvd.cn/gthylwgzfx.html

Py:   json.loads(s)
来源：http://hz.nanxuanxn.top/gtejyhhrwr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.shangyingyoupin.top/gtzhzgpvuf.html

JS:   JSON.parse(s)
来源：http://hz.xinyue.icu/gtidgcyyax.html

TS:   JSON.parse(s)
来源：http://hz.shanyushiyangtech.top/gtpuqnqdoa.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yj20258888.top/gtllyxsbhi.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.guannengcc.top/gteuaqsrvo.html

Ruby: JSON.parse(s)
来源：http://hz.shanyushiyangtech.top/gtvltybveo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xuetiantiany.cn/gtxqrbpmcr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.xuanzx.com/gtyhezbpry.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yangfankeji.com/gtnvkvdbol.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.fengsongda.top/gtlpcelmfz.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.yj20258.top/gtrptaptvg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.jiagoushi.top/gtghctrmaf.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.52xcode.cn/gtrueaynhm.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.redwolf501.top/gtmetzefpp.html


<!-- 参考信息 -->