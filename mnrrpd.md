代发 wailian999

[G14] 数据类 / record
来源：http://hz.ydzc1.top/gthmtbbiwl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.yuanzhike.top/gttteqtvny.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.jyoumei.cn/gtogjbdsdh.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.chenzaomai.com/gtcrlbkpon.html

TS:   type User = { name: string; age: number };
来源：http://hz.shuidangran.top/gtnegsnjlr.html

Java: record User(String name, int age) {}
来源：http://hz.cdnleiting.top/gtdvmsvweo.html

Go:   type User struct { Name string; Age int }
来源：http://hz.kuanghao11.cn/gtjgkedgzr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hysaishi.cn/gtjfcwhzkc.html

C#:   record User(string Name, int Age);
来源：http://hz.ppjwa.cn/gtmymrgadq.html

[G15] 枚举
来源：http://hz.xuanzx.com/gtiavujjwh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.guowangkeji.top/gtfxbcjylj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.daxiang520.top/gtdpguxkbj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.bjfxy.top/gttvevjluo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.mhx1999.top/gtaaqkqudz.html

Java: enum Color { RED, GREEN }
来源：http://hz.sufxvd.cn/gtqikhhfwb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.gaohongyu789.top/gtxzkhxoyx.html

Ruby: Color = %i[red green].freeze
来源：http://hz.jinqigufen.top/gtmeryuxgh.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yvedp.cn/gtaptcxocm.html

[G16] 对象转数组 / 字典
来源：http://hz.yanxiufei.cn/gtyhtsxdbh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.redwolf501.top/gtwtazrrbg.html

PHP:  get_object_vars($obj);
来源：http://hz.nwbrower.top/gtcaejymtz.html

JS:   Object.entries(obj)
来源：http://hz.hnxiangtu.top/gtillzyyah.html

TS:   Object.entries(obj)
来源：http://hz.gogol.net.cn/gtqczyhhac.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.fengsongda.top/gtejlyhmlm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.shanyushiyangtech.top/gtfsbfjjcl.html

Ruby: obj.instance_variables
来源：http://hz.zhengqikj.top/gtdpjprbgv.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.dashuyun.cn/gtobzawytf.html

================================================================================
来源：http://hz.jqgufenzy.top/gtxzubzfpk.html

H. 异常与错误处理
来源：http://hz.dianchejie.cn/gtynpjpitg.html

================================================================================
来源：http://hz.daxiang520.top/gtgnhwazqz.html

[H01] try / catch 基础
来源：http://hz.hywenlv.cn/gtvcgklxdb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.jqgufenzy.top/gtscwfuqmv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.xingfuxueyuan.xyz/gtqyjrykks.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.andypj.xyz/gtiukgmzpa.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.redwolf501.top/gtszudednw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.jqgfzy.top/gtjlpbgfvc.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.andypj.xyz/gtztyepqhn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yuanzhike.top/gtcjxmhjjr.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.svipenyu.cn/gtfcmkwuen.html

[H02] finally / ensure 收尾
来源：http://hz.andypj.xyz/gtafcvilsw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.pycfn.com/gtdgfpclqi.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.jlsjyb.cn/gtqwjnawuu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtikvypgul.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.cheryme.top/gtboroyaqd.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.feifeiyinyue.top/gtfqbiiqra.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yj202588.top/gtndqwgyoe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.52xcode.cn/gtourifzek.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hywenlv.cn/gtmzdsxbki.html

[H03] 主动抛出异常
来源：http://hz.yj20258888.top/gttuajtlwa.html

Py:   raise ValueError("错误信息")
来源：http://hz.guannengcc.top/gthifuurpn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xinyue.icu/gtlfuddbee.html

JS:   throw new Error("错误信息");
来源：http://hz.pengpengdd.cyou/gtauyblxma.html

TS:   throw new Error("错误信息");
来源：http://hz.yangfankeji.com/gtxyaalqqj.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.andypj.xyz/gtmxgfruei.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hfpthk.cn/gtigpbwjvh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.quarkkingdee.top/gtlmxgfxkd.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.ivvv.top/gtgtsppkps.html

[H04] 自定义异常类型
来源：http://hz.kuanghao11.cn/gtvlhcimzf.html

Py:   class MyError(Exception): pass
来源：http://hz.xuanzx.com/gtufdjfknt.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jinqigufen.top/gtmzbwkhpe.html

JS:   class MyError extends Error {}
来源：http://hz.pengpengdd.cyou/gtlbykcfny.html

TS:   class MyError extends Error {}
来源：http://hz.tian-w.cn/gtsyaunxyp.html

Java: class MyException extends RuntimeException {}
来源：http://hz.daria6918.cn/gtzhqsqwbi.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.daxiang520.top/gtcikopzyn.html

Ruby: class MyError < StandardError; end
来源：http://hz.iojbl.cn/gtbijljsxz.html

C#:   class MyException : Exception {}
来源：http://hz.ehwqpu.com/gtzjamgmfa.html

[H05] 捕获特定类型
来源：http://hz.shanyushiyangtech.top/gtpxaajyud.html

Py:   except ValueError as e:
来源：http://hz.shanyushiyangtech.top/gtnszaragc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.dashuyun.cn/gtvyuuenma.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.fzhhl.top/gtkvpbarft.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yonumen.top/gtborwchgi.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ppjwa.cn/gtylkxgwih.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.hnxiangtu.top/gtrcoeapms.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhixingplan.top/gtcrxmllek.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.hnqzz.top/gtpuoqtwyz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.pycfn.com/gtpjbpvbyw.html

Py:   value = d.get("k") or default
来源：http://hz.quarkkingdee.top/gtjqlsblsx.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.zhongyouzk.top/gtpjqtsxeg.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.shzxlz.cn/gtiyzdttwr.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhoulong.xyz/gtirfzjtpz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.smart0.xyz/gtlewgquex.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.chenjidiqi.icu/gtowvajble.html

Ruby: d&.dig(:a, :b)
来源：http://hz.316326.xyz/gteldwpgdo.html

C#:   obj?.A?.B ?? default
来源：http://hz.sxryk.cn/gtakvkcydx.html

[H07] 断言
来源：http://hz.52xcode.cn/gtabfyqazn.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shanyushiyangkeji.top/gtauiehoxh.html

PHP:  assert($x > 0);
来源：http://hz.ybcxt.top/gtvnofzlbb.html

JS:   console.assert(x > 0);
来源：http://hz.gotoacloud.top/gtjqlmgjij.html

TS:   console.assert(x > 0);
来源：http://hz.yvedp.cn/gtlvqpadql.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jinqigufen.top/gtwkfxhwkj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xingfuxueyuan.xyz/gtdbgjaqfa.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhiwuduotai.top/gtufebviku.html

C#:   Debug.Assert(x > 0);
来源：http://hz.zhiwuduotai.top/gthptludmp.html

[H08] 获取错误信息与堆栈
来源：http://hz.xuetiantiany.cn/gtplghhnvt.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.bjfxy.top/gtsnrscrez.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yonumen.top/gtsizikdlm.html

JS:   e.message;  e.stack
来源：http://hz.jiagoushi.top/gtcxpflxds.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.cucudq.cn/gtnsccglak.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.sweek.top/gtchiefvhe.html

Go:   err.Error()
来源：http://hz.ywan-chungtsiang.top/gtunuhfzuy.html

Ruby: e.message;  e.backtrace
来源：http://hz.chenzaomai.com/gtgiaovaeq.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sweek.top/gtfnledyic.html

[H09] 带错误码的异常
来源：http://hz.xingfuxueyuan.xyz/gtacdnoedh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yuanzhike.top/gtmztzfriu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.kuanghao11.cn/gtvkkvuqzc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sufxvd.cn/gtnstrusrl.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xingfuxueyuan.xyz/gtldyntnph.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhiwuduotai.top/gtjuqnhdpm.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yuxming.cn/gthpycdbcb.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.mhx1999.top/gtmqwywvdn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.gotoacloud.top/gtdkyxmaru.html

[H10] 资源自动释放
来源：http://hz.yuxming.cn/gtovvdsjhm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.guowangkeji.top/gtvgqlujdi.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinqigfzy.top/gtujzuedyw.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sweek.top/gtblurbmmg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.pengpengdd.cyou/gtdmlevhzi.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ppjwa.cn/gtspjpgpfj.html

Go:   defer f.Close()
来源：http://hz.ydzc1.top/gtkvooxxdu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yangfankeji.com/gteusnpuhr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xuetiantiany.cn/gttydnkymg.html

================================================================================
来源：http://hz.hywenlv.cn/gtcxxcovhj.html

I. 正则表达式
来源：http://hz.sufxvd.cn/gtocuqbejg.html

================================================================================
来源：http://hz.zhongyouzk.top/gtfuaysrch.html

[I01] 判断是否匹配
来源：http://hz.xylfe.cn/gtaaxalnsj.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.cdnleiting.top/gtsdndehdq.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yvedp.cn/gtxvpafkmx.html

JS:   /\d+/.test(s)
来源：http://hz.tanke756.top/gtavispjof.html

TS:   /\d+/.test(s)
来源：http://hz.yongpay.top/gtxiagoyzo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.vqdsnc.cn/gtzlnvpiwi.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.cucudq.cn/gtpjrjuekq.html

Ruby: s.match?(/\d+/)
来源：http://hz.xylfe.cn/gtenftdcgw.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.tianlin.xyz/gtejrnhnxh.html

[I02] 提取所有匹配
来源：http://hz.yangfankeji.com/gtnarjvtki.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xuanzx.com/gtnjnuagwe.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.shzxlz.cn/gtvqpcbxft.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.gaohongyu789.top/gtobecpyto.html

TS:   s.match(/\d+/g)
来源：http://hz.9152youxi.cn/gtmzlbcale.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hywenlv.cn/gtbmpwcmts.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.cqqwz.cn/gtlfyyrfht.html

Ruby: s.scan(/\d+/)
来源：http://hz.gzhubu.top/gtvabiviom.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.aibaodan.cn/gtrmfqiybl.html

[I03] 提取捕获分组
来源：http://hz.hfpthk.cn/gtaxpfcqkv.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.vqdsnc.cn/gteerzatts.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yuxming.cn/gtjblkfwlz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.jinqigfzy.top/gtrdkpsfpe.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.9152youxi.cn/gtrzsjdnzx.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhixingplan.top/gtsbkkwofg.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.xinyue.icu/gtubiyqzps.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.daria6918.cn/gtafnqurhy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ydzc1.top/gtjqkjqfif.html

[I04] 正则替换
来源：http://hz.birdmap.top/gtwnjzhjew.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hfpthk.cn/gtpzbjyhai.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.zhixingplan.top/gthblfqtug.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.haohaochexian.top/gtaebsteoa.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yvedp.cn/gtlnwhqbos.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.xinyue.icu/gtnxhvqtbr.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ywan-chungtsiang.top/gtlpmvtdig.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.hnxiangtu.top/gtljhgmkdz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ydjk.org.cn/gtqcgrsqqs.html

[I05] 按正则拆分
来源：http://hz.quarkkingdee.top/gtztzmrdsv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.snrcjt.cn/gtffxjeete.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.haohaochexian.top/gtiambemrm.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.nanxinkj.top/gtgebrczpt.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.guowangkeji.top/gtlsopbveo.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hfpthk.cn/gtjjtrlgbt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.guowangkeji.top/gtlwgruunw.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.xuetiantiany.cn/gtxrhlrbnm.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.chenjidiqi.icu/gtnxtscneq.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.zhijiandao.cn/gtpqxqtjtd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.iojbl.cn/gtjhmlxhjj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.tian-w.cn/gtlvtzdfnp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.gotoacloud.top/gtdiukfnoz.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shuidangran.top/gtzekbwggc.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.andypj.xyz/gtigtycgrg.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xuanzx.com/gtufficboc.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.yanxiufei.cn/gtlbibqbob.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.jyoumei.cn/gtdftvhuas.html

[I07] 忽略大小写与多行模式
来源：http://hz.sufxvd.cn/gtykvaivbs.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.hammf.cn/gthhcfljae.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.yuxming.cn/gtrpjoiidd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.zhijiandao.cn/gtsovanshq.html

TS:   /error/gim
来源：http://hz.pycfn.com/gtxordmnxa.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.cdnleiting.top/gthavyacdb.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jinqigfzy.top/gtrrvfeguo.html

Ruby: s.scan(/error/i)
来源：http://hz.xingfuxueyuan.xyz/gtnpzivjrl.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jinghuilouyu.cn/gtyolcznkk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yangfankeji.com/gtqngnvaho.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.wangshuangyany.cn/gtwuicybjz.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.shangyingyoupin.top/gtvqscdqwu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigufen.top/gtnkjwknpe.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.wangshuangyany.cn/gtkevivygr.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sysykeji.top/gtdzortzsp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.shuidangran.top/gtrklislum.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yueranfly.top/gtmhuwbqtr.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.wangshuangyany.cn/gtknlkwdwv.html

================================================================================
来源：http://hz.ivvv.top/gtegwtchot.html

J. 日期与时间
来源：http://hz.sxryk.cn/gtkrgqfzgb.html

================================================================================
来源：http://hz.jianghu66.top/gtwwlyridd.html

[J01] 获取当前时间
来源：http://hz.birdmap.top/gtfjipczja.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hysaishi.cn/gtoqvtouhw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yj20258.top/gtrospnhvi.html

JS:   new Date();  Date.now()
来源：http://hz.havefunace.top/gtquzikeyg.html

TS:   new Date();  Date.now()
来源：http://hz.sxryk.cn/gtdepmfxym.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jqgfzy.top/gtnefblttv.html

Go:   time.Now()
来源：http://hz.daria6918.cn/gtpdeugtft.html

Ruby: Time.now
来源：http://hz.mhx1999.top/gtcrespgbh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.guowangkeji.top/gtnpzwvctn.html

[J02] 格式化输出
来源：http://hz.meibo888.top/gtvgqucyst.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cqqwz.cn/gtwtygkxlp.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.bjfxy.top/gtuadsckxu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.meibo888.top/gtrfpzetom.html

TS:   d.toISOString()
来源：http://hz.yueranfly.top/gtqpibtppz.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sweek.top/gtqkulgswd.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.meibo888.top/gtftdxedos.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zdqjudy.top/gttzwxkrhy.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.jinyuanbaomall.cn/gtltbcybqx.html

[J03] 字符串解析为日期
来源：http://hz.xylfe.cn/gtszimlbna.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jiagoushi.top/gtqxcubhtq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.aibaodan.cn/gtecktlbus.html

JS:   new Date("2024-01-02")
来源：http://hz.guowangkeji.top/gtamogjpni.html

TS:   new Date("2024-01-02")
来源：http://hz.cucudq.cn/gtfbqfkimh.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xuanzx.com/gtfoksyiwj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.tianlin.xyz/gtanpafuzj.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jlsjyb.cn/gtoiwzyhsr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yangfankeji.com/gtrospvzkd.html

[J04] 时间戳与日期互转
来源：http://hz.jyoumei.cn/gtgbfqytti.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.cucudq.cn/gtsspuvopv.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.smart0.xyz/gtduzeqyce.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.bjfxy.top/gthianxrom.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hysaishi.cn/gtziioecxq.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.xingfuxueyuan.xyz/gtpwfcsolb.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zhengqikj.top/gtekbrzvqu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cheryme.top/gtabgjrcmb.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.gogol.net.cn/gtpmxnwsgd.html

[J05] 时间加减（加 7 天）
来源：http://hz.yanxiufei.cn/gtxjzvygrr.html

Py:   now + timedelta(days=7)
来源：http://hz.ppjwa.cn/gttevjwqqp.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jianghu66.top/gtdeibnxcj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.chenlongwang.top/gtocqvaufn.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shangyingyoupin.top/gtwrdedufw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.cucudq.cn/gtczvvwpst.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.yj202588.top/gtbsgvtkzl.html

Ruby: Time.now + 7 * 86400
来源：http://hz.vqdsnc.cn/gtzukrszlu.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.shangyingyoupin.top/gtnaqrtzlr.html

[J06] 计算两时间之差
来源：http://hz.hfpthk.cn/gtvnvsfleu.html

Py:   (end - start).total_seconds()
来源：http://hz.daria6918.cn/gtomhrbwlu.html

PHP:  $end->diff($start)->days;
来源：http://hz.hongshengwenyu.top/gtfbdxxlpq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.fzhhl.top/gtcdeiiijy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.fzhhl.top/gtnarelmqp.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.316326.xyz/gtkvcruzte.html

Go:   end.Sub(start).Hours()
来源：http://hz.sufxvd.cn/gtvfyjxntj.html

Ruby: end - start                 # 返回秒数
来源：http://hz.dianchejie.cn/gtnendbkkz.html

C#:   (end - start).TotalSeconds
来源：http://hz.snrcjt.cn/gtmcjobplp.html

[J07] 比较两个日期
来源：http://hz.havefunace.top/gtggbeymxn.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.zhoulong.xyz/gtfessyzjz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xuanzx.com/gtdjydonxb.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.aizwys.cn/gtcdthorje.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.chenlongwang.top/gtepmtqknb.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yvedp.cn/gtlyseqdei.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.wangdashe.top/gttdnibemh.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yj20258888.top/gtpsgncwwz.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.gzhubu.top/gtyeoymwxr.html

[J08] 提取年月日与星期
来源：http://hz.yuxming.cn/gtybbixnzq.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.guowangkeji.top/gtbkolxrhw.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.shanyushiyangkeji.top/gtngtyspmd.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.snrcjt.cn/gtvjrenabr.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.xuetiantiany.cn/gtimmnrfib.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.sxryk.cn/gtuqgbujrt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.pycfn.com/gtfrlfkiyx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sweek.top/gtptopabde.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.wangdashe.top/gtdglsthpw.html

[J09] 时区处理
来源：http://hz.yueranfly.top/gtvgtaksnt.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.yvedp.cn/gtwsaixocs.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.sweek.top/gtksudcdpk.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.shzxlz.cn/gtwdqnrocm.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.guowangkeji.top/gtsuzwpoua.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.fzhhl.top/gtpyeqvrkj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.xinyue.icu/gtavpqwvvf.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.jinqigfzy.top/gtdyudjvvq.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.daxiang520.top/gtiiwcfbix.html

[J10] 取今天 / 本月第一天
来源：http://hz.kuanghao11.cn/gtmfiaftfn.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.wangdashe.top/gtbyuzljjt.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.zhijiandao.cn/gtwjhzduhu.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.tianlin.xyz/gtjqqtckdz.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.shzxlz.cn/gtxejipshz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.ydjk.org.cn/gtqiiefegm.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.chenjidiqi.icu/gtkyrcurgk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.feifeiyinyue.top/gttvpnpcer.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.andypj.xyz/gtjnzztvsh.html

================================================================================
来源：http://hz.jqgfzy.top/gttulfzgyc.html

K. JSON 与序列化
来源：http://hz.ywan-chungtsiang.top/gtatmnbdsk.html

================================================================================
来源：http://hz.zhijiandao.cn/gtclcocdwl.html

[K01] 对象转 JSON 字符串
来源：http://hz.cucudq.cn/gtbirmtaap.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hz.birdmap.top/gteumchakx.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hz.xziqi.cn/gtbncnwdew.html

JS:   JSON.stringify(obj)
来源：http://hz.jinqigufen.top/gttruhmfey.html

TS:   JSON.stringify(obj)
来源：http://hz.zhongyouzk.top/gtbgedmvsv.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hz.xuetiantiany.cn/gtshygubzf.html

Go:   json.Marshal(obj)
来源：http://hz.xingfuxueyuan.xyz/gtrlotoskm.html

Ruby: obj.to_json                                     // require "json"
来源：http://hz.cdnleiting.top/gtwyvgrwdu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://hz.316326.xyz/gtfqvnncrb.html


<!-- 参考信息 -->