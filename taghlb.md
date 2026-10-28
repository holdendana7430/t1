代发 wailian999

C#:   record User(string Name, int Age);
来源：http://hz.hfpthk.cn/gtjgurettn.html

[G15] 枚举
来源：http://hz.svipenyu.cn/gtpdikawuu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.svipenyu.cn/gtieymbbxr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.havefunace.top/gtffmtdajg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jianghu66.top/gtfruklqwh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jinqigfzy.top/gtyrsfqgys.html

Java: enum Color { RED, GREEN }
来源：http://hz.gotoacloud.top/gtkzrqgqqk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.cucudq.cn/gtqqxvhlfw.html

Ruby: Color = %i[red green].freeze
来源：http://hz.tanke756.top/gtiskmdbvw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cucudq.cn/gtkxfefguj.html

[G16] 对象转数组 / 字典
来源：http://hz.kuanghao11.cn/gtcbajgsjk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.iojbl.cn/gtwbebwriw.html

PHP:  get_object_vars($obj);
来源：http://hz.sufxvd.cn/gthmgizvhu.html

JS:   Object.entries(obj)
来源：http://hz.jinghuilouyu.cn/gtbmtfuaad.html

TS:   Object.entries(obj)
来源：http://hz.yj202588.top/gtrquzcjpd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhiwuduotai.top/gtrsrmycdx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.fzhhl.top/gtvbrhymbv.html

Ruby: obj.instance_variables
来源：http://hz.hywenlv.cn/gtrvldqufe.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.52xcode.cn/gtplxvdoyo.html

================================================================================
来源：http://hz.haohaochexian.top/gtjeslzjuq.html

H. 异常与错误处理
来源：http://hz.aibaodan.cn/gtdysqcszg.html

================================================================================
来源：http://hz.jinqigufen.top/gtqnuufmzk.html

[H01] try / catch 基础
来源：http://hz.ywan-chungtsiang.top/gtssfefmfm.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.ehwqpu.com/gtfxikbhif.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ybcxt.top/gtowqbgcjl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.pengpengdd.cyou/gthwrknuaw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhaomingkeji.xyz/gtphfqclxz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jinyuanbaomall.cn/gtoushdrjs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.chenjidiqi.icu/gtypzpgpdx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yangfankeji.com/gtrytsuiks.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yj20258888.top/gtivgsuwvl.html

[H02] finally / ensure 收尾
来源：http://hz.ppjwa.cn/gtgkwpuclf.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.bjfxy.top/gtgalhjgdv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.dianchejie.cn/gtnwhydmov.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gtlqwbvrwu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xingfuxueyuan.xyz/gtwfwyszvi.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtdguorwxx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yj20258.top/gtewbpuvhv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.chenjidiqi.icu/gtyrczijpp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.wangdashe.top/gtbxxkmrhz.html

[H03] 主动抛出异常
来源：http://hz.tanke756.top/gtgwahnudl.html

Py:   raise ValueError("错误信息")
来源：http://hz.wangshuangyany.cn/gtfkjpblmf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jlsjyb.cn/gtxufhbbhd.html

JS:   throw new Error("错误信息");
来源：http://hz.cqqwz.cn/gtgxrajenr.html

TS:   throw new Error("错误信息");
来源：http://hz.hywenlv.cn/gtlwfycdgz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gzhubu.top/gtdztjxbzr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.ivvv.top/gtvsvlqldz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nanxuanxn.top/gtthzhervs.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.feifeiyinyue.top/gtewutdqnq.html

[H04] 自定义异常类型
来源：http://hz.yangfankeji.com/gtdymrqfvc.html

Py:   class MyError(Exception): pass
来源：http://hz.daria6918.cn/gtbzmjxxmx.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.tian-w.cn/gtcxtnaood.html

JS:   class MyError extends Error {}
来源：http://hz.0kj1m.cn/gtnseynxct.html

TS:   class MyError extends Error {}
来源：http://hz.gzhubu.top/gtoyokayfe.html

Java: class MyException extends RuntimeException {}
来源：http://hz.52xcode.cn/gthbzuphtp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.nanxinkj.top/gtxjagquou.html

Ruby: class MyError < StandardError; end
来源：http://hz.havefunace.top/gtldtoeqxh.html

C#:   class MyException : Exception {}
来源：http://hz.nanxuanxn.top/gtkzjcqosi.html

[H05] 捕获特定类型
来源：http://hz.cqqwz.cn/gtwrzjfnff.html

Py:   except ValueError as e:
来源：http://hz.jinghuilouyu.cn/gtmdkdtnhl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhongyouzk.top/gtviwrtpnv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.bjfxy.top/gtlojqyqwn.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cucudq.cn/gtrmctlsxv.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.quarkkingdee.top/gtdmkqtukp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.dashuyun.cn/gtcwhaitmv.html

Ruby: rescue ArgumentError => e
来源：http://hz.aibaodan.cn/gtlzchbbyc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhengqikj.top/gtufquvgok.html

[H06] 可选值 / 空值安全访问
来源：http://hz.quarkkingdee.top/gtjnccepiy.html

Py:   value = d.get("k") or default
来源：http://hz.jinqigufen.top/gttdpnxdnh.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.meibo888.top/gtihwcgtvv.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.kuanghao11.cn/gtmotgdkcn.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.chenjidiqi.icu/gtbjokvjnp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhongyouzk.top/gtouyiijxb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.mhx1999.top/gttjhsppoj.html

Ruby: d&.dig(:a, :b)
来源：http://hz.gzhubu.top/gtwvwunyqy.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinqigfzy.top/gtinibtxmh.html

[H07] 断言
来源：http://hz.zhijiandao.cn/gtmzgaxrwf.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shangyingyoupin.top/gtmerngjwy.html

PHP:  assert($x > 0);
来源：http://hz.xziqi.cn/gtbbiuqtnm.html

JS:   console.assert(x > 0);
来源：http://hz.hywenlv.cn/gtkdjadtlx.html

TS:   console.assert(x > 0);
来源：http://hz.gaohongyu789.top/gtsyqaxpfy.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jqgfzy.top/gtmdfkdxck.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.havefunace.top/gtjpoezjku.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tianlin.xyz/gtvramlknn.html

C#:   Debug.Assert(x > 0);
来源：http://hz.fzhhl.top/gtzduuybgn.html

[H08] 获取错误信息与堆栈
来源：http://hz.ydjk.org.cn/gtslhysziq.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hammf.cn/gtirwmprhi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.sufxvd.cn/gtywcadvvi.html

JS:   e.message;  e.stack
来源：http://hz.vqdsnc.cn/gtndbnhops.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.havefunace.top/gtuuqknfcu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xuanzx.com/gtuprecknl.html

Go:   err.Error()
来源：http://hz.pycfn.com/gtdofatwpf.html

Ruby: e.message;  e.backtrace
来源：http://hz.jinqigufen.top/gtuzxohrab.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jinqigfzy.top/gturboshkt.html

[H09] 带错误码的异常
来源：http://hz.xuetiantiany.cn/gtkudmeght.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yvedp.cn/gtsfbyfmqs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.zhengqikj.top/gtzsjwinhn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hongshengwenyu.top/gtbterygvw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.pycfn.com/gtmpnilbto.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.9152youxi.cn/gtxxfrwnza.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhaomingkeji.xyz/gtbbneviuq.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sufxvd.cn/gtezqfkrwj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.bjfxy.top/gtnwkrehhi.html

[H10] 资源自动释放
来源：http://hz.havefunace.top/gtukflkfqa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.0kj1m.cn/gtvzcfisir.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xuanzx.com/gtojdugvfz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aizwys.cn/gtsmvuxbsr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gzhubu.top/gthmmrmeqh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.zdqjudy.top/gthyhcqnbu.html

Go:   defer f.Close()
来源：http://hz.pengpengdd.cyou/gtsfwhzaxb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.daxiang520.top/gtofmnddiu.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hnqzz.top/gtqgtieixg.html

================================================================================
来源：http://hz.yongpay.top/gtxgppliob.html

I. 正则表达式
来源：http://hz.gzhubu.top/gtwehxnzyb.html

================================================================================
来源：http://hz.yangfankeji.com/gtbdhhcgyu.html

[I01] 判断是否匹配
来源：http://hz.smart0.xyz/gtorgtbcgp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.hongshengwenyu.top/gtlgymhrml.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.gotoacloud.top/gtsstiqgfn.html

JS:   /\d+/.test(s)
来源：http://hz.aibaodan.cn/gtwoejfupy.html

TS:   /\d+/.test(s)
来源：http://hz.mhx1999.top/gtiizdtdjm.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.redwolf501.top/gtdszusjuw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.snrcjt.cn/gtdkfyrbvw.html

Ruby: s.match?(/\d+/)
来源：http://hz.gaohongyu789.top/gtvgrkzhzl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yonumen.top/gtjwyfyeoq.html

[I02] 提取所有匹配
来源：http://hz.tian-w.cn/gtqfzpgoxr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.9152youxi.cn/gtdkklzzav.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shuidangran.top/gtljjywgng.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.gogol.net.cn/gtthricqvq.html

TS:   s.match(/\d+/g)
来源：http://hz.yueranfly.top/gtcvtvyamh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.0kj1m.cn/gtiyvxtltm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yonumen.top/gtvrjpvoyv.html

Ruby: s.scan(/\d+/)
来源：http://hz.xuanzx.com/gtomrzjxbo.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.haohaochexian.top/gtipndaibh.html

[I03] 提取捕获分组
来源：http://hz.zhaomingkeji.xyz/gtafslfawv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yangfankeji.com/gtdwjdobqf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.guowangkeji.top/gtksdtyurt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj202588.top/gthrpmuerl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.gotoacloud.top/gtmwcogple.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.c1oappe.top/gtkakwegej.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.gotoacloud.top/gtzmdiwkyg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.hnxiangtu.top/gthapublww.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.guannengcc.top/gtdcdyqkww.html

[I04] 正则替换
来源：http://hz.jqgfzy.top/gtfiqivwmr.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhengqikj.top/gtsbnpkpcj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.quarkkingdee.top/gtjrjqiodm.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zycfv.cn/gtykilwljq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.tanke756.top/gtxsxoylhp.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.nanxuanxn.top/gtexgdcraz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yangfankeji.com/gtldziyzvw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gotoacloud.top/gtlyrygnjw.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ivvv.top/gtwhpdvzmt.html

[I05] 按正则拆分
来源：http://hz.shzxlz.cn/gtqnyvmwyk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.sufxvd.cn/gtgiwmkecc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.pengpengdd.cyou/gtdrlspdil.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.aizwys.cn/gtfnjpjksy.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.shangyingyoupin.top/gtdslrztvv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.daxiang520.top/gtoqdzhaau.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.guowangkeji.top/gtzfeobjzq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.birdmap.top/gtpwbvqaog.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zdqjudy.top/gtwgzvigty.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zdqjudy.top/gtgovmxyqa.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.nwbrower.top/gtksakschi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.fzhhl.top/gtwcbyuyyh.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sufxvd.cn/gtskuiobyk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sufxvd.cn/gtwypmiwts.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jianghu66.top/gtxqwjmnhw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.daria6918.cn/gtpchryahr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhaomingkeji.xyz/gtwwncrbkj.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cqqwz.cn/gtnxhjykfe.html

[I07] 忽略大小写与多行模式
来源：http://hz.ehwqpu.com/gtxxpfkgkf.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.xziqi.cn/gtasrgxxhd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.xylfe.cn/gtufbubjyw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shuidangran.top/gtlisiyiwf.html

TS:   /error/gim
来源：http://hz.snrcjt.cn/gtspjmolme.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ehwqpu.com/gtnqlgsouy.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hywenlv.cn/gttldfsrae.html

Ruby: s.scan(/error/i)
来源：http://hz.jinqigfzy.top/gtskzfjdrz.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gogol.net.cn/gtsmcxgbbo.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yvedp.cn/gtmevelopn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.haohaochexian.top/gtwwrbqkel.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yj202588.top/gtmmsfyrhv.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.kuanghao11.cn/gtpczqlokv.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shzxlz.cn/gtnkcmxlhr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.shuidangran.top/gtyndghovz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gaohongyu789.top/gttjbsaijk.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jlsjyb.cn/gtzxvdwepn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.bjfxy.top/gtjohwcqvp.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gttrlkooou.html

J. 日期与时间
来源：http://hz.chenjidiqi.icu/gtxshudkhy.html

================================================================================
来源：http://hz.yuanzhike.top/gthawcscyj.html

[J01] 获取当前时间
来源：http://hz.mhx1999.top/gtxytpfbtl.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.jlsjyb.cn/gtnncipyug.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ivvv.top/gtkzcqxmnl.html

JS:   new Date();  Date.now()
来源：http://hz.jinghuilouyu.cn/gthmzfcydg.html

TS:   new Date();  Date.now()
来源：http://hz.quarkkingdee.top/gtbykvalcv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.fengsongda.top/gtncrxgnkh.html

Go:   time.Now()
来源：http://hz.shzxlz.cn/gtvgnlnapc.html

Ruby: Time.now
来源：http://hz.ehwqpu.com/gtbmtuibmh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yj20258.top/gtvgtagoav.html

[J02] 格式化输出
来源：http://hz.gzhubu.top/gtenqwialk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dianchejie.cn/gtmhfgsmmk.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.guowangkeji.top/gtkzkrakxr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.vqdsnc.cn/gtispqtqia.html

TS:   d.toISOString()
来源：http://hz.shuidangran.top/gtozjswsjs.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.fengsongda.top/gtgbsdgsxw.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jqgfzy.top/gtwautcqjp.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.redwolf501.top/gtvonvhvcu.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jqgfzy.top/gtojlpotip.html

[J03] 字符串解析为日期
来源：http://hz.kuanghao11.cn/gthxqjheym.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jiagoushi.top/gtyeeqcbhn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.fengsongda.top/gtqdwqtjem.html

JS:   new Date("2024-01-02")
来源：http://hz.52xcode.cn/gtwgethlta.html

TS:   new Date("2024-01-02")
来源：http://hz.zhixingplan.top/gtnhcmubxv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hnqzz.top/gtimckaaur.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.yonumen.top/gtgusnnopx.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.andypj.xyz/gtgssftnxp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.tian-w.cn/gtvgzxacqt.html

[J04] 时间戳与日期互转
来源：http://hz.wangdashe.top/gtwcdibqee.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.vqdsnc.cn/gtzxjadgzx.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hywenlv.cn/gtrkqijdmf.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jqgufenzy.top/gtkodtgmsb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hnqzz.top/gtblyfpivs.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sysykeji.top/gtzasqllke.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.aizwys.cn/gtrfuijdrj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.haohaochexian.top/gtqwtuiskb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yuanzhike.top/gtzjjwlbhs.html

[J05] 时间加减（加 7 天）
来源：http://hz.pengpengdd.cyou/gtlfywnvlz.html

Py:   now + timedelta(days=7)
来源：http://hz.9152youxi.cn/gtjehcnxoo.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cdnleiting.top/gtheinrwdf.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yuxming.cn/gtgtzyzrxv.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.pengpengdd.cyou/gtvyazpnsg.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.tanke756.top/gtotyiphgl.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hysaishi.cn/gtesywnjgz.html

Ruby: Time.now + 7 * 86400
来源：http://hz.haohaochexian.top/gtmlengtlm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jqgufenzy.top/gtyoyucjti.html

[J06] 计算两时间之差
来源：http://hz.mhx1999.top/gtlchhrqxp.html

Py:   (end - start).total_seconds()
来源：http://hz.gzhubu.top/gtjcgtcpjo.html

PHP:  $end->diff($start)->days;
来源：http://hz.c1oappe.top/gttknlikut.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.0kj1m.cn/gtcxaxbbdu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hysaishi.cn/gtzfssecxz.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.smart0.xyz/gthxtidgsy.html

Go:   end.Sub(start).Hours()
来源：http://hz.yanxiufei.cn/gttffuvqml.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ywan-chungtsiang.top/gtnjqjrrow.html

C#:   (end - start).TotalSeconds
来源：http://hz.fzhhl.top/gtsbwnhkmp.html

[J07] 比较两个日期
来源：http://hz.xziqi.cn/gtrevophfd.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.tianlin.xyz/gtjskdtxjp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.c1oappe.top/gtbzybmngb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shuidangran.top/gtgghsbfly.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.tanke756.top/gtjosnxurp.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jinqigfzy.top/gtzuvwmydh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.xinyue.icu/gtqwyqpqeu.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yangfankeji.com/gtuwfaacar.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shzxlz.cn/gtbwerwxqu.html

[J08] 提取年月日与星期
来源：http://hz.aizwys.cn/gtephzmrrb.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yvedp.cn/gtmkoymjsn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.52xcode.cn/gttrrnjonx.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.guowangkeji.top/gthxgobgdx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.pycfn.com/gtwmkycssn.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.cqqwz.cn/gtzdjsrvud.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.zhijiandao.cn/gtukfjprjr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.kuanghao11.cn/gtqjzjavxa.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.guowangkeji.top/gtpbylwhoa.html

[J09] 时区处理
来源：http://hz.aibaodan.cn/gtzcqkfymk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yj202588.top/gtqtvuydan.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.zhongyouzk.top/gtkefwzdek.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.jiagoushi.top/gtwsvpsdaa.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hysaishi.cn/gtqlpuolqk.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.svipenyu.cn/gtcaxcrege.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.iojbl.cn/gtlyqrgmiw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shanyushiyangkeji.top/gticpirrsf.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ydzc1.top/gtttycylkj.html

[J10] 取今天 / 本月第一天
来源：http://hz.smart0.xyz/gtoqykzqsp.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.sxryk.cn/gtnocsemnw.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.xuetiantiany.cn/gtjcqzafvl.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.havefunace.top/gtybsbjtoj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.9152youxi.cn/gtjciduwov.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.chenjidiqi.icu/gtslrzjxcf.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hfpthk.cn/gtekhgqkxm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.cheryme.top/gtmcrjmxmm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.svipenyu.cn/gthdnhycmt.html

================================================================================
来源：http://hz.zhixingplan.top/gthulyvtxu.html

K. JSON 与序列化
来源：http://hz.gzhubu.top/gtqbcfzvza.html

================================================================================
来源：http://hz.zdqjudy.top/gtbpsmehvx.html

[K01] 对象转 JSON 字符串
来源：http://hz.cucudq.cn/gtmcjmnqwd.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.iojbl.cn/gthldrcrey.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.jinqigufen.top/gtqjcyhnzp.html

JS:   JSON.stringify(obj)
来源：http://hz.jinqigufen.top/gtxxyjdeyz.html

TS:   JSON.stringify(obj)
来源：http://hz.zycfv.cn/gttqqbyosl.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xylfe.cn/gtpjgafojt.html

Go:   json.Marshal(obj)
来源：http://hz.316326.xyz/gtkpyhggdb.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.redwolf501.top/gtxjijzcyv.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.dashuyun.cn/gthfkoahsi.html

[K02] JSON 字符串转对象
来源：http://hz.c1oappe.top/gtyehuqstw.html

Py:   json.loads(s)
来源：http://hz.c1oappe.top/gtaxgldntm.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.aibaodan.cn/gthllwemce.html

JS:   JSON.parse(s)
来源：http://hz.iojbl.cn/gtarlimonq.html

TS:   JSON.parse(s)
来源：http://hz.dianchejie.cn/gtthbhuafb.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hz.havefunace.top/gtumkixvsf.html

Go:   json.Unmarshal(data, &v)
来源：http://hz.jinqigufen.top/gtbapqsysr.html

Ruby: JSON.parse(s)
来源：http://hz.nanxuanxn.top/gtlzqklybb.html


<!-- 参考信息 -->