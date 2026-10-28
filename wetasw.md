代发 wailian999

PHP:  get_object_vars($obj);
来源：http://hz.zhengqikj.top/gtqzibcyra.html

JS:   Object.entries(obj)
来源：http://hz.dashuyun.cn/gtccxenabp.html

TS:   Object.entries(obj)
来源：http://hz.aibaodan.cn/gtbzvzkvws.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.shangyingyoupin.top/gthntuuugt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.smart0.xyz/gtigupwdhw.html

Ruby: obj.instance_variables
来源：http://hz.guowangkeji.top/gtrkhzzpkm.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.nwbrower.top/gtlknwkznk.html

================================================================================
来源：http://hz.havefunace.top/gtzxcmbdhz.html

H. 异常与错误处理
来源：http://hz.yj20258888.top/gtwysmicem.html

================================================================================
来源：http://hz.52xcode.cn/gtduubjvhm.html

[H01] try / catch 基础
来源：http://hz.jqgufenzy.top/gtbzimepjx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jinqigufen.top/gtqaxqfaqs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yuanzhike.top/gtsziqovac.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hywenlv.cn/gtbizpigte.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.dianchejie.cn/gtckljupfm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yvedp.cn/gtfuttnpjv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.feifeiyinyue.top/gtlrovgobk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.shanyushiyangkeji.top/gthledblho.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yueranfly.top/gtjasoaluw.html

[H02] finally / ensure 收尾
来源：http://hz.yj202588.top/gtjnjzepqp.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.wangdashe.top/gtscyfriai.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gtjehikwfp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtawgosyeh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.gotoacloud.top/gtqxgstdyi.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ywan-chungtsiang.top/gtzdvtsncb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.vqdsnc.cn/gtpkegwijf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.gzhubu.top/gtncukqpon.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.iojbl.cn/gtmqkhtvuw.html

[H03] 主动抛出异常
来源：http://hz.ydzc1.top/gtqblbtgnf.html

Py:   raise ValueError("错误信息")
来源：http://hz.svipenyu.cn/gttmbsvuhs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.vqdsnc.cn/gteqbpugfr.html

JS:   throw new Error("错误信息");
来源：http://hz.shuidangran.top/gtyduekhpf.html

TS:   throw new Error("错误信息");
来源：http://hz.hongshengwenyu.top/gtoqolvidp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.dianchejie.cn/gtixyxrqfb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.gotoacloud.top/gtebkpipyo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.shanyushiyangtech.top/gtzsjflihc.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ivvv.top/gtjnmoozop.html

[H04] 自定义异常类型
来源：http://hz.yangfankeji.com/gtbglybrdd.html

Py:   class MyError(Exception): pass
来源：http://hz.c1oappe.top/gtoanhsakb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.gotoacloud.top/gtgsaeqgqt.html

JS:   class MyError extends Error {}
来源：http://hz.iojbl.cn/gtgogjfior.html

TS:   class MyError extends Error {}
来源：http://hz.hammf.cn/gtrcshatza.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hywenlv.cn/gtdlulgwys.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yj20258.top/gtbqbdkrsf.html

Ruby: class MyError < StandardError; end
来源：http://hz.yongpay.top/gtwyjqsvrt.html

C#:   class MyException : Exception {}
来源：http://hz.hammf.cn/gtgammaqwd.html

[H05] 捕获特定类型
来源：http://hz.shzxlz.cn/gtxfdwcont.html

Py:   except ValueError as e:
来源：http://hz.chenlongwang.top/gtoiqgoqfj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.cheryme.top/gttqrucybv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.shangyingyoupin.top/gtquthargb.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.daxiang520.top/gtzylpvzfb.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhijiandao.cn/gtkklwixjp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ydjk.org.cn/gtfyajgnis.html

Ruby: rescue ArgumentError => e
来源：http://hz.hammf.cn/gtfcerwvrm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.gaohongyu789.top/gtdfnzuinz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yuxming.cn/gtowpcbeme.html

Py:   value = d.get("k") or default
来源：http://hz.tian-w.cn/gtjizmexzh.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hammf.cn/gtfetblkyk.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.quarkkingdee.top/gtjlugabcc.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sufxvd.cn/gtmikacfqo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gaohongyu789.top/gttxyvuobd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.iojbl.cn/gtjovzxznv.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hammf.cn/gtubruouyc.html

C#:   obj?.A?.B ?? default
来源：http://hz.yuanzhike.top/gtavumgtqq.html

[H07] 断言
来源：http://hz.svipenyu.cn/gtebsfycvq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.nwbrower.top/gttvfoqsgb.html

PHP:  assert($x > 0);
来源：http://hz.sweek.top/gtlqxjqypi.html

JS:   console.assert(x > 0);
来源：http://hz.dashuyun.cn/gtibyqhcqi.html

TS:   console.assert(x > 0);
来源：http://hz.ivvv.top/gtjhxcolln.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yangfankeji.com/gtzkyehzja.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ydjk.org.cn/gtkdfscvkn.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.nanxuanxn.top/gtthemnmov.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cashguo.top/gtgynavmbq.html

[H08] 获取错误信息与堆栈
来源：http://hz.ivvv.top/gtegkukqrv.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.fzhhl.top/gtclycfbtg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xziqi.cn/gtfquorzde.html

JS:   e.message;  e.stack
来源：http://hz.hysaishi.cn/gtccdsgigu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.haohaochexian.top/gtxpmdjgov.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.cheryme.top/gtlgacyqfl.html

Go:   err.Error()
来源：http://hz.jianghu66.top/gtjgnhqtau.html

Ruby: e.message;  e.backtrace
来源：http://hz.xuetiantiany.cn/gtqzrynsyj.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ppjwa.cn/gtdqnrqjqf.html

[H09] 带错误码的异常
来源：http://hz.nanxuanxn.top/gttewjjgue.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.wangdashe.top/gtyqgyflql.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shanyushiyangkeji.top/gtvnxwtgpz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.vqdsnc.cn/gtduopxxmw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.wangdashe.top/gtrzrhkpvq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhengqikj.top/gtgwiqtxwl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhixingplan.top/gtstoemeop.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.kuanghao11.cn/gtlcdbflcl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.nanxinkj.top/gtmxgzkozf.html

[H10] 资源自动释放
来源：http://hz.yj20258888.top/gtfglywkvc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yuanzhike.top/gtvjuowona.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.andypj.xyz/gtoucodjux.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ybcxt.top/gtifhbxsny.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hammf.cn/gtfmuflepp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.gotoacloud.top/gtgnxthpgc.html

Go:   defer f.Close()
来源：http://hz.tian-w.cn/gtmqvlkhrf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.ybcxt.top/gtfpwbhezv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.nwbrower.top/gtbfrkfvzm.html

================================================================================
来源：http://hz.wangdashe.top/gtpvurisxm.html

I. 正则表达式
来源：http://hz.jqgfzy.top/gtrzkulpfd.html

================================================================================
来源：http://hz.ybcxt.top/gtcjrhmatd.html

[I01] 判断是否匹配
来源：http://hz.hnxiangtu.top/gturxsaodc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xingfuxueyuan.xyz/gtyplxfghw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hfpthk.cn/gtpbixgwuh.html

JS:   /\d+/.test(s)
来源：http://hz.tanke756.top/gtknvnjfwb.html

TS:   /\d+/.test(s)
来源：http://hz.cucudq.cn/gtpgbrpvtn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.nwbrower.top/gtutwidtyx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jinqigfzy.top/gtsfmguvvn.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhongyouzk.top/gtamwmxvcj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yanxiufei.cn/gtuozomuda.html

[I02] 提取所有匹配
来源：http://hz.dashuyun.cn/gtvopcxijr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zycfv.cn/gttkxtpzkg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.redwolf501.top/gtemllouze.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinqigfzy.top/gtdnerdzxk.html

TS:   s.match(/\d+/g)
来源：http://hz.cucudq.cn/gtvbvdlxnh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jiagoushi.top/gtwpuvkmib.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhijiandao.cn/gtkkgrlrit.html

Ruby: s.scan(/\d+/)
来源：http://hz.xuanzx.com/gtztmpdsvf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shanyushiyangtech.top/gtqomzbwmg.html

[I03] 提取捕获分组
来源：http://hz.hfpthk.cn/gthynofohq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhixingplan.top/gtjeoomikj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xingfuxueyuan.xyz/gtrfmnchqp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xinyue.icu/gtetbhojub.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xinyue.icu/gtehuwlxkv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.gogol.net.cn/gtjqklimvv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.meibo888.top/gtxhppvcyl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yuxming.cn/gtftzooeli.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hongshengwenyu.top/gtazvnepwk.html

[I04] 正则替换
来源：http://hz.pengpengdd.cyou/gtthoakgor.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.chenlongwang.top/gtikuhvdcv.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shanyushiyangkeji.top/gtyciufqol.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ehwqpu.com/gtaraaqzly.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.tanke756.top/gtltlowguu.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.nwbrower.top/gtjuqztfhf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.aizwys.cn/gtywsvadrv.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hnxiangtu.top/gtaqwrdwsv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xylfe.cn/gtmsosenjb.html

[I05] 按正则拆分
来源：http://hz.dianchejie.cn/gtakgplraq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.aibaodan.cn/gtgqnqdiij.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.meibo888.top/gtnhxroztc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hfpthk.cn/gtdapjvvsr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yangfankeji.com/gtokrbpysp.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhengqikj.top/gtntntdgvw.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xuanzx.com/gtpxfosaaj.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jinqigufen.top/gttaevwgip.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hnqzz.top/gttdmkgljs.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.ydjk.org.cn/gtosyotdcz.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gtvahofvgb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ydjk.org.cn/gtospxrjgz.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yuxming.cn/gtngsmmdjd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cdnleiting.top/gtmqrnzbyf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.smart0.xyz/gtyrcfzazp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.wangdashe.top/gtelmxxozd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shangyingyoupin.top/gtwvdvmsre.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.tanke756.top/gtskufalgg.html

[I07] 忽略大小写与多行模式
来源：http://hz.yongpay.top/gtmrvkcizm.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.chenzaomai.com/gtiskohmfk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhiwuduotai.top/gtgprvtvwl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xuetiantiany.cn/gtnfobruui.html

TS:   /error/gim
来源：http://hz.andypj.xyz/gtcegofpqo.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.fzhhl.top/gtizgnudsm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.haohaochexian.top/gtzdlsoxec.html

Ruby: s.scan(/error/i)
来源：http://hz.tanke756.top/gtpatmewxr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.c1oappe.top/gtcitqyqxj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ivvv.top/gtuzelcjco.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.chenjidiqi.icu/gttlsboyjc.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhiwuduotai.top/gtgyorqtcb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cucudq.cn/gtqasuovkk.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnxiangtu.top/gtpqvjifwq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.jqgufenzy.top/gttacbkrmi.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jiagoushi.top/gtmnupdppu.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.316326.xyz/gtueqqttdo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gzhubu.top/gttretcira.html

================================================================================
来源：http://hz.xinyue.icu/gtuqhyzsfp.html

J. 日期与时间
来源：http://hz.hywenlv.cn/gtvgiychwe.html

================================================================================
来源：http://hz.zhengqikj.top/gtkgaxldgm.html

[J01] 获取当前时间
来源：http://hz.chenzaomai.com/gtvxblgaqq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.52xcode.cn/gtpszpdyhc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jinqigfzy.top/gtmgudvzew.html

JS:   new Date();  Date.now()
来源：http://hz.daxiang520.top/gteytidyfc.html

TS:   new Date();  Date.now()
来源：http://hz.tian-w.cn/gtxaaevamz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.yonumen.top/gtufybpoyq.html

Go:   time.Now()
来源：http://hz.guannengcc.top/gtligfmabb.html

Ruby: Time.now
来源：http://hz.smart0.xyz/gtfgjxrpae.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.nwbrower.top/gtbcqrsrzg.html

[J02] 格式化输出
来源：http://hz.ppjwa.cn/gtuytlatpy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ehwqpu.com/gtsenjgknz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.nanxinkj.top/gtnrhwhxnv.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yj20258.top/gtznzvigrv.html

TS:   d.toISOString()
来源：http://hz.wangshuangyany.cn/gtvocfezjp.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.tian-w.cn/gtpoqkiphj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.snrcjt.cn/gtbitquqou.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xuetiantiany.cn/gtbhaojpzn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhongyouzk.top/gttxnqvwfc.html

[J03] 字符串解析为日期
来源：http://hz.tanke756.top/gttrchjfpd.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.wangdashe.top/gtlzassxdm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.guowangkeji.top/gtfouhgrjp.html

JS:   new Date("2024-01-02")
来源：http://hz.sufxvd.cn/gtvijxpuhk.html

TS:   new Date("2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gtjkpenpsg.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hammf.cn/gtwnfocxfx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yangfankeji.com/gtmbnbwecy.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gzhubu.top/gtasmdcoal.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.aizwys.cn/gtwqofmceu.html

[J04] 时间戳与日期互转
来源：http://hz.sweek.top/gtbngheglh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yuanzhike.top/gtyalcimnb.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.smart0.xyz/gtdowtrwrc.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.xuetiantiany.cn/gtbzngkyqv.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhixingplan.top/gtxzitxoee.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhengqikj.top/gtgxlznkqo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yuxming.cn/gttdarrfpf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jianghu66.top/gtyfwmnuzm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.daria6918.cn/gtqvdkgofl.html

[J05] 时间加减（加 7 天）
来源：http://hz.chenjidiqi.icu/gtvdkqncdj.html

Py:   now + timedelta(days=7)
来源：http://hz.gaohongyu789.top/gtbjovvsjk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jinghuilouyu.cn/gtksluubjy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ydjk.org.cn/gtuddpvalf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gotoacloud.top/gtkivefrnk.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.52xcode.cn/gthidgbcge.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ppjwa.cn/gtyqbksovp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.cucudq.cn/gteuippngo.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hongshengwenyu.top/gtgojymvzr.html

[J06] 计算两时间之差
来源：http://hz.jiagoushi.top/gtftuzzjkj.html

Py:   (end - start).total_seconds()
来源：http://hz.jlsjyb.cn/gttctqjbcb.html

PHP:  $end->diff($start)->days;
来源：http://hz.aizwys.cn/gtvwrgtohf.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.gaohongyu789.top/gtjwcsnrsm.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.wangshuangyany.cn/gtnpcmdfci.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhiwuduotai.top/gtwetqmcjf.html

Go:   end.Sub(start).Hours()
来源：http://hz.sysykeji.top/gteyfqwalx.html

Ruby: end - start                 # 返回秒数
来源：http://hz.nanxinkj.top/gtheljahtc.html

C#:   (end - start).TotalSeconds
来源：http://hz.ydjk.org.cn/gtapxxncbo.html

[J07] 比较两个日期
来源：http://hz.snrcjt.cn/gtpawyrikk.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.pycfn.com/gtkumvigei.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hfpthk.cn/gtygyftfpj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zycfv.cn/gtmsyuodva.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jlsjyb.cn/gtcadmvxbe.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.meibo888.top/gtmopxwbay.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.guannengcc.top/gtsdktmnub.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yvedp.cn/gtjexfyoku.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gtypgblhef.html

[J08] 提取年月日与星期
来源：http://hz.hnqzz.top/gtsyjlijlz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.daria6918.cn/gtecvsfqfs.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yonumen.top/gtplhykmwp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.svipenyu.cn/gtxjrsxhfj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.jyoumei.cn/gtcwoinoiy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.smart0.xyz/gtpnwwozbs.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenjidiqi.icu/gtwfjxmvof.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.0kj1m.cn/gtrwubspwg.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.chenzaomai.com/gtgzpgicas.html

[J09] 时区处理
来源：http://hz.c1oappe.top/gtgkunmpnm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.guannengcc.top/gtokfykshi.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.316326.xyz/gtlzvimghy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xuanzx.com/gtexpoforh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.andypj.xyz/gtvijnhtyk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.chenzaomai.com/gtcisffuav.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.ppjwa.cn/gtyoxgclpl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.tian-w.cn/gtmtddmngc.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.birdmap.top/gtqntaplne.html

[J10] 取今天 / 本月第一天
来源：http://hz.jianghu66.top/gtarviufoo.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xinyue.icu/gtrecldbbs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xuanzx.com/gtlitktfki.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.feifeiyinyue.top/gtllkvoynw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gotoacloud.top/gtalkxibvh.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sweek.top/gtaukslwmx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jqgfzy.top/gtfzotfhgm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.shangyingyoupin.top/gtiudufbyp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ywan-chungtsiang.top/gtkcvzjvnv.html

================================================================================
来源：http://hz.jqgfzy.top/gthuuppzwd.html

K. JSON 与序列化
来源：http://hz.sweek.top/gtjmidnvka.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtbzozhrqk.html

[K01] 对象转 JSON 字符串
来源：http://hz.yvedp.cn/gtrhoqufhz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.yueranfly.top/gttnnqypge.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.iojbl.cn/gtgeyeacuw.html

JS:   JSON.stringify(obj)
来源：http://hz.fzhhl.top/gtghznfzap.html

TS:   JSON.stringify(obj)
来源：http://hz.yj202588.top/gttyegcxqw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hongshengwenyu.top/gtikyshlop.html

Go:   json.Marshal(obj)
来源：http://hz.hfpthk.cn/gtyuqewaoe.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinghuilouyu.cn/gtfdavxthe.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.tanke756.top/gtikqkuroh.html

[K02] JSON 字符串转对象
来源：http://hz.zhoulong.xyz/gtnrpcjnnt.html

Py:   json.loads(s)
来源：http://hz.xuetiantiany.cn/gtrbyiihbo.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.zhoulong.xyz/gtuywoaeva.html

JS:   JSON.parse(s)
来源：http://hz.birdmap.top/gtarwsojkl.html

TS:   JSON.parse(s)
来源：http://hz.cucudq.cn/gtvfabrgpg.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.mhx1999.top/gtzccahopz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.daxiang520.top/gtgggzlfhz.html

Ruby: JSON.parse(s)
来源：http://hz.jianghu66.top/gtartspbxv.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.ywan-chungtsiang.top/gtyjlrsajr.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zdqjudy.top/gtbeyzatpa.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.ppjwa.cn/gtivzgvpsa.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yvedp.cn/gtnaagsiwv.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.bjfxy.top/gtijhkeqkp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.mhx1999.top/gtaourjnuz.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.ppjwa.cn/gtdnmmjncp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.daria6918.cn/gtkmvbqwwy.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.c1oappe.top/gtosinxzbg.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zdqjudy.top/gtbpqreily.html

[K04] 读取 JSON 文件
来源：http://hz.hammf.cn/gtuurdmnja.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.jinyuanbaomall.cn/gtvmglogmu.html


<!-- 参考信息 -->