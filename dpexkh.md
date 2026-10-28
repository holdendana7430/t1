代发 wailian999

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xinyue.icu/gtipjdlkhu.html

Ruby: def to_s; @name; end
来源：http://hz.ybcxt.top/gtigukwydd.html

C#:   public override string ToString() => Name;
来源：http://hz.52xcode.cn/gtinfplnvl.html

[G13] 判断对象类型
来源：http://hz.wangdashe.top/gtjqxumaos.html

Py:   isinstance(u, User)
来源：http://hz.wangshuangyany.cn/gthsktgydf.html

PHP:  $u instanceof User
来源：http://hz.zhongyouzk.top/gtbdcykhew.html

JS:   u instanceof User
来源：http://hz.zycfv.cn/gtdjgbrlhq.html

TS:   u instanceof User
来源：http://hz.sufxvd.cn/gtkobzrifk.html

Java: u instanceof User
来源：http://hz.gogol.net.cn/gtokbjrbfj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ppjwa.cn/gtjbhmgnxw.html

Ruby: u.is_a?(User)
来源：http://hz.jqgufenzy.top/gthfthnahu.html

C#:   u is User
来源：http://hz.jianghu66.top/gtymnobjra.html

[G14] 数据类 / record
来源：http://hz.zycfv.cn/gtyuvflqdc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhiwuduotai.top/gtjhnowqru.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yj202588.top/gtlzmrtrar.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cdnleiting.top/gtalvdxlph.html

TS:   type User = { name: string; age: number };
来源：http://hz.jlsjyb.cn/gtxahagzii.html

Java: record User(String name, int age) {}
来源：http://hz.aibaodan.cn/gtayfmisjy.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shanyushiyangkeji.top/gtwgsialrr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.dashuyun.cn/gtzkvrskxe.html

C#:   record User(string Name, int Age);
来源：http://hz.jqgfzy.top/gttixovoxl.html

[G15] 枚举
来源：http://hz.daxiang520.top/gtjyzuqimr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.xuetiantiany.cn/gtjabwdesv.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.zhixingplan.top/gtcvfvodwz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.yuxming.cn/gthbjarbys.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.hfpthk.cn/gtushbuyhy.html

Java: enum Color { RED, GREEN }
来源：http://hz.svipenyu.cn/gtwxmkcony.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sweek.top/gtbwbemndh.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhengqikj.top/gtcbclnxql.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhiwuduotai.top/gtohvhwazk.html

[G16] 对象转数组 / 字典
来源：http://hz.chenlongwang.top/gtaplfttpg.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yangfankeji.com/gtjcqajbec.html

PHP:  get_object_vars($obj);
来源：http://hz.ywan-chungtsiang.top/gtlwytofvf.html

JS:   Object.entries(obj)
来源：http://hz.dashuyun.cn/gthhoxxuwj.html

TS:   Object.entries(obj)
来源：http://hz.cheryme.top/gtpqdctnqz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhoulong.xyz/gtmgbihyis.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.yj202588.top/gtdvbxwjzs.html

Ruby: obj.instance_variables
来源：http://hz.fzhhl.top/gtdcajwilr.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.gzhubu.top/gtihnoaxwc.html

================================================================================
来源：http://hz.chenzaomai.com/gtnoterujr.html

H. 异常与错误处理
来源：http://hz.xinyue.icu/gtjqjvtqjw.html

================================================================================
来源：http://hz.zhijiandao.cn/gtxomvkykg.html

[H01] try / catch 基础
来源：http://hz.sufxvd.cn/gtsmevlxxn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.sweek.top/gtxnnnjtqh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.smart0.xyz/gtszzbxoen.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.yangfankeji.com/gtnrjdkzdu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ppjwa.cn/gtjadpzhti.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.zdqjudy.top/gtdauvqdqh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.svipenyu.cn/gtrgcsswlf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.cheryme.top/gtlqmmzoav.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.quarkkingdee.top/gtmjuepmej.html

[H02] finally / ensure 收尾
来源：http://hz.hysaishi.cn/gtmmaqacyl.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.shuidangran.top/gtwzhhorsk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shuidangran.top/gtbvfjvvld.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.sufxvd.cn/gtghsovrft.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gttttfgubp.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.cdnleiting.top/gtylbtawrn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.shuidangran.top/gtokgzageu.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ppjwa.cn/gtsykcnngp.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.nwbrower.top/gtqqyfmsjh.html

[H03] 主动抛出异常
来源：http://hz.guowangkeji.top/gtmijvbsxd.html

Py:   raise ValueError("错误信息")
来源：http://hz.hnxiangtu.top/gtycofeoih.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xylfe.cn/gtnaugwrai.html

JS:   throw new Error("错误信息");
来源：http://hz.zhiwuduotai.top/gtnedyxtxb.html

TS:   throw new Error("错误信息");
来源：http://hz.jiagoushi.top/gtjfjxcboa.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yj20258888.top/gtggdttbpl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.aibaodan.cn/gtvrhgfxvf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhijiandao.cn/gtajjnllhz.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.zhaomingkeji.xyz/gtbqooephx.html

[H04] 自定义异常类型
来源：http://hz.aizwys.cn/gtosnvyofn.html

Py:   class MyError(Exception): pass
来源：http://hz.nwbrower.top/gtytdpmajx.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.shanyushiyangkeji.top/gtoxfwqbdw.html

JS:   class MyError extends Error {}
来源：http://hz.xinyue.icu/gtgkldivky.html

TS:   class MyError extends Error {}
来源：http://hz.yj20258.top/gtqgprbvqn.html

Java: class MyException extends RuntimeException {}
来源：http://hz.haohaochexian.top/gtibvemqxz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.hnxiangtu.top/gtykpccsfz.html

Ruby: class MyError < StandardError; end
来源：http://hz.wangshuangyany.cn/gtdctsnnle.html

C#:   class MyException : Exception {}
来源：http://hz.zhoulong.xyz/gtllbxofsw.html

[H05] 捕获特定类型
来源：http://hz.jinghuilouyu.cn/gtvkxmmadn.html

Py:   except ValueError as e:
来源：http://hz.0kj1m.cn/gtbvchxajf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.snrcjt.cn/gtxgzohgnq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.yvedp.cn/gtkccvlynw.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hysaishi.cn/gthjakwlus.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.gaohongyu789.top/gttesxiazn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.tanke756.top/gtxwwcdefn.html

Ruby: rescue ArgumentError => e
来源：http://hz.smart0.xyz/gtbutslwce.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.nwbrower.top/gtwjqgzatf.html

[H06] 可选值 / 空值安全访问
来源：http://hz.iojbl.cn/gtjvqgparc.html

Py:   value = d.get("k") or default
来源：http://hz.xinyue.icu/gtensadmqu.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.guannengcc.top/gtspylqbhr.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgfzy.top/gtkeddsrhq.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jinyuanbaomall.cn/gtssomjfkn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hnxiangtu.top/gtprzkefxb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sxryk.cn/gtqsvwxjve.html

Ruby: d&.dig(:a, :b)
来源：http://hz.ivvv.top/gtvjtcjqya.html

C#:   obj?.A?.B ?? default
来源：http://hz.tianlin.xyz/gtonayqxtz.html

[H07] 断言
来源：http://hz.chenjidiqi.icu/gtpuuyekzx.html

Py:   assert x > 0, "必须为正"
来源：http://hz.aizwys.cn/gtolvuubbl.html

PHP:  assert($x > 0);
来源：http://hz.chenjidiqi.icu/gtzerqtyjj.html

JS:   console.assert(x > 0);
来源：http://hz.zhoulong.xyz/gtmtkbhxzb.html

TS:   console.assert(x > 0);
来源：http://hz.ydjk.org.cn/gtkbriuzmc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.snrcjt.cn/gtweieapmv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.fengsongda.top/gttnmzwccs.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.hnqzz.top/gtgrkhhhcs.html

C#:   Debug.Assert(x > 0);
来源：http://hz.cashguo.top/gtovadcier.html

[H08] 获取错误信息与堆栈
来源：http://hz.ybcxt.top/gtteapvfte.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.zhengqikj.top/gteueqdouf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.52xcode.cn/gtvshrixki.html

JS:   e.message;  e.stack
来源：http://hz.svipenyu.cn/gtjtritzua.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.xylfe.cn/gtubtckzxq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhongyouzk.top/gtaqeeecxk.html

Go:   err.Error()
来源：http://hz.chenjidiqi.icu/gtgipatqnz.html

Ruby: e.message;  e.backtrace
来源：http://hz.yueranfly.top/gtdkjfqjez.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xylfe.cn/gtdrraqusi.html

[H09] 带错误码的异常
来源：http://hz.chenlongwang.top/gtkedfkjps.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.iojbl.cn/gtfvvnqjzr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.aibaodan.cn/gtwstrtrwb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yuanzhike.top/gthnjafxrv.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.vqdsnc.cn/gtuosufadh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.cqqwz.cn/gtkfdbirzy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ybcxt.top/gtgjqneuvc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jinqigufen.top/gtmwzltvgq.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.shuidangran.top/gtoomtytwy.html

[H10] 资源自动释放
来源：http://hz.daxiang520.top/gtpoabbehn.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ywan-chungtsiang.top/gttqradxsd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shanyushiyangtech.top/gtiipduulf.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.daxiang520.top/gtmcqylydd.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.0kj1m.cn/gtxqdbwtsr.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.shuidangran.top/gttnruqcxm.html

Go:   defer f.Close()
来源：http://hz.xuetiantiany.cn/gtomjuopdh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jiagoushi.top/gthecemchl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.xinyue.icu/gtuzkqfdxq.html

================================================================================
来源：http://hz.jqgufenzy.top/gthihysryy.html

I. 正则表达式
来源：http://hz.xinyue.icu/gtyyjlpbxb.html

================================================================================
来源：http://hz.sweek.top/gtobdjwaar.html

[I01] 判断是否匹配
来源：http://hz.bjfxy.top/gtnsvoitcg.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.zhijiandao.cn/gtxsvnsmwy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yj202588.top/gtifwojjtj.html

JS:   /\d+/.test(s)
来源：http://hz.shzxlz.cn/gtdekktipa.html

TS:   /\d+/.test(s)
来源：http://hz.c1oappe.top/gtxudmrezv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.zhaomingkeji.xyz/gtygnmagxc.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.guannengcc.top/gtplrernoi.html

Ruby: s.match?(/\d+/)
来源：http://hz.xylfe.cn/gtpfaflfep.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.aibaodan.cn/gthclrdmqu.html

[I02] 提取所有匹配
来源：http://hz.nanxinkj.top/gthhmlltwj.html

Py:   re.findall(r"\d+", s)
来源：http://hz.jinqigfzy.top/gtyayrdecf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zycfv.cn/gttbhroqit.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.redwolf501.top/gtcubpzedj.html

TS:   s.match(/\d+/g)
来源：http://hz.xylfe.cn/gtgsgnqqhd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jinqigfzy.top/gtxebtzjvh.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.ehwqpu.com/gtxhikfzqp.html

Ruby: s.scan(/\d+/)
来源：http://hz.chenzaomai.com/gtcyxttoox.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.fzhhl.top/gtekheyxxk.html

[I03] 提取捕获分组
来源：http://hz.ivvv.top/gtmacrxzvm.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.haohaochexian.top/gtckmylzql.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.haohaochexian.top/gtfbxswkri.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gzhubu.top/gtpzuclrkl.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.snrcjt.cn/gttgshvayj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.yonumen.top/gtbuorirvl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.gaohongyu789.top/gtcrkuiirx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.xylfe.cn/gtauvurwxq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.tanke756.top/gtcpgeedmr.html

[I04] 正则替换
来源：http://hz.vqdsnc.cn/gtbxxqggcc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.ydjk.org.cn/gtbokfnnpd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.pycfn.com/gtcglvpddm.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.shzxlz.cn/gtfawctvqs.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.andypj.xyz/gtffqczfki.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.andypj.xyz/gtijltegtk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ybcxt.top/gtmasjceuh.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shanyushiyangtech.top/gtfbmeykwj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.nwbrower.top/gtsbxoqtsr.html

[I05] 按正则拆分
来源：http://hz.yangfankeji.com/gtitnlergb.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.sysykeji.top/gtkindpvqm.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.shanyushiyangtech.top/gtjmyaltez.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zycfv.cn/gtpwedggrp.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yangfankeji.com/gthacmkxco.html

Java: s.split("\\s*,\\s*")
来源：http://hz.xuetiantiany.cn/gtgrhuxnbr.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.xuetiantiany.cn/gtdcfzlruh.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.birdmap.top/gtcxnowcrk.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.xuetiantiany.cn/gtbkhriuhi.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cdnleiting.top/gttvzedxpt.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.shuidangran.top/gtywqqhnix.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cucudq.cn/gtugrkbzqc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.guannengcc.top/gtdhbfvdgu.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hnxiangtu.top/gtswbefunx.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gtqpbqycqh.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.fzhhl.top/gtzwrowfzs.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.shanyushiyangtech.top/gttgbxybok.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.havefunace.top/gtoofkbzse.html

[I07] 忽略大小写与多行模式
来源：http://hz.yangfankeji.com/gtdvoazoka.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yj20258888.top/gtnwvnqiyp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.chenjidiqi.icu/gtehanbond.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinqigfzy.top/gtphxrvpnd.html

TS:   /error/gim
来源：http://hz.shuidangran.top/gtcaydfved.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.gzhubu.top/gtjszruhql.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.meibo888.top/gtvuuoczyb.html

Ruby: s.scan(/error/i)
来源：http://hz.hnqzz.top/gtjfavzywr.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hammf.cn/gtprxcmkpf.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yonumen.top/gtlsiqroqr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.shuidangran.top/gtignefygo.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.aizwys.cn/gtrotsepjx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.chenlongwang.top/gtuklgoacq.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cucudq.cn/gtkdhpsaya.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.nwbrower.top/gtomoruiuv.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.dianchejie.cn/gtgqkedzaj.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.cheryme.top/gtvxxnoluo.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.ppjwa.cn/gtlqzjcojv.html

================================================================================
来源：http://hz.xylfe.cn/gtugnmlycg.html

J. 日期与时间
来源：http://hz.jiagoushi.top/gtsmvivzpt.html

================================================================================
来源：http://hz.yuanzhike.top/gtqpsfubkt.html

[J01] 获取当前时间
来源：http://hz.sysykeji.top/gttetgudmu.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.hnqzz.top/gtupziohgz.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.cheryme.top/gtjbfqzecg.html

JS:   new Date();  Date.now()
来源：http://hz.shanyushiyangtech.top/gtgehcqwjp.html

TS:   new Date();  Date.now()
来源：http://hz.daria6918.cn/gttejiikhm.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.316326.xyz/gtcubsuucn.html

Go:   time.Now()
来源：http://hz.gotoacloud.top/gtyppjxays.html

Ruby: Time.now
来源：http://hz.svipenyu.cn/gtufhtcyky.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.nwbrower.top/gtwozkfulj.html

[J02] 格式化输出
来源：http://hz.birdmap.top/gtbsvtpcjq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.tian-w.cn/gtmdpyxqzn.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.birdmap.top/gtndebnfju.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.316326.xyz/gtfycuxttc.html

TS:   d.toISOString()
来源：http://hz.jianghu66.top/gtqkkdggjh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.mhx1999.top/gtxioawbmr.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.sxryk.cn/gtwdypuhsw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgfzy.top/gthenucjia.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhoulong.xyz/gtprnfdqrl.html

[J03] 字符串解析为日期
来源：http://hz.zhijiandao.cn/gtuetrobbh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shanyushiyangkeji.top/gtnxcvdjbx.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.bjfxy.top/gtkvknftht.html

JS:   new Date("2024-01-02")
来源：http://hz.sweek.top/gttdthdbpp.html

TS:   new Date("2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtethjntgc.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.xziqi.cn/gteydvpzhj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xylfe.cn/gtksdrdcvx.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jqgufenzy.top/gtqrjtfpkf.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.cucudq.cn/gtaawxmgey.html

[J04] 时间戳与日期互转
来源：http://hz.yvedp.cn/gtcajrvpih.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hywenlv.cn/gtqdghbkuo.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.shanyushiyangtech.top/gtjcsmzval.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.cashguo.top/gtgreqmhgr.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.shuidangran.top/gtzqtfbulc.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.tian-w.cn/gttotbpuqe.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.yvedp.cn/gtmqtvuhvt.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.zdqjudy.top/gtunxexknh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.gaohongyu789.top/gtqfzzymxf.html

[J05] 时间加减（加 7 天）
来源：http://hz.52xcode.cn/gttgsnzqgt.html

Py:   now + timedelta(days=7)
来源：http://hz.iojbl.cn/gtjsryjslf.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.zhoulong.xyz/gthrrvkwew.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jiagoushi.top/gtjgkcimmw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cqqwz.cn/gtlbvsuwxw.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jianghu66.top/gtvfjjtsgu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.nwbrower.top/gthdpcnkzf.html

Ruby: Time.now + 7 * 86400
来源：http://hz.shuidangran.top/gtbbjvgczz.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.nanxuanxn.top/gteqjiyfxj.html

[J06] 计算两时间之差
来源：http://hz.hongshengwenyu.top/gthkbqjcvr.html

Py:   (end - start).total_seconds()
来源：http://hz.zdqjudy.top/gtojwvcwza.html

PHP:  $end->diff($start)->days;
来源：http://hz.cheryme.top/gtlwjgiulb.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.zhixingplan.top/gtzomebntd.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.cdnleiting.top/gtgptqbgxt.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xinyue.icu/gtxobidpwp.html

Go:   end.Sub(start).Hours()
来源：http://hz.daria6918.cn/gtgxffhske.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hongshengwenyu.top/gtehjvkqck.html

C#:   (end - start).TotalSeconds
来源：http://hz.xuetiantiany.cn/gtanclggnw.html

[J07] 比较两个日期
来源：http://hz.chenlongwang.top/gtsqgjncos.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.meibo888.top/gtezziuemh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.gzhubu.top/gtomvrygnl.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xinyue.icu/gtjcmlcgdv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.jyoumei.cn/gtdslngzst.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.cheryme.top/gtauhmbsfi.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.dianchejie.cn/gtdfitwhsv.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.cqqwz.cn/gtxfbmbsyb.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ppjwa.cn/gtpcjvjmrn.html

[J08] 提取年月日与星期
来源：http://hz.zdqjudy.top/gtbmhafwtn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zhaomingkeji.xyz/gtuilqoqqb.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.sxryk.cn/gtceenplyk.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.svipenyu.cn/gtxsqjerqs.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhixingplan.top/gtqjhdlepp.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.dianchejie.cn/gtkeaccfay.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hysaishi.cn/gtynkqzmtg.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.tanke756.top/gtiqkockqa.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.tianlin.xyz/gtjvgoelxu.html

[J09] 时区处理
来源：http://hz.zhixingplan.top/gtgszscfqq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.sufxvd.cn/gttmusvjxf.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.jqgfzy.top/gtgpipqjbs.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xuetiantiany.cn/gtjhdgfpqq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.ybcxt.top/gtwcgmqvzy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.smart0.xyz/gtppwoseez.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.yj202588.top/gtlngbdphq.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.dianchejie.cn/gtgvabuojl.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ybcxt.top/gtcqneyqfj.html

[J10] 取今天 / 本月第一天
来源：http://hz.yueranfly.top/gtdmuukmko.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.cheryme.top/gtgdgqlvpl.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.tanke756.top/gtrerwhonc.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.aibaodan.cn/gtqnliesjm.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.ydjk.org.cn/gtnaziunki.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hz.hnxiangtu.top/gtbanhizxp.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://hz.gotoacloud.top/gtnhscizyz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://hz.jqgufenzy.top/gtcnohzqrq.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://hz.shanyushiyangtech.top/gtmfeiuqse.html


<!-- 参考信息 -->