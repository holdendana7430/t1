代发 wailian999

PHP:  get_object_vars($obj);
来源：http://hz.yj20258888.top/gtvtwzkibu.html

JS:   Object.entries(obj)
来源：http://hz.c1oappe.top/gtcwtaxhbn.html

TS:   Object.entries(obj)
来源：http://hz.sysykeji.top/gtavqhbqdo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jinghuilouyu.cn/gtddyrpxam.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ydzc1.top/gtvzytvpav.html

Ruby: obj.instance_variables
来源：http://hz.havefunace.top/gtzyrjzuhk.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shanyushiyangkeji.top/gtzymjrtso.html

================================================================================
来源：http://hz.yuxming.cn/gteocjpdnf.html

H. 异常与错误处理
来源：http://hz.zdqjudy.top/gtckogirtg.html

================================================================================
来源：http://hz.316326.xyz/gtgvgugscu.html

[H01] try / catch 基础
来源：http://hz.xuanzx.com/gthuxoumzm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhongyouzk.top/gtsbnkkwpk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.redwolf501.top/gtoauaezbc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.bjfxy.top/gtkvcymzsw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ehwqpu.com/gtdyriqaen.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.shanyushiyangkeji.top/gtwmfyjneg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.sufxvd.cn/gthuekhwsd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.redwolf501.top/gtzubvqwah.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.guannengcc.top/gtkqfooron.html

[H02] finally / ensure 收尾
来源：http://hz.nwbrower.top/gtfnggaqfm.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.9152youxi.cn/gtvifutjyl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhengqikj.top/gtlfrpabbz.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.tianlin.xyz/gtodgzmxjq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zycfv.cn/gtknenwskp.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtcgjbycne.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.nwbrower.top/gtdmilqqcq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.birdmap.top/gtulhhaacg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yongpay.top/gtjqjpozhb.html

[H03] 主动抛出异常
来源：http://hz.smart0.xyz/gtadwcympo.html

Py:   raise ValueError("错误信息")
来源：http://hz.shangyingyoupin.top/gtqubifoyj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ydzc1.top/gtmscnrsxo.html

JS:   throw new Error("错误信息");
来源：http://hz.mhx1999.top/gtddmkoeud.html

TS:   throw new Error("错误信息");
来源：http://hz.chenzaomai.com/gtjrvuqzjj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.shanyushiyangtech.top/gtwatowxow.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.aibaodan.cn/gtumemicps.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.guannengcc.top/gteysqngro.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.wangdashe.top/gtnqgsxiao.html

[H04] 自定义异常类型
来源：http://hz.zycfv.cn/gtrbhrcwfi.html

Py:   class MyError(Exception): pass
来源：http://hz.gzhubu.top/gtrjrkofki.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.redwolf501.top/gtcsonxsoc.html

JS:   class MyError extends Error {}
来源：http://hz.dianchejie.cn/gtfeamzitm.html

TS:   class MyError extends Error {}
来源：http://hz.hywenlv.cn/gtwxzleasi.html

Java: class MyException extends RuntimeException {}
来源：http://hz.ywan-chungtsiang.top/gtmbuqerrs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shanyushiyangkeji.top/gtbcvndrag.html

Ruby: class MyError < StandardError; end
来源：http://hz.jqgfzy.top/gteiuxombw.html

C#:   class MyException : Exception {}
来源：http://hz.cashguo.top/gtwseanlmo.html

[H05] 捕获特定类型
来源：http://hz.yueranfly.top/gtozdvdfve.html

Py:   except ValueError as e:
来源：http://hz.hongshengwenyu.top/gtkfywgbcx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.ydzc1.top/gttyeohpto.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.gogol.net.cn/gtgfrikswf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.9152youxi.cn/gtlujtxbmk.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yanxiufei.cn/gtyqvemerf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.sysykeji.top/gtaxawoxqi.html

Ruby: rescue ArgumentError => e
来源：http://hz.gotoacloud.top/gtvqcwcimg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.aizwys.cn/gtfloerbaf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hysaishi.cn/gtigyvyfxk.html

Py:   value = d.get("k") or default
来源：http://hz.jianghu66.top/gtucebtmzw.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gogol.net.cn/gtwsuuzaob.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.pengpengdd.cyou/gtuwccrpts.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jiagoushi.top/gttaiwapmm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.birdmap.top/gtixseemfk.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.ppjwa.cn/gtwyyigaej.html

Ruby: d&.dig(:a, :b)
来源：http://hz.iojbl.cn/gthmpnjhil.html

C#:   obj?.A?.B ?? default
来源：http://hz.xinyue.icu/gthrqaocqb.html

[H07] 断言
来源：http://hz.yonumen.top/gtjyuaedyv.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gogol.net.cn/gtfcczlkby.html

PHP:  assert($x > 0);
来源：http://hz.fengsongda.top/gtyroogoem.html

JS:   console.assert(x > 0);
来源：http://hz.daxiang520.top/gtpuwugxvt.html

TS:   console.assert(x > 0);
来源：http://hz.hongshengwenyu.top/gtypbodpsg.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhengqikj.top/gtjgjaiymx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.havefunace.top/gtfejtceli.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.nanxuanxn.top/gtmlmyllli.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jinyuanbaomall.cn/gtvrwegeuo.html

[H08] 获取错误信息与堆栈
来源：http://hz.pycfn.com/gtvetcvbsh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.bjfxy.top/gtgwazpwsg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cucudq.cn/gtniijwbny.html

JS:   e.message;  e.stack
来源：http://hz.daxiang520.top/gtgebdwlyy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.snrcjt.cn/gtnsjdubbl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.ywan-chungtsiang.top/gtfpbyjjqb.html

Go:   err.Error()
来源：http://hz.0kj1m.cn/gtpjzgqbzn.html

Ruby: e.message;  e.backtrace
来源：http://hz.shanyushiyangkeji.top/gtnumbpqra.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sxryk.cn/gtnzkpftvt.html

[H09] 带错误码的异常
来源：http://hz.wangdashe.top/gtvzymvdct.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.xinyue.icu/gtxtlfmmlx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jiagoushi.top/gtifpqhmko.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.tianlin.xyz/gtrpdokebp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.0kj1m.cn/gtllqpfstj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.vqdsnc.cn/gtwiqsplru.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.haohaochexian.top/gtvjyhyzga.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jianghu66.top/gtjascorpu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yonumen.top/gtnayifnva.html

[H10] 资源自动释放
来源：http://hz.cqqwz.cn/gtvebldphb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ydjk.org.cn/gtonhqnujf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.haohaochexian.top/gtxmxhaccn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.fengsongda.top/gtkugypqfv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yueranfly.top/gtsknkvmno.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.hfpthk.cn/gtruaoukkv.html

Go:   defer f.Close()
来源：http://hz.shuidangran.top/gtlsiodhxm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yvedp.cn/gtecvsgfqu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.kuanghao11.cn/gtqpoufnpp.html

================================================================================
来源：http://hz.9152youxi.cn/gtrbpqdzrz.html

I. 正则表达式
来源：http://hz.xylfe.cn/gtmmhvydhz.html

================================================================================
来源：http://hz.pengpengdd.cyou/gthrkrgfoh.html

[I01] 判断是否匹配
来源：http://hz.yuanzhike.top/gtyvdsuhpx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhoulong.xyz/gtjoohpovk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.feifeiyinyue.top/gtrgfawezl.html

JS:   /\d+/.test(s)
来源：http://hz.shanyushiyangtech.top/gtlfdakpag.html

TS:   /\d+/.test(s)
来源：http://hz.yj202588.top/gtuukcinyq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.0kj1m.cn/gtcusnefpl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.andypj.xyz/gtzkbomnua.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhiwuduotai.top/gtsbcftkda.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.daria6918.cn/gtauelkgtd.html

[I02] 提取所有匹配
来源：http://hz.sufxvd.cn/gthbgzzgie.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinghuilouyu.cn/gtlacoomce.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hywenlv.cn/gtmmkaaoxg.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhoulong.xyz/gtgkliwbfr.html

TS:   s.match(/\d+/g)
来源：http://hz.jqgfzy.top/gtglscjbsi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hysaishi.cn/gtwpqoonfk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ppjwa.cn/gtchhxztqf.html

Ruby: s.scan(/\d+/)
来源：http://hz.daxiang520.top/gtetftzgoe.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ybcxt.top/gtormdwcjc.html

[I03] 提取捕获分组
来源：http://hz.zhixingplan.top/gtupcraqko.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhengqikj.top/gtivuwgzwx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.svipenyu.cn/gthzovqmeh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gzhubu.top/gtmndxiclh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jinghuilouyu.cn/gtnbyejbhv.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.tianlin.xyz/gtsfgzrvcz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shuidangran.top/gtzlcgxcby.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hfpthk.cn/gtpynvrlfd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.feifeiyinyue.top/gttkuddywm.html

[I04] 正则替换
来源：http://hz.jinghuilouyu.cn/gtzslltdoh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.haohaochexian.top/gtqfjpqlme.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.fengsongda.top/gtyzxiyjll.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jyoumei.cn/gtowoblpeq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jyoumei.cn/gtsbdggmgl.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinqigufen.top/gtbvydzmbu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.meibo888.top/gtgzgpfzfc.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.xingfuxueyuan.xyz/gtvznirlgh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jqgfzy.top/gtkqlghnpz.html

[I05] 按正则拆分
来源：http://hz.hfpthk.cn/gtwcqudrci.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.snrcjt.cn/gtccdmrnai.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ywan-chungtsiang.top/gthjwtpxik.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.0kj1m.cn/gtpqxftmpe.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.ydjk.org.cn/gtjkxxfuwu.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shangyingyoupin.top/gtievplmlq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gotoacloud.top/gtyenfyznf.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.nanxuanxn.top/gtgtvhihxl.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.chenzaomai.com/gtreianuiz.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.dashuyun.cn/gtgqpofjpm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.wangdashe.top/gtyfzpjpxv.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ybcxt.top/gttmuaboyw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnqzz.top/gtwyotijnp.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhiwuduotai.top/gtwinfjatf.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.wangdashe.top/gtyjdrfnjo.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yongpay.top/gtypofukcj.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shangyingyoupin.top/gtoyxdcffe.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.nwbrower.top/gthkxbidpp.html

[I07] 忽略大小写与多行模式
来源：http://hz.aibaodan.cn/gtylyrjqgg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.ehwqpu.com/gtzrqetjvj.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.chenjidiqi.icu/gtgkhipxnk.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.feifeiyinyue.top/gteqcbseai.html

TS:   /error/gim
来源：http://hz.xuanzx.com/gthphqfhbf.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.meibo888.top/gtvodtcdfo.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gaohongyu789.top/gthhzcrosa.html

Ruby: s.scan(/error/i)
来源：http://hz.shzxlz.cn/gtqmddkdzx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhiwuduotai.top/gtitunlmgw.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yanxiufei.cn/gtkrsqazjn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.chenzaomai.com/gtyymzzvsd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jqgfzy.top/gtsmypcwpc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yanxiufei.cn/gtimwwbkuc.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.0kj1m.cn/gtqgtnekka.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xingfuxueyuan.xyz/gtvgccqxmw.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jlsjyb.cn/gtusgeqgax.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.daxiang520.top/gtmwuyiqbb.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhaomingkeji.xyz/gtodtzuwdw.html

================================================================================
来源：http://hz.ydjk.org.cn/gthjgmdrmc.html

J. 日期与时间
来源：http://hz.wangshuangyany.cn/gttwxnjltv.html

================================================================================
来源：http://hz.nwbrower.top/gthsmasify.html

[J01] 获取当前时间
来源：http://hz.ppjwa.cn/gttzbwhldk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhijiandao.cn/gtfsaealvm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.nanxuanxn.top/gttwfqcdbq.html

JS:   new Date();  Date.now()
来源：http://hz.daxiang520.top/gtipmfbxnz.html

TS:   new Date();  Date.now()
来源：http://hz.jianghu66.top/gtuzimpdne.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.aizwys.cn/gtzydgiqof.html

Go:   time.Now()
来源：http://hz.fzhhl.top/gtpwjdooey.html

Ruby: Time.now
来源：http://hz.52xcode.cn/gtcwcesxoa.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xingfuxueyuan.xyz/gtlezerqox.html

[J02] 格式化输出
来源：http://hz.xingfuxueyuan.xyz/gtvacjncwo.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhaomingkeji.xyz/gtxgaedklx.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zdqjudy.top/gtbnqrpxyy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hywenlv.cn/gtdvntzfjp.html

TS:   d.toISOString()
来源：http://hz.yueranfly.top/gtqflhaqhh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yangfankeji.com/gtmkbewogp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.shanyushiyangkeji.top/gtnecvutxt.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yonumen.top/gtzkqfnhuz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yuanzhike.top/gtnpicnsyp.html

[J03] 字符串解析为日期
来源：http://hz.dianchejie.cn/gtnnpmoeih.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ppjwa.cn/gtakdzawce.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yj202588.top/gtrtzmzwwc.html

JS:   new Date("2024-01-02")
来源：http://hz.yuanzhike.top/gtcjldwroy.html

TS:   new Date("2024-01-02")
来源：http://hz.daxiang520.top/gtlsflvnob.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.iojbl.cn/gtbcmbypju.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hywenlv.cn/gtvokuakoi.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.316326.xyz/gtojulplna.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.meibo888.top/gtkmdhgkax.html

[J04] 时间戳与日期互转
来源：http://hz.jqgfzy.top/gtsftxmdxe.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jianghu66.top/gtixtuqlmu.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhoulong.xyz/gtvvlvprdn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hfpthk.cn/gtadjkzafn.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhijiandao.cn/gtbluykkeb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.tianlin.xyz/gtlfmhjoga.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yvedp.cn/gtnckmpcwi.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yj20258888.top/gtbvhnldnm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hfpthk.cn/gtdqvzmpej.html

[J05] 时间加减（加 7 天）
来源：http://hz.hammf.cn/gtwclktddr.html

Py:   now + timedelta(days=7)
来源：http://hz.zdqjudy.top/gtutarfpha.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.havefunace.top/gtzvpvxsqp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.0kj1m.cn/gtqdkuapdf.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cdnleiting.top/gtckiwjnsg.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinqigfzy.top/gtkkbaqlee.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jlsjyb.cn/gtvfcgndyv.html

Ruby: Time.now + 7 * 86400
来源：http://hz.dashuyun.cn/gtuhxbtvuu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hammf.cn/gtagagynjp.html

[J06] 计算两时间之差
来源：http://hz.sweek.top/gtchudcojv.html

Py:   (end - start).total_seconds()
来源：http://hz.jyoumei.cn/gthnqtfxna.html

PHP:  $end->diff($start)->days;
来源：http://hz.daria6918.cn/gtegudkjcg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.shzxlz.cn/gteowadvlh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhiwuduotai.top/gtqnivxlje.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yj202588.top/gtkgalkucb.html

Go:   end.Sub(start).Hours()
来源：http://hz.smart0.xyz/gtgzjafsmr.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sufxvd.cn/gtfzvnvfbl.html

C#:   (end - start).TotalSeconds
来源：http://hz.chenjidiqi.icu/gtvldpkurb.html

[J07] 比较两个日期
来源：http://hz.xuanzx.com/gtnqfvpamo.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhaomingkeji.xyz/gttkpagwqp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.pengpengdd.cyou/gtkbyvojdj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.iojbl.cn/gtwmszsdkg.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.tanke756.top/gtsuqqjoxz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zycfv.cn/gtscnemflg.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sweek.top/gtzzjqafzi.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.shangyingyoupin.top/gteibxliya.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gotoacloud.top/gtkwuikzcd.html

[J08] 提取年月日与星期
来源：http://hz.sufxvd.cn/gtkpuhgjdk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.dashuyun.cn/gtcrhhwekl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xinyue.icu/gtagbzugfl.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.52xcode.cn/gtxbirfmly.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yangfankeji.com/gtodfcjcsk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hnqzz.top/gttdqwarlt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jiagoushi.top/gtfsldwdmb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jyoumei.cn/gtdqfjutmm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xuanzx.com/gtnbnhoniy.html

[J09] 时区处理
来源：http://hz.dashuyun.cn/gtckjzhhdw.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.haohaochexian.top/gtdojxwkdv.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.aibaodan.cn/gtcssbcdxy.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cucudq.cn/gtxdoefofo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dashuyun.cn/gtjnlhiofa.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhijiandao.cn/gtjjlzvldf.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cashguo.top/gtbdiylkdm.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ehwqpu.com/gtnzzfmuzs.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.iojbl.cn/gtcdbmewdz.html

[J10] 取今天 / 本月第一天
来源：http://hz.feifeiyinyue.top/gtmygvastd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jqgfzy.top/gtpnusztqf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.daria6918.cn/gtqiaswujc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.shanyushiyangtech.top/gtxnbidumv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.shuidangran.top/gtsbwdbpor.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.cdnleiting.top/gtvbzzgkln.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.iojbl.cn/gtxdvlbdiu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhixingplan.top/gthkzamlji.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.daria6918.cn/gthwbagpjx.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtwmcllmuq.html

K. JSON 与序列化
来源：http://hz.zhoulong.xyz/gthcjfkrpe.html

================================================================================
来源：http://hz.hammf.cn/gtqzwetvuk.html

[K01] 对象转 JSON 字符串
来源：http://hz.ehwqpu.com/gtcbupnare.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ehwqpu.com/gtjoqjizey.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.nanxuanxn.top/gthapmzpxx.html

JS:   JSON.stringify(obj)
来源：http://hz.zhoulong.xyz/gtuvksbxak.html

TS:   JSON.stringify(obj)
来源：http://hz.daria6918.cn/gtwowjqvae.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.haohaochexian.top/gtlqpxosub.html

Go:   json.Marshal(obj)
来源：http://hz.jinghuilouyu.cn/gtybbhrwba.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.daria6918.cn/gtmhdbxaly.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.xylfe.cn/gtzxbiukkp.html

[K02] JSON 字符串转对象
来源：http://hz.smart0.xyz/gtgdfupime.html

Py:   json.loads(s)
来源：http://hz.zycfv.cn/gtvnbeaper.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.xuanzx.com/gtpybrtdcw.html

JS:   JSON.parse(s)
来源：http://hz.wangshuangyany.cn/gtgfuarhea.html

TS:   JSON.parse(s)
来源：http://hz.yj202588.top/gtvmkesxqv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yj20258888.top/gttauqzuhp.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.52xcode.cn/gtjnqpdhvx.html

Ruby: JSON.parse(s)
来源：http://hz.jinyuanbaomall.cn/gtzahjjbzo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.redwolf501.top/gtaspxprha.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.gzhubu.top/gtziynndpw.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.hongshengwenyu.top/gtgxfylztn.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.andypj.xyz/gtsprbmvfk.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnxiangtu.top/gtoaeynwuy.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.havefunace.top/gtsszwlfan.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.xingfuxueyuan.xyz/gtwdjgnxds.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.aibaodan.cn/gtbsvkfvaf.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ydzc1.top/gtdvrlhlse.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.zhixingplan.top/gticnitnbd.html

[K04] 读取 JSON 文件
来源：http://hz.ppjwa.cn/gtoqiahffd.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.yongpay.top/gtpqaypbam.html


<!-- 参考信息 -->