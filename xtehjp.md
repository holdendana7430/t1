代发 wailian999

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.birdmap.top/gtbouwsxbf.html

Ruby: def self.f; end
来源：http://hz.aizwys.cn/gtwphzwnwe.html

C#:   public static void F() {}
来源：http://hz.yangfankeji.com/gtlhhjusyi.html

[G09] 接口 / 抽象类
来源：http://hz.hammf.cn/gtmzlrprew.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.0kj1m.cn/gtydcgsswg.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.chenzaomai.com/gtaqeaogxu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zdqjudy.top/gtjublphxi.html

TS:   interface Shape { area(): number; }
来源：http://hz.316326.xyz/gtvrndgoae.html

Java: interface Shape { double area(); }
来源：http://hz.chenzaomai.com/gtluwzelfn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yangfankeji.com/gtkqyamcwr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.cucudq.cn/gtfddvwwns.html

C#:   interface IShape { double Area(); }
来源：http://hz.chenjidiqi.icu/gtossepmpy.html

[G10] 访问控制
来源：http://hz.zhaomingkeji.xyz/gtfpvxjnkw.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sweek.top/gtlbtdhpul.html

PHP:  public / protected / private
来源：http://hz.kuanghao11.cn/gtkieehhbl.html

JS:   #private 字段；其余公开
来源：http://hz.jinqigufen.top/gthtbqqpiq.html

TS:   public / protected / private
来源：http://hz.mhx1999.top/gtieexfcej.html

Java: public / protected / private / 默认包级
来源：http://hz.gaohongyu789.top/gtotvdxyds.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.redwolf501.top/gtsrsegoka.html

Ruby: public / protected / private
来源：http://hz.yj202588.top/gtyxgmazem.html

C#:   public / protected / private / internal
来源：http://hz.xylfe.cn/gtpvdvhdvd.html

[G11] getter / setter
来源：http://hz.zhiwuduotai.top/gtnkqkyzzv.html

Py:   @property 与 @x.setter
来源：http://hz.ydjk.org.cn/gtpvpywleo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.quarkkingdee.top/gtjvebfzgb.html

JS:   get name() { return this._name; }
来源：http://hz.quarkkingdee.top/gtqdrgalvk.html

TS:   get name(): string { return this._name; }
来源：http://hz.jinghuilouyu.cn/gtjquxcxlo.html

Java: public String getName() { return name; }
来源：http://hz.birdmap.top/gtdagjlvxp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.guannengcc.top/gteeovkgtk.html

Ruby: attr_accessor :name
来源：http://hz.gzhubu.top/gtmzogtxte.html

C#:   public string Name { get; set; }
来源：http://hz.cheryme.top/gtcugectqt.html

[G12] 对象转字符串
来源：http://hz.hammf.cn/gtzzntjnkm.html

Py:   def __str__(self): return self.name
来源：http://hz.sweek.top/gtqkouwjpa.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenzaomai.com/gtsfmgtpgg.html

JS:   toString() { return this.name; }
来源：http://hz.gaohongyu789.top/gtxzllvyxz.html

TS:   toString(): string { return this.name; }
来源：http://hz.mhx1999.top/gtkaqqoxkp.html

Java: @Override public String toString() { return name; }
来源：http://hz.yonumen.top/gtwuqmnsde.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xylfe.cn/gtbotvnpuq.html

Ruby: def to_s; @name; end
来源：http://hz.kuanghao11.cn/gtrmjedpzq.html

C#:   public override string ToString() => Name;
来源：http://hz.ydjk.org.cn/gtqzmasgxu.html

[G13] 判断对象类型
来源：http://hz.yangfankeji.com/gtxkxfqcgs.html

Py:   isinstance(u, User)
来源：http://hz.havefunace.top/gtixdubifb.html

PHP:  $u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtjlgncfgu.html

JS:   u instanceof User
来源：http://hz.yongpay.top/gtybmqbvnv.html

TS:   u instanceof User
来源：http://hz.quarkkingdee.top/gtzxhmcxke.html

Java: u instanceof User
来源：http://hz.gaohongyu789.top/gtdulmaltk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.jinqigufen.top/gthmmgriuf.html

Ruby: u.is_a?(User)
来源：http://hz.aibaodan.cn/gtjnjsfwgr.html

C#:   u is User
来源：http://hz.yvedp.cn/gtqmslbukk.html

[G14] 数据类 / record
来源：http://hz.gogol.net.cn/gtjvnsazfm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.hysaishi.cn/gtsyzoljrj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.gotoacloud.top/gttyezhbaj.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.dianchejie.cn/gtedxmltvp.html

TS:   type User = { name: string; age: number };
来源：http://hz.jianghu66.top/gtqvnwgfmq.html

Java: record User(String name, int age) {}
来源：http://hz.tianlin.xyz/gtmsdnzgnk.html

Go:   type User struct { Name string; Age int }
来源：http://hz.zhijiandao.cn/gtfrywnnpu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.shangyingyoupin.top/gtndbnhbft.html

C#:   record User(string Name, int Age);
来源：http://hz.sxryk.cn/gtwrwluiwq.html

[G15] 枚举
来源：http://hz.fzhhl.top/gtbipgdlwf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.guowangkeji.top/gtgevzuero.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.yongpay.top/gtcddapuzu.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.hnqzz.top/gtrbdaebis.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhengqikj.top/gthddxrkhe.html

Java: enum Color { RED, GREEN }
来源：http://hz.redwolf501.top/gtwvcjoyhl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.dashuyun.cn/gtlcptwyhp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.ppjwa.cn/gtwoszrpiy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.0kj1m.cn/gticwxcpbb.html

[G16] 对象转数组 / 字典
来源：http://hz.bjfxy.top/gtllzzymqt.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.zhongyouzk.top/gtuvrbqffr.html

PHP:  get_object_vars($obj);
来源：http://hz.sysykeji.top/gtkztymuyx.html

JS:   Object.entries(obj)
来源：http://hz.zhoulong.xyz/gtgodragbx.html

TS:   Object.entries(obj)
来源：http://hz.cucudq.cn/gtezfsfvlc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.hysaishi.cn/gtfexxvdtj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.pengpengdd.cyou/gtyodpbjka.html

Ruby: obj.instance_variables
来源：http://hz.tian-w.cn/gtshhiiejo.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.jinghuilouyu.cn/gtzowumvcu.html

================================================================================
来源：http://hz.tian-w.cn/gtjywgoybt.html

H. 异常与错误处理
来源：http://hz.aizwys.cn/gtvsshwzax.html

================================================================================
来源：http://hz.snrcjt.cn/gtbdtthzii.html

[H01] try / catch 基础
来源：http://hz.yueranfly.top/gtbpxfwlui.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.tanke756.top/gtostrpads.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.hfpthk.cn/gtqebiwfkc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.jianghu66.top/gtwvlsldip.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hammf.cn/gtneysgfsl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.pycfn.com/gtfokhicra.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://hz.ybcxt.top/gtxjfwizay.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://hz.feifeiyinyue.top/gtzlstvlln.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hz.tanke756.top/gtlktwqfns.html

[H02] finally / ensure 收尾
来源：http://hz.jianghu66.top/gtuvuzskno.html

Py:   try: f()⏎finally: cleanup()
来源：http://hz.zhengqikj.top/gtqdfizklo.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://hz.ppjwa.cn/gtlkcazhxu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://hz.shzxlz.cn/gtxetyznhs.html

TS:   try { f(); } finally { cleanup(); }
来源：http://hz.pengpengdd.cyou/gtwweezmqu.html

Java: try { f(); } finally { cleanup(); }
来源：http://hz.haohaochexian.top/gtxfuqfwnm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://hz.dashuyun.cn/gtawaoxbpi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://hz.xinyue.icu/gtbvaegssm.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://hz.pycfn.com/gtqeujfmzb.html

[H03] 主动抛出异常
来源：http://hz.shzxlz.cn/gtglnctmxo.html

Py:   raise ValueError("错误信息")
来源：http://hz.sufxvd.cn/gtpatcgcjw.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hz.fzhhl.top/gtndgxqvxs.html

JS:   throw new Error("错误信息");
来源：http://hz.yj20258888.top/gtdaglbxqr.html

TS:   throw new Error("错误信息");
来源：http://hz.yanxiufei.cn/gtadpigwfn.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://hz.daxiang520.top/gtdvsminfx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://hz.jianghu66.top/gtangztzmu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://hz.yonumen.top/gtzkfsjrkx.html

C#:   throw new ArgumentException("错误信息");
来源：http://hz.shanyushiyangkeji.top/gthrubtfnf.html

[H04] 自定义异常类型
来源：http://hz.cheryme.top/gtxdvpjnsh.html

Py:   class MyError(Exception): pass
来源：http://hz.tian-w.cn/gtjwirudye.html

PHP:  class MyError extends RuntimeException {}
来源：http://hz.hnqzz.top/gtkrqatkst.html

JS:   class MyError extends Error {}
来源：http://hz.tanke756.top/gtoerjzdtq.html

TS:   class MyError extends Error {}
来源：http://hz.yonumen.top/gttdurajmq.html

Java: class MyException extends RuntimeException {}
来源：http://hz.yj20258.top/gtemajzisl.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://hz.gotoacloud.top/gtrvextfqg.html

Ruby: class MyError < StandardError; end
来源：http://hz.yongpay.top/gtmlnsclup.html

C#:   class MyException : Exception {}
来源：http://hz.cdnleiting.top/gtynflcimt.html

[H05] 捕获特定类型
来源：http://hz.yangfankeji.com/gtwvdneyiz.html

Py:   except ValueError as e:
来源：http://hz.meibo888.top/gtrzywnfva.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://hz.yvedp.cn/gtwdidzjjm.html

JS:   if (e instanceof TypeError) {}
来源：http://hz.jinqigfzy.top/gtmleoeube.html

TS:   if (e instanceof TypeError) {}
来源：http://hz.yanxiufei.cn/gtarslbghq.html

Java: catch (IOException | SQLException e) {}
来源：http://hz.hongshengwenyu.top/gtqpwputab.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://hz.shangyingyoupin.top/gthiccxhsk.html

Ruby: rescue ArgumentError => e
来源：http://hz.jinghuilouyu.cn/gthewuzgzc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://hz.yj20258.top/gtbiwnatjr.html

[H06] 可选值 / 空值安全访问
来源：http://hz.gogol.net.cn/gtwxfjirlg.html

Py:   value = d.get("k") or default
来源：http://hz.zycfv.cn/gtmesfpvkk.html

PHP:  $v = $d["k"] ?? null;
来源：http://hz.xziqi.cn/gtrjueehdy.html

JS:   obj?.a?.b;  d ?? default
来源：http://hz.yj20258888.top/gtjdlfeisq.html

TS:   obj?.a?.b;  d ?? default
来源：http://hz.ybcxt.top/gtzizhxurt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://hz.yueranfly.top/gtfrxmzkoi.html

Go:   if v, ok := m["k"]; ok { }
来源：http://hz.sweek.top/gthyfmqmpp.html

Ruby: d&.dig(:a, :b)
来源：http://hz.fengsongda.top/gtfkdgmoka.html

C#:   obj?.A?.B ?? default
来源：http://hz.tianlin.xyz/gtfwxliinn.html

[H07] 断言
来源：http://hz.jianghu66.top/gtcqdvpzep.html

Py:   assert x > 0, "必须为正"
来源：http://hz.fengsongda.top/gtrerwnteo.html

PHP:  assert($x > 0);
来源：http://hz.zhongyouzk.top/gtcdpoupry.html

JS:   console.assert(x > 0);
来源：http://hz.sysykeji.top/gttvsdyazx.html

TS:   console.assert(x > 0);
来源：http://hz.nwbrower.top/gtgffubbcg.html

Java: assert x > 0 : "必须为正";
来源：http://hz.shangyingyoupin.top/gtgctgbues.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://hz.gaohongyu789.top/gtrvahugsd.html

Ruby: raise "必须为正" unless x > 0
来源：http://hz.jinqigufen.top/gtcuisunpw.html

C#:   Debug.Assert(x > 0);
来源：http://hz.ehwqpu.com/gtjxvcrwru.html

[H08] 获取错误信息与堆栈
来源：http://hz.gaohongyu789.top/gtogrsovcu.html

Py:   str(e);  traceback.format_exc()
来源：http://hz.cucudq.cn/gtaoplhpsw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://hz.zycfv.cn/gtvoxeuuvf.html

JS:   e.message;  e.stack
来源：http://hz.bjfxy.top/gtchawpayo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://hz.316326.xyz/gtjpankzce.html

Java: e.getMessage();  e.printStackTrace()
来源：http://hz.dashuyun.cn/gtdxzsgmgb.html

Go:   err.Error()
来源：http://hz.jqgufenzy.top/gtlwxtlreg.html

Ruby: e.message;  e.backtrace
来源：http://hz.zhengqikj.top/gtktlvyiha.html

C#:   e.Message;  e.StackTrace
来源：http://hz.xuetiantiany.cn/gtplkjkjfz.html

[H09] 带错误码的异常
来源：http://hz.ydjk.org.cn/gtjnsaoisu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://hz.daria6918.cn/gttrgqsbbc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://hz.c1oappe.top/gtgttezmem.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hz.tianlin.xyz/gtluqyonix.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://hz.cdnleiting.top/gtjtuzcmud.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://hz.kuanghao11.cn/gtzrloxfsq.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://hz.guowangkeji.top/gttyglyzah.html

Ruby: raise MyError.new("fail", 500)
来源：http://hz.chenlongwang.top/gtoeegeqbp.html

C#:   // 自定义异常类中加 Code 属性
来源：http://hz.zdqjudy.top/gtlfejjrvu.html

[H10] 资源自动释放
来源：http://hz.ydzc1.top/gtghalfvts.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://hz.zhaomingkeji.xyz/gtdiylxsgy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://hz.mhx1999.top/gtwlmhcnjs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.dianchejie.cn/gtonglkmay.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://hz.zhixingplan.top/gtdbwlmvbt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://hz.xylfe.cn/gtjellrdsu.html

Go:   defer f.Close()
来源：http://hz.gzhubu.top/gtcbqdnjzw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://hz.0kj1m.cn/gtdmmhfzdx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://hz.shuidangran.top/gtyeidngxx.html

================================================================================
来源：http://hz.gzhubu.top/gttkagrynl.html

I. 正则表达式
来源：http://hz.xziqi.cn/gtxnhpvipl.html

================================================================================
来源：http://hz.zhongyouzk.top/gtlunhxhtk.html

[I01] 判断是否匹配
来源：http://hz.ppjwa.cn/gtwountsnp.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://hz.xuanzx.com/gtuumusggv.html

PHP:  preg_match('/\d+/', $s);
来源：http://hz.yj20258.top/gtibyfmpwj.html

JS:   /\d+/.test(s)
来源：http://hz.ydzc1.top/gtjkqitdly.html

TS:   /\d+/.test(s)
来源：http://hz.wangshuangyany.cn/gtetlycfll.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://hz.havefunace.top/gtcjlrlvau.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://hz.sysykeji.top/gtnjqbxzva.html

Ruby: s.match?(/\d+/)
来源：http://hz.guowangkeji.top/gthazxkdij.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://hz.sxryk.cn/gtjtvmplsm.html

[I02] 提取所有匹配
来源：http://hz.chenjidiqi.icu/gtwvmcrvuk.html

Py:   re.findall(r"\d+", s)
来源：http://hz.dianchejie.cn/gtgkjnthzt.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://hz.ppjwa.cn/gtrcqxxxby.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://hz.316326.xyz/gtofoiybbi.html

TS:   s.match(/\d+/g)
来源：http://hz.kuanghao11.cn/gtngfsgvvn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://hz.ppjwa.cn/gtywhmpioq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hz.xuanzx.com/gtxmtjrgwv.html

Ruby: s.scan(/\d+/)
来源：http://hz.yuxming.cn/gtqwzshqev.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://hz.nanxinkj.top/gtilwdaicy.html

[I03] 提取捕获分组
来源：http://hz.shanyushiyangtech.top/gtuyzulgcn.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://hz.chenlongwang.top/gthsqpsjxx.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://hz.c1oappe.top/gtotmfznqk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://hz.redwolf501.top/gtwbuutotd.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://hz.zhixingplan.top/gtrkghtxwr.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://hz.iojbl.cn/gtaexxplwj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://hz.ivvv.top/gtfhsywmnp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://hz.jinghuilouyu.cn/gtvcysjlud.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://hz.redwolf501.top/gtqvewoqfp.html

[I04] 正则替换
来源：http://hz.haohaochexian.top/gtvuwfdymk.html

Py:   re.sub(r"\d+", "#", s)
来源：http://hz.hfpthk.cn/gtpujckuud.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://hz.quarkkingdee.top/gtyuqxpyvr.html

JS:   s.replace(/\d+/g, "#")
来源：http://hz.gaohongyu789.top/gtyephumps.html

TS:   s.replace(/\d+/g, "#")
来源：http://hz.zhixingplan.top/gtcqbstors.html

Java: s.replaceAll("\\d+", "#")
来源：http://hz.havefunace.top/gtqulqrjwk.html

Go:   re.ReplaceAllString(s, "#")
来源：http://hz.nanxinkj.top/gtpbfcezje.html

Ruby: s.gsub(/\d+/, "#")
来源：http://hz.cdnleiting.top/gtgfmisxol.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://hz.yuanzhike.top/gteqyjnhmq.html

[I05] 按正则拆分
来源：http://hz.snrcjt.cn/gthltjwemm.html

Py:   re.split(r"\s*,\s*", s)
来源：http://hz.jianghu66.top/gtocdowqhc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://hz.gaohongyu789.top/gtwpkmhdyl.html

JS:   s.split(/\s*,\s*/)
来源：http://hz.jinqigfzy.top/gtivhknzmc.html

TS:   s.split(/\s*,\s*/)
来源：http://hz.wangdashe.top/gtkasknecs.html

Java: s.split("\\s*,\\s*")
来源：http://hz.yuxming.cn/gtcvhxzttk.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://hz.ydjk.org.cn/gtdttakqqk.html

Ruby: s.split(/\s*,\s*/)
来源：http://hz.snrcjt.cn/gtcgwyznzt.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://hz.zhiwuduotai.top/gtwskmwcoi.html

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://hz.hnqzz.top/gtqyulufyn.html

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://hz.daxiang520.top/gtxaaioepi.html

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://hz.guannengcc.top/gtigperucp.html

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.sxryk.cn/gterftlmws.html

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://hz.zhaomingkeji.xyz/gtdgevxnat.html

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://hz.havefunace.top/gtpjdimpia.html

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://hz.birdmap.top/gtxtauzeih.html

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://hz.zhaomingkeji.xyz/gtditaisax.html

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hz.cheryme.top/gtmnmxxzxc.html

[I07] 忽略大小写与多行模式
来源：http://hz.nwbrower.top/gtbpthzqnq.html

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://hz.zhixingplan.top/gtvyvtfixq.html

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://hz.daria6918.cn/gtxrmruajv.html

JS:   /error/gim；new RegExp("error", "gim")
来源：http://hz.andypj.xyz/gtdpiwyukw.html

TS:   /error/gim
来源：http://hz.havefunace.top/gtkyefmwwb.html

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://hz.dianchejie.cn/gtqrhxllzw.html

Go:   regexp.MustCompile(`(?im)error`)
来源：http://hz.zhoulong.xyz/gtvpbuydhp.html

Ruby: s.scan(/error/i)
来源：http://hz.zhoulong.xyz/gtzbmczlwv.html

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://hz.hammf.cn/gtkjdvfmtk.html

[I08] 贪婪与非贪婪匹配
来源：http://hz.wangdashe.top/gtpxulrqoe.html

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hz.jinyuanbaomall.cn/gtczvixiab.html

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://hz.yueranfly.top/gtnidvhdll.html

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.wangdashe.top/gtnxporswj.html

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://hz.ppjwa.cn/gtdusbbkvi.html

Java: Pattern.compile("<b>.*?</b>")
来源：http://hz.yongpay.top/gtmeewyhyu.html

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hz.cheryme.top/gtovhehccc.html

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://hz.ybcxt.top/gttdwbgtwi.html

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://hz.dianchejie.cn/gtgxvsfzke.html

================================================================================
来源：http://hz.0kj1m.cn/gtlfmorkqs.html

J. 日期与时间
来源：http://hz.shuidangran.top/gtqsutiqpg.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtpitfvtel.html

[J01] 获取当前时间
来源：http://hz.shanyushiyangkeji.top/gtivatlagn.html

Py:   datetime.now();  datetime.now(UTC)
来源：http://hz.yj202588.top/gtfljryslg.html

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://hz.ppjwa.cn/gtzzczydve.html

JS:   new Date();  Date.now()
来源：http://hz.cdnleiting.top/gtzizmmfpu.html

TS:   new Date();  Date.now()
来源：http://hz.tianlin.xyz/gtxkaubleh.html

Java: LocalDateTime.now();  Instant.now()
来源：http://hz.andypj.xyz/gtjehgdzhd.html

Go:   time.Now()
来源：http://hz.zhijiandao.cn/gtllygnvmd.html

Ruby: Time.now
来源：http://hz.snrcjt.cn/gtpjnummya.html

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://hz.chenlongwang.top/gtpnpabsgw.html

[J02] 格式化输出
来源：http://hz.gotoacloud.top/gtohlbtvxw.html

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.cqqwz.cn/gtkinbjtav.html

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://hz.9152youxi.cn/gtjaqtnmam.html

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://hz.xziqi.cn/gtacsizpju.html

TS:   d.toISOString()
来源：http://hz.hnqzz.top/gtogmdiahr.html

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://hz.gzhubu.top/gtkkoikhkj.html

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://hz.0kj1m.cn/gtuwpzbqeg.html

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://hz.sufxvd.cn/gtdshyogov.html

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hz.gaohongyu789.top/gtpqetutss.html

[J03] 字符串解析为日期
来源：http://hz.guowangkeji.top/gtrrotpzao.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hz.haohaochexian.top/gtwkakhovb.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://hz.yuanzhike.top/gtamqdvmse.html

JS:   new Date("2024-01-02")
来源：http://hz.ybcxt.top/gtzwqlacri.html

TS:   new Date("2024-01-02")
来源：http://hz.fengsongda.top/gtqxuvivls.html

Java: LocalDate.parse("2024-01-02")
来源：http://hz.nwbrower.top/gtrpvurjtj.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hz.52xcode.cn/gtifunvugi.html

Ruby: Date.parse("2024-01-02")
来源：http://hz.daxiang520.top/gtpfjkqtya.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://hz.jinqigufen.top/gtzwcnamll.html

[J04] 时间戳与日期互转
来源：http://hz.jianghu66.top/gtbpwkhuaz.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://hz.shzxlz.cn/gtfguatbnf.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hz.hnqzz.top/gtvhckxxtn.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://hz.jqgfzy.top/gtxlqxekrs.html

TS:   Math.floor(Date.now() / 1000)
来源：http://hz.cashguo.top/gtxnlvmfqb.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://hz.shangyingyoupin.top/gtxykhgogt.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://hz.chenzaomai.com/gtvzchtepw.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hz.cdnleiting.top/gtdyhelceo.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://hz.hammf.cn/gtgitrwwnx.html

[J05] 时间加减（加 7 天）
来源：http://hz.meibo888.top/gttdlkjegr.html

Py:   now + timedelta(days=7)
来源：http://hz.gzhubu.top/gtrltaitiv.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://hz.xinyue.icu/gtrpziiyal.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.guannengcc.top/gtcgmrhpkk.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hz.havefunace.top/gtjucwysvn.html

Java: LocalDate.now().plusDays(7)
来源：http://hz.ydjk.org.cn/gtptkclees.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://hz.cucudq.cn/gtwzftywpi.html

Ruby: Time.now + 7 * 86400
来源：http://hz.wangshuangyany.cn/gtdfrbizkd.html

C#:   DateTime.Now.AddDays(7)
来源：http://hz.wangdashe.top/gtqkdeampv.html

[J06] 计算两时间之差
来源：http://hz.nanxinkj.top/gtyiwysvky.html

Py:   (end - start).total_seconds()
来源：http://hz.c1oappe.top/gtlpysqrsj.html

PHP:  $end->diff($start)->days;
来源：http://hz.chenlongwang.top/gtdmxdqngs.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://hz.xingfuxueyuan.xyz/gtlgnntrxr.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://hz.tanke756.top/gthzahdpof.html

Java: Duration.between(start, end).toSeconds()
来源：http://hz.xingfuxueyuan.xyz/gtxfrbbyfh.html

Go:   end.Sub(start).Hours()
来源：http://hz.hywenlv.cn/gtiqtnssvs.html

Ruby: end - start                 # 返回秒数
来源：http://hz.hysaishi.cn/gtwenrsxhm.html

C#:   (end - start).TotalSeconds
来源：http://hz.cucudq.cn/gtquvjzbdk.html


<!-- 参考信息 -->