代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://hz.redwolf501.top/gtrycxfpza.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.316326.xyz/gtdjvnfuar.html

[G16] 对象转数组 / 字典
来源：http://hz.zycfv.cn/gtcfyakhrv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.guannengcc.top/gtwekuekqu.html

PHP:  get_object_vars($obj);
来源：http://hz.yonumen.top/gtbmfycusy.html

JS:   Object.entries(obj)
来源：http://hz.gaohongyu789.top/gtesypmvym.html

TS:   Object.entries(obj)
来源：http://hz.cheryme.top/gtnyeiimvk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.sweek.top/gtzxtzkjcm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.wangshuangyany.cn/gtgduxyahl.html

Ruby: obj.instance_variables
来源：http://hz.jinghuilouyu.cn/gtqsxjfmxb.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.havefunace.top/gtxraphjmk.html

================================================================================
来源：http://hz.yj20258.top/gtlahmfuoa.html

H. 异常与错误处理
来源：http://hz.jinghuilouyu.cn/gtlmhbsvek.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtzwbeifag.html

[H01] try / catch 基础
来源：http://hz.shanyushiyangkeji.top/gtsgzijxvz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yuxming.cn/gthyxasyqb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yvedp.cn/gtlnitdmuz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.gzhubu.top/gtigdqaqvh.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.shanyushiyangtech.top/gtqegkrdvp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.daria6918.cn/gttohumlkm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yueranfly.top/gtlknhkgea.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.fzhhl.top/gteyehgioq.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hfpthk.cn/gtawdrwpdx.html

[H02] finally / ensure 收尾
来源：http://hz.dianchejie.cn/gtrjtcsjnl.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yongpay.top/gtwfivumdu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gtsdxecgcl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.316326.xyz/gtvoswgumu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jyoumei.cn/gttfyxrmdq.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gtsjqlzmnn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hnxiangtu.top/gtzwckljll.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.bjfxy.top/gtuneribbt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhijiandao.cn/gtuxcvquri.html

[H03] 主动抛出异常
来源：http://hz.meibo888.top/gtcnawzdlb.html

Py:   raise ValueError("错误信息")
来源：http://hz.nanxinkj.top/gtfzrjimwc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.shzxlz.cn/gtuovudepd.html

JS:   throw new Error("错误信息");
来源：http://hz.yj20258888.top/gtfdhengqs.html

TS:   throw new Error("错误信息");
来源：http://hz.jqgufenzy.top/gtqpnwroww.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.sweek.top/gtkvhygmeu.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.xziqi.cn/gtphftwita.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yanxiufei.cn/gtqcplbojt.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.pengpengdd.cyou/gtiroushqo.html

[H04] 自定义异常类型
来源：http://hz.jianghu66.top/gtqtwenljl.html

Py:   class MyError(Exception): pass
来源：http://hz.cdnleiting.top/gtnbvtotmv.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xuanzx.com/gtnmguwyvx.html

JS:   class MyError extends Error {}
来源：http://hz.jqgufenzy.top/gtrirtsnqj.html

TS:   class MyError extends Error {}
来源：http://hz.chenlongwang.top/gtcvzpcjms.html

Java: class MyException extends RuntimeException {}
来源：http://hz.guowangkeji.top/gtechmggwb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.jlsjyb.cn/gttcuhfvop.html

Ruby: class MyError < StandardError; end
来源：http://hz.hywenlv.cn/gtpguuspdn.html

C#:   class MyException : Exception {}
来源：http://hz.yj20258888.top/gtzrptzoqw.html

[H05] 捕获特定类型
来源：http://hz.daria6918.cn/gtgiubaooy.html

Py:   except ValueError as e:
来源：http://hz.hywenlv.cn/gtpdiexikt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.hfpthk.cn/gtxgixevox.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zycfv.cn/gtygulsiwi.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jlsjyb.cn/gtqhdcbedi.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.aizwys.cn/gtgqoostkj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.chenlongwang.top/gtvpedubhk.html

Ruby: rescue ArgumentError => e
来源：http://hz.sysykeji.top/gtclpscsiq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.snrcjt.cn/gtwqddnduc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jyoumei.cn/gtbcajfuwy.html

Py:   value = d.get("k") or default
来源：http://hz.nanxinkj.top/gtshzqpyed.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ydjk.org.cn/gtqygwtysu.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gaohongyu789.top/gtkyerffdg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sufxvd.cn/gtoqincxzw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.aibaodan.cn/gtpcskdbau.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.cdnleiting.top/gtckeemnvw.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yuxming.cn/gtxbwnmpui.html

C#:   obj?.A?.B ?? default
来源：http://hz.hfpthk.cn/gthjxyzmvc.html

[H07] 断言
来源：http://hz.chenjidiqi.icu/gttdxwwfmt.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zycfv.cn/gtlqsuinnm.html

PHP:  assert($x > 0);
来源：http://hz.hnqzz.top/gtxdaebulm.html

JS:   console.assert(x > 0);
来源：http://hz.shzxlz.cn/gturedlksq.html

TS:   console.assert(x > 0);
来源：http://hz.zhoulong.xyz/gtjhdudxpg.html

Java: assert x > 0 : "必须为正";
来源：http://hz.ivvv.top/gtelfcjdjx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.ivvv.top/gthlpnccwh.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hnqzz.top/gtusfuucfs.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhijiandao.cn/gtwkxrvgkx.html

[H08] 获取错误信息与堆栈
来源：http://hz.cashguo.top/gtkejsbmxn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jyoumei.cn/gtzsxdfnlg.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zdqjudy.top/gtetlskgiv.html

JS:   e.message;  e.stack
来源：http://hz.zycfv.cn/gtydeegjim.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.tianlin.xyz/gtbcsgxqke.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.9152youxi.cn/gtumqolvpp.html

Go:   err.Error()
来源：http://hz.shanyushiyangtech.top/gtewxluvks.html

Ruby: e.message;  e.backtrace
来源：http://hz.hongshengwenyu.top/gtybvwhzzk.html

C#:   e.Message;  e.StackTrace
来源：http://hz.tian-w.cn/gtzvkytkxh.html

[H09] 带错误码的异常
来源：http://hz.jinghuilouyu.cn/gtcpcgxivd.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jlsjyb.cn/gtwhkedacy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jqgfzy.top/gtpufucqmv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yvedp.cn/gtzxkqrlka.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.daxiang520.top/gtvciwllwp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.nwbrower.top/gtaledgknj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hfpthk.cn/gthhwuhuwa.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zhoulong.xyz/gtporokbfm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.wangshuangyany.cn/gtqyardluv.html

[H10] 资源自动释放
来源：http://hz.yj20258.top/gthrcbsexo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.dianchejie.cn/gtjwctzvel.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.snrcjt.cn/gtyrkipvrs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.guannengcc.top/gtspqzgksb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.svipenyu.cn/gtyzrrkwke.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.guowangkeji.top/gtauyajuhh.html

Go:   defer f.Close()
来源：http://hz.dashuyun.cn/gthuuqdnok.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shanyushiyangkeji.top/gtyhucajrh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zdqjudy.top/gtutrnhzod.html

================================================================================
来源：http://hz.dashuyun.cn/gttsbtzhde.html

I. 正则表达式
来源：http://hz.jqgufenzy.top/gtxwbsyffv.html

================================================================================
来源：http://hz.snrcjt.cn/gtjhsfykly.html

[I01] 判断是否匹配
来源：http://hz.chenlongwang.top/gtxodynglh.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zycfv.cn/gtyaxfzlpy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.aizwys.cn/gtrgvlkusl.html

JS:   /\d+/.test(s)
来源：http://hz.sweek.top/gtlaxvpcff.html

TS:   /\d+/.test(s)
来源：http://hz.yangfankeji.com/gtctausvtu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zycfv.cn/gtuvknupex.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.daria6918.cn/gtbmulrxcx.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhiwuduotai.top/gtknaefali.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xinyue.icu/gtdotgfcnu.html

[I02] 提取所有匹配
来源：http://hz.jiagoushi.top/gtyteplnpj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ybcxt.top/gthuaqufwz.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.pycfn.com/gtjxrolqjk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cashguo.top/gtnsznvnqx.html

TS:   s.match(/\d+/g)
来源：http://hz.haohaochexian.top/gtnmgzmyeb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.52xcode.cn/gtbedzcsso.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xylfe.cn/gtycyuoooz.html

Ruby: s.scan(/\d+/)
来源：http://hz.sxryk.cn/gtmakchkto.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ydjk.org.cn/gtshirfhsb.html

[I03] 提取捕获分组
来源：http://hz.xuetiantiany.cn/gtwmjtnxsw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.chenlongwang.top/gttyxmskgx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.guannengcc.top/gtrencmwpu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.bjfxy.top/gtssptwqht.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shuidangran.top/gtgwaqgpnb.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.ehwqpu.com/gtycfvxnog.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ybcxt.top/gtlbdbtfsm.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.feifeiyinyue.top/gtyrqcrlcm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.feifeiyinyue.top/gttyarbzil.html

[I04] 正则替换
来源：http://hz.wangshuangyany.cn/gtwetntwzk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.wangshuangyany.cn/gtptlbgmvx.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sweek.top/gtpoppssto.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.wangdashe.top/gtatlxbnji.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.feifeiyinyue.top/gtymntkfks.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jianghu66.top/gtpqucnfes.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhengqikj.top/gtoyztrwqf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.dianchejie.cn/gtghqukjxb.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.pengpengdd.cyou/gtdbvwfhgy.html

[I05] 按正则拆分
来源：http://hz.zycfv.cn/gtzextsjjy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhiwuduotai.top/gtaqatemps.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.kuanghao11.cn/gtvaqxtbdq.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.ehwqpu.com/gtnskpgvgc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.tian-w.cn/gtfuxwbdxk.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenjidiqi.icu/gthklvltgj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yongpay.top/gtkalymmfc.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hnxiangtu.top/gtzeowsslh.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.meibo888.top/gtiglplsxa.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhiwuduotai.top/gtzfxcutbs.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.tian-w.cn/gtfpfifepp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tanke756.top/gtyauuexcv.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tian-w.cn/gtmkkpiuvl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.fengsongda.top/gtckzveupj.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yongpay.top/gtwhrihxdt.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xuetiantiany.cn/gtwaemfvvo.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.wangshuangyany.cn/gtekcrjexs.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.svipenyu.cn/gtnpnbawik.html

[I07] 忽略大小写与多行模式
来源：http://hz.fengsongda.top/gtmszdawib.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xylfe.cn/gtbwyhymwl.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.tianlin.xyz/gthzirwkkp.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.ivvv.top/gtxhmfasnf.html

TS:   /error/gim
来源：http://hz.iojbl.cn/gtcvhxdbky.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gaohongyu789.top/gtacexubna.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.redwolf501.top/gtlbdoqsha.html

Ruby: s.scan(/error/i)
来源：http://hz.wangshuangyany.cn/gtzcaqfvjg.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.xuetiantiany.cn/gtgbszqjjp.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.vqdsnc.cn/gtkqjmcnjs.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.gzhubu.top/gtaxvddtpx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.sufxvd.cn/gtmvrateiq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.havefunace.top/gtwucacbit.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sweek.top/gtcglyqxja.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yj20258888.top/gtmfnnctez.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.pengpengdd.cyou/gtuuoystwo.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yj202588.top/gtybbtqpqp.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhiwuduotai.top/gtvpnfhwyc.html

================================================================================
来源：http://hz.haohaochexian.top/gtcvkurvbn.html

J. 日期与时间
来源：http://hz.ivvv.top/gttlxbmmxm.html

================================================================================
来源：http://hz.aibaodan.cn/gtquboozus.html

[J01] 获取当前时间
来源：http://hz.gaohongyu789.top/gtgwlnapnn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hywenlv.cn/gthtporipi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhijiandao.cn/gtxidqnlzz.html

JS:   new Date();  Date.now()
来源：http://hz.ybcxt.top/gtpafxsbil.html

TS:   new Date();  Date.now()
来源：http://hz.yonumen.top/gtmdfyvjjd.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.dashuyun.cn/gtqgqthfto.html

Go:   time.Now()
来源：http://hz.fzhhl.top/gtricxpzdh.html

Ruby: Time.now
来源：http://hz.316326.xyz/gttsycxevy.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yuanzhike.top/gtmoktfctp.html

[J02] 格式化输出
来源：http://hz.yj20258.top/gtytvcgvhx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.nanxuanxn.top/gthulzyynp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.52xcode.cn/gtxepgrxqg.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gogol.net.cn/gtxufqzfir.html

TS:   d.toISOString()
来源：http://hz.hfpthk.cn/gtgpkidomq.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.cdnleiting.top/gtkiuggenn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.dianchejie.cn/gteyegmfgf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.shzxlz.cn/gtbzsyoonq.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jqgfzy.top/gthkjhrsox.html

[J03] 字符串解析为日期
来源：http://hz.ywan-chungtsiang.top/gtuvkrwevr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.cucudq.cn/gtyhehatdp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.daria6918.cn/gtzofgjtis.html

JS:   new Date("2024-01-02")
来源：http://hz.dianchejie.cn/gtcztsrqbt.html

TS:   new Date("2024-01-02")
来源：http://hz.guannengcc.top/gtuvdrvtdc.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.jinqigfzy.top/gtvltmlgfi.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.kuanghao11.cn/gtvqypsysu.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cqqwz.cn/gtqqoqedhk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinyuanbaomall.cn/gtgcqyfjub.html

[J04] 时间戳与日期互转
来源：http://hz.jinqigufen.top/gtkfxezrza.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.ydjk.org.cn/gtfqsalkyh.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.chenjidiqi.icu/gtfrerkgzk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.sufxvd.cn/gtjidleeyy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.guowangkeji.top/gtrutlmafb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shanyushiyangtech.top/gtsqekfhfq.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yanxiufei.cn/gtzhiqwmbw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yvedp.cn/gtqbgyfhsh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.pengpengdd.cyou/gtkfijigjo.html

[J05] 时间加减（加 7 天）
来源：http://hz.zhongyouzk.top/gtwmsvukjo.html

Py:   now + timedelta(days=7)
来源：http://hz.aizwys.cn/gtvqsqlxlp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ydzc1.top/gtwwkdsckq.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cqqwz.cn/gtcpvtudaj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shangyingyoupin.top/gtjlnbshnp.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.daxiang520.top/gtwqwoinaa.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.pycfn.com/gtbrttskxr.html

Ruby: Time.now + 7 * 86400
来源：http://hz.svipenyu.cn/gtjujffjmo.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.9152youxi.cn/gtkiqnyqei.html

[J06] 计算两时间之差
来源：http://hz.shzxlz.cn/gtgkfooyvu.html

Py:   (end - start).total_seconds()
来源：http://hz.snrcjt.cn/gtzlhqkhzx.html

PHP:  $end->diff($start)->days;
来源：http://hz.9152youxi.cn/gtxolysqdr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.vqdsnc.cn/gtntwsifna.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhaomingkeji.xyz/gtxveanzyq.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.ivvv.top/gtqvmxrmex.html

Go:   end.Sub(start).Hours()
来源：http://hz.shuidangran.top/gtkkjyavqa.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ppjwa.cn/gtsrdrnfbv.html

C#:   (end - start).TotalSeconds
来源：http://hz.iojbl.cn/gtwpzpowuf.html

[J07] 比较两个日期
来源：http://hz.zdqjudy.top/gtrlpfvtvi.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yongpay.top/gthavycnbq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.nanxinkj.top/gtllqzkkew.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yongpay.top/gtplvfsznf.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.havefunace.top/gtycijtkjz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yj20258888.top/gtqglbtkqm.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hammf.cn/gtxdpjpzre.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yuxming.cn/gtqndomxwm.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.wangdashe.top/gtkwkiqtaw.html

[J08] 提取年月日与星期
来源：http://hz.chenlongwang.top/gttqdbjhmt.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xuetiantiany.cn/gtdduxsccj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.gotoacloud.top/gtiidluwet.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yonumen.top/gtysdcvggo.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.gotoacloud.top/gtpnpreekh.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.yuanzhike.top/gtobiiljff.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.pycfn.com/gtfazjxtml.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.aibaodan.cn/gtqlhzqzlk.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.daria6918.cn/gtzuywayef.html

[J09] 时区处理
来源：http://hz.yueranfly.top/gtqlauqxuv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yvedp.cn/gtfkoyqjes.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.aizwys.cn/gtfcpclltt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yuxming.cn/gtitfjiwbe.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yangfankeji.com/gtkehkhfxf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.nwbrower.top/gtxugtrmwi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jqgfzy.top/gtrgdjaofv.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.fengsongda.top/gtbyxszqsb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.fzhhl.top/gtsddpksbc.html

[J10] 取今天 / 本月第一天
来源：http://hz.feifeiyinyue.top/gthzuedakv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.smart0.xyz/gtwupsilve.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ppjwa.cn/gtncifswcq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yangfankeji.com/gtjvyqxdda.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sufxvd.cn/gtuyuqlyam.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhoulong.xyz/gtpyugvqjy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.wangdashe.top/gtfrhlmkrz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhiwuduotai.top/gtyogzoizq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jinghuilouyu.cn/gtwxxfoaxl.html

================================================================================
来源：http://hz.xziqi.cn/gtfkglxxow.html

K. JSON 与序列化
来源：http://hz.feifeiyinyue.top/gtlwaujuzi.html

================================================================================
来源：http://hz.snrcjt.cn/gtjkrszbhk.html

[K01] 对象转 JSON 字符串
来源：http://hz.hnxiangtu.top/gtqldtlsbf.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.xingfuxueyuan.xyz/gtwzdhndpo.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.gaohongyu789.top/gtyuyfkmmh.html

JS:   JSON.stringify(obj)
来源：http://hz.c1oappe.top/gtqcpqlbxa.html

TS:   JSON.stringify(obj)
来源：http://hz.jlsjyb.cn/gtaptkdsdc.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.iojbl.cn/gtjsfiqzjl.html

Go:   json.Marshal(obj)
来源：http://hz.xinyue.icu/gtehlkxgdr.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.ybcxt.top/gtlhkgnwpx.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jyoumei.cn/gtucrrzotq.html

[K02] JSON 字符串转对象
来源：http://hz.yangfankeji.com/gtzzyqhkbh.html

Py:   json.loads(s)
来源：http://hz.tianlin.xyz/gtmtfcvuxj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.andypj.xyz/gtdcifqxeb.html

JS:   JSON.parse(s)
来源：http://hz.hfpthk.cn/gtpgurebqb.html

TS:   JSON.parse(s)
来源：http://hz.havefunace.top/gtgbixyhsc.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.tanke756.top/gtykzltgmr.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.guannengcc.top/gtqurkaoji.html

Ruby: JSON.parse(s)
来源：http://hz.tanke756.top/gttinhslns.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.shuidangran.top/gtwpimgskq.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.jinghuilouyu.cn/gtavvrftig.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.jyoumei.cn/gtkzsoulws.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.jinyuanbaomall.cn/gteyonrelu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.svipenyu.cn/gtmxffehkf.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.cashguo.top/gtsjierijd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.sweek.top/gtbxqhlwpl.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.dashuyun.cn/gtdnecgbxe.html


<!-- 参考信息 -->