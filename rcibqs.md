代发 wailian999

Java: interface Shape { double area(); }
来源：http://hz.snrcjt.cn/gtgnuamvxg.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yj20258.top/gtbnbomifg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.yanxiufei.cn/gtbtiivkcr.html

C#:   interface IShape { double Area(); }
来源：http://hz.smart0.xyz/gtrgpamfnz.html

[G10] 访问控制
来源：http://hz.chenlongwang.top/gtdiauckne.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.chenzaomai.com/gtvrasbeuv.html

PHP:  public / protected / private
来源：http://hz.wangshuangyany.cn/gtgbnzkrkt.html

JS:   #private 字段；其余公开
来源：http://hz.aizwys.cn/gtykazfzzh.html

TS:   public / protected / private
来源：http://hz.pengpengdd.cyou/gtfpaqsqko.html

Java: public / protected / private / 默认包级
来源：http://hz.mhx1999.top/gtomwujknk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.pengpengdd.cyou/gtipspqxom.html

Ruby: public / protected / private
来源：http://hz.xuetiantiany.cn/gtxtykroxd.html

C#:   public / protected / private / internal
来源：http://hz.yvedp.cn/gtjdkbkfdw.html

[G11] getter / setter
来源：http://hz.zdqjudy.top/gtleszbpgm.html

Py:   @property 与 @x.setter
来源：http://hz.yj20258.top/gtzuaptxfc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hywenlv.cn/gtkyfmubga.html

JS:   get name() { return this._name; }
来源：http://hz.cheryme.top/gtgzgrliht.html

TS:   get name(): string { return this._name; }
来源：http://hz.wangshuangyany.cn/gtyswnewdg.html

Java: public String getName() { return name; }
来源：http://hz.yuanzhike.top/gtptyqhjhs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhaomingkeji.xyz/gtetayrrpm.html

Ruby: attr_accessor :name
来源：http://hz.sufxvd.cn/gtadmfegks.html

C#:   public string Name { get; set; }
来源：http://hz.shanyushiyangkeji.top/gtfpucxtca.html

[G12] 对象转字符串
来源：http://hz.pengpengdd.cyou/gtkbidyvlz.html

Py:   def __str__(self): return self.name
来源：http://hz.jqgfzy.top/gtvwkbfxjw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.meibo888.top/gtdhfypypv.html

JS:   toString() { return this.name; }
来源：http://hz.hongshengwenyu.top/gtnftebyug.html

TS:   toString(): string { return this.name; }
来源：http://hz.zdqjudy.top/gtosnqaxdk.html

Java: @Override public String toString() { return name; }
来源：http://hz.sweek.top/gtmqceppbf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.dianchejie.cn/gtoojonksy.html

Ruby: def to_s; @name; end
来源：http://hz.shuidangran.top/gtbxrclewo.html

C#:   public override string ToString() => Name;
来源：http://hz.zhongyouzk.top/gtrgejjxjv.html

[G13] 判断对象类型
来源：http://hz.hfpthk.cn/gtybbqtdln.html

Py:   isinstance(u, User)
来源：http://hz.jqgufenzy.top/gttlqxjddv.html

PHP:  $u instanceof User
来源：http://hz.yj20258.top/gtacicupqa.html

JS:   u instanceof User
来源：http://hz.ppjwa.cn/gtcqrdwiuq.html

TS:   u instanceof User
来源：http://hz.zhoulong.xyz/gtldgdiwea.html

Java: u instanceof User
来源：http://hz.daxiang520.top/gtveakuxvn.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.gogol.net.cn/gtukxcocws.html

Ruby: u.is_a?(User)
来源：http://hz.shanyushiyangkeji.top/gtovjqjgew.html

C#:   u is User
来源：http://hz.tian-w.cn/gtdzlwcwfg.html

[G14] 数据类 / record
来源：http://hz.jqgufenzy.top/gtcswaueav.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.fzhhl.top/gtriknpiuk.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.ppjwa.cn/gtawumobho.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.yanxiufei.cn/gtywzpcnbe.html

TS:   type User = { name: string; age: number };
来源：http://hz.daria6918.cn/gtwrozkplj.html

Java: record User(String name, int age) {}
来源：http://hz.chenzaomai.com/gthtffbzza.html

Go:   type User struct { Name string; Age int }
来源：http://hz.hysaishi.cn/gtxirzsynn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.yj202588.top/gtqcarxspi.html

C#:   record User(string Name, int Age);
来源：http://hz.hywenlv.cn/gtcbivxiax.html

[G15] 枚举
来源：http://hz.smart0.xyz/gtoupclubt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.zhixingplan.top/gtidlgqvrh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.vqdsnc.cn/gtpxgovsut.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.gzhubu.top/gtgcoyyvnf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.0kj1m.cn/gtqicuhdpy.html

Java: enum Color { RED, GREEN }
来源：http://hz.yj20258.top/gtjwgpvcch.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.sweek.top/gtwclidpwv.html

Ruby: Color = %i[red green].freeze
来源：http://hz.gogol.net.cn/gtwhlymghy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.jiagoushi.top/gtdnrzbbqg.html

[G16] 对象转数组 / 字典
来源：http://hz.kuanghao11.cn/gtsfsndfli.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.nanxuanxn.top/gtyzvnzqla.html

PHP:  get_object_vars($obj);
来源：http://hz.jinyuanbaomall.cn/gtezgpsatg.html

JS:   Object.entries(obj)
来源：http://hz.cashguo.top/gtwcyoufhv.html

TS:   Object.entries(obj)
来源：http://hz.cucudq.cn/gtsrvbfxqo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hnqzz.top/gtepdqinug.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.jqgfzy.top/gtwggitpyq.html

Ruby: obj.instance_variables
来源：http://hz.daxiang520.top/gtfwytysnh.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.xylfe.cn/gtsywhiadd.html

================================================================================
来源：http://hz.yj202588.top/gtjtabxhip.html

H. 异常与错误处理
来源：http://hz.jlsjyb.cn/gtwggjzwyw.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtsgulwaco.html

[H01] try / catch 基础
来源：http://hz.shuidangran.top/gtvgjrhbzr.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.yangfankeji.com/gtxyvpdccz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.cashguo.top/gtdzzlieqh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.xinyue.icu/gtabkdbkyz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.nwbrower.top/gtfvhutfik.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yueranfly.top/gtoiwfyocp.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.dashuyun.cn/gtqfpbpjop.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.zhiwuduotai.top/gtxwaejaaz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.gotoacloud.top/gtqatyuwrj.html

[H02] finally / ensure 收尾
来源：http://hz.jqgufenzy.top/gtsmtrfdyy.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.ppjwa.cn/gtydxjxbnk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.shangyingyoupin.top/gtgrsjwcwi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.guannengcc.top/gtxzjmgquo.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.xuetiantiany.cn/gtxbzvfhbu.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.c1oappe.top/gtjcxjujtl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.yj20258.top/gtlmgcklxt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xuanzx.com/gtqjqivomk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.nanxinkj.top/gtqjbfbhiz.html

[H03] 主动抛出异常
来源：http://hz.dashuyun.cn/gtfzsxsfwm.html

Py:   raise ValueError("错误信息")
来源：http://hz.yuanzhike.top/gtqhyupghb.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.jinghuilouyu.cn/gtcnebybog.html

JS:   throw new Error("错误信息");
来源：http://hz.xuetiantiany.cn/gtcfzzomqb.html

TS:   throw new Error("错误信息");
来源：http://hz.tian-w.cn/gtvnecjoue.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.kuanghao11.cn/gterhfqbev.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.feifeiyinyue.top/gtaysmfcxz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.zhengqikj.top/gtpisfhscn.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.aibaodan.cn/gthguouwbd.html

[H04] 自定义异常类型
来源：http://hz.mhx1999.top/gtbqtwmbcs.html

Py:   class MyError(Exception): pass
来源：http://hz.yangfankeji.com/gtcaxvtwca.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.gotoacloud.top/gtvbusboam.html

JS:   class MyError extends Error {}
来源：http://hz.yj20258.top/gtkbxbwxit.html

TS:   class MyError extends Error {}
来源：http://hz.snrcjt.cn/gtrfkxaxoj.html

Java: class MyException extends RuntimeException {}
来源：http://hz.gogol.net.cn/gthtcxntyu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.wangshuangyany.cn/gtnnrxtbqj.html

Ruby: class MyError < StandardError; end
来源：http://hz.yongpay.top/gtvqqokzae.html

C#:   class MyException : Exception {}
来源：http://hz.shuidangran.top/gtjmcpxdkb.html

[H05] 捕获特定类型
来源：http://hz.hnqzz.top/gtvltjnpac.html

Py:   except ValueError as e:
来源：http://hz.hnxiangtu.top/gtryzciihq.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.zdqjudy.top/gtjgwufaru.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.tianlin.xyz/gtirnsoapj.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.zhiwuduotai.top/gtnqkdnjvn.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hnqzz.top/gtenxapdfa.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.redwolf501.top/gtjyflvifn.html

Ruby: rescue ArgumentError => e
来源：http://hz.ydzc1.top/gtprvvtovn.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.gzhubu.top/gtmfrvvbre.html

[H06] 可选值 / 空值安全访问
来源：http://hz.ywan-chungtsiang.top/gtifmprvlv.html

Py:   value = d.get("k") or default
来源：http://hz.yonumen.top/gtqojeoqgj.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.yj20258.top/gtnfqlrnmb.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.xinyue.icu/gtkjxnfivn.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ppjwa.cn/gttmvhziwo.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.hammf.cn/gtbzyeozsq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.pycfn.com/gteihnodad.html

Ruby: d&.dig(:a, :b)
来源：http://hz.yongpay.top/gtfbvjjybg.html

C#:   obj?.A?.B ?? default
来源：http://hz.hfpthk.cn/gtfjftrhdi.html

[H07] 断言
来源：http://hz.shanyushiyangtech.top/gthkzobjko.html

Py:   assert x > 0, "必须为正"
来源：http://hz.zhengqikj.top/gtzkgudcql.html

PHP:  assert($x > 0);
来源：http://hz.nwbrower.top/gtdkoudqsy.html

JS:   console.assert(x > 0);
来源：http://hz.xylfe.cn/gtuualltud.html

TS:   console.assert(x > 0);
来源：http://hz.0kj1m.cn/gtsediiruc.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shuidangran.top/gtelyjoyum.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.jinghuilouyu.cn/gtbokphjkk.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.nwbrower.top/gticslkvts.html

C#:   Debug.Assert(x > 0);
来源：http://hz.xuetiantiany.cn/gtiylegabh.html

[H08] 获取错误信息与堆栈
来源：http://hz.nanxuanxn.top/gtqwinfnzq.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.wangshuangyany.cn/gtlnggzpvx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.yj20258.top/gtydxmavas.html

JS:   e.message;  e.stack
来源：http://hz.hnxiangtu.top/gthuwebzod.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.hnqzz.top/gtmnyffebe.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.kuanghao11.cn/gtxjvprsrp.html

Go:   err.Error()
来源：http://hz.yvedp.cn/gtstdklhuz.html

Ruby: e.message;  e.backtrace
来源：http://hz.chenjidiqi.icu/gtsahexzar.html

C#:   e.Message;  e.StackTrace
来源：http://hz.ehwqpu.com/gtbuibqcnr.html

[H09] 带错误码的异常
来源：http://hz.quarkkingdee.top/gtyfyhddiq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.bjfxy.top/gtdmanizgm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gzhubu.top/gtimdstfae.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.yuxming.cn/gtcwdfaemw.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.zhixingplan.top/gtaaxbfofl.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.hnxiangtu.top/gtsvmuujkc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.ywan-chungtsiang.top/gtuhkrwviw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.yuanzhike.top/gttryasroh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.316326.xyz/gtmkxobwql.html

[H10] 资源自动释放
来源：http://hz.jinqigfzy.top/gtkyutktbc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.jiagoushi.top/gtuyqijeto.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.xziqi.cn/gtqaxscqtj.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.snrcjt.cn/gtwfarhyot.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.nanxuanxn.top/gtfzfoczxy.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.dianchejie.cn/gtuhvisvgo.html

Go:   defer f.Close()
来源：http://hz.guannengcc.top/gtavulzsyz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.hfpthk.cn/gturbmedws.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.guannengcc.top/gtzmeaqfzf.html

================================================================================
来源：http://hz.yj202588.top/gtoonnkant.html

I. 正则表达式
来源：http://hz.52xcode.cn/gtbofzkpdu.html

================================================================================
来源：http://hz.hysaishi.cn/gtcyszqwoy.html

[I01] 判断是否匹配
来源：http://hz.0kj1m.cn/gtpvdqufjv.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.ivvv.top/gtieyflwtx.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.xuanzx.com/gtpwjqrdbg.html

JS:   /\d+/.test(s)
来源：http://hz.chenzaomai.com/gtlkrfhtnv.html

TS:   /\d+/.test(s)
来源：http://hz.vqdsnc.cn/gteotlydvv.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.gaohongyu789.top/gtljubwrxw.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jinqigufen.top/gtcuiuyiwc.html

Ruby: s.match?(/\d+/)
来源：http://hz.hammf.cn/gtonlxyzfe.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.jinghuilouyu.cn/gtboypesul.html

[I02] 提取所有匹配
来源：http://hz.mhx1999.top/gtsvknakiy.html

Py:   re.findall(r"\d+", s)
来源：http://hz.xingfuxueyuan.xyz/gtotnmdhjx.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.yangfankeji.com/gtpdcammup.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.zhengqikj.top/gtbwgdxkbn.html

TS:   s.match(/\d+/g)
来源：http://hz.hysaishi.cn/gtzienmtlf.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.316326.xyz/gtzvvweptv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.nanxuanxn.top/gtvkboqilw.html

Ruby: s.scan(/\d+/)
来源：http://hz.52xcode.cn/gtzjselyco.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.svipenyu.cn/gtbidprorg.html

[I03] 提取捕获分组
来源：http://hz.aibaodan.cn/gttkijrmsf.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.zhiwuduotai.top/gtsxqnqkpm.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.birdmap.top/gtcahqbqhg.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.ppjwa.cn/gttotzpfwv.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.wangdashe.top/gtluuxojwi.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.cdnleiting.top/gtqtlsvrhl.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.redwolf501.top/gtnkoahmxq.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.chenjidiqi.icu/gtjyecrgmq.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhengqikj.top/gtmjqujzps.html

[I04] 正则替换
来源：http://hz.c1oappe.top/gtyfoyqyvu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.nanxuanxn.top/gttbtxqehd.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.ehwqpu.com/gtbqgputow.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.316326.xyz/gtdamgrxsv.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.gaohongyu789.top/gtsmtjjqoi.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.zhongyouzk.top/gtwwoyhxpm.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.ybcxt.top/gtrvynhlow.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.redwolf501.top/gttreuhoec.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.0kj1m.cn/gtixszvozm.html

[I05] 按正则拆分
来源：http://hz.pengpengdd.cyou/gtculrrqfn.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.9152youxi.cn/gtiypxuifg.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.kuanghao11.cn/gtkeqespaw.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.yonumen.top/gtyfjgvvjq.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.sxryk.cn/gtwrfevjul.html

Java: s.split("\\s*,\\s*")
来源：http://hz.0kj1m.cn/gtrwfdsrkt.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.c1oappe.top/gtkgdvjysm.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.kuanghao11.cn/gtqfxddxvd.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.jianghu66.top/gtznhkptbn.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.shanyushiyangkeji.top/gtepjatctk.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.jinghuilouyu.cn/gttddpzraa.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.yueranfly.top/gtdraiixhg.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.tianlin.xyz/gtiuziaqgk.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.hfpthk.cn/gtkdqkiotz.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.zhoulong.xyz/gtcybioiix.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.sxryk.cn/gtrfdlpzsp.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.jinghuilouyu.cn/gtjonkaopm.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.52xcode.cn/gtzcjmfeid.html

[I07] 忽略大小写与多行模式
来源：http://hz.hywenlv.cn/gtjzkjuqgx.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.shanyushiyangtech.top/gtgfvwpgna.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.hnxiangtu.top/gtqmdcevba.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.gotoacloud.top/gtqqezfwct.html

TS:   /error/gim
来源：http://hz.yvedp.cn/gtjpjoqifm.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.shanyushiyangkeji.top/gtmbtduvgr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.hnxiangtu.top/gtivkppqiu.html

Ruby: s.scan(/error/i)
来源：http://hz.jianghu66.top/gtnkajexuh.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.cdnleiting.top/gtescjclen.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.dashuyun.cn/gtlsywdvav.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.zhongyouzk.top/gtgvntlqll.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.cashguo.top/gtwlbucmmd.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.yanxiufei.cn/gtemuhsihw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.jinqigfzy.top/gtcwegqepm.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.cashguo.top/gtayvmlxiy.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.birdmap.top/gtfabsiifv.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.zhixingplan.top/gtufczrsar.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.jqgufenzy.top/gtvcwzzrva.html

================================================================================
来源：http://hz.dianchejie.cn/gtoptdqdlb.html

J. 日期与时间
来源：http://hz.gogol.net.cn/gtxqrvwwwu.html

================================================================================
来源：http://hz.xziqi.cn/gtxqjkkocl.html

[J01] 获取当前时间
来源：http://hz.c1oappe.top/gtcynzmnqa.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.xuanzx.com/gtkhtcecvm.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.shanyushiyangkeji.top/gtaenrwldv.html

JS:   new Date();  Date.now()
来源：http://hz.wangdashe.top/gtzmuhydlg.html

TS:   new Date();  Date.now()
来源：http://hz.svipenyu.cn/gtfxbfblbv.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.sxryk.cn/gtzwcvxbss.html

Go:   time.Now()
来源：http://hz.cashguo.top/gtnyhnjuzb.html

Ruby: Time.now
来源：http://hz.ppjwa.cn/gtjtzwxcfm.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.yj20258888.top/gtdlivamvg.html

[J02] 格式化输出
来源：http://hz.jqgfzy.top/gtcfdvolfg.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.gotoacloud.top/gtlmpgzvyj.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.tianlin.xyz/gtopaicifu.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.jinyuanbaomall.cn/gtcxinlcxm.html

TS:   d.toISOString()
来源：http://hz.zhengqikj.top/gtnozulafo.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.yuxming.cn/gtpbyoabne.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.yonumen.top/gtwojqlfct.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.zhaomingkeji.xyz/gtzfqkbkxz.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.dashuyun.cn/gtrvgnlmxl.html

[J03] 字符串解析为日期
来源：http://hz.tanke756.top/gtippmzihw.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.chenjidiqi.icu/gtbemkrazp.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.sweek.top/gtgokktrvx.html

JS:   new Date("2024-01-02")
来源：http://hz.nwbrower.top/gtucjlmlan.html

TS:   new Date("2024-01-02")
来源：http://hz.smart0.xyz/gtgwuveoay.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.gzhubu.top/gtsuzqmowl.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.xingfuxueyuan.xyz/gtifawylmu.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.jinghuilouyu.cn/gtltujbxmh.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jianghu66.top/gtincrlgbd.html

[J04] 时间戳与日期互转
来源：http://hz.sweek.top/gtshtkdxsz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shanyushiyangtech.top/gtcrmohwpt.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.zhengqikj.top/gtoxmwghal.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.chenzaomai.com/gtsxpdrnkc.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.jiagoushi.top/gtizbyobjr.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.ydzc1.top/gthievlnxz.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.nwbrower.top/gtlnajdfwa.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.9152youxi.cn/gtdvakudxr.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.nanxinkj.top/gtxqjgepcx.html

[J05] 时间加减（加 7 天）
来源：http://hz.hongshengwenyu.top/gtfbnagpwz.html

Py:   now + timedelta(days=7)
来源：http://hz.gzhubu.top/gttxoxfffu.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.guowangkeji.top/gtmgyvnodk.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.gaohongyu789.top/gtqfsybcbu.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.wangshuangyany.cn/gtjdzjfhiy.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.shanyushiyangtech.top/gtlrxdpawk.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.316326.xyz/gtmibqfarj.html

Ruby: Time.now + 7 * 86400
来源：http://hz.hnqzz.top/gteuqaiijr.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhongyouzk.top/gtxoddrhjk.html

[J06] 计算两时间之差
来源：http://hz.wangdashe.top/gtzboyimgs.html

Py:   (end - start).total_seconds()
来源：http://hz.xingfuxueyuan.xyz/gtvnyqkmos.html

PHP:  $end->diff($start)->days;
来源：http://hz.sweek.top/gtbjacmuqx.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xziqi.cn/gtmnqnzuvz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.sweek.top/gterfsygnm.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.smart0.xyz/gtpkiengaq.html

Go:   end.Sub(start).Hours()
来源：http://hz.dianchejie.cn/gtjxxacwkj.html

Ruby: end - start                 # 返回秒数
来源：http://hz.yangfankeji.com/gtrdszlngb.html

C#:   (end - start).TotalSeconds
来源：http://hz.feifeiyinyue.top/gttpkqshpw.html

[J07] 比较两个日期
来源：http://hz.shanyushiyangtech.top/gtdrvbhchx.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.yuanzhike.top/gtijfbslzm.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.tian-w.cn/gtgodxbmua.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.hongshengwenyu.top/gtrylnuwxw.html

TS:   d1.getTime() < d2.getTime()
来源：http://hz.daria6918.cn/gtegpeyioo.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hz.xuanzx.com/gtiktsbhwu.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hz.quarkkingdee.top/gtyifzoaib.html

Ruby: d1 < d2;  d1 == d2
来源：http://hz.ydzc1.top/gtincvaejp.html


<!-- 参考信息 -->