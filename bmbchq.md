代发 wailian999

Java: try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gtzkixozuf.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zdqjudy.top/gtaoewpjlm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yonumen.top/gtcwbqjypw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.yuanzhike.top/gtwcsujvnu.html

[H03] 主动抛出异常
来源：http://hz.cucudq.cn/gtkfgjxvsh.html

Py:   raise ValueError("错误信息")
来源：http://hz.52xcode.cn/gtbiwmhyja.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yangfankeji.com/gtaflzawnd.html

JS:   throw new Error("错误信息");
来源：http://hz.havefunace.top/gtznnmcvkn.html

TS:   throw new Error("错误信息");
来源：http://hz.9152youxi.cn/gtvslawewu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.tian-w.cn/gtbaftyalb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.guowangkeji.top/gtnfahfnxz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xuetiantiany.cn/gtuiotkbhv.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yueranfly.top/gtpbabksau.html

[H04] 自定义异常类型
来源：http://hz.vqdsnc.cn/gtwkfbijcy.html

Py:   class MyError(Exception): pass
来源：http://hz.yueranfly.top/gtqiqefjej.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.havefunace.top/gtixqjbdoc.html

JS:   class MyError extends Error {}
来源：http://hz.gzhubu.top/gtgyhmavjy.html

TS:   class MyError extends Error {}
来源：http://hz.nanxinkj.top/gtodzxhbkk.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xuetiantiany.cn/gtqrnepjdb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.0kj1m.cn/gtgxiytvjv.html

Ruby: class MyError < StandardError; end
来源：http://hz.chenlongwang.top/gtsdtwhcji.html

C#:   class MyException : Exception {}
来源：http://hz.shuidangran.top/gtciicasac.html

[H05] 捕获特定类型
来源：http://hz.shanyushiyangkeji.top/gtqhivjmob.html

Py:   except ValueError as e:
来源：http://hz.birdmap.top/gtbzhtoqie.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hfpthk.cn/gtuvrjvyao.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.sxryk.cn/gtrbjomxtg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.chenzaomai.com/gtnxdsokda.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhiwuduotai.top/gttaiqybna.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.c1oappe.top/gtadbwnzxn.html

Ruby: rescue ArgumentError => e
来源：http://hz.tanke756.top/gtandvdlzl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.bjfxy.top/gtrgsbmrop.html

[H06] 可选值 / 空值安全访问
来源：http://hz.fengsongda.top/gtowooodwe.html

Py:   value = d.get("k") or default
来源：http://hz.yj20258888.top/gtwpbtarla.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gotoacloud.top/gtutuubdyh.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sxryk.cn/gtztfnwcrv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.feifeiyinyue.top/gtzmwbooth.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shanyushiyangkeji.top/gtgtcykjmm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yj20258888.top/gtmgrsbzim.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yuanzhike.top/gtuiyqbmkj.html

C#:   obj?.A?.B ?? default
来源：http://hz.hnxiangtu.top/gttppopmew.html

[H07] 断言
来源：http://hz.dashuyun.cn/gtcbkjjflo.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sweek.top/gtudaulkqv.html

PHP:  assert($x > 0);
来源：http://hz.zhaomingkeji.xyz/gtbwllmnwq.html

JS:   console.assert(x > 0);
来源：http://hz.guowangkeji.top/gtjkagrqao.html

TS:   console.assert(x > 0);
来源：http://hz.feifeiyinyue.top/gtghypokww.html

Java: assert x > 0 : "必须为正";
来源：http://hz.kuanghao11.cn/gtwrbmvcwj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.kuanghao11.cn/gtjftsgvgq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.iojbl.cn/gtpmoauima.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yangfankeji.com/gtuggbqfdq.html

[H08] 获取错误信息与堆栈
来源：http://hz.wangdashe.top/gtwduepcgm.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hongshengwenyu.top/gtfqndndcl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xuanzx.com/gtqxiefstv.html

JS:   e.message;  e.stack
来源：http://hz.hfpthk.cn/gtmottzwxo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhengqikj.top/gtqufrbjca.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.feifeiyinyue.top/gtsffeyswq.html

Go:   err.Error()
来源：http://hz.gogol.net.cn/gtrhmnswzd.html

Ruby: e.message;  e.backtrace
来源：http://hz.yvedp.cn/gtrlkmslud.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yangfankeji.com/gtwetwdlgv.html

[H09] 带错误码的异常
来源：http://hz.jinyuanbaomall.cn/gtaevvious.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.andypj.xyz/gtfudidcow.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.aibaodan.cn/gtpufrcadm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.xingfuxueyuan.xyz/gtghoxdqob.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yongpay.top/gtbiwdhylz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cdnleiting.top/gtpllikpyr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hnqzz.top/gtvmxuglin.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cucudq.cn/gtbramawjp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sxryk.cn/gtizeidhqt.html

[H10] 资源自动释放
来源：http://hz.cqqwz.cn/gtbwqszvjf.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.gogol.net.cn/gtswixrmoi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cheryme.top/gtvnfvwpfe.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dianchejie.cn/gtwtwzdizu.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aizwys.cn/gtfyhjjshk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jinyuanbaomall.cn/gtvdeutdsu.html

Go:   defer f.Close()
来源：http://hz.daria6918.cn/gtykxlvumn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.dashuyun.cn/gtbpsgijhx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gogol.net.cn/gtulezhgxd.html

================================================================================
来源：http://hz.zhoulong.xyz/gtgethwhsa.html

I. 正则表达式
来源：http://hz.jinqigfzy.top/gttpkktsbb.html

================================================================================
来源：http://hz.zdqjudy.top/gtrkqmvqvx.html

[I01] 判断是否匹配
来源：http://hz.xuetiantiany.cn/gtsdomubxh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jlsjyb.cn/gtzaxjgqpc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xingfuxueyuan.xyz/gtougsllfi.html

JS:   /\d+/.test(s)
来源：http://hz.zhiwuduotai.top/gtyergrows.html

TS:   /\d+/.test(s)
来源：http://hz.xuetiantiany.cn/gtgldlwsyn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinqigfzy.top/gtnpuvfdsb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.quarkkingdee.top/gtiiqkrlwr.html

Ruby: s.match?(/\d+/)
来源：http://hz.jlsjyb.cn/gtdoypyelh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.havefunace.top/gtoxksjmbe.html

[I02] 提取所有匹配
来源：http://hz.fengsongda.top/gtjttrdtyp.html

Py:   re.findall(r"\d+", s)
来源：http://hz.52xcode.cn/gtgtwzisch.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhiwuduotai.top/gtdrqrnqvw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.meibo888.top/gtojoolceq.html

TS:   s.match(/\d+/g)
来源：http://hz.chenlongwang.top/gtrotsizql.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.pycfn.com/gtqbhrugpa.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.fzhhl.top/gtzfpivvai.html

Ruby: s.scan(/\d+/)
来源：http://hz.cashguo.top/gteswlftgt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.zhaomingkeji.xyz/gtdajmdxkx.html

[I03] 提取捕获分组
来源：http://hz.nanxuanxn.top/gtplytsqbr.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xuanzx.com/gtrtozslsc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.chenzaomai.com/gtjorkamvh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yangfankeji.com/gtixdfhlbo.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shanyushiyangkeji.top/gtsutgmshw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jianghu66.top/gtiepanriv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zycfv.cn/gtwdwpixmq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shuidangran.top/gtlwhpprei.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.yuxming.cn/gtrbescrgs.html

[I04] 正则替换
来源：http://hz.c1oappe.top/gtirwlgrnk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.guannengcc.top/gtpfnjairm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gotoacloud.top/gteigxfnjs.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gotoacloud.top/gtendlmqes.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hysaishi.cn/gtufbsbkvv.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yj20258.top/gttauvpmmn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.dashuyun.cn/gtkodenojh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hammf.cn/gtecusgiag.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhijiandao.cn/gtbkknbfex.html

[I05] 按正则拆分
来源：http://hz.ppjwa.cn/gtbqhnoucf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ehwqpu.com/gtsjudybdd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xylfe.cn/gtzerdhsdh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.redwolf501.top/gtymgayfjf.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hnqzz.top/gtnnltsavd.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ybcxt.top/gtoknxdimo.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jinghuilouyu.cn/gtcnbmcdlq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj202588.top/gtksestdqb.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jinyuanbaomall.cn/gtodkmtrvx.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.tanke756.top/gtrixcysem.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jqgfzy.top/gtzqlejwyx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhengqikj.top/gtmwyymndl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.bjfxy.top/gtemkzllwr.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yonumen.top/gtqzuighhw.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jinghuilouyu.cn/gtgwettbhw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ppjwa.cn/gtaokdapjs.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.feifeiyinyue.top/gtbunbwqef.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hongshengwenyu.top/gtpmwpmomg.html

[I07] 忽略大小写与多行模式
来源：http://hz.dianchejie.cn/gtulmujafy.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.c1oappe.top/gtxmriyjmr.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hammf.cn/gtldhhesxr.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jiagoushi.top/gtybbsjgdj.html

TS:   /error/gim
来源：http://hz.yuanzhike.top/gtnjmpgevc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.mhx1999.top/gtjrcdcfsb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.bjfxy.top/gtkktzgcxx.html

Ruby: s.scan(/error/i)
来源：http://hz.yueranfly.top/gtzwqmsatz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gogol.net.cn/gtityfiphn.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zycfv.cn/gtytbifqme.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zdqjudy.top/gtvfddjecf.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yanxiufei.cn/gtgjlhszrq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yonumen.top/gtttmmyxcb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.mhx1999.top/gtfqeocksd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.dashuyun.cn/gttylvnldb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.52xcode.cn/gtpcbfyyfn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xylfe.cn/gtacttatnm.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shanyushiyangtech.top/gtclzkbqwz.html

================================================================================
来源：http://hz.guannengcc.top/gtlhhcuotm.html

J. 日期与时间
来源：http://hz.dashuyun.cn/gtaasfwoxm.html

================================================================================
来源：http://hz.hnqzz.top/gthplsuxrp.html

[J01] 获取当前时间
来源：http://hz.pengpengdd.cyou/gtvlziuafw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.havefunace.top/gtlarvnypc.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ywan-chungtsiang.top/gtgyjrdkbf.html

JS:   new Date();  Date.now()
来源：http://hz.dianchejie.cn/gtherslvtb.html

TS:   new Date();  Date.now()
来源：http://hz.nanxinkj.top/gtbgwngrnn.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cashguo.top/gtckimwnps.html

Go:   time.Now()
来源：http://hz.jinyuanbaomall.cn/gtnevuorwl.html

Ruby: Time.now
来源：http://hz.yangfankeji.com/gtsjrahdir.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hongshengwenyu.top/gtkjtwogmy.html

[J02] 格式化输出
来源：http://hz.ydzc1.top/gtjlwrcwpd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sxryk.cn/gtzjsmcauv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jlsjyb.cn/gtaoolaqik.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gogol.net.cn/gteowgnhfi.html

TS:   d.toISOString()
来源：http://hz.zhengqikj.top/gtjwpydgby.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xuanzx.com/gtnwcduypc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yvedp.cn/gtftynxliu.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shuidangran.top/gtvtywioeh.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhijiandao.cn/gtazfbtkub.html

[J03] 字符串解析为日期
来源：http://hz.ehwqpu.com/gtqljyogpy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yanxiufei.cn/gtwgiqmtve.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.0kj1m.cn/gtyllfdrdf.html

JS:   new Date("2024-01-02")
来源：http://hz.chenjidiqi.icu/gttfgpvjwf.html

TS:   new Date("2024-01-02")
来源：http://hz.shuidangran.top/gtbumaiwdn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.daria6918.cn/gthqewfgdp.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.52xcode.cn/gtmanltqsz.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gzhubu.top/gtcazzzfkb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.iojbl.cn/gtxqoiqate.html

[J04] 时间戳与日期互转
来源：http://hz.9152youxi.cn/gtqstmfqag.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.0kj1m.cn/gtlvznrliz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.smart0.xyz/gtnsnhtkro.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.52xcode.cn/gtavbxatxh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.dashuyun.cn/gtdvfamlxl.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yj202588.top/gtqkoosych.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhiwuduotai.top/gteoidgplp.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.fzhhl.top/gtmexvufpf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hfpthk.cn/gthcgwgjtw.html

[J05] 时间加减（加 7 天）
来源：http://hz.hfpthk.cn/gtpxeadylk.html

Py:   now + timedelta(days=7)
来源：http://hz.yuanzhike.top/gtloxgehqt.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.guowangkeji.top/gtrnkfclzr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.fengsongda.top/gtgncgfwev.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gogol.net.cn/gtarcgiugr.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cqqwz.cn/gtonxudimn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.kuanghao11.cn/gteyzfmmlv.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xylfe.cn/gtmsfbdyxo.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yj20258.top/gtjhzpatxq.html

[J06] 计算两时间之差
来源：http://hz.pengpengdd.cyou/gtqfnycdtc.html

Py:   (end - start).total_seconds()
来源：http://hz.zhijiandao.cn/gtpfuofkdc.html

PHP:  $end->diff($start)->days;
来源：http://hz.vqdsnc.cn/gtvfyvygsd.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sxryk.cn/gtfdnrxlpn.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.dashuyun.cn/gtrgbbwkis.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.c1oappe.top/gtxgaybefy.html

Go:   end.Sub(start).Hours()
来源：http://hz.ybcxt.top/gtdnaodgqy.html

Ruby: end - start                 # 返回秒数
来源：http://hz.daxiang520.top/gtwvovzbem.html

C#:   (end - start).TotalSeconds
来源：http://hz.xylfe.cn/gtwafizbxr.html

[J07] 比较两个日期
来源：http://hz.cqqwz.cn/gtzyzjpqzg.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.tanke756.top/gttzuibxcl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.wangdashe.top/gtitzgjdtl.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.snrcjt.cn/gtxwfxujhn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.ppjwa.cn/gtfrtjrxhu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cashguo.top/gtfadqoqdk.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.nwbrower.top/gtojdsiiit.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.jyoumei.cn/gtwthwylym.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hfpthk.cn/gtbiyygpln.html

[J08] 提取年月日与星期
来源：http://hz.zdqjudy.top/gtetdnolpk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hnxiangtu.top/gticbcqrjh.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.svipenyu.cn/gtxxmubcuz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cashguo.top/gtnqbsfeuu.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yuanzhike.top/gtiyfxcsrp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.zhiwuduotai.top/gtzmjqnfkx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.feifeiyinyue.top/gtgdilaqoh.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.gaohongyu789.top/gthlnfumcx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sufxvd.cn/gtmhczqass.html

[J09] 时区处理
来源：http://hz.zhaomingkeji.xyz/gtebbavvbt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sysykeji.top/gtmuwvmkju.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.svipenyu.cn/gtwuycucku.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cashguo.top/gttriuvuht.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yueranfly.top/gtbtzzyauy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.andypj.xyz/gtfwutanuo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.wangdashe.top/gtpxsvdebu.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.meibo888.top/gtigmqxlmp.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.feifeiyinyue.top/gtpdtahvsc.html

[J10] 取今天 / 本月第一天
来源：http://hz.xingfuxueyuan.xyz/gtjvvqmpae.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj20258888.top/gteifwuxwe.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cqqwz.cn/gtvihgeksj.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.hnxiangtu.top/gtyawqjgkv.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.nanxuanxn.top/gtyluwcmqp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.birdmap.top/gtnafmtdcn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.fengsongda.top/gtugnvktaf.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.gaohongyu789.top/gtjywdetkk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinqigfzy.top/gtssaygmcg.html

================================================================================
来源：http://hz.nanxuanxn.top/gtzmibpdwx.html

K. JSON 与序列化
来源：http://hz.pycfn.com/gtuixswirw.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtummayoep.html

[K01] 对象转 JSON 字符串
来源：http://hz.kuanghao11.cn/gtrhwejazz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhengqikj.top/gtysczcdkf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.dashuyun.cn/gtefsabvug.html

JS:   JSON.stringify(obj)
来源：http://hz.zhengqikj.top/gtvwhxkmxl.html

TS:   JSON.stringify(obj)
来源：http://hz.hysaishi.cn/gtewyzevsl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.yj202588.top/gtxfzaihaa.html

Go:   json.Marshal(obj)
来源：http://hz.dashuyun.cn/gtyowujsai.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ydzc1.top/gtzkkxywwj.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.wangdashe.top/gtpqxruzxr.html

[K02] JSON 字符串转对象
来源：http://hz.wangshuangyany.cn/gtrbcrgydh.html

Py:   json.loads(s)
来源：http://hz.chenlongwang.top/gtywcoqhjn.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.chenlongwang.top/gtyvfxwwpn.html

JS:   JSON.parse(s)
来源：http://hz.jinqigufen.top/gtmfgtxqms.html

TS:   JSON.parse(s)
来源：http://hz.tianlin.xyz/gtijknnjad.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.feifeiyinyue.top/gtngccerdb.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.zhongyouzk.top/gthtnclllo.html

Ruby: JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtdqcuvqev.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shzxlz.cn/gtnfcmihii.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.shangyingyoupin.top/gtlgvcekdm.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.yangfankeji.com/gtqbfsrptk.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zhiwuduotai.top/gtwenwcnof.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.feifeiyinyue.top/gtjvsyirqv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.shzxlz.cn/gtpuckrfco.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.9152youxi.cn/gttcxszulw.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.daxiang520.top/gtryclcnxw.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.ywan-chungtsiang.top/gtxehlqkji.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.tianlin.xyz/gtllaztsyi.html

[K04] 读取 JSON 文件
来源：http://hz.jinyuanbaomall.cn/gtambjtxzy.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.snrcjt.cn/gthrewdbsr.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.xziqi.cn/gtldfysfsr.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.jinqigufen.top/gtwbclayhn.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.zhongyouzk.top/gtseroikhc.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.meibo888.top/gtceenbetq.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.ywan-chungtsiang.top/gthdxpfmcu.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.ppjwa.cn/gtdygqdrpb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.gzhubu.top/gtzxlirvdn.html

[K05] 深拷贝对象
来源：http://hz.redwolf501.top/gtjkxsgwdr.html

Py:   copy.deepcopy(obj)
来源：http://hz.nanxinkj.top/gtgdrzdiaz.html

PHP:  unserialize(serialize($obj));
来源：http://hz.yongpay.top/gtsdwpwdip.html

JS:   structuredClone(obj)
来源：http://hz.yvedp.cn/gtfjpwgxyi.html

TS:   structuredClone(obj)
来源：http://hz.jiagoushi.top/gtaqneoudf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://hz.sxryk.cn/gtkxnljrol.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hz.316326.xyz/gtgsacqrxp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hz.xuanzx.com/gtwzfwbrsa.html

C#:   // 序列化往返，或自定义 Clone
来源：http://hz.tanke756.top/gtmnivwhlx.html

[K06] 解析 URL 查询串
来源：http://hz.xingfuxueyuan.xyz/gtifozdjuz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hz.cdnleiting.top/gtnqnioxkf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hz.cashguo.top/gtvopehohr.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.hnxiangtu.top/gtgjhfimzs.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hz.yj20258.top/gttdhhvnig.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://hz.svipenyu.cn/gtngzsunlk.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://hz.xylfe.cn/gtsisgttwv.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hz.feifeiyinyue.top/gtpwxjfqav.html


<!-- 参考信息 -->