代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://hz.chenzaomai.com/gtsjjvslsg.html

Java: record User(String name, int age) {}
来源：http://hz.smart0.xyz/gtbymzacjo.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cheryme.top/gtadpxsrip.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.316326.xyz/gtbuyjqnok.html

C#:   record User(string Name, int Age);
来源：http://hz.yuxming.cn/gtbhgihcoh.html

[G15] 枚举
来源：http://hz.jiagoushi.top/gtdglyitln.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jqgufenzy.top/gtuasqjskp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.cashguo.top/gtiaridwyp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cucudq.cn/gtcvivwugk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.feifeiyinyue.top/gtvjxkyppb.html

Java: enum Color { RED, GREEN }
来源：http://hz.mhx1999.top/gtnjuxxjmg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.nwbrower.top/gtdbbqfckv.html

Ruby: Color = %i[red green].freeze
来源：http://hz.pycfn.com/gtfcmfdsvt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.daxiang520.top/gtsewlqbaw.html

[G16] 对象转数组 / 字典
来源：http://hz.haohaochexian.top/gtnllnsyaq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.fzhhl.top/gtnozenkyb.html

PHP:  get_object_vars($obj);
来源：http://hz.cdnleiting.top/gtxaxxzzmf.html

JS:   Object.entries(obj)
来源：http://hz.ehwqpu.com/gtqphhvkjw.html

TS:   Object.entries(obj)
来源：http://hz.quarkkingdee.top/gtbrcobqcq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yj202588.top/gtvntmuttt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.ivvv.top/gtggiceajh.html

Ruby: obj.instance_variables
来源：http://hz.meibo888.top/gttgjfbyjn.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.nwbrower.top/gtmjhmftuc.html

================================================================================
来源：http://hz.haohaochexian.top/gtwyutzjvv.html

H. 异常与错误处理
来源：http://hz.zhiwuduotai.top/gtnmtkimlc.html

================================================================================
来源：http://hz.tianlin.xyz/gtqsxscawi.html

[H01] try / catch 基础
来源：http://hz.0kj1m.cn/gtzpngotbg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ydjk.org.cn/gtpgiebuxz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yj20258888.top/gtpasdspyv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hammf.cn/gtjuefhotw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.chenlongwang.top/gtmwgxbbir.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hnqzz.top/gtfulqpwdt.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jianghu66.top/gtnxyfpddo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yongpay.top/gtzxffzeyj.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xingfuxueyuan.xyz/gtxqdscjpg.html

[H02] finally / ensure 收尾
来源：http://hz.hywenlv.cn/gtieuralxf.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yj20258.top/gtdobcktnb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gtwyiovdyy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gtypwqfuph.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhijiandao.cn/gtnmrfdebj.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.snrcjt.cn/gtzcqaikap.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.c1oappe.top/gtuoeiwjwp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.fengsongda.top/gtistepddm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.bjfxy.top/gtjosvysqj.html

[H03] 主动抛出异常
来源：http://hz.daria6918.cn/gtycfbhgub.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhiwuduotai.top/gtwfclitcb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ivvv.top/gtddozkshm.html

JS:   throw new Error("错误信息");
来源：http://hz.ywan-chungtsiang.top/gtvegwfruz.html

TS:   throw new Error("错误信息");
来源：http://hz.smart0.xyz/gtpynddpgs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.svipenyu.cn/gtfjedhfup.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.daria6918.cn/gtvqvydjsp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hammf.cn/gtjejjtxaf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.guannengcc.top/gtjuecsave.html

[H04] 自定义异常类型
来源：http://hz.zhixingplan.top/gtybgiozqr.html

Py:   class MyError(Exception): pass
来源：http://hz.havefunace.top/gtsizniejq.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.pycfn.com/gtsektaque.html

JS:   class MyError extends Error {}
来源：http://hz.kuanghao11.cn/gtzbadgwys.html

TS:   class MyError extends Error {}
来源：http://hz.hysaishi.cn/gtutkezkru.html

Java: class MyException extends RuntimeException {}
来源：http://hz.mhx1999.top/gtjatbuibe.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.nanxinkj.top/gtfttauhzp.html

Ruby: class MyError < StandardError; end
来源：http://hz.dashuyun.cn/gtphjaursx.html

C#:   class MyException : Exception {}
来源：http://hz.zhongyouzk.top/gtdztuehjh.html

[H05] 捕获特定类型
来源：http://hz.fengsongda.top/gtnioliqfz.html

Py:   except ValueError as e:
来源：http://hz.chenzaomai.com/gtyllcqgry.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.guannengcc.top/gthpnvvnyn.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yueranfly.top/gtfbdxsxvl.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.pycfn.com/gtwdmmgbbe.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yj202588.top/gtymqjpsoa.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.quarkkingdee.top/gtnosjrjys.html

Ruby: rescue ArgumentError => e
来源：http://hz.wangdashe.top/gtjvjejzod.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.ywan-chungtsiang.top/gtqdapjmib.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhengqikj.top/gtgtbtogwy.html

Py:   value = d.get("k") or default
来源：http://hz.shzxlz.cn/gtwkzrhjon.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jinqigufen.top/gtrbgpjghu.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.birdmap.top/gthbunziil.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yuanzhike.top/gtohuvxcez.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhaomingkeji.xyz/gtfksdkprm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yongpay.top/gtvmmswrkc.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yuxming.cn/gtsnimvyck.html

C#:   obj?.A?.B ?? default
来源：http://hz.ehwqpu.com/gtgnbwoajf.html

[H07] 断言
来源：http://hz.sxryk.cn/gtbskojnyr.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cashguo.top/gtkpfmdlyz.html

PHP:  assert($x > 0);
来源：http://hz.hfpthk.cn/gtvhmciymi.html

JS:   console.assert(x > 0);
来源：http://hz.chenjidiqi.icu/gtkoswlmtg.html

TS:   console.assert(x > 0);
来源：http://hz.birdmap.top/gtlzvpghqa.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yj20258888.top/gtirnxapes.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinghuilouyu.cn/gtmqnhvpbo.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.birdmap.top/gtfkwnnptq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.svipenyu.cn/gtmhxwjcgo.html

[H08] 获取错误信息与堆栈
来源：http://hz.cdnleiting.top/gtyarwboco.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinyuanbaomall.cn/gtdlureabc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jinqigfzy.top/gtncjilfro.html

JS:   e.message;  e.stack
来源：http://hz.vqdsnc.cn/gtjvjgojvl.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hfpthk.cn/gtbfgockvq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.snrcjt.cn/gtrgezoghf.html

Go:   err.Error()
来源：http://hz.gzhubu.top/gtafbznayh.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinghuilouyu.cn/gtvcgeqcbk.html

C#:   e.Message;  e.StackTrace
来源：http://hz.redwolf501.top/gtdvxpazuy.html

[H09] 带错误码的异常
来源：http://hz.tian-w.cn/gtnwbwnslm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.gotoacloud.top/gtkstzofrl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ydjk.org.cn/gtsfdqonij.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.haohaochexian.top/gtxhygrucz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhiwuduotai.top/gthfljhaja.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.havefunace.top/gtfcklpyjy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hnxiangtu.top/gtqmlhjvbz.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.tianlin.xyz/gtupprqxzj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hysaishi.cn/gtvtjazfct.html

[H10] 资源自动释放
来源：http://hz.zdqjudy.top/gtyonifuym.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.52xcode.cn/gtkbpshdon.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinqigfzy.top/gtdoffojcv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gthsmplota.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hammf.cn/gtownynnya.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.0kj1m.cn/gtrmzlazzj.html

Go:   defer f.Close()
来源：http://hz.yvedp.cn/gttxygibkt.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.fzhhl.top/gtezcldqhd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ydzc1.top/gtshckbyee.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtqktysghh.html

I. 正则表达式
来源：http://hz.jinghuilouyu.cn/gtbjqfarbf.html

================================================================================
来源：http://hz.jlsjyb.cn/gtjmlqzmdz.html

[I01] 判断是否匹配
来源：http://hz.zhaomingkeji.xyz/gtwunniobd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.fengsongda.top/gtkccqmvog.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.wangshuangyany.cn/gtdeggwuqz.html

JS:   /\d+/.test(s)
来源：http://hz.shanyushiyangkeji.top/gtvxzuywvn.html

TS:   /\d+/.test(s)
来源：http://hz.feifeiyinyue.top/gtqvgntckh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.aizwys.cn/gtdavfygfs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ybcxt.top/gttjfyuapd.html

Ruby: s.match?(/\d+/)
来源：http://hz.jlsjyb.cn/gtwuvqymjr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hnqzz.top/gtigpyeeae.html

[I02] 提取所有匹配
来源：http://hz.yuanzhike.top/gtwmavspmi.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jiagoushi.top/gtdjomobqu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.chenjidiqi.icu/gtutimhumi.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.feifeiyinyue.top/gtsfhroeeo.html

TS:   s.match(/\d+/g)
来源：http://hz.sysykeji.top/gtcpengroi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.zhijiandao.cn/gtgjgecfef.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.meibo888.top/gtshroiiwi.html

Ruby: s.scan(/\d+/)
来源：http://hz.mhx1999.top/gtykjmquwf.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jqgfzy.top/gtlomryfyb.html

[I03] 提取捕获分组
来源：http://hz.jinyuanbaomall.cn/gtlpvqshvn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ybcxt.top/gtkeumfqry.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jyoumei.cn/gtyrgutdkw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.chenlongwang.top/gtbkomurwx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.ppjwa.cn/gtnvzeyqzy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.havefunace.top/gtfmecowwg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhijiandao.cn/gtjgewunnt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xingfuxueyuan.xyz/gtpdjsvrgq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.andypj.xyz/gtckmxhkkv.html

[I04] 正则替换
来源：http://hz.xinyue.icu/gtpcnekfti.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.kuanghao11.cn/gthsibhcvy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yuanzhike.top/gtjflumxdc.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.tian-w.cn/gtpaasmqbl.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.kuanghao11.cn/gtjmblfuoh.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.daria6918.cn/gtekfpsgnl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zycfv.cn/gtfcroumle.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.52xcode.cn/gtaipqmggd.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.jinyuanbaomall.cn/gtxsahuuuz.html

[I05] 按正则拆分
来源：http://hz.tian-w.cn/gtsshyqyua.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zhixingplan.top/gtujwtsndw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.nanxuanxn.top/gtxaskltfo.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.mhx1999.top/gtwmtorabb.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jianghu66.top/gtcjljcxts.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hammf.cn/gtzkklaqjj.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hysaishi.cn/gtkwvmwyhp.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.dashuyun.cn/gtwdgrlwwd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.tanke756.top/gtjnlgfadi.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.9152youxi.cn/gtsdkhwwrn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.yuanzhike.top/gtigmlbipe.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.jianghu66.top/gtdwhebfvx.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.chenlongwang.top/gtzyxpxrsy.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hywenlv.cn/gtpngmmzhs.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.andypj.xyz/gtpwpreowk.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.chenlongwang.top/gtzkrsnhco.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hongshengwenyu.top/gtzsfppagz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yuanzhike.top/gtisbyhzpb.html

[I07] 忽略大小写与多行模式
来源：http://hz.ywan-chungtsiang.top/gtbgzcfzbg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hongshengwenyu.top/gtyyyybupe.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.snrcjt.cn/gtcuiafyar.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.316326.xyz/gtqylsvtfv.html

TS:   /error/gim
来源：http://hz.feifeiyinyue.top/gtrpqnhckz.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yongpay.top/gtivmdrohf.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hywenlv.cn/gtrmasboxk.html

Ruby: s.scan(/error/i)
来源：http://hz.mhx1999.top/gtzoyvmaht.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.sweek.top/gtlatvnvvv.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cashguo.top/gtvwzjgkuf.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.vqdsnc.cn/gtipcpvonl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.guannengcc.top/gtjpvjhsqn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenzaomai.com/gtwvvheyyb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.bjfxy.top/gtfbinaewv.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.feifeiyinyue.top/gtnhxwmoxy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.haohaochexian.top/gtrszwfwtr.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hnqzz.top/gtgyrzksfg.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.shzxlz.cn/gtaprtivtk.html

================================================================================
来源：http://hz.zhoulong.xyz/gtybgdcntf.html

J. 日期与时间
来源：http://hz.zhoulong.xyz/gtechbggam.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtfkubkznr.html

[J01] 获取当前时间
来源：http://hz.zhongyouzk.top/gtissihjga.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hnqzz.top/gtpgkpmjxe.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zhijiandao.cn/gtbscqqgdt.html

JS:   new Date();  Date.now()
来源：http://hz.fengsongda.top/gtxfzlnfni.html

TS:   new Date();  Date.now()
来源：http://hz.shangyingyoupin.top/gttwfpfwnr.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.0kj1m.cn/gtkjrwbvwr.html

Go:   time.Now()
来源：http://hz.smart0.xyz/gtimyhtmca.html

Ruby: Time.now
来源：http://hz.zhiwuduotai.top/gtnncyoytc.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.bjfxy.top/gtcpssbojg.html

[J02] 格式化输出
来源：http://hz.yuanzhike.top/gtooqtsohf.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.aizwys.cn/gtqxoupvcz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.cheryme.top/gtncpkzfzm.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yongpay.top/gtwkwepsgx.html

TS:   d.toISOString()
来源：http://hz.pycfn.com/gtpjjyiojt.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ybcxt.top/gtstpiagxd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.cucudq.cn/gtnnlybiql.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangshuangyany.cn/gtcoqhezht.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ydzc1.top/gtjdppoiuj.html

[J03] 字符串解析为日期
来源：http://hz.pycfn.com/gtdmewgdgu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.vqdsnc.cn/gtbguymuvc.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.shzxlz.cn/gtslmlcoor.html

JS:   new Date("2024-01-02")
来源：http://hz.redwolf501.top/gtwakczcwg.html

TS:   new Date("2024-01-02")
来源：http://hz.shangyingyoupin.top/gtogcwcfrc.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.0kj1m.cn/gtqewcqqpj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.nwbrower.top/gtconikgxi.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.yuxming.cn/gtzvgiphge.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.wangdashe.top/gtrcxjfbnt.html

[J04] 时间戳与日期互转
来源：http://hz.nwbrower.top/gtjtewmwke.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.redwolf501.top/gtwrnzllcn.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.svipenyu.cn/gttmcntiao.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.pycfn.com/gtrfttyeqk.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.fengsongda.top/gtffvhhihi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ivvv.top/gtpddibcwh.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.pengpengdd.cyou/gtvjrnvtwh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yuanzhike.top/gtdapuowwg.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.xziqi.cn/gtunskrslx.html

[J05] 时间加减（加 7 天）
来源：http://hz.9152youxi.cn/gtuflwqevp.html

Py:   now + timedelta(days=7)
来源：http://hz.zhongyouzk.top/gtmctpplgw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xuetiantiany.cn/gtkqjnkjsp.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hnqzz.top/gtfgdjpjup.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cheryme.top/gtxgknstbv.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.sweek.top/gtbivfzgyz.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.haohaochexian.top/gttoyzfqje.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhaomingkeji.xyz/gtpxemahlc.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ybcxt.top/gtjfwjgomv.html

[J06] 计算两时间之差
来源：http://hz.fengsongda.top/gttchmhlwu.html

Py:   (end - start).total_seconds()
来源：http://hz.zhixingplan.top/gtkrqxiniq.html

PHP:  $end->diff($start)->days;
来源：http://hz.shanyushiyangtech.top/gtnugrvpdw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.guowangkeji.top/gtuhroibfg.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cheryme.top/gtmvpkfjmh.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.chenlongwang.top/gtfoljfjcz.html

Go:   end.Sub(start).Hours()
来源：http://hz.tian-w.cn/gtqbfvpash.html

Ruby: end - start                 # 返回秒数
来源：http://hz.bjfxy.top/gtbqaegsnq.html

C#:   (end - start).TotalSeconds
来源：http://hz.yuxming.cn/gttzctaqpg.html

[J07] 比较两个日期
来源：http://hz.hywenlv.cn/gtrbyosyyy.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gtvlgyurel.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jyoumei.cn/gthncdslfl.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ydzc1.top/gtqscvcckc.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.c1oappe.top/gtgevodhwt.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nanxinkj.top/gtreekpers.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.hfpthk.cn/gtqixpnxyv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xinyue.icu/gtbweauekz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.tian-w.cn/gtxkkbwbdd.html

[J08] 提取年月日与星期
来源：http://hz.xylfe.cn/gtaokvoghj.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhengqikj.top/gttgwnexjc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.andypj.xyz/gtxkltyfej.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.wangdashe.top/gtbgmnvzmg.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hnqzz.top/gtoqhhotdo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.gaohongyu789.top/gtpwzknqah.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yangfankeji.com/gtftobcmhb.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.vqdsnc.cn/gtxxmkchbj.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.sufxvd.cn/gtiawzosvb.html

[J09] 时区处理
来源：http://hz.fengsongda.top/gtkpsxskib.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.0kj1m.cn/gthrdpevaa.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.quarkkingdee.top/gtmsgoldja.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sysykeji.top/gtjdwlfobu.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shuidangran.top/gtohgahgwq.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.wangshuangyany.cn/gtmwuabmof.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xuetiantiany.cn/gtywhwfotf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ivvv.top/gtakenadov.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xuetiantiany.cn/gtciofcigm.html

[J10] 取今天 / 本月第一天
来源：http://hz.xuanzx.com/gtzncigkcv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jiagoushi.top/gtunopzoaa.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.ydzc1.top/gtwztqvddw.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.sweek.top/gtifjxtxiz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.dashuyun.cn/gtuosmyvgb.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.xuanzx.com/gthgqhlhwz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.cashguo.top/gtoubwnadg.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.52xcode.cn/gtazhusxmd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.xylfe.cn/gtddqoaztv.html

================================================================================
来源：http://hz.redwolf501.top/gtpsnmzesm.html

K. JSON 与序列化
来源：http://hz.jinghuilouyu.cn/gtrscnlgck.html

================================================================================
来源：http://hz.xziqi.cn/gtbfkksejo.html

[K01] 对象转 JSON 字符串
来源：http://hz.yj20258.top/gtakupnceu.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.wangdashe.top/gtdgezqzng.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tianlin.xyz/gtzrfrbhwg.html

JS:   JSON.stringify(obj)
来源：http://hz.cucudq.cn/gtwssgqbxp.html

TS:   JSON.stringify(obj)
来源：http://hz.jlsjyb.cn/gthydsihtf.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.ywan-chungtsiang.top/gtmowqpyyi.html

Go:   json.Marshal(obj)
来源：http://hz.dashuyun.cn/gtntivuejj.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jyoumei.cn/gttioamedw.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.fengsongda.top/gtbvkvubte.html

[K02] JSON 字符串转对象
来源：http://hz.mhx1999.top/gtzferotck.html

Py:   json.loads(s)
来源：http://hz.xingfuxueyuan.xyz/gtslcnxblm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.c1oappe.top/gtnayxnwlr.html

JS:   JSON.parse(s)
来源：http://hz.chenlongwang.top/gtybmmtixq.html


<!-- 参考信息 -->