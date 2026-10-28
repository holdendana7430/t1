代发 wailian999

PHP:  get_object_vars($obj);
来源：http://hz.kuanghao11.cn/gtvhfnowcw.html

JS:   Object.entries(obj)
来源：http://hz.sxryk.cn/gtifqaujfu.html

TS:   Object.entries(obj)
来源：http://hz.fzhhl.top/gtvabajrrh.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.chenlongwang.top/gtebcsgoqp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.xinyue.icu/gtwsonhsdk.html

Ruby: obj.instance_variables
来源：http://hz.jinyuanbaomall.cn/gthrneiztk.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.hnxiangtu.top/gtoujbpulq.html

================================================================================
来源：http://hz.dashuyun.cn/gtcqmfbcfj.html

H. 异常与错误处理
来源：http://hz.cqqwz.cn/gttrrqlbkf.html

================================================================================
来源：http://hz.cucudq.cn/gtxrewtsvh.html

[H01] try / catch 基础
来源：http://hz.zhiwuduotai.top/gtpqvlkleb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.nanxuanxn.top/gtvyrmcrxe.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.9152youxi.cn/gtzxhbvmjz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.kuanghao11.cn/gtxefpcisn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.snrcjt.cn/gtoiaglnjp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.gotoacloud.top/gtbmfzixxh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yj202588.top/gtauogkibc.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.nanxuanxn.top/gtemhcdymz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yj20258888.top/gtpuhbwzzg.html

[H02] finally / ensure 收尾
来源：http://hz.ybcxt.top/gtytmzftfd.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yonumen.top/gtoffxbrwj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gtipfrwzsa.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gtzvdvkvzw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gtdnybxkzx.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtdqrdlzkl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.chenzaomai.com/gtamcwzydw.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.hysaishi.cn/gtqqtzrjmp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.havefunace.top/gtowqdgsjd.html

[H03] 主动抛出异常
来源：http://hz.52xcode.cn/gtqqqqgkpj.html

Py:   raise ValueError("错误信息")
来源：http://hz.snrcjt.cn/gtzxacpyxz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.haohaochexian.top/gtzmwviebt.html

JS:   throw new Error("错误信息");
来源：http://hz.daxiang520.top/gtpqjtfeds.html

TS:   throw new Error("错误信息");
来源：http://hz.ydzc1.top/gtgmkhbels.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.guowangkeji.top/gtvxlkpdvs.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhongyouzk.top/gthuwcifbx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yongpay.top/gtyhbfwgwm.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.9152youxi.cn/gtcmewjydn.html

[H04] 自定义异常类型
来源：http://hz.sweek.top/gtgfdqawql.html

Py:   class MyError(Exception): pass
来源：http://hz.jianghu66.top/gtpgsqmese.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.tian-w.cn/gtivnuvzme.html

JS:   class MyError extends Error {}
来源：http://hz.tianlin.xyz/gtwjdxiygo.html

TS:   class MyError extends Error {}
来源：http://hz.cdnleiting.top/gtfqkywwpi.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yangfankeji.com/gtignpwdet.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jlsjyb.cn/gtdactnqpe.html

Ruby: class MyError < StandardError; end
来源：http://hz.haohaochexian.top/gtstfhozcc.html

C#:   class MyException : Exception {}
来源：http://hz.ehwqpu.com/gtfxwaptqt.html

[H05] 捕获特定类型
来源：http://hz.yueranfly.top/gtyagzamzk.html

Py:   except ValueError as e:
来源：http://hz.nanxinkj.top/gtcnnnhjqa.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.dianchejie.cn/gttprlwlom.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.xuetiantiany.cn/gtwcoozqzt.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hfpthk.cn/gtdgamexno.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.zhengqikj.top/gtawtpcmkz.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ydzc1.top/gtckosgjeu.html

Ruby: rescue ArgumentError => e
来源：http://hz.ivvv.top/gtuqipibaa.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.dianchejie.cn/gtxdqqlebb.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nanxinkj.top/gtdzsqnomx.html

Py:   value = d.get("k") or default
来源：http://hz.hysaishi.cn/gtwntzoifm.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zycfv.cn/gtdcuwwteq.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.aibaodan.cn/gtuzjwnjzn.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.daxiang520.top/gtebokqxod.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yj20258.top/gtrnqqgqdv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yangfankeji.com/gtzcndsqcp.html

Ruby: d&.dig(:a, :b)
来源：http://hz.dashuyun.cn/gtoguujwkg.html

C#:   obj?.A?.B ?? default
来源：http://hz.xuanzx.com/gtzxmyvgbs.html

[H07] 断言
来源：http://hz.zhiwuduotai.top/gtmlfvplng.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhaomingkeji.xyz/gtxbksfuth.html

PHP:  assert($x > 0);
来源：http://hz.bjfxy.top/gtgzccacar.html

JS:   console.assert(x > 0);
来源：http://hz.zhoulong.xyz/gtznxhcsmx.html

TS:   console.assert(x > 0);
来源：http://hz.yj20258888.top/gtsrfqdoeq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yj20258.top/gtrbprozbd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.svipenyu.cn/gtdgforeoh.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.snrcjt.cn/gtkmkqwefi.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhengqikj.top/gtnpsogehm.html

[H08] 获取错误信息与堆栈
来源：http://hz.xylfe.cn/gtceufagyo.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.birdmap.top/gtihhmrder.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jyoumei.cn/gtnkgbwfao.html

JS:   e.message;  e.stack
来源：http://hz.snrcjt.cn/gtgrwjroqv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.aizwys.cn/gtevauzngs.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hfpthk.cn/gtgicezvaf.html

Go:   err.Error()
来源：http://hz.xziqi.cn/gtoakmtdrr.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhiwuduotai.top/gtxxzrvhsu.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhiwuduotai.top/gtahxkuntw.html

[H09] 带错误码的异常
来源：http://hz.dianchejie.cn/gtprottqmw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.aizwys.cn/gtzkderzuw.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.vqdsnc.cn/gtuhrwpwcz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhengqikj.top/gtgunjxshp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ehwqpu.com/gtehexwjdc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hammf.cn/gtkvmxliku.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.sxryk.cn/gtcbygkuzl.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhaomingkeji.xyz/gtdfegvidf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.mhx1999.top/gtgvowbkdk.html

[H10] 资源自动释放
来源：http://hz.daxiang520.top/gtohytmwoq.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.shuidangran.top/gtadxfanfu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.smart0.xyz/gtivsohfvi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.wangshuangyany.cn/gtqgxzbkxn.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.ydjk.org.cn/gtqwtuqtkm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jinyuanbaomall.cn/gteuptekxk.html

Go:   defer f.Close()
来源：http://hz.52xcode.cn/gtoxfoiclb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yj202588.top/gtnviromfp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.quarkkingdee.top/gtdcsynjfy.html

================================================================================
来源：http://hz.xuanzx.com/gtcbxytzrh.html

I. 正则表达式
来源：http://hz.yonumen.top/gtaermzwge.html

================================================================================
来源：http://hz.andypj.xyz/gtlqzmflwt.html

[I01] 判断是否匹配
来源：http://hz.yj20258888.top/gtyumcjbfh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yuxming.cn/gtqfbadxid.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.hnxiangtu.top/gtvgobzfxu.html

JS:   /\d+/.test(s)
来源：http://hz.ivvv.top/gtdadcexli.html

TS:   /\d+/.test(s)
来源：http://hz.snrcjt.cn/gthvnjbmts.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhijiandao.cn/gtvpjgqcjo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jinqigfzy.top/gtsphbhhty.html

Ruby: s.match?(/\d+/)
来源：http://hz.nanxuanxn.top/gtazosdjik.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shzxlz.cn/gttvnjulxg.html

[I02] 提取所有匹配
来源：http://hz.daria6918.cn/gtlwotiwce.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ivvv.top/gtianbdnhp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.gaohongyu789.top/gtcsqtdoov.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.svipenyu.cn/gtugjbfump.html

TS:   s.match(/\d+/g)
来源：http://hz.zhixingplan.top/gtekdgincu.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yj20258888.top/gtuevintrx.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zdqjudy.top/gtehqwvxgv.html

Ruby: s.scan(/\d+/)
来源：http://hz.ybcxt.top/gtgvaasgbn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ywan-chungtsiang.top/gtpactacze.html

[I03] 提取捕获分组
来源：http://hz.dianchejie.cn/gtsakktmwf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhixingplan.top/gtdtxcqvrp.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yanxiufei.cn/gtcawqgsos.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yueranfly.top/gtrdemcgbu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yanxiufei.cn/gtyeobjrct.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ppjwa.cn/gtovudwuwu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.cashguo.top/gtewgnojhg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.haohaochexian.top/gtfeopybri.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhongyouzk.top/gtmnenauzw.html

[I04] 正则替换
来源：http://hz.yuanzhike.top/gtkmqzsjdp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.meibo888.top/gtbyspxyvm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.wangshuangyany.cn/gtulenvlby.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.chenjidiqi.icu/gtbyusfllc.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ydjk.org.cn/gtxzalzhzy.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.tianlin.xyz/gtfjwracsb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.shuidangran.top/gtpuipnmpm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.chenlongwang.top/gtwgsowvqp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.tanke756.top/gtkklztgow.html

[I05] 按正则拆分
来源：http://hz.yangfankeji.com/gtkiqicpbs.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.pengpengdd.cyou/gtnxazqetn.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.meibo888.top/gtvgyddkhh.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jinqigufen.top/gtsxwhibua.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.birdmap.top/gtcxcbklsj.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shanyushiyangkeji.top/gtdibueeyy.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hongshengwenyu.top/gtfhjcrcfd.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.tianlin.xyz/gteiqxfuuz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.hongshengwenyu.top/gtckcwbquw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.9152youxi.cn/gtqtdcqduc.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jiagoushi.top/gtospnqoke.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jqgufenzy.top/gtyfrzncvl.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgfzy.top/gtmihysjmw.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.pycfn.com/gtmietazjg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhongyouzk.top/gtltoeairh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jlsjyb.cn/gtsrwbyepd.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.daria6918.cn/gtdrjczbzi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zhiwuduotai.top/gtvulsytal.html

[I07] 忽略大小写与多行模式
来源：http://hz.xuanzx.com/gtahecmluf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.iojbl.cn/gtbhclngeg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.tianlin.xyz/gtxtojukso.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yangfankeji.com/gtqsjatgco.html

TS:   /error/gim
来源：http://hz.aizwys.cn/gtgcrcakxi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.feifeiyinyue.top/gtgactbqjx.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.cdnleiting.top/gtajjsloqb.html

Ruby: s.scan(/error/i)
来源：http://hz.fzhhl.top/gtzypgmmnt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sysykeji.top/gtsalucboj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.pengpengdd.cyou/gtolhkvquy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.chenzaomai.com/gtqibdoszb.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hysaishi.cn/gtgnmzfckj.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cucudq.cn/gtnhtenmht.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ydjk.org.cn/gtingwdtnx.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.xinyue.icu/gtucipouzg.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jinyuanbaomall.cn/gtghwcdytw.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ywan-chungtsiang.top/gtihmbznhz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.quarkkingdee.top/gtkbgllwsv.html

================================================================================
来源：http://hz.vqdsnc.cn/gtfvbkjzll.html

J. 日期与时间
来源：http://hz.cucudq.cn/gthxzpejdo.html

================================================================================
来源：http://hz.ybcxt.top/gtobydyhoc.html

[J01] 获取当前时间
来源：http://hz.andypj.xyz/gtyghintcl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.dashuyun.cn/gtyswteggf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.sxryk.cn/gtgalcjutr.html

JS:   new Date();  Date.now()
来源：http://hz.9152youxi.cn/gtrvdqenfy.html

TS:   new Date();  Date.now()
来源：http://hz.xuetiantiany.cn/gtntzfpzbr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.redwolf501.top/gtlllzaixt.html

Go:   time.Now()
来源：http://hz.dashuyun.cn/gtfsvohmih.html

Ruby: Time.now
来源：http://hz.yuxming.cn/gtxgtoatct.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zhoulong.xyz/gtigudgjid.html

[J02] 格式化输出
来源：http://hz.yonumen.top/gtwjvzztfw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.quarkkingdee.top/gtkkzipzst.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.chenjidiqi.icu/gtzkgdrjep.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shangyingyoupin.top/gtxwycssgl.html

TS:   d.toISOString()
来源：http://hz.shanyushiyangkeji.top/gtzdepklis.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ppjwa.cn/gtykjbngrb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ywan-chungtsiang.top/gtawubegcf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ywan-chungtsiang.top/gtvumdzqqs.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.smart0.xyz/gtkvnyfjqh.html

[J03] 字符串解析为日期
来源：http://hz.hongshengwenyu.top/gtzyycmsqq.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.c1oappe.top/gtuvkpjnuf.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.mhx1999.top/gtwwmwryxl.html

JS:   new Date("2024-01-02")
来源：http://hz.hongshengwenyu.top/gttcmxnjff.html

TS:   new Date("2024-01-02")
来源：http://hz.nwbrower.top/gthwqxnauk.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.guannengcc.top/gtvobrszea.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhongyouzk.top/gtleyqgmeo.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.wangdashe.top/gtygojqogx.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.shanyushiyangtech.top/gthudvjfix.html

[J04] 时间戳与日期互转
来源：http://hz.pycfn.com/gtdodwdhlb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shangyingyoupin.top/gtofhlijfq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.wangdashe.top/gtypfweueb.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.pengpengdd.cyou/gtgjsvxtfh.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sufxvd.cn/gtzveqogcw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jinghuilouyu.cn/gtrykfplzw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.c1oappe.top/gtqlzscfqj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.daxiang520.top/gtraxbqytz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.pycfn.com/gtalyowcve.html

[J05] 时间加减（加 7 天）
来源：http://hz.gotoacloud.top/gtxdrrwvwb.html

Py:   now + timedelta(days=7)
来源：http://hz.ydjk.org.cn/gtacmwqycd.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yongpay.top/gtnkwmjwze.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gaohongyu789.top/gtaufpxibm.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yj20258888.top/gtkooskzvm.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.0kj1m.cn/gtqrivpvep.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cucudq.cn/gtrxpnpqmy.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hnqzz.top/gtbnxezzye.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.shangyingyoupin.top/gtznancejm.html

[J06] 计算两时间之差
来源：http://hz.kuanghao11.cn/gthxjvhhvz.html

Py:   (end - start).total_seconds()
来源：http://hz.yj202588.top/gtzmqdcggj.html

PHP:  $end->diff($start)->days;
来源：http://hz.guannengcc.top/gttkttbkrv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jinyuanbaomall.cn/gtrpxanazh.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yanxiufei.cn/gtejgimldp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shanyushiyangkeji.top/gtifdshfoh.html

Go:   end.Sub(start).Hours()
来源：http://hz.snrcjt.cn/gtcpujcroy.html

Ruby: end - start                 # 返回秒数
来源：http://hz.daria6918.cn/gtlbjeubqt.html

C#:   (end - start).TotalSeconds
来源：http://hz.yuxming.cn/gtjjlwtkfj.html

[J07] 比较两个日期
来源：http://hz.ydzc1.top/gtrwmaltxh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.daria6918.cn/gtyalplwvk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.tian-w.cn/gtmeizckjn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258888.top/gtisewciva.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj202588.top/gtazunksaq.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cashguo.top/gtklxcepiz.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.nanxinkj.top/gtixjfyywb.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.chenlongwang.top/gtuetlnqtt.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtfjtaqgwa.html

[J08] 提取年月日与星期
来源：http://hz.zhengqikj.top/gtocdcgmvj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jqgufenzy.top/gtdjwgmqym.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.52xcode.cn/gtngnttowp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ydjk.org.cn/gtrkhleumt.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.nanxinkj.top/gtjoutzlzk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.sxryk.cn/gtmswhlkzq.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shanyushiyangtech.top/gtncyxcvvx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jqgfzy.top/gtavxutjbj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.bjfxy.top/gtekdmxamm.html

[J09] 时区处理
来源：http://hz.birdmap.top/gtdsywllvu.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.vqdsnc.cn/gtgnerswao.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.cheryme.top/gtezdcvbpf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhiwuduotai.top/gtogcfcuky.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.dianchejie.cn/gtiqlzfotn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.havefunace.top/gtbuybvjfs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cucudq.cn/gtinmhhzbd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yvedp.cn/gthfjihyyr.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ydzc1.top/gthkszryhi.html

[J10] 取今天 / 本月第一天
来源：http://hz.vqdsnc.cn/gtpekxobut.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.daxiang520.top/gtziiczjmb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.haohaochexian.top/gtpnymbzhr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.snrcjt.cn/gtkdacfweu.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zhongyouzk.top/gteosjuemg.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.52xcode.cn/gtqhwylaiw.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.jinyuanbaomall.cn/gtgxotxjmy.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.redwolf501.top/gturvqjcgu.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.havefunace.top/gtbwyvinfa.html

================================================================================
来源：http://hz.52xcode.cn/gtjsypagao.html

K. JSON 与序列化
来源：http://hz.gogol.net.cn/gtkwhhqflr.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtrwnckqle.html

[K01] 对象转 JSON 字符串
来源：http://hz.dashuyun.cn/gtzdsgzlua.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.zhoulong.xyz/gtsvahcmuu.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinghuilouyu.cn/gtoloizpsg.html

JS:   JSON.stringify(obj)
来源：http://hz.smart0.xyz/gtasszdowq.html

TS:   JSON.stringify(obj)
来源：http://hz.jinghuilouyu.cn/gtvlwpwhdc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.jinqigfzy.top/gtfmugojdc.html

Go:   json.Marshal(obj)
来源：http://hz.hfpthk.cn/gttlbsnddc.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.sxryk.cn/gtorcuuuzo.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.snrcjt.cn/gtqbkffplq.html

[K02] JSON 字符串转对象
来源：http://hz.shzxlz.cn/gtrfiphteb.html

Py:   json.loads(s)
来源：http://hz.yuanzhike.top/gtgwwcpfdp.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yj20258.top/gtlpqikqaw.html

JS:   JSON.parse(s)
来源：http://hz.yuanzhike.top/gtzxxvrklt.html

TS:   JSON.parse(s)
来源：http://hz.ybcxt.top/gtiemjuyvk.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.wangshuangyany.cn/gtbixcrulh.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.vqdsnc.cn/gtzscespdh.html

Ruby: JSON.parse(s)
来源：http://hz.jqgufenzy.top/gtcxanzunm.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.yanxiufei.cn/gtxerzdnln.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.tanke756.top/gtqwucjwmj.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.quarkkingdee.top/gtkvljrrpp.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.cucudq.cn/gtqxytcpkq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.aibaodan.cn/gtgllfgmwr.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.zdqjudy.top/gtjedeqyyu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.nanxinkj.top/gthyxnyxfp.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.xuanzx.com/gtebvsfbck.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.meibo888.top/gtzomauszv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.shuidangran.top/gtvspbmdmi.html

[K04] 读取 JSON 文件
来源：http://hz.jinqigfzy.top/gtvyuymfzi.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.nwbrower.top/gtmxrcbuwh.html


<!-- 参考信息 -->