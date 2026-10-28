代发 wailian999

C#:   public / protected / private / internal
来源：http://hz.yueranfly.top/gtzarhzftk.html

[G11] getter / setter
来源：http://hz.316326.xyz/gtvbhwweyx.html

Py:   @property 与 @x.setter
来源：http://hz.shanyushiyangtech.top/gtyfnpmlal.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gtbxwedmem.html

JS:   get name() { return this._name; }
来源：http://hz.jinyuanbaomall.cn/gtmwfltmyp.html

TS:   get name(): string { return this._name; }
来源：http://hz.havefunace.top/gteuazowct.html

Java: public String getName() { return name; }
来源：http://hz.nanxuanxn.top/gtaoucjrbx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.tian-w.cn/gtsfyijqzw.html

Ruby: attr_accessor :name
来源：http://hz.yanxiufei.cn/gtalbdkbzj.html

C#:   public string Name { get; set; }
来源：http://hz.havefunace.top/gtftfsxoxc.html

[G12] 对象转字符串
来源：http://hz.guowangkeji.top/gtyqihjkyl.html

Py:   def __str__(self): return self.name
来源：http://hz.sysykeji.top/gtywmzfzig.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xingfuxueyuan.xyz/gtrqgxioob.html

JS:   toString() { return this.name; }
来源：http://hz.tian-w.cn/gtaqkhxmtu.html

TS:   toString(): string { return this.name; }
来源：http://hz.cheryme.top/gthdvsebys.html

Java: @Override public String toString() { return name; }
来源：http://hz.jqgufenzy.top/gtpassvamf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hongshengwenyu.top/gtdubsukxd.html

Ruby: def to_s; @name; end
来源：http://hz.yj202588.top/gteydzhwio.html

C#:   public override string ToString() => Name;
来源：http://hz.wangshuangyany.cn/gthscxoyij.html

[G13] 判断对象类型
来源：http://hz.xylfe.cn/gtdiabgqxp.html

Py:   isinstance(u, User)
来源：http://hz.zdqjudy.top/gtswpzmhaq.html

PHP:  $u instanceof User
来源：http://hz.yj202588.top/gtxqszijid.html

JS:   u instanceof User
来源：http://hz.guannengcc.top/gtpuzwqbui.html

TS:   u instanceof User
来源：http://hz.iojbl.cn/gtajgjdwmk.html

Java: u instanceof User
来源：http://hz.zycfv.cn/gtbdrpljfq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.sweek.top/gteyhxvopl.html

Ruby: u.is_a?(User)
来源：http://hz.gogol.net.cn/gtldwmxstb.html

C#:   u is User
来源：http://hz.jqgfzy.top/gtbvhbwhov.html

[G14] 数据类 / record
来源：http://hz.jianghu66.top/gtybvfkijk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.fengsongda.top/gtiynlclsq.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.shanyushiyangtech.top/gtjvakldej.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.aizwys.cn/gtmpzewicn.html

TS:   type User = { name: string; age: number };
来源：http://hz.yj20258.top/gtndirgxai.html

Java: record User(String name, int age) {}
来源：http://hz.guowangkeji.top/gtxdwceonn.html

Go:   type User struct { Name string; Age int }
来源：http://hz.yangfankeji.com/gtmqylhgjp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinqigufen.top/gthjweqmhg.html

C#:   record User(string Name, int Age);
来源：http://hz.pengpengdd.cyou/gtarurorip.html

[G15] 枚举
来源：http://hz.xuetiantiany.cn/gtzylzfoeb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yuxming.cn/gtwzhicoix.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.havefunace.top/gtrmhpvzrs.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hysaishi.cn/gtytvocmxx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.xylfe.cn/gtmjfnaydn.html

Java: enum Color { RED, GREEN }
来源：http://hz.sufxvd.cn/gtjxoicrmz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.zhaomingkeji.xyz/gtonynbvtt.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ydzc1.top/gtlnfkqzwd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.guowangkeji.top/gtgtbiakgk.html

[G16] 对象转数组 / 字典
来源：http://hz.jinyuanbaomall.cn/gtjnazzbvn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhoulong.xyz/gtzwlffwpy.html

PHP:  get_object_vars($obj);
来源：http://hz.cheryme.top/gtpapyfawj.html

JS:   Object.entries(obj)
来源：http://hz.yonumen.top/gtlstwlzke.html

TS:   Object.entries(obj)
来源：http://hz.xingfuxueyuan.xyz/gtatrdpexo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.tian-w.cn/gtpqxdhkww.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.wangshuangyany.cn/gtirmlbvzd.html

Ruby: obj.instance_variables
来源：http://hz.mhx1999.top/gtbykrkvim.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.wangdashe.top/gtiodqnelv.html

================================================================================
来源：http://hz.cqqwz.cn/gtcdbkaqlg.html

H. 异常与错误处理
来源：http://hz.wangshuangyany.cn/gtwuhauqmg.html

================================================================================
来源：http://hz.bjfxy.top/gtnplcqrog.html

[H01] try / catch 基础
来源：http://hz.meibo888.top/gtvuoxdbnl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.dashuyun.cn/gtfbuvxvss.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yj202588.top/gtywpyohbn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.nanxinkj.top/gtbcwqtjpg.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.ehwqpu.com/gtkrfkduvx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yangfankeji.com/gtjraxkfdp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.wangdashe.top/gtjzludcut.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.hfpthk.cn/gtfqrblaun.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.c1oappe.top/gtjrhyuuvc.html

[H02] finally / ensure 收尾
来源：http://hz.ppjwa.cn/gtlezbdnjn.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.mhx1999.top/gtmiwkmcyf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.xinyue.icu/gtcweouptb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.daria6918.cn/gtvksybtrg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgufenzy.top/gthrrbismb.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.fzhhl.top/gtfmmjjslz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hnqzz.top/gtwvusqzpf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.zhijiandao.cn/gthgepwkjg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.hammf.cn/gtjrkronvq.html

[H03] 主动抛出异常
来源：http://hz.yongpay.top/gtumjaopbr.html

Py:   raise ValueError("错误信息")
来源：http://hz.xuetiantiany.cn/gtiwuvgnog.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.svipenyu.cn/gtrkgmjthk.html

JS:   throw new Error("错误信息");
来源：http://hz.52xcode.cn/gtrpqizkpm.html

TS:   throw new Error("错误信息");
来源：http://hz.shzxlz.cn/gtjwqohrjb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.gzhubu.top/gtidqifdcz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.hnxiangtu.top/gtbnhqauhc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.chenjidiqi.icu/gtgwyadqfh.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jiagoushi.top/gtcakzarfq.html

[H04] 自定义异常类型
来源：http://hz.smart0.xyz/gthxwuiqfs.html

Py:   class MyError(Exception): pass
来源：http://hz.dianchejie.cn/gtmyrobycb.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.cqqwz.cn/gtoklaecjr.html

JS:   class MyError extends Error {}
来源：http://hz.jqgufenzy.top/gtoklwqxrq.html

TS:   class MyError extends Error {}
来源：http://hz.9152youxi.cn/gtduhcolha.html

Java: class MyException extends RuntimeException {}
来源：http://hz.chenjidiqi.icu/gtrbfkgsmt.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ybcxt.top/gtyztgcahg.html

Ruby: class MyError < StandardError; end
来源：http://hz.cheryme.top/gtouhlrprt.html

C#:   class MyException : Exception {}
来源：http://hz.cqqwz.cn/gtusaofoge.html

[H05] 捕获特定类型
来源：http://hz.ybcxt.top/gtkncsxsca.html

Py:   except ValueError as e:
来源：http://hz.yvedp.cn/gttlsyrdqr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xuanzx.com/gteaefgcjq.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.guowangkeji.top/gtivjegbqo.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jinqigufen.top/gtxgptsrkw.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.aizwys.cn/gtjpwuzvnr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.yvedp.cn/gtgetvdwey.html

Ruby: rescue ArgumentError => e
来源：http://hz.yj202588.top/gtvfdniakp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.fengsongda.top/gtrndkqebv.html

[H06] 可选值 / 空值安全访问
来源：http://hz.0kj1m.cn/gtbfnezovw.html

Py:   value = d.get("k") or default
来源：http://hz.redwolf501.top/gtgxtybxmr.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.ppjwa.cn/gtndpfwywy.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.ywan-chungtsiang.top/gtnppgigsi.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jlsjyb.cn/gtvebhadwl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.xuanzx.com/gtgcyqubnq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.daxiang520.top/gttcnawqsw.html

Ruby: d&.dig(:a, :b)
来源：http://hz.dianchejie.cn/gtjhdjkmqs.html

C#:   obj?.A?.B ?? default
来源：http://hz.jinghuilouyu.cn/gtfhvxnysz.html

[H07] 断言
来源：http://hz.wangdashe.top/gthemzgeiz.html

Py:   assert x > 0, "必须为正"
来源：http://hz.chenlongwang.top/gtlnjgwlyb.html

PHP:  assert($x > 0);
来源：http://hz.tian-w.cn/gtdmrkghls.html

JS:   console.assert(x > 0);
来源：http://hz.jinqigufen.top/gtbksefrxu.html

TS:   console.assert(x > 0);
来源：http://hz.guannengcc.top/gteynaxhxm.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhiwuduotai.top/gtmzlvhydb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gaohongyu789.top/gtaqiumgrp.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tian-w.cn/gtatvkckmg.html

C#:   Debug.Assert(x > 0);
来源：http://hz.iojbl.cn/gtpqzrhrpg.html

[H08] 获取错误信息与堆栈
来源：http://hz.daria6918.cn/gtszelcxcy.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cucudq.cn/gtpamxtgjj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zhengqikj.top/gtvtwjqced.html

JS:   e.message;  e.stack
来源：http://hz.zhixingplan.top/gttqetpdrr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.svipenyu.cn/gtnkcvtkgq.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.havefunace.top/gtwowyzhjt.html

Go:   err.Error()
来源：http://hz.tianlin.xyz/gtscagmrgb.html

Ruby: e.message;  e.backtrace
来源：http://hz.ehwqpu.com/gtkumarjnu.html

C#:   e.Message;  e.StackTrace
来源：http://hz.fengsongda.top/gtwcphoiug.html

[H09] 带错误码的异常
来源：http://hz.sxryk.cn/gtycivwzbk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.jiagoushi.top/gtdndlwmym.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.vqdsnc.cn/gtjjchreqv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jinqigufen.top/gttbfgaaoe.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.redwolf501.top/gtrtybyxtw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.9152youxi.cn/gtpscgubvq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.xinyue.icu/gtoumfkfgl.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.haohaochexian.top/gtbcbsnmjf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.iojbl.cn/gtxzisbjtf.html

[H10] 资源自动释放
来源：http://hz.hammf.cn/gtxqvkicoa.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.sysykeji.top/gtdenypbjf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.shuidangran.top/gtgzpronst.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yj20258.top/gtlwjgpxtr.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.bjfxy.top/gthxojgakb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.ydjk.org.cn/gtvkqyhlop.html

Go:   defer f.Close()
来源：http://hz.kuanghao11.cn/gtzlxddzfh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.nwbrower.top/gtmoidelen.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.ybcxt.top/gtikrpdzdc.html

================================================================================
来源：http://hz.nanxuanxn.top/gtksqutmnt.html

I. 正则表达式
来源：http://hz.cucudq.cn/gtqgilbtly.html

================================================================================
来源：http://hz.chenlongwang.top/gtsbjujrly.html

[I01] 判断是否匹配
来源：http://hz.aibaodan.cn/gtvnrxrlul.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xylfe.cn/gtpdrzaigd.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zycfv.cn/gtsfkztvho.html

JS:   /\d+/.test(s)
来源：http://hz.zhijiandao.cn/gtizkbgzjl.html

TS:   /\d+/.test(s)
来源：http://hz.fengsongda.top/gtxbluuoep.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.nanxuanxn.top/gtinyltmdd.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.ppjwa.cn/gtencrxwpp.html

Ruby: s.match?(/\d+/)
来源：http://hz.aizwys.cn/gtzlnosgyk.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.52xcode.cn/gtzulmkfgf.html

[I02] 提取所有匹配
来源：http://hz.birdmap.top/gtlsanpagt.html

Py:   re.findall(r"\d+", s)
来源：http://hz.zhijiandao.cn/gtdyctxcof.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yueranfly.top/gtyyhylhep.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.bjfxy.top/gtboofavce.html

TS:   s.match(/\d+/g)
来源：http://hz.jqgufenzy.top/gtaeflyhpj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.jqgufenzy.top/gtqiwtlyba.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.hammf.cn/gtjqsciety.html

Ruby: s.scan(/\d+/)
来源：http://hz.redwolf501.top/gttjbwzbvx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.wangdashe.top/gtmvatpvrd.html

[I03] 提取捕获分组
来源：http://hz.gotoacloud.top/gtkygvnbrp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.fengsongda.top/gtqydbatmq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.hywenlv.cn/gtdjmhsjua.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.gaohongyu789.top/gtrnxemsjp.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.hfpthk.cn/gtknqtjuay.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.shzxlz.cn/gtvtvhbqdr.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.jinqigfzy.top/gteepgqgir.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.yueranfly.top/gtzkxagduh.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.birdmap.top/gtgcqneulb.html

[I04] 正则替换
来源：http://hz.sysykeji.top/gtwviexrlc.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.cheryme.top/gtdnwectoo.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.kuanghao11.cn/gtpfldlbxx.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.yangfankeji.com/gtrwlgxcrj.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.pycfn.com/gtzyeyydew.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.0kj1m.cn/gtrawbdavl.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.meibo888.top/gtikzjpuzp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.nanxinkj.top/gtzmntyszk.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yongpay.top/gtxumdlxqy.html

[I05] 按正则拆分
来源：http://hz.gaohongyu789.top/gtuquuldyq.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.xinyue.icu/gtzexxrwev.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.9152youxi.cn/gtpsjorkam.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.zhaomingkeji.xyz/gtirnyphfx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.haohaochexian.top/gtkfvgpntz.html

Java: s.split("\\s*,\\s*")
来源：http://hz.shangyingyoupin.top/gttuheisyn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yvedp.cn/gturwcehpl.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yuxming.cn/gtlfkvhdtd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhaomingkeji.xyz/gtandqwvmv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.pengpengdd.cyou/gtgsqrrsyj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.wangshuangyany.cn/gtouslvlmy.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.pycfn.com/gttpnunzed.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj20258.top/gtobbwjtrj.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.jinghuilouyu.cn/gtyphzgmfg.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tian-w.cn/gtrnxxjkfl.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jqgufenzy.top/gtktopucnz.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.fzhhl.top/gtmiiskhfk.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.yonumen.top/gttrmrhdhy.html

[I07] 忽略大小写与多行模式
来源：http://hz.bjfxy.top/gtffxcqojy.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhiwuduotai.top/gtjxxnsapo.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.nwbrower.top/gtetowfdiy.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.nanxinkj.top/gtgljexqtp.html

TS:   /error/gim
来源：http://hz.yueranfly.top/gtgwjnzhwc.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hnxiangtu.top/gtvglccrms.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.yj202588.top/gtfplvimuh.html

Ruby: s.scan(/error/i)
来源：http://hz.ydjk.org.cn/gtmebccogs.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.jqgufenzy.top/gtgboaorix.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.sxryk.cn/gtdcsiiapg.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhongyouzk.top/gtwjyisvpa.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.jinqigfzy.top/gtbdtjwefm.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.shanyushiyangtech.top/gtvxnudbsf.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tianlin.xyz/gtohzxbvag.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.smart0.xyz/gtcroinpyp.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.chenjidiqi.icu/gtjbppzdtg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.jqgfzy.top/gttxkzhzeh.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.hongshengwenyu.top/gtqhmuexqj.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtauijjirl.html

J. 日期与时间
来源：http://hz.xylfe.cn/gtbaidkner.html

================================================================================
来源：http://hz.daxiang520.top/gtiijnxxzc.html

[J01] 获取当前时间
来源：http://hz.yongpay.top/gttqtlhezn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.zhoulong.xyz/gtibdhxlvr.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.bjfxy.top/gtokwoxgdb.html

JS:   new Date();  Date.now()
来源：http://hz.gaohongyu789.top/gtaqzvuqro.html

TS:   new Date();  Date.now()
来源：http://hz.yueranfly.top/gtfdarggvc.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.feifeiyinyue.top/gtmozefwxa.html

Go:   time.Now()
来源：http://hz.iojbl.cn/gtsoyicsrr.html

Ruby: Time.now
来源：http://hz.zhongyouzk.top/gtmuknnjlw.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.snrcjt.cn/gtoxpnjvza.html

[J02] 格式化输出
来源：http://hz.hysaishi.cn/gtsikiowov.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jqgfzy.top/gtkkpgafmh.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.ehwqpu.com/gtpzpqqeab.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ydzc1.top/gthoounmrh.html

TS:   d.toISOString()
来源：http://hz.yuxming.cn/gtageezpfw.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.sysykeji.top/gtmrortgax.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.tian-w.cn/gtxbxkrsml.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.dashuyun.cn/gthlqnhrki.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.tian-w.cn/gtznylqvml.html

[J03] 字符串解析为日期
来源：http://hz.guowangkeji.top/gttmnkoskk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.iojbl.cn/gttvskiair.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.hywenlv.cn/gtidrkfgav.html

JS:   new Date("2024-01-02")
来源：http://hz.havefunace.top/gtybmfllly.html

TS:   new Date("2024-01-02")
来源：http://hz.shuidangran.top/gtyfgusfyb.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.nanxinkj.top/gtuukoiymt.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.ppjwa.cn/gtbwqtcxhc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.ehwqpu.com/gtmanvlvvt.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hfpthk.cn/gtudlvijch.html

[J04] 时间戳与日期互转
来源：http://hz.zhongyouzk.top/gtmgodozgf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.xziqi.cn/gtswcykoyk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhaomingkeji.xyz/gtdlhelpvo.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.kuanghao11.cn/gtlskbzbaw.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.pycfn.com/gtnuvwwuzg.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.jqgufenzy.top/gtbjlifxdx.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jyoumei.cn/gtsquaupbu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hywenlv.cn/gtgcccszag.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.ybcxt.top/gtzjgipbts.html

[J05] 时间加减（加 7 天）
来源：http://hz.sweek.top/gtrbwnqjgp.html

Py:   now + timedelta(days=7)
来源：http://hz.ehwqpu.com/gthbfoujep.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.ivvv.top/gtrdmakwsj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.cashguo.top/gtfejwwynl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.yonumen.top/gtsvxqafwi.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.zhongyouzk.top/gtztiodjft.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ppjwa.cn/gthyxwqvyd.html

Ruby: Time.now + 7 * 86400
来源：http://hz.gotoacloud.top/gtdwoclepd.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.hnxiangtu.top/gtfehtyyfz.html

[J06] 计算两时间之差
来源：http://hz.pengpengdd.cyou/gtrydrxrot.html

Py:   (end - start).total_seconds()
来源：http://hz.gogol.net.cn/gtobybtmfm.html

PHP:  $end->diff($start)->days;
来源：http://hz.jqgufenzy.top/gtesnshgne.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.bjfxy.top/gtxldkhoph.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sxryk.cn/gtgpmygtub.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.cqqwz.cn/gtwytjqnuf.html

Go:   end.Sub(start).Hours()
来源：http://hz.yuxming.cn/gtzyaqitzt.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yj20258.top/gtwzdleizd.html

C#:   (end - start).TotalSeconds
来源：http://hz.cqqwz.cn/gtrltwilzn.html

[J07] 比较两个日期
来源：http://hz.chenzaomai.com/gtymjvnqtw.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.xziqi.cn/gtbgfksrwr.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xinyue.icu/gtexsvgrib.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.jinyuanbaomall.cn/gtwtcamhxt.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.svipenyu.cn/gtengolbyu.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.daria6918.cn/gtlapaarek.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.dashuyun.cn/gtqwffkdil.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.zycfv.cn/gtyfycpvcy.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.zhoulong.xyz/gtjbiiwcfc.html

[J08] 提取年月日与星期
来源：http://hz.jyoumei.cn/gtucuzouqv.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.xylfe.cn/gtjesbdumy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.c1oappe.top/gtysmwjlje.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.sysykeji.top/gtahoholfn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.daria6918.cn/gtxbwtmmjj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.daxiang520.top/gtchttkyrt.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.andypj.xyz/gtzwbcufhf.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.guowangkeji.top/gtijdnsiqr.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jyoumei.cn/gticabcbuf.html

[J09] 时区处理
来源：http://hz.havefunace.top/gtantthqiz.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.tian-w.cn/gtagfdupki.html


<!-- 参考信息 -->