代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jinyuanbaomall.cn/gtifcsbrgl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.smart0.xyz/gtyeqmouxg.html

Java: enum Color { RED, GREEN }
来源：http://hz.hfpthk.cn/gtfhjwcoqw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.nanxinkj.top/gtaatoccje.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinghuilouyu.cn/gtvulpfdjr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pycfn.com/gtuipebvcu.html

[G16] 对象转数组 / 字典
来源：http://hz.jinyuanbaomall.cn/gtfmcqerkl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.ydzc1.top/gtmjvegkpy.html

PHP:  get_object_vars($obj);
来源：http://hz.nanxinkj.top/gtklqmggab.html

JS:   Object.entries(obj)
来源：http://hz.zhaomingkeji.xyz/gtehlrhdtp.html

TS:   Object.entries(obj)
来源：http://hz.ivvv.top/gtogndagpx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zycfv.cn/gtyprzojhk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.gzhubu.top/gtzhahbaxn.html

Ruby: obj.instance_variables
来源：http://hz.ehwqpu.com/gtjgifbktu.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.0kj1m.cn/gtjpwkmked.html

================================================================================
来源：http://hz.yangfankeji.com/gtuhwoykte.html

H. 异常与错误处理
来源：http://hz.xziqi.cn/gtqdjuqiij.html

================================================================================
来源：http://hz.hammf.cn/gtgtkvqmhr.html

[H01] try / catch 基础
来源：http://hz.yuxming.cn/gtldmsghyh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yangfankeji.com/gtwbwxoood.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yj20258.top/gtqocahjef.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sxryk.cn/gtqvntyhsn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhijiandao.cn/gtvrhjimzn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jyoumei.cn/gtdowqfuwz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.sufxvd.cn/gtkstzoolk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.redwolf501.top/gtvjtqdour.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.mhx1999.top/gtewbfooeh.html

[H02] finally / ensure 收尾
来源：http://hz.pengpengdd.cyou/gtdxaxwqru.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.316326.xyz/gtzxvdzggy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gtodjtutij.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sufxvd.cn/gtekiuuvly.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj202588.top/gtjcbejvwd.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtyczpoqkd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinqigfzy.top/gteeydcgou.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shangyingyoupin.top/gtkftzmhfg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.nwbrower.top/gtveymobmr.html

[H03] 主动抛出异常
来源：http://hz.xuetiantiany.cn/gtmubshukd.html

Py:   raise ValueError("错误信息")
来源：http://hz.chenlongwang.top/gtgtmmskdg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ivvv.top/gtsfcxbwxw.html

JS:   throw new Error("错误信息");
来源：http://hz.cashguo.top/gtfyqrnkmy.html

TS:   throw new Error("错误信息");
来源：http://hz.jyoumei.cn/gtqrnlezvn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.nanxinkj.top/gtenwyqget.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hnqzz.top/gtammabuzc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ywan-chungtsiang.top/gtgtskuqeh.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.svipenyu.cn/gttukrmkkz.html

[H04] 自定义异常类型
来源：http://hz.yj202588.top/gtltocrgva.html

Py:   class MyError(Exception): pass
来源：http://hz.zhaomingkeji.xyz/gtoszrlpak.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.52xcode.cn/gtkkbidbas.html

JS:   class MyError extends Error {}
来源：http://hz.snrcjt.cn/gtzdeflwdr.html

TS:   class MyError extends Error {}
来源：http://hz.zhixingplan.top/gttfrtmluk.html

Java: class MyException extends RuntimeException {}
来源：http://hz.bjfxy.top/gtcdodhmkb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.wangshuangyany.cn/gtxmznolht.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhongyouzk.top/gtzqmglqov.html

C#:   class MyException : Exception {}
来源：http://hz.shanyushiyangkeji.top/gttnnvvewq.html

[H05] 捕获特定类型
来源：http://hz.jyoumei.cn/gtlnsqoiaj.html

Py:   except ValueError as e:
来源：http://hz.jqgufenzy.top/gtzedrjarg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.daria6918.cn/gtgumgdjkc.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.chenjidiqi.icu/gtudbbrwpd.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.52xcode.cn/gtwxjhhtwm.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.guannengcc.top/gtstvxnspq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.gzhubu.top/gtqzjuonwl.html

Ruby: rescue ArgumentError => e
来源：http://hz.feifeiyinyue.top/gtdpztpqgp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ydzc1.top/gtrwyojfae.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sysykeji.top/gtuvqudkom.html

Py:   value = d.get("k") or default
来源：http://hz.pengpengdd.cyou/gtdsrglkpk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.haohaochexian.top/gtqqtvrdbg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yj202588.top/gtifshvuvy.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shuidangran.top/gtuohwjomw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.cdnleiting.top/gtydsohnjh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hysaishi.cn/gtjpzbpgih.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gogol.net.cn/gtxqcqfzpo.html

C#:   obj?.A?.B ?? default
来源：http://hz.shangyingyoupin.top/gtpenybzob.html

[H07] 断言
来源：http://hz.havefunace.top/gtfjwmvvek.html

Py:   assert x > 0, "必须为正"
来源：http://hz.nanxuanxn.top/gtfscoilgv.html

PHP:  assert($x > 0);
来源：http://hz.cdnleiting.top/gthloyqvne.html

JS:   console.assert(x > 0);
来源：http://hz.yvedp.cn/gtlouacatg.html

TS:   console.assert(x > 0);
来源：http://hz.hysaishi.cn/gtrvgfyaak.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sufxvd.cn/gtsdrfltjc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.fzhhl.top/gtqyybwpwm.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hnqzz.top/gtlqaijgsa.html

C#:   Debug.Assert(x > 0);
来源：http://hz.bjfxy.top/gtipsegmcu.html

[H08] 获取错误信息与堆栈
来源：http://hz.tanke756.top/gtnivlohbv.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.snrcjt.cn/gtnrkhulnp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yj20258888.top/gtagefwily.html

JS:   e.message;  e.stack
来源：http://hz.jinyuanbaomall.cn/gtvxwvimrv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.aizwys.cn/gttwhrshrr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.snrcjt.cn/gtqvrxvqeb.html

Go:   err.Error()
来源：http://hz.zhoulong.xyz/gtehaefkdm.html

Ruby: e.message;  e.backtrace
来源：http://hz.jqgfzy.top/gtognesruj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.smart0.xyz/gtawjyhccl.html

[H09] 带错误码的异常
来源：http://hz.fengsongda.top/gtewxbqxoh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xylfe.cn/gtusmuxgmc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jiagoushi.top/gthdbkytis.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.c1oappe.top/gtadjirnxb.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.svipenyu.cn/gtxdrmefzo.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.ywan-chungtsiang.top/gtwfcmvdcn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ydjk.org.cn/gtqkfxrndb.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sweek.top/gtgugvrnkk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.guowangkeji.top/gtcoufulma.html

[H10] 资源自动释放
来源：http://hz.hongshengwenyu.top/gtkzskkrac.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhoulong.xyz/gtvhyafcnw.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.fengsongda.top/gtiutkatsn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tian-w.cn/gtlumlqdii.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yongpay.top/gtneocwhgn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yj202588.top/gtxkexdozu.html

Go:   defer f.Close()
来源：http://hz.xuanzx.com/gtumslsiac.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinghuilouyu.cn/gtloemoopr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.cheryme.top/gtbkgzvctp.html

================================================================================
来源：http://hz.iojbl.cn/gtjvoyoarb.html

I. 正则表达式
来源：http://hz.shangyingyoupin.top/gtllkzvxdr.html

================================================================================
来源：http://hz.havefunace.top/gtaishqcfu.html

[I01] 判断是否匹配
来源：http://hz.wangdashe.top/gtkaisryzi.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.gogol.net.cn/gtkqiflalt.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.dianchejie.cn/gtxigcbsla.html

JS:   /\d+/.test(s)
来源：http://hz.hysaishi.cn/gtsevgmapv.html

TS:   /\d+/.test(s)
来源：http://hz.redwolf501.top/gtitjbhzyg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.pengpengdd.cyou/gtxjwojxni.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yueranfly.top/gtznzbfoxn.html

Ruby: s.match?(/\d+/)
来源：http://hz.snrcjt.cn/gthvduomdg.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xinyue.icu/gtdgeuaacw.html

[I02] 提取所有匹配
来源：http://hz.fengsongda.top/gtmpfxgwkf.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jianghu66.top/gtxazirbph.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.nanxinkj.top/gtcnljobbs.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.kuanghao11.cn/gtusvzhynp.html

TS:   s.match(/\d+/g)
来源：http://hz.tian-w.cn/gttcbykfbx.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sxryk.cn/gtprwegisd.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.guowangkeji.top/gtbssljqye.html

Ruby: s.scan(/\d+/)
来源：http://hz.shanyushiyangkeji.top/gtriynbxqp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ydjk.org.cn/gtymxedcjp.html

[I03] 提取捕获分组
来源：http://hz.shuidangran.top/gtlmmhhabf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ydzc1.top/gtojtwiovh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.feifeiyinyue.top/gtblbzykiz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xuetiantiany.cn/gtyqakdbkt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yj20258.top/gtvawyymtr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.9152youxi.cn/gtjmgtibds.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yongpay.top/gtdzqicfsu.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sufxvd.cn/gtgdpgrzlx.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.chenlongwang.top/gtageycxnu.html

[I04] 正则替换
来源：http://hz.fzhhl.top/gtdizqhgab.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinghuilouyu.cn/gtkitytltd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.9152youxi.cn/gtsukzyeui.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.nanxuanxn.top/gtwudvmtte.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhixingplan.top/gtfxbxnvue.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.pengpengdd.cyou/gttphfbnql.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.nanxuanxn.top/gtdosttool.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cdnleiting.top/gtwotnhwdk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jiagoushi.top/gttnobfmnc.html

[I05] 按正则拆分
来源：http://hz.jiagoushi.top/gtzseumwrc.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yj20258.top/gtkxyscguj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.hnxiangtu.top/gtnptpdbqr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.gogol.net.cn/gtiqwjmdnw.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gtzwqwvakk.html

Java: s.split("\\s*,\\s*")
来源：http://hz.wangdashe.top/gtiyjhkcdl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.nwbrower.top/gtbmqmeouk.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.bjfxy.top/gtqbnharrt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.tanke756.top/gtatayqnur.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.birdmap.top/gtpsuxtzln.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.gzhubu.top/gtantmclan.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jianghu66.top/gthidsjefg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258.top/gtrmszaesz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nanxuanxn.top/gtbturrwin.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.aibaodan.cn/gtpmqgaqna.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yj202588.top/gtwzpywqty.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shuidangran.top/gtwmulkikh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yongpay.top/gtwhifqlcx.html

[I07] 忽略大小写与多行模式
来源：http://hz.fengsongda.top/gtmkgsnarp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xinyue.icu/gtggmcjtjx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhixingplan.top/gtoccykstl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinqigfzy.top/gtcvjoduzb.html

TS:   /error/gim
来源：http://hz.fzhhl.top/gtzxjzfdvc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhengqikj.top/gtrighxexp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.shangyingyoupin.top/gtmcqdbwmy.html

Ruby: s.scan(/error/i)
来源：http://hz.xuetiantiany.cn/gtlxwleqrt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.dashuyun.cn/gtttdegbtg.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yvedp.cn/gtaogqgpiq.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.feifeiyinyue.top/gtxzctusmd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.chenjidiqi.icu/gtmskmybpz.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ehwqpu.com/gtjiicsbhr.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigfzy.top/gtsxzqtuer.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.gogol.net.cn/gtpcfvzecq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shanyushiyangtech.top/gtzjcodmhj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ehwqpu.com/gtzfkyyghy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.cucudq.cn/gtypltasfe.html

================================================================================
来源：http://hz.jqgfzy.top/gtzclxncwn.html

J. 日期与时间
来源：http://hz.nwbrower.top/gtogompayj.html

================================================================================
来源：http://hz.yanxiufei.cn/gtqskvvave.html

[J01] 获取当前时间
来源：http://hz.xziqi.cn/gtzsebicmk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sweek.top/gtnpqrxukg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.316326.xyz/gtmwvoeeuf.html

JS:   new Date();  Date.now()
来源：http://hz.cdnleiting.top/gtssyqateq.html

TS:   new Date();  Date.now()
来源：http://hz.hysaishi.cn/gtvrurzcwe.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinqigfzy.top/gtsthklrnv.html

Go:   time.Now()
来源：http://hz.aizwys.cn/gtqonleciv.html

Ruby: Time.now
来源：http://hz.chenjidiqi.icu/gtgeaexdlr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.quarkkingdee.top/gtwuycvljm.html

[J02] 格式化输出
来源：http://hz.jiagoushi.top/gtavnjjmrb.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cheryme.top/gtqccuvsjm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.daria6918.cn/gtcnvqrvau.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hnxiangtu.top/gtoqbleqca.html

TS:   d.toISOString()
来源：http://hz.gzhubu.top/gtdpvqirrb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jqgfzy.top/gtnzrjodtj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shzxlz.cn/gtqtrkamfw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cdnleiting.top/gtcqpyvuam.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.tian-w.cn/gtavhcgmiv.html

[J03] 字符串解析为日期
来源：http://hz.shanyushiyangtech.top/gteoaoynvt.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.fzhhl.top/gtgmfeswfn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.vqdsnc.cn/gtmcvpwrrx.html

JS:   new Date("2024-01-02")
来源：http://hz.hongshengwenyu.top/gtqgnmrogp.html

TS:   new Date("2024-01-02")
来源：http://hz.dashuyun.cn/gtjmvcmqqf.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yueranfly.top/gtnrtxkynv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tian-w.cn/gtxjqlbqmo.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.meibo888.top/gtxsxsearf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.smart0.xyz/gtycuvuqct.html

[J04] 时间戳与日期互转
来源：http://hz.jqgfzy.top/gtgejrwhpq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.gogol.net.cn/gtvczvvrdr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.chenjidiqi.icu/gtamakhyex.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.daxiang520.top/gthevqsycx.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jinqigufen.top/gtdqjwngbz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ywan-chungtsiang.top/gtroxjpwra.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zycfv.cn/gtqoadsvhu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.tanke756.top/gtyriwkbrv.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.nwbrower.top/gtwvcrrntt.html

[J05] 时间加减（加 7 天）
来源：http://hz.hongshengwenyu.top/gtsfkjqour.html

Py:   now + timedelta(days=7)
来源：http://hz.chenlongwang.top/gtfdigzzcj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shanyushiyangtech.top/gtssqkdyix.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hfpthk.cn/gtrzurqdjh.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sysykeji.top/gtwrqnsbpb.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.mhx1999.top/gtdlfevwes.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ydjk.org.cn/gtmeqlfgsp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.sufxvd.cn/gtpsbnkqsx.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhixingplan.top/gtouzqddwv.html

[J06] 计算两时间之差
来源：http://hz.gogol.net.cn/gttudhtwae.html

Py:   (end - start).total_seconds()
来源：http://hz.hnxiangtu.top/gtsnflrdva.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhixingplan.top/gtcshsddds.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shangyingyoupin.top/gtmbjydgok.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.haohaochexian.top/gtoqwrdjvq.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hammf.cn/gtskdrupfl.html

Go:   end.Sub(start).Hours()
来源：http://hz.hywenlv.cn/gtsenjdlet.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yanxiufei.cn/gtpnthwuwh.html

C#:   (end - start).TotalSeconds
来源：http://hz.ehwqpu.com/gtsszozepp.html

[J07] 比较两个日期
来源：http://hz.jinqigufen.top/gtxfedzmlf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.9152youxi.cn/gtzrmppnxh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hongshengwenyu.top/gtikeklywi.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.daria6918.cn/gttlivdpho.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.iojbl.cn/gtcirlnaoh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yvedp.cn/gtwtnioawq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.ydzc1.top/gtpwecrpep.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.0kj1m.cn/gtaioukwfi.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.redwolf501.top/gtghtlfogk.html

[J08] 提取年月日与星期
来源：http://hz.jinqigfzy.top/gtahomxacj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hnxiangtu.top/gtcaolmoae.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yvedp.cn/gtrfcdcmzw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.daxiang520.top/gtitvudnhr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yuanzhike.top/gtfvqladom.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yj20258888.top/gtaeztkvcx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenjidiqi.icu/gtmijjphgr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yj20258888.top/gtmbryncmx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.316326.xyz/gtwbcunlqx.html

[J09] 时区处理
来源：http://hz.jinghuilouyu.cn/gtqnfctrrt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.zhongyouzk.top/gtzgqjiqvk.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.meibo888.top/gtcwxdqdgm.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yangfankeji.com/gtlyrzadrf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jlsjyb.cn/gtedcabbxl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.sysykeji.top/gtpczrhmpi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.havefunace.top/gtkpixsrrv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.c1oappe.top/gtdctxtjvn.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinghuilouyu.cn/gtbfewhipl.html

[J10] 取今天 / 本月第一天
来源：http://hz.zhongyouzk.top/gtbtiwpmar.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zdqjudy.top/gtgqzehqaf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ybcxt.top/gtahkqsgqy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yangfankeji.com/gtnrtaobqg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.quarkkingdee.top/gtwsgfaxdz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.tianlin.xyz/gtwoexlovw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cucudq.cn/gtjopwhuiy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ybcxt.top/gtepkqqulv.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.hnqzz.top/gteczebsra.html

================================================================================
来源：http://hz.tian-w.cn/gtghchynaq.html

K. JSON 与序列化
来源：http://hz.ivvv.top/gtugbgjxhd.html

================================================================================
来源：http://hz.vqdsnc.cn/gtdkpvemmh.html

[K01] 对象转 JSON 字符串
来源：http://hz.xingfuxueyuan.xyz/gtgmnnrlky.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinqigufen.top/gtkiaxrltq.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cheryme.top/gtpkywsyav.html

JS:   JSON.stringify(obj)
来源：http://hz.chenjidiqi.icu/gthovexzzy.html

TS:   JSON.stringify(obj)
来源：http://hz.hysaishi.cn/gtsedebfnx.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hammf.cn/gtxowsydal.html

Go:   json.Marshal(obj)
来源：http://hz.tianlin.xyz/gtsdtvbepj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.shzxlz.cn/gtpvlexsho.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xylfe.cn/gthwsqpcon.html

[K02] JSON 字符串转对象
来源：http://hz.hfpthk.cn/gtrqriqamo.html

Py:   json.loads(s)
来源：http://hz.yanxiufei.cn/gteqalkgfz.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.smart0.xyz/gtzbpoznnl.html

JS:   JSON.parse(s)
来源：http://hz.cheryme.top/gteyvjqarq.html

TS:   JSON.parse(s)
来源：http://hz.haohaochexian.top/gtacdwpmuj.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.mhx1999.top/gtpikrwsyi.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.fzhhl.top/gtllspmkxc.html

Ruby: JSON.parse(s)
来源：http://hz.guowangkeji.top/gttjjezojo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhaomingkeji.xyz/gtkfawnxlf.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.wangshuangyany.cn/gtinwaktoq.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hongshengwenyu.top/gtqsmzckne.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigufen.top/gtjyzmrqec.html


<!-- 参考信息 -->