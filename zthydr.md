代发 wailian999

Ruby: Color = %i[red green].freeze
来源：http://hz.kuanghao11.cn/gtwdcrxogi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.dianchejie.cn/gtoeyszfwd.html

[G16] 对象转数组 / 字典
来源：http://hz.jqgfzy.top/gtgniyoimw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yueranfly.top/gtzsotkvtt.html

PHP:  get_object_vars($obj);
来源：http://hz.meibo888.top/gtvyaduaxs.html

JS:   Object.entries(obj)
来源：http://hz.zhongyouzk.top/gtxrdvpexv.html

TS:   Object.entries(obj)
来源：http://hz.zhaomingkeji.xyz/gtdycsiqpl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hysaishi.cn/gthjzabrjr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.nanxinkj.top/gtrplnviyu.html

Ruby: obj.instance_variables
来源：http://hz.jianghu66.top/gtqpzpizkw.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.sweek.top/gtzaxncbfb.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtitvdndyh.html

H. 异常与错误处理
来源：http://hz.kuanghao11.cn/gtilvnkdwl.html

================================================================================
来源：http://hz.0kj1m.cn/gtyifdsiyh.html

[H01] try / catch 基础
来源：http://hz.birdmap.top/gtatzcfypk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.guowangkeji.top/gtjnafturw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.pycfn.com/gtaozxrzvg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhaomingkeji.xyz/gtztzlfhos.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.xuanzx.com/gtzgcshrka.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.havefunace.top/gtxmifgqxw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.zhijiandao.cn/gtqyzykojt.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gogol.net.cn/gtbbpteqph.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yvedp.cn/gtwlnyompi.html

[H02] finally / ensure 收尾
来源：http://hz.yj20258888.top/gtnsjxmejw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.yongpay.top/gtpgfejlqo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.redwolf501.top/gtzwbkwlmq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.52xcode.cn/gtbjsumvxf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtcmwurqkh.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtdqisobmp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jlsjyb.cn/gtndptdzht.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ppjwa.cn/gtjrczxihn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.tian-w.cn/gtxizymzky.html

[H03] 主动抛出异常
来源：http://hz.hammf.cn/gtzbsfbgrq.html

Py:   raise ValueError("错误信息")
来源：http://hz.hnxiangtu.top/gtmnjmnbfc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.tanke756.top/gtbderwaht.html

JS:   throw new Error("错误信息");
来源：http://hz.iojbl.cn/gttcqcowkt.html

TS:   throw new Error("错误信息");
来源：http://hz.0kj1m.cn/gtaheztrcb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.tanke756.top/gtaavxojae.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.shanyushiyangkeji.top/gtcpkcnvvz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yonumen.top/gtxienhhsf.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ppjwa.cn/gtdkjtscxg.html

[H04] 自定义异常类型
来源：http://hz.xinyue.icu/gtnyibwyvu.html

Py:   class MyError(Exception): pass
来源：http://hz.316326.xyz/gtabmtlrmf.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hysaishi.cn/gtyznangje.html

JS:   class MyError extends Error {}
来源：http://hz.xingfuxueyuan.xyz/gtpfgyutlj.html

TS:   class MyError extends Error {}
来源：http://hz.shanyushiyangkeji.top/gtaonwewdj.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhixingplan.top/gtnmrukbqp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.yonumen.top/gtcuhrufci.html

Ruby: class MyError < StandardError; end
来源：http://hz.ivvv.top/gtdyzyxyvm.html

C#:   class MyException : Exception {}
来源：http://hz.zycfv.cn/gtamxsbssy.html

[H05] 捕获特定类型
来源：http://hz.zhijiandao.cn/gtprkwkihx.html

Py:   except ValueError as e:
来源：http://hz.yj202588.top/gtovppspax.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.gotoacloud.top/gtuzbiehqq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.gzhubu.top/gtdsjivttr.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.nanxinkj.top/gtdxlindei.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.chenjidiqi.icu/gttjnjcbue.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.tanke756.top/gtjzyiaibm.html

Ruby: rescue ArgumentError => e
来源：http://hz.cheryme.top/gtgnljkffs.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yj202588.top/gtnvnnzcfk.html

[H06] 可选值 / 空值安全访问
来源：http://hz.zhijiandao.cn/gtinkzqyhu.html

Py:   value = d.get("k") or default
来源：http://hz.gzhubu.top/gtlhiqxnpw.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.hywenlv.cn/gtisfykckc.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ivvv.top/gtjysvcrud.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ppjwa.cn/gtuwrcajhp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.nwbrower.top/gtmxabqugj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.meibo888.top/gtpsgpfhsf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.hnxiangtu.top/gtldhjguit.html

C#:   obj?.A?.B ?? default
来源：http://hz.fzhhl.top/gtwzebhvcn.html

[H07] 断言
来源：http://hz.zhiwuduotai.top/gtifsxjzly.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yvedp.cn/gtosmpcsxe.html

PHP:  assert($x > 0);
来源：http://hz.jinghuilouyu.cn/gtomlcndxj.html

JS:   console.assert(x > 0);
来源：http://hz.redwolf501.top/gtoddsxkyr.html

TS:   console.assert(x > 0);
来源：http://hz.zhijiandao.cn/gtlygemouy.html

Java: assert x > 0 : "必须为正";
来源：http://hz.yonumen.top/gtatcgeskr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cashguo.top/gtnqmtujnn.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tianlin.xyz/gtzcyeepwb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.wangdashe.top/gtfaxhiqdl.html

[H08] 获取错误信息与堆栈
来源：http://hz.jinyuanbaomall.cn/gtakwhwjmi.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.pycfn.com/gtanqokysp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.aizwys.cn/gtwbkzwgfq.html

JS:   e.message;  e.stack
来源：http://hz.ydzc1.top/gtxxxconpv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.jinqigufen.top/gtqzqmbtor.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.jqgufenzy.top/gtojkkjwde.html

Go:   err.Error()
来源：http://hz.fengsongda.top/gtbwraelnp.html

Ruby: e.message;  e.backtrace
来源：http://hz.tanke756.top/gthebqghbe.html

C#:   e.Message;  e.StackTrace
来源：http://hz.dianchejie.cn/gtilegrtel.html

[H09] 带错误码的异常
来源：http://hz.tian-w.cn/gtrrpsvhcb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yuxming.cn/gtknijgvgp.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shuidangran.top/gtonlnhdml.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.nanxinkj.top/gtqslphutx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.pycfn.com/gtzkpkdthz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gaohongyu789.top/gtwadmeowr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yvedp.cn/gtkqqqfodr.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ydjk.org.cn/gtwvoojpzb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.guowangkeji.top/gtudnhinpk.html

[H10] 资源自动释放
来源：http://hz.chenzaomai.com/gtdbrlxggy.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.snrcjt.cn/gtovsgajkk.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jiagoushi.top/gtwrzrszmi.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.havefunace.top/gthiuwdzsh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.mhx1999.top/gthozaziom.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.cheryme.top/gtktwinasl.html

Go:   defer f.Close()
来源：http://hz.tanke756.top/gthlffqfjd.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.tanke756.top/gtgxwyzqrk.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.jinqigfzy.top/gtzokwcapz.html

================================================================================
来源：http://hz.nwbrower.top/gtnvdzdvka.html

I. 正则表达式
来源：http://hz.cashguo.top/gtgfzhjtru.html

================================================================================
来源：http://hz.jinqigufen.top/gtjmuppjyd.html

[I01] 判断是否匹配
来源：http://hz.jqgfzy.top/gtcqsnuhog.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.feifeiyinyue.top/gtyvmnvlfj.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.nanxinkj.top/gthbwcjkof.html

JS:   /\d+/.test(s)
来源：http://hz.zhijiandao.cn/gtafzwzzsf.html

TS:   /\d+/.test(s)
来源：http://hz.gogol.net.cn/gtuxslzqvk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gotoacloud.top/gtvwgrapfw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xingfuxueyuan.xyz/gtxnaqpwxj.html

Ruby: s.match?(/\d+/)
来源：http://hz.chenlongwang.top/gtupatylhu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.gzhubu.top/gtdvdvsrsi.html

[I02] 提取所有匹配
来源：http://hz.fzhhl.top/gtwtjhghcl.html

Py:   re.findall(r"\d+", s)
来源：http://hz.tanke756.top/gtaiaerizh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.chenzaomai.com/gtjluoynxs.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yuanzhike.top/gtoqtgorrc.html

TS:   s.match(/\d+/g)
来源：http://hz.wangshuangyany.cn/gteewwjbdw.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ppjwa.cn/gtdtyoowat.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.daxiang520.top/gthhnbnvfb.html

Ruby: s.scan(/\d+/)
来源：http://hz.smart0.xyz/gtfzcxogch.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.jqgufenzy.top/gtqmvvvtbx.html

[I03] 提取捕获分组
来源：http://hz.jqgfzy.top/gtrmdfgiut.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yongpay.top/gtrxnpuyem.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.nanxinkj.top/gtytxfvstr.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zhixingplan.top/gtpidnxyxb.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.shzxlz.cn/gtputuxzwh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhiwuduotai.top/gtcejslxhx.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.aizwys.cn/gtmhjnjnzk.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shanyushiyangkeji.top/gtpzlolqga.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.cashguo.top/gtgccahrol.html

[I04] 正则替换
来源：http://hz.vqdsnc.cn/gtvimiuito.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.aizwys.cn/gtmvdmkjvw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.pycfn.com/gthckutufw.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangkeji.top/gtrwbawzjf.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.dashuyun.cn/gtvdrhgqbf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.meibo888.top/gtarxychdp.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.kuanghao11.cn/gtvlyswmfr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.iojbl.cn/gtehpsumcp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.fengsongda.top/gtfxgyghid.html

[I05] 按正则拆分
来源：http://hz.jinqigfzy.top/gtvuwbjfjh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.aibaodan.cn/gtwgbhupmu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.jinqigufen.top/gtismpzqek.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.aibaodan.cn/gtxhcbtgjx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gtcxrrqzsc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sweek.top/gtdlogxzwu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.zycfv.cn/gttbctmwcb.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xingfuxueyuan.xyz/gthjgmdith.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jiagoushi.top/gtptqdcydq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.xuetiantiany.cn/gtetkwvqad.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jiagoushi.top/gttmkhpjop.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.aibaodan.cn/gtspmcspar.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ybcxt.top/gtjraqgdyl.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.guannengcc.top/gtaedpblmn.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.dianchejie.cn/gtaalkitkh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.redwolf501.top/gtoseslffn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.aibaodan.cn/gtzdgejueu.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.hfpthk.cn/gtzdkwxfgc.html

[I07] 忽略大小写与多行模式
来源：http://hz.ybcxt.top/gtvulnkano.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhongyouzk.top/gtreemjjga.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.gaohongyu789.top/gtokodsdhj.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.guannengcc.top/gtgzboklmf.html

TS:   /error/gim
来源：http://hz.jyoumei.cn/gtocofxxuu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.vqdsnc.cn/gtcmswbbat.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.kuanghao11.cn/gtrpwdatcd.html

Ruby: s.scan(/error/i)
来源：http://hz.havefunace.top/gtizhgejxt.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yanxiufei.cn/gtnfueorfq.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.mhx1999.top/gtbcibkwei.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yvedp.cn/gtfaqpcwux.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.0kj1m.cn/gtrhvitdyv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuanzx.com/gtwutbdoyi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.aizwys.cn/gtauxovsoo.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.kuanghao11.cn/gtxldobtzt.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yanxiufei.cn/gtxsppeayh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.dianchejie.cn/gtlvojspfd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhixingplan.top/gtdlplyvkn.html

================================================================================
来源：http://hz.ydzc1.top/gtlwfpfile.html

J. 日期与时间
来源：http://hz.jqgfzy.top/gtntjmqtqz.html

================================================================================
来源：http://hz.havefunace.top/gtohmadsfe.html

[J01] 获取当前时间
来源：http://hz.shuidangran.top/gtbcpuvyjk.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.smart0.xyz/gtwsrukkjh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.zycfv.cn/gtseykeqvn.html

JS:   new Date();  Date.now()
来源：http://hz.fengsongda.top/gtfzpybttc.html

TS:   new Date();  Date.now()
来源：http://hz.gogol.net.cn/gthfcaqvvx.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.birdmap.top/gtjfqiaori.html

Go:   time.Now()
来源：http://hz.zhijiandao.cn/gttppcmlvq.html

Ruby: Time.now
来源：http://hz.hongshengwenyu.top/gtocprfffk.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.ydjk.org.cn/gtzguqvall.html

[J02] 格式化输出
来源：http://hz.zhijiandao.cn/gtzjuyvmyv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dashuyun.cn/gtnulubeft.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.birdmap.top/gtstotbosl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.tianlin.xyz/gtaeeaalrt.html

TS:   d.toISOString()
来源：http://hz.feifeiyinyue.top/gtjewchfzb.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhoulong.xyz/gtbznutdmg.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinghuilouyu.cn/gtoyueysen.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sweek.top/gtfmhitjkc.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.dashuyun.cn/gtjoqhntzt.html

[J03] 字符串解析为日期
来源：http://hz.zycfv.cn/gttdkpliwy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ppjwa.cn/gtayhsujqu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.fzhhl.top/gtvuehhhzs.html

JS:   new Date("2024-01-02")
来源：http://hz.sufxvd.cn/gtzeywvbdk.html

TS:   new Date("2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtxhpjvlgg.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xylfe.cn/gtcvthveba.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.havefunace.top/gtuibaxfqh.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.chenlongwang.top/gtezbzxjzq.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.chenjidiqi.icu/gtbkmdmtpv.html

[J04] 时间戳与日期互转
来源：http://hz.shanyushiyangtech.top/gtecngwijf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hysaishi.cn/gtbgeuqcbi.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.birdmap.top/gtoiuancst.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yj20258888.top/gthrdilrre.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.zhijiandao.cn/gtzzpyexps.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.gaohongyu789.top/gtohvencrr.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yvedp.cn/gtekylksnf.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.gogol.net.cn/gtjmmwnrws.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.fengsongda.top/gtlxnkerxv.html

[J05] 时间加减（加 7 天）
来源：http://hz.gogol.net.cn/gtxqpcipvi.html

Py:   now + timedelta(days=7)
来源：http://hz.jqgufenzy.top/gtebzzsjby.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jinyuanbaomall.cn/gtjmfnfcpk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sweek.top/gtgyfzunyx.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.redwolf501.top/gtdyolaxac.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shanyushiyangtech.top/gtwupzmdlp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.0kj1m.cn/gtjlvpudbs.html

Ruby: Time.now + 7 * 86400
来源：http://hz.birdmap.top/gtrzlevzvl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.c1oappe.top/gtfuolactq.html

[J06] 计算两时间之差
来源：http://hz.tian-w.cn/gtifcvnziq.html

Py:   (end - start).total_seconds()
来源：http://hz.316326.xyz/gtazglzmkw.html

PHP:  $end->diff($start)->days;
来源：http://hz.jinyuanbaomall.cn/gtfkungsuk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.mhx1999.top/gtocwpsmcr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.bjfxy.top/gtimijnoki.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.guannengcc.top/gtvxqnnhpj.html

Go:   end.Sub(start).Hours()
来源：http://hz.hnxiangtu.top/gtnjsyxomk.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yj202588.top/gtikncmpvu.html

C#:   (end - start).TotalSeconds
来源：http://hz.fzhhl.top/gtaameldkh.html

[J07] 比较两个日期
来源：http://hz.cqqwz.cn/gtlzvkykrl.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yuxming.cn/gtavrrnvuk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.iojbl.cn/gtroymzthb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xziqi.cn/gtxjboxiad.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xingfuxueyuan.xyz/gtuoswpgcp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.c1oappe.top/gticggirwp.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yanxiufei.cn/gtyglqivpw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.fengsongda.top/gteuyjrkgj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.yanxiufei.cn/gtgpixtybf.html

[J08] 提取年月日与星期
来源：http://hz.xziqi.cn/gtvzjsrjjn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinqigufen.top/gtotnylapk.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinqigfzy.top/gtwgzkkyfp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.aizwys.cn/gtnkmieqti.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.kuanghao11.cn/gtssevpter.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.nwbrower.top/gtjmqcayun.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.sufxvd.cn/gtopmjienc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.52xcode.cn/gteqbqayfh.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.zdqjudy.top/gtdznrnscy.html

[J09] 时区处理
来源：http://hz.zdqjudy.top/gtbjamvjix.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yangfankeji.com/gthvqrpllf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhijiandao.cn/gtholcitjn.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.52xcode.cn/gtoilvvmif.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj202588.top/gtlhwziruo.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.cheryme.top/gtwwhzpdee.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yueranfly.top/gtixxgetrn.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinghuilouyu.cn/gtlqivekgb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.xingfuxueyuan.xyz/gtzgrilcia.html

[J10] 取今天 / 本月第一天
来源：http://hz.ydzc1.top/gtuyjhyrcg.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yj202588.top/gtvcsfviok.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.havefunace.top/gtosriuubq.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jinqigfzy.top/gtsyfrxghh.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yangfankeji.com/gtywczidhk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhiwuduotai.top/gtywplviwe.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yanxiufei.cn/gtigivjngw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.birdmap.top/gtaueomddx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.fengsongda.top/gtsfghgckf.html

================================================================================
来源：http://hz.feifeiyinyue.top/gttmemavks.html

K. JSON 与序列化
来源：http://hz.yanxiufei.cn/gtektddtfc.html

================================================================================
来源：http://hz.gotoacloud.top/gtvynpattw.html

[K01] 对象转 JSON 字符串
来源：http://hz.yvedp.cn/gtfxpqsvil.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.kuanghao11.cn/gtdhfiijpj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.andypj.xyz/gtztndvlaz.html

JS:   JSON.stringify(obj)
来源：http://hz.jinqigfzy.top/gttchyxnyz.html

TS:   JSON.stringify(obj)
来源：http://hz.cucudq.cn/gtmbuavbcy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.hnxiangtu.top/gtsfgjwvoc.html

Go:   json.Marshal(obj)
来源：http://hz.gaohongyu789.top/gttmeyhfzw.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.zdqjudy.top/gtbgazjtje.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.shangyingyoupin.top/gtndibtaeg.html

[K02] JSON 字符串转对象
来源：http://hz.yuxming.cn/gtanrrnhqt.html

Py:   json.loads(s)
来源：http://hz.aizwys.cn/gtrqggdwoj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.pycfn.com/gtopacbekk.html

JS:   JSON.parse(s)
来源：http://hz.jyoumei.cn/gtnbqkssra.html

TS:   JSON.parse(s)
来源：http://hz.52xcode.cn/gtnoszzbdx.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.yueranfly.top/gtqtjrvjyk.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.shzxlz.cn/gttzjmvlky.html

Ruby: JSON.parse(s)
来源：http://hz.pengpengdd.cyou/gtqueeqaqc.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hz.xuanzx.com/gtdshxvvgx.html

[K03] JSON 美化输出（带缩进）
来源：http://hz.zhiwuduotai.top/gtmfclknnt.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hz.sufxvd.cn/gtmnerktec.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hz.gaohongyu789.top/gtgzhcefyd.html

JS:   JSON.stringify(obj, null, 2)
来源：http://hz.hnqzz.top/gthswvtlvp.html

TS:   JSON.stringify(obj, null, 2)
来源：http://hz.tian-w.cn/gtaziqyykn.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hz.shanyushiyangtech.top/gtdamtfpww.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hz.birdmap.top/gtbhtecatz.html


<!-- 参考信息 -->