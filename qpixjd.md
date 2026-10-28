代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.aizwys.cn/gtuwelnpfk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhongyouzk.top/gteohyfoas.html

Java: enum Color { RED, GREEN }
来源：http://hz.meibo888.top/gtcjxmejrw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.iojbl.cn/gtkvxibhtg.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gaohongyu789.top/gtllzvvnce.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.smart0.xyz/gtawdkiquk.html

[G16] 对象转数组 / 字典
来源：http://hz.gogol.net.cn/gtqfawgkgx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yj202588.top/gtscvixlmi.html

PHP:  get_object_vars($obj);
来源：http://hz.jinyuanbaomall.cn/gtazdfcqsb.html

JS:   Object.entries(obj)
来源：http://hz.zhaomingkeji.xyz/gtzplwucsf.html

TS:   Object.entries(obj)
来源：http://hz.guowangkeji.top/gtvwhnkvat.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.haohaochexian.top/gtawqafltk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.iojbl.cn/gtqnaqyogw.html

Ruby: obj.instance_variables
来源：http://hz.yangfankeji.com/gtwymsuofb.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.dashuyun.cn/gtstgxcajq.html

================================================================================
来源：http://hz.zhijiandao.cn/gttnsnitex.html

H. 异常与错误处理
来源：http://hz.birdmap.top/gtlddkvzpy.html

================================================================================
来源：http://hz.dashuyun.cn/gtwgkqzyro.html

[H01] try / catch 基础
来源：http://hz.jqgfzy.top/gtqvtnrtra.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhixingplan.top/gtypbtpyay.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.birdmap.top/gtpemvnxqg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yj20258888.top/gtmikxpqqp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.chenlongwang.top/gtsqhgovsf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shanyushiyangtech.top/gtgfkoagsm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.pengpengdd.cyou/gtrmqhdjve.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yangfankeji.com/gtiknhkvie.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.tian-w.cn/gtieyzyaxr.html

[H02] finally / ensure 收尾
来源：http://hz.zhaomingkeji.xyz/gtzedwnzoc.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yonumen.top/gtffdpdztu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtacaunxcw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gtgenltngz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhoulong.xyz/gtzhedltcv.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yonumen.top/gtprvkhqmx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hfpthk.cn/gtxhnczvbo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhongyouzk.top/gtdbowhqda.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ehwqpu.com/gtkirmhkyr.html

[H03] 主动抛出异常
来源：http://hz.yueranfly.top/gtjbgrrufg.html

Py:   raise ValueError("错误信息")
来源：http://hz.jqgfzy.top/gtukenecen.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.havefunace.top/gtpoydzktk.html

JS:   throw new Error("错误信息");
来源：http://hz.jianghu66.top/gthwcaigtu.html

TS:   throw new Error("错误信息");
来源：http://hz.chenzaomai.com/gtdlrmnjri.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.svipenyu.cn/gtumyvnzth.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.fengsongda.top/gtkkcpfgen.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jinyuanbaomall.cn/gtpkacuknn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jyoumei.cn/gtfemhqsub.html

[H04] 自定义异常类型
来源：http://hz.tanke756.top/gtqkpnmdym.html

Py:   class MyError(Exception): pass
来源：http://hz.cucudq.cn/gttiayeuxc.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hongshengwenyu.top/gtmnvjpeux.html

JS:   class MyError extends Error {}
来源：http://hz.gotoacloud.top/gtaszgvwyu.html

TS:   class MyError extends Error {}
来源：http://hz.zhixingplan.top/gtpgwcwpzh.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yanxiufei.cn/gtqzcfabuc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.chenjidiqi.icu/gtnlqxqlrw.html

Ruby: class MyError < StandardError; end
来源：http://hz.9152youxi.cn/gtnfhzxbcb.html

C#:   class MyException : Exception {}
来源：http://hz.zhengqikj.top/gtssbyziht.html

[H05] 捕获特定类型
来源：http://hz.nwbrower.top/gtqefqwepd.html

Py:   except ValueError as e:
来源：http://hz.guowangkeji.top/gtlbeijhke.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xuanzx.com/gtepffeqte.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cqqwz.cn/gtwpiwlagu.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jyoumei.cn/gtyekorrto.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.mhx1999.top/gtgvteeqob.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hysaishi.cn/gtuermjtiu.html

Ruby: rescue ArgumentError => e
来源：http://hz.52xcode.cn/gtrssacxno.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ehwqpu.com/gtbvybsncj.html

[H06] 可选值 / 空值安全访问
来源：http://hz.pycfn.com/gtptnpjbrv.html

Py:   value = d.get("k") or default
来源：http://hz.yj20258.top/gtkxhoakpc.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.daxiang520.top/gtdaatrqhe.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.pycfn.com/gtsdrvbxou.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.vqdsnc.cn/gtnbfuqqyv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yvedp.cn/gtznfgjvsx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.aibaodan.cn/gtnkafrkzi.html

Ruby: d&.dig(:a, :b)
来源：http://hz.haohaochexian.top/gtcsefpxjz.html

C#:   obj?.A?.B ?? default
来源：http://hz.iojbl.cn/gttcrjzemu.html

[H07] 断言
来源：http://hz.hnxiangtu.top/gtmrycsytb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ybcxt.top/gtnczwkswf.html

PHP:  assert($x > 0);
来源：http://hz.yueranfly.top/gtsondakhf.html

JS:   console.assert(x > 0);
来源：http://hz.tianlin.xyz/gtjutncnml.html

TS:   console.assert(x > 0);
来源：http://hz.xinyue.icu/gtlacuhjkp.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zycfv.cn/gtxydgntbo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jqgufenzy.top/gtjpiyyfff.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ppjwa.cn/gtamkrhosd.html

C#:   Debug.Assert(x > 0);
来源：http://hz.fengsongda.top/gtgzuurqyo.html

[H08] 获取错误信息与堆栈
来源：http://hz.fzhhl.top/gttcliebhq.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.bjfxy.top/gttsrtrdgv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.nwbrower.top/gtzppralgd.html

JS:   e.message;  e.stack
来源：http://hz.aibaodan.cn/gtrlpmafvq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.c1oappe.top/gtorgzsopd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xylfe.cn/gtrnyblbzt.html

Go:   err.Error()
来源：http://hz.shangyingyoupin.top/gtdbuuhqfq.html

Ruby: e.message;  e.backtrace
来源：http://hz.wangshuangyany.cn/gtkibgvvmb.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhixingplan.top/gtjnzhnpkt.html

[H09] 带错误码的异常
来源：http://hz.vqdsnc.cn/gtcdsyxuau.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.daxiang520.top/gtzchdcoef.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.mhx1999.top/gtwdqrqrfo.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.smart0.xyz/gtqphiwwsr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.9152youxi.cn/gtogjfwwke.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xuanzx.com/gtiatixmsb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.tian-w.cn/gtyqaldmsp.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.wangshuangyany.cn/gtgccgapdt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.316326.xyz/gtywojddaf.html

[H10] 资源自动释放
来源：http://hz.zhixingplan.top/gtfagbgipv.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhijiandao.cn/gtlijectog.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinghuilouyu.cn/gtmboqpqnp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuanzx.com/gtvraryany.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hnxiangtu.top/gtlylnnfpn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.redwolf501.top/gtjustvckt.html

Go:   defer f.Close()
来源：http://hz.gzhubu.top/gtvyxdrsmp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cashguo.top/gtnrhqlaqf.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.quarkkingdee.top/gtboyyzrqu.html

================================================================================
来源：http://hz.c1oappe.top/gtnkbsjdsw.html

I. 正则表达式
来源：http://hz.jiagoushi.top/gtfhqfpblg.html

================================================================================
来源：http://hz.cqqwz.cn/gtnzvvocjy.html

[I01] 判断是否匹配
来源：http://hz.svipenyu.cn/gtrbywypcg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xingfuxueyuan.xyz/gtrzepywjg.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhiwuduotai.top/gtqssfzayl.html

JS:   /\d+/.test(s)
来源：http://hz.jlsjyb.cn/gthjokmtng.html

TS:   /\d+/.test(s)
来源：http://hz.ybcxt.top/gtoubbvbmh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.hywenlv.cn/gtrxhzluuf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.tian-w.cn/gtrsizfrni.html

Ruby: s.match?(/\d+/)
来源：http://hz.cqqwz.cn/gtmrsnnlet.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.dianchejie.cn/gtzytqfyon.html

[I02] 提取所有匹配
来源：http://hz.ivvv.top/gtlasfuphh.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ivvv.top/gtaakgikbs.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ybcxt.top/gtmjlqcvdc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.gaohongyu789.top/gtpwdzlpdp.html

TS:   s.match(/\d+/g)
来源：http://hz.zhengqikj.top/gtmllijzjz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.haohaochexian.top/gtnaaggjxv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.gzhubu.top/gttlqncoaz.html

Ruby: s.scan(/\d+/)
来源：http://hz.chenlongwang.top/gtlukzuqot.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.snrcjt.cn/gtuztgsnbw.html

[I03] 提取捕获分组
来源：http://hz.sufxvd.cn/gtpdcnakei.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.redwolf501.top/gthugvraid.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shuidangran.top/gtfkbqcvye.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jinqigufen.top/gtuamxdvdc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.haohaochexian.top/gtuwumqtuf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhixingplan.top/gtyzhahjjk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ppjwa.cn/gtnintaqka.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cqqwz.cn/gtfuyodjec.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hnqzz.top/gtcwsshbpy.html

[I04] 正则替换
来源：http://hz.tianlin.xyz/gtmdjvmtvh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.gzhubu.top/gtqdybisyl.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yuxming.cn/gtzwbjtypc.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.guowangkeji.top/gtlokdmoiy.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.havefunace.top/gtsypgfhcy.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.tanke756.top/gtoxibmfqq.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.nwbrower.top/gtrbixqkjm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hnqzz.top/gtpdruvbix.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yonumen.top/gtwywgmsnp.html

[I05] 按正则拆分
来源：http://hz.wangdashe.top/gtrtbnkrga.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zdqjudy.top/gtwzzullqs.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.svipenyu.cn/gtvpyuqvxn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gtihidvhqx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yj20258888.top/gtskufsssh.html

Java: s.split("\\s*,\\s*")
来源：http://hz.cheryme.top/gtlnsuecyg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gzhubu.top/gtwmpqsdhw.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jlsjyb.cn/gtgsyjqhmg.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xziqi.cn/gtvpchuktp.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.dianchejie.cn/gtksfmudie.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.gzhubu.top/gtcoagwnpq.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hnxiangtu.top/gtpjlsgzbv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.pycfn.com/gthcuhquzi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.bjfxy.top/gtfwzpeatu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.redwolf501.top/gthgqurzvy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.wangshuangyany.cn/gtsoqsbftq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yonumen.top/gtcytwjgxf.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jinyuanbaomall.cn/gtgqxevjzb.html

[I07] 忽略大小写与多行模式
来源：http://hz.quarkkingdee.top/gtxjwltwes.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.nwbrower.top/gtapytacol.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hnxiangtu.top/gtkccdrtjd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.daxiang520.top/gthbfkrnev.html

TS:   /error/gim
来源：http://hz.guannengcc.top/gttyfcyffr.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gotoacloud.top/gtdhpozfmp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.tian-w.cn/gtmsygrrkx.html

Ruby: s.scan(/error/i)
来源：http://hz.haohaochexian.top/gtfjybacts.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cheryme.top/gtuxijayui.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yanxiufei.cn/gtzucqwexc.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sweek.top/gtqlwmpoql.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ywan-chungtsiang.top/gtewytptrd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nanxinkj.top/gthvjidfzb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hysaishi.cn/gtyuvwroaw.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.gotoacloud.top/gtxwjbvvzx.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.52xcode.cn/gtfuxiyztc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yueranfly.top/gtvcwsqzoq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.chenjidiqi.icu/gtpszuvfbp.html

================================================================================
来源：http://hz.jqgufenzy.top/gtuqkfnimf.html

J. 日期与时间
来源：http://hz.xingfuxueyuan.xyz/gtpzidxsfm.html

================================================================================
来源：http://hz.andypj.xyz/gtafgedbzz.html

[J01] 获取当前时间
来源：http://hz.yanxiufei.cn/gtcnweqefo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ydzc1.top/gtrjslzicc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.52xcode.cn/gtmtvxwedo.html

JS:   new Date();  Date.now()
来源：http://hz.hongshengwenyu.top/gtpegbhsgn.html

TS:   new Date();  Date.now()
来源：http://hz.dianchejie.cn/gtjjyawktd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.dianchejie.cn/gtvfzgftgz.html

Go:   time.Now()
来源：http://hz.xziqi.cn/gtejovlzcd.html

Ruby: Time.now
来源：http://hz.shangyingyoupin.top/gtakathqea.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.52xcode.cn/gtdxyfieew.html

[J02] 格式化输出
来源：http://hz.fengsongda.top/gtsbzinhmd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cdnleiting.top/gtfcrbivvq.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.chenlongwang.top/gtfjuvihys.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ivvv.top/gtssuzhtpe.html

TS:   d.toISOString()
来源：http://hz.zdqjudy.top/gtanozjvzd.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jiagoushi.top/gtsgiklijy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.xziqi.cn/gthnhaihtt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxuanxn.top/gtihfxygua.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gzhubu.top/gtuimeuijx.html

[J03] 字符串解析为日期
来源：http://hz.jiagoushi.top/gtaehptqxh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.sweek.top/gtstcfxfiu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jqgfzy.top/gtogsxyadq.html

JS:   new Date("2024-01-02")
来源：http://hz.yongpay.top/gtumbiwohx.html

TS:   new Date("2024-01-02")
来源：http://hz.jlsjyb.cn/gtryfeiwzx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.haohaochexian.top/gtesacsnjx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.sufxvd.cn/gtlvvcirvs.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.mhx1999.top/gtpqccssuq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.guowangkeji.top/gtkblrmgyj.html

[J04] 时间戳与日期互转
来源：http://hz.jinyuanbaomall.cn/gthsywcrcb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhixingplan.top/gtbxsdpnyf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.nanxuanxn.top/gtjyxbkbzl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.daxiang520.top/gtztwjjhxd.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cheryme.top/gtvntfigzq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.gzhubu.top/gtowowbemr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.feifeiyinyue.top/gtpuukczvn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhengqikj.top/gtmvmdpoiu.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.havefunace.top/gtafcpoork.html

[J05] 时间加减（加 7 天）
来源：http://hz.ywan-chungtsiang.top/gtdkurzrax.html

Py:   now + timedelta(days=7)
来源：http://hz.chenzaomai.com/gtlflycvjq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ydzc1.top/gtledvkymo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhaomingkeji.xyz/gtyowwppnb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zycfv.cn/gtlwzczirv.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinghuilouyu.cn/gtoyblxoox.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yuxming.cn/gtaczlunao.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gogol.net.cn/gtqkkunhtw.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.chenlongwang.top/gtlwailehd.html

[J06] 计算两时间之差
来源：http://hz.jyoumei.cn/gtpfrydtwn.html

Py:   (end - start).total_seconds()
来源：http://hz.shanyushiyangkeji.top/gtmazjcvfv.html

PHP:  $end->diff($start)->days;
来源：http://hz.fzhhl.top/gtsztqljxr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.nanxinkj.top/gtufrfmudl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinghuilouyu.cn/gtioxqwjkp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hysaishi.cn/gtajiyxnbj.html

Go:   end.Sub(start).Hours()
来源：http://hz.tian-w.cn/gtelzdyuhi.html

Ruby: end - start                 # 返回秒数
来源：http://hz.birdmap.top/gtoldezvif.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhaomingkeji.xyz/gtespyqhgz.html

[J07] 比较两个日期
来源：http://hz.c1oappe.top/gtbfhqimpu.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.hysaishi.cn/gtbeefmgyx.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.chenjidiqi.icu/gtdgzykxwj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258888.top/gtflffttkn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.shangyingyoupin.top/gtzhkrpwyb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jinyuanbaomall.cn/gtouekmhnp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.havefunace.top/gtymwjpbrp.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.chenlongwang.top/gthewiwhlu.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shanyushiyangkeji.top/gtugfceudq.html

[J08] 提取年月日与星期
来源：http://hz.mhx1999.top/gtxqnxvpft.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.aizwys.cn/gtsgngmbuu.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.hfpthk.cn/gtqzbonbmj.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.hongshengwenyu.top/gtmikbektx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.wangdashe.top/gtguisptlz.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.vqdsnc.cn/gtxhqqgxfl.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jqgfzy.top/gtzrjpispd.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jinghuilouyu.cn/gtpqkusnmx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xuanzx.com/gtrfxjowtv.html

[J09] 时区处理
来源：http://hz.jianghu66.top/gtqjgfacdb.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.tanke756.top/gtdczbjdnu.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xingfuxueyuan.xyz/gtretyhkey.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cheryme.top/gtdllybuss.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.mhx1999.top/gtanzaptzy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.9152youxi.cn/gtwrkujzhg.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.chenlongwang.top/gtrhgfpiea.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.daxiang520.top/gtenxyyknh.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.aibaodan.cn/gtlylgtlhw.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinqigfzy.top/gtnmderseu.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jianghu66.top/gtyhrzxflg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhongyouzk.top/gtyetorbuf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.sweek.top/gtzutdgrjm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cucudq.cn/gtvsfxkdru.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zdqjudy.top/gtovshwmjg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gogol.net.cn/gtccohhhne.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gzhubu.top/gtqsushnyu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shanyushiyangkeji.top/gtmztgixbg.html

================================================================================
来源：http://hz.gogol.net.cn/gtvppfgtob.html

K. JSON 与序列化
来源：http://hz.yonumen.top/gtiezrahwl.html

================================================================================
来源：http://hz.yj20258888.top/gthvptofzq.html

[K01] 对象转 JSON 字符串
来源：http://hz.smart0.xyz/gtotfwpkmu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.tianlin.xyz/gtjcakicpk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.yangfankeji.com/gtepfvivyb.html

JS:   JSON.stringify(obj)
来源：http://hz.0kj1m.cn/gtqijyrwpy.html

TS:   JSON.stringify(obj)
来源：http://hz.316326.xyz/gtzelqfhkr.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ybcxt.top/gtvjvkfuzf.html

Go:   json.Marshal(obj)
来源：http://hz.fzhhl.top/gtgjthbpbx.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.aizwys.cn/gtbxtuxgng.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.nanxuanxn.top/gtupufdvtn.html

[K02] JSON 字符串转对象
来源：http://hz.zhongyouzk.top/gtvpllxomy.html

Py:   json.loads(s)
来源：http://hz.c1oappe.top/gtykutoeaj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yuanzhike.top/gtpyjtjqyd.html

JS:   JSON.parse(s)
来源：http://hz.tanke756.top/gtnikdslvt.html

TS:   JSON.parse(s)
来源：http://hz.zhaomingkeji.xyz/gtleqpzuba.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.xylfe.cn/gtpkfqgbpq.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.chenzaomai.com/gtbcsydael.html

Ruby: JSON.parse(s)
来源：http://hz.yueranfly.top/gtevksfzom.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.jlsjyb.cn/gtpigtjein.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.svipenyu.cn/gtvanhbxrk.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zhijiandao.cn/gtrvlbpnkv.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinyuanbaomall.cn/gtayizppif.html


<!-- 参考信息 -->