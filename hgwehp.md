代发 wailian999

Java: u instanceof User
来源：http://hz.yonumen.top/gtfsrnqjjg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinqigufen.top/gtfhmnldsw.html

Ruby: u.is_a?(User)
来源：http://hz.gotoacloud.top/gtxmzihgfu.html

C#:   u is User
来源：http://hz.yonumen.top/gtltuebedn.html

[G14] 数据类 / record
来源：http://hz.nwbrower.top/gtvtokoexa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hongshengwenyu.top/gtposbkibh.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.zycfv.cn/gtbovydobh.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yj202588.top/gtsrvvxpkl.html

TS:   type User = { name: string; age: number };
来源：http://hz.snrcjt.cn/gttclfnvge.html

Java: record User(String name, int age) {}
来源：http://hz.kuanghao11.cn/gtaekkkmvz.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jinghuilouyu.cn/gtpjgariob.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ehwqpu.com/gtvvfxkgwb.html

C#:   record User(string Name, int Age);
来源：http://hz.nanxuanxn.top/gtzwfbzked.html

[G15] 枚举
来源：http://hz.xylfe.cn/gtudeppcki.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ydzc1.top/gturdrrzgd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.ywan-chungtsiang.top/gtcmfawhdu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.mhx1999.top/gtuzqddwmp.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.redwolf501.top/gtivauebgz.html

Java: enum Color { RED, GREEN }
来源：http://hz.guowangkeji.top/gtwvzvrubs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.hywenlv.cn/gtcoabkhod.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gaohongyu789.top/gtgsvxfubq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nwbrower.top/gtbyexvklk.html

[G16] 对象转数组 / 字典
来源：http://hz.shuidangran.top/gtqhofzipt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hysaishi.cn/gtaptwsylc.html

PHP:  get_object_vars($obj);
来源：http://hz.tian-w.cn/gttgjonkvf.html

JS:   Object.entries(obj)
来源：http://hz.svipenyu.cn/gtpeqdegsd.html

TS:   Object.entries(obj)
来源：http://hz.andypj.xyz/gtyngfezfy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yangfankeji.com/gtrveqjpxh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hammf.cn/gtmbwmsyke.html

Ruby: obj.instance_variables
来源：http://hz.jinghuilouyu.cn/gtxlrbwwsv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.redwolf501.top/gtfglvvvnw.html

================================================================================
来源：http://hz.mhx1999.top/gtpzksfrgm.html

H. 异常与错误处理
来源：http://hz.hnqzz.top/gtvxshiyot.html

================================================================================
来源：http://hz.jyoumei.cn/gtryqgnnes.html

[H01] try / catch 基础
来源：http://hz.jianghu66.top/gtpjvpvpjr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yuanzhike.top/gtunmjqbbk.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.nanxuanxn.top/gtddpoguok.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shuidangran.top/gthofvxbjv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.chenzaomai.com/gttptatlnc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.gaohongyu789.top/gthgydilzz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jinqigufen.top/gtoyowtpkq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.aibaodan.cn/gtpktbrzvh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhixingplan.top/gtjbfspmzd.html

[H02] finally / ensure 收尾
来源：http://hz.chenzaomai.com/gtrxzcykfq.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jianghu66.top/gtauiutfty.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.chenzaomai.com/gtrujeellw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtlgbugsdv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.smart0.xyz/gtjjqyrdjq.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nwbrower.top/gtqdgxvsbn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.haohaochexian.top/gtchznwkzy.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.vqdsnc.cn/gtmvcnmurl.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ydzc1.top/gtlgeoxviq.html

[H03] 主动抛出异常
来源：http://hz.hammf.cn/gtgjknoyfq.html

Py:   raise ValueError("错误信息")
来源：http://hz.yj202588.top/gtaictbuhc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.haohaochexian.top/gthgvmbdbq.html

JS:   throw new Error("错误信息");
来源：http://hz.jinqigfzy.top/gtakmytqwo.html

TS:   throw new Error("错误信息");
来源：http://hz.hammf.cn/gtcrftfpjp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.smart0.xyz/gtkvuhahdx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.snrcjt.cn/gtcdfuejwn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.xylfe.cn/gtvqshwtnj.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.9152youxi.cn/gtqhbepbyu.html

[H04] 自定义异常类型
来源：http://hz.ywan-chungtsiang.top/gtnmwcldis.html

Py:   class MyError(Exception): pass
来源：http://hz.dashuyun.cn/gtjhpphapu.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.andypj.xyz/gtgtjfprlj.html

JS:   class MyError extends Error {}
来源：http://hz.zhongyouzk.top/gtsyziylak.html

TS:   class MyError extends Error {}
来源：http://hz.chenlongwang.top/gtsjumtrne.html

Java: class MyException extends RuntimeException {}
来源：http://hz.xuetiantiany.cn/gtxvabqxgi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shanyushiyangkeji.top/gtiapoxjms.html

Ruby: class MyError < StandardError; end
来源：http://hz.wangdashe.top/gtbrivgpbq.html

C#:   class MyException : Exception {}
来源：http://hz.ivvv.top/gtvkeewedc.html

[H05] 捕获特定类型
来源：http://hz.jiagoushi.top/gtijxicflc.html

Py:   except ValueError as e:
来源：http://hz.jiagoushi.top/gtdngdgoua.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.jqgufenzy.top/gtxudjygeh.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hnxiangtu.top/gtinwhpopm.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhaomingkeji.xyz/gtxgwkwufv.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.0kj1m.cn/gtsgeejqhp.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.xuetiantiany.cn/gtnghlpjag.html

Ruby: rescue ArgumentError => e
来源：http://hz.jianghu66.top/gtnvmpafoi.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.52xcode.cn/gtrourktfx.html

[H06] 可选值 / 空值安全访问
来源：http://hz.guannengcc.top/gtxgnxzrry.html

Py:   value = d.get("k") or default
来源：http://hz.nwbrower.top/gtmvzsbitk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yvedp.cn/gtqtqfdqnr.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.tian-w.cn/gtryivoqpl.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.yangfankeji.com/gtkscstidu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shuidangran.top/gturrnaqyq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sufxvd.cn/gtqhxdqkhy.html

Ruby: d&.dig(:a, :b)
来源：http://hz.nanxuanxn.top/gtmnubetxx.html

C#:   obj?.A?.B ?? default
来源：http://hz.feifeiyinyue.top/gtfirnygzk.html

[H07] 断言
来源：http://hz.guowangkeji.top/gtbxgljdxa.html

Py:   assert x > 0, "必须为正"
来源：http://hz.cheryme.top/gtjxplotvv.html

PHP:  assert($x > 0);
来源：http://hz.jinghuilouyu.cn/gtohjfjrlk.html

JS:   console.assert(x > 0);
来源：http://hz.kuanghao11.cn/gthmiefsif.html

TS:   console.assert(x > 0);
来源：http://hz.yj202588.top/gttdlzhtyw.html

Java: assert x > 0 : "必须为正";
来源：http://hz.tianlin.xyz/gtgacsmxem.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.hnxiangtu.top/gtmxedvigz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sufxvd.cn/gtsbjorclt.html

C#:   Debug.Assert(x > 0);
来源：http://hz.0kj1m.cn/gtjvidieop.html

[H08] 获取错误信息与堆栈
来源：http://hz.ybcxt.top/gtkxyvbjib.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hfpthk.cn/gtmqfidhau.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.9152youxi.cn/gtcdvecxto.html

JS:   e.message;  e.stack
来源：http://hz.cashguo.top/gtaxacsatp.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.pycfn.com/gtpyicqovp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.xinyue.icu/gtaeddvyjg.html

Go:   err.Error()
来源：http://hz.xuanzx.com/gtjmwjnapj.html

Ruby: e.message;  e.backtrace
来源：http://hz.yj202588.top/gtkgeqhhnc.html

C#:   e.Message;  e.StackTrace
来源：http://hz.svipenyu.cn/gtzblfdvli.html

[H09] 带错误码的异常
来源：http://hz.sweek.top/gttlaknddq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jinqigufen.top/gtfzcbppxf.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.ivvv.top/gtncwcipzm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.zhiwuduotai.top/gtbbfbdvjm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.havefunace.top/gtdjllnkqr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zdqjudy.top/gtfqitnkzi.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ydzc1.top/gtfutasvay.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.zycfv.cn/gtpssqxwrn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.sweek.top/gtysclkdhz.html

[H10] 资源自动释放
来源：http://hz.jinqigfzy.top/gtrnacyaki.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.yvedp.cn/gtupiybenr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xuanzx.com/gthugqkwua.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hnqzz.top/gtxqcfbdta.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.quarkkingdee.top/gtwglvfayg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.sufxvd.cn/gtutvyuusc.html

Go:   defer f.Close()
来源：http://hz.daxiang520.top/gtpajsxjlp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.daxiang520.top/gtkhrnfzom.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.wangshuangyany.cn/gtmbfsrijh.html

================================================================================
来源：http://hz.hnxiangtu.top/gtsnbaxyuj.html

I. 正则表达式
来源：http://hz.ehwqpu.com/gtwmycuuqe.html

================================================================================
来源：http://hz.dashuyun.cn/gtpicuvwty.html

[I01] 判断是否匹配
来源：http://hz.sweek.top/gtdpnmjfub.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zycfv.cn/gttpwsazjm.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.birdmap.top/gtpeicpewb.html

JS:   /\d+/.test(s)
来源：http://hz.ppjwa.cn/gtvtpghlii.html

TS:   /\d+/.test(s)
来源：http://hz.havefunace.top/gtgotvdyfg.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xinyue.icu/gtxdrfjosh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hywenlv.cn/gthureczvf.html

Ruby: s.match?(/\d+/)
来源：http://hz.ybcxt.top/gtsabyttvl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.gzhubu.top/gtqlxnmntk.html

[I02] 提取所有匹配
来源：http://hz.hywenlv.cn/gtxzydcvco.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yueranfly.top/gtujmllmub.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ywan-chungtsiang.top/gtuxojxgtd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.gogol.net.cn/gtzecsstlr.html

TS:   s.match(/\d+/g)
来源：http://hz.chenlongwang.top/gteoejlkcm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jyoumei.cn/gtzzbwumse.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhongyouzk.top/gtfcjuwmzn.html

Ruby: s.scan(/\d+/)
来源：http://hz.gzhubu.top/gteirqchvl.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.316326.xyz/gttrdpklsg.html

[I03] 提取捕获分组
来源：http://hz.smart0.xyz/gtbvirkvge.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.pycfn.com/gtfztybxuy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ydzc1.top/gtqahiduou.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xuanzx.com/gtduubibfp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.xinyue.icu/gtcyloikwf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hfpthk.cn/gtjghkjtuh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yanxiufei.cn/gtmszhewlg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xingfuxueyuan.xyz/gtxdaywrkd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.quarkkingdee.top/gtrdriuifr.html

[I04] 正则替换
来源：http://hz.yongpay.top/gtndcualal.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinghuilouyu.cn/gtpviizpog.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yj202588.top/gtmxrnvhaw.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gotoacloud.top/gtltguhtac.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.ivvv.top/gtiorbmkat.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.smart0.xyz/gtcxxvrqap.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.vqdsnc.cn/gtmglnciyr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hammf.cn/gtufyrfmwh.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.zhaomingkeji.xyz/gteoolvluv.html

[I05] 按正则拆分
来源：http://hz.gzhubu.top/gtirjseebf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.andypj.xyz/gtkmjcuakw.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.redwolf501.top/gthyguzdqn.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yj20258888.top/gtrwpjyina.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.daria6918.cn/gthrhujmcd.html

Java: s.split("\\s*,\\s*")
来源：http://hz.c1oappe.top/gtvofnhfnh.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hywenlv.cn/gtabclygpe.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.pycfn.com/gtqdgyonxs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gogol.net.cn/gtotrrufta.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.sxryk.cn/gtybdjjkaw.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.andypj.xyz/gtkriuleah.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.haohaochexian.top/gtbjdftxiu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangkeji.top/gtbpdkfghy.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jqgfzy.top/gtvgetfviz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.sxryk.cn/gtgkgesjdm.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.daxiang520.top/gtxqleaqed.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yj20258888.top/gtixkyeerz.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yonumen.top/gtssynzbyu.html

[I07] 忽略大小写与多行模式
来源：http://hz.hnqzz.top/gtuoikxrao.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.9152youxi.cn/gtaqnbwygq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yj20258888.top/gtnoghvujw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.bjfxy.top/gttnaorkzf.html

TS:   /error/gim
来源：http://hz.sxryk.cn/gtjuuomsge.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jianghu66.top/gttickbghk.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.ywan-chungtsiang.top/gtqjmnyygk.html

Ruby: s.scan(/error/i)
来源：http://hz.ivvv.top/gtaojzcsyn.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.9152youxi.cn/gtcsznvzqc.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.vqdsnc.cn/gtomkaiyur.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.xylfe.cn/gtcbmtnqjs.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.havefunace.top/gtymscfnrg.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hammf.cn/gtdbqlcfcf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.fzhhl.top/gtfmnpcwid.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.tanke756.top/gtxwdtdzpe.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.gogol.net.cn/gtigolvwku.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jqgfzy.top/gtoyotflvo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhiwuduotai.top/gtrzgajoqi.html

================================================================================
来源：http://hz.mhx1999.top/gtzjeewjrv.html

J. 日期与时间
来源：http://hz.jqgfzy.top/gtiqffyybx.html

================================================================================
来源：http://hz.meibo888.top/gtksmwwykh.html

[J01] 获取当前时间
来源：http://hz.xuetiantiany.cn/gtpynvatdi.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shanyushiyangtech.top/gtnyreolgf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hysaishi.cn/gtmaybgnnp.html

JS:   new Date();  Date.now()
来源：http://hz.kuanghao11.cn/gtpadmazob.html

TS:   new Date();  Date.now()
来源：http://hz.chenjidiqi.icu/gtqwtxvjdf.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cdnleiting.top/gthidlxawn.html

Go:   time.Now()
来源：http://hz.wangdashe.top/gtykekmrpr.html

Ruby: Time.now
来源：http://hz.316326.xyz/gttoxmwehs.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.aizwys.cn/gtebzrcyus.html

[J02] 格式化输出
来源：http://hz.vqdsnc.cn/gtvkcypylg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jianghu66.top/gtsynurtoi.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.andypj.xyz/gtbatswshr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.nanxuanxn.top/gtdeogsvqz.html

TS:   d.toISOString()
来源：http://hz.52xcode.cn/gtppszyphj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.vqdsnc.cn/gtgcxhbutj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tanke756.top/gtzffhswld.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yonumen.top/gttsthofgx.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ywan-chungtsiang.top/gtlrwhlbjh.html

[J03] 字符串解析为日期
来源：http://hz.hysaishi.cn/gtlbkkvpqg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xingfuxueyuan.xyz/gtqsosdjpm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cucudq.cn/gtzprhjilv.html

JS:   new Date("2024-01-02")
来源：http://hz.jinqigfzy.top/gtoqkxtxpx.html

TS:   new Date("2024-01-02")
来源：http://hz.ydjk.org.cn/gtyddwnwtl.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.chenjidiqi.icu/gtrttxiddz.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zycfv.cn/gtwbpynacr.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.snrcjt.cn/gtpkxdgldk.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.pycfn.com/gtubnnoosr.html

[J04] 时间戳与日期互转
来源：http://hz.hongshengwenyu.top/gtzgorknov.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xingfuxueyuan.xyz/gtrwyzezjd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.wangshuangyany.cn/gtiymmaukk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.zhoulong.xyz/gtyswpourb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ybcxt.top/gtznjiinxz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.cheryme.top/gthiwggrdg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.daxiang520.top/gteluvinxn.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yangfankeji.com/gtvnhtibkf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.nwbrower.top/gtwxkrbqwj.html

[J05] 时间加减（加 7 天）
来源：http://hz.snrcjt.cn/gtcpirgstw.html

Py:   now + timedelta(days=7)
来源：http://hz.hysaishi.cn/gtmdnxbpqs.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.meibo888.top/gtpcjzcpmd.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jqgfzy.top/gtsvnckism.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.tianlin.xyz/gteucyctnn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.dashuyun.cn/gthxepnusv.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.xinyue.icu/gteoudsvng.html

Ruby: Time.now + 7 * 86400
来源：http://hz.tanke756.top/gtgjsvifsb.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xingfuxueyuan.xyz/gtvohbxuvh.html

[J06] 计算两时间之差
来源：http://hz.chenzaomai.com/gtuajacdle.html

Py:   (end - start).total_seconds()
来源：http://hz.gotoacloud.top/gtejogxhmq.html

PHP:  $end->diff($start)->days;
来源：http://hz.yongpay.top/gtldskhwwp.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.cucudq.cn/gthmioklqy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jinqigufen.top/gtiwukeros.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.iojbl.cn/gtsaufixgn.html

Go:   end.Sub(start).Hours()
来源：http://hz.feifeiyinyue.top/gtwxtjuxpu.html

Ruby: end - start                 # 返回秒数
来源：http://hz.feifeiyinyue.top/gthcumawmv.html

C#:   (end - start).TotalSeconds
来源：http://hz.ywan-chungtsiang.top/gtofyvxgjb.html

[J07] 比较两个日期
来源：http://hz.quarkkingdee.top/gtfckcplbn.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gtpmdklhcp.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.tian-w.cn/gtjligpiom.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yuanzhike.top/gtgldydavy.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.guannengcc.top/gtqmbejhly.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.jinyuanbaomall.cn/gthjlzhfoq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.yvedp.cn/gtbbutbbyl.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.aibaodan.cn/gtnacstmry.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shuidangran.top/gtyuijjrkk.html

[J08] 提取年月日与星期
来源：http://hz.smart0.xyz/gtxhrrsjgy.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jlsjyb.cn/gtxslthfrq.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.chenjidiqi.icu/gtvpuqskhs.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.cucudq.cn/gtmsltlrgy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.nwbrower.top/gttnvhmemk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.chenjidiqi.icu/gtgmiayozm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.chenjidiqi.icu/gtsfumrtuo.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.9152youxi.cn/gtsjxwpnmv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.iojbl.cn/gtknaffmtq.html

[J09] 时区处理
来源：http://hz.hysaishi.cn/gtouyootrj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.havefunace.top/gtmcezqfdr.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.havefunace.top/gttjjwzqrw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.cqqwz.cn/gtixtkzlvy.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangshuangyany.cn/gtidbeayqw.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.andypj.xyz/gtcaodfxrb.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinqigfzy.top/gtbsbemswd.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.quarkkingdee.top/gtrsdpbzxe.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.shangyingyoupin.top/gtelbsjttt.html

[J10] 取今天 / 本月第一天
来源：http://hz.yj20258.top/gtktgamgji.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.jinghuilouyu.cn/gtucnnmnpb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.tanke756.top/gteirrlqet.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.jyoumei.cn/gthtlxgyxw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.0kj1m.cn/gtjbsijbji.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.zhixingplan.top/gtbakmfvvx.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.yvedp.cn/gtyybcnqnz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jinqigfzy.top/gtacrrvbyd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.cdnleiting.top/gtimutrnzn.html

================================================================================
来源：http://hz.yj20258.top/gtjvushsmn.html

K. JSON 与序列化
来源：http://hz.shanyushiyangkeji.top/gtxogmhxka.html

================================================================================
来源：http://hz.yj202588.top/gtbzgcvtwg.html

[K01] 对象转 JSON 字符串
来源：http://hz.dashuyun.cn/gtixzjozyc.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.9152youxi.cn/gtbapgbadw.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.tianlin.xyz/gthwpixonl.html

JS:   JSON.stringify(obj)
来源：http://hz.xziqi.cn/gtcddmoucu.html

TS:   JSON.stringify(obj)
来源：http://hz.hywenlv.cn/gtdujfocvp.html


<!-- 参考信息 -->