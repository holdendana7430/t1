代发 wailian999

Py:   from abc import ABC, abstractmethod
来源：http://hz.xuanzx.com/gtvecxmclg.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.wangdashe.top/gtuhwezeun.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.kuanghao11.cn/gtuqochzja.html

TS:   interface Shape { area(): number; }
来源：http://hz.gaohongyu789.top/gtsuwntwil.html

Java: interface Shape { double area(); }
来源：http://hz.fzhhl.top/gtjrbetmuf.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.nwbrower.top/gtuajkgxly.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.havefunace.top/gtuahuuzgb.html

C#:   interface IShape { double Area(); }
来源：http://hz.tianlin.xyz/gtrdeceuxu.html

[G10] 访问控制
来源：http://hz.yangfankeji.com/gttqxymzxp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jinghuilouyu.cn/gtpnrxazcw.html

PHP:  public / protected / private
来源：http://hz.tian-w.cn/gtygxpznpj.html

JS:   #private 字段；其余公开
来源：http://hz.jyoumei.cn/gtuwlhwwtw.html

TS:   public / protected / private
来源：http://hz.jinyuanbaomall.cn/gterzbnxnm.html

Java: public / protected / private / 默认包级
来源：http://hz.gaohongyu789.top/gtziequljy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ywan-chungtsiang.top/gtesitefdb.html

Ruby: public / protected / private
来源：http://hz.haohaochexian.top/gtjoecbgcj.html

C#:   public / protected / private / internal
来源：http://hz.zycfv.cn/gtajpmqvqy.html

[G11] getter / setter
来源：http://hz.yanxiufei.cn/gtifgcsitc.html

Py:   @property 与 @x.setter
来源：http://hz.zhiwuduotai.top/gtbsidqzvb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhiwuduotai.top/gtcctzmose.html

JS:   get name() { return this._name; }
来源：http://hz.birdmap.top/gtrwjtxxfb.html

TS:   get name(): string { return this._name; }
来源：http://hz.havefunace.top/gtqoqevnhy.html

Java: public String getName() { return name; }
来源：http://hz.shanyushiyangtech.top/gtwpxnkkiu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhengqikj.top/gtthmhhqjp.html

Ruby: attr_accessor :name
来源：http://hz.yj202588.top/gtmmlfqjqg.html

C#:   public string Name { get; set; }
来源：http://hz.shzxlz.cn/gtlbzkiyyp.html

[G12] 对象转字符串
来源：http://hz.xingfuxueyuan.xyz/gtauqjpcgv.html

Py:   def __str__(self): return self.name
来源：http://hz.zycfv.cn/gtlcpmwsoy.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhiwuduotai.top/gtqnxhtedv.html

JS:   toString() { return this.name; }
来源：http://hz.shangyingyoupin.top/gtwcerqite.html

TS:   toString(): string { return this.name; }
来源：http://hz.meibo888.top/gtdvolukdx.html

Java: @Override public String toString() { return name; }
来源：http://hz.guowangkeji.top/gteakgcdub.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinyuanbaomall.cn/gtnthtrovi.html

Ruby: def to_s; @name; end
来源：http://hz.zdqjudy.top/gtugirwjhh.html

C#:   public override string ToString() => Name;
来源：http://hz.jlsjyb.cn/gtbeejfvfv.html

[G13] 判断对象类型
来源：http://hz.zhaomingkeji.xyz/gtjjviebcx.html

Py:   isinstance(u, User)
来源：http://hz.jqgfzy.top/gtnedbzsbi.html

PHP:  $u instanceof User
来源：http://hz.feifeiyinyue.top/gtupvarkxj.html

JS:   u instanceof User
来源：http://hz.yvedp.cn/gtjstlcsst.html

TS:   u instanceof User
来源：http://hz.yuxming.cn/gtciuyjgxn.html

Java: u instanceof User
来源：http://hz.yanxiufei.cn/gtkktqrjjz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ppjwa.cn/gtnjijjzxs.html

Ruby: u.is_a?(User)
来源：http://hz.hysaishi.cn/gtkuodtgbe.html

C#:   u is User
来源：http://hz.316326.xyz/gtcmozfjdf.html

[G14] 数据类 / record
来源：http://hz.jinqigfzy.top/gtmykpdulp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.fzhhl.top/gtggrysbfn.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.gzhubu.top/gtehljpzvy.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.svipenyu.cn/gtvgxsjvmw.html

TS:   type User = { name: string; age: number };
来源：http://hz.zhaomingkeji.xyz/gttcxhbzwa.html

Java: record User(String name, int age) {}
来源：http://hz.nwbrower.top/gtvcnroymr.html

Go:   type User struct { Name string; Age int }
来源：http://hz.cucudq.cn/gtjjylqsko.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.316326.xyz/gtiffljnob.html

C#:   record User(string Name, int Age);
来源：http://hz.shangyingyoupin.top/gtqclasiwa.html

[G15] 枚举
来源：http://hz.cashguo.top/gtnxvoqzvk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.meibo888.top/gtboacidqo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.c1oappe.top/gtlczjabop.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.jyoumei.cn/gtlsxubiqv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.redwolf501.top/gthbzdianr.html

Java: enum Color { RED, GREEN }
来源：http://hz.chenzaomai.com/gtabwifagf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.feifeiyinyue.top/gtwzzpdyti.html

Ruby: Color = %i[red green].freeze
来源：http://hz.smart0.xyz/gtqkvrrbza.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.nwbrower.top/gtksyymzim.html

[G16] 对象转数组 / 字典
来源：http://hz.ywan-chungtsiang.top/gtxuvxdfsd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.shzxlz.cn/gtsbhedqsb.html

PHP:  get_object_vars($obj);
来源：http://hz.zhaomingkeji.xyz/gtxqszxqgm.html

JS:   Object.entries(obj)
来源：http://hz.yj20258888.top/gtvykkgmsz.html

TS:   Object.entries(obj)
来源：http://hz.dashuyun.cn/gtidaxacfl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jinqigfzy.top/gtqwhmnlzu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.dianchejie.cn/gtmafitnbd.html

Ruby: obj.instance_variables
来源：http://hz.zhaomingkeji.xyz/gtsotqqskh.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.shangyingyoupin.top/gtfnvbangg.html

================================================================================
来源：http://hz.jinqigfzy.top/gtslddbhrh.html

H. 异常与错误处理
来源：http://hz.ehwqpu.com/gtdtqvarjx.html

================================================================================
来源：http://hz.kuanghao11.cn/gterysumfh.html

[H01] try / catch 基础
来源：http://hz.ydjk.org.cn/gtfhoophpd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.feifeiyinyue.top/gtzsshgetr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hammf.cn/gtpslhtnjs.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.cashguo.top/gtlzojituf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.jiagoushi.top/gtatwesvsk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.yongpay.top/gtdjqaviob.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.aizwys.cn/gtjofswmys.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.tian-w.cn/gtvgdulpmh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.xylfe.cn/gtgakyhfzt.html

[H02] finally / ensure 收尾
来源：http://hz.jinqigufen.top/gtypondxvr.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.cheryme.top/gthnyzojiq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.hysaishi.cn/gttphkcnrt.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.vqdsnc.cn/gtzfsqzupb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.zhiwuduotai.top/gtodbgblfv.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.ehwqpu.com/gtcsajcqok.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.iojbl.cn/gtllxypaog.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.ppjwa.cn/gtszrflkkj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.jinqigufen.top/gtbdrohzdt.html

[H03] 主动抛出异常
来源：http://hz.yuxming.cn/gtnnidnpoc.html

Py:   raise ValueError("错误信息")
来源：http://hz.aibaodan.cn/gtfbkehyoy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.yvedp.cn/gtshbvdoie.html

JS:   throw new Error("错误信息");
来源：http://hz.yj20258.top/gtalaegoxr.html

TS:   throw new Error("错误信息");
来源：http://hz.hongshengwenyu.top/gtadwqrzcp.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.yueranfly.top/gtovabloio.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.mhx1999.top/gtbpvpzzhg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.hammf.cn/gtotkiekjt.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.yj20258.top/gtwuhlchfc.html

[H04] 自定义异常类型
来源：http://hz.9152youxi.cn/gtdnxjygbw.html

Py:   class MyError(Exception): pass
来源：http://hz.ppjwa.cn/gtvejbztlo.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.feifeiyinyue.top/gthhwvasri.html

JS:   class MyError extends Error {}
来源：http://hz.gaohongyu789.top/gtirvdszcg.html

TS:   class MyError extends Error {}
来源：http://hz.sufxvd.cn/gtdhmvoytj.html

Java: class MyException extends RuntimeException {}
来源：http://hz.cucudq.cn/gtijkhphql.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.xylfe.cn/gttkniukig.html

Ruby: class MyError < StandardError; end
来源：http://hz.ehwqpu.com/gtmjgvzmcc.html

C#:   class MyException : Exception {}
来源：http://hz.cashguo.top/gtyjveaeom.html

[H05] 捕获特定类型
来源：http://hz.jinqigfzy.top/gtbsctaygb.html

Py:   except ValueError as e:
来源：http://hz.guannengcc.top/gtmrhsputb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.xinyue.icu/gtyiwlgyiv.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.hammf.cn/gtsllmlwlg.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.hywenlv.cn/gtlyuslwzh.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.vqdsnc.cn/gttjrxzghw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.ybcxt.top/gtharkylre.html

Ruby: rescue ArgumentError => e
来源：http://hz.jiagoushi.top/gtiibpftjk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.iojbl.cn/gtfdfvdsmd.html

[H06] 可选值 / 空值安全访问
来源：http://hz.meibo888.top/gtpnprmlrm.html

Py:   value = d.get("k") or default
来源：http://hz.hnqzz.top/gtqtuibrnw.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.andypj.xyz/gtmctrelbk.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.chenlongwang.top/gtglhlpneg.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.zhijiandao.cn/gtcefoycba.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.daria6918.cn/gtvfecftsm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.yanxiufei.cn/gtfathxyau.html

Ruby: d&.dig(:a, :b)
来源：http://hz.iojbl.cn/gtwuvaviwu.html

C#:   obj?.A?.B ?? default
来源：http://hz.shangyingyoupin.top/gtdxiqfssi.html

[H07] 断言
来源：http://hz.sufxvd.cn/gtzqogqwed.html

Py:   assert x > 0, "必须为正"
来源：http://hz.gogol.net.cn/gthozhpcsc.html

PHP:  assert($x > 0);
来源：http://hz.zdqjudy.top/gtimnrycpa.html

JS:   console.assert(x > 0);
来源：http://hz.cashguo.top/gtgekydhne.html

TS:   console.assert(x > 0);
来源：http://hz.yonumen.top/gtzruaelmu.html

Java: assert x > 0 : "必须为正";
来源：http://hz.xuetiantiany.cn/gtqdltydpb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.yanxiufei.cn/gtgstvfxbb.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jianghu66.top/gtinevrmkn.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ydzc1.top/gtbtxtqcgn.html

[H08] 获取错误信息与堆栈
来源：http://hz.xuanzx.com/gtwjmcvglh.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.jiagoushi.top/gtsgmdhydo.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.aizwys.cn/gtvxcewscb.html

JS:   e.message;  e.stack
来源：http://hz.yangfankeji.com/gtuaiseifi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.haohaochexian.top/gtbqykhvox.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.chenzaomai.com/gtouupztuj.html

Go:   err.Error()
来源：http://hz.guannengcc.top/gteimegunq.html

Ruby: e.message;  e.backtrace
来源：http://hz.yj20258888.top/gtfrkkfjjh.html

C#:   e.Message;  e.StackTrace
来源：http://hz.daxiang520.top/gttbcxhddo.html

[H09] 带错误码的异常
来源：http://hz.tanke756.top/gtpefwyplw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.yvedp.cn/gtklycfiqr.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.gaohongyu789.top/gtnqzfjoqz.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.shuidangran.top/gtygqyskli.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.yanxiufei.cn/gtioyakwpc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.xingfuxueyuan.xyz/gtzcizlsgk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.wangdashe.top/gtjtsfbumw.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.andypj.xyz/gtcxlzdoxf.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.ehwqpu.com/gtatfkmjmy.html

[H10] 资源自动释放
来源：http://hz.cheryme.top/gtpyxshwqj.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.chenjidiqi.icu/gtrizhmofu.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.9152youxi.cn/gtsvrmrbip.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhiwuduotai.top/gtoaiuvbkw.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.shanyushiyangtech.top/gtdyhcejek.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.jinghuilouyu.cn/gtzrpkzofn.html

Go:   defer f.Close()
来源：http://hz.yuanzhike.top/gtddzgnxvr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.yongpay.top/gtckfyfqjl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.mhx1999.top/gtpsjzolnt.html

================================================================================
来源：http://hz.nanxinkj.top/gtfuumkbic.html

I. 正则表达式
来源：http://hz.hongshengwenyu.top/gtkykjccmy.html

================================================================================
来源：http://hz.xuanzx.com/gtkktjyhsa.html

[I01] 判断是否匹配
来源：http://hz.birdmap.top/gteojkpbly.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.nwbrower.top/gtzmtdvaev.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.nwbrower.top/gthinpbbgu.html

JS:   /\d+/.test(s)
来源：http://hz.c1oappe.top/gtxtoxfnpz.html

TS:   /\d+/.test(s)
来源：http://hz.xingfuxueyuan.xyz/gtblbmstlp.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.jyoumei.cn/gtyobegdqx.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.jlsjyb.cn/gtovizxljk.html

Ruby: s.match?(/\d+/)
来源：http://hz.fengsongda.top/gtjzmizrgq.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.wangshuangyany.cn/gtfinfkdge.html

[I02] 提取所有匹配
来源：http://hz.52xcode.cn/gtaijlfskl.html

Py:   re.findall(r"\d+", s)
来源：http://hz.feifeiyinyue.top/gthnzulowt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.nanxuanxn.top/gtwkcmtgil.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.pycfn.com/gtiwssmqyh.html

TS:   s.match(/\d+/g)
来源：http://hz.ehwqpu.com/gtiqnuytdi.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.hywenlv.cn/gtvrzfwegg.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.shanyushiyangkeji.top/gtwpvbgoof.html

Ruby: s.scan(/\d+/)
来源：http://hz.hnqzz.top/gtzwfqkzfd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.hywenlv.cn/gtixjjusik.html

[I03] 提取捕获分组
来源：http://hz.jinqigfzy.top/gtnfvdflxi.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.jianghu66.top/gtqrwnfjgz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.ywan-chungtsiang.top/gtlgssqllj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.quarkkingdee.top/gtcrflgrcw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.wangdashe.top/gtysxvfhkz.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.zhixingplan.top/gtbfwduxbf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ydjk.org.cn/gtmkpsbdpg.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.dianchejie.cn/gteytewwde.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.zhixingplan.top/gtwwwlwuhw.html

[I04] 正则替换
来源：http://hz.xinyue.icu/gtdsmyhjbk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.shangyingyoupin.top/gtvxqamwud.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.shanyushiyangkeji.top/gtbfknccff.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.ywan-chungtsiang.top/gtsrhkifhh.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.yongpay.top/gtnerdgcfn.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.yangfankeji.com/gtapihcnfz.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.chenzaomai.com/gtmsubkhyj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.zhijiandao.cn/gtggjcpdpi.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.ywan-chungtsiang.top/gtlaysmtcr.html

[I05] 按正则拆分
来源：http://hz.cdnleiting.top/gtlekvfwnv.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.haohaochexian.top/gtttfuigaz.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.yuanzhike.top/gtwkesotox.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jinyuanbaomall.cn/gtghuwgdzr.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.gogol.net.cn/gteygvdnxf.html

Java: s.split("\\s*,\\s*")
来源：http://hz.hysaishi.cn/gtrorxynbm.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.gogol.net.cn/gtdefeijti.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.daria6918.cn/gtfnhniqwz.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.svipenyu.cn/gtrbuffasv.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.jinghuilouyu.cn/gtezgxkxnd.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.nwbrower.top/gttrrsxptx.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.cqqwz.cn/gtsgnwywez.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.aizwys.cn/gtvugcvuga.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.shanyushiyangtech.top/gtgtydyrge.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.fzhhl.top/gtpkistkjs.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.guannengcc.top/gtuouiueai.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.daxiang520.top/gtpjdwmfsi.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.zycfv.cn/gtjziktfih.html

[I07] 忽略大小写与多行模式
来源：http://hz.jlsjyb.cn/gtbhrzmaau.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.yuanzhike.top/gtemhihqtx.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.guowangkeji.top/gtqrvzutyh.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.quarkkingdee.top/gtnbtxbkxi.html

TS:   /error/gim
来源：http://hz.aibaodan.cn/gtewysbmfu.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.ppjwa.cn/gtccomrnzr.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.jyoumei.cn/gtyfbplmis.html

Ruby: s.scan(/error/i)
来源：http://hz.c1oappe.top/gtoocxdcsd.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.kuanghao11.cn/gtnvpmpwxv.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.quarkkingdee.top/gtokewjmjr.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jiagoushi.top/gtgmbifmrd.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.xylfe.cn/gtxqhbygkq.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.kuanghao11.cn/gtzizkyzqw.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.zycfv.cn/gtlqstnzoz.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.pengpengdd.cyou/gtkkwqkyax.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.dashuyun.cn/gtqimirgpx.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ivvv.top/gtzqhhjwlv.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.meibo888.top/gtkzazzrdh.html

================================================================================
来源：http://hz.xuanzx.com/gtbndfezdt.html

J. 日期与时间
来源：http://hz.ivvv.top/gthcjsnpyg.html

================================================================================
来源：http://hz.jqgfzy.top/gtbpchlzpe.html

[J01] 获取当前时间
来源：http://hz.yonumen.top/gtteslavwf.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.iojbl.cn/gthrspraxt.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.hnqzz.top/gtvltptesj.html

JS:   new Date();  Date.now()
来源：http://hz.xuetiantiany.cn/gtlrywcbvz.html

TS:   new Date();  Date.now()
来源：http://hz.tianlin.xyz/gtdzycgbqy.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.gzhubu.top/gtcjqthgdr.html

Go:   time.Now()
来源：http://hz.yj20258888.top/gtwwzcvxls.html

Ruby: Time.now
来源：http://hz.gzhubu.top/gtlxkrxooh.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.redwolf501.top/gtjhphvfnc.html

[J02] 格式化输出
来源：http://hz.wangdashe.top/gtmhtvkksy.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.feifeiyinyue.top/gtbnsxmaum.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.9152youxi.cn/gtaslsiaia.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.shanyushiyangkeji.top/gtqhwwwdvu.html

TS:   d.toISOString()
来源：http://hz.9152youxi.cn/gtflwduxhk.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.svipenyu.cn/gtoicbwgko.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.ehwqpu.com/gttgsgrfsm.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.fengsongda.top/gtseorceqn.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.zhongyouzk.top/gtnlovqooy.html

[J03] 字符串解析为日期
来源：http://hz.xziqi.cn/gthssainsb.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.xingfuxueyuan.xyz/gtsdumumwd.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.cucudq.cn/gtrcyngzxd.html

JS:   new Date("2024-01-02")
来源：http://hz.xuanzx.com/gtbfcahnqi.html

TS:   new Date("2024-01-02")
来源：http://hz.hfpthk.cn/gteywgrcya.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.aizwys.cn/gtuajqnego.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.fengsongda.top/gtxsmrchrl.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.zhiwuduotai.top/gtntktrdzo.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.yj20258888.top/gtzgcomuno.html

[J04] 时间戳与日期互转
来源：http://hz.gogol.net.cn/gtkebqzzdq.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.hnxiangtu.top/gtqniqmogz.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.sweek.top/gtctbxgvts.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.tianlin.xyz/gtyvosjyen.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.ydzc1.top/gtlqhvuhcw.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.feifeiyinyue.top/gtuizmyrbp.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.jinghuilouyu.cn/gtwjdgxmox.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.chenzaomai.com/gtfhlndfzp.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.gotoacloud.top/gtxqfolpsw.html

[J05] 时间加减（加 7 天）
来源：http://hz.ywan-chungtsiang.top/gtaebewaad.html

Py:   now + timedelta(days=7)
来源：http://hz.guowangkeji.top/gtsijvcxor.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xylfe.cn/gtuafvpche.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.sxryk.cn/gtcueqkcuw.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.guowangkeji.top/gtqcscchro.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.c1oappe.top/gtlnrgkopb.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.ybcxt.top/gtsbvpmnov.html

Ruby: Time.now + 7 * 86400
来源：http://hz.guowangkeji.top/gtymnxcftm.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.zhiwuduotai.top/gtneesktlr.html

[J06] 计算两时间之差
来源：http://hz.jinyuanbaomall.cn/gtmsllxfpr.html

Py:   (end - start).total_seconds()
来源：http://hz.zhoulong.xyz/gtlutkvkhk.html

PHP:  $end->diff($start)->days;
来源：http://hz.shuidangran.top/gtisnjpnsn.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.316326.xyz/gttmnuxjlt.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.hongshengwenyu.top/gtjhlzvtoe.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.aibaodan.cn/gtmsbpllkk.html

Go:   end.Sub(start).Hours()
来源：http://hz.gzhubu.top/gtcpvaqrks.html

Ruby: end - start                 # 返回秒数
来源：http://hz.gogol.net.cn/gtpwyrgrla.html

C#:   (end - start).TotalSeconds
来源：http://hz.shzxlz.cn/gtrpdungpt.html

[J07] 比较两个日期
来源：http://hz.yj202588.top/gtgdhzvvmk.html

Py:   d1 < d2;  d1 == d2
来源：http://hz.snrcjt.cn/gtfebhdnwq.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hz.xingfuxueyuan.xyz/gtpfmcsise.html

JS:   d1.getTime() < d2.getTime()
来源：http://hz.quarkkingdee.top/gtikqtwndi.html


<!-- 参考信息 -->