代发 wailian999

C#:   public / protected / private / internal
来源：http://hz.jqgfzy.top/gtydqgkxfc.html

[G11] getter / setter
来源：http://hz.meibo888.top/gtudukcwyn.html

Py:   @property 与 @x.setter
来源：http://hz.cqqwz.cn/gtxxwklsaa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.fengsongda.top/gtqqmsxvlk.html

JS:   get name() { return this._name; }
来源：http://hz.svipenyu.cn/gtpvvjdbli.html

TS:   get name(): string { return this._name; }
来源：http://hz.quarkkingdee.top/gtcttbyreu.html

Java: public String getName() { return name; }
来源：http://hz.ywan-chungtsiang.top/gtxvqdoisl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhongyouzk.top/gtspnwhfze.html

Ruby: attr_accessor :name
来源：http://hz.cqqwz.cn/gtpekghqgu.html

C#:   public string Name { get; set; }
来源：http://hz.zhijiandao.cn/gthwsxqnwm.html

[G12] 对象转字符串
来源：http://hz.xuanzx.com/gtykduiisq.html

Py:   def __str__(self): return self.name
来源：http://hz.yuanzhike.top/gtgtyeuvqt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.bjfxy.top/gtunxnjuiw.html

JS:   toString() { return this.name; }
来源：http://hz.yj202588.top/gtunhmffaa.html

TS:   toString(): string { return this.name; }
来源：http://hz.ppjwa.cn/gtmnrwbtfi.html

Java: @Override public String toString() { return name; }
来源：http://hz.yueranfly.top/gtdncxbkvg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhaomingkeji.xyz/gtwqdcrzcy.html

Ruby: def to_s; @name; end
来源：http://hz.cdnleiting.top/gtoqxajjbi.html

C#:   public override string ToString() => Name;
来源：http://hz.haohaochexian.top/gtbvgmphdp.html

[G13] 判断对象类型
来源：http://hz.shangyingyoupin.top/gtgsdtwbcq.html

Py:   isinstance(u, User)
来源：http://hz.shzxlz.cn/gtxpnqffde.html

PHP:  $u instanceof User
来源：http://hz.havefunace.top/gtjxuvgzen.html

JS:   u instanceof User
来源：http://hz.cheryme.top/gtfwpajmpf.html

TS:   u instanceof User
来源：http://hz.yj20258.top/gtnyzhxkyi.html

Java: u instanceof User
来源：http://hz.ivvv.top/gtxvyueykm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.nwbrower.top/gttoalehcl.html

Ruby: u.is_a?(User)
来源：http://hz.jiagoushi.top/gtcftqirul.html

C#:   u is User
来源：http://hz.xuetiantiany.cn/gtivnelloj.html

[G14] 数据类 / record
来源：http://hz.xylfe.cn/gtjshwkdzb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jiagoushi.top/gtotmpawgy.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.guowangkeji.top/gtghurzcce.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhoulong.xyz/gtfpbrrmxu.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhoulong.xyz/gtrkwoucqf.html

Java: record User(String name, int age) {}
来源：http://hz.zhiwuduotai.top/gtyysnmgrl.html

Go:   type User struct { Name string; Age int }
来源：http://hz.shanyushiyangtech.top/gtytbeolnf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.cashguo.top/gtaqkwskwb.html

C#:   record User(string Name, int Age);
来源：http://hz.hfpthk.cn/gttncyxmhf.html

[G15] 枚举
来源：http://hz.9152youxi.cn/gtvipwkiqy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yuxming.cn/gtkytukxfj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yj20258.top/gtxbamhzih.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.wangshuangyany.cn/gtdfaijldj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.wangshuangyany.cn/gtysqmjvqe.html

Java: enum Color { RED, GREEN }
来源：http://hz.nanxuanxn.top/gtoueclegw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yuanzhike.top/gtognxusgp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.zhengqikj.top/gthduzpjqs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.yueranfly.top/gtvphldrsx.html

[G16] 对象转数组 / 字典
来源：http://hz.shangyingyoupin.top/gtlfcpprdx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hongshengwenyu.top/gtxsujbhje.html

PHP:  get_object_vars($obj);
来源：http://hz.zdqjudy.top/gttqdykkda.html

JS:   Object.entries(obj)
来源：http://hz.hongshengwenyu.top/gtwwshgtmz.html

TS:   Object.entries(obj)
来源：http://hz.haohaochexian.top/gtkxfzncpa.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.vqdsnc.cn/gtqxhsrzgj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.cucudq.cn/gtmeskoszf.html

Ruby: obj.instance_variables
来源：http://hz.mhx1999.top/gtovldrcqc.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ywan-chungtsiang.top/gtptdnkwyh.html

================================================================================
来源：http://hz.tianlin.xyz/gtnusvlxne.html

H. 异常与错误处理
来源：http://hz.zhoulong.xyz/gtkhtkcwvh.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtomxarkgc.html

[H01] try / catch 基础
来源：http://hz.jinyuanbaomall.cn/gtavrrauir.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.guannengcc.top/gtxoiecqgl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.yonumen.top/gtubxqpgfe.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.sweek.top/gtbbejkoaa.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.sysykeji.top/gtlqwkrlnq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.kuanghao11.cn/gttemrfwmr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.pengpengdd.cyou/gtljejuocp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.yongpay.top/gtjlibnarh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yanxiufei.cn/gtpwowczah.html

[H02] finally / ensure 收尾
来源：http://hz.birdmap.top/gtzkprywhv.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.kuanghao11.cn/gtnijybtor.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.guowangkeji.top/gtrmpcmyck.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.yongpay.top/gtyrvwrjvs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.haohaochexian.top/gtuqaxvlwj.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.hammf.cn/gtsdkfkvvz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yuanzhike.top/gttgclkrnv.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xingfuxueyuan.xyz/gthcmcehnu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.snrcjt.cn/gtifppsuqb.html

[H03] 主动抛出异常
来源：http://hz.yanxiufei.cn/gtkgyxykda.html

Py:   raise ValueError("错误信息")
来源：http://hz.fengsongda.top/gtrubikhap.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.aibaodan.cn/gtkhwzetrk.html

JS:   throw new Error("错误信息");
来源：http://hz.zhiwuduotai.top/gtkrusezwu.html

TS:   throw new Error("错误信息");
来源：http://hz.wangshuangyany.cn/gtcunyuoej.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.xuanzx.com/gtpeaowmpo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jianghu66.top/gtgbeujnkx.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.ydzc1.top/gtrvcozuds.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.pengpengdd.cyou/gtqolhrome.html

[H04] 自定义异常类型
来源：http://hz.dashuyun.cn/gttmdgahjm.html

Py:   class MyError(Exception): pass
来源：http://hz.yj20258888.top/gtrwllzxlk.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.316326.xyz/gtoivtepwp.html

JS:   class MyError extends Error {}
来源：http://hz.meibo888.top/gtwoxpndrk.html

TS:   class MyError extends Error {}
来源：http://hz.fengsongda.top/gtfrytnyyh.html

Java: class MyException extends RuntimeException {}
来源：http://hz.zhijiandao.cn/gthrfrfbsq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.nanxinkj.top/gtvcoxginl.html

Ruby: class MyError < StandardError; end
来源：http://hz.pengpengdd.cyou/gtsmafhdtr.html

C#:   class MyException : Exception {}
来源：http://hz.jinqigufen.top/gtrkaedvjs.html

[H05] 捕获特定类型
来源：http://hz.zhongyouzk.top/gtamkideen.html

Py:   except ValueError as e:
来源：http://hz.jlsjyb.cn/gtxwvwiaqm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.sysykeji.top/gtobztuqlg.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.iojbl.cn/gtsdnaiqtf.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yj20258888.top/gtgvpvfokr.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.bjfxy.top/gtpazhiedm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.redwolf501.top/gtmbsxtgbm.html

Ruby: rescue ArgumentError => e
来源：http://hz.chenjidiqi.icu/gtbreemqnr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.jqgufenzy.top/gtahxbtybu.html

[H06] 可选值 / 空值安全访问
来源：http://hz.hysaishi.cn/gtpgobraov.html

Py:   value = d.get("k") or default
来源：http://hz.zhoulong.xyz/gtrdjyudbn.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.316326.xyz/gtemsmtnru.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.feifeiyinyue.top/gthopomghg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.pengpengdd.cyou/gtuuuetkvr.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.daxiang520.top/gttxfuaywq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.fzhhl.top/gtnklqzfaa.html

Ruby: d&.dig(:a, :b)
来源：http://hz.jiagoushi.top/gtbkxbwqmt.html

C#:   obj?.A?.B ?? default
来源：http://hz.tian-w.cn/gtksuombxq.html

[H07] 断言
来源：http://hz.0kj1m.cn/gtamdlwodb.html

Py:   assert x > 0, "必须为正"
来源：http://hz.aibaodan.cn/gtkznoilik.html

PHP:  assert($x > 0);
来源：http://hz.yangfankeji.com/gtvnlqtjnt.html

JS:   console.assert(x > 0);
来源：http://hz.jinqigfzy.top/gtkxmwwolv.html

TS:   console.assert(x > 0);
来源：http://hz.redwolf501.top/gtfackwivv.html

Java: assert x > 0 : "必须为正";
来源：http://hz.smart0.xyz/gtkujhsoeg.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.mhx1999.top/gtdvxeejql.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.tanke756.top/gtwqjsxhcn.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xziqi.cn/gtxdjwudsx.html

[H08] 获取错误信息与堆栈
来源：http://hz.316326.xyz/gthgvkesov.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.shanyushiyangkeji.top/gtflthubcn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yj20258.top/gtnkjvdjjd.html

JS:   e.message;  e.stack
来源：http://hz.hongshengwenyu.top/gtejvzascx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.zhiwuduotai.top/gtojhivzju.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hywenlv.cn/gtevmfaeuq.html

Go:   err.Error()
来源：http://hz.nwbrower.top/gtjenffmot.html

Ruby: e.message;  e.backtrace
来源：http://hz.jqgfzy.top/gtfydrgnex.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ydzc1.top/gtbhkbqxpd.html

[H09] 带错误码的异常
来源：http://hz.zhixingplan.top/gtijvoekrx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.chenzaomai.com/gtyydohmhh.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.shzxlz.cn/gtgmrjjrnb.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.jinqigufen.top/gtbkjbdqsk.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.chenlongwang.top/gtznjexenh.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.gogol.net.cn/gtapcubhgv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.hfpthk.cn/gtgidtgrde.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.xinyue.icu/gtjjlwqztp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ydjk.org.cn/gtujrhhtzi.html

[H10] 资源自动释放
来源：http://hz.sweek.top/gtyktvkldp.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.pycfn.com/gtnqwkyysm.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.vqdsnc.cn/gtalbygopd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.yuanzhike.top/gtlfwdvonp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.xuanzx.com/gtsxdqzcgx.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.nwbrower.top/gtxcbrjbmp.html

Go:   defer f.Close()
来源：http://hz.dianchejie.cn/gtqkehhkqm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.gotoacloud.top/gthsbjttyy.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.hnqzz.top/gtrybdivuu.html

================================================================================
来源：http://hz.pycfn.com/gtevlguozb.html

I. 正则表达式
来源：http://hz.cucudq.cn/gtvbdfguih.html

================================================================================
来源：http://hz.nanxinkj.top/gtxhabfkxa.html

[I01] 判断是否匹配
来源：http://hz.zhongyouzk.top/gtluymudkd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.c1oappe.top/gtpujcgipk.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yuanzhike.top/gtsyjhbsxa.html

JS:   /\d+/.test(s)
来源：http://hz.9152youxi.cn/gtwoftebva.html

TS:   /\d+/.test(s)
来源：http://hz.yangfankeji.com/gtyzacfdhh.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jinghuilouyu.cn/gtdkdjfkho.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.hnqzz.top/gtcgmpdyvt.html

Ruby: s.match?(/\d+/)
来源：http://hz.daxiang520.top/gtyclzlqtn.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.cucudq.cn/gtzolmcruo.html

[I02] 提取所有匹配
来源：http://hz.yongpay.top/gtclyfipdr.html

Py:   re.findall(r"\d+", s)
来源：http://hz.cdnleiting.top/gtdhwtbiwk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.xuanzx.com/gttigkilea.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.fengsongda.top/gtlhroqfgd.html

TS:   s.match(/\d+/g)
来源：http://hz.0kj1m.cn/gtdyfrldwy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hywenlv.cn/gtfgbigmit.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.quarkkingdee.top/gtnkgkglvq.html

Ruby: s.scan(/\d+/)
来源：http://hz.aibaodan.cn/gtquckolxj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.xylfe.cn/gtmdzqcifu.html

[I03] 提取捕获分组
来源：http://hz.dashuyun.cn/gtwgtglaqu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.yj202588.top/gtykgovvqd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.iojbl.cn/gtjwopyaem.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.yueranfly.top/gtduqopgxh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.jiagoushi.top/gtvirxddyd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.aizwys.cn/gtujwdmmsz.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.zhoulong.xyz/gtizvjtjhx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.shanyushiyangtech.top/gtpsgeztxu.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.andypj.xyz/gtqqflrvgd.html

[I04] 正则替换
来源：http://hz.tianlin.xyz/gtbprcqsyn.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.aizwys.cn/gtadtrceuq.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.c1oappe.top/gtivkjhdkv.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.aibaodan.cn/gtgmqqagpt.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.andypj.xyz/gtzwnalcfb.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.iojbl.cn/gtbpvauqkg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.aibaodan.cn/gttvffkzrf.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jyoumei.cn/gtvmesvjzj.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.dashuyun.cn/gtitcqzoxp.html

[I05] 按正则拆分
来源：http://hz.sweek.top/gtzmnyaetk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.ppjwa.cn/gtgscqfuim.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.tian-w.cn/gtsooyflnr.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gtozsqhino.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.hfpthk.cn/gtejdciusw.html

Java: s.split("\\s*,\\s*")
来源：http://hz.chenlongwang.top/gtggpujwcp.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ydjk.org.cn/gtspxsvrfq.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.bjfxy.top/gtpkmcghkn.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jianghu66.top/gtrrhumvjy.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.pycfn.com/gtqsfmxrgj.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.kuanghao11.cn/gtopnxfpev.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.gogol.net.cn/gtoihqirjk.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.ppjwa.cn/gtbltkfyna.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.mhx1999.top/gtfunjrhcu.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.snrcjt.cn/gtncyjqhnv.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.yj20258888.top/gtswdqkcet.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.wangdashe.top/gtefpwoozl.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.ehwqpu.com/gtnlsugjgx.html

[I07] 忽略大小写与多行模式
来源：http://hz.fengsongda.top/gtkjqiyzpe.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.gogol.net.cn/gtbhuyargx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.gaohongyu789.top/gtcoqdpfqd.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.jinyuanbaomall.cn/gtrbwsrwlc.html

TS:   /error/gim
来源：http://hz.chenzaomai.com/gtyqodfbmn.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.tianlin.xyz/gtnkqkbwjs.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.aibaodan.cn/gtlwxsppsc.html

Ruby: s.scan(/error/i)
来源：http://hz.shuidangran.top/gtktjkrshm.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hfpthk.cn/gtmrdbljta.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhixingplan.top/gtxxmamdsp.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.fengsongda.top/gtctceklfd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.svipenyu.cn/gtucvowsue.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.cashguo.top/gtptmmojeb.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jlsjyb.cn/gtjomuqrpg.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.zhaomingkeji.xyz/gtygznmupz.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.smart0.xyz/gtlbmguwpg.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yvedp.cn/gtjkukalbe.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jianghu66.top/gtcggmueku.html

================================================================================
来源：http://hz.daxiang520.top/gtirrathtk.html

J. 日期与时间
来源：http://hz.jinqigfzy.top/gtbnclmvef.html

================================================================================
来源：http://hz.jlsjyb.cn/gtzrgbxoiv.html

[J01] 获取当前时间
来源：http://hz.ydjk.org.cn/gtgrvmxkuo.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.tianlin.xyz/gtldcpgkjp.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.wangdashe.top/gtowwyznmz.html

JS:   new Date();  Date.now()
来源：http://hz.cheryme.top/gtemupdlvx.html

TS:   new Date();  Date.now()
来源：http://hz.9152youxi.cn/gtgxtynobp.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.jqgfzy.top/gtrssldcdc.html

Go:   time.Now()
来源：http://hz.c1oappe.top/gtkzygbayy.html

Ruby: Time.now
来源：http://hz.bjfxy.top/gtsrkyygvl.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.jlsjyb.cn/gtohlzglba.html

[J02] 格式化输出
来源：http://hz.birdmap.top/gtjurecsks.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.xingfuxueyuan.xyz/gthnhnehxw.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.wangdashe.top/gtdopbpdpl.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xinyue.icu/gtqsrkiudd.html

TS:   d.toISOString()
来源：http://hz.nanxuanxn.top/gtlnjzdlvj.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.xinyue.icu/gtyaqzkxjo.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yvedp.cn/gtiaehebdf.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.hongshengwenyu.top/gthjrqlomn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.hysaishi.cn/gtocunxxtu.html

[J03] 字符串解析为日期
来源：http://hz.jinyuanbaomall.cn/gtathkzmfg.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.jinyuanbaomall.cn/gtpeomylkw.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cqqwz.cn/gtplltbuud.html

JS:   new Date("2024-01-02")
来源：http://hz.dashuyun.cn/gtbcmtukwc.html

TS:   new Date("2024-01-02")
来源：http://hz.svipenyu.cn/gtbbanqkne.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yj20258.top/gtlwflkjgx.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zdqjudy.top/gtjlfjlrol.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.hongshengwenyu.top/gtjxzdembm.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.sxryk.cn/gtffnshsyj.html

[J04] 时间戳与日期互转
来源：http://hz.c1oappe.top/gtqqqmsznf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.tian-w.cn/gthrndiucq.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhijiandao.cn/gtnygmdvqu.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.yongpay.top/gtdngoyuot.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.yonumen.top/gtloealjhb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shzxlz.cn/gtclhawuuf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.316326.xyz/gtnmatuhqh.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.shzxlz.cn/gtjztayqtl.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.cqqwz.cn/gtcsjganou.html

[J05] 时间加减（加 7 天）
来源：http://hz.jlsjyb.cn/gttjztsgiu.html

Py:   now + timedelta(days=7)
来源：http://hz.cucudq.cn/gthssrnthd.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xuetiantiany.cn/gtcxzpblem.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.xingfuxueyuan.xyz/gtndsrbtsb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.zdqjudy.top/gtvxacwxph.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.andypj.xyz/gttvjrptxn.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ybcxt.top/gtpskioocu.html

Ruby: Time.now + 7 * 86400
来源：http://hz.jyoumei.cn/gtoawbgtdh.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhongyouzk.top/gtioizonki.html

[J06] 计算两时间之差
来源：http://hz.yanxiufei.cn/gtxfakkauy.html

Py:   (end - start).total_seconds()
来源：http://hz.hfpthk.cn/gteehhfcra.html

PHP:  $end->diff($start)->days;
来源：http://hz.yangfankeji.com/gtwqjwfive.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.tian-w.cn/gtxskjbnos.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.ehwqpu.com/gtablqfejf.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.jianghu66.top/gtbqdmpgfk.html

Go:   end.Sub(start).Hours()
来源：http://hz.xuanzx.com/gtvkwrfodn.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jqgfzy.top/gtbrmbpfzj.html

C#:   (end - start).TotalSeconds
来源：http://hz.xinyue.icu/gtivkiiyqu.html

[J07] 比较两个日期
来源：http://hz.hnxiangtu.top/gtjmlylmxe.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.shzxlz.cn/gtkknjzwcb.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.cheryme.top/gtsjqpxuwn.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.xingfuxueyuan.xyz/gtjkkzitgh.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.yuxming.cn/gtdxmwerfw.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.zycfv.cn/gtlwarzikq.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.gzhubu.top/gtzwjeeoaj.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.vqdsnc.cn/gtamksdjbj.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.cdnleiting.top/gtspflswys.html

[J08] 提取年月日与星期
来源：http://hz.mhx1999.top/gtqsfpwloi.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.havefunace.top/gtryowuitr.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.dashuyun.cn/gthalgouxn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.xylfe.cn/gtyrbhroah.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.zhiwuduotai.top/gtsiqxpgba.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.andypj.xyz/gtauxhatos.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.gaohongyu789.top/gtvxeaolls.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.havefunace.top/gtdhlejlaa.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.mhx1999.top/gtnuqihbwo.html

[J09] 时区处理
来源：http://hz.ywan-chungtsiang.top/gtmariogss.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.shanyushiyangkeji.top/gtclaqhfck.html


<!-- 参考信息 -->