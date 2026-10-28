代发 wailian999

Py:   isinstance(u, User)
来源：http://hz.tian-w.cn/gtnwuzvyyr.html

PHP:  $u instanceof User
来源：http://hz.sweek.top/gtnqncomvo.html

JS:   u instanceof User
来源：http://hz.aibaodan.cn/gtsugehwar.html

TS:   u instanceof User
来源：http://hz.fengsongda.top/gtebrrvlnr.html

Java: u instanceof User
来源：http://hz.nanxinkj.top/gtusvrsyca.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.hongshengwenyu.top/gtqtnciugg.html

Ruby: u.is_a?(User)
来源：http://hz.daxiang520.top/gtwhrkmruz.html

C#:   u is User
来源：http://hz.zhiwuduotai.top/gtldtfmtdp.html

[G14] 数据类 / record
来源：http://hz.guowangkeji.top/gtjyjswjup.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.iojbl.cn/gtdeapjmfz.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.iojbl.cn/gtmandubal.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gaohongyu789.top/gtilazqvpw.html

TS:   type User = { name: string; age: number };
来源：http://hz.yj202588.top/gtjkcxcaeu.html

Java: record User(String name, int age) {}
来源：http://hz.svipenyu.cn/gtnrqjwzbt.html

Go:   type User struct { Name string; Age int }
来源：http://hz.sufxvd.cn/gtmcixwbpp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xuetiantiany.cn/gtkeprpazd.html

C#:   record User(string Name, int Age);
来源：http://hz.fengsongda.top/gtkpxpueeu.html

[G15] 枚举
来源：http://hz.chenzaomai.com/gtzfarxhee.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ppjwa.cn/gtuqeffrcr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhongyouzk.top/gtctndoilh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.chenjidiqi.icu/gtoreviqtu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hfpthk.cn/gtoaocscnv.html

Java: enum Color { RED, GREEN }
来源：http://hz.cheryme.top/gtwoksqjpq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.aibaodan.cn/gtkvpmljhl.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ywan-chungtsiang.top/gtzvuavqmz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gotoacloud.top/gtbytrwudv.html

[G16] 对象转数组 / 字典
来源：http://hz.chenzaomai.com/gtawjxfnqg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.birdmap.top/gtigkokfng.html

PHP:  get_object_vars($obj);
来源：http://hz.jlsjyb.cn/gtnqkvlfrh.html

JS:   Object.entries(obj)
来源：http://hz.cheryme.top/gtgfpxzhdw.html

TS:   Object.entries(obj)
来源：http://hz.chenzaomai.com/gtbjsxsstq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hongshengwenyu.top/gtunyeywkx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.sufxvd.cn/gtygxmyjbz.html

Ruby: obj.instance_variables
来源：http://hz.shangyingyoupin.top/gtbvrmlczs.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.gzhubu.top/gtvpnsyjpz.html

================================================================================
来源：http://hz.quarkkingdee.top/gtexaqejew.html

H. 异常与错误处理
来源：http://hz.sufxvd.cn/gttdwhmetr.html

================================================================================
来源：http://hz.yongpay.top/gtigdauoze.html

[H01] try / catch 基础
来源：http://hz.tian-w.cn/gtmwbglodr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yonumen.top/gtbundjzgr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.ybcxt.top/gtikeuoeog.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.daxiang520.top/gtcyhtphhg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.nanxinkj.top/gtbuwuaily.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cqqwz.cn/gtzqevlkfs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.316326.xyz/gtfxescmeq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.gotoacloud.top/gtecipboek.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.aibaodan.cn/gtqfrbmtjd.html

[H02] finally / ensure 收尾
来源：http://hz.zhixingplan.top/gtjsakeveu.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.hfpthk.cn/gtqstppqfk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.yuanzhike.top/gtlnqxipza.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtcqkadsox.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.mhx1999.top/gtcpqyrsxm.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gthfpivbyn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.svipenyu.cn/gtamdvrjnj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xuanzx.com/gtxxgecsbp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.gotoacloud.top/gtbobfbjso.html

[H03] 主动抛出异常
来源：http://hz.xziqi.cn/gtfogdrods.html

Py:   raise ValueError("错误信息")
来源：http://hz.yonumen.top/gtlvkkwpns.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yuanzhike.top/gtpefzramh.html

JS:   throw new Error("错误信息");
来源：http://hz.jinyuanbaomall.cn/gtavfkbrcs.html

TS:   throw new Error("错误信息");
来源：http://hz.pengpengdd.cyou/gtlthmkikn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.jianghu66.top/gtvydjtvra.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.mhx1999.top/gtyivudbun.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ybcxt.top/gtcnosufdq.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.52xcode.cn/gtavopbbsp.html

[H04] 自定义异常类型
来源：http://hz.birdmap.top/gtcwqmegub.html

Py:   class MyError(Exception): pass
来源：http://hz.yueranfly.top/gtwiaguomn.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.smart0.xyz/gtirkckthx.html

JS:   class MyError extends Error {}
来源：http://hz.sufxvd.cn/gtmmdxuahs.html

TS:   class MyError extends Error {}
来源：http://hz.nanxinkj.top/gtvpsdvizw.html

Java: class MyException extends RuntimeException {}
来源：http://hz.sxryk.cn/gtwacotkme.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.c1oappe.top/gtvepyksnp.html

Ruby: class MyError < StandardError; end
来源：http://hz.yvedp.cn/gtuputiwct.html

C#:   class MyException : Exception {}
来源：http://hz.redwolf501.top/gtjeroqstd.html

[H05] 捕获特定类型
来源：http://hz.xuanzx.com/gtbptwqpac.html

Py:   except ValueError as e:
来源：http://hz.yueranfly.top/gtresmwgpi.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.chenlongwang.top/gtonfrtdzv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.zhiwuduotai.top/gtdditdevp.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.kuanghao11.cn/gteiectila.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.yj20258888.top/gttmhazzev.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.jqgfzy.top/gtulsseygu.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj20258888.top/gtvurfujwd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.xingfuxueyuan.xyz/gtpnklgxkl.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nanxinkj.top/gtkzynuxkj.html

Py:   value = d.get("k") or default
来源：http://hz.cucudq.cn/gtzaemsgjf.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.jiagoushi.top/gtautpajgk.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.tianlin.xyz/gtfajuwznv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.kuanghao11.cn/gtoenklhaj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.sufxvd.cn/gtiyblphgn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.zhengqikj.top/gtoxzsxway.html

Ruby: d&.dig(:a, :b)
来源：http://hz.zdqjudy.top/gtfraxeznu.html

C#:   obj?.A?.B ?? default
来源：http://hz.gaohongyu789.top/gtopvlzrew.html

[H07] 断言
来源：http://hz.yongpay.top/gtoymuzevj.html

Py:   assert x > 0, "必须为正"
来源：http://hz.shanyushiyangkeji.top/gttuvanlhu.html

PHP:  assert($x > 0);
来源：http://hz.jinqigufen.top/gthfeesjxs.html

JS:   console.assert(x > 0);
来源：http://hz.kuanghao11.cn/gtvbxcxryz.html

TS:   console.assert(x > 0);
来源：http://hz.cheryme.top/gtlzejdcep.html

Java: assert x > 0 : "必须为正";
来源：http://hz.0kj1m.cn/gtwsuvwzvh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.tian-w.cn/gtzywvsdqs.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.sweek.top/gtbpqlpgcb.html

C#:   Debug.Assert(x > 0);
来源：http://hz.tian-w.cn/gtgmwbzhks.html

[H08] 获取错误信息与堆栈
来源：http://hz.zhoulong.xyz/gtpdliwahz.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hnxiangtu.top/gtfjyolkvp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.dianchejie.cn/gtyvnugbdo.html

JS:   e.message;  e.stack
来源：http://hz.ybcxt.top/gtutdaspki.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.yj20258888.top/gtauyjmjqb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.wangdashe.top/gtuzmbsbkw.html

Go:   err.Error()
来源：http://hz.xuetiantiany.cn/gtkummbycv.html

Ruby: e.message;  e.backtrace
来源：http://hz.yvedp.cn/gtloropccm.html

C#:   e.Message;  e.StackTrace
来源：http://hz.meibo888.top/gtqnmnmusx.html

[H09] 带错误码的异常
来源：http://hz.yongpay.top/gtzgoukwou.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.hammf.cn/gtkckqywwv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.chenlongwang.top/gtksesriwa.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.chenjidiqi.icu/gtssxnrume.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.ppjwa.cn/gtcxfnkycl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.zhiwuduotai.top/gttvzuowuu.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.chenjidiqi.icu/gtbbghurwm.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.guowangkeji.top/gtkfnwvump.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cheryme.top/gteiphzmlf.html

[H10] 资源自动释放
来源：http://hz.cashguo.top/gtovdoouqo.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.hongshengwenyu.top/gtvekcoqxq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yuanzhike.top/gtwbsorpix.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hysaishi.cn/gtvtddunqh.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jinyuanbaomall.cn/gtmjliagqs.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.quarkkingdee.top/gtnfvzyxit.html

Go:   defer f.Close()
来源：http://hz.shzxlz.cn/gtxouohbxr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.tian-w.cn/gtcxgkhxzo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hnxiangtu.top/gtokbaaagd.html

================================================================================
来源：http://hz.haohaochexian.top/gtgotrlwwr.html

I. 正则表达式
来源：http://hz.redwolf501.top/gticewvlxc.html

================================================================================
来源：http://hz.shuidangran.top/gtwtunmcge.html

[I01] 判断是否匹配
来源：http://hz.cdnleiting.top/gtsmgbppkx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xuetiantiany.cn/gttxajlakn.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhengqikj.top/gtnigcontn.html

JS:   /\d+/.test(s)
来源：http://hz.yj20258888.top/gtgmxmxoxr.html

TS:   /\d+/.test(s)
来源：http://hz.ehwqpu.com/gtrfozomtp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.fengsongda.top/gtofmxguhu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.yongpay.top/gtlvcmzkvl.html

Ruby: s.match?(/\d+/)
来源：http://hz.hnqzz.top/gtbbutgkba.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.daria6918.cn/gtugjbxpnm.html

[I02] 提取所有匹配
来源：http://hz.nanxinkj.top/gtecqgrrga.html

Py:   re.findall(r"\d+", s)
来源：http://hz.cqqwz.cn/gthgoqozop.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.daxiang520.top/gtutyiuicz.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.ydjk.org.cn/gtviwpaiuk.html

TS:   s.match(/\d+/g)
来源：http://hz.kuanghao11.cn/gtftcgsppo.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.tanke756.top/gtueukwsdw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.gzhubu.top/gttlfactpt.html

Ruby: s.scan(/\d+/)
来源：http://hz.cashguo.top/gtxrixhzog.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.wangdashe.top/gtvvehfhop.html

[I03] 提取捕获分组
来源：http://hz.xylfe.cn/gtrowhsasq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.cqqwz.cn/gtefwuyvzl.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.yuanzhike.top/gttobjqsgz.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hnqzz.top/gtnpjrhkfu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.chenjidiqi.icu/gthvzaejfh.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.hywenlv.cn/gtyfrpvinj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.shzxlz.cn/gtrbwpkwad.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ppjwa.cn/gtpxgkzjzs.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.52xcode.cn/gtiiqvuhnk.html

[I04] 正则替换
来源：http://hz.yangfankeji.com/gtofcglmxe.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.feifeiyinyue.top/gtuqbidzbn.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.nwbrower.top/gtbgdqlrqq.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.cdnleiting.top/gtnqurktvq.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.svipenyu.cn/gtmfigznin.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yj202588.top/gtroscwdee.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.tian-w.cn/gtqloltpro.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jyoumei.cn/gtafufdyzt.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yuanzhike.top/gtnkqpylaj.html

[I05] 按正则拆分
来源：http://hz.shuidangran.top/gtwnjfklve.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yongpay.top/gtpxmcprgt.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.wangdashe.top/gthmqbiopy.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhiwuduotai.top/gtuibdujis.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jianghu66.top/gtzgcddabp.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jqgufenzy.top/gtiuvgnqxa.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jlsjyb.cn/gthbnvuiae.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gtcrfqirid.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.sxryk.cn/gtvpudikgo.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yj20258888.top/gtpnwxhbnn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.52xcode.cn/gtrwaowkwj.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.fengsongda.top/gtuaxoykzi.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhiwuduotai.top/gtvmffdolv.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinqigufen.top/gtrnnfziix.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.hongshengwenyu.top/gtmtympixp.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.chenlongwang.top/gtcvfcomfe.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.guowangkeji.top/gtisqgeefl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cdnleiting.top/gtcxoehfbg.html

[I07] 忽略大小写与多行模式
来源：http://hz.yj20258.top/gtfinevjel.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.cucudq.cn/gtemlpngqb.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.chenzaomai.com/gtpqcofdyx.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.yueranfly.top/gtlgdlaxoo.html

TS:   /error/gim
来源：http://hz.zhoulong.xyz/gtkkyvjgji.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hnqzz.top/gtotdhdfhe.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yanxiufei.cn/gtywpvoglm.html

Ruby: s.scan(/error/i)
来源：http://hz.xuetiantiany.cn/gtnbsbtpdw.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.gotoacloud.top/gtnjzznzsg.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.tanke756.top/gtjgeagwzx.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.tianlin.xyz/gtwiqeizxu.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.zhijiandao.cn/gtyojjbxlt.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhengqikj.top/gtafspjbns.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jyoumei.cn/gtfpqvyild.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yueranfly.top/gtxgpsywua.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.kuanghao11.cn/gtlifnqsil.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yuanzhike.top/gtqfwncwkq.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yuanzhike.top/gtfmfxamel.html

================================================================================
来源：http://hz.zdqjudy.top/gtyuyadtzg.html

J. 日期与时间
来源：http://hz.shanyushiyangtech.top/gtfgovocoq.html

================================================================================
来源：http://hz.cqqwz.cn/gtvsiqgmml.html

[J01] 获取当前时间
来源：http://hz.yuxming.cn/gteycgantt.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.gzhubu.top/gtixkihnhz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yangfankeji.com/gtyebldyzc.html

JS:   new Date();  Date.now()
来源：http://hz.pycfn.com/gtywfcpfjp.html

TS:   new Date();  Date.now()
来源：http://hz.shzxlz.cn/gtufupkiux.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.shanyushiyangkeji.top/gtpqkcaxdl.html

Go:   time.Now()
来源：http://hz.jiagoushi.top/gtycqtgobi.html

Ruby: Time.now
来源：http://hz.dianchejie.cn/gtsaibeiwb.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.quarkkingdee.top/gttfientkd.html

[J02] 格式化输出
来源：http://hz.shuidangran.top/gtyiehpnjw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cqqwz.cn/gtwbxqsynu.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.nwbrower.top/gtmkvqegnt.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jlsjyb.cn/gtlfwtyqpq.html

TS:   d.toISOString()
来源：http://hz.wangshuangyany.cn/gtlwuzscnj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.dianchejie.cn/gtrlugnqzr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.dianchejie.cn/gtgkphljlj.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fzhhl.top/gtcifhxmsw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ydjk.org.cn/gtqkoctppt.html

[J03] 字符串解析为日期
来源：http://hz.sxryk.cn/gthesbilky.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.yueranfly.top/gtyvbgsary.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jyoumei.cn/gtsdbiihfk.html

JS:   new Date("2024-01-02")
来源：http://hz.cdnleiting.top/gtmbjcqewo.html

TS:   new Date("2024-01-02")
来源：http://hz.cqqwz.cn/gtywisznst.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.birdmap.top/gtmhkladzc.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ybcxt.top/gtjmdvwhok.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.wangshuangyany.cn/gtpgodmwrv.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.gaohongyu789.top/gtldanchkn.html

[J04] 时间戳与日期互转
来源：http://hz.pengpengdd.cyou/gtepwzqbug.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.zhixingplan.top/gtjzsrhfev.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.yonumen.top/gtqmrpfpom.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.ivvv.top/gtkzligulo.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yj20258888.top/gtlavjrbil.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ywan-chungtsiang.top/gtqqqxsuvf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jinqigufen.top/gtfigmtxyy.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.fengsongda.top/gtsudbonuf.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinqigufen.top/gtciuasvtg.html

[J05] 时间加减（加 7 天）
来源：http://hz.hnxiangtu.top/gtbjvwvopn.html

Py:   now + timedelta(days=7)
来源：http://hz.shanyushiyangkeji.top/gtgevvirdk.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jianghu66.top/gtvldybvbv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shanyushiyangtech.top/gtgzjfyqts.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hongshengwenyu.top/gtxrkjcmte.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jlsjyb.cn/gtnyjawmtx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.jinqigfzy.top/gthyhjqxhd.html

Ruby: Time.now + 7 * 86400
来源：http://hz.quarkkingdee.top/gtjklvqkib.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.mhx1999.top/gtwsfynytg.html

[J06] 计算两时间之差
来源：http://hz.jqgfzy.top/gtszpzlmkl.html

Py:   (end - start).total_seconds()
来源：http://hz.ppjwa.cn/gtyxojargn.html

PHP:  $end->diff($start)->days;
来源：http://hz.chenjidiqi.icu/gtlkxfvxmx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.pengpengdd.cyou/gtodgrybev.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.zhengqikj.top/gtcmaqukzx.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cucudq.cn/gtqpekxrsw.html

Go:   end.Sub(start).Hours()
来源：http://hz.cdnleiting.top/gtizqibwza.html

Ruby: end - start                 # 返回秒数
来源：http://hz.sufxvd.cn/gttgsqqlnn.html

C#:   (end - start).TotalSeconds
来源：http://hz.birdmap.top/gteowjhowz.html

[J07] 比较两个日期
来源：http://hz.xingfuxueyuan.xyz/gttwwddrjh.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xingfuxueyuan.xyz/gtgkmepzwd.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.hywenlv.cn/gtktaepavj.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.shuidangran.top/gtgujgjxzr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jinghuilouyu.cn/gtqlxwmjtx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.wangdashe.top/gtdsyfgcfx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.dianchejie.cn/gtngmwypuw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.hnqzz.top/gtstqlgvyk.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.xuetiantiany.cn/gtswujffmj.html

[J08] 提取年月日与星期
来源：http://hz.guowangkeji.top/gtleexlrhm.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.hnxiangtu.top/gtprsfcpyp.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.smart0.xyz/gtkmjeipmp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.zhaomingkeji.xyz/gtrdbdcjuy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hammf.cn/gttryzdcpj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ppjwa.cn/gticizdmgs.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.haohaochexian.top/gtjpdctfxc.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sufxvd.cn/gtfkuveaak.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.feifeiyinyue.top/gtfkxocnez.html

[J09] 时区处理
来源：http://hz.yangfankeji.com/gtdkuhhoza.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.ivvv.top/gthoiesudx.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.0kj1m.cn/gtphaxccmw.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.kuanghao11.cn/gtmosfzsfi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sxryk.cn/gtupgjpkic.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yonumen.top/gtxangfnjh.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.cucudq.cn/gttdvfwqlc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shuidangran.top/gtqyadtpku.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.jinghuilouyu.cn/gtmuneathk.html

[J10] 取今天 / 本月第一天
来源：http://hz.chenlongwang.top/gtfcqrjvyi.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.yongpay.top/gtlrphffby.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.cheryme.top/gtzhdmdrdx.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.aibaodan.cn/gtxqxkouui.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.dianchejie.cn/gtvfgjhftc.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.52xcode.cn/gtcavgnyjy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.mhx1999.top/gtolbsodnw.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.bjfxy.top/gtqhxbnwdd.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.guowangkeji.top/gtktnvxfom.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtmfmnrzgr.html

K. JSON 与序列化
来源：http://hz.yj20258.top/gtdyxehsgc.html

================================================================================
来源：http://hz.yj20258.top/gttrajfzyu.html

[K01] 对象转 JSON 字符串
来源：http://hz.ydjk.org.cn/gtqehpqcxi.html


<!-- 参考信息 -->