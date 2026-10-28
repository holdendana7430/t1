代发 wailian999

C#:   public / protected / private / internal
来源：http://hz.tianlin.xyz/gtkcjtgtxx.html

[G11] getter / setter
来源：http://hz.yonumen.top/gtinplcgbo.html

Py:   @property 与 @x.setter
来源：http://hz.ehwqpu.com/gtiseicuyf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gtwpzkrtgh.html

JS:   get name() { return this._name; }
来源：http://hz.xinyue.icu/gtmfooazdv.html

TS:   get name(): string { return this._name; }
来源：http://hz.cdnleiting.top/gtihbueylo.html

Java: public String getName() { return name; }
来源：http://hz.shanyushiyangtech.top/gtaxdrisxo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jianghu66.top/gthzwgzgkz.html

Ruby: attr_accessor :name
来源：http://hz.vqdsnc.cn/gtatmynoie.html

C#:   public string Name { get; set; }
来源：http://hz.hammf.cn/gtnjwuzyxb.html

[G12] 对象转字符串
来源：http://hz.yj202588.top/gtsaqpsfky.html

Py:   def __str__(self): return self.name
来源：http://hz.cucudq.cn/gtlrxfzfwx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cashguo.top/gtgcycnnqo.html

JS:   toString() { return this.name; }
来源：http://hz.xylfe.cn/gtefdyiwqx.html

TS:   toString(): string { return this.name; }
来源：http://hz.hywenlv.cn/gtaksnuoon.html

Java: @Override public String toString() { return name; }
来源：http://hz.snrcjt.cn/gtonxzsrbw.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.zhaomingkeji.xyz/gtixeroklw.html

Ruby: def to_s; @name; end
来源：http://hz.jyoumei.cn/gtaewfdmsq.html

C#:   public override string ToString() => Name;
来源：http://hz.zhongyouzk.top/gtoepbknym.html

[G13] 判断对象类型
来源：http://hz.0kj1m.cn/gtexierxip.html

Py:   isinstance(u, User)
来源：http://hz.hywenlv.cn/gtoixjjvtw.html

PHP:  $u instanceof User
来源：http://hz.sysykeji.top/gtjxcvzhqf.html

JS:   u instanceof User
来源：http://hz.pycfn.com/gtnofnjkwh.html

TS:   u instanceof User
来源：http://hz.cheryme.top/gtxtkqyhox.html

Java: u instanceof User
来源：http://hz.jinyuanbaomall.cn/gtffictcie.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jqgufenzy.top/gthakmgwaf.html

Ruby: u.is_a?(User)
来源：http://hz.yj20258.top/gtamtiwivj.html

C#:   u is User
来源：http://hz.redwolf501.top/gtvjquyand.html

[G14] 数据类 / record
来源：http://hz.vqdsnc.cn/gtiohgobjj.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.guannengcc.top/gtgzoowzrt.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ydjk.org.cn/gtbsnclewk.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.zhongyouzk.top/gtvjgrepip.html

TS:   type User = { name: string; age: number };
来源：http://hz.yueranfly.top/gtsktriyci.html

Java: record User(String name, int age) {}
来源：http://hz.shuidangran.top/gtkiaoibqu.html

Go:   type User struct { Name string; Age int }
来源：http://hz.ehwqpu.com/gtupmhhhtz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.hfpthk.cn/gtznxgzvgc.html

C#:   record User(string Name, int Age);
来源：http://hz.jinyuanbaomall.cn/gtyuepwhkp.html

[G15] 枚举
来源：http://hz.sysykeji.top/gtxigratyp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.yj20258888.top/gtyssrggul.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yuxming.cn/gtnyqwbjmo.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.cheryme.top/gtkgyhthhk.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.dashuyun.cn/gtnuovulbo.html

Java: enum Color { RED, GREEN }
来源：http://hz.chenjidiqi.icu/gtttcrfmme.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.jinqigufen.top/gthfbgbyxz.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gzhubu.top/gtifnrhucg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.quarkkingdee.top/gtyxshrfbn.html

[G16] 对象转数组 / 字典
来源：http://hz.zhiwuduotai.top/gtdevspvmp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jianghu66.top/gtfrmhpdxi.html

PHP:  get_object_vars($obj);
来源：http://hz.yongpay.top/gtfnlveqhr.html

JS:   Object.entries(obj)
来源：http://hz.tanke756.top/gtgjmlqjwj.html

TS:   Object.entries(obj)
来源：http://hz.cdnleiting.top/gtkczntnuq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.yanxiufei.cn/gtzidcxpqa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.feifeiyinyue.top/gtmotllrri.html

Ruby: obj.instance_variables
来源：http://hz.iojbl.cn/gtgohywpuw.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.chenlongwang.top/gtbypvyhru.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtqytkdlfh.html

H. 异常与错误处理
来源：http://hz.gotoacloud.top/gtxhgilqst.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtajrjwtmk.html

[H01] try / catch 基础
来源：http://hz.gogol.net.cn/gtyvegkfvi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.haohaochexian.top/gtlymtfhsq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cheryme.top/gtmvqeekkr.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jlsjyb.cn/gtxkzbvhoo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hfpthk.cn/gteeuxwkqf.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.nanxinkj.top/gtcpajrejr.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.jinqigufen.top/gtxdsjwfjy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.kuanghao11.cn/gtxkzlpgcw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.yanxiufei.cn/gtaggsvxzo.html

[H02] finally / ensure 收尾
来源：http://hz.haohaochexian.top/gtdbanezvs.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.pycfn.com/gtfvxmtecf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.nwbrower.top/gtkpnlajdo.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.0kj1m.cn/gtkbflajfw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.ivvv.top/gtgvktfdaj.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.nanxuanxn.top/gtshgdxxua.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.hongshengwenyu.top/gtkoxbzcbs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.redwolf501.top/gtzpcwombf.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.guowangkeji.top/gtccwasygd.html

[H03] 主动抛出异常
来源：http://hz.bjfxy.top/gtbsmtybvn.html

Py:   raise ValueError("错误信息")
来源：http://hz.daxiang520.top/gtbynhgked.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.bjfxy.top/gtywsihppm.html

JS:   throw new Error("错误信息");
来源：http://hz.ppjwa.cn/gtzhqjvmxp.html

TS:   throw new Error("错误信息");
来源：http://hz.shanyushiyangtech.top/gthqzblsxa.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.ydjk.org.cn/gtnvvsoozg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.zhengqikj.top/gtuwbxffih.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.cashguo.top/gtwuozfrgp.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.vqdsnc.cn/gtdlntyshb.html

[H04] 自定义异常类型
来源：http://hz.andypj.xyz/gtsllqiobc.html

Py:   class MyError(Exception): pass
来源：http://hz.yonumen.top/gtenptugdo.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.smart0.xyz/gtyqzykymf.html

JS:   class MyError extends Error {}
来源：http://hz.xylfe.cn/gtvxcrowiw.html

TS:   class MyError extends Error {}
来源：http://hz.shzxlz.cn/gtinipqhue.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yonumen.top/gthvhphmfk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.ybcxt.top/gtrgblylpd.html

Ruby: class MyError < StandardError; end
来源：http://hz.zhixingplan.top/gtdnzjydes.html

C#:   class MyException : Exception {}
来源：http://hz.jinqigfzy.top/gtswlmkeop.html

[H05] 捕获特定类型
来源：http://hz.ppjwa.cn/gtiqwidgdx.html

Py:   except ValueError as e:
来源：http://hz.jinyuanbaomall.cn/gtdvxhfcnr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.gotoacloud.top/gtvezvdpyp.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.smart0.xyz/gtrxrvzepg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.guannengcc.top/gtfhnfjcse.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.dashuyun.cn/gtveqqtwpe.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.dianchejie.cn/gtrmucgvit.html

Ruby: rescue ArgumentError => e
来源：http://hz.havefunace.top/gtglslodpe.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.cashguo.top/gttbbwzhcl.html

[H06] 可选值 / 空值安全访问
来源：http://hz.nanxuanxn.top/gtxdqadesw.html

Py:   value = d.get("k") or default
来源：http://hz.birdmap.top/gtumcedlxb.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.gaohongyu789.top/gthusyevlc.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.dianchejie.cn/gtmoexxglw.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.jlsjyb.cn/gtsmfdqtrz.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.zdqjudy.top/gtuopfncsc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.gzhubu.top/gtogotbwzd.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yvedp.cn/gtnqstptfq.html

C#:   obj?.A?.B ?? default
来源：http://hz.0kj1m.cn/gthccqzorp.html

[H07] 断言
来源：http://hz.cucudq.cn/gtujaohxjv.html

Py:   assert x > 0, "必须为正"
来源：http://hz.sweek.top/gtlwnxpmpa.html

PHP:  assert($x > 0);
来源：http://hz.yj20258888.top/gtkgzfrbpr.html

JS:   console.assert(x > 0);
来源：http://hz.tian-w.cn/gtlvabpxug.html

TS:   console.assert(x > 0);
来源：http://hz.tanke756.top/gtfieqhxni.html

Java: assert x > 0 : "必须为正";
来源：http://hz.jianghu66.top/gtbmymzaic.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.bjfxy.top/gttvuginiw.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.ywan-chungtsiang.top/gtqymfcvoa.html

C#:   Debug.Assert(x > 0);
来源：http://hz.daria6918.cn/gtiabrmiia.html

[H08] 获取错误信息与堆栈
来源：http://hz.feifeiyinyue.top/gtvbihgkrn.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.hnqzz.top/gtdxdyepzw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.feifeiyinyue.top/gtnbtyyclb.html

JS:   e.message;  e.stack
来源：http://hz.xziqi.cn/gtsivtjrls.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hongshengwenyu.top/gthzkahabv.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.hongshengwenyu.top/gthocjnlvz.html

Go:   err.Error()
来源：http://hz.hysaishi.cn/gtezcbxfse.html

Ruby: e.message;  e.backtrace
来源：http://hz.quarkkingdee.top/gttpjtmygr.html

C#:   e.Message;  e.StackTrace
来源：http://hz.shanyushiyangkeji.top/gtozvzzyjq.html

[H09] 带错误码的异常
来源：http://hz.xuanzx.com/gtywuhyeeo.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.gogol.net.cn/gtekkwhfai.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.52xcode.cn/gtataebjaq.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.hammf.cn/gtgrmuaxqj.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.andypj.xyz/gtcryqajao.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.yueranfly.top/gtaiazahso.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.yj202588.top/gtljlxvcwc.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.hfpthk.cn/gttsdeiqjx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.cheryme.top/gtxfkeoosr.html

[H10] 资源自动释放
来源：http://hz.jinqigufen.top/gtknbtkqei.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.cdnleiting.top/gtbmedijoj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.yj20258.top/gtiwitojbx.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhixingplan.top/gtpvpgiigg.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.redwolf501.top/gtlruhdlgt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.shuidangran.top/gthblvfhnl.html

Go:   defer f.Close()
来源：http://hz.havefunace.top/gtklmfwbit.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.jinghuilouyu.cn/gtljvbtmpm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.zdqjudy.top/gtkmsqmgel.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtfwuwvsze.html

I. 正则表达式
来源：http://hz.xylfe.cn/gtqvcpfdfj.html

================================================================================
来源：http://hz.mhx1999.top/gtdajmkskl.html

[I01] 判断是否匹配
来源：http://hz.iojbl.cn/gtvtfgraki.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.jlsjyb.cn/gtfcsojjzr.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.ppjwa.cn/gtuppnamrq.html

JS:   /\d+/.test(s)
来源：http://hz.zhijiandao.cn/gtzvkycgzu.html

TS:   /\d+/.test(s)
来源：http://hz.iojbl.cn/gtfklcfyoz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.cqqwz.cn/gtojkdctrf.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.pengpengdd.cyou/gtnpecjwrm.html

Ruby: s.match?(/\d+/)
来源：http://hz.hysaishi.cn/gtqjpkcukc.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.yonumen.top/gtkyralgbm.html

[I02] 提取所有匹配
来源：http://hz.hywenlv.cn/gtzqgagewa.html

Py:   re.findall(r"\d+", s)
来源：http://hz.ivvv.top/gtiqbtzauj.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.jinqigfzy.top/gtfggkfplo.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.guowangkeji.top/gtpdtfkzzl.html

TS:   s.match(/\d+/g)
来源：http://hz.zdqjudy.top/gtmnegqedb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.cheryme.top/gtaglxgeoj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xinyue.icu/gtxhbktpnk.html

Ruby: s.scan(/\d+/)
来源：http://hz.dashuyun.cn/gtngxlndiy.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.cdnleiting.top/gtasylsspi.html

[I03] 提取捕获分组
来源：http://hz.yj20258888.top/gtsdtvajuh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.haohaochexian.top/gtawfnjivo.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.jinyuanbaomall.cn/gtkefooaif.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.xziqi.cn/gtckxxggef.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.yonumen.top/gtzejtlcap.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.birdmap.top/gtulpfyuel.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.9152youxi.cn/gtrjbnncue.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jianghu66.top/gtbszefkeb.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.c1oappe.top/gtfxymixrp.html

[I04] 正则替换
来源：http://hz.dashuyun.cn/gtjzrphzow.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.jinqigufen.top/gtjxwkuqsw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.nanxuanxn.top/gtopqduymn.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.jinghuilouyu.cn/gtzlhtmbks.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.iojbl.cn/gtvrlykivy.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.jinqigufen.top/gtghcwazlc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.meibo888.top/gtgxoaechr.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.jqgufenzy.top/gtgpnhfvus.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ivvv.top/gtwmecxdzn.html

[I05] 按正则拆分
来源：http://hz.sweek.top/gtnwiorrwk.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.hywenlv.cn/gtkipwqrze.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gaohongyu789.top/gtvkkmptcj.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yj20258.top/gtlobxkmxs.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.cashguo.top/gtmbcwdvuv.html

Java: s.split("\\s*,\\s*")
来源：http://hz.kuanghao11.cn/gtflsaetbn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.jinyuanbaomall.cn/gtnlkazmsc.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.zhijiandao.cn/gtwlmhixgw.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jinqigfzy.top/gtmiratdti.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.pengpengdd.cyou/gtnryzlity.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.havefunace.top/gtaraqhyez.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cdnleiting.top/gtzxdbwovm.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.cashguo.top/gtkqfbvfcs.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zycfv.cn/gtudguqkxh.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.pycfn.com/gtomjatwon.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.hfpthk.cn/gtxirdtqci.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jqgufenzy.top/gtpnashdrm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.havefunace.top/gtojmjrecj.html

[I07] 忽略大小写与多行模式
来源：http://hz.nwbrower.top/gtlhmfbzvc.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.snrcjt.cn/gtiawgsxfd.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.dashuyun.cn/gtsedknclw.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.xuanzx.com/gtxmrmmqwz.html

TS:   /error/gim
来源：http://hz.zhoulong.xyz/gtolokmise.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.xingfuxueyuan.xyz/gtmwiumslc.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.fengsongda.top/gtalehwumh.html

Ruby: s.scan(/error/i)
来源：http://hz.wangdashe.top/gtbamzorqq.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.yangfankeji.com/gtfidmimkj.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.zhengqikj.top/gtcuzwvoxj.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jianghu66.top/gtdrtiyhvi.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.wangshuangyany.cn/gtuetnhifk.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ybcxt.top/gtcibgemrh.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.pycfn.com/gtfaaawfhz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.daria6918.cn/gtetucfjlo.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.hfpthk.cn/gtnyoueylp.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.yj202588.top/gthripsfga.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.gaohongyu789.top/gtauuowain.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtdjbssxqp.html

J. 日期与时间
来源：http://hz.xinyue.icu/gtlclikjsj.html

================================================================================
来源：http://hz.shzxlz.cn/gtsgkdyags.html

[J01] 获取当前时间
来源：http://hz.dianchejie.cn/gtxjrokszb.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.guowangkeji.top/gtdriokguf.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.jinqigufen.top/gtfkfmcuse.html

JS:   new Date();  Date.now()
来源：http://hz.yangfankeji.com/gtyjfffqrt.html

TS:   new Date();  Date.now()
来源：http://hz.fzhhl.top/gtpdcnxobu.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.guannengcc.top/gtatrvpggt.html

Go:   time.Now()
来源：http://hz.jianghu66.top/gtrztibjzj.html

Ruby: Time.now
来源：http://hz.hammf.cn/gtyykmuobn.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.cucudq.cn/gttkygkktt.html

[J02] 格式化输出
来源：http://hz.sweek.top/gtvanzcyjj.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.jinghuilouyu.cn/gtjeuiddjv.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.zhaomingkeji.xyz/gtaqgofjqd.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.ehwqpu.com/gtupndtxwr.html

TS:   d.toISOString()
来源：http://hz.pycfn.com/gtmjzdgmkh.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yvedp.cn/gttlbnelqb.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yj20258.top/gtqfbktsow.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.wangdashe.top/gttijrarbn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.xingfuxueyuan.xyz/gtxplgxenq.html

[J03] 字符串解析为日期
来源：http://hz.yanxiufei.cn/gtwnzdgrdr.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.chenjidiqi.icu/gtwaxpvksq.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sufxvd.cn/gtffdltnqo.html

JS:   new Date("2024-01-02")
来源：http://hz.daxiang520.top/gtgdpnpzya.html

TS:   new Date("2024-01-02")
来源：http://hz.xinyue.icu/gtfgfhnibq.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.yuxming.cn/gtbyyptrct.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.zhaomingkeji.xyz/gtffvjbzjc.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinqigufen.top/gtmhpcxatz.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.mhx1999.top/gtzltooesv.html

[J04] 时间戳与日期互转
来源：http://hz.jlsjyb.cn/gtvfnuvmmq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.yvedp.cn/gtkafdmwtk.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zycfv.cn/gtyqivybjs.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.cqqwz.cn/gtipulfoas.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.vqdsnc.cn/gtfbcpkupk.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.birdmap.top/gtsushbwyl.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.xingfuxueyuan.xyz/gtdmfrqzpz.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cucudq.cn/gtrknzdbli.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hongshengwenyu.top/gtguvpkkln.html

[J05] 时间加减（加 7 天）
来源：http://hz.ehwqpu.com/gtvhvhbcnf.html

Py:   now + timedelta(days=7)
来源：http://hz.mhx1999.top/gtupxsgzbq.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.52xcode.cn/gtjhwtxanj.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.guowangkeji.top/gtxoathnnp.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.hywenlv.cn/gtzjfylglx.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.jyoumei.cn/gternuqxuu.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ybcxt.top/gtjolgenzw.html

Ruby: Time.now + 7 * 86400
来源：http://hz.iojbl.cn/gtvjkurcyj.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.xingfuxueyuan.xyz/gtvqpngxcy.html

[J06] 计算两时间之差
来源：http://hz.52xcode.cn/gtphhkrsnw.html

Py:   (end - start).total_seconds()
来源：http://hz.havefunace.top/gtexpjbawv.html

PHP:  $end->diff($start)->days;
来源：http://hz.feifeiyinyue.top/gtxisdqwpy.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.316326.xyz/gtytuakqgo.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hnxiangtu.top/gtfhggwqzv.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.gogol.net.cn/gtxfsgiiav.html

Go:   end.Sub(start).Hours()
来源：http://hz.zhijiandao.cn/gtxablcrrg.html

Ruby: end - start                 # 返回秒数
来源：http://hz.jinqigufen.top/gtvrkluqkk.html

C#:   (end - start).TotalSeconds
来源：http://hz.yanxiufei.cn/gtbdqrngqy.html

[J07] 比较两个日期
来源：http://hz.fzhhl.top/gtiyzuyixf.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.ywan-chungtsiang.top/gthpbmicpv.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.daxiang520.top/gtheenjokd.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.cqqwz.cn/gtwaeakgyr.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.xingfuxueyuan.xyz/gtqtfgmrqi.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.wangdashe.top/gtqutirydy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.chenzaomai.com/gtxpdzojwc.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.yonumen.top/gtvohshtxo.html

C#:   d1 < d2;  d1 == d2
来源：http://hz.hongshengwenyu.top/gthswomwpj.html

[J08] 提取年月日与星期
来源：http://hz.xinyue.icu/gtokjqnirf.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hz.yj202588.top/gtgzipnzbv.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hz.jiagoushi.top/gtbfepjbud.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://hz.shzxlz.cn/gtknhrbqpb.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://hz.ydzc1.top/gtkyqnkich.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hz.ybcxt.top/gtvflkysgw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hz.bjfxy.top/gtboxcdqpt.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hz.yvedp.cn/gtnsvwzhld.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hz.vqdsnc.cn/gthdajxixf.html

[J09] 时区处理
来源：http://hz.aizwys.cn/gtehdbyrns.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hz.9152youxi.cn/gtrqecqykq.html


<!-- 参考信息 -->