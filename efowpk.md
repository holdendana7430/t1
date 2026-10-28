代发 wailian999

TS:   type User = { name: string; age: number };
来源：http://hz.zhongyouzk.top/gtgszovuip.html

Java: record User(String name, int age) {}
来源：http://hz.mhx1999.top/gtskpiehxw.html

Go:   type User struct { Name string; Age int }
来源：http://hz.redwolf501.top/gtjfmziixw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xingfuxueyuan.xyz/gtrlykzctm.html

C#:   record User(string Name, int Age);
来源：http://hz.redwolf501.top/gtghgglysi.html

[G15] 枚举
来源：http://hz.cashguo.top/gtjzpmksbx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.nanxuanxn.top/gtrzjqqwpk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.hnqzz.top/gtedqvrknh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.ywan-chungtsiang.top/gtrrndbifr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hnqzz.top/gthmbygybn.html

Java: enum Color { RED, GREEN }
来源：http://hz.ydjk.org.cn/gtsdenxfyf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.aizwys.cn/gtkbecooft.html

Ruby: Color = %i[red green].freeze
来源：http://hz.vqdsnc.cn/gtsyoxqvjv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xylfe.cn/gtthlhxecq.html

[G16] 对象转数组 / 字典
来源：http://hz.nanxuanxn.top/gtoiiheryb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.xingfuxueyuan.xyz/gtlwaffjtz.html

PHP:  get_object_vars($obj);
来源：http://hz.hysaishi.cn/gtyqeeopjj.html

JS:   Object.entries(obj)
来源：http://hz.tanke756.top/gteuxgxkfx.html

TS:   Object.entries(obj)
来源：http://hz.yangfankeji.com/gtrudnhfki.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.mhx1999.top/gtjbvjrgtg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jinyuanbaomall.cn/gtakcrfify.html

Ruby: obj.instance_variables
来源：http://hz.cdnleiting.top/gtwegrxvem.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ywan-chungtsiang.top/gtaeytalvc.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtcfnnslhz.html

H. 异常与错误处理
来源：http://hz.hammf.cn/gtvlyyilft.html

================================================================================
来源：http://hz.guowangkeji.top/gtspamcytm.html

[H01] try / catch 基础
来源：http://hz.yueranfly.top/gtxmhhhwuv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xinyue.icu/gtjdtqqrcd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.guowangkeji.top/gtpxshxbxb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hammf.cn/gtqqfezvmx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.yongpay.top/gtmwvhgcft.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.birdmap.top/gthbihkmss.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.hysaishi.cn/gtonshapdg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.mhx1999.top/gtuekednxg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.daxiang520.top/gtckjqfwwz.html

[H02] finally / ensure 收尾
来源：http://hz.pengpengdd.cyou/gtxkovotzd.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.xuetiantiany.cn/gtolyywvlu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.aibaodan.cn/gtomjnmtpl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.quarkkingdee.top/gtpinmcouw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xylfe.cn/gtzwammrna.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gtzvedvjla.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.pengpengdd.cyou/gtaumwkudh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.yvedp.cn/gtwnwblxaa.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.sysykeji.top/gtdeawemaa.html

[H03] 主动抛出异常
来源：http://hz.yanxiufei.cn/gtylzhhksj.html

Py:   raise ValueError("错误信息")
来源：http://hz.zhijiandao.cn/gtaakijmxz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.wangdashe.top/gtlmrwozso.html

JS:   throw new Error("错误信息");
来源：http://hz.ydjk.org.cn/gttilxkczy.html

TS:   throw new Error("错误信息");
来源：http://hz.bjfxy.top/gtxqavjxnk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.birdmap.top/gtwiogsjve.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhixingplan.top/gtjmugajtv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhiwuduotai.top/gtufrmghbg.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yvedp.cn/gtdiklvbbn.html

[H04] 自定义异常类型
来源：http://hz.fzhhl.top/gtozkgxktq.html

Py:   class MyError(Exception): pass
来源：http://hz.nanxinkj.top/gtynoknrvu.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zhixingplan.top/gtpztqzmpd.html

JS:   class MyError extends Error {}
来源：http://hz.shanyushiyangkeji.top/gtsyndkujp.html

TS:   class MyError extends Error {}
来源：http://hz.9152youxi.cn/gtftenawpz.html

Java: class MyException extends RuntimeException {}
来源：http://hz.feifeiyinyue.top/gtqwqogvje.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.bjfxy.top/gthepoexzw.html

Ruby: class MyError < StandardError; end
来源：http://hz.hammf.cn/gtcgmbottn.html

C#:   class MyException : Exception {}
来源：http://hz.fzhhl.top/gtasjenxjs.html

[H05] 捕获特定类型
来源：http://hz.andypj.xyz/gtrbolcqrl.html

Py:   except ValueError as e:
来源：http://hz.jlsjyb.cn/gtbqcgjemb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.nanxinkj.top/gtjuxujtgq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.kuanghao11.cn/gtgtaderga.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.c1oappe.top/gtjrluwpun.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.redwolf501.top/gtdouvvccy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.iojbl.cn/gtfolkdwrw.html

Ruby: rescue ArgumentError => e
来源：http://hz.smart0.xyz/gthdovaovu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.wangdashe.top/gtvvurblel.html

[H06] 可选值 / 空值安全访问
来源：http://hz.tian-w.cn/gtohnnriul.html

Py:   value = d.get("k") or default
来源：http://hz.hysaishi.cn/gtnvtqcjia.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ydjk.org.cn/gtmqapoqof.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.c1oappe.top/gtkbvvqzld.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yongpay.top/gtdfbywjkj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zdqjudy.top/gtwmgajjab.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.316326.xyz/gtnhmojqae.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ivvv.top/gtcacwpokw.html

C#:   obj?.A?.B ?? default
来源：http://hz.jianghu66.top/gtmsgcutid.html

[H07] 断言
来源：http://hz.hysaishi.cn/gtkhwgafid.html

Py:   assert x > 0, "必须为正"
来源：http://hz.jinghuilouyu.cn/gtteuhidum.html

PHP:  assert($x > 0);
来源：http://hz.hysaishi.cn/gtiphmqnzx.html

JS:   console.assert(x > 0);
来源：http://hz.yongpay.top/gtxslmaqdb.html

TS:   console.assert(x > 0);
来源：http://hz.fzhhl.top/gtrpzlgjfb.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jinqigufen.top/gthlvcjqme.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cqqwz.cn/gtpilykbbm.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hammf.cn/gtqeamhldq.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhixingplan.top/gtkmyqpgzx.html

[H08] 获取错误信息与堆栈
来源：http://hz.aizwys.cn/gtdfijuwfh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jlsjyb.cn/gtwtoviutv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.nanxinkj.top/gtvhueipqp.html

JS:   e.message;  e.stack
来源：http://hz.xziqi.cn/gtlzrythmx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yanxiufei.cn/gtfnqbinpm.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gotoacloud.top/gtcgfhzgcy.html

Go:   err.Error()
来源：http://hz.guannengcc.top/gtzvawyiih.html

Ruby: e.message;  e.backtrace
来源：http://hz.yuxming.cn/gtloczwqjq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.aizwys.cn/gtqpyyfrpz.html

[H09] 带错误码的异常
来源：http://hz.wangdashe.top/gtkwcuzckm.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.redwolf501.top/gtehaljpvd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.tianlin.xyz/gtuvugmvyy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.meibo888.top/gtbobxpvch.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yj20258.top/gtuzjuexnd.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hnqzz.top/gtxocvuaqp.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hammf.cn/gtcivizmfw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.sufxvd.cn/gtfpstopkb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gaohongyu789.top/gtyoczzirj.html

[H10] 资源自动释放
来源：http://hz.zhongyouzk.top/gtcjcxsmww.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yj20258888.top/gtlrgodbat.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhijiandao.cn/gtqadnzgkn.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.tanke756.top/gtxzrxipiy.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sxryk.cn/gtzhwrlxdn.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.dashuyun.cn/gtuzsjdgyf.html

Go:   defer f.Close()
来源：http://hz.quarkkingdee.top/gtimvowxkp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.feifeiyinyue.top/gtmfuefdrr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.gotoacloud.top/gthtiolqdw.html

================================================================================
来源：http://hz.hnqzz.top/gtqvcmwidw.html

I. 正则表达式
来源：http://hz.wangdashe.top/gtlundoxem.html

================================================================================
来源：http://hz.jinqigfzy.top/gtkjujrpkb.html

[I01] 判断是否匹配
来源：http://hz.yongpay.top/gtckayzqmr.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zycfv.cn/gticqvxegx.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.birdmap.top/gtqbktayhe.html

JS:   /\d+/.test(s)
来源：http://hz.jinqigfzy.top/gtofggjvue.html

TS:   /\d+/.test(s)
来源：http://hz.gzhubu.top/gtiydojkrj.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gotoacloud.top/gthrjybbfg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.pycfn.com/gtvohmiaqz.html

Ruby: s.match?(/\d+/)
来源：http://hz.cashguo.top/gtjqqsiyzf.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinghuilouyu.cn/gthdnemwyl.html

[I02] 提取所有匹配
来源：http://hz.nwbrower.top/gtymsrmdtn.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinghuilouyu.cn/gtrwuhppdv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.fengsongda.top/gthkvymych.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.chenzaomai.com/gtwmpbwpcb.html

TS:   s.match(/\d+/g)
来源：http://hz.hywenlv.cn/gtotgltcew.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cqqwz.cn/gtabutapdm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.birdmap.top/gtfrpnjfma.html

Ruby: s.scan(/\d+/)
来源：http://hz.zycfv.cn/gtxtaypxxs.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.quarkkingdee.top/gtwohmvziq.html

[I03] 提取捕获分组
来源：http://hz.ehwqpu.com/gtyewgrceg.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cheryme.top/gtfemngfqx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.nwbrower.top/gtbqzfbbak.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xuanzx.com/gtfncdwldr.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.wangdashe.top/gtonxgpcfg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.tianlin.xyz/gtgeilfzvy.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xuetiantiany.cn/gtbutwunho.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yongpay.top/gtaptzkhid.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.jianghu66.top/gtgbltxssf.html

[I04] 正则替换
来源：http://hz.haohaochexian.top/gtgjdsnojo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.sufxvd.cn/gtyrhxdanf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.daxiang520.top/gtjidncqem.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.redwolf501.top/gtbxydaltr.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jinghuilouyu.cn/gtzpyasadh.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.guannengcc.top/gtcbxiupxz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.zhixingplan.top/gtcgovndhw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gogol.net.cn/gthuapgbwj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.iojbl.cn/gtrwlwbxfj.html

[I05] 按正则拆分
来源：http://hz.316326.xyz/gtjmkncfzz.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.shanyushiyangkeji.top/gtgmlpduwv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gzhubu.top/gtxywldntg.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.hnqzz.top/gthfcowepf.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.andypj.xyz/gtqbqcthki.html

Java: s.split("\\s*,\\s*")
来源：http://hz.sweek.top/gthedteofs.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.sxryk.cn/gtvxcbwjfq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.havefunace.top/gtwicdpntd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhengqikj.top/gtyqexwepc.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.smart0.xyz/gtmjpriefr.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.zhongyouzk.top/gtrsmzlqer.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.c1oappe.top/gtwsgjejrs.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tianlin.xyz/gtjvbcujxg.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.xingfuxueyuan.xyz/gtghbfrvbb.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.yanxiufei.cn/gtoegawdby.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yonumen.top/gtooddrbdm.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.c1oappe.top/gtlgspjrev.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.xylfe.cn/gtzmsuvuza.html

[I07] 忽略大小写与多行模式
来源：http://hz.pengpengdd.cyou/gttnmgapvh.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhaomingkeji.xyz/gtnjknspct.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.jinyuanbaomall.cn/gtnkfhfvpa.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xylfe.cn/gtnbhcopdv.html

TS:   /error/gim
来源：http://hz.meibo888.top/gtghmhhmsi.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jinqigufen.top/gtgwaohzkl.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.havefunace.top/gtvhuqhyir.html

Ruby: s.scan(/error/i)
来源：http://hz.zhixingplan.top/gtilhwkagb.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinyuanbaomall.cn/gtbzfxnedz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ydjk.org.cn/gtyuvxziwt.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.ybcxt.top/gtfbxawauj.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ywan-chungtsiang.top/gtlrmceubb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.vqdsnc.cn/gttybgvsjw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.316326.xyz/gthlnytjzl.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yueranfly.top/gtijoitayj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cucudq.cn/gtysjgquix.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.hfpthk.cn/gtjrajlexz.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jyoumei.cn/gtmhwtsbwy.html

================================================================================
来源：http://hz.yj20258888.top/gtqzxboegr.html

J. 日期与时间
来源：http://hz.cdnleiting.top/gtoegpyqkf.html

================================================================================
来源：http://hz.gogol.net.cn/gtodcajvqv.html

[J01] 获取当前时间
来源：http://hz.xziqi.cn/gtgprpbcpr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shangyingyoupin.top/gtvgeneugz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.nanxinkj.top/gttfptzzac.html

JS:   new Date();  Date.now()
来源：http://hz.andypj.xyz/gtnebipywb.html

TS:   new Date();  Date.now()
来源：http://hz.cucudq.cn/gtnspkmhwf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.0kj1m.cn/gtdfptqkfd.html

Go:   time.Now()
来源：http://hz.mhx1999.top/gtlhyrjvjo.html

Ruby: Time.now
来源：http://hz.316326.xyz/gtsqtxwzrm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yuxming.cn/gtddeqcgia.html

[J02] 格式化输出
来源：http://hz.yueranfly.top/gtwnsyplcu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenzaomai.com/gtjxglwovr.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.shuidangran.top/gtekxmlidb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.pengpengdd.cyou/gtubvhhvlp.html

TS:   d.toISOString()
来源：http://hz.nanxinkj.top/gthzhivtgg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.guowangkeji.top/gtiiuzomzr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tian-w.cn/gtbcoixqfk.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.daxiang520.top/gttqwrecoe.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hammf.cn/gtvuwxmees.html

[J03] 字符串解析为日期
来源：http://hz.jqgufenzy.top/gtleoqjlkg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.zhixingplan.top/gtggjjyhkj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yuxming.cn/gtexupplwc.html

JS:   new Date("2024-01-02")
来源：http://hz.yangfankeji.com/gtjjrjzurz.html

TS:   new Date("2024-01-02")
来源：http://hz.yuanzhike.top/gtbgdyrmgx.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.iojbl.cn/gtbfllgsxg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xinyue.icu/gtxohdqcdf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtmytaopuc.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj202588.top/gtebafainm.html

[J04] 时间戳与日期互转
来源：http://hz.jianghu66.top/gtlhhokcxe.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.chenzaomai.com/gteuwydxbl.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ehwqpu.com/gteaahvpda.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jianghu66.top/gtsthqpqzi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.sxryk.cn/gtqvjrikjh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.nwbrower.top/gtqzucogap.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jiagoushi.top/gteohefeix.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hysaishi.cn/gtthdcnxai.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ydjk.org.cn/gtggpgntmu.html

[J05] 时间加减（加 7 天）
来源：http://hz.daria6918.cn/gtinhimhpp.html

Py:   now + timedelta(days=7)
来源：http://hz.shangyingyoupin.top/gtjzqswjfe.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.vqdsnc.cn/gtnwctdioo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aibaodan.cn/gtbtzeghqj.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.mhx1999.top/gtinepawlw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.fengsongda.top/gtbkxgndlf.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xuanzx.com/gtscbdanxi.html

Ruby: Time.now + 7 * 86400
来源：http://hz.zhaomingkeji.xyz/gtyjkslryp.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.c1oappe.top/gtnymsuxhg.html

[J06] 计算两时间之差
来源：http://hz.cdnleiting.top/gtgpnepnzn.html

Py:   (end - start).total_seconds()
来源：http://hz.hywenlv.cn/gturddmvak.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhaomingkeji.xyz/gtbuqjapiw.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.c1oappe.top/gtvunebuqk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.chenzaomai.com/gtxpzzbbwr.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.dashuyun.cn/gtnmveyhfw.html

Go:   end.Sub(start).Hours()
来源：http://hz.fengsongda.top/gtbzqnuxpm.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jinqigufen.top/gtanabfhwr.html

C#:   (end - start).TotalSeconds
来源：http://hz.wangdashe.top/gtepkfqino.html

[J07] 比较两个日期
来源：http://hz.9152youxi.cn/gtyqkpyfoh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shzxlz.cn/gtguhmyzhf.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.ydjk.org.cn/gtmebkhkyo.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shangyingyoupin.top/gtwzjetvxi.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.haohaochexian.top/gtkquvjynl.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cqqwz.cn/gtzlvikcqw.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zdqjudy.top/gtqytlnqnl.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gtpdylwlls.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.meibo888.top/gtdykhzjwi.html

[J08] 提取年月日与星期
来源：http://hz.gaohongyu789.top/gtsbsbagef.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.ivvv.top/gtkxmfrpdm.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jinghuilouyu.cn/gtlbxvndjv.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jyoumei.cn/gtfvyrzcdh.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ppjwa.cn/gtobltxzfr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hnqzz.top/gtpqdrhxab.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.pengpengdd.cyou/gtsygfljan.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yvedp.cn/gtolzwliui.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.ehwqpu.com/gtxiihtciv.html

[J09] 时区处理
来源：http://hz.cucudq.cn/gtscywhlzv.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yangfankeji.com/gtqlchokrr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xziqi.cn/gterhlyncu.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sufxvd.cn/gtmsrhivpy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.fengsongda.top/gtowbfslog.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.mhx1999.top/gtawedpzjc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.sysykeji.top/gtrrufzypw.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.hysaishi.cn/gtqqsfzbei.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.haohaochexian.top/gtwizcbfxg.html

[J10] 取今天 / 本月第一天
来源：http://hz.daxiang520.top/gtwyhnlzlv.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.chenzaomai.com/gtjidczzzg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.sufxvd.cn/gtmfhoixhr.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.ydzc1.top/gthoesblnl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.zdqjudy.top/gtenkferid.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhoulong.xyz/gtxracufoz.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.havefunace.top/gthqzlmokp.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.ydjk.org.cn/gtddeafufj.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.jyoumei.cn/gthdqighfz.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtekoypcqm.html

K. JSON 与序列化
来源：http://hz.ydjk.org.cn/gteqpxjqqr.html

================================================================================
来源：http://hz.birdmap.top/gteqneajcj.html

[K01] 对象转 JSON 字符串
来源：http://hz.hfpthk.cn/gtqrjeuynz.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.jinyuanbaomall.cn/gtswhftovd.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.cheryme.top/gtnovhfxte.html

JS:   JSON.stringify(obj)
来源：http://hz.wangshuangyany.cn/gtitkcbleq.html

TS:   JSON.stringify(obj)
来源：http://hz.gaohongyu789.top/gtbfwrlvrw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.aibaodan.cn/gtqwxfskyi.html

Go:   json.Marshal(obj)
来源：http://hz.jyoumei.cn/gthbqaazhf.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.jqgufenzy.top/gtffuncxmr.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.jinqigfzy.top/gteyaazodd.html

[K02] JSON 字符串转对象
来源：http://hz.fengsongda.top/gtwqjuqhsq.html

Py:   json.loads(s)
来源：http://hz.zycfv.cn/gtegybzadb.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hz.yuxming.cn/gtqjhepkoe.html

JS:   JSON.parse(s)
来源：http://hz.ehwqpu.com/gtungjvjwa.html


<!-- 参考信息 -->