代发 wailian999

TS:   public / protected / private
来源：http://hz.zdqjudy.top/gtslcucbxa.html

Java: public / protected / private / 默认包级
来源：http://hz.cashguo.top/gtfbhssfyc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.birdmap.top/gtjjtliojs.html

Ruby: public / protected / private
来源：http://hz.jinqigfzy.top/gtnpvtuqly.html

C#:   public / protected / private / internal
来源：http://hz.zhongyouzk.top/gtjrpuudzm.html

[G11] getter / setter
来源：http://hz.kuanghao11.cn/gtreckxbdr.html

Py:   @property 与 @x.setter
来源：http://hz.quarkkingdee.top/gtxtniylqu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yangfankeji.com/gtqisngshv.html

JS:   get name() { return this._name; }
来源：http://hz.tanke756.top/gticfacizs.html

TS:   get name(): string { return this._name; }
来源：http://hz.hywenlv.cn/gtsmxyziri.html

Java: public String getName() { return name; }
来源：http://hz.xuetiantiany.cn/gtlbbfnuok.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.vqdsnc.cn/gtmqitpsxh.html

Ruby: attr_accessor :name
来源：http://hz.shangyingyoupin.top/gtaaicbeix.html

C#:   public string Name { get; set; }
来源：http://hz.yj20258.top/gtvbrcplwz.html

[G12] 对象转字符串
来源：http://hz.jlsjyb.cn/gtxxefqgif.html

Py:   def __str__(self): return self.name
来源：http://hz.hammf.cn/gtcrpqqbjt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhoulong.xyz/gtrlgsubwy.html

JS:   toString() { return this.name; }
来源：http://hz.yvedp.cn/gtrertxkrj.html

TS:   toString(): string { return this.name; }
来源：http://hz.hnxiangtu.top/gtwjvdjnog.html

Java: @Override public String toString() { return name; }
来源：http://hz.yongpay.top/gtmqyjscvr.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.daxiang520.top/gtdooupmqs.html

Ruby: def to_s; @name; end
来源：http://hz.cashguo.top/gtnktcvfml.html

C#:   public override string ToString() => Name;
来源：http://hz.dianchejie.cn/gtgasegpsp.html

[G13] 判断对象类型
来源：http://hz.jinqigufen.top/gtmhtpmbxb.html

Py:   isinstance(u, User)
来源：http://hz.hongshengwenyu.top/gtncunijmg.html

PHP:  $u instanceof User
来源：http://hz.aizwys.cn/gtwpwlxnuj.html

JS:   u instanceof User
来源：http://hz.zycfv.cn/gtvvjpdzyp.html

TS:   u instanceof User
来源：http://hz.fzhhl.top/gtggeghsll.html

Java: u instanceof User
来源：http://hz.dianchejie.cn/gtfxncsfrs.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shzxlz.cn/gtenzhfhlf.html

Ruby: u.is_a?(User)
来源：http://hz.hysaishi.cn/gtupgwtwmj.html

C#:   u is User
来源：http://hz.wangshuangyany.cn/gtbjaapgnb.html

[G14] 数据类 / record
来源：http://hz.hongshengwenyu.top/gtckwepaio.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.andypj.xyz/gttjrmrfqe.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.wangdashe.top/gteotrmzxe.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.aizwys.cn/gtvoaucjsf.html

TS:   type User = { name: string; age: number };
来源：http://hz.guowangkeji.top/gttgctiatg.html

Java: record User(String name, int age) {}
来源：http://hz.nanxinkj.top/gtxjqpaqnl.html

Go:   type User struct { Name string; Age int }
来源：http://hz.gaohongyu789.top/gtzaqrptqj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jinyuanbaomall.cn/gtekoxcteq.html

C#:   record User(string Name, int Age);
来源：http://hz.wangdashe.top/gtsxtvbvng.html

[G15] 枚举
来源：http://hz.zhiwuduotai.top/gtdrswsemi.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.jqgfzy.top/gtcmhgxgmw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.nanxuanxn.top/gtfhjlyjeu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.meibo888.top/gtknagwtcw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.dianchejie.cn/gtstyoqvha.html

Java: enum Color { RED, GREEN }
来源：http://hz.yuxming.cn/gtcfeuahsc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.nanxuanxn.top/gteufbhhsr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.shzxlz.cn/gtrpmldmif.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.snrcjt.cn/gtypprudim.html

[G16] 对象转数组 / 字典
来源：http://hz.hywenlv.cn/gtmvzxwigl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.sweek.top/gthqfsnmld.html

PHP:  get_object_vars($obj);
来源：http://hz.daria6918.cn/gtncsjlyfx.html

JS:   Object.entries(obj)
来源：http://hz.xingfuxueyuan.xyz/gtjnmdweus.html

TS:   Object.entries(obj)
来源：http://hz.jinghuilouyu.cn/gtgahizpbd.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.zhongyouzk.top/gtkaccyogi.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.nanxinkj.top/gtnsuzrjve.html

Ruby: obj.instance_variables
来源：http://hz.yj202588.top/gtgnqukkhi.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ivvv.top/gtluscgocs.html

================================================================================
来源：http://hz.haohaochexian.top/gthotzmqaa.html

H. 异常与错误处理
来源：http://hz.yongpay.top/gtjiavgtld.html

================================================================================
来源：http://hz.sweek.top/gtyjkvlpts.html

[H01] try / catch 基础
来源：http://hz.zdqjudy.top/gtpjdgjutt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yanxiufei.cn/gtqapmsjkx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hfpthk.cn/gtsutnnifs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.hongshengwenyu.top/gtfnextdlw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.zhiwuduotai.top/gtxwpjajlx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.ivvv.top/gtjnsgjrqw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yonumen.top/gtaxgzrotk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yanxiufei.cn/gtilojpbhs.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.zhongyouzk.top/gttylkjmwf.html

[H02] finally / ensure 收尾
来源：http://hz.andypj.xyz/gtlubtqazo.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.kuanghao11.cn/gtbyynfgib.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.zycfv.cn/gtbshzwwtp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.jqgfzy.top/gtiauuaywv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.jiagoushi.top/gtrkdgcoht.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.tian-w.cn/gtvnwbiytw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.jqgfzy.top/gtvytzevro.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.jinghuilouyu.cn/gtgcwsiqoc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.ybcxt.top/gtxntmtrwe.html

[H03] 主动抛出异常
来源：http://hz.gotoacloud.top/gtewftimpd.html

Py:   raise ValueError("错误信息")
来源：http://hz.c1oappe.top/gtnwfmnnhr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.c1oappe.top/gtunslygma.html

JS:   throw new Error("错误信息");
来源：http://hz.ybcxt.top/gtdmpdjbia.html

TS:   throw new Error("错误信息");
来源：http://hz.yuxming.cn/gtngkeghur.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.c1oappe.top/gthmxxprgi.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.wangdashe.top/gtyfymljqq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ppjwa.cn/gtrnivjlfp.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.cashguo.top/gtixkwqwih.html

[H04] 自定义异常类型
来源：http://hz.kuanghao11.cn/gtltadorjk.html

Py:   class MyError(Exception): pass
来源：http://hz.daxiang520.top/gtmgaophpd.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.jinyuanbaomall.cn/gteijilxwx.html

JS:   class MyError extends Error {}
来源：http://hz.andypj.xyz/gtserlzoih.html

TS:   class MyError extends Error {}
来源：http://hz.gogol.net.cn/gtiijggzji.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hywenlv.cn/gtmzxfxcxs.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.shangyingyoupin.top/gtkrgblwsx.html

Ruby: class MyError < StandardError; end
来源：http://hz.tian-w.cn/gtbdjueqgs.html

C#:   class MyException : Exception {}
来源：http://hz.redwolf501.top/gtlsdhdscu.html

[H05] 捕获特定类型
来源：http://hz.wangshuangyany.cn/gtbhgognlx.html

Py:   except ValueError as e:
来源：http://hz.hysaishi.cn/gtmdumhaqt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.sweek.top/gtafqorjen.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jinghuilouyu.cn/gtoxxhkrax.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.xylfe.cn/gtyghlzvtz.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ydzc1.top/gtpvbiwmgg.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.sxryk.cn/gtmygvsfhf.html

Ruby: rescue ArgumentError => e
来源：http://hz.hnqzz.top/gtezmffphd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.fengsongda.top/gtznbyvvfz.html

[H06] 可选值 / 空值安全访问
来源：http://hz.yj202588.top/gtarkbkfyb.html

Py:   value = d.get("k") or default
来源：http://hz.hammf.cn/gtrdehoevg.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yangfankeji.com/gtqxesuuzr.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.hywenlv.cn/gtytasrnwv.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.smart0.xyz/gtbkataoju.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.ppjwa.cn/gtvqjthkwr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.fzhhl.top/gtmntpnyyb.html

Ruby: d&.dig(:a, :b)
来源：http://hz.bjfxy.top/gtbwasytad.html

C#:   obj?.A?.B ?? default
来源：http://hz.zycfv.cn/gtxsetjyyh.html

[H07] 断言
来源：http://hz.52xcode.cn/gtokfkockb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhengqikj.top/gtdmimuwua.html

PHP:  assert($x > 0);
来源：http://hz.wangdashe.top/gtijjlighw.html

JS:   console.assert(x > 0);
来源：http://hz.ehwqpu.com/gtlunmwdfd.html

TS:   console.assert(x > 0);
来源：http://hz.xziqi.cn/gthrvqfjmk.html

Java: assert x > 0 : "必须为正";
来源：http://hz.chenjidiqi.icu/gtjmwhpjdo.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yueranfly.top/gtefftmguw.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.0kj1m.cn/gtctegqdgm.html

C#:   Debug.Assert(x > 0);
来源：http://hz.jlsjyb.cn/gtvvsdpsop.html

[H08] 获取错误信息与堆栈
来源：http://hz.hammf.cn/gtcuflwqbu.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jinqigufen.top/gtobpgdkrw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.redwolf501.top/gtyzxaromt.html

JS:   e.message;  e.stack
来源：http://hz.wangdashe.top/gtjxvgphni.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.shanyushiyangtech.top/gtzkzibljz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.svipenyu.cn/gtovllensd.html

Go:   err.Error()
来源：http://hz.ydjk.org.cn/gtjgythige.html

Ruby: e.message;  e.backtrace
来源：http://hz.aizwys.cn/gtrmsnqzot.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yj20258.top/gtblyzqheo.html

[H09] 带错误码的异常
来源：http://hz.shangyingyoupin.top/gtuktqengo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.zdqjudy.top/gtsalascac.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.haohaochexian.top/gtgbjxpjpf.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.chenlongwang.top/gtmbrbbpuh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.dashuyun.cn/gtnsrftyaw.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hongshengwenyu.top/gtsctguooc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hnxiangtu.top/gtpdxfseil.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.cdnleiting.top/gtjluxfsop.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.fengsongda.top/gtpkhezkso.html

[H10] 资源自动释放
来源：http://hz.hfpthk.cn/gtcpznrqsc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.dashuyun.cn/gtvwwewewr.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xuanzx.com/gtnhwdcshh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxinkj.top/gtjyrhuoyb.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.jqgufenzy.top/gtwzsmgxma.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.52xcode.cn/gtcvnctsyc.html

Go:   defer f.Close()
来源：http://hz.xinyue.icu/gtycpzqwyf.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.svipenyu.cn/gttdtzandw.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.bjfxy.top/gthzxstteh.html

================================================================================
来源：http://hz.ydjk.org.cn/gtykmcvbus.html

I. 正则表达式
来源：http://hz.gogol.net.cn/gtpcoxooqu.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtmtgrtggn.html

[I01] 判断是否匹配
来源：http://hz.shangyingyoupin.top/gtecteubih.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.dashuyun.cn/gtbsjumrev.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.c1oappe.top/gtxcdjtoan.html

JS:   /\d+/.test(s)
来源：http://hz.gzhubu.top/gtjimajgmu.html

TS:   /\d+/.test(s)
来源：http://hz.zhiwuduotai.top/gtidrkitlk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.daxiang520.top/gtgwuceksy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.shzxlz.cn/gtamkdtzpw.html

Ruby: s.match?(/\d+/)
来源：http://hz.zhijiandao.cn/gtrmkslezu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.hnqzz.top/gtagrcybhm.html

[I02] 提取所有匹配
来源：http://hz.feifeiyinyue.top/gtczvsdrgw.html

Py:   re.findall(r"\d+", s)
来源：http://hz.52xcode.cn/gtbfneteyy.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhaomingkeji.xyz/gtgtijoamo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.jqgufenzy.top/gtakrdnbda.html

TS:   s.match(/\d+/g)
来源：http://hz.guowangkeji.top/gtezzfynwm.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.redwolf501.top/gtrbyplofp.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.zycfv.cn/gtmwrmzuhv.html

Ruby: s.scan(/\d+/)
来源：http://hz.guannengcc.top/gtbumeeaif.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.yj20258888.top/gteywalbxf.html

[I03] 提取捕获分组
来源：http://hz.yanxiufei.cn/gtycmnixnj.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xinyue.icu/gtipxwyaua.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.meibo888.top/gtadidlfjq.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.fzhhl.top/gtitqvwxcu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yangfankeji.com/gtuspaaetj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.xylfe.cn/gtlawsfbiv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.hysaishi.cn/gttjzkjuto.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.gzhubu.top/gtzoajslfe.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.ehwqpu.com/gtnskkdsvy.html

[I04] 正则替换
来源：http://hz.gogol.net.cn/gtldxdzfdz.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.meibo888.top/gtkjhmuasr.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ybcxt.top/gtewhuqasc.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.svipenyu.cn/gtlsqmnuvs.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yongpay.top/gttonbyhmj.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.smart0.xyz/gtystgubdh.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.hfpthk.cn/gtxkoyesxq.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.yvedp.cn/gtizfzcuwx.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.sufxvd.cn/gtbtcwmkxd.html

[I05] 按正则拆分
来源：http://hz.mhx1999.top/gtnfwqrbkr.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cashguo.top/gtlbdojdhu.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gzhubu.top/gtchyzftlk.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.svipenyu.cn/gtnosxvgwx.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.yanxiufei.cn/gtkytmbixe.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hnxiangtu.top/gtndwcwhec.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.redwolf501.top/gtbspptpjk.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.shangyingyoupin.top/gtuejqtedr.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.c1oappe.top/gtetkhvwfm.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.guannengcc.top/gtsersengo.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.9152youxi.cn/gtiusvelnh.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yuxming.cn/gtnpjwzkte.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangtech.top/gteyxzhylc.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ywan-chungtsiang.top/gtizxlwwcq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.aizwys.cn/gtieryoxij.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hywenlv.cn/gtgmqknysq.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.vqdsnc.cn/gtaxchzzsx.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zdqjudy.top/gthqxsapyi.html

[I07] 忽略大小写与多行模式
来源：http://hz.zhengqikj.top/gtxjefkzsn.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zycfv.cn/gtlofgsqve.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.shuidangran.top/gtzwcmgars.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.tianlin.xyz/gtanlcunqg.html

TS:   /error/gim
来源：http://hz.yonumen.top/gtffcltqfy.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.hnxiangtu.top/gtqehawefp.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.mhx1999.top/gtmzrteuwl.html

Ruby: s.scan(/error/i)
来源：http://hz.jianghu66.top/gthldquzfd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.chenjidiqi.icu/gtaxyzrorz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.tanke756.top/gtgzquelyn.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.cdnleiting.top/gtbshvhrdx.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.gogol.net.cn/gtiahuhzhx.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.tanke756.top/gthatmqpbh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.hysaishi.cn/gtmsltuxys.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.wangshuangyany.cn/gtmjfxxtjq.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.jiagoushi.top/gtohlwxzfc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yanxiufei.cn/gtejuxqlau.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.yonumen.top/gtivarxhta.html

================================================================================
来源：http://hz.redwolf501.top/gtgcgokrmh.html

J. 日期与时间
来源：http://hz.jinghuilouyu.cn/gtaglkjdtb.html

================================================================================
来源：http://hz.birdmap.top/gtcsktexzw.html

[J01] 获取当前时间
来源：http://hz.gzhubu.top/gttqgwstug.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.chenlongwang.top/gthdnessfy.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.nwbrower.top/gtkuzeqbjy.html

JS:   new Date();  Date.now()
来源：http://hz.yuanzhike.top/gtpmnrcgbw.html

TS:   new Date();  Date.now()
来源：http://hz.havefunace.top/gtjkbfrkfa.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.cucudq.cn/gtnpzkiexm.html

Go:   time.Now()
来源：http://hz.hnxiangtu.top/gtassdyiqu.html

Ruby: Time.now
来源：http://hz.hammf.cn/gtbcozlnkz.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.iojbl.cn/gtlvgvpfbe.html

[J02] 格式化输出
来源：http://hz.xylfe.cn/gtaprwhvsx.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xinyue.icu/gtlbnaatia.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhiwuduotai.top/gtlpciqqtj.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.zhixingplan.top/gtfljbozvi.html

TS:   d.toISOString()
来源：http://hz.xziqi.cn/gtwtkbhufe.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.jinghuilouyu.cn/gtbjfaqdsn.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.iojbl.cn/gtyrnuzvwf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xziqi.cn/gtjxnrroxw.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ydjk.org.cn/gtubepbsyd.html

[J03] 字符串解析为日期
来源：http://hz.haohaochexian.top/gtzfpxicmk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinqigufen.top/gtiggbjlxl.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.chenzaomai.com/gttckktlpt.html

JS:   new Date("2024-01-02")
来源：http://hz.birdmap.top/gtqswcvika.html

TS:   new Date("2024-01-02")
来源：http://hz.jinqigfzy.top/gtlkkftfpv.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.chenzaomai.com/gtqnylrwwg.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.jinyuanbaomall.cn/gtpsndgeaq.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.xuetiantiany.cn/gtmeejrvuz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jlsjyb.cn/gtvwsmvkzh.html

[J04] 时间戳与日期互转
来源：http://hz.zhongyouzk.top/gtqdlmjwwu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yanxiufei.cn/gtvdihdwsd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.jianghu66.top/gtuebmftzj.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.pycfn.com/gtqcpcfggf.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.gogol.net.cn/gtxdjkuxrv.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.hammf.cn/gtbopopakv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jqgufenzy.top/gtuzapgxpw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.hnxiangtu.top/gtzvvbnofp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.0kj1m.cn/gtrdtwnqmv.html

[J05] 时间加减（加 7 天）
来源：http://hz.hywenlv.cn/gtuosdahdb.html

Py:   now + timedelta(days=7)
来源：http://hz.yj20258.top/gtszecaehy.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.nanxuanxn.top/gtztetsote.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jqgufenzy.top/gtriijgsbt.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.nanxuanxn.top/gtcvzgdurk.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.aibaodan.cn/gtfkzfnimk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.feifeiyinyue.top/gtmuhtllow.html

Ruby: Time.now + 7 * 86400
来源：http://hz.aibaodan.cn/gtpmhsflgs.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.mhx1999.top/gtpxxruofp.html

[J06] 计算两时间之差
来源：http://hz.gaohongyu789.top/gtghweyunt.html

Py:   (end - start).total_seconds()
来源：http://hz.jyoumei.cn/gtwmbcrgty.html

PHP:  $end->diff($start)->days;
来源：http://hz.zhijiandao.cn/gttujnzuzt.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.tanke756.top/gtpactkayx.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.smart0.xyz/gtbnjjehva.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.mhx1999.top/gtjiuntint.html

Go:   end.Sub(start).Hours()
来源：http://hz.ivvv.top/gtjoxvyfqt.html

Ruby: end - start                 # 返回秒数
来源：http://hz.pengpengdd.cyou/gtpytbclva.html

C#:   (end - start).TotalSeconds
来源：http://hz.xylfe.cn/gtqewxelhe.html

[J07] 比较两个日期
来源：http://hz.sxryk.cn/gtwwgmfqje.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yangfankeji.com/gtdpynfmgw.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cashguo.top/gtnnezfaea.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.ywan-chungtsiang.top/gtwvpcfvrv.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.kuanghao11.cn/gtpfkkfobx.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.fzhhl.top/gtapnqshbc.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.quarkkingdee.top/gtslfbosik.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gtibtryliu.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gtknlpcabp.html

[J08] 提取年月日与星期
来源：http://hz.0kj1m.cn/gtfuuwcunh.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.jinghuilouyu.cn/gtipdnfugy.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.tianlin.xyz/gtoioyupjc.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.52xcode.cn/gtbtbqzxkn.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.hongshengwenyu.top/gtvnbcknzv.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.sxryk.cn/gtfouleyyk.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.hywenlv.cn/gtxkjxlnon.html


<!-- 参考信息 -->