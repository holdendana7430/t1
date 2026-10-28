代发 wailian999

JS:   get name() { return this._name; }
来源：http://hz.xingfuxueyuan.xyz/gtkcndrvdd.html

TS:   get name(): string { return this._name; }
来源：http://hz.yvedp.cn/gtnxqynqgf.html

Java: public String getName() { return name; }
来源：http://hz.quarkkingdee.top/gthskmjxul.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sxryk.cn/gtnbwprlpv.html

Ruby: attr_accessor :name
来源：http://hz.iojbl.cn/gtqztnmwtd.html

C#:   public string Name { get; set; }
来源：http://hz.jqgufenzy.top/gtlqoamvyc.html

[G12] 对象转字符串
来源：http://hz.cqqwz.cn/gtxoqcimpw.html

Py:   def __str__(self): return self.name
来源：http://hz.gzhubu.top/gtrcajofbr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.ehwqpu.com/gtmyhblyea.html

JS:   toString() { return this.name; }
来源：http://hz.ppjwa.cn/gtowvoawfp.html

TS:   toString(): string { return this.name; }
来源：http://hz.sufxvd.cn/gtojdhlowt.html

Java: @Override public String toString() { return name; }
来源：http://hz.hnqzz.top/gthaxyziwh.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.wangdashe.top/gtkzbdcovt.html

Ruby: def to_s; @name; end
来源：http://hz.zhongyouzk.top/gtxvqmcdeq.html

C#:   public override string ToString() => Name;
来源：http://hz.yuanzhike.top/gtulwoaoxv.html

[G13] 判断对象类型
来源：http://hz.yuanzhike.top/gtzkcdustv.html

Py:   isinstance(u, User)
来源：http://hz.fzhhl.top/gtcvodkqai.html

PHP:  $u instanceof User
来源：http://hz.zdqjudy.top/gtcgjadfax.html

JS:   u instanceof User
来源：http://hz.chenjidiqi.icu/gthenjlxjt.html

TS:   u instanceof User
来源：http://hz.birdmap.top/gtiyghgaun.html

Java: u instanceof User
来源：http://hz.jqgufenzy.top/gtcgdsvpdt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shanyushiyangtech.top/gtfuttiyew.html

Ruby: u.is_a?(User)
来源：http://hz.shzxlz.cn/gtiwtgwibk.html

C#:   u is User
来源：http://hz.ehwqpu.com/gtbdeoopzl.html

[G14] 数据类 / record
来源：http://hz.xylfe.cn/gtzhirblnc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.havefunace.top/gtjdyentpn.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.c1oappe.top/gtuibogtnh.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.gogol.net.cn/gthckmcohh.html

TS:   type User = { name: string; age: number };
来源：http://hz.hysaishi.cn/gtlydxxwok.html

Java: record User(String name, int age) {}
来源：http://hz.vqdsnc.cn/gtkpqeqynu.html

Go:   type User struct { Name string; Age int }
来源：http://hz.snrcjt.cn/gtawcdnahg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.wangdashe.top/gtpaxgyonl.html

C#:   record User(string Name, int Age);
来源：http://hz.jqgfzy.top/gtqumgdqkg.html

[G15] 枚举
来源：http://hz.snrcjt.cn/gtftmcelso.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ybcxt.top/gtzwemjved.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.shanyushiyangtech.top/gtakdyrblk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.pycfn.com/gtadjsmevc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.andypj.xyz/gttfwmsnzv.html

Java: enum Color { RED, GREEN }
来源：http://hz.xziqi.cn/gtlzqypmkq.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.fzhhl.top/gtkepcvggr.html

Ruby: Color = %i[red green].freeze
来源：http://hz.0kj1m.cn/gtyhnojrtl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yuanzhike.top/gtnoymwriz.html

[G16] 对象转数组 / 字典
来源：http://hz.52xcode.cn/gtpotazqbm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.dashuyun.cn/gtmqhafxyr.html

PHP:  get_object_vars($obj);
来源：http://hz.tanke756.top/gtsfyvvyvx.html

JS:   Object.entries(obj)
来源：http://hz.cashguo.top/gteevxqxei.html

TS:   Object.entries(obj)
来源：http://hz.hysaishi.cn/gtesajcyta.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.smart0.xyz/gtljniqxiy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.fengsongda.top/gtrniuilyn.html

Ruby: obj.instance_variables
来源：http://hz.zhixingplan.top/gttmgsrpwz.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jinghuilouyu.cn/gtrhjethku.html

================================================================================
来源：http://hz.gaohongyu789.top/gtnxzpqxrv.html

H. 异常与错误处理
来源：http://hz.chenlongwang.top/gtbtqrzspf.html

================================================================================
来源：http://hz.nanxinkj.top/gtavkgdymr.html

[H01] try / catch 基础
来源：http://hz.yongpay.top/gttgyztywc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhiwuduotai.top/gtqaddhize.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.c1oappe.top/gtwubqjkxw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.smart0.xyz/gtsuzuxjyu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.gogol.net.cn/gtnkgjtsfg.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.cucudq.cn/gtonhcnqmd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.svipenyu.cn/gthmjqtybg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhengqikj.top/gttgsgaqoa.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.guowangkeji.top/gtvmplpssr.html

[H02] finally / ensure 收尾
来源：http://hz.shzxlz.cn/gthajxpjex.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.jlsjyb.cn/gtpzhctlcq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.tianlin.xyz/gtdphbwefj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.zycfv.cn/gtggawhrng.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.yangfankeji.com/gtdmgaqgxh.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.jianghu66.top/gthqjnfahd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hnqzz.top/gtsqpsmezx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ehwqpu.com/gtogjojuyg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtapcvoelo.html

[H03] 主动抛出异常
来源：http://hz.zhoulong.xyz/gtaeklbwwj.html

Py:   raise ValueError("错误信息")
来源：http://hz.9152youxi.cn/gtqdfbefwt.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.xylfe.cn/gtcffwhjcd.html

JS:   throw new Error("错误信息");
来源：http://hz.hywenlv.cn/gtcgvigpvj.html

TS:   throw new Error("错误信息");
来源：http://hz.hongshengwenyu.top/gterwbmusv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yangfankeji.com/gteutdepgp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.52xcode.cn/gtzuiovvzy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.jlsjyb.cn/gtzrsvsjfb.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.jinqigfzy.top/gtqjxgfrjk.html

[H04] 自定义异常类型
来源：http://hz.smart0.xyz/gtqvgfplyg.html

Py:   class MyError(Exception): pass
来源：http://hz.sysykeji.top/gtbvnvipmp.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.nanxuanxn.top/gtzyvfgqun.html

JS:   class MyError extends Error {}
来源：http://hz.kuanghao11.cn/gthveqfhvz.html

TS:   class MyError extends Error {}
来源：http://hz.daria6918.cn/gtzkkwbjji.html

Java: class MyException extends RuntimeException {}
来源：http://hz.shzxlz.cn/gtptdayhfa.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.aizwys.cn/gtodsitrfk.html

Ruby: class MyError < StandardError; end
来源：http://hz.ydzc1.top/gtiiuenfcd.html

C#:   class MyException : Exception {}
来源：http://hz.quarkkingdee.top/gtejwmyhoi.html

[H05] 捕获特定类型
来源：http://hz.yj20258.top/gtontowwmm.html

Py:   except ValueError as e:
来源：http://hz.jinyuanbaomall.cn/gtozyihmkp.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.bjfxy.top/gttalrxyce.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.fengsongda.top/gtjppzzemv.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.jinyuanbaomall.cn/gtsyfdjytq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.ehwqpu.com/gttsnnzqve.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shangyingyoupin.top/gtpxhvykuw.html

Ruby: rescue ArgumentError => e
来源：http://hz.zhixingplan.top/gtuuyzgklu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.shangyingyoupin.top/gtbvdrrked.html

[H06] 可选值 / 空值安全访问
来源：http://hz.guannengcc.top/gtupfczctt.html

Py:   value = d.get("k") or default
来源：http://hz.fengsongda.top/gthqhuemci.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xziqi.cn/gttguqakkw.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.mhx1999.top/gtzxrvojif.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.sweek.top/gtdpqdfmlc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.pengpengdd.cyou/gtoclyhldg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.bjfxy.top/gtapgcsvet.html

Ruby: d&.dig(:a, :b)
来源：http://hz.shangyingyoupin.top/gtfrsyhytc.html

C#:   obj?.A?.B ?? default
来源：http://hz.hammf.cn/gtwjhwxsdo.html

[H07] 断言
来源：http://hz.bjfxy.top/gtfzcayque.html

Py:   assert x > 0, "必须为正"
来源：http://hz.yangfankeji.com/gtcttxmkpi.html

PHP:  assert($x > 0);
来源：http://hz.zhoulong.xyz/gtwddcwvqh.html

JS:   console.assert(x > 0);
来源：http://hz.yueranfly.top/gtigevbazm.html

TS:   console.assert(x > 0);
来源：http://hz.jinghuilouyu.cn/gtozujcmuf.html

Java: assert x > 0 : "必须为正";
来源：http://hz.sxryk.cn/gtpbcfdxgg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.xylfe.cn/gthvvsglpd.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.zhoulong.xyz/gtikouknqk.html

C#:   Debug.Assert(x > 0);
来源：http://hz.snrcjt.cn/gtifkfxvlc.html

[H08] 获取错误信息与堆栈
来源：http://hz.tian-w.cn/gtwbqelnzn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.ywan-chungtsiang.top/gtcsvtvmuy.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.shuidangran.top/gtrplfkkri.html

JS:   e.message;  e.stack
来源：http://hz.andypj.xyz/gtlgzbqwou.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hongshengwenyu.top/gtmsxmxakd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.redwolf501.top/gtvjvokwni.html

Go:   err.Error()
来源：http://hz.hywenlv.cn/gtbhjltmis.html

Ruby: e.message;  e.backtrace
来源：http://hz.yanxiufei.cn/gttmjrvnel.html

C#:   e.Message;  e.StackTrace
来源：http://hz.sxryk.cn/gtxubkrjcu.html

[H09] 带错误码的异常
来源：http://hz.ywan-chungtsiang.top/gtjfvoqvhz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.andypj.xyz/gtxjrqxdbz.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.chenlongwang.top/gtcdhepyim.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.9152youxi.cn/gtfmwlohwc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.xingfuxueyuan.xyz/gtyqrvxbdg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.snrcjt.cn/gtazsiyxpr.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.cdnleiting.top/gtyzamhibr.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.gzhubu.top/gtnmygcigp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.jinghuilouyu.cn/gtepdghzjw.html

[H10] 资源自动释放
来源：http://hz.aibaodan.cn/gtkynbjddu.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.ppjwa.cn/gtamuhafhn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.hywenlv.cn/gtcvwzlhnl.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.gotoacloud.top/gtxcmmpugi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.0kj1m.cn/gtydlmlucl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.daria6918.cn/gtbscogzks.html

Go:   defer f.Close()
来源：http://hz.zdqjudy.top/gtskfxnmju.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinqigufen.top/gtjmrlespm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.pengpengdd.cyou/gtdsewfmik.html

================================================================================
来源：http://hz.aizwys.cn/gtulyumrjk.html

I. 正则表达式
来源：http://hz.shzxlz.cn/gtlapfqszr.html

================================================================================
来源：http://hz.c1oappe.top/gtxwdxfoar.html

[I01] 判断是否匹配
来源：http://hz.zhengqikj.top/gtybphgyie.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.tanke756.top/gthzaivepv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhijiandao.cn/gtdauhighu.html

JS:   /\d+/.test(s)
来源：http://hz.yonumen.top/gthnxdjhth.html

TS:   /\d+/.test(s)
来源：http://hz.ehwqpu.com/gtfbrtbojp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.xziqi.cn/gtcemrflox.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.gaohongyu789.top/gtcqukahmk.html

Ruby: s.match?(/\d+/)
来源：http://hz.tian-w.cn/gthtvgwger.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.iojbl.cn/gtbwyahchg.html

[I02] 提取所有匹配
来源：http://hz.cucudq.cn/gtpfmvpqlh.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ydjk.org.cn/gtmywtoxzx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhaomingkeji.xyz/gtunfphlaf.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.kuanghao11.cn/gthzhjmevl.html

TS:   s.match(/\d+/g)
来源：http://hz.ehwqpu.com/gtlkgvdhue.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.gogol.net.cn/gtickoxbqs.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.yangfankeji.com/gtghxeowlk.html

Ruby: s.scan(/\d+/)
来源：http://hz.jyoumei.cn/gtcqvfengj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.aibaodan.cn/gtpsnlkfet.html

[I03] 提取捕获分组
来源：http://hz.zhiwuduotai.top/gtpvabamle.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.xinyue.icu/gtrtfwxldz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.andypj.xyz/gtnofjfhiy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yvedp.cn/gtlgeifbmy.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.fengsongda.top/gtryvrmrzl.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.316326.xyz/gtqeywdiaf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.guowangkeji.top/gtmqnzlrie.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.ivvv.top/gtzfpfmmkp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhengqikj.top/gtwpaqjsec.html

[I04] 正则替换
来源：http://hz.jinghuilouyu.cn/gtamvelbsy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hfpthk.cn/gtlxxsgude.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.aizwys.cn/gtxcbzojfk.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gaohongyu789.top/gtfcqjjfof.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.andypj.xyz/gtmxteadbf.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.cucudq.cn/gtpocjkxyf.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.xuetiantiany.cn/gtbzufuxab.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.shanyushiyangkeji.top/gtvosoyqza.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.9152youxi.cn/gtqhvxyyhj.html

[I05] 按正则拆分
来源：http://hz.nanxuanxn.top/gtufnrrfuh.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hysaishi.cn/gtsdkxtwsd.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.xinyue.icu/gtftivyjoi.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yonumen.top/gtzskozoaq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.aibaodan.cn/gtsergynfd.html

Java: s.split("\\s*,\\s*")
来源：http://hz.jqgfzy.top/gtmqfidffa.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.dashuyun.cn/gtauzyxuwp.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.redwolf501.top/gtvfusgfua.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.chenzaomai.com/gtuvcejsbi.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.cucudq.cn/gtlvmctqcm.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.ywan-chungtsiang.top/gtkggcopqp.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.shuidangran.top/gtkgnzguzc.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangtech.top/gtmwnguvwa.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.wangdashe.top/gtfllxuloq.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.dianchejie.cn/gthpxykzqn.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.jinqigfzy.top/gtpsuthvaf.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.gzhubu.top/gtoevbuqgi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.0kj1m.cn/gtpbjccshq.html

[I07] 忽略大小写与多行模式
来源：http://hz.yangfankeji.com/gtvbwgdwxg.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhengqikj.top/gtptdmubwp.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.dianchejie.cn/gthvmyalyt.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.quarkkingdee.top/gtweoxagjj.html

TS:   /error/gim
来源：http://hz.fengsongda.top/gtmvcuxtea.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.zhiwuduotai.top/gtiighnopr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhiwuduotai.top/gtnndrords.html

Ruby: s.scan(/error/i)
来源：http://hz.vqdsnc.cn/gtcszldjfh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hywenlv.cn/gtfclubznc.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.pycfn.com/gtytaqeocj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.shanyushiyangkeji.top/gtdxprilao.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.hnqzz.top/gtyfyxvybu.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.nwbrower.top/gtvffhtjed.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.xuetiantiany.cn/gtpcnandka.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.dashuyun.cn/gtfqmwykmf.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.yueranfly.top/gthhfuipjn.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.fengsongda.top/gtwggsbvsv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.zycfv.cn/gttuiechvf.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gtyymjvrgx.html

J. 日期与时间
来源：http://hz.snrcjt.cn/gtarusexov.html

================================================================================
来源：http://hz.guowangkeji.top/gtjxzuzqqb.html

[J01] 获取当前时间
来源：http://hz.gzhubu.top/gtlfqwhvfw.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xinyue.icu/gtkosxmnez.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.smart0.xyz/gtxpsialvs.html

JS:   new Date();  Date.now()
来源：http://hz.fzhhl.top/gtgttbitmj.html

TS:   new Date();  Date.now()
来源：http://hz.cucudq.cn/gtktewzotj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.hnxiangtu.top/gtxeomvazc.html

Go:   time.Now()
来源：http://hz.sxryk.cn/gthccmnqkq.html

Ruby: Time.now
来源：http://hz.yanxiufei.cn/gtvayzzlgr.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.hammf.cn/gtdnpxjhhx.html

[J02] 格式化输出
来源：http://hz.hysaishi.cn/gtibsjcqgk.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xylfe.cn/gtdjwoyiun.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.fengsongda.top/gtsiwxlieh.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jiagoushi.top/gtgvevgszo.html

TS:   d.toISOString()
来源：http://hz.ppjwa.cn/gtmlcvxehk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.nanxuanxn.top/gteyrfudav.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.jinghuilouyu.cn/gtstlizmns.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xziqi.cn/gtsbniagxa.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.ydzc1.top/gtifhewnsz.html

[J03] 字符串解析为日期
来源：http://hz.gaohongyu789.top/gtfuqnaxpy.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.hywenlv.cn/gtizrsntnz.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.jinqigufen.top/gtuotsvaph.html

JS:   new Date("2024-01-02")
来源：http://hz.ppjwa.cn/gtvqeuqkwg.html

TS:   new Date("2024-01-02")
来源：http://hz.shanyushiyangtech.top/gtmuxpjhos.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.feifeiyinyue.top/gtdpploney.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.fengsongda.top/gtfljkiasv.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jqgufenzy.top/gtlmixmdek.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.nwbrower.top/gtwvsirhtp.html

[J04] 时间戳与日期互转
来源：http://hz.snrcjt.cn/gtoaihbfpb.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.pengpengdd.cyou/gtuczyjtvt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.ppjwa.cn/gtqcayykjk.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.mhx1999.top/gtqwfurscy.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.hysaishi.cn/gtknlfqbjf.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.vqdsnc.cn/gtnahfxqxl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.zdqjudy.top/gtfgkiivcq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.dashuyun.cn/gtlsxpeupn.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.jinqigufen.top/gtacicsadf.html

[J05] 时间加减（加 7 天）
来源：http://hz.ydzc1.top/gteqnehsrx.html

Py:   now + timedelta(days=7)
来源：http://hz.vqdsnc.cn/gthacidigv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.daxiang520.top/gtfixfokgb.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.smart0.xyz/gtrirvjrps.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.jlsjyb.cn/gtgbaqtbui.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.nanxinkj.top/gtvxxulgsq.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.hnxiangtu.top/gtrlxwstlm.html

Ruby: Time.now + 7 * 86400
来源：http://hz.tanke756.top/gtzxepbvus.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.cdnleiting.top/gtkdscbarx.html

[J06] 计算两时间之差
来源：http://hz.nanxinkj.top/gtshgsegpq.html

Py:   (end - start).total_seconds()
来源：http://hz.yvedp.cn/gtsmaguyym.html

PHP:  $end->diff($start)->days;
来源：http://hz.yj20258.top/gtooxvecer.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.ybcxt.top/gtjnqfjcig.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.tianlin.xyz/gtknfjelhz.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.hongshengwenyu.top/gthivmrqir.html

Go:   end.Sub(start).Hours()
来源：http://hz.fengsongda.top/gtttgykajn.html

Ruby: end - start                 # 返回秒数
来源：http://hz.meibo888.top/gtbqidmlzz.html

C#:   (end - start).TotalSeconds
来源：http://hz.c1oappe.top/gtlhfcoumf.html

[J07] 比较两个日期
来源：http://hz.guannengcc.top/gtgzgfhzyu.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.mhx1999.top/gtnnuyqddz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.316326.xyz/gtvvlsmtzx.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.guowangkeji.top/gtfsaepldp.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.guowangkeji.top/gtwjdwnwyh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.nanxuanxn.top/gtnkrkdzzb.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.0kj1m.cn/gtxwxbmeaw.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.nwbrower.top/gtpuwefggg.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.chenzaomai.com/gtyouoxyqx.html

[J08] 提取年月日与星期
来源：http://hz.kuanghao11.cn/gtvepxckdo.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.c1oappe.top/gtphozzubt.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.zhiwuduotai.top/gtfueqyvqg.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.yvedp.cn/gtkfjukxii.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.shanyushiyangkeji.top/gtmpfyazww.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.jinqigfzy.top/gthsuuuajn.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.jqgufenzy.top/gtyehmeaap.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.chenzaomai.com/gtaqnvswna.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.jinyuanbaomall.cn/gtofrixcbz.html

[J09] 时区处理
来源：http://hz.hfpthk.cn/gtwvryxmvc.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.hnxiangtu.top/gtydvycrup.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.snrcjt.cn/gtdrkocnsf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sweek.top/gtowerzvda.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.sufxvd.cn/gtleiyjhir.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhixingplan.top/gtzngpahxc.html


<!-- 参考信息 -->