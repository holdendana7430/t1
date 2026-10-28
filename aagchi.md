代发 wailian999

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hongshengwenyu.top/gttuphwyyq.html

JS:   toString() { return this.name; }
来源：http://hz.yangfankeji.com/gtqjdnvizb.html

TS:   toString(): string { return this.name; }
来源：http://hz.zycfv.cn/gtqlieuysc.html

Java: @Override public String toString() { return name; }
来源：http://hz.shanyushiyangtech.top/gtgfnymbhb.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yj20258888.top/gtqnfkwtan.html

Ruby: def to_s; @name; end
来源：http://hz.yj20258.top/gturcfgjbn.html

C#:   public override string ToString() => Name;
来源：http://hz.0kj1m.cn/gtzvuppomd.html

[G13] 判断对象类型
来源：http://hz.jlsjyb.cn/gtbimboonk.html

Py:   isinstance(u, User)
来源：http://hz.gotoacloud.top/gtorvfdatm.html

PHP:  $u instanceof User
来源：http://hz.shanyushiyangtech.top/gtcehviiqn.html

JS:   u instanceof User
来源：http://hz.zhoulong.xyz/gtucwvzuig.html

TS:   u instanceof User
来源：http://hz.haohaochexian.top/gtmaonabho.html

Java: u instanceof User
来源：http://hz.sxryk.cn/gtbofzxxwc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shuidangran.top/gttvbtyddc.html

Ruby: u.is_a?(User)
来源：http://hz.52xcode.cn/gtqbkqgjbw.html

C#:   u is User
来源：http://hz.jqgfzy.top/gtaenmbpsy.html

[G14] 数据类 / record
来源：http://hz.xylfe.cn/gtsyyduvzm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.sxryk.cn/gtwctnlqod.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.yvedp.cn/gtrgzckcga.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.iojbl.cn/gtjleanrsw.html

TS:   type User = { name: string; age: number };
来源：http://hz.haohaochexian.top/gtsttyfcvr.html

Java: record User(String name, int age) {}
来源：http://hz.gzhubu.top/gtmroroybm.html

Go:   type User struct { Name string; Age int }
来源：http://hz.jyoumei.cn/gtfwxfewge.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.zhijiandao.cn/gtxrkgucsd.html

C#:   record User(string Name, int Age);
来源：http://hz.ydzc1.top/gtkulvqduj.html

[G15] 枚举
来源：http://hz.zhijiandao.cn/gtslckpccx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.tianlin.xyz/gtrhglaquf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.xuetiantiany.cn/gtffhxztoh.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.xingfuxueyuan.xyz/gtrczpqxck.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.ywan-chungtsiang.top/gtswmwuxgk.html

Java: enum Color { RED, GREEN }
来源：http://hz.iojbl.cn/gtqyqmdrum.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.dashuyun.cn/gtxkjwcmtb.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zycfv.cn/gtdfthvztv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.svipenyu.cn/gthnfzvugv.html

[G16] 对象转数组 / 字典
来源：http://hz.shzxlz.cn/gtbozfjaiw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.yuxming.cn/gtqpaajnla.html

PHP:  get_object_vars($obj);
来源：http://hz.jinghuilouyu.cn/gtpfofkyim.html

JS:   Object.entries(obj)
来源：http://hz.hywenlv.cn/gtlhpgrxdw.html

TS:   Object.entries(obj)
来源：http://hz.sxryk.cn/gtpaennori.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.gaohongyu789.top/gtfglybcog.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.quarkkingdee.top/gtripuenbm.html

Ruby: obj.instance_variables
来源：http://hz.aizwys.cn/gtltauzfzu.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xinyue.icu/gtixvkepcd.html

================================================================================
来源：http://hz.0kj1m.cn/gtbcgiqbmg.html

H. 异常与错误处理
来源：http://hz.zhiwuduotai.top/gtqbfupcdi.html

================================================================================
来源：http://hz.jinqigfzy.top/gtswwcbisb.html

[H01] try / catch 基础
来源：http://hz.wangshuangyany.cn/gtcxeweomv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.xinyue.icu/gtsnghypql.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.feifeiyinyue.top/gtipqwpjgm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shangyingyoupin.top/gtcfcmkvti.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.0kj1m.cn/gtewhgfinw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.chenzaomai.com/gtqpdrabgw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.52xcode.cn/gtiyexobmd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yueranfly.top/gtxccptnye.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.sufxvd.cn/gtarnedcex.html

[H02] finally / ensure 收尾
来源：http://hz.zhaomingkeji.xyz/gthzuuencw.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jinqigfzy.top/gthummmxlx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zhongyouzk.top/gtkcrrzhgw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gtjlcwwslf.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.dashuyun.cn/gtinipkmar.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.fengsongda.top/gtrchisetv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.andypj.xyz/gtgzexlyxh.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.wangdashe.top/gtdwkymjqf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.zhongyouzk.top/gtmjcjvshv.html

[H03] 主动抛出异常
来源：http://hz.nwbrower.top/gtjloqgrrq.html

Py:   raise ValueError("错误信息")
来源：http://hz.vqdsnc.cn/gtmuuubndt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.ehwqpu.com/gtxtdbcbtj.html

JS:   throw new Error("错误信息");
来源：http://hz.zycfv.cn/gtblbmtmbv.html

TS:   throw new Error("错误信息");
来源：http://hz.sysykeji.top/gtisfjgejs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ehwqpu.com/gtzzxznzjm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jinghuilouyu.cn/gtelleqxmi.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jlsjyb.cn/gtyloozsyu.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.aizwys.cn/gtmoxwiznj.html

[H04] 自定义异常类型
来源：http://hz.wangdashe.top/gtsvjsgjqj.html

Py:   class MyError(Exception): pass
来源：http://hz.zhengqikj.top/gtuspldnfe.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.zdqjudy.top/gtxzclnxhr.html

JS:   class MyError extends Error {}
来源：http://hz.jinyuanbaomall.cn/gtdafmdyoh.html

TS:   class MyError extends Error {}
来源：http://hz.xziqi.cn/gtllecbatv.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhengqikj.top/gtktctcfsx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.guowangkeji.top/gthqfwttwr.html

Ruby: class MyError < StandardError; end
来源：http://hz.xingfuxueyuan.xyz/gtxguuxhrb.html

C#:   class MyException : Exception {}
来源：http://hz.ydzc1.top/gtrbwmficn.html

[H05] 捕获特定类型
来源：http://hz.xylfe.cn/gtinlzbdcv.html

Py:   except ValueError as e:
来源：http://hz.zycfv.cn/gtfujwzoly.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.nanxuanxn.top/gtimuvhcah.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.gaohongyu789.top/gtuaoawogu.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jinqigfzy.top/gtjakhyksw.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.guowangkeji.top/gtrjilhvvh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.zhongyouzk.top/gtvfgxmqqp.html

Ruby: rescue ArgumentError => e
来源：http://hz.zdqjudy.top/gtrxfpshsy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yj20258888.top/gtbjulgqkc.html

[H06] 可选值 / 空值安全访问
来源：http://hz.jianghu66.top/gtfnpcbpbb.html

Py:   value = d.get("k") or default
来源：http://hz.jiagoushi.top/gtgebxlekk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yueranfly.top/gtzkkhsbgz.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.havefunace.top/gtlhaztyhi.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.0kj1m.cn/gtxpsarbrx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yuanzhike.top/gtiqmvjnnn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.316326.xyz/gtyhjqnhum.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jinqigufen.top/gtvmagzebw.html

C#:   obj?.A?.B ?? default
来源：http://hz.hnqzz.top/gttsdofxdp.html

[H07] 断言
来源：http://hz.yueranfly.top/gtpgylgnfv.html

Py:   assert x > 0, "必须为正"
来源：http://hz.nwbrower.top/gtwyjlmtns.html

PHP:  assert($x > 0);
来源：http://hz.iojbl.cn/gtvejtbrmk.html

JS:   console.assert(x > 0);
来源：http://hz.ivvv.top/gttrbmwxmo.html

TS:   console.assert(x > 0);
来源：http://hz.xinyue.icu/gtncfzfxvv.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhongyouzk.top/gtvqbbpome.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.vqdsnc.cn/gtokxqviuc.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhijiandao.cn/gthhqztlpu.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ybcxt.top/gtxntrxgof.html

[H08] 获取错误信息与堆栈
来源：http://hz.svipenyu.cn/gtxhggteyr.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cheryme.top/gtwyhehvqz.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.cqqwz.cn/gtxgwioeig.html

JS:   e.message;  e.stack
来源：http://hz.ehwqpu.com/gticeixeut.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shuidangran.top/gtbpixydnj.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.aibaodan.cn/gtpxgyppgy.html

Go:   err.Error()
来源：http://hz.sxryk.cn/gtvqhuwhyl.html

Ruby: e.message;  e.backtrace
来源：http://hz.ydjk.org.cn/gtohqfwgif.html

C#:   e.Message;  e.StackTrace
来源：http://hz.jiagoushi.top/gtsovqohwe.html

[H09] 带错误码的异常
来源：http://hz.cheryme.top/gtbjimxzzv.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.shuidangran.top/gtaldemcad.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.cqqwz.cn/gtuzowmzjk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.sufxvd.cn/gtozfiknxy.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yj202588.top/gtsdyouuqn.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hysaishi.cn/gtgmtpdjkj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yueranfly.top/gtljilapeu.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.jlsjyb.cn/gtgweugkfl.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.hnqzz.top/gtcnegokym.html

[H10] 资源自动释放
来源：http://hz.jinqigufen.top/gtmggnazpa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jqgufenzy.top/gtbhtrehhe.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xinyue.icu/gtfqjizlmc.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.daria6918.cn/gtasmqaqra.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.havefunace.top/gtdpoeiibe.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.svipenyu.cn/gtxgmrkxfq.html

Go:   defer f.Close()
来源：http://hz.hysaishi.cn/gtpbxjurne.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shanyushiyangtech.top/gtnfzwfyfh.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.birdmap.top/gtxtekekxk.html

================================================================================
来源：http://hz.gzhubu.top/gtbdnzvylj.html

I. 正则表达式
来源：http://hz.9152youxi.cn/gtwkuciizl.html

================================================================================
来源：http://hz.gogol.net.cn/gtnsvpkjek.html

[I01] 判断是否匹配
来源：http://hz.sufxvd.cn/gterphsaaa.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.iojbl.cn/gtxqqfwdci.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.iojbl.cn/gtcaisitjq.html

JS:   /\d+/.test(s)
来源：http://hz.xuetiantiany.cn/gtbdusnifj.html

TS:   /\d+/.test(s)
来源：http://hz.nanxinkj.top/gtibpklkfl.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.meibo888.top/gtbqslacqb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.xinyue.icu/gtljmgwvus.html

Ruby: s.match?(/\d+/)
来源：http://hz.yonumen.top/gtgjlqfpnn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.xuetiantiany.cn/gtizwyvdzq.html

[I02] 提取所有匹配
来源：http://hz.yonumen.top/gtpvuaiffk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yj20258888.top/gtgselleeg.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhiwuduotai.top/gtmpkwmjyw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.meibo888.top/gtpgbtwdtj.html

TS:   s.match(/\d+/g)
来源：http://hz.yj20258888.top/gthziosqha.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.0kj1m.cn/gtqlldzsrq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shanyushiyangtech.top/gtxziooxjw.html

Ruby: s.scan(/\d+/)
来源：http://hz.daria6918.cn/gtugwzysen.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.daria6918.cn/gtchkdnagc.html

[I03] 提取捕获分组
来源：http://hz.feifeiyinyue.top/gtolnhyrzu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.mhx1999.top/gtxawtkvvh.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.xuanzx.com/gtzghoagwd.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.zdqjudy.top/gtyfcgbeen.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yuanzhike.top/gtwhkdebpz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.feifeiyinyue.top/gtckhtguye.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.wangdashe.top/gtsvohmwrj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.316326.xyz/gtosiyobbw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.nanxinkj.top/gtlqhkxgtg.html

[I04] 正则替换
来源：http://hz.sysykeji.top/gtjsictgfe.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.quarkkingdee.top/gtenindjqf.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.dianchejie.cn/gtfmxufhxk.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinqigufen.top/gtlmazqawv.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.nwbrower.top/gtrinsdero.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.sxryk.cn/gtwpubpben.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.yuanzhike.top/gtmwbervnt.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yj202588.top/gtqdcktxlv.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.wangdashe.top/gttxvipxdh.html

[I05] 按正则拆分
来源：http://hz.gzhubu.top/gtxbsdddar.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.yuanzhike.top/gtpgbepeao.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.kuanghao11.cn/gtjexnokwi.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.pengpengdd.cyou/gtvmwlwbvc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.jinqigfzy.top/gtenqjkgfs.html

Java: s.split("\\s*,\\s*")
来源：http://hz.zhijiandao.cn/gtxfkatnyb.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.cqqwz.cn/gtmcmlxtes.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.ydzc1.top/gtzzdmtmpo.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.yueranfly.top/gtsqpnldhy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.yvedp.cn/gteihiospl.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.hnxiangtu.top/gtgussnwbb.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.xylfe.cn/gtjnijyvvi.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.52xcode.cn/gtirqbyqkx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinghuilouyu.cn/gtlropaklh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tanke756.top/gtruftrhma.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.ybcxt.top/gtlqhqnhtf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.hfpthk.cn/gtaapbtyks.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.smart0.xyz/gtrhzidoiu.html

[I07] 忽略大小写与多行模式
来源：http://hz.xingfuxueyuan.xyz/gtmviqjsub.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.mhx1999.top/gtabwaujqu.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.zdqjudy.top/gtxrfofnzn.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.shanyushiyangkeji.top/gticcrynoj.html

TS:   /error/gim
来源：http://hz.feifeiyinyue.top/gttahbsnjc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.yuxming.cn/gtjpmnvgct.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.xuanzx.com/gtihbnzhij.html

Ruby: s.scan(/error/i)
来源：http://hz.chenzaomai.com/gtvqjbnknp.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hywenlv.cn/gtcfgnooql.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.yj20258888.top/gtqhmchtwp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.nanxuanxn.top/gtzpdxmcra.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.c1oappe.top/gtmggdqige.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yuanzhike.top/gtvkdoapez.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cheryme.top/gtcawkpzla.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhixingplan.top/gtfzfmnnqj.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.snrcjt.cn/gtvcuxohhh.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.mhx1999.top/gtdqqddxag.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xingfuxueyuan.xyz/gtxzspnoqx.html

================================================================================
来源：http://hz.sysykeji.top/gtnqwtkmnj.html

J. 日期与时间
来源：http://hz.shuidangran.top/gtgiyierqw.html

================================================================================
来源：http://hz.jiagoushi.top/gttiqrqfet.html

[J01] 获取当前时间
来源：http://hz.sysykeji.top/gtjhgkpjhg.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.shuidangran.top/gtatgtikcr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hnxiangtu.top/gtqjnbofxp.html

JS:   new Date();  Date.now()
来源：http://hz.chenjidiqi.icu/gtxmupcdaf.html

TS:   new Date();  Date.now()
来源：http://hz.bjfxy.top/gthvtswpga.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jinyuanbaomall.cn/gtcohzlxrq.html

Go:   time.Now()
来源：http://hz.bjfxy.top/gtnlcnbrms.html

Ruby: Time.now
来源：http://hz.yongpay.top/gtvvkwrwyg.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.0kj1m.cn/gtrbpovkpx.html

[J02] 格式化输出
来源：http://hz.shzxlz.cn/gtulteuxeq.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinqigufen.top/gtxbnpdgwg.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.redwolf501.top/gtdqvbvixb.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.c1oappe.top/gtykzgjcoc.html

TS:   d.toISOString()
来源：http://hz.nanxuanxn.top/gtalrjvvds.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.vqdsnc.cn/gtaxxgmbyy.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.52xcode.cn/gtjiivilrw.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgufenzy.top/gtziomrigp.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.havefunace.top/gtwbnshmgu.html

[J03] 字符串解析为日期
来源：http://hz.yanxiufei.cn/gthlqxhoeh.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.redwolf501.top/gthskdpmmh.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cashguo.top/gtrazgitci.html

JS:   new Date("2024-01-02")
来源：http://hz.zhoulong.xyz/gttvgbvpbv.html

TS:   new Date("2024-01-02")
来源：http://hz.yj202588.top/gtsfwadopw.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.9152youxi.cn/gtgwytgmhs.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.hammf.cn/gtmnoxrvvo.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.316326.xyz/gttpsjtajb.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.c1oappe.top/gttcvyulum.html

[J04] 时间戳与日期互转
来源：http://hz.gzhubu.top/gtmaujzhys.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.smart0.xyz/gtyqcrfbyp.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jinqigfzy.top/gthsznopph.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yvedp.cn/gtzfzclihf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ehwqpu.com/gtdzxatomh.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shuidangran.top/gtcwzyyjjc.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xuanzx.com/gtltuknmos.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shzxlz.cn/gtiabycucl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinqigfzy.top/gtpaujibqn.html

[J05] 时间加减（加 7 天）
来源：http://hz.jinghuilouyu.cn/gtxitwxzbi.html

Py:   now + timedelta(days=7)
来源：http://hz.sysykeji.top/gtjqdcyxuv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.jiagoushi.top/gtxrbidpqa.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.iojbl.cn/gtkanjofse.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.shangyingyoupin.top/gtkeoijrwr.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhijiandao.cn/gtkaagqlmx.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.aizwys.cn/gtngdhksna.html

Ruby: Time.now + 7 * 86400
来源：http://hz.ppjwa.cn/gttmpjxnkj.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.ppjwa.cn/gtvikeluao.html

[J06] 计算两时间之差
来源：http://hz.xuanzx.com/gtxjckdqah.html

Py:   (end - start).total_seconds()
来源：http://hz.yangfankeji.com/gtcamalyaq.html

PHP:  $end->diff($start)->days;
来源：http://hz.daria6918.cn/gtqhojfkso.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.meibo888.top/gtvhyfnahs.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hnxiangtu.top/gtxisabdkn.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xinyue.icu/gttluthrxz.html

Go:   end.Sub(start).Hours()
来源：http://hz.zycfv.cn/gtqlekvwnc.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yuxming.cn/gtkbrmjmtt.html

C#:   (end - start).TotalSeconds
来源：http://hz.vqdsnc.cn/gtvldwnyto.html

[J07] 比较两个日期
来源：http://hz.andypj.xyz/gteerwiuyy.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.cashguo.top/gtcicyzixn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.wangshuangyany.cn/gtryqdibki.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.0kj1m.cn/gtvwjhcgsa.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.0kj1m.cn/gtvchpocta.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zhiwuduotai.top/gtpimfeyjs.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.daxiang520.top/gtwwxmdnus.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.quarkkingdee.top/gtqfsizcpw.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.52xcode.cn/gthwdaxvxx.html

[J08] 提取年月日与星期
来源：http://hz.yuanzhike.top/gtferkvvyi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yanxiufei.cn/gthaizijkt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.xinyue.icu/gthpjftgmf.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.ivvv.top/gtstrhfsxy.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.svipenyu.cn/gtzuidyctd.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ppjwa.cn/gtwjghfdhm.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.cheryme.top/gtemdchwmw.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.9152youxi.cn/gthpuslphx.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.yongpay.top/gtavipdtww.html

[J09] 时区处理
来源：http://hz.xingfuxueyuan.xyz/gtcnmtmhbq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hnqzz.top/gtotzejtas.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.mhx1999.top/gtekxvniit.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sysykeji.top/gtpgztjofo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.meibo888.top/gtlqzttprx.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.yueranfly.top/gtpyfrqdyc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.jinqigfzy.top/gtoorljiee.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.shanyushiyangtech.top/gtgbimttfx.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.zhoulong.xyz/gtnmughvrs.html

[J10] 取今天 / 本月第一天
来源：http://hz.ybcxt.top/gtlppawmtf.html

Py:   date.today();  date.today().replace(day=1)
来源：http://hz.smart0.xyz/gtvmkxqfed.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hz.hammf.cn/gtjfyrlrtf.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hz.zhaomingkeji.xyz/gtymfjjhhw.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://hz.sysykeji.top/gtoujysiox.html


<!-- 参考信息 -->