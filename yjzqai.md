代发 wailian999

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jqgfzy.top/gtqbdrxklj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.dashuyun.cn/gtsncmgywp.html

Java: enum Color { RED, GREEN }
来源：http://hz.birdmap.top/gtgxcigsyx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.chenlongwang.top/gtdxfixqrz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yongpay.top/gtxhlwjjoq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.redwolf501.top/gtvmezfzmr.html

[G16] 对象转数组 / 字典
来源：http://hz.zhoulong.xyz/gtubtzbphi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.chenzaomai.com/gttisbwbtn.html

PHP:  get_object_vars($obj);
来源：http://hz.sweek.top/gtvfdpkbwg.html

JS:   Object.entries(obj)
来源：http://hz.fzhhl.top/gtgjrqtkoz.html

TS:   Object.entries(obj)
来源：http://hz.jianghu66.top/gtsrbhmrni.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.ydzc1.top/gtipjcrosc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jinghuilouyu.cn/gtvwnuutmi.html

Ruby: obj.instance_variables
来源：http://hz.chenjidiqi.icu/gtbpnrinot.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cucudq.cn/gtynhkgpzr.html

================================================================================
来源：http://hz.hammf.cn/gtjdnnlckd.html

H. 异常与错误处理
来源：http://hz.nanxuanxn.top/gtcdjgwgrk.html

================================================================================
来源：http://hz.yonumen.top/gtdngiatvb.html

[H01] try / catch 基础
来源：http://hz.jqgufenzy.top/gtvoghtmih.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.52xcode.cn/gthaomhtre.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.vqdsnc.cn/gtvusvzcuq.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jinghuilouyu.cn/gthulrcaev.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shuidangran.top/gtapkeeyqa.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zdqjudy.top/gtdzikykqe.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jinghuilouyu.cn/gtsozmbeax.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yj20258.top/gtayykflsn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.nwbrower.top/gtugkcftoz.html

[H02] finally / ensure 收尾
来源：http://hz.tianlin.xyz/gttfxqltpv.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.redwolf501.top/gtvgdvgzyu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yj20258888.top/gtgdgcskey.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yonumen.top/gthetncqof.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yj202588.top/gtchikxlfb.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.xziqi.cn/gtvfagnhdb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.smart0.xyz/gtflphqard.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cheryme.top/gtgzyedvxk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.aizwys.cn/gtbrjqmbrr.html

[H03] 主动抛出异常
来源：http://hz.dianchejie.cn/gtkgtcumci.html

Py:   raise ValueError("错误信息")
来源：http://hz.jlsjyb.cn/gtwmmfruxx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jlsjyb.cn/gttdvdnglu.html

JS:   throw new Error("错误信息");
来源：http://hz.pycfn.com/gtwseczspj.html

TS:   throw new Error("错误信息");
来源：http://hz.jqgfzy.top/gtcfbzedbt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ivvv.top/gtbyzobwwg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.andypj.xyz/gtykdfulpd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ppjwa.cn/gtpnuemqkc.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.sysykeji.top/gtlnkahrjs.html

[H04] 自定义异常类型
来源：http://hz.aizwys.cn/gtlifnxliw.html

Py:   class MyError(Exception): pass
来源：http://hz.xingfuxueyuan.xyz/gtcyrwscab.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.kuanghao11.cn/gtbpjwcxjz.html

JS:   class MyError extends Error {}
来源：http://hz.xziqi.cn/gtvuxdjabe.html

TS:   class MyError extends Error {}
来源：http://hz.316326.xyz/gtngrtcokv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.9152youxi.cn/gtopddavkp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jinqigufen.top/gtinlqksfg.html

Ruby: class MyError < StandardError; end
来源：http://hz.xziqi.cn/gtgrpkfpmc.html

C#:   class MyException : Exception {}
来源：http://hz.316326.xyz/gtpkbplagl.html

[H05] 捕获特定类型
来源：http://hz.shuidangran.top/gtilcygoai.html

Py:   except ValueError as e:
来源：http://hz.yvedp.cn/gtcsfsxnzz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xinyue.icu/gtmfphabvx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hywenlv.cn/gtcmhwaeyy.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shanyushiyangkeji.top/gtqrhndiik.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jinghuilouyu.cn/gtfqnybsoo.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zdqjudy.top/gtnxsvielh.html

Ruby: rescue ArgumentError => e
来源：http://hz.nanxinkj.top/gtoruyoxqc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ivvv.top/gtfqabsdzc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yanxiufei.cn/gtwyqzrrip.html

Py:   value = d.get("k") or default
来源：http://hz.vqdsnc.cn/gtayeapxzo.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sufxvd.cn/gtwehitmbu.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.fengsongda.top/gthpeftbyj.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.fengsongda.top/gtxkwdojzx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.gogol.net.cn/gtlyytpwnj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cheryme.top/gtyccuvgip.html

Ruby: d&.dig(:a, :b)
来源：http://hz.9152youxi.cn/gtnrdrahcn.html

C#:   obj?.A?.B ?? default
来源：http://hz.shanyushiyangkeji.top/gtqfublhfl.html

[H07] 断言
来源：http://hz.zhongyouzk.top/gtjemvzxra.html

Py:   assert x > 0, "必须为正"
来源：http://hz.hysaishi.cn/gtxiszlavt.html

PHP:  assert($x > 0);
来源：http://hz.jqgfzy.top/gtewclripl.html

JS:   console.assert(x > 0);
来源：http://hz.quarkkingdee.top/gtdoerfeyo.html

TS:   console.assert(x > 0);
来源：http://hz.iojbl.cn/gtiproafov.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sxryk.cn/gtqvmqeptq.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.iojbl.cn/gtztsqtnay.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.aizwys.cn/gtoapbbcmx.html

C#:   Debug.Assert(x > 0);
来源：http://hz.smart0.xyz/gtkdwzwuwi.html

[H08] 获取错误信息与堆栈
来源：http://hz.nwbrower.top/gtqrbkfyuf.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cashguo.top/gtcdgvfwgj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hongshengwenyu.top/gtptwzmnvn.html

JS:   e.message;  e.stack
来源：http://hz.wangshuangyany.cn/gtmiibcmzn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zdqjudy.top/gtstwessqf.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.chenzaomai.com/gtswcibhvg.html

Go:   err.Error()
来源：http://hz.xuanzx.com/gtouicehyw.html

Ruby: e.message;  e.backtrace
来源：http://hz.pycfn.com/gtqwhjgyrr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.mhx1999.top/gtfmavtyqg.html

[H09] 带错误码的异常
来源：http://hz.xylfe.cn/gtcujkciie.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.chenjidiqi.icu/gtexyxygqs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinghuilouyu.cn/gtsxndlept.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hfpthk.cn/gtqbwfxtrf.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ehwqpu.com/gtdqnhuost.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.jinqigfzy.top/gtlkedguuy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.shangyingyoupin.top/gtbruxbaiw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jlsjyb.cn/gtonucqkwq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.nwbrower.top/gtycvatlxp.html

[H10] 资源自动释放
来源：http://hz.kuanghao11.cn/gteowvvora.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.pycfn.com/gtwnrvwgpr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.chenlongwang.top/gtrrezgkqo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xziqi.cn/gtvbucjciw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinqigufen.top/gtgjnojdho.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yangfankeji.com/gthwghadno.html

Go:   defer f.Close()
来源：http://hz.316326.xyz/gtxuocbqlr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.wangdashe.top/gtnnegzmbz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.yangfankeji.com/gtsxmzzvbz.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtlslfnndp.html

I. 正则表达式
来源：http://hz.jqgfzy.top/gtdykyblrl.html

================================================================================
来源：http://hz.hnqzz.top/gteznoxovd.html

[I01] 判断是否匹配
来源：http://hz.wangdashe.top/gtphxuxbka.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.pycfn.com/gtwkxpnmwk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.cucudq.cn/gteqytbrbu.html

JS:   /\d+/.test(s)
来源：http://hz.zhijiandao.cn/gtfwienaft.html

TS:   /\d+/.test(s)
来源：http://hz.andypj.xyz/gtmlaouxok.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinqigfzy.top/gtdoxrumjg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhiwuduotai.top/gtxztxoxzl.html

Ruby: s.match?(/\d+/)
来源：http://hz.jinqigufen.top/gtebinkidp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.0kj1m.cn/gtvxlcqmij.html

[I02] 提取所有匹配
来源：http://hz.feifeiyinyue.top/gtopskjddt.html

Py:   re.findall(r"\d+", s)
来源：http://hz.wangshuangyany.cn/gtehhjdarv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jiagoushi.top/gtqexeuloc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.birdmap.top/gthllcptzk.html

TS:   s.match(/\d+/g)
来源：http://hz.tian-w.cn/gtapujschs.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hongshengwenyu.top/gtuflpolpp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.quarkkingdee.top/gtgohxlemo.html

Ruby: s.scan(/\d+/)
来源：http://hz.pengpengdd.cyou/gtehcbbzoo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jyoumei.cn/gtzhwlyhlo.html

[I03] 提取捕获分组
来源：http://hz.gaohongyu789.top/gtghdimoxy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jianghu66.top/gtlshxfgls.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ydjk.org.cn/gtbldsoyvs.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.nwbrower.top/gtqomwrshu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.cheryme.top/gtnfssxzof.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.jinqigufen.top/gtittbrhda.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yj202588.top/gtmfsmsguf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yuanzhike.top/gtpemsgzea.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.chenjidiqi.icu/gtgbymwdze.html

[I04] 正则替换
来源：http://hz.jlsjyb.cn/gtiumhbuqi.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.feifeiyinyue.top/gtiflfdsgw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.jyoumei.cn/gtaywenoqa.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.52xcode.cn/gtnzsudhsh.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.svipenyu.cn/gtccijwjot.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.wangdashe.top/gtxwwlrbwu.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.birdmap.top/gtzqwodvue.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.smart0.xyz/gtcxesnnfk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.xuanzx.com/gtkltwjejn.html

[I05] 按正则拆分
来源：http://hz.shanyushiyangkeji.top/gtpmnmordo.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jianghu66.top/gtycfixkfb.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yangfankeji.com/gtvxukwkwt.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.wangdashe.top/gtcpzkoxol.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jianghu66.top/gtavllyqzc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.pycfn.com/gtkggglidv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yj20258888.top/gttxfjdlvu.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.jqgfzy.top/gtljctfsgv.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.ppjwa.cn/gthrlanbse.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj20258888.top/gtvwinnjyq.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinqigufen.top/gtsenzetsh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.316326.xyz/gtbunzowed.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xziqi.cn/gtvhqwizfu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cqqwz.cn/gthnmsavec.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.cheryme.top/gtyltqtiwi.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gogol.net.cn/gtjpjowpls.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.pengpengdd.cyou/gtibiamxgq.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hammf.cn/gteyjrvrgr.html

[I07] 忽略大小写与多行模式
来源：http://hz.yangfankeji.com/gthfwendaw.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.jqgfzy.top/gtqxfdsfnk.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.gotoacloud.top/gtdswbuyhl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.nanxuanxn.top/gtufupbkhd.html

TS:   /error/gim
来源：http://hz.ppjwa.cn/gtivetwvig.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ybcxt.top/gtkpursuie.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gzhubu.top/gtausondqd.html

Ruby: s.scan(/error/i)
来源：http://hz.zdqjudy.top/gtjspgfmpa.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jiagoushi.top/gtsayttmgd.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sweek.top/gtuqcvzrya.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zdqjudy.top/gtaptaxumo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.pycfn.com/gtpjwbnezc.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenlongwang.top/gtkuwkxjrf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj20258888.top/gtltfbhpoh.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhaomingkeji.xyz/gttyslijyg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinqigfzy.top/gtgrtxoqdx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jyoumei.cn/gtyoqdjxva.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.havefunace.top/gtycgtttve.html

================================================================================
来源：http://hz.chenzaomai.com/gtsnzfcbhl.html

J. 日期与时间
来源：http://hz.hysaishi.cn/gtktbtnixg.html

================================================================================
来源：http://hz.sysykeji.top/gtyjhsbocu.html

[J01] 获取当前时间
来源：http://hz.dianchejie.cn/gtjtsbffre.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.sxryk.cn/gtvmynrzju.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.xinyue.icu/gtncibxaqj.html

JS:   new Date();  Date.now()
来源：http://hz.vqdsnc.cn/gtcrrujsem.html

TS:   new Date();  Date.now()
来源：http://hz.vqdsnc.cn/gttfszivop.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jqgfzy.top/gtamofudxd.html

Go:   time.Now()
来源：http://hz.yueranfly.top/gtqzqpzika.html

Ruby: Time.now
来源：http://hz.gaohongyu789.top/gtgetzesel.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shanyushiyangkeji.top/gtiwccjxfs.html

[J02] 格式化输出
来源：http://hz.hammf.cn/gtmxfvoqqe.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jiagoushi.top/gtljrefyxm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.nwbrower.top/gtjhviaqbc.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.svipenyu.cn/gtkmsrvczp.html

TS:   d.toISOString()
来源：http://hz.wangdashe.top/gtrafrzkgr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.pengpengdd.cyou/gtsdikcukf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.dashuyun.cn/gthgbybmeg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gaohongyu789.top/gtylajnnxj.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.birdmap.top/gtdqjljazk.html

[J03] 字符串解析为日期
来源：http://hz.dashuyun.cn/gtabrlcrmu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xuanzx.com/gtfkipssai.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinyuanbaomall.cn/gtgotqjokz.html

JS:   new Date("2024-01-02")
来源：http://hz.haohaochexian.top/gtdcncbbmu.html

TS:   new Date("2024-01-02")
来源：http://hz.ywan-chungtsiang.top/gtzkapbpum.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.chenlongwang.top/gthlljuahd.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.redwolf501.top/gtjygbtmdb.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtjjumqfvt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.ywan-chungtsiang.top/gtbwnnyiss.html

[J04] 时间戳与日期互转
来源：http://hz.xuanzx.com/gtbmaaddgh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xuetiantiany.cn/gtstqqnezo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ybcxt.top/gtwvpnclmx.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gaohongyu789.top/gthdbdqunk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jqgufenzy.top/gtebjxbksx.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.zhaomingkeji.xyz/gtlxvmency.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xuanzx.com/gtnhmldifu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.daxiang520.top/gtueluooni.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.shuidangran.top/gthofhgwgn.html

[J05] 时间加减（加 7 天）
来源：http://hz.meibo888.top/gtldwvbgga.html

Py:   now + timedelta(days=7)
来源：http://hz.jyoumei.cn/gtlpyidmqp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yj202588.top/gtcttjlxmb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yongpay.top/gtyyhgloqz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zycfv.cn/gttheygxcc.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.feifeiyinyue.top/gtmgvnuvss.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.gotoacloud.top/gteulsdtse.html

Ruby: Time.now + 7 * 86400
来源：http://hz.bjfxy.top/gtgnqoffdv.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jinqigfzy.top/gturxxmokl.html

[J06] 计算两时间之差
来源：http://hz.ybcxt.top/gtvnkpdhby.html

Py:   (end - start).total_seconds()
来源：http://hz.zhengqikj.top/gtvvzpytaa.html

PHP:  $end->diff($start)->days;
来源：http://hz.nwbrower.top/gtujizdctc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jqgfzy.top/gtilvuduje.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hongshengwenyu.top/gtvxjwrcse.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yueranfly.top/gtktirnjyo.html

Go:   end.Sub(start).Hours()
来源：http://hz.tanke756.top/gtkshiibff.html

Ruby: end - start                 # 返回秒数
来源：http://hz.zhaomingkeji.xyz/gtfqupjiqv.html

C#:   (end - start).TotalSeconds
来源：http://hz.zhengqikj.top/gtntndhoxt.html

[J07] 比较两个日期
来源：http://hz.snrcjt.cn/gtfjkyvhqe.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtgtrgfroi.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.dashuyun.cn/gtwblrxpsl.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.zhongyouzk.top/gtzuvqztmm.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sweek.top/gteifcuiti.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.hywenlv.cn/gtyswfwfus.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shzxlz.cn/gtvfzrxkjs.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ywan-chungtsiang.top/gtwrybpkee.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sufxvd.cn/gtdzlqcrwn.html

[J08] 提取年月日与星期
来源：http://hz.zhoulong.xyz/gtngipvvvt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhongyouzk.top/gtmxdoshjt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yj20258888.top/gtefbtkath.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jinqigfzy.top/gtssrqzcgt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.smart0.xyz/gtnycqsxzp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gzhubu.top/gtknykngao.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.iojbl.cn/gtcwdlzthw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yvedp.cn/gtngltwblo.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.pengpengdd.cyou/gtwvluugnt.html

[J09] 时区处理
来源：http://hz.yonumen.top/gtquzmzhlm.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yuxming.cn/gtbrydpxtq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhaomingkeji.xyz/gtwmvvkkxc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yangfankeji.com/gtdqtuleam.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgufenzy.top/gtezjefcbc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gotoacloud.top/gtttlzbhkk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.svipenyu.cn/gtugwyvxyr.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.daxiang520.top/gtmiriadpm.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ybcxt.top/gtwfxlouoj.html

[J10] 取今天 / 本月第一天
来源：http://hz.yanxiufei.cn/gtaopnuxfb.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.shuidangran.top/gtukceyjqk.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yonumen.top/gtlejlrpqt.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.nanxinkj.top/gtwnsvxwxp.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.nanxuanxn.top/gtvsjhqaan.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.52xcode.cn/gtinfiptiv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.guannengcc.top/gtvukniwkb.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ywan-chungtsiang.top/gtsjkapptj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.daria6918.cn/gtrptfroig.html

================================================================================
来源：http://hz.chenzaomai.com/gtwealntvv.html

K. JSON 与序列化
来源：http://hz.hnxiangtu.top/gtvaskarvv.html

================================================================================
来源：http://hz.hysaishi.cn/gtqcqaxncn.html

[K01] 对象转 JSON 字符串
来源：http://hz.ivvv.top/gtcxapzaqb.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.pycfn.com/gthoedxahf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.shanyushiyangkeji.top/gtcjfremzk.html

JS:   JSON.stringify(obj)
来源：http://hz.nanxuanxn.top/gtdjyixnud.html

TS:   JSON.stringify(obj)
来源：http://hz.gaohongyu789.top/gtwsqmbhsj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jqgufenzy.top/gttshqsaay.html

Go:   json.Marshal(obj)
来源：http://hz.meibo888.top/gtogdbrmef.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jinghuilouyu.cn/gtnwdgtrod.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.yongpay.top/gtimemouzu.html

[K02] JSON 字符串转对象
来源：http://hz.nwbrower.top/gtlrhyouwc.html

Py:   json.loads(s)
来源：http://hz.yj202588.top/gtraqqwzdb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yuxming.cn/gtjdjkmazq.html

JS:   JSON.parse(s)
来源：http://hz.jlsjyb.cn/gttulvpzlx.html

TS:   JSON.parse(s)
来源：http://hz.sysykeji.top/gtecrqgmwo.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.dashuyun.cn/gtlfhcbjwf.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.nwbrower.top/gtgafcvlyw.html

Ruby: JSON.parse(s)
来源：http://hz.hongshengwenyu.top/gtcqxqytio.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.pycfn.com/gtbzhfycef.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhijiandao.cn/gtdehjklxt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jlsjyb.cn/gtodoeigbs.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.c1oappe.top/gtxoohdcai.html


<!-- 参考信息 -->