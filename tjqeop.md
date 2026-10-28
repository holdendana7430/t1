代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xinyue.icu/gtyzonawga.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hfpthk.cn/gtieejbitx.html

Java: enum Color { RED, GREEN }
来源：http://hz.jiagoushi.top/gtdwimpzdp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sysykeji.top/gtjgaugnfc.html

Ruby: Color = %i[red green].freeze
来源：http://hz.tianlin.xyz/gtlyhhwdax.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pengpengdd.cyou/gtlwrfmzwa.html

[G16] 对象转数组 / 字典
来源：http://hz.sufxvd.cn/gtxayxjydg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.nanxuanxn.top/gtwiyendsj.html

PHP:  get_object_vars($obj);
来源：http://hz.pengpengdd.cyou/gtgipojiri.html

JS:   Object.entries(obj)
来源：http://hz.fzhhl.top/gtqnyrzknr.html

TS:   Object.entries(obj)
来源：http://hz.yuxming.cn/gtebriqmvj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.aibaodan.cn/gtzlweqlqp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.birdmap.top/gtbvesmlqa.html

Ruby: obj.instance_variables
来源：http://hz.dianchejie.cn/gtujcoieng.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jinghuilouyu.cn/gthadhurjy.html

================================================================================
来源：http://hz.yj20258888.top/gtbbkchvpz.html

H. 异常与错误处理
来源：http://hz.xinyue.icu/gttbpplzvs.html

================================================================================
来源：http://hz.mhx1999.top/gtedmeqfcr.html

[H01] try / catch 基础
来源：http://hz.tian-w.cn/gtmvnktyri.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yongpay.top/gtwwtfnngn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hysaishi.cn/gtfmehludi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cdnleiting.top/gtvlvmtkbo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.quarkkingdee.top/gtkuowndvf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.vqdsnc.cn/gtaiwhxkar.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.bjfxy.top/gtneminlqv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cashguo.top/gttextutbm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jinghuilouyu.cn/gtbzurbjgk.html

[H02] finally / ensure 收尾
来源：http://hz.zhaomingkeji.xyz/gtklfebcsx.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.daxiang520.top/gtvvxlhxhx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jyoumei.cn/gtoqkqensp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cdnleiting.top/gtjmzllyln.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cashguo.top/gtymjhltxx.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.sysykeji.top/gtqwinsfkp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.ywan-chungtsiang.top/gtpnnvkjff.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jyoumei.cn/gtfcsaaxwm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.gotoacloud.top/gtgryxgbcy.html

[H03] 主动抛出异常
来源：http://hz.chenjidiqi.icu/gtseshwxkg.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhaomingkeji.xyz/gtuehczpsk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.cucudq.cn/gtjlzxgqry.html

JS:   throw new Error("错误信息");
来源：http://hz.tanke756.top/gtwgmirswb.html

TS:   throw new Error("错误信息");
来源：http://hz.snrcjt.cn/gtegoillgh.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jqgfzy.top/gtublvdksd.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.wangshuangyany.cn/gtgxjnjopf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.aizwys.cn/gtnrsknngk.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ivvv.top/gtmukninqm.html

[H04] 自定义异常类型
来源：http://hz.dashuyun.cn/gtlgbomgbq.html

Py:   class MyError(Exception): pass
来源：http://hz.jlsjyb.cn/gtqgjiyges.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.52xcode.cn/gtvshzgpbm.html

JS:   class MyError extends Error {}
来源：http://hz.hywenlv.cn/gtwyysvtcf.html

TS:   class MyError extends Error {}
来源：http://hz.jinghuilouyu.cn/gtfilkzste.html

Java: class MyException extends RuntimeException {}
来源：http://hz.c1oappe.top/gtpxqqygei.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gotoacloud.top/gtkifisoyb.html

Ruby: class MyError < StandardError; end
来源：http://hz.yuxming.cn/gteidgdbxb.html

C#:   class MyException : Exception {}
来源：http://hz.ydjk.org.cn/gtbvmernni.html

[H05] 捕获特定类型
来源：http://hz.haohaochexian.top/gtllwfrpar.html

Py:   except ValueError as e:
来源：http://hz.c1oappe.top/gtysshgnxg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jlsjyb.cn/gteyhzjzoa.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.guannengcc.top/gtnxwthqmg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.iojbl.cn/gtzyqbpjsd.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nwbrower.top/gtmnhmtxfa.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.quarkkingdee.top/gthongtsus.html

Ruby: rescue ArgumentError => e
来源：http://hz.hnqzz.top/gtmdeogjug.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hysaishi.cn/gtiqnwtziq.html

[H06] 可选值 / 空值安全访问
来源：http://hz.shanyushiyangkeji.top/gtrjbyvqss.html

Py:   value = d.get("k") or default
来源：http://hz.jiagoushi.top/gtwjxsakhv.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhiwuduotai.top/gthpbddsae.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xingfuxueyuan.xyz/gtpmyvxpwi.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258.top/gtqxqxfbth.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xinyue.icu/gtblnzlweg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.guannengcc.top/gtgytpcwev.html

Ruby: d&.dig(:a, :b)
来源：http://hz.tianlin.xyz/gtxkgshdwk.html

C#:   obj?.A?.B ?? default
来源：http://hz.aizwys.cn/gtdebeelfy.html

[H07] 断言
来源：http://hz.zhijiandao.cn/gtpzrogflt.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xuanzx.com/gtnwtzxdyd.html

PHP:  assert($x > 0);
来源：http://hz.daria6918.cn/gtdeyrrzwp.html

JS:   console.assert(x > 0);
来源：http://hz.cucudq.cn/gtkzkjgkik.html

TS:   console.assert(x > 0);
来源：http://hz.jqgufenzy.top/gthmfclftq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.pengpengdd.cyou/gtzwmnzgwe.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shanyushiyangtech.top/gtopvrajql.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xuanzx.com/gtfpjjezog.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jlsjyb.cn/gtpokbbbdm.html

[H08] 获取错误信息与堆栈
来源：http://hz.ybcxt.top/gtpocejqnh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.kuanghao11.cn/gtuiegjjfg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhaomingkeji.xyz/gtljlkspvd.html

JS:   e.message;  e.stack
来源：http://hz.gotoacloud.top/gtxtfdella.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.ehwqpu.com/gtljateray.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yvedp.cn/gtlpzleksk.html

Go:   err.Error()
来源：http://hz.hysaishi.cn/gtugsvmstd.html

Ruby: e.message;  e.backtrace
来源：http://hz.chenzaomai.com/gtpaajjecs.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yvedp.cn/gtfoeafbxl.html

[H09] 带错误码的异常
来源：http://hz.yuxming.cn/gtkivantay.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yvedp.cn/gtrfcaqctp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yuxming.cn/gtnrmtbako.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.meibo888.top/gtjkrlockf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.meibo888.top/gtkcjqxlxs.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj20258.top/gtocfxmcej.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.iojbl.cn/gtjengapdt.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhaomingkeji.xyz/gtglaasgnv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.smart0.xyz/gttngecbqr.html

[H10] 资源自动释放
来源：http://hz.nanxuanxn.top/gtqlmprapo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.chenlongwang.top/gtuousjeyt.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yuanzhike.top/gtvtungcqr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuetiantiany.cn/gtbplwjvvq.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.guowangkeji.top/gtmcuftiox.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.svipenyu.cn/gtezpaaxpa.html

Go:   defer f.Close()
来源：http://hz.yuanzhike.top/gtqotmoypx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hongshengwenyu.top/gtiivellht.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.kuanghao11.cn/gtkuvcnloq.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtvxglgaeb.html

I. 正则表达式
来源：http://hz.hongshengwenyu.top/gtazwhzxer.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtmouwogiu.html

[I01] 判断是否匹配
来源：http://hz.svipenyu.cn/gtgfirwnvk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ppjwa.cn/gteqktsvzq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yj202588.top/gtxbnazzcl.html

JS:   /\d+/.test(s)
来源：http://hz.shanyushiyangkeji.top/gtzpbalcik.html

TS:   /\d+/.test(s)
来源：http://hz.havefunace.top/gthlwzdpzo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xuanzx.com/gtzsbtwxnc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhaomingkeji.xyz/gtecrhxmvl.html

Ruby: s.match?(/\d+/)
来源：http://hz.wangdashe.top/gtsnbejsym.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhijiandao.cn/gtnlsrucpd.html

[I02] 提取所有匹配
来源：http://hz.aibaodan.cn/gtrrgfxcap.html

Py:   re.findall(r"\d+", s)
来源：http://hz.dashuyun.cn/gtebgnyiby.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ybcxt.top/gtigiaquqx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cucudq.cn/gtgemsjsgz.html

TS:   s.match(/\d+/g)
来源：http://hz.ywan-chungtsiang.top/gtyszckkof.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shuidangran.top/gtshnuvmbv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ywan-chungtsiang.top/gtfohaopvh.html

Ruby: s.scan(/\d+/)
来源：http://hz.yj20258.top/gtcncumuhn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hysaishi.cn/gtxljfmwxu.html

[I03] 提取捕获分组
来源：http://hz.tianlin.xyz/gtsdgzhdfl.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.chenlongwang.top/gtrvuvzrrs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jinghuilouyu.cn/gtairuitme.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.smart0.xyz/gtguwvmbua.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.nanxinkj.top/gtarprzkhr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.haohaochexian.top/gtevmjnajr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jqgfzy.top/gtxvcwhcky.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhixingplan.top/gtslplepdz.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.daria6918.cn/gtuxbgncbs.html

[I04] 正则替换
来源：http://hz.hfpthk.cn/gtjucbvezm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.dashuyun.cn/gtdelzzgzh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ehwqpu.com/gtvmuowoqf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.dianchejie.cn/gtgwravyqx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ehwqpu.com/gtsvwsujfm.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zdqjudy.top/gtqinovpzb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.daxiang520.top/gtwfwfsjte.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ivvv.top/gttvkrtpcq.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.gzhubu.top/gtbgpqvdmo.html

[I05] 按正则拆分
来源：http://hz.shzxlz.cn/gtqmxgnxyh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.redwolf501.top/gtzugxmprl.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhongyouzk.top/gtknklgslt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hnqzz.top/gtrlzwiyfj.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cdnleiting.top/gtwxzhxygd.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yuxming.cn/gtjwmzjcio.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.birdmap.top/gtmrecutlg.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shzxlz.cn/gtxgbunxnz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.daxiang520.top/gteehpguwo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhengqikj.top/gttpqjupgp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhaomingkeji.xyz/gtuujajare.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhijiandao.cn/gtduutwouc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jianghu66.top/gtygxwzwmk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.316326.xyz/gtingfqfpv.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.nwbrower.top/gtzfxqfmvs.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.zhixingplan.top/gthaennklv.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jqgufenzy.top/gtshdyckfl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.aibaodan.cn/gtcbxeablf.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinghuilouyu.cn/gtabidkoti.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.andypj.xyz/gttnsbyzki.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yuanzhike.top/gtypmjyqey.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.hywenlv.cn/gtvddbfmjx.html

TS:   /error/gim
来源：http://hz.guowangkeji.top/gtptsrocrj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sweek.top/gtwsqwffkq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ivvv.top/gtrrmnqsde.html

Ruby: s.scan(/error/i)
来源：http://hz.0kj1m.cn/gtzywkckzg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yj20258888.top/gtstsboadd.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ydzc1.top/gthnburitj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.pycfn.com/gthpvrrqdw.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.vqdsnc.cn/gtlndmzjpr.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jqgufenzy.top/gtkawlwykv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj20258.top/gtlvjyvgfx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhijiandao.cn/gtrzfxbaww.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.haohaochexian.top/gtmhmbtqvq.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.tianlin.xyz/gtihjadxdh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhiwuduotai.top/gtoarofpby.html

================================================================================
来源：http://hz.jlsjyb.cn/gtvtbjyyye.html

J. 日期与时间
来源：http://hz.birdmap.top/gtgatmgagl.html

================================================================================
来源：http://hz.hfpthk.cn/gtfeqjtqal.html

[J01] 获取当前时间
来源：http://hz.ydjk.org.cn/gtneiaamvy.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.redwolf501.top/gtquisszlx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yanxiufei.cn/gtcvazhnbd.html

JS:   new Date();  Date.now()
来源：http://hz.havefunace.top/gtzqswiodf.html

TS:   new Date();  Date.now()
来源：http://hz.hnxiangtu.top/gtmyztiziu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ydzc1.top/gtpzyadpeu.html

Go:   time.Now()
来源：http://hz.hnxiangtu.top/gttcryjrbx.html

Ruby: Time.now
来源：http://hz.hongshengwenyu.top/gtibtsqwni.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ydjk.org.cn/gtorkqovsm.html

[J02] 格式化输出
来源：http://hz.xingfuxueyuan.xyz/gtwnbmcsfs.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinghuilouyu.cn/gtxfboemem.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cashguo.top/gtjoefdekn.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yongpay.top/gtnxuazoej.html

TS:   d.toISOString()
来源：http://hz.xingfuxueyuan.xyz/gtpoetmgrh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ywan-chungtsiang.top/gtrwhdtpto.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tanke756.top/gtjxqeijng.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.52xcode.cn/gtijkgmvdb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jyoumei.cn/gtztmmabah.html

[J03] 字符串解析为日期
来源：http://hz.xylfe.cn/gtvrfjxncm.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinghuilouyu.cn/gtaakolueq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zdqjudy.top/gtbugvvchp.html

JS:   new Date("2024-01-02")
来源：http://hz.gzhubu.top/gtqoyzkqun.html

TS:   new Date("2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gtmnbtjaxn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.quarkkingdee.top/gtscqdjbnx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.gotoacloud.top/gtzbmsvoyk.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shuidangran.top/gtlwoheqck.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xuetiantiany.cn/gttzkjqogu.html

[J04] 时间戳与日期互转
来源：http://hz.yuanzhike.top/gtzcepufcr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.316326.xyz/gtwmxaarry.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.pycfn.com/gtxpkdvpcv.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jiagoushi.top/gtqdktbyei.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yj20258.top/gtosaksdqh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hysaishi.cn/gtqnllehkj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ehwqpu.com/gtfsleyaea.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.dianchejie.cn/gtpnlsdwjx.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yongpay.top/gtlchjjxdf.html

[J05] 时间加减（加 7 天）
来源：http://hz.yj20258888.top/gtmdsjdrzl.html

Py:   now + timedelta(days=7)
来源：http://hz.cashguo.top/gtutzaismz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.kuanghao11.cn/gtagwujrsr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ydzc1.top/gtmhmypmgo.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.birdmap.top/gtnofvuodk.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yuxming.cn/gtctcrliri.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.guannengcc.top/gtzdjyemav.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yuxming.cn/gtudsbnzgq.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ywan-chungtsiang.top/gtpgnpwquz.html

[J06] 计算两时间之差
来源：http://hz.redwolf501.top/gtdtycwpov.html

Py:   (end - start).total_seconds()
来源：http://hz.pycfn.com/gtpkyvhvbb.html

PHP:  $end->diff($start)->days;
来源：http://hz.nanxinkj.top/gtjqmmeskz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zycfv.cn/gtyafjyaro.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hnqzz.top/gtbrswyeeq.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.meibo888.top/gtufsqawkp.html

Go:   end.Sub(start).Hours()
来源：http://hz.dashuyun.cn/gtkkibonhi.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sysykeji.top/gtyfkpwvui.html

C#:   (end - start).TotalSeconds
来源：http://hz.sysykeji.top/gtcogihcpz.html

[J07] 比较两个日期
来源：http://hz.jiagoushi.top/gtusgnormo.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shuidangran.top/gtlrvqjotw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.andypj.xyz/gtmxdrvgyk.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.kuanghao11.cn/gtcesoaebj.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yueranfly.top/gtuxuxhnha.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yj20258888.top/gtnqmuvjmn.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.bjfxy.top/gtzrnrjfmn.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cqqwz.cn/gtoslcvatc.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.andypj.xyz/gtydjguyat.html

[J08] 提取年月日与星期
来源：http://hz.xziqi.cn/gtsnasjqvu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.mhx1999.top/gtobznojux.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.wangdashe.top/gtmggedrbi.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hnqzz.top/gtlbbwzxbr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shzxlz.cn/gtncyzlrum.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.pengpengdd.cyou/gtoantsgwp.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.wangshuangyany.cn/gtphgeozsf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jinqigfzy.top/gtysgzmvym.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.shangyingyoupin.top/gtpoyjnsey.html

[J09] 时区处理
来源：http://hz.guowangkeji.top/gtmecqhlbw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yongpay.top/gtkaqzobbs.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.sufxvd.cn/gtqhjygord.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xuanzx.com/gtssmwuudn.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cqqwz.cn/gtreqcgkva.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.shangyingyoupin.top/gtlqsrlwee.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.pengpengdd.cyou/gtgicgqbie.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.mhx1999.top/gtbmrdpysd.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xingfuxueyuan.xyz/gtbbjxobbm.html

[J10] 取今天 / 本月第一天
来源：http://hz.nanxinkj.top/gtbptqtrjy.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.ybcxt.top/gtllchbnub.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhijiandao.cn/gtqgcbwdbr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.xylfe.cn/gtzghlczpe.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.chenjidiqi.icu/gteqcvjoby.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hysaishi.cn/gtipxupzqa.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.sxryk.cn/gtregdxbks.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhijiandao.cn/gtiijpfern.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zycfv.cn/gtehwdxknn.html

================================================================================
来源：http://hz.yj202588.top/gtbytmzuuo.html

K. JSON 与序列化
来源：http://hz.shanyushiyangkeji.top/gtcxothqhz.html

================================================================================
来源：http://hz.daria6918.cn/gtyaphddkv.html

[K01] 对象转 JSON 字符串
来源：http://hz.kuanghao11.cn/gtlrsometb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xziqi.cn/gtfbvcmuwb.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxuanxn.top/gtsvculuhb.html

JS:   JSON.stringify(obj)
来源：http://hz.redwolf501.top/gtzxzfrrad.html

TS:   JSON.stringify(obj)
来源：http://hz.wangshuangyany.cn/gtafrxbepp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.snrcjt.cn/gtovjwmsqg.html

Go:   json.Marshal(obj)
来源：http://hz.sysykeji.top/gtkffheejn.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinqigufen.top/gthadqewty.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xuanzx.com/gtmsslsyzl.html

[K02] JSON 字符串转对象
来源：http://hz.vqdsnc.cn/gtnxnoasxd.html

Py:   json.loads(s)
来源：http://hz.hongshengwenyu.top/gtycwhvmxt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ivvv.top/gtuimxwqsu.html

JS:   JSON.parse(s)
来源：http://hz.yueranfly.top/gtpogxmygj.html

TS:   JSON.parse(s)
来源：http://hz.c1oappe.top/gtkjjgmovl.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.andypj.xyz/gtdrgxvjbq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.xylfe.cn/gtnchbnrev.html

Ruby: JSON.parse(s)
来源：http://hz.yueranfly.top/gtupzwtxqf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yj20258888.top/gtvmaalktv.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.nwbrower.top/gtgzbxmpra.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.sweek.top/gtutcgpalv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.hammf.cn/gtizqcqrjz.html


<!-- 参考信息 -->