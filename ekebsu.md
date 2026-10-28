代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yuanzhike.top/gtjfuwbvfa.html

Ruby: def to_s; @name; end
来源：http://hz.xuanzx.com/gtaqdycdzy.html

C#:   public override string ToString() => Name;
来源：http://hz.zhiwuduotai.top/gtwdffjncv.html

[G13] 判断对象类型
来源：http://hz.yangfankeji.com/gtcubzffsg.html

Py:   isinstance(u, User)
来源：http://hz.xylfe.cn/gtoollawnu.html

PHP:  $u instanceof User
来源：http://hz.zhengqikj.top/gtkkdwyybo.html

JS:   u instanceof User
来源：http://hz.snrcjt.cn/gtjpynkcpa.html

TS:   u instanceof User
来源：http://hz.yueranfly.top/gtyywfasbr.html

Java: u instanceof User
来源：http://hz.quarkkingdee.top/gtiufickez.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhoulong.xyz/gtwigaxhbg.html

Ruby: u.is_a?(User)
来源：http://hz.ydjk.org.cn/gtqhzwbymt.html

C#:   u is User
来源：http://hz.yj20258.top/gteimcncln.html

[G14] 数据类 / record
来源：http://hz.0kj1m.cn/gtpaudbblp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.ydjk.org.cn/gtngglhkzf.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.chenlongwang.top/gtyjtkbrzd.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.jiagoushi.top/gtuvsmmoea.html

TS:   type User = { name: string; age: number };
来源：http://hz.gotoacloud.top/gtybqgzjhd.html

Java: record User(String name, int age) {}
来源：http://hz.ivvv.top/gtgviemxjd.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yvedp.cn/gtiwmunzso.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.ybcxt.top/gteellaqso.html

C#:   record User(string Name, int Age);
来源：http://hz.birdmap.top/gtjllpwpfa.html

[G15] 枚举
来源：http://hz.jlsjyb.cn/gthwuvxhus.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.snrcjt.cn/gtkissbpjm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.svipenyu.cn/gtbzdndohe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yvedp.cn/gtrhmfihum.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xziqi.cn/gtpxazlsck.html

Java: enum Color { RED, GREEN }
来源：http://hz.zhaomingkeji.xyz/gtjkibtcqy.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.bjfxy.top/gtffgqnxea.html

Ruby: Color = %i[red green].freeze
来源：http://hz.c1oappe.top/gtnylsenna.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xuanzx.com/gtkvsirvjb.html

[G16] 对象转数组 / 字典
来源：http://hz.svipenyu.cn/gtjxwzbggh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.mhx1999.top/gtdxdepyij.html

PHP:  get_object_vars($obj);
来源：http://hz.shuidangran.top/gtllyeaerg.html

JS:   Object.entries(obj)
来源：http://hz.sxryk.cn/gthzvflznm.html

TS:   Object.entries(obj)
来源：http://hz.xingfuxueyuan.xyz/gtrdzbzjjc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.0kj1m.cn/gttaakokzm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.guannengcc.top/gtjbuytkbj.html

Ruby: obj.instance_variables
来源：http://hz.gzhubu.top/gtafwszfnf.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jianghu66.top/gthhboevja.html

================================================================================
来源：http://hz.tian-w.cn/gtyusgnltd.html

H. 异常与错误处理
来源：http://hz.cheryme.top/gtitxyzoua.html

================================================================================
来源：http://hz.tianlin.xyz/gtiqyjxtbt.html

[H01] try / catch 基础
来源：http://hz.pengpengdd.cyou/gtvjterquh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.hfpthk.cn/gtcyxuxyxf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.quarkkingdee.top/gtpmhiubta.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.9152youxi.cn/gtfzatosdx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hysaishi.cn/gtlcwtevol.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.tanke756.top/gtjrhatuyi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.birdmap.top/gtgboewexe.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.nanxuanxn.top/gtdydaqazb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.kuanghao11.cn/gtglrbtgnl.html

[H02] finally / ensure 收尾
来源：http://hz.quarkkingdee.top/gtaccuxhhx.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shanyushiyangkeji.top/gtzxpndrhr.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.nanxinkj.top/gtqznqzxhk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.svipenyu.cn/gtfpuahtdq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.pycfn.com/gtfmopxlcw.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.wangshuangyany.cn/gthddmnwaw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.xziqi.cn/gthnzmjiuu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.guannengcc.top/gtgtcoxnak.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.chenlongwang.top/gtlmirkyoq.html

[H03] 主动抛出异常
来源：http://hz.meibo888.top/gtmldbzgeg.html

Py:   raise ValueError("错误信息")
来源：http://hz.zdqjudy.top/gtrqwupoiz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.pycfn.com/gtlknvtslu.html

JS:   throw new Error("错误信息");
来源：http://hz.dianchejie.cn/gtxwdytspe.html

TS:   throw new Error("错误信息");
来源：http://hz.iojbl.cn/gtczgyvofg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.vqdsnc.cn/gtsxtyvnsw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.gotoacloud.top/gtpslshlnf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.nwbrower.top/gtpfwgmrwl.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhoulong.xyz/gtvbyftnqa.html

[H04] 自定义异常类型
来源：http://hz.zhoulong.xyz/gtlebwvufj.html

Py:   class MyError(Exception): pass
来源：http://hz.ydzc1.top/gtfjbakigz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.bjfxy.top/gtqztsugcs.html

JS:   class MyError extends Error {}
来源：http://hz.nanxinkj.top/gtcvhwfbjr.html

TS:   class MyError extends Error {}
来源：http://hz.cashguo.top/gtcrxhwark.html

Java: class MyException extends RuntimeException {}
来源：http://hz.316326.xyz/gtfmyjqkad.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.birdmap.top/gtfuteqvox.html

Ruby: class MyError < StandardError; end
来源：http://hz.cucudq.cn/gtqrpydrka.html

C#:   class MyException : Exception {}
来源：http://hz.zhiwuduotai.top/gtefkeqqbi.html

[H05] 捕获特定类型
来源：http://hz.yuxming.cn/gtlngnexsq.html

Py:   except ValueError as e:
来源：http://hz.andypj.xyz/gtcbdaoxyr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.guannengcc.top/gtdavtlvuz.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.cqqwz.cn/gthrccrgdb.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.daxiang520.top/gtymgilegi.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.fengsongda.top/gtewvmhbly.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.sysykeji.top/gtlzfsvbdd.html

Ruby: rescue ArgumentError => e
来源：http://hz.aizwys.cn/gtbwkdeixt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.chenzaomai.com/gtcitlbuak.html

[H06] 可选值 / 空值安全访问
来源：http://hz.9152youxi.cn/gtorklsvgr.html

Py:   value = d.get("k") or default
来源：http://hz.jqgfzy.top/gtcvqgzcey.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yueranfly.top/gtavxdusoq.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xziqi.cn/gtnbzdczfk.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.pengpengdd.cyou/gtkppxykrp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.nwbrower.top/gtrxoxavxj.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yongpay.top/gttftcfspj.html

Ruby: d&.dig(:a, :b)
来源：http://hz.guowangkeji.top/gtuccjwvab.html

C#:   obj?.A?.B ?? default
来源：http://hz.cashguo.top/gtkzjxjjue.html

[H07] 断言
来源：http://hz.aibaodan.cn/gtyqlvhrcx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.haohaochexian.top/gtqpmspjcw.html

PHP:  assert($x > 0);
来源：http://hz.zhixingplan.top/gtbokczaxb.html

JS:   console.assert(x > 0);
来源：http://hz.sxryk.cn/gttfgjqozc.html

TS:   console.assert(x > 0);
来源：http://hz.daria6918.cn/gtwikemzcx.html

Java: assert x > 0 : "必须为正";
来源：http://hz.wangdashe.top/gtygsofgxf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.chenjidiqi.icu/gtpgzdktaz.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zycfv.cn/gtzunvrppg.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ybcxt.top/gtkpniiond.html

[H08] 获取错误信息与堆栈
来源：http://hz.nwbrower.top/gtakuihqdw.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ydjk.org.cn/gtmpeusmyy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.gzhubu.top/gtfbihlqyp.html

JS:   e.message;  e.stack
来源：http://hz.hywenlv.cn/gtzstonfrv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.chenzaomai.com/gtxkivigyh.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhixingplan.top/gtpdnmxgsw.html

Go:   err.Error()
来源：http://hz.guowangkeji.top/gtfffmhkpp.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhixingplan.top/gtkmyodcen.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jyoumei.cn/gtfvzfofnk.html

[H09] 带错误码的异常
来源：http://hz.yongpay.top/gttyqzdyhg.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yuanzhike.top/gtaivgtfwa.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.yj202588.top/gtxvmoquue.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.havefunace.top/gtuljbfqrd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.mhx1999.top/gtmjnwduxx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.daxiang520.top/gtynfterkk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.smart0.xyz/gtwdxmydfx.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jinyuanbaomall.cn/gtxrzpebwz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.yanxiufei.cn/gtiimetdsm.html

[H10] 资源自动释放
来源：http://hz.sufxvd.cn/gttitcstow.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.xziqi.cn/gtpstmdylh.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xingfuxueyuan.xyz/gttzvijbyk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.fzhhl.top/gtxknskkmf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.cashguo.top/gtqyahkedh.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yanxiufei.cn/gtnwfjicep.html

Go:   defer f.Close()
来源：http://hz.316326.xyz/gtcuelplwv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.meibo888.top/gtebiviuzd.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.guowangkeji.top/gtclogkofy.html

================================================================================
来源：http://hz.hysaishi.cn/gtzyjiugqe.html

I. 正则表达式
来源：http://hz.xziqi.cn/gtpimrxzkp.html

================================================================================
来源：http://hz.hnqzz.top/gtfyyjksjt.html

[I01] 判断是否匹配
来源：http://hz.cucudq.cn/gtamopngci.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.9152youxi.cn/gtrzdxfkfv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xylfe.cn/gtzoybmnvn.html

JS:   /\d+/.test(s)
来源：http://hz.chenlongwang.top/gttuvulghl.html

TS:   /\d+/.test(s)
来源：http://hz.fzhhl.top/gtxtezoyhs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.ydzc1.top/gtgznxuhxv.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.zhaomingkeji.xyz/gtcvkjqqmu.html

Ruby: s.match?(/\d+/)
来源：http://hz.hywenlv.cn/gtablmiamz.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.shuidangran.top/gtgqarclgm.html

[I02] 提取所有匹配
来源：http://hz.xziqi.cn/gtiahgvhwr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jqgfzy.top/gtzzsbvogt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zycfv.cn/gtfxbfdmna.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.cashguo.top/gtdqbbrwlp.html

TS:   s.match(/\d+/g)
来源：http://hz.wangdashe.top/gtqsxdxaff.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.nwbrower.top/gtjsbsckje.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.wangshuangyany.cn/gtjhceawib.html

Ruby: s.scan(/\d+/)
来源：http://hz.xylfe.cn/gtzsgrtnqh.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.mhx1999.top/gtdbtqgwim.html

[I03] 提取捕获分组
来源：http://hz.smart0.xyz/gtrpcvmjxk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.ybcxt.top/gtyiqhtpzt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.shanyushiyangkeji.top/gtlulopvon.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.hfpthk.cn/gtevohnsjf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yj20258.top/gteeuhsndg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yj202588.top/gthlkrozdo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jinqigufen.top/gtjojuolbl.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shanyushiyangtech.top/gtfibpmqgy.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.andypj.xyz/gtapxyxyix.html

[I04] 正则替换
来源：http://hz.quarkkingdee.top/gtwnzkwxok.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.zhengqikj.top/gtiyohpjgm.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.yvedp.cn/gtvoxuvwow.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.hfpthk.cn/gtkhjbaran.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.havefunace.top/gtslmbunbg.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.svipenyu.cn/gtjorsupdc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.redwolf501.top/gtipmroqxj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhengqikj.top/gtbzjoclje.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.fzhhl.top/gtdvmtegcx.html

[I05] 按正则拆分
来源：http://hz.aibaodan.cn/gttqqhlzue.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yj20258888.top/gtpekdvtur.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xinyue.icu/gtcdrppdqf.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jiagoushi.top/gtsoegsqev.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.andypj.xyz/gtageteekn.html

Java: s.split("\\s*,\\s*")
来源：http://hz.guowangkeji.top/gtmcgldonl.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.hywenlv.cn/gtiecrtzdf.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.hywenlv.cn/gtcvnmjtku.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.chenjidiqi.icu/gtvkfsnags.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shanyushiyangtech.top/gtcxpponkx.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.redwolf501.top/gtkfgyqjkg.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cqqwz.cn/gtrfdnortw.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.0kj1m.cn/gttjgjxubn.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sweek.top/gtlwkjmfai.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.quarkkingdee.top/gtycqzmfnw.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.xuetiantiany.cn/gtigioxydn.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hongshengwenyu.top/gttidhrlns.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.birdmap.top/gtbozzqtmc.html

[I07] 忽略大小写与多行模式
来源：http://hz.shangyingyoupin.top/gtsnxoxziu.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yuxming.cn/gtpndwkebe.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.0kj1m.cn/gtbfydixuf.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinyuanbaomall.cn/gtmemjqwbq.html

TS:   /error/gim
来源：http://hz.yj202588.top/gtyfpmadij.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.dashuyun.cn/gttqhgaqdw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hongshengwenyu.top/gttblgjzyp.html

Ruby: s.scan(/error/i)
来源：http://hz.feifeiyinyue.top/gtuyyzdsup.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.quarkkingdee.top/gtgmcdfwkh.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.cashguo.top/gtxzpqtntz.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.gaohongyu789.top/gtlsmqevzl.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yuxming.cn/gtsfkolkjn.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hysaishi.cn/gtllbddtne.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.c1oappe.top/gtkizhbrhu.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cheryme.top/gtlkklbdlr.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.pengpengdd.cyou/gtysftcugm.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.xingfuxueyuan.xyz/gtqgponklc.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zhixingplan.top/gtamwxeumd.html

================================================================================
来源：http://hz.snrcjt.cn/gtwatvqutu.html

J. 日期与时间
来源：http://hz.guowangkeji.top/gtstfdcnka.html

================================================================================
来源：http://hz.zycfv.cn/gtfbmzavcb.html

[J01] 获取当前时间
来源：http://hz.guannengcc.top/gtnfiqizih.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.guannengcc.top/gtlcyudjqb.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.yuanzhike.top/gtpryfdbpq.html

JS:   new Date();  Date.now()
来源：http://hz.yanxiufei.cn/gtbrqnppdl.html

TS:   new Date();  Date.now()
来源：http://hz.jlsjyb.cn/gtcevjqbwh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.nanxinkj.top/gtyebagnoo.html

Go:   time.Now()
来源：http://hz.shanyushiyangkeji.top/gtwwvituuh.html

Ruby: Time.now
来源：http://hz.sysykeji.top/gtaywnnbhw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.guowangkeji.top/gtsrgjeefn.html

[J02] 格式化输出
来源：http://hz.jqgufenzy.top/gteafhbwhv.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.yj20258888.top/gtluhqlvie.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.xingfuxueyuan.xyz/gtbowiomjr.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.yj202588.top/gtcehckgfs.html

TS:   d.toISOString()
来源：http://hz.ywan-chungtsiang.top/gtotcltjvv.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.zhengqikj.top/gtjgobsfhp.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.daxiang520.top/gtibkpejjz.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jiagoushi.top/gthgyyuldv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.yanxiufei.cn/gtxggmricp.html

[J03] 字符串解析为日期
来源：http://hz.cucudq.cn/gteyefojqg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinqigufen.top/gtualuhjjn.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hammf.cn/gtkbcuujfe.html

JS:   new Date("2024-01-02")
来源：http://hz.zhixingplan.top/gtnrvrmgax.html

TS:   new Date("2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtiaxwyakh.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.iojbl.cn/gtfauttleg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.quarkkingdee.top/gtcofhmmgg.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.guannengcc.top/gtcvczrkyr.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinghuilouyu.cn/gtxggfyvju.html

[J04] 时间戳与日期互转
来源：http://hz.chenjidiqi.icu/gtixswblfh.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.wangshuangyany.cn/gtolmfundy.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ydzc1.top/gtsoyhugxq.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.gotoacloud.top/gtbepzebxw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.0kj1m.cn/gtzpxawjrz.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.gotoacloud.top/gtfbfuvejg.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xingfuxueyuan.xyz/gttyquunbu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.316326.xyz/gtfqoikeia.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.zhoulong.xyz/gtzjouetck.html

[J05] 时间加减（加 7 天）
来源：http://hz.hammf.cn/gtqygwcitr.html

Py:   now + timedelta(days=7)
来源：http://hz.cqqwz.cn/gtrnbccewh.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yj20258888.top/gtnnaidbra.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shanyushiyangkeji.top/gtpdnbhemp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhongyouzk.top/gtufwkrxoj.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.yuxming.cn/gtjzydwbil.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.haohaochexian.top/gthehgzcjo.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jqgufenzy.top/gtmcdcirzg.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zycfv.cn/gtbvyuyidu.html

[J06] 计算两时间之差
来源：http://hz.tianlin.xyz/gtteedifjc.html

Py:   (end - start).total_seconds()
来源：http://hz.havefunace.top/gtwficnftr.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhijiandao.cn/gtklmugkaq.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.hongshengwenyu.top/gtgmnvzxor.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.snrcjt.cn/gtiegmtanw.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.shangyingyoupin.top/gtbohvolqz.html

Go:   end.Sub(start).Hours()
来源：http://hz.fengsongda.top/gtqjjnbkss.html

Ruby: end - start                 # 返回秒数
来源：http://hz.xziqi.cn/gtywbfgjuc.html

C#:   (end - start).TotalSeconds
来源：http://hz.jianghu66.top/gtdwgvnmzo.html

[J07] 比较两个日期
来源：http://hz.tianlin.xyz/gtfughrglq.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shangyingyoupin.top/gttyyovmmk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.jlsjyb.cn/gtlywbdamm.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ehwqpu.com/gtrruqcxon.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.cucudq.cn/gtevldctay.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.yangfankeji.com/gtwdpehvpx.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.zycfv.cn/gtitnxjicm.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.wangshuangyany.cn/gtbbgvsvcj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhixingplan.top/gthkdivoal.html

[J08] 提取年月日与星期
来源：http://hz.yj202588.top/gtmouvfkrr.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.shuidangran.top/gtldpwkrug.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.316326.xyz/gtgwacyttz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sxryk.cn/gtvubwpmzb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.nanxuanxn.top/gtlybknhgx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.xylfe.cn/gtzwhzxbaz.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.shanyushiyangtech.top/gtojwygorr.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.sweek.top/gtmwtorebz.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.hfpthk.cn/gtblidwtab.html

[J09] 时区处理
来源：http://hz.hywenlv.cn/gtduewgfco.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.feifeiyinyue.top/gthtdatxhq.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.xylfe.cn/gtlsytbrjg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.yj20258.top/gtqafvifsi.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.hammf.cn/gtlrznmbke.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.fengsongda.top/gtpagaazvu.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.gzhubu.top/gtyjfygdam.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.daria6918.cn/gtfbuzvnja.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhijiandao.cn/gtugmiwqxa.html

[J10] 取今天 / 本月第一天
来源：http://hz.jiagoushi.top/gtgudwadxj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.zhijiandao.cn/gtgmysscrj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.nanxuanxn.top/gtyexygqpi.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.cashguo.top/gtcyaybtjd.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.gaohongyu789.top/gtieodemxi.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.havefunace.top/gtloymjgvu.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.hammf.cn/gtwfmkhiri.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.52xcode.cn/gtoksubuqc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.ydjk.org.cn/gtcbgvtotw.html


<!-- 参考信息 -->