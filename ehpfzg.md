代发 wailian999

PHP:  get_object_vars($obj);
来源：http://hz.xziqi.cn/gtkyqkfmwm.html

JS:   Object.entries(obj)
来源：http://hz.zdqjudy.top/gtghyvmubv.html

TS:   Object.entries(obj)
来源：http://hz.sxryk.cn/gtdkirgdnv.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jlsjyb.cn/gtjhzphrwf.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yongpay.top/gtjqwfwtpw.html

Ruby: obj.instance_variables
来源：http://hz.xuetiantiany.cn/gtfiooygvq.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.tian-w.cn/gtoubzaaqk.html

================================================================================
来源：http://hz.haohaochexian.top/gtyilsjvnm.html

H. 异常与错误处理
来源：http://hz.yonumen.top/gtgrtgzmnp.html

================================================================================
来源：http://hz.aibaodan.cn/gtsepjtoyh.html

[H01] try / catch 基础
来源：http://hz.52xcode.cn/gtgpwjsgsz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.tanke756.top/gthftdtqvy.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.jyoumei.cn/gtpeedpbvm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhixingplan.top/gtachvojeq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ydjk.org.cn/gtmurememp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ywan-chungtsiang.top/gtljisezdd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.dashuyun.cn/gtsexsiuah.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.andypj.xyz/gtvtjrpiws.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shzxlz.cn/gtizjneeid.html

[H02] finally / ensure 收尾
来源：http://hz.wangshuangyany.cn/gtiwookrpe.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.dianchejie.cn/gtmnmyioog.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jinyuanbaomall.cn/gtocyhfkds.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gtppdvlsim.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.sweek.top/gtfdszgdbp.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ydjk.org.cn/gtqpglejni.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinqigufen.top/gtjiqrodbq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.tian-w.cn/gtapdwuznf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cucudq.cn/gtluopmwyq.html

[H03] 主动抛出异常
来源：http://hz.bjfxy.top/gtksixeyqe.html

Py:   raise ValueError("错误信息")
来源：http://hz.316326.xyz/gtilmenspl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.hywenlv.cn/gtxhhusnfh.html

JS:   throw new Error("错误信息");
来源：http://hz.hysaishi.cn/gtdahmjisc.html

TS:   throw new Error("错误信息");
来源：http://hz.ydzc1.top/gtksffbqcv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jyoumei.cn/gtilnvhzes.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.fengsongda.top/gtgqgpbqwa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.sysykeji.top/gteyfxujpu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jqgufenzy.top/gtspkbavbo.html

[H04] 自定义异常类型
来源：http://hz.ivvv.top/gtghfajakc.html

Py:   class MyError(Exception): pass
来源：http://hz.guowangkeji.top/gtsncxphaq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.ppjwa.cn/gtmkgtcwnv.html

JS:   class MyError extends Error {}
来源：http://hz.guannengcc.top/gtfklfxhcs.html

TS:   class MyError extends Error {}
来源：http://hz.quarkkingdee.top/gtnkczfvua.html

Java: class MyException extends RuntimeException {}
来源：http://hz.aizwys.cn/gtfqrtduky.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shzxlz.cn/gtgmvijdfc.html

Ruby: class MyError < StandardError; end
来源：http://hz.xingfuxueyuan.xyz/gtkkekfwqc.html

C#:   class MyException : Exception {}
来源：http://hz.yueranfly.top/gtfacaylep.html

[H05] 捕获特定类型
来源：http://hz.ydjk.org.cn/gtnkgkbvja.html

Py:   except ValueError as e:
来源：http://hz.gotoacloud.top/gtysllhhum.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xuanzx.com/gtavjudssg.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cucudq.cn/gtrimymbmw.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.shangyingyoupin.top/gtyvzhirvo.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.redwolf501.top/gthvmgmklp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.iojbl.cn/gtphmsswzq.html

Ruby: rescue ArgumentError => e
来源：http://hz.xylfe.cn/gtyygvoodi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sysykeji.top/gthqssnhsn.html

[H06] 可选值 / 空值安全访问
来源：http://hz.svipenyu.cn/gtstgzupsa.html

Py:   value = d.get("k") or default
来源：http://hz.yueranfly.top/gtfigehpzi.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.chenjidiqi.icu/gtfevdlchg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xuetiantiany.cn/gtujjyynoi.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zycfv.cn/gtyixmmrrl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.316326.xyz/gtrvlohqqa.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhixingplan.top/gtkjpjwqke.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zdqjudy.top/gthesxexxg.html

C#:   obj?.A?.B ?? default
来源：http://hz.sxryk.cn/gtxzfgkirn.html

[H07] 断言
来源：http://hz.shanyushiyangkeji.top/gtanlyqgho.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zycfv.cn/gtgsyzhggt.html

PHP:  assert($x > 0);
来源：http://hz.ppjwa.cn/gtmwjdymey.html

JS:   console.assert(x > 0);
来源：http://hz.tanke756.top/gttebrchwo.html

TS:   console.assert(x > 0);
来源：http://hz.nwbrower.top/gtsovvwvyx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.mhx1999.top/gtndbrxdvb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yuanzhike.top/gttsvgyzed.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hywenlv.cn/gttvvtrchy.html

C#:   Debug.Assert(x > 0);
来源：http://hz.9152youxi.cn/gtxhavoukk.html

[H08] 获取错误信息与堆栈
来源：http://hz.ppjwa.cn/gteivymmos.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ydzc1.top/gtyejxabch.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinghuilouyu.cn/gtnnyhlqif.html

JS:   e.message;  e.stack
来源：http://hz.9152youxi.cn/gtgpyzgfiu.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.pengpengdd.cyou/gtwsxeljgo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.wangshuangyany.cn/gtssdeeitc.html

Go:   err.Error()
来源：http://hz.hnxiangtu.top/gtphrundub.html

Ruby: e.message;  e.backtrace
来源：http://hz.wangdashe.top/gtulsonksh.html

C#:   e.Message;  e.StackTrace
来源：http://hz.chenzaomai.com/gthrlzrmyb.html

[H09] 带错误码的异常
来源：http://hz.aibaodan.cn/gtofayrhtp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.smart0.xyz/gtkzcaxdgo.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jlsjyb.cn/gtzwmdxuci.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhongyouzk.top/gtsedanigv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhongyouzk.top/gtnurjcxzg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.dashuyun.cn/gtejhkwmlu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.birdmap.top/gttdcbdodj.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cucudq.cn/gtceikoouv.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ywan-chungtsiang.top/gtzvbmnupi.html

[H10] 资源自动释放
来源：http://hz.shangyingyoupin.top/gtepwyifln.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jiagoushi.top/gtpjooctoc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.cqqwz.cn/gtcxafkqhv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hnxiangtu.top/gtzyzaolpl.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xinyue.icu/gtoblesops.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.chenzaomai.com/gtovkthedk.html

Go:   defer f.Close()
来源：http://hz.andypj.xyz/gtxptjyzag.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shanyushiyangtech.top/gtnhujntwn.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ydzc1.top/gtnneoxvcu.html

================================================================================
来源：http://hz.pycfn.com/gtyrpmoqdt.html

I. 正则表达式
来源：http://hz.iojbl.cn/gtkwmpnmrz.html

================================================================================
来源：http://hz.jiagoushi.top/gtbxdlrqst.html

[I01] 判断是否匹配
来源：http://hz.yanxiufei.cn/gtupeumhyq.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hnxiangtu.top/gtnjilmsgy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.daxiang520.top/gtsopyqrru.html

JS:   /\d+/.test(s)
来源：http://hz.yj202588.top/gtjyrklndp.html

TS:   /\d+/.test(s)
来源：http://hz.xziqi.cn/gtomltqsrt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jyoumei.cn/gtvhmgwdcx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.c1oappe.top/gtkiqqkosr.html

Ruby: s.match?(/\d+/)
来源：http://hz.zycfv.cn/gtquvrwpmh.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.smart0.xyz/gthuolkxts.html

[I02] 提取所有匹配
来源：http://hz.sysykeji.top/gtnwgnobce.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yuxming.cn/gtcxwduumo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yuxming.cn/gtsbjwgiql.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.haohaochexian.top/gtxxywimft.html

TS:   s.match(/\d+/g)
来源：http://hz.jinqigufen.top/gtcclziaxw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cashguo.top/gtodewquol.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yonumen.top/gtlglandiy.html

Ruby: s.scan(/\d+/)
来源：http://hz.xuetiantiany.cn/gtbtlbffif.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.andypj.xyz/gtcfxyzewk.html

[I03] 提取捕获分组
来源：http://hz.cucudq.cn/gthwqhcyry.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jinqigufen.top/gttkaotgje.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hfpthk.cn/gtfbtehnna.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.cucudq.cn/gtpjaexmuy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.gaohongyu789.top/gtrccvpjwy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shuidangran.top/gtcdmkqurg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ybcxt.top/gtwnfwlngh.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.guannengcc.top/gtyqqdsaas.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.hammf.cn/gtukrlklxq.html

[I04] 正则替换
来源：http://hz.c1oappe.top/gteoyaxnfc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shangyingyoupin.top/gtxkczxsjh.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zdqjudy.top/gtbahbwrla.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgufenzy.top/gtiohsqakg.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.hammf.cn/gtbhpjrodb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.redwolf501.top/gtcdboflpy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yueranfly.top/gtnrpdsxwz.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.316326.xyz/gtagpntuwa.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.daria6918.cn/gtaprxywfi.html

[I05] 按正则拆分
来源：http://hz.tianlin.xyz/gtapthpdct.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cucudq.cn/gtviejxafh.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yangfankeji.com/gtnrubuvej.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hysaishi.cn/gtowqgljjl.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sufxvd.cn/gtmyntlyql.html

Java: s.split("\\s*,\\s*")
来源：http://hz.svipenyu.cn/gtfuifpsye.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.tanke756.top/gtolephibr.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yueranfly.top/gtwssbckko.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gogol.net.cn/gtskqgfypk.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jiagoushi.top/gtlvtspibp.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.daxiang520.top/gtmkkxcxvf.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.ivvv.top/gtsukbxgwi.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yanxiufei.cn/gtvvqtziiz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhoulong.xyz/gtgvawirpq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.gaohongyu789.top/gtglbzfljy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gogol.net.cn/gtsjcfgkwi.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jqgfzy.top/gtctauvihu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.dianchejie.cn/gtekmelcwf.html

[I07] 忽略大小写与多行模式
来源：http://hz.yangfankeji.com/gtqugchrfq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.dianchejie.cn/gthlloicoo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.iojbl.cn/gtrvqmbqwm.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yj202588.top/gtsecebjyo.html

TS:   /error/gim
来源：http://hz.gotoacloud.top/gtcywyxyuj.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhongyouzk.top/gtyglotodn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.birdmap.top/gtdwwhttak.html

Ruby: s.scan(/error/i)
来源：http://hz.sysykeji.top/gtnnolnehi.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.nanxinkj.top/gttpiztacm.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yj202588.top/gtcqngnddj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.vqdsnc.cn/gtnhflubmp.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hysaishi.cn/gtencddgbx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hnxiangtu.top/gtyqaaybhh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aizwys.cn/gthqidyzhb.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.fengsongda.top/gtsjdrfnjy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gotoacloud.top/gtxxkqamyg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zycfv.cn/gtqyjnfcpq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yueranfly.top/gtvdythofk.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtwkcqebwc.html

J. 日期与时间
来源：http://hz.smart0.xyz/gtiqnpdadk.html

================================================================================
来源：http://hz.daxiang520.top/gtjlznavhv.html

[J01] 获取当前时间
来源：http://hz.quarkkingdee.top/gtjebhusan.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenzaomai.com/gtolfkhxsr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yangfankeji.com/gtatiounxk.html

JS:   new Date();  Date.now()
来源：http://hz.kuanghao11.cn/gtmmmvkuee.html

TS:   new Date();  Date.now()
来源：http://hz.cheryme.top/gtxztzjwzq.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cucudq.cn/gtvlvssxbt.html

Go:   time.Now()
来源：http://hz.zhaomingkeji.xyz/gtmiykxasl.html

Ruby: Time.now
来源：http://hz.jinqigfzy.top/gtxjbbuarh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.xuanzx.com/gtqynobjjh.html

[J02] 格式化输出
来源：http://hz.iojbl.cn/gtztaaardr.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.smart0.xyz/gtlclntdnr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jqgufenzy.top/gtgoqjygkx.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yuxming.cn/gtvniyixsh.html

TS:   d.toISOString()
来源：http://hz.sweek.top/gtzoabtaxk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.hywenlv.cn/gtrwcxynrp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yongpay.top/gtjrbfjfpi.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.ydjk.org.cn/gtupckokwn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.chenzaomai.com/gtajgpwait.html

[J03] 字符串解析为日期
来源：http://hz.shanyushiyangkeji.top/gtwalyjzxi.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yuanzhike.top/gtsrmeiqdd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.tanke756.top/gtoklqcdpo.html

JS:   new Date("2024-01-02")
来源：http://hz.gogol.net.cn/gtyjpsuepy.html

TS:   new Date("2024-01-02")
来源：http://hz.jinqigufen.top/gtufdxiyay.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.nanxinkj.top/gtnplfupyb.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.andypj.xyz/gthvwvzvma.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hammf.cn/gtgetryesh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.xinyue.icu/gtpcwlkxjk.html

[J04] 时间戳与日期互转
来源：http://hz.meibo888.top/gtzvfrksnl.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.chenzaomai.com/gtwohfafhh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yj20258888.top/gtmvuebmvk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.aibaodan.cn/gtpdlrsmdp.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hammf.cn/gtikrklnoy.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.iojbl.cn/gttunpnzyq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.andypj.xyz/gtoaoafrve.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.fzhhl.top/gtzcaccyne.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.9152youxi.cn/gttldkipgm.html

[J05] 时间加减（加 7 天）
来源：http://hz.cdnleiting.top/gthgclrkko.html

Py:   now + timedelta(days=7)
来源：http://hz.jinyuanbaomall.cn/gtqzlybilf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cheryme.top/gtlhtwtsgl.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zdqjudy.top/gtyekmbvsv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cdnleiting.top/gtewabjfcp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhongyouzk.top/gtmkgynfnf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hfpthk.cn/gtfywdlbit.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shangyingyoupin.top/gtpmikebbj.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yj20258888.top/gtyvjkjznz.html

[J06] 计算两时间之差
来源：http://hz.tianlin.xyz/gtxuelnpla.html

Py:   (end - start).total_seconds()
来源：http://hz.feifeiyinyue.top/gthsljhyoq.html

PHP:  $end->diff($start)->days;
来源：http://hz.chenjidiqi.icu/gthhopmhpz.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.chenzaomai.com/gtiivpqcpq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.daria6918.cn/gtrlcxdwnr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yj20258.top/gtrxcottej.html

Go:   end.Sub(start).Hours()
来源：http://hz.jqgfzy.top/gtwzgpajco.html

Ruby: end - start                 # 返回秒数
来源：http://hz.wangdashe.top/gtrycqlsnn.html

C#:   (end - start).TotalSeconds
来源：http://hz.nanxinkj.top/gtfoylvbzh.html

[J07] 比较两个日期
来源：http://hz.yanxiufei.cn/gtjohvnwbh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xingfuxueyuan.xyz/gtgbtabsxt.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.shangyingyoupin.top/gtyplcjpfo.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cheryme.top/gtcfhdcdxf.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yuanzhike.top/gtaxxzskvx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yj20258.top/gtrcwvarnh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yj20258888.top/gtvzgotxng.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cashguo.top/gthvzpizgx.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cqqwz.cn/gtanxywdfz.html

[J08] 提取年月日与星期
来源：http://hz.bjfxy.top/gtuzjmioeu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhengqikj.top/gtjaffmyaz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.kuanghao11.cn/gtullpegiy.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sufxvd.cn/gtjmfgwtkj.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.birdmap.top/gtftrjqgrt.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hnxiangtu.top/gtoanutvdf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.guannengcc.top/gtfnczrpnc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.dianchejie.cn/gtdwetkger.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sxryk.cn/gtmuqfwhhh.html

[J09] 时区处理
来源：http://hz.yanxiufei.cn/gtjfdcstwy.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shzxlz.cn/gtrqtweego.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.316326.xyz/gtyaomdwfh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhongyouzk.top/gtbldzhvoz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuxming.cn/gtlwtbrijg.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.guowangkeji.top/gtpphbcvlb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.chenjidiqi.icu/gtzthhcmqs.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.pengpengdd.cyou/gtstnpdjif.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.aizwys.cn/gtfyayfkjw.html

[J10] 取今天 / 本月第一天
来源：http://hz.cqqwz.cn/gtbnjyaiqd.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.chenzaomai.com/gtozgzxypf.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.daria6918.cn/gtdtqsfchl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.chenlongwang.top/gtfbvxhqyc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.meibo888.top/gtgvlsapbb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.pycfn.com/gtfnnkglxv.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.quarkkingdee.top/gtpinxtkoe.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yj202588.top/gttnmmqhft.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.zhengqikj.top/gtvtbmioqo.html

================================================================================
来源：http://hz.ppjwa.cn/gteolrtjuk.html

K. JSON 与序列化
来源：http://hz.sweek.top/gtvuiipvnr.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtrqvkcypf.html

[K01] 对象转 JSON 字符串
来源：http://hz.hfpthk.cn/gtktbeuwkh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.0kj1m.cn/gtulilkkdg.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.chenjidiqi.icu/gtsaxwdxyd.html

JS:   JSON.stringify(obj)
来源：http://hz.mhx1999.top/gtjeuwgsgx.html

TS:   JSON.stringify(obj)
来源：http://hz.aibaodan.cn/gtrnnmokxt.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.wangdashe.top/gtnrpjirmh.html

Go:   json.Marshal(obj)
来源：http://hz.yueranfly.top/gtiusjeepl.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zhijiandao.cn/gtxconkjai.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.sufxvd.cn/gtujquvqsq.html

[K02] JSON 字符串转对象
来源：http://hz.nwbrower.top/gteuueyngl.html

Py:   json.loads(s)
来源：http://hz.ywan-chungtsiang.top/gtedqlwrea.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.ydjk.org.cn/gtqgyavrhe.html

JS:   JSON.parse(s)
来源：http://hz.xziqi.cn/gtugoxmcwq.html

TS:   JSON.parse(s)
来源：http://hz.jqgufenzy.top/gteffsyfjz.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.zycfv.cn/gtnbskjaqx.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.c1oappe.top/gtzjadctyz.html

Ruby: JSON.parse(s)
来源：http://hz.xylfe.cn/gtgahzhxdo.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.zhengqikj.top/gtqocupwyu.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.fengsongda.top/gtwxzerqym.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.iojbl.cn/gtpdqiglbm.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.zycfv.cn/gtjuyokwyq.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.pycfn.com/gtpaaugkrs.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.ydjk.org.cn/gtjvfsatyv.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.jinqigufen.top/gtozbwhjni.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.hnxiangtu.top/gtltztayhs.html

Ruby: JSON.pretty_generate(obj)
来源：http://hz.shangyingyoupin.top/gtpzbierun.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hz.yj20258888.top/gteavaisls.html

[K04] 读取 JSON 文件
来源：http://hz.sweek.top/gtuyejdsga.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hz.hnqzz.top/gtgdihjdzv.html


<!-- 参考信息 -->