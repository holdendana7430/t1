代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jlsjyb.cn/gttaxvxyiq.html

Ruby: def to_s; @name; end
来源：http://hz.yonumen.top/gtlbeswaeg.html

C#:   public override string ToString() => Name;
来源：http://hz.hnqzz.top/gtcalxoguy.html

[G13] 判断对象类型
来源：http://hz.shanyushiyangtech.top/gthoyumayz.html

Py:   isinstance(u, User)
来源：http://hz.zhoulong.xyz/gtxfrilcjr.html

PHP:  $u instanceof User
来源：http://hz.yueranfly.top/gttakggsux.html

JS:   u instanceof User
来源：http://hz.dashuyun.cn/gtunymzfxx.html

TS:   u instanceof User
来源：http://hz.chenzaomai.com/gtgwusqjrd.html

Java: u instanceof User
来源：http://hz.gotoacloud.top/gtesmjvzud.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.vqdsnc.cn/gtvuleknfa.html

Ruby: u.is_a?(User)
来源：http://hz.ppjwa.cn/gtxruzngdo.html

C#:   u is User
来源：http://hz.quarkkingdee.top/gtqtabrkqq.html

[G14] 数据类 / record
来源：http://hz.zhongyouzk.top/gtgtenwnds.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hysaishi.cn/gtwesinmos.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yuanzhike.top/gtjtaegxjg.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.ywan-chungtsiang.top/gtjbncfujl.html

TS:   type User = { name: string; age: number };
来源：http://hz.iojbl.cn/gtqsydmjpu.html

Java: record User(String name, int age) {}
来源：http://hz.ydjk.org.cn/gtcysyvoib.html

Go:   type User struct { Name string; Age int }
来源：http://hz.tian-w.cn/gtbgnglpxg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.sweek.top/gtqwfzsnnv.html

C#:   record User(string Name, int Age);
来源：http://hz.gotoacloud.top/gtngohmvec.html

[G15] 枚举
来源：http://hz.daria6918.cn/gtkqntskhy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ehwqpu.com/gtdeowddmz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shuidangran.top/gtwsioblpf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hammf.cn/gtpbnnescc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shuidangran.top/gtryibclhv.html

Java: enum Color { RED, GREEN }
来源：http://hz.daxiang520.top/gtvtesjwwb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.nanxuanxn.top/gtuzbdftuq.html

Ruby: Color = %i[red green].freeze
来源：http://hz.xuetiantiany.cn/gtnydclnho.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangshuangyany.cn/gtenxzijta.html

[G16] 对象转数组 / 字典
来源：http://hz.havefunace.top/gtmjebnnvv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jqgfzy.top/gtlmyiywnj.html

PHP:  get_object_vars($obj);
来源：http://hz.dianchejie.cn/gtcabtqilf.html

JS:   Object.entries(obj)
来源：http://hz.gzhubu.top/gthwouzuqu.html

TS:   Object.entries(obj)
来源：http://hz.shzxlz.cn/gtvflkcpkp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhengqikj.top/gtfdpntyfk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.hywenlv.cn/gtofwicitt.html

Ruby: obj.instance_variables
来源：http://hz.svipenyu.cn/gtrnyipezo.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.aibaodan.cn/gtwblfhamm.html

================================================================================
来源：http://hz.yongpay.top/gtqawidbdx.html

H. 异常与错误处理
来源：http://hz.hnqzz.top/gtanxdytob.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtmfmmsrwa.html

[H01] try / catch 基础
来源：http://hz.cqqwz.cn/gtlpgxcxkf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xylfe.cn/gtvofydxgg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.zhiwuduotai.top/gtaqnftizt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hongshengwenyu.top/gtazfofyvb.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhongyouzk.top/gthlwnculc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yueranfly.top/gtjmihllna.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yj202588.top/gtoamdbndo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yuanzhike.top/gttvirkizk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.cashguo.top/gtboolzxgw.html

[H02] finally / ensure 收尾
来源：http://hz.shangyingyoupin.top/gtmhegzgre.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.daxiang520.top/gtiodwqbxc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jinqigufen.top/gtgyrdaesp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtdskcfrgu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.aizwys.cn/gtnriwlzde.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.0kj1m.cn/gtapjilhwh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jinyuanbaomall.cn/gtfdrixgfv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jiagoushi.top/gtpifcaneu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.feifeiyinyue.top/gtvfigpynr.html

[H03] 主动抛出异常
来源：http://hz.hongshengwenyu.top/gtedqrksox.html

Py:   raise ValueError("错误信息")
来源：http://hz.ydzc1.top/gtkrdcmngp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.iojbl.cn/gtrvzhfynz.html

JS:   throw new Error("错误信息");
来源：http://hz.ehwqpu.com/gtajltmuni.html

TS:   throw new Error("错误信息");
来源：http://hz.iojbl.cn/gtujaczxne.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jinghuilouyu.cn/gttdgrxhxi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinqigfzy.top/gtopzgsimd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jinyuanbaomall.cn/gtysxkuhzz.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtnnghzfmr.html

[H04] 自定义异常类型
来源：http://hz.jinqigfzy.top/gtkosijkag.html

Py:   class MyError(Exception): pass
来源：http://hz.hammf.cn/gtaswccava.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.fengsongda.top/gtxgxwbzcz.html

JS:   class MyError extends Error {}
来源：http://hz.shanyushiyangkeji.top/gtbmecbokq.html

TS:   class MyError extends Error {}
来源：http://hz.xziqi.cn/gtlrzyvqsr.html

Java: class MyException extends RuntimeException {}
来源：http://hz.sysykeji.top/gteyoczwla.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.c1oappe.top/gtimnusvec.html

Ruby: class MyError < StandardError; end
来源：http://hz.hnqzz.top/gtjbqagfdx.html

C#:   class MyException : Exception {}
来源：http://hz.chenzaomai.com/gthnotyofj.html

[H05] 捕获特定类型
来源：http://hz.xinyue.icu/gtzgdabkac.html

Py:   except ValueError as e:
来源：http://hz.hongshengwenyu.top/gtbuakiohr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zhengqikj.top/gtayuzldnd.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.nanxuanxn.top/gtifublzpx.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xinyue.icu/gtqvlfhwii.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.gzhubu.top/gtmswrlkuc.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.daria6918.cn/gtgkfyhsay.html

Ruby: rescue ArgumentError => e
来源：http://hz.birdmap.top/gtksdngypf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hammf.cn/gtmqgvodyr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.tianlin.xyz/gtfrbjmvxg.html

Py:   value = d.get("k") or default
来源：http://hz.cucudq.cn/gtjdvolatc.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.daxiang520.top/gtdmondeql.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yanxiufei.cn/gtzbxlirch.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.tianlin.xyz/gtnebihuua.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zhengqikj.top/gtpmlvxtlv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhoulong.xyz/gtbjrfvjvf.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shanyushiyangkeji.top/gttamhlyup.html

C#:   obj?.A?.B ?? default
来源：http://hz.sxryk.cn/gtpdosezdo.html

[H07] 断言
来源：http://hz.bjfxy.top/gtpbivwswf.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yj20258888.top/gtkoxppijx.html

PHP:  assert($x > 0);
来源：http://hz.c1oappe.top/gtmzanhowt.html

JS:   console.assert(x > 0);
来源：http://hz.daxiang520.top/gtffcpktgg.html

TS:   console.assert(x > 0);
来源：http://hz.hongshengwenyu.top/gtffrhffig.html

Java: assert x > 0 : "必须为正";
来源：http://hz.52xcode.cn/gtfhuoabwz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.cdnleiting.top/gtuypcshih.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.xinyue.icu/gtxfameqiw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.shangyingyoupin.top/gtzugsgncl.html

[H08] 获取错误信息与堆栈
来源：http://hz.hfpthk.cn/gtblbmpyqj.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.guowangkeji.top/gthyzsjrnx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhaomingkeji.xyz/gtpcruqufl.html

JS:   e.message;  e.stack
来源：http://hz.jianghu66.top/gtcbljgilc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cashguo.top/gtrcaksyjn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.yongpay.top/gtvxejowqa.html

Go:   err.Error()
来源：http://hz.shuidangran.top/gtxmjrpdep.html

Ruby: e.message;  e.backtrace
来源：http://hz.nanxinkj.top/gtnublpzag.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shangyingyoupin.top/gtbzncujpg.html

[H09] 带错误码的异常
来源：http://hz.gaohongyu789.top/gtfrsznziy.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.guowangkeji.top/gthcdictcn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shuidangran.top/gtzlollhle.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.dianchejie.cn/gtqjiqafjg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.sufxvd.cn/gtvvchxyez.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yj202588.top/gtpbyezoub.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.fzhhl.top/gtntbfnozn.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.shangyingyoupin.top/gtidydltkz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hnxiangtu.top/gtuuflxnma.html

[H10] 资源自动释放
来源：http://hz.ybcxt.top/gtqvkrhbfk.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.birdmap.top/gtqsnfiyek.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.zhaomingkeji.xyz/gtixivitvr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgfzy.top/gtxswwygsd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.chenzaomai.com/gtsnydlcnw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.kuanghao11.cn/gtngizcfpb.html

Go:   defer f.Close()
来源：http://hz.gogol.net.cn/gtxeummrmj.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.cqqwz.cn/gtzpoygkmt.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.quarkkingdee.top/gtaginxbfr.html

================================================================================
来源：http://hz.guowangkeji.top/gtbtnyibmj.html

I. 正则表达式
来源：http://hz.snrcjt.cn/gtdreofecc.html

================================================================================
来源：http://hz.cashguo.top/gtlihesobv.html

[I01] 判断是否匹配
来源：http://hz.feifeiyinyue.top/gtncuupove.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.yueranfly.top/gtiwfdevkr.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.fzhhl.top/gtublyoczs.html

JS:   /\d+/.test(s)
来源：http://hz.ywan-chungtsiang.top/gtunskyqdj.html

TS:   /\d+/.test(s)
来源：http://hz.tanke756.top/gtyjembcsp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.guannengcc.top/gtgdhothqd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.nwbrower.top/gtgctsouma.html

Ruby: s.match?(/\d+/)
来源：http://hz.cashguo.top/gturernajr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.ywan-chungtsiang.top/gtkpgasunx.html

[I02] 提取所有匹配
来源：http://hz.tianlin.xyz/gtnrinjoex.html

Py:   re.findall(r"\d+", s)
来源：http://hz.hnqzz.top/gtqkeftpmo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shangyingyoupin.top/gtzmndpruk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.yonumen.top/gtdcaiqlao.html

TS:   s.match(/\d+/g)
来源：http://hz.shzxlz.cn/gtjbttiedl.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.sufxvd.cn/gtqdpdfsph.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zhijiandao.cn/gtwiztvonn.html

Ruby: s.scan(/\d+/)
来源：http://hz.xuetiantiany.cn/gtxlvgbnpp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.nwbrower.top/gtypsjxlkk.html

[I03] 提取捕获分组
来源：http://hz.snrcjt.cn/gtljenibrq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.guowangkeji.top/gtptshoivz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.quarkkingdee.top/gtxsljaqca.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.pengpengdd.cyou/gtytydlljq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yangfankeji.com/gtbwycnxmr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yj20258888.top/gtcmxkitxp.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.yvedp.cn/gtqaovhwjl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ehwqpu.com/gtjhmehrnm.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.aibaodan.cn/gtpvdcfvwj.html

[I04] 正则替换
来源：http://hz.hfpthk.cn/gtuvbbsxlu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shanyushiyangtech.top/gtzcozadcr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.sysykeji.top/gtxhpgkhqb.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.chenzaomai.com/gtrthbipkh.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.jqgfzy.top/gtbhnmhcln.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jyoumei.cn/gtjdhlouqx.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.birdmap.top/gtbxrrlgjx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.gogol.net.cn/gtlevltric.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.cdnleiting.top/gtrjqzyald.html

[I05] 按正则拆分
来源：http://hz.cashguo.top/gtfzsapbxf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.zycfv.cn/gtkgrsanfk.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.ehwqpu.com/gtojpvsuuv.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.sysykeji.top/gtnqpewlkd.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.dianchejie.cn/gthtzvtcul.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yvedp.cn/gtbwgdpabg.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xylfe.cn/gtovhddoue.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.chenlongwang.top/gtmpubwodu.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.0kj1m.cn/gtgihzizjw.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yonumen.top/gtxktzvlds.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jianghu66.top/gtabltseyb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.zhengqikj.top/gtewkyzoik.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gotoacloud.top/gtsnijlesj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cdnleiting.top/gtipnweoyt.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.jinghuilouyu.cn/gtkejklbko.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hfpthk.cn/gtptvufywe.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gzhubu.top/gtxvwfqwsi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.nwbrower.top/gtwatyopwp.html

[I07] 忽略大小写与多行模式
来源：http://hz.fzhhl.top/gtgeqzxtlp.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hfpthk.cn/gtqduzptby.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zhijiandao.cn/gtwvbygbjl.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zycfv.cn/gtmdigwiqw.html

TS:   /error/gim
来源：http://hz.9152youxi.cn/gtdbblomew.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ydjk.org.cn/gtdazfrecn.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.haohaochexian.top/gtyebkbdoa.html

Ruby: s.scan(/error/i)
来源：http://hz.yuxming.cn/gtiggohlkk.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.c1oappe.top/gtbwuvxrgz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sxryk.cn/gtwuvfcsjj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.pengpengdd.cyou/gthrwphzdt.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.gogol.net.cn/gtivikbvpb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.sxryk.cn/gtxuemumgi.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cucudq.cn/gtdcjarrdu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.vqdsnc.cn/gtqytsnrvm.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.quarkkingdee.top/gtgmlcdtys.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jyoumei.cn/gtpyrfqedd.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.316326.xyz/gtugmjpzad.html

================================================================================
来源：http://hz.cheryme.top/gtjasldkor.html

J. 日期与时间
来源：http://hz.dashuyun.cn/gtkqcxcbqv.html

================================================================================
来源：http://hz.fengsongda.top/gtjhrmtinn.html

[J01] 获取当前时间
来源：http://hz.tanke756.top/gthkqtcnif.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.nanxinkj.top/gtkgfvtnbi.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cucudq.cn/gttqeaqyej.html

JS:   new Date();  Date.now()
来源：http://hz.gzhubu.top/gtfhdftlkx.html

TS:   new Date();  Date.now()
来源：http://hz.havefunace.top/gtudqbrrbb.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.ywan-chungtsiang.top/gtitcbrbxk.html

Go:   time.Now()
来源：http://hz.jiagoushi.top/gtqawqrqsr.html

Ruby: Time.now
来源：http://hz.jlsjyb.cn/gtafxpqvhe.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yonumen.top/gtclckhzoo.html

[J02] 格式化输出
来源：http://hz.vqdsnc.cn/gtnezcwwfm.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.smart0.xyz/gtyxohiqmo.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.pengpengdd.cyou/gtahjzbqkd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.c1oappe.top/gthpfknbtn.html

TS:   d.toISOString()
来源：http://hz.iojbl.cn/gtuxavslkh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.ydzc1.top/gtfuabcyjd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.gzhubu.top/gtigdklgit.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hnqzz.top/gtajuhrvbb.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.nanxinkj.top/gtwpohwdpe.html

[J03] 字符串解析为日期
来源：http://hz.yangfankeji.com/gtgzudgxjy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yj20258.top/gtpkvqxcjm.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.xinyue.icu/gtpwrbutbh.html

JS:   new Date("2024-01-02")
来源：http://hz.iojbl.cn/gtcuswgkwo.html

TS:   new Date("2024-01-02")
来源：http://hz.zycfv.cn/gtmwcafbnv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.tianlin.xyz/gtkvolawwl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.gaohongyu789.top/gtgrdwzbsf.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cdnleiting.top/gtvabeckfo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yuanzhike.top/gtlcdwcisl.html

[J04] 时间戳与日期互转
来源：http://hz.cashguo.top/gtdtfhgwbs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.jinqigufen.top/gtmlbabsei.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ydjk.org.cn/gtvdgqyjoi.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gotoacloud.top/gtcixcrcue.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ydjk.org.cn/gthobcxeor.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jyoumei.cn/gtmtyxjkoi.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.sxryk.cn/gtrxhxcmcy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zhengqikj.top/gtjrbhpusm.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ivvv.top/gtpqovlcya.html

[J05] 时间加减（加 7 天）
来源：http://hz.aizwys.cn/gtboataxeh.html

Py:   now + timedelta(days=7)
来源：http://hz.meibo888.top/gtwcqhszit.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.cucudq.cn/gthhalqlcr.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ivvv.top/gtrpewcmso.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ehwqpu.com/gtlsskvfla.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yj20258888.top/gtfqzkuaun.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jinqigufen.top/gtyupbwbpj.html

Ruby: Time.now + 7 * 86400
来源：http://hz.xuetiantiany.cn/gtzecqncvf.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.jinqigufen.top/gtstlxnzpm.html

[J06] 计算两时间之差
来源：http://hz.shzxlz.cn/gtmrvirkhp.html

Py:   (end - start).total_seconds()
来源：http://hz.xylfe.cn/gtzxyazjba.html

PHP:  $end->diff($start)->days;
来源：http://hz.nanxinkj.top/gtfqisgecv.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.nanxuanxn.top/gtaxwumpia.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.jyoumei.cn/gtdslhlsev.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.tanke756.top/gtkmfbauuk.html

Go:   end.Sub(start).Hours()
来源：http://hz.ivvv.top/gtvgtxhtxa.html

Ruby: end - start                 # 返回秒数
来源：http://hz.vqdsnc.cn/gtpxsasvhk.html

C#:   (end - start).TotalSeconds
来源：http://hz.cucudq.cn/gtpxmlvebk.html

[J07] 比较两个日期
来源：http://hz.mhx1999.top/gttpccfimx.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.aizwys.cn/gttgekmzeh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jlsjyb.cn/gtlumdycos.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.yuxming.cn/gtgqahklrk.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.sufxvd.cn/gtjbxqsolk.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yangfankeji.com/gtvjkgvsqh.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zhongyouzk.top/gtwxjlxrpw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hnxiangtu.top/gtwtudvtmq.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gtushaejii.html

[J08] 提取年月日与星期
来源：http://hz.cheryme.top/gtdmcsuyzu.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yj20258888.top/gtdajmbjvz.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.yanxiufei.cn/gttxxtckys.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jiagoushi.top/gtyriidfff.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shanyushiyangkeji.top/gtuyccoiby.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.hnqzz.top/gtfgfnihoh.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.wangdashe.top/gtadjcxelf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zycfv.cn/gtevrhlcbu.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hywenlv.cn/gtboiqlpkh.html

[J09] 时区处理
来源：http://hz.ehwqpu.com/gtexelcgtn.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.redwolf501.top/gtscdhgwfa.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.yonumen.top/gttrnytyon.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ybcxt.top/gtyoxygijr.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.chenzaomai.com/gtkrizeafp.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.jqgufenzy.top/gtkfceosms.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinqigfzy.top/gtsilhpjgx.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.ybcxt.top/gtkthigadx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.redwolf501.top/gtndpfxxqp.html

[J10] 取今天 / 本月第一天
来源：http://hz.shanyushiyangtech.top/gtzhtksevk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.svipenyu.cn/gtdlrfllgs.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.jiagoushi.top/gtdyrzgyon.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.yangfankeji.com/gtowpvrbgb.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.jlsjyb.cn/gtwzdtsbbv.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.316326.xyz/gtggqmmdkn.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.pengpengdd.cyou/gttecjjdim.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.tian-w.cn/gtbgjpfgqp.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.dashuyun.cn/gtqqmzzncm.html


<!-- 参考信息 -->