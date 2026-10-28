代发 wailian999

H. 异常与错误处理
来源：http://hz.zhijiandao.cn/gtalntacfs.html

================================================================================
来源：http://hz.gzhubu.top/gtrxirqcec.html

[H01] try / catch 基础
来源：http://hz.pycfn.com/gtxmugatjj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.birdmap.top/gtozdrjcfx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.316326.xyz/gtocvbfvgg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.aizwys.cn/gtlifuzmqp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xuanzx.com/gtiaixhdbu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cheryme.top/gtufcgvitc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.52xcode.cn/gtknphulot.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.aizwys.cn/gtlhrekohr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.0kj1m.cn/gtmqbxzqnb.html

[H02] finally / ensure 收尾
来源：http://hz.ywan-chungtsiang.top/gtfxzswwmt.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.havefunace.top/gtprvswxvh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gtewubzden.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtiaiiljzl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sufxvd.cn/gtmmpiprww.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gtallfpkip.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jyoumei.cn/gtucdmqwab.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hammf.cn/gtzscqecqh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhiwuduotai.top/gthzavzaas.html

[H03] 主动抛出异常
来源：http://hz.hnqzz.top/gtqfcxydut.html

Py:   raise ValueError("错误信息")
来源：http://hz.shanyushiyangtech.top/gtkzqufetm.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.0kj1m.cn/gtzwcnrdzd.html

JS:   throw new Error("错误信息");
来源：http://hz.daria6918.cn/gtuvuxapee.html

TS:   throw new Error("错误信息");
来源：http://hz.dianchejie.cn/gtmwfehwxy.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.iojbl.cn/gttnvfhpns.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinghuilouyu.cn/gtztkfuolb.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.snrcjt.cn/gtjbogjqos.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ydzc1.top/gtdzxlyzhs.html

[H04] 自定义异常类型
来源：http://hz.sweek.top/gtimrapirf.html

Py:   class MyError(Exception): pass
来源：http://hz.chenlongwang.top/gtwsylthja.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hammf.cn/gtyqrthobk.html

JS:   class MyError extends Error {}
来源：http://hz.havefunace.top/gtmyhxkuoc.html

TS:   class MyError extends Error {}
来源：http://hz.xylfe.cn/gtjlbuuadq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.c1oappe.top/gtqqizqrfg.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jiagoushi.top/gtoqrpcysh.html

Ruby: class MyError < StandardError; end
来源：http://hz.smart0.xyz/gtrcvfwuoj.html

C#:   class MyException : Exception {}
来源：http://hz.mhx1999.top/gtlschfwzb.html

[H05] 捕获特定类型
来源：http://hz.gotoacloud.top/gtthbeigwg.html

Py:   except ValueError as e:
来源：http://hz.zhaomingkeji.xyz/gtflvpzllc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jiagoushi.top/gtdliahskr.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.vqdsnc.cn/gtqsiccwww.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cucudq.cn/gtlsbchkiz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.bjfxy.top/gtnnebncdn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hammf.cn/gtyfvlhqns.html

Ruby: rescue ArgumentError => e
来源：http://hz.aibaodan.cn/gtylkvzabp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.bjfxy.top/gttebgganj.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yangfankeji.com/gtltxjxpeq.html

Py:   value = d.get("k") or default
来源：http://hz.smart0.xyz/gtgzyaawlj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xuanzx.com/gtzfnkpuml.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yvedp.cn/gtaahinvay.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ydzc1.top/gtqdbuxllb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ywan-chungtsiang.top/gtzmtmvcss.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jqgfzy.top/gthhxpodea.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhixingplan.top/gteiqoituj.html

C#:   obj?.A?.B ?? default
来源：http://hz.snrcjt.cn/gtmayrftui.html

[H07] 断言
来源：http://hz.gzhubu.top/gtphytbvsx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.fzhhl.top/gtrfgjubnp.html

PHP:  assert($x > 0);
来源：http://hz.smart0.xyz/gtpohwlvru.html

JS:   console.assert(x > 0);
来源：http://hz.yj20258888.top/gtotxzbeiu.html

TS:   console.assert(x > 0);
来源：http://hz.jiagoushi.top/gtdqokowfm.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xuanzx.com/gttkhilqvx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jqgufenzy.top/gtywoamtds.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sxryk.cn/gtweeofnlu.html

C#:   Debug.Assert(x > 0);
来源：http://hz.birdmap.top/gtvogkpbqv.html

[H08] 获取错误信息与堆栈
来源：http://hz.pycfn.com/gtunjcdihz.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jiagoushi.top/gtsufbvrdf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.ivvv.top/gtekjnrmvk.html

JS:   e.message;  e.stack
来源：http://hz.shanyushiyangtech.top/gtelmdmdzy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinqigufen.top/gtefwzeoqb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xingfuxueyuan.xyz/gtasgyqvzb.html

Go:   err.Error()
来源：http://hz.yongpay.top/gtgouqvcmq.html

Ruby: e.message;  e.backtrace
来源：http://hz.daxiang520.top/gtsabnvoad.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yj20258888.top/gtwthxtbmz.html

[H09] 带错误码的异常
来源：http://hz.shangyingyoupin.top/gttlxhionw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.feifeiyinyue.top/gtwxnkqbwe.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.daxiang520.top/gtkmeihgic.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shanyushiyangkeji.top/gtoxipluap.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.hysaishi.cn/gtrukpxmcl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jyoumei.cn/gtscebkzoa.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ywan-chungtsiang.top/gtgdwgbrmw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.vqdsnc.cn/gtizvuhgwc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jianghu66.top/gtbdzwfmlm.html

[H10] 资源自动释放
来源：http://hz.bjfxy.top/gtkubcjgwm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.dianchejie.cn/gtwtvznujg.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xylfe.cn/gtapziopzi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yanxiufei.cn/gtwfcfidnv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sysykeji.top/gtzfzrtgvv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.bjfxy.top/gtvurknqxd.html

Go:   defer f.Close()
来源：http://hz.zycfv.cn/gtiwovqzwb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jqgfzy.top/gtiyzgjddb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hongshengwenyu.top/gttjtuqyzr.html

================================================================================
来源：http://hz.yuxming.cn/gtcrmarpxq.html

I. 正则表达式
来源：http://hz.xziqi.cn/gtytnkopmo.html

================================================================================
来源：http://hz.zhixingplan.top/gtwcgjevaj.html

[I01] 判断是否匹配
来源：http://hz.hnxiangtu.top/gtjdliwujr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hammf.cn/gtbdjeoxiw.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.bjfxy.top/gtkquelegm.html

JS:   /\d+/.test(s)
来源：http://hz.aibaodan.cn/gtpezwfrvu.html

TS:   /\d+/.test(s)
来源：http://hz.birdmap.top/gtcriiskpt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.iojbl.cn/gtvrrhixmc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hammf.cn/gtqpwulxkx.html

Ruby: s.match?(/\d+/)
来源：http://hz.guannengcc.top/gtqjhbwkyo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ehwqpu.com/gtyibxrwwl.html

[I02] 提取所有匹配
来源：http://hz.cucudq.cn/gtnnspkbyc.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hammf.cn/gtofhgstys.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hongshengwenyu.top/gtgxaezjdy.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.iojbl.cn/gtulpbobik.html

TS:   s.match(/\d+/g)
来源：http://hz.hammf.cn/gtjgtrqcuc.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinqigufen.top/gtyqtvzzzc.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.sweek.top/gtlgrxpjvi.html

Ruby: s.scan(/\d+/)
来源：http://hz.yvedp.cn/gtxnxrcbzd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cheryme.top/gtlbdyeuxk.html

[I03] 提取捕获分组
来源：http://hz.wangshuangyany.cn/gtcvqlbvcd.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.dashuyun.cn/gtqciluhvg.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.dashuyun.cn/gtxoatiaex.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yonumen.top/gtminzvzvn.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.gogol.net.cn/gtotnaiitc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.fengsongda.top/gtdzfforen.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cheryme.top/gtizxgbjuy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.pengpengdd.cyou/gtipkyigxf.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.mhx1999.top/gtdtqafnud.html

[I04] 正则替换
来源：http://hz.kuanghao11.cn/gtlbyteltd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.daria6918.cn/gtdclbgjwi.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yuanzhike.top/gtjppqxemb.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gogol.net.cn/gtatqygyxm.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gaohongyu789.top/gtobxnjanq.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jiagoushi.top/gtieyocbsk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.havefunace.top/gtfsofuecd.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.sufxvd.cn/gtdsfsggjl.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nanxinkj.top/gttingqrdv.html

[I05] 按正则拆分
来源：http://hz.jinyuanbaomall.cn/gtrjglreqi.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xylfe.cn/gtcddixqph.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zdqjudy.top/gtpkxlacyc.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hnxiangtu.top/gtwsowrxvi.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.chenzaomai.com/gtqqspulta.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xuetiantiany.cn/gtzilrsroo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.guannengcc.top/gtbgwrkbgs.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yanxiufei.cn/gtcqgkqmos.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hammf.cn/gtusspomhv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yonumen.top/gtwfhypsce.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.nwbrower.top/gttvuipkmp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ivvv.top/gtkafshlcg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.svipenyu.cn/gtalhgkqbi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.0kj1m.cn/gtqmwjnhvl.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hnxiangtu.top/gtlgfnhlye.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.mhx1999.top/gtyriwtogg.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hongshengwenyu.top/gtrarmzszc.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.gogol.net.cn/gtdxuoxbrb.html

[I07] 忽略大小写与多行模式
来源：http://hz.cucudq.cn/gtkozdzdnb.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hongshengwenyu.top/gtsvpiwgzs.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zycfv.cn/gtlfvqkplv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.havefunace.top/gtgobwcxzy.html

TS:   /error/gim
来源：http://hz.zycfv.cn/gtuttgmbpy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yuxming.cn/gtlpagtgug.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xinyue.icu/gthogfsgdu.html

Ruby: s.scan(/error/i)
来源：http://hz.aibaodan.cn/gtoitxrhtn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.daria6918.cn/gtbsqnckzx.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yuxming.cn/gtkfcovahk.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.chenzaomai.com/gtxdksfbej.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.chenlongwang.top/gtvymqisoc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ehwqpu.com/gtthhmnmkg.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yanxiufei.cn/gtfcfipmny.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.gogol.net.cn/gtjthqzinp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.chenjidiqi.icu/gtkowxnbeg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jianghu66.top/gtpezrsmia.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.guowangkeji.top/gtalgjatdg.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtnjntkmmz.html

J. 日期与时间
来源：http://hz.yvedp.cn/gtfanoepnm.html

================================================================================
来源：http://hz.aibaodan.cn/gtojmfqxna.html

[J01] 获取当前时间
来源：http://hz.gogol.net.cn/gtnabupsuh.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xingfuxueyuan.xyz/gteppksvfy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yongpay.top/gtyrogobmv.html

JS:   new Date();  Date.now()
来源：http://hz.hnxiangtu.top/gtsmawctiz.html

TS:   new Date();  Date.now()
来源：http://hz.iojbl.cn/gthsnmsyyb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.zhengqikj.top/gtoouwjqdd.html

Go:   time.Now()
来源：http://hz.tian-w.cn/gtcijkfozd.html

Ruby: Time.now
来源：http://hz.pycfn.com/gtthnmicmq.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.snrcjt.cn/gtjxeltqav.html

[J02] 格式化输出
来源：http://hz.guowangkeji.top/gtsyyxpncy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fzhhl.top/gtepwdjvbt.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.tianlin.xyz/gthjrwopkm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.chenlongwang.top/gtsrpgjjqa.html

TS:   d.toISOString()
来源：http://hz.jqgfzy.top/gtnhdciefo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhijiandao.cn/gtplmoahef.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.bjfxy.top/gtgwgbncen.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yanxiufei.cn/gteuykvpqa.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gogol.net.cn/gtkmgcbbke.html

[J03] 字符串解析为日期
来源：http://hz.hnqzz.top/gtbcrnoaml.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.vqdsnc.cn/gtrlrqblzq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jyoumei.cn/gtzmajfaji.html

JS:   new Date("2024-01-02")
来源：http://hz.yj20258.top/gtrdsvvuzk.html

TS:   new Date("2024-01-02")
来源：http://hz.zhengqikj.top/gtorbfqsnx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtjarpbxlq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.c1oappe.top/gtdidotirk.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cheryme.top/gtpbiosaip.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinqigufen.top/gtgzqnxvhl.html

[J04] 时间戳与日期互转
来源：http://hz.yvedp.cn/gtskdklvtd.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhengqikj.top/gtwozbfcza.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ehwqpu.com/gtnhkkrpne.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.guowangkeji.top/gtnbkazwwm.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yj202588.top/gtklhrkkta.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xylfe.cn/gtcjvtvrex.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.ybcxt.top/gtnfgdupfo.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zdqjudy.top/gtrelruzyg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yuanzhike.top/gtzkiexbej.html

[J05] 时间加减（加 7 天）
来源：http://hz.smart0.xyz/gtxnbqykru.html

Py:   now + timedelta(days=7)
来源：http://hz.guowangkeji.top/gtcjhuspud.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.0kj1m.cn/gtfcahtios.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ywan-chungtsiang.top/gtdbizzxrv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jqgfzy.top/gtetzpgupm.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.hywenlv.cn/gtatocqksi.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cqqwz.cn/gtgniorexa.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jqgfzy.top/gtmhgyzphs.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.snrcjt.cn/gtlbliuebz.html

[J06] 计算两时间之差
来源：http://hz.zhiwuduotai.top/gtzimmthrx.html

Py:   (end - start).total_seconds()
来源：http://hz.fzhhl.top/gtqbacxfnf.html

PHP:  $end->diff($start)->days;
来源：http://hz.jlsjyb.cn/gtzwantewi.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.mhx1999.top/gtjckrojph.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ydzc1.top/gthptdaiyi.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jlsjyb.cn/gtoiafnjqj.html

Go:   end.Sub(start).Hours()
来源：http://hz.aibaodan.cn/gtlfokifva.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ivvv.top/gtspilgrxu.html

C#:   (end - start).TotalSeconds
来源：http://hz.daria6918.cn/gtmcoqopdm.html

[J07] 比较两个日期
来源：http://hz.havefunace.top/gtsplrpzij.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.redwolf501.top/gthnadmjpp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.wangdashe.top/gtiyzucwap.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.fengsongda.top/gtvksndbri.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.feifeiyinyue.top/gtmdonxojp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.dashuyun.cn/gtuozlrmtu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.chenlongwang.top/gthvusdhxx.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.sufxvd.cn/gtcrgnzofv.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jinqigfzy.top/gtbukbwmfe.html

[J08] 提取年月日与星期
来源：http://hz.52xcode.cn/gtudmoaxrr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.chenlongwang.top/gtxegjfxrc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.bjfxy.top/gtlycjkedm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.aizwys.cn/gtclqiifdm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.kuanghao11.cn/gtxbqoklya.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.fengsongda.top/gtyexddugr.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yuanzhike.top/gtlragsmwy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jiagoushi.top/gtepbikccm.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ybcxt.top/gtzfwpefwv.html

[J09] 时区处理
来源：http://hz.sxryk.cn/gtkgzorbmo.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.andypj.xyz/gtrkdftyco.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jiagoushi.top/gtugrodssl.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xuetiantiany.cn/gtotzqgscc.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.0kj1m.cn/gtcjtjuezl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cheryme.top/gtlwlymflq.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.hfpthk.cn/gtwndqgqrp.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.zhaomingkeji.xyz/gtarkmopha.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinghuilouyu.cn/gtcnceyibw.html

[J10] 取今天 / 本月第一天
来源：http://hz.52xcode.cn/gtrqyvossm.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.xziqi.cn/gtxkjingsl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yj202588.top/gtxgkuzkfq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.dianchejie.cn/gtuzomqmub.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.xuanzx.com/gtokpigaec.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.yanxiufei.cn/gtpoksdtmc.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.pycfn.com/gttnbqlfjm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhijiandao.cn/gtqrkhgmyn.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.yanxiufei.cn/gtzebrbsvt.html

================================================================================
来源：http://hz.jianghu66.top/gtlxmyokmh.html

K. JSON 与序列化
来源：http://hz.shuidangran.top/gtpbnxvhqk.html

================================================================================
来源：http://hz.shuidangran.top/gtgbrnhyqo.html

[K01] 对象转 JSON 字符串
来源：http://hz.shangyingyoupin.top/gthyrzvhcz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.ydjk.org.cn/gtowzdsfxn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.zhoulong.xyz/gtcsbqrdie.html

JS:   JSON.stringify(obj)
来源：http://hz.zdqjudy.top/gtsfmwctvo.html

TS:   JSON.stringify(obj)
来源：http://hz.c1oappe.top/gtgmjrufkp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.guannengcc.top/gtymxhmztc.html

Go:   json.Marshal(obj)
来源：http://hz.wangshuangyany.cn/gtthpsusir.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.tianlin.xyz/gtqzwbzprs.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.nanxinkj.top/gtoufdkrlp.html

[K02] JSON 字符串转对象
来源：http://hz.xziqi.cn/gtpaxakjzx.html

Py:   json.loads(s)
来源：http://hz.jinyuanbaomall.cn/gtszjcxkqv.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.sxryk.cn/gtsbjtyimr.html

JS:   JSON.parse(s)
来源：http://hz.jlsjyb.cn/gtoslrdpgs.html

TS:   JSON.parse(s)
来源：http://hz.yj202588.top/gtiqnbbacn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.jinghuilouyu.cn/gtlwtsrkxo.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.quarkkingdee.top/gtkvacvlso.html

Ruby: JSON.parse(s)
来源：http://hz.xinyue.icu/gtsamexptz.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.tanke756.top/gtsouvwhqk.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.hongshengwenyu.top/gtqwmrsrfi.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.gotoacloud.top/gtznwlodzt.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zdqjudy.top/gtioeymuga.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.xingfuxueyuan.xyz/gtrznktrop.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.sysykeji.top/gtgsnypuam.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.hysaishi.cn/gtjgvqyvjo.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.zhoulong.xyz/gtbqnwgbzx.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.zhengqikj.top/gtuptjgewf.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.nwbrower.top/gtirmyhxxc.html

[K04] 读取 JSON 文件
来源：http://hz.fzhhl.top/gtruszurfk.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hnxiangtu.top/gtfmoznbfe.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xziqi.cn/gtfgawkkcv.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.wangshuangyany.cn/gtstbxxyvn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhaomingkeji.xyz/gtvricrypc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.snrcjt.cn/gthpugypee.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.redwolf501.top/gtaaprukwu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.52xcode.cn/gtwcipgkif.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.yuanzhike.top/gtrywmisos.html

[K05] 深拷贝对象
来源：http://hz.xylfe.cn/gtbgugzpou.html


<!-- 参考信息 -->