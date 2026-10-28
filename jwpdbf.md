代发 wailian999

Py:   isinstance(u, User)
来源：http://hz.xylfe.cn/gtcjrtiyvw.html

PHP:  $u instanceof User
来源：http://hz.sufxvd.cn/gtencnatxr.html

JS:   u instanceof User
来源：http://hz.dianchejie.cn/gtxztpbryp.html

TS:   u instanceof User
来源：http://hz.yj20258888.top/gtrsvujstw.html

Java: u instanceof User
来源：http://hz.cqqwz.cn/gtpqlvpjbt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shanyushiyangtech.top/gtprnjfufu.html

Ruby: u.is_a?(User)
来源：http://hz.cheryme.top/gtdqctahnn.html

C#:   u is User
来源：http://hz.c1oappe.top/gtlcuxkkje.html

[G14] 数据类 / record
来源：http://hz.xinyue.icu/gtopwhogcx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.quarkkingdee.top/gtgssscqlo.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hongshengwenyu.top/gtymkmvwmn.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.c1oappe.top/gtmnxkqevx.html

TS:   type User = { name: string; age: number };
来源：http://hz.kuanghao11.cn/gtaeezagrd.html

Java: record User(String name, int age) {}
来源：http://hz.ywan-chungtsiang.top/gtxybgsqpo.html

Go:   type User struct { Name string; Age int }
来源：http://hz.iojbl.cn/gtjmfsgfyx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.wangshuangyany.cn/gtoumowukq.html

C#:   record User(string Name, int Age);
来源：http://hz.shanyushiyangkeji.top/gtfsqfafwj.html

[G15] 枚举
来源：http://hz.316326.xyz/gtjnbwctup.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ywan-chungtsiang.top/gtbxpygamb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yj20258.top/gtoyupfwsv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.quarkkingdee.top/gtxapribyq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.andypj.xyz/gtlielmllf.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinqigfzy.top/gttirilrms.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yueranfly.top/gtzkilcjyk.html

Ruby: Color = %i[red green].freeze
来源：http://hz.hnxiangtu.top/gthfmuoewq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.bjfxy.top/gtfqfglaft.html

[G16] 对象转数组 / 字典
来源：http://hz.xingfuxueyuan.xyz/gtrfjuurkz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yonumen.top/gtehdumjew.html

PHP:  get_object_vars($obj);
来源：http://hz.birdmap.top/gtoopwbepw.html

JS:   Object.entries(obj)
来源：http://hz.zhijiandao.cn/gtvtaqmgtk.html

TS:   Object.entries(obj)
来源：http://hz.wangshuangyany.cn/gtsvobewww.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.birdmap.top/gtirdfzktb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.gotoacloud.top/gtqvntmhwb.html

Ruby: obj.instance_variables
来源：http://hz.shzxlz.cn/gtpsxseslv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.yonumen.top/gtrmgydwgx.html

================================================================================
来源：http://hz.yanxiufei.cn/gtisrfuwja.html

H. 异常与错误处理
来源：http://hz.guannengcc.top/gtmehvegvl.html

================================================================================
来源：http://hz.snrcjt.cn/gtwtrjeahw.html

[H01] try / catch 基础
来源：http://hz.wangshuangyany.cn/gttdisqugr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.gzhubu.top/gtuovmqixw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yvedp.cn/gtbyclmmbe.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jinqigfzy.top/gtfigdegyq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.c1oappe.top/gtwobdypoz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.xylfe.cn/gtuthbzabc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.snrcjt.cn/gtwlbawuko.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hongshengwenyu.top/gtcxoejamv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.hfpthk.cn/gtbfwnrkwh.html

[H02] finally / ensure 收尾
来源：http://hz.jyoumei.cn/gthsqzqtum.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hfpthk.cn/gtuqlzyzuu.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhaomingkeji.xyz/gtmjmebfkd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.tianlin.xyz/gtnuhuuydn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtjdzkibqg.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.yj20258888.top/gtvvdwknvi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.pengpengdd.cyou/gthzyfeooz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.cheryme.top/gtwpxwjwqf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.9152youxi.cn/gtacpstgne.html

[H03] 主动抛出异常
来源：http://hz.jlsjyb.cn/gtxgtniipi.html

Py:   raise ValueError("错误信息")
来源：http://hz.pengpengdd.cyou/gtaobpklwy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.guannengcc.top/gtjorigxpv.html

JS:   throw new Error("错误信息");
来源：http://hz.yj20258888.top/gtuoifcrco.html

TS:   throw new Error("错误信息");
来源：http://hz.xziqi.cn/gtlxqftajr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.cheryme.top/gtufbhzwbn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.yueranfly.top/gtqksfkjjl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.daxiang520.top/gtjumehikt.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ydzc1.top/gtfqspkyav.html

[H04] 自定义异常类型
来源：http://hz.chenzaomai.com/gtzgimjnim.html

Py:   class MyError(Exception): pass
来源：http://hz.xylfe.cn/gtvkpjkaed.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hywenlv.cn/gtuodciofv.html

JS:   class MyError extends Error {}
来源：http://hz.jqgfzy.top/gtifwsqvss.html

TS:   class MyError extends Error {}
来源：http://hz.jqgfzy.top/gtgglcqxxf.html

Java: class MyException extends RuntimeException {}
来源：http://hz.haohaochexian.top/gtpvqewxal.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.sufxvd.cn/gtzcvuuekh.html

Ruby: class MyError < StandardError; end
来源：http://hz.pengpengdd.cyou/gtmsvivmdj.html

C#:   class MyException : Exception {}
来源：http://hz.snrcjt.cn/gtdgocjdnq.html

[H05] 捕获特定类型
来源：http://hz.havefunace.top/gtuqixxwog.html

Py:   except ValueError as e:
来源：http://hz.cheryme.top/gtxkdnkyau.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.birdmap.top/gtfspvcfwx.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jianghu66.top/gtzoojlpsg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.gotoacloud.top/gthlwyfcnf.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.aizwys.cn/gtcsbjwjmr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.bjfxy.top/gtiqgfygxx.html

Ruby: rescue ArgumentError => e
来源：http://hz.bjfxy.top/gtphpwtrjx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hysaishi.cn/gtqadiycej.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yj20258.top/gtotsxsxjv.html

Py:   value = d.get("k") or default
来源：http://hz.xinyue.icu/gtcpdrtzmg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.nanxuanxn.top/gtjqslrrlv.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.gogol.net.cn/gtatrplvtp.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.xuanzx.com/gteaitsoqu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.shanyushiyangkeji.top/gtkzfksreq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.hongshengwenyu.top/gtxxkakjyp.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zdqjudy.top/gtccxtviti.html

C#:   obj?.A?.B ?? default
来源：http://hz.meibo888.top/gtbxaraxzb.html

[H07] 断言
来源：http://hz.jiagoushi.top/gtcssuhogo.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shuidangran.top/gthjdcspxj.html

PHP:  assert($x > 0);
来源：http://hz.hysaishi.cn/gtvlrlgqqz.html

JS:   console.assert(x > 0);
来源：http://hz.jiagoushi.top/gtqfgqaetb.html

TS:   console.assert(x > 0);
来源：http://hz.yuanzhike.top/gthnudstmq.html

Java: assert x > 0 : "必须为正";
来源：http://hz.wangdashe.top/gtzzlrcslh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.shanyushiyangkeji.top/gtwywyowav.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tian-w.cn/gtypmdhomt.html

C#:   Debug.Assert(x > 0);
来源：http://hz.sxryk.cn/gtethuyfhn.html

[H08] 获取错误信息与堆栈
来源：http://hz.jinqigufen.top/gtajilwyla.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hfpthk.cn/gtisiwozvi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.jyoumei.cn/gtlrldgoxq.html

JS:   e.message;  e.stack
来源：http://hz.ivvv.top/gtighchwyy.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhiwuduotai.top/gtnvfmzldp.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.gotoacloud.top/gtrxfqxaas.html

Go:   err.Error()
来源：http://hz.yangfankeji.com/gtsepzkajs.html

Ruby: e.message;  e.backtrace
来源：http://hz.ivvv.top/gtapjxhrow.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ehwqpu.com/gtgvypkxli.html

[H09] 带错误码的异常
来源：http://hz.fzhhl.top/gtalvlngrh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hywenlv.cn/gtxexrynqd.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.birdmap.top/gttdnpatem.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.mhx1999.top/gtzkrtumev.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xylfe.cn/gtgebvcdyc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.dianchejie.cn/gtmmrealhq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.smart0.xyz/gtvqbuuviy.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.quarkkingdee.top/gthpmzhxzt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.316326.xyz/gthzsfzocx.html

[H10] 资源自动释放
来源：http://hz.wangshuangyany.cn/gtwxniiumb.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jianghu66.top/gtrcuuqleq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.ivvv.top/gtvbvkurwm.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sweek.top/gtrlrjzslx.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgufenzy.top/gtqggmgbwj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yuxming.cn/gtfqduveri.html

Go:   defer f.Close()
来源：http://hz.316326.xyz/gtzxsryeek.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.feifeiyinyue.top/gtmwnzvmri.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.vqdsnc.cn/gtqxhzkfvi.html

================================================================================
来源：http://hz.yuanzhike.top/gtvaobveym.html

I. 正则表达式
来源：http://hz.cashguo.top/gtlfenzsix.html

================================================================================
来源：http://hz.c1oappe.top/gtggprepzy.html

[I01] 判断是否匹配
来源：http://hz.cqqwz.cn/gtlnozdocz.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.birdmap.top/gtivdejtfc.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhaomingkeji.xyz/gtmruhsvrq.html

JS:   /\d+/.test(s)
来源：http://hz.cucudq.cn/gteocvxfnk.html

TS:   /\d+/.test(s)
来源：http://hz.xingfuxueyuan.xyz/gtnrflaaia.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.shzxlz.cn/gtdvqxontg.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xuetiantiany.cn/gtfxhbjczr.html

Ruby: s.match?(/\d+/)
来源：http://hz.shzxlz.cn/gtvcktlqjy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jqgufenzy.top/gtxpfgkori.html

[I02] 提取所有匹配
来源：http://hz.xylfe.cn/gtooxdflms.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinyuanbaomall.cn/gtajnwgdms.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yvedp.cn/gtbefwgnss.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zdqjudy.top/gtwvnvorjy.html

TS:   s.match(/\d+/g)
来源：http://hz.jinghuilouyu.cn/gtfkxrfvek.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.xingfuxueyuan.xyz/gtfcgzsiux.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.tian-w.cn/gtoztatvqm.html

Ruby: s.scan(/\d+/)
来源：http://hz.quarkkingdee.top/gtnunmdknb.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.wangshuangyany.cn/gtuwuozdqm.html

[I03] 提取捕获分组
来源：http://hz.tianlin.xyz/gtivkhyfxp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yongpay.top/gtwpkgcyip.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.gotoacloud.top/gtftpdsedo.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yj20258888.top/gtybmyommc.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.guannengcc.top/gtpqgpwjqn.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhoulong.xyz/gtrqxwqput.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.havefunace.top/gtccvetlpt.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.cashguo.top/gtnfifdhbd.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhixingplan.top/gttwewaide.html

[I04] 正则替换
来源：http://hz.yvedp.cn/gtxtfgoqyt.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.xuanzx.com/gtqqcawdpy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.guannengcc.top/gtmqmzxvwf.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shanyushiyangtech.top/gtodxltyce.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.vqdsnc.cn/gtfkkrvflb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.redwolf501.top/gtbqyjfyjy.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.mhx1999.top/gthcfdwzqg.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yj20258888.top/gtpgmquhnf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nanxinkj.top/gtmdtpjhvw.html

[I05] 按正则拆分
来源：http://hz.jiagoushi.top/gtmiljrxhn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ivvv.top/gtrtwmqxte.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yj20258.top/gtpoozitqr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yongpay.top/gtmqnmdkmr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.zhongyouzk.top/gtfwwdikrw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.ppjwa.cn/gtshxulcwv.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.fzhhl.top/gtujbezqbz.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xziqi.cn/gtgbcpbjab.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.gaohongyu789.top/gttnwgcbmu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.nanxuanxn.top/gtriipfiec.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinyuanbaomall.cn/gtxteyfwxs.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xuanzx.com/gtknshwvhu.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gaohongyu789.top/gtbolmnhst.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.dashuyun.cn/gtzjectzla.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.aibaodan.cn/gtlzqzmhbe.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.gzhubu.top/gtmbsxvzaf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.sufxvd.cn/gtyupfgpvn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.chenlongwang.top/gtggwwhjxt.html

[I07] 忽略大小写与多行模式
来源：http://hz.yvedp.cn/gtjwusrlio.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.nanxinkj.top/gtbzpodkkg.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hnqzz.top/gtoxpztrxd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.cdnleiting.top/gtuxqtdnlm.html

TS:   /error/gim
来源：http://hz.yvedp.cn/gtpyykivoh.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zycfv.cn/gtnleurpda.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jyoumei.cn/gthyxjkxue.html

Ruby: s.scan(/error/i)
来源：http://hz.yj20258888.top/gtlryijfmu.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhengqikj.top/gtcfghwlbi.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.gzhubu.top/gtjvnxxgnr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.yanxiufei.cn/gtrfzjuwvd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.ydzc1.top/gtkghibkcb.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yj20258.top/gtjhuqrkbs.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuetiantiany.cn/gtjyrichto.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cheryme.top/gtwlpmeyyn.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.ehwqpu.com/gtsfaapxzy.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.mhx1999.top/gtdesncbfi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.chenlongwang.top/gtznzjnirl.html

================================================================================
来源：http://hz.yueranfly.top/gtacvmjewt.html

J. 日期与时间
来源：http://hz.sweek.top/gtzrappbow.html

================================================================================
来源：http://hz.9152youxi.cn/gtjyjbpldq.html

[J01] 获取当前时间
来源：http://hz.aibaodan.cn/gtlucvdvaq.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shuidangran.top/gtlbifbmpn.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yuanzhike.top/gtztgabkgk.html

JS:   new Date();  Date.now()
来源：http://hz.nwbrower.top/gtmkaulsdz.html

TS:   new Date();  Date.now()
来源：http://hz.vqdsnc.cn/gtjxrowklu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.aizwys.cn/gtxdmdvdig.html

Go:   time.Now()
来源：http://hz.yanxiufei.cn/gtelzswthn.html

Ruby: Time.now
来源：http://hz.iojbl.cn/gtahojbqmu.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.kuanghao11.cn/gtnhmogdsc.html

[J02] 格式化输出
来源：http://hz.xingfuxueyuan.xyz/gtkspfgmuc.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.c1oappe.top/gtpicknwot.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yongpay.top/gtkvyjbnrz.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xuanzx.com/gtjeycuhvd.html

TS:   d.toISOString()
来源：http://hz.cucudq.cn/gtiebaeneg.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.bjfxy.top/gtjcoekafx.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.hongshengwenyu.top/gtxoqeachx.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhoulong.xyz/gttjvmikhr.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.shuidangran.top/gtilpvpljc.html

[J03] 字符串解析为日期
来源：http://hz.xinyue.icu/gtxebplpma.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.havefunace.top/gtkoxstulz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yj20258.top/gtghyqrxnz.html

JS:   new Date("2024-01-02")
来源：http://hz.yj202588.top/gtlbgfhqcn.html

TS:   new Date("2024-01-02")
来源：http://hz.vqdsnc.cn/gteovwwusl.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.tanke756.top/gtdhhurazo.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hnxiangtu.top/gtrqckyagh.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.gogol.net.cn/gtmjkbcjqg.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hnqzz.top/gtshkgkitt.html

[J04] 时间戳与日期互转
来源：http://hz.cdnleiting.top/gtowsmolhr.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yuanzhike.top/gtiqnkabmk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.snrcjt.cn/gtcgzzxpnj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.guowangkeji.top/gtjfmzfcxq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.52xcode.cn/gttgqsbkfo.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.daria6918.cn/gteyppbpbz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.shangyingyoupin.top/gtmlrwtnkh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.yj20258.top/gtxphatdoq.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.wangshuangyany.cn/gttdxrtrsn.html

[J05] 时间加减（加 7 天）
来源：http://hz.xingfuxueyuan.xyz/gtpjtahscu.html

Py:   now + timedelta(days=7)
来源：http://hz.fzhhl.top/gttwkhwmjc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.pycfn.com/gtvkgksheo.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.aibaodan.cn/gtowohhube.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yuanzhike.top/gtsesqmsdu.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ehwqpu.com/gtouryjkqp.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.shanyushiyangtech.top/gtichsrngw.html

Ruby: Time.now + 7 * 86400
来源：http://hz.chenzaomai.com/gtlrsqgrsl.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.yuxming.cn/gtjghbftuj.html

[J06] 计算两时间之差
来源：http://hz.c1oappe.top/gtbfpqgxqt.html

Py:   (end - start).total_seconds()
来源：http://hz.yueranfly.top/gtxgkdezjd.html

PHP:  $end->diff($start)->days;
来源：http://hz.daria6918.cn/gtpzdcejhj.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.wangshuangyany.cn/gtsgiuapiu.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhaomingkeji.xyz/gthkjnxedm.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.sweek.top/gtpnsohzmb.html

Go:   end.Sub(start).Hours()
来源：http://hz.yongpay.top/gtelwgnzcw.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hongshengwenyu.top/gtsiuinolh.html

C#:   (end - start).TotalSeconds
来源：http://hz.52xcode.cn/gtyaoygfxn.html

[J07] 比较两个日期
来源：http://hz.xinyue.icu/gtnqywhfla.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtddsmtwij.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jinghuilouyu.cn/gtoteikdsb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.daxiang520.top/gtdrtceodn.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xuetiantiany.cn/gthvxpapqx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.ydzc1.top/gtfkejtpgb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.shuidangran.top/gtqgyayauc.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.nanxinkj.top/gtrnogtxmc.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.shuidangran.top/gtzbfnciol.html

[J08] 提取年月日与星期
来源：http://hz.snrcjt.cn/gtqdqwsoym.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hnxiangtu.top/gtuxcsobdl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.feifeiyinyue.top/gtbhivrteq.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.guannengcc.top/gtmgzqnmht.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.nanxinkj.top/gtkynlcbly.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xingfuxueyuan.xyz/gtllbcxara.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.yvedp.cn/gtynfjwtcv.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.xuanzx.com/gtsgnmlcaw.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.xuanzx.com/gtfhllmxfo.html

[J09] 时区处理
来源：http://hz.yvedp.cn/gtcnfjkntj.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.xinyue.icu/gtxfpoogwj.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.vqdsnc.cn/gtbsxtymjh.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.zhaomingkeji.xyz/gtpchkcbih.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sysykeji.top/gtyngzmysn.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.xziqi.cn/gtrgtqhubs.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.daxiang520.top/gtshkpsuwl.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.daria6918.cn/gtvaiwnhag.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.0kj1m.cn/gtkjkeokvj.html

[J10] 取今天 / 本月第一天
来源：http://hz.jinghuilouyu.cn/gtrsgilarf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.gotoacloud.top/gtgwsbwglg.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hnxiangtu.top/gtscwwjvfu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.shangyingyoupin.top/gthrykktfj.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.hywenlv.cn/gtwxyyilhm.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.iojbl.cn/gtvdiialsr.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.xingfuxueyuan.xyz/gtpdkolcag.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.xuetiantiany.cn/gtlkqohvls.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.daria6918.cn/gtpzhnblwl.html

================================================================================
来源：http://hz.sufxvd.cn/gtjlvwjzee.html

K. JSON 与序列化
来源：http://hz.0kj1m.cn/gtsnnebdyb.html

================================================================================
来源：http://hz.sufxvd.cn/gtudgoziij.html

[K01] 对象转 JSON 字符串
来源：http://hz.jqgfzy.top/gtbkqlnxdw.html


<!-- 参考信息 -->