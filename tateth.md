代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://hz.hysaishi.cn/gtthgeenfo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.tianlin.xyz/gtwnviqoak.html

[G16] 对象转数组 / 字典
来源：http://hz.svipenyu.cn/gtjssethei.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yanxiufei.cn/gtgrwvyvby.html

PHP:  get_object_vars($obj);
来源：http://hz.quarkkingdee.top/gtboljawqk.html

JS:   Object.entries(obj)
来源：http://hz.fzhhl.top/gtsvghnjvp.html

TS:   Object.entries(obj)
来源：http://hz.gzhubu.top/gtobdvddsn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.mhx1999.top/gttefpbola.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yueranfly.top/gtdnodexgs.html

Ruby: obj.instance_variables
来源：http://hz.cashguo.top/gthokbtdsb.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yanxiufei.cn/gtcolldqck.html

================================================================================
来源：http://hz.yj20258.top/gteeainpzx.html

H. 异常与错误处理
来源：http://hz.pycfn.com/gteiinmvht.html

================================================================================
来源：http://hz.dashuyun.cn/gtimuqgaqf.html

[H01] try / catch 基础
来源：http://hz.gaohongyu789.top/gtcyudfvgs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ywan-chungtsiang.top/gtkcxjphbd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ydzc1.top/gtslkbhtix.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yuanzhike.top/gtadxvlqfb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yuxming.cn/gtnkrnprpu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhongyouzk.top/gtryecztig.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.nwbrower.top/gtpdlpmlvp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.nanxinkj.top/gtzpgnqypd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hnxiangtu.top/gtioesswjf.html

[H02] finally / ensure 收尾
来源：http://hz.gotoacloud.top/gtftebyxfo.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xuetiantiany.cn/gtfnnbibyq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtfswbzkqa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gtuomeblio.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ehwqpu.com/gtmalessoe.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shzxlz.cn/gtxvdkrfkh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.tian-w.cn/gtrurehong.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jqgufenzy.top/gtjakvkcgb.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.andypj.xyz/gtxxqerciq.html

[H03] 主动抛出异常
来源：http://hz.jyoumei.cn/gtripikecd.html

Py:   raise ValueError("错误信息")
来源：http://hz.nwbrower.top/gtgnmiiprf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.tianlin.xyz/gtqebfowqq.html

JS:   throw new Error("错误信息");
来源：http://hz.xziqi.cn/gtijpsuztj.html

TS:   throw new Error("错误信息");
来源：http://hz.wangshuangyany.cn/gtwdfvzkse.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.316326.xyz/gtxkjnddad.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.kuanghao11.cn/gtbjmkkbgg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jinghuilouyu.cn/gtqyeqxvqg.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.svipenyu.cn/gtdussidrv.html

[H04] 自定义异常类型
来源：http://hz.daxiang520.top/gtkungpgyn.html

Py:   class MyError(Exception): pass
来源：http://hz.sweek.top/gtpycesyjl.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhijiandao.cn/gtdygdpzwl.html

JS:   class MyError extends Error {}
来源：http://hz.smart0.xyz/gtrbnuhmux.html

TS:   class MyError extends Error {}
来源：http://hz.mhx1999.top/gtwooiaijz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.havefunace.top/gtlhmrvhuu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yueranfly.top/gtchvfmmui.html

Ruby: class MyError < StandardError; end
来源：http://hz.0kj1m.cn/gthqjlmqtj.html

C#:   class MyException : Exception {}
来源：http://hz.jianghu66.top/gtzflegcvq.html

[H05] 捕获特定类型
来源：http://hz.sysykeji.top/gtefdfepvz.html

Py:   except ValueError as e:
来源：http://hz.feifeiyinyue.top/gtobtrdduv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jlsjyb.cn/gtwqkputmg.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhixingplan.top/gttxebwnds.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.redwolf501.top/gttxamlfef.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.nwbrower.top/gtvbineblo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhiwuduotai.top/gtizqubxsf.html

Ruby: rescue ArgumentError => e
来源：http://hz.jqgfzy.top/gtogdzltok.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.shuidangran.top/gtlyrwwihj.html

[H06] 可选值 / 空值安全访问
来源：http://hz.xziqi.cn/gtitfyqpoz.html

Py:   value = d.get("k") or default
来源：http://hz.cucudq.cn/gtvfsloeyd.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.aibaodan.cn/gteqrtflfq.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xuanzx.com/gtrovzfyli.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shzxlz.cn/gtnfqgzdim.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.tianlin.xyz/gtreceitkx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.gogol.net.cn/gtthkyfoyj.html

Ruby: d&.dig(:a, :b)
来源：http://hz.meibo888.top/gtxogncbmg.html

C#:   obj?.A?.B ?? default
来源：http://hz.mhx1999.top/gtgwxchlkr.html

[H07] 断言
来源：http://hz.yuxming.cn/gtpumnvtay.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hywenlv.cn/gthqiooqew.html

PHP:  assert($x > 0);
来源：http://hz.yongpay.top/gtqszpgnwt.html

JS:   console.assert(x > 0);
来源：http://hz.sysykeji.top/gtzgxkdzbn.html

TS:   console.assert(x > 0);
来源：http://hz.bjfxy.top/gtbbeybqdk.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ywan-chungtsiang.top/gtshvbgruo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.feifeiyinyue.top/gttnmsttim.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hnxiangtu.top/gtwadeoojt.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cdnleiting.top/gtexitiigm.html

[H08] 获取错误信息与堆栈
来源：http://hz.fzhhl.top/gtrlcyifaq.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinqigufen.top/gtvkgjuinq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yvedp.cn/gtyqeyrrux.html

JS:   e.message;  e.stack
来源：http://hz.jlsjyb.cn/gtwbddhirc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xylfe.cn/gtfdykduph.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gotoacloud.top/gtravcrbde.html

Go:   err.Error()
来源：http://hz.chenjidiqi.icu/gtgpdzoitn.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinqigufen.top/gtdeqokmue.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhaomingkeji.xyz/gtgcwfevpq.html

[H09] 带错误码的异常
来源：http://hz.xingfuxueyuan.xyz/gtrjaexrwt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.wangshuangyany.cn/gtzhdkiurn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.bjfxy.top/gteafajnlh.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.birdmap.top/gtqpppovod.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zycfv.cn/gtpjpearoa.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhengqikj.top/gtkwmkfgec.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.dashuyun.cn/gtzyynqdoo.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yvedp.cn/gtuoshepoj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shanyushiyangkeji.top/gtkmzbtqiy.html

[H10] 资源自动释放
来源：http://hz.feifeiyinyue.top/gtlyaoxhes.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shanyushiyangkeji.top/gtawttdihx.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yongpay.top/gtmzkyyqux.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dianchejie.cn/gtchrkdpcf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xziqi.cn/gtszzwngcm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jqgfzy.top/gtabrcsoni.html

Go:   defer f.Close()
来源：http://hz.cqqwz.cn/gtthchfkbr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cheryme.top/gtegjyljhs.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ppjwa.cn/gtvqqiicgm.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtyratekbj.html

I. 正则表达式
来源：http://hz.yonumen.top/gtmimekzcr.html

================================================================================
来源：http://hz.daria6918.cn/gtewlhkigd.html

[I01] 判断是否匹配
来源：http://hz.cqqwz.cn/gtsxoeaovh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yvedp.cn/gtsqkspzbr.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yangfankeji.com/gtwpjlvhlx.html

JS:   /\d+/.test(s)
来源：http://hz.jqgfzy.top/gtxjspnsan.html

TS:   /\d+/.test(s)
来源：http://hz.zhengqikj.top/gtmbtakqsd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.kuanghao11.cn/gtjwszaadd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.aibaodan.cn/gtsoommbqy.html

Ruby: s.match?(/\d+/)
来源：http://hz.pengpengdd.cyou/gthuhjzqip.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.havefunace.top/gtglayqfpr.html

[I02] 提取所有匹配
来源：http://hz.hammf.cn/gtfpnxpyff.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hnqzz.top/gtpthkzupi.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.cheryme.top/gtjiurpyzi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jinghuilouyu.cn/gtencjxvos.html

TS:   s.match(/\d+/g)
来源：http://hz.fzhhl.top/gttcdfomso.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.andypj.xyz/gtwwgoyubu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jianghu66.top/gtjidwfcoi.html

Ruby: s.scan(/\d+/)
来源：http://hz.svipenyu.cn/gthhxylroc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ydzc1.top/gtnutplikd.html

[I03] 提取捕获分组
来源：http://hz.zycfv.cn/gtsfippqbh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.hnqzz.top/gtnlzsxcop.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ppjwa.cn/gtbzzmrchc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.feifeiyinyue.top/gtsqxpjdwv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yanxiufei.cn/gtjdbbiytb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jqgufenzy.top/gtdslcoiio.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.0kj1m.cn/gtuoeweswo.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shanyushiyangkeji.top/gtcxihtjne.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hfpthk.cn/gtkizbgveg.html

[I04] 正则替换
来源：http://hz.xziqi.cn/gtzmuxytsb.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.sxryk.cn/gtoqojdpnk.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.nanxinkj.top/gtsjwlsnni.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yangfankeji.com/gtdbaprnmo.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.shangyingyoupin.top/gtuggzhkbm.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.sysykeji.top/gtvjijtyev.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xylfe.cn/gtlhbqlohy.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yj20258.top/gtqkugljod.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xuanzx.com/gtzoyeghxz.html

[I05] 按正则拆分
来源：http://hz.dianchejie.cn/gtxnkggxqh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.0kj1m.cn/gtwcfqtsib.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ydzc1.top/gtgmlianzo.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zdqjudy.top/gtdhpjlrgs.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangkeji.top/gtbnjtlyky.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jlsjyb.cn/gtfjeblxax.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.aizwys.cn/gtxqnwjhcm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhixingplan.top/gtqygxbyvv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hysaishi.cn/gtwlycnyjz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.vqdsnc.cn/gtripnoadr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yj20258888.top/gtbzypymen.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.hysaishi.cn/gtrbmrhgos.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ehwqpu.com/gtcfbxifol.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ehwqpu.com/gturzgxubj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tian-w.cn/gtmrwvhqif.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.birdmap.top/gthffuamvl.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jinqigfzy.top/gtlikwzkfu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yvedp.cn/gtfrwgwlhw.html

[I07] 忽略大小写与多行模式
来源：http://hz.shzxlz.cn/gtdytpggye.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.0kj1m.cn/gtymhjpzyw.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhengqikj.top/gtdaypkoxj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.chenjidiqi.icu/gtvvpwnqou.html

TS:   /error/gim
来源：http://hz.ybcxt.top/gteiwsaxpv.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.sufxvd.cn/gthzbdevls.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yangfankeji.com/gtlomxtftd.html

Ruby: s.scan(/error/i)
来源：http://hz.zhaomingkeji.xyz/gthpuzxyqi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.meibo888.top/gtyecgpiui.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.smart0.xyz/gtwogrsruk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.sufxvd.cn/gtwyncxxeg.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yongpay.top/gtcqvimmxw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.52xcode.cn/gtiyrbzbok.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.316326.xyz/gtskimjivo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.gogol.net.cn/gtodlvirmd.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yvedp.cn/gtyaxmaqpv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xinyue.icu/gtyqdqxcxy.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.aizwys.cn/gtwzlprldu.html

================================================================================
来源：http://hz.52xcode.cn/gtnuegggfy.html

J. 日期与时间
来源：http://hz.snrcjt.cn/gtxaunoilc.html

================================================================================
来源：http://hz.sysykeji.top/gtxxcwllby.html

[J01] 获取当前时间
来源：http://hz.hysaishi.cn/gtcjnijguz.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hywenlv.cn/gtbqbkkpxr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jinqigfzy.top/gtddaoupta.html

JS:   new Date();  Date.now()
来源：http://hz.smart0.xyz/gtlfidmmza.html

TS:   new Date();  Date.now()
来源：http://hz.sxryk.cn/gthdgtszyk.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ydjk.org.cn/gtctsmjrcm.html

Go:   time.Now()
来源：http://hz.gzhubu.top/gtqeujzbgq.html

Ruby: Time.now
来源：http://hz.dianchejie.cn/gtrinhyqqx.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhixingplan.top/gtlihambcc.html

[J02] 格式化输出
来源：http://hz.xingfuxueyuan.xyz/gtnqylsyyv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ybcxt.top/gtwmbfnjau.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.bjfxy.top/gtqhcozsse.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ydzc1.top/gtrhqjxgrv.html

TS:   d.toISOString()
来源：http://hz.bjfxy.top/gtlsynrnlc.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.shanyushiyangkeji.top/gtacxglfei.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.birdmap.top/gtindbxmad.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sxryk.cn/gtoyqypmpj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yvedp.cn/gtuqftevrp.html

[J03] 字符串解析为日期
来源：http://hz.nwbrower.top/gtijazxjti.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.redwolf501.top/gtaewgowzy.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.ywan-chungtsiang.top/gtwrsfkhsq.html

JS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtoqtljuye.html

TS:   new Date("2024-01-02")
来源：http://hz.52xcode.cn/gtmhlrrzhn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.vqdsnc.cn/gtopcifmur.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.aibaodan.cn/gttkmtbiil.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtodgiunvc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.tianlin.xyz/gtjtufndoq.html

[J04] 时间戳与日期互转
来源：http://hz.yonumen.top/gtpkgmbnqh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.smart0.xyz/gtokdnmpfe.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ivvv.top/gtjhsjkdss.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.daxiang520.top/gtzahambcw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hammf.cn/gtevyduhsu.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.gaohongyu789.top/gtumbmguok.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nanxuanxn.top/gttacbaszt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zycfv.cn/gtuyzsanqj.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.kuanghao11.cn/gtusgbuzck.html

[J05] 时间加减（加 7 天）
来源：http://hz.sweek.top/gtskogxaiq.html

Py:   now + timedelta(days=7)
来源：http://hz.cheryme.top/gtjturxtqn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ehwqpu.com/gtxqqwkwgn.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.quarkkingdee.top/gtriycwdur.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.316326.xyz/gtlkntjzsr.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shzxlz.cn/gtlcvnwqah.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hnxiangtu.top/gtyzwfhitp.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jinqigufen.top/gtcqgwiegf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cheryme.top/gtfwtleyzr.html

[J06] 计算两时间之差
来源：http://hz.guannengcc.top/gthjqfjsvu.html

Py:   (end - start).total_seconds()
来源：http://hz.cqqwz.cn/gtscptszze.html

PHP:  $end->diff($start)->days;
来源：http://hz.vqdsnc.cn/gtlqjbhtjm.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xziqi.cn/gtxbifpnaf.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yanxiufei.cn/gthuvrbvhk.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.snrcjt.cn/gtbdemsjis.html

Go:   end.Sub(start).Hours()
来源：http://hz.cqqwz.cn/gtcsxdwcag.html

Ruby: end - start                 # 返回秒数
来源：http://hz.tanke756.top/gtpurhobby.html

C#:   (end - start).TotalSeconds
来源：http://hz.tianlin.xyz/gtkbrmrezt.html

[J07] 比较两个日期
来源：http://hz.yvedp.cn/gtayptotjp.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.wangdashe.top/gtfzdmaybc.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yuxming.cn/gtnqbvywsw.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yvedp.cn/gtmoxnjikd.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ydjk.org.cn/gtamilkvfm.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hnqzz.top/gtnqhxkeoc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.c1oappe.top/gtxekjybmu.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hysaishi.cn/gtjroebtqk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.tanke756.top/gtfoxldycy.html

[J08] 提取年月日与星期
来源：http://hz.yonumen.top/gttafndbne.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jqgufenzy.top/gtbqwcwkoc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhengqikj.top/gtrcubqega.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xziqi.cn/gtdmwoexvp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yongpay.top/gtevkxrhdg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jianghu66.top/gtagcknzpq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.feifeiyinyue.top/gtomzacfgw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xuetiantiany.cn/gtyoildrzo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.vqdsnc.cn/gtwnzvklya.html

[J09] 时区处理
来源：http://hz.redwolf501.top/gtolutqity.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.chenlongwang.top/gtuszmroqg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yuanzhike.top/gtfdsiwznq.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ehwqpu.com/gtqkcjiovp.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ywan-chungtsiang.top/gtpdjpbwge.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.fzhhl.top/gtcgxkwqet.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.shangyingyoupin.top/gtbopbwtgy.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.havefunace.top/gtidefesrm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.guowangkeji.top/gtqumcolma.html

[J10] 取今天 / 本月第一天
来源：http://hz.guowangkeji.top/gtixzyfzxv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.vqdsnc.cn/gtutggpnft.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.gaohongyu789.top/gtqzjropns.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jinqigufen.top/gtkmuwpakg.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.c1oappe.top/gtgesezhqj.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sweek.top/gtaiduyfzg.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.nanxinkj.top/gtmmfyybnh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ppjwa.cn/gtwjsxutlb.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.wangshuangyany.cn/gtyvnoolrv.html

================================================================================
来源：http://hz.yongpay.top/gtsiuzkxuv.html

K. JSON 与序列化
来源：http://hz.ivvv.top/gtkpmewhpq.html

================================================================================
来源：http://hz.yangfankeji.com/gtqkaokvqj.html

[K01] 对象转 JSON 字符串
来源：http://hz.jqgfzy.top/gtwuzekwao.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.chenzaomai.com/gttcazyqil.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.kuanghao11.cn/gtggsmnoel.html

JS:   JSON.stringify(obj)
来源：http://hz.hnxiangtu.top/gtfqvkmwxw.html

TS:   JSON.stringify(obj)
来源：http://hz.hywenlv.cn/gtpxjladkh.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.gogol.net.cn/gtrcjqjezw.html

Go:   json.Marshal(obj)
来源：http://hz.ybcxt.top/gtxkqeerra.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.smart0.xyz/gtxdmtevwr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.daria6918.cn/gtdtfvalvo.html

[K02] JSON 字符串转对象
来源：http://hz.ywan-chungtsiang.top/gtevtelgpv.html

Py:   json.loads(s)
来源：http://hz.daxiang520.top/gtiseqqnxs.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.cucudq.cn/gtppgdohuj.html

JS:   JSON.parse(s)
来源：http://hz.yvedp.cn/gtzdvrzxly.html

TS:   JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtdcpjczdr.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zhijiandao.cn/gtpzmiuzso.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.tanke756.top/gtwjavintl.html

Ruby: JSON.parse(s)
来源：http://hz.pycfn.com/gtkbjbomoc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.aizwys.cn/gtdwswnxak.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.mhx1999.top/gtsnfxvett.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.shzxlz.cn/gtvmbhekaw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.havefunace.top/gtqthzekzt.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.jyoumei.cn/gtncysdtpg.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.yuanzhike.top/gtvvkgtjxm.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.wangdashe.top/gtztdluvmq.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.pycfn.com/gtigrpgbpu.html


<!-- 参考信息 -->