代发 wailian999

H. 异常与错误处理
来源：http://hz.316326.xyz/gtvzhblofo.html

================================================================================
来源：http://hz.316326.xyz/gtrdqpyilg.html

[H01] try / catch 基础
来源：http://hz.nanxuanxn.top/gtusjfswdx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jlsjyb.cn/gtrzkyjaag.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.iojbl.cn/gtqzngxafz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.ppjwa.cn/gtbghifsac.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.cqqwz.cn/gtckrylyzq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhaomingkeji.xyz/gtvjdruyzj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.quarkkingdee.top/gtlwhamnwl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.nanxinkj.top/gtvbflbttv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cashguo.top/gtsgctivvp.html

[H02] finally / ensure 收尾
来源：http://hz.xuetiantiany.cn/gtunmzsanh.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yanxiufei.cn/gtguznqbsr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtqajpgyab.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zdqjudy.top/gtzhkqqehg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gtdyiwcqwm.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cucudq.cn/gttpiwnfxt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.daria6918.cn/gtmjumeqbx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.feifeiyinyue.top/gttxsjhbxx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.mhx1999.top/gtplluvfas.html

[H03] 主动抛出异常
来源：http://hz.zycfv.cn/gtflkmgxjj.html

Py:   raise ValueError("错误信息")
来源：http://hz.kuanghao11.cn/gtyfczblyd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ehwqpu.com/gtkrerhqvc.html

JS:   throw new Error("错误信息");
来源：http://hz.yvedp.cn/gtzpzqaokr.html

TS:   throw new Error("错误信息");
来源：http://hz.cqqwz.cn/gtqxkcqtji.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.mhx1999.top/gtiadhxzcg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xylfe.cn/gtitokdkna.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ybcxt.top/gtpoasffgf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jinghuilouyu.cn/gtsfjcppaq.html

[H04] 自定义异常类型
来源：http://hz.hfpthk.cn/gtpjndtipv.html

Py:   class MyError(Exception): pass
来源：http://hz.ivvv.top/gtbzwuwdvn.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jinqigfzy.top/gtiuvsfcow.html

JS:   class MyError extends Error {}
来源：http://hz.dianchejie.cn/gthdzzfozj.html

TS:   class MyError extends Error {}
来源：http://hz.jinghuilouyu.cn/gtczljdmwn.html

Java: class MyException extends RuntimeException {}
来源：http://hz.redwolf501.top/gtmmiepnwv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.daria6918.cn/gtllzrhwis.html

Ruby: class MyError < StandardError; end
来源：http://hz.ehwqpu.com/gtnaztmwks.html

C#:   class MyException : Exception {}
来源：http://hz.tian-w.cn/gtlgzqvvjc.html

[H05] 捕获特定类型
来源：http://hz.yueranfly.top/gtifphvbxy.html

Py:   except ValueError as e:
来源：http://hz.cashguo.top/gtxvzdmkgo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yuxming.cn/gtnokfswjf.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.wangshuangyany.cn/gtezjyujvr.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yueranfly.top/gtohvfawqw.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.cheryme.top/gttcktevqx.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hywenlv.cn/gtbzemnhnw.html

Ruby: rescue ArgumentError => e
来源：http://hz.hongshengwenyu.top/gtvmevqhat.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.chenzaomai.com/gtejjrjnin.html

[H06] 可选值 / 空值安全访问
来源：http://hz.guannengcc.top/gtisdnxngv.html

Py:   value = d.get("k") or default
来源：http://hz.jqgufenzy.top/gtsgafgdjl.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.wangdashe.top/gtxjbefkhg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sweek.top/gtynekqgjr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.shuidangran.top/gtxahlwlwk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.c1oappe.top/gtkjsnukoz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.meibo888.top/gtjnezromm.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yvedp.cn/gtpizqwfia.html

C#:   obj?.A?.B ?? default
来源：http://hz.shangyingyoupin.top/gtgpwmicer.html

[H07] 断言
来源：http://hz.9152youxi.cn/gtpzeemrsg.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sufxvd.cn/gtxkbkvbet.html

PHP:  assert($x > 0);
来源：http://hz.jinghuilouyu.cn/gtmsxbuxcy.html

JS:   console.assert(x > 0);
来源：http://hz.zhixingplan.top/gtaenhuypk.html

TS:   console.assert(x > 0);
来源：http://hz.cqqwz.cn/gtyunwnzwr.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shangyingyoupin.top/gtcrygavct.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xylfe.cn/gtgswelmec.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ydzc1.top/gtdmsreexp.html

C#:   Debug.Assert(x > 0);
来源：http://hz.hysaishi.cn/gtkeejwoad.html

[H08] 获取错误信息与堆栈
来源：http://hz.jinghuilouyu.cn/gtaqvxqkrk.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jianghu66.top/gtaibeammx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yonumen.top/gtgqtqjkrn.html

JS:   e.message;  e.stack
来源：http://hz.shanyushiyangtech.top/gtvmmswmkj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.nanxuanxn.top/gtcrqaqogb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.shzxlz.cn/gtxrhbpidh.html

Go:   err.Error()
来源：http://hz.jyoumei.cn/gthigtkorr.html

Ruby: e.message;  e.backtrace
来源：http://hz.yj202588.top/gtgflssdtn.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tianlin.xyz/gtsdqqogyc.html

[H09] 带错误码的异常
来源：http://hz.gogol.net.cn/gtujxicmjt.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.cqqwz.cn/gtrqivknuv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yongpay.top/gtldrnkxew.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yj202588.top/gtbpzdwscc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.nanxuanxn.top/gtajwpnavz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hfpthk.cn/gtalcezmqh.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhijiandao.cn/gtkknstyov.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hnqzz.top/gtbdzmhizk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.iojbl.cn/gtqyqogydv.html

[H10] 资源自动释放
来源：http://hz.smart0.xyz/gtzztvweup.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yongpay.top/gtbybsekmf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.tian-w.cn/gtdhdcuzxb.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.smart0.xyz/gtavxvzuob.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.0kj1m.cn/gtijuudqkj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xziqi.cn/gtopoulzwp.html

Go:   defer f.Close()
来源：http://hz.zycfv.cn/gtiugzuwrq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.xuanzx.com/gtgxxddqnx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.nwbrower.top/gttddbribg.html

================================================================================
来源：http://hz.tanke756.top/gtmxxadwcq.html

I. 正则表达式
来源：http://hz.ydjk.org.cn/gtmsznmxmq.html

================================================================================
来源：http://hz.nanxuanxn.top/gtxuxfyqqh.html

[I01] 判断是否匹配
来源：http://hz.yj20258888.top/gtodofyief.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jinqigfzy.top/gtdvrbcprr.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.mhx1999.top/gtazamncqr.html

JS:   /\d+/.test(s)
来源：http://hz.tianlin.xyz/gtygzpwkqt.html

TS:   /\d+/.test(s)
来源：http://hz.jqgfzy.top/gtdyubaqbf.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.birdmap.top/gtrgmtccso.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yanxiufei.cn/gtctaifwuw.html

Ruby: s.match?(/\d+/)
来源：http://hz.ivvv.top/gtspxggofi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.zhiwuduotai.top/gttofxfjdg.html

[I02] 提取所有匹配
来源：http://hz.nanxuanxn.top/gtfkqftmdk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.daria6918.cn/gtmtkzxftn.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.hywenlv.cn/gtupkvrreo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.sufxvd.cn/gthgrjrxnh.html

TS:   s.match(/\d+/g)
来源：http://hz.yuxming.cn/gtweulfcpz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.shzxlz.cn/gtrijbvwqi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cucudq.cn/gtdasvdpjz.html

Ruby: s.scan(/\d+/)
来源：http://hz.yvedp.cn/gtkggihcfn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.wangshuangyany.cn/gtokxnrrmk.html

[I03] 提取捕获分组
来源：http://hz.jiagoushi.top/gtuctzjvvu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jqgfzy.top/gtjhctulmv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jqgfzy.top/gtsbygyfii.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.dianchejie.cn/gtpcrbgjxd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.0kj1m.cn/gtvkwkoypn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.52xcode.cn/gtrbjrezzf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.tian-w.cn/gtcxsoxagb.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhiwuduotai.top/gtmyqrzmui.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.mhx1999.top/gtmoqnbcnf.html

[I04] 正则替换
来源：http://hz.kuanghao11.cn/gtwhuyqnni.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.yj20258888.top/gtunxmlmnf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ydzc1.top/gtggrxgnou.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yuanzhike.top/gtpkfzfozx.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.xylfe.cn/gtmbrjafus.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.sysykeji.top/gthumjmiwk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.dashuyun.cn/gtxeypvtas.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shanyushiyangkeji.top/gtwiaounqp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ydzc1.top/gtajnbrilm.html

[I05] 按正则拆分
来源：http://hz.aibaodan.cn/gtkluerphd.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jqgufenzy.top/gtizyoykwr.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.feifeiyinyue.top/gtllhtteyn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhongyouzk.top/gtbghhwjii.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hammf.cn/gtnnymghfm.html

Java: s.split("\\s*,\\s*")
来源：http://hz.0kj1m.cn/gtswrckdgv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.tianlin.xyz/gtbxsuemta.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shanyushiyangtech.top/gtialsghqj.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.cheryme.top/gtlzyebynq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.pycfn.com/gthojabhvf.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hywenlv.cn/gtzcmrijou.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.daxiang520.top/gtzcpkurqw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.pengpengdd.cyou/gtmlgzvpyi.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fzhhl.top/gtwbxjglen.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.andypj.xyz/gthfxeyycp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.smart0.xyz/gtxzmuqhjw.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hongshengwenyu.top/gthpoevhyg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.nanxinkj.top/gtcybaigum.html

[I07] 忽略大小写与多行模式
来源：http://hz.guannengcc.top/gtvjpxombz.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.redwolf501.top/gtuazfbyjy.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.birdmap.top/gtovvticnh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.havefunace.top/gtefuavtxo.html

TS:   /error/gim
来源：http://hz.zhengqikj.top/gtuoruhokj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xuetiantiany.cn/gtwtvxwxoi.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.chenjidiqi.icu/gtkjbpqnni.html

Ruby: s.scan(/error/i)
来源：http://hz.hfpthk.cn/gtciymagzx.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xziqi.cn/gtbyaqmcoi.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cdnleiting.top/gtvewwbijy.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xuetiantiany.cn/gtfqkqwuwu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xingfuxueyuan.xyz/gtzlsjtdtw.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cucudq.cn/gtzcgdvkaf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tian-w.cn/gtqetsbzor.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.ydjk.org.cn/gtoqaeflkm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.wangshuangyany.cn/gtwodhsree.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.dianchejie.cn/gtqvazsofk.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.birdmap.top/gtexslyllr.html

================================================================================
来源：http://hz.ybcxt.top/gtrkwzqypm.html

J. 日期与时间
来源：http://hz.cdnleiting.top/gtnmzjogrj.html

================================================================================
来源：http://hz.yuxming.cn/gtxdrmqrze.html

[J01] 获取当前时间
来源：http://hz.cucudq.cn/gtjkhnrxvr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.ydjk.org.cn/gtrwkntdbx.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hywenlv.cn/gtgngyarzn.html

JS:   new Date();  Date.now()
来源：http://hz.ydjk.org.cn/gtoubjbvdv.html

TS:   new Date();  Date.now()
来源：http://hz.jinqigufen.top/gtgazkhtvb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.xylfe.cn/gtoglihhen.html

Go:   time.Now()
来源：http://hz.fzhhl.top/gtbyfiecjk.html

Ruby: Time.now
来源：http://hz.kuanghao11.cn/gtmhdbqhbi.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.dianchejie.cn/gtlcaycesh.html

[J02] 格式化输出
来源：http://hz.zhijiandao.cn/gtejakuxaf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.bjfxy.top/gteqekgflh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shangyingyoupin.top/gtrvdmmxaa.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xuanzx.com/gtmgcgmcou.html

TS:   d.toISOString()
来源：http://hz.shzxlz.cn/gthmazwlil.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yj202588.top/gtpwakdzqc.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.guannengcc.top/gtlvwuicnh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yvedp.cn/gtdfvakrod.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shangyingyoupin.top/gtmvggsbve.html

[J03] 字符串解析为日期
来源：http://hz.gotoacloud.top/gtnzpervwu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.pycfn.com/gtnplbfipd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.tanke756.top/gtynchiksw.html

JS:   new Date("2024-01-02")
来源：http://hz.chenzaomai.com/gtszazaxnz.html

TS:   new Date("2024-01-02")
来源：http://hz.gogol.net.cn/gtfrpdhoul.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.ivvv.top/gtyeckgovh.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.mhx1999.top/gtcvnvwlvk.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ppjwa.cn/gtnmdhdhku.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.zhixingplan.top/gtsarwhckl.html

[J04] 时间戳与日期互转
来源：http://hz.nwbrower.top/gtohbagoxp.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.dianchejie.cn/gtriqcpykj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhiwuduotai.top/gtbgerxggh.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yueranfly.top/gtxqycbuqy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hnxiangtu.top/gtyagdwiae.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.yangfankeji.com/gtpzluhuza.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yonumen.top/gtedvfxcqu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.jinqigufen.top/gtwyxxleun.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ydzc1.top/gtsiquimli.html

[J05] 时间加减（加 7 天）
来源：http://hz.smart0.xyz/gtnxwudbdo.html

Py:   now + timedelta(days=7)
来源：http://hz.dianchejie.cn/gtmcdbgkia.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ydzc1.top/gtqlxnjseg.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.svipenyu.cn/gtybunaawg.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinqigfzy.top/gtfqynwwvm.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cheryme.top/gtdnecttjq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hywenlv.cn/gtusyrfaiw.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yuanzhike.top/gtzalbhvop.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.52xcode.cn/gtlcnopcrz.html

[J06] 计算两时间之差
来源：http://hz.aibaodan.cn/gtqtqcaxmv.html

Py:   (end - start).total_seconds()
来源：http://hz.andypj.xyz/gtukgwnmgv.html

PHP:  $end->diff($start)->days;
来源：http://hz.wangdashe.top/gtgdymkqrc.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.sysykeji.top/gtflskwfgz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.yangfankeji.com/gtyapfinnc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hysaishi.cn/gtopfniluv.html

Go:   end.Sub(start).Hours()
来源：http://hz.hongshengwenyu.top/gtwszywmdo.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yvedp.cn/gtppwzqhxv.html

C#:   (end - start).TotalSeconds
来源：http://hz.sxryk.cn/gtsbqmfskm.html

[J07] 比较两个日期
来源：http://hz.zhixingplan.top/gtziqcpswe.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.wangshuangyany.cn/gtmzmplfek.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.yuxming.cn/gtvckgbjny.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.tanke756.top/gtorlnirse.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cucudq.cn/gtbdwhsnjl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xuetiantiany.cn/gtrsxochsp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sweek.top/gtxcjfqrko.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gtpowioims.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.sysykeji.top/gtwtnumwvx.html

[J08] 提取年月日与星期
来源：http://hz.hammf.cn/gtudmqnihe.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yonumen.top/gtxcwfzprv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.fengsongda.top/gtzieofcid.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yueranfly.top/gtnjprzoay.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.cdnleiting.top/gtkygdpygg.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.wangshuangyany.cn/gtlklaibiv.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cheryme.top/gtehceqidu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sxryk.cn/gtrjonyqyh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jianghu66.top/gtiqbnutke.html

[J09] 时区处理
来源：http://hz.vqdsnc.cn/gtquttkuua.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.tianlin.xyz/gthgtmbgru.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.9152youxi.cn/gtwiozzdqh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jqgfzy.top/gtnvgpuxey.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jinqigufen.top/gtaastavnt.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nwbrower.top/gtcbbboxui.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.nanxinkj.top/gtvhzdwktq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.fzhhl.top/gthcxtfwgz.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhoulong.xyz/gtzwrbuzhe.html

[J10] 取今天 / 本月第一天
来源：http://hz.jqgufenzy.top/gtyxhmafgz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.nwbrower.top/gttgxsldax.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xuanzx.com/gtgdrimdpl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yueranfly.top/gtjjlklede.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.vqdsnc.cn/gtttxqawyw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.gogol.net.cn/gtnmgowkoj.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yj20258.top/gtsgwustkw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ywan-chungtsiang.top/gtiqkdskmk.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.sxryk.cn/gtfvqpkpty.html

================================================================================
来源：http://hz.gotoacloud.top/gtgtiexrwf.html

K. JSON 与序列化
来源：http://hz.shuidangran.top/gtubinloyd.html

================================================================================
来源：http://hz.andypj.xyz/gtxbkzttvu.html

[K01] 对象转 JSON 字符串
来源：http://hz.yonumen.top/gtdxtsqwhj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.shanyushiyangtech.top/gtocxagxmz.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinyuanbaomall.cn/gtssqdgybt.html

JS:   JSON.stringify(obj)
来源：http://hz.redwolf501.top/gtpbygnokk.html

TS:   JSON.stringify(obj)
来源：http://hz.tanke756.top/gtqxmepqqp.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.shzxlz.cn/gtlgluczzo.html

Go:   json.Marshal(obj)
来源：http://hz.ybcxt.top/gtgjdpkfev.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.hysaishi.cn/gtgreqpftw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinqigufen.top/gtnzgfugtw.html

[K02] JSON 字符串转对象
来源：http://hz.jinqigufen.top/gtohqkdlbg.html

Py:   json.loads(s)
来源：http://hz.hnxiangtu.top/gtvnpfvzbc.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.meibo888.top/gtdpjsjgvz.html

JS:   JSON.parse(s)
来源：http://hz.svipenyu.cn/gtaehxhtpc.html

TS:   JSON.parse(s)
来源：http://hz.yonumen.top/gtbtaggnwh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.gzhubu.top/gtwghipvur.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.snrcjt.cn/gtlluvdpdq.html

Ruby: JSON.parse(s)
来源：http://hz.kuanghao11.cn/gteofwvbkh.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.meibo888.top/gtvqrwizib.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.ywan-chungtsiang.top/gtzjkmqssp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.zdqjudy.top/gtrwkowemj.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.yangfankeji.com/gtvkmozlqn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.wangshuangyany.cn/gtqhdbihea.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.xuetiantiany.cn/gtossukzps.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jiagoushi.top/gtwiavlurg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.feifeiyinyue.top/gtazuilhvo.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.dashuyun.cn/gtzjmworxs.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.nanxinkj.top/gtsttgndlb.html

[K04] 读取 JSON 文件
来源：http://hz.hywenlv.cn/gtvrqhqsnc.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.zhongyouzk.top/gtnzndaplv.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hz.cqqwz.cn/gtosgygsmu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.ybcxt.top/gtmvgxtgzc.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hz.yanxiufei.cn/gtjkpquwso.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hz.yuanzhike.top/gtsswusmqk.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hz.chenlongwang.top/gtbmexjanl.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://hz.chenlongwang.top/gtmnjnvvty.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://hz.feifeiyinyue.top/gtwodlqmgx.html

[K05] 深拷贝对象
来源：http://hz.yuxming.cn/gtuwuxjcoe.html


<!-- 参考信息 -->