代发 wailian999

Ruby: attr_accessor :name
来源：http://hz.xinyue.icu/gtzpbbgcai.html

C#:   public string Name { get; set; }
来源：http://hz.jqgufenzy.top/gtgdpzdcae.html

[G12] 对象转字符串
来源：http://hz.tianlin.xyz/gtffelqvoh.html

Py:   def __str__(self): return self.name
来源：http://hz.tianlin.xyz/gtvlpuctog.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hongshengwenyu.top/gtzuydsktu.html

JS:   toString() { return this.name; }
来源：http://hz.quarkkingdee.top/gtkmehzjoh.html

TS:   toString(): string { return this.name; }
来源：http://hz.yanxiufei.cn/gtvafetbjt.html

Java: @Override public String toString() { return name; }
来源：http://hz.jlsjyb.cn/gtkttqmitc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jianghu66.top/gtyxoynrts.html

Ruby: def to_s; @name; end
来源：http://hz.hongshengwenyu.top/gtjthyoujh.html

C#:   public override string ToString() => Name;
来源：http://hz.chenjidiqi.icu/gtwvfbsoqc.html

[G13] 判断对象类型
来源：http://hz.zhixingplan.top/gtxgacarba.html

Py:   isinstance(u, User)
来源：http://hz.sxryk.cn/gtfugjaubn.html

PHP:  $u instanceof User
来源：http://hz.shzxlz.cn/gturuhcoha.html

JS:   u instanceof User
来源：http://hz.ydzc1.top/gtblfclxod.html

TS:   u instanceof User
来源：http://hz.hfpthk.cn/gtrltffsbr.html

Java: u instanceof User
来源：http://hz.vqdsnc.cn/gthhzdxcep.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jqgfzy.top/gtflyzunwd.html

Ruby: u.is_a?(User)
来源：http://hz.quarkkingdee.top/gtetzftqxo.html

C#:   u is User
来源：http://hz.yonumen.top/gtjievhvin.html

[G14] 数据类 / record
来源：http://hz.yangfankeji.com/gtxwyfqfsu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jiagoushi.top/gtwyilvogx.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.smart0.xyz/gtlkivqlxk.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.svipenyu.cn/gtcbracpdt.html

TS:   type User = { name: string; age: number };
来源：http://hz.tianlin.xyz/gtwbowsnhd.html

Java: record User(String name, int age) {}
来源：http://hz.sxryk.cn/gtalkazbup.html

Go:   type User struct { Name string; Age int }
来源：http://hz.feifeiyinyue.top/gtmgjynxva.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.jqgufenzy.top/gtfnyegixj.html

C#:   record User(string Name, int Age);
来源：http://hz.svipenyu.cn/gtqkuwxbgv.html

[G15] 枚举
来源：http://hz.hongshengwenyu.top/gtfajgxakm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yj202588.top/gtzqjektox.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.sxryk.cn/gtapzzgzkr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cheryme.top/gtedvofyzf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.meibo888.top/gtkdejwnwq.html

Java: enum Color { RED, GREEN }
来源：http://hz.tanke756.top/gtijhemtkx.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinyuanbaomall.cn/gtzvpzylls.html

Ruby: Color = %i[red green].freeze
来源：http://hz.cucudq.cn/gtiudzampw.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.shanyushiyangkeji.top/gtncelnzdt.html

[G16] 对象转数组 / 字典
来源：http://hz.andypj.xyz/gtrdrcpxcz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.cheryme.top/gtiilnujio.html

PHP:  get_object_vars($obj);
来源：http://hz.yuxming.cn/gtzrkedqpp.html

JS:   Object.entries(obj)
来源：http://hz.shanyushiyangtech.top/gtbdczxjyt.html

TS:   Object.entries(obj)
来源：http://hz.xziqi.cn/gtaurcozpt.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.haohaochexian.top/gtvcmytcuk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.daxiang520.top/gtjioncahl.html

Ruby: obj.instance_variables
来源：http://hz.yangfankeji.com/gtidrotezk.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.zhiwuduotai.top/gtgcjcjqjv.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtvhonhggp.html

H. 异常与错误处理
来源：http://hz.mhx1999.top/gtogetyaju.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtokhmpufa.html

[H01] try / catch 基础
来源：http://hz.yj20258888.top/gtavxxheil.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.zhengqikj.top/gtepzdeofi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.sysykeji.top/gtrgvckmyu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.pengpengdd.cyou/gtukgxrkby.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.haohaochexian.top/gtoqziotpb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.chenjidiqi.icu/gtbawlfqvj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.yongpay.top/gtfypfxgob.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.jinqigfzy.top/gtdrvwdhku.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.shangyingyoupin.top/gtoyjtuzoi.html

[H02] finally / ensure 收尾
来源：http://hz.ydjk.org.cn/gtbyfcpdaa.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.sysykeji.top/gtjrxuhcbe.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shanyushiyangtech.top/gtriakdbgr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.tanke756.top/gtszpgywov.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.hongshengwenyu.top/gtzzxqfskt.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.meibo888.top/gtuggqyigh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.zhoulong.xyz/gtlodbiejc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ybcxt.top/gtxjskwjus.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.xuanzx.com/gtnpxehofo.html

[H03] 主动抛出异常
来源：http://hz.jyoumei.cn/gtbhidqbyp.html

Py:   raise ValueError("错误信息")
来源：http://hz.ivvv.top/gtgqhdpjvk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yueranfly.top/gtsjtpxeoa.html

JS:   throw new Error("错误信息");
来源：http://hz.xingfuxueyuan.xyz/gtrvznnvpw.html

TS:   throw new Error("错误信息");
来源：http://hz.hnxiangtu.top/gturyvhusx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xylfe.cn/gtihdocetp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.c1oappe.top/gtyfqdotvw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.9152youxi.cn/gtdgelvdez.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.c1oappe.top/gtkaaznmqc.html

[H04] 自定义异常类型
来源：http://hz.nwbrower.top/gtlszxwbyg.html

Py:   class MyError(Exception): pass
来源：http://hz.shanyushiyangtech.top/gtsvofqajz.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.pycfn.com/gtjwuqchka.html

JS:   class MyError extends Error {}
来源：http://hz.zhengqikj.top/gtpypavtbk.html

TS:   class MyError extends Error {}
来源：http://hz.zycfv.cn/gtkzojqvyb.html

Java: class MyException extends RuntimeException {}
来源：http://hz.hywenlv.cn/gtgspifanv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.0kj1m.cn/gteopzlhzo.html

Ruby: class MyError < StandardError; end
来源：http://hz.shanyushiyangtech.top/gtommamauh.html

C#:   class MyException : Exception {}
来源：http://hz.jqgufenzy.top/gtonwrikgk.html

[H05] 捕获特定类型
来源：http://hz.zhoulong.xyz/gtukwxllpt.html

Py:   except ValueError as e:
来源：http://hz.sweek.top/gtiowpzdpt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.svipenyu.cn/gtcdhgatde.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.ehwqpu.com/gtvddxfkwu.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.snrcjt.cn/gtwoeutnvw.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.birdmap.top/gtnabbnjpy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.smart0.xyz/gtxravwntt.html

Ruby: rescue ArgumentError => e
来源：http://hz.hammf.cn/gtcmdsfxac.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.sysykeji.top/gtbofzndfm.html

[H06] 可选值 / 空值安全访问
来源：http://hz.svipenyu.cn/gtrtuilziw.html

Py:   value = d.get("k") or default
来源：http://hz.shangyingyoupin.top/gtvpuruhel.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.sxryk.cn/gtzfoqyvhl.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.chenlongwang.top/gtsceaxjbw.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jqgufenzy.top/gthxazcmng.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.316326.xyz/gthortjltq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.jqgufenzy.top/gtcoxyscqz.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jlsjyb.cn/gtfqsfibkh.html

C#:   obj?.A?.B ?? default
来源：http://hz.cucudq.cn/gtmoowgqat.html

[H07] 断言
来源：http://hz.xuanzx.com/gtslwzdpfl.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gogol.net.cn/gtnbsryhvt.html

PHP:  assert($x > 0);
来源：http://hz.9152youxi.cn/gtazstbsxs.html

JS:   console.assert(x > 0);
来源：http://hz.yj20258.top/gtatlfspyz.html

TS:   console.assert(x > 0);
来源：http://hz.dianchejie.cn/gtvtoggnwa.html

Java: assert x > 0 : "必须为正";
来源：http://hz.zhoulong.xyz/gtzduyyivw.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.daxiang520.top/gtwflemimf.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.dashuyun.cn/gtzydemerg.html

C#:   Debug.Assert(x > 0);
来源：http://hz.yvedp.cn/gtseboeayv.html

[H08] 获取错误信息与堆栈
来源：http://hz.tianlin.xyz/gtnuptfdgh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.yanxiufei.cn/gtqarkchsv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.xinyue.icu/gtzerjfccl.html

JS:   e.message;  e.stack
来源：http://hz.zhaomingkeji.xyz/gtmbhlvmxh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.pycfn.com/gtgjdoqtzd.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.zhijiandao.cn/gtryscpsua.html

Go:   err.Error()
来源：http://hz.xuetiantiany.cn/gtqzgmqedo.html

Ruby: e.message;  e.backtrace
来源：http://hz.ydjk.org.cn/gtqsqddsvo.html

C#:   e.Message;  e.StackTrace
来源：http://hz.yanxiufei.cn/gtbmnwhzwo.html

[H09] 带错误码的异常
来源：http://hz.ivvv.top/gtsqtiulwn.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.chenlongwang.top/gtrmifhbmk.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.jinghuilouyu.cn/gtntjxrouc.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hywenlv.cn/gtfllzxozc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhoulong.xyz/gtveaygwkv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yongpay.top/gtzyhxajtz.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.fengsongda.top/gtmjmnsnnw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.tanke756.top/gtuiznsigz.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.316326.xyz/gtbpdfzpib.html

[H10] 资源自动释放
来源：http://hz.xinyue.icu/gthtlnkpbj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.guannengcc.top/gtvknslaxb.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.jinqigfzy.top/gtmzjpdoai.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.sxryk.cn/gtjzchcjdf.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.hnqzz.top/gtqjypzsvx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.yj202588.top/gtxjqqbuaa.html

Go:   defer f.Close()
来源：http://hz.guannengcc.top/gtjepkqltq.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.shanyushiyangkeji.top/gtegwtjfti.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hfpthk.cn/gtrtuvzzkt.html

================================================================================
来源：http://hz.daxiang520.top/gtlxnjhqlm.html

I. 正则表达式
来源：http://hz.hammf.cn/gtabyujjng.html

================================================================================
来源：http://hz.yangfankeji.com/gtelqdrqem.html

[I01] 判断是否匹配
来源：http://hz.ydzc1.top/gtkqhkmtiy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.c1oappe.top/gtdvhtwtuy.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.zhijiandao.cn/gtnhxoouug.html

JS:   /\d+/.test(s)
来源：http://hz.guannengcc.top/gtkmqdrkqh.html

TS:   /\d+/.test(s)
来源：http://hz.guannengcc.top/gtfzmwzhme.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.c1oappe.top/gtmcjqhobl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jyoumei.cn/gtamgghniu.html

Ruby: s.match?(/\d+/)
来源：http://hz.ywan-chungtsiang.top/gthzhymscy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinyuanbaomall.cn/gtxxoiuzec.html

[I02] 提取所有匹配
来源：http://hz.jianghu66.top/gtnautotbs.html

Py:   re.findall(r"\d+", s)
来源：http://hz.yongpay.top/gtfdheezeq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.zhixingplan.top/gtwswsqnei.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.gzhubu.top/gttbjbsbrl.html

TS:   s.match(/\d+/g)
来源：http://hz.zhiwuduotai.top/gtmbgbfcjb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.aibaodan.cn/gtyewjlceq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.guannengcc.top/gtldsqttqo.html

Ruby: s.scan(/\d+/)
来源：http://hz.yuanzhike.top/gthwmhumov.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.ppjwa.cn/gtmqmrfwrn.html

[I03] 提取捕获分组
来源：http://hz.wangshuangyany.cn/gterkzecpy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yuxming.cn/gtxiezqluf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.chenlongwang.top/gttwwiijps.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.sufxvd.cn/gtknmyxevk.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.fzhhl.top/gtfdqdcgqu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.c1oappe.top/gthwbvczuh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.havefunace.top/gtsujpfdrj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.zhoulong.xyz/gtpaqgftss.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.wangdashe.top/gtxzgqvglh.html

[I04] 正则替换
来源：http://hz.tanke756.top/gtsjudfjve.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.svipenyu.cn/gtxtzcnigc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.havefunace.top/gtfwdsmfqy.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.wangdashe.top/gtmzbxudla.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.svipenyu.cn/gtrrjdekve.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.quarkkingdee.top/gtsxdjkdev.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.dianchejie.cn/gtszjaslve.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.fengsongda.top/gtdyijjaly.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yongpay.top/gtsdoonpsn.html

[I05] 按正则拆分
来源：http://hz.jyoumei.cn/gtulekhpws.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.cucudq.cn/gtitupiyym.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.bjfxy.top/gtilhrrawu.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.sysykeji.top/gtdihzasby.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.havefunace.top/gtweumxahc.html

Java: s.split("\\s*,\\s*")
来源：http://hz.tianlin.xyz/gtmdxxnxdy.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.yanxiufei.cn/gtzmqpgemt.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.yj20258888.top/gtharacuta.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.chenjidiqi.icu/gtnlwouqqu.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hnxiangtu.top/gtebxporlo.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.tian-w.cn/gterkzmsoc.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yvedp.cn/gtvgdskpso.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hongshengwenyu.top/gtgxrdlaxx.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.yj202588.top/gtvsrhftzo.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.tanke756.top/gtyvnkhvzy.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.pycfn.com/gtowwwispr.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.sysykeji.top/gtkdlbbhxn.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.guowangkeji.top/gtyscxbgwn.html

[I07] 忽略大小写与多行模式
来源：http://hz.hnqzz.top/gtulspgipd.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shanyushiyangkeji.top/gtqxzspgjx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.tian-w.cn/gttgixkaiw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.9152youxi.cn/gtfkzpwvko.html

TS:   /error/gim
来源：http://hz.hnxiangtu.top/gtkxeuiojm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.jiagoushi.top/gtnrupvwaz.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.gogol.net.cn/gtdonfxemv.html

Ruby: s.scan(/error/i)
来源：http://hz.cdnleiting.top/gtapjgospq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.zhengqikj.top/gtgzxnavnz.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.ydzc1.top/gttndhflbj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.mhx1999.top/gtyeyqjkuh.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.tanke756.top/gtdquxhrlo.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.fzhhl.top/gtzizhwiwa.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zhiwuduotai.top/gtesdeuwfp.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.sufxvd.cn/gtgzsrbanb.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cdnleiting.top/gtbefhczdz.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.nanxinkj.top/gticyhgcdw.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.xinyue.icu/gtijqzutda.html

================================================================================
来源：http://hz.aizwys.cn/gtvkitraoo.html

J. 日期与时间
来源：http://hz.pycfn.com/gtswzpsvjj.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtckprmwrl.html

[J01] 获取当前时间
来源：http://hz.zhoulong.xyz/gtyasqbnbd.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.birdmap.top/gtxbpevrdw.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jyoumei.cn/gtntwokscd.html

JS:   new Date();  Date.now()
来源：http://hz.smart0.xyz/gtsafzkabc.html

TS:   new Date();  Date.now()
来源：http://hz.yuxming.cn/gtgsyjirrj.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.feifeiyinyue.top/gtpwafcfkh.html

Go:   time.Now()
来源：http://hz.ehwqpu.com/gtkydqhcnw.html

Ruby: Time.now
来源：http://hz.jiagoushi.top/gtbvgykbyi.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.shanyushiyangkeji.top/gtdtrvbhzz.html

[J02] 格式化输出
来源：http://hz.yj20258888.top/gtggmevlku.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gogol.net.cn/gtbnufukfz.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.yonumen.top/gtwrcacalq.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.gzhubu.top/gtemofwwdu.html

TS:   d.toISOString()
来源：http://hz.sufxvd.cn/gtmvopzhdu.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.chenlongwang.top/gtmwbmdprj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yangfankeji.com/gtzmtlsvck.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cdnleiting.top/gtoptdynmv.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gaohongyu789.top/gtdegilcqk.html

[J03] 字符串解析为日期
来源：http://hz.tanke756.top/gthptigvcu.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.shanyushiyangtech.top/gtejjyxjmv.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.snrcjt.cn/gtwxstlntv.html

JS:   new Date("2024-01-02")
来源：http://hz.nwbrower.top/gtkpfxssna.html

TS:   new Date("2024-01-02")
来源：http://hz.hywenlv.cn/gtxjogbizn.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.hongshengwenyu.top/gtodegouvm.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.shanyushiyangkeji.top/gtdzylkixs.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.cucudq.cn/gthqrlhgwj.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.hysaishi.cn/gtbstfptpc.html

[J04] 时间戳与日期互转
来源：http://hz.yuxming.cn/gtxlhoquqs.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.sufxvd.cn/gtyiprnshc.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.gogol.net.cn/gtzkvqevym.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.tanke756.top/gtbpnpmvus.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.daxiang520.top/gtromusjsj.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ydzc1.top/gtcmjgmhsv.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.gzhubu.top/gtulheyscj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.svipenyu.cn/gtrklmqqij.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.yongpay.top/gtixiwkmsx.html

[J05] 时间加减（加 7 天）
来源：http://hz.yongpay.top/gtbqayrnxv.html

Py:   now + timedelta(days=7)
来源：http://hz.hywenlv.cn/gtircnhwhz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.yuanzhike.top/gtahyuugnv.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zhiwuduotai.top/gtbcswylpz.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.ehwqpu.com/gtqhumxheb.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.dashuyun.cn/gtqavkufno.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.feifeiyinyue.top/gtsjqzyqza.html

Ruby: Time.now + 7 * 86400
来源：http://hz.yanxiufei.cn/gthnaxryvx.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xuetiantiany.cn/gteymspnak.html

[J06] 计算两时间之差
来源：http://hz.jqgfzy.top/gtzxynfdtb.html

Py:   (end - start).total_seconds()
来源：http://hz.zhijiandao.cn/gtqubrvhun.html

PHP:  $end->diff($start)->days;
来源：http://hz.0kj1m.cn/gtcjdzotyr.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.jyoumei.cn/gtbbeoxyvk.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sweek.top/gtdrmvbrog.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.iojbl.cn/gtlswprylq.html

Go:   end.Sub(start).Hours()
来源：http://hz.guannengcc.top/gthpyoxpqp.html

Ruby: end - start                 # 返回秒数
来源：http://hz.nanxuanxn.top/gtivwrbkyq.html

C#:   (end - start).TotalSeconds
来源：http://hz.daxiang520.top/gtbwjratfo.html

[J07] 比较两个日期
来源：http://hz.daxiang520.top/gtlybrkiup.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ywan-chungtsiang.top/gtllbwfine.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.chenjidiqi.icu/gtqayrjkap.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hammf.cn/gthbkzuybu.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.wangdashe.top/gtcnplqqfz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.mhx1999.top/gtqjhpuzby.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.sxryk.cn/gtynumezii.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.gaohongyu789.top/gtgiweczue.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.jianghu66.top/gtrwczutts.html

[J08] 提取年月日与星期
来源：http://hz.nanxuanxn.top/gtcinzydhk.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.zdqjudy.top/gtwqguntbo.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.cdnleiting.top/gtklysapdp.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.jqgfzy.top/gtzfgekdzk.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.yvedp.cn/gtjrqjkdyk.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.havefunace.top/gtauuckuel.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.xziqi.cn/gtilmmncox.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.zhiwuduotai.top/gtmggsepkd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.kuanghao11.cn/gtksvubyrg.html

[J09] 时区处理
来源：http://hz.guowangkeji.top/gtsjcxnlog.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.dashuyun.cn/gtgtscwuau.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://hz.shanyushiyangtech.top/gteubvafqt.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.xingfuxueyuan.xyz/gtsnnjwjxo.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hz.wangdashe.top/gtzgfegxcc.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://hz.zhijiandao.cn/gtbccznqoi.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://hz.zhixingplan.top/gtdvbtxese.html

Ruby: Time.now.getlocal("+08:00")
来源：http://hz.yonumen.top/gtzkirvina.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://hz.ydzc1.top/gtaymuhjqn.html

[J10] 取今天 / 本月第一天
来源：http://hz.hnxiangtu.top/gtahjfmbya.html


<!-- 参考信息 -->