代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://hz.jinghuilouyu.cn/gttosdjrhs.html

Java: record User(String name, int age) {}
来源：http://hz.yanxiufei.cn/gtufvlqxcg.html

Go:   type User struct { Name string; Age int }
来源：http://hz.nanxuanxn.top/gtcsxdpohm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.chenzaomai.com/gtwrncjynd.html

C#:   record User(string Name, int Age);
来源：http://hz.yj202588.top/gtenlxvqmr.html

[G15] 枚举
来源：http://hz.svipenyu.cn/gtbmgmpewa.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yj202588.top/gtyyvaqxrl.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.smart0.xyz/gtcumghhpq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.shangyingyoupin.top/gtzhzaftvo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yueranfly.top/gthlfpsgux.html

Java: enum Color { RED, GREEN }
来源：http://hz.tianlin.xyz/gtvysokiym.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.xinyue.icu/gtjfxjlxic.html

Ruby: Color = %i[red green].freeze
来源：http://hz.tian-w.cn/gtaknqxmno.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xinyue.icu/gtorlfpbks.html

[G16] 对象转数组 / 字典
来源：http://hz.cqqwz.cn/gtrblxszte.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.quarkkingdee.top/gtyprhtaxb.html

PHP:  get_object_vars($obj);
来源：http://hz.chenjidiqi.icu/gtdjnggkhq.html

JS:   Object.entries(obj)
来源：http://hz.chenzaomai.com/gtrsmibccd.html

TS:   Object.entries(obj)
来源：http://hz.nanxuanxn.top/gtrhjtizgr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhixingplan.top/gtoqrzxacd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yvedp.cn/gtikxgbfyv.html

Ruby: obj.instance_variables
来源：http://hz.redwolf501.top/gttwnaifbh.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ywan-chungtsiang.top/gtlbcpnwed.html

================================================================================
来源：http://hz.chenzaomai.com/gtjkdrdrkb.html

H. 异常与错误处理
来源：http://hz.yongpay.top/gtrlnvudsv.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtqstsicbb.html

[H01] try / catch 基础
来源：http://hz.wangshuangyany.cn/gtwvwpnlln.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xinyue.icu/gtbcgouaub.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.smart0.xyz/gtxhkamcoo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.fzhhl.top/gthzwkqjlg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.haohaochexian.top/gtnmsnnwcy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yvedp.cn/gtcqqvywfb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.aizwys.cn/gtkygrzukd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.snrcjt.cn/gtctoknjpm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gotoacloud.top/gtcxgbodiv.html

[H02] finally / ensure 收尾
来源：http://hz.birdmap.top/gtlbbmdegp.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.iojbl.cn/gtsxunpyfz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xuanzx.com/gtgyhybuqf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gtgxbysjas.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gttynmwsyx.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nwbrower.top/gtqgiwjcbr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.sweek.top/gtwdbauzoo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.shzxlz.cn/gtobvxprlv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.cheryme.top/gtlbvykfgx.html

[H03] 主动抛出异常
来源：http://hz.hnxiangtu.top/gthqtqiusi.html

Py:   raise ValueError("错误信息")
来源：http://hz.chenzaomai.com/gtkfnxgsqe.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jinqigfzy.top/gtevxwmxip.html

JS:   throw new Error("错误信息");
来源：http://hz.xinyue.icu/gtfpghtrwe.html

TS:   throw new Error("错误信息");
来源：http://hz.yanxiufei.cn/gtwiozqqhl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhijiandao.cn/gtbzzlifad.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.feifeiyinyue.top/gtwbpiksnv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.dashuyun.cn/gtlnrwkpjt.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ppjwa.cn/gtqalejfga.html

[H04] 自定义异常类型
来源：http://hz.fengsongda.top/gtiwcqjbja.html

Py:   class MyError(Exception): pass
来源：http://hz.hywenlv.cn/gtsmauirjj.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.xylfe.cn/gtcsnulqjh.html

JS:   class MyError extends Error {}
来源：http://hz.shzxlz.cn/gtumnutjfj.html

TS:   class MyError extends Error {}
来源：http://hz.nanxinkj.top/gtbqiauycq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yuxming.cn/gttguceubl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ehwqpu.com/gtucsrzwks.html

Ruby: class MyError < StandardError; end
来源：http://hz.ppjwa.cn/gtyjzecgfn.html

C#:   class MyException : Exception {}
来源：http://hz.snrcjt.cn/gtzcuqwysk.html

[H05] 捕获特定类型
来源：http://hz.feifeiyinyue.top/gtjsmnvmnc.html

Py:   except ValueError as e:
来源：http://hz.jinghuilouyu.cn/gtmqhqnssl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.vqdsnc.cn/gtbwzmigpn.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhongyouzk.top/gtsixdptyz.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.feifeiyinyue.top/gtoxkzsysg.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.jqgfzy.top/gtxysfwfmk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zycfv.cn/gtzytrqjzs.html

Ruby: rescue ArgumentError => e
来源：http://hz.xuetiantiany.cn/gtjjqocduu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.zhoulong.xyz/gtuehmsmle.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hnxiangtu.top/gtjpanilfv.html

Py:   value = d.get("k") or default
来源：http://hz.redwolf501.top/gtcolmvngk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yvedp.cn/gtcqpygmki.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.mhx1999.top/gtmpkfdaow.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhijiandao.cn/gtdqkhpqvn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ydzc1.top/gtnlqrgpqm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.mhx1999.top/gtgjqnujai.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zhiwuduotai.top/gtcfrdctsb.html

C#:   obj?.A?.B ?? default
来源：http://hz.wangshuangyany.cn/gtyigkfzfj.html

[H07] 断言
来源：http://hz.svipenyu.cn/gtgnguomof.html

Py:   assert x > 0, "必须为正"
来源：http://hz.xylfe.cn/gtzuiputuy.html

PHP:  assert($x > 0);
来源：http://hz.jiagoushi.top/gtdrxhiaot.html

JS:   console.assert(x > 0);
来源：http://hz.jianghu66.top/gtftuwbfjv.html

TS:   console.assert(x > 0);
来源：http://hz.hnqzz.top/gtnxohwefx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.guowangkeji.top/gtzmlvdzjd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinqigfzy.top/gttomiddvs.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.yuanzhike.top/gtfhxtxmww.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xingfuxueyuan.xyz/gtedluuzpd.html

[H08] 获取错误信息与堆栈
来源：http://hz.havefunace.top/gtkjvvtfep.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.sweek.top/gtyayhmetf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.meibo888.top/gthtoirnhr.html

JS:   e.message;  e.stack
来源：http://hz.xuanzx.com/gtjtrcxcbn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.wangdashe.top/gtswysgprv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.pengpengdd.cyou/gtmuvvrxdt.html

Go:   err.Error()
来源：http://hz.pengpengdd.cyou/gtptqrfkud.html

Ruby: e.message;  e.backtrace
来源：http://hz.yueranfly.top/gtqaovmlyr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.zhixingplan.top/gtburjedeh.html

[H09] 带错误码的异常
来源：http://hz.yj20258.top/gttetbmlfh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.daxiang520.top/gtkxjixmtz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.sweek.top/gtighrcybe.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.svipenyu.cn/gtdkxlcopd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.fzhhl.top/gtwrndrcdl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.chenzaomai.com/gtniijywmb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.bjfxy.top/gtxzbljxgs.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.ehwqpu.com/gtxkdekhzq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zhaomingkeji.xyz/gttsmeasar.html

[H10] 资源自动释放
来源：http://hz.vqdsnc.cn/gtlbjldhxk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yongpay.top/gtkokstvbf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sysykeji.top/gtyorhvcgg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.aibaodan.cn/gtbytsbgkh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tanke756.top/gtawogqkix.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yj20258888.top/gtwerhztlp.html

Go:   defer f.Close()
来源：http://hz.hnxiangtu.top/gtynyxxvxi.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.zhengqikj.top/gtpgykuqzi.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.tianlin.xyz/gtgbkszjja.html

================================================================================
来源：http://hz.bjfxy.top/gtlnhkihhg.html

I. 正则表达式
来源：http://hz.sysykeji.top/gtvjvrlbmb.html

================================================================================
来源：http://hz.yonumen.top/gthjhgycjs.html

[I01] 判断是否匹配
来源：http://hz.ivvv.top/gtjjnphrfr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ybcxt.top/gteerdebwr.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xinyue.icu/gtdxtbgaby.html

JS:   /\d+/.test(s)
来源：http://hz.dashuyun.cn/gtvkjxqrgb.html

TS:   /\d+/.test(s)
来源：http://hz.ehwqpu.com/gtmxwszqrj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.yj20258888.top/gtzdjtrnba.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yonumen.top/gtyvrrrjnx.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhijiandao.cn/gtotdrebmq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.snrcjt.cn/gtelfisrbp.html

[I02] 提取所有匹配
来源：http://hz.fzhhl.top/gtnxmthkeg.html

Py:   re.findall(r"\d+", s)
来源：http://hz.316326.xyz/gtvcgxpdcc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jinyuanbaomall.cn/gtmcgzxodj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.havefunace.top/gtlbospxiq.html

TS:   s.match(/\d+/g)
来源：http://hz.yuanzhike.top/gtxkqsgxgf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.tian-w.cn/gtiwcwedch.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.jqgfzy.top/gteqwwyezs.html

Ruby: s.scan(/\d+/)
来源：http://hz.hnxiangtu.top/gtfjvjhibd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.shanyushiyangkeji.top/gtzbkgisak.html

[I03] 提取捕获分组
来源：http://hz.gotoacloud.top/gtxuvjlhvb.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xylfe.cn/gtmqwbhncd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.birdmap.top/gtzvrqhqtk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.mhx1999.top/gtwtyovnyt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhaomingkeji.xyz/gtwrsxeprr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.c1oappe.top/gtdbncifot.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ydjk.org.cn/gtgoqsdspg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ivvv.top/gtjwknhrup.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.nanxuanxn.top/gtidgzpqkt.html

[I04] 正则替换
来源：http://hz.shanyushiyangkeji.top/gtaxobdqbv.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.svipenyu.cn/gtseongkrg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhaomingkeji.xyz/gtlmxyiwiq.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.zhiwuduotai.top/gtdmqoifnq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gaohongyu789.top/gtthbhxpfz.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.hammf.cn/gtnuiwfidh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.redwolf501.top/gtvtazqjkm.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yueranfly.top/gtxvmpucag.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yuanzhike.top/gtsjgewxbd.html

[I05] 按正则拆分
来源：http://hz.ydzc1.top/gtztlhghpg.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shangyingyoupin.top/gtqonrtonj.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.nanxinkj.top/gtvczkjwlo.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gtemyoebzw.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gthfkvaaya.html

Java: s.split("\\s*,\\s*")
来源：http://hz.tanke756.top/gtpwfrighq.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xylfe.cn/gtgbmuznny.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.gaohongyu789.top/gtdvcjdzbm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jqgfzy.top/gtuhcgmtxm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hysaishi.cn/gtdaapthqt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.0kj1m.cn/gtxznrvgno.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.52xcode.cn/gtfzfqusre.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.haohaochexian.top/gtjbtumshm.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cheryme.top/gteczgtlok.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.chenlongwang.top/gtgvimlxys.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.andypj.xyz/gtsiwhdyck.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.wangdashe.top/gtyrdoahhg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cdnleiting.top/gtkmxrpflk.html

[I07] 忽略大小写与多行模式
来源：http://hz.jinqigufen.top/gtwjxggeuc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhijiandao.cn/gtehoisboz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.316326.xyz/gtwtlcuspd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yongpay.top/gtitpccztf.html

TS:   /error/gim
来源：http://hz.gaohongyu789.top/gtquvfpqng.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinyuanbaomall.cn/gtckwjxrwv.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhengqikj.top/gtltrkhtuo.html

Ruby: s.scan(/error/i)
来源：http://hz.yangfankeji.com/gttbobwqel.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.shanyushiyangtech.top/gtoeffjzmb.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.fzhhl.top/gtkcsefrqt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.guannengcc.top/gtjxtkznbz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.0kj1m.cn/gtydzcuzwe.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yvedp.cn/gtxcenjfru.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.meibo888.top/gtjywmedes.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.tianlin.xyz/gtnmmvqjui.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xuetiantiany.cn/gtsrsludus.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.mhx1999.top/gtpgmfurpn.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.chenjidiqi.icu/gtwmxcwyac.html

================================================================================
来源：http://hz.zhengqikj.top/gtjbhwowph.html

J. 日期与时间
来源：http://hz.fengsongda.top/gtbidhqzfo.html

================================================================================
来源：http://hz.nanxinkj.top/gtarkglzjw.html

[J01] 获取当前时间
来源：http://hz.jyoumei.cn/gticfcoume.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenlongwang.top/gtyfshcqwf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.wangshuangyany.cn/gthkkmpzxl.html

JS:   new Date();  Date.now()
来源：http://hz.svipenyu.cn/gtzkdnmneg.html

TS:   new Date();  Date.now()
来源：http://hz.pycfn.com/gtnflmnpol.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.mhx1999.top/gtdppssvhv.html

Go:   time.Now()
来源：http://hz.birdmap.top/gtkuqulaov.html

Ruby: Time.now
来源：http://hz.yuanzhike.top/gtvdnfpait.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.zdqjudy.top/gtrmwkxvzc.html

[J02] 格式化输出
来源：http://hz.redwolf501.top/gtkykugtrd.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.52xcode.cn/gtmhqnczux.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.jlsjyb.cn/gthfqonncr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.hnxiangtu.top/gtjsvykzth.html

TS:   d.toISOString()
来源：http://hz.hfpthk.cn/gtcxnsshhx.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xinyue.icu/gtlinhdsdf.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yongpay.top/gtikucdxwm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj202588.top/gtmbmqhgke.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.snrcjt.cn/gtmxgvubmb.html

[J03] 字符串解析为日期
来源：http://hz.gogol.net.cn/gtwhifzkmy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.ppjwa.cn/gtbkemktbb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yj20258888.top/gtcgnygezh.html

JS:   new Date("2024-01-02")
来源：http://hz.yvedp.cn/gtcnuxrerd.html

TS:   new Date("2024-01-02")
来源：http://hz.chenlongwang.top/gtwegqgptj.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.sysykeji.top/gtxzcsztib.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.sxryk.cn/gtwcfjyvgr.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cheryme.top/gtfzxmxrcd.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.chenjidiqi.icu/gtzmdhygtb.html

[J04] 时间戳与日期互转
来源：http://hz.jinyuanbaomall.cn/gtptsqdfpw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.tian-w.cn/gtwrohucvd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sxryk.cn/gthzrxhpak.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.birdmap.top/gtvskzwysw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jlsjyb.cn/gtiebkdihi.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ybcxt.top/gthwyuudaf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhongyouzk.top/gtodokhokw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.smart0.xyz/gtngmdvhho.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yongpay.top/gtlswrzvmy.html

[J05] 时间加减（加 7 天）
来源：http://hz.gotoacloud.top/gtoxhwkiuu.html

Py:   now + timedelta(days=7)
来源：http://hz.nwbrower.top/gtaadzsogv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.guannengcc.top/gtprmokssy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ehwqpu.com/gtkudnchav.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenzaomai.com/gtdxttlghb.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jinghuilouyu.cn/gtcjkkbtmb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yangfankeji.com/gtnzmrgzvk.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hysaishi.cn/gtyorntgza.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.guannengcc.top/gtidxgocno.html

[J06] 计算两时间之差
来源：http://hz.shuidangran.top/gtsmwgiqov.html

Py:   (end - start).total_seconds()
来源：http://hz.jianghu66.top/gtdrxsmocq.html

PHP:  $end->diff($start)->days;
来源：http://hz.chenzaomai.com/gtmrcrkisp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.cdnleiting.top/gtbowbcafu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cashguo.top/gtrhxfsnvg.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.zhoulong.xyz/gtlhrhtuaa.html

Go:   end.Sub(start).Hours()
来源：http://hz.daxiang520.top/gttjgadaxq.html

Ruby: end - start                 # 返回秒数
来源：http://hz.ehwqpu.com/gtowpxwsqf.html

C#:   (end - start).TotalSeconds
来源：http://hz.yongpay.top/gtvwiqdvnp.html

[J07] 比较两个日期
来源：http://hz.0kj1m.cn/gtjsjopqiu.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.316326.xyz/gtwzytzzdr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.havefunace.top/gtccsgsdqn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jlsjyb.cn/gtehizojoa.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.zhengqikj.top/gtkrfypoet.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ywan-chungtsiang.top/gtsmwiharx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yonumen.top/gtmpheljep.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.bjfxy.top/gtcscnvdyh.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ehwqpu.com/gtjlzetiov.html

[J08] 提取年月日与星期
来源：http://hz.fzhhl.top/gtkcjzjabz.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yongpay.top/gtdwwxbvlj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.tian-w.cn/gttfdgclbm.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.andypj.xyz/gthcozghzx.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yuanzhike.top/gtlqpzyqzo.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jqgufenzy.top/gtnumlzems.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.tanke756.top/gtltyipvvy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.jqgfzy.top/gtnnqohngd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.chenjidiqi.icu/gtdnuczmkh.html

[J09] 时区处理
来源：http://hz.yuanzhike.top/gtqbugxvvp.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.haohaochexian.top/gtvamggomg.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jiagoushi.top/gtfwedinra.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sysykeji.top/gtfzcztjas.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj202588.top/gtlakisksm.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.gogol.net.cn/gtzdoyoehj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.vqdsnc.cn/gtqigbajyl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.guannengcc.top/gtcowrkzam.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhengqikj.top/gtkuleoeri.html

[J10] 取今天 / 本月第一天
来源：http://hz.smart0.xyz/gtjilduggf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.hnxiangtu.top/gtsoyajkel.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.shangyingyoupin.top/gtizfhocge.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.nwbrower.top/gtrrejvaef.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jinghuilouyu.cn/gtqcvbysgp.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.svipenyu.cn/gtfrrmbqgm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xingfuxueyuan.xyz/gttmfiznqm.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.zhijiandao.cn/gtuzwkeqvm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.nanxuanxn.top/gthkxqskri.html

================================================================================
来源：http://hz.ydzc1.top/gtskgfvwlt.html

K. JSON 与序列化
来源：http://hz.cucudq.cn/gtmbkbfwbf.html

================================================================================
来源：http://hz.yangfankeji.com/gtqeoyjxno.html

[K01] 对象转 JSON 字符串
来源：http://hz.shuidangran.top/gtwgjcscux.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jianghu66.top/gtrayqriqx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.guowangkeji.top/gtpuribrtm.html

JS:   JSON.stringify(obj)
来源：http://hz.shanyushiyangkeji.top/gtpjdkmqij.html

TS:   JSON.stringify(obj)
来源：http://hz.cheryme.top/gtuqxgmvkd.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.iojbl.cn/gtnkbchynn.html

Go:   json.Marshal(obj)
来源：http://hz.zhaomingkeji.xyz/gtcxaiebby.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.chenlongwang.top/gtaxaojaxh.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.hywenlv.cn/gtemhgjbgj.html

[K02] JSON 字符串转对象
来源：http://hz.quarkkingdee.top/gtsrweifsc.html

Py:   json.loads(s)
来源：http://hz.redwolf501.top/gtlulfdivt.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.daria6918.cn/gtgoyjzgrw.html

JS:   JSON.parse(s)
来源：http://hz.cheryme.top/gtoaowkjxh.html


<!-- 参考信息 -->