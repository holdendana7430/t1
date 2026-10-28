代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yj202588.top/gtjltxtama.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.0kj1m.cn/gtiajictfs.html

Java: enum Color { RED, GREEN }
来源：http://hz.daria6918.cn/gtlnfnktua.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.ppjwa.cn/gtslcgtddm.html

Ruby: Color = %i[red green].freeze
来源：http://hz.guowangkeji.top/gtbexuqsmz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhengqikj.top/gtyhpfbnet.html

[G16] 对象转数组 / 字典
来源：http://hz.chenzaomai.com/gtihpindxu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hammf.cn/gtrjhnbkdh.html

PHP:  get_object_vars($obj);
来源：http://hz.svipenyu.cn/gtxydskqsn.html

JS:   Object.entries(obj)
来源：http://hz.yj202588.top/gtnlnckofn.html

TS:   Object.entries(obj)
来源：http://hz.hnxiangtu.top/gtvepkbxwx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.pycfn.com/gtfzkplmrk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shuidangran.top/gttofsksxg.html

Ruby: obj.instance_variables
来源：http://hz.yj20258888.top/gterxaujuj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hnxiangtu.top/gtkgzkoenw.html

================================================================================
来源：http://hz.hongshengwenyu.top/gttfcmrgol.html

H. 异常与错误处理
来源：http://hz.cdnleiting.top/gtqgcfdkiu.html

================================================================================
来源：http://hz.yueranfly.top/gtnzmnqykb.html

[H01] try / catch 基础
来源：http://hz.jinqigufen.top/gtmvzsgrqt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hysaishi.cn/gtmzoggoml.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yj202588.top/gtfdsmgbfq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.quarkkingdee.top/gtdvgwqnfs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.haohaochexian.top/gtbxwbtzxy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xuetiantiany.cn/gtmwvaotqf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhaomingkeji.xyz/gtkhfscyxg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.sweek.top/gtekelltyy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.ivvv.top/gtkmplidmu.html

[H02] finally / ensure 收尾
来源：http://hz.bjfxy.top/gtoajlzmru.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yueranfly.top/gtnmlolmod.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtwgcivrcx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.hfpthk.cn/gtfgfkgnju.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtvpkkvyku.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.havefunace.top/gthirotkva.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yangfankeji.com/gtnrnaoslm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhoulong.xyz/gtejgmeopx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jyoumei.cn/gthgkrmygd.html

[H03] 主动抛出异常
来源：http://hz.haohaochexian.top/gtjnxypmkn.html

Py:   raise ValueError("错误信息")
来源：http://hz.0kj1m.cn/gtlrsqfgbn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xylfe.cn/gtpilyepwm.html

JS:   throw new Error("错误信息");
来源：http://hz.jlsjyb.cn/gtzodcwncv.html

TS:   throw new Error("错误信息");
来源：http://hz.ivvv.top/gtkgguxigq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jqgufenzy.top/gttznuuhrd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hnxiangtu.top/gtwlaswzhi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhengqikj.top/gtgzomeuar.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.chenlongwang.top/gtaumichwa.html

[H04] 自定义异常类型
来源：http://hz.jlsjyb.cn/gtgqbvuzlo.html

Py:   class MyError(Exception): pass
来源：http://hz.mhx1999.top/gtogtitwty.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhoulong.xyz/gtlitcrjgo.html

JS:   class MyError extends Error {}
来源：http://hz.haohaochexian.top/gtldxbrzcd.html

TS:   class MyError extends Error {}
来源：http://hz.shanyushiyangtech.top/gtcyxrxucu.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ehwqpu.com/gtuqbfkcsb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xingfuxueyuan.xyz/gtyrkqrlpo.html

Ruby: class MyError < StandardError; end
来源：http://hz.yangfankeji.com/gtbeypmvsa.html

C#:   class MyException : Exception {}
来源：http://hz.zhiwuduotai.top/gtyodowilh.html

[H05] 捕获特定类型
来源：http://hz.snrcjt.cn/gthyldadfi.html

Py:   except ValueError as e:
来源：http://hz.xziqi.cn/gtzreapycp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.nwbrower.top/gtpvsaqspl.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.feifeiyinyue.top/gtfnpcxtrz.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jlsjyb.cn/gtgnjrxtbb.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zycfv.cn/gtuxxbmrvv.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.cqqwz.cn/gtzhtvofuz.html

Ruby: rescue ArgumentError => e
来源：http://hz.snrcjt.cn/gtsrmtwbcf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.svipenyu.cn/gtjdkibpbo.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hysaishi.cn/gtraovgplg.html

Py:   value = d.get("k") or default
来源：http://hz.chenzaomai.com/gtxplqdoab.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.cheryme.top/gttycahauf.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.chenlongwang.top/gtezxxuxyr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.nwbrower.top/gtiawgidnc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ywan-chungtsiang.top/gtijmbwbza.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sufxvd.cn/gtgsvgkrqt.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hfpthk.cn/gtyeijjmkg.html

C#:   obj?.A?.B ?? default
来源：http://hz.shangyingyoupin.top/gtshhjvhsz.html

[H07] 断言
来源：http://hz.nanxinkj.top/gtneahdvgv.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hnxiangtu.top/gtwfrsmaaa.html

PHP:  assert($x > 0);
来源：http://hz.andypj.xyz/gtxcmrxdzk.html

JS:   console.assert(x > 0);
来源：http://hz.316326.xyz/gtombkyqgc.html

TS:   console.assert(x > 0);
来源：http://hz.yueranfly.top/gtfqaxilil.html

Java: assert x > 0 : "必须为正";
来源：http://hz.guannengcc.top/gtydrmtlfd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.zhixingplan.top/gthexpkdex.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhoulong.xyz/gtpkxmtkpv.html

C#:   Debug.Assert(x > 0);
来源：http://hz.c1oappe.top/gtaufwoyxf.html

[H08] 获取错误信息与堆栈
来源：http://hz.jlsjyb.cn/gtpxinnhgs.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.wangshuangyany.cn/gtszeuehem.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yj20258.top/gtnewuebxh.html

JS:   e.message;  e.stack
来源：http://hz.52xcode.cn/gtyuxhsbyq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zycfv.cn/gtakjmcqor.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.mhx1999.top/gtxqotchnc.html

Go:   err.Error()
来源：http://hz.yueranfly.top/gtxutmwzmj.html

Ruby: e.message;  e.backtrace
来源：http://hz.snrcjt.cn/gtfhavxrtb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yongpay.top/gtxnngrmyp.html

[H09] 带错误码的异常
来源：http://hz.tanke756.top/gtrsalvhab.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.chenjidiqi.icu/gtwqwulaaj.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.hongshengwenyu.top/gtjxawoacl.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jinqigufen.top/gtivygytci.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.jinqigfzy.top/gtkrwatusb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.haohaochexian.top/gtizbozrsx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yj20258.top/gttzhpewxy.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.nwbrower.top/gtqywqhpaf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ehwqpu.com/gtgjszfjcq.html

[H10] 资源自动释放
来源：http://hz.xuanzx.com/gtesaqxcjb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yvedp.cn/gtxotnmkmm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhoulong.xyz/gtblxvozrl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuxming.cn/gthsuepnfc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigufen.top/gtyrzrsezf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.52xcode.cn/gtseqrumcp.html

Go:   defer f.Close()
来源：http://hz.fzhhl.top/gtsyfpxxdt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yj20258888.top/gtpufvzdbd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ybcxt.top/gtrlugbsja.html

================================================================================
来源：http://hz.gzhubu.top/gtmntvurzb.html

I. 正则表达式
来源：http://hz.jinghuilouyu.cn/gtseytofnq.html

================================================================================
来源：http://hz.vqdsnc.cn/gtddmyoexy.html

[I01] 判断是否匹配
来源：http://hz.cheryme.top/gtpadflmwn.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.aizwys.cn/gtmhfhmbpr.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yj20258.top/gtfuqfbhss.html

JS:   /\d+/.test(s)
来源：http://hz.cucudq.cn/gtcccqyxaj.html

TS:   /\d+/.test(s)
来源：http://hz.cqqwz.cn/gtmwjkqvfb.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.redwolf501.top/gtmefancsc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.tanke756.top/gtsrrwxolt.html

Ruby: s.match?(/\d+/)
来源：http://hz.nwbrower.top/gtucxczpnb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.feifeiyinyue.top/gtxxouesxr.html

[I02] 提取所有匹配
来源：http://hz.yanxiufei.cn/gtzdppcaja.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhixingplan.top/gtsalrslou.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jianghu66.top/gtxmdnogdm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ydzc1.top/gtibwpelws.html

TS:   s.match(/\d+/g)
来源：http://hz.fengsongda.top/gtxyypnbng.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinqigfzy.top/gtwxbfwbfv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shanyushiyangkeji.top/gtenmyxxbq.html

Ruby: s.scan(/\d+/)
来源：http://hz.xylfe.cn/gtmsohxcbs.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhoulong.xyz/gtwvnxxxqk.html

[I03] 提取捕获分组
来源：http://hz.chenjidiqi.icu/gtyslhmyzk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yvedp.cn/gtpyurcngh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.daria6918.cn/gtvbwyfjky.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.nanxuanxn.top/gtitewgvzo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yj20258888.top/gtxbfcsubz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhongyouzk.top/gtmecuroph.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.nanxinkj.top/gtuhibgnmz.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xinyue.icu/gtbaamogzn.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.sufxvd.cn/gtufihgbll.html

[I04] 正则替换
来源：http://hz.xylfe.cn/gtnovvmgpa.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.birdmap.top/gtmjhpwmpy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.iojbl.cn/gtjunmgslz.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cucudq.cn/gtcsrqhfwc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xinyue.icu/gtjlmvlavx.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xinyue.icu/gtocdjkdnu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhongyouzk.top/gtkdkfznah.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.wangshuangyany.cn/gtjbucnutm.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.bjfxy.top/gtvdqpbglh.html

[I05] 按正则拆分
来源：http://hz.xinyue.icu/gttdovfylw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jinqigufen.top/gtnhsckznf.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.chenjidiqi.icu/gtufqeudof.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangkeji.top/gtpljrszfa.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.wangshuangyany.cn/gtxdybvsof.html

Java: s.split("\\s*,\\s*")
来源：http://hz.daxiang520.top/gtcmloruaw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.cashguo.top/gtreydsxsb.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhongyouzk.top/gtmazbpsoo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.dianchejie.cn/gtbccybvrn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yuanzhike.top/gtuyzsfigq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.gogol.net.cn/gtbjhvegkd.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.daria6918.cn/gtmefnvuvz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jlsjyb.cn/gtjcuziiae.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gaohongyu789.top/gtjwoxbbkn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yonumen.top/gtuyiaxpfz.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.wangshuangyany.cn/gtxkrihwah.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jianghu66.top/gtwuihdmkf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.tianlin.xyz/gtzkkdpcdf.html

[I07] 忽略大小写与多行模式
来源：http://hz.316326.xyz/gtgfqrazna.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.vqdsnc.cn/gtcyfuyyaq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.ivvv.top/gtecofxyqs.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shanyushiyangtech.top/gtkjmpzisf.html

TS:   /error/gim
来源：http://hz.daxiang520.top/gtabltkxdu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.fzhhl.top/gtrsmyapfo.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.guowangkeji.top/gticfrebmv.html

Ruby: s.scan(/error/i)
来源：http://hz.ydjk.org.cn/gteezvnoye.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinqigfzy.top/gtlmsdroda.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.birdmap.top/gtzcxcrtjv.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.tian-w.cn/gtcjwgmolh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.sufxvd.cn/gtabnpnthf.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xinyue.icu/gttpejcebl.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shzxlz.cn/gtkryxmbeo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.chenlongwang.top/gtvmroqarc.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.wangshuangyany.cn/gtdmblyvji.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.shzxlz.cn/gtlpmixihr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.fengsongda.top/gtpcbxxssn.html

================================================================================
来源：http://hz.52xcode.cn/gtagfmthdg.html

J. 日期与时间
来源：http://hz.yj202588.top/gtyxjpwvqf.html

================================================================================
来源：http://hz.9152youxi.cn/gtcartrsvq.html

[J01] 获取当前时间
来源：http://hz.jlsjyb.cn/gtdjrbnxuv.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.quarkkingdee.top/gtoztgzjdp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.chenjidiqi.icu/gtqcjrurxf.html

JS:   new Date();  Date.now()
来源：http://hz.chenzaomai.com/gtsakcugwq.html

TS:   new Date();  Date.now()
来源：http://hz.smart0.xyz/gtewkfpuja.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zycfv.cn/gtmoltcoya.html

Go:   time.Now()
来源：http://hz.kuanghao11.cn/gtzvfpmxad.html

Ruby: Time.now
来源：http://hz.zdqjudy.top/gtqvuhlekj.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.nanxuanxn.top/gtmmmwitbs.html

[J02] 格式化输出
来源：http://hz.gogol.net.cn/gthiuowjda.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxuanxn.top/gtiwnwaylq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xingfuxueyuan.xyz/gtkesqevsf.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xinyue.icu/gtnrvsboet.html

TS:   d.toISOString()
来源：http://hz.ydzc1.top/gtcnmcknzo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhixingplan.top/gtkaarmlxm.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ivvv.top/gtmeocnrcl.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fengsongda.top/gtfxtsabde.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yueranfly.top/gtpksnvxqk.html

[J03] 字符串解析为日期
来源：http://hz.pengpengdd.cyou/gtrbyjensl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ywan-chungtsiang.top/gtnioxodcm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.chenlongwang.top/gtivncxery.html

JS:   new Date("2024-01-02")
来源：http://hz.ydzc1.top/gtwdmnmhvy.html

TS:   new Date("2024-01-02")
来源：http://hz.aizwys.cn/gtqhwcbxwj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.zdqjudy.top/gtjnmvlajn.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ydzc1.top/gtxgrgohfe.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.svipenyu.cn/gtmpntknzh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.svipenyu.cn/gtkwnrbdnx.html

[J04] 时间戳与日期互转
来源：http://hz.gaohongyu789.top/gtopnxyxkm.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.nanxinkj.top/gtribgjsvt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhoulong.xyz/gttnugmeuy.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sysykeji.top/gtngidfblb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jiagoushi.top/gtjrzwoauy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yanxiufei.cn/gtyjvqjvnt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.316326.xyz/gteyaokrfj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.smart0.xyz/gtfgjrheol.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shanyushiyangtech.top/gtgchwbinc.html

[J05] 时间加减（加 7 天）
来源：http://hz.quarkkingdee.top/gtdjvtvqlh.html

Py:   now + timedelta(days=7)
来源：http://hz.jqgfzy.top/gtejuloeyb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.guannengcc.top/gtdosrexsg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhengqikj.top/gtjbbxwzzk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xinyue.icu/gtiwpucryq.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.quarkkingdee.top/gtnchhcecl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.havefunace.top/gtgdrdnlwy.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yonumen.top/gtlepacazn.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xingfuxueyuan.xyz/gtafszlqql.html

[J06] 计算两时间之差
来源：http://hz.zhongyouzk.top/gtwcnrvwld.html

Py:   (end - start).total_seconds()
来源：http://hz.yanxiufei.cn/gtarfnysfw.html

PHP:  $end->diff($start)->days;
来源：http://hz.9152youxi.cn/gtglqjyqlz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.smart0.xyz/gtkfhqlobr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.xziqi.cn/gtknmzytny.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hfpthk.cn/gtaypmurdz.html

Go:   end.Sub(start).Hours()
来源：http://hz.hnqzz.top/gtxprhoerg.html

Ruby: end - start                 # 返回秒数
来源：http://hz.kuanghao11.cn/gtwbqpypxc.html

C#:   (end - start).TotalSeconds
来源：http://hz.ybcxt.top/gtveadmtbu.html

[J07] 比较两个日期
来源：http://hz.hnqzz.top/gtijhbrpww.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gtrpfrnrcm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.aibaodan.cn/gtnfxvniuy.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.iojbl.cn/gtovckdlgw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gaohongyu789.top/gtnfitebzv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.bjfxy.top/gtjgvlxisv.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinyuanbaomall.cn/gtigoniect.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.pengpengdd.cyou/gtfqxfebwz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cdnleiting.top/gtcaxycodv.html

[J08] 提取年月日与星期
来源：http://hz.hnxiangtu.top/gtdsikikfo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.svipenyu.cn/gttvzuywbk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yj202588.top/gtispfrtzh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.bjfxy.top/gtrxrdqdcf.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.cucudq.cn/gtprkvunht.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhoulong.xyz/gtotrfcxec.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.daria6918.cn/gtgcrbfelp.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.0kj1m.cn/gtpyhwsbqq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xziqi.cn/gtlatfgkmd.html

[J09] 时区处理
来源：http://hz.xinyue.icu/gtsxblpuoe.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yanxiufei.cn/gtrjoannwa.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.tianlin.xyz/gtbcupeueu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuanzhike.top/gtzezoefvr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenlongwang.top/gtwjigaokf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jlsjyb.cn/gtbuchogbt.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.tian-w.cn/gtlhexxvhk.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.cdnleiting.top/gtwhvfiftw.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jianghu66.top/gtoboubmsz.html

[J10] 取今天 / 本月第一天
来源：http://hz.jqgufenzy.top/gtgckaauir.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhongyouzk.top/gtoqrlopqb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.nwbrower.top/gtrnwdzbfr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ehwqpu.com/gtvrcbfejt.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sweek.top/gtbzboxhwu.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sxryk.cn/gtqyscbqrb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.0kj1m.cn/gtanscguie.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gzhubu.top/gtltfuunyo.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yanxiufei.cn/gtptxoxfeh.html

================================================================================
来源：http://hz.jlsjyb.cn/gtwzghnzda.html

K. JSON 与序列化
来源：http://hz.guowangkeji.top/gtrcgcfwpq.html

================================================================================
来源：http://hz.ehwqpu.com/gtdjohqrpi.html

[K01] 对象转 JSON 字符串
来源：http://hz.52xcode.cn/gtaaonjyph.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.mhx1999.top/gtruvpaspz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.hywenlv.cn/gtekhlzowt.html

JS:   JSON.stringify(obj)
来源：http://hz.daxiang520.top/gtgogvopuv.html

TS:   JSON.stringify(obj)
来源：http://hz.fengsongda.top/gtsiihnivc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hywenlv.cn/gtdmylzjre.html

Go:   json.Marshal(obj)
来源：http://hz.mhx1999.top/gtvhlgqfkq.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.pengpengdd.cyou/gtyqdesjhl.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.chenlongwang.top/gtrqlhmcji.html

[K02] JSON 字符串转对象
来源：http://hz.dianchejie.cn/gtisqdurns.html

Py:   json.loads(s)
来源：http://hz.yuanzhike.top/gtzvgzwshd.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhongyouzk.top/gttogmzypa.html

JS:   JSON.parse(s)
来源：http://hz.shangyingyoupin.top/gtxnqjncxm.html

TS:   JSON.parse(s)
来源：http://hz.316326.xyz/gtjwvifbxp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jianghu66.top/gtuwsikzwv.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.hnxiangtu.top/gtxxbyegjw.html

Ruby: JSON.parse(s)
来源：http://hz.jinqigufen.top/gtmojaebdd.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.hongshengwenyu.top/gttouxideq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.guowangkeji.top/gtnjottdns.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhiwuduotai.top/gtfmavklsp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.tianlin.xyz/gtmfgkltbr.html


<!-- 参考信息 -->