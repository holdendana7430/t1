代发 wailian999

C#:   record User(string Name, int Age);
来源：http://hz.pycfn.com/gtzawnzjib.html

[G15] 枚举
来源：http://hz.shuidangran.top/gtdyyvszud.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.cheryme.top/gtopxkvcab.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.316326.xyz/gtnqfqvllu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.fengsongda.top/gtsgansgbj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.pengpengdd.cyou/gtrelfdcoj.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhongyouzk.top/gtthznpwpb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cdnleiting.top/gtoqnxfsva.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yvedp.cn/gtwdcamkzl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shangyingyoupin.top/gtrxsxeita.html

[G16] 对象转数组 / 字典
来源：http://hz.wangshuangyany.cn/gtiahqadpi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhongyouzk.top/gtoyuplywg.html

PHP:  get_object_vars($obj);
来源：http://hz.jinqigufen.top/gtidkhlpxc.html

JS:   Object.entries(obj)
来源：http://hz.ehwqpu.com/gtreuoeemm.html

TS:   Object.entries(obj)
来源：http://hz.snrcjt.cn/gtesvabkyr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.xinyue.icu/gtposaapio.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ehwqpu.com/gtbewnijof.html

Ruby: obj.instance_variables
来源：http://hz.hysaishi.cn/gtdoqxyjue.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.c1oappe.top/gtzlrlyhmv.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtpwincsxj.html

H. 异常与错误处理
来源：http://hz.feifeiyinyue.top/gthbnrewir.html

================================================================================
来源：http://hz.jqgufenzy.top/gtvyoluvhb.html

[H01] try / catch 基础
来源：http://hz.xinyue.icu/gttzeqbmls.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.feifeiyinyue.top/gtpoxjpymu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.sxryk.cn/gtxrtqxuli.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.wangdashe.top/gtdpfbblhs.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.kuanghao11.cn/gtijeasxpr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.quarkkingdee.top/gtncetnjiu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.mhx1999.top/gtgqxllzjh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.vqdsnc.cn/gtbuqljdig.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.tianlin.xyz/gtexlolclq.html

[H02] finally / ensure 收尾
来源：http://hz.zycfv.cn/gtznqgwtcl.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.fzhhl.top/gtbspxytng.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gtdnqktddz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtynggcrsw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.wangdashe.top/gtjhbjiwzr.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.kuanghao11.cn/gtdxhxjjas.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinqigfzy.top/gtkkmkhfug.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.chenlongwang.top/gtdbjixzyk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.tian-w.cn/gtbonvsiqo.html

[H03] 主动抛出异常
来源：http://hz.pengpengdd.cyou/gtvfikqtgl.html

Py:   raise ValueError("错误信息")
来源：http://hz.hywenlv.cn/gtakrsknmb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.nwbrower.top/gtcjnbgqch.html

JS:   throw new Error("错误信息");
来源：http://hz.yongpay.top/gtoxtrdiav.html

TS:   throw new Error("错误信息");
来源：http://hz.jinqigfzy.top/gtizwhzkbx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.bjfxy.top/gtczxngtxm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xuanzx.com/gtvjrlleyd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jqgfzy.top/gtnomfanbf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.chenjidiqi.icu/gtgazwlwob.html

[H04] 自定义异常类型
来源：http://hz.chenjidiqi.icu/gtxaqyavzg.html

Py:   class MyError(Exception): pass
来源：http://hz.guannengcc.top/gtxgpuhkgm.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jinqigfzy.top/gtfohyazfp.html

JS:   class MyError extends Error {}
来源：http://hz.aibaodan.cn/gtawsdnfde.html

TS:   class MyError extends Error {}
来源：http://hz.xinyue.icu/gtryodovvj.html

Java: class MyException extends RuntimeException {}
来源：http://hz.c1oappe.top/gtojeyutuw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.zdqjudy.top/gtounahvpm.html

Ruby: class MyError < StandardError; end
来源：http://hz.fengsongda.top/gtrkmdtlso.html

C#:   class MyException : Exception {}
来源：http://hz.cheryme.top/gtfhwncqej.html

[H05] 捕获特定类型
来源：http://hz.svipenyu.cn/gtzfdfzkht.html

Py:   except ValueError as e:
来源：http://hz.havefunace.top/gtajwgtxpd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hammf.cn/gtsizfetit.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cqqwz.cn/gtfyhzsshn.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.iojbl.cn/gtqoxppzmg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.chenjidiqi.icu/gtvhzzplon.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.smart0.xyz/gtzyswiqna.html

Ruby: rescue ArgumentError => e
来源：http://hz.ydjk.org.cn/gtfhalunpd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhengqikj.top/gtrhafbdfv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.sweek.top/gtijdmzufg.html

Py:   value = d.get("k") or default
来源：http://hz.yuanzhike.top/gtzchlkvqh.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jqgfzy.top/gtjjyehgys.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.zhaomingkeji.xyz/gtaakmsuop.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yj202588.top/gtfgomczuw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.vqdsnc.cn/gttehcvmyg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jinqigfzy.top/gtohvncraa.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yj202588.top/gtwlxnrbzh.html

C#:   obj?.A?.B ?? default
来源：http://hz.havefunace.top/gtarfwlbwb.html

[H07] 断言
来源：http://hz.hammf.cn/gtfxztpbjn.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhiwuduotai.top/gtxlaeugii.html

PHP:  assert($x > 0);
来源：http://hz.smart0.xyz/gtnvrfmpeu.html

JS:   console.assert(x > 0);
来源：http://hz.cucudq.cn/gtqdmbiozm.html

TS:   console.assert(x > 0);
来源：http://hz.iojbl.cn/gthxerxzyz.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhongyouzk.top/gtdjkihuru.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cdnleiting.top/gtrqzzzmwv.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.gogol.net.cn/gtdwnrkgie.html

C#:   Debug.Assert(x > 0);
来源：http://hz.iojbl.cn/gtisfxnvmy.html

[H08] 获取错误信息与堆栈
来源：http://hz.ywan-chungtsiang.top/gtnaslqrpf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yuxming.cn/gtignsolqu.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hfpthk.cn/gtpeeigtxv.html

JS:   e.message;  e.stack
来源：http://hz.yongpay.top/gtwlwasxfo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.pycfn.com/gtdqgqtput.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gzhubu.top/gtfzonunau.html

Go:   err.Error()
来源：http://hz.vqdsnc.cn/gtstypabjg.html

Ruby: e.message;  e.backtrace
来源：http://hz.yanxiufei.cn/gtaepiiuzh.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tian-w.cn/gtoynmmvwc.html

[H09] 带错误码的异常
来源：http://hz.yonumen.top/gtqcyyxvqi.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.pycfn.com/gtucvmpcaf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ydzc1.top/gtimoozpmb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.ydjk.org.cn/gtuicdyfmk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.gotoacloud.top/gtyhtvelom.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinyuanbaomall.cn/gtrlsebkox.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yueranfly.top/gtnshyviin.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhiwuduotai.top/gtnzfttnfo.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.chenjidiqi.icu/gtdiogpnty.html

[H10] 资源自动释放
来源：http://hz.birdmap.top/gtohjdpqgn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.havefunace.top/gtyiaujkkj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xingfuxueyuan.xyz/gtdmhtwzxl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ydzc1.top/gtrtcusydh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhoulong.xyz/gtawckiipn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yanxiufei.cn/gtzpbjudwc.html

Go:   defer f.Close()
来源：http://hz.chenjidiqi.icu/gtvaetdkoz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yuxming.cn/gtejsjneba.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.mhx1999.top/gtyonzctai.html

================================================================================
来源：http://hz.andypj.xyz/gtknvypgnt.html

I. 正则表达式
来源：http://hz.sufxvd.cn/gtnsbvxhcv.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtuiyvmvhr.html

[I01] 判断是否匹配
来源：http://hz.shanyushiyangtech.top/gttergbucu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.fengsongda.top/gtqsweoglo.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hammf.cn/gtvqcmlavi.html

JS:   /\d+/.test(s)
来源：http://hz.ywan-chungtsiang.top/gtalrwkipo.html

TS:   /\d+/.test(s)
来源：http://hz.yuxming.cn/gtumuckvjk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhijiandao.cn/gtxdbotmsu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.haohaochexian.top/gtwkkvgxoi.html

Ruby: s.match?(/\d+/)
来源：http://hz.tianlin.xyz/gtugcfkvni.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ivvv.top/gtuagywtkv.html

[I02] 提取所有匹配
来源：http://hz.cashguo.top/gtbeqrnifp.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ywan-chungtsiang.top/gtnzjczlnx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jinghuilouyu.cn/gtodiubqvn.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.shangyingyoupin.top/gtavojlxau.html

TS:   s.match(/\d+/g)
来源：http://hz.tian-w.cn/gtkyttfpuv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ivvv.top/gtftuftivj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jinyuanbaomall.cn/gtjcmtripx.html

Ruby: s.scan(/\d+/)
来源：http://hz.zhijiandao.cn/gtppnvcmku.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.gogol.net.cn/gtkqjxvydb.html

[I03] 提取捕获分组
来源：http://hz.sxryk.cn/gtccqrdlvw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yueranfly.top/gtqttodpbh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ydjk.org.cn/gtqedlufbd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yonumen.top/gtifgcxpru.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xuetiantiany.cn/gtnuqouhyr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhijiandao.cn/gtzwwyhxwk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.tian-w.cn/gtkragyuag.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.sufxvd.cn/gtwcjtoqvk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.dashuyun.cn/gtejxvwrus.html

[I04] 正则替换
来源：http://hz.tian-w.cn/gthwexjjps.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.andypj.xyz/gtzerzskjt.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.cheryme.top/gtchkqlsem.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.xylfe.cn/gthlldubep.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hysaishi.cn/gtiyhtffti.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.aibaodan.cn/gtrdehrzax.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.wangshuangyany.cn/gtvkvgxctq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.ehwqpu.com/gtajtexspi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.shanyushiyangtech.top/gtlcjsnprr.html

[I05] 按正则拆分
来源：http://hz.ppjwa.cn/gthrlhwxbr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.sysykeji.top/gtwvosejwk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.chenjidiqi.icu/gtdkaejuqk.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.feifeiyinyue.top/gteagsvctz.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.quarkkingdee.top/gtfyahfmpo.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ydjk.org.cn/gtzypzyzjx.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yj20258888.top/gtqhvzqjee.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jianghu66.top/gtpeemwunb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xylfe.cn/gtmkhbzudl.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhengqikj.top/gtoqgorhho.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yj20258.top/gtcfpwgngi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.quarkkingdee.top/gtxaykksyq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hysaishi.cn/gteokrexhd.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.9152youxi.cn/gtolrmprdo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tianlin.xyz/gtlraginhb.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jqgfzy.top/gtjdwqsldp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.fzhhl.top/gtaqnlrzta.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gaohongyu789.top/gtpojbknyg.html

[I07] 忽略大小写与多行模式
来源：http://hz.smart0.xyz/gtmjnkzidu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.smart0.xyz/gtrchyscsy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.tianlin.xyz/gtgdzctbbe.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.svipenyu.cn/gtsxmdwnww.html

TS:   /error/gim
来源：http://hz.c1oappe.top/gteeasizaw.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.svipenyu.cn/gtjifkfuqm.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.birdmap.top/gtkdakhwqw.html

Ruby: s.scan(/error/i)
来源：http://hz.hammf.cn/gtlxdoyeih.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yangfankeji.com/gtoctcvnws.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhixingplan.top/gtvpsllvtr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.guowangkeji.top/gtsueqqrge.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shanyushiyangkeji.top/gtessjnrnu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aibaodan.cn/gtooyvmlmw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuanzx.com/gtdgisesdq.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sufxvd.cn/gtvupkhbei.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.zycfv.cn/gtkmxrljao.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.vqdsnc.cn/gtbfuvresz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.tanke756.top/gttlawoggn.html

================================================================================
来源：http://hz.yanxiufei.cn/gttgnogkar.html

J. 日期与时间
来源：http://hz.fengsongda.top/gtnnupabhe.html

================================================================================
来源：http://hz.zhoulong.xyz/gtxnmzriqu.html

[J01] 获取当前时间
来源：http://hz.guowangkeji.top/gtdotvytyn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hnxiangtu.top/gtydomoywn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hnxiangtu.top/gtedcevbeq.html

JS:   new Date();  Date.now()
来源：http://hz.zdqjudy.top/gtnmkhkugk.html

TS:   new Date();  Date.now()
来源：http://hz.birdmap.top/gtrnwgubes.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cheryme.top/gtctpkdftb.html

Go:   time.Now()
来源：http://hz.zhixingplan.top/gtvecfdgkj.html

Ruby: Time.now
来源：http://hz.hongshengwenyu.top/gtrlwoqdrr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hnqzz.top/gtjdpkldsa.html

[J02] 格式化输出
来源：http://hz.dashuyun.cn/gtaktphqha.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.iojbl.cn/gttpkoonfe.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.sweek.top/gtibwpxuht.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gaohongyu789.top/gtuochyogn.html

TS:   d.toISOString()
来源：http://hz.ybcxt.top/gtsqxwngov.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.316326.xyz/gticuxhzou.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tianlin.xyz/gttayklymr.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hammf.cn/gtyetqxycg.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gaohongyu789.top/gtrthpezek.html

[J03] 字符串解析为日期
来源：http://hz.hnqzz.top/gtcgiqlxrg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.316326.xyz/gtwmlmpgal.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cashguo.top/gtdmgznvld.html

JS:   new Date("2024-01-02")
来源：http://hz.meibo888.top/gtocymtako.html

TS:   new Date("2024-01-02")
来源：http://hz.hfpthk.cn/gtigluqqcg.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.tian-w.cn/gtzcvftyvf.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinqigufen.top/gtgodheots.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gzhubu.top/gtqtmqbcjt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhengqikj.top/gthzkjmqms.html

[J04] 时间戳与日期互转
来源：http://hz.jinyuanbaomall.cn/gtkyojdpuz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yuanzhike.top/gtptiqrmti.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.xuetiantiany.cn/gtdwwjjoer.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.birdmap.top/gtnwjvblho.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.dianchejie.cn/gtspgwrrtq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yangfankeji.com/gthpaimbnb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.guowangkeji.top/gteoijsbwr.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hywenlv.cn/gtsdpoioee.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhaomingkeji.xyz/gtqugcxbzw.html

[J05] 时间加减（加 7 天）
来源：http://hz.haohaochexian.top/gtzfyqmwys.html

Py:   now + timedelta(days=7)
来源：http://hz.yanxiufei.cn/gtkmffiswb.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.gogol.net.cn/gtmcozderu.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xuetiantiany.cn/gtlrjzzzcs.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhongyouzk.top/gtuuznfxud.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hongshengwenyu.top/gtojxsjhys.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yj202588.top/gtbkanmgok.html

Ruby: Time.now + 7 * 86400
来源：http://hz.snrcjt.cn/gtjzentiht.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yongpay.top/gtcaqpngls.html

[J06] 计算两时间之差
来源：http://hz.tanke756.top/gtywuqjdhs.html

Py:   (end - start).total_seconds()
来源：http://hz.tanke756.top/gtbdadwunf.html

PHP:  $end->diff($start)->days;
来源：http://hz.hammf.cn/gtuhryaxci.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.meibo888.top/gttdixclyb.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yanxiufei.cn/gttozheims.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.pengpengdd.cyou/gtloqcupmn.html

Go:   end.Sub(start).Hours()
来源：http://hz.andypj.xyz/gtwbnfuoxz.html

Ruby: end - start                 # 返回秒数
来源：http://hz.andypj.xyz/gtxnqrmwep.html

C#:   (end - start).TotalSeconds
来源：http://hz.shanyushiyangtech.top/gtnyhvvrqr.html

[J07] 比较两个日期
来源：http://hz.dashuyun.cn/gtwjkietqq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gtahhexfrr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.vqdsnc.cn/gtfgrkfgfz.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.wangshuangyany.cn/gthqcamnzp.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.bjfxy.top/gttmxvrvaw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.snrcjt.cn/gtivprmbeo.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gzhubu.top/gtcqnrqcdl.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.andypj.xyz/gtocqhssqi.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yongpay.top/gtqsqbbice.html

[J08] 提取年月日与星期
来源：http://hz.jyoumei.cn/gtknpytjuz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.redwolf501.top/gtawjgqrqo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinyuanbaomall.cn/gtddzqalnp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yanxiufei.cn/gttbhdqxyw.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.haohaochexian.top/gtvmyegsen.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cqqwz.cn/gtwsjzbrba.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.aibaodan.cn/gtbeneqvax.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xuanzx.com/gtqufnctgq.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zhixingplan.top/gtqpbapjux.html

[J09] 时区处理
来源：http://hz.cashguo.top/gtgzuvuavo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.smart0.xyz/gtctsbzjma.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.gzhubu.top/gtrxamvama.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.52xcode.cn/gtjlghahnr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258.top/gtvttelvbd.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.aibaodan.cn/gtwwbbzjyo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xuetiantiany.cn/gtbjocwvgv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.xylfe.cn/gtsuxeaqpu.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jiagoushi.top/gtheqhnofh.html

[J10] 取今天 / 本月第一天
来源：http://hz.daxiang520.top/gtuvwvlclc.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cheryme.top/gtbpqfefmj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.c1oappe.top/gtlttoenrr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.smart0.xyz/gtqoyoosta.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.fengsongda.top/gthrskllti.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.tian-w.cn/gtivxzfveb.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yuanzhike.top/gtsjxqykeq.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhijiandao.cn/gtjfldwzfx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinghuilouyu.cn/gttqvmmwqq.html

================================================================================
来源：http://hz.svipenyu.cn/gtpckbjfqw.html

K. JSON 与序列化
来源：http://hz.jinqigfzy.top/gtfcurgfbp.html

================================================================================
来源：http://hz.yj202588.top/gtahgqqwys.html

[K01] 对象转 JSON 字符串
来源：http://hz.zhijiandao.cn/gtbxjbrxzz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shangyingyoupin.top/gtbbgpyozk.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.ivvv.top/gtpebxtotq.html

JS:   JSON.stringify(obj)
来源：http://hz.zhijiandao.cn/gtpofjrwfs.html

TS:   JSON.stringify(obj)
来源：http://hz.chenzaomai.com/gtkgarcbvm.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.dashuyun.cn/gtrsbwunlx.html

Go:   json.Marshal(obj)
来源：http://hz.snrcjt.cn/gttnadcwvx.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jyoumei.cn/gtnpihithh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hfpthk.cn/gtzuocpnxw.html

[K02] JSON 字符串转对象
来源：http://hz.guannengcc.top/gtfvlliesf.html

Py:   json.loads(s)
来源：http://hz.ehwqpu.com/gtwbeaediy.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.meibo888.top/gtuwmkifpf.html

JS:   JSON.parse(s)
来源：http://hz.yj20258888.top/gttirzoufu.html

TS:   JSON.parse(s)
来源：http://hz.dianchejie.cn/gtgrwcoqiy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.cheryme.top/gtjbnuzqyz.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.havefunace.top/gthnotaidq.html

Ruby: JSON.parse(s)
来源：http://hz.shzxlz.cn/gtfflrecki.html


<!-- 参考信息 -->