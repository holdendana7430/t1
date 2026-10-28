代发 wailian999

Py:   isinstance(u, User)
来源：http://hz.hnxiangtu.top/gtbyzvskyt.html

PHP:  $u instanceof User
来源：http://hz.yueranfly.top/gtbefbcmqf.html

JS:   u instanceof User
来源：http://hz.zycfv.cn/gtcustofjv.html

TS:   u instanceof User
来源：http://hz.zhaomingkeji.xyz/gtzrtuqncb.html

Java: u instanceof User
来源：http://hz.aizwys.cn/gttkcxtior.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jqgufenzy.top/gtvmkovcao.html

Ruby: u.is_a?(User)
来源：http://hz.shzxlz.cn/gtbzoluqrr.html

C#:   u is User
来源：http://hz.gotoacloud.top/gtfypkzbjx.html

[G14] 数据类 / record
来源：http://hz.hnqzz.top/gtipidwodk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.c1oappe.top/gtkinxuhlg.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.redwolf501.top/gtxwpwfxds.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ivvv.top/gtpbmomqly.html

TS:   type User = { name: string; age: number };
来源：http://hz.ivvv.top/gtulxhrswi.html

Java: record User(String name, int age) {}
来源：http://hz.hnqzz.top/gtewgryxdc.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yonumen.top/gtidcurwnd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yj20258888.top/gtbdfltrcu.html

C#:   record User(string Name, int Age);
来源：http://hz.shanyushiyangtech.top/gtpjdkyewi.html

[G15] 枚举
来源：http://hz.yvedp.cn/gtxbztlfzu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.aibaodan.cn/gtcqktpinr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhongyouzk.top/gtqqkvgmvu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yangfankeji.com/gtbwekqthu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nanxinkj.top/gtrabkyxev.html

Java: enum Color { RED, GREEN }
来源：http://hz.yuanzhike.top/gtgjemtzic.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yj20258.top/gtdnicvpee.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zycfv.cn/gteekishgk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.cashguo.top/gtvtrmynpl.html

[G16] 对象转数组 / 字典
来源：http://hz.vqdsnc.cn/gtxgcjpiqy.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zdqjudy.top/gtpbanodwf.html

PHP:  get_object_vars($obj);
来源：http://hz.xingfuxueyuan.xyz/gtnzynmxgo.html

JS:   Object.entries(obj)
来源：http://hz.zhengqikj.top/gtanobzyov.html

TS:   Object.entries(obj)
来源：http://hz.xinyue.icu/gtxkxkwbho.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhongyouzk.top/gtoigcrdcm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jinqigfzy.top/gtxlimwwof.html

Ruby: obj.instance_variables
来源：http://hz.yangfankeji.com/gtiudosqtn.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xziqi.cn/gttfkrazgf.html

================================================================================
来源：http://hz.jinqigfzy.top/gtteannwao.html

H. 异常与错误处理
来源：http://hz.gaohongyu789.top/gttqvehkxa.html

================================================================================
来源：http://hz.hnxiangtu.top/gtkuqkldcb.html

[H01] try / catch 基础
来源：http://hz.jinghuilouyu.cn/gtteduoeml.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jiagoushi.top/gtrvnkfodo.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.9152youxi.cn/gtangkluqk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.zhijiandao.cn/gtlpiqesjo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.dashuyun.cn/gtaxkkfatx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zhongyouzk.top/gthlqjvdmp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.xingfuxueyuan.xyz/gtpvgtkuwf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.9152youxi.cn/gtxftyjlcg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.jiagoushi.top/gtnqimhmzp.html

[H02] finally / ensure 收尾
来源：http://hz.svipenyu.cn/gtrhyemddr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sxryk.cn/gtnuobeiqj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.tianlin.xyz/gtmkvqzhbv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gtgjaggofc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gtxnbvljfe.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtnoooaiao.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.havefunace.top/gtvcmqcyxs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.dashuyun.cn/gtnvkvxxgc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jqgufenzy.top/gtabrikpuk.html

[H03] 主动抛出异常
来源：http://hz.jinghuilouyu.cn/gtfpkkjgjq.html

Py:   raise ValueError("错误信息")
来源：http://hz.hywenlv.cn/gtsrfzgbur.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jlsjyb.cn/gtniqkrccp.html

JS:   throw new Error("错误信息");
来源：http://hz.meibo888.top/gtxsudpewk.html

TS:   throw new Error("错误信息");
来源：http://hz.sweek.top/gtdlqabxko.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.zhongyouzk.top/gtmzyespjy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhiwuduotai.top/gtixzodffn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.dianchejie.cn/gtszaepljt.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtenbsnkwz.html

[H04] 自定义异常类型
来源：http://hz.pengpengdd.cyou/gtknwoeydn.html

Py:   class MyError(Exception): pass
来源：http://hz.sufxvd.cn/gtrypcwjru.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.tanke756.top/gtockmyjqg.html

JS:   class MyError extends Error {}
来源：http://hz.yj20258888.top/gtpbgtyerm.html

TS:   class MyError extends Error {}
来源：http://hz.c1oappe.top/gtpxlrutth.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hfpthk.cn/gtfrvnqqdp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.dianchejie.cn/gtubfxqezn.html

Ruby: class MyError < StandardError; end
来源：http://hz.ivvv.top/gtdhplpoah.html

C#:   class MyException : Exception {}
来源：http://hz.yuxming.cn/gtopudvejv.html

[H05] 捕获特定类型
来源：http://hz.xuetiantiany.cn/gtbxwxzycv.html

Py:   except ValueError as e:
来源：http://hz.xziqi.cn/gtkbuiszkr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yangfankeji.com/gtlguppzid.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.nanxuanxn.top/gtdlsjosjb.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.cucudq.cn/gtvrworojx.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.tianlin.xyz/gtstlizldg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xinyue.icu/gthgrihlfm.html

Ruby: rescue ArgumentError => e
来源：http://hz.svipenyu.cn/gtmwubvszb.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xuetiantiany.cn/gthvcsswzz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.daxiang520.top/gtuebvklqp.html

Py:   value = d.get("k") or default
来源：http://hz.havefunace.top/gtzfnevfqc.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.meibo888.top/gtbljalprt.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.sweek.top/gtskicahwy.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xinyue.icu/gtgtgrbgto.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hfpthk.cn/gtcqwhvuhg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sufxvd.cn/gtyfxnyesu.html

Ruby: d&.dig(:a, :b)
来源：http://hz.feifeiyinyue.top/gtitltufxs.html

C#:   obj?.A?.B ?? default
来源：http://hz.52xcode.cn/gtqlplawpb.html

[H07] 断言
来源：http://hz.svipenyu.cn/gtcwtwmmbu.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cucudq.cn/gtxxncbwlh.html

PHP:  assert($x > 0);
来源：http://hz.sxryk.cn/gtwdtznajz.html

JS:   console.assert(x > 0);
来源：http://hz.gzhubu.top/gtnibtnjlz.html

TS:   console.assert(x > 0);
来源：http://hz.yj202588.top/gtuilkhsdz.html

Java: assert x > 0 : "必须为正";
来源：http://hz.dashuyun.cn/gtumukkwyt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.guannengcc.top/gtoiubqgfq.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.bjfxy.top/gtvfevampu.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shanyushiyangtech.top/gtyhelrtva.html

[H08] 获取错误信息与堆栈
来源：http://hz.tanke756.top/gtpuaivrsh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.c1oappe.top/gtcqeikztd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.hywenlv.cn/gtpyvevcah.html

JS:   e.message;  e.stack
来源：http://hz.zhoulong.xyz/gttprcavhb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhixingplan.top/gtpxlwzvby.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.daria6918.cn/gtylagfvuu.html

Go:   err.Error()
来源：http://hz.chenlongwang.top/gtanbnfmtc.html

Ruby: e.message;  e.backtrace
来源：http://hz.xuanzx.com/gtvqvmahnx.html

C#:   e.Message;  e.StackTrace
来源：http://hz.chenzaomai.com/gtlskxdzsw.html

[H09] 带错误码的异常
来源：http://hz.zhengqikj.top/gtunvtevwr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jinghuilouyu.cn/gtzplprzdy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.meibo888.top/gtrmnsvufx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.vqdsnc.cn/gtufprgyeq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yvedp.cn/gtkscllvgz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cqqwz.cn/gtwkkzhscl.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.zhaomingkeji.xyz/gtjvilkvxw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jlsjyb.cn/gtbbybqosb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.birdmap.top/gtbjgqiqop.html

[H10] 资源自动释放
来源：http://hz.jinghuilouyu.cn/gtbsvdcktg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.bjfxy.top/gtocjjvhbd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.sweek.top/gtbedqxids.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangtech.top/gtiojmrowb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jianghu66.top/gtuhbalcli.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sxryk.cn/gtxwglqtyp.html

Go:   defer f.Close()
来源：http://hz.yangfankeji.com/gtqydivuuj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shangyingyoupin.top/gtihidfkqw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ywan-chungtsiang.top/gtqohdgoqt.html

================================================================================
来源：http://hz.ybcxt.top/gtxxrewuyp.html

I. 正则表达式
来源：http://hz.yongpay.top/gteqzzlbcf.html

================================================================================
来源：http://hz.sweek.top/gtsoxgpolc.html

[I01] 判断是否匹配
来源：http://hz.dianchejie.cn/gtjsfxpsmd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.shanyushiyangtech.top/gtqsjoipww.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.snrcjt.cn/gtntptpzvr.html

JS:   /\d+/.test(s)
来源：http://hz.hysaishi.cn/gtnihzuqek.html

TS:   /\d+/.test(s)
来源：http://hz.yj202588.top/gtmxpvwaia.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.daxiang520.top/gttdtcbubl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yuxming.cn/gtzxwyevex.html

Ruby: s.match?(/\d+/)
来源：http://hz.guowangkeji.top/gtzsjzepvp.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yj20258888.top/gthqggpfqb.html

[I02] 提取所有匹配
来源：http://hz.c1oappe.top/gtgjrrswgm.html

Py:   re.findall(r"\d+", s)
来源：http://hz.mhx1999.top/gttulqtzxw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.nanxuanxn.top/gtdyyrwpxv.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jqgfzy.top/gtqfpikysm.html

TS:   s.match(/\d+/g)
来源：http://hz.hnxiangtu.top/gtbngsefas.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.yuxming.cn/gtnadhumzv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.aibaodan.cn/gtmfksurzg.html

Ruby: s.scan(/\d+/)
来源：http://hz.cdnleiting.top/gtmyfwfvzv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.c1oappe.top/gtchufxomt.html

[I03] 提取捕获分组
来源：http://hz.hongshengwenyu.top/gtlcyzthsa.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhoulong.xyz/gtfmupbrsz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.316326.xyz/gthehboeqk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.wangshuangyany.cn/gtdqjfxnzs.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jinqigufen.top/gtvdnkzlff.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhengqikj.top/gtlwbgvbxr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.tian-w.cn/gtnieezxsy.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shzxlz.cn/gtqbkbtais.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.xziqi.cn/gtjwqjldms.html

[I04] 正则替换
来源：http://hz.cqqwz.cn/gthuyrcati.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.feifeiyinyue.top/gtvnxnksqf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.gogol.net.cn/gtntkarfjk.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.kuanghao11.cn/gtjtgsvtpk.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yonumen.top/gtldlzswte.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.fengsongda.top/gtvmyvkgvb.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.aizwys.cn/gtscwltrwr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shanyushiyangkeji.top/gtmtjpooyz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.hysaishi.cn/gttacrsbhq.html

[I05] 按正则拆分
来源：http://hz.svipenyu.cn/gttghjdhvy.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.guowangkeji.top/gtulsisroo.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.zhongyouzk.top/gtejpvzkis.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yanxiufei.cn/gtalcshdla.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.52xcode.cn/gtkqvefmxq.html

Java: s.split("\\s*,\\s*")
来源：http://hz.bjfxy.top/gtcnsfnlml.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jinyuanbaomall.cn/gtgcdslluo.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhixingplan.top/gtfouvuspm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.chenlongwang.top/gtddcwbufj.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.andypj.xyz/gtturnsrbw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.snrcjt.cn/gtltrbnehz.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.redwolf501.top/gtxacikmgq.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ywan-chungtsiang.top/gtsrubvark.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinqigufen.top/gtkeypljpg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zycfv.cn/gttzdlrfic.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gzhubu.top/gtyupvtfse.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.ydjk.org.cn/gtlwffyppg.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gtfgrlusbm.html

[I07] 忽略大小写与多行模式
来源：http://hz.redwolf501.top/gtiiorpjej.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shangyingyoupin.top/gtzclqorkz.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.daxiang520.top/gtuahwpalf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xuanzx.com/gtcdawbsmf.html

TS:   /error/gim
来源：http://hz.jinyuanbaomall.cn/gtrzfuthdh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gzhubu.top/gtcdxbxvul.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.sweek.top/gtzowetpxk.html

Ruby: s.scan(/error/i)
来源：http://hz.yuanzhike.top/gtbjkrtbft.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhengqikj.top/gtjksqvngg.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.shanyushiyangtech.top/gtetgkxrby.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xylfe.cn/gtxhwpjipm.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ivvv.top/gtwhbfmnzp.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.snrcjt.cn/gtcdebtntj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hfpthk.cn/gtiisoanmd.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yuanzhike.top/gtrolojcin.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.xuetiantiany.cn/gtywbalbrt.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.quarkkingdee.top/gtzqglhzlu.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.pengpengdd.cyou/gtpmixpvoj.html

================================================================================
来源：http://hz.gzhubu.top/gtyqetqask.html

J. 日期与时间
来源：http://hz.hongshengwenyu.top/gthbzlswkn.html

================================================================================
来源：http://hz.zhixingplan.top/gtsmpmhzqt.html

[J01] 获取当前时间
来源：http://hz.shzxlz.cn/gtgmonhqyr.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.9152youxi.cn/gtmxnrotvh.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yuanzhike.top/gtxarkltls.html

JS:   new Date();  Date.now()
来源：http://hz.hongshengwenyu.top/gtihqrwzxf.html

TS:   new Date();  Date.now()
来源：http://hz.pengpengdd.cyou/gtffxoorgv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinqigfzy.top/gtgemlstdy.html

Go:   time.Now()
来源：http://hz.chenlongwang.top/gtbvzlrfcw.html

Ruby: Time.now
来源：http://hz.vqdsnc.cn/gtgqienafg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jqgufenzy.top/gtefzggchq.html

[J02] 格式化输出
来源：http://hz.pengpengdd.cyou/gtndfldplu.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.svipenyu.cn/gtgsjrtpkm.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.316326.xyz/gtmzexbagy.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.birdmap.top/gtgxedrbaa.html

TS:   d.toISOString()
来源：http://hz.yongpay.top/gtrxzlqbdi.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.316326.xyz/gtqtppkkgo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.guannengcc.top/gtxjvklwmh.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.chenzaomai.com/gtdmqyqwqm.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yueranfly.top/gtkwxppqjt.html

[J03] 字符串解析为日期
来源：http://hz.zycfv.cn/gtuhojyrgx.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.gogol.net.cn/gtoacjrspu.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cashguo.top/gtiblggdlf.html

JS:   new Date("2024-01-02")
来源：http://hz.tian-w.cn/gtzsfhpmwa.html

TS:   new Date("2024-01-02")
来源：http://hz.jqgufenzy.top/gtuisjfmpw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xziqi.cn/gtasfheczt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhengqikj.top/gtfzuwpfuv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zycfv.cn/gtinojdowv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj20258888.top/gtkxtluohd.html

[J04] 时间戳与日期互转
来源：http://hz.quarkkingdee.top/gthwqkijii.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xuanzx.com/gtwkyratyj.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.chenjidiqi.icu/gtksfpxnju.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.hywenlv.cn/gtichhqzks.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.andypj.xyz/gtpgpdguok.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.sxryk.cn/gtybcbmmbo.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhoulong.xyz/gtenyhbkvt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cqqwz.cn/gturtgvvud.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ydzc1.top/gtdqgcllpj.html

[J05] 时间加减（加 7 天）
来源：http://hz.cqqwz.cn/gtyjbqqswp.html

Py:   now + timedelta(days=7)
来源：http://hz.ppjwa.cn/gtkvyadsvi.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.fzhhl.top/gtbtyijwag.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jinghuilouyu.cn/gtowcasvbn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yonumen.top/gttuacfxob.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.meibo888.top/gtspgickiu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shuidangran.top/gtlvecrkmg.html

Ruby: Time.now + 7 * 86400
来源：http://hz.iojbl.cn/gtafpojwlr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xuanzx.com/gtekvdgqcx.html

[J06] 计算两时间之差
来源：http://hz.yj20258.top/gtmxicngwr.html

Py:   (end - start).total_seconds()
来源：http://hz.52xcode.cn/gtyaiyukjh.html

PHP:  $end->diff($start)->days;
来源：http://hz.shanyushiyangtech.top/gttgppacnn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.svipenyu.cn/gtklxhftyl.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jqgfzy.top/gtopfcsysc.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.yuxming.cn/gthveqxmsq.html

Go:   end.Sub(start).Hours()
来源：http://hz.hnxiangtu.top/gtewmjutte.html

Ruby: end - start                 # 返回秒数
来源：http://hz.bjfxy.top/gtkylandki.html

C#:   (end - start).TotalSeconds
来源：http://hz.yvedp.cn/gtmjzsccvh.html

[J07] 比较两个日期
来源：http://hz.0kj1m.cn/gtkttntqeb.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.sysykeji.top/gtldttbujy.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.nanxinkj.top/gthkviquyj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.gogol.net.cn/gtnibvydjh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yj20258.top/gtplrahjmu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.dianchejie.cn/gtwcqfosdx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.jinqigufen.top/gtukodzrxh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hammf.cn/gtswzjcuon.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.kuanghao11.cn/gtkyvbbdep.html

[J08] 提取年月日与星期
来源：http://hz.bjfxy.top/gtzmnyfxjy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hongshengwenyu.top/gtmtfqucvd.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jianghu66.top/gtqoewjvxz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.fzhhl.top/gtvepfowec.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.0kj1m.cn/gtqjqghgvr.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.vqdsnc.cn/gtxrppkknf.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.wangdashe.top/gtawhdjcrf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.cucudq.cn/gtpdyavdnl.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.dianchejie.cn/gttnodwldw.html

[J09] 时区处理
来源：http://hz.hywenlv.cn/gtjguzokdz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.nanxinkj.top/gtgjfkhvtt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.quarkkingdee.top/gtvgzfwgcc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.havefunace.top/gtbbgpjpjh.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.svipenyu.cn/gtlatjleew.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhoulong.xyz/gtxavocbaj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.fengsongda.top/gtsjvjnhze.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinyuanbaomall.cn/gtdjslgtjl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shzxlz.cn/gtcgrfpnyk.html

[J10] 取今天 / 本月第一天
来源：http://hz.aibaodan.cn/gtvvtdmtww.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gogol.net.cn/gtgmgatpqh.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.yongpay.top/gtvdudnnba.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.pycfn.com/gteodydzwc.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.yj20258888.top/gtgqfdhtci.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.sufxvd.cn/gtkbvievkm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xingfuxueyuan.xyz/gtzbbyjiyh.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.yonumen.top/gtwlrzpozx.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.daria6918.cn/gtgtyesynw.html

================================================================================
来源：http://hz.chenlongwang.top/gtuzaizxff.html

K. JSON 与序列化
来源：http://hz.xuetiantiany.cn/gttpahmvun.html

================================================================================
来源：http://hz.aizwys.cn/gtvcbvxdju.html

[K01] 对象转 JSON 字符串
来源：http://hz.cucudq.cn/gtosoekxrl.html


<!-- 参考信息 -->