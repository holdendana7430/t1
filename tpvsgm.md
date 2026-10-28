代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.aibaodan.cn/gtbcwhysyp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hongshengwenyu.top/gtqacvbzlb.html

Java: enum Color { RED, GREEN }
来源：http://hz.meibo888.top/gtamkqfjhd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xziqi.cn/gtivwiyghr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.wangdashe.top/gtcjhhumpf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.feifeiyinyue.top/gtextqqrpo.html

[G16] 对象转数组 / 字典
来源：http://hz.shuidangran.top/gtiiejgfhw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xingfuxueyuan.xyz/gtenozpodo.html

PHP:  get_object_vars($obj);
来源：http://hz.xylfe.cn/gtoujplvop.html

JS:   Object.entries(obj)
来源：http://hz.xuanzx.com/gtvpjttrel.html

TS:   Object.entries(obj)
来源：http://hz.yj202588.top/gtzejaetbg.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yangfankeji.com/gtfvjfwgzw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.smart0.xyz/gtlxbpnhrt.html

Ruby: obj.instance_variables
来源：http://hz.gaohongyu789.top/gtjedquocj.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cqqwz.cn/gtnkovcfhh.html

================================================================================
来源：http://hz.xinyue.icu/gtzqjctxtx.html

H. 异常与错误处理
来源：http://hz.gotoacloud.top/gtkzkhgmgq.html

================================================================================
来源：http://hz.jqgfzy.top/gtrlbrmory.html

[H01] try / catch 基础
来源：http://hz.yuxming.cn/gtgvsutpzy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.aibaodan.cn/gtbkvlsmpc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.haohaochexian.top/gtmghnzzfd.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jqgufenzy.top/gtorozjxtq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xuanzx.com/gtlnuknuqx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinghuilouyu.cn/gtmpxfdnpd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.aibaodan.cn/gtcujubhlv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jyoumei.cn/gtwbvjqzra.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.sweek.top/gtuttennkj.html

[H02] finally / ensure 收尾
来源：http://hz.xuetiantiany.cn/gttnyjnqfp.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.316326.xyz/gtfbswnrrg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jinqigufen.top/gtrvkdpbai.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj202588.top/gtwwwrhyab.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtvdsyavgw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtfudnuwpj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xuanzx.com/gtapgfqave.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xinyue.icu/gtqkkamluj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.chenzaomai.com/gtykycfpsx.html

[H03] 主动抛出异常
来源：http://hz.9152youxi.cn/gtflkdtmil.html

Py:   raise ValueError("错误信息")
来源：http://hz.wangshuangyany.cn/gtigpwivub.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.dashuyun.cn/gtistafwqr.html

JS:   throw new Error("错误信息");
来源：http://hz.redwolf501.top/gtbcmejprb.html

TS:   throw new Error("错误信息");
来源：http://hz.xylfe.cn/gtpzynjvcw.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.0kj1m.cn/gtzpapjonc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.nanxuanxn.top/gtojwrxxuk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cqqwz.cn/gtsbfvybfb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.chenzaomai.com/gtpuegtlie.html

[H04] 自定义异常类型
来源：http://hz.dianchejie.cn/gtjdjyuoqy.html

Py:   class MyError(Exception): pass
来源：http://hz.cqqwz.cn/gthravnbgy.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jinghuilouyu.cn/gtvsfzzgji.html

JS:   class MyError extends Error {}
来源：http://hz.ydjk.org.cn/gtuamsjylp.html

TS:   class MyError extends Error {}
来源：http://hz.gogol.net.cn/gtojxmtfdw.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xuanzx.com/gtbrnxavjd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.fengsongda.top/gtpixpoaca.html

Ruby: class MyError < StandardError; end
来源：http://hz.kuanghao11.cn/gtvnnchxgc.html

C#:   class MyException : Exception {}
来源：http://hz.mhx1999.top/gtvijklwel.html

[H05] 捕获特定类型
来源：http://hz.zhijiandao.cn/gtpjswtamd.html

Py:   except ValueError as e:
来源：http://hz.fengsongda.top/gtzfbnuesj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhijiandao.cn/gtirfdaltk.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.gaohongyu789.top/gtfkkmbmla.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yj20258.top/gtborgutoh.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yj202588.top/gthfsgvqca.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hnqzz.top/gtwwggnlup.html

Ruby: rescue ArgumentError => e
来源：http://hz.redwolf501.top/gtvqncexap.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yuanzhike.top/gtpjwllyao.html

[H06] 可选值 / 空值安全访问
来源：http://hz.feifeiyinyue.top/gtpdxaclrz.html

Py:   value = d.get("k") or default
来源：http://hz.xylfe.cn/gthepdqbkj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.svipenyu.cn/gtxxovmmud.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.bjfxy.top/gtfuvtfqjb.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.pengpengdd.cyou/gthjvwrxha.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.feifeiyinyue.top/gtnsuhveyh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ywan-chungtsiang.top/gtaasdfhuc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jqgfzy.top/gtjhripswk.html

C#:   obj?.A?.B ?? default
来源：http://hz.chenzaomai.com/gtotxikffy.html

[H07] 断言
来源：http://hz.sysykeji.top/gtfnucsfrq.html

Py:   assert x > 0, "必须为正"
来源：http://hz.ywan-chungtsiang.top/gtmxjlksph.html

PHP:  assert($x > 0);
来源：http://hz.andypj.xyz/gtdjlhsuvy.html

JS:   console.assert(x > 0);
来源：http://hz.shangyingyoupin.top/gthufraszm.html

TS:   console.assert(x > 0);
来源：http://hz.dashuyun.cn/gtuzvujvvp.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhijiandao.cn/gthzqnrnlp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xziqi.cn/gtoptoumlq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.wangdashe.top/gtmkaxajhe.html

C#:   Debug.Assert(x > 0);
来源：http://hz.iojbl.cn/gtdcvrrwhf.html

[H08] 获取错误信息与堆栈
来源：http://hz.ydzc1.top/gtriuafiix.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.pengpengdd.cyou/gtovqiypqk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yvedp.cn/gtjljbvhkn.html

JS:   e.message;  e.stack
来源：http://hz.fzhhl.top/gtcmixjlaj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.sysykeji.top/gtloavpwtt.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.dianchejie.cn/gtefxoeajh.html

Go:   err.Error()
来源：http://hz.gogol.net.cn/gtueygekhe.html

Ruby: e.message;  e.backtrace
来源：http://hz.ydzc1.top/gtpuwarooc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.daria6918.cn/gtlzsftgyt.html

[H09] 带错误码的异常
来源：http://hz.xylfe.cn/gtdhrwufoy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.wangshuangyany.cn/gtllkfajlo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.feifeiyinyue.top/gtzjujobvg.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.quarkkingdee.top/gtzrssmysd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ivvv.top/gtmyjyyywx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zdqjudy.top/gtbovirxne.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sufxvd.cn/gtucjslwdg.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yangfankeji.com/gtnomzjddx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhengqikj.top/gtypnbdypy.html

[H10] 资源自动释放
来源：http://hz.iojbl.cn/gtmdcaxmtx.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.guowangkeji.top/gtzfmyvoyl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.guannengcc.top/gtgipdcbsx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangtech.top/gtfsvttlvw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhoulong.xyz/gthlyccsuv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hammf.cn/gtnbamgkvk.html

Go:   defer f.Close()
来源：http://hz.ywan-chungtsiang.top/gtnxoiswwq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.sufxvd.cn/gtepwcllxy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jqgfzy.top/gtzqreahxs.html

================================================================================
来源：http://hz.hnqzz.top/gtwojkqhea.html

I. 正则表达式
来源：http://hz.wangdashe.top/gtxdqxmreq.html

================================================================================
来源：http://hz.dashuyun.cn/gtkdphpbhb.html

[I01] 判断是否匹配
来源：http://hz.tanke756.top/gtvcuhyjob.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.aibaodan.cn/gtpmsenbek.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.wangshuangyany.cn/gtddzobker.html

JS:   /\d+/.test(s)
来源：http://hz.c1oappe.top/gteesslxkh.html

TS:   /\d+/.test(s)
来源：http://hz.yj20258888.top/gtvumgobfu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cqqwz.cn/gtgztxqken.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hnxiangtu.top/gtkdgwmxqd.html

Ruby: s.match?(/\d+/)
来源：http://hz.yanxiufei.cn/gtxysfltcl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinghuilouyu.cn/gtgbyijtok.html

[I02] 提取所有匹配
来源：http://hz.meibo888.top/gtxhgojuoj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.tanke756.top/gtincpaxzb.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yj20258888.top/gtuplsivcb.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.kuanghao11.cn/gtielplfkd.html

TS:   s.match(/\d+/g)
来源：http://hz.xingfuxueyuan.xyz/gtlotxncek.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hywenlv.cn/gtmficqquu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yj20258.top/gtppyrsvqk.html

Ruby: s.scan(/\d+/)
来源：http://hz.bjfxy.top/gtqaamdckp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.andypj.xyz/gtowwxqmyj.html

[I03] 提取捕获分组
来源：http://hz.zhengqikj.top/gtxgjwgzfy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.c1oappe.top/gtsgssnfte.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.mhx1999.top/gtzyrrtkgb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hongshengwenyu.top/gteelfbatu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.nanxinkj.top/gturkgsdhg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hnqzz.top/gtkkfuzily.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj202588.top/gtpjuncgkf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhengqikj.top/gtnnnwkkcq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.nwbrower.top/gtwnytchjg.html

[I04] 正则替换
来源：http://hz.snrcjt.cn/gtcmkqgojn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.svipenyu.cn/gtxjluagfi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.guannengcc.top/gtybbmrugf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.birdmap.top/gtsjjpgfgm.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yonumen.top/gtazmprnbs.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.tanke756.top/gtjqanfnqn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.jinghuilouyu.cn/gtapwbaigi.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.9152youxi.cn/gtojqmonha.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.vqdsnc.cn/gtptvklyge.html

[I05] 按正则拆分
来源：http://hz.ehwqpu.com/gtgcgkjodl.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.sysykeji.top/gtzrzuaout.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.fengsongda.top/gthjlvphqm.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gtmrbreeng.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.guannengcc.top/gtegqghaqp.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yuxming.cn/gtvfscdrir.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yuxming.cn/gtwgeilxmz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangkeji.top/gtgzcirnnm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.aibaodan.cn/gtwriecmxr.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.feifeiyinyue.top/gtuykytqzu.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.sxryk.cn/gtmfgxtrux.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.wangshuangyany.cn/gtxymcnymo.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgfzy.top/gtflxspugo.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.nanxuanxn.top/gtyihxmruf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jqgufenzy.top/gtvxakwldk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ybcxt.top/gtgcndtppj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.vqdsnc.cn/gtfbiqjhhh.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.0kj1m.cn/gtvblmycnf.html

[I07] 忽略大小写与多行模式
来源：http://hz.hywenlv.cn/gtdrzjefen.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shanyushiyangtech.top/gtkwmryvcz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.bjfxy.top/gthiqbnsdw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ehwqpu.com/gtgskngstu.html

TS:   /error/gim
来源：http://hz.snrcjt.cn/gthskfocfq.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xuanzx.com/gtxbeiqvxq.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.52xcode.cn/gtuurmayjz.html

Ruby: s.scan(/error/i)
来源：http://hz.aizwys.cn/gtvnwxuvxf.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinqigfzy.top/gtsimbuhkq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zdqjudy.top/gtvisdoact.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.hammf.cn/gtwltbruoj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yonumen.top/gtprmhnnnh.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sxryk.cn/gtqoupssbh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zycfv.cn/gtnjkuvfjy.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ydzc1.top/gtbstxoplk.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.tianlin.xyz/gtqxotzpzf.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yj20258888.top/gtpcfwlqxb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jqgfzy.top/gtpukpcadu.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtxitihjsm.html

J. 日期与时间
来源：http://hz.yuanzhike.top/gtjokfyfvs.html

================================================================================
来源：http://hz.daria6918.cn/gtqdtmlcio.html

[J01] 获取当前时间
来源：http://hz.tianlin.xyz/gtxtoxsqkq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shanyushiyangtech.top/gtbgovmsyp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.dashuyun.cn/gtxjxssohe.html

JS:   new Date();  Date.now()
来源：http://hz.ehwqpu.com/gtitsozssr.html

TS:   new Date();  Date.now()
来源：http://hz.pengpengdd.cyou/gtvkbejjbz.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.52xcode.cn/gtkkdiztzd.html

Go:   time.Now()
来源：http://hz.ehwqpu.com/gtpmwcaien.html

Ruby: Time.now
来源：http://hz.dianchejie.cn/gtndjzzopd.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hywenlv.cn/gtqbhdeyax.html

[J02] 格式化输出
来源：http://hz.yuanzhike.top/gtzromlpfi.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258888.top/gtnedmtfzt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.hnxiangtu.top/gtoitqrygu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.pycfn.com/gtmisxizty.html

TS:   d.toISOString()
来源：http://hz.gogol.net.cn/gtezwjekvk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hnqzz.top/gtxmwonnom.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gaohongyu789.top/gtdlhfcbhi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tian-w.cn/gtulbxmbzv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shangyingyoupin.top/gtgadcbveg.html

[J03] 字符串解析为日期
来源：http://hz.pycfn.com/gtinofuaye.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.pengpengdd.cyou/gtiitcucem.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.zhixingplan.top/gtdilxdldk.html

JS:   new Date("2024-01-02")
来源：http://hz.dashuyun.cn/gtydmgxzvt.html

TS:   new Date("2024-01-02")
来源：http://hz.yangfankeji.com/gtgptqxush.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.bjfxy.top/gtoqkpzqbv.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hammf.cn/gtjqriiurg.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.52xcode.cn/gtbeefyvbo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.haohaochexian.top/gthnbnanlq.html

[J04] 时间戳与日期互转
来源：http://hz.xuanzx.com/gtadfmsehh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.havefunace.top/gtmhakxmvr.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.52xcode.cn/gtysduvgoa.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.tianlin.xyz/gtbvwtgsrz.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jqgufenzy.top/gtljqjboyw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.havefunace.top/gtilsxkapp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nanxuanxn.top/gtbbfogemm.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.ywan-chungtsiang.top/gthouvmjeh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.bjfxy.top/gtlluzlmay.html

[J05] 时间加减（加 7 天）
来源：http://hz.ppjwa.cn/gtpnajhzmu.html

Py:   now + timedelta(days=7)
来源：http://hz.daxiang520.top/gtvgjulfsj.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.shanyushiyangkeji.top/gtunzjmror.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenzaomai.com/gtucjjcmrn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pengpengdd.cyou/gtnfxqdafc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yangfankeji.com/gtocxkbdbq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.snrcjt.cn/gtixslirfc.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xziqi.cn/gtsckmvmho.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jqgufenzy.top/gtyykaydkh.html

[J06] 计算两时间之差
来源：http://hz.9152youxi.cn/gtrdlbgwcx.html

Py:   (end - start).total_seconds()
来源：http://hz.gotoacloud.top/gtxarmuhvv.html

PHP:  $end->diff($start)->days;
来源：http://hz.yangfankeji.com/gtatbwguxa.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.52xcode.cn/gtqsyagqwj.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinghuilouyu.cn/gtssdetkdx.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yangfankeji.com/gtmzesmqej.html

Go:   end.Sub(start).Hours()
来源：http://hz.iojbl.cn/gtupszxkdg.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yj20258888.top/gtlopztict.html

C#:   (end - start).TotalSeconds
来源：http://hz.hfpthk.cn/gtsevjbqno.html

[J07] 比较两个日期
来源：http://hz.sxryk.cn/gtkbcoklnk.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.jyoumei.cn/gtnnrkdrqg.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hywenlv.cn/gtpjnundpb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shzxlz.cn/gtevgbtawb.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.gogol.net.cn/gtokyyqebw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.aizwys.cn/gttmdfrmws.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hysaishi.cn/gtrxvkkbew.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.chenlongwang.top/gthobyxmvm.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.tanke756.top/gttdmqokfu.html

[J08] 提取年月日与星期
来源：http://hz.yvedp.cn/gthzmowtxg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.snrcjt.cn/gtizzjpnhi.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.chenzaomai.com/gtstsekydz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhixingplan.top/gtncayrcox.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gzhubu.top/gtrcrpkcjb.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ehwqpu.com/gtwdaiqdkw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jqgufenzy.top/gtzlfqjkgk.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.hnxiangtu.top/gtdbeizpbb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.daxiang520.top/gtsdzrzljc.html

[J09] 时区处理
来源：http://hz.hongshengwenyu.top/gtsvsbtnpi.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.meibo888.top/gtcufwujtm.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.sufxvd.cn/gtcsemqkfq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ppjwa.cn/gtaddbydua.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgufenzy.top/gtgdadkmfr.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.hnqzz.top/gtgwnaqqrt.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gotoacloud.top/gtjbxrpooy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xuetiantiany.cn/gtvsutxrkt.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.316326.xyz/gtnppyyurh.html

[J10] 取今天 / 本月第一天
来源：http://hz.ywan-chungtsiang.top/gtiatoibfd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.fzhhl.top/gtkenzyjzm.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jqgufenzy.top/gtijrhtegw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.svipenyu.cn/gtzswnnrpd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.cucudq.cn/gteukpsqmv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.gogol.net.cn/gtppdpyxpf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.nanxuanxn.top/gtydppjczs.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ybcxt.top/gtujxxjbsu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhaomingkeji.xyz/gtgwgpwgyz.html

================================================================================
来源：http://hz.9152youxi.cn/gtgxjabscc.html

K. JSON 与序列化
来源：http://hz.jinqigfzy.top/gtnyuebedn.html

================================================================================
来源：http://hz.haohaochexian.top/gtajepsfgr.html

[K01] 对象转 JSON 字符串
来源：http://hz.xuanzx.com/gtjnomyjfe.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.316326.xyz/gtiuyzxogc.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.haohaochexian.top/gttphowmia.html

JS:   JSON.stringify(obj)
来源：http://hz.dashuyun.cn/gtyobrmjjd.html

TS:   JSON.stringify(obj)
来源：http://hz.hfpthk.cn/gtixjterpz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.zhengqikj.top/gtrldjgkoj.html

Go:   json.Marshal(obj)
来源：http://hz.daria6918.cn/gtfjbxmlhe.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.chenjidiqi.icu/gtlyjydgzz.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.c1oappe.top/gttekyhznb.html

[K02] JSON 字符串转对象
来源：http://hz.quarkkingdee.top/gtdfsvubcg.html

Py:   json.loads(s)
来源：http://hz.52xcode.cn/gtfxjwavio.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.sufxvd.cn/gtaxpphxxm.html

JS:   JSON.parse(s)
来源：http://hz.aibaodan.cn/gtpmwayjie.html

TS:   JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtlbjypdnf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.haohaochexian.top/gtcwxkkbfh.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.redwolf501.top/gtepfsoaha.html

Ruby: JSON.parse(s)
来源：http://hz.zhaomingkeji.xyz/gtvibcwzqq.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yj20258888.top/gthetevdrz.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.yvedp.cn/gtwsjxivjg.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.cucudq.cn/gtecrbvlyx.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.meibo888.top/gtggwpnenb.html


<!-- 参考信息 -->